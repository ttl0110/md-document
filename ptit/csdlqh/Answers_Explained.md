# DBI202 Paper Answers Explained

Tài liệu này tổng hợp lời giải cho các câu `Q1` đến `Q10`, kèm theo giải thích chi tiết và dễ hiểu. Nội dung được trình bày dựa trên các file SQL đã tạo trong thư mục `sqlserver/RollNo_Name_DBI202_PaperNo`.

## Question 1

### Yêu cầu

Tạo các bảng được mô tả trong ERD ở Hình 1.1, gồm bảng, khóa chính và khóa ngoại. Đề bài yêu cầu chỉ nộp các lệnh tạo bảng, không cần viết lệnh tạo database hoặc chuyển database context.

### Lời giải SQL

```sql
CREATE TABLE Students (
    StudentID int PRIMARY KEY,
    [Name] nvarchar(50),
    Address nvarchar(200),
    Gender char(1)
);

CREATE TABLE Teachers (
    TeacherID int PRIMARY KEY,
    [Name] nvarchar(50),
    Address nvarchar(200),
    Gender char(1)
);

CREATE TABLE Classes (
    ClassID int PRIMARY KEY,
    GroupID char(6),
    courseID char(6),
    NoCredits int,
    Semester char(10),
    [year] int
);

CREATE TABLE Teach (
    TeacherID int,
    ClassID int,
    PRIMARY KEY (TeacherID, ClassID),
    FOREIGN KEY (TeacherID) REFERENCES Teachers(TeacherID),
    FOREIGN KEY (ClassID) REFERENCES Classes(ClassID)
);

CREATE TABLE Attend (
    StudentID int,
    ClassID int,
    [Date] date,
    Slot int,
    Attend bit,
    PRIMARY KEY (StudentID, ClassID, [Date], Slot),
    FOREIGN KEY (StudentID) REFERENCES Students(StudentID),
    FOREIGN KEY (ClassID) REFERENCES Classes(ClassID)
);
```

### Giải thích chi tiết

- `Students` là bảng lưu thông tin sinh viên. Thuộc tính `StudentID` được đặt là `PRIMARY KEY` vì mỗi sinh viên phải có mã duy nhất.
- `Teachers` là bảng lưu thông tin giảng viên. Tương tự, `TeacherID` là khóa chính.
- `Classes` là bảng lưu thông tin lớp học. `ClassID` là khóa chính, còn `GroupID`, `courseID`, `NoCredits`, `Semester`, `year` là các thuộc tính mô tả lớp.
- Quan hệ `Teach` thể hiện giảng viên dạy lớp nào. Đây là bảng liên kết giữa `Teachers` và `Classes`, nên khóa chính được tạo theo dạng khóa ghép `(TeacherID, ClassID)`.
- Quan hệ `Attend` thể hiện việc điểm danh của sinh viên trong từng lớp, vào từng ngày và từng slot. Vì một sinh viên có thể học nhiều lớp, và trong một lớp có nhiều lần điểm danh, nên khóa chính cần gồm `StudentID`, `ClassID`, `Date`, `Slot` để phân biệt từng bản ghi điểm danh.
- `FOREIGN KEY` trong `Teach` và `Attend` được dùng để đảm bảo tính toàn vẹn tham chiếu, nghĩa là không thể gán một `TeacherID`, `StudentID` hay `ClassID` không tồn tại trong bảng cha.

### Ý nghĩa thiết kế

- Đây là cách chuyển ERD thành mô hình quan hệ trong SQL Server.
- Một bảng thực thể thành một `CREATE TABLE`.
- Một quan hệ nhiều-nhiều thường trở thành bảng trung gian.
- Thuộc tính gạch chân trong ERD chính là khóa chính trong bảng.

## Question 2

### Yêu cầu

Hiển thị tất cả khách hàng có `Segment = 'Consumer'` và sống tại thành phố `Arlington`.

### Lời giải SQL

```sql
USE [master];
GO
USE [PE_Demo_S2019];
GO

SELECT *
FROM dbo.Customer
WHERE Segment = 'Consumer'
  AND City = 'Arlington';
```

### Giải thích chi tiết

- `USE [master]` rồi `USE [PE_Demo_S2019]` giúp đảm bảo script đang chạy đúng vào database chứa dữ liệu đề bài.
- `SELECT *` có nghĩa là lấy tất cả các cột của bảng `Customer`.
- `FROM dbo.Customer` chỉ rõ bảng cần truy vấn. Thêm `dbo.` là để tránh lỗi do schema mặc định khác nhau giữa các môi trường.
- Điều kiện `Segment = 'Consumer'` lọc ra những khách hàng thuộc nhóm Consumer.
- Điều kiện `City = 'Arlington'` lọc tiếp những người sống ở Arlington.
- Toán tử `AND` có nghĩa là bản ghi chỉ được chọn khi đồng thời thỏa mãn cả hai điều kiện.

### Tại sao truy vấn này đúng

- Đề bài yêu cầu lọc theo 2 tiêu chí, và truy vấn đã lọc đúng 2 tiêu chí đó.
- Không cần `JOIN` vì toàn bộ thông tin nằm trong bảng `Customer`.

## Question 3

### Yêu cầu

Hiển thị các khách hàng có `CustomerName` bắt đầu bằng chữ `B` và đã đặt hàng trong tháng 12 năm 2017. Sắp xếp giảm dần theo `Segment`, sau đó tăng dần theo `CustomerName`.

### Lời giải SQL

```sql
USE [master];
GO
USE [PE_Demo_S2019];
GO

SELECT c.*
FROM dbo.Customer c
JOIN dbo.Orders o ON o.CustomerID = c.ID
WHERE c.CustomerName LIKE 'B%'
  AND YEAR(o.OrderDate) = 2017
  AND MONTH(o.OrderDate) = 12
ORDER BY c.Segment DESC, c.CustomerName ASC;
```

### Giải thích chi tiết

- Ở câu này không thể chỉ truy vấn bảng `Customer`, vì thông tin về ngày đặt hàng nằm trong bảng `Orders`.
- `JOIN dbo.Orders o ON o.CustomerID = c.ID` nối bảng `Customer` với bảng `Orders` thông qua khóa liên kết giữa khách hàng và đơn hàng.
- `c.CustomerName LIKE 'B%'` có nghĩa là tên khách hàng bắt đầu bằng ký tự `B`.
- `YEAR(o.OrderDate) = 2017` lọc các đơn hàng trong năm 2017.
- `MONTH(o.OrderDate) = 12` lọc tiếp các đơn hàng trong tháng 12.
- `ORDER BY c.Segment DESC, c.CustomerName ASC` sắp xếp kết quả theo đúng thứ tự đề bài yêu cầu.

### Lưu ý quan trọng

- Một khách hàng có thể có nhiều đơn hàng trong tháng 12/2017. Khi đó truy vấn có thể trả về nhiều dòng cho cùng một khách hàng nếu khách hàng đó có nhiều order thỏa điều kiện.
- Cách viết này phù hợp với kết quả minh họa của đề, vì đề đang tập trung vào việc lọc theo khách hàng có đặt hàng, không bắt buộc loại bỏ bản ghi trùng lặp bằng `DISTINCT`.

## Question 4

### Yêu cầu

Hiển thị `SubCategoryID`, `SubCategoryName` và số lượng sản phẩm trong mỗi subcategory, chỉ lấy những subcategory có hơn 100 sản phẩm, sắp xếp giảm dần theo số lượng sản phẩm.

### Lời giải SQL

```sql
USE [master];
GO
USE [PE_Demo_S2019];
GO

SELECT sc.ID AS SubCategoryID,
       sc.SubCategoryName,
       COUNT(p.ID) AS NumberOfProducts
FROM dbo.SubCategory sc
JOIN dbo.Product p ON p.SubCategoryID = sc.ID
GROUP BY sc.ID, sc.SubCategoryName
HAVING COUNT(p.ID) > 100
ORDER BY NumberOfProducts DESC;
```

### Giải thích chi tiết

- `SubCategory` chứa thông tin nhóm con sản phẩm, còn `Product` chứa từng sản phẩm cụ thể.
- Muốn đếm xem mỗi subcategory có bao nhiêu sản phẩm, ta phải `JOIN` hai bảng này qua điều kiện `p.SubCategoryID = sc.ID`.
- `COUNT(p.ID)` đếm số sản phẩm trong từng nhóm con.
- Vì dùng hàm tổng hợp `COUNT`, ta phải `GROUP BY sc.ID, sc.SubCategoryName` để gom dữ liệu theo từng subcategory.
- `HAVING COUNT(p.ID) > 100` dùng để lọc trên kết quả sau khi đã nhóm. Đây là điểm khác biệt quan trọng giữa `WHERE` và `HAVING`:
  - `WHERE` lọc trước khi nhóm
  - `HAVING` lọc sau khi nhóm
- `ORDER BY NumberOfProducts DESC` để subcategory có nhiều sản phẩm nhất hiện trước.

### Vì sao không dùng WHERE cho COUNT

- Hàm tổng hợp `COUNT` được tính sau bước `GROUP BY`, nên không thể viết `WHERE COUNT(...) > 100`.
- Dùng `HAVING` là cú pháp đúng cho bài này.

## Question 5

### Yêu cầu

Hiển thị `ProductID`, `ProductName`, `Quantity` của tất cả sản phẩm có số lượng lớn nhất trong một order.

### Lời giải SQL

```sql
USE [master];
GO
USE [PE_Demo_S2019];
GO

SELECT p.ID AS ProductID,
       p.ProductName,
       od.Quantity
FROM dbo.Product p
JOIN dbo.OrderDetails od ON od.ProductID = p.ID
WHERE od.Quantity = (
    SELECT MAX(Quantity)
    FROM dbo.OrderDetails
)
ORDER BY p.ID;
```

### Giải thích chi tiết

- Bảng `OrderDetails` chứa thông tin chi tiết sản phẩm trong đơn hàng, trong đó có cột `Quantity`.
- Ta cần tìm giá trị `Quantity` lớn nhất trong toàn bộ bảng `OrderDetails`, nên dùng truy vấn con:

```sql
SELECT MAX(Quantity)
FROM dbo.OrderDetails
```

- Kết quả truy vấn con là một giá trị duy nhất, ví dụ `14`.
- Sau đó truy vấn ngoài lấy tất cả những dòng trong `OrderDetails` có `Quantity` bằng giá trị lớn nhất đó.
- `JOIN dbo.Product` để lấy thêm `ProductName` từ bảng sản phẩm.
- `ORDER BY p.ID` giúp kết quả ổn định, dễ đọc và dễ đối chiếu với đáp án mẫu.

### Ý nghĩa tư duy SQL trong bài này

- Bài này là mẫu kinh điển của kiểu bài “tìm tất cả bản ghi có giá trị bằng lớn nhất”.
- Mẫu giải rất thông dụng là:
  1. Tìm giá trị lớn nhất bằng truy vấn con
  2. Lấy tất cả dòng có giá trị bằng mức lớn nhất đó

## Question 6

### Yêu cầu

Hiển thị `CustomerID`, `CustomerName` và số lượng đơn hàng của những khách hàng có số đơn hàng nhiều nhất.

### Lời giải SQL

```sql
USE [master];
GO
USE [PE_Demo_S2019];
GO

WITH OrderCount AS (
    SELECT c.ID AS CustomerID,
           c.CustomerName,
           COUNT(o.ID) AS Num
