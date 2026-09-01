---
book: ac
book_title: Commutative Algebra
chapter: IX
chapter_title: ANNEAUX LOCAUX NOETHÉRIENS COMPLETS
section: 2
section_title: Anneaux de Cohen
lang: vi
source: ac-viii-ix-fr
book_pages: AC IX.17-AC IX.27, AC IX.68-AC IX.75
pdf_pages: 0129-0139, 0180-0187
extraction: ocr
subsections:
    - "no": 1
      title: $p$-anneaux
      page: 17
      pdf_page: 129
    - "no": 2
      title: Anneaux de Cohen
      page: 20
      pdf_page: 132
    - "no": 3
      title: Existence et unicité des $p$-anneaux
      page: 22
      pdf_page: 134
    - "no": 4
      title: Représentants multiplicatifs
      page: 24
      pdf_page: 136
    - "no": 5
      title: Structure des anneaux locaux noethériens complets
      page: 0
      pdf_page: 138
statements: 30
exercises: 17
content_sha256: e2dbe237c0de88cb82bf1a4f66b316685171771f4e5087f37b65adf85386f906
translated_from: content/en-mt/ac/IX/02_s2_anneaux_de_cohen.md
source_lang: en-mt
translation_method: machine
source_content_sha256: d23599edc2c0840270fb99102a3340399d8d1e5d81cbfe51a36bfda141c52698
translation_model: gpt-5.4
translation_run: translate-vi-6e965cd1
glossary_version: 34
glossary_terms_sha256: 9f2193f49bb0fe76bacae1d5c2acffa123db960a44d91f76ba7021b4d93e1639
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 2. VÀNH COHEN

Trong suốt số này, $p$ ký hiệu một số nguyên tố.

### 1. Các $p$-vành

#### Định nghĩa 1 {#ac-ix-s2-def-1 .statement}

Một vành $C$ được gọi là một $p$-vành nếu iđêan $pC$ của $C$ là cực đại, và nếu $C$ tách biệt và đầy đủ đối với tôpô $pC$-adic.

Cho $C$ là một vành; nếu $p1_C$ lũy linh và nếu iđêan $pC$ của $C$ là cực đại, thì $C$ là một $p$-vành, vì tôpô $pC$-adic của $C$ là rời rạc. Đặc biệt, mọi trường có đặc số $p$ đều là một $p$-vành.

#### Mệnh đề 1 {#ac-ix-s2-prop-1 .statement}

Cho $C$ là một $p$-vành.

a) Vành $C$ là địa phương, với iđêan cực đại $pC$.

b) Giả sử $p1_C$ lũy linh. Gọi $d$ là số nguyên dương nhỏ nhất sao cho $p^d1_C = 0$. Các iđêan của $C$ có dạng $p^kC$ với $0 \leq k \leq d$, và ta có $p^kC \neq p^lC$ khi $k$ và $l$ là hai số nguyên phân biệt thỏa mãn $0 \leq k \leq d, 0 \leq l \leq d$. $C$-môđun $C$ có độ dài $d$.

c) Giả sử rằng $p1_C$ không lũy linh. Khi đó $C$ là một vành định giá rời rạc có trường thặng dư là trường có đặc số $p$, và có trường phân thức là trường có đặc số $0$. Các iđêan có dạng $p^nC$, với $n \in \mathbf{N}$, phân biệt từng đôi một; chúng tạo thành tất cả các iđêan khác không của $C$. $C$-môđun $C$ không có độ dài hữu hạn.

Mệnh đề a) suy ra từ mệnh đề 19 của III, $§ 2$, no. 13.

Theo giả thiết, ta có $\bigcap_{n \geqslant 0} p^n C = \{0\}$. Cho $x \neq 0$ trong $C$; tồn tại một số nguyên $n \geqslant 0$ sao cho $x \in p^n C$, $x \notin p^{n+1} C$; do đó tồn tại một phần tử $y$ của $C$ sao cho $x = p^n y$; vì $y$ không thuộc $pC$, $y$ khả nghịch.

Giả sử rằng $p 1_C$ không lũy linh. Nếu $x$ và $x'$ là hai phần tử khác không của $C$, thì tồn tại hai số nguyên $n \geqslant 0$, $n' \geqslant 0$ và hai phần tử khả nghịch $y$, $y'$ của $C$ sao cho $x = p^n y$, $x' = p^{n'} y'$. Khi đó ta có $xx' = p^{n+n'} yy' \neq 0$, do đó $C$ là một miền nguyên. Vì $C$ là một vành địa phương, nhưng không phải là một trường, và vì iđêan cực đại $m_C = pC$ của $C$ là chính, nên $C$ là một vành định giá rời rạc (VI, $§ 3$, số 6, mệnh đề 9). Khi đó các iđêan khác không của $C$ có dạng $p^n C$ theo *nơi đã dẫn*, mệnh đề 8, và từng đôi một phân biệt. Đặc biệt, vành $C$ không phải là Artin, do đó $C$-môđun $C$ không có độ dài hữu hạn. Trường thặng dư $C/pC$ của $C$ có đặc số $p$. Gọi $q$ là đặc số của trường phân thức của $C$. Ta có $p 1_C \neq 0$, do đó $p \neq q$. Hơn nữa, nếu $q$ khác không, thì ta sẽ có $q 1_C = 0$ nên $C/pC$ sẽ có đặc số $q \neq p$, điều này vô lý. Điều này chứng minh c).

Giả sử rằng $p 1_C$ là lũy linh. Gọi $d$ là số nguyên dương nhỏ nhất sao cho $p^d 1_C = 0$. Ta có một dãy các iđêan

(E)
$$
C \supset pC \supset p^2 C \supset ... \supset p^{d-1} C \supset p^d C = \{0\} .
$$

Nếu $k$ là một số nguyên sao cho $0 \leqslant k < d$ và $p^k C = p^{k+1} C$, ta suy ra

$$
p^{d-k-1} p^k C = p^{d-k-1} p^{k+1} C = \{0\}
$$

trái với giả thiết $p^{d-1} 1_C \neq 0$. Do đó các phần tử của dãy (E) từng đôi một phân biệt. Cho $a$ là một iđêan của $C$ và cho $k$ là số nguyên dương nhỏ nhất sao cho $a \supset p^k C$. Cho $x$ là một phần tử khác không của $a$; ta đã thấy rằng $x$ có dạng $p^m u$ với $m \geqslant 0$ và $u$ khả nghịch trong $C$. Suy ra $p^m C \subset a$, do đó $m \geqslant k$, và cuối cùng $x \in p^k C$. Kết luận, ta có $a = p^k C$. Khi đó dãy (E) là một dãy Jordan-Hölder của $C$-môđun $C$, có độ dài $d$.

#### Hệ quả 1 {#ac-ix-s2-prop-1-cor-1 .statement}

Nếu $p$-vành $C$ là một miền nguyên, thì nó là một vành định giá rời rạc, hoặc một trường có đặc số $p$.

Giả sử $C$ là một miền nguyên. Nếu $p 1_C$ là lũy linh, ta có $p 1_C = 0$, và $\{0\}$ là một iđêan cực đại của $C$, do đó $C$ là một trường có đặc số $p$. Nếu $p 1_C$ không lũy linh, thì $C$ là một vành định giá rời rạc theo Mệnh đề 1, c).

#### Hệ quả 2 {#ac-ix-s2-prop-1-cor-2 .statement}

Cho $C$ là một $p$-vành và $a$ là một iđêan của $C$ phân biệt với $C$. Vành $C/a$ là một $p$-vành.

Có thể giả sử $a \neq \{0\}$. Khi đó tồn tại một số nguyên $i \geqslant 1$ sao cho $a = p^i C$; iđêan $pC/a$ của $C/a$ là cực đại và ta có $p^i 1_{C/a} = 0$, vì vậy $C/a$ là một $p$-vành.

Cho $C$ là một $p$-vành. *Độ dài của* $C$, ký hiệu là $l(C)$, là cận trên nhỏ nhất trong $\overline{\mathbf{R}}$ của tập hợp các số nguyên $n \geqslant 1$ sao cho $p^{n-1} 1_C \neq 0$. Khi $l(C)$ hữu hạn, nó là độ dài của $C$-môđun $C$, và khi $l(C)$ bằng $+ \infty$, $C$-môđun $C$ không có độ dài hữu hạn (mệnh đề 1).

#### Ví dụ 1 {#ac-ix-s2-n1-exa-1 .statement}

Với mọi số nguyên $n \geqslant 1$, vành $\mathbf{Z}/p^n\mathbf{Z}$ là một $p$-vành có độ dài $n$. Vành $\mathbf{Z}_p$ các số nguyên $p$-adic là một $p$-vành có độ dài vô hạn.

#### Ví dụ 2 {#ac-ix-s2-n1-exa-2 .statement}

Cho $K$ là một trường hoàn hảo có đặc số $p$. Theo mệnh đề 8 của § 1, No. 8, vành $W(K)$ các vectơ Witt là một $p$-vành có độ dài vô hạn. Ánh xạ $(a_n)_{n \in \mathbf{N}} \mapsto a_0$ cảm sinh, khi chuyển qua thương, một đẳng cấu của $W(K)/pW(K)$ lên trường $K$ (loc. cit., mệnh đề 7). Với mọi số nguyên $n \geqslant 1$, vành
$$
W_n(K) = W(K)/p^nW(K)
$$
là một $p$-vành có độ dài $n$.

#### Mệnh đề 2 {#ac-ix-s2-prop-2 .statement}

Cho $C$ và $C'$ là hai $p$-vành và $u$ là một đồng cấu từ $C$ vào $C'$. Gọi $v$ là đồng cấu từ $\kappa_C = C/pC$ vào $\kappa_{C'} = C'/pC'$ suy ra từ $u$ khi chuyển qua thương.

a) Ta có $l(C) \geqslant l(C')$, và $u$ là đơn ánh khi và chỉ khi ta có $l(C) = l(C')$.

b) Để $u$ là toàn ánh, điều kiện cần và đủ là $v$ là một đẳng cấu.

c) Để $u$ là một đẳng cấu, điều kiện cần và đủ là $v$ là một đẳng cấu và ta có $l(C) = l(C')$.

Cho $n \geqslant 1$ là một số nguyên. Ta có $u(p^{n-1}1_C) = p^{n-1}1_{C'}$, do đó quan hệ $p^{n-1}1_{C'} \neq 0$ kéo theo $p^{n-1}1_C \neq 0$ và là tương đương với nó nếu $u$ là đơn ánh. Vậy $l(C') \leqslant l(C)$, với đẳng thức nếu $u$ là đơn ánh. Nếu $u$ không đơn ánh, tồn tại một số nguyên $i < l(C)$ sao cho hạt nhân của $u$ là iđêan $p^iC$ của $C$; khi đó $p^i1_{C'} = 0$, do đó $l(C') \leqslant i$. Điều này chứng minh a).

Vì $\kappa_C$ và $\kappa_{C'}$ là các trường, đồng cấu $v$ là đơn ánh. Nếu $u$ là toàn ánh thì $v$ cũng vậy, do đó là một đẳng cấu. Ngược lại, giả sử $v$ toàn ánh. Khi đó với mọi số nguyên $n \geqslant 0$, ánh xạ $v_n : p^nC/p^{n+1}C \to p^nC'/p^{n+1}C'$ cảm sinh bởi $u$ là toàn ánh. Vì $C$ đầy đủ đối với lọc $pC$-adic và $C'$ phân cách đối với lọc $pC'$-adic, $u$ là toàn ánh theo Hệ quả 2 của Định lý 1 của III, § 2, No. 8. Điều này chứng minh b).

Cuối cùng, c) suy ra từ a) và b).

#### Mệnh đề 3 {#ac-ix-s2-prop-3 .statement}

Cho $(C_n, \pi_{n,m})$ là một hệ xạ ảnh các vành theo tập chỉ số $\mathbf{N}$. Giả sử rằng $C_n$ là một vành $p$ với mọi $n \in \mathbf{N}$ và các đồng cấu $\pi_{n,m}$ là toàn ánh. Khi đó $C = \varprojlim C_n$ là một vành $p$, và với mọi $n \in \mathbf{N}$, đồng cấu chính tắc $\pi_n : C \to C_n$ là toàn ánh và cảm sinh một đẳng cấu từ $\kappa_C$ lên $\kappa_{C_n}$.

Vì các ánh xạ $\pi_{n,m}$ là toàn ánh, các ánh xạ $\pi_n$ cũng vậy (E, III, p. 58, mệnh đề 5). Ta sẽ chứng minh rằng $C$ là một vành $p$. Gọi $d_n$ là độ dài của $C_n$. Theo mệnh đề 2, a), dãy các phần tử $d_n$ của $\mathbf{N} \cup \{ + \infty \}$ là tăng; nếu nó dừng, thì tồn tại một số nguyên $n_0$ sao cho $\pi_{n,m}$ là một đẳng cấu từ $C_m$ lên $C_n$ mỗi khi $n_0 \leqslant n \leqslant m$, do đó $C$, đẳng cấu với $C_{n_0}$, là một vành $p$.

Vì vậy chỉ cần xét trường hợp mỗi $d_n$ đều hữu hạn, và dãy $(d_n)$ tiến tới $+ \infty$. Trang bị cho vành $C$ lọc tầm thường (III, § 2, No. 1, ví dụ 5). Với $n \in \mathbf{N}$, gọi $I_n$ là hạt nhân của $\pi_n$; đặt $I_n = C$ nếu $n < 0$. Gọi $E$ là $C$-môđun $C$ được trang bị lọc $(I_n)_{n \in \mathbf{Z}}$. Nó là phân cách và đầy đủ, vì tôpô $\mathcal{T}$ xác định bởi lọc $(I_n)_{n \in \mathbf{Z}}$ là tôpô giới hạn xạ ảnh của các tôpô rời rạc trên các $C_n$.

Cho $k$ là một số nguyên $\geqslant 1$. Ta có $p^k C \subset \varprojlim (p^k C_n)$ (E, III, p. 55, công thức (9)). Ngược lại, nếu $x = (x_n)_{n \in \mathbf{N}} \in \varprojlim (p^k C_n)$ và nếu đặt $X_n = \{ y \in C | \pi_n(p^k y) = x_n \}$, thì dãy $(X_n)_{n \in \mathbf{N}}$ là một dãy giảm gồm các phần afin đóng khác rỗng của E. Vì $E/I_n$ là một C-môđun Artin, nên giao của các $X_n$ là khác rỗng (III, § 2, No. 7, mệnh đề 7); với mọi $z \in \bigcap_{n \in \mathbf{N}} X_n$, ta có $p^k z = x$. Vậy ta đã chứng minh rằng $p^k C = \varprojlim p^k C_n$ với mọi số nguyên $k \geqslant 1$. Đặc biệt iđêan $p^k C$ của C là đóng đối với tôpô $\mathcal{T}$. Trên C, tôpô $p$-adic mịn hơn tôpô $\mathcal{T}$ vì ta có $p^{d_n} C \subset I_n$. Khi đó suy ra từ TG, III, p. 26, hệ quả 1 của mệnh đề 10, rằng C tách biệt và đầy đủ đối với tôpô $pC$-adic. Hơn nữa ta có $pC = \varprojlim pC_n = \pi_0^{-1}(pC_0)$ và do đó đồng cấu toàn ánh từ $C/pC$ vào $C_0/pC_0$ suy ra từ $\pi_0$ là một đẳng cấu. Điều này cho thấy iđêan $pC$ của C là cực đại và do đó C là một $p$-vành. Khẳng định cuối cùng của mệnh đề 3 suy ra từ mệnh đề 2, b).

### 2. Các vành Cohen

#### Định nghĩa 2 {#ac-ix-s2-def-2 .statement}

Cho A là một vành địa phương tách biệt và đầy đủ, mà trường thặng dư có đặc số p. Một vành con Cohen của A có nghĩa là một vành con C của A là một $p$-vành sao cho $A = m_A + C$ (tức là $A/m_A = C/(m_A \cap C)$).

Nếu C là một vành con Cohen của A, thì iđêan $m_A \cap C$ của C là cực đại, nên bằng $pC$. Do đó ánh xạ chính tắc của $\kappa_C = C/pC$ lên $\kappa_A = A/m_A$ là một đẳng cấu trường.

#### Ví dụ {#ac-ix-s2-n2-exa-1 .statement}

Cho C là một $p$-vành. Vành các chuỗi hình thức $A = C[[T_1, ..., T_n]]$ là một vành Noether, địa phương, tách biệt và đầy đủ, mà iđêan cực đại được sinh bởi dãy $(p, T_1, ..., T_n)$. Ngay lập tức thấy rằng C là một vành con Cohen của A. Điều này áp dụng đặc biệt khi C bằng $\mathbf{Z}_p$, $\mathbf{Z}/p^n \mathbf{Z}$ hoặc một trường có đặc số $p$.

#### Định lý 1 {#ac-ix-s2-thm-1 .statement}

Cho A là một vành địa phương, tách biệt và đầy đủ, mà trường thặng dư k có đặc số p. Cho $\pi$ là ánh xạ chính tắc của A lên k, và cho S là một tập con của A, sao cho $\pi$ cảm sinh một song ánh từ S lên một $p$-cơ sở của k (A, V, p. 95).
a) Tồn tại một và chỉ một vành con Cohen C của A chứa S.
b) Vành con C của A là đóng, và tôpô $pC$-adic của C được cảm sinh bởi tôpô $m_A$-adic của A.
c) Mọi vành con đóng $A'$ của A, chứa S, và sao cho $A = A' + m_A$, đều chứa C.

A) Trường hợp riêng: $m_A$ lũy linh

Cho n là một số nguyên dương sao cho $m_A^{n+1} = \{0\}$. Nếu $\Phi_n$ là đa thức Witt thứ n ($§ 1$, No. 1), thì ánh xạ $u : [a_0, ..., a_n] \mapsto \Phi_n(a_0, ..., a_n)$ là một đồng cấu vành từ $W_{n+1}(A)$ vào A ($§ 1$, No. 7). Cho $B_n$ là ảnh của $u$ và cho $C_n$ là vành con của A được sinh bởi $B_n \cup S$.

#### Bổ đề 1 {#ac-ix-s2-lem-1 .statement}

Cho $A'$ là một vành con của $A$ chứa $S$. Để $A'$ chứa $C_n$, điều kiện cần và đủ là có $A' + m_A = A$.

Ta có $pA \subset m_A$ và $B_n$ gồm các phần tử có dạng $a_0^{p^n} + pa_1^{p^{n-1}} + \cdots + p^n a_n$ với $a_0, ..., a_n$ thuộc $A$. Do đó ta có $\pi(B_n) = k^{p^n}$, do đó $\pi(C_n) = k^{p^n}[\pi(S)]$. Nhưng vì $\pi(S)$ là một $p$-cơ sở của $k$, ta có $k = k^{p^n}[\pi(S)]$ (A, V, p. 96), do đó $\pi(C_n) = k$, nghĩa là $C_n + m_A = A$.

Cho $A'$ là một vành con của $A$ chứa $S$. Nếu $A'$ chứa $C_n$, ta có
$$
A' + m_A \supset C_n + m_A = A, \quad \text{do đó} \quad A' + m_A = A.
$$
Ngược lại, giả sử rằng ta có $A' + m_A = A$. Cho $a_0, ..., a_n$ là các phần tử của $A$; theo giả thiết tồn tại các phần tử $a'_0, ..., a'_n$ của $A'$ sao cho $a_i \equiv a'_i \mod m_A$ với $0 \leq i \leq n$. Theo mệnh đề 1 của § 1, No. 1 và giả thiết $m_A^{n+1} = \{0\}$, do đó ta có $\Phi_n(a_0, ..., a_n) = \Phi_n(a'_0, ..., a'_n) \in A'$, do đó $B_n \subset A'$. Vì $C_n$ là vành sinh bởi $B_n \cup S$, ta có $C_n \subset A'$.

Trong tập hợp $S$ các vành con $A'$ của $A$ chứa $S$ và sao cho $A' + m_A = A$, theo bổ đề 1 tồn tại một phần tử nhỏ nhất $C$, và ta có $C_n = C$ với mọi số nguyên $n \geq 0$ sao cho $m_A^{n+1} = \{0\}$.

Ta có $C + m_A = A$ theo phép dựng và $p1_C$ là lũy linh. Hiển nhiên ta có $pC \subset C \cap m_A$ và do đó bổ đề 2 dưới đây chứng tỏ rằng $pC$ là một iđêan cực đại của $C$ và do đó $C$ là một vành Cohen của $A$.

#### Bổ đề 2 {#ac-ix-s2-lem-2 .statement}

Ta có $C \cap m_A \subset pC$.

Chọn một số nguyên $m \geq 1$ sao cho $m_A^m = \{0\}$, do đó $C = C_m = C_{m-1}$. Gọi $\Lambda$ là tập con của $\mathbf{N}^{(S)}$ gồm các họ số nguyên $(\alpha_s)_{s \in S}$ có giá hữu hạn thỏa mãn $0 \leq \alpha_s < p^m$ với mọi $s \in S$. Vì $B_m$ chứa $s^{p^m} = \Phi_m(s, 0, ..., 0)$ với mọi $s \in S$, các đơn thức $Z_\alpha = \prod_{s \in S} s^{\alpha_s}$, trong đó $\alpha$ chạy qua $\Lambda$, sinh $C_m$ như một $B_m$-môđun.

Hơn nữa, từ công thức
$$
\Phi_m(a_0, ..., a_m) = a_0^{p^m} + p \Phi_{m-1}(a_1, ..., a_m),
$$
mọi phần tử của $B_m$ đều có dạng $a^{p^m} + pb$ với $a \in A$ và $b \in B_{m-1}$. Do đó mọi phần tử của $C = C_m$ đều có dạng
$$
x = \sum_{\alpha \in \Lambda} c_\alpha^{p^m} Z_\alpha + py
$$
với $c_\alpha \in A$ với mọi $\alpha \in \Lambda$, và $y \in C_{m-1} = C$. Nếu $x$ thuộc $C \cap m_A$, ta có $\pi(x) = 0$, do đó $\sum_{\alpha \in \Lambda} \pi(c_\alpha)^{p^m} \pi(Z_\alpha) = 0$. Vì $\pi(S)$ là một $p$-cơ sở của $k$, theo A, V, p. 96 ta có $\pi(c_\alpha) = 0$ với mọi $\alpha \in \Lambda$. Khi đó ta có $c_\alpha \in m_A$, do đó $c_\alpha^m = 0$ và a fortiori $c_\alpha^{p^m} = 0$. Từ (1), ta có $x = py$, do đó bổ đề 2.

Ta có $p^m C = m_A^m = \{0\}$ với $m$ đủ lớn, và vì thế mệnh đề b) là tầm thường. Mệnh đề c) suy ra từ bổ đề 1. Nếu $C'$ là một vành con Cohen của $A$ chứa $S$, thì ta có $C' \supset C$ theo bổ đề 1. Nhưng vì phép nhúng của $C$ vào $C'$ cảm sinh một đẳng cấu của $\kappa_C$ lên $\kappa_{C'}$, nên ta có $C = C'$ (No. 1, mệnh đề 2, b)), và điều này hoàn tất việc chứng minh a).

B) *Trường hợp tổng quát*

Với mọi số nguyên $n \geqslant 0$, gọi $A_n$ là vành địa phương $A/m_A^{n+1}$, gọi $m_n = m_A/m_A^{n+1}$ là iđêan cực đại của nó, và gọi $\pi_n$ là đồng cấu chính tắc từ $A$ lên $A_n$. Theo A), tồn tại một vành con Cohen duy nhất $C_n$ của $A_n$ chứa $\pi_n(S)$. Khi $0 \leqslant n \leqslant m$, ta ký hiệu bởi $\pi_{n,m}$ đồng cấu chính tắc từ $A_m$ lên $A_n$. Theo Hệ quả 2 của Mệnh đề 1 ở No. 1, $\pi_{n,m}(C_m)$ là một $p$-vành; ta có $\pi_{n,m}(C_m) + m_n = A_n$, do đó $\pi_{n,m}(C_m)$ bằng vành con Cohen $C_n$ của $A_n$. Theo Mệnh đề 3 ở No. 1, vành con $\lim C_n$ của $\lim A_n$ là một $p$-vành. Đặt $C = \bigcap_{n \in \mathbf{N}} \pi_n^{-1}(C_n)$. Vì $C$ là ảnh ngược của $\lim C_n$ qua đẳng cấu $a \mapsto (\pi_n(a))_{n \in \mathbf{N}}$ từ $A$ lên $\lim A_n$, nên nó là một vành con đóng của $A$, và là một $p$-vành. Ta có $\pi_n(C) = C_n$ với mọi $n \in \mathbf{N}$ (No. 1, Mệnh đề 3), và đặc biệt $\pi_0(C) = A_0$, nghĩa là $\pi(C) = k$. Vậy $C$ là một vành con Cohen của $A$.

Với mọi số nguyên $n \geqslant 0$, đặt $J_n = C \cap m_A^n$. Vì vành địa phương $A$ là tách biệt, ta có $\bigcap_{n \in \mathbf{N}} J_n = \{0\}$, và xét cấu trúc của các iđêan của một $p$-vành (No. 1, Mệnh đề 1), mọi iđêan của $C$ có dạng $p^kC$ đều chứa một trong các $J_n$. Ngược lại, $J_n$ chứa $p^nC$. Do đó, tôpô $pC$-adic của $C$ được cảm sinh bởi tôpô $m_A$-adic của $A$. Điều này chứng minh b).

Cho $A'$ là một vành con đóng của $A$, chứa $S$ và sao cho $A' + m_A = A$. Vì $A'$ đóng, ta có $A' = \bigcap_{n \in \mathbf{N}} \pi_n^{-1}(\pi_n(A'))$. Ta có $\pi_n(A') \supset \pi_n(S)$ và $\pi_n(A') + m_n = A_n$, do đó $\pi_n(A') \supset C_n$ theo điều đã thấy trong A). Sau hết, ta có $\pi_n^{-1}(\pi_n(A')) \supset \pi_n^{-1}(C_n)$, do đó $A' \supset C$. Điều này chứng minh c). Suy ra tính duy nhất của một vành con Cohen như trong A).

#### Nhận xét {#ac-ix-s2-n2-rem-1 .statement}

Giả sử rằng $p1_A$ không lũy linh (điều này xảy ra đặc biệt khi $A$ là một vành nguyên mà trường phân thức có đặc số 0). Khi đó $C$ là một vành định giá rời rạc mà trường phân thức có đặc số 0.

### 3. Sự tồn tại và tính duy nhất của các $p$-vành

#### Mệnh đề 4 {#ac-ix-s2-prop-4 .statement}

*Cho $C$ và $C'$ là hai $p$-vành sao cho $l(C) \geqslant l(C')$, và gọi $\pi$ (tương ứng $\pi'$) là đồng cấu chính tắc của $C$ (tương ứng $C'$) lên $\kappa_C$ (tương ứng $\kappa_{C'}$). Gọi $(x_\lambda)_{\lambda \in \Lambda}$ (tương ứng $(x'_\lambda)_{\lambda \in \Lambda}$) là một họ các phần tử của $C$ (tương ứng của $C'$) mà ảnh qua $\pi$ (tương ứng $\pi'$) là một $p$-cơ sở của $\kappa_C$ (tương ứng $\kappa_{C'}$). Gọi $v$ là một đẳng cấu từ $\kappa_C$ lên $\kappa_{C'}$ sao cho $v(\pi(x_\lambda)) = \pi'(x'_\lambda)$ với mọi $\lambda \in \Lambda$. Khi đó tồn tại một đồng cấu duy nhất $u$ từ $C$ vào $C'$, sao cho $v \circ \pi = \pi' \circ u$ và $u(x_\lambda) = x'_\lambda$ với mọi $\lambda \in \Lambda$. Nó là toàn ánh. Nếu $l(C) = l(C')$, thì nó là một đẳng cấu.*

Hãy chứng minh sự tồn tại của $u$. Gọi $A$ là vành con của $C \times C'$ gồm các cặp $(x, x')$ sao cho $v(\pi(x)) = \pi'(x')$. Ánh xạ $(x, x') \mapsto \pi(x)$ là một đồng cấu toàn ánh các vành từ A lên $\kappa_C$. Hạt nhân của nó $m$, bằng $pC \times pC'$, do đó là một iđêan cực đại của A. Không gian con tôpô A của $C \times C'$ là đóng trong $C \times C'$, nên đầy đủ, và tôpô cảm sinh trên A bởi tôpô của $C \times C'$ là tôpô $m$-adic. Vì thế A là một vành địa phương tách biệt đầy đủ với iđêan cực đại $m$ (III, § 2, No. 13, Prop. 19). Với mọi $\lambda \in \Lambda$, theo giả thiết ta có $(x_\lambda, x'_\lambda) \in A$; nếu $\xi_\lambda$ là lớp của $(x_\lambda, x'_\lambda)$ modulo $m$, thì họ $(\xi_\lambda)_{\lambda \in \Lambda}$ là một $p$-cơ sở của trường $A/m$. Theo định lý 1 của No. 2, tồn tại một vành con Cohen $C''$ của A, và chỉ có một, chứa $(x_\lambda, x'_\lambda)$ với mọi $\lambda \in \Lambda$. Ta có $l(C'') = l(C) \geq l(C')$. Hạn chế trên $C''$ của phép chiếu từ $C \times C'$ lên C là một đồng cấu $h : C'' \to C$ cảm sinh một đẳng cấu từ $\kappa_{C''}$ lên $\kappa_C$. Theo Prop. 2, c) của No. 2, $h$ là một đẳng cấu từ $C''$ lên C. Tương tự, ta thấy rằng hạn chế $h'$ trên $C''$ của phép chiếu từ $C \times C'$ lên $C'$ là một đồng cấu toàn ánh từ $C''$ lên $C'$. Do đó, $C''$ là đồ thị của một đồng cấu toàn ánh $u = h' \circ h^{-1}$ từ C lên $C'$, và hiển nhiên ta có $v \circ \pi = \pi' \circ u$, $u(x_\lambda) = x'_\lambda$ với mọi $\lambda \in \Lambda$. Hơn nữa, nếu $l(C) = l(C')$, thì $u$ là một đẳng cấu.

Hãy chứng minh tính duy nhất của $u$. Gọi $u_1$ là một đồng cấu từ C vào $C'$ sao cho $v \circ \pi = \pi' \circ u_1$ và $u_1(x_\lambda) = x'_\lambda$ với mọi $\lambda \in \Lambda$, và gọi $C_1$ là đồ thị của $u_1$. Ngay lập tức thấy rằng $C_1$ là một vành con Cohen của A, chứa $(x_\lambda, x'_\lambda)$ với mọi $\lambda \in \Lambda$, do đó $C_1 = C''$ (định lý 1 của No. 2) và cuối cùng $u_1 = u$.

#### Mệnh đề 5 {#ac-ix-s2-prop-5 .statement}

Cho k là một trường có đặc số p, và cho n là một số nguyên $\geq 1$, hoặc $+ \infty$. Tồn tại một p-vành có độ dài n mà trường thặng dư đẳng cấu với k.

Vành $W(k)$ các vectơ Witt với hệ số trong k là một vành địa phương nguyên phân tách đầy đủ mà trường thặng dư đẳng cấu với k ($§ 1$, no. 8, mệnh đề 8), và ta có $p \cdot 1_{W(k)} \neq 0$ (loc. cit., công thức (52)). Cho C là một vành con Cohen của $W(k)$ (no. 2, định lý 1). Khi đó C là một p-vành có độ dài $+ \infty$ mà trường thặng dư đẳng cấu với k, và, nếu n là một số nguyên $\geq 1$, thương $C/p^nC$ là một p-vành có độ dài n mà trường thặng dư đẳng cấu với k.

#### Nhận xét 1 {#ac-ix-s2-n3-rem-1 .statement}

Cho n là một số nguyên $\geq 1$ và S là một p-cơ sở của k. Có thể chứng minh rằng vành con của $W_n(k)$ được sinh bởi $W_n(k^{p^n})$ và bởi các phần tử $[\xi, 0, ..., 0]$ ($\xi \in S$), là một p-vành có độ dài n mà trường thặng dư đẳng cấu với k (xem p. 72, bài tập 10).

#### Nhận xét 2 {#ac-ix-s2-n3-rem-2 .statement}

Bạn đọc sẽ tìm thấy trong Phụ lục một chứng minh của mệnh đề 5 không dùng các kết quả của $§ 1$, cũng không dùng định lý tồn tại đối với các vành con Cohen (no. 2, định lý 1).

#### Hệ quả {#ac-ix-s2-n3-cor-1 .statement}

Cho C là một p-vành có độ dài hữu hạn n. Tồn tại một p-vành $C'$ có độ dài vô hạn sao cho C đẳng cấu với $C'/p^nC'$.

Theo mệnh đề 5, tồn tại một p-vành $C'$ có độ dài vô hạn sao cho $\kappa_{C'}$ đẳng cấu với $\kappa_C$. Khi đó $C'/p^nC' = C'_n$ là một p-vành có độ dài n, và trường $\kappa_{C'_n}$ đẳng cấu với $\kappa_{C'}$, do đó với $\kappa_C$. Vậy theo mệnh đề 4, các vành C và $C'_n$ là đẳng cấu.

### 4. Các Đại Diện Nhân Tính

#### Mệnh đề 6 {#ac-ix-s2-prop-6 .statement}

Cho C là một p-vành, mà trường thặng dư k là hoàn hảo. Giả sử rằng C có độ dài hữu hạn n (tương ứng vô hạn). Tồn tại một đẳng cấu duy nhất $u : W_n(k) \to C$ (tương ứng $u : W(k) \to C$) cảm sinh, bằng cách chuyển qua các thương, ánh xạ đồng nhất của k.

Vì $W_n(k)$ (tương ứng $W(k)$) là một p-vành có trường thặng dư k, và có độ dài n (tương ứng có độ dài vô hạn) (No. 1, Ví dụ 2), và vì $\varnothing$ là một p-cơ sở của trường hoàn hảo k, nên mệnh đề 6 là một trường hợp riêng của mệnh đề 4 của No. 3.

#### Định lý 2 {#ac-ix-s2-thm-2 .statement}

Cho A là một vành địa phương phân tách đầy đủ, k là trường thặng dư của nó và $\pi$ là đồng cấu chính tắc từ A lên k. Giả sử rằng k là một trường hoàn hảo có đặc số p.

a) Tồn tại một đồng cấu vành duy nhất $u : W(k) \to A$ sao cho $\pi(u(a)) = a_0$ đối với $a = (a_n)_{n \in \mathbf{N}}$ trong W(k).

b) Đồng cấu u liên tục khi W(k) được trang bị tôpô $pW(k)$-adic, và ảnh của u là vành con Cohen duy nhất của A.

Theo định lý 1 của no. 2, tồn tại một vành con Cohen duy nhất của A; ta ký hiệu nó là C. Cho u là một đồng cấu từ W(k) vào A sao cho $\pi(u(a)) = a_0$ với mọi $a = (a_n)_{n \in \mathbf{N}}$ trong W(k); ngay lập tức thấy rằng ảnh của u là một vành con Cohen của A, do đó bằng C. Sự tồn tại và tính duy nhất của u khi đó suy ra từ mệnh đề 6. Tôpô $pC$-adic của C được cảm sinh bởi tôpô $m_A$-adic của A (no. 2, định lý 1, b)), do đó suy ra tính liên tục của u.

Để có một phép dựng trực tiếp của u, xem p. 70, bài tập 6.

#### Mệnh đề 7 {#ac-ix-s2-prop-7 .statement}

Giữ lại các giả thiết và ký hiệu của định lý 2. Tồn tại một tập con nhân tính duy nhất S của A sao cho $\pi$ cảm sinh một song ánh từ S lên k. Để một phần tử a của A thuộc S, điều kiện cần và đủ là với mọi $n \in \mathbf{N}$, tồn tại một phần tử $a_n$ của A sao cho $a = a_n^{p^n}$. Tập S là tập các phần tử có dạng $u(x, 0, 0, ...)$.

Trước hết ta chứng minh tính duy nhất của S. Cho S là một tập con nhân tính của A, sao cho $\pi$ cảm sinh một song ánh từ S lên k. Cho T là tập các phần tử của A là các lũy thừa bậc $p^n$ đối với mọi $n \in \mathbf{N}$.

a) Ta có $S \subset T$ : Cho $a \in S$ và $n \in \mathbf{N}$; vì trường k là hoàn hảo, tồn tại một phần tử $x_n$ của k sao cho $x_n^{p^n} = \pi(a)$; vì ta có $\pi(S) = k$, tồn tại một phần tử $a_n$ của S sao cho $x_n = \pi(a_n)$. Khi đó ta có $\pi(a_n^{p^n}) = \pi(a)$ do đó $a_n^{p^n} = a$ vì hạn chế của $\pi$ lên S là đơn ánh.

b) Hạn chế của $\pi$ lên T là đơn ánh: giả sử a và b là hai phần tử của T sao cho $\pi(a) = \pi(b)$. Cho $n \in \mathbf{N}$; tồn tại hai phần tử $a_n$ và $b_n$ của A sao cho $a = a_n^{p^n}, b = b_n^{p^n}$. Khi đó ta có $\pi(a_n)^{p^n} = \pi(b_n)^{p^n}$, do đó $\pi(a_n) = \pi(b_n)$, nghĩa là $a_n \equiv b_n$ mod. $m_A$. Theo Bổ đề 1 của § 1, No. 1, ta có $a_n^{p^n} \equiv b_n^{p^n}$ mod. $m_A^{n+1}$ nghĩa là $a \equiv b$ mod. $m_A^{n+1}$. Vì n là tùy ý, suy ra $a = b$.

Các tính chất a) và b) ở trên, cùng với công thức $\pi(S) = k$, suy ra quan hệ $S = T$, do đó có tính duy nhất.

Bây giờ ta chứng minh sự tồn tại của S. Với ký hiệu của Định lý 2, đặt $\varphi = u \circ \tau_k$, nghĩa là (§ 1, No. 6)

(2)
$$
\varphi(x) = u(x, 0, 0, ...)
$$
với mọi $x \in k$. Theo Mệnh đề 4 của loc. cit., ta có

(3)
$$
\varphi(1) = 1,\quad \varphi(xy) = \varphi(x) \varphi(y) \text{ với } x, y \text{ trong } k.
$$

Rõ ràng ánh xạ $\pi \circ \varphi$ là ánh xạ đồng nhất của $k$. Do đó ảnh S của $\varphi$ thỏa mãn các điều kiện của Mệnh đề 7.

Các phần tử của S thường được gọi là các đại diện nhân tính (hay các đại diện Teichmüller) của A.

#### Nhận xét 1 {#ac-ix-s2-n4-rem-1 .statement}

Giữ các giả thiết và ký hiệu ở trên. Ta có
$$
a = \sum_{n=0}^{\infty} p^n \tau_k(a_n^{p^{-n}}) \quad (a = (a_n)_{n \in \mathbf{N}} \in \mathbf{W}(k))
$$
theo Mệnh đề 7 của § 1, No. 8. Do đó
(4)
$$
u(a) = \sum_{n=0}^{\infty} p^n \varphi(a_n^{p^{-n}})
$$
với mọi $a = (a_n)_{n \in \mathbf{N}}$ trong $\mathbf{W}(k)$, vì $u$ là liên tục (Định lý 2, b)). Theo công thức (4), vành con Cohen duy nhất của A gồm các phần tử có dạng $\sum_{n=0}^{\infty} p^n s_n$ với $s_n \in S$ với mọi số nguyên $n \geq 0$.

#### Nhận xét 2 {#ac-ix-s2-n4-rem-2 .statement}

Cho A là một vành địa phương tách biệt và đầy đủ, $k$ là trường thặng dư của nó và $\pi$ là đồng cấu chính tắc từ A lên $k$. Có thể chứng minh rằng tồn tại một tập con nhân tính S của A (nói chung không duy nhất) sao cho $\pi$ cảm sinh một song ánh từ S lên $k$ (xem p. 72, Bài tập 11).

#### Ví dụ 1 {#ac-ix-s2-n4-exa-1 .statement}

Cho $k$ là một trường hoàn hảo có đặc số $p$. Các đại diện nhân tính của vành $\mathbf{W}(k)$ là các vectơ Witt $\tau(x) = (x, 0, 0, ...)$ với $x \in k$.

#### Ví dụ 2 {#ac-ix-s2-n4-exa-2 .statement}

Cho A là một vành địa phương nguyên, tách biệt và đầy đủ. Giả sử rằng trường thặng dư $k$ của A là hữu hạn, có $q = p^f$ phần tử, do đó là hoàn hảo và có đặc số $p$. Ta có $x^q = x$ với mọi $x \in k$, do đó $s^q = s$ với mọi đại diện nhân tính s. Suy ra rằng tập hợp các đại diện nhân tính gồm 0 và $q - 1$ căn bậc $(q - 1)$ của đơn vị trong trường phân thức của A. Nếu trường phân thức của A là compact địa phương, sự tồn tại của các đại diện nhân tính cũng suy ra từ VI, § 9, No. 2, Mệnh đề 3 (xem thêm VI, § 9, Bài tập 5).

#### Ví dụ 3 {#ac-ix-s2-n4-exa-3 .statement}

Đặc biệt hơn, xét trường hợp $A = \mathbf{Z}_p$. Khi đó các đại diện nhân tính là 0 và các căn bậc $(p - 1)$ của đơn vị trong trường phân thức $\mathbf{Q}_p$ của $\mathbf{Z}_p$.

### 5. Cấu trúc của các vành địa phương Noether đầy đủ

Cho $A$ và $C$ là các vành địa phương Noether đầy đủ, và cho $u$ là một đồng cấu địa phương từ $C$ vào $A$, cảm sinh, bằng cách chuyển qua thương, một đẳng cấu của $\kappa_C$ lên $\kappa_A$. Cho $(p_1, ..., p_m)$ là một dãy sinh iđêan $m_C$ của $C$, và cho $t_1, ..., t_n$ là các phần tử của $m_A$. Đặt $B = C[[T_1, ..., T_n]]$.

#### Bổ đề 3 {#ac-ix-s2-lem-3 .statement}

a) Tồn tại một đồng cấu duy nhất $v : B \to A$ mở rộng $u$ và ánh xạ $T_i$ thành $t_i$ với $1 \leq i \leq n$.

b) Để $v$ là toàn ánh, điều kiện cần và đủ là dãy $(u(p_1), ..., u(p_m), t_1, ..., t_n)$ sinh iđêan $m_A$ của $A$, hay tương đương, các lớp của những phần tử này modulo $m_A^2$ sinh $m_A/m_A^2$ như một không gian vectơ trên trường $\kappa_A$.

c) Để $v$ biến $A$ thành một $B$-đại số hữu hạn, điều kiện cần và đủ là dãy $(u(p_1), ..., u(p_m), t_1, ..., t_n)$ sinh một iđêan định nghĩa của $A$ (đối với tôpô $m_A$-adic).

Cho $n$ ký hiệu iđêan của vành $B$ sinh bởi $T_1, ..., T_n$. Mọi đồng cấu $v$ từ $B$ vào $A$ mở rộng $u$ và sao cho $v(T_i) = t_i$ đều ánh xạ $n$ vào $m_A$, và do đó là liên tục khi $B$ được trang bị tôpô $n$-adic. Khi đó sự tồn tại và tính duy nhất của $v$ suy ra từ A, IV, p. 26, Prop. 4.

Vành $B = C[[T_1, ..., T_n]]$ là một vành địa phương Noether đầy đủ (III, § 2, No. 10, Hệ quả 6 của Định lý 2 và No. 6, Mệnh đề 6), mà iđêan cực đại $m_B$ được sinh bởi $p_1, ..., p_m, T_1, ..., T_n$. Do đó $v(m_B) \subset m_A$ và $v$ xác định một đồng cấu gr$(v)$ từ $\operatorname{gr}(B) = \bigoplus_{n=0}^\infty m_B^n/m_B^{n+1}$ vào $\operatorname{gr}(A) = \bigoplus_{n=0}^\infty m_A^n/m_A^{n+1}$. Bây giờ vành $\operatorname{gr}(A)$ được sinh bởi $A/m_A = \kappa_A$ và $m_A/m_A^2$, gr$(v)$ gây ra một đẳng cấu của $\kappa_B = \kappa_C$ lên $\kappa_A$, và các lớp modulo $m_B^2$ của các phần tử $p_1, ..., p_m, T_1, ..., T_n$ sinh ra $m_B/m_B^2$ như một không gian vectơ trên $\kappa_B$; hơn nữa $v$ là toàn ánh khi và chỉ khi gr$(v)$ là toàn ánh (III, § 2, No. 8, Hệ quả 2 của Định lý 1). Điều này chứng minh $b$.

Iđêan của $A$ được sinh bởi dãy $(u(p_1), ..., u(p_m), t_1, ..., t_n)$ không gì khác hơn là $v(m_B)$ $A$. Vì $m_A$ chứa $v(m_B)$, $A$ là một vành Zariski đối với tôpô $v(m_B)$ $A$-adic. Vành $A/v(m_B)$ $A$ là Artin khi và chỉ khi độ dài của nó như một $A$-môđun là hữu hạn. Nhưng vì mọi môđun đơn trên $A$ đều bị triệt tiêu bởi $m_A$ và vì, theo giả thiết, $A/m_A$ và $B/m_B$ là đẳng cấu, điều này xảy ra khi và chỉ khi chiều trên trường $B/m_B$ của không gian vectơ $A/v(m_B)$ $A$ là hữu hạn. Bởi IV, § 2, No. 5, Hệ quả 2 của Mệnh đề 9, do đó ta thấy rằng $v(m_B)$ $A$ là một iđêan định nghĩa của $A$ khi và chỉ khi chiều của $A/v(m_B)$ $A$ trên $B/m_B$ là hữu hạn. Điều này quả thật đúng nếu $A$ là một $B$-đại số hữu hạn.

Giả sử rằng $v(m_B)$ $A$ là một iđêan định nghĩa của $A$. Khi đó tôpô $m_B$-adic của $B$-môđun $A$ trùng với tôpô $m_A$-adic của vành $A$, và vì thế là tách. Vì $A/v(m_B)$ $A$ là một môđun hữu hạn sinh trên $B/m_B$, nên $A$ là một $B$-môđun hữu hạn sinh (III, § 2, No. 3, Ví dụ 3 và No. 9, hệ quả 1 của Mệnh đề 12). Điều này chứng minh $c$.

#### Bổ đề 4 {#ac-ix-s2-lem-4 .statement}

Giả sử rằng vành địa phương Noether C là chính quy, và rằng $(p_1, ..., p_m)$ là một hệ tọa độ của C (VIII, § 5, No. 1, Định nghĩa 1).

a) Nếu dãy $(u(p_1), ..., u(p_m), t_1, ..., t_n)$ là cát tuyến đối với A (VIII, § 3, No. 2, Định nghĩa 1), đồng cấu $v : B \to A$ là đơn cấu.

b) Để $v$ là đơn cấu và làm cho A thành một đại số hữu hạn trên B, điều kiện cần và đủ là $(u(p_1), ..., u(p_m), t_1, ..., t_n)$ là một dãy cát tuyến cực đại đối với A. Khi đó A có chiều $m + n$.

Để dãy $(u(p_1), ..., u(p_m), t_1, ..., t_n)$ là một dãy cát tuyến cực đại đối với A, điều kiện cần và đủ là nó sinh ra một iđêan định nghĩa của A, và A có chiều $m + n$ (VIII, § 3, No. 2, Định lý 1). Theo bổ đề 3, c), điều này có nghĩa là A là một B-đại số hữu hạn, và là một vành có chiều $m + n$. Bây giờ C là một vành nguyên Noether có chiều $m$, do đó $B = C[[T_1, ..., T_n]]$ là một vành nguyên Noether có chiều $m + n$ (VIII, § 3, No. 4, hệ quả 3 của Mệnh đề 8). Nếu A là một B-đại số hữu hạn, và nếu $a$ là hạt nhân của $v$, ta có $\dim(A) = \dim(B/a)$ (VIII, § 2, No. 3, định lý 1, c)); vì B là một vành nguyên có chiều hữu hạn, ta có $\dim(B/a) < \dim(B)$ nếu $a \neq \{0\}$ (VIII, § 1, No. 3, mệnh đề 6, e)). Do đó, nếu A là một B-đại số hữu hạn, $v$ là đơn cấu khi và chỉ khi A có chiều $m + n$. Điều này chứng minh b).

Giả sử rằng dãy $(u(p_1), ..., u(p_m), t_1, ..., t_n)$ các phần tử của $m_A$ là cát tuyến. Có thể thêm vào đó (VIII, § 3, No. 2, Định lý 1) các phần tử $t_{n+1}, ..., t_{n+r}$ của $m_A$ để biến nó thành một dãy cát tuyến cực đại. Theo điều đi trước, khi đó tồn tại một đồng cấu đơn ánh $w$ của $C[[T_1, ..., T_n, T_{n+1}, ..., T_{n+r}]] = B[[T_{n+1}, ..., T_{n+r}]]$ mở rộng $v$ và ánh xạ $T_{n+j}$ tới $t_{n+j}$ với $1 \leq j \leq r$. Do đó $v$ là đơn cấu. Điều này chứng minh a).

#### Định lý 3 {#ac-ix-s2-thm-3 .statement}

Cho A là một vành địa phương, Noether và đầy đủ, có trường thặng dư k với đặc số p. Cho C là một vành p có độ dài vô hạn, mà trường thặng dư đẳng cấu với k (No. 3, Mệnh đề 5).

a) Gọi m là chiều của không gian vectơ $m_A/(m_A^2 + pA)$ trên trường k. Tồn tại một iđêan $a$ của vành $C[[T_1, ..., T_m]]$ sao cho A đẳng cấu với $C[[T_1, ..., T_m]]/a$.

b) Gọi d là chiều của A. Giả sử rằng $p1_A$ không phải là một ước của 0 trong A. Khi đó tồn tại một vành con $A'$ của A đẳng cấu với $C[[T_1, ..., T_{d-1}]]$ và sao cho A là một đại số hữu hạn trên $A'$.

Cho $C'$ là một vành con Cohen của $A$ (No. 2, Định lý 1). Vì $C$ có độ dài vô hạn, tồn tại một đồng cấu từ $C$ lên $C'$ (No. 3, Mệnh đề 4). Do đó, tồn tại một đồng cấu địa phương $u : C \to A$. Hãy chọn các phần tử $t_1, ..., t_m$ của $m_A$ sao cho các lớp của chúng tạo thành một cơ sở của không gian vectơ $m_A/(m_A^2 + pA)$ trên trường $k$. Ta có $u(p1_C) = p1_A$, và Bổ đề 3, b) chứng minh sự tồn tại của một đồng cấu toàn ánh từ $C[[T_1, ..., T_m]]$ lên $A$, kéo dài $u$ và ánh xạ $T_i$ lên $t_i$ với $1 \leq i \leq m$. Điều này chứng minh a).

Giả sử rằng $p1_A$ không là một ước của $0$ trong $A$, do đó là secant đối với $A$ (VIII, § 3, No. 2, Mệnh đề 3). Khi đó tồn tại (VIII, § 3, No. 2, Định lý 1) các phần tử $t_1, ..., t_{d-1}$ của $m_A$ sao cho dãy $(p1_A, t_1, ..., t_{d-1})$ là một dãy secant cực đại của $A$. Vành địa phương Noether $C$ là chính quy, và $(p1_C)$ là một hệ tọa độ của $C$. Mệnh đề b) của Định lý 3 khi đó suy ra từ Bổ đề 4, b).

## BÀI TẬP {#ac-ix-s2-exercises}

Trong các bài tập của § 2, $p$ là một số nguyên tố cố định. Nếu $a$ là một iđêan của một vành $A$, $a^p$ ký hiệu iđêan sinh bởi các phần tử $a^p$, trong đó $a$ chạy qua $a$.

Xem [bài tập của § 2](exercises/s2/).
