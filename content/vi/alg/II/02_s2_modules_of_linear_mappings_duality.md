---
book: alg
book_title: Algebra
chapter: II
chapter_title: LINEAR ALGEBRA
section: 2
section_title: Modules of linear mappings. Duality
lang: vi
source: alg-i-iii
source_edition: 1998, Springer
pdf_pages: 0251-0267, 0410-0419
extraction: ocr
subsections:
    - "no": 1
      title: PROPERTIES OF $\mathrm{Hom}_A(E, F)$ RELATIVE TO EXACT SEQUENCES
      page: 0
      pdf_page: 251
    - "no": 2
      title: PROJECTIVE MODULES
      page: 0
      pdf_page: 255
    - "no": 3
      title: LINEAR FORMS; DUAL OF A MODULE
      page: 0
      pdf_page: 256
    - "no": 4
      title: ORTHOGONALITY
      page: 0
      pdf_page: 258
    - "no": 5
      title: TRANSPOSE OF A LINEAR MAPPING
      page: 0
      pdf_page: 258
    - "no": 6
      title: DUAL OF A QUOTIENT MODULE. DUAL OF A DIRECT SUM. DUAL BASES
      page: 0
      pdf_page: 260
    - "no": 7
      title: BIDUAL
      page: 0
      pdf_page: 263
    - "no": 8
      title: LINEAR EQUATIONS
      page: 0
      pdf_page: 264
statements: 42
exercises: 3
content_sha256: e3a952582be81d836d4a07b41846aae61300d2726b5b87ffc40deb770aca2b4b
translated_from: content/en/alg/II/02_s2_modules_of_linear_mappings_duality.md
source_content_sha256: 3b782f3a14dd64b6c4820e944b52b743d6c50f9a631627053d96cf898326cdfe
translation_model: gpt-5-6, gpt-5-6-mini
translation_run: translate-vi-b0e91fc7
glossary_version: 34
glossary_terms_sha256: 42955ea110dde08e810ec87a96dba277c42547c2146017768b456caebb9538a4
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 2. MÔĐUN CỦA CÁC ÁNH XẠ TUYẾN TÍNH. ĐỐI NGẪU

### 1. CÁC TÍNH CHẤT CỦA $\mathrm{Hom}_A(E, F)$ LIÊN QUAN ĐẾN CÁC DÃY KHỚP

#### Định lý 1 {#alg-ii-s2-thm-1 .statement}

*Cho A là một vành, E', E, E'' là ba A-môđun và u : E' \to E, v : E \to E'' là hai đồng cấu. Dãy*

$$
\text{(1)} \quad E' \xrightarrow{u} E \xrightarrow{v} E'' \longrightarrow 0
$$

*là khớp khi và chỉ khi, với mọi A-môđun F, dãy*

$$
\text{(2)} \quad 0 \longrightarrow \mathrm{Hom}(E'', F) \xrightarrow{\bar{v}} \mathrm{Hom}(E, F) \xrightarrow{\bar{u}} \mathrm{Hom}(E', F)
$$

*(trong đó $\bar{u} = \mathrm{Hom}(u, 1_F)$, $\bar{v} = \mathrm{Hom}(v, 1_F)$) là khớp*.

Giả sử dãy (1) là khớp. Nếu $w \in \mathrm{Hom}(E'', F)$ và $\bar{v}(w) = w \circ v = 0$, thì $w = 0$ vì $v$ là toàn ánh. Do đó dãy (2) khớp tại $\mathrm{Hom}(E'', F)$. Ta chứng minh rằng nó khớp tại $\mathrm{Hom}(E, F)$. $\bar{u} \circ \bar{v} = \mathrm{Hom}(v \circ u, 1_F)$ (\S 1, no. 2, công thức (10)) và $v \circ u = 0$ vì dãy (1) khớp tại E. Do đó $\bar{u} \circ \bar{v} = 0$, tức là $\mathrm{Im}(\bar{v}) \subset \mathrm{Ker}(\bar{u})$. Mặt khác, nếu $w \in \mathrm{Ker}(\bar{u})$, thì $w \circ u = 0$ và do đó $\mathrm{Ker}(w) \supset \mathrm{Im}(u)$. Nhưng vì dãy (1) khớp tại E, $\mathrm{Im}(u) = \mathrm{Ker}(v)$ và do đó $\mathrm{Ker}(w) \supset \mathrm{Ker}(v)$; vì $v$ là toàn ánh, theo \S 1, no. 3, *Nhận xét*, tồn tại một $w' \in \mathrm{Hom}(E'', F)$ sao cho w = w' \circ v = \bar{v}(w'). Do đó $\mathrm{Ker}(\bar{u}) \subset \operatorname{Im}(\bar{v}),$ và điều này hoàn tất chứng minh rằng dãy (2) là khớp.

Ngược lại, giả sử rằng (2) là khớp với mọi A-môđun F. Vì $\bar{u} \circ \bar{v} = \operatorname{Hom}(v \circ u, 1_F) = 0, w \circ v \circ u = 0$ với mọi đồng cấu $w : E'' \to F$. Lấy $F = E''$ và $w = 1_{E''}$, trước hết suy ra $v \circ u = 0$ và do đó $u(E') \subset \operatorname{Ker}(v)$. Bây giờ lấy $F = \operatorname{Coker}(u)$ và gọi $\phi : E \to F = E/u(E')$ là ánh xạ chính tắc. Khi đó $\bar{u}(\phi) = \phi \circ u = 0$ theo định nghĩa và do đó tồn tại một $\psi \in \operatorname{Hom}(E'', F)$ sao cho $\phi = \bar{v}(\psi) = \psi \circ v$; điều này hiển nhiên kéo theo $u(E') = \operatorname{Ker}(\phi) \supset \operatorname{Ker}(v)$, và do đó chứng minh rằng dãy (1) khớp tại E. Cuối cùng, gọi $\theta$ là đồng cấu chính tắc của $E''$ lên $F = E''/v(E)$; khi đó $\bar{v}(\theta) = \theta \circ v = 0$, suy ra $\theta = 0$; do đó $F = \{0\}$ và $v$ là toàn ánh. Vì vậy dãy (1) khớp tại $E''$.

#### Hệ quả {#alg-ii-s2-n1-cor-1 .statement}

*Một ánh xạ A-tuyến tính* $u : E \to F$ *là toàn ánh* (tương ứng *song ánh*, tương ứng *không*) *khi và chỉ khi, với mọi A-môđun G, ánh xạ* $\operatorname{Hom}(u, 1_G) : \operatorname{Hom}(F, G) \to \operatorname{Hom}(E, G)$ *là đơn ánh* (tương ứng *song ánh*, tương ứng *không*).

Chỉ cần áp dụng Định lý 1 vào trường hợp $E'' = \{0\}$ (tương ứng $E' = \{0\}$ tương ứng $E'' = E$ và $v = 1_E$).

Chú ý rằng bắt đầu từ một dãy khớp

$$
0 \longrightarrow E' \xrightarrow{u} E \xrightarrow{v} E'' \longrightarrow 0
$$

dãy tương ứng

$$
0 \longrightarrow \operatorname{Hom}(E'', F) \xrightarrow{\bar{v}} \operatorname{Hom}(E, F) \xrightarrow{\bar{u}} \operatorname{Hom}(E', F) \longrightarrow 0
$$

*không nhất thiết khớp*, nói cách khác, đồng cấu $\bar{u}$ không nhất thiết toàn ánh. Nếu $E'$ được đồng nhất với một môđun con của E, điều này có nghĩa là một ánh xạ tuyến tính từ $E'$ vào F không phải lúc nào cũng mở rộng được thành một ánh xạ tuyến tính từ E vào F (Bài tập 11 và 12). Tuy nhiên:

#### Mệnh đề 1 {#alg-ii-s2-prop-1 .statement}

*Nếu dãy khớp các ánh xạ tuyến tính*

(3)
$$
0 \longrightarrow E' \xrightarrow{u} E \xrightarrow{v} E'' \longrightarrow 0
$$

*tách* (nói cách khác, nếu $u(E')$ là một *nhân tử trực tiếp* của E) *thì dãy*

(4)
$$
0 \longrightarrow \operatorname{Hom}(E'', F) \xrightarrow{\bar{v}} \operatorname{Hom}(E, F) \xrightarrow{\bar{u}} \operatorname{Hom}(E', F) \longrightarrow 0
$$

*là khớp và tách*. *Ngược lại, nếu, với mọi A-môđun F, dãy (4) là khớp thì dãy (3) tách*.

Nếu dãy khớp (3) tách, tồn tại một ánh xạ tuyến tính co rút $u' : E \to E'$ liên kết với $u$ (\S 1, no. 9, Mệnh đề 15); nếu

$$
\bar{u}' = \operatorname{Hom}(u', 1_F) : \operatorname{Hom}(E', F) \to \operatorname{Hom}(E, F),
$$

sự kiện rằng $u' \circ u$ là đồng nhất thức suy ra rằng $\bar{u} \circ \bar{u}'$ là đồng nhất thức ($\S 1$, no. 2, công thức (10)) và do đó mệnh đề thứ nhất suy ra từ $\S 1$, no. 9, Mệnh đề 15. Ngược lại, giả sử dãy (4) là khớp với $F = E'$. Khi đó tồn tại một phần tử $f \in \mathrm{Hom}(E, E')$ sao cho $f \circ u = 1_{E'}$, và kết luận suy ra từ $\S 1$, no. 9, Mệnh đề 15.

Chú ý rằng mệnh đề thứ nhất của Mệnh đề 1 cũng có thể được xem như một trường hợp đặc biệt của $\S 1$, no. 6, Hệ quả 1 của Mệnh đề 6, bằng cách đồng nhất một cách chính tắc $\mathrm{Hom}(E', F) \oplus \mathrm{Hom}(E'', F)$ với $\mathrm{Hom}(E' \oplus E'', F)$ nhờ ánh xạ $\mathbf{Z}$-tuyến tính $\mathrm{Hom}(p', 1_F) + \mathrm{Hom}(p'', 1_F)$, trong đó $p': E' \oplus E'' \to E'$ và $p'': E' \oplus E'' \to E''$ là các phép chiếu chính tắc.

#### Định lý 2 {#alg-ii-s2-thm-2 .statement}

*Nếu $A$ là một vành, $F', F, F''$ là ba $A$-môđun và $u: F' \to F, v: F \to F''$ là hai đồng cấu, thì dãy*

$$
0 \longrightarrow F' \xrightarrow{v} F \xrightarrow{u} F''
$$

*khớp khi và chỉ khi, với mọi $A$-môđun $E$, dãy*

$$
0 \longrightarrow \mathrm{Hom}(E, F') \xrightarrow{\bar{u}} \mathrm{Hom}(E, F) \xrightarrow{\bar{v}} \mathrm{Hom}(E, F'')
$$

*(trong đó $\bar{u} = \mathrm{Hom}(1_E, u), \bar{v} = \mathrm{Hom}(1_E, v)$) là khớp.*

Giả sử dãy (5) là khớp. Trước hết, chú ý rằng

$$
\bar{v} \circ \bar{u} = \mathrm{Hom}(1_E, v \circ u) = 0
$$

(II, $\S 1$, no. 2, công thức (10)) vì $v \circ u = 0$. Ảnh của $\mathrm{Hom}(E, F')$ qua $\bar{u}$ do đó được chứa trong hạt nhân $N$ của $\bar{v}$; gọi $f$ là đồng cấu của $\mathbf{Z}$-môđun $\mathrm{Hom}(E, F')$ vào $N$ có đồ thị bằng đồ thị của $\bar{u}$; cần chứng minh rằng $f$ là *song ánh* và do đó định nghĩa một ánh xạ $g: N \to \mathrm{Hom}(E, F')$ sao cho $f \circ g$ và $g \circ f$ là các ánh xạ đồng nhất. Với mục đích này, lấy $w$ là một phần tử của $N$, tức là một ánh xạ tuyến tính $w: E \to F$ sao cho $v \circ w = 0$. Quan hệ sau tương đương với $w(E) \subset \mathrm{Ker}(v) = u(F')$ theo giả thiết, do đó, vì $u$ đơn ánh, tồn tại duy nhất một ánh xạ tuyến tính $w': E \to F'$ sao cho $w = u \circ w'$ và ta đặt $g(w) = w'$; ngay lập tức kiểm tra được rằng $g$ thỏa mãn các điều kiện mong muốn.

Ngược lại, giả sử rằng dãy (6) là khớp đối với mọi $A$-môđun $E$. Vì $\mathrm{Hom}(1_E, v \circ u) = \bar{v} \circ \bar{u} = 0$, nên $v \circ u \circ w = 0$ với mọi đồng cấu $w: E \to F'$. Lấy $E = F'$ và $w = 1_{F'}$, trước hết ta thấy rằng $v \circ u = 0$ và do đó $u(F') \subset \mathrm{Ker}(v)$. Bây giờ lấy $E = \mathrm{Ker}(v)$ và gọi $\phi: E \to F$ là đơn ánh chính tắc. Khi đó $\bar{v}(\phi) = v \circ \phi = 0$ theo định nghĩa và do đó tồn tại $\psi \in \mathrm{Hom}(E, F')$ sao cho $\phi = \bar{u}(\psi) = u \circ \psi$, điều này hiển nhiên suy ra $\mathrm{Ker}(v) \subset u(F')$ và hoàn tất chứng minh tính khớp của (5) tại $F$. Cuối cùng, nếu $\theta$ là ánh xạ đồng nhất của $\mathrm{Ker}\, u$, thì $\bar{u}(\theta) = 0$, do đó $\theta = 0$ và $\mathrm{Ker}\, u = \{0\}$, điều này chứng minh tính khớp của (5) tại $F'$.

#### Nhận xét {#alg-ii-s2-n1-rem-1 .statement}

(1) Định lý 2 cho phép ta, đối với mọi môđun con F' của F, đồng nhất $\operatorname{Hom}(E, F')$ với một môđun con trên $\mathbf{Z}$ của $\operatorname{Hom}(E, F)$. Khi sự đồng nhất này được thực hiện, thì, đối với mọi họ $(M_\lambda)$ các môđun con của F

$$
\operatorname{Hom}(E, \bigcap_\lambda M_\lambda) = \bigcap_\lambda \operatorname{Hom}(E, M_\lambda)
$$

vì nếu $u \in \operatorname{Hom}(E, F)$ thuộc mỗi $\operatorname{Hom}(E, M_\lambda)$, thì, với mọi $x \in E$, $u(x) \in M_\lambda$ với mọi $\lambda$ và do đó $u$ ánh xạ E vào $\bigcap_\lambda M_\lambda$.

#### Hệ quả {#alg-ii-s2-n1-cor-2 .statement}

*Đối với một ánh xạ A-tuyến tính* $u : E \to F$ *là đơn ánh, điều kiện cần và đủ là, với mọi A-môđun G, ánh xạ* $\operatorname{Hom}(1_G, u) : \operatorname{Hom}(G, E) \to \operatorname{Hom}(G, F)$ *là đơn ánh*.

Chỉ cần áp dụng Định lý 2 cho trường hợp $F' = \{0\}$.

Xuất phát từ một dãy khớp

$$
0 \longrightarrow F' \xrightarrow{u} F \xrightarrow{v} F'' \longrightarrow 0
$$

dãy tương ứng

$$
0 \longrightarrow \operatorname{Hom}(E, F') \xrightarrow{\bar{u}} \operatorname{Hom}(E, F) \xrightarrow{\bar{v}} \operatorname{Hom}(E, F'') \longrightarrow 0
$$

*không nhất thiết khớp*, nói cách khác $\bar{v}$ không nhất thiết toàn ánh. Nếu F' được đồng nhất với một môđun con của F và F'' với môđun thương F/F', điều này có nghĩa là một ánh xạ tuyến tính từ E vào F'' không nhất thiết có dạng $v \circ w$, trong đó $w$ là một ánh xạ tuyến tính từ E vào F. Tuy nhiên:

#### Mệnh đề 2 {#alg-ii-s2-prop-2 .statement}

*Nếu dãy khớp*

(7)

$$
0 \longrightarrow F' \xrightarrow{u} F \xrightarrow{v} F'' \longrightarrow 0
$$

*tách* (nói cách khác, nếu $u(F')$ là một *nhân tử trực tiếp* của F), *dãy*

(8)

$$
0 \longrightarrow \operatorname{Hom}(E, F') \xrightarrow{\bar{u}} \operatorname{Hom}(E, F) \xrightarrow{\bar{v}} \operatorname{Hom}(E, F'') \longrightarrow 0
$$

*là khớp và tách*. *Ngược lại, nếu dãy* (8) *là khớp đối với mọi A-môđun E, dãy khớp* (7) *tách*.

Mệnh đề đầu tiên suy ra từ sự kiện rằng

$$
\operatorname{Hom}(E, F') \oplus \operatorname{Hom}(E, F'')
$$

được đồng nhất một cách chính tắc với $\operatorname{Hom}(E, F' \oplus F'')$ nhờ ánh xạ $\mathbf{Z}$-tuyến tính $\operatorname{Hom}(1_E, j') + \operatorname{Hom}(1_E, j''), j' : F' \to F' \oplus F''$ và $j'' : F'' \to F' \oplus F''$ lần lượt là các đơn ánh chính tắc (§ 1, no. 6, Hệ quả 1 của Mệnh đề 6). Ngược lại, nếu dãy (8) là khớp với $E = F''$, thì tồn tại một phần tử $g \in \operatorname{Hom}(F'', F)$ sao cho $v \circ g = 1_{F''}$ và kết luận suy ra từ § 1, no. 9, Mệnh đề 15.

Nhận xét (2). Các kết quả của no. này có giá trị không thay đổi đối với mọi nhóm giao hoán có toán tử.

### 2. CÁC MÔĐUN XẠ ẢNH

#### Định nghĩa 1 {#alg-ii-s2-def-1 .statement}

Một A-môđun P được gọi là xạ ảnh nếu, đối với mọi dãy khớp F' → F → F'' của các ánh xạ A-tuyến tính, dãy

$$
\operatorname{Hom}(P, F') \to \operatorname{Hom}(P, F) \to \operatorname{Hom}(P, F'')
$$

là khớp.

#### Mệnh đề 3 {#alg-ii-s2-prop-3 .statement}

Đối với một A-môđun P, tổng trực tiếp của một họ các môđun con $(M_i)$ là xạ ảnh khi và chỉ khi mỗi $M_i$ là xạ ảnh.

Đối với mọi đồng cấu A-môđun $u : E \to F$,

$$
\operatorname{Hom}(1_P, u) : \operatorname{Hom}(P, E) \to \operatorname{Hom}(P, F)
$$

được đồng nhất với $\prod_i \operatorname{Hom}(1_{M_i}, u)$ (\S 1, no. 6, Hệ quả 1 của Mệnh đề 6); do đó kết luận suy ra từ Định nghĩa 1 và \S 1, no. 5, Mệnh đề 5 (ii).

#### Hệ quả {#alg-ii-s2-n2-cor-1 .statement}

Mọi A-môđun tự do đều là xạ ảnh.

Theo Mệnh đề 3, chỉ cần chứng minh rằng $A_s$ là xạ ảnh, điều này suy ra ngay lập tức từ tính giao hoán của biểu đồ (50) của \S 1, no. 14.

#### Mệnh đề 4 {#alg-ii-s2-prop-4 .statement}

Cho P là một A-môđun. Các tính chất sau là tương đương:

(a) P là xạ ảnh.
(b) Đối với mọi dãy khớp $0 \to F' \to F \to F'' \to 0$ của các ánh xạ A-tuyến tính, dãy

$$
0 \to \operatorname{Hom}(P, F') \to \operatorname{Hom}(P, F) \to \operatorname{Hom}(P, F'') \to 0
$$

là khớp.

(c) Đối với mọi đồng cấu A-môđun toàn ánh $u : E \to E''$ và mọi đồng cấu $f : P \to E''$, tồn tại một đồng cấu $g : P \to E$ sao cho $f = u \circ g$ (người ta nói rằng $f$ có thể được "nâng" thành một đồng cấu từ P vào E).

(d) Mọi dãy khớp $0 \to E' \to E \to P \to 0$ của các ánh xạ A-tuyến tính đều tách (và do đó P đẳng cấu với một nhân tử trực tiếp của E).

(e) P đẳng cấu với một nhân tử trực tiếp của một A-môđun tự do.

Hiển nhiên rằng (a) kéo theo (b). Để thấy rằng (b) kéo theo (c), chỉ cần áp dụng (b) cho dãy khớp $0 \to E' \to E \to E'' \to 0$, trong đó $E' = Ker(u)$, vì (c) biểu thị rằng

$$
\operatorname{Hom}(1_P, u) : \operatorname{Hom}(P, E) \to \operatorname{Hom}(P, E'')
$$

là toàn ánh. Để thấy rằng (c) kéo theo (d), chỉ cần áp dụng (c) cho đồng cấu toàn ánh $v : E \to P$ và đồng cấu $l_P : P \to P$; sự tồn tại của một đồng cấu $g : P \to E$ sao cho $l_P = v \circ g$ kéo theo rằng dãy

$$
0 \longrightarrow E' \longrightarrow E \xrightarrow{v} P \longrightarrow 0
$$

tách (\S 1, no. 9, Mệnh đề 15). Vì đối với mọi A-môđun M tồn tại một A-môđun tự do L và một dãy khớp $0 \to R \to L \to M \to 0$ (\S 1, no. 11, Mệnh đề 20), rõ ràng (d) kéo theo (e). Cuối cùng (e) kéo theo (a) theo Mệnh đề 3 và Hệ quả của nó.

#### Hệ quả 1 {#alg-ii-s2-prop-4-cor-1 .statement}

*Để một A-môđun là xạ ảnh và sinh hữu hạn, điều kiện cần và đủ là nó là một nhân tử trực tiếp của một A-môđun tự do có một cơ sở hữu hạn.*

Điều kiện này hiển nhiên là đủ; ngược lại, một môđun xạ ảnh hữu hạn sinh E đẳng cấu với một môđun thương của một môđun tự do F có một cơ sở hữu hạn (\S 1, no. 11) và E đẳng cấu với một nhân tử trực tiếp của F theo Mệnh đề 4 (d).

#### Hệ quả 2 {#alg-ii-s2-prop-4-cor-2 .statement}

*Cho C là một vành giao hoán và E, F là hai C-môđun xạ ảnh hữu hạn sinh; khi đó $\operatorname{Hom}_C(E, F)$ là một C-môđun xạ ảnh hữu hạn sinh.*

Có thể giả sử rằng tồn tại hai C-môđun tự do hữu hạn sinh M, N sao cho $M = E \oplus E', N = F \oplus F'$; từ \S 1, no. 6, Hệ quả 1 của Mệnh đề 6 suy ra rằng $\operatorname{Hom}_C(M, N)$ là hữu hạn sinh và tự do, và mặt khác rằng $\operatorname{Hom}_C(M, N)$ đẳng cấu với

$$
\operatorname{Hom}_C(E, F) \oplus \operatorname{Hom}_C(E', F) \oplus \operatorname{Hom}_C(E, F') \oplus \operatorname{Hom}(E', F'),
$$

do đó có hệ quả.

### 3. CÁC DẠNG TUYẾN TÍNH; ĐỐI NGẪU CỦA MỘT MÔĐUN

Cho E là một A-môđun *trái*. Vì A là một song môđun $(A, A)$, $\operatorname{Hom}_A(E, A_s)$ có một cấu trúc A-môđun *phải* chính tắc (\S 1, no. 14).

#### Định nghĩa 2 {#alg-ii-s2-def-2 .statement}

*Đối với mọi A-môđun phải E, A-môđun phải $\operatorname{Hom}_A(E, A_s)$ được gọi là môđun đối ngẫu của E* (hoặc đơn giản là *đối ngẫu†* của E) *và các phần tử của nó được gọi là các dạng tuyến tính trên E*.

Nếu E là một A-môđun *phải*, tập hợp $\operatorname{Hom}_A(E, A_d)$ với cấu trúc A-môđun *trái* chính tắc của nó cũng được gọi là *đối ngẫu* của E và các phần tử của nó được gọi là *các dạng tuyến tính* trên E.

† Trong *Không gian vectơ tôpô*, IV, ta sẽ định nghĩa, đối với các không gian vectơ có một *tôpô*, một khái niệm "không gian đối ngẫu" sẽ phụ thuộc vào tôpô này và sẽ phân biệt với khái niệm được định nghĩa ở đây. Người đọc phải cẩn thận không áp dụng một cách thiếu thận trọng cho không gian đối ngẫu "tôpô" các tính chất của đối ngẫu "đại số" được thiết lập trong đoạn này.

Trong chương này, $E^*$ sẽ được dùng để ký hiệu đối ngẫu của một A-môđun (trái hoặc phải) $E$.

#### Ví dụ {#alg-ii-s2-n3-exa-1 .statement}

*Trên không gian vectơ (đối với trường $\mathbf{R}$) của các hàm liên tục nhận giá trị thực trên một khoảng $[a, b]$ của $\mathbf{R}$, ánh xạ $x \mapsto \int_a^b x(t) dt$ là một dạng tuyến tính.*

Cho $E$ là một A-môđun trái và $E^*$ là đối ngẫu của nó; đối với mọi cặp có thứ tự các phần tử $x \in E, x^* \in E^*$, phần tử $x^*(x)$ của A được ký hiệu bởi $\langle x, x^* \rangle$. Khi đó các hệ thức

$$
\begin{align*}
(9) \quad & \langle x + y, x^* \rangle = \langle x, x^* \rangle + \langle y, x^* \rangle \\
(10) \quad & \langle x, x^* + y^* \rangle = \langle x, x^* \rangle + \langle x, y^* \rangle \\
(11) \quad & \langle \alpha x, x^* \rangle = \alpha \langle x, x^* \rangle \\
(12) \quad & \langle x, x^* \alpha \rangle = \langle x, x^* \rangle \alpha
\end{align*}
$$

đúng với $x, y$ trong $E, x^*, y^*$ trong $E^*$ và $\alpha \in A$. Ánh xạ $(x, x^*) \mapsto \langle x, x^* \rangle$ từ $E \times E^*$ vào $A$ được gọi là dạng song tuyến tính chính tắc trên $E \times E^*$ (khái niệm dạng song tuyến tính sẽ được định nghĩa nói chung trong IX, § 1). Mọi dạng tuyến tính $x^*$ trên $E$ đều có thể được xem như ánh xạ riêng phần $x \mapsto \langle x, x^* \rangle$ tương ứng với dạng song tuyến tính chính tắc.

Khi $E$ là một A-môđun phải, giá trị $x^*(x)$ của một dạng tuyến tính $x^* \in E^*$ tại một phần tử $x \in E$ được ký hiệu bởi $\langle x^*, x \rangle$ và các công thức tương ứng với (11) và (12) được viết là

$$
\begin{align*}
\langle x^*, x \alpha \rangle &= \langle x^*, x \rangle \alpha \\
\langle \alpha x^*, x \rangle &= \alpha \langle x^*, x \rangle.
\end{align*}
$$

Khi A giao hoán, cả hai ký hiệu đều được phép dùng.

#### Mệnh đề 5 {#alg-ii-s2-prop-5 .statement}

Với mọi vành A, ánh xạ gán cho mỗi $\xi \in A$ dạng tuyến tính $\eta \mapsto \eta \xi$ trên $A_s$ là một đẳng cấu từ $A_d$ lên đối ngẫu của $A_s$.

Đây là trường hợp riêng của đẳng cấu chính tắc $E \to \mathrm{Hom}_A(A_s, E)$ của § 1, no. 14, Nhận xét 2, tương ứng với $E = A_s$; tính giao hoán của biểu đồ (50) của § 1, no. 14, cho thấy ở đây ta có một đẳng cấu của các A-môđun phải.

Nếu $A_d$ được đồng nhất với đối ngẫu của $A_s$ nhờ đẳng cấu của Mệnh đề 5, thì dạng song tuyến tính chính tắc trên $A_s \times A_d$ khi đó được biểu diễn bởi

$$
\langle \xi, \xi^* \rangle = \xi \xi^* \quad \text{với } \xi, \xi^* \text{ trong } A.
$$

Tương tự, đối ngẫu của $A_d$ được đồng nhất một cách chính tắc với $A_s$, dạng song tuyến tính chính tắc trên $A_d \times A_s$ được biểu diễn bởi

$$
\langle \xi^*, \xi \rangle = \xi^* \xi \quad \text{với } \xi, \xi^* \text{ trong } A.
$$

### 4. TÍNH TRỰC GIAO

#### Định nghĩa 3 {#alg-ii-s2-def-3 .statement}

Cho E là một A-môđun và E* là đối ngẫu của nó; một phần tử x ∈ E và một phần tử x* ∈ E* được gọi là trực giao nếu ⟨x, x*⟩ = 0.

Một tập con M của E và một tập con M' của E* được gọi là các tập hợp trực giao nếu, với mọi x ∈ M, x* ∈ M', x và x* trực giao. Đặc biệt, x* ∈ E* (tương ứng x ∈ E) được gọi là trực giao với M (tương ứng M') nếu nó trực giao với mọi phần tử của M (tương ứng M'). Nếu x* và y* trực giao với M, thì x* + y* và x*α cũng trực giao với M với mọi α ∈ A theo (10) và (12) (no. 3), điều này dẫn đến định nghĩa sau:

#### Định nghĩa 4 {#alg-ii-s2-def-4 .statement}

Cho một tập con M của E (tương ứng một tập con M' của E*), tập hợp các x* ∈ E* (tương ứng tập hợp các x ∈ E) trực giao với M (tương ứng M') được gọi là môđun con hoàn toàn trực giao với M (tương ứng M') (hoặc đơn giản là môđun con trực giao với M (tương ứng M') nếu không thể gây nhầm lẫn).

Theo định nghĩa của một dạng tuyến tính, môđun con của E* trực giao với E là 0; môđun con của E* trực giao với {0} đồng nhất với E*.

#### Mệnh đề 6 {#alg-ii-s2-prop-6 .statement}

Cho M, N là hai tập con của E sao cho M ⊂ N; nếu M' và N' lần lượt là các môđun con của E* trực giao với M và N, thì N' ⊂ M'.

#### Mệnh đề 7 {#alg-ii-s2-prop-7 .statement}

Cho (M_i) là một họ các tập con của E; môđun con trực giao với hợp của các M_i là giao của các môđun con M'_i lần lượt trực giao với các M_i; môđun con này cũng là môđun con trực giao với môđun con của E được sinh bởi hợp của các M_i.

Các kết quả này là những hệ quả ngay lập tức của các định nghĩa.

Có một mệnh đề tương tự (ta để người đọc tự phát biểu) đối với các môđun con của E trực giao với các tập con của E*.

Nếu M là một môđun con của E, M' là môđun con của E* trực giao với M và M'' là môđun con của E trực giao với M', thì M ⊂ M'' nhưng có thể M ≠ M'' (Bài tập 9). Tuy nhiên, lưu ý rằng nếu M'' là trực giao của M'' trong E*, thì M'' = M'; vì M' ⊂ M'' và mặt khác quan hệ M ⊂ M'' kéo theo M'' ⊂ M'.

### 5. ÁNH XẠ TUYẾN TÍNH CHUYỂN VỊ

Cho E, F là hai A-môđun trái; với mọi ánh xạ tuyến tính u : E → F, ánh xạ Hom(u, l_{A_s}) là một ánh xạ tuyến tính từ A-môđun phải F* vào A-môđun phải E* (§ 1, no. 2), được gọi là ánh xạ chuyển vị của u.

Nói cách khác:

#### Định nghĩa 5 {#alg-ii-s2-def-5 .statement}

Với mọi ánh xạ tuyến tính u của một A-môđun E vào một A-môđun F, ánh xạ tuyến tính y* ↦ y* ∘ u từ đối ngẫu F* của F vào đối ngẫu E* của E được gọi là ánh xạ chuyển vị của u và được ký hiệu là t u.

Ánh xạ chuyển vị $^t u$ do đó được định nghĩa bởi quan hệ
(15) $$
\langle u(x), y^* \rangle = \langle x, ^t u(y^*) \rangle \quad \text{với mọi } x \in E \text{ và mọi } y^* \in F^*.
$$

Định nghĩa 5 áp dụng không thay đổi cho các A-môđun phải và khi đó tương đương với quan hệ
$$
\langle y^*, u(x) \rangle = \langle ^t u(y^*), x \rangle \quad \text{với mọi } x \in E \text{ và mọi } y^* \in F^*.
$$

Các công thức (9) và (10) của § 1, no. 2 ở đây cho
(16) $$
^t(u_1 + u_2) = ^t u_1 + ^t u_2
$$
đối với hai phần tử $u_1, u_2$ của $\mathrm{Hom}_A(E, F)$ và
(17) $$
^t(v \circ u) = ^t u \circ ^t v
$$
đối với $u \in \mathrm{Hom}_A(E, F)$ và $v \in \mathrm{Hom}_A(F, G)$, trong đó G là một A-môđun thứ ba; cuối cùng, rõ ràng
(18) $$
^t 1_E = 1_{E^*}.
$$

#### Nhận xét {#alg-ii-s2-n5-rem-1 .statement}

Từ (17) và (18) suy ra rằng nếu $u$ khả nghịch trái (tương ứng phải), thì $^t u$ khả nghịch phải (tương ứng trái).

#### Mệnh đề 8 {#alg-ii-s2-prop-8 .statement}

*Cho $u : E \to F$ là một ánh xạ A-tuyến tính, M một môđun con của E và $M'$ là trực giao của M trong $E^*$; trực giao của $u(M)$ trong $F^*$ là ảnh ngược $^t u^{-1}(M')$.*

Điều này suy ra ngay lập tức từ (15).

#### Hệ quả {#alg-ii-s2-n5-cor-1 .statement}

*Trực giao của ảnh $u(E)$ trong $F^*$ là hạt nhân $^t u^{-1}(0)$ của $^t u$.*

Trực giao của E trong $E^*$ là 0.

Nếu $u : E \to F$ là một đẳng cấu, $^t u : F^* \to E^*$ là một đẳng cấu và nếu $v : F \to E$ là đẳng cấu nghịch đảo của $u$, $^t v$ là đẳng cấu nghịch đảo của $^t u$ (các công thức (17) và (18)).

#### Định nghĩa 6 {#alg-ii-s2-def-6 .statement}

*Một đẳng cấu đối ngẫu của một A-môđun E lên một A-môđun F, chuyển vị của đẳng cấu nghịch đảo của u (bằng đẳng cấu nghịch đảo của chuyển vị của u) được gọi là đẳng cấu đối phản của u và được ký hiệu bởi $\tilde{u}$.*

Đẳng cấu $\tilde{u}$ do đó được đặc trưng bởi quan hệ
(19) $$
\langle u(x), \tilde{u}(y^*) \rangle = \langle x, x^* \rangle \quad \text{cho } x \in E, x^* \in E^*.
$$

Nếu $v : F \to G$ là một đẳng cấu, đẳng cấu đối phản của $v \circ u$ là $\tilde{v} \circ \tilde{u}$.

Đặc biệt, ánh xạ $u \mapsto \tilde{u}$ là một *đẳng cấu* của nhóm tuyến tính $\mathbf{GL}(E)$ lên một nhóm con của nhóm tuyến tính $\mathbf{GL}(E^*)$.

Cho $\sigma : A \to B$ là một *đẳng cấu* của một vành $A$ lên một vành $B$, $E$ là một $A$-môđun trái, $F$ là một $B$-môđun trái và $u : E \to F$ là một ánh xạ *nửa tuyến tính* (\S 1, no. 13) *đối với* $\sigma$. Gọi $\sigma^{-1}$ là đẳng cấu nghịch đảo của $\sigma$; với mọi $y^* \in F^*$, ánh xạ $x \mapsto \langle u(x), y^* \rangle^{\sigma^{-1}}$ của $E$ vào $A$ là một *dạng tuyến tính*; nếu nó cũng được ký hiệu là ${}^t u(y^*)$, một ánh xạ ${}^t u : F^* \to E^*$ được xác định, cũng được gọi là *chuyển vị* của ánh xạ nửa tuyến tính $u$; do đó nó được đặc trưng bởi đồng nhất thức

$$
\langle u(x), y^* \rangle = \langle x, {}^t u(y^*) \rangle^\sigma
$$

với $x \in E, y^* \in F^*$. Người ta kiểm tra ngay lập tức rằng ${}^t u$ là một ánh xạ *nửa tuyến tính* *đối với* $\sigma^{-1}$. Nếu $v$ ký hiệu ánh xạ $u$ được xem như một ánh xạ *A-tuyến tính* của $E$ vào $\sigma_*(F)$ (\S 1, no. 13), ta có thể viết $u = \phi \circ v$, trong đó $\phi$ là ánh xạ đồng nhất $\sigma_*(F) \to F$, được xem như một ánh xạ nửa tuyến tính đối với $\sigma$. Hiển nhiên rằng ${}^t u = {}^t v \circ {}^t \phi$ và $({}^t \phi, \sigma^{-1})$ là một song đẳng cấu của $F^*$ lên $(\sigma_*(F))^*$ đối với đẳng cấu $\sigma^{-1}$; quan hệ này cho phép ta ngay lập tức mở rộng các tính chất của các chuyển vị của các ánh xạ tuyến tính sang các chuyển vị của các ánh xạ nửa tuyến tính.

### 6. ĐỐI NGẪU CỦA MÔĐUN THƯƠNG. ĐỐI NGẪU CỦA TỔNG TRỰC TIẾP. CÁC CƠ SỞ ĐỐI NGẪU

Ta áp dụng Định lý 1 của no. 1 cho trường hợp $F = A_s$:

#### Mệnh đề 9 {#alg-ii-s2-prop-9 .statement}

*Cho* $E', E, E''$ *là các A-môđun và*

$$
E' \xrightarrow{u} E \xrightarrow{v} E'' \longrightarrow 0
$$

*là một dãy khớp của các ánh xạ tuyến tính.* *Khi đó dãy các ánh xạ chuyển vị*

$$
0 \longrightarrow {E''}^* \xrightarrow{{}^t v} E^* \xrightarrow{{}^t u} {E'}^*
$$

*là khớp.*

#### Hệ quả {#alg-ii-s2-n6-cor-1 .statement}

*Cho M là một môđun con của một A-môđun E và $\phi : E \to E/M$ là đồng cấu chính tắc. Khi đó* ${}^t \phi$ *là một đẳng cấu của đối ngẫu của* $E/M$ *lên môđun con* $M'$ *của* $E^*$ *trực giao với* $M$.

Nếu $j : M \to E$ là đơn ánh chính tắc, hạt nhân của ${}^t j$ theo định nghĩa là trực giao của $M$ trong $E^*$.

Hơn nữa, trong ký hiệu của hệ quả, một đồng cấu *đơn ánh* $E^*/M' \to M^*$ thu được từ ${}^t j$ khi chuyển qua thương.

#### Mệnh đề 10 {#alg-ii-s2-prop-10 .statement}

*Cho* $(E_i)_{i \in I}$ *là một họ các A-môđun và với mọi* $i \in I$ *cho* $j_i : E_i \to E = \bigoplus_{i \in I} E_i$ *là đơn ánh chính tắc.* *Khi đó ánh xạ tích* $x^* \mapsto ({}^t j_i(x^*))$

*là một đẳng cấu của đối ngẫu* $E^*$ *của* $E$ *lên tích* $\prod_{i \in I} E_i^*$.

Đây là một trường hợp riêng của § 1, no. 6, Hệ quả 1 của Mệnh đề 6, áp dụng cho trường hợp $\prod_{\lambda} F_{\lambda} = A_s$.

Nếu, bằng các đơn ánh chính tắc $j_i$, các $E_i$ được đồng nhất với các môđun con của tổng trực tiếp của chúng $E$ và nếu, bằng ánh xạ tích $x^* \mapsto (tj_i(x^*))$, $E^*$ được đồng nhất với $\prod_{i \in I} E_i^*$, thì khi đó có thể nói rằng $\prod_{i \in I} E_i^*$ là đối ngẫu của $\bigoplus_{i \in I} E_i$, dạng song tuyến tính chính tắc được cho bởi

$$
\langle (x_i), (x_i^*) \rangle = \sum_{i \in I} \langle x_i, x_i^* \rangle.
$$

(22)

#### Hệ quả {#alg-ii-s2-n6-cor-2 .statement}

*Cho M, N là hai môđun con bù nhau trong một A-môđun E và $p : E \to M, q : E \to N$ là các phép chiếu tương ứng; khi đó $^tp + ^tq : M^* \oplus N^* \to E^*$ là một đẳng cấu và $^tp$ (tương ứng $^tq$) là một đẳng cấu của $M^*$ (tương ứng $N^*$) lên môđun con của $E^*$ trực giao với $N$ (tương ứng $M$). Hơn nữa, nếu $i : M \to E$ và $j : N \to E$ là các đơn ánh chính tắc, $^tp \circ ^ti$ và $^tq \circ ^tj$ là các phép chiếu $E^* \to ^tp(M^*)$, $E^* \to ^tq(N^*)$ tương ứng với phân tích của $E^*$ thành tổng trực tiếp của $^tp(M^*)$ và $^tq(N^*)$.

$p \circ i = 1_M, \quad q \circ j = 1_N, \quad p \circ j = q \circ i = 0, \quad i \circ p + j \circ q = 1_E$, do đó, bằng chuyển vị (no. 5, các công thức (16), (17) và (18)), $^ti \circ ^tp = 1_{M^*}, \ ^tj \circ ^tq = 1_{N^*}, \ ^tj \circ ^tp = ^ti \circ ^tq = 0. \ ^tp \circ ^ti + ^tq \circ ^tj = 1_{E^*}$ và mệnh đề suy ra từ § 1, no. 6, Hệ quả 2 của Mệnh đề 6.

Dưới các giả thiết của Hệ quả, $M^*$ (tương ứng $N^*$) thường được đồng nhất với trực giao $^tp(M^*)$ (tương ứng $^tq(N^*)$) của $N$ (tương ứng $M$) trong $E^*$, do đó đồng nhất mỗi dạng tuyến tính $u$ trên $M$ (tương ứng $N$) với dạng tuyến tính trên $E$ mở rộng $u$ và bằng không trên $N$ (tương ứng $M$).

Khi một A-môđun $E$ có một *cơ sở* $(e_t)_{t \in T}$, ta đã thấy rằng việc cho cơ sở này xác định một cách chính tắc một đẳng cấu $u : A_s^{(T)} \to E$. Theo Mệnh đề 10 và no. 3, Mệnh đề 5, đối ngẫu của $A_s^{(T)}$ được đồng nhất một cách chính tắc với tích $A_d^T$; xét đẳng cấu đối ngẫu $\tilde{u} : A_d^T \to E^*$. Nếu, với mọi $t \in T, f_t$ là phần tử của $A_d^T$ mà mọi phép chiếu của nó đều bằng không, ngoại trừ phép chiếu có chỉ số $t$, bằng 1, và nếu ta viết $e_t^* = \tilde{u}(f_t)$, thì các phần tử $e_t^*$ của $E^*$, theo (19) và (22), được đặc trưng bởi các hệ thức

$$
\langle e_t, e_{t'}^* \rangle = \begin{cases}
0 & \text{với } t' \neq t \\
1 & \text{với } t' = t.
\end{cases}
$$

(23)

Nói cách khác, với mọi $x = \sum_{t \in T} \xi_t e_t \in E, \ e_t^*(x) = \xi_t$; $e_t^*$ cũng được gọi là *dạng tọa độ* có chỉ số $t$ trên $E$. Từ (23) suy ra rằng $(e_t^*)$ là một *hệ tự do* trong $E^*$.

Đặc biệt, nếu $T$ là *hữu hạn*, thì $e_t^*$ tạo thành một *cơ sở* của $E^*$, khi đó $f_t$ tạo thành cơ sở chính tắc của $A_d^T$. Do đó:

#### Mệnh đề 11 {#alg-ii-s2-prop-11 .statement}

*Đối ngẫu của một môđun tự do có cơ sở gồm n phần tử là một môđun tự do có cơ sở gồm n phần tử.*

Chú ý rằng đối ngẫu của một môđun tự do có cơ sở vô hạn không nhất thiết là một môđun tự do (VII, § 3, Bài tập 10).

#### Định nghĩa 7 {#alg-ii-s2-def-7 .statement}

*Nếu E là một môđun tự do có cơ sở hữu hạn* $(e_t)$, *thì cơ sở* $(e_t^*)$ *của môđun đối ngẫu E* *của E được xác định bởi các hệ thức (23) được gọi là cơ sở đối ngẫu của* $(e_t)$.

Các hệ thức (23) cũng có thể được viết dưới dạng
$$
\langle e_t, e_{t'}^* \rangle = \delta_{tt'}
$$
trong đó $\delta_{tt'}$ là *ký hiệu Kronecker* trên $T \times T$.

Chú ý rằng nếu $T$ hữu hạn và $(e_t^*)$ là cơ sở đối ngẫu của $(e_t)$, thì, với
$$ x = \sum_{t \in T} \xi_t e_t \in E, \quad x^* = \sum_{t \in T} \xi_t^* e_t^* \in E^*, $$
$$
\langle x, x^* \rangle = \sum_{t \in T} \xi_t \xi_t^*.
$$

Cơ sở đối ngẫu của một cơ sở hữu hạn của một A-môđun *phải* tất nhiên được định nghĩa tương tự.

#### Hệ quả {#alg-ii-s2-n6-cor-3 .statement}

*Đối ngẫu của một môđun xạ ảnh hữu hạn sinh là một môđun xạ ảnh hữu hạn sinh.*

Một A-môđun trái xạ ảnh sinh hữu hạn có thể được đồng nhất với một nhân tử trực tiếp M của một A-môđun tự do $A_s^n$ có cơ sở hữu hạn (no. 2, Hệ quả 1 của Mệnh đề 4). Khi đó (Mệnh đề 11 và Hệ quả của Mệnh đề 10) M* đẳng cấu với một nhân tử trực tiếp của $A_d^n$, do đó có hệ quả.

#### Mệnh đề 12 {#alg-ii-s2-prop-12 .statement}

*Cho E là một A-môđun và* $(a_t)_{t \in T}$ *là một hệ sinh của E. Các điều kiện sau là tương đương:*
(a) *E là một A-môđun xạ ảnh.*
(b) *Tồn tại một họ* $(a_t^*)_{t \in T}$ *các dạng tuyến tính trên E sao cho, với mọi* $x \in E$, *họ* $(\langle x, a_t^* \rangle)_{t \in T}$ *có giá hữu hạn và*
$$
x = \sum_{t \in T} \langle x, a_t^* \rangle a_t.
$$

Tồn tại một đồng cấu toàn ánh $u : L \to E$, trong đó $L = A_s^{(T)}$, sao cho nếu $(e_t)_{t \in T}$ là cơ sở chính tắc của L thì $u(e_t) = a_t$ (\S 1, no. 11, Mệnh đề 17); để E là xạ ảnh, điều kiện cần và đủ là tồn tại một ánh xạ tuyến tính $v : E \to L$ sao cho $u \circ v = 1_E$ (no. 2, Mệnh đề 4 và \S 1, no. 9, Mệnh đề 15). Nếu tồn tại một ánh xạ như vậy và ta viết ${}^tv(e_t^*) = a_t^*$, thì $\langle x, a_t^* \rangle = \langle x, {}^tv(e_t^*) \rangle = \langle v(x), e_t^* \rangle$, do đó họ $(\langle x, a_t^* \rangle)$ có giá hữu hạn và $x = u \left( \sum_{t \in T} \langle (x), e_t^* \rangle e_t \right) = \sum_{t \in T} \langle x, a_t^* \rangle a_t$ với mọi $x \in E$. Ngược lại, nếu điều kiện (b) của mệnh đề được thỏa mãn, tổng $\sum_{t \in T} \langle x, a_t^* \rangle e_t$ được xác định với mọi $x \in E$ và $x \to \sum_{t \in T} \langle x, a_t^* \rangle e_t$ là một ánh xạ tuyến tính $v : E \to L$ sao cho $u \circ v = 1_E$.

### 7. ĐỐI ĐẲNG DUAL

Cho E là một A-môđun trái. Đối ngẫu $E^{**}$ của môđun đối ngẫu $E^*$ của E được gọi là môđun bidual của E; nó cũng là một A-môđun trái (no. 3). Với mọi $x \in E$, suy ra từ no. 3, các công thức (10) và (12), rằng ánh xạ $x^* \mapsto \langle x, x^* \rangle$ là một dạng tuyến tính trên A-môđun phải $E^*$, nói cách khác là một phần tử của bidual $E^{**}$, mà ta sẽ ký hiệu bởi $\tilde{x}$; hơn nữa, suy ra ngay từ (9) và (11) (no. 3) rằng ánh xạ $c_E : x \mapsto \tilde{x}$ của E vào $E^{**}$ là tuyến tính; ánh xạ này sẽ được gọi là chính tắc; nói chung, nó không đơn ánh cũng không toàn ánh, ngay cả khi E là sinh hữu hạn (xem Bài tập 9(e) và § 7, no. 5, Định lý 6).

Một A-môđun E được gọi là phản xạ nếu đồng cấu chính tắc $c_E : E \to E^{**}$ là song ánh.

Cho F là một A-môđun trái thứ hai; với mọi ánh xạ tuyến tính $u : E \to F$, ánh xạ $t(tu) : E^{**} \to F^{**}$, cũng sẽ được ký hiệu bởi $tu$, là tuyến tính và biểu đồ

$$
\begin{array}{ccc}
E & \xrightarrow{u} & F \\
c_E \downarrow & & \downarrow c_F \\
E^{**} & \xrightarrow{tu} & F^{**}
\end{array}
$$

là giao hoán, như suy ra ngay từ các định nghĩa và công thức (15) cho chuyển vị của một ánh xạ tuyến tính.

#### Mệnh đề 13 {#alg-ii-s2-prop-13 .statement}

*Nếu E là một môđun tự do* (tương ứng *một môđun tự do có cơ sở hữu hạn*), *ánh xạ chính tắc* $c_E : E \to E^{**}$ *là đơn ánh* (tương ứng *song ánh*).

Cho $(e_t)_{t \in T}$ là một cơ sở của E và cho $(e_t^*)$ là họ các dạng tọa độ tương ứng; theo định nghĩa, nếu $x \in E$ là sao cho $\tilde{x} = 0$, thì $\langle x, e_t^* \rangle = 0$ với mọi $t \in T$, nói cách khác mọi tọa độ của $x$ đều bằng không, do đó $x = 0$. Giả sử thêm rằng T là hữu hạn; vì $\langle \tilde{e}_t, e_{t'}^* \rangle = \delta_{tt'}$, $(\tilde{e}_t)$ là cơ sở đối ngẫu của $(e_t^*)$ trong $E^{**}$ và, vì $c_E$ biến một cơ sở của E thành một cơ sở của $E^{**}$, $c_E$ là song ánh (\S 1, no. 11, Hệ quả 3 của Mệnh đề 17). Ta còn đã chứng minh được:

#### Hệ quả 1 {#alg-ii-s2-prop-13-cor-1 .statement}

*Cho E là một A-môđun tự do có một cơ sở hữu hạn; với mọi cơ sở* $(e_t)$ *của E, $(c_E(e_t))$ *là cơ sở đối ngẫu của cơ sở* $(e_t^*)$ *của* $E^*$ *đối ngẫu với* $(e_t)$.

Trong trường hợp này người ta nói rằng $(e_t)$ và $(e_t^*)$ là hai *cơ sở đối ngẫu của nhau*.

#### Hệ quả 2 {#alg-ii-s2-prop-13-cor-2 .statement}

*Nếu E là một A-môđun tự do có một cơ sở hữu hạn, mọi cơ sở hữu hạn của E* là cơ sở đối ngẫu của một cơ sở của E.*

Chỉ cần xét trong E** cơ sở đối ngẫu của cơ sở đã cho và đồng nhất một cách chính tắc E với E**.

#### Hệ quả 3 {#alg-ii-s2-prop-13-cor-3 .statement}

*Cho E, F là hai A-môđun mỗi môđun có một cơ sở hữu hạn, E (tương ứng F) được đồng nhất một cách chính tắc với bidual E** (tương ứng F**). Khi đó, với mọi ánh xạ tuyến tính u : E → F, $t^t u = u$.*

Điều này suy ra ngay từ tính giao hoán của biểu đồ (27).

#### Hệ quả 4 {#alg-ii-s2-prop-13-cor-4 .statement}

*Nếu P là một môđun xạ ảnh* (tương ứng *một môđun xạ ảnh sinh hữu hạn*) *ánh xạ chính tắc* $c_P : P \to P**$ *là đơn ánh* (tương ứng *song ánh*).

Ta sẽ sử dụng bổ đề sau:

#### Bổ đề 1 {#alg-ii-s2-lem-1 .statement}

*Cho M, N là hai môđun con bù nhau trong một A-môđun E và i : M → E, j : N → E là các phép nhúng chính tắc. Khi đó biểu đồ*

$$
\begin{array}{ccc}
M \oplus N & \xrightarrow{c_M \oplus c_N} & M** \oplus N** \\
i + j \downarrow & & \uparrow t_{i_1} + t_{j_1} \\
E & \xrightarrow{c_E} & E**
\end{array}
$$

(28)

*là giao hoán.*

Theo định nghĩa, với $x \in M, y \in N, z^* \in E*$,

$$
\begin{align*}
\langle c_E(i(x) + j(y)), z^* \rangle &= \langle i(x) + j(y), z^* \rangle \\
&= \langle i(x), z^* \rangle + \langle j(y), z^* \rangle \\
&= \langle x, t_i(z^*) \rangle + \langle y, t_j(z^*) \rangle \\
&= \langle c_M(x), t_i(z^*) \rangle + \langle c_N(y), t_j(z^*) \rangle \\
&= \langle t_i(c_M(x)) + t_j(c_N(y)), z^* \rangle.
\end{align*}
$$

Điều này đúng như vậy, nếu E là một môđun tự do (tương ứng một môđun tự do có một cơ sở hữu hạn), $c_E$ là đơn ánh (tương ứng song ánh); mặt khác, suy ra từ no. 6, Mệnh đề 10, rằng $t_i \oplus t_j$ là song ánh; tính giao hoán của biểu đồ (28) khi đó kéo theo rằng $c_M \oplus c_N$ là đơn ánh (tương ứng song ánh) và do đó $c_M$ và $c_N$ cũng vậy (\S 1, no. 6, Hệ quả 1 của Mệnh đề 7), do đó có hệ quả, xét đến no. 2, Mệnh đề 4.

### 8. CÁC PHƯƠNG TRÌNH TUYẾN TÍNH

Cho E, F là hai A-môđun. Mọi phương trình có dạng $u(x) = y_0$, trong đó $u : E \to F$ là một ánh xạ tuyến tính đã cho, $y_0$ là một phần tử đã cho của F và ẩn $x$ chịu điều kiện rằng nó nhận các giá trị trong E, được gọi là một phương trình *tuyến tính*; $y_0$ được gọi là vế phải của phương trình; nếu $y_0 = 0$, phương trình được gọi là tuyến tính thuần nhất.

Mọi phần tử $x_0 \in E$ sao cho $u(x_0) = y_0$ được gọi là một nghiệm của phương trình tuyến tính $u(x) = y_0$.†

Người ta thường nói, theo nghĩa lỏng lẻo, rằng một bài toán là tuyến tính nếu nó tương đương với việc xác định các nghiệm của một phương trình tuyến tính.

Cho một phương trình tuyến tính $u(x) = y_0$, phương trình $u(x) = 0$ được gọi là phương trình tuyến tính thuần nhất liên kết với $u(x) = y_0$.

#### Mệnh đề 14 {#alg-ii-s2-prop-14 .statement}

*Nếu $x_0$ là một nghiệm của phương trình tuyến tính $u(x) = y_0$, tập hợp các nghiệm của phương trình này bằng tập hợp các phần tử $x_0 + z$, trong đó $z$ chạy qua tập hợp các nghiệm của phương trình thuần nhất liên kết $u(x) = 0$.*

Quan hệ $u(x) = y_0$ có thể được viết là $u(x) = u(x_0)$, tương đương với $u(x - x_0) = 0$.

Nói cách khác, nếu phương trình $u(x) = y_0$ có ít nhất một nghiệm $x_0$, tập hợp các nghiệm của nó là tập hợp $x_0 + \overline{u}(0)$, thu được bằng phép tịnh tiến từ hạt nhân $\overline{u}(0)$ của $u$. Nhận xét rằng $\overline{u}(0)$, vì là một môđun con, không bao giờ rỗng, vì nó chứa 0 (được gọi là nghiệm không, hay nghiệm tầm thường, của phương trình thuần nhất $u(x) = 0$).

Theo Mệnh đề 14, để một phương trình tuyến tính $u(x) = y_0$ có *chính xác một nghiệm*, điều kiện cần và đủ là nó có ít nhất một nghiệm và $\overline{u}(0) = \{0\}$ (nói cách khác, phương trình thuần nhất liên kết không có nghiệm khác không, hoặc cũng tương đương là $u$ là *đơn ánh*); trong trường hợp này, với *mọi* $y \in F$, phương trình $u(x) = y$ có *nhiều nhất* một nghiệm.

#### Mệnh đề 15 {#alg-ii-s2-prop-15 .statement}

*Cho $u$ là một ánh xạ tuyến tính từ một môđun $E$ vào một môđun $F$. Nếu phương trình $u(x) = y_0$ có ít nhất một nghiệm, $y_0$ vuông góc với hạt nhân của $^t u$.*

Nói rằng $u(x) = y_0$ có một nghiệm nghĩa là $y_0 \in u(E)$ và mệnh đề suy ra từ no. 5, Hệ quả của Mệnh đề 8.

† Đây thực sự là một sự lạm dụng ngôn ngữ; xét về phương diện lôgic, ở đây ta không định nghĩa từ "nghiệm", mà chỉ định nghĩa câu "$x_0$ là một nghiệm của phương trình $u(x) = y_0$" là tương đương với quan hệ "$x_0 \in E$ và $u(x_0) = y_0$". Nhận xét rằng trong một lý thuyết toán học $\mathcal{T}$ trong đó quan hệ "$A$ là một vành, $E$ và $F$ là $A$-môđun, $u$ là một đồng cấu của $E$ vào $F$, $y_0$ là một phần tử của $F$" là một định lý, mọi *số hạng* $T$ của $\mathcal{T}$ sao cho quan hệ "$T \in E$ và $u(T) = y_0$" là đúng trong $\mathcal{T}$ đều là một *nghiệm* của phương trình $u(x) = y_0$ theo nghĩa của *Lý thuyết Tập hợp*, I, § 5, no. 2; điều này biện minh cho sự lạm dụng ngôn ngữ ở trên.

Nhận xét rằng tiêu chuẩn cần cho sự tồn tại của một nghiệm của $u(x) = y_0$, được cho bởi Mệnh đề 15, là đủ khi $A$ là một trường (\S 7, no. 6, Mệnh đề 12), nhưng *không đúng nói chung* (Bài tập 10).

#### Nhận xét {#alg-ii-s2-n8-rem-1 .statement}

(1) Cho $E$ là một $A$-môđun, $(F_i)_{i \in I}$ là một họ các $A$-môđun và với mọi $i \in I$ cho $u_i : E \to F_i$ là một ánh xạ tuyến tính. Mọi hệ phương trình tuyến tính
$$
u_i(x) = y_i \quad (i \in I)
$$
trong đó các $y_i \in F_i$ đã cho, là tương đương với *một* phương trình tuyến tính duy nhất $u(x) = y$, trong đó $u$ là ánh xạ $x \mapsto (u_i(x))$ của $E$ vào $F = \prod_{i \in I} F_i$ và $y = (y_i)$. Hệ (29) được gọi là *thuần nhất* nếu $y_i = 0$ với mọi $i \in I$.

(2) Giả sử rằng $E$ thừa nhận một *cơ sở* $(a_\lambda)_{\lambda \in L}$; nếu đặt $u(a_\lambda) = b_\lambda$ với mọi $\lambda \in L$, nói rằng $x = \sum_{\lambda \in L} \xi_\lambda a_\lambda$ thỏa mãn phương trình $u(x) = y_0$ tương đương với nói rằng họ (có giá hữu hạn) $(\xi_\lambda)_{\lambda \in L}$ các phần tử của $A$ thỏa mãn quan hệ
$$
\sum_{\lambda \in L} \xi_\lambda b_\lambda = y_0.
$$

Ngược lại, việc tìm các họ $(\xi_\lambda)_{\lambda \in L}$ các phần tử của $A$ có giá hữu hạn thỏa mãn (30), tương đương với việc giải phương trình tuyến tính $u(x) = y_0$, trong đó $u$ là ánh xạ tuyến tính duy nhất của $E$ vào $F$ sao cho $u(a_\lambda) = b_\lambda$ với mọi $\lambda \in L$ (\S 1, no. 11, Hệ quả 3 của Mệnh đề 17).

(3) Một phương trình tuyến tính $u(x) = y_0$ được gọi là *vô hướng* khi $F = A_s$ và do đó $u$ là một *dạng tuyến tính* trên $E$ và $y_0$ là một *vô hướng*. Nếu $E$ thừa nhận một cơ sở $(a_\lambda)_{\lambda \in L}$, suy ra từ *Nhận xét* (2) rằng một phương trình như vậy cũng có thể được viết dưới dạng
$$
\sum_{\lambda \in L} \xi_\lambda \alpha_\lambda = y_0 \in A
$$
trong đó họ các vô hướng $(\alpha_\lambda)$ là tùy ý và trong đó hiểu rằng họ $(\xi_\lambda)$ phải có giá hữu hạn. Nói chung, nghiệm *nghiệm* (trong $A$) của một hệ các phương trình tuyến tính vô hướng
$$
\sum_{\lambda \in L} \xi_\lambda \alpha_{\lambda_i} = \eta_i \quad (i \in I)
$$
trong đó $\alpha_{\lambda_i} \in A$ và $\eta_i \in A$, được hiểu là một họ $(\xi_\lambda)_{\lambda \in L}$ các phần tử của $A$ có *giá* hữu hạn và thỏa mãn (32); các $\alpha_{\lambda_i}$ được gọi là các *hệ số* của hệ phương trình và các $\eta_i$ là các *vế phải*. Nghiệm của một hệ như vậy tương đương với nghiệm của phương trình $u(x) = y$, trong đó $y = (\eta_i)$ và $u : A_s^{(L)} \to A_s^I$ là ánh xạ tuyến tính
$$
(\xi_\lambda) \mapsto \left( \sum_{\lambda \in L} \xi_\lambda \alpha_{\lambda_i} \right).
$$

(4) Một hệ tuyến tính (32) còn được gọi là *hệ các phương trình tuyến tính vô hướng trái* khi cần tránh nhầm lẫn. Một hệ phương trình
$$
\sum_{\lambda \in L} \alpha_{\lambda_i} \xi_\lambda = \eta_i \quad (i \in I)
$$

tương tự được gọi là một hệ các phương trình tuyến tính vô hướng phải; một hệ như vậy có thể ngay lập tức được biến đổi thành một hệ (32) bằng cách xem các $\xi_{\lambda}, \eta_i$ và $\alpha_{\lambda_i}$ như thuộc vành đối $A^0$ của A.

### Bài tập {#alg-ii-s2-exercises}

Xem [các bài tập cho § 2](exercises/s2/).
