---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VIII
chapter_title: SPLIT SEMI-SIMPLE LIE ALGEBRAS
section: 2
section_title: Root system of a split semi-simple Lie algebra
lang: vi
source: lie-vii-ix
book_pages: 77-86, 226-229
pdf_pages: 0085-0094, 0234-0237
extraction: native
subsections:
    - "no": 1
      title: SPLIT SEMI-SIMPLE LIE ALGEBRAS
      page: 77
      pdf_page: 85
    - "no": 2
      title: ROOTS OF A SPLIT SEMI-SIMPLE LIE ALGEBRA
      page: 78
      pdf_page: 86
    - "no": 3
      title: INVARIANT BILINEAR FORMS
      page: 83
      pdf_page: 91
    - "no": 4
      title: THE COEFFICIENTS N$_{\boldsymbol{\alpha \beta }}$
      page: 83
      pdf_page: 91
statements: 28
exercises: 11
content_sha256: 81ce4377e88dc1b9aeaa54039185d6683805a340b699d7630369714cedd46942
translated_from: content/en/lie/VIII/02_s2_root_system_of_a_split_semi_simple_lie.md
source_content_sha256: 5b8fba70b72c8f243ecb19eff11bd99a4fc4e1594703137b927fa6344b3f9e7f
translation_model: gpt-5.4
translation_run: translate-vi-cd36f7b1
glossary_version: 34
glossary_terms_sha256: 0ff6f9f38c6b41997659a8077edde346663dc4b507fc6495c3e52e35149b5e06
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 2. HỆ NGHIỆM CỦA MỘT ĐẠI SỐ LIE NỬA ĐƠN TÁCH

### 1. CÁC ĐẠI SỐ LIE NỬA ĐƠN TÁCH

#### Định nghĩa 1 {#lie-viii-s2-def-1 .statement tag=00YK}

Cho $\mathfrak{g}$ là một đại số Lie nửa đơn. Một đại số con Cartan $\mathfrak{h}$ của $\mathfrak{g}$ được gọi là tách nếu, với mọi $x\in \mathfrak{h}$, ad$_{\mathfrak{g}}x$ tam giác hóa được. Một đại số Lie nửa đơn được gọi là tách được nếu nó có một đại số con Cartan tách. Một đại số Lie nửa đơn tách là một cặp $(\mathfrak{g},\mathfrak{h})$ trong đó $\mathfrak{g}$ là một đại số Lie nửa đơn và $\mathfrak{h}$ là một đại số con Cartan tách của $\mathfrak{g}$.

#### Nhận xét 1 {#lie-viii-s2-n1-rem-1 .statement tag=00YL}

Cho $\mathfrak{g}$ là một đại số Lie nửa đơn, $\mathfrak{h}$ là một đại số con Cartan của $\mathfrak{g}$. Với mọi $x\in \mathfrak{h}$, ad$_{\mathfrak{g}}x$ là nửa đơn (Chap. VII, §2, no. 4, Th. 2). Do đó, nói rằng $\mathfrak{h}$ là tách có nghĩa là ad$_{\mathfrak{g}}x$ là chéo hóa được với mọi $x\in \mathfrak{h}$.

#### Nhận xét 2 {#lie-viii-s2-n1-rem-2 .statement tag=00YM}

Nếu $k$ đóng đại số, mọi đại số Lie nửa đơn $\mathfrak{g}$ đều tách được, và mọi đại số con Cartan của $\mathfrak{g}$ đều tách. Khi $k$ không đóng đại số, tồn tại các đại số Lie nửa đơn không tách được (Bài tập $2a$)$)$; hơn nữa, nếu $\mathfrak{g}$ tách được, có thể tồn tại các đại số con Cartan của $\mathfrak{g}$ không tách (Bài tập $2b$)$)$.

#### Nhận xét 3 {#lie-viii-s2-n1-rem-3 .statement tag=00YN}

Cho $\mathfrak{g}$ là một đại số Lie nửa đơn, $\mathfrak{h}$ là một đại số con Cartan của $\mathfrak{g}$, và $\rho$ là một biểu diễn đơn ánh hữu hạn chiều của $\mathfrak{g}$ sao cho $\rho (\mathfrak{h})$ chéo hóa được. Khi đó ad$_{\mathfrak{g}}x$ chéo hóa được với mọi $x\in \mathfrak{h}$ (Chap. VII, §2, no. 1, Ví dụ 2), nên $\mathfrak{h}$ là tách.

#### Nhận xét 4 {#lie-viii-s2-n1-rem-4 .statement tag=00YO}

Ta sẽ thấy (§3, no. 3, Hệ quả của Mệnh đề 10) rằng nếu $\mathfrak{h},\mathfrak{h}'$ là các đại số con Cartan tách của $\mathfrak{g}$, thì tồn tại một tự đẳng cấu sơ cấp của $\mathfrak{g}$ biến $\mathfrak{h}$ thành $\mathfrak{h}'$.

#### Nhận xét 5 {#lie-viii-s2-n1-rem-5 .statement tag=00YP}

Cho $\mathfrak{g}$ là một đại số Lie khả quy. Khi đó $\mathfrak{g}=\mathfrak{c}\times \mathfrak{s}$ trong đó $\mathfrak{c}$ là tâm của $\mathfrak{g}$ và $\mathfrak{s}=\mathscr{D}\mathfrak{g}$ là nửa đơn. Các đại số con Cartan của $\mathfrak{g}$ là các đại số con có dạng $\mathfrak{h}=\mathfrak{c}\times \mathfrak{h}'$ trong đó $\mathfrak{h}'$ là một đại số con Cartan của $\mathfrak{s}$ (Chap. VII, §2, no. 1, Prop. 2). Khi đó $\mathfrak{h}$ được gọi là tách nếu $\mathfrak{h}'$ là tách đối với $\mathfrak{s}$. Điều này dẫn một cách hiển nhiên đến định nghĩa các đại số khả quy phân tích được hoặc tách.

### 2. CÁC NGHIỆM CỦA MỘT ĐẠI SỐ LIE ĐƠN NỬA ĐƠN TÁCH

Trong số này, $(\mathfrak{g},\mathfrak{h})$ ký hiệu một đại số Lie nửa đơn tách.

Với mọi $\lambda \in \mathfrak{h}^*$, ký hiệu $\mathfrak{g}^{\lambda}(\mathfrak{h})$, hoặc đơn giản $\mathfrak{g}^{\lambda}$, không gian con nguyên sơ của $\mathfrak{g}$ đối với $\lambda$ (xem Chương VII, §1, no. 3). Nhắc lại rằng $\mathfrak{g}^0=\mathfrak{h}$ (Chương VII, §2, no. 1, Mệnh đề 4), rằng $\mathfrak{g}$ là tổng trực tiếp của các $\mathfrak{g}^{\lambda}$ (Chương VII, §1, no. 3, Mệnh đề 8 và 9), rằng $\mathfrak{g}^{\lambda}$ là tập hợp các $x\in \mathfrak{g}$ sao cho $[h, x] =\lambda (h)x$ với mọi $h\in \mathfrak{h}$ (Chương VII, §2, no. 4, Hệ quả 1 của Định lý 2), và rằng các trọng của $\mathfrak{h}$ trên $\mathfrak{g}$ là các dạng tuyến tính $\lambda$ trên $\mathfrak{h}$ sao cho $\mathfrak{g}^{\lambda}\not= 0$ (Chương VII, §1, no. 1).

#### Định nghĩa 2 {#lie-viii-s2-def-2 .statement tag=00YQ}

Một nghiệm của $(\mathfrak{g},\mathfrak{h})$ là một trọng số khác không của $\mathfrak{h}$ trên $\mathfrak{g}$.

Ký hiệu bởi $R(\mathfrak{g},\mathfrak{h})$, hoặc đơn giản là bởi R, tập hợp các nghiệm của $(\mathfrak{g},\mathfrak{h})$. Ta có

$$
\mathfrak{g}=\mathfrak{h}\oplus \bigoplus_{\alpha\in R}\mathfrak{g}^{\alpha}
$$

#### Mệnh đề 1 {#lie-viii-s2-prop-1 .statement tag=00YR}

Cho $\alpha ,\beta$ là các nghiệm của $(\mathfrak{g},\mathfrak{h})$ và cho $\langle \cdot ,\cdot \rangle$ là một dạng song tuyến tính đối xứng bất biến không suy biến trên $\mathfrak{g}($chẳng hạn dạng Killing của $\mathfrak{g})$.

(i) Nếu $\alpha +\beta \not= 0,\mathfrak{g}^{\alpha}$ và $\mathfrak{g}^{\beta}$ trực giao. Hạn chế của $\langle \cdot ,\cdot \rangle$ trên $\mathfrak{g}^{\alpha}\times \mathfrak{g}^{-\alpha}$ là không suy biến. Hạn chế của $\langle \cdot ,\cdot \rangle$ trên $\mathfrak{h}$ là không suy biến.

(ii) Cho $x\in \mathfrak{g}^{\alpha},y\in \mathfrak{g}^{-\alpha}$ và $h\in \mathfrak{h}$. Khi đó $[x, y]\in \mathfrak{h}$ và

$$
\langle h,[x, y]\rangle =\alpha (h)\langle x, y\rangle
$$

Mệnh đề (i) là một trường hợp riêng của Mệnh đề 10 (iii) của Chương VII, §1, no. 3. Nếu $x\in \mathfrak{g}^{\alpha},y\in \mathfrak{g}^{-\alpha}$ và $h\in \mathfrak{h}$, ta có $[x, y]\in \mathfrak{g}^{\alpha-\alpha}=\mathfrak{h}$, và

$$
\langle h,[x, y]\rangle =\langle [h, x], y\rangle =\langle \alpha (h)x, y\rangle =\alpha (h)\langle x, y\rangle
$$

#### Định lý 1 {#lie-viii-s2-thm-1 .statement tag=00YS}

Cho $\alpha$ là một nghiệm của $(\mathfrak{g},\mathfrak{h})$.

(i) Không gian vectơ $\mathfrak{g}^{\alpha}$ có chiều 1.

(ii) Không gian con vectơ $\mathfrak{h}_{\alpha}= [\mathfrak{g}^{\alpha},\mathfrak{g}^{-\alpha}]$ của $\mathfrak{h}$ có chiều 1. Nó chứa một phần tử duy nhất $H_{\alpha}$ sao cho $\alpha (H_{\alpha}) = 2$.

(iii) Không gian con vectơ $\mathfrak{s}_{\alpha}=\mathfrak{h}_{\alpha}+\mathfrak{g}^{\alpha}+\mathfrak{g}^{-\alpha}$ là một đại số Lie con của $\mathfrak{g}$.

(iv) Nếu $X_{\alpha}$ là một phần tử khác không của $\mathfrak{g}^{\alpha}$, thì tồn tại một $X_{-\alpha}\in \mathfrak{g}^{-\alpha}$ duy nhất sao cho $[X_{\alpha}, X_{-\alpha}] =-H_{\alpha}$. Gọi $\varphi$ là ánh xạ tuyến tính từ $\mathfrak{s}\mathfrak{l}(2, k)$ vào $\mathfrak{g}$ biến $X_+$ thành $X_{\alpha},X_-$ thành $X_{-\alpha}$, và $H$ thành $H_{\alpha}$; khi đó $\varphi$ là một đẳng cấu từ đại số Lie $\mathfrak{s}\mathfrak{l}(2, k)$ lên đại số Lie $\mathfrak{s}_{\alpha}$.

a) Gọi $h_{\alpha}$ là phần tử duy nhất của $\mathfrak{h}$ sao cho $\alpha (h) =\langle h_{\alpha}, h\rangle$ với mọi $h\in \mathfrak{h}$. Theo Mệnh đề $1, [x, y] =\langle x, y\rangle h_{\alpha}$ với mọi $x\in \mathfrak{g}^{\alpha},y\in \mathfrak{g}^{-\alpha}$; mặt khác $\langle \mathfrak{g}^{\alpha},\mathfrak{g}^{-\alpha}\rangle  \not= 0$. Do đó $\mathfrak{h}_{\alpha}= [\mathfrak{g}^{\alpha},\mathfrak{g}^{-\alpha}] =kh_{\alpha}$.

b) Chọn $x\in \mathfrak{g}^{\alpha},y\in \mathfrak{g}^{-\alpha}$ sao cho $\langle x, y\rangle = 1$, do đó $[x, y] =h_{\alpha}$. Nhắc lại rằng $[h_{\alpha}, x] =\alpha (h_{\alpha})x, [h_{\alpha}, y] =-\alpha (h_{\alpha})y$. Nếu $\alpha (h_{\alpha}) = 0$, suy ra $kx+ky+kh_{\alpha}$ là một đại số con lũy linh $\mathfrak{t}$ của $\mathfrak{g}$; vì $h_{\alpha}\in [\mathfrak{t},\mathfrak{t}]$, ad$_{\mathfrak{g}}h_{\alpha}$ là lũy linh (Chương I, §5, no. 3, Định lý 1), điều này vô lý vì ad$_{\mathfrak{g}}h_{\alpha}$ là nửa đơn khác không. Vậy $\alpha (h_{\alpha})\not= 0$. Do đó tồn tại duy nhất $H_{\alpha}\in \mathfrak{h}_{\alpha}$ sao cho $\alpha (H_{\alpha}) = 2$, điều này chứng minh (ii).

c) Chọn một phần tử khác không $X_{\alpha}$ của $\mathfrak{g}^{\alpha}$. Tồn tại $X_{-\alpha}\in \mathfrak{g}^{-\alpha}$ sao cho $[X_{\alpha}, X_{-\alpha}] =-H_{\alpha}$ (vì $[X_{\alpha},\mathfrak{g}^{-\alpha}] =\mathfrak{h}_{\alpha}$ theo $b$)$)$. Khi đó

$$
[H_{\alpha}, X_{\alpha}] =\alpha (H_{\alpha})X_{\alpha}= 2X_{\alpha},[H_{\alpha}, X_{-\alpha}] =-\alpha (H_{\alpha})X_{-\alpha}=-2X_{-\alpha}
$$

$$
[X_{\alpha}, X_{-\alpha}] =-H_{\alpha}
$$

do đó $kX_{\alpha}+kX_{-\alpha}+kH_{\alpha}$ là một đại số con của $\mathfrak{g}$ và ánh xạ tuyến tính $\varphi$ từ $\mathfrak{s}\mathfrak{l}(2, k)$ tới $kX_{\alpha}+kX_{-\alpha}+kH_{\alpha}$ sao cho $\varphi (X_+) =X_{\alpha},\varphi (X_-) =X_{-\alpha}$, $\varphi (H) =H_{\alpha}$ là một đẳng cấu của các đại số Lie.

d) Giả sử dim$\mathfrak{g}^{\alpha}>1$. Cho $y$ là một phần tử khác không của $\mathfrak{g}^{-\alpha}$. Tồn tại một phần tử khác không $X_{\alpha}$ của $\mathfrak{g}_{\alpha}$ sao cho $\langle y, X_{\alpha}\rangle = 0$. Chọn $X_{-\alpha}$ như trong c), và xét biểu diễn $\rho :u \rightarrow$ ad$_{\mathfrak{g}}\varphi (u)$ từ $\mathfrak{s}\mathfrak{l}(2, k)$ vào $\mathfrak{g}$. Ta có

$$
\rho (H)y= [\varphi (H), y] = [H_{\alpha}, y] =-2y
$$

$$
\rho (X_+)y= [\varphi (X_+), y] = [X_{\alpha}, y] =\langle X_{\alpha}, y\rangle h_{\alpha}= 0
$$

Vì thế, $y$ là nguyên thủy đối với $\rho$, có trọng số $-2$, điều này mâu thuẫn với Mệnh đề 2 của §1, no. 2. Điều này chứng minh (i).

e) Mệnh đề (iii) bây giờ là một hệ quả của c). Mặt khác, nếu $X_{\alpha}$ là một phần tử khác không của $\mathfrak{g}^{\alpha}$, thì phần tử $X_{-\alpha}$ được xây dựng trong c) là phần tử duy nhất của $\mathfrak{g}^{-\alpha}$ sao cho $[X_{\alpha}, X_{-\alpha}] =-H_{\alpha}$ vì dim $\mathfrak{g}^{-\alpha}= 1$. Khẳng định cuối cùng của (iv) là một hệ quả của c). Q.E.D.

Các ký hiệu $h_{\alpha},H_{\alpha},\mathfrak{s}_{\alpha}$ sẽ được giữ lại trong phần sau. (Để định nghĩa $h_{\alpha}$, ta lấy $\langle \cdot ,\cdot \rangle$ bằng dạng Killing.) Nếu $X_{\alpha}$ là một phần tử khác không của $\mathfrak{g}^{\alpha}$, thì đẳng cấu $\varphi$ của Định lý 1 và biểu diễn $u \rightarrow$ ad$_{\mathfrak{g}}\varphi (u)$ của $\mathfrak{s}\mathfrak{l}(2, k)$ trên $\mathfrak{g}$ sẽ được gọi là liên kết với $X_{\alpha}$.

#### Hệ quả {#lie-viii-s2-n2-cor-1 .statement tag=00YT}

Cho $\Phi$ là dạng Killing của $\mathfrak{g}$. Với mọi $a, b\in \mathfrak{h}$,

$$
\Phi (a, b) =\sum_{\gamma\in R}\gamma (a)\gamma (b)
$$

Thật vậy, ad $a$.ad $b$ để ổn định mỗi $\mathfrak{g}^{\gamma}$, và hạn chế của nó trên $\mathfrak{g}^{\gamma}$ là phép vị tự có tỉ số $\gamma (a)\gamma (b)$; nếu $\gamma \not= 0$, dim$\mathfrak{g}^{\gamma}= 1$.

#### Mệnh đề 2 {#lie-viii-s2-prop-2 .statement tag=00YU}

Cho $\alpha , \beta \in R$.

(i) $\beta (H_{\alpha})\in \mathbf{Z}$.

(ii) Nếu $\Phi$ ký hiệu dạng Killing của $\mathfrak{g},\Phi (H_{\alpha}, H_{\beta})\in \mathbf{Z}$.

Gọi $X_{\alpha}$ là một phần tử khác không của $\mathfrak{g}^{\alpha}$, và gọi $\rho$ là biểu diễn của $\mathfrak{s}\mathfrak{l}(2, k)$ trên $\mathfrak{g}$ liên kết với $X_{\alpha}$. Các trị riêng của $\rho (H)$ là 0 và các $\beta (H_{\alpha})$ với $\beta \in R$. Do đó (i) suy ra từ §1, no. 2, Hệ quả của Mệnh đề 2. Mệnh đề (ii) suy ra từ (i) và Hệ quả của Định lý 1. Q.E.D.

Cho $\alpha \in R,X_{\alpha}$ là một phần tử khác không của $\mathfrak{g}^{\alpha},X_{-\alpha}$ là phần tử của $\mathfrak{g}^{-\alpha}$ sao cho $[X_{\alpha}, X_{-\alpha}] =-H_{\alpha}$, và $\rho$ là biểu diễn của $\mathfrak{s}\mathfrak{l}(2, k)$ trên $\mathfrak{g}$ liên kết với $X_{\alpha}$. Gọi $\pi$ là biểu diễn của $\mathbf{S}\mathbf{L}(2, k)$ trên $\mathfrak{g}$ tương thích với $\rho ($§1, no. 4, Đl. 2). Vì ad $X_{\alpha}$ là lũy linh (Chap. VII, §1, no. 3, Prop. 10 (iv)), nên $\pi (e^{X_+}) =e^{adX_{\alpha}}$ là một tự đẳng cấu sơ cấp của $\mathfrak{g}$. Tương tự, $\pi (e^{X_-}) =$ $e^{adX_{-\alpha}}$ là một tự đẳng cấu sơ cấp của $\mathfrak{g}$. Do đó $\pi (\mathbf{S}\mathbf{L}(2, k))\subset$ Aut$_e(\mathfrak{g})$. Ta dùng ký hiệu $\theta (t)$ của §1, no. 5. Với $t\in k^*$, đặt

$$
\theta_{\alpha}(t) =\pi (\theta (t)) =e^{adtX_{\alpha}}e^{adt^{-1}X_{-\alpha}}e^{adtX_{\alpha}} \tag{1}
$$

#### Bổ đề 1 {#lie-viii-s2-lem-1 .statement tag=00YV}

(i) Với mọi $h\in \mathfrak{h},\theta_{\alpha}(t).h=h-\alpha (h)H_{\alpha}$.

(ii) Với mọi $\beta \in R,\theta_{\alpha}(t)(\mathfrak{g}^{\beta}) =\mathfrak{g}^{\beta-\beta(H_{\alpha})\alpha}$.

(iii) Nếu $\alpha , \beta \in R,\beta -\beta (H_{\alpha})\alpha \in R$.

Lấy $h\in \mathfrak{h}$. Nếu $\alpha (h) = 0, [X_{\alpha}, h] = [X_{-\alpha}, h] = 0$, nên $\theta_{\alpha}(t).h=h$. Mặt khác, các công thức (5) của §1, no. 5 cho thấy rằng $\theta_{\alpha}(t).H_{\alpha}=-H_{\alpha}$. Điều này chứng minh mệnh đề (i). Suy ra $\theta_{\alpha}(t)^2|\mathfrak{h}=$ Id. Nếu $x\in \mathfrak{g}^{\beta}$ và $h\in \mathfrak{h}$,

$$
[h, \theta_{\alpha}(t)x] =\theta_{\alpha}(t).[\theta_{\alpha}(t)h, x]-\beta (\theta_{\alpha}(t)h).\theta_{\alpha}(t)x
$$

$$
= (\beta (h)-\alpha (h)\beta (H_{\alpha})).\theta_{\alpha}(t)x
$$

$$
= (\beta -\beta (H_{\alpha})\alpha )(h).\theta_{\alpha}(t)x
$$

nên $\theta_{\alpha}(t)x\in \mathfrak{g}^{\beta-\beta(H_{\alpha})\alpha}$. Điều này chứng minh (ii). Mệnh đề (iii) suy ra từ (ii).

#### Định lý 2 {#lie-viii-s2-thm-2 .statement tag=00YW}

(i) Tập hợp $R = R(\mathfrak{g},\mathfrak{h})$ là một hệ căn rút gọn trong $\mathfrak{h}^*$.

(ii) Cho $\alpha \in R$. Ánh xạ $s_{\alpha ,H_{\alpha}}:\lambda  \rightarrow \lambda -\lambda (H_{\alpha})\alpha$ từ $\mathfrak{h}^*$ đến $\mathfrak{h}^*$ là phép đối xứng duy nhất $s$ của $\mathfrak{h}^*$ sao cho $s(\alpha ) =-\alpha$ và $s(R) = R$. Với mọi $t\in k^*$, $s$ là chuyển vị của $\theta_{\alpha}(t)|\mathfrak{h}$.

Trước hết, R sinh ra $\mathfrak{h}^*$, vì nếu $h\in \mathfrak{h}$ sao cho $\alpha (h) = 0$ với mọi $\alpha \in R$, thì ad $h= 0$ và do đó $h= 0$ vì tâm của $\mathfrak{g}$ là không. Theo định nghĩa, $0\notin R$. Cho $\alpha \in R$. Vì $\alpha (H_{\alpha}) = 2,s=s_{\alpha ,H_{\alpha}}$ là một phép đối xứng sao cho $s(\alpha ) =-\alpha$. Khi đó $s(R) = R$ theo Bổ đề 1 (iii), và $\beta (H_{\alpha})\in \mathbf{Z}$ với mọi $\beta \in R$ (Mệnh đề 2 (i)). Điều này cho thấy R là một hệ nghiệm trong $\mathfrak{h}^*$. Với mọi $h\in \mathfrak{h}$ và $\lambda \in \mathfrak{h}^*$,

$$
\langle s(\lambda ), h\rangle =\langle \lambda -\lambda (H_{\alpha})\alpha , h\rangle =\langle \lambda , h-\alpha (h)H_{\alpha}\rangle =\langle \lambda , \theta_{\alpha}(t)h\rangle
$$

vậy $s$ là chuyển vị của $\theta_{\alpha}(t)|\mathfrak{h}$. Cuối cùng, ta chứng minh rằng hệ nghiệm R là rút gọn. Cho $\alpha \in R$ và $y\in \mathfrak{g}^{2\alpha}$. Vì $3\alpha  \notin R$ (Chap. VI, §1, no. 3, Mệnh đề $8$)$, [X_{\alpha}, y] = 0$; mặt khác, $[X_{-\alpha}, y]\in \mathfrak{g}^{-\alpha+2\alpha}=\mathfrak{g}^{\alpha}=kX_{\alpha}$, nên $[X_{\alpha},[X_{-\alpha}, y]] = 0$; do đó

$$
4y= 2\alpha (H_{\alpha})y= [H_{\alpha}, y] =-[[X_{\alpha}, X_{-\alpha}], y] = 0
$$

suy ra $y= 0$ và $\mathfrak{g}^{2\alpha}= 0$. Nói cách khác, $2\alpha$ không phải là một nghiệm. C.Q.F.D.

Đồng nhất $\mathfrak{h}$ một cách chính tắc với $\mathfrak{h}^{**}$. Với các ký hiệu của Chương VI, §1, no. 1, khi đó theo Định lý 2 (ii),

$H_{\alpha}=\alpha^{\vee}$ với mọi $\alpha \in R$. (2)

Do đó, các $H_{\alpha}$ tạo thành hệ nghiệm $R^{\vee}$ trong $\mathfrak{h}$ nghịch đảo với R.

Ta sẽ gọi $R(\mathfrak{g},\mathfrak{h})$ là hệ nghiệm của $(\mathfrak{g},\mathfrak{h})$. Các phép đối xứng $s_{\alpha ,H_{\alpha}}$ sẽ được ký hiệu đơn giản bởi $s_{\alpha}$. Nhóm Weyl, nhóm trọng số, số Coxeter $. .$. của $R(\mathfrak{g},\mathfrak{h})$ được gọi là nhóm Weyl, nhóm trọng số, số Coxeter $. .$. của $(\mathfrak{g},\mathfrak{h})$. Như trong Chương VI, §1, no. 1, ta xét nhóm Weyl như tác động không chỉ trên $\mathfrak{h}^*$, mà còn trên $\mathfrak{h}$ bằng phép chuyển cấu trúc, sao cho $s_{\alpha}=\theta_{\alpha}(t)|\mathfrak{h}$. Vì các $\theta_{\alpha}(t)$ là những tự đẳng cấu sơ cấp của $\mathfrak{g}$, ta có:

#### Hệ quả {#lie-viii-s2-n2-cor-2 .statement tag=00YX}

Mọi phần tử của nhóm Weyl của $(\mathfrak{g},\mathfrak{h})$, tác động trên $\mathfrak{h}$, đều là hạn chế trên $\mathfrak{h}$ của một tự đẳng cấu sơ cấp của $\mathfrak{g}$.

Để có một đảo lại của kết quả này, xem §5, no. 2, Mệnh đề 4.

#### Nhận xét 1 {#lie-viii-s2-n2-rem-1 .statement tag=00YY}

Nếu $\mathfrak{h}_{\mathbf{Q}}$ (tương ứng $\mathfrak{h}^*_{\mathbf{Q}}$) ký hiệu không gian con vectơ trên $\mathbf{Q}$ của $\mathfrak{h}$ (tương ứng của $\mathfrak{h}^*$) sinh bởi các $H_{\alpha}$ (tương ứng các $\alpha$ ), với $\alpha \in R$, thì $\mathfrak{h}$ (tương ứng $\mathfrak{h}^*$) có thể được đồng nhất một cách chính tắc với $\mathfrak{h}_{\mathbf{Q}}\otimes_{\mathbf{Q}}k$ (tương ứng với $\mathfrak{h}^*_{\mathbf{Q}}\otimes_{\mathbf{Q}}k$) và $\mathfrak{h}^*_{\mathbf{Q}}$ có thể được đồng nhất với đối ngẫu của $\mathfrak{h}_{\mathbf{Q}}$ (Chương VI, §1, no. 1, Mệnh đề 1). Ta gọi $\mathfrak{h}_{\mathbf{Q}}$ và $\mathfrak{h}^*_{\mathbf{Q}}$ là các $\mathbf{Q}$-cấu trúc chính tắc trên $\mathfrak{h}$ và $\mathfrak{h}^*($Đại số, Chương II, §8, no. 1, Định nghĩa 1). Khi nói đến tính hữu tỉ trên $\mathbf{Q}$ đối với một không gian con vectơ của $\mathfrak{h}$, đối với một dạng tuyến tính trên $\mathfrak{h}$, v.v., ta sẽ hiểu theo các cấu trúc ấy, trừ khi có chỉ dẫn ngược lại. Khi nói đến các buồng Weyl, hoặc các mặt, của $R(\mathfrak{g},\mathfrak{h})$, ta sẽ làm việc trong $\mathfrak{h}_{\mathbf{Q}}\otimes_{\mathbf{Q}}\mathbf{R}$ hoặc $\mathfrak{h}^*_{\mathbf{Q}}\otimes_{\mathbf{Q}}\mathbf{R}$, mà ta sẽ ký hiệu bởi $\mathfrak{h}_{\mathbf{R}}$ và $\mathfrak{h}^*_{\mathbf{R}}$.

#### Nhận xét 2 {#lie-viii-s2-n2-rem-2 .statement tag=00YZ}

Hệ nghiệm $R^{\vee}$ trong $\mathfrak{h}$ xác định một dạng song tuyến tính đối xứng không suy biến $\beta$ trên $\mathfrak{h}$ (Chap. VI, §1, no. 1, Prop. 3), cụ thể là dạng $(a, b) \rightarrow$ $\sum_{\alpha\in R}\langle \alpha , a\rangle \langle \alpha , b\rangle$. Theo Hệ quả của Định lý 1, dạng này chính là hạn chế của

dạng Killing lên $\mathfrak{h}$. Mở rộng của $\beta |\mathfrak{h}_{\mathbf{Q}}\times \mathfrak{h}_{\mathbf{Q}}$ tới $\mathfrak{h}_{\mathbf{Q}}\otimes_{\mathbf{Q}}\mathbf{R}$ là dương không suy biến (Chap. VI, §1, no. 1, Prop. 3). Mặt khác, ta thấy rằng dạng nghịch đảo trên $\mathfrak{h}^*$ của hạn chế lên $\mathfrak{h}$ của dạng Killing trên $\mathfrak{g}$ là dạng song tuyến tính chính tắc $\Phi_R$ của R (Chap. VI, §1, no. 12).

Cho $(\mathfrak{g}_1,\mathfrak{h}_1), (\mathfrak{g}_2,\mathfrak{h}_2)$ là các đại số Lie nửa đơn tách, $\varphi$ là một đẳng cấu từ $\mathfrak{g}_1$ lên $\mathfrak{g}_2$ sao cho $\varphi (\mathfrak{h}_1) =\mathfrak{h}_2$. Bởi phép chuyển cấu trúc, chuyển vị của ánh xạ $\varphi |\mathfrak{h}_1$ đưa $R(\mathfrak{g}_2,\mathfrak{h}_2)$ vào $R(\mathfrak{g}_1,\mathfrak{h}_1)$.

#### Mệnh đề 3 {#lie-viii-s2-prop-3 .statement tag=00Z0}

Cho $\mathfrak{g}$ là một đại số Lie nửa đơn, $\mathfrak{h}_1$ và $\mathfrak{h}_2$ là các đại số con Cartan tách của $\mathfrak{g}$. Tồn tại một đẳng cấu từ $\mathfrak{h}^*_1$ đến $\mathfrak{h}^*_2$ đưa $R(\mathfrak{g},\mathfrak{h}_1)$ lên $R(\mathfrak{g},\mathfrak{h}_2)$.

(Để có các kết quả chính xác hơn, xem §3, no. 3, Hệ quả của Mệnh đề 10, và §5, no. 3, Mệnh đề 5).

Cho $k'$ là một bao đóng đại số của $k,\mathfrak{g}'=\mathfrak{g}\otimes_kk',\mathfrak{h}'_i=\mathfrak{h}_i\otimes_kk'$. Khi đó $R(\mathfrak{g}',\mathfrak{h}'_i)$ là ảnh của $R(\mathfrak{g},\mathfrak{h}_i)$ dưới ánh xạ $\lambda  \rightarrow \lambda \otimes 1$ từ $\mathfrak{h}^*_i$ vào $\mathfrak{h}^*_i\otimes_kk'={\mathfrak{h}'_i}^*$. Theo Chương VII, §3, no. 2, Định lý 1, tồn tại một tự đẳng cấu của $\mathfrak{g}'$ biến $\mathfrak{h}'_1$ thành $\mathfrak{h}'_2$, do đó một đẳng cấu $\varphi$ từ ${\mathfrak{h}'_1}^*$ lên ${\mathfrak{h}'_2}^*$ biến $R(\mathfrak{g}',\mathfrak{h}'_1)$ thành $R(\mathfrak{g}',\mathfrak{h}'_2)$. Khi đó $\varphi |\mathfrak{h}^*_1$ biến $R(\mathfrak{g},\mathfrak{h}_1)$ thành $R(\mathfrak{g},\mathfrak{h}_2)$, và do đó biến $\mathfrak{h}^*_1$ thành $\mathfrak{h}^*_2$. C.Q.F.D.

Theo Mệnh đề 3, hệ nghiệm của $(\mathfrak{g},\mathfrak{h})$ chỉ phụ thuộc, tới đẳng cấu, vào $\mathfrak{g}$ mà không phụ thuộc vào $\mathfrak{h}$. Cũng vậy, nhóm Weyl, nhóm các trọng số $. .$. của $(\mathfrak{g},\mathfrak{h})$ được gọi đơn giản, do lạm dụng ngôn ngữ, là nhóm Weyl, nhóm các trọng số $. .$. của $\mathfrak{g}$ (xem thêm §5, no. 3, Nhận xét 2). Nếu đồ thị Dynkin của $\mathfrak{g}$ thuộc kiểu $A_l$, hoặc $B_l,. .$. (x. Chương VI, §4, no. 2, Định lý 3), ta nói rằng $\mathfrak{g}$ thuộc kiểu $A_l$, hoặc $B_l,. .$..

Nhớ rằng, nếu $\alpha$ và $\beta$ là các nghiệm độc lập tuyến tính, thì tập hợp các $j\in \mathbf{Z}$ sao cho $\beta +j\alpha \in R$ là một khoảng $[-q, p]$ của $\mathbf{Z}$ chứa 0, với $p-q=$ $-\langle \beta , \alpha^{\vee}\rangle =-\beta (H_{\alpha})$ (Chương VI, §1, no. 3, Mệnh đề 9).

#### Mệnh đề 4 {#lie-viii-s2-prop-4 .statement tag=00Z1}

Cho $\alpha$ và $\beta$ là các nghiệm độc lập tuyến tính. Gọi $p$ (tương ứng $q$) là số nguyên lớn nhất $j$ sao cho $\beta +j\alpha$ (tương ứng $\beta -j\alpha$ ) là một nghiệm.

(i) Không gian con vectơ $\sum_{-q\leq j\leq p}\mathfrak{g}^{\beta+j\alpha}$ của $\mathfrak{g}$ là một $\mathfrak{s}_{\alpha}$-môđun đơn có chiều $p+q+ 1$.

(ii) Nếu $\alpha +\beta$ là một nghiệm, thì $[\mathfrak{g}^{\alpha},\mathfrak{g}^{\beta}] =\mathfrak{g}^{\alpha+\beta}$.

Cho $X_{\alpha}$ (resp. $x$) là một phần tử khác không của $\mathfrak{g}^{\alpha}$ (resp. $\mathfrak{g}^{\beta+p\alpha}$). Khi đó

$$
[X_{\alpha}, x]\in \mathfrak{g}^{\beta+(p+1)\alpha}= 0
$$

$$
[H_{\alpha}, x] = (\beta (H_{\alpha}) +p\alpha (H_{\alpha}))x= (-p+q+ 2p)x= (p+q)x
$$

Như vậy, $x$ là nguyên thủy có trọng số $p+q$ đối với biểu diễn của $\mathfrak{s}\mathfrak{l}(2, k)$ trên $\mathfrak{g}$ liên kết với $X_{\alpha}$; nhưng $\mathfrak{s}\mathfrak{l}(2, k$)-môđun $\sum_{-q\leq j\leq p}\mathfrak{g}^{\beta+j\alpha}$ có chiều $p+q+ 1$; do đó nó là đơn (§1, no. 2, Mệnh đề 2). Nếu $\alpha +\beta \in R$, thì $p\geq 1$, nên các phần tử của $\mathfrak{g}^{\beta}$ không nguyên thủy, và do đó $[X_{\alpha},\mathfrak{g}^{\beta}]\not= 0$. Vì $[\mathfrak{g}^{\alpha},\mathfrak{g}^{\beta}]\subset$ $\mathfrak{g}^{\alpha+\beta}$, cuối cùng ta thấy rằng $[\mathfrak{g}^{\alpha},\mathfrak{g}^{\beta}] =\mathfrak{g}^{\alpha+\beta}$.

#### Nhận xét 3 {#lie-viii-s2-n2-rem-3 .statement tag=00Z2}

Nhớ rằng, theo Chương VI, §1, no. 3, Hệ quả của Mệnh đề 9, số nguyên $p+q+ 1$ chỉ có thể nhận các giá trị $1,2,3,4$.

#### Nhận xét 4 {#lie-viii-s2-n2-rem-4 .statement tag=00Z3}

Cho $(\mathfrak{g},\mathfrak{h})$ là một đại số Lie khả quy tách được, $\mathfrak{c}$ là tâm của $\mathfrak{g},\mathfrak{g}'=\mathscr{D}\mathfrak{g}$, $\mathfrak{h}'=\mathfrak{h}\cap \mathfrak{g}'$. Khi đó $\mathfrak{h}=\mathfrak{c}\times \mathfrak{h}'$, và ta đồng nhất $\mathfrak{h}^{'*}$ với một không gian con vectơ của $\mathfrak{h}^*$. Với mọi $\lambda \in \mathfrak{h}^*$ sao cho $\lambda \not= 0$, không gian con nguyên sơ $\mathfrak{g}^{\lambda}$ đối với $\lambda$ bằng ${\mathfrak{g}'}^{\lambda|\mathfrak{h}'}$. Một trọng số khác không của $\mathfrak{h}$ trên $\mathfrak{g}$ được gọi là một nghiệm của $(\mathfrak{g},\mathfrak{h})$; mọi nghiệm đều triệt tiêu trên $\mathfrak{c}$. Ký hiệu $R(\mathfrak{g},\mathfrak{h})$ là tập hợp các nghiệm của $(\mathfrak{g},\mathfrak{h})$; nó có thể được đồng nhất một cách chính tắc với $R(\mathfrak{g}',\mathfrak{h}')$. Cho $\alpha \in R(\mathfrak{g},\mathfrak{h})$. Ta định nghĩa $h_{\alpha},H_{\alpha}$, $\mathfrak{s}_{\alpha}$, các đẳng cấu $\mathfrak{s}\mathfrak{l}(2, k)\rightarrow \mathfrak{s}_{\alpha}$, và các biểu diễn của $\mathfrak{s}\mathfrak{l}(2, k)$ trên $\mathfrak{g}$ liên kết với $\alpha$, như trong trường hợp nửa đơn.

### 3. CÁC DẠNG SONG TUYẾN TÍNH BẤT BIẾN

#### Mệnh đề 5 {#lie-viii-s2-prop-5 .statement tag=00Z4}

Cho $(\mathfrak{g},\mathfrak{h})$ là một đại số Lie nửa đơn tách, $\Phi$ là một dạng song tuyến tính đối xứng bất biến trên $\mathfrak{g}$, và W là nhóm Weyl của $(\mathfrak{g},\mathfrak{h})$. Khi đó hạn chế $\Phi '$ của $\Phi$ trên $\mathfrak{h}$ là bất biến dưới W. Hơn nữa, nếu $\Phi$ không suy biến thì $\Phi '$ cũng vậy.

Cho $\alpha \in R$, $X_{\alpha}$ là một phần tử khác không của $\mathfrak{g}^{\alpha},\rho$ là biểu diễn liên kết của $\mathfrak{s}\mathfrak{l}(2, k)$ trên $\mathfrak{g}$, và $\pi$ là biểu diễn của $\mathbf{S}\mathbf{L}(2, k)$ trên $\mathfrak{g}$ tương thích với $\rho$. Khi đó $\Phi$ là bất biến dưới $\rho$, và do đó dưới $\pi ($§1, no. 4). Đặc biệt, $\Phi '$ là bất biến dưới $\theta_{\alpha}(t)|\mathfrak{h}$ (no. 2), và do đó dưới W. Khẳng định cuối cùng suy ra từ Mệnh đề 1 (i).

#### Mệnh đề 6 {#lie-viii-s2-prop-6 .statement tag=00Z5}

Cho $(\mathfrak{g},\mathfrak{h})$ là một đại số Lie nửa đơn tách, $\Phi$ là một dạng song tuyến tính đối xứng bất biến không suy biến trên $\mathfrak{g}$. Với mọi $\alpha \in R$, gọi $X_{\alpha}$ là một phần tử khác không của $\mathfrak{g}^{\alpha}$. Gọi $(H_i)_{i\in I}$ là một cơ sở của $\mathfrak{h}$, và $(H'_i)_{i\in I}$ là cơ sở của $\mathfrak{h}$ sao cho $\Phi (H_i, H'_j) =\delta_{ij}$. Khi đó phần tử Casimir liên kết với $\Phi$ trong đại số bao của $\mathfrak{g}$ (Chương I, §3, no. 7) là

$$
\sum\frac{1}{\Phi(X_{\alpha}, X_{-\alpha})}X_{\alpha}X_{-\alpha}+\sum H_iH'_i
$$

$\alpha \in Ri\in I$

Thật vậy, theo Mệnh đề $1,\Phi (H_i, X_{\alpha}) =\Phi (H'_i, X_{\alpha}) = 0$ với mọi $i\in I,\alpha \in R$, và $\Phi (\frac{1}{\Phi(X_{\alpha},X_{-\alpha})}X_{\alpha}, X_{-\beta})=\delta_{\alpha \beta}$ với mọi $\alpha , \beta \in R$.

### 4. CÁC HỆ SỐ N$_{\boldsymbol{\alpha \beta }}$

Trong số này, ta lại ký hiệu bởi $(\mathfrak{g},\mathfrak{h})$ một đại số Lie nửa đơn tách.

#### Bổ đề 2 {#lie-viii-s2-lem-2 .statement tag=00Z6}

Tồn tại một họ $(X_{\alpha})_{\alpha\in R}$ sao cho, với mọi $\alpha \in R$,

$X_{\alpha}\in \mathfrak{g}^{\alpha}$ và $[X_{\alpha}, X_{-\alpha}] =-H_{\alpha}$.

Cho $R_1$ là một tập con của R sao cho $R = R_1\cup (-R_1)$ và $R_1\cap (-R_1) =\emptyset$. Với $\alpha \in R_1$, chọn một phần tử khác không tùy ý $X_{\alpha}$ của $\mathfrak{g}^{\alpha}$. Tồn tại một phần tử duy nhất $X_{-\alpha}\in \mathfrak{g}^{-\alpha}$ sao cho $[X_{\alpha}, X_{-\alpha}] =-H_{\alpha}$ (Định lý 1 (iv)). Khi đó

$$
[X_{-\alpha}, X_{\alpha}] =H_{\alpha}=-H_{-\alpha}.Q.E.D
$$

Nếu $(X_{\alpha})_{\alpha\in R}$ là một họ thỏa mãn các điều kiện của Bổ đề 2, thì họ tổng quát nhất thỏa mãn các điều kiện ấy là $(t_{\alpha}X_{\alpha})_{\alpha\in R}$ trong đó $t_{\alpha}\in k^*$ và $t_{\alpha}t_{-\alpha}= 1$ với mọi $\alpha \in R$.

Trong phần còn lại của số này, ta ký hiệu bởi $(X_{\alpha})_{\alpha\in R}$ một họ thỏa mãn các điều kiện của Bổ đề 2. Ta ký hiệu bởi $\langle \cdot ,\cdot \rangle$ một dạng song tuyến tính đối xứng bất biến không suy biến trên $\mathfrak{g}$.

Mọi $x\in \mathfrak{g}$ đều có thể viết duy nhất dưới dạng

$$
x=h+\sum_{\alpha\in R}\mu_{\alpha}X_{\alpha}(h\in \mathfrak{h}, \mu_{\alpha}\in k)
$$

Dấu ngoặc của hai phần tử như vậy có thể được tính bằng các công thức sau:

$$
[h, X_{\alpha}] =\alpha (h)X_{\alpha}
$$

0 nếu $\alpha +\beta  \notin R\cup  \{0\}$

$[X_{\alpha}, X_{\beta}] =-H_{\alpha}$ nếu $\alpha +\beta = 0$

$N_{\alpha \beta}X_{\alpha+\beta}$ nếu $\alpha +\beta \in R$

các $N_{\alpha \beta}$ là những phần tử khác không của $k$.

#### Bổ đề 3 {#lie-viii-s2-lem-3 .statement tag=00Z7}

Với mọi $\alpha \in R$,

$$
\langle X_{\alpha}, X_{-\alpha}\rangle =-\frac{1}{2}\langle H_{\alpha}, H_{\alpha}\rangle
$$

Thật vậy,

$$
2\langle X_{\alpha}, X_{-\alpha}\rangle =\langle \alpha (H_{\alpha})X_{\alpha}, X_{-\alpha}\rangle =\langle [H_{\alpha}, X_{\alpha}], X_{-\alpha}\rangle
$$

$$
=\langle H_{\alpha},[X_{\alpha}, X_{-\alpha}]\rangle =-\langle H_{\alpha}, H_{\alpha}\rangle
$$

#### Bổ đề 4 {#lie-viii-s2-lem-4 .statement tag=00Z8}

Cho $\alpha , \beta \in R$ sao cho $\alpha +\beta \in R$. Gọi $p$ (resp. $q$) là số nguyên lớn nhất $j$ sao cho $\beta +j\alpha \in R$ (resp. $\beta -j\alpha \in R$). Khi đó,

$$
N_{\alpha ,\beta}N_{-\alpha ,\alpha+\beta}=-p(q+ 1) \tag{3}
$$

$$
N_{-\alpha ,\alpha+\beta}\langle H_{\beta}, H_{\beta}\rangle =-N_{-\alpha ,-\beta}\langle H_{\alpha+\beta}, H_{\alpha+\beta}\rangle \tag{4}
$$

$$
N_{\alpha ,\beta}N_{-\alpha ,-\beta}= (q+ 1)^2 \tag{5}
$$

Cho $\rho$ là biểu diễn của $\mathfrak{s}\mathfrak{l}(2, k)$ trên $\mathfrak{g}$ được xác định bởi $X_{\alpha}$. Phần tử $e=X_{\beta+p\alpha}$ là nguyên thủy có trọng số $p+q$ (Mệnh đề 4 (i)). Đặt

$e_n=(-n1)$! $^n\rho (X_-)^ne$ với $n\geq 0$.

Theo Mệnh đề 1 của §1,

(ad $X_{\alpha}$)$e_p= (q+ 1)e_{p-1}$

(ad $X_{-\alpha}$)(ad $X_{\alpha}$)$e_p=-p(q+ 1)e_p$.

Điều này chứng minh (3) vì $e_p$ là một phần tử khác không của $\mathfrak{g}^{\beta}$.

Do dạng $\langle \cdot ,\cdot \rangle$ là bất biến, ta có

$$
\langle [X_{-\alpha}, X_{\alpha+\beta}], X_{-\beta}\rangle =-\langle X_{\alpha+\beta},[X_{-\alpha}, X_{-\beta}]\rangle
$$

do đó

$$
N_{-\alpha ,\alpha+\beta}\langle X_{\beta}, X_{-\beta}\rangle =-N_{-\alpha ,-\beta}\langle X_{\alpha+\beta}, X_{-\alpha-\beta}\rangle
$$

điều này, theo Bổ đề 3, chứng minh (4).

Hạn chế của $\langle \cdot ,\cdot \rangle$ lên $\mathfrak{h}$ là không suy biến và bất biến dưới nhóm Weyl (Mệnh đề 5). Đồng nhất $\mathfrak{h}$ và $\mathfrak{h}^*$ bằng hạn chế này. Nếu $\gamma \in R,H_{\gamma}$ được đồng nhất với $2\gamma /\langle \gamma , \gamma \rangle$ (Chap. VI, §1, no. 1, Bổ đề 2); do đó, với mọi $\gamma , \delta \in R$,

$$
\langle \gamma , \gamma \rangle \langle H_{\delta}, H_{\delta}\rangle
$$

$$
\overline{\langle\delta , \delta\rangle}=\overline{\langle H_{\gamma}, H_{\gamma}\rangle} \tag{6}
$$

Bây giờ, theo Chap. VI, §1, no. 3, Mệnh đề 10,

$$
\frac{\langle\alpha + \beta , \alpha + \beta\rangle}{\langle\beta , \beta\rangle}=\frac{q + 1}{p} \tag{7}
$$

do đó, theo (3), (4), (6), (7),

$$
N_{\alpha ,\beta}N_{-\alpha ,-\beta}=-N_{\alpha ,\beta}N_{-\alpha ,\alpha+\beta}\frac{\langle H_{\beta}, H_{\beta}\rangle}{\langle H_{\alpha+\beta}, H_{\alpha+\beta}\rangle}
$$

$$
=-N_{\alpha ,\beta}N_{-\alpha ,\alpha+\beta}\frac{q + 1}{p}= (q+ 1)^2
$$

#### Định nghĩa 3 {#lie-viii-s2-def-3 .statement tag=00Z9}

Một hệ Chevalley cho $(\mathfrak{g},\mathfrak{h})$ là một họ $(X_{\alpha})_{\alpha\in R}$ sao cho

(i) $X_{\alpha}\in \mathfrak{g}^{\alpha}$ với mọi $\alpha \in R$;

(ii) $[X_{\alpha}, X_{-\alpha}] =-H_{\alpha}$ với mọi $\alpha \in R$;

(iii) ánh xạ tuyến tính từ $\mathfrak{g}$ vào $\mathfrak{g}$ bằng $-1$ trên $\mathfrak{h}$ và biến $X_{\alpha}$ thành $X_{-\alpha}$ với mọi $\alpha \in R$ là một tự đẳng cấu của $\mathfrak{g}$.

Việc mở rộng định nghĩa này cho trường hợp $(\mathfrak{g},\mathfrak{h})$ là khả quy tách là ngay lập tức.

Ta sẽ chỉ ra (§4, no. 4, Hệ quả của Mệnh đề 5) rằng các hệ Chevalley cho $(\mathfrak{g},\mathfrak{h})$ tồn tại.

#### Mệnh đề 7 {#lie-viii-s2-prop-7 .statement tag=00ZA}

Cho $(X_{\alpha})_{\alpha\in R}$ là một hệ Chevalley của $(\mathfrak{g},\mathfrak{h})$. Ta giữ ký hiệu của Bổ đề 4. Khi đó, $N_{-\alpha ,-\beta}= N_{\alpha ,\beta}$ và $N_{\alpha ,\beta}=\pm (q+ 1)$ với $\alpha , \beta , \alpha +\beta \in R$.

Cho $\varphi$ là tự đẳng cấu của $\mathfrak{g}$ được xét trong Định nghĩa 3 (iii). Khi đó

$$
N_{-\alpha ,-\beta}X_{-\alpha-\beta}= [X_{-\alpha}, X_{-\beta}] = [\varphi (X_{\alpha}), \varphi (X_{\beta})] =\varphi ([X_{\alpha}, X_{\beta}])
$$

$$
=\varphi (N_{\alpha ,\beta}X_{\alpha+\beta}) = N_{\alpha ,\beta}X_{-\alpha-\beta}
$$

nên $N_{-\alpha ,-\beta}= N_{\alpha ,\beta}$. Bây giờ $N_{\alpha ,\beta}=\pm (q+ 1)$ theo (5).

#### Mệnh đề 8 {#lie-viii-s2-prop-8 .statement tag=00ZB}

Cho $(X_{\alpha})_{\alpha\in R}$ là một hệ Chevalley của $(\mathfrak{g},\mathfrak{h})$. Cho M là một $\mathbf{Z}$-môđun con của $\mathfrak{h}$ chứa các $H_{\alpha}$ và được chứa trong nhóm các trọng số của $R^{\vee}$. Gọi $\mathfrak{g}_{\mathbf{Z}}$ là môđun con trên $\mathbf{Z}$ của $\mathfrak{g}$ được sinh bởi M và các $X_{\alpha}$. Khi đó $\mathfrak{g}_{\mathbf{Z}}$ là một đại số Lie con trên $\mathbf{Z}$ của $\mathfrak{g}$, và ánh xạ chính tắc từ $\mathfrak{g}_{\mathbf{Z}}\otimes_{\mathbf{Z}}k$ đến $\mathfrak{g}$ là một đẳng cấu.

Nếu $\alpha , \beta \in R$ sao cho $\alpha +\beta \in R$, thì $N_{\alpha ,\beta}\in \mathbf{Z}$ (Mệnh đề 7). Mặt khác, nếu $\alpha \in R$ và $h\in M$, thì $\alpha (h)\in \mathbf{Z}$ (Đại số, Chương VI, §1, no. 9). Điều đó chứng tỏ rằng $\mathfrak{g}_{\mathbf{Z}}$ là một đại số con Lie trên $\mathbf{Z}$ của $\mathfrak{g}$. Mặt khác, M là một nhóm Abel tự do hạng dim$\mathfrak{h}($Đại số, Chương VII, §3, Định lý 1), nên $\mathfrak{g}_{\mathbf{Z}}$ là một nhóm Abel tự do hạng dim$\mathfrak{g}$; điều này suy ra khẳng định cuối cùng.

### Bài tập {#lie-viii-s2-exercises}

Xem [các bài tập của § 2](exercises/s2/).
