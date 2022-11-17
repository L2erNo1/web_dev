# Report

>
> Tên đề tài: HTML5  
> Thời gian task được giao 10/11/2022-18/11/2022  
> Người thực hiện: Lê Đức Ninh  
> Mentor: Nguyễn Quang Đức  

# Nội dung
>[I. Khái quát HTML5](#I)  
>[II. So sánh HTML vs HTML5](#II)  
>  [1. Các thẻ hỗ trợ media](#1)  
>  [2. Các thẻ cho các phần tử trong trang web](#2)  
>  [3. Các thẻ hỗ trợ đồ họa](#3)  
>  [4. Các thuộc tính hỗ trợ cho thẻ form](#4)  

<a name="I"></a>
# Khái quát HTML5
Ở task trước chúng ta đã tìm hiểu qua kiến thức cơ bản về HTML, ở task này mình sẽ giới thiệu về HTML5, một cải tiến của HTML.  
Vậy đầu tiên chúng ta cần biết HTML5 là gì?  
HTML5 có thể hiểu đơn là nó là một phiên bản mới (thứ 5) của HTML, được cập nhật cải tiến hơn giúp cho người trực tiếp sử dụng HTML dễ dàng hơn và những người sử dụng sản phẩm của HTML có trải nghiệm tốt nhất.  
Ở đây mình sẽ đề cập với những đặc điểm khác nhau giữa HTML & HTML5, và tập trung vào những cái mới được nhà phát triển thêm vào để tối ưu hóa khi sử dụng.  

<a name="II"></a>
# So sánh HTML vs HTML5
Mình sẽ giới thiệu qua một số điểm khác nhau giữa HTML & HTML5 và kèm theo ví dụ:  
<a name="1"></a>
## Các thẻ hỗ trợ media  
- Việc tích hợp các chức năng `<audio>`, `<video>`,.. (media)  
  Đối với các phiên bản HTML trước đây để thêm các media vào thì cần phải có phần mềm hỗ trợ flash player. Đến tận bây giờ mình còn bắt gặp một số website vẫn giữ cái này nhưng đều không xem được vì đã bị ngưng hỗ trợ.  
Ví dụ:  
  Để chèn một video trong trình duyệt chúng ta có thể sử dụng thẻ `<video>...</video>` kết hợp với các thuộc tính  `src`, `controls`, `autoplay`, các thuộc tính thay đổi kích thước như là `height`, `width`,..
  `<video src="/video.mp4" autoplay controls></video>` tương tự như thế để chèn một tập tin âm thanh thì sử dụng thẻ `<audio>...</audio>`...  
<a name="2"></a>
## Các thẻ cho các phần tử trong trang web
- Bổ sung thêm các thẻ cho các phần tử thông dụng  
  Để giúp những lập trình viên đơn giản hóa việc khai báo các thành phần trong một trang web, HTML5 đã cung cấp các thẻ mới như là  `<header>`, `<footer>`, `<article>`, `<section>`,... Ví dụ trước đây developer define một header sẽ sử dụng một thẻ `div` và dùng thêm thuộc tính `class` với giá trị  `header` thì bây giờ có thể đơn giản hóa nó bằng cách chỉ sử dụng một thẻ `<header>` để khai báo.  
  Ví dụ: 
  ```
  <header>
    <h1> Hallo </h1>
  </header>
  ```
  Chỉ vậy thôi, tương tự đối với các thẻ khác được nêu ở trên. Thẻ `<footer>` sẽ tạo `footer` cho trang web, `<section>` sẽ gộp lại hoặc chứa các nhiều thông tin khác nhau,  `<article>` để bao bọc các nội dung có thể là một bài post chẳng hạn,..  
<a name="3"></a>
## Các thẻ hỗ trợ đồ họa  
- Hỗ trợ đồ họa `<canvas>..</canvas>`  
  Việc HTML5 cho phép sử dụng `canvas` nhằm mục đích tạo các đối tượng đồ họa, và để nó hoạt động thì phải đi kèm với javascript. Canvas dựa trên mô hình 2d tọa độ Oxy, có thể tạo tùy ý ví dụ như vẽ hình, vẽ chữ, các ký tự,...nhưng lưu ý luôn luôn đi kèm js.  
  Ví dụ: Vẽ hình chữ nhật bằng canvas:
  ```
  <canvas id="hinhchunhat" width="300" height="200" style="background: whitesmoke;"></canvas>

  <script>
    var c=document.getElementById("hinhchunhat");
    //Lấy context
    var ctx=c.getContext("2d");
    ctx.fillRect(20,20,100,50);
  </script>
  ```
  Đầu tiên sẽ get context sau đó sẽ xác định tọa độ và chiều rộng chiều cao của hình. Ví dụ như trên (x, y, w, h) tọa độ điểm bắt đầu vẽ sẽ là (20, 20) và chiều rộng và chiều cao của hình chữ nhật tương ứng với (100, 50).
  Để hỗ trợ đồ họa thì HTML5 còn cung cấp thêm một thẻ nữa đó là `<svg>`. Đối với thẻ `svg` chúng ta có thể chèn ảnh, vẽ ảnh,.. mà không nhất thiết phải đi cùng với javascript như thẻ `<canva>`
  Ví dụ:
  ```
  <svg width="340" height="120">
    <rect width="300" height="100"  x="20" y="20" fill="green" />
  </svg>
  ```
  Ở ví dụ trên chúng ta có thể vẽ hình chữ nhật bằng thẻ `<rect/>`, tương tự như thế để vẽ hình tròn sử dụng `<circle>`, đường thẳng dùng `<line/>`,...  
<a name="4"></a>
## Các thuộc tính bổ sung cho thẻ form  
- Ngoài ra HTML5 còn bổ sung thêm các thuộc tính mới cho thẻ `form`  
  - `<datalist>` dùng để xác định danh sách tùy chọn được xác định trước cho các thẻ `<input>`   
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
  Đối với thẻ output dùng để trả về kết quả một phép toán. Ví dụ đơn giản chúng ta có một phép toán cộng như sau:
  ```
  <form action="">
    <input name="num01" type="number" /> + <input name="num02" type="number" /> = <output name="result" onforminput="value=num01.valueAsNumber + num02.valueAsNumber"></output>
  </form>
  ```
  
  Ví dụ trên sẽ có 2 input đầu vào là num01 và num02 và kết quả trả trực tiếp trong thẻ output.  
  Ngoài ra còn rất nhiều cải tiến ở HTML5 như storage, cache,... tuy nhiên mình chưa trực tiếp sử dụng đến nên sẽ không nhắc ở phần này.  
  
  ## Kết luận
  Vậy làm thế nào để HTML5 có thể tiếp cận người dùng dễ dàng như vậy, những ưu điểm sau đây sẽ chứng mình được điều đó:  
    - Bổ sung các tính năng tuyệt vời (một trong số đó được trình bày ở trên)  
    - HTML5 giúp đồng bộ hóa giữa các trình duyệt (đa số các trình duyệt đều hỗ trợ)  
    - Giúp cho việc khai báo các thẻ trở nên đơn giản hơn  
    - Làm cho website có hiệu suất tốt hơn
  
  
  
  
  
  
