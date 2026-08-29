---
book: alg
book_title: Algebra
chapter: IX
chapter_title: Formes sesquilinéaires et formes quadratiques
section: 2
section_title: Discriminant d'une forme sesquilinéaire
lang: vi
source: alg-ix-fr
pdf_pages: 0039-0047
extraction: ocr
statements: 12
exercises: 0
content_sha256: af3d2703c08d110b9cc82b0984b91f57ad14f7b65ecb0f55c3ed63f765d2081b
translated_from: content/en-mt/alg/IX/02_s2_discriminant_d_une_forme_sesquilineaire.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 74216b1983a14730e4a90fe3ef714c5d502c977a67246ee11dfa0177303bbb68
translation_model: gpt-5-mini, gpt-5-6
translation_run: translate-vi-80128cb7
glossary_version: 34
glossary_terms_sha256: 47310e2c64bfea1558b6892aa6ae9c173cdd5c29b3fd9b73435a44576651776c
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 2. ĐỊNH THỨC CỦA MỘT DẠNG NỬA SONG TUYẾN TÍNH

ví dụ $A = \mathbf{F}_p(X)$, trong đó $p$ là nguyên tố ; $E'' = A'' \otimes_A E$ khi đó là một không gian vectơ có cùng chiều trên $A''$ với $E$ trên $A$; xét ánh xạ $M \to A'' \otimes_A M$.

c) Giả sử $A' = A$. Cho $\omega$ là một ánh xạ song ánh từ $\mathfrak{F}(E)$ lên tập hợp $\mathfrak{F}'(E')$ các không gian con có đối chiều hữu hạn của $E'$, sao cho $\operatorname{codim} \omega(M) = \dim M$, và $\omega(M + N) = \omega(M) \cap \omega(N)$. Chứng minh rằng tồn tại một dạng nửa song tuyến tính $\Phi$ trên $E \times E'$, không suy biến phải, và sao cho $\omega(M) = M^0$ với mọi $M \in \mathfrak{F}(E)$. (Dùng Định lý 1 của Chương II, § 4, No. 6).

¶ 11) a) Cho $A$ là một vành Artin trái và phải (Chương VIII, § 2, No. 3). Chứng minh rằng các điều kiện sau là tương đương: 1° linh tử phải (tương ứng linh hóa tử trái) của mọi iđêan trái (tương ứng iđêan phải) $\neq A$ không rút gọn về 0 ; 2° đối ngẫu của mọi $A$-môđun đơn trái (tương ứng phải) không rút gọn về 0 ; 3° đối ngẫu của mọi $A$-môđun trái (tương ứng phải) kiểu hữu hạn không rút gọn về 0. Một vành $A$ được gọi là thỏa mãn điều kiện $(N_s)$ (tương ứng $(N_d)$) nếu nó thỏa mãn các điều kiện này đối với các $A$-môđun trái (tương ứng phải).

b) Cho $A$ là một vành Artin trái và phải thỏa mãn điều kiện $(N_d)$, $E$ (tương ứng $F$) là một $A$-môđun trái (tương ứng phải) tự do, có một cơ sở đếm được trên $A$, $\Phi$ là một dạng song tuyến tính trên $E \times F$ sao cho $s_\Phi$ là đơn ánh. Cho $M$ là một môđun con tự do của $E$; chứng minh rằng tồn tại một môđun con tự do $N$ của $F$ và một cơ sở $(e_n)$ (tương ứng $(f_n)$) của $M$ (tương ứng $N$) sao cho $\Phi(e_i, f_j) = \delta_{ij}$; hơn nữa có thể chọn $e_1$ là bất kỳ phần tử tự do nào của $M$. (Chú ý rằng nếu $x$ là một phần tử tự do của $M$, ảnh của $F$ qua ánh xạ $y \to \Phi(x, y)$ là chính vành $A$; khi đó dùng quy nạp để xây dựng các cơ sở $(e_n)$ và $(f_n)$). Suy ra rằng nếu cơ sở $(e_n)$ của $M$ là hữu hạn, $E$ là tổng trực tiếp của $M$ và $N^0$, và ta có $M^{00} = M$.

c) Giữ các giả thiết của b), và giả sử thêm rằng $A$ thỏa mãn điều kiện $(N_s)$ và rằng $d_\Phi$ là đơn ánh. Chứng minh rằng tồn tại một cơ sở $(e_n)$ trong $E$ và một cơ sở $(f_n)$ trong $F$ sao cho $\Phi(e_i, f_j) = \delta_{ij}$. (Dùng b) bằng cách xác định luân phiên $e_n$ và $f_n$ theo phép quy nạp).

*12) Cho $E$ là một không gian Hilbert thực kiểu đếm được, $\Phi(x, y)$ là tích vô hướng trong $E$. Chứng minh rằng không tồn tại một hệ gồm hai cơ sở đại số $(e_\lambda), (f_\mu)$ của không gian vectơ $E$ trên $\mathbf{R}$ sao cho $\Phi(e_\lambda, f_\mu) = \delta_{\lambda \mu}$ đối với mọi cặp chỉ số. (Trước hết nhận xét rằng tập hợp các chỉ số của các cơ sở này sẽ có lũy thừa của continuum ($Esp. vect. top.$, chương II, § 3, exerc. 15)); sau đó xét một cơ sở trực chuẩn (đếm được) $(a_n)$ của $E$ và nhận xét rằng không gian con sinh bởi các $a_n$ được chứa trong không gian con sinh bởi một họ con đếm được của $(e_\lambda)$.*

#### Định nghĩa 1 {#alg-ix-s2-def-1 .statement}

Cho một dạng sesquilinear $\Phi$ đối với $J$ trên $E$ và một hệ $S = (x_1, \ldots, x_n)$ gồm $n$ phần tử của $E$, biệt thức của $\Phi$ đối với hệ này được gọi là, và được ký hiệu bởi $D_\Phi(x_1, \ldots, x_n)$ hoặc $D_\Phi(S)$, phần tử $\det(\Phi(x_i, x_j))$ của $A$.

Nếu $(e_1, \ldots, e_n)$ là một cơ sở của $E$, thì biệt thức của $\Phi$ đối với cơ sở này không gì khác ngoài định thức của ma trận của $\Phi$ đối với cơ sở này.

Từ định nghĩa về mở rộng của $\Phi$ đến $\wedge^n E$ ($§ 1$, no 9) suy ra rằng ta có

$$
D_\Phi(x_1, \ldots, x_n) = \Phi_{(n)}(x_1 \wedge \ldots \wedge x_n, x_1 \wedge \ldots \wedge x_n),
$$

trong đó $\Phi_{(n)}$ ký hiệu mở rộng của $\Phi$ đến $\wedge^n E$. Đối với mọi phép hoán vị $\sigma \in \mathfrak{S}_n$, do đó ta có

$$
D_\Phi(x_{\sigma(1)}, \ldots, x_{\sigma(n)}) = D_\Phi(x_1, x_2, \ldots, x_n).
$$

#### Ví dụ {#alg-ix-s2-n0-exa-1 .statement}

Cho $B$ là một đại số trên vành $A$, sao cho $B$ là một A-môđun tự do có số chiều hữu hạn $n$. Khi đó ánh xạ $(x, y) \to \mathrm{Tr}_{B/A}(xy)$ (Chương VIII, § 12, no 2) là một dạng song tuyến tính trên $B$. Cho một hệ $(x_1, \ldots, x_n)$ gồm $n$ phần tử của $B$, biệt thức của dạng này đối với hệ này được gọi là biệt thức của hệ $(x_1, \ldots, x_n)$ trên $A$, và được ký hiệu bởi $D_{B/A}(x_1, \ldots, x_n)$. Như vậy

$$
D_{B/A}(x_1, \ldots, x_n) = \det (\mathrm{Tr}_{B/A}(x_ix_j)).
$$

#### Nhận xét {#alg-ix-s2-n0-rem-1 .statement}

Cho $(e_1, \ldots, e_n)$ là một cơ sở của $B$ trên $A$, và

$$
e_ie_j = \sum_{k=1}^n c_{ijk}e_k \quad (c_{ijk} \in A)
$$

(chương II, § 7, no 2). Vì ma trận của tự đồng cấu $A$-tuyến tính $x \to e_kx$ của $B$ đối với $(e_r)$ là $(c_{ksr})$, ta có $\mathrm{Tr}_{B/A}(e_k) = \sum_{r=1}^n c_{krr}$, do đó $\mathrm{Tr}_{B/A}(e_ie_j) = \sum_{k,r} c_{ijk}c_{krr}$. Suy ra rằng

$$
D_{B/A}(e_1, \ldots, e_n) = \det_{i,j} (\sum_{k,r} c_{ijk}c_{krr}).
$$

#### Mệnh đề 1 {#alg-ix-s2-prop-1 .statement}

Cho $\Phi$ là một dạng sesqui tuyến tính đối với $J$ trên $E$, $(\tilde{x}_1, \ldots, x_n)$ là một hệ gồm $n$ phần tử của $E$, và $(a_{ij})_{(i,j = 1, \ldots, n)}$ là một họ gồm $n^2$ phần tử của $A$; đặt $y_i = \sum_{i=1}^n a_{ji}x_i$. Khi đó ta có

$$
D_\Phi(y_1, \ldots, y_n) = \det (a_{ij}) \cdot \det (a_{ij})^j \cdot D_\Phi(x_1, \ldots, x_n).
$$

Thật vậy, vì $\Phi$ là một dạng sesqui tuyến tính, ta có $\Phi(y_i, y_j) = \sum_{k,m} a_{ik} \Phi(x_k, x_m) a_{jm}^j$. Do đó, nếu ký hiệu ma trận $(a_{ij})$ là $A$, thì ma trận $(\Phi(y_i, y_j))$ bằng $A . (\Phi(x_i, x_j)). {}^t A^j$. Vì $\det({}^t A) = \det(A)$, và $\det(A^j) = \det(A)^j$, mệnh đề của ta được chứng minh.

Đặc biệt, nếu $(e_i)$ và $(e'_i)$ là hai cơ sở của $E, D$ và $D'$ là các biệt thức của $\Phi$ tương ứng với các cơ sở này, và $a$ là định thức của ma trận chuyển qua từ cơ sở $(e_i)$ sang cơ sở $(e'_i)$, ta có
$$
(4) \qquad D' = aa^j D.
$$

Suy ra từ mệnh đề 1 rằng, nếu $(e_i)$ là một cơ sở của $E$ và $(x_i)$ là một hệ tùy ý gồm $n$ phần tử của $E$, $D_\Phi(e_1, \ldots, e_n)$ *chia hết* $D_\Phi(x_1, \ldots, x_n)$. Đặc biệt các biệt thức của $\Phi$ đối với hai cơ sở bất kỳ của $E$ sinh ra cùng một iđêan chính của $A$.

Cho $(E_i)_{i \in I}$ là một họ hữu hạn các môđun $A$-tự do hữu hạn chiều, $\Phi_i$ là một dạng sesquilinear đối với $J$ trên $E_i$, và $B_i$ là một cơ sở của $E_i$. Nếu $\Phi$ ký hiệu *tổng trực tiếp* của các $\Phi_i$ (§ 1, số 3) và $B$ là cơ sở của $\prod_{i \in I} E_i$ thu được bằng cách ghép các $B_i$, thì hiển nhiên
$$
(5) \qquad D_\Phi(B) = \prod_{i \in I} D_{\Phi_i}(B_i).
$$

Cho $\Phi$ là một dạng sesquilinear đối với $J$ trên $E$, $h$ là một đồng cấu từ $A$ vào một vành giao hoán $A'$, $\Phi'$ là dạng sesquilinear trên $A' \otimes_A E$ thu được bằng mở rộng của $\Phi$ (§ 1, số 4) và $(x_1, \ldots, x_n)$ là một hệ tùy ý các phần tử của $E$. Vì $A' \otimes_A E$ là một $A'$-môđun tự do, $D_{\Phi'}(1 \otimes x_1, \ldots, 1 \otimes x_n)$ được xác định, và ta có hiển nhiên
$$
(6) \qquad D_{\Phi'}(1 \otimes x_1, \ldots, 1 \otimes x_n) = h(D_\Phi(x_1, \ldots, x_n)).
$$

#### Ví dụ {#alg-ix-s2-n0-exa-2 .statement}

Cho $B$ là một đại số trên $A$ là một $A$-môđun tự do có số chiều hữu hạn $n$, $(x_1, \ldots, x_n)$ là một cơ sở của $B$ trên $A$, và $m$ là một iđêan của $A$. Nếu $h$ ký hiệu đồng cấu chính tắc từ $B$ lên $B/mB$, thì $(h(x_1), \ldots, h(x_n))$ là một cơ sở của $B/mB$ trên $A/m$ (chương I, § 6, số 5, mệnh đề 5), và $B/mB$ đẳng cấu với $(A/m) \otimes_A B$. Do đó ta có
$$
D_{(B/mB)/(A/m)}(h(x_1), \ldots, h(x_n)) = h(D_{B/A}(x_1, \ldots, x_n)).
$$

#### Mệnh đề 2 {#alg-ix-s2-prop-2 .statement}

Giả sử rằng $A$ là một miền nguyên. Cho $\Phi$ là một dạng sesquilinear đối với $J$ trên $E$ và $(e_1, \ldots, e_n)$ là một cơ sở của $E$, sao cho $D_\Phi(e_1, e_2, \ldots, e_n) \neq 0$.

a) Để một hệ $(x_1, \ldots, x_n)$ gồm $n$ phần tử của $E$ là tự do, điều kiện cần và đủ là $D_\Phi(x_1, \ldots, x_n)$ phải là $\neq 0$.

b) Để một hệ $(x_1, \ldots, x_n)$ gồm $n$ phần tử của $E$ là một cơ sở của $E$, điều kiện cần và đủ là $D_\Phi(x_1, \ldots, x_n)$ và $D_\Phi(e_1, \ldots, e_n)$ là các phần tử liên kết trong $A$ (xem Chương VI, § 1, No. 5).

Cho $x_j = \sum_{i=1}^n a_{ji} e_i$ ($a_{ji} \in A$). Trước hết ta chứng minh a). Nếu $D_\Phi(x_1, \ldots, x_n) = 0$, ta có $\det(a_{ji}) \cdot \det(a_{ji})' = 0$ (Mệnh đề 1) vì $D_\Phi(e_1, \ldots, e_n) \neq 0$ và $A$ là nguyên; do đó ta có $\det(a_{ji}) = 0$, và các vectơ $x_j$ phụ thuộc tuyến tính (Chương III, § 7, No. 1, Định lý 1, áp dụng cho không gian vectơ $K \otimes_A E$, trong đó $K$ là trường các phân thức của $A$). Đảo lại, nếu các vectơ này phụ thuộc tuyến tính thì ta có $\det(a_{ji}) = 0$ (*ibid.*), do đó $D_\Phi(x_1, \ldots, x_n) = 0$ (Mệnh đề 1).

Bây giờ ta chứng minh b). Nếu $D_\Phi(x_1, \ldots, x_n)$ và $D_\Phi(e_1, \ldots, e_n)$ liên kết trong $A$, Mệnh đề 1 chỉ ra rằng $\det(a_{ij}) \cdot \det(a_{ij})'$ là khả nghịch trong $A$. Do đó $\det(a_{ij})$ tự nó là khả nghịch trong $A$; vì thế ma trận $(a_{ij})$ trên $A$ là khả nghịch (Chương III, § 6, No. 5, Định lý 2), và tự đồng cấu $g$ của $E$ được xác định bởi $g(e_i) = x_i$ ($i = 1, \ldots, n$) là một tự đẳng cấu; do đó $(x_1, \ldots, x_n)$ là một cơ sở của $E$. Đảo lại suy ra ngay lập tức từ Mệnh đề 1.

#### Mệnh đề 3 {#alg-ix-s2-prop-3 .statement}

Cho $\Phi$ là một dạng sesquilinear đối với $J$ trên $E$, và cho $S$ là một cơ sở của $E$. Các điều kiện sau là tương đương:

a) Ánh xạ $s_\Phi$ từ $E$ vào $E^*$ liên kết với $\Phi$ là song ánh.

b) Ánh xạ $d_\Phi$ từ $E$ vào $E^*$ liên kết với $\Phi$ là song ánh.

c) Phần tử $D_\Phi(S)$ là khả nghịch trong $A$.

Thật vậy điều kiện c) biểu thị rằng ma trận của $\Phi$ đối với $S$ là khả nghịch (Chương III, § 6, No. 5, Định lý 2). Do đó c) tương đương với a) ($§ 1,$ No. 10); tương tự c) tương đương với b).

#### Mệnh đề 4 {#alg-ix-s2-prop-4 .statement}

Giả sử rằng $A$ là nguyên. Cho $S$ là một cơ sở của $E$. Điều kiện cần và đủ để một dạng sesquilinear $\Phi$ trên $E$ là không suy biến là có $D_\Phi(S) \neq 0$.

Quả vậy, đặt K là trường các phân thức của A, và gọi $\Phi'$ là mở rộng của $\Phi$ lên không gian vectơ trên K $K \otimes_A E$; đồng nhất E với một tập con của không gian vectơ này. Quan hệ $D_{\Phi}(S) \neq 0$ khi đó tương đương với $D_{\Phi'}(S) \neq 0$ (công thức (6)), mà bản thân điều này biểu thị rằng $s_{\Phi'}$ là song ánh (mệnh đề 3), nghĩa là $\Phi'$ không suy biến (§ 1, No. 6, mệnh đề 6). Bây giờ, với mọi $x \in K \otimes_A E$, tồn tại $a \in A$ sao cho $ax \in E$; do đó, để $\Phi$ suy biến, điều kiện cần và đủ là $\Phi'$ cũng suy biến. Điều này chứng minh mệnh đề của chúng ta.

#### Mệnh đề 5 {#alg-ix-s2-prop-5 .statement}

*Cho A là một trường, B là một đại số giao hoán có số chiều hữu hạn n trên A, và S là một cơ sở của B. Để B tách được (chương VIII, § 7, No. 5, định nghĩa 1), điều kiện cần và đủ là phải có* $D_{B/A}(S) \neq 0$.

Quả vậy, đặt $A'$ là bao đóng đại số của A, và gọi $B'$ là đại số $A' \otimes_A B$ trên $A'$. Nếu B tách được, thì $B'$ là nửa đơn (chương VIII, § 7, No. 5, hệ quả của mệnh đề 7) và do đó là tổng trực tiếp của n trường đẳng cấu với $A'$ (chương VIII, § 6, No. 4, hệ quả của mệnh đề 9). Nếu $S'$ ký hiệu cơ sở chính tắc của $B'$ (đồng nhất với ${A'}^n$), thì có $D_{B'/A'}(S') = 1$, do đó $D_{B'/A'}(S) \neq 0$ (mệnh đề 1) và $D_{B/A}(S) \neq 0$ (công thức (6)).

Ngược lại, giả sử rằng có $D_{B/A}(S) \neq 0$. Để chứng minh rằng B tách được, chỉ cần chứng minh rằng $B'$ là nửa đơn, nghĩa là nó không chứa phần tử lũy linh khác không. Bây giờ, nếu $x'$ là một phần tử lũy linh khác không của $B'$, nó có thể được lấy làm phần tử đầu tiên của một cơ sở $S'$ của $B'$, và khi đó ta có $\mathrm{Tr}_{B'/A'}(x'y') = 0$ với mọi $y' \in S'$ vì một tự đồng cấu lũy linh có các trị riêng bằng không (chương VII, § 5, No. 3, hệ quả 3 của mệnh đề 8), và do đó có vết bằng không. Suy ra rằng $D_{B'/A'}(S') = 0$, do đó $D_{B'/A'}(S) = 0$ (mệnh đề 1) và $D_{B/A}(S) = 0$ (công thức (6)), trái với giả thiết.

#### Nhận xét {#alg-ix-s2-n0-rem-2 .statement}

Giả sử rằng B là một trường mở rộng của A. Gọi $S = (x_1, \ldots, x_n)$ là một cơ sở của B, và $(s_1, \ldots, s_n)$ là các A-đẳng cấu của B vào bao đóng đại số $A'$ của A (mỗi $s_j$ được lặp lại $[B : A]_i$ lần). Nhắc lại rằng, với mọi $z \in B$, ta có $\mathrm{Tr}_{B/A}(z) = \sum_{j=1}^n s_j(z)$ (chương VIII, § 12, No. 2, mệnh đề 4).

Từ công thức về phép nhân của các định thức suy ra rằng ta có

$$(7)\quad (\det(s_j(x_i)))^2 = D_{B/A}(x_1, \ldots, x_n).$$

Công thức này chỉ ra rằng Mệnh đề 5 tổng quát hóa điều kiện tách được được cho trong chương V, § 7, No. 2, Nhận xét.

#### Mệnh đề 6 {#alg-ix-s2-prop-6 .statement}

Cho $\Phi$ là một dạng A-song tuyến tính trên E, và K là một vành con của A sao cho A là một K-môđun tự do có số chiều hữu hạn q. Nếu $(e_i)_{i=1,\ldots,n}$ là một cơ sở của E trên A và $(a_j)_{j=1,\ldots,q}$ là một cơ sở của A trên K, thì $(a_j e_i)$ là một cơ sở của E trên K. Ánh xạ $\Phi'$ của $E \times E$ vào K được xác định bởi $\Phi'(x, y) = \mathrm{Tr}_{A/K}(\Phi(x, y))$ là một dạng K-song tuyến tính trên E, và ta có

$$(8)\quad D_{\Phi'}(a_j e_i) = N_{A/K}(D_\Phi(e_1, \ldots, e_n)) \cdot (D_{A/K}(a_1, \ldots, a_q))^n.$$

Hai mệnh đề đầu là hiển nhiên, nên chỉ cần chứng minh (7). Theo định nghĩa, vế thứ nhất là định thức của tự đồng cấu K-tuyến tính $u$ của E được xác định bởi

$$u(a_j e_i) = \sum_{r,s} \mathrm{Tr}_{A/K}(a_j a_r \Phi(e_i, e_s)) a_r e_s.$$

Xét tự đồng cấu A-tuyến tính $v$ của E được xác định bởi $v(e_i) = \sum_s \Phi(e_i, e_s) e_s$, và tự đồng cấu K-tuyến tính $w$ của E được xác định bởi $w(a_j e_i) = (\sum_r \mathrm{Tr}_{A/K}(a_j a_r) a_r) e_i$. Ta có

$$w(v(a_j e_i)) = w(\sum_s a_j \Phi(e_i, e_s) e_s) = \sum_{r,s} \mathrm{Tr}_{A/K}(a_j \Phi(e_i, e_s) a_r) a_r e_s$$

vì $w(a e_s) = \sum_r \mathrm{Tr}_{A/K}(a a_r) a_r e_s$ với mọi $a \in A$; do đó $u$ là ánh xạ hợp thành $w \circ v$. Vì vậy, ký hiệu $v_K$ là ánh xạ $v$ được xem như một ánh xạ K-tuyến tính, ta có $\det(u) = \det(v_K) \det(w)$. Bây giờ $\det(v_K) = N_{A/K}(\det(v))$ (chương VIII, § 12, số 2, mệnh đề 7), và rõ ràng là $\det(v) = D_\Phi(e_1, \ldots, e_n)$. Mặt khác, vì mỗi A-môđun $Ae_i (i = 1, \ldots, n)$ là ổn định đối với $w$, và định thức của hạn chế của $w$ lên $Ae_i$ là $\det(\mathrm{Tr}_{A/K}(a_j a_r)) = D_{A/K}(a_1, \ldots, a_q)$, nên ta có $\det(w) = (D_{A/K}(a_1, \ldots, a_q))^n$. Công thức (8) do đó rút gọn thành $\det(u) = \det(v_K) \det(w)$, một công thức đã được chứng minh ở trên.

#### Hệ quả (« Công thức bắc cầu đối với các biệt thức ») {#alg-ix-s2-n0-cor-1 .statement}

Cho K là một vành giao hoán, A là một đại số giao hoán nhận một cơ sở hữu hạn $(a_j)_{j=1,\ldots,q}$ trên K, và E là một đại số trên A nhận một cơ sở hữu hạn $(e_i)_{i=1,\ldots,n}$. Khi đó $(a_j e_i)$ là một cơ sở của E trên K, và ta có

$$
D_{E/K}(a_j e_i) = N_{A/K}(D_{E/A}(e_1, \ldots, e_n)) \cdot (D_{A/K}(a_1, \ldots, a_q))^n.
$$

Thật vậy, nếu ta đặt $\Phi(x, y) = \operatorname{Tr}_{E/A}(xy)$, thì dạng K-song tuyến tính $\Phi'$ của Mệnh đề 6 là $\Phi'(x, y) = \operatorname{Tr}_{E/K}(xy)$ theo công thức bắc cầu đối với các vết (Chương VIII, § 12, số 2, hệ quả của Mệnh đề 7).

Bài tập. — 1) Cho A là một đại số có hạng hữu hạn trên một trường giao hoán K, có phần tử đơn vị.
   a) Chứng minh rằng nếu căn của A khác không, thì dạng song tuyến tính $(x, y) \to \operatorname{Tr}_{A/K}(xy)$ trên A là suy biến.
   b) Giả sử K có đặc số 0. Chứng minh rằng nếu A là một đại số ma trận $M_n(K)$, S là cơ sở chính tắc của A trên K, thì $D_{A/K}(S) \neq 0$.
   c) Suy ra từ a) và b) rằng, đối với một đại số A có hạng hữu hạn trên một trường K có đặc số 0 để là nửa đơn tuyệt đối, điều kiện cần và đủ là dạng song tuyến tính $(x, y) \to \operatorname{Tr}_{A/K}(xy)$ không suy biến (hoặc, điều tương đương, là $D_{A/K}(S) \neq 0$ với mọi cơ sở S của A trên K).

¶ 2) Cho B là một vành, A là một vành con của B chứa phần tử đơn vị của B; do đó B là một song môđun (A, A); ký hiệu $^sB$ (tương ứng $^dB$) là tập hợp B được xem như một A-môđun trái (tương ứng phải), ký hiệu $^sB^*$ (tương ứng $^dB^*$) là môđun đối ngẫu A bên phải (tương ứng bên trái) của $^sB$ (tương ứng $^dB$). Với mọi $x' \in ^sB^*$ và mọi $b \in B$, $x \to \langle xb, x' \rangle$ là một dạng A-tuyến tính trên $^sB$, do đó là một phần tử của $^sB^*$ được ký hiệu là $bx'$; ánh xạ $(b, x') \to bx'$ xác định trên $^sB^*$ một cấu trúc B-môđun trái (xem chương III, lần xuất bản thứ 2, Phụ lục II, No. 7).
   a) Cho $\varphi$ là một đồng cấu của song môđun (A, A) B vào song môđun (A, A) A; để ánh xạ A-song tuyến tính $\Phi : (x, y) \to \varphi(xy)$ từ $^sB \times ^dB$ vào A là không suy biến, điều kiện cần và đủ là $\varphi(0)$ không chứa iđêan nào (trái hoặc phải) của B phân biệt với $\{0\}$. Khi đó người ta nói rằng $\varphi$ là một đồng cấu Frobenius của B vào A.
   b) Cho $\varphi$ là một đồng cấu Frobenius của B vào A; chứng minh rằng ánh xạ $d_\varphi$ liên kết ở bên phải với $\Phi$ là một đẳng cấu của B-môđun trái $B_s$ lên một môđun con của B-môđun trái $^sB^*$. Chứng minh rằng $d_\varphi$ là song ánh trong mỗi hai trường hợp sau: 1° A là một vành Artin trái và phải thỏa mãn các điều kiện (N_s) và (N_d) (§ 1, bài tập 11), và $^sB$ và $^dB$ là các A-môđun có độ dài hữu hạn (dùng bài tập 11 b) của § 1); 2° A là một vành Artin giao hoán và đối hợp (chương VIII, § 3, bài tập 11), chứa trong tâm của B, và $^sB$ là một A-môđun có độ dài hữu hạn (dùng bài tập 11 của chương VIII, § 3).

c) Ngược lại, chứng minh rằng nếu $B_s$ và $^sB^*$ là đẳng cấu, thì tồn tại một đồng cấu Frobenius từ B vào A khi ta ở trong một trong hai trường hợp đã xét trong b) và $^sB$ và $^dB$ có cùng độ dài (dùng bài tập 11 b) của § 1).

d) Với các giả thiết và ký hiệu của a), chứng minh rằng linh hóa tử phải (tương ứng linh hóa tử trái) của một iđêan trái I (tương ứng của một iđêan phải r) của B, là trực giao $l^0$ (tương ứng $r^0$) đối với dạng $\Phi$ của môđun con I (tương ứng r) của $^sB$ (tương ứng $^dB$).

e) Cho $\varphi$ là một đồng cấu Frobenius của B vào A. Chứng minh rằng nếu A là một vành Artin có đối hợp (chương VIII, § 3, bài tập 11) thì B cũng có tính chất tương tự, khi giả sử thêm rằng một trong hai điều kiện của b) được thỏa mãn (dùng b) và d)).

¶ 3) Cho A là một trường giao hoán, B là một đại số hạng hữu hạn trên A, có một phần tử đơn vị.

a) Để B là một đại số Frobenius, điều kiện cần và đủ là tồn tại một đồng cấu Frobenius từ B vào A (bài tập 2). (Dùng bài tập 2 c) và e) ở trên, và bài tập 6 b) của chương VIII, § 13).

b) Cho $\varphi$ là một đồng cấu Frobenius của B vào A; mọi dạng A-tuyến tính trên B khi đó có thể được viết theo một và chỉ một cách $x \to \varphi(b'x)$ (tương ứng $x \to \varphi(xb'')$) trong đó $b'$ và $b''$ thuộc B; để dạng này là một đồng cấu Frobenius, điều kiện cần và đủ là $b'$ (tương ứng $b''$) khả nghịch trong B.

c) Với mọi $x \in B$, gọi $x^\sigma$ là phần tử duy nhất (xem b)) sao cho $\varphi(xy) = \varphi(yx^\sigma)$ với mọi $y \in B$. Chứng minh rằng $x \to x^\sigma$ là một tự đẳng cấu A của B. Người ta nói rằng đại số Frobenius B là đối xứng nếu $\sigma$ là một tự đẳng cấu trong của B; khi đó tồn tại một đồng cấu Frobenius từ B vào A mà đối với nó $\sigma$ là đồng nhất (xem b)). Điều này tương đương với việc nói rằng các song môđun (B, B) B và $^sB^* = ^dB^*$ (được viết là B*) là đẳng cấu (bài tập 2 c)).

d) Cho E là một B-môđun trái có độ dài hữu hạn, E’ là đối ngẫu của nó, E’* là đối ngẫu của E’ được xét như không gian vectơ trên A; E’* được trang bị một cấu trúc B-môđun trái bằng cách đặt, với $x' \in E'$, $x'' \in {E'}^*$, $b \in B$, $\langle x', bx'' \rangle = \langle x'b, x'' \rangle$ (Chương III, ấn bản lần thứ 2, Phụ lục II, No. 7). Với mỗi $x \in E$, gọi $f_E(x)$ (hoặc đơn giản là $f(x)$) là phần tử của E’* sao cho $\langle x', f(x) \rangle = \varphi(\langle x, x' \rangle)$ với mọi $x' \in E'$; bây giờ chứng minh rằng $f$ là một song ánh nửa tuyến tính đối với tự đẳng cấu $\sigma$, từ B-môđun trái E lên B-môđun trái E’* (dùng Bài tập 10 của Chương VIII, § 4). Với $E = B_s$, ta có (với các ký hiệu của Bài tập 2 b)) $d_\Phi(x^\sigma) = f_{B_s}(x)$ với mọi $x \in B$.

4) a) Cho G là một nhóm hữu hạn. Chứng minh rằng đại số B của nhóm G trên một trường giao hoán bất kỳ A là một đại số Frobenius đối xứng (Bài tập 3). (Xét ánh xạ $\varphi$ của B vào A gán cho mỗi phần tử $x = \sum_{s \in G} \xi_s . s$, phần tử $\varphi(x) = \xi_e$, trong đó e ký hiệu phần tử đơn vị của G).

b) Cho E là một không gian vectơ hữu hạn chiều có chiều $n$ trên một trường giao hoán A, và B là đại số ngoài $\wedge E$. Chứng minh rằng B là một đại số Frobenius. (Nếu $(e_i)_{1 \leq i \leq n}$ là một cơ sở của E, xét ánh xạ gán cho mỗi phần tử $x$ của B hệ số của $e_1 \wedge e_2 \wedge \ldots \wedge e_n$ trong biểu thức của $x$ theo cơ sở của B tương ứng với $(e_i)$). Để đại số Frobenius B là đối xứng, điều kiện cần và đủ là $n$ chẵn hoặc A có đặc số 2.

¶ 5) a) Chứng minh rằng tích tenxơ của hai đại số Frobenius (tương ứng đại số Frobenius và đối xứng) có hạng hữu hạn trên một trường giao hoán K là một đại số Frobenius (tương ứng Frobenius và đối xứng) (xem § 1, No. 9, Mệnh đề 9).

b) Cho B là một đại số hạng hữu hạn trên K, L là một mở rộng của K có bậc hữu hạn trên K. Chứng minh rằng nếu đại số $B_{(L)} = B \otimes_K L$ trên L là Frobenius (tương ứng Frobenius và đối xứng), thì B cũng có tính chất tương tự. (Dùng các Bài tập 2 c) và 3 c) ở trên và Bài tập 2 của Chương VIII, § 2).

6) Chứng minh rằng mọi đại số nửa đơn tuyệt đối B có hạng hữu hạn trên một trường giao hoán A là một đại số Frobenius đối xứng. (Quy về trường hợp B là đơn; dùng Bài tập 5 b) ở trên, cũng như Mệnh đề 9 của Chương VIII, § 12, No. 3).
