---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 4
section_title: Semisimple Modules
lang: vi
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.55-A VIII.75
pdf_pages: 0072-0092
extraction: native
subsections:
    - "no": 1
      title: Semisimple Modules
      page: 55
      pdf_page: 72
    - "no": 2
      title: The homomorphism $\bigoplus_i$ Hom$_A(M,N_i)\longrightarrow$ Hom$_A(M,\bigoplus_iN_i)$
      page: 57
      pdf_page: 74
    - "no": 3
      title: Some Operations on Modules
      page: 58
      pdf_page: 75
    - "no": 4
      title: Isotypical Modules
      page: 61
      pdf_page: 78
    - "no": 5
      title: Description of an Isotypical Module
      page: 62
      pdf_page: 79
    - "no": 6
      title: Isotypical Components of a Module
      page: 65
      pdf_page: 82
    - "no": 7
      title: Description of a Semisimple Module
      page: 69
      pdf_page: 86
    - "no": 8
      title: Multiplicities and Lengths in Semisimple Modules
      page: 71
      pdf_page: 88
statements: 43
exercises: 8
content_sha256: 394ffd36d44bbad65eff93ed8c63974294629aa260517acc68d18719a0f535de
translated_from: content/en/alg/VIII/04_s4_semisimple_modules.md
source_content_sha256: 9d4584b8ed5e9b2ea8bfc7a3b377164098496c5ee0e2c21f520fa31ff9205f9d
translation_model: gpt-5.4
translation_run: translate-vi-d30757fd
glossary_version: 34
glossary_terms_sha256: 8b66e8365384f747887f733e2891f210ff3485351af7dab1388a6ce552f405fd
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 4. MÔĐUN NỬA ĐƠN

### 1. Môđun Nửa Đơn

#### Định nghĩa 1 {#alg-viii-s4-def-1 .statement tag=0040}

Một môđun được gọi là nửa đơn nếu nó là tổng trực tiếp của một họ môđun đơn.[^1].

Một đa môđun được gọi là nửa đơn nếu nó là tổng trực tiếp của một họ đa môđun đơn (x. I, §4, No. 4, p. 37, Định nghĩa 7).

Một A-môđun M là nửa đơn khi và chỉ khi nó là nửa đơn khi được xem như một môđun trên vành các vị tự của nó $A_M$.

#### Ví dụ 1 {#alg-viii-s4-n1-exa-1 .statement tag=0041}

Một môđun thu về 0 và một môđun đơn là những môđun nửa đơn.

#### Ví dụ 2 {#alg-viii-s4-n1-exa-2 .statement tag=0042}

Nếu A là một trường, thì mọi A-môđun đều nửa đơn theo Định lý 1 của II, §7, No. 1, p. 292. Điều này cho thấy rằng, nói chung, một môđun nửa đơn phân tích được theo nhiều cách thành một tổng trực tiếp của các môđun con đơn (xem, tuy nhiên, Hệ quả 2 của VIII, p. 68).

#### Ví dụ 3 {#alg-viii-s4-n1-exa-3 .statement tag=0043}

Cho A là một miền iđêan chính, và cho P là một hệ đại diện gồm các phần tử bất khả quy của A (VII, §1, No. 3, p. 3). Cho M là một A-môđun, và, với mọi $\pi \in P$, gọi $M(\pi )$ là tập hợp các $x\in M$ sao cho $\pi x= 0$. Theo VII, §2, No. 2, p. 9, A-môđun M là nửa đơn khi và chỉ khi nó là tổng của các môđun con $M(\pi )$; khi đó nó là tổng trực tiếp của các môđun con này. Ví dụ này sẽ được tổng quát hóa thêm về sau (VIII, p. 65).

Cho $A_1$ và $A_2$ là các đại số trên một vành giao hoán K. Trong III, §4, No. 3, p. 466, chúng tôi đã đưa vào khái niệm song môđun trái trên các đại số $A_1$ và $A_2$ và đã chỉ ra rằng khái niệm này tương đương với khái niệm môđun trái trên vành $A_1\otimes_KA_2$. Ta nói rằng M là một song môđun đơn (tương ứng nửa đơn, sinh hữu hạn) nếu nó là một môđun đơn (tương ứng nửa đơn, sinh hữu hạn) trên vành $A_1\otimes_KA_2$.

#### Định lý 1 {#alg-viii-s4-thm-1 .statement tag=0044}

Cho M là một môđun là tổng (không nhất thiết trực tiếp) của một họ $(S_i)_{i\in I}$ các môđun con đơn, và cho N là một môđun con của M. Tồn tại một tập con J của I sao cho M là tổng trực tiếp của họ gồm N và các môđun $S_j$ với $j$ chạy qua J.

Cho $\mathscr{S}$ là tập hợp các tập con $I'$ của I sao cho tổng của họ gồm các môđun N và $S_i$ với $i$ trong $I'$ là trực tiếp. Tập hợp $\mathscr{S}$ có đặc trưng hữu hạn: một tập con J của I thuộc $\mathscr{S}$ khi và chỉ khi điều đó cũng đúng với mọi tập con hữu hạn của J. Do đó, tập hợp $\mathscr{S}$ có một phần tử cực đại J (Lý thuyết tập hợp, III, §4, No. 5, p. 171). Đặt $N'= N +\sum_{j\in J}S_j$. Cho $i$ thuộc I - J. Vì J là cực đại trong $\mathscr{S}$, tập hợp $J\cup  \{i\}$ không thuộc $\mathscr{S}$, nên $S_i\cap N'\not= 0$. Vì $S_i$ là một môđun đơn, ta có $S_i\cap N'= S_i$. Do đó ta có $S_i\subset N'$ với mọi $i\in I$, do đó $N'= M$. Điều này hoàn tất chứng minh.

#### Hệ quả 1 {#alg-viii-s4-thm-1-cor-1 .statement tag=0045}

Mọi môđun là tổng của một họ các môđun đơn đều là nửa đơn.

Chỉ cần áp dụng Định lý 1 cho trường hợp N = 0.

#### Hệ quả 2 {#alg-viii-s4-thm-1-cor-2 .statement tag=0046}

Một môđun M là nửa đơn khi và chỉ khi mọi môđun con của M đều là một nhân tử trực tiếp.

Điều kiện đó là cần theo Định lý 1.

Ngược lại, giả sử rằng mọi môđun con của M đều thừa nhận một phần bù. Gọi $M'$ là tổng của các môđun con đơn của M, và $M''$ là một phần bù của $M'$ trong M. Giả sử $M'\not= M$ và do đó $M''\not= 0$. Gọi N là một môđun con đơn sinh khác không của $M''$. Theo Mệnh đề 3 của VIII, p. 49, tồn tại một môđun con cực đại P của N. Gọi Q là một môđun con phụ với P trong M. Khi đó $N\cap Q$ là một môđun con của N, phụ với P trong N, nên đẳng cấu với $N/P$ (II, §1, No. 9, p. 210, Mệnh đề 13). Do đó, $N\cap Q$ là một môđun con đơn của $M''$, trái với định nghĩa của $M'$.

Vậy $M'= M$, và môđun M là nửa đơn theo Hệ quả 1.

#### Hệ quả 3 {#alg-viii-s4-thm-1-cor-3 .statement tag=0047}

Cho M là một môđun nửa đơn và N là một môđun con của M. Các môđun N và $M/N$ đều là nửa đơn. Chính xác hơn, nếu M là tổng trực tiếp của một họ $(S_i)_{i\in I}$ các môđun đơn, thì tồn tại một tập con J của I sao cho $M/N$ đẳng cấu với $\bigoplus_{j\in J}S_j$ và N đẳng cấu với $\bigoplus_{i\in I-J}S_i$.

Chọn J như trong Định lý 1. Môđun $N'=\bigoplus_{j\in J}S_j$ là bổ sung với N trong M; do đó nó đẳng cấu với $M/N$. Hơn nữa, các môđun con N và $\bigoplus_{i\in I-J}S_i$ của M đều bổ sung với $N'$ và do đó đẳng cấu với $M/N'$.

#### Hệ quả 4 {#alg-viii-s4-thm-1-cor-4 .statement tag=0048}

Cho M là một môđun nửa đơn. Khi đó M là đơn khi và chỉ khi vành tự đồng cấu E của M là một trường.

Nếu M là đơn, thì E là một trường theo hệ quả của Mệnh đề 2 của VIII, p. 47.

Nếu E là một trường, thì môđun M là không phân tích được (VIII, p. 31, Mệnh đề 4, a)). Vì hơn nữa nó là nửa đơn, nên nó là đơn.

#### Nhận xét {#alg-viii-s4-n1-rem-1 .statement tag=0049}

Cho K là một trường giao hoán đóng đại số và A là một đại số trên K. Cho M là một A-môđun nửa đơn đồng thời là một không gian vectơ hữu hạn chiều trên trường K. Khi đó M là đơn khi và chỉ khi mọi tự đồng cấu của A-môđun M đều có dạng $x\mapsto \alpha x$ với $\alpha$ thuộc K: điều này là cần theo Định lý 1 của VIII, p. 47, và đủ theo Hệ quả 4 ở trên.

### 2. Đồng cấu $\bigoplus_i$ Hom$_A(M,N_i)\longrightarrow$ Hom$_A(M,\bigoplus_iN_i)$

Cho A là một vành, M là một A-môđun, và $(N_i)_{i\in I}$ là một họ các A-môđun. Với mỗi phần tử $(u_i)$ của $\bigoplus_i$ Hom$_A(M,N_i)$, ta gắn với nó phần tử $m\mapsto (u_i(m))$ của Hom$_A(M,\bigoplus_iN_i)$. Như vậy ta định nghĩa một đồng cấu chính tắc

$\varphi :\bigoplus_i$ Hom$_A(M,N_i)\longrightarrow$ Hom$_A(M,\bigoplus_iN_i)$.

Rõ ràng là $\varphi$ đơn ánh. Cho $u$ là một phần tử của Hom$_A(M,\bigoplus_iN_i)$. Khi đó $u$ thuộc ảnh của $\varphi$ khi và chỉ khi tập hợp các chỉ số $i$ sao cho pr$_i\circ u\not= 0$ là hữu hạn. Điều kiện này tự động được thỏa mãn khi môđun M sinh hữu hạn.

Do đó, nếu môđun M sinh hữu hạn, thì đồng cấu $\varphi$ là song ánh.

### 3. Một số phép toán trên môđun

Cho A và B là các vành, và cho P là một $(A$, B)-song môđun (II, §1, No. 14, p. 225). Ta sẽ định nghĩa hai thủ tục, một thủ tục để đi từ một B-môđun trái tới một A-môđun trái, thủ tục kia để đi từ một A-môđun trái tới một B-môđun trái.

3.1. Phép toán $\mathscr{T}$. — Cho V là một B-môđun trái. Ký hiệu A-môđun trái $P\otimes_BV$ (II, §3, No. 4, p. 247) bởi $\mathscr{T}(V)$. Luật tác động trên $\mathscr{T}(V)$ được cho bởi công thức

$$
a(p\otimes v) = (ap)\otimes v \tag{1}
$$

với $a\in A,p\in P$, và $v\in V$.

Cho $V'$ là một B-môđun trái. Với mọi ánh xạ B-tuyến tính $g$ từ V đến $V'$, ánh xạ $1_P\otimes g$ từ $\mathscr{T}(V)$ đến $\mathscr{T}(V')$ là A-tuyến tính; ta ký hiệu nó bởi $\mathscr{T}(g)$. Ánh xạ $g\mapsto \mathscr{T}(g)$ từ Hom$_B(V,V')$ đến Hom$_A(\mathscr{T}(V),\mathscr{T}(V'))$ là $\mathbf{Z}$-tuyến tính, và ta có

$$
\mathscr{T}(1_V) = 1_{\mathscr{T}(V)},\mathscr{T}(g'\circ g) =\mathscr{T}(g')\circ \mathscr{T}(g) \tag{2}
$$

nếu $V, V', V''$ là các B-môđun trái và $g: V\rightarrow V',g': V'\rightarrow V''$ là các ánh xạ B-tuyến tính. Vì tích tenxơ giao hoán với các tổng trực tiếp, nên nếu V là tổng trực tiếp của một họ các môđun con $(V_i)_{i\in I}$, thì có thể đồng nhất A-môđun $\mathscr{T}(V)$ với $\bigoplus_i\mathscr{T}(V_i)$.

3.2. Phép toán $\mathscr{H}$. — Cho M là một A-môđun trái. Ký hiệu B-môđun trái Hom$_A(P,M)$ (II, §1, No. 14, p. 225) bởi $\mathscr{H}(M)$. Luật tác động trên $\mathscr{H}(M)$ được cho bởi công thức

$$
(bf)(p) =f(pb) \tag{3}
$$

với $b\in B,f\in$ Hom$_A(P,M)$, và $p\in P$.

Cho $M'$ là một A-môđun trái. Với mọi ánh xạ A-tuyến tính $g$ từ M vào $M'$, ánh xạ Hom$_A(1_P, g)$ từ $\mathscr{H}(M)$ vào $\mathscr{H}(M')$ là B-tuyến tính; ta ký hiệu nó bởi $\mathscr{H}(g)$. Ánh xạ $g\mapsto \mathscr{H}(g)$ từ Hom$_A(M,M')$ vào Hom$_B(\mathscr{H}(M),\mathscr{H}(M'))$ là $\mathbf{Z}$-tuyến tính, và ta có

$$
\mathscr{H}(1_M) = 1_{\mathscr{H}(M)},\mathscr{H}(g'\circ g) =\mathscr{H}(g')\circ \mathscr{H}(g) \tag{4}
$$

nếu $M, M', M''$ là các A-môđun trái và $g: M\rightarrow M',g': M'\rightarrow M''$ là các ánh xạ A-tuyến tính. Giả sử hơn nữa rằng P là một A-môđun hữu hạn sinh; nếu M là tổng trực tiếp của một họ các môđun con $(M_i)_i$, thì theo VIII, p. 57, ta có thể đồng nhất $\mathscr{H}(M)$ với $\bigoplus_i\mathscr{H}(M_i)$. 3.3. Quan hệ giữa $\mathscr{T}$ và $\mathscr{H}$. — Theo Mệnh đề 1 của II, §4, No. 1, p. 268, với mọi A-môđun trái M và mọi B-môđun trái V, tồn tại một đẳng cấu nhóm duy nhất

(5) $\gamma :$ Hom$_A(\mathscr{T}(V),M)\longrightarrow$ Hom$_B(V,\mathscr{H}(M))$

được đặc trưng bởi quan hệ

$$
(\gamma (h)(v))(p) =h(p\otimes v) \tag{6}
$$

với $h\in$ Hom$_A(\mathscr{T}(V),M),v\in V$, và $p\in P$. Đẳng cấu $\gamma$ được gọi là đẳng cấu liên hợp.

Cho M là một A-môđun trái. A-môđun $\mathscr{T}(\mathscr{H}(M))$ đơn giản là A-môđun $P\otimes_B$ Hom$_A(P,M)$. Bằng cách áp dụng điều trên cho B-môđun $\mathscr{H}$ (M), ta thấy rằng ánh xạ

$\alpha_M=\gamma^{-1}$(Id$_{\mathscr{H}(M)}$) $:\mathscr{T}(\mathscr{H}(M))\longrightarrow M$

là ánh xạ duy nhất thỏa mãn

$$
\alpha_M(p\otimes f) =f(p) \tag{7}
$$

với $p\in P$ và $f\in$ Hom$_A(P,M)$. Ta nói rằng $\alpha_M$ là ánh xạ A-tuyến tính chính tắc từ $\mathscr{T}(\mathscr{H}(M))$ tới M. Với mọi ánh xạ A-tuyến tính $g: M\rightarrow M'$, ta có một biểu đồ giao hoán

$\mathscr{T}(\mathscr{H}(M))^{\alpha_M}$ // M

(I) $\mathscr{T}_{(\mathscr{H}(g))}g$

$\mathscr{T}(\mathscr{H}(M'))^{\alpha_{M'}}$ // $M'$.

Nghịch đảo

$\gamma^{-1}:$ Hom$_B(V,\mathscr{H}(M))\longrightarrow$ Hom$_A(\mathscr{T}(V),M)$

của đẳng cấu liên hợp trùng với ánh xạ $h\mapsto \alpha_M\circ \mathscr{T}(h)$. Thật vậy, theo (6) và (7), ta có các hệ thức

$$
\gamma^{-1}(h)(p\otimes v) = (h(v))(p) =\alpha_M(p\otimes h(v)) =\alpha_M\circ \mathscr{T}(h)(p\otimes v)
$$

với mọi $h\in$ Hom$_B(V,\mathscr{H}$ (M)), $v\in V$, và $p\in P$.

Cho V là một B-môđun. B-môđun $\mathscr{H}(\mathscr{T}(V))$ đơn giản là B-môđun Hom$_A(P,P\otimes_BV)$. Áp dụng (5) cho A-môđun $\mathscr{T}$ (V), ta thấy ánh xạ B-tuyến tính $\beta_V=\gamma$(Id$_{\mathscr{T}(V)}$) từ V vào $\mathscr{H}(\mathscr{T}(V))$ được đặc trưng bởi quan hệ

$$
\beta_V(v)(p) =p\otimes v \tag{8}
$$

với $p\in P$ và $v\in V$. Ta gọi $\beta_V$ là ánh xạ B-tuyến tính chính tắc từ V vào $\mathscr{H}(\mathscr{T}(V))$. Với mọi B-môđun $V'$ và mọi ánh xạ B-tuyến tính $g: V\rightarrow V'$, ta có một biểu đồ giao hoán

V $^{\beta_V}$ /$/\mathscr{H}(\mathscr{T}(V))$

(II) $g\mathscr{H}_{\mathscr{T}}$

( $(g)$)

${V'}^{\beta_{V'}}$ /$/\mathscr{H}(\mathscr{T}(V'))$.

Chú ý rằng cấu xạ của phép nối (5) trùng với ánh xạ biến $u$ thành $\mathscr{H}(u)\circ \beta_V$. Thật vậy, từ các hệ thức (6) và (8), suy ra các đẳng thức

$$
(\gamma (u)(v))(p) =u(p\otimes v) =u\circ (\beta_V(v))(p)
$$

với mọi $u\in$ Hom$_A(\mathscr{T}(V),M),v\in V$, và $p\in P$.

#### Nhận xét 1 {#alg-viii-s4-n3-rem-1 .statement tag=004A}

Cho V và $V'$ là các B-môđun. Đẳng cấu liên hợp

$\gamma :$ Hom$_A(\mathscr{T}(V),\mathscr{T}(V'))\longrightarrow$ Hom$_B(V,\mathscr{H}(\mathscr{T}(V')))$

thỏa mãn hệ thức $\gamma (\mathscr{T}(f)) =\beta_{V'}\circ f$ với mọi $f\in$ Hom$_B(V,V')$ bởi vì

$$
(\gamma (\mathscr{T}(f))(v))(p) =\mathscr{T}(f)(p\otimes v) =p\otimes f(v) = (\beta_{V'}\circ f)(v)(p)
$$

Cho M và $M'$ là các A-môđun; nghịch đảo của đẳng cấu liên hợp

$\gamma^{-1}:$ Hom$_B(\mathscr{H}(M),\mathscr{H}(M'))\longrightarrow$ Hom$_A(\mathscr{T}(\mathscr{H}(M)),M')$

thỏa mãn hệ thức $\gamma^{-1}(\mathscr{H}(u)) =u\circ \alpha_M$ với mọi $u\in$ Hom$_B(M,M')$. Thật vậy, ta có các hệ thức

$$
\gamma^{-1}(\mathscr{H}(u))(p\otimes v) = (\mathscr{H}(u)(v))(p) =u(v(p)) =u\circ \alpha_M(p\otimes v)
$$

với mọi $u\in$ Hom$_B(M,M'),v\in \mathscr{H}$ (M), và $p\in P$.

#### Nhận xét 2 {#alg-viii-s4-n3-rem-2 .statement tag=004B}

Cho M là một A-môđun trái. Các ánh xạ B-tuyến tính

$\beta_{\mathscr{H}(M)}:\mathscr{H}(M)\rightarrow \mathscr{H}(\mathscr{T}(\mathscr{H}(M)))$ và $\mathscr{H}(\alpha_M) :\mathscr{H}(\mathscr{T}(\mathscr{H}(M)))\rightarrow \mathscr{H}(M)$ thỏa mãn quan hệ $\mathscr{H}(\alpha_M)\circ \beta_{\mathscr{H}(M)}= 1_{\mathscr{H}(M)}$. Nói chung, chúng không song ánh.

Cho V là một B-môđun trái. Các ánh xạ A-tuyến tính

$\mathscr{T}(\beta_V) :\mathscr{T}(V)\rightarrow \mathscr{T}(\mathscr{H}(\mathscr{T}(V)))$ và $\alpha_{\mathscr{T}(V)}:\mathscr{T}(\mathscr{H}(\mathscr{T}(V)))\rightarrow \mathscr{T}(V)$ thỏa mãn quan hệ $\alpha_{\mathscr{T}(V)}\circ \mathscr{T}(\beta_V) = 1_{\mathscr{T}(V)}$. Nói chung, chúng không song ánh.

#### Nhận xét 3 {#alg-viii-s4-n3-rem-3 .statement tag=004C}

Giả sử rằng P sinh hữu hạn như một A-môđun. Gọi M là tổng trực tiếp của một họ $(M_i)_{i\in I}$ các A-môđun. Các A-môđun $\mathscr{T}(\mathscr{H}(M))$ và $\bigoplus_i\mathscr{T}(\mathscr{H}(M_i))$ đẳng cấu chính tắc. Khi ta đồng nhất chúng, $\alpha_M$ được đồng nhất với $\bigoplus_i\alpha_{M_i}$. Tương tự, gọi V là tổng trực tiếp của một họ $(V_j)_{j\in J}$ các B-môđun. B-môđun $\mathscr{H}(\mathscr{T}(V))$ được đồng nhất với $\bigoplus_j\mathscr{H}(\mathscr{T}(V_j))$, và ánh xạ tuyến tính $\beta_V$ với $\bigoplus_j\beta_{V_j}$.

### 4. Các Môđun Đẳng Kiểu

Cho A là một vành và S là một A-môđun trái đơn. Gọi D là vành đối của vành tự đồng cấu của S; đó là một trường. Được trang bị các tác động của A và D, S là một $(A$, D)-song môđun.

#### Mệnh đề 1 {#alg-viii-s4-prop-1 .statement tag=004D}

Cho M là một A-môđun. Các tính chất sau là tương đương:

(i) Tồn tại một tập hợp I sao cho M đẳng cấu với $S^{(I)}$.

(ii) Môđun M là tổng trực tiếp của một họ các môđun con đẳng cấu với S.

(iii) Môđun M là tổng của một họ các môđun con đẳng cấu với S.

(iv) Tồn tại một không gian vectơ trái V trên trường D sao cho A-môđun M đẳng cấu với $S\otimes_DV$.

Tính tương đương của (i) và (ii) là ngay lập tức, và tính tương đương của (ii) và (iii) suy ra từ Định lý 1 của VIII, p. 56, áp dụng cho trường hợp N = 0. Mọi không gian vectơ trái trên D đều đẳng cấu với một không gian vectơ có dạng $D_s^{(I)}$, trong đó I là một tập hợp (II, §7, No. 1, p. 292, Định lý 1). Vì tích tenxơ giao hoán với các tổng trực tiếp, nên (i) tương đương với (iv).

#### Định nghĩa 2 {#alg-viii-s4-def-2 .statement tag=004E}

Một A-môđun M là đẳng kiểu kiểu S nếu nó có các tính chất tương đương của Mệnh đề 1. Môđun M được gọi là đẳng kiểu nếu tồn tại một A-môđun đơn T sao cho M là đẳng kiểu kiểu T.

Mọi môđun đẳng kiểu đều nửa đơn.

#### Mệnh đề 2 {#alg-viii-s4-prop-2 .statement tag=004F}

Nếu một môđun là tổng của các môđun con đẳng kiểu kiểu S, thì nó là đẳng kiểu kiểu S. Các môđun con và các môđun thương của một môđun đẳng kiểu kiểu S đều là đẳng kiểu kiểu S.

Mệnh đề thứ nhất suy ra từ các định nghĩa, mệnh đề thứ hai suy ra từ Hệ quả 3 của VIII, p. 56.

#### Nhận xét {#alg-viii-s4-n4-rem-1 .statement tag=004G}

Mọi môđun đẳng kiểu khác không kiểu S đều có một môđun thương và một môđun con đẳng cấu với S; do đó, nếu M và $M'$ là các A-môđun đẳng kiểu khác không kiểu S, thì nhóm Hom$_A(M,M')$ không bị rút gọn về 0.

#### Mệnh đề 3 {#alg-viii-s4-prop-3 .statement tag=004H}

a) Cho M là một A-môđun đẳng kiểu kiểu S. Ánh xạ A-tuyến tính $\alpha_M: S\otimes_D$Hom$_A(S,M)\rightarrow M$ được xác định bởi $\alpha_M(s\otimes f) =f(s)$ (VIII, p. 59) là song ánh.

b) Cho V là một không gian vectơ trái trên trường D. Ánh xạ D-tuyến tính $\beta_V: V\rightarrow$ Hom$_A(S,S\otimes_DV)$ được xác định bởi $\beta_V(v)(s) =s\otimes v$ (VIII, p. 59) là song ánh.

Ký hiệu không gian vectơ trái trên D Hom$_A(S,M)$ bởi $\mathscr{H}(M)$. Theo giả thiết, A-môđun M là tổng trực tiếp của một họ các môđun con đẳng cấu với S. A-môđun S là đơn sinh; do đó để chứng minh rằng ánh xạ $\alpha_M$ là song ánh, chỉ cần xét trường hợp M = S (VIII, p. 60, Nhận xét 3). Khi đó, $\mathscr{H}(S)$ đơn giản là không gian vectơ trên D $D_s$, và $\alpha_S$ đơn giản là đẳng cấu $\iota : S\otimes_DD_s\rightarrow S$ được xác định bởi $\iota (s\otimes d) =sd$.

Tương tự, để chứng minh b), chỉ cần xét trường hợp $V = D_s$. Vì ánh xạ $\alpha_S$ là song ánh, nên ánh xạ $\beta_{D_s}=\beta_{\mathscr{H}(S)}$ cũng vậy (VIII, p. 60, Nhận xét 2).

### 5. Mô tả một môđun đẳng kiểu

Như trong tiểu mục trước, A ký hiệu một vành, S một A-môđun đơn trái, và D trường End$_A(S)^o$. Ta xem S như một $(A$, D)-song môđun.

#### Định nghĩa 3 {#alg-viii-s4-def-3 .statement tag=004I}

Cho M là một A-môđun đẳng kiểu thuộc kiểu S. Một mô tả của M đối với S là một cặp $(V, \alpha )$, trong đó V là một không gian vectơ trái trên trường D và $\alpha : S\otimes_DV\rightarrow M$ là một đẳng cấu các A-môđun.

Mọi A-môđun đẳng kiểu M kiểu S đều có một mô tả chính tắc: đó là cặp (Hom$_A(S,M), \alpha_M$), trong đó $\alpha_M: S\otimes_D$ Hom$_A(S,M)\rightarrow M$ là đẳng cấu của các A-môđun được đặc trưng bởi $\alpha_M(s\otimes f) =f(s)$ (VIII, p. 62, Mệnh đề 3, a)).

#### Định lý 2 {#alg-viii-s4-thm-2 .statement tag=004J}

Cho M là một A-môđun đẳng kiểu kiểu S và $(V, \alpha )$ là một mô tả của M. Ký hiệu bởi $\mathscr{D}_D(V)$ tập hợp các không gian con D-tuyến tính của V, được sắp thứ tự bởi quan hệ bao hàm, và bởi $\mathscr{D}_A(M)$ tập hợp các A-môđun con của M. Với mọi $W\in$ $\mathscr{D}_D(V)$, đồng nhất A-môđun $S\otimes_DW$ với ảnh chính tắc của nó trong $S\otimes_DV$.

a) Ánh xạ $W\mapsto \alpha (S\otimes_DW)$ là một đẳng cấu của các tập hợp có thứ tự từ $\mathscr{D}_D(V)$ lên $\mathscr{D}_A(M)$.

b) Đẳng cấu nghịch đảo biến một môđun con N của M thành không gian con tuyến tính của V gồm các phần tử $v$ sao cho $\alpha (s\otimes v)$ thuộc về N với mọi $s\in S$.

Với $W\in \mathscr{D}_D$(V), đặt $\varphi (W) =\alpha (S\otimes_DW)$. Với $N\in \mathscr{D}_A$(M), ký hiệu bởi $\psi (N)$ tập hợp các phần tử $v\in V$ sao cho $\alpha (s\otimes v)\in N$ với mọi $s\in S$. Điều này xác định hai ánh xạ $\varphi :\mathscr{D}_D(V)\rightarrow \mathscr{D}_A(M)$ và $\psi :\mathscr{D}_A(M)\rightarrow \mathscr{D}_D(V)$. Chúng rõ ràng là tăng.

Cho N là một môđun con của M. Nó là đẳng kiểu kiểu S (VIII, p. 61, Mệnh đề 2). Đặt $W =\psi (N)$. Theo Mệnh đề 3, b) của VIII, p. 62, các ánh xạ A-tuyến tính $h: S\rightarrow M$ đơn giản là các ánh xạ $s\mapsto \alpha (s\otimes v)$, trong đó $v$ chạy qua V. Những ánh xạ có ảnh được chứa trong N là các ánh xạ $s\mapsto \alpha (s\otimes w)$ trong đó $w$ chạy qua W; các ảnh của chúng sinh ra N vì N là đẳng kiểu kiểu S. Do đó ta có $\alpha (S\otimes_DW) = N$, tức là $\varphi (\psi (N)) = N$. Điều đó chứng minh rằng $\varphi \circ \psi$ là ánh xạ đồng nhất trên $\mathscr{D}_A(M)$. Đặc biệt, $\varphi$ là toàn ánh và $\psi$ là đơn ánh.

Để hoàn tất chứng minh, chỉ cần chứng minh rằng ánh xạ $\varphi$ là đơn ánh. Cho W và $W'$ là các không gian con tuyến tính của V sao cho $\varphi (W) =\varphi (W')$. Các không gian vectơ $S\otimes_DW$ và $S\otimes_DW'$ trùng nhau khi được xem như các không gian con tuyến tính của $S\otimes_DV$. Chọn một dạng tuyến tính khác không $f$ trên không gian vectơ trên D S, và gọi $g: S\otimes_DV\rightarrow V$ là đồng cấu nhóm được xác định bởi $g(s\otimes v) =f(s)v$. Ta có $W =g(S\otimes_DW) =g(S\otimes_DW') = W'$, do đó $\varphi$ là đơn ánh.

#### Nhận xét 1 {#alg-viii-s4-n5-rem-1 .statement tag=004K}

Cho M là một A-môđun đẳng kiểu kiểu S và $(V, \alpha )$ một mô tả của M. Khi đó M có độ dài hữu hạn khi và chỉ khi V là hữu hạn chiều, và trong trường hợp này, ta có quan hệ

long$_A(M) =$ dim$_D(V)$.

#### Hệ quả 1 {#alg-viii-s4-thm-2-cor-1 .statement tag=004L}

Cho M là một A-môđun đẳng kiểu thuộc kiểu S. Với mọi A-môđun con N của M, đồng nhất Hom$_A(S,N)$ với không gian con tuyến tính của Hom$_A(S,M)$ gồm các ánh xạ có ảnh được chứa trong N.

a) Ánh xạ $N\mapsto$ Hom$_A(S,N)$ là một đẳng cấu của các tập hợp có thứ tự từ $\mathscr{D}_A(M)$ đến $\mathscr{D}_D$(Hom$_A(S,M)$).

b) Song ánh ngược gửi một không gian con tuyến tính W của Hom$_A(S,M)$ lên môđun con $\sum_{h\in W}h(S)$ của M.

Đây là một sự phát biểu lại của Định lý 2 khi ta lấy $(V, \alpha )$ làm mô tả chính tắc của M.

#### Hệ quả 2 {#alg-viii-s4-thm-2-cor-2 .statement tag=004M}

Cho V là một không gian vectơ trái trên D và $\mathscr{F}$ là một tập hợp các tự đồng cấu của V. Một A-môđun con của $S\otimes_DV$ ổn định đối với mọi tự đồng cấu $1_S\otimes u$, trong đó $u$ chạy qua $\mathscr{F}$, khi và chỉ khi nó có dạng $S\otimes_DW$, trong đó W là một không gian con tuyến tính của V ổn định đối với mọi tự đồng cấu thuộc $\mathscr{F}$.

Thật vậy, theo Định lý 2, mọi A-môđun con N của $S\otimes_DV$ đều bằng $S\otimes_DW$, trong đó W là không gian con tuyến tính của V gồm các phần tử $v$ sao cho $s\otimes v$ thuộc N với mọi $s\in S$.

#### Định lý 3 {#alg-viii-s4-thm-3 .statement tag=004N}

Cho M và $M'$ là các A-môđun đẳng kiểu kiểu S. Gọi $(V, \alpha )$ và $(V', \alpha ')$ lần lượt là các mô tả của M và $M'$. Với mọi ánh xạ D-tuyến tính $f: V\rightarrow V'$, ký hiệu bởi $\widetilde{f}: M\rightarrow M'$ ánh xạ A-tuyến tính duy nhất làm cho biểu đồ sau giao hoán:

$S\otimes_DV^{\alpha}$ // M

$$
1_{_S\otimes f}\widetilde{f} \tag{9}
$$

$S\otimes_D{V'}^{\alpha'}$ // $M'$.

Ánh xạ $f\mapsto \widetilde{f}$ từ Hom$_D(V,V')$ đến Hom$_A(M,M')$ là một đẳng cấu nhóm.

Chỉ cần chứng minh rằng ánh xạ $\mathbf{Z}$-tuyến tính $u\mapsto 1_S\otimes u$ từ Hom$_D(V,V')$ đến Hom$_A(S\otimes_DV,S\otimes_DV')$ là song ánh. Theo ký hiệu của No.3 áp dụng cho $(A$, D)-song môđun S, điều này quy về việc chỉ ra rằng ánh xạ

$\mathscr{T}:$ Hom$_D(V,V')\longrightarrow$ Hom$_A(\mathscr{T}(V),\mathscr{T}(V'))$

là song ánh. Nhưng theo Nhận xét 1 của VIII, p. 60, vì đẳng cấu liên hợp (VIII, p. 59) là song ánh, điều này quy về việc chỉ ra rằng ánh xạ biến $u$ thành $\beta_{V'}\circ u$ là song ánh, điều này suy ra từ việc ánh xạ D-tuyến tính $\beta_{V'}$ là song ánh (VIII, p. 62, Mệnh đề 3, b)).

Ta giữ ký hiệu của Định lý 3. Cho $M''$ là một A-môđun đẳng kiểu kiểu S, và cho $(V'', \alpha '')$ là một mô tả của $M''$. Với mọi $f\in$ Hom$_D(V,V')$ và mọi $g\in$ Hom$_D(V',V'')$, ta có $g]\circ f=\widetilde{g}\circ \widetilde{f}$. Đặc biệt, với $M = M'$, $V = V'$, và $\alpha =\alpha '$, ánh xạ $f\mapsto \widetilde{f}$ từ End$_D(V)$ đến End$_A(M)$ là một đẳng cấu vành.

#### Nhận xét 2 {#alg-viii-s4-n5-rem-2 .statement tag=004O}

Cho M là một A-môđun đẳng kiểu kiểu S, và cho $(V, \alpha )$ là một mô tả của M. Cho B là một vành con của vành End$_A(M)^o$. Đẳng cấu vành từ End$_D(V)^o$ tới End$_A(M)^o$ trang bị cho V cấu trúc của một $(D$, B)-song môđun, sao cho $\alpha$ là một đẳng cấu của các $(A$, B)-song môđun. Có một đẳng cấu từ tập hợp các $(D$, B)-song môđun con của V, có thứ tự bởi bao hàm, tới tập hợp các $(A$, B)-song môđun con của M (VIII, p. 62, Định lý 2 and VIII, p. 63, Hệ quả 2).

#### Hệ quả {#alg-viii-s4-n5-cor-1 .statement tag=004P}

Cho M và $M'$ là các A-môđun đẳng kiểu thuộc kiểu S. Ánh xạ $u\mapsto$ Hom(1$_S, u$) từ Hom$_A(M,M')$ vào Hom$_D$(Hom$_A(S,M)$, Hom$_A(S,M')$) là một đẳng cấu nhóm. Khi M bằng $M'$, đó là một đẳng cấu vành từ End$_A(M)$ lên End$_D$(Hom$_A(S,M)$).

Do tính giao hoán của biểu đồ (I) trong VIII, p. 59, hệ quả này suy ra từ Định lý 3, áp dụng cho các mô tả chính tắc của M và $M'$.

### 6. Các thành phần đẳng kiểu của một môđun

#### Định nghĩa 4 {#alg-viii-s4-def-4 .statement tag=004Q}

Cho A là một vành, M là một A-môđun, và S là một A-môđun đơn. Thành phần đẳng kiểu thuộc kiểu S của M, ký hiệu bởi $M_S$, là tổng của các môđun con của M đẳng cấu với S.

Rõ ràng $M_S$ là môđun con lớn nhất của M đẳng kiểu kiểu S. Vì mọi môđun con của $M_S$ đều đẳng kiểu kiểu S (VIII, p. 61, Mệnh đề 2), ta có $N_S= M_S\cap N$ với mọi môđun con N của M.

Nếu $S'$ là một A-môđun đơn đẳng cấu với S, thì rõ ràng ta có $M_S=$ $M_{S'}$, nên $M_S$ chỉ phụ thuộc vào lớp của S (VIII, p. 51).

Cho M là một A-môđun. Tồn tại một môđun con nửa đơn lớn nhất của M, gọi là đế của M; nó là tổng của các môđun con đơn của M và cũng là tổng của các thành phần đẳng kiểu của M. Đặc biệt, M là nửa đơn khi và chỉ khi nó bằng đế của nó.

#### Mệnh đề 4 {#alg-viii-s4-prop-4 .statement tag=004R}

Cho A là một vành. Ký hiệu tập hợp các lớp của các A-môđun đơn là $\mathscr{S}$. Cho M là một A-môđun nửa đơn.

a) Môđun M là tổng trực tiếp của họ $(M_{\lambda})_{\lambda\in\mathscr{S}}$ các thành phần đẳng kiểu của nó.

b) Giả sử rằng M là tổng trực tiếp của một họ $(N_i)_{i\in I}$ các môđun con đơn. Với mọi $\lambda \in \mathscr{S}$, gọi $I(\lambda )$ là tập hợp các chỉ số $i\in I$ sao cho $N_i$ thuộc lớp $\lambda$. Ta có $M_{\lambda}=\bigoplus_{i\in I(\lambda)}N_i$.

c) Nếu M sinh hữu hạn, thì tập hợp các $\lambda \in \mathscr{S}$ sao cho $M_{\lambda}\not= 0$ là hữu hạn.

d) Với mọi môđun con N của M và mọi $\lambda \in \mathscr{S}$, ta có $N_{\lambda}= N\cap M_{\lambda}$ và $(M/N)_{\lambda}= (M_{\lambda}+ N)/N$.

Vì M là nửa đơn, nó là tổng của họ $(M_{\lambda})_{\lambda\in\mathscr{S}}$; hãy chứng minh rằng tổng này là trực tiếp. Cho $\lambda \in \mathscr{S}$. Ký hiệu tổng của họ $(M_\mu)_{\mu\in\mathscr{S}-\{\lambda\}}$ là $M'_{\lambda}$. Môđun $M'_{\lambda}$ là tổng trực tiếp của một họ các môđun đơn không đẳng cấu với $\lambda$ (VIII, p. 56, Định lý 1). Theo Hệ quả 3 của Định lý 1 của VIII, p. 56, $M'_{\lambda}$ không chứa môđun con đơn nào thuộc lớp $\lambda$. Do đó ta có $M_{\lambda}\cap M'_{\lambda}= 0$. Vậy mệnh đề a) được chứng minh. Theo phép dựng, ta có $M_{\lambda}\supset \bigoplus_{i\in I(\lambda)}N_i$, nên mệnh đề b) suy ra từ Nhận xét 1 của II, §1, No. 8, p. 208.

Mệnh đề c) suy ra từ a) và Mệnh đề 23 của II, §1, No. 12, p. 221.

Cho N là một môđun con của M và $\lambda \in \mathscr{S}$. Thành phần đẳng kiểu $N_{\lambda}$ kiểu $\lambda$ của N được chứa trong $M_{\lambda}$ và $M_{\lambda}\cap N\subset N_{\lambda}$. Do đó giao $N\cap M_{\lambda}$ là thành phần đẳng kiểu của N kiểu $\lambda$.

Với mọi $\lambda \in \mathscr{S}$, môđun $M_{\lambda}+N/N$ đẳng cấu với $M_{\lambda}/(M_{\lambda}\cap N)$. Vì vậy nó là đẳng kiểu kiểu $\lambda$ và được chứa trong $(M/N)_{\lambda}$. Khẳng định cuối cùng khi đó suy ra từ a) và II, §1, No. 8, p. 208, Nhận xét 1.

#### Hệ quả {#alg-viii-s4-n6-cor-1 .statement tag=004S}

Cho A là một vành và $\mathscr{S}$ là tập hợp các lớp của các A-môđun đơn. Cho M là một A-môđun nửa đơn và N là một môđun con của M. Khi đó ta có $N =\bigoplus_{\lambda\in\mathscr{S}}N\cap M_{\lambda}$ và $M/N =\bigoplus_{\lambda\in\mathscr{S}}(M_{\lambda}+ N)/N$.

Vì N và $M/N$ là nửa đơn (VIII, p. 56, Hệ quả 3), hệ quả suy ra từ Mệnh đề 4, d).

Giá của A-môđun nửa đơn M là tập hợp các lớp $\lambda$ của các A-môđun đơn sao cho thành phần đẳng kiểu của M kiểu $\lambda$ là khác không. Giá của một A-môđun nửa đơn sinh hữu hạn là hữu hạn.

#### Mệnh đề 5 {#alg-viii-s4-prop-5 .statement tag=004T}

Cho A là một vành, và $\mathscr{S}$ là tập hợp các lớp của các A-môđun đơn. Cho M và N là các A-môđun.

a) Cho $f: M\rightarrow N$ là một đồng cấu. Với mọi $\lambda \in \mathscr{S},f$ cảm sinh một đồng cấu $f_{\lambda}$ từ $M_{\lambda}$ đến $N_{\lambda}$; nếu M là nửa đơn và $f$ toàn ánh, thì mỗi đồng cấu $f_{\lambda}$ đều toàn ánh.

b) Giả sử rằng M là nửa đơn. Ánh xạ $f\mapsto (f_{\lambda})_{\lambda\in\mathscr{S}}$ là một đẳng cấu nhóm từ Hom$_A(M,N)$ lên $\prod_{\lambda\in\mathscr{S}}$ Hom$_A(M_{\lambda},N_{\lambda})$. Khi M bằng N, ánh xạ này là một đẳng cấu vành từ End$_A(M)$ lên $\prod_{\lambda\in\mathscr{S}}$ End$_A(M_{\lambda})$.

Với mọi $\lambda \in \mathscr{S}$, môđun con $f(M_{\lambda})$ của N đẳng cấu với một thương của một môđun đẳng kiểu kiểu $\lambda$; do đó nó là đẳng kiểu kiểu $\lambda$ và, do đó, được chứa trong $N_{\lambda}$.

Giả sử rằng M là nửa đơn và $f$ toàn ánh. Khi đó $f$ cảm sinh một đẳng cấu từ $M/$ Ker($f$) lên N biến $(M_{\lambda}$+Ker($f$))$/$ Ker($f$) thành $f(M_{\lambda})$. Theo Mệnh đề 4 của VIII, p. 65, ta có $N_{\lambda}=f(M_{\lambda})$, điều này hoàn tất chứng minh của a).

Ánh xạ được xét trong b) rõ ràng là một đồng cấu nhóm, và là một đồng cấu vành khi M bằng N. Cho $(f_{\lambda})_{\lambda\in\mathscr{S}}$ là một phần tử của $\prod_{\lambda\in\mathscr{S}}$ Hom(M$_{\lambda},N_{\lambda}$). Phần tử duy nhất của ảnh ngược của nó qua ánh xạ trong b) là đồng cấu $f: M\rightarrow N$ được xác định bởi

$$
f((\sum_{\lambda\in\mathscr{S}}x_{\lambda})=\sum_{\lambda\in\mathscr{S}}f_{\lambda}(x_{\lambda})
$$

với mọi $(x_{\lambda})_{\lambda\in\mathscr{S}}\in \bigoplus_{\lambda}M_{\lambda}$.

#### Nhận xét {#alg-viii-s4-n6-rem-1 .statement tag=004U}

Cho A và B là các vành. Cho M là một song môđun $(A$, B). Suy ra từ Mệnh đề 5 rằng các thành phần đẳng kiểu của A-môđun M là các song môđun con của M. Điều này đúng, đặc biệt, khi M là một A-môđun và B là vành đối của End$_A(M)$.

#### Ví dụ {#alg-viii-s4-n6-exa-1 .statement tag=004V}

Xét trường hợp vành A là giao hoán. Ánh xạ gửi một iđêan cực đại $\mathfrak{m}$ lên cl(A$/\mathfrak{m}$) là một song ánh từ tập hợp các iđêan cực đại của A tới tập hợp $\mathscr{S}$ các lớp của các A-môđun đơn (VIII, p. 51). Song ánh ngược gửi $\lambda$ tới linh hóa tử của nó $\mathfrak{m}_{\lambda}$.

Cho M là một A-môđun. Với mọi $\lambda \in \mathscr{S}$, thành phần đẳng kiểu $M_{\lambda}$ kiểu $\lambda$ của M gồm các phần tử bị triệt tiêu bởi $\mathfrak{m}_{\lambda}$, và ta có thể xem $M_{\lambda}$ như một không gian vectơ trên trường $A/\mathfrak{m}_{\lambda}$. Nếu M là nửa đơn và N là một A-môđun khác, thì từ Mệnh đề 5 ta suy ra một đẳng cấu nhóm từ Hom$_A(M,N)$ tới $\prod_{\lambda\in\mathscr{S}}$ Hom$_{A/\mathfrak{m}_{\lambda}}(M_{\lambda},N_{\lambda})$.

#### Hệ quả 1 {#alg-viii-s4-prop-5-cor-1 .statement tag=004W}

Cho M là một A-môđun nửa đơn và N là một môđun con của M. Các tính chất sau là tương đương:

(i) Tồn tại duy nhất một môđun con phụ với N trong M.

(ii) Ta có Hom$_A(M/N,N) = 0$.

(iii) Tồn tại một tập con Λ của $\mathscr{S}$ sao cho $N =\bigoplus_{\lambda\in\Lambda}M_{\lambda}$.

Chọn một môđun con $N'$ bổ sung cho N trong M (VIII, p. 56, Hệ quả 2). Nếu đồng nhất M với $N'\times N$, thì các môđun con của M bổ sung cho N là các đồ thị của các ánh xạ A-tuyến tính từ $N'$ đến N. Vì $N'$ đẳng cấu với $M/N$, ta đã chứng minh được tính tương đương của các tính chất (i) và (ii). Theo Mệnh đề 5, b), nhóm Hom$_A(N',N)$ đẳng cấu với nhóm $\prod_{\lambda\in\mathscr{S}}$ Hom$_A(N'_{\lambda},N_{\lambda})$. Nhóm này bằng không khi và chỉ khi với mọi $\lambda \in \mathscr{S}$, ta có $N_{\lambda}= 0$ hoặc $N'_{\lambda}= 0$ (VIII, p. 61, Nhận xét), nghĩa là $N_{\lambda}= 0$ hoặc $N_{\lambda}= M_{\lambda}$. Điều này chứng minh tính tương đương của các tính chất (ii) và (iii).

#### Hệ quả 2 {#alg-viii-s4-prop-5-cor-2 .statement tag=00R0}

Cho M là một A-môđun. Hai điều kiện sau tương đương:

(i) Mọi môđun con của M đều có một môđun con bổ sung duy nhất.

(ii) Môđun M là tổng trực tiếp của một họ $(S_i)_{i\in I}$ các môđun đơn, từng đôi một không đẳng cấu.

Giả sử rằng M thỏa mãn các điều kiện này. Khi đó, với mọi môđun con N của M, tồn tại duy nhất một tập con J của I sao cho ta có $N =\bigoplus_{j\in J}S_j$ và mọi môđun con đơn của M đều bằng một trong các $S_i$.

Các điều kiện (i) và (ii) đều suy ra rằng M là nửa đơn.

Giả sử rằng điều kiện (i) được thỏa mãn. Cho $\lambda \in \mathscr{S}$. Theo sự tương đương của (i) và (iii) trong Hệ quả 1, mọi môđun con của $M_{\lambda}$ đều bằng không hoặc bằng $M_{\lambda}$. Do đó, $M_{\lambda}$ bằng không hoặc đơn, và (ii) suy ra từ việc M là tổng trực tiếp của họ $(M_{\lambda})_{\lambda\in\mathscr{S}}$.

Ngược lại, nếu điều kiện (ii) được thỏa mãn, thì $M_{\lambda}$ bằng không hoặc đơn với mọi $\lambda \in \mathscr{S}$. Nếu N là một môđun con của M, thì $N\cap M_{\lambda}$ bằng 0 hoặc $M_{\lambda}$ với mọi $\lambda \in \mathscr{S}$. Vì ta có $N =\bigoplus_{\lambda\in\mathscr{S}}(N\cap M_{\lambda})$ (VIII, p. 66, Hệ quả), môđun con N có tính chất (iii) của Hệ quả 1 và vì thế thừa nhận một môđun con bổ sung duy nhất trong M. Điều này chứng minh rằng (ii) suy ra (i), cũng như các khẳng định cuối cùng của hệ quả.

Cho M là một A-môđun và S là một A-môđun đơn. Ký hiệu vành đối của trường End$_A(S)$ bởi D, và xem S như một song môđun $(A$, D). Khi đó Hom$_A(S,M)$ là một không gian vectơ trái trên D, và Hom$_A(M,S)$ là một không gian vectơ phải trên D. Đối ngẫu của không gian vectơ trái trên D Hom$_A(S,M)$ là một không gian vectơ phải trên D (II, §2, No. 3, p. 232, Định nghĩa 2). Với mọi $u\in$ Hom$_A(M,S)$, ánh xạ $h(u) :v\mapsto u\circ v$ từ Hom$_A(S,M)$ vào Hom$_A(S,S) = D$ là một dạng tuyến tính trên không gian vectơ trái trên D Hom$_A(S,M)$.

#### Mệnh đề 6 {#alg-viii-s4-prop-6 .statement tag=004X}

Giữ ký hiệu ở trên, và giả sử rằng A-môđun M là nửa đơn. Ánh xạ $u\mapsto h(u)$ từ không gian vectơ phải trên D Hom$_A(M,S)$ vào đối ngẫu của không gian vectơ trái trên D Hom$_A(S,M)$ là D-tuyến tính và song ánh.

Cho $u\in$ Hom$_A(M,S),v\in$ Hom$_A(S,M)$, và $d\in D$. Ta có

$$
h(ud)(v) =h(d\circ u)(v) =d\circ u\circ v=d\circ (h(u)(v)) =h(u)(v)d
$$

Điều này chứng tỏ rằng ánh xạ $h$ là D-tuyến tính. Nó đơn giản là ánh xạ được cho bởi $u\mapsto$ Hom(1$_S, u$) từ Hom$_A(M,S)$ đến Hom$_D$(Hom$_A(S,M)$, Hom$_A(S,S)$). Để chứng minh rằng nó là song ánh, theo Mệnh đề 5, b) của VIII, p. 66, chỉ cần xét trường hợp M là đẳng kiểu kiểu S; khi đó ta có thể áp dụng hệ quả của VIII, p. 65.

### 7. Mô tả một môđun nửa đơn

Trong phần còn lại của tiết này, A là một vành, và $\mathscr{S}$ là tập hợp các lớp của các A-môđun đơn. Với mọi $\lambda \in \mathscr{S}$, ta chọn một môđun đơn $S_{\lambda}$ thuộc lớp $\lambda$ (chẳng hạn, $S_{\lambda}=\lambda$ ); ta ký hiệu vành đối của trường các tự đồng cấu của $S_{\lambda}$ bởi $D_{\lambda}$. Ta xem $S_{\lambda}$ như một $(A,D_{\lambda}$)-song môđun.

Cho M là một A-môđun. Với mọi $\lambda \in \mathscr{S}$, Hom$_A(S_{\lambda},M)$ là một không gian vectơ trái trên trường $D_{\lambda}$. Theo VIII, p. 59, và II, §1, No. 6, p. 202, Mệnh đề 6, tồn tại một ánh xạ A-tuyến tính duy nhất, gọi là chính tắc,

$\alpha_M:\bigoplus_{\lambda\in\mathscr{S}}(S_{\lambda}\otimes_{D_{\lambda}}$ Hom$_A(S_{\lambda},M))\rightarrow M$

thỏa mãn quan hệ

$$
\alpha_M(s\otimes f) =f(s) \tag{10}
$$

với $\lambda \in \mathscr{S},s\in S_{\lambda}$, và $f\in$ Hom$_A(S_{\lambda},M)$. Nếu ta trang bị cho $\bigoplus_{\lambda\in\mathscr{S}}(S_{\lambda}\otimes_{D_{\lambda}}$ Hom$_A(S_{\lambda},M))$ và M các cấu trúc tự nhiên của các End$_A$(M)-môđun, thì ánh xạ $\alpha_M$ là End$_A$(M)-tuyến tính.

#### Mệnh đề 7 {#alg-viii-s4-prop-7 .statement tag=004Y}

Cho M là một A-môđun. Ánh xạ chính tắc $\alpha_M$ là đơn ánh. Với mọi $\lambda \in \mathscr{S}$, ảnh qua $\alpha_M$ của $S_{\lambda}\otimes_{D_{\lambda}}$ Hom$_A(S_{\lambda},M)$ là thành phần đẳng kiểu của M thuộc kiểu $\lambda$. Ảnh của $\alpha_M$ là đế của M. A-môđun M là nửa đơn khi và chỉ khi ánh xạ $\alpha_M$ là song ánh.

Cho $\lambda \in \mathscr{S}$. Ký hiệu thành phần đẳng kiểu của M thuộc kiểu $\lambda$ là $M_{\lambda}$. Mọi ánh xạ A-tuyến tính từ $S_{\lambda}$ vào M đều nhận giá trị trong $M_{\lambda}$ (VIII, p. 66, Mệnh đề 5). Do đó, theo Mệnh đề 3, a) của VIII, p. 62, ánh xạ $\alpha_M$ cảm sinh một song ánh từ $S_{\lambda}\otimes_{D_{\lambda}}$ Hom$_A(S_{\lambda},M)$ lên $M_{\lambda}$. Mệnh đề được suy ra vì đế của M là tổng trực tiếp của họ $(M_{\lambda})_{\lambda\in\mathscr{S}}$ và môđun M là nửa đơn khi và chỉ khi nó bằng đế của nó.

#### Định nghĩa 5 {#alg-viii-s4-def-5 .statement tag=004Z}

Cho M là một A-môđun nửa đơn. Một mô tả của M (đối với họ $(S_{\lambda})_{\lambda\in\mathscr{S}}$) là một cặp $((V_{\lambda})_{\lambda\in\mathscr{S}}, \alpha )$, trong đó $V_{\lambda}$ là một không gian vectơ trái trên trường $D_{\lambda}$ với mỗi $\lambda \in \mathscr{S}$ và $\alpha :\bigoplus_{\lambda\in\mathscr{S}}(S_{\lambda}\otimes_{D_{\lambda}}V_{\lambda})\rightarrow M$ là một đẳng cấu của các A-môđun.

Theo Mệnh đề 7, mọi A-môđun nửa đơn M đều có một mô tả chính tắc: đó là cặp ((Hom$_A(S_{\lambda},M)$)$_{\lambda\in\mathscr{S}}, \alpha_M$), trong đó $\alpha_M$ là ánh xạ A-tuyến tính được xác định bởi công thức (10).

#### Mệnh đề 8 {#alg-viii-s4-prop-8 .statement tag=0050}

Cho M là một A-môđun nửa đơn và $((V_{\lambda})_{\lambda\in\mathscr{S}}, \alpha )$ là một mô tả của M.

a) Với mọi $\lambda \in \mathscr{S}$, ánh xạ $\alpha$ cảm sinh một đẳng cấu từ A-môđun $S_{\lambda}\otimes_{D_{\lambda}}V_{\lambda}$ lên thành phần đẳng kiểu của M thuộc kiểu $\lambda$.

b) Với mọi $\lambda \in \mathscr{S}$, ánh xạ $\beta_{\lambda}: V_{\lambda}\rightarrow$ Hom$_A(S_{\lambda},M)$ được xác định bởi $\beta_{\lambda}(v)(s) =\alpha (s\otimes v)$ là $D_{\lambda}$-tuyến tính và song ánh.

c) Cho N là một môđun con của M. Tồn tại một họ duy nhất $(W_{\lambda})_{\lambda\in\mathscr{S}}$ có các tính chất sau: $W_{\lambda}$ là một không gian con $D_{\lambda}$-tuyến tính của $V_{\lambda}$ với mọi $\lambda \in \mathscr{S}$, và N là ảnh bởi $\alpha$ của môđun $\bigoplus_{\lambda\in\mathscr{S}}(S_{\lambda}\otimes_{D_{\lambda}}W_{\lambda})$ được đồng nhất với ảnh chính tắc của nó trong môđun $\bigoplus_{\lambda\in\mathscr{S}}(S_{\lambda}\otimes_{D_{\lambda}}V_{\lambda})$. Với mọi $\lambda \in \mathscr{S},W_{\lambda}$ là tập hợp các phần tử $v\in V_{\lambda}$ sao cho $\alpha (s\otimes v)$ thuộc N với mọi $s\in S_{\lambda}$.

A-môđun $S_{\lambda}\otimes_{D_{\lambda}}V_{\lambda}$ là đẳng kiểu kiểu $\lambda$ với mọi $\lambda \in \mathscr{S}$. Khi đó mệnh đề a) suy ra từ các sự kiện rằng $\alpha$ là một đẳng cấu và M là tổng trực tiếp của họ $(M_{\lambda})_{\lambda\in\mathscr{S}}$ (VIII, p. 65, Mệnh đề 4, a)).

Cho $\lambda \in \mathscr{S}$. Ký hiệu hạn chế của $\alpha$ lên $S_{\lambda}\otimes_{D_{\lambda}}V_{\lambda}$ bởi $\alpha_{\lambda}: S_{\lambda}\otimes_{D_{\lambda}}V_{\lambda}\rightarrow$ M. Với ký hiệu của No. 3 áp dụng cho song môđun $(A,D_{\lambda}$)-$S_{\lambda}$, ta có

$$
\beta_{\lambda}=\gamma (\alpha_{\lambda}) =\mathscr{H}(\alpha_{\lambda})\circ \beta_{V_{\lambda}}
$$

trong đó đẳng thức cuối cùng suy ra từ VIII, p. 60. Do đó, $\beta_{\lambda}$ là hợp thành của đồng cấu $D_{\lambda}$-tuyến tính $\mathscr{H}(\alpha_{\lambda})$ và $\beta_{V_{\lambda}}$. Khi đó mệnh đề b) suy ra từ Mệnh đề 3, b) của VIII, p. 62.

Cho N là một môđun con của M. Ta có $N =\bigoplus_{\lambda\in\mathscr{S}}(N\cap M_{\lambda})$ (VIII, p. 66, Hệ quả), do đó c) suy ra từ Định lý 2 của VIII, p. 62.

#### Hệ quả {#alg-viii-s4-n7-cor-1 .statement tag=0051}

Cho M là một A-môđun nửa đơn. Với mọi môđun con N của M và mọi phần tử $\lambda$ của $\mathscr{S}$, đồng nhất Hom$_A(S_{\lambda},N)$ với không gian con $D_{\lambda}$-tuyến tính của Hom$_A(S_{\lambda},M)$ gồm các ánh xạ có ảnh được chứa trong N.

a) Ánh xạ $N\mapsto$ (Hom$_A(S_{\lambda},N)$)$_{\lambda\in\mathscr{S}}$ là một song ánh từ tập hợp các A-môđun con của M lên tập hợp các họ $(W_{\lambda})_{\lambda\in\mathscr{S}}$ sao cho với mọi $\lambda \in \mathscr{S}$, $W_{\lambda}$ là một không gian con tuyến tính trên $D_{\lambda}$ của Hom$_A(S_{\lambda},M)$.

b) Song ánh ngược biến một họ $(W_{\lambda})_{\lambda\in\mathscr{S}}$ thành A-môđun con $\sum_{\lambda\in\mathscr{S}}\sum_{w\in W_{\lambda}}w(S_{\lambda})$ của M.

Đây là một cách phát biểu lại của Mệnh đề 8, c), áp dụng cho mô tả chính tắc của M.

#### Mệnh đề 9 {#alg-viii-s4-prop-9 .statement tag=0052}

Cho M và $M'$ là các A-môđun nửa đơn, và xét các mô tả $((V_{\lambda})_{\lambda\in\mathscr{S}}, \alpha )$ và $((V'_{\lambda})_{\lambda\in\mathscr{S}}, \alpha ')$ của M và $M'$, tương ứng. Với mọi họ $\boldsymbol{f}= (f_{\lambda})_{\lambda\in\mathscr{S}}$ trong $\prod_{\lambda\in\mathscr{S}}$ Hom$_{D_{\lambda}}(V_{\lambda},V_{\lambda}')$, tồn tại một ánh xạ A-tuyến tính duy nhất $\varphi (\boldsymbol{f})\in$ Hom$_A(M,M')$ sao cho biểu đồ sau giao hoán:

$\bigoplus(S_{\lambda}\otimes_DV_{\lambda})^{\alpha}$ // M

$$
\lambda \in \mathscr{S}\lambda
$$

$$
\bigoplus(1_S\otimes f_{\lambda})
$$

$$
_{\lambda}\varphi (\boldsymbol{f})
$$

$\lambda \in \mathscr{S}$

$\bigoplus(S_{\lambda}\otimes_DV'_{\lambda})^{\alpha'}$ // $M'$.

$\lambda \in \mathscr{S}\lambda$

Ánh xạ $\varphi :\prod_{\lambda\in\mathscr{S}}$ Hom$_{D_{\lambda}}(V_{\lambda},V'_{\lambda})\rightarrow$ Hom$_A(M,M')$ được xác định như vậy là một đẳng cấu nhóm. Khi có $M = M',V_{\lambda}= V'_{\lambda}$ với mọi $\lambda \in \mathscr{S}$, và $\alpha =\alpha '$, ánh xạ $\varphi$ là một đẳng cấu vành từ $\prod_{\lambda\in\mathscr{S}}$ End$_{D_{\lambda}}(V_{\lambda})$ lên End$_A(M)$.

Theo mô tả các thành phần đẳng kiểu của M và $M'$ đã cho trong Mệnh đề 8, a), điều này suy ra từ Định lý 3 của VIII, p. 64 và Mệnh đề 5, b) của VIII, p. 66.

#### Hệ quả {#alg-viii-s4-n7-cor-2 .statement tag=0053}

Cho M là một A-môđun nửa đơn và $M'$ là một A-môđun. Ánh xạ $u\mapsto$ (Hom(1$_{S_{\lambda}}, u$))$_{\lambda\in\mathscr{S}}$ từ Hom$_A(M,M')$ đến

$\prod_{\lambda\in\mathscr{S}}$ Hom$_{D_{\lambda}}$(Hom$_A(S_{\lambda},M)$, Hom$_A(S_{\lambda},M')$)

là một đẳng cấu nhóm. Khi $M'$ bằng M, nó là một đẳng cấu từ vành End$_A(M)$ đến vành $\prod_{\lambda\in\mathscr{S}}$ End$_{D_{\lambda}}$(Hom$_A(S_{\lambda},M)$).

Đây là một sự phát biểu lại của Mệnh đề 9 áp dụng cho các mô tả chính tắc của M và của đế của $M'$.

### 8. Bội số và Độ dài trong các môđun nửa đơn

#### Mệnh đề 10 {#alg-viii-s4-prop-10 .statement tag=0054}

Cho M là một A-môđun nửa đơn. Cho $(M_i)_{i\in I}$ là một họ các môđun con đơn có tổng trực tiếp là M. Các tính chất sau là tương đương:

(i) M có độ dài hữu hạn.

(ii) M là Artin.

(iii) M là Noether.

(iv) M sinh hữu hạn.

(v) I là hữu hạn.

Nếu M có các tính chất này, thì độ dài của M bằng lực lượng của I.

Nếu tập hợp I là hữu hạn, thì M có các tính chất (i), (ii), (iii) và (iv). Giả sử rằng tập hợp I là vô hạn. Theo Ví dụ 2 của VIII, p. 2, môđun M không là Artin cũng không là Noether; vì mọi môđun có độ dài hữu hạn đều là Artin và Noether (VIII, p. 2, Mệnh đề 1), nên M cũng không có độ dài hữu hạn. Sau cùng, mọi phần tử của M đều thuộc vào tổng của một số hữu hạn môđun con $M_i$, vì thế M không sinh hữu hạn. Điều này chứng minh tính tương đương của các tính chất từ (i) đến (v). Nếu các tính chất này được thỏa mãn, thì ta có long(M) $=\sum_{i\in I}$ long(M$_i$) $=$ Card(I) (II, §1, No. 10, p. 213, Hệ quả 5).

#### Mệnh đề 11 {#alg-viii-s4-prop-11 .statement tag=0055}

Cho M là một A-môđun nửa đơn là tổng trực tiếp của một họ $(M_i)_{i\in I}$ các môđun con đơn. Với mọi $\lambda \in \mathscr{S}$, ta ký hiệu bởi $I(\lambda )$ tập hợp các chỉ số $i\in I$ sao cho $M_i$ thuộc lớp $\lambda$. Lực lượng của $I(\lambda )$ bằng chiều của không gian vectơ trái $D_{\lambda}$ Hom$_A(S_{\lambda},M)$.

Thành phần đẳng kiểu của A kiểu $\lambda$ đẳng cấu với $S_{\lambda}^{(I(\lambda))}$ (VIII, p. 65, Mệnh đề 4, b)). Không gian vectơ $D_{\lambda}$ Hom$_A(S_{\lambda},M)$ có thể được đồng nhất với Hom$_A(S_{\lambda},M_{\lambda})$, nên đẳng cấu với $D_{\lambda}^{(I(\lambda))}$ (No. 2). Điều này chứng minh mệnh đề.

Mọi môđun đơn đều nguyên thủy (VIII, p. 45), nên mọi môđun nửa đơn đều nửa nguyên thủy. Cho M là một A-môđun nửa đơn, và cho $\lambda \in \mathscr{S}$. Bội số của $\lambda$ trong M là bội nguyên thủy $[M :\lambda ]$ của $\lambda$ trong M được định nghĩa ở VIII, p. 34. Mệnh đề 11 chuyển thành đẳng thức

(11) $[M :\lambda ] =$ dim$_{D_{\lambda}}$(Hom$_A(S_{\lambda},M)$).

Nói chung hơn, nếu $((V_{\lambda})_{\lambda\in\mathscr{S}}, \alpha )$ là một mô tả của M, thì $[M :\lambda ]$ bằng dim$_{D_{\lambda}}(V_{\lambda})$. Theo Mệnh đề 6 của VIII, p. 68, ta cũng có

(12) $[M :\lambda ] =$ dim$_{D_{\lambda}}$(Hom$_A(M,S_{\lambda})$)

khi bội số $[M :\lambda ]$ là hữu hạn. Các A-môđun nửa đơn M và $M'$ là đẳng cấu khi và chỉ khi ta có $[M :\lambda ] = [M':\lambda ]$ với mọi $\lambda \in \mathscr{S}$.

Cho M là một A-môđun nửa đơn. Tồn tại một lực lượng $\mathbf{I}$ có tính chất sau: với mọi phân tích $M =\bigoplus_{i\in I}M_i$ của M thành một tổng trực tiếp các môđun đơn, lực lượng của I bằng $\mathbf{I}$ (VIII, p. 34, Hệ quả 2). Lực lượng này được gọi là độ dài của A-môđun nửa đơn M và được ký hiệu là long$_A(M)$ hoặc long(M). Khi M có độ dài hữu hạn, định nghĩa này tương thích với định nghĩa ở II, §1, No. 10, p. 212, theo Mệnh đề 10.

Các A-môđun đơn là các A-môđun nửa đơn có độ dài 1, và ta có công thức

(13) long$_A(\bigoplus_{j\in J}M_j)=\sum_{j\in J}$ long$_A(M_j)$

đối với mọi họ $(M_j)_{j\in J}$ các A-môđun nửa đơn. Theo Mệnh đề 11, ta có

(14) long$_A(M) =\sum_{\lambda\in\mathscr{S}}$ dim$_{D_{\lambda}}$ Hom$_A(S_{\lambda},M)$.

Khi áp dụng công thức này cho $M_{\lambda}$, ta thu được $[M :\lambda ] =$ long$_A(M_{\lambda})$ với mọi $\lambda \in \mathscr{S}$.

Khi A là một trường, các A-môđun đơn là các không gian vectơ có chiều 1; khi đó mọi A-môđun đều nửa đơn (II, §7, No. 1, p. 292, Định lý 1), và độ dài của nó đơn giản là chiều của nó như một không gian vectơ trên A (II, §7, No. 2, p. 293) .

### Bài tập {#alg-viii-s4-exercises}

Xem [các bài tập của § 4](exercises/s4/).

[^1]: Theo Hệ quả 2 của VIII, p. 56, định nghĩa này trùng với định nghĩa đã cho trong VII, §2, No. 2, p. 9
