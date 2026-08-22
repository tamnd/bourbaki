---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 6
section_title: Morita Equivalence of Modules and Algebras
lang: vi
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.95-A VIII.117
pdf_pages: 0112-0134
extraction: native+ocr
subsections:
    - "no": 1
      title: Commutant and Duality
      page: 95
      pdf_page: 112
    - "no": 2
      title: Generating Modules and Finitely Generated Projective Modules
      page: 98
      pdf_page: 115
    - "no": 3
      title: Invertible Bimodules and Morita Equivalence
      page: 100
      pdf_page: 117
    - "no": 4
      title: The Morita Correspondence of Modules
      page: 103
      pdf_page: 120
    - "no": 5
      title: Ordered Sets of Submodules
      page: 106
      pdf_page: 123
    - "no": 6
      title: Other Properties Preserved by the Morita Correspondence
      page: 109
      pdf_page: 126
    - "no": 7
      title: Morita Equivalence of Algebras
      page: 111
      pdf_page: 128
statements: 40
exercises: 8
content_sha256: 046371409ef0bc7b4efc379b291fba8fe60090ea9f6074a96dee604887fade3a
translated_from: content/en/alg/VIII/06_s6_morita_equivalence_of_modules_and.md
source_content_sha256: 25fb547cdd0923e402adfb7298b0fc0f1bd6503c596ee2106e24c4da92314558
translation_model: gpt-5.4
translation_run: translate-vi-cd398399
glossary_version: 34
glossary_terms_sha256: aca19b8b6fd6e6d651ca1af11ba556d96ca5841ee940f6b218c056df601b3cc5
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 6. TƯƠNG ĐƯƠNG MORITA CỦA CÁC MÔĐUN VÀ CÁC ĐẠI SỐ

Trong tiết diện này, $k$ ký hiệu một vành giao hoán.

### 1. Hoán tập và đối ngẫu

Cho A và B là các đại số trên $k$. Nhắc lại (III, §4, No. 3, p. 466) rằng một song môđun trên các đại số A và B là một $(A$, B)-song môđun P mà trên đó hai cấu trúc $k$-môđun suy ra từ các cấu trúc A-môđun và B-môđun trùng nhau. Để tránh mọi sự nhập nhằng, ta nói rằng P là một $(A,B)_k$-song môđun. Cho P là một $(A,B)_k$-song môđun. Ta ký hiệu bởi $P^*$ đối ngẫu Hom$_A(P,A)$ của A-môđun trái suy ra từ P. Đó là một $(B,A)_k$-song môđun (II, §1, No. 14, p. 226); với $a\in A$, $b\in B,x\in P$, và $x^*\in P^*$, ta có

$$
\langle x, bx^*a\rangle =\langle xb, x^*\rangle a \tag{1}
$$

Ta ký hiệu bởi $_sA_d$ đại số A được xem như một $(A,A)_k$-song môđun (loc. cit.) và bởi $\Lambda  : P\otimes_BP^*\rightarrow_sA_d$ đồng cấu của các $(A,A)_k$-song môđun được xác định bởi

$$
\Lambda (x\otimes x^*) =\langle x, x^*\rangle \tag{2}
$$

đối với $x\in P$ và $x^*\in P^*$. Ta ký hiệu bởi $\widetilde{P}$ đối ngẫu Hom$_B(P,B)$ của B-môđun phải nền tảng của P; đó là một $(B,A)_k$-song môđun. Ta ký hiệu bởi $\widetilde{\Lambda} :\widetilde{P}\otimes_AP\rightarrow_sB_d$ đồng cấu của các $(B,B)_k$-song môđun được xác định bởi (3) $\widetilde{\Lambda}(\widetilde{x}\otimes x) =\langle \widetilde{x}, x\rangle$

đối với $x\in P$ và $\widetilde{x}\in \widetilde{P}$.

Bây giờ, giả sử rằng ánh xạ $b\mapsto b_P$ là một song ánh từ B lên End$_A(P)$; khi đó nó là một đẳng cấu từ B lên đại số đối của End$_A(P)$. Đồng cấu chính tắc của các $\mathbf{Z}$-môđun từ $P^*\otimes_AP$ đến End$_A(P)$ (II, §4, No. 2, p. 271) khi đó xác định một đồng cấu của các $\mathbf{Z}$-môđun $\Theta  : P^*\otimes_AP\rightarrow$ B được định nghĩa bởi

$$
x\Theta (x^*\otimes y) =\langle x, x^*\rangle y \tag{4}
$$

với $x, y\in P$ và $x^*\in P^*$. Vì (1), đồng cấu này là tuyến tính $(B$, B), và ta có

$$
\Theta (x^*\otimes y)y^*=x^*\langle y, y^*\rangle \tag{5}
$$

với $y\in P$ và $x^*, y^*\in P^*$. Từ (4) và (5), ta suy ra các đẳng thức sau trong $(B,B)_k$-song môđun $P^*\otimes_AP:$

$$
(y^*\otimes x)\Theta (x^*\otimes y) =y^*\otimes  \langle x, x^*\rangle y=y^*\langle x, x^*\rangle  \otimes y= \Theta (y^*\otimes x)(x^*\otimes y)
$$

với $x, y\in P$ và $x^*, y^*\in P^*$, và do đó

$$
s\Theta (t) = \Theta (s)t \tag{6}
$$

với $s, t\in P^*\otimes_AP$. Tương tự, với $x, y$ trong P và $x^*, y^*$ trong $P^*$, ta suy ra các đẳng thức sau trong $(A,A)_k$-song môđun $P\otimes_BP^*$ từ (4) và (5):

$$
(x\otimes x^*)\langle y, y^*\rangle =x\otimes \Theta (x^*\otimes y)y^*=x\Theta (x^*\otimes y)\otimes y^*=\langle x, x^*\rangle (y\otimes y^*)
$$

và do đó

$$
u\Lambda (v) = \Lambda (u)v \tag{7}
$$

với $u, v\in P\otimes_BP^*$.

Với mọi phần tử $x^*$ của $P^*$, ký hiệu ánh xạ B-tuyến tính $x\mapsto \Theta (x^*\otimes x)$ từ P vào B bởi $\sigma (x^*)$. Như vậy ta định nghĩa một ánh xạ $\sigma$ từ $P^*$ vào $\widetilde{P}$, ánh xạ này là $(B$, A)-tuyến tính và theo định nghĩa thỏa mãn

$$
\Theta (x^*\otimes y) =\langle \sigma (x^*), y\rangle \tag{8}
$$

với $x^*\in P^*$ và $y\in P$. Do định nghĩa của $\widetilde{\Lambda}$, vì thế ta có

$$
\Theta  =\widetilde{\Lambda}\circ (\sigma \otimes 1_P) \tag{9}
$$

Giả sử rằng ánh xạ $a\mapsto a_P$ từ A đến End$_B(P)$ là song ánh; khi đó nó là một đẳng cấu đại số. Tương tự, ta định nghĩa một đồng cấu của các $(A,A)_k$-song môđun $\widetilde{\Theta} : P\otimes_B\widetilde{P}\rightarrow_sA_d$ bằng cách đặt

$$
\widetilde{\Theta}(x\otimes \widetilde{y})y=x\langle \widetilde{y}, y\rangle \tag{10}
$$

với $x, y\in P$ và $\widetilde{y}\in \widetilde{P}$. Ta cũng định nghĩa một đồng cấu của các $(B,A)_k$-song môđun $\widetilde{\sigma}:\widetilde{P}\rightarrow P^*$ bằng cách đặt

$$
\widetilde{\Theta}(x\otimes \widetilde{y}) =\langle x,\widetilde{\sigma}(\widetilde{y})\rangle \tag{11}
$$

với $x\in P,\widetilde{y}\in \widetilde{P}$. Ta có

$$
\widetilde{\Theta} = \Lambda \circ (1_P\otimes \widetilde{\sigma}) \tag{12}
$$

#### Mệnh đề 1 {#alg-viii-s6-prop-1 .statement tag=006R}

Giả sử rằng các ánh xạ $b\mapsto b_P$ từ B vào End$_A(P)$ và $a\mapsto a_P$ từ A vào End$_B(P)$ là song ánh. Khi đó $\sigma$ và $\widetilde{\sigma}$ là các đẳng cấu nghịch đảo của nhau, và ta có các hệ thức

$$
\Lambda  =\widetilde{\Theta}\circ (1_P\otimes \sigma ) \tag{13}
$$

$$
\widetilde{\Lambda} = \Theta \circ (\widetilde{\sigma}\otimes 1_P) \tag{14}
$$

Với $x\in P,x^*\in P^*$, và $y\in P$, theo các hệ thức (4), (8), (10), và (11), ta có

$$
(15)\langle x, x^*\rangle y=x\Theta (x^*\otimes y) =x\langle \sigma (x^*), y\rangle =\widetilde{\Theta}(x\otimes \sigma (x^*))y=\langle x,\widetilde{\sigma}(\sigma (x^*))\rangle y
$$

Tương tự, với $x\in P,\widetilde{y}\in \widetilde{P}$, và $y\in P$, ta có

$$
x\langle \widetilde{y}, y\rangle =\widetilde{\Theta}(x\otimes \widetilde{y})y=\langle x,\widetilde{\sigma}(\widetilde{y})\rangle y=x\Theta  (\widetilde{\sigma}(\widetilde{y})\otimes y) =x\langle \sigma (\widetilde{\sigma}(\widetilde{y})), y\rangle \tag{16}
$$

Do các giả thiết, P là trung thành như một A-môđun và như một B-môđun. Từ các hệ thức (15) và (16), tương ứng, suy ra $\widetilde{\sigma}\circ \sigma = 1_{P^*}$ và $\sigma \circ \widetilde{\sigma}=$ $1_{\widetilde{P}}$. Khi đó các hệ thức (13) và (14) lần lượt suy ra từ (12) và (9).

#### Nhận xét 1 {#alg-viii-s6-n1-rem-1 .statement tag=006S}

Giả sử rằng ánh xạ $b\mapsto b_P$ từ B vào End$_A(P)$ là song ánh. Khi đó

a) B-môđun P có thể được đồng nhất với môđun đối của P; do đó nó là trung thành và cân bằng;

b) ánh xạ $a\mapsto a_P$ từ A vào End$_B(P)$ là song ánh khi và chỉ khi A-môđun P là trung thành và cân bằng.

#### Nhận xét 2 {#alg-viii-s6-n1-rem-2 .statement tag=006T}

Dưới các giả thiết của Mệnh đề 1, A-môđun P là cân bằng; vì các vành $A_P$ và $A'_P$ có cùng tâm (VIII, p. 77), tồn tại một đẳng cấu $\varphi$ từ tâm Z(A) của vành A lên tâm Z(B) của vành B, được xác định bởi quan hệ $\varphi (z)_P=z_P$ với $z\in Z(A)$. Hơn nữa, các nội đồng cấu của song môđun $(A,B)_k$ P là các phép vị tự $z_P$ khi $z$ chạy qua Z(A); các tự đẳng cấu của song môđun $(A,B)_k$ P là các phép vị tự $z_P$ khi $z$ khả nghịch trong Z(A).

### 2. Các môđun sinh và các môđun xạ ảnh sinh hữu hạn

#### Mệnh đề 2 {#alg-viii-s6-prop-2 .statement tag=006U}

Cho A và B là các đại số trên $k$, và cho P là một song môđun $(A,B)_k$. Giả sử rằng ánh xạ $b\mapsto b_P$ từ B tới End$_A(P)$ là song ánh. Các mệnh đề sau là tương đương:

(i) A-môđun P là xạ ảnh và sinh hữu hạn.

(ii) Ánh xạ Θ (VIII, p. 96) là một đẳng cấu của các $(B,B)_k$-song môđun từ $P^*\otimes_AP$ đến $_sB_d$.

(iii) Ảnh của Θ chứa phần tử đơn vị của B.

Hơn nữa, nếu ánh xạ $a\mapsto a_P$ từ A đến End$_B(P)$ là song ánh, thì các khẳng định trên là tương đương với mệnh đề sau:

(iv) Tồn tại một $(B,A)_k$-song môđun Q và một đồng cấu toàn ánh của các $(B,B)_k$-song môđun từ $Q\otimes_AP$ đến $_sB_d$.

Theo hệ quả của II, §4, No. 2, p. 271, mệnh đề (i) kéo theo (ii). Hơn nữa, (iii) suy ra từ (ii). Cho $t\in B^*\otimes_AB$ sao cho $\Theta (t) = 1$. Cho $n$ là một số nguyên, và cho $(x_1, . . . , x_n)\in P^n$ và $(x^*_1, . . . , x^*_n)\in P^{*n}$ sao cho $t=\sum^n_{i=1}x^*_i\otimes x_i$. Với mọi $x$ thuộc P, quan hệ $x\Theta (t) =x$ có thể viết thành

$$
\sum_{i=1}^n\langle x, x^*_i\rangle x_i=x
$$

Suy ra A-môđun P là sinh hữu hạn bởi họ $(x_i)_{1\leqslant i\leqslant n}$, và ta kết luận chứng minh của kéo theo (iii) $\Rightarrow$ (i) bằng cách dùng Mệnh đề 12 của II, §2, No. 6, p. 238.

Hiển nhiên ta có (ii) $\Rightarrow$ (iv). Cho Q là một $(B,A)_k$-song môđun và $\theta$ là một đồng cấu toàn ánh của các $(B,B)_k$-song môđun từ $Q\otimes_AP$ đến $_sB_d$. Theo ký hiệu của tiểu mục trước, tồn tại một đồng cấu của các $(B,A)_k$-song môđun $\zeta : Q\rightarrow \widetilde{P}$ sao cho $\theta (y\otimes x) =\langle \zeta (y), x\rangle$ với $x\in P$ và $y\in Q$, và ta có $\theta =\widetilde{\Lambda}\circ (\zeta \otimes 1_P)$. Vì $\theta$ là toàn ánh, điều tương tự cũng đúng với $\widetilde{\Lambda}$. Nếu ánh xạ $a\mapsto a_P$ từ A đến End$_B(P)$ là song ánh, thì Θ là toàn ánh theo quan hệ (14) của Mệnh đề 1 ở VIII, p. 97; suy ra kéo theo (iv) $\Rightarrow$ (iii).

#### Mệnh đề 3 {#alg-viii-s6-prop-3 .statement tag=006V}

Cho A và B là các đại số trên $k$ và P là một $(A,B)_k$-song môđun. Các tính chất sau là tương đương:

(i) A-môđun P là sinh.

(ii) Ảnh của ánh xạ Λ từ $P\otimes_BP^*$ đến $_sA_d$ (VIII, p. 95) chứa phần tử đơn vị.

(iii) Tồn tại một $(B,A)_k$-song môđun Q và một đồng cấu toàn ánh của các $(A,A)_k$-song môđun từ $P\otimes_BQ$ đến $_sA_d$.

Hơn nữa, nếu ánh xạ $b\mapsto b_P$ từ B đến End$_A(P)$ là song ánh, thì các khẳng định ấy tương đương với mệnh đề sau:

(iv) Ánh xạ Λ là một đẳng cấu từ $P\otimes_BP^*$ đến $_sA_d$.

(i) $\Leftrightarrow$ (ii): Ảnh của Λ là iđêan vết $\tau (P)$ (VIII, p. 80). Do đó tính tương đương của (i) và (ii) suy ra từ Định lý 1 của VIII, p. 80.

(ii) $\Rightarrow$ (iii): Chỉ cần lấy $Q = P^*$.

(iii) $\Rightarrow$ (ii): Cho Q là một song môđun $(B,A)_k$ và $\psi$ là một đồng cấu các song môđun $(A,A)_k$ từ $P\otimes_BQ$ đến $_sA_d$. Tồn tại một đồng cấu các song môđun $(B,A)_k$ Ψ từ Q đến $P^*$ sao cho $\psi (x\otimes y) =\langle x,\Psi (y)\rangle$ với $x\in P$ và $y\in Q$, và ta có đẳng thức $\psi = \Lambda \circ (1_P\otimes \Psi )$. Nếu $\psi$ là toàn ánh, thì Λ cũng vậy.

Rõ ràng là (iv) suy ra (ii). Ngược lại, giả sử rằng tính chất (ii) được thỏa mãn và ánh xạ $b\mapsto b_P$ từ B đến End$_A(P)$ là song ánh. Gọi $e$ là một phần tử của $P\otimes_BP^*$ sao cho $\Lambda (e) = 1$. Theo quan hệ (7) của VIII, p. 96, ta có $u= \Lambda (u)e$ với mọi $u$ trong $P\otimes_BP^*$; do đó suy ra tính đơn ánh của Λ.

#### Mệnh đề 4 {#alg-viii-s6-prop-4 .statement tag=006W}

Cho A và B là các $k$-đại số và P là một song môđun $(A,B)_k$. Giả sử rằng ánh xạ $b\mapsto b_P$ từ B đến End$_A(P)$ là song ánh.

a) Nếu A-môđun P là sinh, thì B-môđun phải P là xạ ảnh và sinh hữu hạn.

b) Nếu A-môđun P là xạ ảnh và sinh hữu hạn, thì B-môđun phải P là sinh.

Giả sử rằng A-môđun P là sinh. Khi đó nó là trung thành và cân bằng (VIII, p. 82, Định lý 2), và do đó ánh xạ $a\mapsto a_P$ từ A tới End$_B(P)$ là song ánh (VIII, p. 97, Nhận xét 1). Hơn nữa, ánh xạ $\Lambda  : P\otimes_BP^*\rightarrow_sA_d$ là song ánh (VIII, p. 98, Mệnh đề 3). Ta xem P như một $(B^o,A^o)_k$-song môđun. Ánh xạ Λ cảm sinh một ánh xạ song ánh $P^*\otimes_{B^o}P\rightarrow A^o$; theo Mệnh đề 2 của VIII, p. 98, (iv) $\Rightarrow$ (i), B-môđun phải P là xạ ảnh và sinh hữu hạn.

Bây giờ, giả sử rằng A-môđun P là xạ ảnh và sinh hữu hạn. Khi đó ánh xạ $\Theta  : P^*\otimes_AP\rightarrow_sB_d$ là song ánh (loc. cit., (i) $\Rightarrow$ (ii)). Theo hàm ý (iii) $\Rightarrow$ (i) của Mệnh đề 3 ở trên áp dụng cho $(B^o,A^o)_k$-song môđun P, B-môđun phải P là sinh.

#### Hệ quả 1 {#alg-viii-s6-prop-4-cor-1 .statement tag=006X}

Môđun đối của một môđun sinh là xạ ảnh và sinh hữu hạn. Môđun đối của một môđun xạ ảnh hữu hạn sinh là sinh.

Cho A là một $k$-đại số, và cho M là một A-môđun. Ta ký hiệu đối $k$-đại số của đại số End$_A(M)$ bởi B. Hệ quả suy ra từ Mệnh đề 4 áp dụng cho $(A,B)_k$-song môđun M.

#### Hệ quả 2 {#alg-viii-s6-prop-4-cor-2 .statement tag=006Y}

Cho A và B là các $k$-đại số và P là một $(A,B)_k$-song môđun. Các tính chất sau là tương đương:

(i) A-môđun P là sinh, và ánh xạ $b\mapsto b_P$ từ B vào End$_A(P)$ là song ánh.

(ii) B-môđun phải P là xạ ảnh, sinh hữu hạn, trung thành, và cân bằng, và ánh xạ $a\mapsto a_P$ từ A vào End$_B(P)$ là song ánh.

Hệ quả (i) $\Rightarrow$ (ii) suy ra từ Mệnh đề 4, a) và Nhận xét 1 (VIII, p. 97). Giả sử rằng (ii) đúng; khi đó A-môđun P là sinh (Mệnh đề 4, b) áp dụng cho $(B^o,A^o)_k$-song môđun P). Vì B-môđun P là trung thành và cân bằng, mệnh đề thứ hai của (i) cũng được thỏa mãn (VIII, p. 97, Nhận xét 1).

### 3. Song môđun khả nghịch và tương đương Morita

#### Định nghĩa 1 {#alg-viii-s6-def-1 .statement tag=006Z}

Cho A và B là các $k$-đại số và P là một $(A,B)_k$-song môđun. Ta nói rằng P là khả nghịch nếu tồn tại một $(B,A)_k$-song môđun Q sao cho $P\otimes_BQ$ đẳng cấu với $_sA_d$ và $Q\otimes_AP$ đẳng cấu với $_sB_d$. Một song môđun như vậy Q được gọi là một nghịch đảo của P.

Cho A và B là các đại số $k$, và cho P là một $(A,B)_k$-song môđun khả nghịch. Cho C là một đại số $k$ và $P'$ là một $(B,C)_k$-song môđun khả nghịch. Cuối cùng, cho Q và $Q'$ lần lượt là các song môđun nghịch đảo của P và $P'$. Do tính kết hợp của tích tenxơ (II, §3, No. 8, p. 258, Mệnh đề 8) và Mệnh đề 4 của II, §3, No. 4, p. 249, $(C,A)_k$-song môđun $Q'\otimes_BQ$ là một song môđun nghịch đảo của $(A,C)_k$-song môđun $P\otimes_BP'$, do đó $P\otimes_BP'$ là một $(A,C)_k$-song môđun khả nghịch.

Do đó, quan hệ

“A và B là các đại số $k$, và tồn tại một $(A,B)_k$-song môđun khả nghịch” là một quan hệ tương đương.

#### Định nghĩa 2 {#alg-viii-s6-def-2 .statement tag=0070}

Hai $k$-đại số A và B được gọi là tương đương Morita nếu tồn tại một song môđun $(A,B)_k$ khả nghịch. Các vành A và B được gọi là tương đương Morita nếu các $\mathbf{Z}$-đại số A và B là tương đương Morita.

Hai $k$-đại số đẳng cấu thì tương đương Morita. Nếu hai $k$-đại số tương đương Morita, thì các đại số đối của chúng tương đương Morita.

Cho P là một song môđun $(A, B)_k$ khả nghịch và Q là một nghịch đảo của P. Khi đó Q là một song môđun $(B, A)_k$ khả nghịch, và nó có P làm nghịch đảo. Hơn nữa, khi được xem như một song môđun $(B^\circ, A^\circ)_k$, P là khả nghịch và có song môđun $(A^\circ, B^\circ)_k$ Q làm nghịch đảo.

#### Bổ đề 1 {#alg-viii-s6-lem-1 .statement tag=0071}

— *Cho A và B là các k-đại số, P là một song môđun $(A, B)_k$ khả nghịch, M và N là các B-môđun, và $u : M \to N$ là một ánh xạ B-tuyến tính. Nếu ánh xạ $1_P \otimes u : P \otimes_B M \to P \otimes_B N$ bằng không (resp. song ánh), thì u cũng vậy.*

Cho Q là một nghịch đảo song môđun của P và $\theta : Q \otimes_A P \to {}_s B_d$ là một đẳng cấu các song môđun $(B, B)_k$. Bổ đề suy ra từ tính giao hoán của biểu đồ

$$
\begin{array}{ccc}
Q \otimes_A P \otimes_B M & \xrightarrow{1_Q \otimes 1_P \otimes u} & Q \otimes_A P \otimes_B N \\
\downarrow \theta \otimes 1_M & & \downarrow \theta \otimes 1_M \\
M & \xrightarrow{u} & N.
\end{array}
$$

*Định lý 1.* — *Cho A và B là các đại số trên K và P là một song môđun $(A, B)_k$. Ký hiệu song môđun $(B, A)_k$ $\operatorname{Hom}_A(P, A_s)$ bởi $P^*$. Các tính chất sau là tương đương:*

(i) *Song môđun $(A, B)_k$ P là khả nghịch.*

(ii) *A-môđun P là xạ ảnh, sinh hữu hạn, và sinh, và ánh xạ $b \mapsto b_P$ từ B vào $\operatorname{End}_A(P)^{\circ}$ là một đẳng cấu đại số.*

(iii) *B-môđun phải P là xạ ảnh, sinh hữu hạn, và sinh, và ánh xạ $a \mapsto a_P$ từ A vào $\operatorname{End}_B(P)$ là một đẳng cấu đại số.*

*Nếu các tính chất này đúng, thì các đồng cấu*

$$
\Theta : P^* \otimes P \to {}_s B_d \quad \text{và} \quad \Lambda : P \otimes P^* \to {}_s A_d
$$

*là các đẳng cấu, do đó song môđun $(B, A)_k$ $P^*$ là một nghịch đảo của P.*

*Nếu tính chất (ii) đúng, thì P là một song môđun khả nghịch $(A, B)_k$ có nghịch đảo là $P^*$ (VIII, p. 98, Mệnh đề 2 and p. 98, Mệnh đề 3). Điều này chứng minh rằng (ii) suy ra (i) và khẳng định cuối cùng.*

Giả sử song môđun $(A, B)_k$ P là khả nghịch. Khi đó A-môđun P là sinh (VIII, p. 98, Mệnh đề 3, (iii) $\Rightarrow$ (i)). Vậy nên nó trung thành và cân bằng (VIII, p. 82, Định lý 2) và, do đó, ánh xạ $a \mapsto a_p$ từ A vào $\operatorname{End}_B(P)$ là song ánh.

Bây giờ ta chứng minh rằng ánh xạ $b \mapsto b_P$ từ B đến $\operatorname{End}_A(P)$ là song ánh. Cho Q là một $(B, A)_k$-song môđun, nghịch đảo của P. Lấy $u \in \operatorname{End}_A(P)$; khi đó $1_Q \otimes u$ là một tự đồng cấu của B-môđun trái $Q \otimes_A P$. Vì $(B, B)_k$-song môđun $Q \otimes_A P$ đẳng cấu với $_s B_d$, tồn tại một phần tử duy nhất $b$ của B sao cho $1_Q\otimes u$ là phép vị tự với tỉ số $b$ của B-môđun phải $Q\otimes_AP$. Do đó, ta có $1_Q\otimes (u-b_P) = 0$. Suy ra $u=b_P$ theo Bổ đề 1; điều này chứng minh rằng ánh xạ $b\mapsto b_P$ từ B đến End$_A(P)$ là song ánh.

Theo Mệnh đề 2 của VIII, p. 98, A-môđun P khi đó là xạ ảnh và sinh hữu hạn. Vậy chúng ta đã chứng minh được tính tương đương của (i) và (ii).

Bằng cách đổi chỗ vai trò của A và B, ta thu được tính tương đương của (i) và (iii), điều này kết thúc chứng minh của mệnh đề.

#### Hệ quả 1 {#alg-viii-s6-lem-1-cor-1 .statement}

Cho A và B là các $k$-đại số tương đương Morita, và cho P là một $(A,B)_k$-song môđun khả nghịch. Tồn tại một đẳng cấu $\varphi$ từ tâm Z(A) của A đến tâm của B được xác định bởi quan hệ $\varphi (z)_P=z_P$ với mọi $z\in Z(A)$. Các tự đẳng cấu của $(A,B)_k$-song môđun P là các phép vị tự $z_P$ trong đó $z$ là một phần tử khả nghịch của Z(A).

Với Định lý 1, điều này suy ra từ Nhận xét 2 của VIII, p. 97.

#### Hệ quả 2 {#alg-viii-s6-lem-1-cor-2 .statement}

Cho A và B là các $k$-đại số tương đương Morita, và cho P là một $(A,B)_k$-song môđun khả nghịch. Mọi nghịch đảo $(B,A)_k$-song môđun của P đều đẳng cấu với đối ngẫu $P^*=$ Hom$_A(P,A)$ của P. Chính xác hơn, cho Q là một $(B,A)_k$-song môđun là một nghịch đảo của P, và cho $\lambda : P\otimes_BQ\rightarrow_sA_d$ là một đẳng cấu của các $(A,A)_k$-song môđun. Tồn tại một ánh xạ duy nhất $\tau : Q\rightarrow P^*$ được xác định bởi quan hệ $\langle p, \tau (q)\rangle =\lambda (p\otimes q)$ với $p\in P$ và $q\in Q$, và $\tau$ là một đẳng cấu của các $(B,A)_k$-song môđun.

Sự tồn tại và tính duy nhất của ánh xạ $\tau$ là hiển nhiên. Nó là một đồng cấu của các $(B,A)_k$-song môđun, và ta có $\lambda = \Lambda \circ (1_P\otimes \tau )$. Vì $\lambda$ và Λ là các đẳng cấu của các $(A,A)_k$-song môđun (VIII, p. 101, Định lý 1), nên $1_P\otimes \tau$ cũng vậy. Theo Bổ đề 1, ánh xạ $\tau$ là song ánh.

#### Nhận xét {#alg-viii-s6-n3-rem-1 .statement tag=0075}

Dưới các giả thiết của hệ quả, cho $q$ là một phần tử của Q sao cho ta có $\lambda (p\otimes q) = 0$ với mọi $p\in P$. Khi đó ta có $\tau (q) = 0$, nghĩa là, $q= 0$. Tương tự, nếu $p$ là một phần tử của P sao cho ta có $\lambda (p\otimes q) = 0$ với mọi $q\in Q$, thì $p= 0$.

#### Ví dụ 1 {#alg-viii-s6-n3-exa-1 .statement tag=0076}

Cho B là một $k$-đại số, $n$ là một số nguyên $\geqslant 1$, và A là $k$-đại số $\mathbf{M}_n(B)$. B-môđun phải $P = B^n_d$ là xạ ảnh, sinh hữu hạn, và sinh, và A có thể được đồng nhất với đại số tự đồng cấu của P (II, §10, No. 7, p. 349). Theo Định lý 1, $(A,B)_k$-song môđun P là khả nghịch. Do đó, các đại số B và $\mathbf{M}_n(B)$ là tương đương Morita.

#### Ví dụ 2 {#alg-viii-s6-n3-exa-2 .statement tag=00SH}

Cho A là một $k$-đại số giao hoán và P là một A-môđun. Ta xem P như một $(A,A)_k$-song môđun mà hai luật tác động của nó bằng nhau. Nếu $(A,A)_k$-song môđun P là khả nghịch, thì A-môđun P là sinh hữu hạn (Định lý 1). Theo Định lý 3 của Comm. Alg., II, §5, No. 4, p. 114, các tính chất sau là tương đương:

(i) $(A,A)_k$-song môđun P là khả nghịch.

(ii) Tồn tại một A-môđun Q sao cho $P\otimes_AQ$ đẳng cấu với A.

(iii) A-môđun P là xạ ảnh, sinh hữu hạn, và có hạng $1.*$

### 4. Tương ứng Morita của các môđun

Trong tiểu mục này, các chữ cái A và B chỉ các $k$-đại số tương đương Morita và P chỉ một song môđun $(A,B)_k$ khả nghịch. Chọn một song môđun $(B,A)_k$ Q nghịch đảo của P và các đẳng cấu

$\lambda : P\otimes_BQ\rightarrow_sA_d$ and $\theta : Q\otimes_AP\rightarrow_sB_d$.

Với mọi B-môđun trái V, ký hiệu bởi $\theta_V$ đồng cấu của các B-môđun $\theta \otimes 1_V: Q\otimes_AP\otimes_BV\rightarrow V$; đó là một đẳng cấu vì $\theta$ là một đẳng cấu. Tương tự, với mọi A-môđun trái M, ký hiệu bởi $\lambda_M$ đồng cấu của các A-môđun $\lambda \otimes 1_M: P\otimes_BQ\otimes_AM\rightarrow M$; đó là một đẳng cấu vì $\lambda$ là một đẳng cấu.

#### Định lý 2 (Morita) {#alg-viii-s6-thm-2 .statement tag=00S2}

a) Cho V và W là các B-môđun trái. Ánh xạ $g\mapsto 1_P\otimes g$ là một song ánh từ Hom$_B(V,W)$ đến Hom$_A(P\otimes_BV,P\otimes_BW)$. Song ánh ngược gửi một phần tử $h$ của Hom$_A(P\otimes_BV,P\otimes_BW)$ lên phần tử $\theta_W\circ (1_Q\otimes h)\circ \theta_V^{-1}$ của Hom$_B(V,W)$.

b) Mọi A-môđun trái M đều đẳng cấu với một môđun có dạng $P\otimes_BV$, trong đó V là một B-môđun trái.

Cho V và W là các B-môđun trái. Theo Bổ đề 1 của VIII, p. 101, ánh xạ $\varphi :g\mapsto 1_P\otimes g$ từ Hom$_B(V,W)$ vào Hom$_A(P\otimes_BV,P\otimes_BW)$ là đơn ánh. Bằng cách đổi chỗ vai trò của P và Q (và của A và B), ta thấy rằng ánh xạ $\psi :h\mapsto 1_Q\otimes h$ từ Hom$_A(P\otimes_BV,P\otimes_BW)$ vào Hom$_A(Q\otimes_AP\otimes_BV,Q\otimes_AP\otimes_BW)$ cũng là đơn ánh. Bây giờ, hợp thành $\psi \circ \varphi$ là ánh xạ $g\mapsto \theta^{-1}_W\circ g\circ \theta_V$. Nó là song ánh, vì thế $\psi$ cũng vậy. Do đó, $\varphi$ là song ánh, và nghịch đảo của nó là ánh xạ $h\mapsto \theta_W\circ (1_Q\otimes h)\circ \theta^{-1}_V$.

Mệnh đề b) suy ra từ việc $\lambda_M$ là một đẳng cấu từ $P\otimes_B$ $\otimes_A\otimes M$ tới M.

Cho V là một B-môđun trái và W là một môđun con của V. Vì B-môđun P là xạ ảnh (VIII, p. 101, Định lý 1), ánh xạ chính tắc từ $P\otimes_BW$ đến $P\otimes_BV$ là đơn ánh. Ta đồng nhất $P\otimes_BW$ với ảnh của nó trong $P\otimes_BV$ qua ánh xạ này. Ta dùng các quy ước tương tự khi thay P và B lần lượt bằng Q và A.

#### Mệnh đề 5 {#alg-viii-s6-prop-5 .statement tag=0077}

Cho V là một B-môđun trái. Ánh xạ $W\mapsto P\otimes_BW$ là một đẳng cấu từ tập hợp các B-môđun con của V, có thứ tự bởi quan hệ bao hàm, lên tập hợp các A-môđun con của $P\otimes_BV$, có thứ tự bởi quan hệ bao hàm. Đẳng cấu nghịch đảo biến một A-môđun con N của $P\otimes_BV$ thành ảnh qua $\theta_V$ của B-môđun con $Q\otimes_AN$ của $Q\otimes_AP\otimes_BV$.

Ký hiệu $D_B(V)$ là tập hợp các B-môđun con của V, có thứ tự bởi quan hệ bao hàm, và định nghĩa các tập hợp $D_A(P\otimes_BV)$ và $D_B(Q\otimes_AP\otimes_BV)$ cũng tương tự như vậy. Cho $\varphi : D_B(V)\rightarrow$ $D_A(P\otimes_BV)$ là ánh xạ $W\mapsto P\otimes_BW$ và $\psi$ là ánh xạ từ $D_A(P\otimes_BV)$ đến $D_B(Q\otimes_AP\otimes_BV)$ cho bởi $N\mapsto Q\otimes_AN$. Đây là các ánh xạ tăng, và hợp thành $\psi \circ \varphi$ là ánh xạ $W\mapsto \theta^{-1}_V$(W), ánh xạ này là song ánh. Do đó, $\varphi$ là đơn ánh, và $\psi$ là toàn ánh. Khi thay thế B bằng A và V bằng $P\otimes_BV$, ta thấy rằng $\psi$ cũng là đơn ánh. Vậy, $\varphi$ và $\psi$ là song ánh, và ánh xạ nghịch đảo của $\varphi$ quả thực là ánh xạ đã được mô tả trong mệnh đề.

#### Ví dụ 1 {#alg-viii-s6-n4-exa-1 .statement tag=0078}

Hãy áp dụng Mệnh đề 5 của VIII, p. 104, cho trường hợp riêng $V = B_s$.

a) Ánh xạ $J\mapsto$ PJ là một đẳng cấu từ tập hợp có thứ tự $D(B_s)$ các iđêan trái của B lên tập hợp có thứ tự D(P) các A-môđun con của P. Ánh xạ nghịch đảo gửi một A-môđun con M của P tới iđêan trái J(M) của B gồm các phần tử $b$ của B sao cho M chứa $Pb$.

b) Ánh xạ $K\mapsto$ KP là một đẳng cấu từ tập hợp có thứ tự $D(A_d)$ các iđêan phải của A lên tập hợp có thứ tự D(P) các B-môđun con của P. Ánh xạ nghịch đảo gửi một B-môđun con V của P tới iđêan phải K(V) của A gồm các phần tử $a$ của A sao cho V chứa $aP$.

Thật vậy, A-môđun $P\otimes_BB_s$ có thể được đồng nhất một cách chính tắc với P. Nếu J là một iđêan trái của B, thì ảnh chính tắc của $P\otimes_BJ$ trong $P\otimes_BB_s$ tương ứng với PJ qua sự đồng nhất này. Do đó, ánh xạ $J\mapsto$ PJ là một đẳng cấu của các tập hợp có thứ tự từ $D(B_s)$ đến D(P). Cho $J\in D(B_s)$. Ký hiệu tập hợp các phần tử $b$ của B sao cho PJ chứa $Pb$ bởi $J'$. Đó là một iđêan trái của B chứa J, và ta có PJ$'\subset$ PJ. Vì ánh xạ $J\mapsto$ PJ là một đẳng cấu của các tập hợp có thứ tự, tất yếu ta có PJ$'=$ PJ và $J = J'$. Điều này chứng minh a).

Mệnh đề b) suy ra từ mệnh đề a) khi áp dụng cho song môđun khả nghịch $(B^o,A^o)_k$ P.

Chú ý rằng vành A là một trường khi và chỉ khi B-môđun P là đơn.

#### Ví dụ 2 {#alg-viii-s6-n4-exa-2 .statement tag=0079}

Ký hiệu bởi $\mathscr{B}_A,\mathscr{B}_B$, và $\mathscr{B}_P$ các tập hợp các iđêan hai phía của A, các iđêan hai phía của B, và các môđun con song $(A,B)_k$ của P, tương ứng.

a) Ánh xạ $\mathfrak{b}\mapsto P\mathfrak{b}$ là một đẳng cấu của các tập hợp có thứ tự từ $\mathscr{B}_B$ tới $\mathscr{B}_P$; đẳng cấu nghịch đảo biến một môđun con song $(A,B)_k$ $P'$ của P thành iđêan hai phía của B gồm các phần tử $b$ sao cho $Pb\subset P'$.

b) Ánh xạ $\mathfrak{a}\mapsto \mathfrak{a}P$ là một đẳng cấu của các tập hợp có thứ tự từ $\mathscr{B}_A$ lên $\mathscr{B}_P$; đẳng cấu nghịch đảo biến một $(A,B)_k$-môđun con song $P'$ của P thành iđêan hai phía của A gồm các phần tử $a$ sao cho $aP\subset P'$.

Thật vậy, cho J là một iđêan trái của B và $P'=$ PJ. Khi đó $P'$ là một A-môđun con của P và, theo Ví dụ 1, iđêan J gồm các phần tử $b$ của B sao cho $Pb\subset P'$. Hơn nữa, $P'$ là một $(A,B)_k$-môđun con song của P khi và chỉ khi J là một iđêan hai phía của B. Do đó a) suy ra từ loc. cit.

Mệnh đề b) suy ra từ mệnh đề a) áp dụng cho song môđun khả nghịch $(B^o,A^o)_k$ P.

#### Mệnh đề 6 {#alg-viii-s6-prop-6 .statement tag=007A}

Ký hiệu bởi $\mathscr{B}_A$ và $\mathscr{B}_B$ các tập hợp iđêan hai phía của A và các iđêan hai phía của B.

a) Tồn tại một đẳng cấu của các tập hợp có thứ tự $f$ từ $\mathscr{B}_A$ đến $\mathscr{B}_B$ được xác định bởi tính chất sau: nếu $\mathfrak{a}$ là một iđêan hai phía của A và $\mathfrak{b}$ là một iđêan hai phía của B, thì quan hệ $f(\mathfrak{a}) =\mathfrak{b}$ tương đương với $\mathfrak{a}P = P\mathfrak{b}$.

b) Giả sử rằng vành A là giao hoán, do đó A có thể được đồng nhất với tâm của B (VIII, p. 102, Hệ quả 1). Đẳng cấu $f:\mathscr{B}_A\rightarrow$ $\mathscr{B}_B$ biến một iđêan $\mathfrak{a}$ của A thành iđêan hai phía $B\mathfrak{a}$ của B, và ta có $\mathfrak{a}= A\cap B\mathfrak{a}$.

Mệnh đề a) suy ra từ Ví dụ 2.

Bây giờ, giả sử rằng A là giao hoán, và đồng nhất A với tâm của B. Cho $\mathfrak{a}$ là một iđêan của A. Khi đó $B\mathfrak{a}$ là một iđêan hai phía của B; ta có PB$\mathfrak{a}=\mathfrak{a}P$ và do đó $f(\mathfrak{a}) = B\mathfrak{a}$. Gọi $\mathfrak{a}'$ là iđêan $A\cap B\mathfrak{a}$ của A; nó được chứa trong $B\mathfrak{a}$ và chứa $\mathfrak{a}$, nên $B\mathfrak{a}'$ bằng $B\mathfrak{a}$. Vì $f$ là song ánh, suy ra $\mathfrak{a}'=\mathfrak{a}$.

#### Ví dụ 3 {#alg-viii-s6-n4-exa-3 .statement tag=007B}

Cho V là một B-môđun trái. Khi đó sự tương ứng đã cho ở trên gửi linh hóa tử của B-môđun V tới linh hóa tử của A-môđun $P\otimes_BV$. Thật vậy, ký hiệu linh hóa tử của A-môđun $P\otimes_BV$ là $\mathfrak{a}$ và linh hóa tử của B-môđun V là $\mathfrak{b}$. Cho W là môđun con song $(A,B)_k$ của P gồm các phần tử sao cho $p\otimes v= 0$ với mọi phần tử $v$ của V. Ta có bao hàm $P\mathfrak{b}\subset W$; ngược lại, với mọi $p\in W$ và $q\in Q$, ta có $\theta (q\otimes p)$ thuộc $\mathfrak{b}$. Do đó, phần tử $\mathfrak{b}$ của $D(B_s)$ tương ứng với phần tử W của D(P). Tương tự, $\mathfrak{a}\in D(A_d)$ tương ứng với W.

#### Ví dụ 4 {#alg-viii-s6-n4-exa-4 .statement tag=007C}

Với mọi iđêan hai phía $\mathfrak{a}$ của A, ký hiệu tập con của $\mathbf{M}_n(A)$ gồm các ma trận có các phần tử thuộc $\mathfrak{a}$ bởi $\mathbf{M}_n(\mathfrak{a})$. Đó là một iđêan hai phía của $\mathbf{M}_n(A)$. Ta có $\mathbf{M}_n(\mathfrak{a})A^n=\mathfrak{a}^n= A^n\mathfrak{a}$. Suy ra từ Mệnh đề 6 rằng mọi iđêan hai phía của $\mathbf{M}_n(A)$ đều có dạng $\mathbf{M}_n(\mathfrak{a})$, trong đó $\mathfrak{a}$ là một iđêan hai phía của A.

#### Nhận xét {#alg-viii-s6-n4-rem-1 .statement tag=007D}

Ta giữ các giả thiết và ký hiệu ở trên và giả sử rằng song môđun $(B,A)_k$ Q là đối ngẫu $P^*$ của A-môđun P và các đẳng cấu $\lambda$ và $\theta$ là các ánh xạ chính tắc $\Lambda  : P\otimes_BP^*\rightarrow_sA_d$ và Θ : $P^*\otimes_AP\rightarrow_sB_d$ (VIII, p. 101, Định lý 1). Vì A-môđun P là xạ ảnh và sinh hữu hạn, ta có một đẳng cấu chính tắc $\vartheta_M: P^*\otimes_AM\rightarrow$ Hom$_A(P,M)$ với mọi A-môđun M (II, §4, No. 2, p. 271, Hệ quả). Chúng tôi để bạn đọc tự phát biểu lại các kết quả của các tiểu mục 3 và 4 bằng cách thay thế phép dựng $M\mapsto Q\otimes_AM$ bằng phép dựng $M\mapsto$ Hom$_A(P,M)$.

### 5. Các Tập Hợp Có Thứ Tự của Các Môđun Con

Trong tiểu mục này, A và B là các $k$-đại số, M là một A-môđun trái, và V là một B-môđun trái. Ta ký hiệu bởi D(M) (resp. D(V)) tập hợp các môđun con của M (resp. của V), được sắp thứ tự bởi quan hệ bao hàm. Ta giả sử đã cho một đẳng cấu của các tập hợp có thứ tự $\varphi : D(V)\rightarrow D(M)$.

Theo định lý Morita (VIII, p. 103, Định lý 2), ta thu được một đẳng cấu như vậy trong tình huống sau: P là một song môđun $(A,B)_k$ khả nghịch, M là A-môđun $P\otimes_BV$, và với mọi môđun con W của $V,\varphi (W)$ là ảnh chính tắc của $P\otimes_BW$ trong M.

Một số tính chất của môđun M, hoặc của các môđun con của nó, có thể được biểu thị theo tập hợp có thứ tự D(M): chúng được liệt kê trong Bảng I và II.

Môđun M là tổng trực tiếp của một họ $(M_i)_{i\in I}$ các môđun con khi và chỉ khi ta có $M =\sum_{i\in I}M_i$ và $M_i\cap \sum_{j\not=i}M_j= 0$ với mọi $i\in I$. Nhận xét này và việc khảo sát Bảng I cho kết quả sau.

#### Mệnh đề 7 {#alg-viii-s6-prop-7 .statement tag=007E}

a) Ta có $\varphi (0) = 0$ và $\varphi (V) = M$.

b) Cho $(V_i)_{i\in I}$ là một họ các môđun con của V. Ta có

$$
\varphi (\sum_{i\in I}V_i)=\sum_{i\in I}\varphi (V_i),\varphi (\bigcap_{i\in I}V_i)=\bigcap_{i\in I}\varphi (V_i)
$$

Các môđun con của M Tập hợp có thứ tự D(M)

Môđun con không Phần tử nhỏ nhất của D(M)

Môđun con M Phần tử lớn nhất của D(M)

$\bigcap_{i\in I}M_i$ Cận dưới lớn nhất inf$_{i\in I}M_i$

$\sum_{i\in I}M_i$ Cận trên bé nhất sup$_{i\in I}M_i$

Các môđun con bù nhau inf(M$',M''$) $= 0$, sup(M$',M''$) $= M$

Môđun con đơn của M Phần tử cực tiểu của D(M) $-\{0\}$

Môđun con cực đại của M Phần tử cực đại của D(M) $-\{M\}$

Đế $\mathscr{S}(M)$ của M Cận trên bé nhất trong D(M) của tập hợp các

phần tử cực tiểu của D(M)$-\{0\}$

$*$Căn $\mathfrak{R}(M)$ của M Cận dưới lớn nhất trong D(M) của tập hợp

$$
*
$$

(VIII, p. 151) các phần tử cực đại của D(M)$-\{M\}$

Bảng I.

Các tính chất của môđun M Các tính chất của D(M)

M là Noether. Tập hợp có thứ tự D(M) là Noether (Lý thuyết

Tập hợp, III, §6, No. 5, p. 190).

M là Artin. Tập hợp D(M), được sắp thứ tự bởi $\supset$, là

Noether.

M không phân tích được. Ta có M $\not= 0$, và không có

hai phần tử khác không $M'$ và $M''$ của

D(M) thỏa mãn inf(M$',M''$) $= 0$,

sup(M$',M''$) $= M$.

M sinh hữu hạn. Với mọi họ $(M_i)_{i\in I}$ trong D(M) có

cận trên M, tồn tại một tập con hữu hạn

J của I sao cho M = sup$_{j\in I}M_j$. M đơn. Card(D(M)) = 2.

M nửa đơn. M là cận trên bé nhất, trong D(M),

của tập hợp các phần tử cực tiểu của

D(M)$-\{0\}$.

Bảng II.

c) B-môđun V là tổng trực tiếp của họ $(V_i)_{i\in I}$ các môđun con nếu và chỉ nếu M là tổng trực tiếp của họ $(\varphi (V_i))_{i\in I}$.

Cho $V'$ và $V''$ là các môđun con của V sao cho $V'$ được chứa trong $V''$; đặt $M'=\varphi (V')$ và $M''=\varphi (V'')$, để $M''$ chứa $M'$. Ký hiệu bởi $[V',V'']$ khoảng trong D(V) gồm các môđun con W của V sao cho ta có $V'\subset W\subset V''$, và định nghĩa khoảng $[M',M'']$ trong D(M) cũng tương tự. Ánh xạ $W\mapsto W/V'$ là một đẳng cấu của các tập hợp có thứ tự từ $[V',V'']$ đến $D(V''/V')$; ta định nghĩa một đẳng cấu của các tập hợp có thứ tự từ $[M',M'']$ đến $D(M''/M')$ cũng tương tự. Vì $\varphi$ biến khoảng $[V',V'']$ thành $[M',M'']$, nó xác định một đẳng cấu $\varphi$ của các tập hợp có thứ tự từ $D(V''/V')$ đến $D(M''/M')$. Từ điều này và các Bảng I và II, ta suy ra mệnh đề sau.

#### Mệnh đề 8 {#alg-viii-s6-prop-8 .statement tag=007F}

a) Cho $V'$ và $V''$ là các môđun con của V sao cho $V''$ chứa $V'$. B-môđun $V''/V'$ là đơn khi và chỉ khi A-môđun $\varphi (V'')/\varphi (V')$ là đơn.

b) Nếu $V'$ là một môđun con đơn, môđun con cực đại, hoặc nhân tử trực tiếp của V, thì tương ứng $\varphi (V')$ là một môđun con đơn, môđun con cực đại, hoặc nhân tử trực tiếp của M.

c) Đẳng cấu $\varphi$ biến đế $\mathscr{S}(V)$ của V thành đế $\mathscr{S}(M)$ của $M*$và căn (VIII, p. 151, Định nghĩa 1)$\mathfrak{R}(V)$ của V thành căn $\mathfrak{R}(M)$ của M$.*$

d) Cho $(V_i)_{0\leqslant i\leqslant n}$ là một dãy hữu hạn các môđun con của V. Nó là một chuỗi Jordan–Hölder của V khi và chỉ khi $(\varphi (V_i)_{0\leqslant i\leqslant n})$ là một chuỗi Jordan–Hölder của M.

#### Bổ đề 2 {#alg-viii-s6-lem-2 .statement tag=007G}

Cho H và $H'$ là các môđun con của V sao cho $H\cap H'= 0$. Các B-môđun H và $H'$ đẳng cấu khi và chỉ khi các A-môđun $\varphi (H)$ và $\varphi (H')$ đẳng cấu.

Ta đồng nhất $H+H'$ với tích $H\times H'$. Đồ thị của một đẳng cấu từ H tới $H'$ là một môđun con $H''$ của V thỏa mãn

$$
H\cap H''= H'\cap H''= 0,H + H'= H + H''= H'+ H'' \tag{17}
$$

ngược lại, mọi môđun con có các tính chất ấy đều là đồ thị của một đẳng cấu từ H tới $H'$. Theo Mệnh đề 7, quan hệ $H\cap H'= 0$ tương đương với $\varphi (H)\cap \varphi (H') = 0$, và các quan hệ (17) tương đương với các quan hệ

$$
\varphi (H)\cap \varphi (H'') =\varphi (H')\cap \varphi (H'') = 0
$$

$$
\varphi (H) +\varphi (H') =\varphi (H) +\varphi (H'') =\varphi (H') +\varphi (H'')
$$

bổ đề được suy ra.

#### Mệnh đề 9 {#alg-viii-s6-prop-9 .statement tag=00R6}

Cho S là một môđun con đơn của V và T là môđun con đơn $\varphi (S)$ của M. Nếu $V_S$ ký hiệu thành phần đẳng kiểu của V thuộc kiểu S và $M_T$ thành phần đẳng kiểu của M thuộc kiểu T, thì ta có $\varphi (V_S) = M_T$.

Mọi môđun con đơn $S'$ của V phân biệt với S đều thỏa mãn $S'\cap S = 0$. Do đó, nó đẳng cấu với S khi và chỉ khi $\varphi (S')$ đẳng cấu với T (Bổ đề 2). Mặt khác, $V_S$ là tổng của các môđun con đơn của V đẳng cấu với S, và $M_T$ là tổng của các môđun con đơn của M đẳng cấu với T. Vì vậy Mệnh đề 9 suy ra ngay lập tức từ các Mệnh đề 7 và 8.

#### Mệnh đề 10 {#alg-viii-s6-prop-10 .statement tag=007H}

a) B-môđun V là Artin (resp. Noether, không phân tích được, đơn, sinh hữu hạn) khi và chỉ khi M cũng vậy.

b) B-môđun V có độ dài hữu hạn khi và chỉ khi A-môđun M có độ dài hữu hạn, và khi đó ta có long$_B(V) =$ long$_A(M)$.

c) B-môđun V là nửa đơn (resp. đẳng kiểu) khi và chỉ khi A-môđun M là nửa đơn (resp. đẳng kiểu). Trong trường hợp đó, ta có long$_B(V) =$ long$_A(M)$.

Mệnh đề a) suy ra từ tính chất thứ hai được liệt kê trong Bảng II.

Mệnh đề b) suy ra từ Mệnh đề 8, d).

Môđun V là nửa đơn khi và chỉ khi nó bằng đế của nó $\mathscr{S}(V)$; nó là đẳng kiểu khi và chỉ khi tồn tại một môđun con đơn S của V sao cho $V = V_S$. Vì vậy mệnh đề c) suy ra từ các Mệnh đề 7, c), 8, c), và 9 (VIII, p. 106 and 109).

### 6. Các tính chất khác được bảo toàn bởi tương ứng Morita

Cho A và B là các $k$-đại số tương đương Morita và P là một $(A,B)_k$-song môđun khả nghịch.

#### Mệnh đề 11 {#alg-viii-s6-prop-11 .statement tag=007I}

Cho

$$
(\mathscr{E})V'-\overset{f}{\rightarrow}V-\overset{g}{\rightarrow}V''
$$

là một biểu đồ các B-môđun và các ánh xạ B-tuyến tính, và cho

$$
(P\otimes \mathscr{E})P\otimes_BV'\longrightarrow^{1_P\otimes f}P\otimes_BV\longrightarrow^{1_P\otimes g}P\otimes_BV''
$$

là biểu đồ tương ứng của các A-môđun. Khi đó $(\mathscr{E})$ là một dãy khớp khi và chỉ khi $(P\otimes \mathscr{E})$ là một dãy khớp.

Giả sử rằng dãy $(\mathscr{E})$ là khớp. Vì B-môđun phải P là xạ ảnh, dãy $(P\otimes \mathscr{E})$ là khớp (II, §3, No. 6, p. 251, Mệnh đề 5 and II, §3, No. 7, p. 257, Hệ quả 6).

Ngược lại, giả sử rằng dãy $(P\otimes \mathscr{E})$ là khớp. Cho Q là một $(B,A)_k$-song môđun nghịch đảo của P, và $\theta : Q\otimes_AP\rightarrow_sB_d$ là một đẳng cấu. Xét biểu đồ giao hoán

$Q\otimes_AP\otimes_B{V'}^{1_Q\otimes 1_P\otimes f}/$/ $Q\otimes_AP\otimes_BV^{1_Q\otimes 1_P\otimes g}/$/ $Q\otimes_AP\otimes_BV''$

$\theta \otimes 1_{V'}\theta \otimes 1_V\theta \otimes 1_{V''}$

$V'f$ // V $g$ // $V''$.

Vì Q là một A-môđun xạ ảnh và dãy $(P\otimes \mathscr{E})$ là khớp, dòng thứ nhất của biểu đồ này là một dãy khớp. Vì các mũi tên thẳng đứng là các đẳng cấu, dòng thứ hai cũng khớp.

#### Hệ quả {#alg-viii-s6-n6-cor-1 .statement tag=007J}

Cho $f: V\rightarrow W$ là một ánh xạ B-tuyến tính. Khi đó $f$ là đơn ánh (resp. toàn ánh) nếu và chỉ nếu $1_P\otimes f$ là như vậy.

#### Mệnh đề 12 {#alg-viii-s6-prop-12 .statement tag=007K}

Cho V là một B-môđun trái. B-môđun V là xạ ảnh (resp. sinh, trung thành, $*$đơn ánh, hữu hạn trình bày ) nếu và chỉ nếu A-môđun

$$
*
$$

$P\otimes_BV$ là như vậy.

a) Giả sử rằng V là xạ ảnh. Tồn tại một tập hợp I sao cho V đẳng cấu với một môđun con hạng tử trực tiếp của $B^{(I)}_s$ . Khi đó A-môđun $P\otimes_BV$ đẳng cấu với một môđun con hạng tử trực tiếp của $P^{(I)}$; vì P là một A-môđun xạ ảnh, điều tương tự cũng đúng với $P\otimes_BV$.

b) Giả sử rằng B-môđun V là sinh. Cho M là một A-môđun. Tồn tại một B-môđun W sao cho M đẳng cấu với $P\otimes_BW$. Theo Định lý 1 của VIII, p. 80, tồn tại một tập hợp I và một toàn ánh $\varphi : V^{(I)}\rightarrow W$. Theo hệ quả, ánh xạ $1_P\otimes \varphi$ từ $P\otimes (V^{(I})$ tới $P\otimes_AW$ là toàn ánh, điều này cho một toàn ánh $(P\otimes V)^{(I)}\rightarrow M$. Theo Định lý 1 của VIII, p. 80, $P\otimes V$ là một A-môđun sinh.

c) B-môđun V là trung thành khi và chỉ khi linh hóa tử của nó thu về 0. Do đó mệnh đề c) suy ra từ Ví dụ 3 của VIII, p. 105.

$*$d) Giả sử rằng V là đơn ánh. Theo nhận xét ở VIII, p. 106, A-môđun $P\otimes_BV$ đẳng cấu với Hom$_B(Q,V)$, trong đó Q là một nghịch đảo song môđun của A thuộc loại $(B,A)_k$. Vì A-môđun Q là xạ ảnh, do đó phẳng (X, §1, n$^o3$, p. 9, ví dụ 1), nên A-môđun Hom$_B(Q,V)$ là đơn ánh theo X, §1, n$^o8$, p. 18, mệnh đề 11.

e) Giả sử rằng V có một trình bày hữu hạn $L_1\rightarrow L_0\rightarrow V\rightarrow 0$ (X, §1, n$^o4$, p. 10). Lấy tích tenxơ với P, suy ra một dãy khớp các A-môđun $N'_1-\overset{u}{\rightarrow}N'_0\rightarrow P\otimes_BV\rightarrow 0$, trong đó $N'_1$ và $N'_0$ là xạ ảnh và sinh hữu hạn (Mệnh đề 11 và a)). Gọi $N''_0$ là một A-môđun sinh hữu hạn sao cho A-môđun $N_0= N'_0\oplus N''_0$ là tự do và sinh hữu hạn, và gọi $u': N'_1\oplus N''_0\rightarrow N_0$ là đồng cấu $(u,1_{N''_0})$; khi đó $P\otimes_BV$ có thể được đồng nhất với đối hạt nhân của $u'$. Gọi $N_1$ là một A-môđun tự do sinh hữu hạn và $p: N_1\rightarrow N'_1\oplus N''_0$ là một đồng cấu toàn ánh; dãy $N_1\longrightarrow^{u'\circ p}N_0\rightarrow P\otimes_BV\rightarrow 0$ là một trình bày hữu hạn của A-môđun $P\otimes_BV.*$

f) Giả sử A-môđun $P\otimes_BV$ là xạ ảnh (tương ứng, sinh, trung thành, $*$đơn ánh, hữu hạn trình bày ). Áp dụng điều trên (đổi chỗ

$$
*
$$

vai trò của A và B và của P và Q), ta thấy B-môđun $Q\otimes_AP\otimes_BV$ cũng có tính chất này. Do đó điều này cũng đúng với B-môđun V, môđun này đẳng cấu với nó.

#### Hệ quả {#alg-viii-s6-n6-cor-2 .statement tag=007L}

Vành A là Artin trái (tương ứng, Noether trái) khi và chỉ khi vành B là như vậy.

Do có đẳng cấu giữa tập hợp có thứ tự các iđêan trái của B và tập hợp các A-môđun con của P, vành B là Artin trái (tương ứng, Noether trái) khi và chỉ khi A-môđun P là Artin (tương ứng, Noether). Tuy nhiên, theo Định lý 1 của VIII, p. 101, A-môđun P là sinh và sinh hữu hạn; đặc biệt, $A_s$ đẳng cấu với một nhân tử trực tiếp của $P^n$ với một số nguyên $n\geqslant 1$. Do đó, P là Artin (tương ứng, Noether) khi và chỉ khi A là Artin trái (tương ứng, Noether trái).

### 7. Tương đương Morita của các đại số

#### Mệnh đề 13 {#alg-viii-s6-prop-13 .statement tag=007M}

a) Nếu hai $k$-đại số tương đương Morita, thì tâm của chúng là các $k$-đại số đẳng cấu.

b) Hai $k$-đại số giao hoán tương đương Morita khi và chỉ khi chúng đẳng cấu.

c) Hai $k$-đại số là các trường tương đương Morita khi và chỉ khi chúng đẳng cấu.

d) Với $i= 1,2$, cho $A_i$ và $B_i$ là các $k$-đại số tương đương Morita và $P_i$ là một $(A_i,B_i)_k$-song môđun khả nghịch. Đặt $A = A_1\otimes_kA_2,B = B_1\otimes_kB_2$, và $P = P_1\otimes_kP_2$. Các $k$-đại số A và B là tương đương Morita, và P là một $(A,B)_k$-song môđun khả nghịch.

e) Nếu A và B là các $k$-đại số tương đương Morita và $k'$ là một $k$-đại số giao hoán, thì các $k'$-đại số $A_{(k')}$ và $B_{(k')}$ là tương đương Morita.

Mệnh đề a) suy ra từ Hệ quả 1 của VIII, p. 102, và kéo theo b).

Cho K và L là các $k$-đại số là các trường, và cho P là một $(K,L)_k$-song môđun khả nghịch. Không gian vectơ phải trên L P là một môđun đơn (VIII, p. 104), do đó có chiều bằng 1, nên các $k$-đại số End$_L(P)$ và L là đẳng cấu. Theo VIII, p. 101, Định lý 1, ánh xạ $a\mapsto a_P$ từ K đến End$_L(P)$ là một đẳng cấu. Vì vậy, các trường K và L đẳng cấu trên $k$; mệnh đề c) suy ra.

Dưới các giả thiết của d), cho $Q_i(i= 1,2)$ là một nghịch đảo song môđun $(B_i,A_i)_k$ của $P_i$. Ký hiệu song môđun $(B,A)_k$ $Q_1\otimes_kQ_2$ bởi Q. Xét đẳng cấu $k$-tuyến tính chính tắc $(P_1\otimes_kP_2)\otimes_k(Q_1\otimes_kQ_2)\rightarrow (P_1\otimes_kQ_1)\otimes_k$ $(P_2\otimes_kQ_2)$; khi chuyển qua thương, nó xác định một cấu xạ

$$
(P_1\otimes_kP_2)\otimes_B(Q_1\otimes_kQ_2)\rightarrow (P_1\otimes_{B_1}Q_1)\otimes_k(P_2\otimes_{B_2}Q_2)
$$

tức là $(A$, A)-tuyến tính. Ngược lại, đẳng cấu nghịch đảo $(P_1\otimes_kQ_1)\otimes_k(P_2\otimes_k$ $Q_2)\rightarrow (P_1\otimes_kP_2)\otimes_k(Q_1\otimes_kQ_2)$ xác định một cấu xạ $(A$, A)-tuyến tính $(P_1\otimes_{B_1}$ $Q_1)\otimes_k(P_2\otimes_{B_2}Q_2)\rightarrow (P_1\otimes_kP_2)\otimes_B(Q_1\otimes_kQ_2)$. Hai cấu xạ này là nghịch đảo của nhau và do đó là các đẳng cấu. Vì song môđun $(A_i,A_i$)-song môđun $P_i\otimes_{B_i}Q_i$ đẳng cấu với $A_i$, ta thu được một đẳng cấu $(A$, A)-tuyến tính $P\otimes_B$ $Q\rightarrow A$. Tương tự, ta cũng thu được một đẳng cấu $(B$, B)-tuyến tính $Q\otimes_AP\rightarrow B$, điều này hoàn tất chứng minh của d).

Dưới các giả thiết của e), cho P là một $(A,B)_k$-song môđun khả nghịch; khi đó $P_{(k')}$ là một $(A_{(k')},B_{(k')})_{k'}$-song môđun khả nghịch.

Cho A là một $k$-đại số, và $e$ là một phần tử lũy đẳng của A. Tập hợp $eAe$, được trang bị phép cộng, phép nhân và tác động của $k$ cảm sinh bởi các phép tương ứng của A, là một $k$-đại số có phần tử đơn vị $e$.

#### Mệnh đề 14 {#alg-viii-s6-prop-14 .statement tag=007N}

Cho A và B là các $k$-đại số. Khi đó A và B tương đương Morita nếu và chỉ nếu tồn tại một số nguyên $n\geqslant 1$ và một ma trận bình phương $e= (e_{ij})$ trong $\mathbf{M}_n(B)$ thỏa mãn các điều kiện sau:

(i) Ta có $e^2=e$.

(ii) Iđêan hai phía của B sinh bởi các phần tử $e_{ij}$ bằng B.

(iii) $k$-đại số A đẳng cấu với $e\mathbf{M}_n(B)e$.

Nếu các điều kiện (i) và (ii) được thỏa mãn, thì $(e\mathbf{M}_n(B)e,B)_k$-song môđun $eB^n_d$ là khả nghịch.

Theo Định lý 1 (VIII, p. 101), $k$-đại số A tương đương Morita với B nếu và chỉ nếu nó đẳng cấu với đại số tự đồng cấu của một B-môđun phải xạ ảnh, sinh hữu hạn, và sinh. Vì vậy mệnh đề suy ra từ các Bổ đề 3 và 4 dưới đây.

#### Bổ đề 3 {#alg-viii-s6-lem-3 .statement tag=007O}

Một B-môđun phải P là xạ ảnh, sinh hữu hạn, và sinh nếu và chỉ nếu tồn tại một số nguyên $n\geqslant 0$ và một phần tử lũy đẳng $e= (e_{ij})$ trong $\mathbf{M}_n(B)$ có các tính chất sau:

(i) B-môđun P đẳng cấu với $eB^n_d$.

(ii) Iđêan hai phía của B sinh bởi các phần tử $e_{ij}$ bằng B.

Cho P là một B-môđun phải. Khi đó P là xạ ảnh và sinh hữu hạn khi và chỉ khi nó đẳng cấu với một môđun con hạng tử trực tiếp của một B-môđun có dạng $B^n_d$, trong đó $n$ là một số nguyên $\geqslant 0$ (II, §2, No. 2, p. 232, Hệ quả 1). Nếu ta đồng nhất các $k$-đại số $\mathbf{M}_n(B)$ và End(B$^n_d$), thì điều này có nghĩa là tồn tại một phần tử lũy đẳng $e$ trong $\mathbf{M}_n(B)$ sao cho P đẳng cấu với $eB^n_d$.

B-môđun P là sinh nếu và chỉ nếu iđêan vết $\tau (P)$ của nó bằng B, tức là $\tau (eB^n_d) = B$ (VIII, p. 80, Định lý 1). Gọi $x_1, . . . , x_n$ là các phần tử của $B^n_d$ tương ứng với các cột của ma trận $e$, và gọi $x^*_i$ (với $1\leqslant i\leqslant n$) là dạng tuyến tính $(b_1, . . . , b_n)\mapsto b_i$ trên $eB^n_d$. Họ $(x_1, . . . , x_n)$ sinh B-môđun $eB^n_d$, và họ $(x^*_1, . . . , x^*_n)$ sinh đối ngẫu của nó. Bây giờ, ta có $\langle x^*_i, x_j\rangle =e_{ij}$, nên $\tau (eB^n_d)$ là iđêan hai phía của B sinh bởi các $e_{ij}$. Điều này chứng minh Bổ đề 3.

#### Bổ đề 4 {#alg-viii-s6-lem-4 .statement tag=007P}

Cho V là một B-môđun và E là $k$-đại số các tự đồng cấu của V. Cho $e$ là một phép chiếu của V và P là ảnh của $e$. Ánh xạ gửi $v\in eEe$ tới tự đồng cấu $x\mapsto v(x)$ của B-môđun P là một đẳng cấu $k$-đại số từ $eEe$ tới End$_B(P)$.

Ký hiệu ánh xạ được mô tả trong mệnh đề là $\varphi :eEe\rightarrow$ End$_B(P)$; đó là một đồng cấu các $k$-đại số. Cho $u\in$ End$_B(P)$. Ký hiệu bởi $v$ tự đồng cấu của V được xác định bởi $v(x) =u(e(x))$ với $x\in V$. Ta có $(eve)(x) =$ $u(x)$ với $x\in P$, nghĩa là, $\varphi (eve) =u$. Do đó, $\varphi$ là toàn ánh. Cho $w$ là một phần tử của hạt nhân của $\varphi$; các hạn chế của $w$ lên hạt nhân và lên ảnh của $e$ đều bằng không, nên $w$ bằng không, điều đó chứng tỏ rằng $\varphi$ là đơn ánh.

#### Ví dụ 1 {#alg-viii-s6-n7-exa-1 .statement tag=007Q}

Cho A là một $k$-đại số và $e$ là một phần tử lũy đẳng trong A sao cho $AeA = A$. $k$-đại số $eAe$ có thể được đồng nhất với $k$-đại số các tự đồng cấu của môđun con $eA_d$ của $A_d$ (Bổ đề 4). Vì $AeA = A$, suy ra từ Mệnh đề 14 rằng $eA_d$ là một $(eAe,A)_k$-song môđun khả nghịch, do đó các $k$-đại số $eAe$ và A là tương đương Morita. Hơn nữa, định lý của Morita (VIII, p. 103) suy ra các kết quả sau:

a) Cho M và N là các A-môđun trái. Mọi ánh xạ $eAe$-tuyến tính từ $eM$ đến $eN$ mở rộng duy nhất thành một ánh xạ A-tuyến tính từ M đến N.

b) Mọi môđun trái trên $k$-đại số $eAe$ đều đẳng cấu với một môđun dạng $eM$, trong đó M là một A-môđun trái.

#### Ví dụ 2 {#alg-viii-s6-n7-exa-2 .statement tag=007R}

Cho A là một $k$-đại số và $n\geqslant 1$ là một số nguyên. Ta đồng nhất đại số ma trận $\mathbf{M}_n(A)$ với đại số tự đồng cấu của A-môđun phải $A^n_d$. Ta đã thấy rằng A và $\mathbf{M}_n(A)$ tương đương Morita. Với mọi A-môđun trái M, đồng nhất $A^n_d\otimes_AM$ với $M^n$. Khi đó đại số $\mathbf{M}_n(A)$ có một tác động trái trên $M^n$, và ta có

$$
(a\cdot m)_i=\sum_{j=1}^na_{ij}m_j
$$

với $a= (a_{ij})$ trong $\mathbf{M}_n(A)$ và $m= (m_i)$ trong $M^n$. Định lý Morita kéo theo các kết quả sau:

a) Mọi môđun trái trên đại số $\mathbf{M}_n(A)$ đều đẳng cấu với một môđun có dạng $M^n$, trong đó M là một A-môđun trái.

b) Cho M là một A-môđun trái. Ánh xạ $N\mapsto N^n$ là một song ánh từ tập hợp các A-môđun con của M đến tập hợp các $\mathbf{M}_n$(A)-môđun con của $M^n$.

c) Cho M và N là các A-môđun trái. Với một ánh xạ A-tuyến tính $g: M\rightarrow N$, ký hiệu $g_n$ là ánh xạ $(m_i)\mapsto (g(m_i))$ từ $M^n$ vào $N^n$. Khi đó ánh xạ $g\mapsto g_n$ là một song ánh từ Hom$_A(M,N)$ lên Hom$_{\mathbf{M}_n(A)}(M^n,N^n)$.

d) Cho M là một A-môđun trái. Môđun $M^n$ trên vành $\mathbf{M}_n(A)$ là không phân tích được (tương ứng, nửa đơn, đơn, Artin, Noether, sinh hữu hạn) khi và chỉ khi A-môđun M là như vậy.

#### Ví dụ 3 {#alg-viii-s6-n7-exa-3 .statement tag=007S}

Cho A là một miền iđêan chính và L là một A-môđun tự do, sinh hữu hạn, khác không. Gọi B là vành tự đồng cấu của L; khi đó L là một song môđun $(A,B)_{\mathbf{Z}}$ khả nghịch, và các vành A và B là tương đương Morita. Theo định lý Morita, Mệnh đề 10, a) (VIII, p. 109), và định lý cấu trúc của các A-môđun sinh hữu hạn (VII, §4, No. 4, p. 19, Định lý 2), mọi B-môđun sinh hữu hạn đều đẳng cấu với $\oplus^m_{i=1}(L/\mathfrak{a}_iL)$, trong đó $m$ là một số tự nhiên và các $\mathfrak{a}_i$ là các iđêan của A thỏa mãn $\mathfrak{a}_1\subset \mathfrak{a}_2\subset  \cdots  \subset \mathfrak{a}_m$ và $\mathfrak{a}_m\not= A$; số nguyên $m$ và các iđêan $\mathfrak{a}_i$ được xác định duy nhất. Theo Mệnh đề 6 của VIII, p. 105, mọi iđêan hai phía của B đều có dạng $dB$, trong đó $d$ là một phần tử của A.

### Bài tập {#alg-viii-s6-exercises}

Xem [bài tập cho § 6](exercises/s6/).
