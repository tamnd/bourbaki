---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 15
section_title: Brauer Groups
lang: vi
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.277-A VIII.284
pdf_pages: 0294-0301
extraction: native
subsections:
    - "no": 1
      title: Classes of Algebras
      page: 277
      pdf_page: 294
    - "no": 2
      title: Definition of the Brauer Group
      page: 278
      pdf_page: 295
    - "no": 3
      title: Change of Base Field
      page: 281
      pdf_page: 298
    - "no": 4
      title: Examples of Brauer Groups
      page: 283
      pdf_page: 300
statements: 12
exercises: 2
content_sha256: 6ae764fd5ad9435f013dcdbe826324099527d212166cb345d92b763a16cc48f2
translated_from: content/en/alg/VIII/15_s15_brauer_groups.md
source_content_sha256: de0ee49b9fce0132064e5387825b803ddb4c6aeb3c6c606b44846dc5403449fc
translation_model: gpt-5.4
translation_run: translate-vi-1732bc39
glossary_version: 34
glossary_terms_sha256: 1939f9e1cd22c1841541ed3abdff4f7866adae70338473a10967dea9d0915939
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 15. NHÓM BRAUER

Trong mục này, K là một trường giao hoán.

### 1. Các lớp đại số

Ta ký hiệu bởi Iso$_K(A,B)$ quan hệ

“ A và B là các đại số trên K đẳng cấu bậc hữu hạn.”

Đây là một quan hệ tương đương đối với A và B. Cho A là một đại số trên K bậc hữu hạn; lớp của A, ký hiệu bởi cl(A) (hoặc đôi khi cl$_K$(A)), là lớp của các đối tượng tương đương với A đối với quan hệ Iso$_K($Lý thuyết Tập hợp, II, §6, No. 9, p. 122). Theo định nghĩa, cl(A) là một đại số trên K đẳng cấu với A; hai đại số trên K bậc hữu hạn thuộc cùng một lớp khi và chỉ khi chúng đẳng cấu.

Ta ký hiệu bởi $\mathscr{A}$ tập hợp các cặp $(W, \mu)$, trong đó W là một không gian con tuyến tính của $K^{(\mathbf{N})}$ hữu hạn chiều trên K và $\mu$ là một ánh xạ song tuyến tính trên K từ $W\times W$ vào W biến W thành một đại số trên K (kết hợp và có đơn vị). Mọi đại số trên K bậc hữu hạn đều đẳng cấu với một đại số như vậy. Theo loc. cit., quan hệ

“$\alpha$ là một lớp các đại số trên K bậc hữu hạn”

do đó là xác định tập theo $\alpha ($Lý thuyết Tập hợp, II, §1, No. 4, p. 68). Ta ký hiệu tập hợp các lớp các đại số trên K bậc hữu hạn bởi $\mathscr{C}_K$.

#### Mệnh đề 1 {#alg-viii-s15-prop-1 .statement tag=00HV}

Tập hợp $\mathscr{C}_K$, được trang bị luật hợp thành cho bởi $(\alpha , \beta )\mapsto$ cl($\alpha \otimes_K\beta$ ), là một monoid giao hoán. Phần tử đơn vị của $\mathscr{C}_K$ là lớp $\varepsilon$ của K-đại số K. Hơn nữa, nếu A và B là các K-đại số bậc hữu hạn, thì ta có quan hệ

(1) cl(A $\otimes_KB$) $=$ cl(A) cl(B).

Cho A, B và C là các đại số trên K bậc hữu hạn, với các lớp tương ứng $\alpha$, $\beta$, và $\gamma$. Các đại số trên K A và $\alpha$ là đẳng cấu, cũng như B và $\beta$. Do đó, các đại số trên K $A\otimes_KB$ và $\alpha \otimes_K\beta$ là đẳng cấu, và ta có cl(A$\otimes_KB$) $=$ cl($\alpha \otimes_K\beta$ ), suy ra công thức (1). Suy ra $(\alpha \beta )\gamma$ là lớp của đại số trên K $(A\otimes_KB)\otimes_KC$ và $\alpha (\beta \gamma )$ là lớp của đại số trên K $A\otimes_K(B\otimes_KC)$. Bây giờ, các đại số trên K này là đẳng cấu (III, §4, No. 1, p. 461), nên ta có đẳng thức $(\alpha \beta )\gamma =\alpha (\beta \gamma )$. Tương tự, quan hệ $\alpha \varepsilon =\varepsilon \alpha =\alpha$ suy ra từ việc các đại số trên K $A\otimes_KK, K\otimes_KA$, và A là đẳng cấu, và quan hệ $\alpha \beta =\beta \alpha$ suy ra từ việc các đại số $A\otimes_KB$ và $B\otimes_KA$ là đẳng cấu.

Trong tập hợp $\mathscr{C}_K$, quan hệ “$\alpha$ và $\beta$ là các đại số tương đương Morita” là một quan hệ tương đương (VIII, p. 100). Theo Mệnh đề 13, d) của VIII, p. 111, nó tương thích với luật hợp thành trên $\mathscr{C}_K$. Ta ký hiệu $\mathscr{M}_K$ là monoit thương của $\mathscr{C}_K$ theo quan hệ tương đương này và $\varphi$ là đồng cấu chính tắc từ $\mathscr{C}_K$ tới $\mathscr{M}_K$. Với mọi K-đại số A có bậc hữu hạn, ta ký hiệu [A] là ảnh của cl(A) bởi $\varphi$. Nếu A và B là các K-đại số có bậc hữu hạn, thì ta có [A] = [B] khi và chỉ khi các K-đại số A và B tương đương Morita; hơn nữa, ta có quan hệ

$$
[A\otimes_KB] = [A][B] \tag{2}
$$

trong monoit $\mathscr{M}_K$.

#### Bổ đề 1 {#alg-viii-s15-lem-1 .statement tag=00HW}

Cho A là một K-đại số có bậc hữu hạn và D là một trường có bậc hữu hạn trên K. Ta có [A] = [D] trong $\mathscr{M}_K$ khi và chỉ khi tồn tại một số nguyên $n\geqslant 1$ sao cho A đẳng cấu với $\mathbf{M}_n(K)$.

Theo định nghĩa, ta có [A] = [D] khi và chỉ khi tồn tại một song môđun $(A$, D) khả nghịch, tức là (VIII, p. 101, Định lý 1), một không gian vectơ phải V có số chiều hữu hạn khác không trên D được trang bị một đẳng cấu các K-đại số $A\rightarrow$ End$_D(V)$. Bổ đề 1 suy ra.

### 2. Định nghĩa nhóm Brauer

Ta ký hiệu bởi Br(K) tập hợp các phần tử của $\mathscr{M}_K$ có dạng [A], trong đó A là một đại số đơn tâm bậc hữu hạn trên K.

#### Mệnh đề 2 {#alg-viii-s15-prop-2 .statement tag=00HX}

Tập hợp Br(K) là tập hợp các phần tử khả nghịch của $\mathscr{M}_K$, trong đó nghịch đảo của một phần tử [A] của Br(K) là $[A^o]$. Do đó, luật hợp thành trên monoide $\mathscr{M}_K$ trang bị cho Br(K) cấu trúc của một nhóm Abel.

Cho A là một đại số đơn tâm bậc hữu hạn trên K. Đại số $A^o$ là đơn tâm và bậc hữu hạn trên K (VIII, p. 251). Đại số $A\otimes_KA^o$ đẳng cấu với một đại số ma trận $\mathbf{M}_n$(K), trong đó $n^2=$ dim(A) (VIII, p. 252, Định lý 1). Vì vậy ta có $[A][A^o] = [A\otimes_KA^o] = [K]$ (Bổ đề 1), điều này chứng minh rằng [A] là khả nghịch, với nghịch đảo là $[A^o]$.

Ngược lại, cho A là một đại số trên K có bậc hữu hạn. Nếu [A] khả nghịch trong $\mathscr{M}_K$, thì tồn tại một đại số trên K B có bậc hữu hạn sao cho [A][B] = [K]; theo công thức (2) và Bổ đề 1, điều đó có nghĩa là đại số trên K $A\otimes_KB$ đẳng cấu với một đại số ma trận $\mathbf{M}_n(K)$ với $n\geqslant 1$. Theo Nhận xét 1 của VIII, p. 251, khi đó đại số A là đơn tâm.

#### Định nghĩa 1 {#alg-viii-s15-def-1 .statement tag=00HY}

Nhóm Abel Br(K) được gọi là nhóm Brauer của trường K.

#### Bổ đề 2 {#alg-viii-s15-lem-2 .statement tag=00HZ}

Cho I và J là các tập hợp hữu hạn, $k$ là một vành giao hoán, và A và B là các đại số trên $k$. Ký hiệu bởi $\mathbf{M}_I(A)$ đại số trên $k$ của các ma trận vuông kiểu $(I,I)$ với các phần tử thuộc A, và định nghĩa tương tự các đại số trên $k$ $\mathbf{M}_J(B)$ và $\mathbf{M}_{I\times J}(A\otimes_KB)$. Tồn tại một đẳng cấu đại số trên $k$ duy nhất

$$
\varphi :\mathbf{M}_I(A)\otimes_k\mathbf{M}_J(B)\longrightarrow \mathbf{M}_{I\times J}(A\otimes_kB)
$$

sao cho $\varphi ((a_{ii'})\otimes (b_{jj'}))$ là ma trận có phần tử với chỉ số $((i, j),(i', j'))$ bằng $a_{ii'}\otimes b_{jj'}$.

Sự tồn tại của một song ánh $k$-tuyến tính $\varphi$ có tính chất được phát biểu trong bổ đề suy ra từ tính tương thích của tích tenxơ với các tổng trực tiếp (II, §3, No. 7, p. 255, Mệnh đề 7). Việc $\varphi$ là một đồng cấu đại số suy ra từ định nghĩa của tích hai ma trận.

#### Mệnh đề 3 {#alg-viii-s15-prop-3 .statement tag=00I0}

Cho A và B là các đại số trên K đơn tâm bậc hữu hạn. Các tính chất sau là tương đương:

(i) Ta có [A] = [B] trong nhóm Brauer Br(K).

(ii) Tồn tại một số nguyên $t\geqslant 1$ sao cho đại số trên K $A\otimes_KB^o$ đẳng cấu với đại số ma trận $\mathbf{M}_t(K)$.

(iii) Tồn tại các số nguyên dương ngặt $r$ và $s$ sao cho các đại số trên K $A\otimes_K\mathbf{M}_r(K)$ và $B\otimes_K\mathbf{M}_s(K)$ là đẳng cấu.

(iv) Tồn tại một trường D chứa K và các số nguyên $m\geqslant 1$ và $n\geqslant 1$ sao cho A đẳng cấu với $\mathbf{M}_m(D)$ và B với $\mathbf{M}_n(D)$.

(v) Các K-đại số A và B tương đương Morita.

Giả sử rằng ta có [A] = [B]. Vì $[B^o]$ là nghịch đảo của [B] trong nhóm Brauer, nên ta có $[K] = [B][B^o] = [A][B^o] = [A\otimes_KB^o]$. Theo Bổ đề 1, tồn tại một số nguyên $t\geqslant 1$ sao cho các đại số $A\otimes_KB^o$ và $\mathbf{M}_t(K)$ đẳng cấu. Vậy (i) suy ra (ii).

Giả sử rằng (ii) đúng. Vì $B^o\otimes_KB$ đẳng cấu với một đại số ma trận $\mathbf{M}_s(K)$ với $s\geqslant 1$ (VIII, p. 252, Định lý 1), nên đại số $A\otimes_KB^o\otimes_KB$ một mặt đẳng cấu với $A\otimes_K\mathbf{M}_s$(K), mặt khác đẳng cấu với $\mathbf{M}_t(K)\otimes_KB$. Vậy tính chất (ii) suy ra tính chất (iii).

Giả sử rằng (iii) đúng. Theo định lý của Wedderburn (VIII, p. 120, Định lý 1), tồn tại các số nguyên $m\geqslant 1$ và $n\geqslant 1$ và các trường D và $D'$ có bậc hữu hạn trên K với tâm là K sao cho A đẳng cấu với $\mathbf{M}_m(D)$ và B với $\mathbf{M}_n(D')$. Khi đó đại số $A\otimes_K\mathbf{M}_r(K)$ đẳng cấu với $\mathbf{M}_{mr}$(D), và đại số $B\otimes_K\mathbf{M}_{r'}(K)$ đẳng cấu với $\mathbf{M}_{nr'}(D')$ (Bổ đề 2). Theo Hệ quả 2 của VIII, p. 121, các K-đại số D và $D'$ là đẳng cấu. Vậy (iii) suy ra (iv).

Giả sử rằng (iv) đúng. Các đại số A và D tương đương Morita, cũng như các đại số B và D (VIII, p. 114, Ví dụ 2). Do đó, A và B tương đương Morita, nên (iv) suy ra (v).

Cuối cùng, suy ra (v)$\Rightarrow$(i) là định nghĩa của tập hợp Br(K).

Khi các tính chất tương đương của mệnh đề được thỏa mãn, ta nói rằng các đại số A và B là tương tự.

#### Hệ quả {#alg-viii-s15-n2-cor-1 .statement tag=00I1}

Cho A và B là các đại số đơn tâm bậc hữu hạn trên K. Khi đó A và B đẳng cấu khi và chỉ khi chúng tương tự và có cùng bậc.

Điều này suy ra từ tính tương đương của các tính chất (i) và (iv) của Mệnh đề 3 và từ việc dim$_K(\mathbf{M}_n(D)) =$ dim$_K(D)\times n^2$.

#### Mệnh đề 4 {#alg-viii-s15-prop-4 .statement tag=00I2}

Cho $\mathscr{K}_K$ là tập hợp các lớp của các đại số trên K trung tâm bậc hữu hạn là các trường. Ánh xạ $D\mapsto [D]$ từ $\mathscr{K}_K$ vào Br(K) là song ánh.

Điều này suy ra từ Bổ đề 1 của VIII, p. 278 và định lý của Wedderburn (VIII, p. 120, Định lý 1).

### 3. Đổi Trường Cơ Sở

Cho L là một mở rộng của trường K. Cho A và B là các đại số trên K bậc hữu hạn; khi đó các đại số trên L $A_{(L)}$ và $B_{(L)}$ đều có bậc hữu hạn. Các đại số trên L $A_{(L)}\otimes_LB_{(L)}$ và $(A\otimes_KB)_{(L)}$ là đẳng cấu (III, §4, No. 1, p. 462, Mệnh đề 3). Đại số trên L $K_{(L)}$ đẳng cấu với L. Do đó, tồn tại một đồng cấu monoit duy nhất $\rho_{L/K}$ từ $\mathscr{C}_K$ vào $\mathscr{C}_L$ sao cho

(3) $\rho_{L/K}$(cl(A)) = cl(A$_{(L)}$)

đối với mọi đại số trên K A có bậc hữu hạn.

Nếu các đại số trên K A và B tương đương Morita, thì các đại số trên L $A_{(L)}$ và $B_{(L)}$ cũng vậy (VIII, p. 111, Mệnh đề 13, e)). Nếu đại số trên K A là đơn tâm và bậc hữu hạn, thì đại số trên L $A_{(L)}$ cũng vậy (VIII, p. 251, Nhận xét 2). Do đó ta suy ra từ $\rho_{L/K}$ một đồng cấu nhóm $r_{L/K}$ từ Br(K) vào Br(L) sao cho

$$
r_{L/K}([A]) = [A_{(L)}] \tag{4}
$$

đối với mọi đại số đơn tâm trên K A có bậc hữu hạn.

Cho M là một mở rộng của trường L. Vì mở rộng vô hướng có tính bắc cầu (III, §1, No. 5, p. 434), ta có quan hệ

$$
r_{M/K}=r_{M/L}\circ r_{L/K} \tag{5}
$$

Cho A là một đại số đơn tâm trên K có bậc hữu hạn, và cho L là một mở rộng của K. Ta nói rằng L là một trường phân rã của A (hoặc phân rã A) nếu đại số trên L $A_{(L)}$ đẳng cấu với một đại số ma trận $\mathbf{M}_n(L)$ với một số nguyên $n\geqslant 1$. Theo ký hiệu nói trên, điều này tương ứng với việc nói rằng lớp của A trong Br(K) thuộc hạt nhân của đồng cấu $r_{L/K}:$ Br(K) $\rightarrow$ Br(L).

Nếu B tương tự với A, thì L là một trường phân rã của A khi và chỉ khi nó là một trường phân rã của B.

Nếu L là một trường phân rã của A, thì mọi mở rộng của L đều là một trường phân rã của A. Theo Định lý 1 của VIII, p. 252, tồn tại một mở rộng Galois của K có bậc hữu hạn là một trường phân rã của A, và mọi bao đóng tách được của K đều là một trường phân rã của A.

#### Mệnh đề 5 {#alg-viii-s15-prop-5 .statement tag=00I3}

Cho A là một đại số đơn tâm trên K có bậc hữu hạn, và cho L là một mở rộng của K có bậc hữu hạn. Các tính chất sau là tương đương:

(i) Mở rộng L là một trường phân rã của A.

(ii) Tồn tại một đại số đơn tâm trên K có bậc hữu hạn, tương tự với A, chứa một đại số con giao hoán cực đại đẳng cấu với L.

Ta hãy chứng minh rằng (ii) suy ra (i); chỉ cần xét trường hợp L là một đại số con giao hoán cực đại của A. Cho $\psi : A\otimes_KA^o\rightarrow$ End$_K(A)$ là đẳng cấu chính tắc gửi $a\otimes a'$ lên ánh xạ K-tuyến tính $x\mapsto axa'$ (VIII, p. 252, Định lý 1). Ta xem A như một không gian vectơ phải trên L; khi đó $\psi$ gửi $A\otimes_KL$ vào không gian con End$_L(A)$ của End$_K(A)$ và, bởi hạn chế, cảm sinh một đồng cấu đơn cấu của các L-đại số $\psi ': A\otimes_KL\rightarrow$ End$_L(A)$. Đặt $n= [L : K]$. Theo VIII, p. 262, Mệnh đề 3, ta có $[A : L] =n$, và do đó $[A\otimes_KL : L] = [A : K] =n^2$ và [End$_L(A) : L] =n^2$. Do đó, $\psi '$ là một đẳng cấu, điều này chứng minh (i).

Mệnh đề đảo lại suy ra từ Bổ đề 3 dưới đây.

#### Bổ đề 3 {#alg-viii-s15-lem-3 .statement tag=00I4}

Cho A là một đại số đơn tâm trên K bậc hữu hạn, và cho L là một mở rộng của K bậc hữu hạn là một trường phân rã của A. Gọi V là một $A_{(L)}$-môđun đơn, sao cho cấu xạ tự nhiên $\varphi : A_{(L)}\rightarrow$ End$_L(V)$ là một đẳng cấu. Gọi C là vành End$_A(V)$. Khi đó C tương tự với $A^o$, và ảnh của $L\otimes 1\subset A_{(L)}$ là một đại số con giao hoán cực đại của C.

Ta đồng nhất A với một vành con của $A_{(L)}$. Ta xem V như một không gian vectơ trên K. Vành C là hoán tập của $\varphi (A)$ trong End$_K(V)$. Nó là một đại số đơn tâm trên K bậc hữu hạn, và đồng cấu $a\otimes c\mapsto ac$ từ $A\otimes_KC$ đến End$_K(V)$ là một đẳng cấu (VIII, p. 260, Định lý 6, a)). Do đó các đại số trên K A và $C^o$ là tương tự (VIII, p. 279, Mệnh đề 3).

Gọi $L_V$ là vành các phép vị tự của không gian vectơ V trên L; đó là hoán tập của End$_L(V)$ trong End$_K(V)$ (VIII, p. 82, Hệ quả 1). Bây giờ, đại số trên K End$_L(V)$ được sinh bởi $\varphi (A)$ và $L_V$; do đó, trong End$_K$(V), ta có

$L_V=$ End$_L(V)'=\varphi (A)'\cap L'_V= C\cap L'_V$,

trong đó với mọi tập con B của End$_K$(V), hoán tập của B trong End$_K(V)$ được ký hiệu bởi $B'$. Vậy $L_V$ là một đại số con giao hoán cực đại của C (VIII, p. 261, Bổ đề 3), và do đó cũng là một đại số con giao hoán cực đại của $C^o$. Ánh xạ $\lambda \mapsto \lambda_V$ là một đẳng cấu đại số trên K từ L tới $L_V$. Điều này chứng minh bổ đề.

#### Hệ quả 1 {#alg-viii-s15-lem-3-cor-1 .statement tag=00I5}

Cho A là một đại số đơn tâm trên K có bậc hữu hạn, và L là một mở rộng của K có bậc hữu hạn. Giả sử $[A : K] = [L : K]^2$. Khi đó L là một trường phân rã của A khi và chỉ khi A chứa một đại số con đẳng cấu với L.

Giả sử tồn tại một cấu xạ $\varphi$ từ L vào A. Gọi M là một đại số con giao hoán nửa đơn cực đại chứa $\varphi (L)$. Theo Mệnh đề 3 của VIII, p. 262, ta có $[A : K] = [M : K]^2$, nên [M : K] = [L : K] và $M =\varphi (L)$. Theo Mệnh đề 5, trường L phân rã A. Ngược lại, giả sử rằng trường L phân rã A; khi đó nó đẳng cấu với một đại số con giao hoán cực đại của một đại số đơn tâm trên K B đồng dạng với A (Mệnh đề 5). Ta có $[B : K] = [L : K]^2$ (VIII, p. 262, Mệnh đề 3), nên [B : K] = [A : K]. Do đó, B đẳng cấu với A (VIII, p. 280, Hệ quả). Hệ quả 1 được suy ra.

#### Hệ quả 2 {#alg-viii-s15-lem-3-cor-2 .statement tag=00I6}

Cho D là một trường có bậc hữu hạn trên K với tâm là K, và L là một mở rộng của K có bậc hữu hạn, là một trường phân rã của D. Bậc rút gọn của D chia hết cho [L : K].

Ký hiệu bậc thu gọn của D (VIII, p. 253) là $r$; theo định nghĩa, ta có $[D : K] =r^2$. Theo Mệnh đề 5, tồn tại một đại số đơn tâm trên K B tương tự với D mà trong đó L là một đại số con giao hoán cực đại. Vì B đẳng cấu với một đại số ma trận $\mathbf{M}_n(D)$ (VIII, p. 278, Bổ đề 1), ta có $[B : K] =n^2r^2$ và do đó $[L : K] =nr$ (VIII, p. 262, Mệnh đề 3).

### 4. Ví dụ về các nhóm Brauer

Nhóm Brauer Br(K) chỉ còn phần tử đơn vị trong ba trường hợp sau:

a) K là đóng tách được (VIII, p. 253, Hệ quả 1).

$*$b) K là một trường hữu hạn (VIII, p. 357, Hệ quả 2).

c) K có tính chất $(C_1)$ (VIII, p. 357, Nhận xét 2).

Giả sử K là một trường có thứ tự cực đại (VI, §2, No. 5, p. 25). Khi đó nhóm Brauer của K là cyclic cấp 2; các phần tử của nó là lớp của K và lớp của đại số quaternion trên K kiểu $(-1,0,-1)$ (III, §2, No. 5, p. 444 and VIII, p. 367, Định lý 1).

Giả sử K là một trường tôpô giao hoán, compact địa phương, không rời rạc. Nếu K không liên thông, thì nó là một trường đầy đủ đối với một định giá rời rạc, với trường thặng dư hữu hạn (Comm. Alg., VI, §9, No. 3, p. 433, Định lý 1), và tồn tại một đẳng cấu từ Br(K) tới $\mathbf{Q}/\mathbf{Z}$ (VIII, p. 332, Bài tập 17). Nếu K liên thông, thì nó đẳng cấu với $\mathbf{R}$ hoặc $\mathbf{C}$. Nhóm Brauer của trường $\mathbf{R}$ là cyclic cấp 2. Phần tử không tầm thường của nó là lớp của đại số $\mathbf{H}$ các quaternion Hamilton (Gen. Top., VIII, §1, No. 4, p. 104); nhóm Brauer của $\mathbf{C}$ có cấp 1.

### Bài tập {#alg-viii-s15-exercises}

Xem [các bài tập cho § 15](exercises/s15/).
