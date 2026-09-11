---
book: top
book_title: General Topology
chapter: VI
chapter_title: Real number spaces and projective spaces
section: 3
section_title: Real projective spaces
lang: vi
source: top-v-x
pdf_pages: 0050-0060, 0067-0069
extraction: ocr
subsections:
    - "no": 1
      title: TOPOLOGY OF REAL PROJECTIVE SPACES
      page: 0
      pdf_page: 51
    - "no": 2
      title: PROJECTIVE LINEAR VARIETIES
      page: 0
      pdf_page: 53
    - "no": 3
      title: EMBEDDING REAL NUMBER SPACE IN PROJECTIVE SPACE
      page: 0
      pdf_page: 54
    - "no": 4
      title: APPLICATION TO THE EXTENSION OF REAL-VALUED FUNCTIONS
      page: 0
      pdf_page: 55
    - "no": 5
      title: SPACES OF PROJECTIVE LINEAR VARIETIES
      page: 0
      pdf_page: 56
    - "no": 6
      title: GRASSMANNIANS
      page: 0
      pdf_page: 59
statements: 14
exercises: 10
content_sha256: 25e90f5c97abf509f5001fd04d9e2af7ceb1d5b82622b1657330c25288ce5ae4
translated_from: content/en/top/VI/03_s3_real_projective_spaces.md
source_content_sha256: 53d9a6c6d16fec228a219b9d179e95bab1a2ba49b45ee6d650a09b758196d514
translation_model: gpt-5-6-mini, gpt-5.4-mini, gpt-5-6
translation_run: translate-vi-1fc55e42
glossary_version: 34
glossary_terms_sha256: 285999771845454636bb3c1f3cd46f2fe645ffe6c86299e203039a06a9a84c0c
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 3. CÁC KHÔNG GIAN XẠ ẢNH THỰC

Trong mục này chúng ta sẽ cần thường xuyên viện dẫn các khái niệm và kết quả về *các không gian thương* (Chương I, § 3), và đặc biệt là hai tính chất sau đây, mà để tiện lợi chúng ta phát biểu dưới dạng các bổ đề:

Cho $E$ là một không gian tôpô, $R$ một quan hệ tương đương trên $E$, $A$ một tập con của $E$, $R_A$ là quan hệ tương đương cảm sinh trên $A$ bởi $R$ và cho $f$ là ánh xạ chính tắc của $E$ lên $E/R$. Khi đó:

#### Bổ đề 1 {#top-vi-s3-lem-1 .statement}

*Nếu mọi tập hợp mở (tương ứng đóng) trong $A$ bão hòa đối với $R_A$ là vết trên $A$ của một tập hợp mở (tương ứng đóng) trong $E$ bão hòa đối với $R$, thì không gian thương $A/R_A$ là đồng phôi với không gian con $f(A)$ của $E/R$. Điều này đặc biệt đúng nếu $A$ là mở hoặc đóng trong $E$ và bão hòa đối với $R$.*

Điều này suy ra từ Mệnh đề 10 của Chương I, § 3, no. 6.

#### Bổ đề 2 {#top-vi-s3-lem-2 .statement}

*Nếu có một ánh xạ liên tục* g *của* E *lên* A *sao cho, với mọi* x ∈ E, g(x) *thuộc lớp tương đương của* x, *thì không gian thương* A/R_A *là đồng phôi với* E/R.

Đây là Hệ quả 2 của Mệnh đề 10 của Chương I, § 3, no. 6.

### 1. TÔPÔ CỦA CÁC KHÔNG GIAN XẠ ẢNH THỰC

Chúng ta nhắc lại các định nghĩa sau đây từ đại số: cho một vành chia hoặc một trường K, tập hợp các *đường thẳng* đi qua o (tức là các không gian vectơ con có chiều 1) trong không gian vectơ trái K_s^{n+1} trên K được gọi là *không gian xạ ảnh trái chiều n* trên K, và được ký hiệu là P_n(K).

Nếu ta cho tương ứng với mỗi đường thẳng đi qua o trong K_s^{n+1} cùng đường thẳng ấy *bỏ đi gốc tọa độ*, ta có một song ánh của P_n(K) lên *thương* của K_{n+1}^* (phần bù của {o} trong K_s^{n+1}) bởi quan hệ tương đương sau đây Δ_n(K) giữa các vectơ x và y của K_{n+1}^*: "tồn tại t ∈ K sao cho t ≠ o và y = tx". Trong phần sau chúng ta sẽ *đồng nhất* P_n(K) với tập thương này. Trong lý thuyết các không gian xạ ảnh, ta lấy khoảng [0, n] của N làm tập chỉ số cho các tọa độ của một điểm của K_{n+1}^*. Các tọa độ x_i (0 ≤ i ≤ n) của bất kỳ một điểm nào của K_{n+1}^* mà ảnh chính tắc là x ∈ P_n(K) tạo thành cái được gọi là một *hệ tọa độ thuần nhất* của điểm x.

Với mỗi số nguyên p sao cho −1 ≤ p ≤ n, ảnh chính tắc trong P_n(K) của một không gian vectơ con chiều p + 1 (không chứa gốc tọa độ) của K_s^{n+1} được gọi là một *đa tạp tuyến tính xạ ảnh* chiều p. Một hệ gồm p điểm của P_n(K) được gọi là *tự do* nếu nó gồm các ảnh chính tắc của p điểm của K_{n+1}^* tạo thành một *hệ tự do* trong không gian vectơ K_s^{n+1}. Đa tạp tuyến tính xạ ảnh của P_n(K) được sinh bởi một hệ tự do gồm p + 1 điểm (tức là đa tạp tuyến tính xạ ảnh nhỏ nhất chứa p + 1 điểm này) có chiều p.

Khi K là trường R, các không gian xạ ảnh tương ứng có thể được trang bị tôpô, và đó là những không gian mà chúng ta sẽ nghiên cứu.

#### Định nghĩa 1 {#top-vi-s3-def-1 .statement}

*Không gian xạ ảnh* P_n(R) *được trang bị tôpô thương của tôpô của* R_{n+1}^* *bởi quan hệ tương đương* Δ_n(R) *được gọi là không gian xạ ảnh thực chiều n.*

Không gian xạ ảnh P_1(R) được gọi là *đường xạ ảnh thực*, và P_2(R) được gọi là *mặt phẳng xạ ảnh thực*.

Khi không có nguy cơ nhầm lẫn, chúng ta sẽ viết P_n và Δ_n thay cho P_n(R) và Δ_n(R).

#### Mệnh đề 1 {#top-vi-s3-prop-1 .statement}

Không gian xạ ảnh $P_n$ là Hausdorff.

Ta bắt đầu bằng việc chỉ ra rằng quan hệ $\Delta_n$ là mở (Chương I, § 5, no. 2). Cho $A$ là một tập hợp mở trong $\mathbf{R}_{n+1}^*$; để làm bão hòa $A$ đối với $\Delta_n$ ta phải lấy hợp của các tập hợp $tA$ đồng dạng với $A$, khi $t$ chạy qua tập hợp các số thực $\neq 0$; vì mỗi tập hợp này là mở, nên hợp của chúng cũng là mở.

Theo Mệnh đề 8 của Chương I, § 8, no. 3, mệnh đề sẽ được chứng minh nếu ta chỉ ra rằng tập con $M$ của $\mathbf{R}_{n+1}^* \times \mathbf{R}_{n+1}^*$ được xác định bởi quan hệ $\Delta_n$ là đóng. Khi đó cho $(x, y)$ là một điểm của $\mathbf{R}_{n+1}^* \times \mathbf{R}_{n+1}^*$ nằm trong bao đóng của $M$. Nếu $x = (x_i)$, có một chỉ số $i$ sao cho $x_i \neq 0$; do đó có một lân cận $V$ của $(x, y)$ sao cho với mọi điểm $(x', y') \in M \cap V$ tọa độ thứ i $x'_i$ của $x'$ không là 0. Khi $(x', y')$ tiến tới $(x, y)$ trong khi vẫn thuộc $M$, $y'_i {x'}^{-1}_i$ tiến tới $t = y_i x_i^{-1}$; vì $y' = (y'_i {x'}^{-1}_i) x'$, ta thấy bằng cách chuyển qua giới hạn rằng $y = x$, điều này chỉ ra rằng $(x, y) \in M$.

#### Mệnh đề 2 {#top-vi-s3-prop-2 .statement}

Không gian xạ ảnh $P_n$ là compact và liên thông, và là đồng phôi với thương của mặt cầu $S_n$ bởi quan hệ tương đương cảm sinh trên mặt cầu bởi $\Delta_n$.

Cho $\Delta'_n$ là quan hệ tương đương cảm sinh trên $S_n$ bởi $\Delta_n$ (các lớp tương đương của $\Delta'_n$ là các cặp điểm đối xứng diametrically của $S_n$). Ánh xạ $x \to x/||x||$ của $\mathbf{R}_{n+1}^*$ lên $S_n$ là liên tục, do đó (Bổ đề 2) $P_n$ là đồng phôi với $S_n / \Delta'_n$. Vì $S_n$ là compact và liên thông, mọi không gian thương Hausdorff của $S_n$ cũng compact và liên thông (Chương I, § 9, no. 4, Định lý 2, Hệ quả 1; § 11, no. 3, Mệnh đề 7).

#### Mệnh đề 3 {#top-vi-s3-prop-3 .statement}

Nếu $n \geq 0$, không gian xạ ảnh $P_n$ là đồng phôi với không gian thương của quả cầu $B_n$ thu được bằng cách đồng nhất mỗi điểm của $S_{n-1}$ với điểm đối xứng diametrically của nó.

Gọi $H$ là bán cầu đóng của $S_n$ được xác định bởi $x_0 \leq 0$. $P_n$, vốn đồng phôi với không gian thương của $S_n$ theo quan hệ $\Delta'_n$, cũng đồng phôi với thương của tập con $H$ của $S_n$ theo quan hệ $\Delta''_n$ cảm sinh trên $H$ bởi $\Delta'_n$. Mỗi lớp tương đương của $\Delta'_n$ giao với $H$ tại ít nhất một điểm, và vì thế (Bổ đề 1) chỉ cần kiểm tra rằng nếu ta bão hòa theo $\Delta'_n$ một tập con mở $U$ của $H$ bão hòa theo $V''_n$, ta thu được một tập con mở $V$ của $S_n$. Bây giờ nếu $a = (a_i) \in U$ và nếu $a_0 < 0$, tồn tại một lân cận $W$ của $a$ trong $S_n$ được chứa trong $U$, và hợp của $W$ và $-W$ là một lân cận của $a$ bão hòa theo $\Delta'_n$ và được chứa trong $V$. Mặt khác, nếu $a_0 = 0$, ta có $-a \in U$, và tồn tại $r > 0$ sao cho tập hợp các điểm $x \in H$ thỏa mãn một trong hai quan hệ ||x - a|| < r, ||x + a|| < r được chứa trong U; tập hợp các điểm x \in S_n thỏa mãn một trong hai quan hệ này là lân cận của a bão hòa theo $\Delta'_n$ và được chứa trong V.

Nhận xét rằng không gian thương $H / \Delta''_n$ thu được bằng cách đồng nhất, trong H, mỗi điểm của giao $S_{n-1}$ của H và siêu phẳng $x_0 = 0$ với điểm đối của nó. Để hoàn tất chứng minh chỉ cần nhận xét rằng phép chiếu lập thể với đỉnh $e_0$ ($\S$ 2, no. 4) là một đồng phôi của H lên $B_n$ giữ bất biến các điểm của $S_{n-1}$.

### 2. CÁC ĐA TẠP TUYẾN TÍNH XẠ ẢNH

Mọi ánh xạ tuyến tính đơn ánh $f$ từ $\mathbf{R}^{n+1}$ vào $\mathbf{R}^{m+1}$ ($m \geq n$) xác định, bằng cách hạn chế trên $\mathbf{R}_{n+1}^*$ rồi sau đó đi qua thương theo các quan hệ $\Delta_n$ và $\Delta_m$ (Lý thuyết tập hợp, R, $\S$ 5, no 8), một ánh xạ đơn ánh g của $P_n$ vào $P_m$, được gọi là một *ánh xạ tuyến tính xạ ảnh*. Nếu $\varphi$ (tương ứng $\psi$) là ánh xạ chính tắc của $\mathbf{R}_{n+1}^*$ lên $P_n$ (tương ứng của $\mathbf{R}_{m+1}^*$ lên $P_m$), ta có $g \circ \varphi = \psi \circ f$, điều đó cho thấy rằng g là *liên tục* trên $P_n$ (Chương I, $\S$ 3, no. 4, Hệ quả của Mệnh đề 6). Đặc biệt, mọi *biến đổi tuyến tính xạ ảnh* của $P_n$ (tức là một ánh xạ tuyến tính xạ ảnh của $P_n$ lên chính nó) là một *đồng phôi* của $P_n$ lên chính nó.

Ta cũng nhắc lại rằng, nếu V và V' là hai đa tạp tuyến tính xạ ảnh có p chiều trong $P_n$, thì tồn tại một biến đổi tuyến tính xạ ảnh của $P_n$ biến V thành V'. Đặc biệt, nếu $p \geq 0$, tồn tại một biến đổi tuyến tính xạ ảnh biến V thành một đa tạp tuyến tính xạ ảnh *tọa độ*, tức là ảnh chính tắc của một đa tạp tọa độ W' có $p + 1$ chiều (không có điểm o) của $\mathbf{R}^{n+1}$. Nếu đồng nhất W' với $\mathbf{R}_{p+1}^*$, quan hệ cảm sinh bởi $\Delta_n$ trên W' chính xác là $\Delta_p$; vì W' đóng và bão hòa đối với $\Delta_n$, Bổ đề 1 cho thấy rằng V' đồng phôi với $P_p$ và đóng trong $P_n$; hơn nữa, nếu $p < n$, phần bù của nó trù mật trong $P_n$ ($\S$ 1, no. 4, Hệ quả của Mệnh đề 3). Suy ra:

#### Mệnh đề 4 {#top-vi-s3-prop-4 .statement}

*Mỗi đa tạp tuyến tính xạ ảnh có p chiều trong một không gian xạ ảnh $P_n$ đều đóng trong $P_n$ và đồng phôi với $P_p$; nếu $p < n$ thì phần bù của nó trù mật trong $P_n$.*

![Biểu đồ cho thấy một siêu phẳng H trong không gian xạ ảnh $P_n$, với các điểm $x_0^{-1}x$, x, và o, cùng một mặt phẳng B khác.](https://i.imgur.com/3Q5z5QG.png)

Hình 4.

tọa độ thuần nhất thỏa mãn một quan hệ dạng $\sum_{i=0}^{n} a_i x_i = 0$, trong đó các $a_i$ không đồng thời bằng không ("phương trình" của siêu phẳng).

#### Mệnh đề 5 {#top-vi-s3-prop-5 .statement}

*Trong một không gian xạ ảnh* $\mathbf{P}_n$ ($n \geq 0$), *phần bù của một siêu phẳng xạ ảnh* $\mathbf{H}$ *đồng phôi với* $\mathbf{R}^n$.

Bằng cách thực hiện một phép biến đổi tuyến tính xạ ảnh, ta có thể giả sử rằng $\mathbf{H}$ là siêu phẳng có phương trình là $x_0 = 0$. Tập hợp $A$ các điểm $x = (x_i)$ của $\mathbf{R}_{n+1}^*$ sao cho $x_0 \neq 0$ là mở và bão hòa đối với $\Delta_n$; ảnh chính tắc $C$ của nó trong $\mathbf{P}_n$, là phần bù của $\mathbf{H}$ trong $\mathbf{P}_n$, do đó là đồng phôi với thương của $A$ bởi quan hệ tương đương $\Theta$ cảm sinh trên $A$ bởi $\Delta_n$ (Bổ đề 1). Gọi $B$ là siêu phẳng có phương trình là $x_0 = 1$ trong $\mathbf{R}^{n+1}$. Với mỗi điểm $x \in A$ tương ứng điểm $x_0^{-1} x$ là nơi đường thẳng đi qua $0$ và $x$ cắt $B$ (Hình 4); theo cách này ta định nghĩa một ánh xạ liên tục $g$ của $A$ lên $B$ sao cho $g(x)$ là điểm duy nhất của $B$ đồng dư với $x$ modulo $\Theta$. Suy ra rằng $B$ là đồng phôi với $A/\Theta$ (Bổ đề 2), do đó với $C$; vì $B$ là đồng phôi với $\mathbf{R}^n$, chứng minh được hoàn tất.

#### Hệ quả {#top-vi-s3-n2-cor-1 .statement}

*Mọi điểm của* $\mathbf{P}_n$ *đều có một lân cận mở đồng phôi với* $\mathbf{R}^n$.

Đặc biệt suy ra rằng các không gian xạ ảnh thực là *liên thông địa phương* (điều này cũng suy ra từ Chương I, § II, no. 6, Mệnh đề 12).

### 3. NHÚNG KHÔNG GIAN SỐ THỰC VÀO KHÔNG GIAN XẠ ẢNH

Mệnh đề 5 của no. 2 chỉ ra rằng nếu ta cho một siêu phẳng xạ ảnh $\mathbf{H}$ trong $\mathbf{P}_n$ ($n \geq 0$), thì tồn tại một đồng phôi từ $\mathbf{R}^n$ lên phần bù $\mathbf{C}H$ của siêu phẳng này. Một khi $\mathbf{H}$ đã được chọn, thường thuận tiện khi *đồng nhất* $\mathbf{R}^n$ và $\mathbf{C}H$ bằng đồng phôi được định nghĩa trong Mệnh đề 5; khi đó siêu phẳng xạ ảnh $H$ được gọi là "ở vô cực", và các điểm cũng như các tập con của nó cũng vậy. Thông thường người ta lấy $H$ là siêu phẳng "tọa độ" có phương trình là $x_0 = 0$; và khi đó điểm $z = (z_1)$ của $\mathbf{R}^n$ được đồng nhất với điểm của $P_n$ có các tọa độ thuần nhất là $1, z_1, z_2, \ldots, z_n$.

Sau khi đã thực hiện sự đồng nhất này, bao đóng trong $P_n$ của bất kỳ đa tạp tuyến tính afin nào $V$ có $p$ chiều trong $\mathbf{R}^n$ là một đa tạp tuyến tính xạ ảnh có $p$ chiều, không được chứa trong siêu phẳng ở vô cực, và đồng nhất với đa tạp tuyến tính xạ ảnh được sinh bởi $V$. Ngược lại, mọi đa tạp tuyến tính xạ ảnh $P$ có $p$ chiều mà không được chứa trong siêu phẳng ở vô cực thì có vết trên $\mathbf{R}^n$ là một đa tạp tuyến tính afin có $p$ chiều, mà bao đóng của nó trong $P_n$ là $P$.

Trong trường hợp riêng $n = 1$, siêu phẳng ở vô cực là một điểm; vì $P_1$ là compact, suy ra từ định lý của Alexandroff (Chương I, § 9, no. 8, Định lý 4) rằng $P_1$ đồng phôi với không gian $\tilde{\mathbf{R}}$ thu được bằng cách compact hóa không gian địa phương compact $\mathbf{R}$ bằng phép nối một điểm (the "điểm ở vô cực"). Theo Mệnh đề 4 của § 2, no. 4, ta cũng thấy rằng đường thẳng xạ ảnh thực $P_1' \mathbf{R}$ đồng phôi với đường tròn $S_1$ và với xuyến $T$.

Mặt khác, nếu $n > 1$, thì $P_n(\mathbf{R})$ không đồng phôi với $S_n$, như ta sẽ thấy sau (cf. Bài tập 4).

"Điểm ở vô cực" của không gian $\tilde{\mathbf{R}}$ được ký hiệu bởi $\infty$, không có dấu nào gắn kèm. Cần tránh nhầm lẫn $\tilde{\mathbf{R}}$ với đường thẳng thực mở rộng $\mathbf{R}$ được định nghĩa trong Chương IV, § 4, vốn có hai "điểm ở vô cực"; thật vậy, $\tilde{\mathbf{R}}$ đồng phôi với không gian thương của $\mathbf{R}$ thu được bằng cách đồng nhất hai điểm $+\infty$ và $-\infty$.

### 4. ỨNG DỤNG VÀO MỞ RỘNG CÁC HÀM GIÁ TRỊ THỰC

Vì $\mathbf{R}$ có thể được xem như một tập con của $\tilde{\mathbf{R}}$, nên mọi ánh xạ của một tập $E$ vào $\mathbf{R}$ (tức là mọi hàm giá trị thực trên $E$) đều có thể được xem như một ánh xạ của $E$ vào $\tilde{\mathbf{R}}$; cụ thể hơn, nếu $E$ là một tập con của một không gian tôpô $F$ và $f$ là một ánh xạ của $E$ vào $\mathbf{R}$, thì có thể xảy ra rằng tại một số điểm của bao đóng $F_c$ của $E$, $f(x)$ tiến tới giới hạn $\infty$ khi $x$ tiến tới một trong các điểm này nhưng vẫn nằm trong $E$; khi đó ta có thể mở rộng hàm $f$ liên tục bằng cách gán cho nó giá trị $\infty$ tại các điểm này (Chương I, § 8, no. 5, Định lý 1).

Xét riêng trường hợp $E$ là một tập con của $\mathbf{R}^n$, trong đó chính không gian $\mathbf{R}^n$ được xem như được nhúng trong không gian xạ ảnh $P_n$; nếu ta giả sử rằng siêu phẳng ở vô cực là $x_0 = 0$, thì một hàm giá trị thực $f$ được xác định trên $E$ có thể được đồng nhất với ánh xạ

$$
(x_0, x_1, x_2, \ldots, x_n) \to f \left( \frac{x_1}{x_0}, \frac{x_2}{x_0}, \ldots, \frac{x_n}{x_0} \right)
$$

của $E$ vào $\tilde{\mathbf{R}}$; từ những gì đã nói ở đoạn trước có thể có thể mở rộng hàm này, không những tới một số điểm của $\mathbf{R}^n$ trong bao đóng của $E$, mà còn tới một số "điểm ở vô cực" của $\mathbf{P}_n$ trong bao đóng của $E$.

Ta hãy chỉ ra rằng, theo cách này, chẳng hạn, ta thu được sự mở rộng liên tục lên toàn bộ $\tilde{\mathbf{R}}$ của một hàm hữu tỉ của một biến thực, đã được định nghĩa trong đại số. Ta đồng nhất $\tilde{\mathbf{R}}$ với $\mathbf{P}_1$, mọi số thực $x \in \mathbf{R}$ được đồng nhất với điểm có tọa độ thuần nhất là $(1, x)$, và điểm $\infty$ với điểm có tọa độ thuần nhất là $(0, 1)$. Cho $u(x, y)$ là một hàm hữu tỉ, trong đó $u$ và $v$ là hai đa thức nguyên tố cùng nhau có bậc lần lượt là $m$ và $n$; nếu chẳng hạn ta giả sử rằng $m \leq n$, và nếu ta đặt $u_1(x, y) = x^n u(x, y)$, $v_1(x, y) = x^n v(x, y)$, thì hàm hữu tỉ $u/v$ có thể được xem như sự hạn chế, trên tập các số thực $x$ sao cho $v(x) \neq 0$, của ánh xạ $(x, y) \to (u_1(x, y), v_1(x, y))$. Nói cách khác, ta mở rộng $u/v$ bằng liên tục, bằng cách cho nó giá trị $\infty$ tại những điểm $x \in \mathbf{R}$ nơi $v(x) = 0$, và bằng cách cho nó tại điểm $\infty$ giá trị $0$ nếu $m < n$, giá trị $\infty$ nếu $m > n$, và giá trị của tỉ số các hệ số đầu nếu $m = n$.

Đặc biệt, hàm $1/x$ có thể được mở rộng tới điểm $0$ bằng cách lấy giá trị $\infty$ ở đó, tới $\infty$ bằng cách lấy giá trị $0$ ở đó; hàm đã mở rộng này hiển nhiên là một đồng phôi của $\tilde{\mathbf{R}}$ lên chính nó. Điều tương tự đúng với hàm phân tuyến tính $(ax + b)/(cx + d)$ khi $ad - bc \neq 0$.

Tương tự, nếu $n$ là một số nguyên $> 0$, thì hàm $x^n$ được mở rộng tới điểm $\infty$ bằng cách lấy giá trị $\infty$ ở đó.

Ngược lại, nhìn chung không thể mở rộng bằng liên tục một hàm hữu tỉ của hai biến thực hoặc tới không gian $\mathbf{P}_1 \times \mathbf{P}_1$ hoặc tới không gian $\mathbf{P}_2$ (xem Bài tập 5).

### 5. CÁC KHÔNG GIAN CỦA CÁC ĐA TẠP TUYẾN TÍNH XẠ ẢNH

Giả sử $K$ là một vành chia, tập $\mathbf{P}_{n,p}(K)$ các đa tạp tuyến tính xạ ảnh có số chiều $p \geq 0$ của không gian xạ ảnh trái $\mathbf{P}_n(K)$ rõ ràng tương ứng một-một với tập các không gian con vectơ có số chiều $p - 1$ của không gian vectơ trái $K_s^{p-1}$. Ký hiệu $L_{s-1,s-1}(K)$ là tập các hệ tự do $(x_i)_{1 \leq i \leq s-1}$ gồm $p - 1$ vectơ của $K_s^{p-1}$; khi đó tập $\mathbf{P}_{n,p}(K)$ lại tương ứng một-một với thương của $L_{n+1,\ p+1}(K)$ bởi quan hệ tương đương $\Delta_{n,\ p}(K)$: " $(x^k)$ và $(y^k)$ sinh ra cùng một không gian con vectơ có số chiều $p + 1$ của $K_s^{n+1}$". Trong phần sau, ta sẽ đồng nhất $P_{n,\ p}(K)$ với tập thương này. Mặt khác, nếu với mỗi hệ tự do $(x_k)$ gồm $p + 1$ vectơ của $K_s^{n+1}$ ta cho tương ứng ma trận $X$ gồm $p + 1$ hàng và $n + 1$ cột, trong đó $x_k$ là hàng thứ $k$ ($1 \leq k \leq p + 1$), thì ta có một sự tương ứng một-một giữa $L_{n+1,\ p+1}(K)$ và tập tất cả các ma trận có $p + 1$ hàng và $n + 1$ cột có hạng $p + 1$; ta sẽ đồng nhất $L_{n+1,\ p+1}(K)$ với tập các ma trận này, và quan hệ $\Delta_{n,\ p}(K)$ giữa hai ma trận $X, Y$ khi đó là như sau: "tồn tại một ma trận vuông khả nghịch $T$ có cấp $p + 1$ sao cho $Y = T.X$".

Trong phần sau, ta sẽ lấy $K$ là trường $\mathbf{R}$, và sẽ bỏ chữ $K$ trong ký hiệu ở trên. Ta có thể định nghĩa một tôpô trên $P_{n,\ p}$ bằng một quá trình khái quát hóa định nghĩa tôpô của các không gian xạ ảnh thực. Cụ thể, $L_{n+1,\ p+1}$ được chứa trong không gian $M_{p+1,\ n+1}$ của tất cả các ma trận có $p + 1$ hàng và $n + 1$ cột với phần tử thực; ta trang bị cho $L_{n+1,\ p+1}$ tôpô cảm sinh bởi tôpô của không gian ma trận này ($\S \ 1$, no. 6).

#### Định nghĩa 2 {#top-vi-s3-def-2 .statement}

*Không gian $P_{n,\ p}$, là thương của không gian tôpô $L_{n+1,\ p+1}$ bởi quan hệ tương đương $\Delta_{n,\ p}$, được gọi là không gian các đa tạp tuyến tính xạ ảnh có số chiều $p \geq 0$ trong không gian xạ ảnh thực $P_n$.*

Ta sẽ dùng ký hiệu sau: cho một ma trận $X$ gồm $p + 1$ hàng và $n + 1$ cột, và cho bất kỳ dãy tăng ngặt nào

$$
\sigma = (i_1, \ldots, i_{p+1})
$$

của $p + 1$ chỉ số thuộc khoảng $[0, n]$ của $\mathbf{N}$, ta ký hiệu $X_\sigma$ là ma trận con vuông của $X$ được tạo bởi các cột có các chỉ số là $i_1, i_2, \ldots, i_{p+1}$. Ta ký hiệu $A_\sigma$ là tập con của $L_{p+1,\ p+1}$ gồm các ma trận $X$ sao cho $X_\sigma$ không suy biến. Theo Mệnh đề 6 của $\S \ 1$, số 6, $A_\sigma$ là một tập *trù mật mở* trong $M_{p+1,\ n+1}$, và hàm $X \to X_\sigma^{-1}$ là *liên tục* trên $A_\sigma$.

Một diễn giải hình học của tập $A_\sigma$ như sau: gọi $E_\sigma$ là không gian con vectơ của $\mathbf{R}^{n+1}$ sinh bởi các vectơ $e_i$ của cơ sở chính tắc sao cho $i \in \sigma$, và gọi $E'_\sigma$ là không gian con bổ sung sinh bởi các $e_i$ sao cho $i \notin \sigma$; khi đó nói rằng một ma trận $x$ thuộc $A_\sigma$ có nghĩa là các hình chiếu trên $E_\sigma$ của $p + 1$ hàng của nó $x_k$ tạo thành một hệ tự do, hoặc cũng có nghĩa là không gian con vectơ sinh bởi các $x_k$ là một *phần bù* của $E'_\sigma$ (hoặc rằng giao của nó với $E'_\sigma$ chỉ gồm 0).

#### Mệnh đề 6 {#top-vi-s3-prop-6 .statement}

*Không gian $P_{n,\ p}$ là Hausdorff.*

Trước hết ta chứng minh rằng quan hệ $\Delta_{n,p}$ là mở. Nếu $U$ là một tập mở trong $L_{n+1,p+1}$, để bão hòa $U$ theo $\Delta_{n,p}$ ta phải lấy hợp các ảnh của $U$ qua ánh xạ $X \to T.X$, trong đó $T$ chạy qua tập các ma trận vuông không suy biến cấp $p+1$; vì mỗi ánh xạ này đều song liên tục, nên tất cả các ảnh đó đều là các tập mở và do đó hợp của chúng cũng vậy.

Theo Mệnh đề 8 của Chương I, § 8, no. 3, chứng minh sẽ hoàn tất nếu ta chứng minh rằng tập con $N$ của $L_{n+1,p+1} \times L_{n+1,p+1}$, được xác định bởi $\Delta_{n,p}$, là đóng. Gọi $(X, Y)$ là một điểm của không gian tích nằm trong bao đóng của $N$, và gọi $\sigma$ là một dãy chỉ số sao cho $X_\sigma$ không suy biến: vì $A_\sigma$ là mở, tồn tại một lân cận $V$ của $(X, Y)$ sao cho, với mỗi cặp $(X', Y') \in N \cap V$, ma trận $X'_\sigma$ không suy biến; khi $(X', Y')$ tiến tới $(X, Y)$ trong khi vẫn ở trong $N$, ma trận $Y'_\sigma {X'_\sigma}^{-1}$ do đó tiến tới $T = Y_\sigma X_\sigma^{-1}$; vì ta có $Y' = (Y'_\sigma {X'_\sigma}^{-1}) X'$, suy ra khi chuyển qua giới hạn rằng $Y = T.X$, và chứng minh hoàn tất.

#### Mệnh đề 7 {#top-vi-s3-prop-7 .statement}

*Không gian $P_{n,p}$ là compact.*

Chỉ cần chứng minh rằng tồn tại một không gian con compact của $L_{n+1,p+1}$ cắt mọi lớp tương đương mod $\Delta_{n,p}$ tại ít nhất một điểm; vì khi đó $P_{n,p}$ là ảnh của không gian con này qua ánh xạ chính tắc của $L_{n+1,p+1}$ lên $P_{n,p}$, và do đó compact (Chương I, § 9, no. 4, Định lý 2).

Cho $V_{n+1,p+1}$ là không gian con của $L_{n+1,p+1}$ mà các phần tử của nó là các hệ $(x_k)$ gồm $p+1$ vectơ tạo thành một *cơ sở Euclid trực chuẩn* của không gian con vectơ mà chúng sinh ra, tức là sao cho $(x_h/x_k) = 0$ khi nào $h \neq k$, $(x_h/x_k) = 1$ với $1 \leq h \leq p+1$. Mọi không gian con vectơ $p+1$ chiều của $\mathbf{R}^{n+1}$ đều có một cơ sở như thế, và do đó mọi lớp mod. $\Delta_{n,p}$ đều cắt $V_{n+1,p+1}$. Mặt khác, các ma trận $X = (x_{ij})$ của $V_{n+1,p+1}$ được xác định bởi các hệ thức

$$
\sum_{j=0}^n x_{ij}^2 = 1 \quad (1 \leq i \leq p+1),
$$
$$
\sum_{j=0}^n x_{ij} x_{kj} = 0 \quad (i \neq k);
$$

vì thế chúng tạo thành một tập *đóng* trong $M_{p+1,n+1}$; và vì các hệ thức này suy ra rằng $|x_{ij}| \leq 1$ đối với mỗi cặp chỉ số $(i, j)$, nên tập này *bị chặn* và do đó *compact*.

#### Mệnh đề 8 {#top-vi-s3-prop-8 .statement}

$P_{n,p}$ *liên thông và liên thông địa phương, và mọi điểm đều có một lân cận mở đồng phôi với* $\mathbf{R}^{(p+1)(n-p)}$.

Với mọi dãy chỉ số (tăng ngặt) $\sigma$, tập $A_\sigma$ là mở trong $L_{n+1,p+1}$ và bão hòa đối với $\Delta_{n,p}$; ảnh chính tắc của nó

C_σ trong P_{n,p} do đó là một tập mở đồng phôi với thương của A_σ theo quan hệ tương đương Θ_σ cảm sinh trên A_σ bởi Δ_{n,p} (Bổ đề 1).

Cho $B_σ$ là tập con của $A_σ$ gồm các ma trận $X$ sao cho $X_σ$ là ma trận đơn vị cấp $p + 1$; các phần tử của $X$ khác với những phần tử của $X_σ$ khi đó là tùy ý, và do đó $B_σ$ đồng phôi với không gian $\mathbf{R}^{(p+1)(n-p)}$. Ứng với mỗi ma trận $X \in A_σ$, ta cho ma trận $Y = X_σ^{-1}X$, thuộc $B_σ$; khi đó ta đã xác định một ánh xạ liên tục $g$ của $A_σ$ lên $B_σ$, sao cho $g(X)$ là ma trận duy nhất của $B_σ$ đồng dư với X mod Θ_σ. Suy ra rằng $B_σ$ đồng phôi với $A_σ/\Theta_σ$ (Bổ đề 2), nên cũng đồng phôi với $C_σ$.

Do đó tập $C_σ$ liên thông. Vì $A_σ$ trù mật trong $L_{n+1,p+1}$, nên $C_σ$ trù mật trong $P_{n,p}$ và do đó $P_{n,p}$ cũng liên thông (Chương I, § 11, no. 1, Mệnh đề 1). Mặt khác, mỗi điểm của $P_{n,p}$ thuộc về $C_σ$ đối với ít nhất một dãy chỉ số $\sigma$, và do đó có một lân cận mở đồng phôi với $\mathbf{R}^{(p+1)(n-p)}$.

Ma trận $Y = g(X)$ có thể được hiểu như sau: để đơn giản, ta giả sử rằng dãy $\sigma$ gồm $p + 1$ chỉ số $n - p$, $n - p + 1$, ..., $n$, và cho $a_{ij}$ (1 ≤ i ≤ p + 1, 0 ≤ j ≤ n − p − 1) ký hiệu các phần tử của $n - p$ cột đầu của y; khi đó không gian con vectơ của $\mathbf{R}^{n+1}$ được sinh bởi các hàng của x là không gian được xác định bởi các phương trình

$$
x_j = \sum_{i=1}^{p+1} a_{ij} x_{n-p+i-1} \quad (0 ≤ j ≤ n-p-1).
$$

### 6. GRASSMANNIANS

Nếu $K$ là một trường và $X$ là một ma trận bất kỳ của $L_{n+1,p+1}(K)$, hãy ký hiệu $c_σ(X)$ là định thức của $X_σ$; theo cách đó, ứng với mỗi ma trận $X$ của $L_{n+1,p+1}(K)$ ta có

$$
h = \binom{n+1}{p+1}
$$

định thức, không phải tất cả đều bằng không (các thành phần của tích ngoài của $p + 1$ hàng của $X$). Nếu ta cho ứng với $X$ là điểm của không gian xạ ảnh $P_{n-1}(K)$ có các tọa độ thuần nhất là các $c_σ(X,)$, ta đã xác định một ánh xạ của $L_{n+1,p+1}(K)$ vào $P_{n-1}(K)$, tương thích với quan hệ $\Delta_{n,p}(K)$; đi qua thương, do đó ta có một ánh xạ $f$ của $P_{n,p}(K)$ vào $P_{n-1}(K)$. Ảnh $G_{n,p}(K)$ của $P_{n,p}(K)$ qua ánh xạ này được gọi là Grassmannian của các chỉ số n, p. Ta cũng nhắc lại rằng ánh xạ $f$ là đơn ánh, vì nếu $X$ là một ma trận sao cho $X_σ$ không suy biến, thì ma trận $Y = X_σ^{-1}X$ thuộc $B_σ$ ứng với lớp của $X$ mod. $\Delta_{n,p}(K)$ là ma trận $(d_{ij}/c_σ(X))$ (1 ≤ i ≤ p + 1, 0 ≤ j ≤ n), trong đó $d_{ij}$ ký hiệu định thức của ma trận thu được từ $X_{\sigma}$ bằng cách thay thế cột thứ $i$ của $X_{\sigma}$ bằng cột thứ $j$ của $X$ [điều này suy ra rằng $d_{ij}$, tới dấu, bằng một trong các $c_{\tau}(X)$].

Khi $K$ là trường $\mathbf{R}$, ánh xạ $f$ này hiển nhiên là *liên tục*. Ánh xạ nghịch đảo $g$ cũng liên tục; vì các phần tử của một ma trận thuộc $B_{\sigma}$ là các hàm hữu tỉ của các tọa độ thuần nhất của điểm của Grassmannian mà nó tương ứng với; vì $f(B_{\sigma}) = B'_{\sigma}$ là tập các điểm của $G_{n,p}$ có tọa độ thuần nhất với chỉ số $\sigma$ khác 0, nên đó là một tập mở trong $G_{n,p}$; do đó $g$ liên tục tại mọi điểm của $B'_{\sigma}$, và vì mọi điểm của $G_{n,p}$ thuộc về ít nhất một tập $B'_{\sigma}$, nên $g$ liên tục tại mọi điểm. Vậy:

#### Mệnh đề 9 {#top-vi-s3-prop-9 .statement}

*Grassmannian* $G_{n,p}$ *đồng phôi với không gian* $P_{n,p}$.

Chúng tôi nhắc lại cuối cùng rằng các Grassmannian $G_{n,p}(K)$ và $G_{n,n-p-1}(K)$ là các tập con của cùng một không gian xạ ảnh $P_{n-1}(K)$ và có thể được biến đổi thành nhau bởi một phép biến đổi tuyến tính xạ ảnh; suy ra rằng $G_{n,p}$ và $G_{n,n-p-1}$ là *đồng phôi*.

### Bài tập {#top-vi-s3-exercises}

Xem [các bài tập cho § 3](exercises/s3/).
