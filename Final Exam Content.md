* **Hình thức:** tự luận
* **Thời gian:** 90 phút
* **Không** sử dụng tài liệu
* Tính toán, lập trình bằng **Python** qua **VS Code**
* **Ghi chú**: trường hợp lớp thi trên phòng thường, sinh viên chủ động mang **máy tính**, **sạc**, **ổ cắm**:
  + Trên máy tính phải **xóa** toàn bộ các tệp liên quan đến môn học
  + Màn hình máy tính chỉ hiển thị duy nhất giao diện **VS Code màu đen**
  + Thanh điều khiển chỉ có duy nhất biểu tượng VS Code (**bỏ ghim** tất cả các ứng dụng không liên quan)
  + Trên thanh thông báo phải có biểu tượng **wifi** đang ở trạng thái **ngắt kết nối**

# Phần lý thuyết (học thuộc, 2-3đ, chọn 1 câu, bỏ câu 3)
<ol>
 <li>
   <ol>
     <li>Định nghĩa tổ hợp lặp</li>
     <li>Liệt kê các tổ hợp lặp chập 4 của 3 loại vật $A, B, C$</li>
     Ký hiệu $a(n, r)$ là số tổ hợp lặp chập $r$ từ $n$ vật
     <li>Chứng minh $a(n, r) = a(n, r-1) + a(n-1, r)$ trong đó $n \ge 1$ và $r \ge 1$</li>
     <li>Xác định $a(n, 0)$ với $n \ge 0$, và $a(0, r)$ với $r > 0$</li>
     <li>Lập bảng tính $a(n, r)$ với $0\le n, r \le 5$</li>
     <li>Áp dụng phương pháp hàm sinh, chứng minh $a(n, r) = \binom{n+r-1}{r}$</li>
   </ol>
 </li>
 
 <li>
   <ol>
     <li>Định nghĩa phân hạng của một số nguyên dương</li>
     <li>Liệt kê các phân hạng của 2, 3, và 4</li>
     <li>Áp dụng phương pháp hàm sinh, đếm số phân hạng của số nguyên dương $n$</li>
   </ol>
 </li>
 
 <li>
   <ol>
     <li>Định nghĩa phân hạng của một số nguyên dương</li>
     <li>Liệt kê các phân hạng đối xứng của 3, 4, và 5</li>
     <li>Áp dụng phương pháp hàm sinh, đếm số phân hạng đối xứng của số nguyên dương $n$</li>
   </ol>
 </li>
 
 <li>
   <ol>
     <li>Liệt kê các cách tính tích $a_0 a_1 a_2\cdots a_n$ bằng cách đặt các dấu ngoặc, với $n = 2, 3$</li>
      Đặt $C_n$ là số cách tính tích $a_0 a_1 a_2\cdots a_n$
     <li>Lập hệ thức đệ quy cho dãy $\{C_n\}$</li>
     <li>Áp dụng phương pháp hàm sinh để giải hệ thức đệ quy trên</li>  
  </ol>
 </li>
</ol>

# Phần bài tập (6-7đ, 2-3 câu)
<ol>
  <li>
    Lập công thức, và xác định hàm sinh (bằng Python) của một dãy $\{a_n\}_{n \ge 0}$, chẳng hạn dãy 1, 4, 9, 16, 25,...
  </li>
 
 <li><b>(Chương 8)</b>
  Đặt $\left( {{a_n}} \right)_{n \ge 0}$ là dãy sinh bởi hàm $f\left( x \right) = \sqrt {1 - 2x} $.
  <ol>
   <li>Tính $a_3$</li>
   <li>Xác định $a_n$</li>
  </ol>
 </li>

<li><b>(Chương 8)</b>
  Lập và xác định hàm sinh mũ của một dãy $\left( {{a_n}} \right)_{n \ge 0}$, chẳng hạn dãy 1, 2, 3,...
 </li>
 
 <li><b>(Chương 8)</b>
  Đặt $\left( {{a_n}} \right)_{n \ge 0}$ là dãy sinh mũ ứng với $f\left( x \right) = \sqrt {1 - 2x} $.
  <ol>
   <li>Tính $a_3$</li>
   <li>Xác định $a_n$</li>
  </ol>
 </li>

 <li><b>(Chương 9)</b>
  Giải hệ thức đệ quy $a_n = 3 a_{n-1} - 2 a_{n-2} + n$ với $a_0 = -1$, $a_1 = 2$
 </li>

 <li><b>(Chương 9)</b>
  Giải hệ thức chia để trị $f\left( n \right) = 2f\left( {\dfrac{n}{3}} \right) + {n^2}$ với $f(1) = 4$
 </li>
 
 <li><b>(Mã hóa Rabin)</b>
  <ol>
   <li>Số hóa tin nhắn bằng mã Cipher / ASCII thành $M$. Với khóa công khai $n$, tìm tin nhắn mã hóa $N$</li>
   <li>Biết tin nhắn mã hóa $N$. Với khóa bí mật $p$ và $q$, giải mã $N$ và cho biết tin nhắn gốc theo mã Cipher / ASCII là gì?</li>
  </ol>
 </li>
 <li><b>(Mã hóa RSA)</b>
   <ol>
     <li>Số hóa tin nhắn bằng mã Cipher / ASCII thành $M$. Với khóa công khai $n$ và $e$, tìm tin nhắn mã hóa $N$</li>
     <li>Cho tin nhắn mã hóa $N$. Với khóa bí mật $\varPhi(n)$, kết hợp với khóa công khai $n$ và $e$, giải mã $N$ và cho biết tin nhắn gốc theo mã Cipher / ASCII là gì?</li>
   </ol>
 </li>
</ol>

