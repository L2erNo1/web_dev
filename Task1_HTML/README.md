# Report

>
> Tên đề tài: Tìm hiểu về HTML cơ bản  
> Thời gian task được giao 10/11/2022-17/11/2022  
> Người thực hiện: Lê Đức Ninh  
> Mentor: Nguyễn Quang Đức  
### Mục lục: 
[I. Giới thiệu về HTML](#HTML)
- Nội dung:
  - 1.
<a name = "HTML"></a>
# HTML là gì?
- HTML (Hyper Text Markup Language) là ngôn ngữ đánh dấu siêu văn bản dùng để tạo giao diện web, mỗi trang web là một file html hoặc có thể là một tập tin HTML.  
- File HTML được cấu tạo bởi các tag (thẻ), các thẻ có cấu tạo `<tagname>` và thường sẽ đi theo cặp bao gồm thẻ mở và thẻ đóng, ví dụ `<p></p>`. Đôi khi một số tag đặc biệt sẽ không có thẻ đóng ví dụ như `<br>`  
- File HTML có dạng filename.html hoặc filename.htm
# Vai trò của HTML trong website.
HTML là ngôn ngữ đánh dấu siêu văn bản nên nó có vai trò xây dựng cấu trúc văn bản trên một website, bao gồm văn bản, hình ảnh, video, âm nhạc,...
# Các thẻ và thuộc tính phổ biến trong HTML.
Để khai báo loại tài liệu HTML chúng ta cần khai báo `<!DOCTYPE html>` - HTML5  
Chúng ta sẽ tham khảo một chương trình HTML bao gồm những thành phần nào.
```
<!DOCTYPE html>
<html>
<head>
        <title>My blog</title>
	<meta charset="utf-8">
	<meta name="description" content="This is my blog">
	<meta name="author" content="DucNinh">
</head>
<body>
	<p>Welcome to my Blog</p>
</body>
</html>
```
Đầu tiên chúng ta có thể thấy bắt đầu với chương trình sẽ là dòng khai báo file HTML (ngoài ra còn cho biết bạn đang dùng phiên bản html bao nhiêu). Tiếp theo là thẻ mở `<html>` và kết thúc bằng thẻ đóng `<html>` có ý nghĩa bao hàm cả nội dung file html - cấu trúc file html. Bên trong thẻ `<html>` được chia ra làm 2 phần đó là head và body. Ở phần head sẽ bắt đầu với thẻ mở `<head>` và thẻ đóng `</head>`, ở phần này chứa những thẻ khai báo thông tin cho trang như tiêu đề, mô tả, bảng mã ký tự. Và phần `head` không hiển thị nội dung bên trong nó lên trang web. Tiếp theo là thẻ `body` cũng tương tự như thế thẻ body cũng bắt đầu với một thẻ mở `<body>` và kết thúc bằng thẻ đóng `</body>`. Ở phần này sẽ chứa toàn bộ nội dung sẽ hiển thị lên website.
## Các thẻ phổ biến trong phần `<head>`
Đầu tiên phải kể đến đó là thẻ `<title>My blog</title>` sẽ khai báo tiêu đề/ nhan đề bài viết.<br>
Tiếp theo là thẻ `<meta>` đi kèm với các thuộc tính dùng để định nghĩa các thông tin cơ bản như mô tả trang web, từ khóa, tác giả, chỉnh sửa cuối cùng và các metadata khác.  
Ví dụ: 
- Định nghĩa tác giả của trang web  
`<meta name="author" content="DucNinh">`
- Định nghĩa mô tả cho trang web  
`<meta name="description" content="This is my blog">`
- Định nghĩa bảng mã cho trang web  
`<meta charset="utf-8">`
## Các thẻ phổ biến trong phần `<body>`
### Định dạng đoạn văn bản
![markdown](https://suntech.edu.vn/storage/wink/images/7Kpd4riIaCUoin6L25xIt4WYZ4yEKcXsDUrz1J8a.jpg)
- Đầu tiên sẽ là các thẻ `heading` của văn bản từ `<h1>-<h6>`. Ở thẻ này giúp chúng ta tạo tiêu đề, đề mục tài liệu trong cấu trúc trang web HTML. Trong một trang HTML có thể phân chia ra thành nhiều đề mục với các cấp độ khác nhau từ 1 đến 6. Cấp độ cao nhất là `<h1>` và thấp nhất là `<h6>`.  
- 




