# Report

>
> Tên đề tài: Tìm hiểu về HTML cơ bản  
> Thời gian task được giao 10/11/2022-17/11/2022  
> Người thực hiện: Lê Đức Ninh  
> Mentor: Nguyễn Quang Đức  
# Nội dung: 
[I. HTML là gì?](#I)  
[II. Vai trò của HTML](#II)  
[III. Các thẻ và thuộc tính phổ biến trong HTML](#IIII)  
  [1. Cấu trúc chung](#1)
  [2. Các thẻ trong `<head>`](#2)
  [3. Các thẻ trong `<body>`](#3)
    [3.1. Định dạng đoạn văn bản](#3.1.)
    [3.2. Chèn media](#3.2.)
    [3.3. Tạo form nhập liệu](#3.3.)
<a name = "I"></a>
# HTML là gì?
- HTML (Hyper Text Markup Language) là ngôn ngữ đánh dấu siêu văn bản dùng để tạo giao diện web, mỗi trang web là một file html hoặc có thể là một tập tin HTML.  
- File HTML được cấu tạo bởi các tag (thẻ), các thẻ có cấu tạo `<tagname>` và thường sẽ đi theo cặp bao gồm thẻ mở và thẻ đóng, ví dụ `<p></p>`. Đôi khi một số tag đặc biệt sẽ không có thẻ đóng ví dụ như `<br>`  
- File HTML có dạng filename.html hoặc filename.htm

<a name = "II"></a>
# Vai trò của HTML trong website.
HTML là ngôn ngữ đánh dấu siêu văn bản nên nó có vai trò xây dựng cấu trúc văn bản trên một website, bao gồm văn bản, hình ảnh, video, âm nhạc,...

<a name = "III"></a>
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
![7Kpd4riIaCUoin6L25xIt4WYZ4yEKcXsDUrz1J8a](https://user-images.githubusercontent.com/81867521/201452984-b7d2130d-7e0b-44fb-919b-6d978f447a0c.jpg)

- Đầu tiên sẽ là các thẻ `heading` của văn bản từ `<h1>-<h6>`. Ở thẻ này giúp chúng ta tạo tiêu đề, đề mục tài liệu trong cấu trúc trang web HTML. Trong một trang HTML có thể phân chia ra thành nhiều đề mục với các cấp độ khác nhau từ 1 đến 6. Cấp độ cao nhất là `<h1>` và thấp nhất là `<h6>`.  
- Tiếp theo là thẻ `<p>...</p>` đùng để khai báo đoạn văn bản. Thẻ `<p>` chứa các thuộc tính (các thuộc tính luôn luôn đi kèm với thẻ mở) như align, style, id, title,... Tương tự chúng ta cũng có thẻ `<pre>` tuy nhiên ở thẻ này thì đoạn văn bản sẽ giữ nguyên định dạng ở trình soạn thảo hiển thị lên website.
- Một số thẻ thường xuyên được sử dụng khác như là:
  - `<br>` - Thẻ ngắt dòng văn bản
  - `<hr>` - Thẻ chèn đường nằm ngang
  - `<b>` - Thẻ bôi đậm chữ
  - `<strong>` - Thẻ nhấn mạnh văn bản
  - `<i>` - Thẻ in nghiêng
  - `<u>` - Thẻ gạch chân
- Để sắp xếp cho văn bản mạch lạc hơn thì HTML cung cấp một số thẻ để tạo danh sách trong văn bản HTML. Để tạo danh sách trong HTML thì chúng ta có 2 loại đó là tạo danh sách có sắp xếp và tạo danh sách không có sắp xếp.Đối với tạo danh sách có sắp xếp sẽ có dạng như sau:
```
<ol type="I">	
	<li>Hallo</li>
	<li>Brother</li>
</ol>
```
Thẻ được sử dụng là `<ol>...</ol>` đi kèm với thuộc tính `type` để chỉ định ký tự của danh mục, Ở đây mình sử dụng `I` có nghĩa là danh sách sẽ bắt đầu với các ký tự I, II, III, IV,... Tương tự chúng ta có thể thay đổi bằng các ký tự khác như số `1`, chữ cái `a`,...  
Đối với tạo danh sách không sắp xếp:
```
<ul>
	<li>Mục con 1</li>
	<ul>
		<li>hallo</li>
	</ul>
	<li>Mục con 2</li>
	<li>Mục con 3</li>
</ul>
```
Đối với kiểu danh sách này sẽ sử dụng thẻ `<ul>...</ul>` để tạo. Và đặt điểm chung của cả 2 loại đó chính là bên trong phải chứ các phần tử cho danh sách. Cách phần tử được khai báo bởi thẻ `<li>...</li>` hoặc có thể lồng các danh sách vào bên trong danh sách như trên.
- Tạo một liên kết điều hướng trong HTML chúng ta sử dụng thẻ `<a>`, đây cũng được xem là thẻ được sử dụng phổ biến nhất khi tạo một website. Cấu trúc của thẻ `<a>` như sau:
```
<a href="myblog.html" title="noi-dung" target="_self">My blog</a>
```
Có thể thấy thẻ `<a>` đi kèm với các thuộc tính `href`, `title`, `target`,.. ngoài ra còn nhiều thuộc tính khác. Thuộc tính `href` sẽ tạo liên kết muốn chuyển đến, nếu không muốn trỏ đến liên kết nào cả thì chúng ta sử dụng `href="#"`. Thuộc tính `title` sẽ khai báo tiêu đề cho thẻ a. Thuộc tính target sẽ chỉ định mở liên kết trong một trang mới `(_blank)` hoặc chuyển hướng từ trang hiện tại `(_self)`.
### Chèn media: hình ảnh, video, nhạc,... trong HTML
Để trang web thêm hấp dẫn thì HTML cung cấp các thẻ để chèn media vào trang web.
- Chèn hình ảnh vào trang web:
```
<img src="console.png" alt="Hinh anh Console" title="WS" width="500px" height="300px">
```
Để chèn một hình ảnh vào HTML chúng ta sử dụng thẻ `<img>` với các thuộc tính như `src`(quan trọng), `alt`, `title`, `width`, `height`. Thuộc tính `src` sẽ chỉ định nguồn của hình ảnh được load, có thể sử dụng một liên kết bên ngoài internet hoặc cũng có thể sử dụng tài nguyên trên web của mình. Các thuộc tính điều chỉnh kích thường cho hình ảnh về chiều rộng và chiều cao `width` và `height`. Thuộc tính `title` khai báo tiêu đề cho hình ảnh. Thuộc tính `alt` có nhiệm vụ thay thế bằng cụm từ giá trị của thuộc tính này khi hình ảnh gặp sự cố không thể hiển thị.
- Chèn video vào trang web:
```
<video width="320px" height="auto" controls>
	<source src="hack.mp4" type="video/mp4">
	Trình duyệt của bạn không hỗ trợ html5
</video>
```
Cấu trúc trên sẽ hướng dẫn ta chèn một video vào trang web bằng html5. Thẻ dùng để chèn video là `<video>...</video>` với các thuộc tính tinh chỉnh kích thước như `width`, `height`, ngoài ra nếu muốn video chứa các nút điều khiển thì chúng ta sử dụng thuộc tính `controls` và còn rất nhiều thuộc tính khác nữa. Bên trong thẻ `<video>` sẽ chứa một thẻ con - thẻ này rất quan trọng trong việc chèn một video - đó chính là thẻ `<source>`. Thẻ này sẽ chỉ định video nào được chèn vào trang web với thuộc tính `src` có thể là video trên máy chúng ta hoặc là video bất kỳ trên youtube (sử dụng nhúng), thuộc tính tiếp theo là `type` để chỉ loại video.
- Chèn audio vào trang web:
```
<audio>
	<source src="http://www.w3schools.com/tags/horse.mp3" type="audio/mp3">
</audio>
```
Tương tự như chèn video, chèn audio sẽ sử dụng thẻ `<audio>...</audio>` thay vì `<video>`, và mọi thuộc tính đều tương tự như `video`, chúng ta cũng có thể chèn một bản nhạc trên zingmp3 bằng cách chèn mã nhúng.
- Chèn một website khác vào trang web:
```
<iframe src="https://www.instagram.com/" width="500px" height="600px" scrolling="auto" name="cua-so-1"></iframe>
```
Để chèn một website vào trang web ta sử dụng thẻ `<iframe>...</iframe>` với các thuộc tính `src`, `width`, `height`, `scrolling` - Có thể cuộn nếu trang web kích thước lớn, `name`,...
### Tạo form nhập liệu trong HTML
Một trong những tính năng khác được xem là sử dụng nhiều trong HTML đó chính là tạo form nhập liệu cho trang web. Ở đây mình sẽ ví dụ cơ bản một loại cụ thể đó chính là tạo form đăng nhập:
```
<form action="trangchu.html" method="post" name="login">
	Username: <input type="text" name="username"> <br>
	Password: <input type="password" name="password"><br>
	<input type="submit" value="Login" name="submit">
</form>
```
Để bắt đầu tạo một form đăng nhập, chúng ta sử dụng thẻ `<form>...</form>` với các thuộc tính:
  - `action`: Thực hiện một action nào đó khi nhấn Submit (có thể là một JS), ở đây mình sẽ cho nó đơn giản là chuyển hướng sang một site khác.
  - `method`: chỉ phương thức được sử dụng, có rất nhiều phương thức khác nhau như POST, GET, TRACE,... mỗi phương thức sẽ có cách truy vấn khác nhau.
  - `name`: khái bảo tên cho form, sử dụng khi thao tác với các ngôn ngữ khác.

Tiếp theo bên trong thẻ `<form>` sẽ chứa các phần tử của thẻ `form` này. Mỗi phần sẽ được khai báo với thẻ `<input>` với các thuộc tính `type`, `name`, `value`,... Với `type` tùy thuộc vào nhu cầu sử dụng của người dùng, như ví dụ trên để nhập vào username thì sử dụng `text`, password sử dụng `password` và nút Submit sử dụng `submit` với giá trị bên trong nút là `Login`.
