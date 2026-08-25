---
book: top
book_title: General Topology
chapter: I
chapter_title: Topological Structures
section: 7
section_title: Limits
lang: vi
source: top-i-iv
pdf_pages: 0074-0080, 0138-0139
extraction: ocr
subsections:
    - "no": 1
      title: LIMIT OF A FILTER
      page: 0
      pdf_page: 74
    - "no": 2
      title: CLUSTER POINT OF A FILTER BASE
      page: 0
      pdf_page: 75
    - "no": 3
      title: LIMIT POINT AND CLUSTER POINT OF A FUNCTION
      page: 0
      pdf_page: 76
    - "no": 4
      title: LIMITS AND CONTINUITY
      page: 0
      pdf_page: 78
    - "no": 5
      title: LIMITS RELATIVE TO A SUBSPACE
      page: 0
      pdf_page: 79
    - "no": 6
      title: LIMITS IN PRODUCT SPACES AND QUOTIENT SPACES
      page: 0
      pdf_page: 80
statements: 23
exercises: 7
content_sha256: 92b070747ad61a3fbd2013d61946e7f39b68c9228397cf43abe28472cff13701
translated_from: content/en/top/I/07_s7_limits.md
source_content_sha256: 8fe36d3d61f3f8eba3dff884ac608e18a0cc790c414cc3bec399444177eeb152
translation_model: gpt-5.4
translation_run: translate-vi-65ba7a71
glossary_version: 34
glossary_terms_sha256: e4b560dc287bbaa2528ec24c36f5d94613a35e2b393441e4f9a322dcede43e4c
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 7. GIỚI HẠN

### 1. GIỚI HẠN CỦA MỘT BỘ LỌC

#### Định nghĩa 1 {#top-i-s7-def-1 .statement}

Cho $X$ là một không gian tôpô và $\mathfrak{F}$ là một bộ lọc trên $X$. Một điểm $x \in X$ được gọi là một điểm giới hạn (hoặc đơn giản là một giới hạn) của $\mathfrak{F}$, nếu $\mathfrak{F}$ mịn hơn bộ lọc lân cận $\mathcal{B}(x)$ của $x$; cũng nói rằng $\mathfrak{F}$ hội tụ (hoặc là hội tụ) đến $x$. *Điểm* $x$ *được gọi là một giới hạn của một cơ sở bộ lọc* $\mathcal{B}$ *trên* $X$, *và* $\mathcal{B}$ *được nói là hội tụ đến* $x$, *nếu bộ lọc có cơ sở là* $\mathcal{B}$ *hội tụ đến* $x$.

Định nghĩa này, cùng với Mệnh đề 4 của § 6, no. 3, cho tiêu chuẩn sau đây:

#### Mệnh đề 1 {#top-i-s7-prop-1 .statement}

*Một cơ sở lọc* $\mathcal{B}$ *trên một không gian tôpô* $X$ *hội tụ tới* $x$ *khi và chỉ khi mọi tập hợp của một hệ cơ bản các lân cận của* $x$ *đều chứa một tập hợp của* $\mathcal{B}$.

Phù hợp với thuật ngữ được đưa vào ở § 1, no. 2, ta có thể phát biểu Mệnh đề 1 theo cách sau: $\mathcal{B}$ hội tụ tới $x$ khi và chỉ khi có những tập hợp của $\mathcal{B}$ *ở gần tùy ý của* $x$.

Nếu một bộ lọc $\mathfrak{F}$ hội tụ tới $x$, thì mọi bộ lọc *mịn hơn* $\mathfrak{F}$ cũng hội tụ tới $x$, theo Định nghĩa 1. Tương tự, nếu tôpô của $X$ được thay bằng một tôpô *thô hơn*, thì bộ lọc lân cận của $x$ được thay bằng một bộ lọc *thô hơn* ($\S$ 2, no. 2, Mệnh đề 3), và do đó $\mathfrak{F}$ vẫn hội tụ tới $x$ trong tôpô mới này.

Vì thế ta có thể nói rằng *tôpô càng mịn thì trong tôpô ấy càng có ít bộ lọc hội tụ*. Đặc biệt, trong tôpô rời rạc, các bộ lọc hội tụ duy nhất là các bộ lọc lân cận, vì đó là các siêu bộ lọc tầm thường trên $X$ ($\S$ 6, no. 4).

Cho $\Phi$ là một tập hợp các bộ lọc trên $X$, tất cả đều hội tụ đến cùng một điểm $x$; bộ lọc lân cận $\mathcal{B}(x)$ thô hơn tất cả các bộ lọc của $\Phi$, vì thế cũng thô hơn *giao* $\mathfrak{J}$ của các bộ lọc này; nói cách khác, $\mathfrak{J}$ cũng hội tụ đến $x$.

#### Mệnh đề 2 {#top-i-s7-prop-2 .statement}

*Một bộ lọc* $\mathfrak{F}$ *trên một không gian tôpô* $X$ *hội tụ đến một điểm* $x$ *khi và chỉ khi mọi siêu bộ lọc mịn hơn* $\mathfrak{F}$ *đều hội tụ đến* $x$.

Đây là một hệ quả ngay lập tức của các nhận xét trước đó và Mệnh đề 7 của § 6, no. 4.

Nói chung một bộ lọc có thể có *nhiều điểm giới hạn phân biệt*; chúng ta sẽ trở lại câu hỏi này trong § 8, no. 1.

### 2. ĐIỂM TỤ CỦA MỘT CƠ SỞ BỘ LỌC

#### Định nghĩa 2 {#top-i-s7-def-2 .statement}

*Trong một không gian tôpô* $X$, *một điểm* $x$ *là một điểm tụ của một cơ sở lọc* $\mathcal{B}$ *trên* $X$ *nếu nó nằm trong bao đóng của mọi tập hợp thuộc* $\mathcal{B}$.

Nếu $x$ là một điểm tụ của một cơ sở lọc $\mathcal{B}$, thì nó cũng là một điểm tụ của mọi cơ sở lọc *tương đương* theo § 6, no. 3, hệ quả của Mệnh đề 4; đặc biệt, $x$ là một điểm tụ của *bộ lọc* có cơ sở là $\mathcal{B}$.

#### Mệnh đề 3 {#top-i-s7-prop-3 .statement}

*Một điểm x là một điểm tụ của một cơ sở lọc B khi và chỉ khi mọi tập hợp của một hệ cơ bản các lân cận của x đều giao với mọi tập hợp của B.*

Điều này suy ra ngay lập tức từ các định nghĩa.

Mệnh đề này và Hệ quả 2 của Mệnh đề 1 ở § 6, no. 2 cho thấy tính chất "x là một điểm tụ của bộ lọc $\mathfrak{F}$" là tương đương với tính chất "tồn tại một bộ lọc mịn hơn cả $\mathfrak{F}$ lẫn bộ lọc lân cận của x". Nói cách khác:

#### Mệnh đề 4 {#top-i-s7-prop-4 .statement}

*Một điểm x là một điểm tụ của một bộ lọc $\mathfrak{F}$ khi và chỉ khi tồn tại một bộ lọc mịn hơn $\mathfrak{F}$ và hội tụ đến x.*

Đặc biệt, mọi *điểm giới hạn* của một bộ lọc $\mathfrak{F}$ đều là một *điểm tụ* của $\mathfrak{F}$.

#### Hệ quả {#top-i-s7-n2-cor-1 .statement}

*Một siêu bộ lọc $\mathcal{U}$ hội tụ đến một điểm x khi và chỉ khi x là một điểm tụ của $\mathcal{U}$.*

Nếu x là một điểm tụ của một bộ lọc $\mathfrak{F}$, thì nó cũng là một điểm tụ của mọi bộ lọc *thô hơn* $\mathfrak{F}$; tương tự, nếu ta thay thế tôpô của X bằng một tôpô *thô hơn*, thì x vẫn là một điểm tụ của $\mathfrak{F}$ đối với tôpô mới.

Theo định nghĩa, tập hợp các điểm tụ của một cơ sở bộ lọc $\mathcal{B}$ trên X là tập hợp $\bigcap_{M \in \mathcal{B}} \overline{M}$, do đó

#### Mệnh đề 5 {#top-i-s7-prop-5 .statement}

*Tập hợp các điểm tụ của một cơ sở bộ lọc trên một không gian tôpô X là đóng trong X.*

#### Mệnh đề 6 {#top-i-s7-prop-6 .statement}

*Cho $\mathcal{B}$ là một cơ sở bộ lọc trên một tập con A của một không gian tôpô X. Khi đó mọi điểm tụ của $\mathcal{B}$ trong X đều thuộc $\overline{A}$; và ngược lại mọi điểm của $\overline{A}$ đều là một điểm giới hạn của một bộ lọc trên A.*

Mệnh đề thứ nhất là tầm thường; mặt khác, nếu $x \in \overline{A}$, thì vết trên A của bộ lọc lân cận của x trong X là một bộ lọc trên A hiển nhiên hội tụ đến x.

#### Nhận xét {#top-i-s7-n2-rem-1 .statement}

Một bộ lọc trên một không gian tôpô có thể không có điểm tụ nào (và *a fortiori* không có điểm giới hạn nào); ví dụ, trong một *không gian rời rạc vô hạn* thì bộ lọc các phần bù của các tập con hữu hạn không có điểm tụ nào. Các không gian mà trong đó mọi bộ lọc đều có một điểm tụ giữ một vai trò quan trọng trong toán học, và chúng ta sẽ nghiên cứu chúng trong § 9.

### 3. ĐIỂM GIỚI HẠN VÀ ĐIỂM TỤ CỦA MỘT HÀM

#### Định nghĩa 3 {#top-i-s7-def-3 .statement}

*Cho f là một ánh xạ từ một tập hợp X vào một không gian tôpô Y, và cho $\mathfrak{F}$ là một bộ lọc trên X. Một điểm $y \in Y$ được gọi là một điểm giới hạn (hoặc đơn giản là một giới hạn) (resp. điểm tụ) của f đối với bộ lọc $\mathfrak{F}$ nếu y là một điểm giới hạn (resp. điểm tụ) của cơ sở lọc $f(\mathfrak{F})$.*

Quan hệ "y là một giới hạn của f đối với bộ lọc $\mathfrak{F}$" được viết là $\lim_{\mathfrak{F}} f = y$, hoặc $\lim_{x, \mathfrak{F}} f(x) = y$, hoặc $\lim_x f(x) = y$ nếu không có nguy cơ nhầm lẫn.

Từ Định nghĩa 3 và các Mệnh đề 1 (no. 1) và 3 (no. 2) suy ra các tiêu chuẩn sau:

#### Mệnh đề 7 {#top-i-s7-prop-7 .statement}

*Một điểm $y \in Y$ là một giới hạn của $f$ đối với bộ lọc $\mathfrak{F}$ khi và chỉ khi, với mỗi lân cận $V$ của $y$ trong $Y$, tồn tại một tập hợp $M \in \mathfrak{F}$ sao cho $f(M) \subset V$ (nghĩa là $\overline{f}(V) \in \mathfrak{F}$ với mỗi lân cận $V$ của $y$).*
*Một điểm $y \in Y$ là một điểm tụ của $f$ đối với bộ lọc $\mathfrak{F}$ khi và chỉ khi với mỗi lân cận $V$ của $y$ và mỗi $M \in \mathfrak{F}$ tồn tại một điểm $x \in M$ sao cho $f(x) \in V$.*

#### Ví dụ 1 {#top-i-s7-n3-exa-1 .statement}

Một dãy các điểm $(x_n)_{n \in \mathbf{N}}$ của một không gian tôpô là một ánh xạ $n \to x_n$ từ $\mathbf{N}$ vào $X$. Trong giải tích người ta thường dùng các khái niệm điểm giới hạn và điểm tụ của một ánh xạ như thế *đối với bộ lọc Fréchet* (\S 6, no. 1) trên $\mathbf{N}$; nếu $y$ là một giới hạn của $n \to x_n$ đối với bộ lọc Fréchet, thì $y$ được gọi là một *giới hạn của dãy* $(x_n)$ *khi n tiến ra vô hạn*, và ta viết $\lim_{n \to \infty} x_n = y$. Một điểm tụ của ánh xạ $n \to x_n$ đối với bộ lọc Fréchet được gọi là một *điểm tụ của dãy* $(x_n)$.

Như vậy một điểm $y \in X$ là một giới hạn (tương ứng, điểm tụ) của một dãy $(x_n)$ các điểm của $X$ nếu nó là một điểm giới hạn (tương ứng, điểm tụ) của *bộ lọc sơ cấp liên kết với* $(x_n)$ (\S 6, no. 8).

Điểm $y$ là một giới hạn của một dãy $(x_n)$ trong $X$ khi và chỉ khi, với *mọi* lân cận $V$ của $y$ trong $X$, *mọi số hạng trừ một số hữu hạn của dãy* $(x_n)$ *đều thuộc* $V$, tức là tồn tại một số nguyên $n_0$ sao cho $x_n \in V$ với mọi $n \geq n_0$. Tương tự, $y$ là một điểm tụ của dãy $(x_n)$ khi và chỉ khi, với *mọi* lân cận $V$ của $y$ trong $X$ và *mọi* số nguyên $n_0$, tồn tại một số nguyên $n \geq n_0$ sao cho $x_n \in V$.

#### Ví dụ 2 {#top-i-s7-n3-exa-2 .statement}

Nói chung hơn, cho $f$ là một ánh xạ từ một tập hợp *có hướng* $A$ vào một không gian tôpô $X$. Nếu $x \in X$ là một giới hạn (tương ứng, điểm tụ) của $f$ đối với *bộ lọc tiết diện* của $A$ thì nói rằng $x$ là một *giới hạn* (tương ứng, *điểm tụ*) của $f$ *đối với tập có hướng* $A$, và ta viết $x = \lim_{z \in A} f(z)$.

Nếu $y$ là một giới hạn (tương ứng, điểm tụ) của một ánh xạ $f : X \to Y$ đối với một bộ lọc $\mathfrak{F}$ trên $X$, thì $y$ vẫn là một giới hạn (tương ứng, điểm tụ) của $f$ đối với $\mathfrak{F}$ nếu ta thay thế tôpô của $Y$ bằng một tôpô *thô hơn*, hoặc nếu ta thay thế bộ lọc $\mathfrak{F}$ bằng một bộ lọc *mịn hơn* (tương ứng, *thô hơn*).

#### Mệnh đề 8 {#top-i-s7-prop-8 .statement}

*Cho $f$ là một ánh xạ từ một tập hợp $X$ vào một không gian tôpô $Y$; khi đó $y \in Y$ là một điểm tụ của $f$ đối với $\mathfrak{F}$ nếu và chỉ nếu tồn tại một bộ lọc $\mathfrak{G}$ trên $X$ mịn hơn $\mathfrak{F}$ và sao cho $y$ là một giới hạn của $f$ đối với $\mathfrak{G}$.*

Vì nếu $y$ là một điểm tụ của $f$ đối với $\mathfrak{F}$, và nếu $\mathcal{B}$ là bộ lọc lân cận của $y$, thì $\overline{f}^{-1}(\mathcal{B})$ là một cơ sở bộ lọc trên $X$ vì mọi tập hợp của $\overline{f}^{-1}(\mathcal{B})$ đều gặp mọi tập hợp của $\mathfrak{F}$ (\S 6, no. 6). Nhận xét này cũng cho thấy rằng có một bộ lọc $\mathcal{G}$ trên $X$ mịn hơn cả $\mathfrak{F}$ lẫn bộ lọc có cơ sở $\overline{f}^{-1}(\mathcal{B})$ (\S 6, no. 2, Mệnh đề 1, Hệ quả 2), do đó $y$ là một điểm giới hạn của $f$ đối với $\mathcal{G}$.

Sau cùng, hãy lưu ý rằng nếu $f$ là một ánh xạ của một tập hợp $X$ vào một không gian tôpô $Y$, thì tập hợp các điểm tụ của $f$ đối với một bộ lọc $\mathfrak{F}$ trên $X$ là *đóng* trong $Y$ (no. 2, Mệnh đề 5) và có thể rỗng.

#### Nhận xét {#top-i-s7-n3-rem-1 .statement}

Nếu $y \in Y$ là một giới hạn (tương ứng, điểm tụ) của một ánh xạ $f : X \to Y$ đối với một bộ lọc $\mathfrak{F}$ trên $X$, thì $y$ cũng là một giới hạn (tương ứng, điểm tụ) của mọi hàm $g : X \to Y$ có *cùng mầm* với $f$ đối với $\mathfrak{F}$ (\S 6, no. 9); khi đó nói rằng $y$ là một *giới hạn* (tương ứng, *điểm tụ*) *của mầm* $\tilde{f}$ *của* $f$ đối với $\mathfrak{F}$.

### 4. GIỚI HẠN VÀ TÍNH LIÊN TỤC

Cho $X, Y$ là hai không gian tôpô, $f$ là một ánh xạ từ $X$ vào $Y$, $\mathcal{B}$ là bộ lọc lân cận trong $X$ của một điểm $a \in X$. Thay cho việc nói rằng $y \in Y$ là một giới hạn của $f$ đối với bộ lọc $\mathcal{B}$ và viết $y = \lim_{\mathcal{B}} f$, chúng tôi dùng ký hiệu đặc biệt

$$
y = \lim_{i \in I} f(x),
$$

và ta nói rằng $y$ là *giới hạn của* $f$ *tại điểm* $a$, hoặc rằng $f(x)$ *tiến tới* $y$ *khi* $x$ *tiến tới* $a$. Tương tự, thay vì nói rằng $y$ là một điểm tụ của $f$ đối với $\mathcal{B}$, ta nói rằng $y$ *là một điểm tụ của* $f$ *tại điểm* $a$.

Việc xét định nghĩa của tính liên tục (\S 2, no. 1, Định nghĩa 1) và Mệnh đề 7 của no. 3 cho thấy rằng:

#### Mệnh đề 9 {#top-i-s7-prop-9 .statement}

*Một ánh xạ* $f$ *từ một không gian tôpô* $X$ *vào một không gian tôpô* $Y$ *liên tục tại điểm* $a \in X$ *khi và chỉ khi* $\lim_{i \in I} f(x) = f(a)$.

#### Hệ quả 1 {#top-i-s7-prop-9-cor-1 .statement}

*Cho* $X, Y$ *là hai không gian tôpô, $f$ là một ánh xạ của* $X$ *vào* $Y$ *liên tục tại một điểm* $a \in X$; *khi đó, với mọi cơ sở lọc* $\mathcal{B}$ *trên* $X$ *hội tụ đến* $a$, *cơ sở lọc* $f(\mathcal{B})$ *hội tụ đến* $f(a)$. *Ngược lại, nếu với mọi siêu lọc* $\mathcal{U}$ *trên* $X$ *hội tụ đến* $a$, *cơ sở siêu lọc* $f(\mathcal{U})$ *hội tụ đến* $f(a)$, *thì* $f$ *liên tục tại* $a$.

Mệnh đề thứ nhất là một hệ quả ngay lập tức của Mệnh đề 9. Để chứng minh mệnh đề thứ hai, giả sử rằng $f$ không liên tục tại $a$; khi đó tồn tại một lân cận W của $f(a)$ trong Y sao cho $\overline{f}^{-1}(W)$ không thuộc bộ lọc $\mathfrak{B}$ các lân cận của $a$ trong X. Do đó (\S 6, no. 4, Mệnh đề 7) tồn tại một siêu bộ lọc $\mathfrak{U}$, mịn hơn $\mathfrak{B}$, không chứa $\overline{f}^{-1}(W)$ và vì thế chứa phần bù của nó $A = X - \overline{f}^{-1}(W)$ (\S 6, no. 4, Mệnh đề 5); vì $f(A) \cap W = \varnothing$, $f(\mathfrak{U})$ không hội tụ tới $f(a)$.

#### Hệ quả 2 {#top-i-s7-prop-9-cor-2 .statement}

*Nếu g là một ánh xạ từ một tập hợp Z vào một không gian tôpô X, có giới hạn a đối với một bộ lọc $\mathfrak{F}$ trên Z, thì nếu ánh xạ $f : X \to Y$ liên tục tại a, hợp thành $f \circ g$ có $f(a)$ làm một điểm giới hạn đối với $\mathfrak{F}$.*

### 5. GIỚI HẠN TƯƠNG ĐỐI ĐỐI VỚI MỘT KHÔNG GIAN CON

Cho X, Y là hai không gian tôpô, cho A là một tập con của X, và cho $a \in X$ là một điểm của *bao đóng* của A (nhưng không nhất thiết thuộc A). Cho $\mathfrak{F}$ là *vết* trên A của bộ lọc lân cận của $a$ trong X. Nếu $f$ là một ánh xạ từ A vào Y, thì thay vì nói rằng $y \in Y$ là một giới hạn của $f$ đối với $\mathfrak{F}$ và viết $y = \lim_{\mathfrak{F}} f$, ta viết

$$
y = \lim_{x \to a, x \in A} f(x)
$$

và ta nói rằng $y$ là một *giới hạn của f tại a, tương đối với không gian con* A, hoặc rằng $f(x)$ *tiến tới y khi x tiến tới a mà vẫn thuộc* A. Khi đó ta có $y \in f(A)$.

Nếu $A = \mathbf{C}\{a\}$ trong đó $a$ *không* là một điểm cô lập của X, thì ta viết

$$
y = \lim_{x \to a, x \neq a} f(x)
$$

thay cho $y = \lim_{x \to a, x \in A} f(x)$.

Ta đưa ra các định nghĩa tương tự cho các điểm tụ.

Nếu $f$ là *hạn chế* của một ánh xạ $g : X \to Y$ lên A, thì ta nói rằng $g$ có một giới hạn (tương ứng, điểm tụ) $y$ tương đối với A tại một điểm $a \in \overline{A}$, nếu $y$ là một giới hạn (tương ứng, điểm tụ) của $f$ tại $a$, tương đối với A.

Cho B là một tập con của A và cho $a \in X$ là một điểm của bao đóng của B; nếu $y$ là một giới hạn tại $a$, *đối với* A, của một ánh xạ $f : A \to Y$, thì $y$ cũng là một giới hạn của $f$ tại $a$, *đối với* B; điều đảo lại không nhất thiết đúng.

Nhưng nếu V là một *lân cận* trong X của một điểm $a \in \overline{A}$ và nếu $f$ có giới hạn $y$ tại $a$, *đối với* $V \cap A$, thì $y$ vẫn là một giới hạn của $f$ tại $a$, *đối với* A.

Cho $a$ là một điểm *không cô lập* của X, sao cho $a$ thuộc bao đóng của $\mathbf{C}\{a\}$. Khi đó một ánh xạ $f : X \to Y$ là *liên tục tại* $a$ nếu và chỉ nếu ta có $f(a) = \lim_{x \to a, x \neq a} f(x)$; điều này suy ra ngay lập tức từ các định nghĩa.

### 6. GIỚI HẠN TRONG CÁC KHÔNG GIAN TÍCH VÀ CÁC KHÔNG GIAN THƯƠNG

#### Mệnh đề 10 {#top-i-s7-prop-10 .statement}

Cho $X$ là một tập hợp, cho $(Y_i)_{i \in I}$ là một họ các không gian tôpô, và với mỗi $i \in I$ cho $f_i$ là một ánh xạ từ $X$ vào $Y_i$. Cho $X$ được trang bị tôpô thô nhất $\mathcal{T}$ sao cho các $f_i$ là liên tục. Khi đó, điều kiện cần và đủ để một bộ lọc $\mathfrak{F}$ trên $X$ hội tụ đến $a \in X$ là, với mỗi $i \in I$, cơ sở bộ lọc $f_i(\mathfrak{F})$ hội tụ đến $f_i(a)$ trong $Y_i$.

Điều kiện là cần thiết vì các $f_i$ là liên tục (no. 4, Mệnh đề 9, Hệ quả 1). Ngược lại, giả sử rằng điều kiện được thỏa mãn, và cho $V$ là một lân cận mở của $a$ trong $X$. Theo định nghĩa của $\mathcal{T}$ (\S 2, no. 3, Mệnh đề 4), tồn tại một tập con hữu hạn $J$ của $I$, và với mỗi $i \in J$ một tập con mở $U_i$ của $Y_i$, sao cho $f_i(a) \in U_i$ với $i \in J$ và sao cho $V$ chứa tập hợp
$$
\bigcap_{i \in J} f_i^{-1}(U_i).
$$
Giả thiết suy ra rằng $f_i^{-1}(U_i) \in \mathfrak{F}$ (no. 3, Mệnh đề 7); vì $J$ là hữu hạn, suy ra rằng
$$
M = \bigcap_{i \in J} f_i^{-1}(U_i)
$$
thuộc $\mathfrak{F}$, và $M \subset V$. Điều này hoàn thành chứng minh.

#### Hệ quả 1 {#top-i-s7-prop-10-cor-1 .statement}

Một bộ lọc $\mathfrak{F}$ trên một không gian tích $X = \prod_{i \in I} X_i$ hội tụ đến một điểm $x$ khi và chỉ khi với mỗi $i \in I$ cơ sở lọc $\operatorname{pr}_i(\mathfrak{F})$ hội tụ đến $\operatorname{pr}_i(x)$.

#### Hệ quả 2 {#top-i-s7-prop-10-cor-2 .statement}

Cho $f = (f_i)$ là một ánh xạ từ một tập hợp $X$ vào một không gian tích $Y = \prod_{i \in I} Y_i$. Khi đó $f$ có giới hạn $y = (y_i)$ đối với một bộ lọc $\mathfrak{F}$ trên $X$ nếu và chỉ nếu với mọi $i \in I$ thì $f_i$ có giới hạn $y_i$ đối với $\mathfrak{F}$.

#### Mệnh đề 11 {#top-i-s7-prop-11 .statement}

Cho $R$ là một quan hệ tương đương mở trên một không gian tôpô $X$ và gọi $\varphi$ là ánh xạ chính tắc $X \to X/R$. Khi đó, với mỗi $x \in X$ và mỗi cơ sở bộ lọc $\mathcal{B}'$ trên $X/R$ hội tụ đến $\varphi(x)$, tồn tại một cơ sở bộ lọc $\mathcal{B}$ trên $X$ hội tụ đến $x$ và sao cho $\varphi(\mathcal{B})$ tương đương với $\mathcal{B}'$.

Nếu $U$ là một lân cận bất kỳ của $x$ trong $X$, thì $\varphi(U)$ là một lân cận của $\varphi(x)$ trong $X/R$ (\S 5, no. 3, Mệnh đề 5), do đó tồn tại một tập hợp $M' \in \mathcal{B}'$ sao cho $M' \subset \varphi(U)$; nếu đặt $M = U \cap \varphi^{-1}(M')$, thì $M' = \varphi(M)$. Điều này cho thấy rằng khi $M'$ chạy qua $\mathcal{B}'$ và $U$ chạy qua bộ lọc lân cận của $x$, thì các tập hợp $U \cap \varphi^{-1}(M')$ tạo thành một cơ sở của bộ lọc $\mathcal{B}$ trên $X$; rõ ràng $\mathcal{B}$ hội tụ đến $x$ và $\varphi(\mathcal{B})$ tương đương với $\mathcal{B}'$.

### Bài tập {#top-i-s7-exercises}

Xem [các bài tập của § 7](exercises/s7/).
