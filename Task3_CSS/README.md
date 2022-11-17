# Report

>
> Tên đề tài: CSS  
> Thời gian task được giao 10/11/2022-18/11/2022  
> Người thực hiện: Lê Đức Ninh  
> Mentor: Nguyễn Quang Đức  

# Nội dung
> [I. Khái quát CSS](#I)  
> [II. Bố cục](#II)  
> [III. Cấu trúc CSS](#III)  
> [IV. Các thuộc tính và giá trị phổ biến CSS](IV)

<a name="I"></a>
# Khái quát CSS  
CSS (Cascading Style Sheets) hiểu đơn giản là ngôn ngữ dùng để định dạng cả phần tử trong một website như bố cục, màu sắc trang, đổi màu chữ, font chữ,...  
Chèn CSS vào HTML  
Có thể chèn CSS vào HTML bằng nhiều cách khác nhau như: chèn trực tiếp vào `<header>` bằng thẻ `<style>` hoặc có thể chèn qua một link liên kết `<link>` hoặc có thể chèn trực tiếp thuộc tính vào các thẻ thành phần.  

<a name="II"></a>  
# Bố cục (Box Model)  
![box model](https://user-images.githubusercontent.com/81867521/202347328-9811ef25-de78-44b7-988e-03b1b727096b.png)
- Padding: phần xung quang nội dung.  
- Border: đường viền bên ngoài phần padding.  
- Margin: khoảng cách ngoài cùng xung quanh box.  
Để tùy chỉnh thì sẽ đề cập ở bên dưới.  
<a name="III"></a>
# Cấu trúc CSS  
Cấu trúc của một đoạn CSS (trong một chương trình sẽ chứa nhiều đoạn như vậy)  
```
vùng chọn{
  thuộc tính: giá trị;
  thuộc tính: giá trị;
  ...
}
```
Vùng chọn ở đây là khu vực, phần tử mà chúng ta muốn định dạng. Các thuộc tính là những gì chúng ta muốn định dạng cho phần được chọn đi kèm với các giá trị.  
## Vùng chọn:  
- Vùng chọn có thể là các thẻ như `<p>`, `<h1>`, `<h2>`,...
- Các thuộc tính của thẻ như là `id`, `class`,..
- Chọn dựa vào sự phân cấp  
Đối với chọn các thẻ thì ta chỉ cần khai báo tên thẻ. Ví dụ:
```
p{
....
}
```
Đối với chọn thuộc tính id thì:
```
#giatri_id{
...
}
```
Đối với chọn thuộc tính là class thì:  
```
.giatri_class{
...
}
```
Đối với chọn thứ cấp thì chúng ta sử dụng operator `>`, tùy biến theo từng trường hợp.  
<a name="IV"></a>  
# Các thuộc tính phổ biến trong CSS:
## Một số thuộc tính trang trí văn bản thông dụng:
- text-align: Căn lề văn bản 	: left, right, center, justify
- text-decoration: Thêm gạch dưới, gạch trên, gạch giữa vào văn bản
- text-indent: Tạo khoảng trống bên tay trái cho văn bản
- text-shadow: Đổ bóng văn bản
- text-transform: Tùy chỉnh hiển thị in Hoa và thường. 

## Thuộc tính trang trí chữ viết:
- font-family: đổi kiểu font chữ
- font-style: kiểu chữ (in nghiêng,...)
- font-weight: Độ đậm nhạt của chữ
- color: thêm màu chữ

## Box Model  
Box Model là kỹ thuật tinh chỉnh lại các phần tử box (block) trong Box Model có 4 thành phần chính:
- Margin: lề bên ngoài của box
- Border: Viền của box
- Padding phần lót bên trong box ngăn cách với nội dung
- Content phần nội dung bên trong box

## Tuy chỉnh kích thước box:  
 - height: thiết lập chiều cao.  
 - max-height: thiết lập chiều cao tối đa  
 - max-width: thiết lập chiều rộng tối đa  
 - width: thiết lập chiều rộng  
 Ngoài ra còn có min-height, min-width
## FLoat va clear float  
Với thuộc tính float có các giá trị như là: left, right, none, inherit. Mình chỉ mới sử dụng left với right. Thuộc tính này sẽ chỉ định các phần tử được đặt ở đâu, bên trái hay bên phải hay vv,...  

## Thuộc tính position  
Các giá trị của thuộc tính position bao gồm:  
- Static: hiển thị mặc định
- relative: ví trí tương đối so với vị trí tĩnh
- Absolute: vị trí sẽ được xác định từ phần tử padding của phần tử cha
- fixed: vị trí sẽ được cố định một chỗ
## Reset CSS  
Reset trong CSS là làm cho các style của đối tượng theo một chuẩn khi mà trình duyệt nó không hỗ trợ một trong các style được định nghĩa. Ở phần này chúng ta nên tham khảo các format reset CSS trên các diễn đàn. Và lưu ý reset CSS luôn được đặt đầu các file CSS.  
