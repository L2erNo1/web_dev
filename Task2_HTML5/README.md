Tên đề tài: HTML5
Thời gian task được giao 10/11/2022-18/11/2022
Người thực hiện: Lê Đức Ninh
Mentor: Nguyễn Quang Đức

Ở task trước chúng ta đã tìm hiểu qua kiến thức cơ bản về HTML, ở task này mình sẽ giới thiệu về HTML5, một cải tiến của HTML.  
Vậy đầu tiên chúng ta cần biết HTML5 là gì?  
HTML5 có thể hiểu đơn là nó là một phiên bản mới (thứ 5) của HTML, được cập nhật cải tiến hơn giúp cho người trực tiếp sử dụng HTML dễ dàng hơn và những người sử dụng sản phẩm của HTML có trải nghiệm tốt nhất.  
Ở đây mình sẽ đề cập với những đặc điểm khác nhau giữa HTML & HTML5, và tập trung vào những cái mới được nhà phát triển thêm vào để tối ưu hóa khi sử dụng.  

Mình sẽ giới thiệu qua một số điểm khác nhau giữa HTML & HTML5 và kèm theo ví dụ:  
- Việc tích hợp các chức năng <audio>, <video>,.. (media)  
  Đối với các phiên bản HTML trước đây để thêm các media vào thì cần phải có phần mềm hỗ trợ flash player. Đến tận bây giờ mình còn bắt gặp một số website vẫn giữ cái này nhưng đều không xem được vì đã bị ngưng hỗ trợ.  
Ví dụ:  
  Để chèn một video trong trình duyệt chúng ta có thể sử dụng thẻ `<video>...</video>` kết hợp với các thuộc tính src, controls, autoplay, các thuộc tính thay đổi kích thước như là height, width,..
  `<video src="/video.mp4" autoplay controls></video>` tương tự như thế để chèn một tập tin âm thanh thì sử dụng thẻ `<audio>...</audio>`...  
- Bổ sung thêm các thẻ cho các phần tử thông dụng  
  Để giúp những lập trình viên đơn giản hóa việc khai báo các thành phần trong một trang web, HTML5 đã cung cấp các thẻ mới như là  `<header>, <footer>, <article>, <section>,...` Ví dụ trước đây developer define một header sẽ sử dụng một thẻ `div` và dùng thêm thuộc tính `class` với giá trị  `header` thì bây giờ có thể đơn giản hóa nó bằng cách chỉ sử dụng một thẻ `<header>` để khai báo.  
  Ví dụ: 
  ```
  <header>
    <h1> Hallo </h1>
  </header>
  ```
  Chỉ vậy thôi, tương tự đối với các thẻ khác được nêu ở trên. Thẻ `<footer>` sẽ tạo footer cho trang web, section sẽ gộp lại hoặc chứa các nhiều thông tin khác nhau,  article để bao bọc các nội dung có thể là một bài post chẳng hạn,..
- Hỗ trợ đồ họa `<canvas>..</canvas>`  
  Việc HTML5 cho phép sử dụng `canvas` nhằm mục đích tạo các đối tượng đồ họa, và để nó hoạt động thì phải đi kèm với javascript. Canvas dựa trên mô hình 2d tọa độ Oxy, có thể tạo tùy ý ví dụ như vẽ hình, vẽ chữ, các ký tự,...nhưng lưu ý luôn luôn đi kèm js.
- Ngoài ra HTML5 còn bổ sung thêm các thuộc tính mới cho thẻ `form`  
  - `<datalist>` dùng để xác định danh sách tùy chọn được xác định trước cho các thẻ `<input>`  
  - `<keygen>` định nghĩa một bộ tạo cặp cho `<form>`  
  - `<output>` định nghĩa kết quả của một phép toán  
  Ví dụ: 
  ```
  <input type="text" id="options" list="vaccine">
  <datalist id="vaccine">
    <option value="AstraZeneca">
    <option value="Pfizer">
  </datalist>
  ```
  Một ví dụ cơ bản ở trên sẽ yêu cầu người dùng chọn loại vaccine đã tiêm với danh sách cung cấp sẵn có 2 loại. Tuy nhiên nếu không tồn tại trong 2 trường hợp này thì người dùng hoàn toàn có thể nhập vào dữ liệu khác.
  
  
  
  
  
  
  
