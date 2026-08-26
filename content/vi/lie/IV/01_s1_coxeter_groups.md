---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IV
chapter_title: COXETER GROUPS AND TITS SYSTEMS
section: 1
section_title: Coxeter Groups
lang: vi
source: lie-iv-vi
pdf_pages: 0014-0028, 0044-0056
extraction: ocr
subsections:
    - "no": 1
      title: LENGTH AND REDUCED DECOMPOSITIONS
      page: 0
      pdf_page: 14
    - "no": 2
      title: DIHEDRAL GROUPS
      page: 0
      pdf_page: 15
    - "no": 3
      title: FIRST PROPERTIES OF COXETER GROUPS
      page: 0
      pdf_page: 17
    - "no": 4
      title: REDUCED DECOMPOSITIONS IN A COXETER GROUP
      page: 0
      pdf_page: 18
    - "no": 5
      title: THE EXCHANGE CONDITION
      page: 0
      pdf_page: 20
    - "no": 6
      title: CHARACTERISATION OF COXETER GROUPS
      page: 0
      pdf_page: 23
    - "no": 7
      title: FAMILIES OF PARTITIONS
      page: 0
      pdf_page: 23
    - "no": 8
      title: SUBGROUPS OF COXETER GROUPS
      page: 0
      pdf_page: 25
    - "no": 9
      title: COXETER MATRICES AND COXETER GRAPHS
      page: 0
      pdf_page: 26
statements: 30
exercises: 16
content_sha256: 366ca6a5d5522dffa822c7bc14c4c955c09d3ddb4eb1600ad3c05f4924f580f0
translated_from: content/en/lie/IV/01_s1_coxeter_groups.md
source_content_sha256: 846049a9e3a37f523599bdee0b7a1e284e6822579c039f0c2d0832710fdc4cd5
translation_model: gpt-5-6-mini, gpt-5-6, gpt-5-mini
translation_run: translate-vi-80dc7717
glossary_version: 34
glossary_terms_sha256: 1a56c4598d836c4a6712d5960d9e01ab5cb62db39deaf13239056767c24fd6cc
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 1. NHÓM COXETER

Trong tiết này, W ký hiệu một nhóm được viết theo phép nhân, với phần tử đơn vị 1, và S ký hiệu một tập hợp các phần tử sinh của W sao cho S = S^{-1} và 1 \notin S. Mọi phần tử của W là tích của một dãy hữu hạn các phần tử của S. Từ No. 3 trở đi, ta giả sử rằng mọi phần tử của S đều có cấp 2.

### 1. ĐỘ DÀI VÀ CÁC PHÂN TÍCH RÚT GỌN

#### Định nghĩa 1 {#lie-iv-s1-def-1 .statement}

Cho w \in W. Độ dài của w (đối với S), ký hiệu là l_S(w) hoặc đơn giản là l(w), là số nguyên nhỏ nhất q \geq 0 sao cho w là tích của một dãy gồm q phần tử của S. Một phân tích rút gọn của w (đối với S) là một dãy bất kỳ s = (s_1, \ldots, s_q) gồm các phần tử của S sao cho w = s_1 \cdots s_q và q = l(w).

Như vậy 1 là phần tử duy nhất có độ dài 0 và S gồm các phần tử có độ dài 1.

#### Mệnh đề 1 {#lie-iv-s1-prop-1 .statement}

Cho w và w' thuộc W. Ta có các công thức:

$$
l(ww') \leq l(w) + l(w'), \tag{1}
$$
$$
l(w^{-1}) = l(w), \tag{2}
$$
$$
|l(w) - l(w')| \leq l(ww'^{-1}). \tag{3}
$$

Cho (s_1, \ldots, s_p) và (s'_1, \ldots, s'_q) lần lượt là các phân tích rút gọn của w và w'. Khi đó l(w) = p và l(w') = q. Vì ww' = s_1 \ldots s_p s'_1 \ldots s'_q, ta có l(ww') \leq p + q, chứng minh (1). Vì S = S^{-1} và w^{-1} = s_p^{-1} \ldots s_1^{-1}, ta có l(w^{-1}) \leq p = l(w). Thay w bởi w^{-1} cho bất đẳng thức đối l(w) \leq l(w^{-1}), chứng minh (2). Thay w bởi ww'^{-1} trong (1) và (2) cho các hệ thức

$$
l(w) - l(w') \leq l(ww'^{-1}), \tag{4}
$$
$$
l(ww'^{-1}) = l(w'w^{-1}). \tag{5}
$$

Đổi chỗ $w$ và $w'$ trong (4) cho $l(w') - l(w) \leq l(ww'^{-1})$ theo (5), chứng minh (3).

#### Hệ quả {#lie-iv-s1-n1-cor-1 .statement}

*Cho $s = (s_1, \ldots, s_p)$ và $s' = (s'_1, \ldots, s'_q)$ là hai dãy các phần tử của $S$ sao cho $w = s_1 \ldots s_p$ và $w' = s'_1 \ldots s'_q$. Nếu dãy $(s_1, \ldots, s_p, s'_1, \ldots, s'_q)$ là một phân tích rút gọn của $ww'$, thì $s$ là một phân tích rút gọn của $w$ và $s'$ là một phân tích rút gọn của $w'$.*

Theo giả thiết, $l(w) \leq p$, $l(w') \leq q$ và $l(ww') = p + q$. Theo (1), ta phải có $l(w) = p$ và $l(w') = q$, do đó có hệ quả.

*Nhận xét* Theo các công thức (1) và (2), công thức $d(w, w') = l(ww'^{-1})$ xác định một khoảng cách trên $W$, bất biến qua các phép tịnh tiến phải.

### 2. CÁC NHÓM NHỊ DIỆN

#### Định nghĩa 2 {#lie-iv-s1-def-2 .statement}

*Một nhóm nhị diện là một nhóm được sinh bởi hai phần tử phân biệt có cấp hai.*

#### Ví dụ {#lie-iv-s1-n2-exa-1 .statement}

Cho $M$ là nhóm nhân $\{1, -1\}$, và cho $m$ là một số nguyên $\geq 2$ (tương ứng. $m = \infty$). Khi đó $M$ tác động lên nhóm $\mathbf{Z}/m\mathbf{Z}$ (tương ứng. lên $\mathbf{Z}$) bởi $(-1).x = -x$, và tích bán trực tiếp tương ứng của $M$ bởi $\mathbf{Z}/m\mathbf{Z}$ (tương ứng. của $M$ bởi $\mathbf{Z}$) được ký hiệu bởi $D_m$. Các phần tử của $D_m$ do đó là các cặp $(\varepsilon, x)$ với $\varepsilon = \pm 1$ và $x \in \mathbf{Z}/m\mathbf{Z}$ (tương ứng. $x \in \mathbf{Z}$); luật nhóm trên $D_m$ được cho bởi công thức
$$
(\varepsilon, x).(\varepsilon', x') = (\varepsilon \varepsilon', \varepsilon' x + x').
$$
Ta ký hiệu $\iota$ là lớp của 1 modulo $m$ (tương ứng. $\iota = 1$) và đặt
$$
\rho = (-1, 0), \quad \rho' = (-1, \iota), \quad \pi = (1, \iota).
$$
Khi đó $\rho^2 = \rho'^2 = 1$ và $\pi = \rho \rho'$. Các công thức
$$
\pi^n = (1, n\iota), \quad \rho \pi^n = (-1, n\iota)
$$
chỉ ra rằng $D_m$ là một nhóm nhị diện được sinh bởi $\{\rho, \rho'\}$.

#### Mệnh đề 2 {#lie-iv-s1-prop-2 .statement}

*Giả sử rằng $S$ gồm hai phần tử phân biệt $s$ và $s'$ có cấp 2.*

(i) *Nhóm con $P$ của $W$ sinh bởi $p = ss'$ là chuẩn, và $W$ là tích bán trực tiếp của nhóm con $T = \{1, s\}$ và $P$. Hơn nữa, $(W : P) = 2$.*

(ii) *Cho $m$ là cấp (hữu hạn hoặc vô hạn) của $p$. Khi đó $m \geq 2$ và $W$ có cấp $2m$. Có một đẳng cấu duy nhất $\varphi$ từ $D_m$ đến $W$ sao cho $\varphi(\rho) = s$ và $\varphi(\rho') = s'$.*

(i) Ta có $sps^{-1} = sss's = s's = p^{-1}$, và do đó
$$
sp^n s^{-1} = p^{-n}
$$

với mọi số nguyên $n$. Vì $W$ được sinh bởi $\{ s, s' \}$, và do đó bởi $\{ s, p \}$, nên nhóm con $P$ là chuẩn. Suy ra rằng $TP$ là một nhóm con của $W$, và vì $TP$ chứa $s$ và $s' = sp$, ta có $W = TP = P \cup sP$. Để chứng minh (i), do đó chỉ cần chỉ ra rằng $W \neq P$. Nếu $W = P$, nhóm $W$ sẽ giao hoán, nên $p^2 = s^2 s'^2 = 1$. Nhưng khi đó các phần tử duy nhất của $W = P$ sẽ là 1 và $p$, mâu thuẫn với giả thiết rằng $W$ chứa ít nhất ba phần tử, cụ thể là 1, $s$ và $s'$.

(ii) Vì $s \neq s'$, ta có $p \neq 1$ và do đó $m \geq 2$. Vì $P$ có cấp $m$ và $(W : P) = 2$, cấp của $W$ là $2m$. Nếu $m$ hữu hạn (tương ứng vô hạn), tồn tại một đẳng cấu $\varphi'$ từ $\mathbf{Z}/m\mathbf{Z}$ (tương ứng $\mathbf{Z}$) đến $P$ đưa $\pi$ đến $p$. Hơn nữa, tồn tại một đẳng cấu $\varphi''$ từ $M = \{ 1, -1 \}$ đến $T$ đưa $-1$ đến $s$. Nhóm $W$ là tích nửa trực tiếp của $T$ và $P$. Theo các công thức (9) và $\rho \pi^n \rho^{-1} = \pi^{-n}$, $\varphi'$ và $\varphi''$ cảm sinh một đẳng cấu $\varphi$ từ $D_m$ đến $W$ sao cho $\varphi(\rho) = s$ và $\varphi(\pi) = p$, và do đó $\varphi(\rho') = s'$. Tính duy nhất của $\varphi$ suy ra từ sự kiện rằng $D_m$ được sinh bởi $\{ \rho, \rho' \}$.

#### Nhận xét {#lie-iv-s1-n2-rem-1 .statement}

Xét một nhóm nhị diện $W$ có cấp $2m$ được sinh bởi hai phần tử phân biệt $s$ và $s'$ có cấp 2. Ký hiệu bởi $s_q$ (tương ứng $s'_q$) dãy có độ dài $q$ mà các số hạng được đánh số lẻ (tương ứng chẵn) bằng $s$ và các số hạng được đánh số chẵn (tương ứng lẻ) bằng $s'$, và gọi $w_q$ (tương ứng $w'_q$) là tích của dãy $s_q$ (tương ứng $s'_q$). Ta có

$$
w_{2k} = (ss')^k, \quad w_{2k+1} = (ss')^k s,
$$
$$
w'_{2k} = (s's)^k = (ss')^{-k}, \quad w'_{2k+1} = (s's)^k s' = (ss')^{-k-1} s.
$$

Nếu $s = (s_1, \ldots, s_q)$ là một phân tích thu gọn (đối với $\{ s, s' \}$) của một phần tử $w$ của $W$, thì rõ ràng $s_i \neq s_{i+1}$ với $1 \leq i \leq q-1$. Do đó, $s = s_q$ hoặc $s = s'_q$.

Nếu $m = \infty$, các phần tử $(ss')^n$ và $(ss')^n s$ với $n \in \mathbf{Z}$ là phân biệt. Do đó, các phần tử $w_q$ ($q \geq 0$) và $w'_q$ ($q > 0$) là phân biệt, và nếu $s$ là một phân tích rút gọn của $w_q$ (tương ứng $w'_q$) thì tất yếu ta có $s = s_q$ (tương ứng $s = s'_q$). Từ đó suy ra rằng $l(w_q) = l(w'_q) = q$ và rằng *tập hợp các phân tích rút gọn của các phần tử của $W$ gồm các $s_q$ và các $s'_q$*. Hơn nữa, mọi phần tử của $W$ đều có một phân tích rút gọn duy nhất.

Giả sử bây giờ rằng $m$ là *hữu hạn*. Nếu $q \geq 2m$, ta có $w_q = w_{q-2m}$ và $w'_q = w'_{q-2m}$; nếu $m \leq q \leq 2m$, ta có $w_q = w'_{2m-q}$, $w'_q = w_{2m-q}$. Do đó, cả $s_q$ lẫn $s'_q$ đều không là các phân tích rút gọn nếu $q > m$. Suy ra rằng mỗi phần tử trong số $2m$ phần tử của $W$ là một trong $2m$ phần tử $w_0 = w'_0$, $w_q$ và $w'_q$ với $1 \leq q \leq m-1$, và $w_m = w'_m$. Vậy $2m$ phần tử này là phân biệt và từ trên suy ra rằng $l(w_q) = l(w'_q) = q$ với $q \leq m$ và rằng *tập hợp các phân tích rút gọn của các phần tử của $W$ gồm các $s_q$ và các $s'_q$ với $0 \leq q \leq m$*. Mọi phần tử của $W$ ngoại trừ $w_m$ đều có một phân tích rút gọn duy nhất; $w_m$ có hai.

### 3. CÁC TÍNH CHẤT ĐẦU TIÊN CỦA NHÓM COXETER

Nhắc lại rằng từ nay ta giả sử rằng các phần tử của S có cấp 2.

#### Định nghĩa 3 {#lie-iv-s1-def-3 .statement}

$(W, S)$ được gọi là một hệ Coxeter nếu nó thỏa mãn điều kiện sau:

(C) Với $s$, $s'$ trong $S$, đặt $m(s, s')$ là cấp của $ss'$ và đặt $I$ là tập hợp các cặp $(s, s')$ sao cho $m(s, s')$ là hữu hạn. Tập sinh $S$ và các hệ thức $(ss')^{m(s,s')} = 1$ đối với $(s, s')$ trong $I$ lập thành một phép trình bày¹ của nhóm $W$.

Khi $(W, S)$ là một hệ Coxeter, người ta cũng nói, bằng sự lạm dụng ngôn ngữ, rằng $W$ là một nhóm Coxeter.

#### Ví dụ 1 {#lie-iv-s1-n3-exa-1 .statement}

Cho $m$ là một số nguyên $\geq 2$ hoặc $\infty$ và cho $W$ là một nhóm được xác định bởi một tập các phần tử sinh $S = {s, s'}$ và các hệ thức $s^2 = s'^2 = 1$ khi $m = \infty$, $s^2 = s'^2 = (ss')^m = 1$ khi $m$ là hữu hạn. Xét mặt khác nhóm nhị diện $D_m$ (no. 2, Ví dụ) và các phần tử $\rho$ và $\rho'$ của $D_m$ được xác định bởi (7). Vì $\rho^2 = (\rho')^2 = 1$ và $(\rho\rho')^m = 1$ khi $m$ là hữu hạn, tồn tại một đồng cấu duy nhất $f$ từ $W$ vào $D_m$ sao cho $f(s) = \rho$ và $f(s') = \rho'$. Vì $\rho\rho'$ có cấp $m$, suy ra rằng bản thân $ss'$ có cấp $m$. Do đó, $(W, S)$ là một hệ Coxeter, $W$ là một nhóm nhị diện có cấp $2m$ và $f$ là một đẳng cấu (Mệnh đề 2).

Bằng phép chuyển cấu trúc, suy ra rằng mọi nhóm nhị diện đều là một nhóm Coxeter.

#### Ví dụ 2 {#lie-iv-s1-n3-exa-2 .statement}

Cho $\mathfrak{S}_n$ là nhóm đối xứng bậc n, với $n \geq 2$. Cho $s_i$ là phép chuyển vị của i và $i+1$ với $1 \leq i < n$, và cho S = {s_1, ..., s_{n-1}}. Có thể chứng minh (§ 2, no.4, Ví dụ và § 1, Exerc. 4) rằng $(\mathfrak{S}_n, S)$ là một hệ Coxeter.

#### Ví dụ 3 {#lie-iv-s1-n3-exa-3 .statement}

Về sự phân loại các nhóm Coxeter hữu hạn, xem Chương 4, § 4.

#### Nhận xét {#lie-iv-s1-n3-rem-1 .statement}

Giả sử rằng (W, S) là một hệ Coxeter. Tồn tại một đồng cấu $\varepsilon$ từ W vào nhóm {1, -1} được đặc trưng bởi $\varepsilon(s) = -1$ với mọi $s \in S$. Ta gọi $\varepsilon(w)$ là dấu của w; nó bằng $(-1)^{l(w)}$. Công thức $\varepsilon(ww') = \varepsilon(w)\varepsilon(w')$ do đó chuyển thành $l(ww') \equiv l(w) + l(w') \mod 2$.

¹ Điều này có nghĩa là (W, S) có tính chất phổ quát sau: cho một nhóm G và một ánh xạ f từ S vào G sao cho $(f(s)f(s'))^{m(s,s')} = 1$ với (s, s') trong I, tồn tại một đồng cấu g từ W vào G mở rộng f. Đồng cấu này là duy nhất vì S sinh W. Một dạng tương đương của định nghĩa này là như sau. Cho $\overline{W}$ là một nhóm, f là một đồng cấu từ $\overline{W}$ vào W và h là một ánh xạ từ S vào $\overline{W}$ sao cho $f(h(s)) = s$ và $(h(s)h(s'))^{m(s,s')} = 1$ với (s, s') trong S và sao cho các h(s) (với $s \in S$) sinh $\overline{W}$. Khi đó f là đơn ánh (và do đó là một đẳng cấu từ $\overline{W}$ vào W).

#### Mệnh đề 3 {#lie-iv-s1-prop-3 .statement}

Giả sử rằng (W, S) là một hệ Coxeter. Khi đó, hai phần tử s và s' của S là liên hợp$^2$ trong W khi và chỉ khi điều kiện sau được thỏa mãn:

(I) Tồn tại một dãy hữu hạn $(s_1, \ldots, s_q)$ các phần tử của S sao cho $s_1 = s, s_q = s'$ và $s_j s_{j+1}$ có cấp lẻ hữu hạn với $1 \leq j < q$.

Cho s và s' trong S sao cho $p = ss'$ có cấp hữu hạn $2n + 1$. Theo (9), $sp^{-n} = p^n s$ do đó

$$
p^n sp^{-n} = p^n p^n s - p^{-1} s = s' ss = s',
$$

và $s'$ là liên hợp với s.

Với mọi s trong S, cho $A_s$ là tập hợp các $s' \in S$ thỏa mãn (I). Với các giả thiết trong (I), các phần tử $s_j$ và $s_{j+1}$ là liên hợp với nhau với $1 \leq j < q$ theo điều trên, do đó mọi phần tử $s'$ của $A_s$ đều liên hợp với s.

Cho $f$ là ánh xạ từ S vào $M = \{1, -1\}$ bằng 1 trên $A_s$ và bằng -1 trên $S - A_s$. Cho $s'$ và $s''$ trong S sao cho $s's''$ có cấp hữu hạn m. Khi đó $f(s') f(s'') = 1$ nếu $s'$ và $s''$ đều thuộc $A_s$ hoặc đều thuộc $S - A_s$. Trong trường hợp còn lại, $f(s') f(s'') = -1$, nhưng m là chẵn. Do đó $(f(s') f(s''))^m = 1$ trong mọi trường hợp. Vì (W, S) là một hệ Coxeter, tồn tại một đồng cấu g từ W vào M cảm sinh f trên S. Cho $s'$ là một liên hợp của s. Vì s thuộc hạt nhân của g, $s'$ cũng vậy, do đó $f(s') = g(s') = 1$ và cuối cùng $s' \in A_s$. Q.E.D.

### 4. CÁC PHÂN TÍCH RÚT GỌN TRONG MỘT NHÓM COXETER

Giả sử rằng (W, S) là một hệ Coxeter. Cho T là tập hợp các liên hợp trong W của các phần tử của S. Với mọi dãy hữu hạn $s = (s_1, \ldots, s_q)$ các phần tử của S, ký hiệu $\Phi(s)$ là dãy $(t_1, \ldots, t_q)$ các phần tử của T được xác định bởi

$$
t_j = (s_1 \ldots s_{j-1}) s_j (s_1 \ldots s_{j-1})^{-1} \quad \text{cho } 1 \leq j \leq q.
$$

Khi đó $t_1 = s_1$ và $s_1 \ldots s_q = t_q t_{q-1} \ldots t_1$. Với mọi phần tử $t \in T$, ký hiệu $n(s, t)$ là số các số nguyên $j$ sao cho $1 \leq j \leq q$ và $t_j = t$. Cuối cùng, đặt

$$
R = \{1, -1\} \times T.
$$

#### Bổ đề 1 {#lie-iv-s1-lem-1 .statement}

(i) Cho $w \in W$ và $t \in T$. Số $(-1)^{n(s, t)}$ có cùng giá trị $\eta(w, t)$ đối với mọi dãy $s = (s_1, \ldots, s_q)$ gồm các phần tử của S sao cho $w = s_1 \ldots s_q$.

(ii) Với $w \in W$, xét ánh xạ $U_w$ từ R vào chính nó được định nghĩa bởi

$$
U_w(\varepsilon, t) = (\varepsilon \cdot \eta(w^{-1}, t), wtw^{-1}) \quad (\varepsilon = \pm 1, t \in T).
$$

Ánh xạ $w \mapsto U_w$ là một đồng cấu từ W vào nhóm các phép hoán vị của R.

\footnotetext{2 Nhắc lại rằng hai phần tử (tương ứng, hai tập con) của một nhóm W được gọi là liên hợp nếu tồn tại một tự đẳng cấu trong của W biến phần tử này thành phần tử kia.}

Với $s \in S$, định nghĩa một ánh xạ $U_s$ từ $R$ vào chính nó bởi
$$
U_s(\varepsilon, t) = (\varepsilon.(-1)^{\delta_{s,t}}, st s^{-1}) \quad (\varepsilon = \pm 1, t \in T),
$$
trong đó $\delta_{s,t}$ là ký hiệu Kronecker. Ta thấy ngay lập tức rằng $U_s^2 = \mathrm{Id}_R$, điều này chỉ ra rằng $U_s$ là một phép hoán vị của $R$.

Cho $s = (s_1, \ldots, s_q)$ là một dãy các phần tử của S. Đặt $w = s_q \ldots s_1$ và $U_s = U_{s_q} \ldots U_{s_1}$. Ta sẽ chứng minh, bằng quy nạp theo $q$, rằng
$$
U_s(\varepsilon, t) = (\varepsilon.(-1)^{n(s,t)}, wt w^{-1}).
$$
Điều này hiển nhiên đối với $q = 0, 1$. Nếu $q > 1$, đặt $s' = (s_1, \ldots, s_{q-1})$ và
$$
w' = s_{q-1} \ldots s_1.
$$
Sử dụng giả thiết quy nạp, ta thu được
$$
\begin{align*}
U_s(\varepsilon, t) &= U_{s_q}(U_{s_q}(\varepsilon.(-1)^{n(s',t)}, w't w'^{-1})) \\
&= (\varepsilon.(-1)^{n(s',t)+\delta_{s_q,w't w'^{-1}}}, wt w^{-1}).
\end{align*}
$$
Nhưng $\Phi(s) = (\Phi(s'), w'^{-1} s_q w')$ và $n(s, t) = n(s', t) + \delta_{w', -1} s_q w', t$, chứng minh công thức (14).

Bây giờ cho $s, s' \in S$ sao cho $p = ss'$ có cấp hữu hạn $m$. Cho $s = (s_1, \ldots, s_{2m})$ là dãy các phần tử của $S$ được xác định bởi $s_j = s$ với $j$ lẻ và $s_j = s'$ với $j$ chẵn. Khi đó $s_{2m} \ldots s_1 = p^{-m} = 1$ và công thức (11) suy ra rằng
$$
t_j = p^{j-1} s \quad \text{với } 1 \leq j \leq 2m.
$$
Vì $p$ có cấp $m$, các phần tử $t_1, \ldots, t_m$ là phân biệt và $t_{j+m} = t_j$ với $1 \leq j \leq m$. Với mọi $t \in T$, số nguyên $n(s, t)$ do đó bằng 0 hoặc 2 và (14) chỉ ra rằng $U_s = \mathrm{Id}_R$. Nói cách khác, $(U_s U_{s'})^m = \mathrm{Id}_R$. Do đó, theo định nghĩa của các hệ Coxeter, tồn tại một đồng cấu $w \mapsto U_w$ từ $W$ vào nhóm các hoán vị của $R$ sao cho $U_s$ được cho bởi vế phải của (13). Khi đó $U_w = U_s$ với mọi dãy $s = (s_1, \ldots, s_q)$ sao cho $w = s_q \ldots s_1$ và Bổ đề 1 suy ra ngay lập tức từ (14).

#### Bổ đề 2 {#lie-iv-s1-lem-2 .statement}

*Cho $s = (s_1, \ldots, s_q)$, $\Phi(s) = (t_1, \ldots, t_q)$ và $w = s_1 \ldots s_q$. Cho $T_w$ là tập hợp các phần tử của $T$ sao cho $\eta(w, t) = -1$. Khi đó $s$ là một phân tích rút gọn của $w$ khi và chỉ khi các $t_i$ là phân biệt, và trong trường hợp đó $T_w = \{ t_1, \ldots, t_q \}$ và $\mathrm{Card}(T_w) = l(w)$.*

Rõ ràng $T_w \subset \{ t_1, \ldots, t_q \}$. Lấy $s$ là rút gọn, suy ra rằng $\mathrm{Card}(T_w) \leq l(w)$. Hơn nữa, nếu các $t_i$ là phân biệt, thì $n(s, t)$ bằng 1 hoặc 0 tùy theo $t$ có thuộc hoặc không thuộc $\{ t_1, \ldots, t_q \}$. Suy ra rằng $T_w = \{ t_1, \ldots, t_q \}$ và rằng $q = \mathrm{Card}(T_w) \leq l(w)$, điều này kéo theo rằng $s$ là rút gọn. Cuối cùng, giả sử rằng $t_i = t_j$ với $i < j$. Điều này cho $s_i = us_j u^{-1}$, với $u = s_{i+1} \ldots s_{j-1}$, do đó

$$
w = s_1 \ldots s_{i-1} s_{i+1} \ldots s_{j-1} s_{j+1} \ldots s_q.
$$

Điều này chứng tỏ rằng $s$ không phải là một phân tích rút gọn của $w$.

#### Bổ đề 3 {#lie-iv-s1-lem-3 .statement}

*Cho $w \in W$ và $s \in S$ sao cho $l(sw) \leq l(w)$. Với mọi dãy $s = (s_1, \ldots, s_q)$ gồm các phần tử của $S$ với $w = s_1 \ldots s_q$, tồn tại một số nguyên $j$ sao cho $1 \leq j \leq q$ và*

$$
ss_1 \ldots s_{j-1} = s_1 \ldots s_{j-1} s_j.
$$

Gọi $p$ là độ dài của $w$ và $w' = sw$. Theo *Nhận xét* của no. 3, $l(w') \equiv l(w) + 1$ mod. 2. Giả thiết $l(w') \leq l(w)$ và quan hệ

$$
|l(w) - l(w')| \leq l(ww'^{-1}) = l(s) = 1
$$

do đó dẫn đến $l(w') = p - 1$. Chọn một phân tích rút gọn

$$
(s'_1, \ldots, s'_{p-1})
$$

của $w'$ và đặt $s = (s, s'_1, \ldots, s'_{p-1})$ và $\Phi(s') = (t'_1, \ldots, t'_p)$. Rõ ràng $s'$ là một phân tích rút gọn của $w$ và $t'_1 = s$. Các phần tử $t'_1, \ldots, t'_p$ đôi một phân biệt theo Bổ đề 2, ta có $n(s', s) = 1$. Vì $w$ là tích của dãy $s$, ta có $n(s, s) \equiv n(s', s)$ mod. 2 theo Bổ đề 1, do đó $n(s, s) \neq 0$. Do đó, $s$ bằng một trong các phần tử $t_j$ của dãy $\Phi(s)$, suy ra bổ đề.

#### Nhận xét {#lie-iv-s1-n4-rem-1 .statement}

Tập hợp $T_w$ được định nghĩa trong Bổ đề 2 gồm các phần tử có dạng $w''sw''^{-1}$ tương ứng với các bộ ba $(w', w'', s) \in W \times W \times S$ sao cho $w = w''sw'$ và $l(w') + l(w'') + 1 = l(w)$.

### 5. ĐIỀU KIỆN TRAO ĐỔI

"Điều kiện trao đổi" là mệnh đề sau đây về $(W, S)$:

**(E)** *Cho $w \in W$ và $s \in S$ sao cho $l(sw) \leq l(w)$. Với mọi phân tích rút gọn $(s_1, \ldots, s_q)$ của $w$, tồn tại một số nguyên $j$ sao cho $1 \leq j \leq q$ và*

$$
ss_1 \ldots s_{j-1} = s_1 \ldots s_{j-1} s_j.
$$

Trong số này, ta giả thiết rằng $(W, S)$ thỏa mãn (E). Theo Bổ đề 3, điều này đúng nếu $(W, S)$ là một hệ Coxeter. Do đó, các kết quả của số này áp dụng cho các hệ Coxeter.

#### Mệnh đề 4 {#lie-iv-s1-prop-4 .statement}

*Cho $s \in S, w \in W$ và $s = (s_1, \ldots, s_q)$ là một phân tích rút gọn của $w$. Khi đó một trong các trường hợp sau đây phải xảy ra:*

a) $l(sw) = l(w) + 1$ và $(s, s_1, \ldots, s_q)$ là một phân tích rút gọn của $sw$.

b) $l(sw) = l(w) - 1$ và tồn tại một số nguyên $j$ sao cho $1 \leq j \leq q$, $(s_1, \ldots, s_{j-1}, s_{j+1}, \ldots, s_q)$ là một phân tích thu gọn của $sw$ và $(s, s_1, \ldots, s_{j-1}, s_{j+1}, \ldots, s_q)$ là một phân tích thu gọn của $w$.

Đặt $w' = sw$. Theo công thức (3) của no. 1, ta có
$$
|l(w) - l(w')| \leq l(s) = 1.
$$
Ta phân biệt hai trường hợp:

a) $l(w') > l(w)$. Khi đó $l(w') = q + 1$ và $w' = ss_1 \ldots s_q$, do đó
$$
(s, s_1, \ldots, s_q)
$$
là một phân tích thu gọn của $w'$.

b) $l(w') \leq l(w)$. Theo (E), tồn tại một số nguyên $j$ sao cho $1 \leq j \leq q$ và (16) được thỏa mãn. Khi đó $w = ss_1 \ldots s_{j-1} s_{j+1} \ldots s_q$ và do đó
$$
w' = s_1 \ldots s_{j-1} s_{j+1} \ldots s_q.
$$
Vì $q - 1 \leq l(w') \leq q$, suy ra $l(w') = q - 1$ và $(s_1, \ldots, s_{j-1}, s_{j+1}, \ldots, s_q)$ là một phân tích thu gọn của $w'$.

#### Bổ đề 4 {#lie-iv-s1-lem-4 .statement}

Cho $w \in W$ có độ dài $q \geq 1$, cho D là tập hợp các phân tích thu gọn của $w$, và cho F là một ánh xạ từ D vào một tập hợp E. Giả sử rằng $F(s) = F(s')$ nếu các phần tử $s = (s_1, \ldots, s_q); s' = (s'_1, \ldots, s'_q)$ của D thỏa mãn một trong các giả thiết sau:

a) $s_1 = s'_1$ hoặc $s_q = s'_q$.
b) Tồn tại s và $s'$ trong S sao cho $s_j = s'_k = s$ và $s_k = s'_j = s'$ với $j$ lẻ và $k$ chẵn.

Khi đó F là hằng.

A) Cho $s, s' \in D$ và đặt $t = (s'_1, s_1, \ldots, s_{q-1})$. Ta sẽ chứng minh rằng nếu $F(s) \neq F(s')$ thì $t \in D$ và $F(t) \neq F(s)$. Thật vậy, $w = s'_1 \ldots s'_q$ và do đó $s'_1 w = s'_2 \ldots s'_q$ có độ dài $< q$. Theo Mệnh đề 4, tồn tại một số nguyên $j$ sao cho $1 \leq j \leq q$ và dãy $u = (s'_1, s_1, \ldots, s_{j-1}, s_{j+1}, \ldots, s_q)$ thuộc D. Ta có $F(u) = F(s')$ theo điều kiện a); nếu $j \neq q$ thì ta sẽ có $F(s) = F(u)$ vì cùng một lý do, và do đó $F(s) = F(s')$ trái với giả thiết của ta. Vậy $j = q$ và do đó $t = u \in D$ và $F(t) = F(s') \neq F(s)$.

B) Cho s và $s'$ thuộc D. Với mọi số nguyên $j$ sao cho $0 \leq j \leq q + 1$, định nghĩa một dãy $s_j$ gồm q phần tử của S như sau:
$$
s_0 = (s'_1, \ldots, s'_q)
$$
$$
s_1 = (s_1, \ldots, s_q)
$$
$$
s_{q+1-k} = (s_1, s'_1, \ldots, s_1, s'_1, s_1, s_2, \ldots, s_k)
$$
với $q - k$ chẵn và $0 \leq k \leq q$
$$
s_{q+1-k} = (s'_1, s_1, \ldots, s_1, s'_1, s_1, s_2, \ldots, s_k)
$$
với $q - k$ lẻ và $0 \leq k \leq q$.

Ký hiệu (H_j) là mệnh đề "s_j \in D, s_{j+1} \in D \text{ và } F(s_j) \neq F(s_{j+1})". Theo A), (H_j) $\implies$ (H_{j+1}) với $0 \leq j < q$, và (H_q) không được thỏa mãn bởi điều kiện b). Do đó, (H_0) không được thỏa mãn. Vì $s_0 = s'$ và $s_1 = s$, suy ra $F(s) = F(s')$.

#### Mệnh đề 5 {#lie-iv-s1-prop-5 .statement}

*Cho M là một nửa nhóm (với phần tử đơn vị 1) và f là một ánh xạ từ S vào M. Với s, $s' \in S$, đặt m(s, s') là cấp của ss' và đặt*

$$
a(s, s') = \begin{cases}
(f(s)f(s'))^l & \text{nếu } m(s, s') = 2l, l \text{ hữu hạn} \\
(f(s)f(s'))^lf(s) & \text{nếu } m(s, s') = 2l + 1, l \text{ hữu hạn} \\
1 & \text{nếu } m(s, s') = \infty.
\end{cases}
$$

*Nếu $a(s, s') = a(s', s)$ bất cứ khi nào $s \neq s'$ thuộc S, tồn tại một ánh xạ g từ W vào M sao cho*
$$
g(w) = f(s_1) \ldots f(s_q)
$$
*đối với mọi $w \in W$ và mọi phân tích rút gọn $(s_1, \ldots, s_q)$ của w.*

Với mọi $w \in W$, đặt $D_w$ là tập hợp các phân tích rút gọn của w và $F_w$ là ánh xạ từ $D_w$ vào M được định nghĩa bởi
$$
F_w(s_1, \ldots, s_q) = f(s_1) \ldots f(s_q).
$$
Ta sẽ chứng minh bằng quy nạp theo độ dài của w rằng $F_w$ là hằng, điều này sẽ thiết lập Mệnh đề 5. Vì các trường hợp $l(w) = 0, 1$ là tầm thường, ta giả sử rằng $q \geq 2$ và rằng mệnh đề của ta đã được chứng minh cho các phần tử w với $l(w) < q$. Cho w có độ dài q và $s, s' \in D_w$; theo Bổ đề 4 chỉ cần chứng minh rằng $F_w(s) = F_w(s')$ trong các trường hợp a) và b) của bổ đề đó.

a) Công thức
$$
F_w(s_1, \ldots, s_q) = f(s_1)F_{w''}(s_2, \ldots, s_q) = F_{w'}(s_1, \ldots, s_{q-1})f(s_q)
$$
với $w' = s_1 \ldots s_{q-1}$ và $w'' = s_2 \ldots s_q$ cùng với giả thiết quy nạp chỉ ra rằng $F_w(s) = F_w(s')$ nếu $s_1 = s'_1$ hoặc $s_q = s'_q$.

b) Giả sử rằng tồn tại hai phần tử s và s' của S sao cho $s_j = s'_k = s$ và $s_k = s'_j = s'$ với j lẻ và k chẵn. Chỉ cần xét trường hợp $s \neq s'$. Khi đó các dãy s và s' là hai phân tích rút gọn phân biệt của w trong nhóm lưỡng diện sinh bởi s và s'. Theo *Nhận xét* trong no. 2, cấp m của ss' nhất thiết hữu hạn và, theo ký hiệu của nhận xét đó, $s = s_m$ và $s' = s'_m$. Do đó, $F_w(s) = a(s, s')$ và $F_w(s') = a(s', s)$ và vì vậy
$$
F_w(s) = F_w(s').
$$

### 6. ĐẶC TRƯNG CỦA CÁC NHÓM COXETER

#### Định lý 1 {#lie-iv-s1-thm-1 .statement}

(W, S) là một hệ Coxeter khi và chỉ khi nó thỏa mãn điều kiện trao đổi (E) của no. 5.

Bổ đề 3 của no. 4 chỉ ra rằng mọi hệ Coxeter đều thỏa mãn (E).

Ngược lại, giả sử rằng (E) được thỏa mãn. Cho G là một nhóm và f là một ánh xạ từ S vào G sao cho $(f(s)f(s'))^m = 1$ bất cứ khi nào s và $s'$ thuộc S và $ss'$ có cấp hữu hạn m. Theo Mệnh đề 5, tồn tại một ánh xạ g từ W vào G sao cho
$$
g(w) = f(s_1) \ldots f(s_q)
$$
bất cứ khi nào $w = s_1 \ldots s_q$ có độ dài q. Để chứng minh rằng (W, S) là một hệ Coxeter, chỉ cần chứng minh rằng g là một đồng cấu, điều này là một hệ quả của công thức
$$
g(sw) = f(s)g(w) \quad \text{với } s \in S, w \in W
$$
vì S sinh W. Theo Mệnh đề 4 của no. 5, chỉ có hai trường hợp có thể xảy ra:

a) $l(sw) = l(w) + 1$: nếu $(s_1, \ldots, s_q)$ là một phân tích rút gọn của w, thì $(s, s_1, \ldots, s_q)$ là một phân tích rút gọn của sw, do đó (21).

b) $l(sw) = l(w) - 1$: đặt $w' = sw$; khi đó $w = sw'$ và $l(sw') = l(w') + 1$. Theo a), $g(w) = f(s)g(sw)$ và do đó $f(s)g(w) = g(sw)$ vì $(f(s))^2 = 1$.

### 7. HỌ CÁC PHÂN HOẠCH

Giả sử rằng $(W, S)$ là một hệ Coxeter. Với mọi $s \in S$, gọi $P_s$ là tập hợp các phần tử $w$ trong W sao cho $l(sw) > l(w)$. Ta có các tính chất sau:

(A) $\bigcap_{s \in S} P_s = \{1\}$.

Thật vậy, cho $w \neq 1$ thuộc W và cho $(s_1, \ldots, s_q)$ là một phân tích rút gọn của $w$. Khi đó $q \geq 1$ và $(s_2, \ldots, s_q)$ là một phân tích rút gọn của $s_2w$, do đó $l(w) = q$ và $l(s_1w) = q - 1$. Suy ra, $w \notin P_{s_1}$.

(B) *Với mọi s trong S, các tập hợp $P_s$ và $sP_s$ tạo thành một phân hoạch của W.*

Cho $w \in W$ và $s \in S$. Theo Mệnh đề 4 của no. 5, ta phải phân biệt hai trường hợp:

a) $l(sw) = l(w) + 1$: khi đó $w \in P_s$.
b) $l(sw) = l(w) - 1$: đặt $w' = sw$ sao cho $w = sw'$; khi đó
$$
l(w') < l(sw')
$$
do đó $w' \in P_s$, nghĩa là $w \in sP_s$.

(C) *Cho s, s' thuộc S và cho w thuộc W. Nếu $w \in P_s$ và $ws' \in P_s$ thì $sw = ws'$.*

Gọi $q$ là độ dài của $w$. Từ $w \in P_s$ suy ra rằng $l(sw) = q + 1$; và từ $ws' \in P_s$ suy ra rằng $l(sws') = l(ws') - 1 \leq q$. Vì $l(sws') = l(sw) \pm 1$, cuối cùng ta có $l(ws') = q + 1$ và $l(sws') = q$.

Cho $(s_1, \ldots, s_q)$ là một phân tích rút gọn của $w$ và $s_{q+1} = s'$; khi đó $(s_1, \ldots, s_q, s_{q+1})$ là một phân tích rút gọn của phần tử $ws'$ có độ dài $q + 1$. Theo điều kiện đổi chỗ, tồn tại một số nguyên $j$ với $1 \leq j \leq q + 1$ sao cho
$$
ss_1 \ldots s_{j-1} = s_1 \ldots s_j.
$$
(22)
Nếu $1 \leq j \leq q$, ta sẽ có $sw = s_1 \ldots s_{j-1} s_{j+1} \ldots s_q$ mâu thuẫn với công thức $l(sw) = q + 1$. Vậy $j = q + 1$ và công thức (22) có thể được viết là $sw = ws'$.

Ngược lại, ta có kết quả sau:

#### Mệnh đề 6 {#lie-iv-s1-prop-6 .statement}

*Cho* $(P_s)_{s \in S}$ *là một họ các tập con của* $W$ *thỏa mãn* (C) *và các điều kiện sau*:

(A') $1 \in P_s$ *với mọi* $s \in S$.
(B') *Các tập hợp* $P_s$ *và* $sP_s$ *rời nhau với mọi* $s \in S$.

*Khi đó*, $(W, S)$ *là một hệ Coxeter và* $P_s$ *gồm các phần tử* $w$ *của* $W$ *sao cho* $l(sw) > l(w)$.

Cho $s \in S$ và $w \in W$. Có hai khả năng:

a) $w \notin P_s$. Cho $(s_1, \ldots, s_q)$ là một phân tích rút gọn của $w$ và
$$
w_j = s_1 \ldots s_j
$$
với $1 \leq j \leq q$; cũng đặt $w_0 = 1$. Vì $w_0 \in P_s$ theo (A') và vì $w = w_q$ không thuộc $P_s$, tồn tại một số nguyên $j$ với $1 \leq j \leq q$ sao cho $w_{j-1} \in P_s$ và $w_j = w_{j-1} s_j$ không thuộc $P_s$. Theo (C),
$$
sw_{j-1} = w_{j-1} s_j.
$$
Do đó ta đã chứng minh công thức
$$
ss_1 \ldots s_{j-1} = s_1 \ldots s_{j-1} s_j
$$
suy ra rằng $sw = s_1 \ldots s_{j-1} s_{j+1} \ldots s_q$ và $l(sw) < l(w)$.

b) $w \in P_s$: đặt $w' = sw$, sao cho $w' \notin P_s$ theo (B'). Theo a), ta có $l(sw') < l(w')$, tức là $l(w) < l(sw)$.

So sánh a) và b) chứng minh rằng $P_s$ gồm các $w \in W$ sao cho $l(sw) > l(w)$. Điều kiện trao đổi suy ra từ điều này như ta đã thấy trong a), do đó $(W, S)$ là một hệ Coxeter (Đl. 1 của no. 6).

### 8. NHÓM CON CỦA CÁC NHÓM COXETER

Trong số này, ta giả sử rằng $(W, S)$ là một hệ Coxeter. Với mọi tập con $X$ của $S$, ta ký hiệu $W_X$ là nhóm con của $W$ sinh bởi $X$.

#### Mệnh đề 7 {#lie-iv-s1-prop-7 .statement}

*Cho $w$ thuộc* $W$. *Tồn tại một tập con* $S_w$ *của* $S$ *sao cho* $\{s_1, \ldots, s_q\} = S_w$ *với mọi phân tích rút gọn* $(s_1, \ldots, s_q)$ *của* $w$.

Ký hiệu $M$ là nửa nhóm gồm các tập con của $S$ với luật hợp thành $(A, B) \mapsto A \cup B$; phần tử đơn vị của $M$ là $\varnothing$. Đặt $f(s) = \{s\}$ với $s \in S$. Ta sẽ áp dụng Mệnh đề 5 của no. 5 cho $M$ và $f$. Ta có $a(s, s') = \{s, s'\}$ với $s, s'$ thuộc $S$ nếu $m(s, s')$ là hữu hạn, do đó tồn tại một ánh xạ $g : w \mapsto S_w$ từ $W$ vào $M$ sao cho $g(w) = f(s_1) \cup \cdots \cup f(s_q)$, nghĩa là $S_w = \{s_1, \ldots, s_q\}$ đối với mọi $w \in W$ và mọi phân tích rút gọn $(s_1, \ldots, s_q)$ của $w$.

#### Hệ quả 1 {#lie-iv-s1-prop-7-cor-1 .statement}

*Với mọi tập con $X$ của $S$, nhóm con $W_X$ của $W$ gồm các phần tử $w$ của $W$ sao cho $S_w \subset X$.

Nếu $w = s_1 \ldots s_q$ với $s_1, \ldots, s_q$ thuộc $S$, thì $w^{-1} = s_q \ldots s_1$; do đó

$$
S_{w^{-1}} = S_w.
$$

Mệnh đề 4 của no. 5 chỉ ra rằng $S_{sw'} \subset \{s\} \cup S_{w'}$ với $s \in S$ và $w' \in W$, điều này suy ra công thức

$$
S_{ww'} \subset S_w \cup S_{w'}
$$

bằng quy nạp theo độ dài của $w$. Theo (23) và (24), tập hợp $U$ gồm các $w \in W$ sao cho $S_w \subset X$ là một nhóm con của $W$; ta có $X \subset U \subset W_X$, do đó $U = W_X$.

#### Hệ quả 2 {#lie-iv-s1-prop-7-cor-2 .statement}

*Với mọi tập con $X$ của $S$, ta có $W_X \cap S = X$.

Điều này suy ra từ Hệ quả 1 và công thức $S_s = \{s\}$ với $s$ thuộc $S$.

#### Hệ quả 3 {#lie-iv-s1-prop-7-cor-3 .statement}

*Tập hợp $S$ là một tập sinh cực tiểu của $W$.

Nếu $X \subset S$ sinh ra $W$, thì $W = W_X$ và do đó $X = S \cap W_X = S$ theo Hệ quả 2.*

#### Hệ quả 4 {#lie-iv-s1-prop-7-cor-4 .statement}

*Với mọi tập con $X$ của $S$ và mọi $w$ trong $W_X$, độ dài của $w$ đối với tập sinh $X$ của $W_X$ bằng $l_S(w)$.

Cho $(s_1, \ldots, s_q)$ là một phân tích rút gọn của $w$ được xem như một phần tử của $W$. Ta có $w = s_1 \ldots s_q$ và $s_j \in X$ với $1 \leq j \leq q$ (Hệ quả 1); hơn nữa, $w$ không thể là một tích của $q' < q$ phần tử của $X \subset S$ theo định nghĩa của $q = l_S(w)$.*

#### Định lý 2 {#lie-iv-s1-thm-2 .statement}

(i) *Với mọi tập con $X$ của $S$, cặp $(W_X, X)$ là một hệ Coxeter.*

(ii) Cho $(X_i)_{i \in I}$ là một họ các tập con của $S$. Nếu $X = \bigcap_{i \in I} X_i$, thì $W_X = \bigcap_{i \in I} W_{X_i}$.

(iii) Cho $X$ và $X'$ là hai tập con của $S$. Khi đó $W_X \subset W_{X'}$ (tương ứng $W_X = W_{X'}$) khi và chỉ khi $X \subset X'$ (tương ứng $X = X'$).

Mọi phần tử của $X$ có cấp 2 và $X$ sinh ra $W_X$. Cho $x \in X$ và $w \in W_X$ với $l_X(xw) \leq l_X(w) = q$. Theo Hệ quả 4 của Mệnh đề 7, ta có
$$
l_S(xw) \leq l_S(w) = q.
$$
Cho $x_1, \ldots, x_q$ là các phần tử của $X$ sao cho $w = x_1 \ldots x_q$. Vì $(W, S)$ thỏa mãn điều kiện đổi chỗ (Định lý 1 của no. 6), tồn tại một số nguyên $j$ sao cho $1 \leq j \leq q$ và $xx_1 \ldots x_{j-1} = x_1 \ldots x_{j-1} x_j$. Do đó, $(W_X, X)$ thỏa mãn điều kiện đổi chỗ và vì vậy là một hệ Coxeter (Định lý 1 của no. 6). Điều này chứng minh (i).

Các khẳng định (ii) và (iii) suy ra ngay lập tức từ Hệ quả 1 của Mệnh đề 7.

### 9. MA TRẬN COXETER VÀ ĐỒ THỊ COXETER

#### Định nghĩa 4 {#lie-iv-s1-def-4 .statement}

Cho $I$ là một tập hợp. Một ma trận Coxeter kiểu $I$ là một ma trận vuông đối xứng $M = (m_{ij})_{i,j \in I}$ mà các phần tử của nó là các số nguyên hoặc $+\infty$ thỏa mãn các hệ thức
$$
m_{ii} = 1 \quad \text{cho mọi } i \in I; \tag{25}
$$
$$
m_{ij} \geq 2 \quad \text{với } i, j \in I \text{ với } i \neq j. \tag{26}
$$

Một đồ thị Coxeter kiểu $I$ là (do lạm dụng ngôn ngữ) một cặp gồm một đồ thị $\Gamma^3$ có $I$ làm tập hợp các đỉnh của nó và một ánh xạ $f$ từ tập hợp các cạnh của đồ thị này vào tập hợp gồm $+\infty$ và tập hợp các số nguyên $\geq 3$. $\Gamma$ được gọi là đồ thị nền của đồ thị Coxeter $(\Gamma, f)$.

Một đồ thị Coxeter $(\Gamma, f)$ được liên kết với mọi ma trận Coxeter $M$ kiểu $I$ như sau:

đồ thị $\Gamma$ có tập hợp các đỉnh là $I$ và tập hợp các cạnh là tập hợp các cặp $\{i, j\}$ của các phần tử của $I$ sao cho $m_{ij} \geq 3$, và ánh xạ $f$ gán cho cạnh $\{i, j\}$ phần tử tương ứng $m_{ij}$ của $M$.

Rõ ràng điều này tạo ra một song ánh giữa tập hợp các ma trận Coxeter kiểu $I$ và tập hợp các đồ thị Coxeter kiểu $I$.

Để giúp người đọc theo dõi các lập luận của chúng tôi, chúng tôi thường biểu diễn một đồ thị Coxeter kiểu $I$ bằng biểu đồ dùng để biểu diễn đồ thị nền của nó, và viết bên cạnh hoặc phía trên mỗi cạnh $\{i, j\}$ số $f(\{i, j\})$. Nói chung chúng tôi bỏ qua các số này nếu chúng bằng 3.

3 Xem phụ lục về định nghĩa và các tính chất của các đồ thị được sử dụng ở đây.

Nếu $(W, S)$ là một hệ Coxeter, ma trận $M = (m(s, s'))_{s, s' \in S}$, trong đó $m(s, s')$ là cấp của $ss'$, là một ma trận Coxeter kiểu S được gọi là ma trận Coxeter của $(W, S)$: thật vậy, $m(s, s) = 1$ vì $s^2 = 1$ với mọi $s \in S$, và $m(s, s') = m(s', s) \geqslant 2$ nếu $s \neq s'$ vì khi đó $ss' = (s's)^{-1}$ là $\neq 1$. Đồ thị Coxeter $(\Gamma, f)$ liên kết với M được gọi là đồ thị Coxeter của $(W, S)$. Chúng tôi nhận xét rằng hai đỉnh $s$ và $s'$ của $\Gamma$ được *nối* khi và chỉ khi $s$ và $s'$ không giao hoán. Ví dụ, ma trận Coxeter của một nhóm nhị diện cấp $2m$ là $\begin{pmatrix} 1 & m \\ m & 1 \end{pmatrix}$ và đồ thị Coxeter của nó được biểu diễn bởi

$$
\circ \overset{m}{\text{---}} \circ
$$

khi $m \geqslant 3$ (hoặc

$$
\circ \text{---} \circ
$$

nếu $m = 3$) và bởi

$$
\circ \qquad \circ
$$

khi $m = 2$. \* Đồ thị Coxeter của nhóm đối xứng $\mathfrak{S}_n$ được biểu diễn bởi

$$
\circ \text{---} \circ \text{---} \circ \cdots \circ \text{---} \circ
$$

($n - 1$ đỉnh.) \*

Chúng tôi sẽ chỉ ra sau (Chương V, § 4) rằng, ngược lại, mọi ma trận Coxeter là ma trận của một hệ Coxeter.

Một hệ Coxeter $(W, S)$ được gọi là *bất khả quy* nếu đồ thị nền của đồ thị Coxeter của nó là *liên thông* (Phụ lục, no. 2) và *không rỗng*. Tương đương, S là không rỗng và không tồn tại một phân hoạch của S thành hai tập con phân biệt S' và S'' của S sao cho mọi phần tử của S' giao hoán với mọi phần tử của S''. Nói chung hơn, cho $(\Gamma_i)_{i \in I}$ là họ các thành phần liên thông của $\Gamma$ (Phụ lục, no. 2) và cho $S_i$ là tập hợp các đỉnh của $\Gamma_i$. Cho $W_i = W_{S_i}$ là nhóm con của W sinh bởi $S_i$ (xem no. 8). Khi đó các $(W_i, S_i)$ là các hệ Coxeter bất khả quy (no. 8, Th. 2) được gọi là các *thành phần bất khả quy* của $(W, S)$. Hơn nữa, nhóm W là *tích trực tiếp hạn chế*[^1] của các nhóm con $W_i$ với $i \in I$. Thật vậy, điều này suy ra từ mệnh đề tổng quát hơn sau:

#### Mệnh đề 8 {#lie-iv-s1-prop-8 .statement}

Cho $(S_i)_{i \in I}$ là một phân hoạch của S sao cho mọi phần tử của $S_i$ giao hoán với mọi phần tử của $S_j$ nếu $i \neq j$. Với mọi $i \in I$, cho $W_i$ là nhóm con sinh bởi $S_i$. Khi đó W là tích trực tiếp hạn chế của họ $(W_i)_{i \in I}$.

Hiển nhiên rằng với mọi $i \in I$, nhóm con $W'_i$ sinh bởi hợp của các $W_j$ với $j \neq i$ cũng được sinh bởi $S'_i = \bigcup_{j \neq i} S_j$. Do đó
$$
W_i \cap W'_i = W_\varnothing = \{1\}
$$
theo Định lý 2 của no. 8. Vì W được sinh bởi hợp của các $W_i$, điều này chứng minh mệnh đề.

### Bài tập {#lie-iv-s1-exercises}

Xem [các bài tập của § 1](exercises/s1/).

[^1]: Một nhóm G là *tích trực tiếp hạn chế* của một họ $(G_i)_{i \in I}$ các nhóm con nếu, với mọi tập con hữu hạn J của I, nhóm con $G_J$ của G sinh bởi các $G_i$ với $i \in J$ là tích trực tiếp của các $G_i$ với $i \in J$ và nếu G là hợp của các $G_J$. Tương đương, mọi phần tử của $G_i$ giao hoán với mọi phần tử của $G_j$ với $i \neq j$ và mọi phần tử của G có thể được viết duy nhất dưới dạng một tích $\prod_{i \in I} g_i$ với $g_i \in G_i$ và $g_i = 1$ với tất cả trừ hữu hạn các chỉ số $i$. Điều kiện cuối cùng này tương đương với việc nói rằng G được sinh bởi hợp của các $G_i$ và rằng $G_i \cap G_J = \{1\}$ với mọi $i \in I$ và mọi tập con hữu hạn J sao cho $i \notin J$.
