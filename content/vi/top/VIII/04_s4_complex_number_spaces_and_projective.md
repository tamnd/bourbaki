---
book: top
book_title: General Topology
chapter: VIII
chapter_title: Complex numbers
section: 4
section_title: Complex number spaces and projective spaces
lang: vi
source: top-v-x
pdf_pages: 0124-0128, 0133-0136
extraction: ocr
subsections:
    - "no": 1
      title: THE VECTOR SPACE $\mathbf{C}^n$
      page: 0
      pdf_page: 124
    - "no": 2
      title: TOPOLOGY OF VECTOR SPACES AND ALGEBRAS OVER THE FIELD $\mathbf{C}$
      page: 0
      pdf_page: 125
    - "no": 3
      title: COMPLEX PROJECTIVE SPACES
      page: 0
      pdf_page: 125
    - "no": 4
      title: SPACES OF COMPLEX PROJECTIVE LINEAR VARIETIES
      page: 0
      pdf_page: 127
statements: 3
exercises: 8
content_sha256: aaa47bb096e212186ce67b58e048f7d8dcc8cbfcedbfbabfa4863c21f9ca35ed
translated_from: content/en/top/VIII/04_s4_complex_number_spaces_and_projective.md
source_content_sha256: 5ec593cebbee52dc556dcb0f772698b7cf66722f409a4e9d29745d7be45ccbab
translation_model: gpt-5-6-mini, gpt-5-6
translation_run: translate-vi-837ccc39
glossary_version: 34
glossary_terms_sha256: c3c9eb2a6d76aa333a97f0202f1591cfb64ecddfd73ed55909baa4d99a82af0e
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 4. KHÔNG GIAN SỐ PHỨC VÀ KHÔNG GIAN XẠ ẢNH

### 1. KHÔNG GIAN VECTƠ $\mathbf{C}^n$

Vì không gian tôpô $\mathbf{C}$ có thể được đồng nhất với $\mathbf{R}^2$, tích tôpô $\mathbf{C}^n$ của $n$ không gian đồng nhất với $\mathbf{C}$ có thể được đồng nhất với $\mathbf{R}^{2n}$ như một không gian tôpô; tương tự, cấu trúc nhóm tôpô của $\mathbf{C}^n$, là tích của các cấu trúc nhóm cộng (tôpô) của $n$ thừa số, có thể được đồng nhất với cấu trúc của nhóm cộng $\mathbf{R}^{2n}$. Nhưng vì $\mathbf{C}$ là một trường, ta có thể định nghĩa trên $\mathbf{C}^n$ cấu trúc của một không gian vectơ $n$ chiều trên $\mathbf{C}$, tích $az$ của một số phức $a$ và một điểm $z = (z_i)$ của $\mathbf{C}^n$ là điểm $(az_i)$; cần phân biệt cẩn thận cấu trúc không gian vectơ này với cấu trúc của một không gian vectơ $2n$ chiều trên $\mathbf{R}$, được định nghĩa trên $\mathbf{R}^{2n}$ (Chương VI, § 1, no. 3). Ta sẽ dành ký hiệu $\mathbf{C}^n$ cho không gian tôpô là tích của $n$ không gian đồng nhất với $\mathbf{C}$, được trang bị thêm cấu trúc không gian vectơ trên $\mathbf{C}$ vừa được định nghĩa; $\mathbf{C}^n$ được gọi là không gian số phức $n$ chiều. Chú ý rằng ánh xạ $(t, z) \to tz$ là liên tục trên $\mathbf{C} \times \mathbf{C}^n$.

Một ánh xạ tuyến tính afin của $\mathbf{C}^n$ vào $\mathbf{C}^m$ cũng là một ánh xạ tuyến tính afin của $\mathbf{R}^{2n}$ vào $\mathbf{R}^{2m}$, nhưng điều đảo lại là sai.

Ví dụ, ánh xạ $z \to \overline{z}$ là một ánh xạ tuyến tính của không gian vectơ $\mathbf{R}^2$ lên chính nó nhưng không phải là một ánh xạ tuyến tính của không gian vectơ $\mathbf{C}$ lên chính nó.

Mọi ánh xạ tuyến tính afin của $\mathbf{C}^n$ vào $\mathbf{C}^m$ do đó đều liên tục đều; đặc biệt, mọi ánh xạ tuyến tính afin của $\mathbf{C}^n$ lên chính nó là một đồng phôi.

Mọi đa tạp tuyến tính afin $p$ chiều ($p \leq n$) trong không gian vectơ $\mathbf{C}^n$ cũng là một đa tạp tuyến tính afin $2p$ chiều trong không gian vectơ $\mathbf{R}^{2n}$; ở đây một lần nữa, điều đảo lại là sai. Để tránh mọi sự nhầm lẫn, các đa tạp tuyến tính (afin) $p$ chiều trong $\mathbf{C}^n$ sẽ được gọi là các đa tạp tuyến tính phức $p$ chiều (các đa tạp tuyến tính của $\mathbf{R}^{2n}$ được gọi là các đa tạp tuyến tính thực khi cần thiết để tránh sự hiểu lầm). Đặc biệt, các đa tạp tuyến tính phức một chiều (resp. hai chiều) được gọi là các đường thẳng phức (resp. các mặt phẳng phức), và các đa tạp tuyến tính phức $n - 1$ chiều được gọi là các siêu phẳng phức.

Thường thuận tiện khi xem không gian số thực $\mathbf{R}^n$ như được nhúng trong không gian số phức $\mathbf{C}^n$, bằng cách đồng nhất $\mathbf{R}^n$ với tập con của $\mathbf{C}^n$ được xác định bởi các hệ thức $J(z_k) = 0$ ($1 \leq k \leq n$). Cấu trúc nhóm tôpô cảm sinh trên tập con này bởi cấu trúc nhóm tôpô của $\mathbf{C}^n$ trùng với cấu trúc của $\mathbf{R}^n$.

Chú ý rằng $\mathbf{R}^n$, được nhúng như vậy trong $\mathbf{C}^n$, không phải là một đa tạp tuyến tính phức trong $\mathbf{C}^n$.

Một hệ gồm $p$ vectơ của $\mathbf{R}^n$ tự do trên $\mathbf{R}$ cũng tự do trên $\mathbf{C}$. Mọi đa tạp tuyến tính thực $V$ có $p$ chiều trong $\mathbf{R}^n$ sinh ra một đa tạp tuyến tính phức $V'$ có $p$ chiều trong $\mathbf{C}^n$ sao cho $V$ là vết của $V'$ trên $\mathbf{R}^n$; nếu $V$ được định nghĩa bởi một hệ gồm $n - p$ phương trình tuyến tính $f_k(x) = a_k$, trong đó các $f_k$ là các dạng tuyến tính trên $\mathbf{R}^n$ (với các hệ số thực, và độc lập tuyến tính trên $\mathbf{R}$) và các $a_k$ là các số thực, thì cùng các phương trình đó định nghĩa $V'$, nhưng bây giờ các tọa độ của $x$ nhận các giá trị phức.

Ngược lại, nếu một đa tạp tuyến tính phức có $p$ chiều có giao không rỗng với $\mathbf{R}^n$, thì giao này là một đa tạp tuyến tính thực, nhưng chiều của nó có thể là $< p$.

### 2. TÔPÔ CỦA CÁC KHÔNG GIAN VECTƠ VÀ CÁC ĐẠI SỐ TRÊN TRƯỜNG $\mathbf{C}$

Tất cả các định nghĩa và tất cả các kết quả của các số 5 và 6 của Chương VI, § 1, liên quan đến các tôpô trên các không gian vectơ và các đại số trên trường $\mathbf{R}$, và đặc biệt là các không gian và các đại số của các ma trận có các phần tử trong $\mathbf{R}$, vẫn đúng không cần thay đổi nào khi ta thay $\mathbf{R}$ bởi $\mathbf{C}$ trong toàn bộ.

### 3. CÁC KHÔNG GIAN XẠ ẢNH PHỨC

Với ký hiệu được nhắc lại trong Chương VI, § 3, no. 1, ta đưa ra định nghĩa sau đây, tương tự như định nghĩa về các không gian xạ ảnh thực:

#### Định nghĩa 1 {#top-viii-s4-def-1 .statement}

*Không gian xạ ảnh* $\mathbf{P}_n(\mathbf{C})$, *được trang bị tôpô là thương của tôpô của* $\mathbf{C}_{n+1}^*$ *bởi quan hệ tương đương* $\Delta_n(\mathbf{C})$, *được gọi là không gian xạ ảnh phức có* $n$ *chiều.*

Không gian xạ ảnh $\mathbf{P}_1(\mathbf{C})$ được gọi là *đường xạ ảnh phức*, và $\mathbf{P}_2(\mathbf{C})$ được gọi là *mặt phẳng xạ ảnh phức*.

Phần lớn các lập luận liên quan đến các không gian xạ ảnh thực mở rộng, với những thay đổi rất nhỏ, sang các không gian xạ ảnh phức.

Trước hết ta thấy rằng không gian tôpô $P_n(\mathbf{C})$ là *Hausdorff* theo lập luận của Mệnh đề 1 của Chương VI, § 3. no. 1, lập luận này áp dụng từng chữ chỉ bằng cách thay $\mathbf{R}$ bởi $\mathbf{C}$. Một lần nữa, chứng minh của Mệnh đề 2 của Chương VI, § 3. no. 1 chỉ ra rằng $P_n(\mathbf{C})$ là *compact và liên thông*, và đồng phôi với thương của mặt cầu $S_{2n-1}$ (được xem như nhúng trong không gian $C_{n-1}^*$, đồng nhất với $R_{2n-2}^*$) bởi quan hệ tương đương cảm sinh trên mặt cầu này bởi $\Delta_n(\mathbf{C})$; điểm khác biệt duy nhất là bây giờ, nếu $n \geqslant 0$, các lớp tương đương đối với quan hệ này đồng phôi với đường tròn $S_1$.

Vì lý do này, Mệnh đề 3 của Chương VI. § 3, no. 1 không có tương tự cho các không gian xạ ảnh phức.

Tiếp theo chứng minh, như trong Chương VI, § 3, no. 2, rằng mọi đa tạp tuyến tính xạ ảnh $p$-chiều trong không gian $P_n(\mathbf{C})$ là một tập hợp đóng, đồng phôi với $P_r \mathbf{C}$, và rằng phần bù của nó là trù mật trong $P_n(\mathbf{C})$ nếu $p < n$. Chứng minh của Mệnh đề 5 của Chương VI, § 3, no. 2 có thể được chuyển nguyên trạng, đơn giản bằng cách thay $\mathbf{C}$ cho $\mathbf{R}$, và cho thấy rằng (nếu $n \geqslant 0$) phần bù của một siêu phẳng xạ ảnh trong $P_n(\mathbf{C})$ là đồng phôi với $\mathbf{C}^*$, và do đó mọi điểm đều có một lân cận đồng phôi với $\mathbf{C}^*$. Kết quả này cho phép ta *nhúng* không gian số phức $\mathbf{C}^n$ vào không gian xạ ảnh phức $P_n(\mathbf{C})$, bằng cách đồng nhất $\mathbf{C}^*$ với phần bù của một siêu phẳng xạ ảnh, được gọi là "siêu phẳng ở vô tận" (thông thường là siêu phẳng có phương trình là $x_0 = 0$). Trong trường hợp riêng $n = 1$, siêu phẳng ở vô tận là một *điểm*, và định lý Alexandroff cho thấy rằng $P_1 \mathbf{C}$ là đồng phôi với không gian $\tilde{\mathbf{C}}$ thu được bằng cách compact hóa không gian phức địa phương compact $\mathbf{C}$ bằng cách thêm một "điểm ở vô tận", ký hiệu bởi $\infty$. Mệnh đề 4 của Chương VI. § 2, no. 4 khi đó cho thấy rằng *đường thẳng xạ ảnh phức* $P_1(\mathbf{C})$ *là đồng phôi với mặt cầu* $S_2$.

Ta để lại cho người đọc nhiệm vụ phát biểu các kết quả tương tự với các kết quả của Chương VI. § 3. no. 4, đối với các hàm nhận giá trị trong $\mathbf{C}$.

Xét không gian $\mathbf{R}^{n+1}$ như được *nhúng* trong $\mathbf{C}^{n+1}$ (no. 1). Gọi $f$ là ánh xạ chính tắc của $C_{n-1}^*$ lên không gian thương của nó $P_n(\mathbf{C})$. Không gian con $f(\mathbf{R}_{n-1}^*)$ gồm các điểm của $P_n(\mathbf{C})$ có ít nhất một hệ tọa độ thuần nhất *thực*; ta hãy chứng minh rằng $f(\mathbf{R}_{n-1}^*)$ là đồng phôi với không gian xạ ảnh thực $P_n(\mathbf{R})$, điều này cho phép ta xem không gian $P_n(\mathbf{R})$ như được *nhúng* trong $P_n(\mathbf{C})$. Bây giờ quan hệ cảm sinh bởi $\Delta_n(\mathbf{C})$ trên $\mathbf{R}_{n+1}^*$ là $\Delta_n(\mathbf{R})$; ánh xạ chính tắc $\varphi$ của

$$
\mathbf{R}_{n+1}^*/\Delta_n(\mathbf{R}) = P_n(\mathbf{R})
$$

lên $f(\mathbf{R}_{n-1}^*)$ là *liên tục* (Chương I, § 3, no. 6, Mệnh đề 10); vì

$P_n(\mathbf{R})$ là compact, $\varphi$ phải là một đồng phôi (Chương I, § 9, no. 4, Định lý 2, Hệ quả 2).

Ta cũng có thể chứng minh rằng $\varphi$ là song liên tục mà không dùng tính compact của $P_n(\mathbf{R})$, bằng cách viện dẫn tiêu chuẩn của Mệnh đề 10 của Chương I, § 3, no. 6 (xem Bài tập 3).

Vì mọi không gian con vectơ có $p + 1$ chiều của $\mathbf{R}^{n+1}$ sinh ra một không gian con vectơ phức có $p + 1$ chiều trong $\mathbf{C}^{n+1}$, ta thấy rằng mọi đa tạp tuyến tính xạ ảnh $V$ có $p$ chiều trong $P_n(\mathbf{R})$ ($V$ được gọi là một đa tạp tuyến tính xạ ảnh *thực*) sinh ra một đa tạp tuyến tính xạ ảnh $V'$ có $p$ chiều trong $P_n(\mathbf{C})$ ($V'$ được gọi là một đa tạp tuyến tính xạ ảnh *phức*), sao cho $V$ là vết của $V'$ trên $P_n(\mathbf{R})$. Hơn nữa, mọi hệ phương trình (thuần nhất) của $V$ cũng là một hệ phương trình (thuần nhất) của $V'$ khi ta cho phép các biến nhận các giá trị phức.

### 4. CÁC KHÔNG GIAN CỦA CÁC ĐA TẠP TUYẾN TÍNH XẠ ẢNH PHỨC

Với ký hiệu đã nhắc lại trong Chương VI, § 3, no. 5, ta định nghĩa tương tự các không gian của các đa tạp tuyến tính xạ ảnh trong một không gian xạ ảnh phức:

#### Định nghĩa 2 {#top-viii-s4-def-2 .statement}

*Không gian thương* $P_{n,p}(\mathbf{C})$ *của không gian tôpô* $L_{n+1,\ p+1}(\mathbf{C})$ *theo quan hệ tương đương* $\Delta_{n,p}(\mathbf{C})$ *được gọi là không gian của các đa tạp tuyến tính xạ ảnh có* $p \geqslant 0$ *chiều trong không gian xạ ảnh* $P_n(\mathbf{C})$.

Theo lập luận của Mệnh đề 6 của Chương VI, § 3, no. 5, trước hết ta thấy rằng $P_{n,p}(\mathbf{C})$ là *Hausdorff*. Tiếp theo ta chứng minh rằng nó là *compact* bằng cách thay thế không gian con $V_{n+1,\ p+1}$ (trong chứng minh của Mệnh đề 7 của Chương VI, § 3, no. 5) bởi không gian con $W_{n+1,\ p+1}$ của $L_{n+1,\ p+1}(\mathbf{C})$ gồm các hệ gồm $p + 1$ vectơ tạo thành một *cơ sở Hermit trực chuẩn* của không gian con vectơ mà chúng sinh ra; nghĩa là, $W_{n+1,\ p+1}$ gồm các ma trận $X = (x_{ij})$ thỏa mãn các điều kiện

$$
\sum_{j=0}^n x_{ij} \overline{x}_{ij} = 1 \quad (1 \leq i \leq p + 1),
$$
$$
\sum_{j=0}^n x_{ij} \overline{x}_{kj} = 0 \quad (i \neq k).
$$

Chứng minh của Mệnh đề 8 của Chương VI, § 3, no. 5 được mở rộng không thay đổi cho không gian $P_{n,p}(\mathbf{C})$ và chỉ ra rằng không gian này là *liên thông* và *liên thông địa phương* và mỗi điểm của nó có một lân cận đồng phôi với $\mathbf{C}^{p+1,(n-p)}$. Cuối cùng chứng minh của Mệnh đề 9 của Chương VI, § 3, no. 6 áp dụng không thay đổi, và do đó đa tạp Grassmann $G_{n,p}(\mathbf{C})$ đồng phôi với $\mathbf{P}_{n,p}(\mathbf{C})$.

#### Nhận xét {#top-viii-s4-n4-rem-1 .statement}

Phần lớn các tính chất chung của các không gian số thực và phức (tương ứng các không gian xạ ảnh) cũng đúng đối với các không gian số (tương ứng các không gian xạ ảnh) được định nghĩa theo cùng một cách trên vành chia của các quaternion $\mathbf{H}$; thực vậy, chúng có khả năng mở rộng đến nhiều trường tôpô và vành chia khác (xem các Bài tập 2 và 6).

### Bài tập {#top-viii-s4-exercises}

Xem [các bài tập cho § 4](exercises/s4/).
