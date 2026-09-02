---
book: ac
book_title: Commutative Algebra
chapter: X
chapter_title: Profondeur, régularité, dualité
section: 1
section_title: Profondeur
lang: vi
source: ac-x-fr
book_pages: AC X.3-AC X.22
pdf_pages: 0002-0021, 0150-0153
extraction: ocr
subsections:
    - "no": 2
      title: Profondeur et acyclicité
      page: 4
      pdf_page: 3
    - "no": 3
      title: Profondeur et complexe de Koszul
      page: 5
      pdf_page: 4
    - "no": 4
      title: Profondeur et suites régulières
      page: 8
      pdf_page: 7
    - "no": 5
      title: Profondeur le long d’une partie fermée
      page: 0
      pdf_page: 9
    - "no": 6
      title: Profondeur des algèbres
      page: 11
      pdf_page: 10
    - "no": 7
      title: Majorations de la profondeur
      page: 13
      pdf_page: 12
    - "no": 8
      title: Anneaux noethériens localement intègres ; anneaux noethériens normaux
      page: 15
      pdf_page: 14
    - "no": 9
      title: Profondeur et connexité
      page: 0
      pdf_page: 15
    - "no": 10
      title: Profondeur et normalité
      page: 19
      pdf_page: 18
statements: 60
exercises: 18
content_sha256: 03bd9f6820271ba279dccfcd6bf31d42ec8e1811cefe4fff782d7f6774e8f59b
translated_from: content/en-mt/ac/X/01_s1_profondeur.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 45ce4aed8b702b2a4fc75c122b0bedf601f22162b148fd2e307422069f1eee3b
translation_model: gpt-5.4
translation_run: translate-vi-c5e1c906
glossary_version: 34
glossary_terms_sha256: 0635de4f4044dd8c02681e45193a8e81ca66e26bbfd58bbcf95b2b5af2192689
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 1. ĐỘ SÂU

#### Mệnh đề 1 {#ac-x-s1-prop-1 .statement}

Cho $A$ là một vành, $J$ là một iđêan của $A$ và $0 \to M' \to M \to M'' \to 0$ là một dãy khớp các $A$-môđun. Đặt

$$
p' = \operatorname{prof}(J; M') \quad , \quad p = \operatorname{prof}(J; M) \quad , \quad p'' = \operatorname{prof}(J; M'') .
$$

Khi đó rơi vào một trong ba trường hợp sau đây, loại trừ lẫn nhau:

$$
p' = p \leqslant p'' \quad , \quad p = p'' < p' \quad , \quad p'' = p' - 1 < p .
$$

Xét dãy khớp các môđun mở rộng liên kết với $A/J$ và với dãy khớp trên (A, X, p. 92, th. 2). Loại trừ trường hợp $p = p' = p'' = +\infty$; khi đó tồn tại trong dãy này một môđun khác không đầu tiên, và môđun tiếp theo nó cũng khác không. Điều này cho ba khả năng sau:

a) Môđun khác không đầu tiên là $\operatorname{Ext}_A^{p'}(A/J, M')$. Khi đó $p' = p \leqslant p''$.

b) Môđun khác không đầu tiên là $\operatorname{Ext}_A^p(A/J, M)$. Khi đó $p = p'' < p'$.

c) Môđun khác không đầu tiên là $\operatorname{Ext}_A^{p''}(A/J, M'')$. Khi đó $p'' + 1 = p' \leqslant p$.

#### Nhận xét 5 {#ac-x-s1-rem-5 .statement}

Giả sử rằng ta có $p = p'$ và đơn ánh $u : M' \to M$ xuất hiện trong dãy khớp của mệnh đề 1 thuộc $J \operatorname{Hom}_A(M', M)$. *Khi đó ta có* $p'' = p - 1$. Thật vậy, giả thiết kéo theo ánh xạ $\operatorname{Ext}_A^i(1_{A/J}, u)$ bằng không với mọi số nguyên $i$; điều này loại trừ trường hợp a) đã xét ở trên.

#### Mệnh đề 2 {#ac-x-s1-prop-2 .statement}

Cho $A$ là một vành, $J$ là một iđêan của $A$, $M$ là một $A$-môđun và $N$ là một $A$-môđun bị triệt tiêu bởi một lũy thừa của $J$. *Ta có* $\operatorname{Ext}_A^i(N, M) = 0$ *với mọi số nguyên* $i < \operatorname{prof}_A(J; M)$.

Trước hết giả sử $JN = 0$ và lập luận bằng quy nạp theo số nguyên $i < \operatorname{prof}_A(J; M)$. Mệnh đề là hiển nhiên khi $i < 0$. Xem $N$ như một $(A/J)$-môđun và chọn một dãy khớp các $(A/J)$-môđun

$$
0 \to K \longrightarrow (A/J)^{(I)} \longrightarrow N \to 0 .
$$

Từ đó suy ra một dãy khớp các môđun mở rộng

$$
\operatorname{Ext}_A^{i-1}(K, M) \longrightarrow \operatorname{Ext}_A^i(N, M) \longrightarrow \operatorname{Ext}_A^i((A/J)^{(I)}, M) .
$$

$A$-môđun $\operatorname{Ext}_A^{i-1}(K, M)$ bằng không theo giả thiết quy nạp, và $A$-môđun $\operatorname{Ext}_A^i((A/J)^{(I)}, M)$ đẳng cấu với $\operatorname{Ext}_A^i(A/J, M)^I$ (A, X, p. 89, prop. 7), môđun này bằng không theo định nghĩa của độ sâu. Do đó ta có $\operatorname{Ext}_A^i(N, M) = 0$.

Xét trường hợp tổng quát, và lập luận bằng quy nạp theo số nguyên nhỏ nhất $m > 0$ sao cho $J^m N = 0$. Ta vừa xét trường hợp $m = 1$. Giả sử $m > 1$ và cho $i < \operatorname{prof}_A(J; M)$ là một số nguyên. Xét dãy khớp

$$
\operatorname{Ext}_A^i(N/JN, M) \longrightarrow \operatorname{Ext}_A^i(N, M) \longrightarrow \operatorname{Ext}_A^i(JN, M)
$$

suy ra từ dãy khớp $0 \to JN \to N \to N/JN \to 0$. Hai môđun ở hai đầu bằng không theo giả thiết quy nạp, vì $N/JN$ và $JN$ bị triệt tiêu bởi $J^{m-1}$. Vậy ta có $\operatorname{Ext}_A^i(N, M) = 0$, đúng như phải chứng minh.

#### Hệ quả 1 {#ac-x-s1-prop-2-cor-1 .statement}

Cho m là một số nguyên > 0 và cho J' là một iđêan của A chứa J^m. Ta có prof_A(J ; M) \leq prof_A(J' ; M).

Thật vậy J^m triệt tiêu A-môđun A/J', nên Ext^i_A(A/J', M) bằng không với mọi số nguyên i < prof_A(J ; M) (mệnh đề 2).

#### Hệ quả 2 {#ac-x-s1-prop-2-cor-2 .statement}

Giả sử iđêan J là hữu hạn sinh, và cho J' là một iđêan của A sao cho V(J) \supset V(J').

a) Ta có prof_A(J ; M) \leq prof_A(J' ; M).

b) Nếu iđêan J' là hữu hạn sinh và nếu V(J) = V(J'), thì ta có prof_A(J ; M) = prof_A(J' ; M).

Theo II, § 4, No. 3, cor. 2 of prop. 11 và § 2, No. 6, prop. 15, tồn tại một số nguyên m > 0 sao cho J^m \subset J'. Mệnh đề a) do đó suy ra từ hệ quả 1 và mệnh đề b) được suy ra từ đó.

Hệ quả 2 có thể sai khi iđêan J không hữu hạn sinh (bài tập 2).

### 2. Độ sâu và tính không đồng điều

#### Mệnh đề 3 {#ac-x-s1-prop-3 .statement}

Cho A là một vành, C là một phức các A-môđun bị chặn về bên trái và p là một số nguyên. Giả sử rằng với mọi cặp số nguyên (m, n) sao cho m \geq n \geq p, độ sâu của A-môđun C_m đối với linh hóa tử của H_n(C) là > m - n. Khi đó ta có H_n(C) = 0 với n \geq p.

Vì C bị chặn về bên trái nên H_n(C) bằng không với n đủ lớn. Nếu kết luận là sai, sẽ tồn tại một số nguyên q \geq p sao cho H_n(C) = 0 với n > q và H_q(C) \neq 0. Ký hiệu bởi J linh hóa tử của H_q(C); khi đó ta có prof_A(J ; H_q(C)) = 0. Hơn nữa, vì Z_q(C) là một môđun con của C_q, và vì theo giả thiết ta có prof_A(J ; C_q) > q - q = 0, nên ta có prof_A(J ; Z_q(C)) > 0. Khi đó từ dãy khớp

$$
0 \to B_q(C) \to Z_q(C) \to H_q(C) \to 0
$$

suy ra đẳng thức prof_A(J ; B_q(C)) = 1 (No. 1, prop. 1). Theo định nghĩa của q, B_n(C) bằng Z_n(C) với mọi số nguyên n > q. Từ các dãy khớp chính tắc

$$
0 \to B_n(C) \to C_n \to B_{n-1}(C) \to 0 \quad (n > q)
$$

và từ giả thiết prof_A(J ; C_n) > n - q, ta thu được bằng quy nạp đẳng thức prof_A(J ; B_n(C)) = n - q + 1 với mọi n \geq q (loc. cit.). Nhưng điều này vô lý vì B_n(C) bằng không với n đủ lớn.

#### Hệ quả 1 {#ac-x-s1-prop-3-cor-1 .statement}

Cho A là một vành, J là một iđêan của A, C là một phức các A-môđun bị chặn về bên trái và p là một số nguyên. Giả sử rằng ta có JH_m(C) = 0 và prof_A(J ; C_m) > m - p với m \geq p. Khi đó ta có H_n(C) = 0 với n \geq p.

Thật vậy với n \geq p, linh hóa tử J_n của H_n(C) chứa J, nên ta có prof_A(J_n ; C_m) \geq prof_A(J ; C_m) (No. 1, cor. 1 of prop. 2), vì thế giả thiết của mệnh đề được thỏa mãn.

#### Hệ quả 2 {#ac-x-s1-prop-3-cor-2 .statement}

Cho $A$ là một vành địa phương, $C$ là một phức các $A$-môđun bị chặn về bên trái, $p$ là một số nguyên. Giả sử rằng với $m \geq p$, $H_m(C)$ có độ dài hữu hạn và $C_m$ có độ sâu $> m - p$. Khi đó $H_n(C) = 0$ với $n \geq p$.

$A$-môđun $\bigoplus_{m \geq p} H_m(C)$ có độ dài hữu hạn. Gọi $J$ là linh hóa tử của nó; theo A, VIII, § 1, No. 3, hệ quả, vành $A/J$ là Artin, do đó $J$ chứa một lũy thừa của iđêan cực đại của $A$ (A, VIII, § 10, No. 1, định lý 1). Suy ra $\operatorname{prof}_A(J; C_m) \geq \operatorname{prof}(C_m) > m - p$ với $m \geq p$ (No. 1, hệ quả 1 của mệnh đề 2), nên có thể áp dụng hệ quả 1.

### 3. Độ sâu và phức Koszul

Cho $A$ là một vành, $M$ là một $A$-môđun, $x = (x_i)_{i \in I}$ là một họ các phần tử của $A$. Gọi $u : A^{(I)} \to A$ là dạng tuyến tính sao cho $u(e_i) = x_i$ với mọi $i \in I$, và $K^\bullet(x, M)$ là phức $K_A^\bullet(u, M)$ liên kết với $u$ (A, X, p. 147). Ta có $K^p(x, M) = 0$ với $p < 0$; với $p \geq 0$ thì $A$-môđun $K^p(x, M) = \operatorname{Hom}_A(\Lambda^p(A^{(I)}), M)$ được đồng nhất một cách chính tắc với $A$-môđun $C_I^p(M)$ tạo bởi các ánh xạ phản xứng từ $I^p$ vào $M$ (A, X, p. 153), vi phân $\partial^p : K^p(x, M) \to K^{p+1}(x, M)$ được cho bởi công thức

$$
(\partial^p m)(\alpha_1, \ldots, \alpha_{p+1}) = \sum_{j=1}^{p+1} (-1)^{j+1} x_{\alpha_j} m(\alpha_1, \ldots, \alpha_{j-1}, \alpha_{j+1}, \ldots, \alpha_{p+1})
$$

với $m \in K^p(x, M)$ và $(\alpha_1, \ldots, \alpha_{p+1}) \in I^{p+1}$ (A, X, p. 154, công thức (12)). Đặc biệt suy ra rằng phức $K^\bullet(x, M)$ chỉ phụ thuộc vào cấu trúc của $M$ như một $\mathbf{Z}$-môđun và vào các nội tự đồng cấu $(x_i)_M$.

Ta ký hiệu bởi $H^\bullet(x, M)$ đồng điều của phức $K^\bullet(x, M)$. $A$-môđun $H^0(x, M)$ được đồng nhất với $\operatorname{Hom}_A(A/J, M)$, trong đó $J$ là iđêan của $A$ sinh bởi các $x_i$ (A, X, p. 147, bổ đề 1).

Cho $(M_\alpha)_{\alpha \in K}$ là một họ các $A$-môđun, và $M$ là tích của chúng; phức $K^\bullet(x, M)$ đẳng cấu chính tắc với phức tích của các $K^\bullet(x, M_\alpha)$, sao cho với mỗi số nguyên $s$ thì $A$-môđun $H^s(x, M)$ được đồng nhất với tích của các $H^s(x, M_\alpha)$ (A, X, p. 28, Mệnh đề 1).

#### Định lý 1 {#ac-x-s1-thm-1 .statement}

Cho $A$ là một vành, $J$ một iđêan của $A$, $x = (x_i)_{i \in I}$ một họ sinh của $J$, $M$ một $A$-môđun. Độ sâu của $M$ đối với $J$ là cận dưới lớn nhất (trong $\mathbf{N} \cup \{+\infty\}$) của các số nguyên $n$ sao cho $H^n(x, M) \neq 0$.

Đặt $p = \operatorname{prof}_A(J; M)$. Xét phức $K^\bullet(x, M)$. Đồng điều của nó bị triệt tiêu bởi $J$ (A, X, p. 148, Hệ quả 2), và độ sâu đối với $J$ của mỗi môđun $K^i(x, M)$ bằng $p$ hoặc $+\infty$ (No. 1, Nhận xét 4). Khi đó từ Hệ quả 1 của No. 2 suy ra rằng $H^i(x, M) = 0$ với $i < p$. Còn phải chứng minh rằng $H^p(x, M)$ khác không khi $p < +\infty$.

Trường hợp $p = 0$ là hiển nhiên, giả sử $0 < p < +\infty$ và $H^p(x, M) = 0$. Cho $L$ là một phân giải tự do của $A$-môđun $A/J$; ký hiệu $C$ là phức $\operatorname{Homgr}_A(L, M)$. $A$-môđun $H^i(C)$ đẳng cấu với $\operatorname{Ext}_A^i(A/J, M)$ (A, X, p. 100, Định lý 1); do đó nó bằng không với $i < p$. Khi đó với $i < p$ ta có các dãy khớp chính tắc

$$
0 \to B^i(C) \to C^i \to B^{i+1}(C) \to 0 .
$$

$A$-môđun $C^i$ là một tích của các $A$-môđun đẳng cấu với $M$; do đó $H^s(x, C^i) = 0$ với $s \leq p$. Từ các dãy khớp ở trên và từ A, X, p. 150, suy ra rằng đồng cấu nối $\partial^s : H^s(x, B^{i+1}(C)) \longrightarrow H^{s+1}(x, B^i(C))$ là đơn ánh với $s \leq p$ và $i < p$; vì $B^0(C) = 0$, suy ra $H^{p-i}(x, B^{i+1}(C))$ bằng không với $i < p$. Đặc biệt, ta có $H^1(x, B^p(C)) = 0$, do đó dãy khớp

$$
0 \to B^p(C) \to Z^p(C) \to H^p(C) \to 0
$$

suy ra một toàn cấu $H^0(x, Z^p(C)) \longrightarrow H^0(x, H^p(C))$. Vì $H^p(C)$ đẳng cấu với $\operatorname{Ext}_A^p(A/J, M)$, môđun này khác không và bị J triệt tiêu, nên ta có $H^0(x, H^p(C)) \neq 0$, do đó $H^0(x, Z^p(C)) \neq 0$ và vì thế $H^0(x, C^p) \neq 0$. Nhưng điều này kéo theo $H^0(x, M) \neq 0$, trái với giả thiết. Vậy $H^p(x, M) \neq 0$, điều này hoàn tất chứng minh.

#### Hệ quả 1 {#ac-x-s1-thm-1-cor-1 .statement}

*Giả sử iđêan J là kiểu hữu hạn và JM $\neq$ M. Khi đó* $\operatorname{prof}_A(J; M)$ *là hữu hạn và $\leq$ Card(I)* ; *để có đẳng thức với Card(I), điều kiện cần và đủ là họ x là hoàn toàn cát tuyến đối với M* (A, X, p. 157, Định nghĩa 2).

Trước hết giả sử I là hữu hạn, và ký hiệu r là lực lượng của nó. A-môđun $H^r(x, M)$ đẳng cấu chính tắc với $H_0(x, M)$, mà chính nó lại đẳng cấu với $M/JM$ (A, X, p. 155); do đó bất đẳng thức $\operatorname{prof}_A(J; M) \leq r$ suy ra từ Định lý 1. Để có đẳng thức, điều kiện cần và đủ là A-môđun $H^i(x, M)$ bằng không với $i < r$, điều này có nghĩa là họ x hoàn toàn cát tuyến đối với M (A, X, p. 157).

Từ những điều vừa nói, $\operatorname{prof}_A(J; M)$ là hữu hạn; còn phải chứng minh rằng nếu họ x hoàn toàn cát tuyến đối với M thì tập hợp I là hữu hạn. Bây giờ điều kiện $H_1(x, M) = 0$ (A, X, p. 157, Định nghĩa 2) suy ra rằng ta có một dãy khớp

$$
\Lambda^2(A^{(I)}) \otimes_A M \xrightarrow{\partial_2} M^{(I)} \xrightarrow{\partial_1} JM \to 0 ,
$$

trong đó ảnh của $\partial_2$ được chứa trong $JM^{(I)}$. Bằng cách lấy tích tenxơ với $A/J$, từ đó suy ra một đẳng cấu A-tuyến tính từ $(M/JM)^{(I)}$ lên $JM/J^2M$. Mà môđun sau là kiểu hữu hạn, vì J và M đều như vậy; do $M/JM$ khác không, suy ra tập hợp I là hữu hạn.

#### Hệ quả 2 {#ac-x-s1-thm-1-cor-2 .statement}

*Cho A là một vành địa phương, J một iđêan kiểu hữu hạn của A khác A, M một A-môđun khác không kiểu hữu hạn. Đặt* $r = [J/m_AJ : \kappa_A]$. *Ta có* $\operatorname{prof}_A(J; M) \leq r$ ; *có đẳng thức khi và chỉ khi J được sinh bởi một họ hoàn toàn cát tuyến đối với M. Trong trường hợp đó, để một họ sinh của J là hoàn toàn cát tuyến, điều kiện cần và đủ là nó có r phần tử*.

Theo bổ đề Nakayama, ta có $JM \neq M$, và r là số cực tiểu các phần tử sinh của J; do đó Hệ quả 2 suy ra từ Hệ quả 1.

#### Mệnh đề 4 {#ac-x-s1-prop-4 .statement}

Cho $\rho : A \to B$ là một đồng cấu vành, $J$ một iđêan của $A$ và $N$ một $B$-môđun. Ta có đẳng thức $\operatorname{prof}_A(J; N) = \operatorname{prof}_B(JB; N)$.

Cho $x = (x_i)_{i \in I}$ là một họ sinh của $J$; họ $\rho(x) = (\rho(x_i))_{i \in I}$ sinh ra $JB$. Theo phép dựng, phức $K^\bullet(\rho(x), N)$ bằng $K^\bullet(x, N)$. Do đó mệnh đề suy ra từ Định lý 1.

#### Hệ quả {#ac-x-s1-n3-cor-1 .statement}

Cho $A$ là một vành địa phương, $a$ một iđêan của $A$ khác $A$ và $M$ một $A$-môđun bị $a$ triệt tiêu. Ta có $\operatorname{prof}_A(M) = \operatorname{prof}_{A/a}(M)$.

Cho $\rho : A \to B$ là một đồng cấu vành, $x = (x_i)_{i \in I}$ một họ hữu hạn các phần tử của $A$ và $M$ một $A$-môđun. Với mọi số nguyên $p$, ký hiệu $u^p : B \otimes_A C_I^p(M) \to C_I^p(B \otimes_A M)$ là đồng cấu $B$-tuyến tính gán cho $b \otimes m$ ánh xạ phản xứng $(\alpha_1, \ldots, \alpha_p) \mapsto b \otimes m(\alpha_1, \ldots, \alpha_p)$. Họ $(u^p)$ xác định một đẳng cấu các phức

$$
u : B \otimes_A K^\bullet(x, M) \to K^\bullet(x, B \otimes_A M)
$$

Xét đồng cấu chính tắc

$$
\gamma^p(B, K^\bullet(x, M)) : B \otimes_A H^p(x, M) \to H^p(B \otimes_A K^\bullet(x, M))
$$

(A, X, p. 62); bằng cách hợp thành với $H^p(u)$, ta suy ra từ đó một đồng cấu

$$
v^p : B \otimes_A H^p(x, M) \to H^p(x, B \otimes_A M)
$$

#### Bổ đề 1 {#ac-x-s1-lem-1 .statement}

Nếu $A$-môđun $B$ là phẳng, thì đồng cấu $v^p$ là song ánh với mọi số nguyên $p$.

Điều này suy ra từ A, X, p. 66, Hệ quả 2.

#### Mệnh đề 5 {#ac-x-s1-prop-5 .statement}

Cho $A$ là một vành, $J$ là một iđêan kiểu hữu hạn của $A$ và $M$ là một $A$-môđun. Ký hiệu $\Omega$ là tập hợp các iđêan cực đại của $A$ thuộc $\operatorname{Supp}(M)$ và chứa $J$. Khi đó

$$
\operatorname{prof}_A(J; M) = \inf_{p \in \operatorname{Spec}(A)} \operatorname{prof}_{A_p}(J_p; M_p) = \inf_{m \in \Omega} \operatorname{prof}_{A_m}(J_m; M_m)
$$

Cho $x = (x_i)_{i \in I}$ là một họ sinh hữu hạn của $J$. Cho $p$ là một iđêan nguyên tố của $A$; iđêan $J_p$ được sinh bởi ảnh $x_p$ của họ $(x_i)$ trong $A_p$. Với mọi $p \geq 0$, $A_p$-môđun $(H^p(x, M))_p$ đẳng cấu với $H^p(x_p, M_p)$ (Bổ đề 1); do đó, theo Định lý 1, ta có $\operatorname{prof}_A(J; M) \leq \inf_{p \in \operatorname{Spec}(A)} \operatorname{prof}_{A_p}(J_p; M_p) \leq \inf_{m \in \Omega} \operatorname{prof}_{A_m}(J_m; M_m)$.

Cho $p$ là một số nguyên nhỏ hơn $\operatorname{prof}_{A_m}(JA_m; M_m)$ với mọi $m \in \Omega$. Khi đó $H^p(x_m, M_m) = 0$ với mọi iđêan cực đại $m$ của $A$: điều này suy ra từ Định lý 1 nếu $m \in \Omega$, từ việc $M_m = 0$ nếu $m \not\in \operatorname{Supp}(M)$, và từ việc iđêan $JA_m$, vốn triệt tiêu $H^p(x_m, M_m)$ (A, X, p. 148, Hệ quả 2), bằng $A_m$ nếu $m \not\in V(J)$. Do đó $(H^p(x, M))_m = 0$ với mọi iđêan cực đại $m$ của $A$, kéo theo $H^p(x, M) = 0$ (II, § 3, No. 3, Hệ quả 2 của Định lý 1). Mệnh đề được suy ra từ Định lý 1.

#### Mệnh đề 6 {#ac-x-s1-prop-6 .statement}

Cho $A$ là một vành, $J$ là một iđêan kiểu hữu hạn của $A$ và $M$ là một $A$-môđun. Cho $B$ là một vành và $\rho : A \to B$ là một đồng cấu vành biến $B$ thành một $A$-môđun phẳng.

a) Ta có $\operatorname{prof}_A(J; M) \leq \operatorname{prof}_B(JB; B \otimes_A M)$.

b) Giả sử thêm rằng mọi iđêan cực đại của $\operatorname{Supp}(M)$ chứa $J$ đều thuộc ảnh của ánh xạ chính tắc $\operatorname{Spec}(B) \to \operatorname{Spec}(A)$. Khi đó ta có $\operatorname{prof}_A(J; M) = \operatorname{prof}_B(JB; B \otimes_A M)$. Đây là trường hợp, chẳng hạn, nếu A-môđun $B$ là phẳng trung thành.

Mệnh đề a) suy ra từ Định lý 1 và Bổ đề 1.

Cho $p$ là một số nguyên nhỏ hơn nghiêm ngặt $\operatorname{prof}_B(JB; B \otimes_A M)$, và cho $m$ là một iđêan cực đại của $A$ thuộc $\operatorname{Supp}(M) \cap V(J)$. Cho $x$ là một họ sinh hữu hạn của iđêan $J$. Theo giả thiết của b), tồn tại một iđêan nguyên tố $n$ của $B$ nằm trên $m$, và ta có một đẳng cấu chính tắc

$$
B_n \otimes_{A_m} (A_m \otimes_A H^p(x, M)) \longrightarrow B_n \otimes_B (B \otimes_A H^p(x, M))
$$

Bây giờ $B \otimes_A H^p(x, M)$ đẳng cấu với $H^p(\rho(x), B \otimes_A M)$ (Bổ đề 1), do đó bằng không; hơn nữa $B_n$ là phẳng trung thành trên $A_m$ (I, § 3, No. 5, Proposition 9 and II, § 3, No. 4, Proposition 14 and Remark). Do đó ta có $A_m \otimes_A H^p(x, M) = 0$ và vì vậy $p < \operatorname{prof}_{A_m}(J_m; M_m)$ (Bổ đề 1 và Định lý 1). Mệnh đề thứ nhất của b) khi đó suy ra từ Mệnh đề 5; mệnh đề thứ hai suy ra từ I, § 3, No. 5, Proposition 9).

#### Hệ quả {#ac-x-s1-n3-cor-2 .statement}

Cho $A$ là một vành Noether, $J$ là một iđêan của $A$, $M$ là một A-môđun sinh hữu hạn, $\widehat{A}$ và $\widehat{M}$ là các hoàn thành tách của $A$ và $M$ đối với tôpô $J$-adic. Khi đó ta có $\operatorname{prof}_A(J; M) = \operatorname{prof}_{\widehat{A}}(J\widehat{A}; \widehat{M})$.

Thật vậy, A-môđun $\widehat{A}$ là phẳng và $\widehat{A}$-môđun $\widehat{M}$ đẳng cấu với $\widehat{A} \otimes_A M$ (III, § 3, No. 4, Định lý 3); hơn nữa, mọi iđêan cực đại của $A$ chứa $J$ đều thuộc ảnh của ánh xạ $\operatorname{Spec}(\widehat{A}) \to \operatorname{Spec}(A)$ (*loc. cit.*, Mệnh đề 8).

### 4. Độ sâu và các dãy chính quy

Cho $A$ là một vành, $M$ là một $A$-môđun. Nhớ lại (A, X, p. 158) rằng một dãy hữu hạn $(x_1, \ldots, x_r)$ các phần tử của $A$ được gọi là *chính quy đối với $M$* hay *$M$-chính quy* nếu, với $i = 1, \ldots, r$, phép vị tự tỉ số $x_i$ trong $A$-môđun $M/(x_1 M + \ldots + x_{i-1} M)$ là đơn ánh. Cho $(x_1, \ldots, x_r)$ là một dãy $M$-chính quy; với mọi $A$-môđun phẳng $N$, dãy $(x_1, \ldots, x_r)$ là chính quy đối với $M \otimes_A N$. Nếu $\rho : A \to B$ là một đồng cấu vành biến $B$ thành một $A$-môđun phẳng, thì dãy $(\rho(x_1), \ldots, \rho(x_r))$ là chính quy đối với $B$-môđun $B \otimes_A M$. Đặc biệt, với mọi iđêan nguyên tố $p$ của $A$, ảnh trong $A_p$ của dãy $(x_1, \ldots, x_r)$ là $M_p$-chính quy.

Trong phần sau, ta sẽ chủ yếu xét khái niệm một dãy $M$-chính quy trong trường hợp vành $A$ là địa phương Noether, môđun $M$ là sinh hữu hạn và các phần tử của dãy thuộc $m_A$; khi đó khái niệm dãy $M$-chính quy trùng với khái niệm dãy hoàn toàn cát tuyến đối với $M$ (A, X, p. 160, hệ quả 1).

#### Mệnh đề 7 {#ac-x-s1-prop-7 .statement}

Cho $A$ là một vành, $J$ là một iđêan của $A$, $M$ là một $A$-môđun, và $(x_1, \ldots, x_r)$ là một dãy $M$-chính quy gồm các phần tử của $J$. Khi đó
$$
\operatorname{prof}_A(J; M) = r + \operatorname{prof}_A(J; M/(x_1M + \ldots + x_rM))
$$
và đặc biệt $\operatorname{prof}_A(J; M) \geqslant r$.

Trường hợp $r = 1$ suy ra từ Nhận xét 5 của No. 1, áp dụng cho dãy khớp
$$
0 \to M \xrightarrow{(x_1)_M} M \longrightarrow M/x_1M \to 0 .
$$
Trường hợp tổng quát suy ra bằng quy nạp theo $r$.

#### Định lý 2 {#ac-x-s1-thm-2 .statement}

Cho $A$ là một vành Noether, $J$ là một iđêan của $A$ và $M$ là một $A$-môđun sinh hữu hạn.

a) Giả sử rằng $\operatorname{prof}_A(J; M)$ là hữu hạn. Khi đó mọi dãy $M$-chính quy gồm các phần tử của $J$ đều có thể được bổ sung thành một dãy $M$-chính quy có độ dài $\operatorname{prof}_A(J; M)$ gồm các phần tử của $J$.

b) Độ sâu của $M$ đối với $J$ là cận trên bé nhất của các độ dài của những dãy $M$-chính quy tạo thành từ các phần tử của $J$.

c) Để $\operatorname{prof}_A(J; M)$ là hữu hạn, điều kiện cần và đủ là giá của $M$ cắt $V(J)$, hay cũng vậy, là có $JM \neq M$.

Cho $(x_1, \ldots, x_r)$ là một dãy $M$-chính quy gồm các phần tử của $J$. Ta có $r \leqslant \operatorname{prof}_A(J; M)$ (Mệnh đề 7); giả sử rằng bất đẳng thức này là ngặt. Gọi $N$ là A-môđun $M/(x_1M + \ldots + x_rM)$. Ta có $\operatorname{prof}_A(J; N) > 0$ (*loc. cit.*), nên tồn tại một phần tử $x$ của $J$ sao cho phép vị tự $x_N$ là đơn ánh (No. 1, Nhận xét 2), nghĩa là sao cho dãy $(x_1, \ldots, x_r, x)$ là $M$-chính quy. Suy ra bằng quy nạp rằng với mọi số nguyên $s$ sao cho $r \leqslant s \leqslant \operatorname{prof}_A(J; M)$, dãy $(x_1, \ldots, x_r)$ có thể được bổ sung thành một dãy $M$-chính quy có độ dài $s$, điều này kéo theo các mệnh đề a) và b). Mệnh đề c) suy ra từ Nhận xét 1 của No. 1 và Hệ quả 1 của Định lý 1 của No. 3.

#### Hệ quả 1 {#ac-x-s1-thm-2-cor-1 .statement}

Với mọi dãy $M$-chính quy $(x_1, \ldots, x_r)$ gồm các phần tử của $J$, các tính chất sau là tương đương:

(i) ta có $r = \operatorname{prof}_A(J; M)$ ;
(ii) dãy $(x_1, \ldots, x_r)$ là cực đại trong số các dãy $M$-chính quy tạo thành từ các phần tử của $J$ ;
(iii) A-môđun $M/(x_1M + \ldots + x_rM)$ có một phần tử khác không bị triệt tiêu bởi $J$ ;
(iv) ta có $\operatorname{Ass}(M/(x_1M + \ldots + x_rM)) \cap V(J) \neq \varnothing$.

Tính tương đương của (i) và (ii) suy ra từ Định lý 2; tính tương đương của (ii), (iii) và (iv) suy ra từ Nhận xét 2 của No. 1 áp dụng cho A-môđun $M/(x_1M + \ldots + x_rM)$.

#### Hệ quả 2 {#ac-x-s1-thm-2-cor-2 .statement}

Cho $A$ là một vành địa phương Noether, $M$ là một A-môđun hữu hạn sinh khác không. Ta có
$$
\operatorname{prof}_A(M) \leqslant \dim_A(M) < +\infty .
$$

### 5. Độ sâu dọc theo một tập con đóng

Cho A là một vành Noether, F là một tập con đóng của $\mathrm{Spec}(A)$ và M là một A-môđun. Theo Hệ quả 2 của Mệnh đề 2 của No. 1, phần tử $\mathrm{prof}_A(J;M)$ của $\mathbf{N} \cup \{+\infty\}$ không phụ thuộc vào iđêan J của A sao cho $F = V(J)$; nó được gọi là *độ sâu của M dọc theo F* và được ký hiệu là $\mathrm{prof}_F(M)$.

#### Nhận xét 1 {#ac-x-s1-n5-rem-1 .statement}

Cho r là một số nguyên. Theo Mệnh đề 2 của No. 1 và II, § 4, No. 4, Hệ quả 2 của Mệnh đề 17, bất đẳng thức $\mathrm{prof}_F(M) \geqslant r$ tương đương với tính chất sau: với mọi A-môđun hữu hạn sinh N mà giá được chứa trong F, ta có $\mathrm{Ext}_A^i(N,M) = 0$ với $i < r$.

#### Nhận xét 2 {#ac-x-s1-n5-rem-2 .statement}

Giả sử rằng A-môđun M là hữu hạn sinh. Theo Nhận xét 2 của No. 1 và Định lý 2 của No. 4, ta có các tương đương sau

$$
\mathrm{prof}_F(M) = 0 \iff \mathrm{Ass}(M) \cap F \neq \varnothing \\
\mathrm{prof}_F(M) < +\infty \iff \mathrm{Supp}(M) \cap F \neq \varnothing .
$$

#### Mệnh đề 8 {#ac-x-s1-prop-8 .statement}

*Cho A là một vành Noether, F là một tập con đóng của $\mathrm{Spec}(A)$, và M là một A-môđun hữu hạn sinh. Ta có*

$$
\mathrm{prof}_F(M) = \inf_{p \in F} \mathrm{prof}_{A_p}(M_p) = \inf_{p \in \mathrm{Supp}(M) \cap F} \mathrm{prof}_{A_p}(M_p) .
$$

Điều này là hiển nhiên nếu $\mathrm{prof}_F(M) = +\infty$ (Nhận xét 2). Nếu $\mathrm{prof}_F(M) = 0$, tồn tại một iđêan nguyên tố $p \in \mathrm{Ass}(M) \cap F$ (Nhận xét 2); ta có $pA_p \in \mathrm{Ass}(M_p)$ (IV, § 1, No. 2, Mệnh đề 5), nên $\mathrm{prof}_{A_p}(M_p) = 0$ (Nhận xét 2 của No. 1), do đó có mệnh đề trong trường hợp này.

Giả sử $0 < \mathrm{prof}_F(M) < +\infty$; cho J là một iđêan của A sao cho $V(J) = F$, và cho x là một phần tử của J sao cho phép vị tự $x_M$ là đơn ánh (*loc. cit.*). Với mỗi iđêan nguyên tố p, phép vị tự $x_{M_p}$ là đơn ánh. Theo Mệnh đề 7 của No. 4, do đó ta có

$$
\mathrm{prof}_F(M/xM) = \mathrm{prof}_F(M) - 1 \\
\mathrm{prof}_{A_p}((M/xM)_p) = \mathrm{prof}_{A_p}(M_p) - 1 .
$$

Khi đó suy ra kết luận bằng quy nạp theo số nguyên $\mathrm{prof}_F(M)$.

#### Nhận xét 3 {#ac-x-s1-n5-rem-3 .statement}

Nếu q là một điểm của $\mathrm{Supp}(M)$, do đó ta có $\mathrm{prof}_A(q;M) = \inf_{p \supseteq q} \mathrm{prof}_{A_p}(M_p)$. Đặc biệt, ta có bất đẳng thức $\mathrm{prof}_A(q;M) \leqslant \mathrm{prof}_{A_q}(M_q)$; có đẳng thức khi q là cực đại. Trong trường hợp tổng quát, có thể có $\mathrm{prof}_A(q;M) < \mathrm{prof}_{A_q}(M_q)$; cũng có thể có $\mathrm{prof}_A(q;M) < \inf \mathrm{prof}_{A_m}(M_m)$ trong đó m chạy qua tập hợp các iđêan cực đại của A chứa q. Chẳng hạn, cho p là một iđêan nguyên tố không cực đại của A, chứa q và phân biệt với q; đặt $M = A/p$. Ta có $\mathrm{prof}_A(q;M) = 0$, $\mathrm{prof}_{A_q}(M_q) = +\infty$ và $\mathrm{prof}_{A_m}(M_m) > 0$ với mọi iđêan cực đại m của A.

#### Mệnh đề 9 {#ac-x-s1-prop-9 .statement}

Cho $A$ là một vành Noether, $M$ và $N$ là hai A-môđun kiểu hữu hạn, và $F$ là giá của $N$. Khi đó $\mathrm{prof}_F(M)$ là cận dưới lớn nhất (trong $N \cup \{+\infty\}$) của tập hợp các số nguyên $n$ sao cho $\mathrm{Ext}_A^n(N, M) \neq 0$.

Theo Nhận xét 1, ta có $\mathrm{Ext}_A^i(N, M) = 0$ với mọi $i < \mathrm{prof}_F(M)$. Còn phải chứng minh rằng nếu $\mathrm{prof}_F(M) = n < +\infty$, thì $\mathrm{Ext}_A^n(N, M) \neq 0$. Cho $J$ là linh hóa tử của $N$; ta có $F = V(J)$, do đó $\mathrm{prof}_F(M) = \mathrm{prof}_A(J; M)$. Theo Hệ quả 1 của Định lý 2 (No. 4), tồn tại một dãy $M$-chính quy $(x_1, \ldots, x_n)$ có độ dài $n$ gồm các phần tử của $J$, và độ sâu đối với $J$ của A-môđun $\overline{M} = M/(x_1 M + \ldots + x_n M)$ bằng không. Theo A, X, p. 166, Mệnh đề 9, chỉ cần chứng minh rằng $\mathrm{Hom}_A(N, \overline{M})$ là khác không. Bây giờ, theo Mệnh đề 8, tồn tại $p \in \mathrm{Supp}(M) \cap \mathrm{Supp}(N)$ sao cho $\mathrm{prof}_{A_p}(\overline{M}_p) = 0$, nghĩa là $\mathrm{Hom}_{A_p}(\kappa(p), \overline{M}_p) \neq 0$. Vì $N_p$ là khác không, không gian vectơ $\kappa(p)$ $N_p \otimes_{A_p} \kappa(p)$ là khác không (bổ đề Nakayama), và đối ngẫu của nó cũng vậy; do đó tồn tại một ánh xạ tuyến tính $A_p$-tuyến tính toàn ánh từ $N_p$ lên trên $\kappa(p)$. Suy ra ta có $\mathrm{Hom}_{A_p}(N_p, \overline{M}_p) \neq 0$, do đó $\mathrm{Hom}_A(N, \overline{M}) \neq 0$ (II, § 2, No. 7, Mệnh đề 19), điều phải chứng minh.

#### Nhận xét 4 {#ac-x-s1-n5-rem-4 .statement}

Cho $A$ là một vành Noether, $N$ là một A-môđun sinh hữu hạn. Cận dưới lớn nhất trong $N \cup \{+\infty\}$ của tập hợp các số nguyên $n$ sao cho $\mathrm{Ext}_A^n(N, A)$ khác không đôi khi được gọi là cấp của $N$, và được ký hiệu là grade$(N)$. Theo Mệnh đề 9, đó cũng là độ sâu của $A$ dọc theo giá đỡ của $N$, hoặc còn là cận trên nhỏ nhất của tập hợp các độ dài của các dãy $A$-chính quy gồm các phần tử của linh hóa tử của $N$ (No. 4, Định lý 2). Vì với mọi iđêan nguyên tố $p$ của $A$, linh hóa tử của $N_p$ bằng $\mathrm{Ann}(N)_p$ (II, § 2, No. 4, công thức (9)), từ Mệnh đề 5 của No. 3 ta suy ra đẳng thức

$$
\mathrm{grade}(N) = \inf_{p \in \mathrm{Spec}(A)} \mathrm{grade}(N_p) = \inf_{m \in \Omega} \mathrm{grade}(N_m),
$$

trong đó $\Omega$ ký hiệu tập hợp các iđêan cực đại của $A$.

### 6. Độ sâu của các đại số

#### Bổ đề 2 {#ac-x-s1-lem-2 .statement}

Cho $\rho : A \to B$ là một đồng cấu địa phương của các vành địa phương Noether, $N$ là một B-môđun sinh hữu hạn và $y$ là một phần tử của $m_B$. Hai điều kiện sau là tương đương:

(i) A-môđun $N/yN$ là phẳng và phép vị tự $y_N$ là đơn ánh;
(ii) A-môđun $N$ là phẳng và phép vị tự $y_{\kappa_A \otimes N}$ là đơn ánh.

Khi các điều kiện đó được thỏa mãn, phép vị tự $y_{M \otimes_A N}$ là đơn ánh với mọi A-môđun $M$.

Giả sử các giả thiết của (i) được thỏa mãn, và hãy chứng minh (ii) cũng như khẳng định cuối cùng. Cho $M$ là một A-môđun. Vì A-môđun $N/yN$ là phẳng, từ dãy khớp $0 \to N \xrightarrow{y_N} N \to N/yN \to 0$ ta suy ra các dãy khớp

$$
0 \to M \otimes_A N \xrightarrow{u} M \otimes_A N \to M \otimes_A (N/yN) \to 0
$$
$$
0 \to \mathrm{Tor}_1^A(M, N) \xrightarrow{v} \mathrm{Tor}_1^A(M, N) \to 0
$$

trong đó $u = 1_M \otimes y_N$ và $v = \mathrm{Tor}_1^A(1_M, y_N)$; suy ra phép vị tự tỉ số $y$ là đơn ánh trong $M \otimes_A N$, và song ánh trong $\mathrm{Tor}_1^A(M, N)$. Giả sử hơn nữa rằng A-môđun $M$ sinh hữu hạn; khi đó B-môđun $\mathrm{Tor}_1^A(M, N)$ sinh hữu hạn (A, X, p. 107, Mệnh đề 6), do đó bằng không vì $y$ thuộc $m_B$ (bổ đề Nakayama), điều này kéo theo A-môđun $N$ là phẳng (A, X, p. 74, Định lý 2).

(ii) $\Rightarrow$ (i): giả sử các giả thiết của (ii) được thỏa mãn. Xét hai dãy khớp sau của các B-môđun

(1)
$$
0 \to \mathrm{Ker}(y_N) \longrightarrow N \xrightarrow{p} \mathrm{Im}(y_N) \to 0
$$

(2)
$$
0 \to \mathrm{Im}(y_N) \xrightarrow{i} N \longrightarrow N/yN \to 0,
$$

trong đó $p$ và $i$ là các đồng cấu chính tắc. Suy ra đồng cấu $1 \otimes p : \kappa_A \otimes_A N \longrightarrow \kappa_A \otimes_A \mathrm{Im}(y_N)$ là toàn ánh, và (vì $N$ là phẳng) hạt nhân của đồng cấu $1 \otimes i : \kappa_A \otimes_A \mathrm{Im}(y_N) \longrightarrow \kappa_A \otimes_A N$ đẳng cấu với $\mathrm{Tor}_1^A(\kappa_A, N/yN)$. Nhưng ánh xạ $(1 \otimes i) \circ (1 \otimes p)$, bằng $y_{\kappa_A \otimes_A N}$, là đơn ánh theo giả thiết; suy ra $1 \otimes p$ là song ánh và $1 \otimes i$ đơn ánh, và do đó ta có $\mathrm{Tor}_1^A(\kappa_A, N/yN) = 0$. Suy ra A-môđun $N/yN$ là phẳng (III, § 5, No. 2, Định lý 1 and No. 4, Mệnh đề 2).

Vì $N$ và $N/yN$ đều phẳng trên $A$, điều tương tự cũng đúng với $\mathrm{Im}(y_N)$ (dãy khớp (2)). Khi đó từ dãy khớp (1) suy ra $\kappa_A \otimes_A \mathrm{Ker}(y_N)$ đẳng cấu với hạt nhân của $1 \otimes p$, nên bằng không; do đó phép vị tự $y_N$ là đơn ánh theo bổ đề Nakayama.

#### Mệnh đề 10 {#ac-x-s1-prop-10 .statement}

*Cho $\rho : \Lambda \to B$ là một đồng cấu địa phương của các vành địa phương Noether, $N$ là một B-môđun hữu hạn sinh và $y = (y_1, \ldots, y_s)$ là một dãy phần tử của $m_B$. Ký hiệu $\mathfrak{y}$ là iđêan của $B$ sinh bởi dãy này. Các điều kiện sau là tương đương:

(i) A-môđun $N/\mathfrak{y}N$ là phẳng và dãy $y$ là N-chính quy;
(ii) A-môđun $N$ là phẳng và dãy $y$ là $(\kappa_A \otimes_A N)$-chính quy.*

Khi các điều kiện này được thỏa mãn, với mọi A-môđun $M$, dãy $y$ là $M \otimes_A N$-chính quy.

Ta sẽ chứng minh tính tương đương của (i) và (ii) bằng quy nạp theo $s$. Trường hợp $s = 0$ là hiển nhiên, giả sử $s \geqslant 1$; gọi $y'$ là dãy $(y_1, \ldots, y_{s-1})$ và $\mathfrak{y}'$ là iđêan của $B$ sinh bởi dãy đó. Theo bổ đề 2 áp dụng cho B-môđun $N/\mathfrak{y}'N$ và cho phần tử $y_s$ của $B$, điều kiện (i) là tương đương với

(i') A-môđun $N/\mathfrak{y}'N$ là phẳng, dãy $y'$ là N-chính quy, và phép vị tự tỉ số $y_s$ trong $\kappa_A \otimes_A (N/\mathfrak{y}'N) = (\kappa_A \otimes_A N)/\mathfrak{y}'(\kappa_A \otimes_A N)$ là đơn ánh.

Điều kiện này tương đương với (ii) theo giả thiết quy nạp.

Khẳng định cuối cùng cũng suy ra tương tự bằng quy nạp theo $s$ từ khẳng định cuối cùng của bổ đề 2.

#### Mệnh đề 11 {#ac-x-s1-prop-11 .statement}

*Cho $\rho : \Lambda \to B$ là một đồng cấu địa phương của các vành địa phương Noether, $M$ là một A-môđun hữu hạn sinh và $N$ là một B-môđun hữu hạn sinh; giả sử rằng A-môđun $N$ là phẳng.*

a) Cho $(x_1, \ldots, x_r)$ là một dãy các phần tử của $m_A$ chính quy đối với A-môđun $M$, và $(y_1, \ldots, y_s)$ là một dãy các phần tử của $m_B$ chính quy đối với B-môđun $\kappa_A \otimes_A N$; khi đó dãy $(y_1, \ldots, y_s, \rho(x_1), \ldots, \rho(x_r))$ các phần tử của $m_B$ là chính quy đối với B-môđun $M \otimes_A N$.

b) Ta có đẳng thức

$$
\operatorname{prof}_B(M \otimes_A N) = \operatorname{prof}_A(M) + \operatorname{prof}_B(\kappa_A \otimes_A N)
$$

Ký hiệu $x$ là iđêan của A sinh bởi dãy $x$ và $y$ là iđêan của B sinh bởi $y$. Theo Mệnh đề 10, dãy $y$ là $M \otimes_A N$-chính quy và $N/yN$ phẳng trên A, nên dãy $\rho(x) = (\rho(x_1), \ldots, \rho(x_r))$ là chính quy đối với $M \otimes_A (N/yN) = (M \otimes_A N)/y(M \otimes_A N)$. Điều này chứng minh a).

Để chứng minh b), ta có thể giả sử rằng M và N khác không. Theo bổ đề Nakayama, $\kappa_A \otimes_A N$ cũng khác không, nên $\operatorname{prof}_A(M)$ và $\operatorname{prof}_B(\kappa_A \otimes_A N)$ là hữu hạn (No. 4, Hệ quả 2 của Định lý 2). Lấy các dãy chính quy cực đại $x$ và $y$; khi đó ta có $r = \operatorname{prof}_A(M)$, $s = \operatorname{prof}_B(\kappa_A \otimes_A N)$, và tồn tại một ánh xạ a-tuyến tính đơn ánh $u : \kappa_A \to M/xM$ và một ánh xạ b-tuyến tính đơn ánh $v : \kappa_B \to \kappa_A \otimes_A (N/yN)$ (No. 4, Hệ quả 1 của Định lý 2). Vì $N/yN$ phẳng trên A, ánh xạ b-tuyến tính $(u \otimes 1_{N/yN}) \circ v$ từ $\kappa_B$ vào $(M/xM) \otimes_A (N/yN) = (M \otimes_A N)/(\rho(x) + y)(M \otimes_A N)$ là đơn ánh. Điều này kéo theo đẳng thức $\operatorname{prof}_B(M \otimes_A N) = r + s$ (*loc. cit.*).

#### Nhận xét {#ac-x-s1-n6-rem-1 .statement}

Nhắc lại rằng, dưới các giả thiết trước đó,

$$
\dim_B(M \otimes_A N) = \dim_A(M) + \dim_B(\kappa_A \otimes_A N)
$$
(VIII, § 3, No. 4, Mệnh đề 7).

#### Hệ quả {#ac-x-s1-n6-cor-1 .statement}

Cho $\rho : A \to B$ là một đồng cấu địa phương của các vành địa phương Noether làm cho B thành một A-môđun phẳng. Ta có

$$
\operatorname{prof}(B) = \operatorname{prof}(A) + \operatorname{prof}(\kappa_A \otimes_A B),
$$
$$
\dim(B) = \dim(A) + \dim(\kappa_A \otimes_A B).
$$

Thật vậy, chiều sâu (tương ứng, chiều) của B-môđun $\kappa_A \otimes_A B$ bằng chiều sâu (tương ứng, chiều) của vành $\kappa_A \otimes_A B$ theo hệ quả của Mệnh đề 4 (tương ứng, theo VIII, § 1, No. 4).

### 7. Cận Trên Cho Chiều Sâu

#### Mệnh đề 12 {#ac-x-s1-prop-12 .statement}

Cho A là một vành địa phương Noether, M một A-môđun hữu hạn sinh khác không và J một iđêan của A phân biệt với A. Ta có dãy bất đẳng thức

$$
\operatorname{prof}_A(J; M) \leq \operatorname{codim}(\operatorname{Supp}(M) \cap V(J), \operatorname{Supp}(M)) \leq \dim(M) - \dim(M/JM)
$$
$$
\leq [J/m_A J : \kappa_A].
$$

Với mọi phần tử $p$ của $\operatorname{Supp}(M) \cap V(J)$, $\operatorname{prof}_A(J; M)$ nhỏ hơn hoặc bằng $\dim_{A_p}(M_p)$ (No. 5, Mệnh đề 8 và No. 4, Hệ quả 2 của Định lý 2), tức là (VIII, § 1, No. 4, Mệnh đề 9)

#### Nhận xét 1 {#ac-x-s1-n7-rem-1 .statement}

Xét chuỗi các bất đẳng thức của Mệnh đề 12.

a) Để có prof_A(J ; M) = [J/m_AJ : κ_A], điều kiện cần và đủ là J có thể được sinh bởi một dãy M-chính quy (No. 3, Hệ quả 2 của Định lý 1 và A, X, p. 160, Hệ quả 1).

b) Đẳng thức dim(M) − dim(M/JM) = [J/m_AJ : κ_A] có nghĩa là J có thể được sinh bởi một dãy cát tuyến đối với M (VIII, § 3, No. 2).

c) *Nếu M là Macaulay, ta có prof_A(J ; M) = dim(M) − dim(M/JM) (§ 2, No. 2, hệ quả của Mệnh đề 2).*

#### Bổ đề 3 {#ac-x-s1-lem-3 .statement}

Cho A là một vành Noether, p ⊂ p_1 ⊂ ... ⊂ p_{r−1} ⊂ q một chuỗi bão hòa độ dài r các iđêan nguyên tố của A, M một Λ-môđun hữu hạn sinh và n một số nguyên. Nếu A-môđun Ext^n_{A_p}(κ(p), M_p) khác không, thì Ext^{n+r}_{A_q}(κ(q), M_q) cũng vậy.

Hiển nhiên là chỉ cần xét trường hợp r = 1; khi đó, thay A, M, p và q lần lượt bởi A_q, M_q, pA_q và qA_q, ta được quy về trường hợp A là địa phương và q = m_A. Cho $x$ là một phần tử của m_A − p. A_p-môđun Ext^n_A(A/p, M) ⊗_A A_p đẳng cấu với Ext^n_{A_p}(κ(p), M_p) (A, X, p. 111, Mệnh đề 10 b)), do đó khác không theo giả thiết; a fortiori Ext^n_A(A/p, M) khác không. Dãy khớp

$$
0 \to A/p \xrightarrow{x_{A/p}} A/p \to A/(p + xA) \to 0
$$

sinh ra một dãy khớp các môđun mở rộng

$$
\text{Ext}^n_A(A/p, M) \xrightarrow{u} \text{Ext}^n_A(A/p, M) \to \text{Ext}^{n+1}_A(A/(p + xA), M),
$$

trong đó u là phép vị tự tỉ số x. Theo bổ đề Nakayama, ánh xạ này không toàn ánh, nên A-môđun Ext^{n+1}_A(A/(p + xA), M) khác không. Nhưng iđêan nguyên tố duy nhất của A chứa p + xA là m_A, nên A-môđun A/(p + xA) có độ dài hữu hạn (VIII, § 3, No. 2, Bổ đề 2). Nếu Ext^{n+1}_A(κ_A, M) bằng không, thì từ đó, bằng quy nạp theo độ dài của N, ta suy ra rằng Ext^{n+1}_A(N, M) = 0 với mọi A-môđun N có độ dài hữu hạn. Mâu thuẫn này hoàn tất chứng minh.

#### Mệnh đề 13 {#ac-x-s1-prop-13 .statement}

Cho A là một vành Noether, M một A-môđun hữu hạn sinh, p và q là hai iđêan nguyên tố của Supp(M) với p ⊂ q. Ta có

$$
\text{prof}_{A_q}(M_q) \leq \text{prof}_{A_p}(M_p) + \dim(A_q/pA_q).
$$

Chính xác hơn, với mọi chuỗi bão hòa các iđêan nguyên tố p ⊂ p_1 ⊂ ... ⊂ p_{r−1} ⊂ q, ta có \text{prof}_{A_q}(M_q) \leq \text{prof}_{A_p}(M_p) + r.

Đặt p = \text{prof}_{A_p}(M_p), và hãy chứng minh bất đẳng thức thứ hai. Điều đó hiển nhiên nếu p = +∞; trong trường hợp ngược lại ta có \text{Ext}^p_{A_p}(κ(p), M_p) ≠ 0, do đó

$Ext_{A_q}^{p+r}(\kappa(q), M_q) \neq 0$ theo bổ đề 3, điều này kéo theo $prof_{A_q}(M_q) \leq p + r$. Vì $\dim(A_q/pA_q)$ là cận trên bé nhất của các độ dài của những chuỗi bão hòa các iđêan nguyên tố có đầu mút là $p$ và $q$, khẳng định thứ nhất là hệ quả của khẳng định thứ hai.

#### Hệ quả 1 {#ac-x-s1-prop-13-cor-1 .statement}

*Ta có bất đẳng thức*

$$
\dim(M_q) - prof_{A_q}(M_q) \geq \dim(M_p) - prof_{A_p}(M_p) \geq 0 .
$$

Điều này suy ra từ mệnh đề 13 và bất đẳng thức $\dim(M_q) \geq \dim(M_p) + \dim(A_q/pA_q)$ (VIII, § 1, No. 4, mệnh đề 9, a) và No. 3, mệnh đề 7, b)).

#### Hệ quả 2 {#ac-x-s1-prop-13-cor-2 .statement}

*Cho A là một vành Noether địa phương và M là một A-môđun hữu hạn sinh. Ta có bất đẳng thức*

$$
prof_A(M) \leq \inf_{p \in \operatorname{Ass}(M)} \dim(A/p) .
$$

Cho $p$ là một iđêan nguyên tố liên kết với $M$; ta có $prof_{A_p}(M_p) = 0$ (No. 1, nhận xét 2). Mệnh đề 13 áp dụng cho các iđêan $p \subset m_A$ cho bất đẳng thức $prof_A(M) \leq \dim(A/p)$, do đó suy ra hệ quả.

#### Nhận xét 2 {#ac-x-s1-n7-rem-2 .statement}

Ta có $\sup_{p \in \operatorname{Ass}(M)} \dim(A/p) = \dim(M)$ (VIII, § 1, No. 4, nhận xét 2), và thu được lại bất đẳng thức $prof(M) \leq \dim(M)$ với $M \neq 0$ (No. 4, hệ quả 2 của định lý 2).

### 8. Các Vành Noether Địa phương Nguyên; Các Vành Noether Chuẩn tắc

Cho $A$ là một vành Noether. Ký hiệu bởi $(Y_i)_{i \in I}$ họ hữu hạn (II, § 4, No. 2, mệnh đề 10 và No. 3, hệ quả 7 của mệnh đề 11) các thành phần liên thông của $\operatorname{Spec}(A)$. Theo II, § 4, No. 3, mệnh đề 15, với mỗi $i$ tồn tại duy nhất một phần tử lũy đẳng $e_i$ của $A$ sao cho $Y_i = V(e_i)$, và ánh xạ chính tắc từ $A$ vào tích của các vành $A/Ae_i$ là song ánh. Các vành thương $A/Ae_i$ của $A$ được gọi là các *thành phần chính tắc* của $A$. Đặt $f_i = 1 - e_i$. Ta có $\sum_{i \in I} f_i = 1$, và $(f_i)_{i \in I}$ là một họ trực giao các phần tử lũy đẳng khác không của $A$ (*loc. cit.*). Suy ra ảnh của $f_i$ trong $A/Ae_j$ bằng 1 nếu $j = i$ và bằng 0 nếu $j \neq i$; do đó từ đồng cấu vành $A \to \prod_j A/Ae_j$ suy ra một đẳng cấu chính tắc $A_{f_i} \to A/Ae_i$.

Theo *loc. cit.*, hệ quả 2 của mệnh đề 14, các điều kiện sau là tương đương:
(i) các thành phần liên thông của $\operatorname{Spec}(A)$ là bất khả quy;
(ii) mọi iđêan nguyên tố (tương ứng, cực đại) của $A$ chỉ thuộc một thành phần bất khả quy của $\operatorname{Spec}(A)$;
(iii) mọi iđêan nguyên tố (tương ứng, cực đại) của $A$ chỉ chứa một iđêan nguyên tố cực tiểu;
(iv) với mọi iđêan nguyên tố (tương ứng, cực đại) $p$ của $A$, không gian tôpô $\operatorname{Spec}(A_p)$ là bất khả quy;
(v) với mọi thành phần chính tắc $C$ của $A$, không gian tôpô $\operatorname{Spec}(C)$ là bất khả quy.

(i) $A$ là thu gọn và các thành phần liên thông của $\mathrm{Spec}(A)$ là bất khả quy;
(ii) với mọi iđêan nguyên tố (tương ứng, cực đại) $p$ của $A$, vành $A_p$ là một miền nguyên;
(iii) các thành phần chính tắc của $A$ là các miền nguyên.

Một vành Noether được gọi là *địa phương nguyên* nếu nó thỏa mãn các điều kiện tương đương (i) đến (iii) ở trên.

Giả sử vành $A$ địa phương nguyên; gọi $u$ là một đẳng cấu từ $A$ lên một tích (hữu hạn) $\prod_{j \in J} A_j$ của các miền nguyên. Tồn tại một song ánh $\sigma : J \to I$ sao cho ánh xạ từ $\mathrm{Spec}(\prod_{j \in J} A_j)$ vào $\mathrm{Spec}(A)$ liên kết với $u$ xác định một đồng phôi từ $\mathrm{Spec}(A_j)$ lên thành phần liên thông $Y_{\sigma(j)}$ của $\mathrm{Spec}(A)$; khi đó từ $u$ suy ra được một đẳng cấu của thành phần chính tắc $A/Ae_{\sigma(j)}$ lên $A_j$.

#### Mệnh đề 14 {#ac-x-s1-prop-14 .statement}

*Cho $A$ là một vành Noether. Các điều kiện sau là tương đương:*

(i) $A$ là rút gọn và nguyên khép kín trong vành phân thức toàn phần của nó ;
(ii) $A$ đẳng cấu với tích của một họ hữu hạn các vành nguyên khép kín ;
(iii) *các thành phần chính tắc của $A$ là nguyên khép kín* ;
(iv) *với mọi iđêan nguyên tố (tương ứng, iđêan cực đại) $p$ của $A$, vành $A_p$ là nguyên khép kín*.

Tính tương đương của (i) và (ii) suy ra từ V, § 1, No. 2, Hệ quả 2 của Mệnh đề 9, và tính tương đương của (ii) và (iii) suy ra từ các nhận xét đứng trước mệnh đề này. Cho $p$ là một iđêan nguyên tố của $A$; tồn tại một thành phần chính tắc duy nhất $A'$ của $A$ sao cho $p$ thuộc tập con đóng $\mathrm{Spec}(A')$ của $\mathrm{Spec}(A)$, và có một đẳng cấu chính tắc $A_p \to A'_pA'$. Do đó tính tương đương của (iii) và (iv) suy ra từ *loc. cit.*, No. 5, Hệ quả 1 và Hệ quả 3 của Mệnh đề 16.

Một vành $A$ được gọi là *chuẩn tắc* nếu nó là Noether và thỏa mãn các điều kiện tương đương (i) đến (iv) của Mệnh đề 14. Một vành Noether là nguyên khép kín khi và chỉ khi nó nguyên và chuẩn tắc. Một vành địa phương chuẩn tắc là nguyên khép kín.

### 9. Bề sâu và tính liên thông

#### Bổ đề 4 {#ac-x-s1-lem-4 .statement}

*Cho $A$ là một vành Noether, $F$ là một tập con đóng của $\mathrm{Spec}(A)$, $U$ là tập mở bù, và $u : M \to N$ là một đồng cấu của các $A$-môđun sinh hữu hạn.*

a) *Giả sử $u_p : M_p \to N_p$ là đơn ánh với mọi $p \in U$ và có $\mathrm{prof}_F(M) \geqslant 1$. Khi đó $u$ là đơn ánh.*

b) Giả sử $u_p : M_p \to N_p$ là song ánh với mọi $p \in U$ và có $\mathrm{prof}_F(M) \geqslant 2$ và $\mathrm{prof}_F(N) \geqslant 1$. Khi đó $u$ là song ánh.

a) Các giả thiết kéo theo $\mathrm{Supp}(\mathrm{Ker}\,u) \subset F$, do đó $\mathrm{Hom}_\Lambda(\mathrm{Ker}\,u, M) = 0$ (No. 5, Nhận xét 1); vì vậy có $\mathrm{Ker}\,u = 0$.

b) Ta đã biết $u$ là đơn ánh, và có $\mathrm{Supp}(\mathrm{Coker}\,u) \subset F$. Theo loc. cit., ta có $\mathrm{Hom}_A(\mathrm{Coker}\,u, N) = 0$ và $\mathrm{Ext}_A^1(\mathrm{Coker}\,u, M) = 0$. Từ dãy khớp của các môđun mở rộng

$$
\mathrm{Hom}_A(\mathrm{Coker}\,u, N) \to \mathrm{Hom}_A(\mathrm{Coker}\,u, \mathrm{Coker}\,u) \to \mathrm{Ext}_A^1(\mathrm{Coker}\,u, M)
$$

suy ra $\mathrm{Hom}_A(\mathrm{Coker}\,u, \mathrm{Coker}\,u) = 0$, điều này kéo theo $\mathrm{Coker}\,u = 0$.

#### Nhận xét 1 {#ac-x-s1-n9-rem-1 .statement}

Cho $A$ là một vành Noether, $F$ là một tập con đóng của $\mathrm{Spec}(A)$, $U$ là tập mở bù. Để có $\mathrm{prof}_F(A) \geqslant 1$, điều cần và đủ là $\mathrm{Ass}(A) \subset U$ (nhận xét 2, No. 5). Khi điều kiện này được thỏa mãn, mỗi thành phần bất khả quy của $\mathrm{Spec}(A)$ đều gặp $U$, do đó $U$ trù mật trong $\mathrm{Spec}(A)$.

#### Định lý 3 (Hartshorne) {#ac-x-s1-thm-3 .statement}

Cho $A$ là một vành Noether, $F$ là một tập con đóng của $\mathrm{Spec}(A)$ và $U$ là tập mở bù. Giả sử rằng $\mathrm{prof}_F(A) \geqslant 2$. Khi đó, với mọi thành phần liên thông $Y$ của $\mathrm{Spec}(A)$, tập hợp $Y \cap \overline{U}$ là liên thông và trù mật trong $Y$.

Trước hết giả sử rằng $\mathrm{Spec}(A)$ là liên thông. Theo nhận xét 1, $U$ trù mật trong $\mathrm{Spec}(A)$, và còn phải chứng minh rằng nó liên thông. Lập luận phản chứng, giả sử tồn tại hai tập mở rời nhau $U_0$ và $U_1$ của $\mathrm{Spec}(A)$, khác rỗng và có hợp là $U$. Vì tập hợp $\mathrm{Ass}(\Lambda)$ được chứa trong $U$ theo nhận xét 1, nên nó là hợp rời nhau của $\mathrm{Ass}(A) \cap U_0$ và $\mathrm{Ass}(A) \cap U_1$. Theo IV, § 1, No. 1, Mệnh đề 4, tồn tại các iđêan $J_0$ và $J_1$ của $A$ sao cho $\mathrm{Ass}(J_i) = \mathrm{Ass}(A) \cap U_i$, $\mathrm{Ass}(A/J_i) = \mathrm{Ass}(A) \cap U_{1-i} \quad (i = 0, 1)$. Phần bù của $U_i$ trong $\mathrm{Spec}(A)$ chứa $\mathrm{Ass}(A/J_i)$ và $\mathrm{Ass}(J_{1-i})$; vì nó đóng, nó chứa $\mathrm{Supp}(A/J_i)$ và $\mathrm{Supp}(J_{1-i})$. Với $p \in U_i$, do đó có $(J_i)_p = A_p$ và $(J_{1-i})_p = 0$; điều này đặc biệt suy ra rằng $J_0$ và $J_1$ khác $A$. Cho $B$ là A-môđun $A/J_0 \times A/J_1$ và cho $u : A \to B$ là đồng cấu chính tắc. Theo điều đã có ở trên, đồng cấu $u_p$ là song ánh với mọi $p \in U$; hơn nữa, ta có $\mathrm{Ass}(B) \subset U_0 \cup U_1 = U$, nên $\mathrm{prof}_F(B) \geqslant 1$ theo nhận xét 1. Bổ đề 4 khi đó suy ra rằng $u$ là song ánh, điều này mâu thuẫn với tính liên thông của $\mathrm{Spec}(A)$.

Xét trường hợp tổng quát. Cho $J$ là một iđêan của $A$ sao cho $F = V(J)$ và cho $Y$ là một thành phần liên thông của $\mathrm{Spec}(A)$. Theo II, § 4, No. 3, Mệnh đề 15, tồn tại một phần tử lũy đẳng $f$ của $\Lambda$ sao cho $Y$ được đồng nhất với tập con $\mathrm{Spec}(A_f)$ của $\mathrm{Spec}(A)$. Khi đó $Y \cap F$ được đồng nhất với $V(J_f)$; ta có $\mathrm{prof}_{\Lambda_f}(J_f, A_f) \geqslant \mathrm{prof}_A(J; A) \geqslant 2$ theo Mệnh đề 6, a) của No. 3. Từ phần đầu của chứng minh suy ra rằng $Y \cap U = Y - (Y \cap F)$ là liên thông và trù mật trong $Y$.

#### Hệ quả 1 {#ac-x-s1-thm-3-cor-1 .statement}

Ánh xạ gán cho mỗi thành phần liên thông của $U$ bao đóng của nó trong $\mathrm{Spec}(A)$ là một song ánh từ tập hợp các thành phần liên thông của $U$ lên tập hợp các thành phần liên thông của $\mathrm{Spec}(A)$.

#### Hệ quả 2 {#ac-x-s1-thm-3-cor-2 .statement}

Với mọi vành địa phương Noether B có độ sâu $\geq 2$, không gian tôpô $\operatorname{Spec}(B) - \{ m_B \}$ là liên thông.

#### Hệ quả 3 {#ac-x-s1-thm-3-cor-3 .statement}

Dưới các giả thiết của Định lý 3, giả sử rằng $\operatorname{Spec}(A_p)$ là bất khả quy (resp. rằng $A_p$ là một miền nguyên) với mọi $p \in U$; khi đó $\operatorname{Spec}(A_p)$ là bất khả quy (resp. $A_p$ là một miền nguyên) với mọi $p \in \operatorname{Spec}(A)$.

Cho $(Y_i)_{i \in I}$ là họ (hữu hạn) các thành phần bất khả quy của $\operatorname{Spec}(A)$. Cho $p \in U$; vì $\operatorname{Spec}(\Lambda_p)$ là bất khả quy, $p$ chỉ chứa một iđêan nguyên tố cực tiểu của $\Lambda$, và do đó chỉ thuộc về một trong các $Y_i$ (II, § 4, No. 3, Hệ quả 2 của Mệnh đề 14). Các tập con $Y_i \cap U$ là các tập con đóng của $U$, rời nhau từng đôi một, không rỗng vì $U$ trù mật trong $\operatorname{Spec}(A)$, và bất khả quy theo II, § 4, No. 1, Mệnh đề 7; do đó chúng là các thành phần liên thông của $U$. Các bao đóng $Y_i$ của chúng là các thành phần liên thông của $\operatorname{Spec}(\Lambda)$ (Hệ quả 1). Điều này chứng minh rằng các thành phần liên thông của $\operatorname{Spec}(A)$ là bất khả quy, và do đó $\operatorname{Spec}(A_p)$ là bất khả quy với mọi $p$ (No. 8).

Giả sử rằng $A_q$ là một miền nguyên với mọi $q \in U$. Cho $p \in \operatorname{Spec}(A)$. Vì $\operatorname{Spec}(A_p)$ là bất khả quy, căn nil của $A_p$ là iđêan nguyên tố cực tiểu duy nhất của $A_p$; do đó nó thuộc $\operatorname{Ass}(A_p)$ (IV, § 1, No. 3, Hệ quả 1 của Mệnh đề 7), và vì thế bằng $qA_p$, trong đó $q$ là một iđêan nguyên tố liên kết với $A$ (IV, § 1, No. 2, Hệ quả của Mệnh đề 5). Ta có $q \in U$ (Nhận xét 1) và $qA_q \in \operatorname{Ass}(A_q)$ (loc. cit.); vì $A_q$ là một miền nguyên, $q$ bằng không, và do đó $A_p$ là một miền nguyên.

#### Hệ quả 4 {#ac-x-s1-thm-3-cor-4 .statement}

Cho $\Lambda$ là một vành Noether mà phổ của nó là liên thông. Giả sử tồn tại một số nguyên $d \geq 1$ sao cho ta có $\operatorname{prof}(\Lambda_p) \geq 2$ với mọi iđêan nguyên tố $p$ của $A$ có chiều cao $> d$.

a) Với mọi tập con đóng $Z$ của $\operatorname{Spec}(A)$ có đối chiều $> d$, không gian $\operatorname{Spec}(A) - Z$ là liên thông.

b) Cho $Y$ và $Y'$ là các thành phần bất khả quy của $\operatorname{Spec}(A)$. Tồn tại một dãy $X_1, X_2, \ldots, X_n$ các thành phần bất khả quy của $\operatorname{Spec}(A)$ sao cho ta có $X_1 = Y$, $X_n = Y'$ và, với $i = 1, \ldots, n-1$

$$
\operatorname{codim}(X_i \cap X_{i+1}, \operatorname{Spec}(A)) \leq d .
$$

Cho $Z \subset \operatorname{Spec}(A)$ là một tập con đóng có đối chiều $> d$. Với mọi $p \in Z$, ta có $\dim(A_p) > d$, do đó $\operatorname{prof}(A_p) \geq 2$, suy ra $\operatorname{prof}_Z(A)$ là $\geq 2$ (No. 5, Mệnh đề 8) và vì thế $\operatorname{Spec}(A) - Z$ là liên thông (Định lý 3).

Ta chứng minh b). Ký hiệu $Z$ là hợp của các tập hợp $X' \cap X''$ khi $(X', X'')$ chạy qua tập hợp (hữu hạn) các cặp thành phần bất khả quy của $\operatorname{Spec}(A)$ sao cho $\operatorname{codim}(X' \cap X'', \operatorname{Spec}(A)) > d$. Theo a), tập hợp $\operatorname{Spec}(A) - Z$ là liên thông. Mọi thành phần bất khả quy của $\operatorname{Spec}(A)$ đều cắt $\operatorname{Spec}(A) - Z$; các vết của chúng trên $\operatorname{Spec}(A) - Z$ là các thành phần bất khả quy của $\operatorname{Spec}(A) - Z$ (II, § 4, No. 1, Mệnh đề 7). Vì $\operatorname{Spec}(A) - Z$ là liên thông, tồn tại một dãy $X_1, \ldots, X_n$ các thành phần bất khả quy của $\operatorname{Spec}(A)$ sao cho ta có $X_1 - Z = Y - Z$, $X_n - Z = Y' - Z$ và $(X_i - Z) \cap (X_{i+1} - Z) \neq \varnothing$ với $1 \leq i \leq n-1$; nói cách khác ta có $X_1 = Y$, $X_n = Z$ và $\operatorname{codim}(X_i \cap X_{i+1}) \leq d$.

#### Nhận xét 2 {#ac-x-s1-n9-rem-2 .statement}

*Khi A là một vành Macaulay, có thể áp dụng hệ quả với $d = 1$ (§ 2, No. 5).*

#### Ví dụ (Giao hoàn chỉnh tạo bởi bốn mặt phẳng tọa độ của một không gian afin chiều 4) {#ac-x-s1-n9-exa-1 .statement}

Cho $k$ là một trường. Ký hiệu S là vành đa thức $k[T_1, T_2, T_3, T_4]$. Nhắc lại rằng (VIII, § 2, No. 4, Định lý 3) mọi dãy cực đại các iđêan nguyên tố của S đều có độ dài 4. Ký hiệu m là iđêan của S sinh bởi các $T_i$, a là iđêan sinh bởi $T_1T_2$ và $T_3T_4$, và $p_{ij}$, với $1 \leq i < j \leq 4$, là iđêan sinh bởi $T_i$ và $T_j$. Các iđêan $p_{ij}$ là nguyên tố, có chiều cao 2, tổng của chúng là iđêan cực đại m, và ta có $a = p_{13} \cap p_{14} \cap p_{23} \cap p_{24}$.

a) Vành $A = S/a$ là reduced; các thành phần bất khả quy của Spec(A) là các tập hợp $X_{ij} = V(p_{ij}/a)$ với $i = 1,2,\ j = 3,4$, có chiều 2 và đều chứa điểm $m/a$. Đặc biệt, Spec(A) là liên thông và có chiều 2. Giao của hai thành phần phân biệt $X_{ij}$ và $X_{kl}$ thu về $\{m/a\}$ nếu $\{i,j\} \cap \{k,l\} = \varnothing$, và có chiều 1 trong trường hợp ngược lại. Suy ra kết luận của hệ quả 4 được thỏa mãn với $d = 1$ (sau này ta sẽ thấy rằng A là một vành Macaulay, nên chính giả thiết của hệ quả 4 cũng được thỏa mãn với $d = 1$).

b) Gọi b là iđêan của S sinh bởi $T_1T_2$, $T_1T_3$, $T_2T_4$, $T_3T_4$, và B là vành $S/b$. Ta có $b = p_{14}p_{23} = p_{14} \cap p_{23}$. Vành B là reduced. Phổ của nó được đồng nhất với tập con đóng $X_{14} \cup X_{23}$ của Spec(A); nó có hai thành phần bất khả quy (có chiều 2) mà giao của chúng thu về một điểm. Độ sâu của B dọc theo điểm này là dương ngặt vì B là reduced, và nhỏ hơn 1 theo Định lý 3, nên bằng 1.* Vì vậy B không phải là một vành Macaulay. \*

### 10. Độ sâu và tính chuẩn tắc

Cho A là một vành Noether và $p$ là một iđêan nguyên tố của A. Ta có $\mathrm{prof}(A_p) \leq \mathrm{ht}(p)$ (No. 4, hệ quả 2 của Định lý 2). Nếu hơn nữa A là reduced, vành địa phương $A_p$ là reduced (II, § 2, No. 6, mệnh đề 17), do đó:

a) nếu $\mathrm{ht}(p) = 0$, thì $A_p$ là một trường;
b) nếu $\mathrm{ht}(p) \geq 1$, thì ta có $\mathrm{prof}(A_p) \geq 1$ (No. 1, nhận xét 3).

Ngược lại:

#### Mệnh đề 15 {#ac-x-s1-prop-15 .statement}

Cho A là một vành Noether thỏa mãn hai điều kiện sau:
(i) với mọi iđêan nguyên tố cực tiểu $p$ của $\Lambda$, vành $\Lambda_p$ là reduced;
(ii) với mọi iđêan nguyên tố $p$ của A có chiều cao $\geq 1$, ta có $\mathrm{prof}(A_p) \geq 1$.
Khi đó A là reduced.

Gọi $n$ là căn lũy linh của A. Với mọi iđêan nguyên tố cực tiểu $p$ của A, theo (i) ta có $n_p = 0$, nghĩa là $p \not\in \mathrm{Supp}(n)$ và $a fortiori$ $p \not\in \mathrm{Ass}_A(n)$. Với mọi $p \in \mathrm{Spec}(A)$ có chiều cao $\geq 1$, theo (ii) ta có $pA_p \not\in \mathrm{Ass}_{A_p}(A_p)$ và $a fortiori$ $pA_p \not\in \mathrm{Ass}_{A_p}(n_p)$, do đó $p \not\in \mathrm{Ass}_A(n)$ (IV, § 1, No. 2, mệnh đề 5). Vì thế tập hợp $\mathrm{Ass}_A(n)$ là rỗng, điều này kéo theo $n$ bằng không.

#### Mệnh đề 16 {#ac-x-s1-prop-16 .statement}

Cho $A$ là một vành Noether nguyên đóng, $J$ là một iđêan của $A$ có chiều cao $\geqslant 2$, và $M$ là một $A$-môđun phản xạ kiểu hữu hạn. Ta có $\operatorname{prof}_A(J; M) \geqslant 2$.

Hãy chọn một không gian vectơ hữu hạn chiều $V$ trên trường phân thức của $A$ và một dàn $N$ trong $V$ đẳng cấu với $M$ (VII, § 4, No. 2, Nhận xét 1). Các iđêan nguyên tố liên kết với $V/N$, vì có chiều cao 1 (*loc. cit.*, Định lý 2), không chứa $J$; theo Nhận xét 2 của No. 1, điều này kéo theo $\operatorname{prof}_A(J; V/N) \geqslant 1$. Mặt khác, A-môđun $V$ là chia được và không xoắn, do đó đơn ánh (A, X, p. 17, Hệ quả 2 của Mệnh đề 10), điều này kéo theo $\operatorname{prof}_A(J; V) = +\infty$. Khi đó bất đẳng thức $\operatorname{prof}_A(J; N) \geqslant 2$ suy ra từ Mệnh đề 1 của No. 1.

#### Hệ quả {#ac-x-s1-n10-cor-1 .statement}

*Một vành địa phương Noether nguyên đóng có chiều $\geqslant 2$ có độ sâu $\geqslant 2$*.

Cho $A$ là một vành chuẩn tắc (No. 8) và $\mathfrak{p}$ là một iđêan nguyên tố của $A$. Khi đó:
a) nếu $\operatorname{ht}(\mathfrak{p}) = 0$, $A_{\mathfrak{p}}$ là một trường;
b) nếu $\operatorname{ht}(\mathfrak{p}) = 1$, $A_{\mathfrak{p}}$ là một vành định giá rời rạc (VII, § 1, No. 7, Mệnh đề 11);
c) nếu $\operatorname{ht}(\mathfrak{p}) \geqslant 2$, ta có $\operatorname{prof}(A_{\mathfrak{p}}) \geqslant 2$ (hệ quả của Mệnh đề 16).

Ngược lại:

#### Định lý 4 (Serre) {#ac-x-s1-thm-4 .statement}

*Cho $A$ là một vành Noether thỏa mãn các điều kiện sau*:
(i) *với mọi iđêan nguyên tố cực tiểu $\mathfrak{p}$ của $A$, vành $A_{\mathfrak{p}}$ là rút gọn*;
(ii) *với mọi iđêan nguyên tố $\mathfrak{p}$ của $A$ có chiều cao 1, vành $A_{\mathfrak{p}}$ là nguyên đóng*;
(iii) *với mọi iđêan nguyên tố $\mathfrak{p}$ của $A$ có chiều cao $\geqslant 2$, ta có $\operatorname{prof}(A_{\mathfrak{p}}) \geqslant 2$*.

*Thì $A$ là chuẩn tắc*.

Cần chứng minh rằng vành $A_{\mathfrak{p}}$ là nguyên đóng với mọi $\mathfrak{p} \in \operatorname{Spec}(A)$, điều này ta sẽ làm bằng quy nạp theo $\operatorname{ht}(\mathfrak{p})$. Với $\operatorname{ht}(\mathfrak{p}) \leqslant 1$ điều này suy ra từ các giả thiết (i) và (ii). Vậy giả sử rằng $\operatorname{ht}(\mathfrak{p}) \geqslant 2$ và rằng $A_q$ là nguyên đóng với mọi iđêan nguyên tố $q$ của $A$ có chiều cao $< \operatorname{ht}(\mathfrak{p})$. Theo giả thiết (iii), ta có $\operatorname{prof}(A_{\mathfrak{p}}) \geqslant 2$. Theo giả thiết quy nạp và hệ quả 3 của định lý 3 của No. 9, áp dụng cho vành $A_{\mathfrak{p}}$ và cho tập con đóng $\{\mathfrak{p}A_{\mathfrak{p}}\}$ của $\operatorname{Spec}(A_{\mathfrak{p}})$, vành $A_{\mathfrak{p}}$ là một miền nguyên. Gọi $K$ là trường phân thức của nó và gọi $B$ là một vành con của $K$, chứa $A_{\mathfrak{p}}$ và hữu hạn trên $A_{\mathfrak{p}}$. Cần chứng minh rằng $B$ bằng $A_{\mathfrak{p}}$. Ký hiệu bởi $i$ đơn ánh chính tắc từ $A_{\mathfrak{p}}$ vào $B$. Vì $B$ được chứa trong $K$, nó là một $A_{\mathfrak{p}}$-môđun không xoắn, do đó có độ sâu $\geqslant 1$. Hơn nữa, với mọi iđêan nguyên tố $q$ của $A_{\mathfrak{p}}$ phân biệt với $\mathfrak{p}A_{\mathfrak{p}}$, đồng cấu $i_q : (A_{\mathfrak{p}})_q \to B_q$ là song ánh vì $A_q$ là nguyên đóng. Theo bổ đề 4 của No. 9, áp dụng cho tập con đóng $F = \{\mathfrak{p}A_{\mathfrak{p}}\}$ của $\operatorname{Spec}(A_{\mathfrak{p}})$, đồng cấu $i$ là song ánh, điều này hoàn tất chứng minh định lý.

#### Nhận xét 1 {#ac-x-s1-n10-rem-1 .statement}

Một dạng thuận tiện của định lý 4 là như sau: cho $A$ là một vành Noether, sao cho với mọi iđêan nguyên tố $p$ của $A$ thì vành $A_p$ hoặc là nguyên đóng hoặc có độ sâu $\geqslant 2$; khi đó $A$ là chuẩn tắc. Thật vậy, hãy kiểm tra các giả thiết của định lý 4. Cho $p \in \mathrm{Spec}(A)$. Nếu $\mathrm{ht}(p) \leqslant 1$, thì ta có $\mathrm{prof}(A_p) \leqslant 1$, do đó $A_p$ là nguyên đóng. Nếu $\mathrm{ht}(p) \geqslant 2$, vành $A_p$ hoặc có độ sâu $\geqslant 2$, hoặc là nguyên đóng, điều này lại kéo theo $\mathrm{prof}(A_p) \geqslant 2$ (No. 1, hệ quả 2 của mệnh đề 1), do đó suy ra kết luận mong muốn. Tương tự, ta kiểm tra được mệnh đề sau: cho $A$ là một vành Noether sao cho với mọi iđêan nguyên tố $p$ của $A$, vành $A_p$ hoặc là rút gọn hoặc có độ sâu $\geqslant 1$; khi đó $A$ là rút gọn.

#### Hệ quả 1 {#ac-x-s1-thm-4-cor-1 .statement}

*Cho $\Lambda$ là một vành Noether, $F$ là một tập con đóng của $\mathrm{Spec}(A)$, $U$ là tập mở bù. Giả sử rằng $\mathrm{prof}_F(A)$ là $\geqslant 2$ (resp. $\geqslant 1$) và rằng, với mọi $p \in U$, vành $A_p$ là nguyên đóng (resp. rút gọn). Khi đó $A$ là chuẩn tắc* (resp. rút gọn).

Với mọi $p \in F$, ta có $\mathrm{prof}(A_p) \geqslant \mathrm{prof}_F(A)$ (No. 5, Prop. 8); vì vậy chỉ cần áp dụng nhận xét trước đó.

#### Hệ quả 2 {#ac-x-s1-thm-4-cor-2 .statement}

*Cho $\rho : A \to B$ là một đồng cấu của các vành Noether khiến $B$ trở thành một A-môđun phẳng.

a) *Nếu $B$ là chuẩn tắc và phẳng trung thành trên $A$, thì $A$ là chuẩn tắc.*

b) *Giả sử rằng $A$ là chuẩn tắc và rằng vành $\kappa(p) \otimes_A B$ là chuẩn tắc khi $p$ là một iđêan nguyên tố cực tiểu của $A$, và rút gọn khi $p$ là một iđêan nguyên tố có chiều cao 1. Khi đó vành $B$ là chuẩn tắc.*

a) Giả sử $B$ chuẩn tắc và phẳng trung thành trên $A$. Khi đó $\rho$ là đơn ánh (I, § 3, No. 5, Prop. 9) và $B$ là rút gọn, suy ra $A$ là rút gọn. Gọi $S$ là tập hợp các ước không của không của $A$. Vì $B$ phẳng trên $A$, $\rho(S)$ gồm các ước không của không trong $B$, do đó $B$ là nguyên đóng trong $\rho(S)^{-1}B$. Gọi $x$ là một phần tử của $S^{-1}A$ nguyên trên $A$; khi đó phần tử $x \otimes 1_B$ của vành $S^{-1}A \otimes_A B$ (được đồng nhất với $\rho(S)^{-1}B$) là nguyên trên $B$, nên thuộc $B$. Vì $B$ phẳng trung thành trên $A$, ta có $x \in A$ (I, § 3, No. 5, Prop. 10, (ii)), và $A$ là chuẩn tắc.

b) Dưới các giả thiết của b), theo Nhận xét 1, chỉ cần chứng minh rằng với mọi iđêan nguyên tố $q$ của $B$, vành địa phương $B_q$ là chuẩn tắc hoặc có độ sâu $\geqslant 2$. Gọi $p$ là iđêan nguyên tố $\rho^{-1}(q)$ của $A$; đồng cấu địa phương $A_p \to B_q$ suy ra từ $\rho$ khiến $B_q$ trở thành một A_p-môđun phẳng trung thành (I, § 3, No. 5, Prop. 9). Ta phân biệt bốn trường hợp :

1) $\mathrm{ht}(p) = 0$. Khi đó $A_p$ là một trường, bằng $\kappa(p)$; vành $A_p \otimes_A B$ là chuẩn tắc theo giả thiết. Điều tương tự cũng đúng với $B_q$, là một vành phân thức của nó.

#### Nhận xét 2 {#ac-x-s1-n10-rem-2 .statement}

$\mathrm{ht}(p) = 1$ và $\mathrm{ht}(q) \leqslant 1$. Khi đó $A_p$ là một vành định giá rời rạc; gọi $\pi$ là một phần tử chuẩn hóa của $A_p$. Vì $B_q$ là phẳng trung thành trên $A_p$, phần tử $\pi 1_{B_q}$ của $B_q$ không phải là một ước của không, nên vành địa phương $B_q/\pi B_q$ có chiều $0$ (VIII, § 3, No. 1, Hệ quả 2 của Mệnh đề 1). Nó là thu gọn, vì nó là một vành phân thức của vành thu gọn $\kappa(p) \otimes_A B$, và do đó nó là một trường. Vậy $B_q$ là một vành định giá rời rạc (VI, § 1, No. 4, Mệnh đề 2), nên đóng nguyên.

#### Nhận xét 3 {#ac-x-s1-n10-rem-3 .statement}

$\mathrm{ht}(p) = 1$ và $\mathrm{ht}(q) \geq 2$. Khi đó, theo quan hệ
$$
\dim(B_q) = \dim(A_p) + \dim(\kappa(p) \otimes_A B_q)
$$
(VIII, § 3, No. 4, Hệ quả 1 của Mệnh đề 7), vành $\kappa(p) \otimes_A B_q$ có chiều $\geq 1$. Nó là thu gọn theo giả thiết, nên có độ sâu $\geq 1$ (No. 1, Nhận xét 3). Khi đó ta có (No. 6, Hệ quả của Mệnh đề 11)
$$
\mathrm{prof}(B_q) = \mathrm{prof}(A_p) + \mathrm{prof}(\kappa(p) \otimes_A B_q) \geq 1 + 1 = 2 .
$$

#### Nhận xét 4 {#ac-x-s1-n10-rem-4 .statement}

$\mathrm{ht}(p) \geq 2$. Vì $A_p$ có độ sâu $\geq 2$ (Hệ quả của Mệnh đề 16), điều tương tự cũng đúng với $B_q$ theo *loc. cit*.

#### Hệ quả 3 {#ac-x-s1-thm-4-cor-3 .statement}

*Cho $\rho : A \to B$ là một đồng cấu của các vành Noether. Giả sử rằng $B$ là một A-môđun phẳng, rằng $A$ là chuẩn tắc, và rằng $\kappa(p) \otimes_A B$ là chuẩn tắc với mọi $p \in \mathrm{Spec}(A)$. Khi đó $B$ là chuẩn tắc.*

## BÀI TẬP {#ac-x-s1-exercises}

Xem [các bài tập của § 1](exercises/s1/).
