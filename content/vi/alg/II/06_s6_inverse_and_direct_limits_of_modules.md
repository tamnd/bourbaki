---
book: alg
book_title: Algebra
chapter: II
chapter_title: LINEAR ALGEBRA
section: 6
section_title: Inverse and direct limits of modules
lang: vi
source: alg-i-iii
source_edition: 1998, Springer
pdf_pages: 0308-0315, 0423-0424
extraction: ocr
subsections:
    - "no": 1
      title: INVERSE LIMITS OF MODULES
      page: 0
      pdf_page: 308
    - "no": 2
      title: DIRECT LIMITS OF MODULES
      page: 0
      pdf_page: 310
    - "no": 3
      title: TENSOR PRODUCT OF DIRECT LIMITS
      page: 0
      pdf_page: 313
statements: 17
exercises: 4
content_sha256: 90d2e343799095a16e41af5f5752bab1e3a3de4be6a2a9ecb3a8c2a186bafca4
translated_from: content/en/alg/II/06_s6_inverse_and_direct_limits_of_modules.md
source_content_sha256: 0071494e46f0d6a4a97c19ea9a8d779c617f3943739c71f4a78db61ff9daaa81
translation_model: gpt-5-6-mini, gpt-5.4-mini
translation_run: translate-vi-44386587
glossary_version: 34
glossary_terms_sha256: 68868b394eeda8e8fd2dd6d6194f990a55bb897c8efb63d3ee77beedec14be5b
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 6. GIỚI HẠN NGƯỢC VÀ TRỰC TIẾP CỦA CÁC MÔĐUN

Trong suốt đoạn này, ta ký hiệu một tập tiền thứ tự khác rỗng và $\alpha \leq \beta$ là quan hệ tiền thứ tự trên I. Trừ khi có nói khác đi, các hệ ngược và hệ trực tiếp đều có tập chỉ số là I.

### 1. GIỚI HẠN NGƯỢC CỦA CÁC MÔĐUN

Cho $(A_\alpha, \phi_{\alpha \beta})$ là một hệ ngược các vành (I, § 10, no. 1), $(E_\alpha, f_{\alpha \beta})$ là một hệ ngược các nhóm giao hoán (viết theo phép cộng) (I, § 10, no. 1) và giả sử mỗi $E_\alpha$ có một cấu trúc môđun trái trên $A_\alpha$; hơn nữa, giả sử rằng với $\alpha \leq \beta$ $(f_{\alpha \beta}, \phi_{\alpha \beta})$ là một dimorphism của $E_\beta$ vào $E_\alpha$ (§ 1, no. 13), nói cách khác,
$$
f_{\alpha \beta}(\lambda_\beta x_\beta) = \phi_{\alpha \beta}(\lambda_\beta) f_{\alpha \beta}(x_\beta),
$$
với $x_\beta \in E_\beta$, $\lambda_\beta \in A_\beta$; khi đó từ I, § 10, no. 2 suy ra rằng $E = \lim \leftarrow E_\alpha$ có một cấu trúc môđun trái trên $A = \lim \leftarrow A_\alpha$. Với mọi $\alpha \in I$, gọi $f : E \to E_\alpha$, $\phi_\alpha : A \to A_\alpha$ là các ánh xạ chính tắc; khi đó $(f_\alpha, \phi_\alpha)$ là một dimorphism của E vào $E_\alpha$. Ta sẽ nói rằng $(E_\alpha, f_{\alpha\beta})$ là một *hệ ngược các môđun trái $A_\alpha$* và môđun $A$ $E$ là *giới hạn ngược* của nó.

Cho $(E'_\alpha, f'_{\alpha\beta})$ là một hệ ngược khác của các môđun trái $A_\alpha$ và, với mọi $\alpha$, gọi $u_\alpha : E'_\alpha \to E_\alpha$ là một *ánh xạ tuyến tính $A_\alpha$*, các ánh xạ này lập thành một *hệ ngược*; khi đó $u = \lim u_\alpha$ là một *ánh xạ tuyến tính $A$* của $\lim E'_\alpha$ vào $\lim E_\alpha$.

Hơn nữa:

#### Mệnh đề 1 {#alg-ii-s6-prop-1 .statement}

*Cho* $(E_\alpha, f_{\alpha\beta}),\ (E'_\alpha, f'_{\alpha\beta}),\ (E''_\alpha, f''_{\alpha\beta})$ *là ba hệ ngược các môđun $A_\alpha$ và* $(u_\alpha),\ (v_\alpha)$ *là hai hệ ngược các ánh xạ tuyến tính $A_\alpha$ sao cho các dãy*

$$
0 \longrightarrow E'_\alpha \xrightarrow{u_\alpha} E_\alpha \xrightarrow{v_\alpha} E''_\alpha
$$

*là khớp với mọi $\alpha$.* *Khi đặt* $u = \lim u_\alpha,\ v = \lim v_\alpha$, *dãy*

$$
0 \longrightarrow \lim E'_\alpha \xrightarrow{u} \lim E_\alpha \xrightarrow{v} \lim E''_\alpha
$$

*là khớp*.

*Vì* $u_\alpha^{-1}(0) = \{0\}$ *với mọi $\alpha$, theo Lý thuyết Tập hợp, III, § 7, no. 2, Mệnh đề 2 suy ra rằng* $u^{-1}(0) = \{0\}$, *do đó* $u$ *là đơn ánh; hơn nữa, các* $u_\alpha(E'_\alpha)$ *lập thành một hệ ngược các tập con của các* $E_\alpha$ *và do đó* $u(\lim E'_\alpha) = \lim u_\alpha(E'_\alpha)$. *Theo* $u_\alpha(E'_\alpha) = v_\alpha^{-1}(0)$ *do giả thiết,* $v^{-1}(0) = \lim u_\alpha(E'_\alpha) = u(\lim E'_\alpha)$ (*Lý thuyết Tập hợp*, III, § 7, no. 2, Mệnh đề 2), *điều này hoàn tất chứng minh*.

#### Nhận xét {#alg-ii-s6-n1-rem-1 .statement}

(1) Mệnh đề 1 và chứng minh của nó đúng với các *nhóm* tùy ý, ngoại trừ thay đổi ký hiệu.

(2) Chú ý rằng nếu có các dãy khớp

$$
0 \longrightarrow E'_\alpha \xrightarrow{u_\alpha} E_\alpha \xrightarrow{v_\alpha} E''_\alpha \longrightarrow 0
$$

*thì không nhất thiết suy ra* rằng dãy

$$
0 \longrightarrow \lim E'_\alpha \xrightarrow{u} \lim E_\alpha \xrightarrow{v} \lim E''_\alpha \longrightarrow 0
$$

*là khớp; nói cách khác, giới hạn ngược của một hệ ngược các ánh xạ tuyến tính toàn ánh không nhất thiết là toàn ánh* (xem Bài tập 1).

Giả sử bây giờ các $A_\alpha$ bằng *cùng một vành* $A$ và các $\phi_{\alpha\beta}$ bằng $1_A$; khi đó với mọi hệ ngược $(E_\alpha, f_{\alpha\beta})$ của các môđun $A$, $E = \lim E_\alpha$ là một $A$-môđun. Cho $F$ là một $A$-môđun và, với mọi $\alpha$, cho $u_\alpha : F \to E_\alpha$ là một ánh xạ $A$-tuyến tính sao cho $(u_\alpha)$ là một hệ ngược của các ánh xạ; khi đó $u = \lim u_\alpha$ là một ánh xạ $A$-tuyến tính từ $F$ vào $\lim E_\alpha$. *Ngược lại*, với mọi ánh xạ $A$-tuyến tính $v : F \to \lim E_\alpha$, họ của các $v_\alpha = f_\alpha \circ v$ là một hệ ngược của các ánh xạ $A$-tuyến tính sao cho $v = \lim_{\leftarrow} v_\alpha$. Mặt khác ta chú ý rằng với $\alpha \leq \beta$ ánh xạ

$$
\operatorname{Hom}(1_F, f_{\alpha \beta}) = \bar{f}_{\alpha \beta}: \operatorname{Hom}_A(F, E_\beta) \to \operatorname{Hom}_A(F, E_\alpha)
$$

là một đồng cấu môđun $\mathbf{Z}$ sao cho $(\operatorname{Hom}_A(F, E_\alpha), \bar{f}_{\alpha \beta})$ là một *hệ ngược của các môđun $\mathbf{Z}$*; vì $\bar{f}_{\alpha \beta}(v_\beta) = f_{\alpha \beta} \circ v_\beta$, các nhận xét trên do đó có thể được biểu diễn như sau:

#### Mệnh đề 2 {#alg-ii-s6-prop-2 .statement}

*Với mọi hệ ngược* $(E_\alpha, f_{\alpha \beta})$ *của các môđun $A$*-và mọi *môđun $A$*-module $F$, *ánh xạ chính tắc* $u \mapsto (f_\alpha \circ u)$ *là một đẳng cấu môđun $\mathbf{Z}$*

(2)

$$
l_F: \operatorname{Hom}_A(F, \lim_{\leftarrow} E_\alpha) \to \lim_{\leftarrow} \operatorname{Hom}_A(F, E_\alpha).
$$

#### Hệ quả {#alg-ii-s6-n1-cor-1 .statement}

*Với mọi đồng cấu môđun $A$ $v: F \to F'$, ánh xạ*

$$
\bar{v}_\alpha = \operatorname{Hom}(v, 1_{E_\alpha}): \operatorname{Hom}(F', E_\alpha) \to \operatorname{Hom}(F, E_\alpha)
$$

*tạo thành một hệ ngược của các ánh xạ tuyến tính $\mathbf{Z}$* *và biểu đồ*

(3)

$$
\begin{array}{ccc}
\operatorname{Hom}(F', \lim_{\leftarrow} E_\alpha) & \xrightarrow{l_{F'}} & \lim_{\leftarrow} \operatorname{Hom}(F', E_\alpha) \\
\downarrow \operatorname{Hom}(v, 1_E) & & \downarrow \lim_{\leftarrow} \bar{v}_\alpha \\
\operatorname{Hom}(F, \lim_{\leftarrow} E_\alpha) & \xrightarrow{l_F} & \lim_{\leftarrow} \operatorname{Hom}(F, E_\alpha)
\end{array}
$$

*là giao hoán*.

Với mọi $u \in \operatorname{Hom}(F', \lim_{\leftarrow} E_\alpha)$, $l_F(u \circ v) = (f_\alpha \circ u \circ v)$ theo định nghĩa và tính giao hoán của biểu đồ (3) suy ra ngay lập tức từ các định nghĩa.

### 2. GIỚI HẠN TRỰC TIẾP CỦA CÁC MÔĐUN

*Từ nay I được giả sử là có hướng phải.*

Cho $(A_\alpha, \phi_{\beta \alpha})$ là một hệ trực tiếp của các vành (I, § 10, no. 3), $(E_\alpha, f_{\beta \alpha})$ là một hệ trực tiếp của các nhóm giao hoán (viết theo phép cộng) (I, § 10, no. 3) và giả sử rằng mỗi $E_\alpha$ có một *cấu trúc môđun $A_\alpha$ trái*; hơn nữa, giả sử rằng, với $\alpha \leq \beta$, $(f_{\beta \alpha}, \phi_{\beta \alpha})$ là một *đồng cấu đôi* của $E_\alpha$ vào $E_\beta$ (§ 1, no. 13), nói cách khác rằng

(4)

$$
f_{\beta \alpha}(\lambda_\alpha x_\alpha) = \phi_{\beta \alpha}(\lambda_\alpha) f_{\beta \alpha}(x_\alpha)
$$

với $x_\alpha \in E_\alpha, \lambda_\alpha \in A_\alpha$; khi đó $E = \lim_{\longrightarrow} E_\alpha$ có cấu trúc *môđun trái* trên $A = \lim_{\longrightarrow} A_\alpha$ (I, § 10, no. 4). Với mọi $\alpha \in I$, đặt $f_\alpha: E_\alpha \to E, \phi_\alpha: A_\alpha \to A$ là các ánh xạ chính tắc; khi đó $(f_\alpha, \phi_\alpha)$ là một *đồng cấu* của $E_\alpha$ vào $E$. Ta sẽ nói rằng $(E_\alpha, f_{\beta \alpha})$ là một *hệ trực tiếp các môđun trái $A_\alpha$* và môđun $A$* $E$ là *giới hạn trực tiếp* của nó.

Cho $(E'_\alpha, f'_{\beta \alpha})$ là một hệ trực tiếp khác của các môđun trái $A_\alpha$* và, với mọi $\alpha$, cho $u_\alpha : E'_\alpha \to E_\alpha$ là một ánh xạ tuyến tính $A_\alpha$-tuyến tính, các ánh xạ này lập thành một hệ trực tiếp; khi đó $u = \lim \to u_\alpha$ là một ánh xạ $A$-tuyến tính của $\lim \to E'_\alpha$ vào $\lim \to E_\alpha$.

Hơn nữa:

#### Mệnh đề 3 {#alg-ii-s6-prop-3 .statement}

*Cho* $(E_\alpha, f_{\beta \alpha}), (E'_\alpha, f'_{\beta \alpha}), (E''_\alpha, f''_{\beta \alpha})$ *là ba hệ trực tiếp của các* $A_\alpha$*-môđun và* $(u_\alpha), (v_\alpha)$ *là hai hệ trực tiếp của các ánh xạ* $A_\alpha$*-tuyến tính sao cho các dãy*

$$
E'_\alpha \xrightarrow{u_\alpha} E_\alpha \xrightarrow{v_\alpha} E''_\alpha
$$

*là khớp với mọi* $\alpha$. *Khi viết* $u = \lim \to u_\alpha, v = \lim \to v_\alpha$, *dãy*

$$
\lim \to E'_\alpha \xrightarrow{u} \lim \to E_\alpha \xrightarrow{v} \lim \to E''_\alpha
$$

*là khớp.*

$u(\lim \to E'_\alpha) = \lim \to u_\alpha(E'_\alpha)$ *và* $v^{-1}(0) = \lim \to v_\alpha^{-1}(0)$ *(Lý thuyết Tập hợp, III, § 7, no. 6, Hệ quả của Mệnh đề 7).*

Nói một cách không chính thức, Mệnh đề 3 cũng có thể được phát biểu bằng cách nói rằng *chuyển qua giới hạn trực tiếp bảo toàn tính khớp*.

#### Mệnh đề 4 {#alg-ii-s6-prop-4 .statement}

*Cho* $(E_\alpha, f_{\beta \alpha})$ *là một hệ trực tiếp của các* $A_\alpha$*-môđun, $E = \lim \to E_\alpha$ *là giới hạn trực tiếp của nó và* $\phi_\alpha : A_\alpha \to A$ *và* $f_\alpha : E_\alpha \to E$ *là các ánh xạ chính tắc với mọi* $\alpha \in I$. *Nếu, với mọi* $\alpha \in I$, $S_\alpha$ *là một hệ sinh của* $E_\alpha$, *thì* $S = \bigcup_{\alpha \in I} f_\alpha(S_\alpha)$ *là một hệ sinh của* $E$.

Mọi $x \in E$ *đều có dạng* $f_\alpha(x_\alpha)$ *với một* $\alpha \in I$ *nào đó và một* $x_\alpha \in E_\alpha$ *nào đó và theo giả thiết* $x = \sum_i \lambda^{(i)}_\alpha y^{(i)}_\alpha$, *trong đó* $\lambda^{(i)}_\alpha \in A_\alpha$ *và* $y^{(i)}_\alpha \in S_\alpha$; *viết* $\lambda^{(i)} = \phi_\alpha(\lambda^{(i)}_\alpha)$, $y^{(i)} = f_\alpha(y^{(i)}_\alpha)$, *ta được* $x = \sum_i \lambda^{(i)} y^{(i)}$.

#### Mệnh đề 5 {#alg-ii-s6-prop-5 .statement}

*Với các giả thiết và ký hiệu của Mệnh đề 4, giả sử rằng với mọi* $\alpha \in I$, $E_\alpha$ *là tổng trực tiếp của một họ* $(M^\lambda_\alpha)_{\alpha \in L}$ *gồm các môđun con (tập chỉ số* $L$ *độc lập với* $\alpha$) *và rằng* $f_{\beta \alpha}(M^\lambda_\alpha) \subset M^\lambda_\alpha$ *đối với* $\alpha \leq \beta$ *và với mọi* $\lambda \in L$. *Khi đó* $E$ *là tổng trực tiếp của các môđun con* $M^\lambda = \lim \to M^\lambda_\alpha$ $(\lambda \in L)$.

Suy ra từ Mệnh đề 4 rằng $E$ là tổng của các $M^\lambda$. Cho $(y^\lambda)_{\lambda \in L}$ *là một họ sao cho* $y^\lambda \in M^\lambda$ *với mọi* $\lambda \in L$ *và có giá hữu hạn, và giả sử rằng* $\sum_\lambda y^\lambda = 0$. *Nhờ Lý thuyết tập hợp, III, § 7, no. 5, Bổ đề 1, tồn tại một* $\alpha \in I$ *và một họ* $(x^\lambda_\alpha)_{\alpha \in L}$ *có giá hữu hạn gồm các phần tử của* $E_\alpha$ *sao cho* $x^\lambda_\alpha \in M^\lambda_\alpha$ *và* $y^\lambda = f_\alpha(x^\lambda_\alpha)$ *với mọi* $\lambda \in L$. *Quan hệ* $f_\alpha \left( \sum_{\lambda \in L} x^\lambda_\alpha \right) = 0$ *kéo theo sự tồn tại của một* $\beta \geq \alpha$ *sao cho* $f_{\beta \alpha} \left( \sum_{\lambda \in L} x^\lambda_\alpha \right) = 0$ *(Lý thuyết tập hợp, III, § 7, no. 5, Bổ đề 1), điều này có thể viết là* $\sum_{\lambda \in L} x_\beta^\lambda = 0$, *trong đó* $x_\beta^\lambda = f_{\beta \alpha}(x_\alpha^\lambda) \in M_\beta^\lambda$ *theo giả thiết; do đó* $x_\beta^\lambda = 0$ *với mọi* $\lambda \in L$ *và vì thế* $y^\lambda = f_\beta(x_\beta^\lambda) = 0$ *với mọi* $\lambda \in L$, *điều này chứng tỏ rằng tổng của các* $M^\lambda$ *là trực tiếp.*

#### Hệ quả {#alg-ii-s6-n2-cor-1 .statement}

*Cho* $(P_\alpha)$ *là một hệ trực tiếp của các tập con của* $E_\alpha$ *và đặt* $P = \lim \overrightarrow{P_\alpha}$. *Nếu, với mọi* $\alpha \in I$, $P_\alpha$ *là một tập con tự do (resp. cơ sở) của* $E_\alpha$, *thì* $P$ *là một tập con tự do (resp. cơ sở) của* $E$.

Khẳng định thứ hai suy ra ngay lập tức từ khẳng định thứ nhất và Mệnh đề 4. Do đó đủ để chứng minh rằng nếu các $P_\alpha$ đều tự do thì mọi tập con $\{ y^{(i)} \}_{1 \leq i \leq n}$ gồm các phần tử phân biệt của $P$, đều tự do. Tồn tại một $\alpha \in I$ và các phần tử $x_\alpha^{(i)} \in P_\alpha$ sao cho $y^{(i)} = f_\alpha(x_\alpha^{(i)})$ với $1 \leq i \leq n$ (*Set Theory*, III, § 7, no. 5, Bổ đề 1); nếu $\sum_i \lambda^{(i)} y^{(i)} = 0$, thì có thể giả sử rằng $\lambda^{(i)} = \phi_\alpha(\lambda_\alpha^{(i)})$ với $1 \leq i \leq n$ và do đó $f_\alpha \left( \sum_i \lambda_\beta^{(i)} x_\beta^{(i)} \right) = 0$; điều này suy ra $\sum_i \lambda_\beta^{(i)} x_\beta^{(i)} = 0$ với một $\beta \geq \alpha$ nào đó, trong đó $\lambda_\beta^{(i)} = \phi_{\beta \alpha}(\lambda_\alpha^{(i)})$, $x_\beta^{(i)} = f_{\beta \alpha}(x_\alpha^{(i)})$ và các $x_\beta^{(i)}$ thuộc $P_\beta$ và phân biệt vì $y^{(i)} = f_\beta(x_\beta^{(i)})$; khi đó $\lambda_\beta^{(i)} = 0$ với $1 \leq i \leq n$, do đó
$$
\lambda^{(i)} = \phi_\beta(\lambda_\beta^{(i)}) = 0
$$
với $1 \leq i \leq n$.

Giả sử bây giờ rằng tất cả các vành $A_\alpha$ đều bằng cùng một vành $A$ và các $\phi_{\beta \alpha}$ đều bằng $1_A$; khi đó, với mọi hệ trực tiếp $(E_\alpha, f_{\beta \alpha})$ của các $A$-môđun, $E = \lim \overrightarrow{E_\alpha}$ là một $A$-môđun. Cho $F$ là một $A$-môđun và với mọi $\alpha$ đặt $u_\alpha : E_\alpha \to F$ là một ánh xạ $A$-tuyến tính sao cho $(u_\alpha)$ là một hệ trực tiếp các ánh xạ; khi đó $u = \lim \overrightarrow{u_\alpha}$ là một ánh xạ $A$-tuyến tính từ $E$ vào $F$. *Ngược lại*, với mọi ánh xạ $A$-tuyến tính $v : \lim \overrightarrow{E_\alpha} \to F$, họ của $v_\alpha = v \circ f_\alpha$ là một hệ trực tiếp các ánh xạ $A$-tuyến tính sao cho $v = \lim \overrightarrow{v_\alpha}$. Mặt khác ta nhận thấy rằng với $\alpha \leq \beta$ thì ánh xạ
$$
\operatorname{Hom}(f_{\beta \alpha}, 1_F) = \bar{f}_{\alpha \beta} : \operatorname{Hom}_A(E_\beta, F) \to \operatorname{Hom}_A(E_\alpha, F)
$$
là một đồng cấu $\mathbf{Z}$-môđun sao cho $(\operatorname{Hom}_A(E_\alpha, F), \bar{f}_{\alpha \beta})$ là một *hệ ngược của* $\mathbf{Z}$*-môđun*; vì $\bar{f}_{\alpha \beta}(v_\beta) = v_\beta \circ f_{\beta \alpha}$, các nhận xét trên có thể phát biểu như sau:

#### Mệnh đề 6 {#alg-ii-s6-prop-6 .statement}

*Với mọi hệ trực tiếp* $(E_\alpha, f_{\beta \alpha})$ *của các* $A$*-môđun và mọi* $A$*-môđun* $F$, *ánh xạ chính tắc* $u \mapsto (u \circ f_\alpha)$ *là một đẳng cấu* $\mathbf{Z}$*-môđun*
$$
d_F : \operatorname{Hom}_A(\lim \overrightarrow{E_\alpha}, F) \to \lim \leftarrow \operatorname{Hom}_A(E_\alpha, F).
$$

#### Hệ quả 1 {#alg-ii-s6-prop-6-cor-1 .statement}

*Với mọi* $A$*-đồng cấu môđun* $v : F \to F'$, *các*
$$
\bar{v}_\alpha = \operatorname{Hom}(1_{E_\alpha}, v) : \operatorname{Hom}(E_\alpha, F) \to \operatorname{Hom}(E_\alpha, F')
$$

lập thành một hệ ngược các $\mathbf{Z}$-ánh xạ tuyến tính và biểu đồ

$$
\begin{array}{ccc}
\operatorname{Hom}(\lim E_\alpha, F) & \xrightarrow{d_F} & \lim \operatorname{Hom}(E_\alpha, F) \\
\downarrow \operatorname{Hom}(1_E, v) & & \downarrow \lim \overline{v}_\alpha \\
\operatorname{Hom}(\lim E_\alpha, F') & \xrightarrow{d_{F'}} & \lim \operatorname{Hom}(E_\alpha, F')
\end{array}
$$

giao hoán.

Với mọi $u \in \operatorname{Hom}(\lim E_\alpha, F)$, $d_{F'}(v \circ u) = (v \circ u \circ f_\alpha)$ theo định nghĩa, và tính giao hoán của biểu đồ (6) suy ra ngay lập tức từ các định nghĩa.

#### Hệ quả 2 {#alg-ii-s6-prop-6-cor-2 .statement}

*Nếu* $(E_\alpha, f_{\beta \alpha})$ *là một hệ trực tiếp các* $A$*-môđun trái và* $E = \lim \longrightarrow E_\alpha$, $(E_\alpha^*, t f_{\beta \alpha})$ *là một hệ ngược các* $A$*-môđun phải và* $\lim \leftarrow E_\alpha^*$ *đẳng cấu chính tắc với* $E^*$.

#### Nhận xét {#alg-ii-s6-n2-rem-1 .statement}

Cho $E$ là một $A$*-môđun và* $(M_\alpha)_{\alpha \in I}$ *một họ tăng các môđun con của* $E$ *sao cho* $E$ *là hợp của các* $M_\alpha$; nếu $j_{\beta \alpha}: M_\alpha \to M_\beta$ (với $\alpha \leq \beta$) và $j_\alpha: M_\alpha \to E$ *là các ánh xạ nhúng chính tắc, thì rõ ràng* $j = \lim \longrightarrow j_\alpha$ *là một đẳng cấu từ* $\lim \longrightarrow M_\alpha$ *lên* $E$ *(Set Theory, III, § 7, no. 6, Remark 1)*. Đặc biệt, mọi $A$*-môđun đều là giới hạn trực tiếp của họ có hướng phải các* *môđun con sinh hữu hạn* của nó.

### 3. TÍCH TENXƠ CỦA CÁC GIỚI HẠN TRỰC TIẾP

Cho $(A_\alpha, \rho_{\beta \alpha})$ là một hệ trực tiếp các vành và $(E_\alpha, f_{\beta \alpha})$ (tương ứng $(F_\alpha, g_{\beta \alpha})$) là một hệ trực tiếp các $A_\alpha$*-môđun phải* (tương ứng *trái*). Với $\alpha \leq \beta$, có một đồng cấu môđun $\mathbf{Z}$*-*

$$
f_{\beta \alpha} \otimes g_{\beta \alpha}: E_\alpha \otimes_{A_\alpha} F_\alpha \to (E_\beta)_{[A_\alpha]} \otimes_{A_\alpha} (F_\beta)_{[A_\alpha]}
$$

và mặt khác có một đồng cấu môđun $\mathbf{Z}$*chính tắc*

$$
(E_\beta)_{[A_\alpha]} \otimes_{A_\alpha} (F_\beta)_{[A_\alpha]} \to E_\beta \otimes_{A_\beta} F_\beta
$$

tương ứng với đồng cấu vành $\rho_{\beta \alpha}$ ($§ 3$, no. 3, Mệnh đề 2); do đó bằng hợp thành ta thu được một đồng cấu môđun $\mathbf{Z}$*-*

$$
h_{\beta \alpha}: E_\alpha \otimes_{A_\alpha} F_\alpha \to E_\beta \otimes_{A_\beta} F_\beta
$$

ánh xạ tích tenxơ $x_\alpha \otimes y_\alpha$ thành $f_{\beta \alpha}(x_\alpha) \otimes g_{\beta \alpha}(y_\alpha)$. Rõ ràng

$$
(E_\alpha \otimes_{A_\alpha} F_\alpha, h_{\beta \alpha})
$$

là một *hệ trực tiếp* các $\mathbf{Z}$*-môđun. Đặt* $A = \lim \longrightarrow A_\alpha$, $E = \lim \longrightarrow E_\alpha$, $F = \lim \longrightarrow F_\alpha$ *và*

gọi $\rho_\alpha : A_\alpha \to A, f_\alpha : E_\alpha \to E, g_\alpha : F_\alpha \to F$ là các ánh xạ chính tắc. Như trên, xác định một ánh xạ tuyến tính trên $\mathbf{Z}$ $\pi_\alpha : E_\alpha \otimes_{A_\alpha} F_\alpha \to E \otimes_A F$, ánh xạ tích tenxơ $x_\alpha \otimes y_\alpha$ thành $f_\alpha(x_\alpha) \otimes g_\alpha(y_\alpha)$, và rõ ràng các ánh xạ này lập thành một hệ trực tiếp. Do đó ta thu được một ánh xạ tuyến tính trên $\mathbf{Z}$
$$
\pi = \lim \pi_\alpha : \lim (E_\alpha \otimes_{A_\alpha} F_\alpha) \to E \otimes_A F.
$$

#### Mệnh đề 7 {#alg-ii-s6-prop-7 .statement}

*Ánh xạ tuyến tính trên $\mathbf{Z}$ (7) là song ánh.*

Đặt $P = \lim (E_\alpha \otimes_{A_\alpha} F_\alpha)$ và, với mọi $\alpha \in I$, cho $h_\alpha : E_\alpha \otimes_{A_\alpha} F_\alpha \to P$ là ánh xạ chính tắc. Mặt khác, với mọi $\alpha \in I$, cho
$$
t_\alpha : E_\alpha \times F_\alpha \to E_\alpha \otimes_{A_\alpha} F_\alpha
$$
là ánh xạ song tuyến tính $\mathbf{Z}$ chính tắc; với $\alpha \leq \beta$,
$$
t_\beta(f_{\beta \alpha}(x_\alpha), g_{\beta \alpha}(y_\alpha)) = f_{\beta \alpha}(x_\alpha) \otimes g_{\beta \alpha}(y_\alpha) = h_{\beta \alpha}(t_\alpha(x_\alpha, y_\alpha))
$$
và do đó $(t_\alpha)$ là một hệ trực tiếp các ánh xạ. Đồng nhất một cách chính tắc $\lim (E_\alpha \times F_\alpha)$ với $E \times F$ (*Set Theory*, III, § 7, no. 7, Mệnh đề 10), ta suy ra một ánh xạ $t = \lim t_\alpha : E \times F \to P$ sao cho
$$
t(f_\alpha(x_\alpha), g_\alpha(y_\alpha)) = h_\alpha(t_\alpha(x_\alpha, y_\alpha)) = h_\alpha(x_\alpha \otimes y_\alpha).
$$
Xét đến *Set Theory*, III, § 7, no. 5, Bổ đề 1, dễ thấy ngay rằng $t$ là $\mathbf{Z}$-song tuyến tính; hơn nữa, với $x \in E, y \in F, \lambda \in A$, tồn tại $\alpha \in I$ sao cho $x = f_\alpha(x_\alpha), y = g_\alpha(y_\alpha), \lambda = \rho_\alpha(\lambda_\alpha)$ với $\lambda_\alpha \in A_\alpha, x_\alpha \in E_\alpha, y_\alpha \in F_\alpha$ (*Set Theory*, III, § 3, no. 7, Bổ đề 1); do đó
$$
t(x \lambda, y) = h_\alpha((x_\alpha \lambda_\alpha) \otimes y_\alpha) = h_\alpha(x_\alpha \otimes (\lambda_\alpha y_\alpha)) = t(x, \lambda y).
$$
Vậy tồn tại duy nhất một ánh xạ $\mathbf{Z}$-tuyến tính $\pi' : E \otimes_A F \to P$ sao cho $\pi'(x \otimes y) = t(x, y)$ (§ 3, no. 1, Mệnh đề 1). Hơn nữa, theo định nghĩa
$$
\pi'(\pi(h_\alpha(x_\alpha \otimes y_\alpha))) = \pi'(f_\alpha(x_\alpha) \otimes g_\alpha(y_\alpha)) = h_\alpha(x_\alpha \otimes y_\alpha)
$$
$$
\pi(\pi'(f_\alpha(x_\alpha) \otimes g_\alpha(y_\alpha))) = \pi(h_\alpha(x_\alpha \otimes y_\alpha)) = f_\alpha(x_\alpha) \otimes g_\alpha(y_\alpha)
$$
và vì các phần tử dạng $f_\alpha(x_\alpha) \otimes g_\alpha(y_\alpha)$ (hay $h_\alpha(x_\alpha \otimes y_\alpha)$) sinh môđun $\mathbf{Z}$ $E \otimes_A F$ (hay $P$), $\pi' \circ \pi$ và $\pi \circ \pi'$ là các ánh xạ đồng nhất.

Nói một cách đại lược, Mệnh đề 7 có thể được phát biểu bằng cách nói rằng *tích tenxơ giao hoán với giới hạn trực tiếp* và thường hai vế của (7) được đồng nhất nhờ đẳng cấu $\pi$.

#### Hệ quả 1 {#alg-ii-s6-prop-7-cor-1 .statement}

*Cho* $(E'_\alpha, f'_{\beta \alpha})$ (resp. $(F'_\alpha, g'_{\alpha \beta})$) *là một hệ trực tiếp khác của các môđun phải* (resp. *trái*) *$A_\alpha$; với mọi* $\alpha \in I$, *cho* $u_\alpha : E_\alpha \to E'_\alpha$ (resp. $v_\alpha : F_\alpha \to F'_\alpha$) *là một* $A_\alpha$-ánh xạ tuyến tính sao cho $(u_\alpha)$ (resp. $(v_\alpha)$) là một hệ trực tiếp. Khi đó $(u_\alpha \oplus v_\alpha)$ là một hệ trực tiếp các $\mathbf{Z}$-ánh xạ tuyến tính và biểu đồ

$$
\begin{array}{ccc}
\lim(E_\alpha \otimes_{A_\alpha} F_\alpha) & \longrightarrow & (\lim E_\alpha) \otimes_A (\lim F_\alpha) \\
\downarrow & & \downarrow \\
\lim(u_\alpha \otimes v_\alpha) & & (\lim u_\alpha) \otimes (\lim v_\alpha) \\
\lim(E'_\alpha \otimes_{A_\alpha} F'_\alpha) & \longrightarrow & (\lim E'_\alpha) \otimes_A (\lim F'_\alpha)
\end{array}
$$

là giao hoán.

Việc kiểm tra là ngay lập tức.

Cho $(A'_\alpha, \rho'_{\beta\alpha})$ là một hệ trực tiếp khác của các vành và giả sử rằng mỗi $E_\alpha$ là một song môđun $(A'_\alpha, A_\alpha)$, các $f_{\beta\alpha}$ là $(A'_\alpha, A_\alpha)$-tuyến tính với $\alpha \leq \beta$. Khi đó nếu ta viết $A' = \lim A'_\alpha$, thì đẳng cấu (7) là tuyến tính đối với các cấu trúc môđun trái $A'$ trên hai vế nhờ Hệ quả 1. Điều này có thể được khái quát hóa ngay lập tức cho các đa môđun tùy ý.

Đặc biệt, nếu các $A_\alpha$ giao hoán, thì $A = \lim A_\alpha$ giao hoán và đẳng cấu (7) là một đẳng cấu môđun $A$.

#### Hệ quả 2 {#alg-ii-s6-prop-7-cor-2 .statement}

*Cho* $(E_\alpha, f_{\beta\alpha})$ *là một hệ trực tiếp các môđun phải* $A_\alpha$*và cho* $E'_\alpha = E_\alpha \otimes_{A_\alpha} A$ *là môđun* $A$ *thu được bằng cách mở rộng vành vô hướng lên* $A = \lim A_\alpha$ *nhờ đồng cấu chính tắc* $\rho_\alpha : A_\alpha \to A$. *Khi đó* $(E'_\alpha, f_{\beta\alpha} \otimes 1_A)$ *là một hệ trực tiếp các môđun phải* $A$, *mà giới hạn trực tiếp của nó đẳng cấu chính tắc với* $\lim E_\alpha$.

Chỉ cần áp dụng Mệnh đề 7 với $F_\alpha$ là vành $A$ được xét như một song môđun $(A_\alpha, A)$ nhờ $\rho_\alpha$.

#### Hệ quả 3 {#alg-ii-s6-prop-7-cor-3 .statement}

*Cho* $A$ *là một vành,* $(E_\alpha, f_{\beta\alpha})$ *là một hệ trực tiếp các $A$-môđun phải và* $F$ *là một $A$-môđun trái.* *Khi đó các* $\mathbf{Z}$*-môđun* $\lim (E_\alpha \otimes_A F)$ *và* $(\lim E_\alpha) \otimes_A F$ *đẳng cấu một cách chính tắc*.

Chỉ cần lấy $A_\alpha = A$ và $F_\alpha = F$ với mọi $\alpha \in I$ trong Mệnh đề 7.

Đặc biệt, nếu $\rho : A \to B$ là một đồng cấu vành, $\lim \rho^*(E_\alpha)$ và $\rho^*(\lim E_\alpha)$ đẳng cấu một cách chính tắc.

#### Hệ quả 4 {#alg-ii-s6-prop-7-cor-4 .statement}

*Cho* $M$ *là một $A$-môđun phải,* $N$ *là một $A$-môđun trái,* $(x_i)_{1 \leq i \leq n}$ *là một họ các phần tử của* $M$, $(y_i)_{1 \leq i \leq n}$ *là một họ các phần tử của* $N$, *sao cho* $\sum_i (x_i \otimes y_i) = 0$ *trong* $M \otimes_A N$. *Khi đó tồn tại một môđun con sinh hữu hạn* $M_1$ *(resp. $N_1$) của* $M$ *(resp. $N$) chứa các* $x_i$ *(resp. các* $y_i$) *và sao cho* $\sum_i (x_i \otimes y_i) = 0$ *trong* $M_1 \otimes_A N_1$.

$M$ (resp. $N$) được đồng nhất một cách chính tắc với giới hạn trực tiếp của họ có hướng phải các môđun con sinh hữu hạn của nó chứa các $x_i$ (resp. các $y_i$) và chỉ cần áp dụng *Lý thuyết tập hợp, III, § 7, no. 5, Bổ đề 1.*

### Bài tập {#alg-ii-s6-exercises}

Xem [các bài tập cho § 6](exercises/s6/).
