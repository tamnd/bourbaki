---
book: alg
book_title: Algebra
chapter: II
chapter_title: LINEAR ALGEBRA
section: 7
section_title: Vector spaces
lang: vi
source: alg-i-iii
source_edition: 1998, Springer
pdf_pages: 0316-0340, 0424-0433
extraction: ocr
subsections:
    - "no": 1
      title: BASES OF A VECTOR SPACE
      page: 0
      pdf_page: 316
    - "no": 2
      title: DIMENSION OF VECTOR SPACES
      page: 0
      pdf_page: 317
    - "no": 3
      title: DIMENSION AND CODIMENSION OF A SUBSPACE OF A VECTOR SPACE
      page: 0
      pdf_page: 319
    - "no": 4
      title: RANK OF A LINEAR MAPPING
      page: 0
      pdf_page: 322
    - "no": 5
      title: DUAL OF A VECTOR SPACE
      page: 0
      pdf_page: 323
    - "no": 6
      title: LINEAR EQUATIONS IN VECTOR SPACES
      page: 0
      pdf_page: 328
    - "no": 7
      title: TENSOR PRODUCTS OF VECTOR SPACES
      page: 0
      pdf_page: 330
    - "no": 8
      title: RANK OF AN ELEMENT OF A TENSOR PRODUCT
      page: 0
      pdf_page: 333
    - "no": 9
      title: EXTENSION OF SCALARS FOR A VECTOR SPACE
      page: 0
      pdf_page: 334
    - "no": 10
      title: MODULES OVER INTEGRAL DOMAINS
      page: 0
      pdf_page: 336
statements: 87
exercises: 39
content_sha256: 27e76d1b3f4cab2a438dde6d769bec3f964e3f1065c649ad920ea669e34b5fb5
translated_from: content/en/alg/II/07_s7_vector_spaces.md
source_content_sha256: 4788796aa08009db5601bccc827085a26b1025a9c1c0eac7c83a0824728f68c2
translation_model: gpt-5-6-mini, gpt-5.4, gpt-5-6
translation_run: translate-vi-59713daf
glossary_version: 34
glossary_terms_sha256: b870f51848a51208e81da7ecf1a02edad7b0cf6aabcfac28b12eb5536069cf51
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 7. KHÔNG GIAN VECTƠ

### 1. CƠ SỞ CỦA MỘT KHÔNG GIAN VECTƠ

#### Định lý 1 {#alg-ii-s7-thm-1 .statement}

Mọi không gian vectơ trên một trường K đều là một K-môđun tự do.

Cần chứng minh rằng mọi không gian vectơ đều có một cơ sở; điều này sẽ suy ra từ định lý chính xác hơn sau đây:

#### Định lý 2 {#alg-ii-s7-thm-2 .statement}

Cho một hệ sinh S của một không gian vectơ E trên một trường K và một tập con tự do L của E được chứa trong S, tồn tại một cơ sở B của E sao cho L ⊂ B ⊂ S.

Định lý 1 suy ra từ mệnh đề này bằng cách lấy L = ∅.

Để chứng minh Định lý 2, ta nhận xét rằng tập hợp Λ các tập con tự do của E được chứa trong S, có thứ tự bởi quan hệ bao hàm, là một tập quy nạp (Lý thuyết tập hợp, III, § 2, no. 4), nhờ § 1, no. 11; do đó tập hợp M các tập con tự do chứa L và được chứa trong S cũng vậy. Theo Bổ đề Zorn, M có một phần tử cực đại B và chỉ cần chứng minh rằng không gian con vectơ của E sinh bởi B bằng E. Điều này suy ra ngay lập tức từ định nghĩa của B và bổ đề sau:

#### Bổ đề 1 {#alg-ii-s7-lem-1 .statement}

Cho (a_i)_{i \in I} là một họ tự do các phần tử của E; nếu b \in E không thuộc không gian con F sinh bởi (a_i), tập con của E gồm các a_i và b là tự do.

Giả sử có một quan hệ $\mu b + \sum_i \lambda_i a_i = 0$ với $\mu \in K$ và $\lambda_i \in K$ với mọi $i \in I$, họ $(\lambda_i)$ có giá hữu hạn; nếu $\mu \neq 0$, thì suy ra $b = -\sum_i (\mu^{-1} \lambda_i) a_i$ và do đó $b \in F$, trái với giả thiết; vậy $\mu = 0$ và quan hệ trở thành $\sum_i \lambda_i a_i = 0$, điều này kéo theo $\lambda_i = 0$ với mọi $i \in I$ theo giả thiết; do đó có bổ đề.

#### Hệ quả {#alg-ii-s7-n1-cor-1 .statement}

Đối với một tập con B của một không gian vectơ E, các tính chất sau là tương đương:
(a) B là một cơ sở của E.
(b) B là một tập con tự do cực đại của E.
(c) B là một hệ sinh cực tiểu của E.
Điều này suy ra ngay lập tức từ Định lý 2.

#### Ví dụ {#alg-ii-s7-n1-exa-1 .statement}

Cho một vành A và một trường con K của A, A là một không gian vectơ (phải hoặc trái) trên K và do đó có một cơ sở; đặc biệt, mọi trường mở rộng của một trường K đều có một cơ sở như một không gian vectơ trái (tương ứng phải) trên K.
*Do đó trường R các số thực có một cơ sở (vô hạn) như một không gian vectơ trên trường Q các số hữu tỉ; một cơ sở như vậy của R được gọi là cơ sở Hamel.*

#### Nhận xét {#alg-ii-s7-n1-rem-1 .statement}

Đối với một họ $(a_i)_{i \in I}$ các phần tử của một không gian vectơ $E$ trên một trường $K$ là *tự do*, điều kiện cần và đủ là, với mọi $\kappa \in I$, $a_\kappa$ không thuộc bất kỳ không gian con nào của $E$ sinh bởi các $a_i$ có chỉ số $i \neq \kappa$. Ta biết rằng điều kiện này là cần thiết trong mọi môđun (§ 1, no. 11, *Nhận xét* 1). Nó là đủ nhờ Bổ đề 1, như thấy ngay lập tức bằng cách lập luận theo *reductio ad absurdum* và xét một họ con liên quan cực tiểu của $(a_i)$.

### 2. CHIỀU CỦA CÁC KHÔNG GIAN VECTƠ

#### Định lý 3 {#alg-ii-s7-thm-3 .statement}

*Hai cơ sở của cùng một không gian vectơ* $E$ *trên một trường* $K$ *có cùng lực lượng*.

Trước hết ta nhận xét rằng nếu $E$ có một cơ sở *vô hạn* $B$, thì suy ra từ § 1, no. 12, Hệ quả 2 của Mệnh đề 23 rằng mọi cơ sở khác của $E$ đều có cùng lực lượng với $B$. Vì vậy ta có thể chỉ xét trường hợp $E$ có một cơ sở hữu hạn gồm $n$ phần tử. Ta nhận xét rằng mọi không gian vectơ *đơn sinh* trên $K$, khác 0, là một $K$-môđun *đơn* (I, § 4, no. 4, Định nghĩa 7), vì nó được sinh bởi mỗi phần tử của nó $\neq 0$, nhờ quan hệ $\mu a = (\mu \lambda)(\lambda^{-1}a)$ với $\mu \in K$, $\lambda \in K$ và $\lambda \neq 0$. Do đó nếu $(a_i)_{1 \leq i \leq n}$ là một cơ sở của $E$, thì $E = \bigoplus_{i=1}^n Ka_i$ đến đẳng cấu và các không gian con $E_k = \bigoplus_{i=1}^\kappa Ka_i$ với $0 \leq k \leq n$ tạo thành một *chuỗi Jordan-Hölder* của $E$, $E_k/E_{k-1}$ đẳng cấu với $Ka_k$. Định lý 3 khi đó suy ra trong trường hợp này từ Định lý Jordan-Hölder (I, § 4, no. 7, Định lý 6).

Có thể cho một chứng minh độc lập với Định lý Jordan-Hölder, bằng cách chứng minh bằng quy nạp theo $n$ rằng, nếu $E$ thừa nhận một cơ sở gồm $n$ phần tử, thì mọi cơ sở khác $B'$ đều có *nhiều nhất* $n$ phần tử. Mệnh đề là hiển nhiên đối với $n = 0$. Nếu $n \geq 1$, thì $B'$ khác rỗng; khi đó lấy $a \in B'$. Theo Định lý 2 (no. 1), tồn tại một tập con $C$ của $B$ sao cho $\{a\} \cup C$ là một cơ sở của $E$ và $a \notin C$, vì $\{a\} \cup B$ hiển nhiên là một hệ sinh của $E$. Vì $B$ là một cơ sở của $E$, nên $C = B$ là không thể xảy ra (no. 1, Hệ quả của Định lý 2), và do đó $C$ có nhiều nhất $n - 1$ phần tử. Gọi $V$ là không gian con sinh bởi $C$ và $V'$ là không gian con sinh bởi $B' - \{a\}$; $V$ và $V'$ đều là các phần bù của không gian con $Ka$ trong $E$ và do đó đẳng cấu (§ 1, no. 10, Mệnh đề 13). Vì $V$ thừa nhận một cơ sở có nhiều nhất $n - 1$ phần tử, nên theo giả thiết quy nạp, $B' - \{a\}$ có nhiều nhất $n - 1$ phần tử, và do đó $B'$ có nhiều nhất $n$ phần tử.

#### Định nghĩa 1 {#alg-ii-s7-def-1 .statement}

***Chiều của một không gian vectơ*** $E$ *trên một trường* $K$, *ký hiệu là* $\dim_K E$ *hoặc* $[E:K]$ (*hoặc đơn giản là* $\dim E$) *là lực lượng của bất kỳ cơ sở nào của* $E$. *Nếu* $M$ *là một tập con của* $E$, *thì hạng của* $M$ *(trên* $K$*), ký hiệu là* $\operatorname{rg} M$ *hoặc* $\operatorname{rg}_K M$, *là chiều của không gian vectơ con của* $E$ *được sinh bởi* $M$.

Nói rằng $E$ là hữu hạn chiều tương đương với việc nói rằng $E$ là một $K$-môđun có *độ dài hữu hạn* và $\dim_K E = \operatorname{long}_K E$.

#### Hệ quả {#alg-ii-s7-n2-cor-1 .statement}

*Với mọi tập con M của E, hạng của M nhiều nhất bằng dim E.*

Nếu V là không gian vectơ con của E được sinh bởi M, thì M chứa một cơ sở B' của V (no. 1, Định lý 2) và vì B' là một tập con tự do của E, nên nó được chứa trong một cơ sở B của E (no. 1, Định lý 2); khi đó Card(B') $\leq$ Card(B), do đó có hệ quả.

Các Định lý 2 và 3 ngay lập tức suy ra mệnh đề sau:

#### Mệnh đề 1 {#alg-ii-s7-prop-1 .statement}

(i) *Để một không gian vectơ trái trên K có số chiều hữu hạn n, điều kiện cần và đủ là nó đẳng cấu với K_s^n.*

(ii) *Để hai không gian vectơ K_s^m và K_s^n đẳng cấu (m và n là các số nguyên $\geq 0$), điều kiện cần và đủ là m = n.*

(iii) *Trong một không gian vectơ E có số chiều hữu hạn n, mọi hệ sinh đều có ít nhất n phần tử; một hệ sinh của E có n phần tử là một cơ sở của E.*

(iv) *Trong một không gian vectơ E có số chiều hữu hạn n, mọi tập con tự do đều có nhiều nhất n phần tử; một tập con tự do có n phần tử là một cơ sở của E.*

#### Mệnh đề 2 {#alg-ii-s7-prop-2 .statement}

*Cho (E_t)_{t \in I} là một họ các không gian vectơ trên K. Khi đó*

$$
\dim_K \left( \bigoplus_{t \in I} E_t \right) = \sum_{t \in I} \dim_K E_t.
$$

Nếu các E_t được đồng nhất một cách chính tắc với các không gian con của $E = \bigoplus_{t \in I} E_t$ và B_t là một cơ sở của E_t ($t \in I$), thì $B = \bigcup_{t \in I} B_t$ là một cơ sở của E ($§ 1$, no. 11, Proposition 19); do đó có quan hệ (1) vì các B_t từng đôi một rời nhau.

#### Nhận xét {#alg-ii-s7-n2-rem-1 .statement}

(1) Có thể cho các ví dụ về những môđun thừa nhận hai cơ sở hữu hạn không có cùng số phần tử ($§ 1$, Bài tập 16(c)). Tuy nhiên:

#### Mệnh đề 3 {#alg-ii-s7-prop-3 .statement}

*Một vành A được giả sử sao cho tồn tại một đồng cấu $\rho$ từ A vào một trường D; khi đó với mọi A-môđun tự do E, hai cơ sở bất kỳ của E đều có cùng lực lượng.*

Xét không gian vectơ $\rho^*(E) = D \otimes_A E$ trên D thu được bằng cách mở rộng vành vô hướng lên D ($§ 5$, no. 1) và gọi $\phi : x \mapsto 1 \otimes x$ là ánh xạ chính tắc từ E vào $\rho^*(E)$; nếu $(a_\lambda)$ là một cơ sở của E thì $(\phi(a_\lambda))$ là một cơ sở của $\rho^*(E)$ ($§ 5$, no. 1, Mệnh đề 4); khi đó mệnh đề suy ra từ Định lý 3.

#### Hệ quả {#alg-ii-s7-n2-cor-2 .statement}

*Nếu A là một vành giao hoán $\neq 0$ và E là một A-môđun tự do, thì hai cơ sở bất kỳ của E đều có cùng lực lượng.*

Trong A tồn tại ít nhất một iđêan cực đại m (I, $§ 8$, no. 6, Định lý 1) và, vì A/m là một trường, các điều kiện của Mệnh đề 3 được thỏa mãn.

#### Nhận xét {#alg-ii-s7-n2-rem-2 .statement}

(2) Khi một A-môđun tự do E có tính chất là hai cơ sở bất kỳ của E đều có cùng lực lượng, thì lực lượng của một cơ sở tùy ý của E trên A cũng được gọi là *chiều* hoặc *hạng* của E và được ký hiệu bởi $\dim_A E$ hoặc $\dim E$.

(3) Gọi $A$ là một vành sao cho hai cơ sở bất kỳ của một $A$-môđun tự do đều có cùng lực lượng và gọi $K$ là một trường con của $A$, để rồi $A$ có thể được xem như một *không gian vectơ trái* trên $K$ bằng cách hạn chế các vô hướng. Tương tự, mọi $A$-môđun tự do $E$ đều có thể được xem như một không gian vectơ trái trên $K$ và khi đó từ § 1, no. 13, Mệnh đề 25 suy ra rằng

$$
\dim_K E = \dim_K E \cdot \dim_K A_s.
$$

(4) Trong Chương VIII, ta sẽ thấy các ví dụ về những vành thỏa mãn kết luận của Mệnh đề 3 nhưng không thỏa mãn giả thiết.

### 3. CHIỀU VÀ ĐỐI CHIỀU CỦA MỘT KHÔNG GIAN CON CỦA MỘT KHÔNG GIAN VECTƠ

#### Mệnh đề 4 {#alg-ii-s7-prop-4 .statement}

*Mọi không gian con $F$ của một không gian vectơ $E$ đều là một nhân tử trực tiếp của $E$ và*

$$
\dim F + \dim(E/F) = \dim E.
$$

Vì không gian vectơ thương $E/F$ là một môđun tự do, nên ta biết (§ 1, no. 11, Mệnh đề 21) rằng $F$ là một nhân tử trực tiếp của $E$; khi đó quan hệ (3) là một trường hợp riêng của công thức (1) (no. 2).

#### Hệ quả 1 {#alg-ii-s7-prop-4-cor-1 .statement}

*Nếu $E, F, G$ là các không gian vectơ trên một trường $K$, thì mọi dãy khớp các ánh xạ tuyến tính $0 \to E \to F \to G \to 0$ đều tách được.*

Đây là một cách khác để phát biểu Mệnh đề 4 (§ 1, no. 9).

#### Hệ quả 2 {#alg-ii-s7-prop-4-cor-2 .statement}

*Gọi $(E_i)_{0 \leq i \leq n}$ là một họ hữu hạn các không gian vectơ trên một trường $K$. Nếu tồn tại một dãy khớp các ánh xạ tuyến tính*

$$
0 \longrightarrow E_0 \xrightarrow{u_0} E_1 \xrightarrow{u_1} E_2 \longrightarrow \cdots \longrightarrow E_{n-1} \xrightarrow{u_{n-1}} E_n \xrightarrow{u_n} 0
$$

*thì quan hệ*

$$
\sum_{2k+1 \leq n} \dim E_{2k+1} = \sum_{2k \leq n} \dim E_{2k}
$$

*đúng, hoặc, nếu mọi không gian đều hữu hạn chiều, thì*

$$
\sum_{i=1}^n (-i)^i \dim E_i = 0.
$$

Đặt $I_k = \operatorname{Im}\ u_k = \operatorname{Ker}\ u_{k+1}$ với $0 \leq k \leq n-1$; do đó $I_{k+1}$ đẳng cấu với $E_{k+1}/I_k$, nên (công thức (3)) $\dim I_k + \dim I_{k+1} = \dim E_{k+1}$ với $0 \leq k \leq n-2$ và hơn nữa $\dim I_0 = \dim E_0$ và $I_{n-1} = E_n$, do đó $\dim I_{n-1} = \dim E_n$. Thay thế $\dim E_i$ bằng biểu thức của nó như một hàm của các $\dim I_k$ trong hai vế của (5), ta thu được ở mỗi vế $\sum_{k=0}^{n-1} \dim I_k$, do đó có hệ quả.

#### Hệ quả 3 {#alg-ii-s7-prop-4-cor-3 .statement}

*Nếu M và N là hai không gian con của một không gian vectơ E, thì*

(7) $$
\dim(M + N) + \dim(M \cap N) = \dim M + \dim N.
$$

Chỉ cần áp dụng Hệ quả 2 cho dãy khớp

$$ 0 \to M \cap N \to M \oplus N \to M + N \to 0 $$

(§ 1, no. 8, Mệnh đề 10) đồng thời lưu ý rằng

$$
\dim(M \oplus N) = \dim M + \dim N
$$

(no. 2, Mệnh đề 2).

#### Hệ quả 4 {#alg-ii-s7-prop-4-cor-4 .statement}

*Với mọi không gian con F của một không gian vectơ E, $\dim F \leq \dim E$; nếu E hữu hạn chiều, thì quan hệ $\dim F = \dim E$ tương đương với $F = E$.*

Mệnh đề thứ nhất là hiển nhiên từ (3); hơn nữa, nếu $\dim E$ là hữu hạn, thì quan hệ $\dim F = \dim E$ kéo theo $\dim(E/F) = 0$ theo (3), và một không gian vectơ có chiều bằng 0 thì thu về 0.

#### Hệ quả 5 {#alg-ii-s7-prop-4-cor-5 .statement}

*Nếu một không gian vectơ E là tổng của một họ $(F_i)$ các không gian con vectơ, thì*

(8) $$
\dim E \leq \sum_i \dim F_i.
$$

*Nếu thêm $\dim E$ là hữu hạn, hai vế của (8) bằng nhau khi và chỉ khi E là tổng trực tiếp của họ $(F_i)$.*

Bất đẳng thức (8) suy ra từ (3) và sự kiện rằng E đẳng cấu với một thương của $\bigoplus_i F_i$ (§ 1, no. 7, công thức (28)). Mệnh đề thứ hai là một trường hợp riêng của § 1, no. 10, Hệ quả 5 của Mệnh đề 16, vì sự bằng nhau của hai vế của (8) kéo theo rằng $\dim F_i = 0$ ngoại trừ một số hữu hạn chỉ số.

#### Định nghĩa 2 {#alg-ii-s7-def-2 .statement}

*Một không gian vectơ E đã cho, đối chiều (đối với E) của một không gian con F của E, ký hiệu bởi $\operatorname{codim}_E F$, hoặc đơn giản là $\operatorname{codim} F$, là chiều của $E/F$ (bằng chiều của mọi phần bù của F trong E).*

Khi đó quan hệ (3) có thể được viết

(9) $$
\dim F + \operatorname{codim} F = \dim E.
$$

#### Mệnh đề 5 {#alg-ii-s7-prop-5 .statement}

*Cho F, F' là hai không gian con của một không gian vectơ E, sao cho $F \subset F'$. Khi đó $\operatorname{codim}_E F' \leq \operatorname{codim}_E F \leq \dim E$. Nếu $\operatorname{codim}_E F$ là hữu hạn, quan hệ $\operatorname{codim}_E F' = \operatorname{codim}_E F$ kéo theo $F = F'$.*

Bất đẳng thức $\operatorname{codim}_E F \leq \dim E$ là hiển nhiên từ (9) và nếu $\dim E$ là hữu hạn thì quan hệ $\operatorname{codim}_E F = \dim E$ kéo theo $\dim F = 0$ và do đó $F = \{0\}$. Phần còn lại của mệnh đề suy ra từ điều này, vì
$$
\operatorname{codim}_E F' = \operatorname{codim}_{E/F'}(F'/F),
$$
do $E/F'$ đẳng cấu chính tắc với $(E/F)/(F'/F)$ (I, § 4, no. 7, Định lý 4).

#### Mệnh đề 6 {#alg-ii-s7-prop-6 .statement}

*Nếu M và N là hai không gian con của một không gian vectơ E, thì*
$$
\operatorname{codim}(M + N) + \operatorname{codim}(M \cap N) = \operatorname{codim} M + \operatorname{codim} N.
$$
(10)
Chỉ cần áp dụng Hệ quả 2 của Mệnh đề 4 vào dãy khớp
$$
0 \to E/(M \cap N) \to (E/M) \oplus (E/N) \to E/(M + N) \to 0
$$
(§ 1, no. 7, Mệnh đề 10) và sử dụng no. 2, Mệnh đề 2.

Chú ý rằng nếu E là hữu hạn chiều, (10) là một hệ quả của (7) và (9).

#### Mệnh đề 7 {#alg-ii-s7-prop-7 .statement}

*Nếu $(F_i)$ là một họ hữu hạn các không gian con của một không gian vectơ E, thì*
$$
\operatorname{codim}\left(\bigcap_i F_i\right) \leq \sum_i \operatorname{codim} F_i.
$$
Nếu $F = \bigcap_i F_i$, $E/F$ đẳng cấu với một không gian con của tổng trực tiếp của các $E/F_i$ (§ 1, no. 7, công thức (27)).

Các không gian con vectơ có chiều 1 (tương ứng, chiều 2) của một không gian vectơ E thường được gọi là *các đường thẳng đi qua 0* (tương ứng, *các mặt phẳng đi qua 0*) (hoặc đơn giản là *các đường thẳng* (tương ứng, *các mặt phẳng*) nếu không có sự nhầm lẫn nào xảy ra (xem § 9, no. 3)), theo phép tương tự với ngôn ngữ của Hình học cổ điển; một không gian con của E được gọi là một *siêu phẳng đi qua 0* (hoặc đơn giản là một *siêu phẳng*) nếu nó có đối chiều 1. Các siêu phẳng cũng có thể được định nghĩa là các phần tử *cực đại* của tập hợp $\mathcal{S}$ các không gian con vectơ của E *phân biệt* với E, có thứ tự bởi quan hệ bao hàm. Có một sự tương ứng một-một giữa các không gian con của E chứa một không gian con H và các không gian con của $E/H$ (I, § 4, no. 7, Định lý 4); nếu E có chiều $\geq 1$, $\mathcal{S}$ không rỗng và nói rằng H là cực đại trong $\mathcal{S}$ có nghĩa là $E/H$ không chứa không gian con nào phân biệt với $\{0\}$ và $E/H$, điều này kéo theo rằng $E/H$ được sinh bởi mọi phần tử của nó $\neq 0$, nói cách khác nó có chiều 1.

Trong một không gian vectơ có số chiều hữu hạn $n \geq 1$, các siêu phẳng là các không gian con *có chiều* $n - 1$ theo công thức (3).

#### Mệnh đề 8 {#alg-ii-s7-prop-8 .statement}

*Trong một không gian vectơ E trên một trường K, mọi không gian con vectơ F là giao của các siêu phẳng chứa nó.*

Chỉ cần chứng minh rằng với mọi $x \notin F$ tồn tại một siêu phẳng H chứa F và không chứa x. Theo giả thiết $F \cap Kx = \{0\}$ và do đó tổng M của F và $Kx$ là trực tiếp. Gọi N là phần bù của M trong E; khi đó E là tổng trực tiếp của $H = F + N$ và $Kx$ và vì vậy H là một siêu phẳng có tính chất mong muốn.

#### Nhận xét {#alg-ii-s7-n3-rem-1 .statement}

Phần lớn các tính chất đã được chứng minh trong no. này cho các không gian con của một không gian vectơ không đúng đối với các môđun con của một môđun tự do mà số chiều của nó ($§ 2,$ no. 7, Nhận xét 2) được định nghĩa. *Ví dụ, một iđêan của một vành giao hoán không nhất thiết có cơ sở, vì có những miền nguyên $A$ trong đó một số iđêan không chính (VII, $§ 1,$ no. 1) và hai phần tử bất kỳ của một vành như vậy phụ thuộc tuyến tính ($§ 1,$ no. 11, Nhận xét 1).* Một môđun con của một môđun tự do $A$-môđun $E$ có thể là tự do, phân biệt với $E$ và có cùng số chiều với $E$, như được chỉ ra bởi các iđêan chính trong một miền nguyên $A$; cùng ví dụ còn chứng minh thêm rằng một môđun con tự do của một $A$-môđun tự do không nhất thiết có một phần bù.

### 4. HẠNG CỦA MỘT ÁNH XẠ TUYẾN TÍNH

#### Định nghĩa 3 {#alg-ii-s7-def-3 .statement}

*Cho $E, F$ là hai không gian vectơ trên một trường $K$. Đối với mọi ánh xạ tuyến tính $u$ của $E$ vào $F$, chiều của không gian con $u(E)$ của $F$ được gọi là hạng của $u$ và ký hiệu là $\mathrm{rg}(u)$.

Nếu $N = \mathrm{Ker}(u)$, $E/N$ đẳng cấu với $u(E)$, do đó có quan hệ
$$
\mathrm{rg}(u) = \mathrm{codim}_E(\mathrm{Ker}(u))
$$
và vì vậy
$$
\mathrm{rg}(u) + \dim(\mathrm{Ker}(u)) = \dim E.
$$
Hơn nữa, theo công thức (3)
$$
\mathrm{rg}(u) + \dim(\mathrm{Coker}(u)) = \dim F.
$$

#### Mệnh đề 9 {#alg-ii-s7-prop-9 .statement}

*Cho $E, F$ là hai không gian vectơ trên một trường $K$ và $u : E \to F$ là một ánh xạ tuyến tính.*
(i) $\mathrm{rg}(u) \leq \inf(\dim E, \dim F)$.
(ii) *Giả sử rằng $E$ là hữu hạn chiều; để có $\mathrm{rg}(u) = \dim E$, điều kiện cần và đủ là $u$ đơn ánh.*
(iii) *Giả sử rằng $F$ là hữu hạn chiều; để có $\mathrm{rg}(u) = \dim F$, điều kiện cần và đủ là $u$ toàn ánh.*

Điều này suy ra ngay lập tức từ các quan hệ (12) và (13).

#### Hệ quả {#alg-ii-s7-n4-cor-1 .statement}

*Cho $E$ là một không gian vectơ có số chiều hữu hạn $n$ và $u$ là một tự đồng cấu của $E$. Các tính chất sau là tương đương:*
(a) $u$ là song ánh;
(b) $u$ là đơn ánh;
(c) $u$ là toàn ánh;
(d) $u$ là khả nghịch phải;
(e) $u$ là khả nghịch trái;
(f) $u$ có hạng $n$.

Nếu E là một không gian vectơ vô hạn chiều, tồn tại các tự đồng cấu đơn ánh (tương ứng toàn ánh) của E không song ánh (Bài tập 9).

Cho K, K' là hai trường, $\sigma : K \to K'$ là một *đẳng cấu* của K lên K', E là một không gian vectơ K, E' là một không gian vectơ K' và $u : K \to K'$ là một ánh xạ *nửa tuyến tính* đối với $\sigma$ (§ 1, no. 13); chiều của không gian con $u(E)$ của E' cũng được gọi là *hạng* của $u$. Nó cũng là hạng của $u$ được xem như một ánh xạ tuyến tính của E vào $\sigma_*(E')$, vì mọi cơ sở của $u(E)$ cũng là một cơ sở của $\sigma_*(u(E))$.

### 5. ĐỐI NGẪU CỦA MỘT KHÔNG GIAN VECTƠ

#### Định lý 4 {#alg-ii-s7-thm-4 .statement}

*Chiều của đối ngẫu* $E^*$ *của một không gian vectơ* E *ít nhất bằng chiều của* E. *Để* $E^*$ *hữu hạn chiều, điều kiện cần và đủ là* E *hữu hạn chiều, và khi đó* $\dim E^* = \dim E$.

Nếu K là trường các vô hướng của E, E đẳng cấu với một không gian $K_s^{(I)}$ và do đó $E^*$ đẳng cấu với $K_d^I$ (§ 2, no. 6, Mệnh đề 10). Vì $K_s^{(I)}$ là một không gian con của $K_d^I$, $\dim E = \mathrm{Card}(I) \leq \dim E^*$ (no. 3, Hệ quả 4 của Mệnh đề 4); hơn nữa, nếu I hữu hạn, $K_d^I = K_d^{(I)}$ (xem Bài tập 3(d)).

#### Hệ quả {#alg-ii-s7-n5-cor-1 .statement}

*Đối với một không gian vectơ* E, *các quan hệ* $E = \{0\}$ *và* $E^* = \{0\}$ *là tương đương*.

#### Định lý 5 {#alg-ii-s7-thm-5 .statement}

*Cho hai dãy khớp của các không gian vectơ (trên cùng một trường* K*) và các ánh xạ tuyến tính*
$$
\begin{align*}
0 &\to E' \to E \to E'' \to 0 \\
0 &\to F' \to F \to F'' \to 0
\end{align*}
$$
*và hai không gian vectơ* G, H *trên* K, *các dãy tương ứng*
$$
\begin{align*}
0 &\to \mathrm{Hom}(E'', G) \to \mathrm{Hom}(E, G) \to \mathrm{Hom}(E', G) \to 0 \\
0 &\to \mathrm{Hom}(H, F') \to \mathrm{Hom}(H, F) \to \mathrm{Hom}(H, F'') \to 0
\end{align*}
$$
*là khớp và tách*.

Điều này suy ra từ sự kiện rằng mọi không gian con vectơ là một nhân tử trực tiếp (no. 3, Mệnh đề 4) và từ § 2, no. 1, các Mệnh đề 1 và 2.

#### Hệ quả {#alg-ii-s7-n5-cor-2 .statement}

*Với mọi dãy khớp*
$$
0 \longrightarrow E' \xrightarrow{u} E \xrightarrow{v} E'' \longrightarrow 0
$$
*của các không gian vectơ trên cùng một trường* K *và các ánh xạ tuyến tính, dãy*
$$
0 \longrightarrow E''* \xrightarrow{t_v} E^* \xrightarrow{t_u} {E'}^* \longrightarrow 0
$$
*là khớp và phân rã*.

Đặc biệt suy ra rằng với mọi không gian con vectơ M của E, đồng cấu chính tắc $E^*/M' \to M^*$, trong đó $M'$ là không gian con của $E^*$ trực giao với M (§ 2, no. 4), là *song ánh*.

#### Định lý 6 {#alg-ii-s7-thm-6 .statement}

*Với mọi không gian vectơ E trên một trường K, ánh xạ chính tắc $c_E : E \to E^{**}$ (§ 2, no. 7) là đơn ánh; để nó là song ánh, điều kiện cần và đủ là E hữu hạn chiều.*

Mệnh đề thứ nhất và việc $c_E$ là song ánh khi E hữu hạn chiều là những trường hợp riêng của § 2, no. 7, Mệnh đề 14. Giả sử E vô hạn chiều, nên ta có thể giả thiết rằng $E = K_s^{(L)}$, trong đó L là một tập vô hạn và do đó $E^* = K_d^L$. Gọi $(e_\lambda)_{\lambda \in L}$ là cơ sở chính tắc của E và $(e_\lambda^*)_{\lambda \in L}$ là họ tương ứng các dạng tọa độ trong $E^*$ (§ 2, no. 6); không gian con vectơ của $E^*$ sinh bởi các $e_\lambda^*$ chính là tổng trực tiếp $F' = K_d^{(L)}$ và giả thiết L vô hạn kéo theo $F' \neq E^*$. Khi đó tồn tại một siêu phẳng $H'$ của $E^*$ chứa $F'$ (no. 3, Mệnh đề 8) và, vì $E^*/H'$ khác không, đối ngẫu của nó նույնպես cũng khác không (Hệ quả của Định lý 4), đối ngẫu này được đồng nhất với phần trực giao $H''$ của $H'$ trong $E^{**}$ (§ 2, no. 6, Hệ quả của Mệnh đề 9). Nhưng $H'' \cap c_E(E)$ được chứa trong ảnh qua $c_E$ của phần trực giao của $F'$ trong E, mà theo định nghĩa là 0; do đó $c_E(E) = E^{**}$ là điều không thể.

Thông thường E sẽ được *đồng nhất* với không gian con của $E^{**}$ là ảnh của $c_E$.

Cho E, F là hai không gian vectơ trên một trường K và $u : E \to F$ là một ánh xạ tuyến tính. Ta sẽ định nghĩa các *đẳng cấu chính tắc*:

(1) *Từ đối ngẫu của Im(u) = u(E) lên Im($^t u$) = $^t u(F^*)$.*

(2) *Từ đối ngẫu của Ker(u) = $^{-1}u(0)$ lên Coker($^t u$) = $E^*/^t u(F^*)$.*

(3) *Từ đối ngẫu của Coker(u) = F/u(E) lên Ker($^t u$) = $^t u^{-1}(0)$.*

Ta viết I = Im(u), N = Ker(u), C = Coker(u); từ các dãy khớp

(14) $0 \to N \to E \xrightarrow{p} I \to 0,\quad 0 \to I \xrightarrow{j} F \to C \to 0$

ta suy ra, bằng phép chuyển vị (Hệ quả của Định lý 5), các dãy khớp

(15)
$$
\begin{array}{ccccccccc}
0 & \to & I^* & \xrightarrow{^t p} & E^* & \to & N^* & \to & 0, \\
0 & \to & C^* & \to & F^* & \xrightarrow{^t j} & I^* & \to & 0.
\end{array}
$$

Hơn nữa, vì $u = j \circ p,\ ^t u = ^t p \circ ^t j$; do đó các dãy khớp (15) xác định các đẳng cấu chính tắc từ $C^*$ lên Ker($^t u$), từ $I^*$ lên Im($^t u$) và từ $N^*$ lên Coker($^t u$), vì $^t p$ là đơn ánh và $^t j$ là toàn ánh. Nói chính xác hơn, gọi $y \in \mathrm{Im}(u)$, $z \in \mathrm{Ker}(u)$, $t \in \mathrm{Coker}(u)$, $y' \subset \mathrm{Im}(^t u)$, $z' \in \mathrm{Coker}(^t u)$, $t' \in \mathrm{Ker}(^t u)$; khi $y'$, $z'$, $t'$ được đồng nhất một cách chính tắc với các dạng tuyến tính trên $\mathrm{Im}(u)$, $\mathrm{Ker}(u)$ và $\mathrm{Coker}(u)$ tương ứng, thì

(16) $\langle y, y' \rangle = \langle x, y' \rangle$ với mọi $x \in E$ sao cho $u(x) = y$;

(17) $\langle z, z' \rangle = \langle z, x^* \rangle$ với mọi $x^* \in E^*$ mà lớp mod. $^t u(F)$ bằng $z'$;

(18) $\langle t, t' \rangle = \langle s, t' \rangle$ với mọi $s \in F$ mà lớp mod. $u(E)$ bằng $t$.

Đặc biệt, từ các kết quả này ta suy ra:

#### Mệnh đề 10 {#alg-ii-s7-prop-10 .statement}

*Cho E, F là hai không gian vectơ trên cùng một trường K và u : E \to F là một ánh xạ tuyến tính.*

(i) *Để u là đơn ánh (tương ứng, toàn ánh), điều kiện cần và đủ là $^t u$ toàn ánh (tương ứng, đơn ánh).*

(ii) $\operatorname{rg}(u) \leq \operatorname{rg}(^t u)$ và $\operatorname{rg}(u) = \operatorname{rg}(^t u)$ nếu $\operatorname{rg}(u)$ hữu hạn.

Mệnh đề thứ hai suy ra từ trên và Định lý 4.

#### Định lý 7 {#alg-ii-s7-thm-7 .statement}

*Cho E là một không gian vectơ trên một trường K, F là một không gian con của E và F' là phần trực giao của F trong E*.*

(i) $\dim F' \geq \operatorname{codim}_E F;$ để $\dim F'$ là hữu hạn, điều kiện cần và đủ là $\operatorname{codim}_E F$ hữu hạn, và khi đó $\dim F' = \operatorname{codim}_E F$.

(ii) *Phần trực giao của F' trong E bằng F.*

(iii) *Mọi không gian con hữu hạn chiều G' của E* là phần trực giao của một không gian con nào đó của E, tất yếu bằng phần trực giao của G' trong E và có đối chiều hữu hạn.*

(i) Ta biết rằng F' đẳng cấu với đối ngẫu $(E/F)^*$ (§ 2, no. 6, Hệ quả của Mệnh đề 9) và do đó mệnh đề suy ra từ Định lý 4, vì $\dim(E/F) = \operatorname{codim}_E F$ theo định nghĩa.

(ii) Gọi $F_1$ là phần trực giao của F' trong E; rõ ràng $F \subset F_1$ và phần trực giao $F'_1$ của $F_1$ bằng F' (§ 2, no. 4); do đó ánh xạ tuyến tính chính tắc $(E/F_1)^* \to (E/F)^*$, chuyển vị của $E/F \to E/F_1$ là song ánh (§ 2, no. 6, Hệ quả của Mệnh đề 10); khi đó từ Mệnh đề 10 suy ra rằng ánh xạ chính tắc $E/F \to E/F_1$ là song ánh, điều này kéo theo $F_1 = F$.

(iii) Cho G' là một không gian con của E* có số chiều hữu hạn $p$ và gọi F là phần trực giao của nó trong E; khi đó $\operatorname{codim}_E F \leq \dim G'$. Thật vậy, nếu $(a_i^*)_{1 \leq i \leq p}$ là một cơ sở của G', thì F là hạt nhân của ánh xạ tuyến tính $x \mapsto (\langle x, a_i^* \rangle)$ từ E đến $K_s^p$ có hạng nhiều nhất là $p$ (no. 4, Mệnh đề 9), do đó kết luận được suy ra (no. 4). Bây giờ gọi F' là phần trực giao của F trong E*; từ (i) suy ra $\dim F' \leq \dim G'$; nhưng mặt khác hiển nhiên $G' \subset F'$, do đó $F' = G'$ (§ 2, no. 3, Hệ quả 4 của Mệnh đề 4).

#### Nhận xét {#alg-ii-s7-n5-rem-1 .statement}

Một không gian con vô hạn chiều G' của E* không nhất thiết là phần trực giao của một không gian con của E, nói cách khác, nếu F là phần trực giao của G' trong E, thì phần trực giao F' của F trong E* có thể phân biệt với G' (Bài tập 20(b)).†

† Bằng cách trang bị cho E và E* những tôpô thích hợp và chỉ xét trong E và E* các không gian con đóng đối với các tôpô đó, có thể tái lập một đối xứng hoàn hảo giữa các tính chất của E và E* khi E vô hạn chiều (xem Không gian vectơ tôpô, II, § 6).

#### Hệ quả 1 {#alg-ii-s7-thm-7-cor-1 .statement}

Cho $(x_i^*)_{1 \leq i \leq p}$ là một dãy hữu hạn các dạng tuyến tính trên E và gọi F là không gian con của E gồm các x sao cho

$$
\langle x, x_i^* \rangle = 0 \quad \text{với } 1 \leq i \leq p.
$$

Khi đó $\operatorname{codim}_E F$ bằng hạng của tập hợp các $x_i^*$ và mọi dạng tuyến tính trên E triệt tiêu trên F đều là một tổ hợp tuyến tính của các $x_i^*$. Vậy $\operatorname{codim}_E F \leq p$ và để $\operatorname{codim}_E F = p$, điều kiện cần và đủ là các $x_i^*$ độc lập tuyến tính.

Tập hợp $G'$ các tổ hợp tuyến tính của các $x_i^*$ là một không gian con của $E^*$ và F là phần trực giao của $G'$ trong E, do đó $\operatorname{codim}_E F = \dim G'$ theo Định lý 7; hơn nữa $\dim G' \leq p$ và hệ thức $\dim G' = p$ có nghĩa là $(x_i^*)$ là một hệ tự do (no. 2, Mệnh đề 1); do đó có hệ quả.

#### Hệ quả 2 {#alg-ii-s7-thm-7-cor-2 .statement}

(i) *Cho* $(x_i^*)_{1 \leq i \leq p}$ *là một dãy hữu hạn các dạng tuyến tính trên* E. *Để* $(x_i^*)$ *là một hệ tự do, điều kiện cần và đủ là tồn tại một dãy* $(x_i)_{1 \leq i \leq p}$ *các phần tử của* E *sao cho* $\langle x_i, x_j^* \rangle = \delta_{ij}$ *(chỉ số Kronecker)*.

(ii) *Cho* $(x_i)_{1 \leq i \leq p}$ *là một dãy hữu hạn các phần tử của* E. *Để* $(x_i)$ *là một hệ tự do, điều kiện cần và đủ là tồn tại một dãy* $(x_i^*)_{1 \leq i \leq p}$ *các dạng tuyến tính trên* E *sao cho* $\langle x_i, x_j^* \rangle = \delta_{ij}$.

Rõ ràng (ii) suy ra từ (i) khi xét E được đồng nhất với một không gian con của $E^{**}$ nhờ $c_E$ (Định lý 6). Gọi $G'$ là không gian con của $E^*$ sinh bởi các $x_i^*$ và F là trực giao của nó trong E; E/F và $G'$ mỗi cái đều có thể được đồng nhất một cách chính tắc với đối ngẫu của cái kia; nếu họ $(x_i^*)$ là tự do, thì tồn tại trong E/F một cơ sở $(\dot{x}_i)$ đối ngẫu của $(x_i^*)$ và mọi hệ đại diện $(x_i)$ của các lớp $\dot{x}_i$ đều có các tính chất cần có. Ngược lại, sự tồn tại của hệ $(x_i)$ sao cho $\langle x_i, x_j^* \rangle = \delta_{ij}$ kéo theo rằng với mọi $i$, không gian con của $E^*$ trực giao với K.$x_i$ chứa các $x_j^*$ có chỉ số $j \neq i$ nhưng không chứa $x_i^*$, do đó hệ $(x_i^*)_{1 \leq i \leq p}$ là tự do.

#### Hệ quả 3 {#alg-ii-s7-thm-7-cor-3 .statement}

*Cho S là một tập hợp và V là một không gian con vectơ của không gian vectơ phải trên K* $K_d^S$ *gồm các ánh xạ từ S vào K*. *Để có* $\dim V \geq p$ *(trong đó p là một số nguyên)*, *điều kiện cần và đủ là tồn tại p phần tử* $s_i$ *của S và p phần tử* $f_i$ *của V* $(1 \leq i \leq p)$ *sao cho* $f_i(s_j) = \delta_{ij}$.

Không gian $K_d^S$ được đồng nhất một cách chính tắc với đối ngẫu của $E = K_d^{(S)}$ và $f(s) = \langle e_s, f \rangle$ với $s \in S$ và $f \in K_s^S$, trong đó $(e_s)_{s \in S}$ là cơ sở chính tắc của E. Khi đó Hệ quả 2 cho thấy điều kiện ấy là đủ. Ngược lại, giả sử rằng $\dim V \geq p$, nên tồn tại một không gian con $G'$ của V có chiều $p$; gọi F là trực giao của $G'$ trong E, khi đó $\dim(E/F) = p$. Từ no. 1, Định lý 2 suy ra rằng tồn tại $p$ phần tử $s_i \in S$ sao cho các $e_{s_i}$ $(1 \leq i \leq p)$ lập thành một cơ sở của một phần bù F của E (áp dụng Định lý 2 (no. 1) cho một tập con tự do gồm một cơ sở của E và hệ sinh là hợp của tập con tự do này với cơ sở chính tắc của E); khi đó ta lấy các $f_i$ là các phần tử của một cơ sở của G' đối ngẫu với cơ sở của E/F gồm các lớp của $e_{s_i}$ mod. F.

#### Hệ quả 4 {#alg-ii-s7-thm-7-cor-4 .statement}

*Cho E là một không gian vectơ và M, N là hai không gian con của E có đối chiều hữu hạn; nếu M', N' là các trực giao của M và N trong E*, trực giao của M ∩ N trong E* là M' + N'.

Vì M (tương ứng N) là trực giao của M' (tương ứng N') trong E (Định lý 7), M ∩ N là trực giao của M' + N' trong E và do đó M' + N' là trực giao của M ∩ N trong E* (Định lý 7 (iii)).

#### Hệ quả 5 {#alg-ii-s7-thm-7-cor-5 .statement}

*Cho E là một không gian vectơ có số chiều hữu hạn n. Với mọi không gian con F của E có chiều p, trực giao F' của F trong E* có chiều n − p. Với mọi không gian con G' của E* có chiều q, trực giao G của G' trong E có chiều n − q và G' là trực giao của G trong E*.

Định lý 7 cho một đặc trưng hóa khác của các *siêu phẳng* trong E:

#### Mệnh đề 11 {#alg-ii-s7-prop-11 .statement}

*Với mọi siêu phẳng H trong một không gian vectơ E, tồn tại một dạng tuyến tính $x_0^*$ trên E sao cho H = $x_0^{*-1}(0)$. Với một dạng $x_0^*$ như vậy, để một dạng tuyến tính $x^*$ trên E thỏa mãn H = $x^{*-1}(0)$, điều kiện cần và đủ là $x^* = x_0^* \alpha$, trong đó $\alpha$ là một vô hướng ≠ 0. Ngược lại, với mọi dạng tuyến tính $x^* \neq 0$ trên E, không gian con $x^{*-1}(0)$ là một siêu phẳng của E.*

Mệnh đề này chỉ đơn thuần diễn đạt Định lý 7 cho các không gian con của E có đối chiều 1 và các không gian con của E* có chiều 1.

Nếu H là một siêu phẳng và $x_0^*$ là một dạng tuyến tính sao cho H = $x^{*-1}(0)$, quan hệ

$$
\langle x, x_0^* \rangle = 0
$$

đặc trưng các phần tử $x \in H$, được gọi là *một phương trình của H*.

Nói tổng quát hơn, nếu $(x_i^*)$ là một họ các dạng tuyến tính trên E và F ký hiệu không gian con vectơ là giao của các siêu phẳng $x_i^{*-1}(0)$, thì quan hệ "với mọi $i, \langle x, x_i^* \rangle = 0$" đặc trưng các phần tử của F; các quan hệ

$$
\langle x, x_i^* \rangle = 0 \quad \text{với mọi } i
$$

lập thành *một hệ phương trình* của không gian con F. Định lý 7 (ii) biểu thị sự kiện rằng *mọi không gian con vectơ của E đều có thể được xác định bởi một hệ phương trình*.

Hơn nữa, Định lý 7 (i) và (ii) chứng minh rằng một không gian con có đối chiều *hữu hạn* $p$ có thể được xác định bởi một hệ gồm $p$ phương trình

(19)
$$
\langle x, x_i^* \rangle = 0, \quad 1 \leq i \leq p,
$$

trong đó các dạng $x_i^*$ là *độc lập tuyến tính*. Ngược lại, Hệ quả 1 của Định lý 7 cho thấy rằng một không gian con F được xác định bởi một hệ gồm $p$ phương trình (19) thì có đối chiều $\leq p$ và có đối chiều $p$ khi và chỉ khi các $x_i^*$ độc lập tuyến tính; điều này cũng tương đương với việc nói rằng F không thể được xác định bởi một hệ gồm nhiều nhất $p - 1$ trong các phương trình (19).

### 6. PHƯƠNG TRÌNH TUYẾN TÍNH TRONG CÁC KHÔNG GIAN VECTƠ

#### Mệnh đề 12 {#alg-ii-s7-prop-12 .statement}

Cho E, F là hai không gian vectơ trên một trường K và $u : E \to F$ là một ánh xạ tuyến tính. Để phương trình tuyến tính

$$
u(x) = y_0
$$

có ít nhất một nghiệm $x \in E$, điều kiện cần và đủ là $y_0$ trực giao với hạt nhân của ánh xạ chuyển vị ${}^t u$.

Phần trực giao của $u(E)$ trong $F^*$ là ${}^t u^{-1}(0)$ (§ 2, no. 5, Hệ quả của Mệnh đề 8) và do đó phần trực giao của ${}^t u^{-1}(0)$ trong F là $u(E)$ (no. 5, Định lý 7 (ii)).

Ta sẽ thu được một tiêu chuẩn thuận tiện hơn cho các hệ phương trình tuyến tính vô hướng

$$
\langle x, x_i^* \rangle = \eta_i \quad (i \in I)
$$

trong đó ẩn $x$ nhận giá trị trong một không gian vectơ E trên một trường K, các $x_i^*$ là các dạng tuyến tính trên E và các vế phải $\eta_i$ là các phần tử của K.

Nếu ta xét một cơ sở $(a_\lambda)_{\lambda \in L}$ của E, thì hệ (21) tương đương với hệ phương trình

$$
\sum_{\lambda \in L} \xi_\lambda \langle a_\lambda, x_i^* \rangle = \eta_i \quad (i \in I)
$$

với $x = \sum_{\lambda \in L} \xi_\lambda a_\lambda$, các nghiệm của (22) tất yếu là các họ $(\xi_\lambda)$ các phần tử của K có giá hữu hạn.

#### Định nghĩa 4 {#alg-ii-s7-def-4 .statement}

Chiều của không gian con của $E^*$ sinh bởi họ $(x_i^*)$ được gọi là hạng của hệ (21).

#### Mệnh đề 13 {#alg-ii-s7-prop-13 .statement}

Để hệ (21) có hạng hữu hạn r, điều kiện cần và đủ là ánh xạ tuyến tính $u : x \mapsto (\langle x, x_i^* \rangle)$ từ E vào $K_s^I$ có hạng r.

Nếu F' là không gian con của $E^*$ sinh bởi các $x_i^*$, thì hạt nhân của u là phần trực giao F của F' trong E; nếu F' có chiều r, thì F có đối chiều r và ngược lại (no. 5, Định lý 7) và $\mathrm{rg}(u) = \mathrm{codim}_E F$ (no. 4, công thức (11)).

#### Định lý 8 {#alg-ii-s7-thm-8 .statement}

Cho

$$
\langle x, x_i^* \rangle = \eta_i \quad (i \in I)
$$

là một hệ phương trình tuyến tính vô hướng trên một không gian vectơ E trên một trường K. Để hệ này có ít nhất một nghiệm, điều kiện cần là, với mọi họ $(\rho_i)$ các vô hướng có giá hữu hạn sao cho $\sum_i x_i^* \rho_i = 0,\ \sum_i \eta_i \rho_i = 0.$ *Nếu hạng của hệ (21) là hữu hạn, thì điều kiện này cũng đủ.*

Điều kiện đó hiển nhiên là cần. Nó nói rằng, nếu $F'$ là không gian con của $E^*$ sinh bởi họ $(x_i^*)$, thì tồn tại một ánh xạ tuyến tính $f : F' \to K_d$ sao cho $f(x_i^*) = \eta_i$ với mọi $i \in I$. Nếu $F'$ có số chiều hữu hạn $r$, thì $F'$ là trực giao của một không gian con $F$ của $E$ có đối chiều $r$ (no. 5, Định lý 7) và $F'$ được đồng nhất với đối ngẫu của $E/F$ (§ 2, no. 6, Hệ quả của Mệnh đề 9); do đó $f$ là một phần tử của đối ngẫu kép $(E/F)**$. Vì $E/F$ hữu hạn chiều nên tồn tại một và chỉ một phần tử $y \in E/F$ sao cho $f(x^*) = \langle y, x^* \rangle$ với mọi $x^* \in F'$ (no. 5, Định lý 6). Khi đó các nghiệm của (21) là những $x \in E$ mà ảnh chính tắc trong $E/F$ là $y$.

#### Nhận xét {#alg-ii-s7-n6-rem-1 .statement}

Khi hạng của hệ (21) là *vô hạn*, điều kiện của Định lý 8 không còn đủ nữa. Chẳng hạn, giả sử các $x_i^*$ là các *dạng tọa độ* trên không gian $E = K_s^{(I)}$, với $I$ vô hạn (§ 2, no. 6); vì các $x_i^*$ độc lập tuyến tính, điều kiện của Định lý 8 được thỏa mãn với mọi họ $(\eta_i)$ nhưng hệ (21) chỉ có nghiệm nếu họ $(\eta_i)$ có giá hữu hạn.

Một hệ (21) luôn luôn có hạng hữu hạn nếu nó chỉ có một *số hữu hạn phương trình* và khi đó hạng của nó *không vượt quá* số phương trình (no. 2, Mệnh đề 1). Tương tự, nếu $E$ có số chiều hữu hạn $n$ (đối với một hệ (22), điều này tương ứng với trường hợp chỉ có một *số hữu hạn n ẩn*), thì đối ngẫu $E^*$ của nó có chiều $n$ và do đó hạng của hệ (21) không vượt quá $n$ (no. 3, Hệ quả 4 của Mệnh đề 4). Từ đó suy ra:

#### Hệ quả 1 {#alg-ii-s7-thm-8-cor-1 .statement}

*Một hệ phương trình tuyến tính vô hướng trong một không gian vectơ, gồm một số hữu hạn phương trình mà các vế trái là những dạng độc lập tuyến tính, luôn luôn có nghiệm.*

#### Hệ quả 2 {#alg-ii-s7-thm-8-cor-2 .statement}

*Để một hệ tuyến tính thuần nhất (22) gồm các phương trình theo n ẩn với các hệ số trong một trường $K$ có các nghiệm không tầm thường gồm các phần tử của $K$, điều kiện cần và đủ là hạng của nó < n.*

Điều này luôn luôn đúng nếu số phương trình là hữu hạn và < n.

#### Hệ quả 3 {#alg-ii-s7-thm-8-cor-3 .statement}

*Để một hệ tuyến tính (22) với các hệ số và các vế phải trong một trường $K$, gồm n phương trình theo n ẩn, có một và chỉ một nghiệm gồm các phần tử của $K$, điều kiện cần và đủ là hệ thuần nhất liên kết không có nghiệm không tầm thường* (hay, điều tương đương, là các vế trái của hệ này là những *dạng độc lập tuyến tính*).

### 7. TÍCH TENXƠ CỦA CÁC KHÔNG GIAN VECTƠ

Các kết quả của §§ 3, 4 và 5 liên quan đến các môđun tự do hoặc xạ ảnh áp dụng đặc biệt cho các không gian vectơ và cho các tính chất sau đây:

#### Mệnh đề 14 {#alg-ii-s7-prop-14 .statement}

*Cho một dãy khớp*

(23)
$$
0 \to E' \to E \to E'' \to 0
$$
*các không gian vectơ phải trên một trường K và các ánh xạ tuyến tính và một không gian vectơ trái F trên K, thì dãy tương ứng các ánh xạ tuyến tính trên $\mathbf{Z}$*
$$
0 \to E' \otimes_K F \to E \otimes_K F \to E'' \otimes_K F \to 0
$$
*là khớp và tách được*.

Vì dãy (23) tách được, đây là một trường hợp riêng của § 3, no. 7, Hệ quả 5 của Mệnh đề 7 và § 3, no. 6, Mệnh đề 5.

Do Mệnh đề 14, khi $E'$ là một không gian con vectơ của $E$, $j : E' \to E$ là đơn ánh chính tắc, thì $E' \otimes_K F$ thường được *đồng nhất* với một môđun con *trên $\mathbf{Z}$* của $E \otimes_K F$ nhờ đơn ánh $j \otimes 1_F$. Với quy ước này:

#### Hệ quả {#alg-ii-s7-n7-cor-1 .statement}

*Cho K là một trường, E là một không gian vectơ phải trên K, F là một không gian vectơ trái trên K, $(M_\alpha)_{\alpha \in A}$ là một họ các không gian con vectơ của E và $(N_\beta)_{\beta \in B}$ là một họ các không gian con vectơ của F. Khi đó*
$$
\left( \bigcap_{\alpha \in A} M_\alpha \right) \otimes_K \left( \bigcap_{\beta \in B} N_\beta \right) = \bigcap_{(\alpha, \beta) \in A \times B} (M_\alpha \otimes_K N_\beta).
$$

Hiển nhiên là đủ để chứng minh trường hợp riêng
$$
\left( \bigcap_{\alpha \in A} M_\alpha \right) \otimes_K F = \bigcap_{\alpha \in A} (M_\alpha \otimes_K F).
$$

Rõ ràng vế trái của (25) được chứa trong vế phải. Để chứng minh đảo lại, ta xét một cơ sở $(f_\lambda)_{\lambda \in L}$ của $F$. Khi đó mọi phần tử của $E \otimes_K F$ có thể được biểu diễn duy nhất dưới dạng $\sum_{\lambda \in L} x_\lambda \otimes f_\lambda$, trong đó $x_\lambda \in E$ (§ 3, no. 7, Hệ quả 1 của Mệnh đề 7); nếu $E'$ là một không gian con vectơ của $E$, quan hệ $\sum_{\lambda \in L} x_\lambda \otimes f_\lambda \in E' \otimes_K F$ tương đương, theo Mệnh đề 14, với $x_\lambda \in E'$ với mọi $\lambda \in L$. Do đó, nói rằng $\sum_{\lambda \in L} x_\lambda \otimes f_\lambda$ thuộc mỗi $M_\alpha \otimes_K F$ có nghĩa là với mọi $\lambda \in L$ và mọi $\alpha \in A$, ta có $x_\lambda \in M_\alpha$, tức là $x_\lambda \in \bigcap_{\alpha \in A} M_\alpha$ với mọi $\lambda \in L$, điều này chứng tỏ rằng vế phải của (25) được chứa trong vế trái.

#### Mệnh đề 15 {#alg-ii-s7-prop-15 .statement}

*Nếu $(E_\lambda)_{\lambda \in L}$ là một họ các không gian vectơ phải trên một trường K và $(F_\mu)_{\mu \in M}$ là một họ các không gian vectơ trái trên K, thì ánh xạ chính tắc*
$$
\left( \prod_{\lambda \in L} E_\lambda \right) \otimes_K \left( \prod_{\mu \in M} F_\mu \right) \to \prod_{(\lambda, \mu) \in L \times M} (E_\lambda \otimes_K F_\mu)
$$
*(§ 3, no. 7, công thức (22)) là đơn ánh.*

Ta viết $F = \prod_{\mu \in M} F_\mu$; ánh xạ (26) là hợp thành của các ánh xạ chính tắc
$$
\left( \prod_{\lambda \in L} E_\lambda \right) \otimes_K F \to \prod_{\lambda \in L} (E_\lambda \otimes_K F)
$$
và
$$
\prod_{\lambda \in L} (E_\lambda \otimes_K F) \to \prod_{\lambda \in L} \left( \prod_{\mu \in M} (E_\lambda \otimes_K F_\mu) \right);
$$
vì $F$ và các $E_\lambda$ là các không gian vectơ trên $K$, điều này quy về § 3, no. 7, Hệ quả 3 của Mệnh đề 7.

Khi các điều kiện của Mệnh đề 15 được thỏa mãn, tích tenxơ
$$
\left( \prod_{\lambda \in L} E_\lambda \right) \otimes_K \left( \prod_{\mu \in M} F_\mu \right)
$$
thường được đồng nhất với ảnh chính tắc của nó trong
$$
\prod_{\lambda, \mu} (E_\lambda \otimes_K F_\mu).
$$
Với quy ước này:

#### Hệ quả {#alg-ii-s7-n7-cor-2 .statement}

*Cho $F$ là một không gian vectơ trái trên $K$; với mọi tập hợp $X$, không gian vectơ trái $K_d^X \otimes_K F$ được đồng nhất với không gian con của không gian $F^X$ gồm mọi ánh xạ từ $X$ vào $F$, gồm các ánh xạ $u$ sao cho $u(X)$ có hạng hữu hạn trong $F$.*

Nếu $(f_\lambda)$ là một cơ sở của $F$, phần tử $\sum_{\lambda \in L} v_\lambda \otimes f_\lambda$ của $K_d^X \otimes_K F$ được đồng nhất qua (26) với ánh xạ $x \mapsto \sum_\lambda v_\lambda(x) f_\lambda$. Vì $v_\lambda = 0$ trừ các chỉ số $\lambda$ thuộc một tập con hữu hạn $H$ của $L$, ảnh của $X$ dưới ánh xạ trên được chứa trong không gian con hữu hạn chiều của $F$ sinh bởi các $f_\lambda$ có chỉ số $\lambda \in H$. Ngược lại, cho $u : X \to F$ là một ánh xạ sao cho $u(X)$ được chứa trong một không gian con hữu hạn chiều $G$ của $F$ và cho $(b_i)_{1 \leq i \leq n}$ là một cơ sở của $G$. Với mọi $x \in X$, ta có thể viết $u(x) = \sum_{i=1}^n v_i(x) b_i$, trong đó các $v_i(x)$ là những phần tử được xác định của $K$; do đó xác định được $n$ ánh xạ $v_i : X \to K$ và rõ ràng khi ấy $u$ được đồng nhất với phần tử $\sum_{i=1}^n v_i \otimes b_i$.

Tương tự, với một không gian vectơ phải $E$ trên $K$ và một tập hợp $Y$, $E \otimes_K K_s^Y$ được đồng nhất với một không gian con của không gian $E^Y$, gồm các ánh xạ $v : Y \to E$ sao cho $v(Y)$ có hạng hữu hạn. Đặc biệt hơn, với mọi trường $K$, $K_d^X \otimes_K K_s^Y$ được đồng nhất với một không gian con của không gian $K^{X \times Y}$ gồm các ánh xạ từ $X \times Y$ vào $K$ ($K$ được xét như một song môđun $(K, K)$); một phần tử $\sum_i u_i \otimes v_i$, trong đó $u_i$ là một ánh xạ từ $X$ vào $K$ và $v_i$ là một ánh xạ từ $Y$ vào $K$, được đồng nhất với ánh xạ $(x, y) \mapsto \sum_i u_i(x) v_i(y)$ từ $X \times Y$ vào $K$.

#### Mệnh đề 16 {#alg-ii-s7-prop-16 .statement}

(i) *Cho K, L là hai trường, E là một không gian vectơ trái trên K, F là một không gian vectơ trái trên L và G là một song môđun (K, L). Khi đó $\mathbf{Z}$-đồng cấu chính tắc*

$$
\nu : \operatorname{Hom}_K(E, G) \otimes_L F \to \operatorname{Hom}_K(E, G \otimes_L F)
$$

(§ 4, no. 2, công thức (7)) *là đơn ánh; nó là song ánh khi một trong hai không gian vectơ E, F là hữu hạn chiều*.

(ii) *Cho $E_1, E_2, F_1, F_2$ là bốn không gian vectơ trên một trường giao hoán K; khi đó K-đồng cấu chính tắc*

$$
\lambda : \operatorname{Hom}(E_1, F_1) \otimes \operatorname{Hom}(E_2, F_2) \to \operatorname{Hom}(E_1 \otimes E_2, F_1 \otimes F_2)
$$

(§ 4, no. 4, công thức (21)) *là đơn ánh; nó là song ánh nếu một trong các cặp có thứ tự $(E_1, E_2), (E_1, F_1), (E_2, F_2)$ gồm các không gian hữu hạn chiều*.

Mệnh đề (i) là một trường hợp riêng của § 4, no. 2, Mệnh đề 2. Tương tự, mệnh đề thứ hai của (ii) là một trường hợp riêng của § 4, no. 4, Mệnh đề 4. Sau hết, để thấy rằng đồng cấu (28) luôn luôn là đơn ánh, hãy nhận xét rằng $\operatorname{Hom}(E_i, F_i)$ là một không gian con vectơ của $F_i^{E_i}$ ($i = 1, 2$) và rằng

$$
\operatorname{Hom}(E_1 \otimes E_2, F_1 \otimes F_2)
$$

được đồng nhất một cách chính tắc với một không gian con vectơ của không gian $(F_1 \otimes F_2)^{E_1 \times E_2}$ (II, § 3, no. 1, Mệnh đề 1); khi thực hiện các sự đồng nhất này và đồng thời đồng nhất vế trái của (28) với một không gian con của $F_1^{E_1} \otimes F_2^{E_2}$ (Mệnh đề 14), thì ánh xạ chính tắc (28) trở thành hạn chế lên không gian con này của ánh xạ chính tắc (26), và đã thấy (Mệnh đề 15) rằng ánh xạ sau là đơn ánh.

#### Hệ quả 1 {#alg-ii-s7-prop-16-cor-1 .statement}

*Cho E và F là hai không gian vectơ trên một trường K; ánh xạ chính tắc*

$$
E^* \otimes_K F \to \operatorname{Hom}_K(E, F)
$$

(§ 4, no. 2, công thức (11)) *là đơn ánh; nó là song ánh khi E hoặc F là hữu hạn chiều*.

Đây là một trường hợp riêng của Mệnh đề 16 (i).

#### Hệ quả 2 {#alg-ii-s7-prop-16-cor-2 .statement}

*Cho E là một không gian vectơ phải và F là một không gian vectơ trái trên cùng trường K; ánh xạ chính tắc*

$$
E \otimes_K F \to \operatorname{Hom}_K(E^*, F)
$$

(§ 4, no. 2, công thức (15)) *là đơn ánh; nó là song ánh khi E là hữu hạn chiều*.

Đây là một trường hợp riêng của § 4, no. 2, Nhận xét 2.

#### Nhận xét {#alg-ii-s7-n7-rem-1 .statement}

(1) Cho K là một trường *giao hoán*, E, F là hai không gian vectơ trên K, (a_\lambda) là một cơ sở của E và (b_\mu) là một cơ sở của F; khi đó (a_\lambda \otimes b_\mu) là một cơ sở của không gian vectơ K E \otimes_K F (II, § 3, no. 7, Hệ quả 2 của Mệnh đề 2) và do đó
$$
\dim_K(E \otimes_K F) = \dim_K E \cdot \dim_K F.
$$
(2) Cho K là một trường *giao hoán*, E_1, E_2, F_1, F_2 là bốn không gian vectơ trên K và u:E_1 \to F_1, v:E_2 \to F_2 là hai ánh xạ tuyến tính; khi đó
$$
\operatorname{rg}(u \otimes v) = \operatorname{rg}(u) \cdot \operatorname{rg}(v).
$$
Ngay lập tức thấy rằng $(u \otimes v)(E_1 \otimes E_2)$ là ảnh chính tắc của $u(E_1) \otimes v(E_2)$ trong $F_1 \otimes F_2$ và do đó (Mệnh đề 14) đẳng cấu với $u(E_1) \otimes v(E_2)$; khi đó kết luận suy ra từ (30).
(3) Dưới cùng các giả thiết như trong *Nhận xét* 1,
$$
\dim_K(\operatorname{Hom}_K(E, F)) \geq \dim_K E \cdot \dim_K F.
$$
Nếu E đẳng cấu với $K^{(I)}$, $\operatorname{Hom}(E, F)$ đẳng cấu với $(\operatorname{Hom}(K, F))^I$ (§ 1, no. 6, Hệ quả 1 của Mệnh đề 6) và do đó với $F^I$ (§ 1, no. 14); vì $F^{(I)}$ là một không gian con của $F^I$ và $\dim(F^{(I)}) = \operatorname{Card}(I) \cdot \dim F = \dim E \cdot \dim F$ (no. 2, Mệnh đề 2), bất đẳng thức (32) suy ra từ no. 3, Hệ quả 4 của Mệnh đề 4. Lập luận tương tự cũng cho thấy hai vế của (32) bằng nhau khi $\dim E$ là *hữu hạn* (xem § 10, nos. 3 và 4).

### 8. HẠNG CỦA MỘT PHẦN TỬ CỦA MỘT TÍCH TENXƠ

Cho E là một không gian vectơ phải và F là một không gian vectơ trái trên cùng trường K; với mỗi phần tử $u \in E \otimes_K F$ tương ứng một cách chính tắc theo (29) một đồng cấu $u_1 \in \operatorname{Hom}_K(E^*, F)$; nếu $u = \sum_i x_i \otimes y_i$ với $x_i \in E, y_i \in F$, phần tử $u_1$ là ánh xạ tuyến tính
$$
x^* \mapsto \sum_i \langle x^*, x_i \rangle y_i.
$$
Mặt khác, $E \otimes_K F$ được đồng nhất một cách chính tắc với $F \otimes_{K^0} E$, trong đó E được xét như một không gian vectơ trái và F như một không gian vectơ phải trên trường đối $K^0$; do đó tương ứng một cách chính tắc với $u$ là một đồng cấu $u_2 \in \operatorname{Hom}_K(F^*, E)$ được cho bởi
$$
y^* \mapsto \sum_i x_i \langle y_i, y^* \rangle;
$$
$u_1$ (tương ứng $u_2$), được xét như một ánh xạ từ $E^*$ vào $F^{**}$ (tương ứng từ $F^*$ vào $E^{**}$), chính là *chuyển vị* của $u_2$ (tương ứng $u_1$). Do đó các *hạng* của $u_1$ và $u_2$ *bằng* cùng một số *hữu hạn* $r$, là chiều chung của các không gian con $u_1(E^*)$ của F và $u_2(F^*)$ của E, mỗi không gian được đẳng cấu chính tắc với đối ngẫu của không gian kia (no. 5); ta sẽ nói rằng $r$ (ký hiệu là $\operatorname{rg}(u)$) là *hạng* của phần tử $u$ của $E \otimes_K F$ và rằng $u_1(E^*)$ và $u_2(F^*)$ là các không gian con (lần lượt của F và E) *liên kết* với $u$.

#### Mệnh đề 17 {#alg-ii-s7-prop-17 .statement}

Cho u là một phần tử của $E \otimes_K F$ và $M \subset E$ và $N \subset F$ là các không gian con liên kết của nó. Với mọi biểu thức $u = \sum_{i=1}^s x_i \otimes y_i$ của $u$, trong đó $x_i \in E$ và $y_i \in F$ với $1 \leq i \leq s$, không gian con $M$ (tương ứng $N$) được chứa trong không gian con của $E$ (tương ứng $F$) sinh bởi các $x_i$ (tương ứng các $y_i$). Hơn nữa, các tính chất sau là tương đương:

(a) Số nguyên $s$ bằng hạng của $u$.
(b) Họ $(x_i)_{1 \leq i \leq s}$ là một cơ sở của $M$.
(c) Họ $(y_i)_{1 \leq i \leq s}$ là một cơ sở của $N$.
(d) Các họ $(x_i)_{1 \leq i \leq s}$ và $(y_i)_{1 \leq i \leq s}$ đều tự do.

Theo (33) (tương ứng (34)) mỗi phần tử của $N = u_1(E^*)$ (tương ứng $M = u_2(F^*)$) là một tổ hợp tuyến tính của các $y_i$ (tương ứng các $x_i$); do đó có mệnh đề thứ nhất. Nếu $s = r$, không gian con sinh bởi các $x_i$ (tương ứng các $y_i$), có chiều $\leq \dim M$ (tương ứng $\leq \dim N$) và chứa $M$ (tương ứng $N$), là đồng nhất với nó, và vì thế (a) kéo theo (b) và (c) và *a fortiori* (d). Ngược lại, mỗi điều kiện (b) và (c) đều kéo theo (a) theo định nghĩa của $\mathrm{rg}(u)$. Cuối cùng nếu (d) đúng, tồn tại một họ $(x_i^*)_{1 \leq i \leq s}$ gồm các phần tử của $E^*$ sao cho $\langle x_i, x_j^* \rangle = \delta_{ij}$ (no. 5, Hệ quả 1 của Định lý 7) và do đó suy ra từ (33) rằng $(y_i)$ là một cơ sở của $N$, điều này hoàn tất chứng minh.

#### Hệ quả 1 {#alg-ii-s7-prop-17-cor-1 .statement}

*Hạng của u là số nguyên nhỏ nhất s sao cho tồn tại một biểu thức* $u = \sum_{i=1}^s x_i \otimes y_i$, *trong đó* $x_i \in E$ *và* $y_i \in F$ *với* $1 \leq i \leq s$.

Điều này suy ra ngay lập tức từ Mệnh đề 17 và no. 2, Mệnh đề 1.

#### Hệ quả 2 {#alg-ii-s7-prop-17-cor-2 .statement}

*Cho K là một trường giao hoán, E, F là hai không gian vectơ trên K và L là một trường mở rộng giao hoán của K. Cho u là một phần tử của* $E \otimes_K F$, *M và N là các không gian con liên kết của nó và u' là ảnh chính tắc của u trong* $(E \otimes_K F)_{(L)}$ *(được đồng nhất một cách chính tắc với* $E_{(L)} \otimes_L F_{(L)}$, *xem § 5, no. 1, Mệnh đề 3); khi đó* $\mathrm{rg}(u') = \mathrm{rg}(u)$ *và các không gian con liên kết với u' được đồng nhất một cách chính tắc với* $M_{(L)}$ *và* $N_{(L)}$.

Nếu $u = \sum_{i=1}^r x_i \otimes y_i$, trong đó các họ $(x_i)$ và $(y_i)$ đều tự do, thì $u' = \sum_{i=1}^r (1 \otimes x_i) \otimes (1 \otimes y_i)$ và các họ $(1 \otimes x_i)$ và $(1 \otimes y_i)$ lần lượt tự do trong $E_{(L)}$ và $F_{(L)}$ (§ 5, no. 1, Mệnh đề 4).

### 9. MỞ RỘNG VÔ HƯỚNG CHO MỘT KHÔNG GIAN VECTƠ

Nhắc lại (I, § 9, no. 1, Định lý 2) rằng một đồng cấu từ một trường K vào một vành khác không A tất yếu là *đơn ánh*.

#### Proposition 18 {#alg-ii-s7-prop-18 .statement}

Cho $\varphi$ là một đồng cấu của một trường $K$ vào một vành $A$. Với mọi dãy khớp các không gian vectơ $K$ và các ánh xạ tuyến tính $K$

$$
E' \xrightarrow{u} E \xrightarrow{v} E''
$$

thì dãy

$$
E'_{(A)} \xrightarrow{u_{(A)}} E_{(A)} \xrightarrow{v_{(A)}} E''_{(A)}
$$

là khớp.

Đây là một trường hợp riêng của no. 7, Proposition 14, có tính đến § 1, no. 4, Remark 4.

#### Hệ quả {#alg-ii-s7-n9-cor-1 .statement}

Với mọi ánh xạ tuyến tính $K$ $f : E' \to E$, $\operatorname{Im}(f_{(A)}) = (\operatorname{Im}(f))_{(A)}$, $\operatorname{Ker}(f_{(A)}) = (\operatorname{Ker}(f))_{(A)}$, $\operatorname{Coker}(f_{(A)}) = (\operatorname{Coker}(f))_{(A)}$, sai khác bởi các đẳng cấu chính tắc.

#### Mệnh đề 19 {#alg-ii-s7-prop-19 .statement}

Cho $\varphi$ là một đơn cấu của một trường $K$ vào một vành $A$. Với mọi không gian vectơ trái $E$ trên $K$, ánh xạ chính tắc $\phi : E \to \varphi^*(E) = A \otimes_K E$ là đơn ánh. Hơn nữa, với mọi không gian con vectơ $E'$ của $E$, $\varphi^*(E') = A \otimes_K E'$ được đồng nhất một cách chính tắc với một môđun con-$A$ nhân tử trực tiếp của $A \otimes_K E$ và, với sự đồng nhất này,

$$
(A \otimes_K E') \cap \phi(E) = \phi(E').
$$

Mệnh đề thứ nhất là một trường hợp riêng của § 5, no. 1, Proposition 4; mệnh đề thứ hai là một trường hợp riêng của no. 7, Proposition 14; sau cùng, để chứng minh (35), chỉ cần lấy trong $A$ (được xét như một $K$-môđun phải) một cơ sở $(a_\lambda)_{\lambda \in L}$ sao cho $a_{\lambda_0} = 1$ đối với một chỉ số nào đó $\lambda_0$ (no. 1, Theorem 2); các phần tử của $A \otimes_K E$ có thể được viết duy nhất dưới dạng $\sum \lambda a_\lambda \otimes x_\lambda$ với $x_\lambda \in E$ và, để một phần tử như thế thuộc $A \otimes_K E'$, điều kiện cần và đủ là $x_\lambda \in E'$ với mọi $\lambda$. Mặt khác, các phần tử của $\phi(E)$ là những phần tử mà đối với chúng $x_\lambda = 0$ với $\lambda \neq \lambda_0$; để một phần tử $\sum \lambda a_\lambda \otimes x_\lambda$ thuộc $(A \otimes_K E') \cap \phi(E)$, điều kiện cần và đủ là $x_\lambda = 0$ với $\lambda \neq \lambda_0$ và $x_{\lambda_0} \in E'$, do đó suy ra kết luận.

#### Hệ quả {#alg-ii-s7-n9-cor-2 .statement}

Cho $\varphi$ là một đơn cấu của một trường $K$ vào một vành $A$. Để một ánh xạ tuyến tính $K$ $f : E \to F$ (trong đó $E$ và $F$ là hai không gian vectơ trên $K$) là đơn ánh (tương ứng, toàn ánh, không), điều kiện cần và đủ là $f_{(A)} : E_{(A)} \to F_{(A)}$ là đơn ánh (tương ứng, toàn ánh, không).

Điều này suy ra ngay lập tức từ Mệnh đề 19 và Hệ quả của Mệnh đề 18.

#### Mệnh đề 20 {#alg-ii-s7-prop-20 .statement}

Cho $\rho$ là một đồng cấu của một trường $K$ vào một vành $A$. Với mọi không gian vectơ trái $E$ trên $K$, đồng cấu chính tắc môđun phải $A$

$$
v : (E^*)_{(A)} \to (E_{(A)})^*
$$

(§ 5, no. 4) là đơn ánh; nó là song ánh khi $E$ hữu hạn chiều.

Mệnh đề thứ hai suy ra từ § 5, no. 4, Mệnh đề 8. Để chứng minh mệnh đề thứ nhất, ta nhận thấy rằng mọi phần tử của $(E^*)_{(A)}$ đều có thể viết dưới dạng $\sum_i x_i^* \otimes \alpha_i$, trong đó $\alpha_i \in A$ và $(x_i^*)_{1 \leq i \leq n}$ là một họ tự do trong $E^*$; ứng với nó trong $(E_{(A)})^*$ là dạng tuyến tính $y^*$ sao cho $y^*(1 \otimes x) = \sum_i \rho(\langle x, x_i^* \rangle) \alpha_i$ với mọi $x \in E$. Nhưng tồn tại trong $E$ một họ $(x_i)_{1 \leq i \leq n}$ sao cho $\langle x_i, x_j^* \rangle = \delta_{ij}$ (no. 5, Hệ quả 2 của Định lý 7), do đó $y^*(1 \otimes x_i) = \alpha_i$; vì thế quan hệ $y^* = 0$ kéo theo $\alpha_i = 0$ với mọi $i$, điều đó chứng minh mệnh đề của ta.

#### Mệnh đề 21 {#alg-ii-s7-prop-21 .statement}

Cho $K$ là một trường và $L$ là một trường mở rộng của $K$.

(i) Với mọi không gian vectơ $E$ trên $K$, $\dim_L(E_{(L)}) = \dim_K E$.

(ii) Với mọi ánh xạ tuyến tính trên $K$ $u : E \to F$, trong đó $E$ và $F$ là các không gian vectơ trên $K$, $\operatorname{rg}(u_{(L)}) = \operatorname{rg}(u)$.

Nếu $(e_i)_{i \in I}$ là một cơ sở của $E$ trên $K$, thì $(1 \otimes e_i)_{i \in I}$ là một cơ sở của $E_{(L)}$ trên $L$ (§ 5, no. 1, Mệnh đề 4), do đó có mệnh đề thứ nhất; mệnh đề thứ hai suy ra từ mệnh đề thứ nhất và sự kiện rằng $u_{(L)}(E_{(L)})$ được đồng nhất một cách chính tắc với $(u(E))_{(L)}$ bởi Hệ quả của Mệnh đề 18.

#### Mệnh đề 22 {#alg-ii-s7-prop-22 .statement}

Cho $K$ là một trường giao hoán, $\rho : K \to A$ là một đồng cấu trung tâm đơn ánh và $E, F$ là hai không gian vectơ trên $K$. Khi đó đồng cấu chính tắc

$$
\omega : A \otimes_K \operatorname{Hom}(E, F) \to \operatorname{Hom}_A(E_{(A)}, F_{(A)})
$$

(§ 5, no. 3, công thức (17)) là đơn ánh; nó là song ánh nếu $A$ hoặc $E$ là một không gian vectơ hữu hạn chiều trên $K$.

Đây là một trường hợp riêng của § 5, no. 3, Mệnh đề 7.

### 10. MÔĐUN TRÊN CÁC MIỀN NGUYÊN

#### Mệnh đề 23 {#alg-ii-s7-prop-23 .statement}

Trong một môđun $E$ trên một miền nguyên $A$, tập hợp $T$ của các phần tử không tự do là một môđun con của $E$.

Nếu $x$ và $y$ không tự do, tồn tại hai phần tử khác không $\alpha, \beta$ của $A$ sao cho $\alpha x = 0$ và $\beta y = 0$. Khi đó $\alpha \beta \neq 0$ vì $A$ là một miền nguyên và $\alpha \beta (\lambda x + \mu y) = 0$ với mọi $\lambda$ và $\mu$ trong $A$ vì $A$ giao hoán; do đó $\lambda x + \lambda y$ không tự do.

#### Nhận xét {#alg-ii-s7-n10-rem-1 .statement}

Cho $E$ là một môđun trên một vành giao hoán bất kỳ $A$. Nếu $x$ là một phần tử không tự do của $E$, mọi phần tử của môđun con $Ax$ đều không tự do. Mặt khác, nếu $A$ chứa các ước số của 0, tổng của hai phần tử không tự do của $E$ có thể là tự do; chẳng hạn, trong $\mathbf{Z}/6\mathbf{Z}$ được xét như một môđun trên chính nó, 3 và 4 không tự do, nhưng $3 + 4 = 1$ là tự do.

Mệnh đề 23 dẫn đến định nghĩa sau đây:

#### Định nghĩa 5 {#alg-ii-s7-def-5 .statement}

*Trong một môđun $E$ trên một miền nguyên $A$, môđun con xoắn của $E$ là môđun con của $E$ gồm các phần tử không tự do* (cũng gọi là các *phần tử xoắn* của $E$).

Khi $E$ bằng môđun con xoắn của nó (nghĩa là khi mọi phần tử của $E$ bị triệt tiêu bởi một phần tử $\neq 0$ của $A$) thì $E$ được gọi là một *môđun xoắn*. Khi môđun con xoắn của $E$ thu về 0 (nghĩa là mọi phần tử khác không của $E$ là *tự do*) thì $E$ được gọi (do lạm dụng ngôn ngữ) là một *môđun không xoắn*.

Mọi môđun con của một $A$-môđun tự do (và đặc biệt mọi $A$-môđun *xạ ảnh*) đều không xoắn. $\mathbf{Z}$-môđun $\mathbf{Q}$ là không xoắn.

#### Mệnh đề 24 {#alg-ii-s7-prop-24 .statement}

*Cho $A$ là một miền nguyên. Với mọi $A$-môđun $E$, ký hiệu $T(E)$ là môđun con xoắn của $E$. Cho $f : E \to E'$ là một ánh xạ tuyến tính $A$, trong đó $E$ và $E'$ là các $A$-môđun.*

(i) $f(T(E)) \subset T(E')$.
(ii) *Nếu $f$ là đơn ánh, thì $f(T(E)) = T(E') \cap f(E)$.*
(iii) *Nếu $f$ là toàn ánh và $\operatorname{Ker}(f) \subset T(E)$, thì $f(T(E)) = T(E')$.*

Các khẳng định (i) và (ii) là hiển nhiên. Mặt khác, nếu $f$ là toàn ánh và $x' \in T(E')$, thì $x' = f(x)$, trong đó $x \in E$, và theo giả thiết tồn tại $\alpha \neq 0$ trong $A$ sao cho $f(\alpha x) = \alpha x' = 0$; do đó $\alpha x \in \operatorname{Ker}(f)$ và theo giả thiết tồn tại $\beta \neq 0$ trong $A$ sao cho $\beta(\alpha x) = 0$; vì $\beta \alpha \neq 0$, nên $x \in T(E)$.

#### Hệ quả 1 {#alg-ii-s7-prop-24-cor-1 .statement}

*Với mọi $A$-môđun $E$, $E/T(E)$ là không xoắn.*

Nếu $f : E \to E'$ là một ánh xạ $A$-tuyến tính, ký hiệu $f_T$ là ánh xạ $T(E) \to T(E')$ có cùng đồ thị với hạn chế của $f$ trên $T(E)$. Với ký hiệu đó:

#### Hệ quả 2 {#alg-ii-s7-prop-24-cor-2 .statement}

*Với mọi dãy khớp các $A$-môđun và các ánh xạ $A$-tuyến tính*

$$
0 \longrightarrow E' \xrightarrow{f} E \xrightarrow{g} E''
$$

*dãy*

$$
0 \longrightarrow T(E') \xrightarrow{f_T} T(E) \xrightarrow{g_T} T(E'')
$$

*là khớp*.

$$
\operatorname{Ker}(g_T) = \operatorname{Ker}(g) \cap T(E) = f(E') \cap T(E) = f(T(E')) = \operatorname{Im}(f_T).
$$

#### Mệnh đề 25 {#alg-ii-s7-prop-25 .statement}

*Cho $A$ là một miền nguyên và $(E_i)$ là một họ các $A$-môđun; khi đó*

$$
T\left( \bigoplus_i E_i \right) = \bigoplus_i T(E_i).
$$

Cho $(x_i)$ là một phần tử của $\bigoplus_i E_i$ sao cho $x_i \in T(E_i)$ với mọi $i$; khi đó mỗi $x_i$ bị triệt tiêu bởi một phần tử $\alpha_i \neq 0$ của $A$ và có thể giả sử rằng $\alpha_i = 1$ khi $x_i = 0$; vì họ $(x_i)$ có giá hữu hạn, phần tử $\alpha = \prod_i \alpha_i$ của $A$ được xác định và $\neq 0$; hiển nhiên nó triệt tiêu $\bigoplus_i x_i$ và do đó $\bigoplus_i T(E_i) \subset T\left(\bigoplus_i E_i\right)$; đảo lại là ngay lập tức.

Nếu $E$ và $F$ là hai $A$-môđun, thì rõ ràng $T(E \otimes_A F)$ chứa các ảnh chính tắc của $T(E) \otimes_A F$ và $E \otimes_A T(F)$; nhưng có thể cho các ví dụ về những $A$-môđun *không xoắn* $E, F$ sao cho $T(E \otimes_A F) \neq 0$ (Bài tập 31).

Chú ý rằng một tích *vô hạn* của các môđun xoắn không nhất thiết là một môđun xoắn; chẳng hạn, trong $\mathbf{Z}$-môđun $\prod_{n=1}^\infty (\mathbf{Z}/p^n\mathbf{Z})$ ($p$ là một số nguyên > 1), phần tử mà mọi tọa độ đều bằng 1 là tự do.

#### Mệnh đề 26 {#alg-ii-s7-prop-26 .statement}

*Cho $A$ là một miền nguyên, $K$ là trường phân thức của nó, $E$ là một $A$-môđun và $E_{(K)} = K \otimes_A E$ là không gian vectơ trên $K$ thu được bằng cách mở rộng vành các toán tử; kí hiệu $\phi$ là ánh xạ $A$-tuyến tính chính tắc $x \mapsto 1 \otimes x$ của $E$ vào $E_{(K)}$.*

(i) *Mọi phần tử của $E_{(K)}$ đều có dạng $\lambda^{-1} \phi(x)$ với $\lambda \in A, \lambda \neq 0$ và $x \in E$.*
(ii) *Hạt nhân của $\phi$ là môđun con xoắn $T(E)$ của $E$.*

(i) Mọi phần tử của $E_{(K)}$ đều có dạng $z = \sum_{i=1}^n \xi_i \phi(x_i)$ với $\xi_i \in K$ và $x_i \in E$; với mọi $i$, tồn tại $\alpha_i \in A$ sao cho $\alpha_i \neq 0$ và $\alpha_i \xi_i \in A$; nếu $\alpha = \prod_{i=1}^n \alpha_i$, thì $\alpha \neq 0$ và $\alpha \xi_i = \beta_i \in A$ với mọi $i$, do đó, trong $E_{(K)}$,

$$
z = \alpha^{-1}(\alpha z) = \alpha^{-1} \sum_{i=1}^n \beta_i \phi(x_i) = \alpha^{-1} \phi\left( \sum_{i=1}^n \beta_i x_i \right)
$$

vì $\phi$ là $A$-tuyến tính.

(ii) Nếu $x \neq 0$ không tự do trong $E$, thì tồn tại $\alpha \neq 0$ trong $A$ sao cho $\alpha x = 0$, do đó $\alpha \phi(x) = \phi(\alpha x) = 0$ trong $E_{(K)}$, suy ra $\phi(x) = 0$. Ngược lại, giả sử rằng, với một $x \in E$, $1 \otimes x = 0$ trong $E_{(K)}$; ta sẽ chứng minh rằng $x$ là một phần tử xoắn của $E$. Xét tập $\mathfrak{M}$ các $A$-môđun con *đơn sinh* của $K$; đó là một tập có hướng phải đối với quan hệ bao hàm, vì mọi hai phần tử $\alpha, \beta$ của $K$ đều có thể viết dưới dạng $\alpha = \zeta^{-1} \xi, \beta = \zeta^{-1} \eta$, trong đó $\xi, \eta, \zeta$ thuộc $A$ và $\zeta \neq 0$, do đó $A.\alpha \subset A.\zeta^{-1}$ và $A.\beta \subset A.\zeta^{-1}$. Hơn nữa $K$ là hợp của các môđun $M \in \mathfrak{M}$ và vì thế có thể được xem như *giới hạn trực tiếp* của hệ trực tiếp xác định bởi các môđun $M \in \mathfrak{M}$ và các đơn ánh chính tắc (§ 6, no. 2, *Nhận xét*). Do đó, cũng như vậy, sai khác bởi một đẳng cấu chính tắc, $E_{(K)} = \lim \rightarrow (M \otimes_A E)$ (§ 6, no. 3, Mệnh đề 7) và hệ thức $1 \otimes x = 0$ trong $E_{(K)}$ kéo theo rằng tồn tại một

M ∈ 𝒫 sao cho l ∈ M và l ⊗ x = 0 trong tích tenxơ M ⊗_A E (Set Theory, III, § 7, no. 5, Bổ đề 1). Hơn nữa có thể giả sử (nếu cần thay thế M bằng một môđun con đơn sinh M' ⊃ M của K) rằng M = A.γ^{-1}, trong đó γ ∈ A và γ ≠ 0. Khi đó ánh xạ ξ ↦ γξ là một đẳng cấu của M lên A-môđun A; mặt khác, đẳng cấu chính tắc A ⊗_A E → E (§ 3, no. 4, Mệnh đề 4) ánh xạ ξ ⊗ x lên phần tử ξx của E; vì thế tồn tại một đẳng cấu M ⊗_A E → E ánh xạ tích tenxơ ξ ⊗ x lên phần tử (γξ)x của E. Giả thiết l ⊗ x = 0 trong M ⊗_A E do đó suy ra γx = 0.

#### Nhận xét {#alg-ii-s7-n10-rem-2 .statement}

Cho α^{-1}φ(x), β^{-1}φ(y) là hai phần tử của E_{(K)}, với α ∈ A, β ∈ A, x ∈ E, y ∈ E, αβ ≠ 0. Để có α^{-1}φ(x) = β^{-1}φ(y), điều kiện cần và đủ là βx − αy là một phần tử xoắn của E, vì quan hệ này tương đương với βφ(x) = αφ(y), và cũng có thể viết là φ(βx − αy) = 0.

#### Hệ quả 1 {#alg-ii-s7-prop-26-cor-1 .statement}

*Nếu E là một A-môđun không xoắn, thì ánh xạ chính tắc* φ : E → E_{(K)} *là đơn ánh*.

Nhắc lại (§ 5, no. 1) rằng với mọi ánh xạ A-tuyến tính từ E vào một không gian vectơ F trên K, tồn tại duy nhất một ánh xạ K-tuyến tính $\vec{f} : E_{(K)} \to F$ sao cho $f = \vec{f} \circ \phi$; ta sẽ nói rằng $\vec{f}$ *liên kết* với $f$.

#### Hệ quả 2 {#alg-ii-s7-prop-26-cor-2 .statement}

*Cho f là một ánh xạ A-tuyến tính từ E vào một không gian vectơ F trên K; nếu Ker(f) ⊂ T(E), thì ánh xạ K-tuyến tính* $\vec{f}$ *liên kết với f là đơn ánh*.

Ta viết một phần tử của Ker($\vec{f}$) dưới dạng $\lambda^{-1}\phi(x)$, trong đó $\lambda \in A, \lambda \neq 0, x \in E$; hệ thức $\vec{f}(\lambda^{-1}\phi(x)) = 0$ tương đương với $\lambda^{-1}\vec{f}(\phi(x)) = 0$ trong F và vì thế với $f(x) = \vec{f}(\phi(x)) = 0$. Theo giả thiết, điều này kéo theo $x \in T(E)$ và do đó $\phi(x) = 0$, điều phải chứng minh.

#### Hệ quả 3 {#alg-ii-s7-prop-26-cor-3 .statement}

*Cho E là một A-môđun và g là một ánh xạ A-tuyến tính từ E vào một không gian vectơ F trên K sao cho g(E) sinh ra F và Ker(g) ⊂ T(E). Khi đó ánh xạ K-tuyến tính* $\bar{g}$ *liên kết với g là một đẳng cấu của* E_{(K)} *lên F*.

$\bar{g}$ là đơn ánh theo Hệ quả 2, và giả thiết rằng $g(E)$ sinh ra F kéo theo $\bar{g}$ là toàn ánh.

Với mọi A-môđun E, không gian vectơ E_{(K)} được gọi là *liên kết* với E. Với mọi tập con S của E, *hạng* của S trên K (hoặc, do lạm dụng ngôn ngữ, *hạng* của S) là hạng của ảnh chính tắc $\phi(S)$ của S trong E_{(K)}, nói cách khác (no. 2, Định nghĩa 1) là chiều trên K của không gian con vectơ của E_{(K)} được sinh bởi $\phi(S)$.

Khi E là một A-môđun *không xoắn*, người ta thường đồng nhất nó với ảnh chính tắc $\phi(E)$ của nó trong E_{(K)}. Với quy ước này, mọi hệ sinh của E đều chứa một *cơ sở* của E_{(K)} (no. 1, Định lý 2). Đặc biệt:

#### Hệ quả 4 {#alg-ii-s7-prop-26-cor-4 .statement}

*Mọi A-môđun hữu hạn sinh đều có hạng hữu hạn*.

Chú ý rằng đảo lại của hệ quả này không nhất thiết đúng; chẳng hạn $\mathbf{Q}$ là một $\mathbf{Z}$-môđun hạng 1 nhưng không sinh hữu hạn trên $\mathbf{Z}$.

Nhắc lại (§ 5, no. 1) rằng với mọi ánh xạ tuyến tính $f : E \to E'$ (trong đó $E$ và $E'$ là các $A$-môđun), $f_{(K)}$ ký hiệu ánh xạ $K$-tuyến tính $1_K \otimes f : E_{(K)} \to E'_{(K)}$.

#### Mệnh đề 27 {#alg-ii-s7-prop-27 .statement}

*Với mọi dãy khớp*

$$
E' \xrightarrow{f} E \xrightarrow{g} E''
$$

*của các ánh xạ $A$-tuyến tính, thì dãy tương ứng các ánh xạ $K$-tuyến tính*

$$
E'_{(K)} \xrightarrow{f_{(K)}} E_{(K)} \xrightarrow{g_{(K)}} E''_{(K)}
$$

*là khớp.*

Giả sử $g_{(K)}(\lambda^{-1} \otimes x) = 0$, với $\lambda \in A, \lambda \neq 0, x \in E$; điều này tương đương với $\lambda^{-1} \otimes g(x) = 0$ trong $E''_{(K)}$ và do đó cũng tương đương với

$$
1 \otimes g(x) = \lambda(\lambda^{-1} \otimes g(x)) = 0;
$$

theo Mệnh đề 26, tồn tại $\alpha \neq 0$ trong $A$ sao cho $\alpha g(x) = 0$ trong $E''$, hay cũng là $g(\alpha x) = 0$. Theo giả thiết, vì thế tồn tại một $x' \in E'$ sao cho $\alpha x = f(x')$ và do đó $\lambda^{-1} \otimes x = f_{(K)}(\alpha^{-1}\lambda^{-1} \otimes x')$, điều này chứng minh mệnh đề.

#### Hệ quả 1 {#alg-ii-s7-prop-27-cor-1 .statement}

*Nếu $E'$ là một môđun con của $E$, thì $E'_{(K)}$ được đồng nhất một cách chính tắc với một không gian con vectơ của $E_{(K)}$ và $(E/E')_{(K)}$ với $E_{(K)}/E'_{(K)}$.*

Chỉ cần áp dụng Mệnh đề 27 cho dãy khớp

$$
0 \to E' \to E \to E/E' \to 0.
$$

#### Hệ quả 2 {#alg-ii-s7-prop-27-cor-2 .statement}

*Với mọi ánh xạ $A$-tuyến tính $f : E \to F$, ta có $\operatorname{Ker}(f_{(K)}) = (\operatorname{Ker}(f))_{(K)}$, $\operatorname{Im}(f_{(K)}) = (\operatorname{Im}(f))_{(K)}$, $\operatorname{Coker}(f_{(K)}) = (\operatorname{Coker}(f))_{(K)}$ sai khác bởi các đẳng cấu chính tắc. Đặc biệt, để $f_{(K)}$ là đơn ánh (resp. toàn ánh, resp. không), điều kiện cần và đủ là $\operatorname{Ker}(f) \subset T(E)$ (resp. là $\operatorname{Coker}(f)$ là một môđun xoắn, resp. là $\operatorname{Im}(f) \subset T(F)$).*

Điều này suy ra từ Hệ quả 1 và Mệnh đề 26.

#### Hệ quả 3 {#alg-ii-s7-prop-27-cor-3 .statement}

*Cho $E$ là một $A$-môđun và $(x_\lambda)_{\lambda \in L}$ một họ các phần tử của $E$. Để $(x_\lambda)$ là một họ tự do, điều kiện cần và đủ là trong không gian $K$-vectơ $E_{(K)}$ họ $(1 \otimes x_\lambda)$ là tự do.*

Họ $(x_\lambda)$ xác định một ánh xạ $A$-tuyến tính $f : A^{(L)} \to E$ sao cho $f(e_\lambda) = x_\lambda$ với mọi $\lambda \in L$ ($(e_\lambda)$ là cơ sở chính tắc của $A^{(L)}$) và nói rằng $(x_\lambda)$ là tự do có nghĩa là $f$ là đơn ánh. Chỉ cần áp dụng Hệ quả 2 cho $f$, nhận thấy rằng $A^{(L)}$ là không có xoắn (Mệnh đề 25).

### Bài tập {#alg-ii-s7-exercises}

Xem [bài tập cho § 7](exercises/s7/).
