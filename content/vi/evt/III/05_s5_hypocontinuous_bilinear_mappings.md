---
book: evt
book_title: Topological Vector Spaces
chapter: III
chapter_title: SPACES OF CONTINUOUS LINEAR MAPPINGS
section: 5
section_title: Hypocontinuous bilinear mappings
lang: vi
source: evt-i-v
book_pages: TVS III.28-TVS III.33, TVS III.46-TVS III.49
pdf_pages: 0160-0165, 0178-0181
extraction: ocr
subsections:
    - "no": 1
      title: Separately continuous bilinear mappings
      page: 28
      pdf_page: 160
    - "no": 2
      title: Separately continuous bilinear mappings on a product of Fréchet spaces
      page: 29
      pdf_page: 161
    - "no": 3
      title: Hypocontinuous bilinear mappings
      page: 30
      pdf_page: 162
    - "no": 4
      title: Extension of a hypocontinuous bilinear mapping
      page: 32
      pdf_page: 164
    - "no": 5
      title: Hypocontinuity of the mapping $(u, v) \mapsto v \circ u$
      page: 32
      pdf_page: 164
statements: 16
exercises: 15
content_sha256: 06e260806e85baf1fe4b11b64c328fdca99decbb5facabf26e221cab9750214f
translated_from: content/en/evt/III/05_s5_hypocontinuous_bilinear_mappings.md
source_content_sha256: b5755948295cc28eeaa8a16dd678ffa2ce677b2bb914f5ea6530d05c0e05a8cd
translation_model: gpt-5.4-mini
translation_run: translate-vi-f8d5b184
glossary_version: 34
glossary_terms_sha256: 48a3190f6e710dc0974709c4ed88709316ff2f058c9cd45a538f205f21e1f38e
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 5. CÁC ÁNH XẠ SONG TUYẾN TÍNH NỬA LIÊN TỤC

### 1. Các ánh xạ song tuyến tính liên tục riêng

Cho $E, F, G$ là ba không gian lồi địa phương. Với mọi ánh xạ song tuyến tính $u$ từ $E \times F$ vào $G$, và với mọi $x \in E$ (tương ứng $y \in F$), ta ký hiệu bởi $u(x, .)$ (tương ứng $u(., y)$) ánh xạ $y \mapsto u(x, y)$ (tương ứng $x \mapsto u(x, y)$) từ $F$ vào $G$ (tương ứng từ $E$ vào $G$).

#### Định nghĩa 1 {#evt-iii-s5-def-1 .statement}

*Một ánh xạ song tuyến tính $u$ từ $E \times F$ vào $G$ được gọi là liên tục riêng nếu, với mọi $x \in E$, ánh xạ tuyến tính $u(x, .)$ từ $F$ vào $G$ là liên tục, và với mọi $y \in F$, ánh xạ tuyến tính $u(., y)$ từ $E$ vào $G$ là liên tục.*

Mệnh đề sau suy ra ngay lập tức từ định nghĩa.

#### Mệnh đề 1 {#evt-iii-s5-prop-1 .statement}

*Để một ánh xạ song tuyến tính $u$ từ $E \times F$ vào $G$ là liên tục riêng, cần và đủ rằng với mọi $y \in F$, ánh xạ tuyến tính $u(., y)$ từ $E$ vào $G$ là liên tục và ánh xạ tuyến tính $y \mapsto u(., y)$ từ $F$ vào $\mathcal{L}_s(E; G)$ là liên tục.*

Ta cũng có thể nói rằng, với mỗi ánh xạ tuyến tính $v \in \mathcal{L}(F; \mathcal{L}_s(E; G))$ được liên kết với ánh xạ song tuyến tính $(x, y) \mapsto v(y)(x)$, ta định nghĩa một song ánh tuyến tính từ $\mathcal{L}(F; \mathcal{L}_s(E; G))$ lên không gian vectơ các ánh xạ song tuyến tính liên tục riêng từ $E \times F$ vào $G$.

Một ánh xạ song tuyến tính liên tục riêng từ $E \times F$ vào $G$ không nhất thiết liên tục trên $E \times F$ (III, p. 47, Bài tập 2; xem thêm III, p. 30, và IV, p. 26, Định lý 2).

Khái niệm về một dạng song tuyến tính liên tục riêng rẽ trên một tích $E_1 \times E_2$ của hai không gian lồi địa phương liên hệ trực tiếp với khái niệm về một ánh xạ tuyến tính liên tục khi $E_1$ và $E_2$ được trang bị các tôpô *yếu* (II, p. 42), Giả sử rằng $(E_1, F_1)$ và $(E_2, F_2)$ là hai cặp không gian vectơ thực (tương ứng phức) ở đối ngẫu tách biệt (*loc. cit.*); ta gán cho $E_i$ (tương ứng $F_i$) tôpô yếu $\sigma(E_i, F_i)$ (tương ứng $\sigma(F_i, E_i)$) với $i = 1, 2$, và ký hiệu $B(E_1, E_2)$ là không gian vectơ của các dạng song tuyến tính *liên tục* trên $E_1 \times E_2$. Áp dụng mệnh đề 1 cho trường hợp $G = K$, ta thấy rằng, với mọi dạng song tuyến tính $\Phi \in B(E_1, E_2)$ và mọi $x_2 \in E_2$, ánh xạ $x_1 \mapsto \Phi(x_1, x_2)$ là một dạng tuyến tính liên tục trên $E_1$, do đó (II, p. 43, mệnh đề 3) tồn tại một và chỉ một phần tử $^d\Phi(x_2) \in F_1$ sao cho

$$
\Phi(x_1, x_2) = \langle x_1, ^d\Phi(x_2) \rangle
$$

với mọi $x_1 \in E_1$ và $x_2 \in E_2$; hơn nữa, ánh xạ $^d\Phi : E_2 \to F_1$ là tuyến tính và *liên tục* đối với các tôpô (yếu) của $E_2$ và của $F_1$.

Ngược lại, với mọi ánh xạ tuyến tính *liên tục* $u : E_2 \to F_1$ ánh xạ $(x_1, x_2) \mapsto \Phi(x_1, x_2) = \langle x_1, u(x_2) \rangle$ là một dạng song tuyến tính liên tục riêng rẽ trên $E_1 \times E_2$, và ta có $u = {}^d \Phi$. Vì vậy ta đã định nghĩa một đẳng cấu $d : \Phi \mapsto {}^d \Phi$ từ $B(E_1, E_2)$ lên $\mathcal{L}(E_2; F_1)$, được gọi là *chính tắc*. Tương tự, công thức

$$
\Phi(x_1, x_2) = \langle {}^s \Phi(x_1), x_2 \rangle
$$

định nghĩa một đẳng cấu *chính tắc* $s : \Phi \to {}^s \Phi$ từ $B(E_1, E_2)$ lên $\mathcal{L}(E_1, F_2)$; hiển nhiên ta có biểu đồ giao hoán

$$
\begin{array}{ccc}
& B(E_1, E_2) & \\
s & / & d \\
\downarrow & & \downarrow \\
\mathcal{L}(E_1; F_2) & \leftrightarrow & \mathcal{L}(E_2; F_1)
\end{array}
$$

trong đó $t$ là đẳng cấu của phép chuyển vị (II, p. 46, mệnh đề 5 và hệ quả). Xét theo định nghĩa các tôpô yếu trên $F_1$ và $F_2$, hiển nhiên rằng khi $B(E_1, E_2)$, $\mathcal{L}(E_1; E_2)$ và $\mathcal{L}(E_2; F_1)$ được trang bị *tôpô hội tụ đơn*, *các đẳng cấu của biểu đồ (3) là các đẳng cấu không gian vectơ tôpô*.

### 2. Các ánh xạ song tuyến tính liên tục riêng rẽ trên một tích của các không gian Fréchet

#### Mệnh đề 2 {#evt-iii-s5-prop-2 .statement}

*Cho E, F và G là ba không gian lồi địa phương. Giả sử E và F là mêtric hóa được và E là một không gian đầy thùng. Cho H là một tập hợp các ánh xạ song tuyến tính liên tục riêng rẽ từ E × F vào G. Giả sử rằng với mọi $x \in E$, tập hợp các ánh xạ $u(x, .)$ từ F vào G, khi u chạy qua H, là đều liên tục. Khi đó H là đều liên tục.*

Cho $U_n$ (resp. $V_n$) là một dãy cơ bản các lân cận của 0 trong E (resp. F). Nếu H không đều liên tục, thì tồn tại một lân cận W của 0 trong G, đóng, lồi, cân bằng, sao cho với mọi $n$, $H(U_n \times V_n)$ không được chứa trong W. Khi đó tồn tại một dãy các cặp $(x_n, y_n) \in U_n \times V_n$, và một dãy $(u_n)$ gồm các phần tử của H, sao cho $u_n(x_n, y_n) \notin W$. Đặt $p$ là gauge của W. Với mọi $y \in F$ và mọi $u \in H$, ánh xạ $u(., y)$ từ E vào G là liên tục, do đó $p \circ u(., y)$ là một nửa chuẩn liên tục trên E. Mặt khác, với mọi $x \in E$, tập các ánh xạ $u(x, .)$ với $u \in H$ là đều liên tục; vì dãy $(y_n)$ tiến tới 0, nên nó bị chặn, và tập tất cả các $u(x, y_n)$, với $n \geq 0$ và $u \in H$, là bị chặn (III, p. 22, mệnh đề 9). Suy ra rằng hàm $p'(x) = \sup_{\substack{u \in H \\ n \geq 0}} p(u(x, y_n))$ là một nửa chuẩn nửa liên tục dưới (hữu hạn) trên E. Vì E là đầy thùng, nên $p'$ là liên tục (III, p. 24, hệ quả). Vì $(x_n)$ tiến tới 0 trong E, nên $p'(x_n)$ tiến tới 0, do đó ta có $p'(x_n) \leq 1$ nếu $n$ đủ lớn; nhưng khi đó $p(u_n(x_n, y_n)) \leq p'(x_n) \leq 1$, suy ra $u_n(x_n, y_n) \in W$, mâu thuẫn với giả thiết về $u_n, x_n, y_n$.

#### Hệ quả 1 {#evt-iii-s5-prop-2-cor-1 .statement}

— Cho E và F là hai không gian Fréchet, và G là một không gian lồi địa phương. Mọi ánh xạ song tuyến tính liên tục riêng rẽ từ $E \times F$ vào G đều liên tục.

Thực vậy, mọi không gian Fréchet đều đầy thùng (III, p. 25, hệ quả).

Cho E và F là hai không gian lồi địa phương. Ta dùng ký hiệu $\mathcal{B}(E, F)$ để chỉ không gian các dạng song tuyến tính liên tục trên $E \times F$, với tôpô hội tụ đều trên các tập có dạng $A \times B$, trong đó A (resp. B) bị chặn trong E (resp. F). Công thức
$$
u(x, y) = \langle y, \phi(u)(x) \rangle
$$
(với $x \in E, y \in F$ và $u \in \mathcal{B}(E, F)$) định nghĩa một ánh xạ tuyến tính đơn ánh liên tục $\phi$ từ $\mathcal{B}(E, F)$ vào $\mathcal{L}_b(E; F'_b)$.

#### Hệ quả 2 {#evt-iii-s5-prop-2-cor-2 .statement}

— Giả sử E và F là khả metrizable và E là đầy thùng. Khi đó $\phi$ là một đẳng cấu không gian vectơ tôpô từ $\mathcal{B}(E, F)$ lên $\mathcal{L}_b(E; F'_b)$.

Cho $f \in \mathcal{L}_b(E; F'_b)$. Đặt $u(x, y) = \langle y, f(x) \rangle$ với $x \in E$ và $y \in F$. Dạng song tuyến tính $u$ trên $E \times F$ là liên tục riêng rẽ; theo mệnh đề 2, nó thuộc $\mathcal{B}(E, F)$, và ta có $f = \phi(u)$. Vậy $\phi$ là một song ánh tuyến tính từ $\mathcal{B}(E, F)$ lên $\mathcal{L}_b(E; F'_b)$. Hiển nhiên $\phi$ là song liên tục, do đó suy ra hệ quả 2.

### 3. Các ánh xạ song tuyến tính nửa liên tục

Trong phần sau, ta sẽ định nghĩa một khái niệm trung gian giữa khái niệm của một ánh xạ song tuyến tính liên tục và khái niệm của một ánh xạ song tuyến tính liên tục riêng rẽ.

#### Mệnh đề 3 {#evt-iii-s5-prop-3 .statement}

— Cho E, F, G là ba không gian lồi địa phương, $\mathfrak{S}$ là một họ các tập con bị chặn của E. Cho u là một ánh xạ song tuyến tính liên tục riêng rẽ từ $E \times F$ vào G. Các tính chất sau là tương đương :

a) Với mọi lân cận W của 0 trong G và mọi tập $M \in \mathfrak{S}$, tồn tại một lân cận V của 0 trong F sao cho $u(M \times V) \subset W$.

b) Với mọi tập $M \in \mathfrak{S}$, ảnh của M qua ánh xạ $x \mapsto u(x, .)$ là một tập con đều liên tục của $\mathcal{L}(F; G)$.

c) Ánh xạ $y \mapsto u(., y)$ từ F vào $\mathcal{L}_{\mathfrak{S}}(E; G)$ là liên tục.

a) biểu thị rằng $y \mapsto u(., y)$ là liên tục tại điểm 0, do định nghĩa các lân cận của 0 trong $\mathcal{L}_{\mathfrak{S}}(E; G)$ (III, p. 13); tương tự a) biểu thị rằng ảnh của M qua ánh xạ $x \mapsto u(x, .)$ là đẳng liên tục tại điểm 0 (III, p. 16).

#### Định nghĩa 2 {#evt-iii-s5-def-2 .statement}

— Cho u là một ánh xạ song tuyến tính từ $E \times F$ vào G. Ta nói u là $\mathfrak{S}$-hypocontinuous nếu u liên tục riêng rẽ và nếu nó thỏa một trong các điều kiện tương đương a), b), c) của mệnh đề 3.

Điều kiện c) của mệnh đề 3 cho thấy khái niệm ánh xạ song tuyến tính $\mathfrak{S}$-hypocontinuous chỉ phụ thuộc vào $\mathfrak{S}$ qua $\mathfrak{S}$-tôpô trên $\mathcal{L}(E, G)$.

Với mỗi tập $\mathfrak{T}$ các tập con bị chặn của F, ta cũng định nghĩa khái niệm ánh xạ $\mathfrak{T}$-hypocontinuous, bằng cách đổi chỗ vai trò của E và F trong mệnh đề 3. Một ánh xạ song tuyến tính u liên tục riêng rẽ được gọi là $(\mathfrak{S}, \mathfrak{T})$-hypocontinuous nếu nó vừa là $\mathfrak{S}$-hypocontinuous vừa là $\mathfrak{T}$-hypocontinuous.

Mọi ánh xạ song tuyến tính *liên tục* từ $E \times F$ vào $G$ đều là $(\mathcal{S}, \mathcal{T})$-hypocontinuous đối với mọi cặp $(\mathcal{S}, \mathcal{T})$ các tập hợp tập con bị chặn : với mọi lân cận $W$ của 0 trong $G$, tồn tại một lân cận $U$ của 0 trong $E$ và một lân cận $V$ của 0 trong $F$ sao cho $u(U \times V) \subset W$; vì mọi tập $M \in \mathcal{S}$ đều bị chặn, tồn tại $\lambda > 0$ sao cho $\lambda M \subset V$, và do đó

$$
u(M \times \lambda V) = u(\lambda M \times V) \subset u(U \times V) \subset W .
$$

Mệnh đề đảo lại nói chung là sai (III, p. 47, Bài tập 3).

#### Mệnh đề 4 {#evt-iii-s5-prop-4 .statement}

*Cho $u$ là một ánh xạ song tuyến tính $\mathcal{S}$-hypocontinuous từ $E \times F$ vào $G$. Với mọi tập $M \in \mathcal{S}$, hạn chế của $u$ lên $M \times F$ là liên tục, và $u(M \times Q)$ bị chặn trong $G$ với mọi tập con bị chặn $Q$ của $F$.*

Mệnh đề đầu tiên suy ra từ hệ quả 3 của GT, X, § 2, No. 1. Cho $W$ là một lân cận của 0 trong $G$; theo giả thiết, tồn tại một lân cận $V$ của 0 trong $F$ sao cho $u(M \times V) \subset W$. Vì tồn tại $\lambda \neq 0$ sao cho $\lambda Q \subset V$, ta có $\lambda u(M \times Q) = u(M \times \lambda Q) \subset W$, và điều này chứng minh phần thứ hai của mệnh đề.

#### Mệnh đề 5 {#evt-iii-s5-prop-5 .statement}

*Cho $u$ là một ánh xạ song tuyến tính $(\mathcal{S}, \mathcal{T})$-hypocontinuous từ $E \times F$ vào $G$. Với mọi cặp tập $M \in \mathcal{S}$, $N \in \mathcal{T}$, $u$ liên tục đều trên $M \times N$.*

Mệnh đề này suy ra ngay từ mệnh đề 2 của GT, X, § 2, No. 1 và mệnh đề 5 của GT, X, § 2, No. 2.

#### Mệnh đề 6 {#evt-iii-s5-prop-6 .statement}

*Nếu $F$ là một không gian barrelled, thì mọi ánh xạ song tuyến tính liên tục riêng phần $u$ từ $E \times F$ vào một không gian lồi địa phương $G$ đều là $\mathcal{S}$-hypocontinuous đối với mọi tập hợp $\mathcal{S}$ của các tập con bị chặn của $E$.*

Nói cách khác, *ánh xạ tuyến tính* $y \mapsto u(., y)$ từ $F$ vào $\mathcal{L}_b(E; G)$ *là liên tục*.

Đủ (III, p. 30, mệnh đề 3) để chứng minh rằng ảnh của mọi tập con bị chặn $M$ của $E$ qua $x \mapsto u(x, .)$ là đều liên tục trong $\mathcal{L}(F; G)$. Nhưng, nhờ mệnh đề 1 (III, p. 28) ảnh này là một tập con bị chặn đơn của $\mathcal{L}(F; G)$, và vì $F$ là barrelled, mọi tập con bị chặn đơn của $\mathcal{L}(F; G)$ đều đều liên tục (III, p. 25, định lý 1).

#### Nhận xét {#evt-iii-s5-n3-rem-1 .statement}

— Giả sử tôpô của $F$ là tôpô lồi địa phương mạnh nhất trên $F$ sao cho các ánh xạ tuyến tính $h_\alpha : F_\alpha \to F$ liên tục (II, p. 27). Khi đó điều kiện *c)* của mệnh đề 3 (III, p. 30) cho thấy rằng nếu $E$ và $G$ là lồi địa phương, thì ánh xạ song tuyến tính $u : E \times F \to G$ là $\mathcal{S}$-hypocontinuous khi và chỉ khi mỗi một trong các ánh xạ song tuyến tính

$$
(x, y_\alpha) \mapsto u(x, h_\alpha(y_\alpha))
$$

từ $E \times F_\alpha$ vào $G$ là $\mathcal{S}$-hypocontinuous.

Bây giờ giả sử rằng $E$ là một không gian lồi địa phương, là giới hạn quy nạp *ngặt* của một dãy tăng $(E_n)$ các không gian con vectơ đóng của $E$ (II, p. 33); khi đó mọi tập hợp $M \in \mathcal{S}$ đều được chứa trong một trong các $E_n$ và bị chặn trong không gian con này (III, p. 5, mệnh đề 6). Ký hiệu $\mathcal{S}_n$ là họ tất cả các tập con thuộc $\mathcal{S}$ được chứa trong $E_n$.

Điều kiện a) của mệnh đề 3 (III, p. 30) cho thấy rằng để một ánh xạ song tuyến tính $u : E \times F \to G$ là $\mathfrak{S}$-hypocontinuous, cần và đủ rằng mỗi một trong các hạn chế $u_n : E_n \times F \to G$ của $u$ là $\mathfrak{S}_n$-hypocontinuous.

### 4. Mở rộng của một ánh xạ song tuyến tính hypocontinuous

#### Mệnh đề 7 {#evt-iii-s5-prop-7 .statement}

*Cho* $E, F, G$ *là ba không gian lồi địa phương*, $G$ *được giả sử Hausdorff*; *cho* $E_0$ *(tương ứng* $F_0$ *) là một không gian con vectơ trù mật của* $E$ *(tương ứng* $F$*). Cho* $u$ *là một ánh xạ song tuyến tính liên tục riêng phần từ* $E \times F$ *vào* $G$.

1) *Nếu* $u(E_0 \times F_0) = \{0\}$, *thì* $u = 0$.

2) *Cho* $\mathfrak{S}_0$ *là một họ các tập con bị chặn của* $E_0$; *nếu hạn chế của* $u$ *lên* $E_0 \times F_0$ *là* $\mathfrak{S}_0$*-hypocontinuous thì* $u$ *cũng vậy*.

1) Theo giả thiết, với mọi $x \in E_0$, ánh xạ tuyến tính liên tục $u(x, .)$ bằng không trên $F_0$, do đó trên $F$: vì vậy với mọi $y \in F$, ánh xạ tuyến tính liên tục $u(., y)$ bằng không trên $E_0$, do đó trên $E$. Điều này chứng tỏ rằng $u = 0$.

2) Với mọi lân cận đóng $W$ của $0$ trong $G$ và với mọi tập hợp $M \in \mathfrak{S}_0$, theo giả thiết, tồn tại một lân cận $V$ của $0$ trong $F_0$ sao cho $u(M \times V) \subset W$. Nhưng $\overline{V}$ là một lân cận của $0$ trong $F$; với mọi $x \in M$, quan hệ $u(\{x\} \times V) \subset W$ suy ra rằng $u(\{x\} \times \overline{V}) \subset W$, vì $u(x, .)$ liên tục và $W$ là đóng; do đó $u(M \times \overline{V}) \subset W$, điều này chứng tỏ rằng $u$ là $\mathfrak{S}_0$*-giả liên tục.

#### Mệnh đề 8 {#evt-iii-s5-prop-8 .statement}

*Cho* $E, F, G$ *là ba không gian lồi địa phương*; *giả sử* $G$ *là Hausdorff và đầy đủ từng phần*. *Cho* $E_0$ *(tương ứng $F_0$) là một không gian con vectơ trù mật của* $E$ *(tương ứng $F$), $\mathfrak{S}_0$ *(tương ứng $\mathfrak{T}_0$) là một họ các tập con bị chặn của* $E_0$ *(tương ứng $F_0$) sao cho mọi điểm của* $E$ *(tương ứng $F$) đều nằm trong bao đóng của một phần tử của* $\mathfrak{S}_0$ *(tương ứng $\mathfrak{T}_0$). Khi đó mọi ánh xạ song tuyến tính $(\mathfrak{S}_0, \mathfrak{T}_0)$*-giả liên tục* $u$ *từ* $E_0 \times F_0$ *vào* $G$ *đều mở rộng duy nhất thành một ánh xạ song tuyến tính liên tục riêng* $\overline{u}$ *từ* $E \times F$ *vào* $G$ *và* $\overline{u}$ *là* $(\mathfrak{S}_0, \mathfrak{T}_0)$*-giả liên tục*.

Tính duy nhất và tính nửa liên tục của $\overline{u}$ suy ra từ mệnh đề 7; còn phải chứng minh sự tồn tại của $\overline{u}$. Với mọi $y' \in F_0$, ánh xạ tuyến tính liên tục $x' \mapsto u(x', y')$ từ $E_0$ vào $G$ được mở rộng duy nhất thành một ánh xạ tuyến tính liên tục $x \mapsto u_1(x, y')$ từ $E$ vào $G$ (III, p. 8, mệnh đề 10). Suy ra ngay rằng với mọi $x \in E$, ánh xạ $y' \mapsto u_1(x, y')$ từ $F_0$ vào $G$ là tuyến tính; và ta sẽ chứng minh nó liên tục. Theo giả thiết, tồn tại $M \in \mathfrak{S}_0$, sao cho $x \in \overline{M}$. Với mọi lân cận đóng $W$ của 0 trong $G$, theo giả thiết, tồn tại một lân cận $V$ của 0 trong $F_0$ sao cho $u(M \times V) \subset W$; vì $x \mapsto u_1(x, y')$ là liên tục, ta suy ra rằng $u_1(\overline{M} \times V) \subset W$, và đặc biệt $u_1(x, y') \in W$ với mọi $y' \in V$. Điều này thiết lập mệnh đề của chúng ta. Nhờ mệnh đề 7, ánh xạ song tuyến tính $u_1$ từ $E \times F_0$ vào $G$ là $(\mathfrak{S}_0, \mathfrak{T}_0)$*-nửa liên tục. Ta kết thúc chứng minh bằng cách đổi chỗ vai trò của $E$ và $F$ trong phần đầu của chứng minh, áp dụng cho $u_1$.

### 5. Tính nửa liên tục của ánh xạ $(u, v) \mapsto v \circ u$

#### Mệnh đề 9 {#evt-iii-s5-prop-9 .statement}

*Cho* $R, S, T$ *là ba không gian Hausdorff lồi địa phương*. *Giả sử rằng các không gian* $\mathcal{L}(R; S), \mathcal{L}(S; T), \mathcal{L}(R; T)$ *mỗi không gian được gán tôpô hội tụ đơn* (resp. *compact*, *bị chặn*). *Khi đó ánh xạ song tuyến tính* $(u, v) \mapsto v \circ u$ *từ* $\mathcal{L}(R; S) \times \mathcal{L}(S; T)$ *vào* $\mathcal{L}(R; T)$ *là* $(\mathfrak{S}, \mathfrak{T})$-*nửa liên tục*, *trong đó* $\mathfrak{T}$ *là họ các tập con đẳng liên tục của* $\mathcal{L}(S; T)$, *và* $\mathfrak{S}$ *là họ các tập con hữu hạn* (resp. *compact, bị chặn*) *của* $\mathcal{L}(R; S)$.

Trước hết ta chứng minh rằng $(u, v) \mapsto v \circ u$ là $\mathfrak{T}$-nửa liên tục. Cho H là một tập đẳng liên tục trong $\mathcal{L}(S; T)$, cho W là một lân cận của 0 trong T và cho M là một tập con hữu hạn (resp. compact, bị chặn) của R. Ta phải chứng minh rằng tồn tại một lân cận V của 0 trong S sao cho nếu $u(M) \subset V$ và $v \in H$, thì $v(u(M)) \subset W$. Nhưng để làm điều này, chỉ cần có $v(V) \subset W$ với mọi $v \in H$, và sự tồn tại của một lân cận như vậy suy ra từ tính đẳng liên tục của H.

Để thấy rằng $(u, v) \mapsto v \circ u$ là $S$-hypocontinuous, ta sẽ chứng minh rằng, với mọi lân cận W của 0 trong T, mọi tập con hữu hạn (tương ứng compact, bị chặn) M của R và mọi tập con hữu hạn (tương ứng compact, bị chặn) L của $\mathcal{L}(R; S)$ tồn tại một tập con hữu hạn (tương ứng compact, bị chặn) N của S sao cho các quan hệ $v(N) \subset W$ và $u \in L$ kéo theo $v(u(M)) \subset W$. Hiển nhiên chỉ cần chỉ ra rằng ta có thể lấy $N = \bigcup_{u \in L} u(M)$, *tức là* tập N là hữu hạn (tương ứng compact, bị chặn) bất cứ khi nào L và M như vậy. Điều này là hiển nhiên nếu L và M hữu hạn, hoặc nếu M bị chặn trong R và L bị chặn trong $\mathcal{L}(R; S)$ (đối với tôpô của hội tụ bị chặn, *xem* III, p. 22). Cuối cùng, ta chứng minh rằng nếu M là compact trong R và L là compact trong $\mathcal{L}(R; S)$ đối với tôpô của hội tụ compact, thì N là compact trong S. Nhưng nếu $u_M$ là hạn chế trên M của $u \in L$, thì ánh xạ $u \mapsto u_M$ từ L vào không gian $\mathcal{C}(M; S)$ của mọi ánh xạ liên tục từ M vào S, với tôpô của hội tụ đều, là liên tục; do đó ảnh của L qua ánh xạ này là compact, và mệnh đề của chúng ta suy ra từ tính liên tục của ánh xạ $(w, x) \mapsto w(x)$ từ $\mathcal{C}(M; S) \times M$ vào S (GT, X, § 1, No. 6, mệnh đề 9).

Trong hai hệ quả sau đây, ta giả sử như trong mệnh đề 9, rằng các không gian $\mathcal{L}(R; S)$, $\mathcal{L}(S; T)$, $\mathcal{L}(R; T)$ đều được trang bị hoặc cả ba tôpô của hội tụ đơn, hoặc cả ba tôpô của hội tụ compact, hoặc cả ba tôpô của hội tụ bị chặn.

#### Hệ quả 1 {#evt-iii-s5-prop-9-cor-1 .statement}

*Với mọi tập con đều liên tục H của* $\mathcal{L}(S; T)$ *ánh xạ* $(u, v) \mapsto v \circ u$ *từ* $\mathcal{L}(R; S) \times H$ *vào* $\mathcal{L}(R; T)$ *là liên tục*.

Điều này suy ra ngay từ mệnh đề 9 (III, p. 32) và 4 (III, p. 31).

#### Hệ quả 2 {#evt-iii-s5-prop-9-cor-2 .statement}

*Giả sử S là barrelled. Nếu dãy* $(u_n)$ *tiến tới u trong* $\mathcal{L}(R; S)$ *và dãy* $(v_n)$ *tiến tới v trong* $\mathcal{L}(S, T)$, *thì dãy* $(v_n \circ u_n)$ *tiến tới* $v \circ u$ *trong* $\mathcal{L}(R; T)$.

Thật vậy, dãy $(v_n)$, vì chỉ bị chặn trong $\mathcal{L}(S; T)$, là đều liên tục, bởi S là barrelled (III, p. 25, định lý 1); do đó hệ quả này suy ra từ hệ quả 1.

### Bài tập {#evt-iii-s5-exercises}
