* **Hình thức:** tự luận
* **Thời gian:** 90 phút
* **Không** sử dụng tài liệu
* Tính toán, lập trình bằng **Python** qua **VS Code**
* **Ghi chú**: trường hợp lớp thi trên phòng thường, sinh viên chủ động mang **máy tính**, **sạc**, **ổ cắm**:
  + Trên máy tính phải **xóa** toàn bộ các tệp liên quan đến môn học
  + Màn hình máy tính chỉ hiển thị duy nhất giao diện **VS Code màu đen**
  + Thanh điều khiển chỉ có duy nhất biểu tượng VS Code (**bỏ ghim** tất cả các ứng dụng không liên quan)
  + Trên thanh thông báo phải có biểu tượng **wifi** đang ở trạng thái **ngắt kết nối**

# Phần lý thuyết (học thuộc, 2-3đ, chọn 1 câu)
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
      <li>Liệt kê nghiệm nguyên không âm của phương trình $c_1 + c_2 + c_3 = 4$.</li>
      <li>Áp dụng phương pháp hàm sinh để đếm số nghiệm nguyên không âm của phương trình trên.</li>
      <li>Tổng quát, áp dụng phương pháp hàm sinh để đếm số nghiệm nguyên không âm của phương trình $c_1 + c_2 + \cdots + c_n = r$.</li>
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
    <ol>
      <li>Lập công thức của hàm sinh dãy $\{a_n\}_{n \ge 0}$, chẳng hạn dãy 1, 4, 9, 16, 25,...</li>
      <li><i>(Trả lời nhanh)</i> Tính hàm sinh ở trên</li>
    </ol>
    
  </li>
 
  <li>
    Đặt $\{a_n\}_{n \ge 0}$ là dãy sinh bởi hàm $f\left( x \right) = \sqrt {1 - 2x} $.
    <ol>
      <li><i>(Trả lời nhanh)</i> Tính $a_3$</li>
      <li>Xác định $a_n$</li>
    </ol>
  </li>

  <li>
    <ol>
      <li>Lập công thức của hàm sinh mũ của dãy $\{a_n\}_{n \ge 0}$, chẳng hạn dãy 1, -2, 3, -4, 5,...</li>
      <li><i>(Trả lời nhanh)</i> Tính hàm sinh mũ ở trên</li>
    </ol>
  </li>
 
  <li>
    Đặt $\left( {{a_n}} \right)_{n \ge 0}$ là dãy có hàm sinh mũ $f\left( x \right) = \sqrt {1 - 2x} $.
    <ol>
      <li><i>(Trả lời nhanh)</i> Tính $a_3$</li>
      <li>Xác định $a_n$</li>
    </ol>
  </li>

 <li><i>(Đánh giá độ phức tạp của thuật toán đệ quy)</i>
   Cho thuật toán đệ quy xác định dãy $f_n$, với $n \in \Bbb N$
<pre>
def f(n):
    if n == 0:
        return -1
    if n == 1:
        return 2
    x = f(n-1)
    for i in range(6):
        x = x + f(n-2)
    return x
</pre>
   <ol>
     <li><i>(Trả lời nhanh)</i> Xác định $f_2, f_3, f_4$</li>
     <li>Xác định hệ thức đệ quy cho dãy $\{f_n\}$. Từ đó kiểm chứng kết quả ở ý (i)</li>
     Đặt $a_n$ là số phép toán (số học, so sánh, gán) mà thuật toán dùng để tính $f_n$
     <li>Xác định hệ thức đệ quy cho dãy $\{a_n\}$</li>
     <li><i>(Trả lời nhanh)</i> Giải hệ thức đệ quy để xác định $a_n$</li>
   </ol>
 </li>

  <li><i>(Đánh giá độ phức tạp của thuật toán chia để trị)</i>
    Cho thuật toán đệ quy xác định dãy $u_n$, với $n \in \Bbb N$
<pre>
def u(n):
    if n == 0:
        return -1
    x = 2
    for i in range(3):
        x = x + u(n // 2)
    for i in range(n):
        x = x + 1
    return x
</pre>
  <ol>
   <li><i>(Trả lời nhanh)</i> Xác định $u_1, u_2, u_3, u_4$</li>
     <li>Xác định hệ thức đệ quy cho dãy $\{u_n\}$. Từ đó kiểm chứng kết quả ở ý (i)</li>
     Đặt $f(n)$ là số phép toán (số học, so sánh, gán) mà thuật toán dùng để tính $u_n$
     <li>Xác định hệ thức chia để trị cho $f(n)$</li>
     <li><i>(Trả lời nhanh)</i> Giải hệ thức chia để trị để xác định $f(n)$</li>
   </ol>
  </li>

  <li>
    Giải hệ phương trình đồng dư<br>
    $x \equiv 1 \pmod 2,\quad x \equiv -3 \pmod 5,\quad x \equiv 4 \pmod 7$
  </li>
 
  <li><b>(Mã hóa Rabin)</b>
    <ol>
      <li>Số hóa tin nhắn bằng mã thứ tự chữ cái / ASCII thành $M$. Với khóa công khai $n$, tìm tin nhắn mã hóa $N$</li>
      <li>Biết tin nhắn mã hóa $N$. Với khóa bí mật $p$ và $q$, giải mã $N$ và cho biết tin nhắn gốc theo mã thứ tự chữ cái / ASCII là gì?</li>
    </ol>
  </li>
 
  <li><b>(Mã hóa RSA)</b>
    <ol>
      <li>Số hóa tin nhắn bằng mã Cipher / ASCII thành $M$. Với khóa công khai $n$ và $e$, tìm tin nhắn mã hóa $N$</li>
      <li>Cho tin nhắn mã hóa $N$. Với khóa bí mật $\varPhi(n)$, kết hợp với khóa công khai $n$ và $e$, giải mã $N$ và cho biết tin nhắn gốc theo mã Cipher / ASCII là gì?</li>
    </ol>
  </li>
</ol>


# Chú ý
  * Phần lý thuyết bỏ câu 4
  * Phần bài tập bỏ các ý liên quan đến phương pháp mã hóa và giải mã Rabin
