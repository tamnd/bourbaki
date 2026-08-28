---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VIII
chapter_title: SPLIT SEMI-SIMPLE LIE ALGEBRAS
section: 7
section_title: Finite dimensional modules over a split semi-simple Lie algebra
lang: vi
source: lie-vii-ix
book_pages: 124-140, 238-250
pdf_pages: 0132-0148, 0246-0258
extraction: native+ocr
subsections:
    - "no": 1
      title: WEIGHTS OF A FINITE DIMENSIONAL SIMPLE $\mathfrak{g}$-MODULE
      page: 124
      pdf_page: 132
    - "no": 2
      title: HIGHEST WEIGHT OF A FINITE DIMENSIONAL SIMPLE $\mathfrak{g}$-MODULE
      page: 126
      pdf_page: 134
    - "no": 3
      title: MINUSCULE WEIGHTS
      page: 130
      pdf_page: 138
    - "no": 4
      title: TENSOR PRODUCTS OF $\mathfrak{g}$-MODULES
      page: 132
      pdf_page: 140
    - "no": 5
      title: DUAL OF A $\mathfrak{g}$-MODULE
      page: 134
      pdf_page: 142
    - "no": 6
      title: REPRESENTATION RING
      page: 136
      pdf_page: 144
    - "no": 7
      title: CHARACTERS OF $\mathfrak{g}$-MODULES
      page: 139
      pdf_page: 147
statements: 46
exercises: 27
content_sha256: 32d5dec4bca5382737d75cd64a51c422e13fc1cb54f637229e4155d0e09a5358
translated_from: content/en/lie/VIII/07_s7_finite_dimensional_modules_over_a_split.md
source_content_sha256: 07b1f00fe3cea79efdf639a1f4947eddb8bebdd9fb3701734ea3bf156aa46bd8
translation_model: gpt-5-6-mini, gpt-5-mini, gpt-5-6
translation_run: translate-vi-e69c3a82
glossary_version: 34
glossary_terms_sha256: 84278b211d488e8d7298f76d3ef1fc4fcd3ba16cbe4621e1e01cc65d55eb0dbf
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 7. MÔĐUN HỮU HẠN CHIỀU TRÊN MỘT ĐẠI SỐ LIE NỬA ĐƠN TÁCH

Trong đoạn này, ta giữ lại các ký hiệu tổng quát của §6. Ta ký hiệu P (tương ứng Q) là nhóm các trọng số của R (tương ứng các trọng số căn của R). Ta ký hiệu $P_+$ (tương ứng $Q_+$) là tập hợp các phần tử của P (tương ứng Q) dương đối với quan hệ thứ tự được xác định bởi B. Ta ký hiệu $P_{++}$ là tập hợp các trọng số trội của R đối với B (Chương VI, §1, no. 10). Một phần tử $\lambda$ của $\mathfrak{h}^*$ thuộc P (tương ứng thuộc $P_{++}$) khi và chỉ khi tất cả các $\lambda (H_{\alpha}),\alpha \in B$, là các số nguyên (tương ứng các số nguyên $\geq 0$). Ta có $P_{++}\subset P_+$ (Chương VI, §1, no. 6). Nếu $w\in W$, ta ký hiệu $\varepsilon (w)$ là định thức của $w$, bằng 1 hoặc $-1$. Ta đặt $\rho =\frac{1}{2}\sum_{\alpha\in R_+}\alpha$.

### 1. CÁC TRỌNG SỐ CỦA MỘT $\mathfrak{g}$-MÔĐUN ĐƠN HỮU HẠN CHIỀU

#### Mệnh đề 1 {#lie-viii-s7-prop-1 .statement tag=0138}

Cho V là một $\mathfrak{g}$-môđun hữu hạn chiều.

(i) Tất cả các trọng số của V đều thuộc P.

(ii) $V =\bigoplus_{\mu\in P}V^\mu$.

(iii) Với mọi $\mu\in \mathfrak{h}^*,V^\mu$ là tập hợp các $x\in V$ sao cho $h.x=\mu(h)x$ với mọi $h\in \mathfrak{h}$.

Với mọi $\alpha \in B$, tồn tại một đồng cấu từ $\mathfrak{s}\mathfrak{l}(2, k)$ vào $\mathfrak{g}$ đưa $H$ thành $H_{\alpha}$. Do đó, theo §1, no. 2, Hệ quả của Mệnh đề $2, (H_{\alpha})_V$ là chéo hóa được và các giá trị riêng của nó là các số nguyên. Vì vậy, tập hợp các $(H_{\alpha})_V$, với $\alpha \in B$, là chéo hóa được (Đại số, Chương VII, §5, no. 6, Mệnh đề 13). Do đó, với mọi $h\in \mathfrak{h},h_V$ là chéo hóa được. Theo Chương VII, §1, no. 3, Mệnh đề $9, V =\bigoplus_{\mu\in\mathfrak{h}^*}V^\mu$. Mặt khác, nếu $V^\mu\not= 0$, điều trên cho thấy rằng $\mu(H_{\alpha})\in \mathbf{Z}$ với mọi $\alpha \in B$, do đó $\mu\in P$. Điều này chứng minh (i) và (ii). Ta thấy theo cùng cách rằng $\mathfrak{h}_V$ là chéo hóa được, do đó (iii).

#### Hệ quả {#lie-viii-s7-n1-cor-1 .statement tag=0139}

Cho $\rho$ là một biểu diễn hữu hạn chiều của $\mathfrak{g}$ và $\Phi$ là dạng song tuyến tính liên kết với $\rho$.

(i) Nếu $x, y\in \mathfrak{h}_{\mathbf{Q}}$, thì $\Phi (x, y)\in \mathbf{Q}$ và $\Phi (x, x)\in \mathbf{Q}_+$.

(ii) Nếu $\rho$ là đơn ánh, hạn chế của $\Phi$ lên $\mathfrak{h}$ là không suy biến.

Mệnh đề (i) suy ra từ Mệnh đề 1 vì các phần tử của P có các giá trị hữu tỉ trên $\mathfrak{h}_{\mathbf{Q}}$. Nếu $\rho$ là đơn ánh, $\Phi$ là không suy biến (Chương I, §6, no. 1, Mệnh đề 1), do đó hạn chế của $\Phi$ lên $\mathfrak{h}$ là không suy biến (Chương VII, §1, no. 3, Mệnh đề 10 (iii)).

#### Bổ đề 1 {#lie-viii-s7-lem-1 .statement tag=013A}

Cho V là một $\mathfrak{g}$-môđun và $\rho$ là biểu diễn tương ứng của $\mathfrak{g}$.

(i) Nếu $a$ là một phần tử lũy linh của $\mathfrak{g}$, và nếu $\rho (a)$ là lũy linh địa phương,

$$
\rho (e^{ada}b) =e^{\rho(a)}\rho (b)e^{-\rho(a)}
$$

với mọi $b\in \mathfrak{g}$.

(ii) Nếu $\alpha \in R$ và nếu các ảnh qua $\rho$ của các phần tử của $\mathfrak{g}^{\alpha}$ và $\mathfrak{g}^{-\alpha}$ là lũy linh địa phương, tập hợp các trọng số của V là ổn định qua phép phản xạ $s_{\alpha}$.

Với các giả thiết trong (i), ta có $\rho$((ad $a$)$^nb$) $=$ (ad $\rho (a)$)$^n\rho (b)$ với mọi $n\geq 0$, do đó $\rho (e^{ada}b) =e^{ad\rho(a)}\rho (b)$. Mặt khác,

$$
e^{ad\rho(a)}\rho (b) =e^{\rho(a)}\rho (b)e^{-\rho(a)}
$$

là mệnh đề (ii) của Chương VII, §3, no. 1, Bổ đề 1.

Bây giờ ta chấp nhận các giả thiết trong (ii). Đặt $\theta_{\alpha}=e^{adX_{\alpha}}e^{adX_{-\alpha}}e^{adX_{\alpha}}$. Theo (i), tồn tại $S\in \mathbf{G}\mathbf{L}(V)$ sao cho $\rho (\theta_{\alpha}b) = S\rho (b)S^{-1}$ với mọi $b\in \mathfrak{g}$. Bây giờ $\theta_{\alpha}|\mathfrak{h}$ là chuyển vị của $s_{\alpha}($§2, no. 2, Bổ đề 1). Gọi $\lambda$ là một trọng số của V. Tồn tại một phần tử khác không $x$ của V sao cho $\rho (h)x=\lambda (h)x$ với mọi $h\in \mathfrak{h}$. Khi đó

$$
\rho (h)S^{-1}x= S^{-1}\rho (^ts_{\alpha}h)x= S^{-1}\lambda (^ts_{\alpha}h)x= (s_{\alpha}\lambda )(h)S^{-1}x
$$

với mọi $h\in \mathfrak{h}$. Do đó, $s_{\alpha}\lambda$ là một trọng số của V.

#### Mệnh đề 2 {#lie-viii-s7-prop-2 .statement tag=013B}

Cho V là một $\mathfrak{g}$-môđun hữu hạn chiều và $s\in$ Aut$_0(\mathfrak{g})$.

(i) Tồn tại $S\in \mathbf{G}\mathbf{L}(V)$ sao cho $(s(x))_V= Sx_VS^{-1}$ với mọi $x\in \mathfrak{g}$.

(ii) Nếu $s\in$ Aut$_e(\mathfrak{g})$, S có thể được chọn là một phần tử của $\mathbf{S}\mathbf{L}(V)$ làm cho tất cả các $\mathfrak{g}$-môđun con của V ổn định.

Mệnh đề (ii) suy ra từ Bổ đề 1 (i). Bây giờ cho $s\in$ Aut$_0(\mathfrak{g})$ và ký hiệu $\rho$ là biểu diễn của $\mathfrak{g}$ được xác định bởi V. Theo (ii), các biểu diễn $\rho$ và $\rho \circ s$ trở nên tương đương sau mở rộng vô hướng. Do đó chúng tương đương (Chương I, §3, no. 8, Mệnh đề 13), suy ra sự tồn tại của S.

#### Nhận xét 1 {#lie-viii-s7-n1-rem-1 .statement tag=013C}

Cho S thỏa mãn điều kiện trong Mệnh đề 2 (i), và đặt $\mathfrak{h}'=s(\mathfrak{h})$; ký hiệu $s^*$ là đẳng cấu $\lambda  \rightarrow \lambda \circ s^{-1}$ từ $\mathfrak{h}^*$ đến $\mathfrak{h}^{'*}$. Rõ ràng rằng

$$
S(V^{\lambda}) = V^{s^*\lambda}
$$

Đặc biệt:

#### Hệ quả 1 {#lie-viii-s7-prop-2-cor-1 .statement tag=013D}

Đẳng cấu $s^*$ đưa các trọng số của V đối với $\mathfrak{h}$ thành các trọng số của V đối với $\mathfrak{h}'$; các trọng số tương ứng có cùng bội số.

#### Hệ quả 2 {#lie-viii-s7-prop-2-cor-2 .statement tag=013E}

Cho $w\in W$. Với mọi $\lambda \in \mathfrak{h}^*$, các không gian vectơ con $V^{\lambda}$ và $V^{w\lambda}$ có cùng chiều. Tập hợp các trọng số của V là ổn định qua W.

Thật vậy, $w$ có dạng $s^*$ với $s\in$ Aut$_e(\mathfrak{g},\mathfrak{h}) ($§2, no. 2, Hệ quả của Định lý 2).

#### Nhận xét 2 {#lie-viii-s7-n1-rem-2 .statement tag=01L8}

Theo Hệ quả 1 của Mệnh đề 2 và §5, no. 3, Nhận xét 2, có ý nghĩa khi nói về các trọng số của V đối với đại số con Cartan chính tắc của $\mathfrak{g}$, và về các bội số của chúng.

#### Nhận xét 3 {#lie-viii-s7-n1-rem-3 .statement tag=013F}

Bổ đề 1 (i) và Mệnh đề 2 vẫn đúng, với cùng chứng minh, ngay cả khi $\mathfrak{g}$ không được giả thiết là khả phân.

### 2. TRỌNG SỐ CAO NHẤT CỦA MỘT $\mathfrak{g}$-MÔĐUN ĐƠN HỮU HẠN CHIỀU

#### Định lý 1 {#lie-viii-s7-thm-1 .statement tag=013G}

Một $\mathfrak{g}$-môđun đơn là hữu hạn chiều khi và chỉ khi nó có một trọng số cao nhất thuộc $P_{++}$.

Ta ký hiệu V là một $\mathfrak{g}$-môđun đơn và $\mathscr{X}$ là tập hợp các trọng số của nó.

a) Giả sử rằng V là hữu hạn chiều. Khi đó $\mathscr{X}$ là hữu hạn và không rỗng (Mệnh đề 1) và do đó có một phần tử cực đại $\omega$. Cho $\alpha \in B$. Khi đó $\omega +\alpha  \notin \mathscr{X}$, điều này chứng minh rằng $\omega$ là trọng số cao nhất của V (§6, no. 2, Bổ đề 2). Mặt khác, tồn tại một đồng cấu từ $\mathfrak{s}\mathfrak{l}(2, k)$ vào $\mathfrak{g}$ đưa $H$ thành $H_{\alpha}$; theo §1, Mệnh đề 2 (i), $\omega (H_{\alpha})$ là một số nguyên $\geq 0$, do đó $\omega \in P_{++}$.

b) Giả sử rằng V có một trọng số cao nhất $\omega \in P_{++}$. Cho $\alpha \in B$ và cho $e$ là một phần tử nguyên thủy có trọng số $\omega$ trong V. Đặt $e_j=X_{-\alpha}^je$ với $j\geq 0$,

$m=\omega (H_{\alpha})\in \mathbf{N}$, và N = $\sum_{j=0}^mke_j$. Theo §1, no. 2, Mệnh đề $1,X_{\alpha}e_{m+1}$ = 0.

Nếu $\beta \in B$ và $\beta \not=\alpha$, thì $[X_{\beta}, X_{-\alpha}] = 0$ nên $X_{\beta}e_{m+1}=X_{\beta}X_{-\alpha}^{m+1}e$ = $X_{-\alpha}^{m+1}X_{\beta}e= 0$. Nếu $e_{m+1}\not= 0$, ta kết luận rằng $e_{m+1}$ là nguyên thủy, điều này là vô lý (§6, Mệnh đề 3 (i)); vậy $e_{m+1}= 0$. Do đó, theo §1, no. 2, Hệ quả của Mệnh đề 1, N ổn định dưới đại số con $\mathfrak{s}_{\alpha}$ được sinh bởi $H_{\alpha}, X_{\alpha}$ và $X_{-\alpha}$. Bây giờ $\mathfrak{s}_{\alpha}$ là khả quy trong $\mathfrak{g}$, nên tổng của các không gian con hữu hạn chiều của V ổn định dưới $\mathfrak{s}_{\alpha}$ là một $\mathfrak{g}$-môđun con của V (Chương I, §6, no. 6, Mệnh đề 7); vì tổng này khác không, nó bằng V. Từ đó suy ra rằng $(X_{\alpha})_V$ và $(X_{-\alpha})_V$ là lũy linh địa phương. Theo Bổ đề 1 (ii), $\mathscr{X}$ ổn định dưới $s_{\alpha}$, và điều này đúng với mọi $\alpha$. Vì vậy $\mathscr{X}$ ổn định dưới W. Bây giờ mọi quỹ đạo của W trên P đều gặp $P_{++}$ (Chương VI, §1, no. 10). Mặt khác, nếu $\lambda \in \mathscr{X}\cap P_{++}$, thì $\lambda =\omega -\sum_{\alpha\in B}n_{\alpha}\alpha =\sum_{\alpha\in B}n'_{\alpha}\alpha$ với $n_{\alpha}\in \mathbf{N}$ và $n'_{\alpha}\geq 0$ với mọi $\alpha \in B$

(Chương V, §3, no. 5, Bổ đề 6). Vậy $\mathscr{X}\cap P_{++}$ là hữu hạn và do đó $\mathscr{X}$ cũng hữu hạn. Vì mỗi trọng số có bội số hữu hạn (§6, no. 1, Mệnh đề 1 (ii)), V là hữu hạn chiều.

#### Hệ quả 1 {#lie-viii-s7-thm-1-cor-1 .statement tag=013H}

Nếu $\lambda \in \mathfrak{h}^*$ và $\lambda  \notin P_{++}$, môđun $\mathfrak{g}$ $E(\lambda ) ($§6, no. 3) là vô hạn chiều.

#### Hệ quả 2 {#lie-viii-s7-thm-1-cor-2 .statement tag=013I}

Các môđun $\mathfrak{g}$ $E(\lambda )$ với $\lambda \in P_{++}$ tạo thành một tập hợp các đại diện của các lớp các môđun $\mathfrak{g}$ đơn hữu hạn chiều.

Các môđun $\mathfrak{g}$ $E(\lambda )$, trong đó $\lambda$ là một trọng số cơ bản, được gọi là các môđun $\mathfrak{g}$ cơ bản; các biểu diễn tương ứng được gọi là các biểu diễn cơ bản của $\mathfrak{g}$; chúng là bất khả quy tuyệt đối (§6, no. 2, Mệnh đề 3 (iv)).

Nếu V là một môđun $\mathfrak{g}$ hữu hạn chiều và $\lambda \in P_{++}$, thành phần đẳng kiểu của V kiểu $E(\lambda )$ được gọi là thành phần đẳng kiểu của trọng số cao nhất $\lambda$ của V.

#### Nhận xét 1 {#lie-viii-s7-n2-rem-1 .statement tag=013J}

Cho $\lambda \in P_{++},\rho_{\lambda}$ là biểu diễn của $\mathfrak{g}$ trên $E(\lambda ),s\in$ Aut($\mathfrak{g}$), và $\sigma$ là ảnh chính tắc của $s$ trong Aut(R$,B$) $($§5, no. 3, Hệ quả 1 của Mệnh đề 5). Khi đó $\rho_{\lambda}\circ s$ tương đương với $\rho_{\sigma \lambda}$; thật vậy, nếu $s\in$ Aut$_0(\mathfrak{g}),\rho_{\lambda}\circ s$ và $\rho_{\sigma \lambda}$ tương đương với $\rho_{\lambda}$ (Mệnh đề 2); và, nếu $s$ giữ $\mathfrak{h}$ và B ổn định, $\rho_{\lambda}\circ s$ là đơn có trọng số cao nhất $\sigma \lambda$.

Đặc biệt, các biểu diễn cơ bản được hoán vị bởi $s$, và phép hoán vị này là đồng nhất khi và chỉ khi $s\in$ Aut$_0(\mathfrak{g})$.

#### Mệnh đề 3 {#lie-viii-s7-prop-3 .statement tag=013K}

Cho V là một môđun $\mathfrak{g}$ hữu hạn chiều và $\mathscr{X}$ là tập hợp các trọng số của nó. Cho $\lambda \in \mathscr{X},\alpha \in R$, I là tập hợp các $t\in \mathbf{Z}$ sao cho $\lambda +t\alpha \in \mathscr{X},p$ (tương ứng $-q$) là phần tử lớn nhất (tương ứng nhỏ nhất) của I. Gọi $m_t$ là bội số của $\lambda +t\alpha$.

(i) I = $-q, p$ và $q-p=\lambda (H_{\alpha})$.

(ii) Với mọi số nguyên $u\in 0, p+q,\lambda + (p-u)\alpha$ và $\lambda + (-q+u)\alpha$ liên hợp dưới $s_{\alpha}$, và $m_{-q+u}=m_{p-u}$.

(iii) Nếu $t\in \mathbf{Z}$ và $t <(p-q)/2$, $(X_{\alpha})_V$ ánh xạ $V^{\lambda+t\alpha}$ đơn ánh vào $V^{\lambda+(t+1)\alpha}$.

(iv) Hàm $t \rightarrow m_t$ tăng trên $-q,(p-q)/2$ và giảm trên $(p-q)/2, p$.

Cho $\alpha \in B$. Cho V cấu trúc $\mathfrak{s}\mathfrak{l}(2, k$)-môđun được xác định bởi các phần tử $X_{\alpha}, X_{-\alpha}, H_{\alpha}$ của $\mathfrak{g}$. Mọi phần tử khác không của $V^{\lambda+p\alpha}$ khi đó đều là nguyên thủy. Do đó, $(\lambda +p\alpha )(H_{\alpha})\geq 0$ và $(X_{-\alpha})^rV^{\lambda+p\alpha}\not= 0$ với

$$
0\leq r\leq (\lambda +p\alpha )(H_{\alpha}) =\lambda (H_{\alpha}) + 2p
$$

(§1, no. 2, Mệnh đề 2). Suy ra rằng $V^{\lambda+t\alpha}\not= 0$ với $p\geq t\geq p-(\lambda (H_{\alpha}) + 2p)$, do đó $p+q\geq \lambda (H_{\alpha}) + 2p$. Áp dụng kết quả này cho $-\alpha$ ta được

$$
p+q\geq \lambda (H_{-\alpha}) + 2q=-\lambda (H_{\alpha}) + 2q
$$

Suy ra $q-p=\lambda (H_{\alpha})$ và $\lambda +t\alpha \in \mathscr{X}$ với $p\geq t\geq  -q$, điều này chứng minh (i).

Ta có $s_{\alpha}(\alpha ) =-\alpha$, và $s_{\alpha}(\mu)\in \mu+k\alpha$ với mọi $\mu\in \mathfrak{h}^*$. Vì W giữ $\mathscr{X}$ ổn định (Hệ quả 2 của Mệnh đề $2$)$,s_{\alpha}$ giữ $\{\lambda -q\alpha , \lambda -q\alpha +\alpha , . . . , \lambda +p\alpha \}$ ổn định và biến $\lambda -q\alpha +u\alpha$ thành $\lambda +p\alpha -u\alpha$ với mọi $u\in k$. Lại áp dụng Hệ quả 2 của Mệnh đề 2, ta thấy rằng $m_{-q+u}=m_{p-u}$ với mọi số nguyên $u\in 0, p+q$. Điều này chứng minh (ii).

Theo §1, Hệ quả của Mệnh đề $2, (X_{\alpha})_V|V^{\lambda+t\alpha}$ là đơn ánh với $t <(p-q)/2$. Bây giờ $(X_{\alpha})_V$ ánh xạ $V^{\lambda+t\alpha}$ vào $V^{\lambda+(t+1)\alpha}$. Do đó $m_{t+1}\geq m_t$ với $t <(p-q)/2$. Thay $\alpha$ bởi $-\alpha$, ta thấy rằng $m_{t+1}\leq m_t$ với $t >(p-q)/2$. Điều này chứng minh (iii) và (iv).

#### Hệ quả 1 {#lie-viii-s7-prop-3-cor-1 .statement tag=013L}

Nếu $\lambda \in \mathscr{X}$ và $\lambda (H_{\alpha})\geq 1$, thì $\lambda -\alpha \in \mathscr{X}$. Nếu $\lambda +\alpha \in \mathscr{X}$ và $\lambda (H_{\alpha}) = 0$, thì $\lambda \in \mathscr{X}$ và $\lambda -\alpha \in \mathscr{X}$.

Điều này suy ra ngay lập tức từ Mệnh đề 3 (i).

#### Hệ quả 2 {#lie-viii-s7-prop-3-cor-2 .statement tag=01J4}

Cho $\mu\in P_{++}$ và $\nu \in Q_+$. Nếu $\mu+\nu \in \mathscr{X}$, thì $\mu\in \mathscr{X}$.

Viết $\nu =\sum_{\alpha\in B}c_{\alpha}.\alpha$, trong đó $c_{\alpha}\in \mathbf{N}$ với mọi $\alpha \in B$. Hệ quả là hiển nhiên

khi $\sum_{\alpha\in B}c_{\alpha}= 0$; giả sử rằng $\sum_{\alpha\in B}c_{\alpha}>0$ và lập luận bằng quy nạp theo $\sum_{\alpha\in B}c_{\alpha}$. Gọi $(\cdot  | \cdot )$ là một dạng song tuyến tính đối xứng dương không suy biến W-bất biến trên $\mathfrak{h}^*_{\mathbf{R}}$. Khi đó $(\nu |\sum_{\alpha\in B}c_{\alpha}.\alpha )>0$, do đó tồn tại $\beta \in B$ sao cho $c_{\beta}\geq 1$ và

$(\nu |\beta )>0$, suy ra $\nu (H_{\beta})\geq 1$. Vì $\mu\in P_{++}$, ta có $(\mu+\nu )(H_{\beta})\geq 1$. Theo Hệ quả $1,\mu+ (\nu -\beta )\in \mathscr{X}$, và chỉ cần áp dụng giả thiết quy nạp.

#### Hệ quả 3 {#lie-viii-s7-prop-3-cor-3 .statement tag=013M}

Cho $v\in V$ là nguyên thủy có trọng số $\omega$. Gọi $\Sigma$ là tập hợp các $\alpha \in B$ sao cho $\omega (H_{\alpha}) = 0$. Nhóm ổn định trong $\mathfrak{g}$ của đường thẳng $kv$ là đại số con parabolic $\mathfrak{p}_{\Sigma}$ liên kết với $\Sigma ($§3, no. 4, Nhận xét).

Thay V bởi $\mathfrak{g}$-môđun con sinh bởi $v$, nếu cần, ta có thể giả sử rằng V là đơn. Gọi $\mathfrak{s}$ là nhóm ổn định. Ta có $(\mathfrak{n}_+)_Vv$ = 0, $(\mathfrak{h})_Vv\subset kv$. Cho $\alpha \in B$ sao cho $\omega (H_{\alpha}) = 0$. Ta có $\omega +\alpha  \notin \mathscr{X}$, do đó $\omega -\alpha  \notin \mathscr{X}$ (Mệnh đề 3 (i)) và do đó $(\mathfrak{g}^{-\alpha})_Vv= 0$. Điều trên chứng minh rằng $\mathfrak{p}_{\Sigma}\subset \mathfrak{s}$. Nếu $\mathfrak{p}_{\Sigma}\not=\mathfrak{s}$, thì $\mathfrak{s}=\mathfrak{p}_{\Sigma'}$, trong đó $\Sigma '$ là một tập con của B chứa thực sự $\Sigma$. Cho $\beta \in \Sigma '$ **--** $\Sigma$. Khi đó $\mathfrak{g}^{-\beta}$ ổn định $kv$, và do đó triệt tiêu $v$. Nhưng, vì $\omega (H_{\beta})>0$, điều này mâu thuẫn với Mệnh đề 3 (iii). Q.E.D.

Một tập con $\mathscr{X}$ của P được gọi là R-bão hòa nếu nó thỏa mãn điều kiện sau: với mọi $\lambda \in \mathscr{X}$ và mọi $\alpha \in R$, ta có $\lambda -t\alpha \in \mathscr{X}$ với mọi số nguyên $t$ nằm giữa 0 và $\lambda (H_{\alpha})$. Vì $s_{\alpha}(\lambda ) =\lambda -\lambda (H_{\alpha})\alpha$, ta thấy rằng một tập con R-bão hòa của P là ổn định đối với W. Cho $\mathscr{Y}\subset P$. Một phần tử $\lambda$ của $\mathscr{Y}$ được gọi là R-biên trong $\mathscr{Y}$ nếu, với mọi $\alpha \in R$, hoặc là $\lambda +\alpha  \notin \mathscr{Y}$ hoặc là $\lambda -\alpha  \notin \mathscr{Y}$.

#### Mệnh đề 4 {#lie-viii-s7-prop-4 .statement tag=013N}

Cho V là một $\mathfrak{g}$-môđun hữu hạn chiều và $d$ là một số nguyên $\geq 1$. Tập hợp các trọng số của V có bội số $\geq d$ là R-bão hòa.

Điều này suy ra ngay lập tức từ Mệnh đề 3.

#### Mệnh đề 5 {#lie-viii-s7-prop-5 .statement tag=013O}

Cho V là một $\mathfrak{g}$-môđun đơn hữu hạn chiều, $\omega$ là trọng số cao nhất của nó, $\mathscr{X}$ là tập hợp các trọng số của nó. Chọn một dạng song tuyến tính đối xứng dương bất biến theo W không suy biến $(\cdot |\cdot )$ trên $\mathfrak{h}^*_{\mathbf{R}}$, và đặt $\lambda  \rightarrow  \|\lambda \|= (\lambda |\lambda )^{1/2}$ là chuẩn tương ứng.

(i) $\mathscr{X}$ là tập con R-bão hòa nhỏ nhất của P chứa $\omega$.

(ii) Các phần tử R-cực đại của $\mathscr{X}$ là các biến đổi theo W của $\omega$.

(iii) Nếu $\mu\in \mathscr{X}$, ta có $\|\mu\| \leq  \|\omega \|$. Nếu thêm vào đó, $\mu\not=\omega$, ta có $\|\mu+\rho \|<\|\omega +\rho \|$. Nếu $\mu$ không là R-cực đại trong $\mathscr{X}$, thì $\|\mu\|<\|\omega \|$.

(iv) Ta có $\mathscr{X}= W.(\mathscr{X}\cap P_{++})$. Một phần tử $\lambda$ của $P_{++}$ thuộc $\mathscr{X}\cap P_{++}$ khi và chỉ khi $\omega -\lambda \in Q_+$.

(i) Gọi $\mathscr{X}'$ là tập con R-bão hòa nhỏ nhất của P chứa $\omega$. Ta có $\mathscr{X}'\subset \mathscr{X}$ (Mệnh đề 4). Giả sử rằng $\mathscr{X}\not=\mathscr{X}'$. Cho $\lambda$ là một phần tử cực đại của $\mathscr{X}$ **--** $\mathscr{X}'$. Vì $\lambda \not=\omega$, tồn tại $\alpha \in B$ sao cho $\lambda +\alpha \in \mathscr{X}$. Đưa vào $p$ và $q$ như trong Mệnh đề 3. Vì $\lambda$ là cực đại trong $\mathscr{X}$ **--** $\mathscr{X}',\lambda +p\alpha \in \mathscr{X}'$. Theo Mệnh đề 3 (ii), $\lambda -q\alpha \in \mathscr{X}'$ vì $\mathscr{X}'$ ổn định theo W. Do đó $\lambda +u\alpha \in \mathscr{X}'$ với mọi số nguyên $u$ trong khoảng $-q, p$. Điều này mâu thuẫn với $\lambda  \notin \mathscr{X}'$ và chứng minh (i).

(ii) Rõ ràng rằng $\omega$ là một phần tử R-cực biên của $\mathscr{X}$; các biến đổi W của nó do đó cũng là R-cực biên trong $\mathscr{X}$. Cho $\lambda$ là một phần tử R-cực biên của $\mathscr{X}$; ta sẽ chứng minh rằng $\lambda \in W.\omega$. Vì tồn tại $w\in W$ sao cho $w\lambda \in P_{++}$ (Ch. VI, §1, no. 10), ta có thể giả sử rằng $\lambda \in P_{++}$. Cho $\alpha \in B$; đưa vào $p$ và $q$ như trong Mệnh đề 3. Vì $\lambda$ là R-cực biên, hoặc $p= 0$ hoặc $q= 0$. Vì

$$
q-p=\lambda (H_{\alpha})\geq 0
$$

ta không thể có $p >0$. Do đó $p= 0$ và $\lambda =\omega$.

(iii) Cho $\mu\in \mathscr{X}\cap P_{++}$. Khi đó $\omega +\mu\in P_{++}$ và $\omega -\mu\in Q_+($§6, no. 1, Mệnh đề 1), nên $0\leq (\omega -\mu|\omega +\mu) = (\omega |\omega )-(\mu|\mu)$; do đó, $(\mu|\mu)\leq (\omega |\omega )$, và điều này mở rộng cho mọi $\mu\in \mathscr{X}$ bằng cách sử dụng nhóm Weyl. Nếu $\mu\in \mathscr{X}$ **--** $\{\omega \}$,

$$
(\mu+\rho |\mu+\rho ) = (\mu|\mu) + 2(\mu|\rho ) + (\rho |\rho )\leq (\omega |\omega ) + 2(\mu|\rho ) + (\rho |\rho )
$$

$$
= (\omega +\rho |\omega +\rho )-2(\omega -\mu|\rho )
$$

Bây giờ $\omega -\mu=\sum_{\alpha\in B}n_{\alpha}\alpha$ với các số nguyên $n_{\alpha}\geq 0$ không phải tất cả đều bằng không, nên $(\omega -\mu|\rho )>0$ vì $(\rho |\alpha )>0$ với mọi $\alpha \in B$ (Ch. VI, §1, no. 10, Mệnh đề 29 (iii)). Nếu $\mu$ không R-cực biên trong $\mathscr{X}$, tồn tại $\alpha \in R$ sao cho $\mu+\alpha \in \mathscr{X}$ và $\mu-\alpha \in \mathscr{X}$; khi đó

$\|\mu\|<$ sup($\|\mu+\alpha \|,\|\mu-\alpha \|$)$\leq$ sup$_{\lambda\in\mathscr{X}}\|\lambda \|$

và cận trên cuối cùng này là $\|\omega \|$ theo điều đã chứng minh trước đó.

(iv) Ta có $\mathscr{X}= W.(\mathscr{X}\cap P_{++})$ theo Ch. VI, §1, no. 10. Nếu $\lambda \in \mathscr{X}$, thì $\omega -\lambda \in Q_+($§6, no. 1, Mệnh đề 1). Nếu $\lambda \in P_{++}$ và $\omega -\lambda \in Q_+$, thì $\lambda \in \mathscr{X}$ (Hệ quả 2 của Mệnh đề 3).

#### Hệ quả {#lie-viii-s7-n2-cor-1 .statement tag=013P}

Cho $\mathscr{X}$ là một tập con R-bão hòa hữu hạn của P. Tồn tại một $\mathfrak{g}$-môđun hữu hạn chiều mà tập hợp các trọng số của nó là $\mathscr{X}$.

Vì $\mathscr{X}$ ổn định đối với $W,\mathscr{X}$ là tập R-bão hòa nhỏ nhất chứa $\mathscr{X}\cap P_{++}$. Theo Mệnh đề 5 (i), $\mathscr{X}$ là tập hợp các trọng số của $\bigoplus_{\lambda\in\mathscr{X}\cap P_{++}}E(\lambda )$.

#### Nhận xét 2 {#lie-viii-s7-n2-rem-2 .statement tag=013Q}

Nhắc lại (Ch. VI, §1, no. 6, Hệ quả 3 của Mệnh đề 17) rằng tồn tại một phần tử duy nhất $w_0$ của W biến B thành $-B$; ta có $w_0^2= 1$. và $-w_0$ tôn trọng quan hệ thứ tự trên P. Với điều này, cho V là một $\mathfrak{g}$-môđun đơn hữu hạn chiều, $\omega$ là trọng số cao nhất của nó. Khi đó $w_0(\omega )$ là trọng số thấp nhất của V, và bội số của nó là 1.

### 3. CÁC TRỌNG SỐ MINUSCULE

#### Mệnh đề 6 {#lie-viii-s7-prop-6 .statement tag=013R}

Cho $\lambda \in P$, và $\mathscr{X}$ là tập con R-bão hòa nhỏ nhất của P chứa $\lambda$. Chọn một chuẩn $\| \cdot  \|$ như trong Mệnh đề 5. Các điều kiện sau là tương đương:

(i) $\mathscr{X}= W.\lambda$;

(ii) mọi phần tử của $\mathscr{X}$ có cùng chuẩn;

(iii) với mọi $\alpha \in R$, ta có $\lambda (H_{\alpha})\in  \{0,1,-1\}$.

Mọi tập con R-bão hòa không rỗng của P đều chứa một phần tử $\lambda$ thỏa mãn các điều kiện trên.

Đưa vào điều kiện:

(ii$'$) với mọi $\alpha \in R$ và mọi số nguyên $t$ giữa 0 và $\lambda (H_{\alpha})$,

$$
\|\lambda -t\alpha \| \geq  \|\lambda \|
$$

(i) $=\Rightarrow$ (ii) $=\Rightarrow$ (ii$'$)$:$ Điều này là hiển nhiên.

(ii$'$) $=\Rightarrow$ (iii): Giả sử điều kiện (ii$'$) được thỏa mãn. Cho $\alpha \in R$. Ta có $\|\lambda \|=\|\lambda -\lambda (H_{\alpha})\alpha \|$, do đó $\|\lambda -t\alpha \|<\|\lambda \|$ với mọi số nguyên $t$ nằm nghiêm ngặt giữa 0 và $\lambda (H_{\alpha})$; vì vậy, không thể có các số nguyên như vậy, nên $|\lambda (H_{\alpha})| \leq 1$.

(iii) $=\Rightarrow$ (i): Giả sử điều kiện (iii) được thỏa mãn. Cho $w\in W$ và $\alpha \in R$. Khi đó $(w\lambda )(H_{\alpha}) =\lambda (H_{w^{-1}\alpha})\in  \{0,1,-1\}$; do đó, nếu $t$ là một số nguyên giữa 0 và $(w\lambda )(H_{\alpha}),w\lambda -t\alpha$ bằng $w\lambda$ hoặc $s_{\alpha}(w\lambda )$. Điều này chứng minh rằng $W.\lambda$ là R-bão hòa, vậy $\mathscr{X}= W.\lambda$.

Cho $\mathscr{Y}$ là một tập con R-bão hòa không rỗng của P. Tồn tại trong $\mathscr{Y}$ một phần tử $\lambda$ có chuẩn nhỏ nhất. Rõ ràng rằng $\lambda$ thỏa mãn điều kiện (ii$'$), do đó là khẳng định cuối cùng của mệnh đề.

#### Mệnh đề 7 {#lie-viii-s7-prop-7 .statement tag=013S}

Cho V là một $\mathfrak{g}$-môđun đơn hữu hạn chiều, $\mathscr{X}$ là tập hợp các trọng số của V, và $\lambda$ là phần tử cao nhất của $\mathscr{X}$ (xem Mệnh đề 5 (i)). Các điều kiện (i), (ii) và (iii) của Mệnh đề 6 tương đương với:

(iv) với mọi $\alpha \in R$ và mọi $x\in \mathfrak{g}^{\alpha}$, ta có $(x_V)^2= 0$.

Nếu các điều kiện này được thỏa mãn, mọi trọng số của V đều có bội số 1.

Nếu (i) được thỏa mãn, thì $\mathscr{X}= W.\lambda$ và các trọng số đều có cùng bội số với $\lambda$ (Hệ quả 2 của Mệnh đề 2), nói cách khác, bội số bằng 1. Hơn nữa, nếu $w\in W$ và $\alpha \in R,w\lambda +t\alpha$ không thể là một trọng số của V trừ khi $|t| \leq 1$; do đó, nếu $x\in \mathfrak{g}^{\alpha}$,

$$
(x_V)^2(V^{w(\lambda)})\subset V^{w(\lambda)+2\alpha}= 0
$$

nên $(x_V)^2= 0$, điều này chứng minh rằng (i) $=\Rightarrow$ (iv).

Ngược lại, giả sử rằng (iv) được thỏa mãn. Cho $\alpha \in R$, và cho V cấu trúc môđun $\mathfrak{s}\mathfrak{l}(2, k)$ được xác định bởi các phần tử $X_{\alpha}, X_{-\alpha}, H_{\alpha}$ của $\mathfrak{g}$. Điều kiện (iv), áp dụng cho $x=X_{\alpha}$, suy ra rằng các trọng số của môđun $\mathfrak{s}\mathfrak{l}(2, k$)-môđun V thuộc vào $\{0,1,-1\}$ (xem §1, no. 2, Hệ quả của Mệnh đề 2). Đặc biệt, $\lambda (H_{\alpha})\in  \{0,1,-1\}$, do đó (iv) $=\Rightarrow$ (iii).

#### Mệnh đề 8 {#lie-viii-s7-prop-8 .statement tag=013T}

Giả sử rằng $\mathfrak{g}$ là đơn. Ký hiệu bởi $\alpha_1, . . . , \alpha_l$ các phần tử của B. Gọi $\varpi_1, . . . , \varpi_l$ là các trọng số cơ bản tương ứng. Gọi $H$ = $n_1H_{\alpha_1}+\cdots +n_lH_{\alpha_l}$ là nghiệm cao nhất của $R^{\vee}$, và J là tập hợp các $i\in  \{1, . . . , l\}$ sao cho $n_i= 1$. Cho $\lambda \in P_{++}$ **--** $\{0\}$. Khi đó các điều kiện (i), (ii) và (iii) của Mệnh đề 6 tương đương với từng điều kiện sau:

(v) $\lambda (H) = 1$;

(vi) tồn tại $i\in J$ sao cho $\lambda =\varpi_i$.

Các $\varpi_i$, với $i\in J$, tạo thành một hệ các đại diện trong P(R) của các phần tử khác không của $P(R)/Q(R)$.

Cho $\lambda =u_1\varpi_1+\cdots +u_l\varpi_l$, trong đó $u_1, . . . , u_l$ là các số nguyên $\geq 0$ và không đồng thời bằng không. Khi đó $\lambda (H) =u_1n_1+\cdots +u_ln_l$ và $n_1\geq 1, . . . , n_l\geq 1$, điều này cho ngay lập tức sự tương đương của (v) và (vi). Mặt khác, $\lambda (H) =$ sup$_{\alpha\in R_+}\lambda (H_{\alpha})$, và $\lambda (H)>0$ vì $\lambda$ là một phần tử khác không của $P_{++}$. Do đó

điều kiện (v) tương đương với điều kiện $\lambda (H_{\alpha})\in  \{0,1\}$ với mọi $\alpha \in R$, nói cách khác tương đương với điều kiện (iii) của Mệnh đề 6.

Khẳng định cuối cùng của mệnh đề suy ra từ Chap. VI, §2, no. 3, Hệ quả của Mệnh đề 6.

#### Định nghĩa 1 {#lie-viii-s7-def-1 .statement tag=013U}

Giả sử rằng $\mathfrak{g}$ là đơn. Một trọng lượng minuscule của $(\mathfrak{g},\mathfrak{h})$ là một phần tử của $P_{++}$ **--** $\{0\}$ thỏa mãn các điều kiện tương đương (i), (ii), (iii), (iv), (v) và (vi) của Mệnh đề 6, 7 và 8.

#### Nhận xét {#lie-viii-s7-n3-rem-1 .statement tag=013V}

Giả sử rằng $\mathfrak{g}$ là đơn. Gọi $\Sigma^{'\vee}$ là đồ thị Coxeter của nhóm Weyl affine $W_a(R^{\vee})$. Nhắc lại rằng các đỉnh của $\Sigma^{'\vee}$ là các đỉnh của đồ thị Coxeter $\Sigma^{\vee}$ của $W(R^{\vee})$, cùng với một đỉnh phụ 0. Nhóm $A(R^{\vee})$ tác động trên $\Sigma^{'\vee}$ và giữ 0 cố định. Nhóm Aut($\Sigma^{'\vee}$) đẳng cấu chính tắc với tích nửa trực tiếp của $A(R^{\vee})/W(R^{\vee})$ với một nhóm $\Gamma_C$ (xem Chương VI, §2, no. 3, và Chương VI, §4, no. 3); rõ ràng (Aut $\Sigma^{'\vee}$)$(0) =\Gamma_C(0)$; và $\Gamma_C(0)$ gồm 0 và các đỉnh của $\Sigma^{\vee}$ tương ứng với các $\varpi_i$ với $i\in J$ (xem Chương VI, §2, Mệnh đề 5 và Nhận xét 1 của no. 3). Tóm lại, các trọng số tối tiểu là các trọng số cơ bản tương ứng với các đỉnh của $\Sigma^{\vee}$ có thể thu được từ 0 bởi phép toán của một phần tử của Aut($\Sigma^{'\vee}$).

Với các ký hiệu của Chương VI, các Bảng I đến IX, từ điều trước suy ra rằng các trọng số tối tiểu là các trọng số sau:

Đối với kiểu $A_l(l\geq 1):\varpi_1, . . . , \varpi_l$.

Đối với kiểu $B_l(l\geq 2):\varpi_l$.

Đối với kiểu $C_l(l\geq 2):\varpi_1$.

Đối với kiểu $D_l(l\geq 3):\varpi_1, \varpi_{l-1}, \varpi_l$.

Đối với kiểu $E_6:\varpi_1, \varpi_6$.

Đối với kiểu $E_7:\varpi_7$.

Đối với các kiểu $E_8,F_4,G_2$ không có trọng số tối tiểu.

### 4. TÍCH TENXƠ CỦA $\mathfrak{g}$-MÔĐUN

Cho $E,F$ là các $\mathfrak{g}$-môđun. Với mọi $\lambda , \mu\in \mathfrak{h}^*, E^{\lambda}\otimes F^\mu\subset (E\otimes F)^{\lambda+\mu}$ (Chương VII, §1, no. 1, Mệnh đề 2 (ii)). Nếu E và F là hữu hạn chiều, thì $E =\sum_{\lambda\in P}E^{\lambda}$

và $F =\sum_{\mu\in P}F^\mu$; do đó,

$$
(E\otimes F)^{\nu}=\sum_{\lambda ,\mu\in P,\lambda+\mu=\nu}E^{\lambda}\otimes F^\mu
$$

Nói cách khác, được trang bị phân bậc kiểu $P, E\otimes F$ là tích tenxơ phân bậc của các không gian vectơ phân bậc E và F.

#### Mệnh đề 9 {#lie-viii-s7-prop-9 .statement tag=013W}

Cho $E,F$ là các $\mathfrak{g}$-môđun đơn hữu hạn chiều, với các trọng số cao nhất lần lượt là $\lambda , \mu$.

(i) Thành phần của $E\otimes F$ có trọng số cao nhất $\lambda +\mu$ là một môđun con đơn, được sinh bởi $(E\otimes F)^{\lambda+\mu}= E^{\lambda}\otimes F^\mu$.

(ii) Trọng số cao nhất của bất kỳ môđun con đơn nào của $E\otimes F$ đều $\leq \lambda +\mu$ (xem §9, Mệnh đề 2).

Nếu $\alpha , \beta \in P$ và nếu $E^{\alpha}\otimes F^{\beta}\not= 0$, thì $\alpha \leq \lambda$ và $\beta \leq \mu$. Do đó, $(E\otimes F)^{\lambda+\mu}$ bằng $E^{\lambda}\otimes F^\mu$, và vì vậy có chiều bằng 1, và $\lambda +\mu$ là trọng số cao nhất của $E\otimes F$. Mọi phần tử khác không của $E^{\lambda}\otimes F^\mu$ đều là nguyên thủy. Theo Mệnh đề 4 của §6, no. 2, độ dài của thành phần đẳng kiểu của $E\otimes F$ có trọng số cao nhất $\lambda +\mu$ là 1.

#### Nhận xét {#lie-viii-s7-n4-rem-1 .statement tag=013X}

Giữ lại các ký hiệu của Mệnh đề 9. Gọi C là thành phần đẳng kiểu của $E\otimes F$ có trọng số cao nhất $\lambda +\mu$. Khi đó C chỉ phụ thuộc vào E và F chứ không phụ thuộc vào lựa chọn $\mathfrak{h}$ và cơ sở B. Nói cách khác, cho $\mathfrak{h}'$ là một đại số con Cartan tách của $\mathfrak{g}, R'$ là hệ nghiệm của $(\mathfrak{g},\mathfrak{h}')$, và $B'$ là một cơ sở của $R'$; cho $\lambda ', \mu'$ là các trọng số cao nhất của $E,F$ tương ứng với $\mathfrak{h}'$ và $B'$; cho $C'$ là thành phần đẳng kiểu của $E\otimes F$ có trọng số cao nhất $\lambda '+\mu'$; khi đó $C'= C$. Thật vậy, để chứng minh điều này ta có thể giả sử, bằng mở rộng trường cơ sở, rằng $k$ là đóng đại số. Khi đó tồn tại $s\in$ Aut$_e(\mathfrak{g})$ biến $\mathfrak{h}$ thành $\mathfrak{h}', R$ thành $R', B$ thành $B'$. Cho $S\in \mathbf{S}\mathbf{L}(E\otimes F)$ có các tính chất trong Mệnh đề 2 của no. 1. Khi đó $S((E\otimes F)^{\lambda+\mu}) = (E\otimes F)^{\lambda'+\mu'}$ và S(C) = C. Do đó $(E\otimes F)^{\lambda'+\mu'}\subset C'\cap S(C) = C'\cap C$, suy ra $C'= C$. Như vậy, với 2 lớp các môđun $\mathfrak{g}$ đơn hữu hạn chiều ta có thể gán một lớp thứ ba một cách chính tắc; nói cách khác, ta đã xác định trên tập hợp $\mathfrak{S}_{\mathfrak{g}}$ các lớp của các môđun $\mathfrak{g}$ đơn hữu hạn chiều một luật hợp thành. Với cấu trúc này, $\mathfrak{S}_{\mathfrak{g}}$ đẳng cấu một cách chính tắc với nửa nhóm cộng tính $P_{++}$.

#### Hệ quả 1 {#lie-viii-s7-prop-9-cor-1 .statement tag=01J5}

Cho $(\varpi_{\alpha})_{\alpha\in B}$ là họ các trọng số cơ bản tương ứng với B. Cho $\lambda =\sum_{\alpha\in B}m_{\alpha}\varpi_{\alpha}\in P_{++}$. Với mọi $\alpha \in B$, cho $E_{\alpha}$ là một môđun $\mathfrak{g}$ đơn có trọng số cao nhất $\varpi_{\alpha}$. Trong môđun $\mathfrak{g}$ $\bigotimes_{\alpha\in B}(\bigotimes^{m_{\alpha}}E_{\alpha})$, thành phần đẳng kiểu có trọng số cao nhất $\lambda$ có độ dài 1.

Điều này suy ra từ Mệnh đề 9 bằng quy nạp theo $\sum_{\alpha\in B}m_{\alpha}$.

#### Hệ quả 2 {#lie-viii-s7-prop-9-cor-2 .statement tag=013Y}

Giả sử rằng $k$ là $\mathbf{R}$ hoặc $\mathbf{C}$ hoặc một trường ultrametric đầy đủ không rời rạc. Cho G là một nhóm Lie có đại số Lie $\mathfrak{g}$. Giả sử rằng, với mọi biểu diễn cơ bản $\rho$ của $\mathfrak{g}$, tồn tại một biểu diễn tuyến tính giải tích $\rho '$ của G sao cho $\rho = L(\rho ')$. Khi đó, với mọi biểu diễn tuyến tính hữu hạn chiều $\pi$ của $\mathfrak{g}$, tồn tại một biểu diễn tuyến tính giải tích $\pi '$ của G sao cho $\pi = L(\pi ')$.

Ta sử dụng các ký hiệu của Hệ quả 1. Có một biểu diễn $\sigma$ của G trên $X =\bigotimes_{\alpha\in B}(\bigotimes^{m_{\alpha}}E_{\alpha})$ sao cho $L(\sigma )$ tương ứng với cấu trúc $\mathfrak{g}$-môđun của X (Chương III, §3, no. 11, Hệ quả 3 của Mệnh đề 41). Gọi C là thành phần đẳng kiểu của X có trọng số cao nhất $\lambda$. Theo Chương III, §3, no. 11, Mệnh đề 40, chỉ cần chứng minh rằng C ổn định dưới $\sigma (G)$. Cho $g\in G$ và $\varphi =$ Ad($g$). Khi đó $\sigma (g)a_X\sigma (g)^{-1}= (\varphi (a))_X$ với mọi $a\in \mathfrak{g}$. Mặt khác, $\varphi$ là một tự đẳng cấu của $\mathfrak{g}$ đưa $\mathfrak{h}$ vào $\mathfrak{h}'$, $R$ vào $R'= R(\mathfrak{g},\mathfrak{h}')$, $B$ vào một cơ sở $B'$ của $R'$, và $\varpi_{\alpha}$ vào trọng số cao nhất $\varpi '_{\alpha}$ của $E_{\alpha}$ đối với $\mathfrak{h}'$ và $B'$ (vì $\varphi$ biến $E_{\alpha}$ thành một $\mathfrak{g}$-môđun đẳng cấu với $E_{\alpha}$). Do đó $\varphi$ đưa $\lambda$ thành $\sum m_{\alpha}\varpi '_{\alpha}$. Theo Nhận xét ở trên, $\sigma (g)(C) = C$.

#### Mệnh đề 10 {#lie-viii-s7-prop-10 .statement tag=013Z}

Cho $\lambda , \mu\in P_{++}$. Cho $E,F,G$ là các $\mathfrak{g}$-môđun đơn có các trọng số cao nhất $\lambda , \mu, \lambda +\mu$. Gọi $\mathscr{X}$ (tương ứng $\mathscr{X}',\mathscr{X}''$) là tập hợp các trọng số của E (tương ứng $F,G$). Khi đó $\mathscr{X}''=\mathscr{X}+\mathscr{X}'$.

Ta có $E =\bigoplus_{\nu\in P}E^{\nu},F =\bigoplus_{\sigma\in P}F^{\sigma}$, do đó $E\otimes F$ là tổng trực tiếp của

$$
(E\otimes F)^{\tau}=\sum_{\nu+\sigma=\tau}E^{\nu}\otimes F^{\sigma}
$$

Theo Mệnh đề 9, G có thể được đồng nhất với một $\mathfrak{g}$-môđun con của $E\otimes F$, do đó $\mathscr{X}''\subset \mathscr{X}+\mathscr{X}'$. Ta có $G^{\tau}= G\cap (E\otimes F)^{\tau}$, và chỉ cần chứng minh rằng, với $\nu \in \mathscr{X}$ và $\sigma \in \mathscr{X}'$, ta có $G\cap (E\otimes F)^{\nu+\sigma}\not= 0$. Gọi $(e_1, . . . , e_n)$ (tương ứng $(f_1, . . . , f_p)$) là một cơ sở của E (tương ứng F) gồm các phần tử mà mỗi phần tử đều thuộc một $E^{\nu}$ (tương ứng $F^{\sigma}$) nào đó, và sao cho $e_1\in E^{\lambda}$ (tương ứng $f_1\in F^\mu$). Các $e_i\otimes f_j$ lập thành một cơ sở của $E\otimes F$. Giả sử kết quả cần chứng minh là sai. Khi đó tồn tại một cặp $(i, j)$ sao cho tọa độ có chỉ số $(i, j)$ của mọi phần tử của G đều bằng không. Gọi U là đại số bao quanh của $\mathfrak{g}, U'$ là đối ngẫu của $U,c$ là đồng tích của U. Với mọi $u\in U$, gọi $x_i(u)$ (tương ứng $y_j(u)$) là tọa độ có chỉ số i (tương ứng j) của $u(e_1)$ (tương ứng $u(f_1)$); gọi $z_{ij}(u)$ là tọa độ có chỉ số $(i, j)$ của $u(e_1\otimes f_1)$. Khi đó $x_i, y_j, z_{ij}\in U'$. Bây giờ $e_1$ sinh ra $\mathfrak{g}$-môđun E, nên $x_i\not= 0$, và tương tự $y_j\not= 0$. Theo định nghĩa của $\mathfrak{g}$-môđun $E\otimes F$ (Chap. I, §3, no. 2), nếu $c(u) =\sum u_s\otimes u'_s$, ta có

$$
z_{ij}(u) =\sum_sx_i(u_s).y_j(u'_s) =\langle c(u), x_i\otimes y_j\rangle
$$

Nói cách khác, $z_{ij}$ là tích của $x_i$ và $y_j$ trong đại số $U'$. Nhưng đại số này là một miền nguyên (Chap. II, §1, no. 5, Mệnh đề 10), do đó $z_{ij}\not= 0$. Vì $u(e_1\otimes f_1)\in G$ với mọi $u\in U$, đây là một mâu thuẫn.

### 5. Đối ngẫu của một $\mathfrak{g}$-môđun

Cho $E,F$ là các $\mathfrak{g}$-môđun. Nhắc lại (Chap. I, §3, no. 3) rằng Hom$_k(E,F)$ có một cấu trúc $\mathfrak{g}$-môđun chính tắc. Gọi $\varphi$ là một phần tử có trọng số $\lambda$ trong Hom$_k(E,F)$. Nếu $\mu\in \mathfrak{h}^*$, thì $\varphi (E^\mu)\subset F^{\lambda+\mu}$ (Chap. VII, §1, no. 1, Mệnh đề 2 (ii)). Do đó, nếu E và F là hữu hạn chiều, các phần tử có trọng số $\lambda$ trong Hom$_k(E,F)$ là các đồng cấu phân bậc có bậc $\lambda$ theo nghĩa của Đại số, Chap. II, §11, no. 2, Định nghĩa 4.

#### Mệnh đề 11 {#lie-viii-s7-prop-11 .statement tag=0140}

Cho E là một $\mathfrak{g}$-môđun hữu hạn chiều, và xét $\mathfrak{g}$-môđun $E^*=$ Hom$_k(E, k)$.

(i) Một phần tử $\lambda \in P$ là một trọng số của $E^*$ khi và chỉ khi $-\lambda$ là một trọng số của E, và bội số của $\lambda$ trong $E^*$ bằng bội số của $-\lambda$ trong E.

(ii) Nếu E là đơn và có trọng số cao nhất $\omega ,E^*$ là đơn và có trọng số cao nhất $-w_0(\omega )$ (xem no. 2, Nhận xét 2).

Xét $k$ như một $\mathfrak{g}$-môđun tầm thường mà các phần tử của nó có trọng số 0. Theo điều đã nói ở trên, các phần tử của $E^*$ có trọng số $\lambda$ là các đồng cấu từ E vào $k$ triệt tiêu trên $E^\mu$ nếu $\mu\not=-\lambda$. Điều này chứng minh (i). Nếu E là đơn, $E^*$ là đơn (Chương I, §3, no. 3), và khẳng định cuối cùng suy ra từ Nhận xét 2 của no. 2.

#### Nhận xét 1 {#lie-viii-s7-n5-rem-1 .statement tag=0141}

Cho $E,E^*$ như trong Mệnh đề 11, và $\sigma \in$ Aut($\mathfrak{g},\mathfrak{h}$) sao cho $\varepsilon (\sigma ) =-w_0$ theo các ký hiệu của §5, no. 1 (§5, no. 2, Mệnh đề 2). Gọi $\rho , \rho '$ là các biểu diễn của $\mathfrak{g}$ liên kết với $E,E^*$. Khi đó $\rho \circ \sigma$ là một biểu diễn đơn của $\mathfrak{g}$ có trọng số cao nhất $-w_0(\omega )$, do đó $\rho \circ \sigma$ tương đương với $\rho '$.

#### Nhận xét 2 {#lie-viii-s7-n5-rem-2 .statement tag=0142}

Giả sử rằng $w_0=-1$. Khi đó, với mọi $\mathfrak{g}$-môđun hữu hạn chiều E, E đẳng cấu với $E^*$. Nhắc lại rằng, nếu $\mathfrak{g}$ là đơn, thì $w_0=-1$ trong các trường hợp sau: $\mathfrak{g}$ kiểu $A_1,B_l(l\geq 2), C_l(l\geq 2), D_l(l$ chẵn $\geq 4), E_7,E_8,F_4,G_2$ (Chương VI, Các bảng).

#### Bổ đề 2 {#lie-viii-s7-lem-2 .statement tag=0143}

Cho $h^0=\sum_{\alpha\in R_+}H_{\alpha}$. Khi đó $h^0=\sum_{\alpha\in B}a_{\alpha}H_{\alpha}$, trong đó các $a_{\alpha}$ là các số nguyên $\geq 1$. Cho $(b_{\alpha})_{\alpha\in B},(c_{\alpha})_{\alpha\in B}$ là các họ vô hướng sao cho $b_{\alpha}c_{\alpha}=a_{\alpha}$ với mọi $\alpha \in B$. Đặt $x=\sum_{\alpha\in B}b_{\alpha}X_{\alpha}, y=\sum_{\alpha\in B}c_{\alpha}X_{-\alpha}$. Tồn tại một đồng cấu $\varphi$

từ $\mathfrak{s}\mathfrak{l}(2, k)$ vào $\mathfrak{g}$ sao cho $\varphi (H) =h^0, \varphi (X_+) =x, \varphi (X_-) =y$.

Sự kiện các $a_{\alpha}$ là các số nguyên $\geq 1$ suy ra từ sự kiện $(H_{\alpha})_{\alpha\in B}$ là một cơ sở của hệ nghiệm $(H_{\alpha})_{\alpha\in B}$ (xem Chương VI, §1, no. 5, Nhận xét 5). Ta có:

$$
\alpha (h^0) = 2 \tag{1}
$$

với mọi $\alpha \in B$ (Chương VI, §1, no. 10, Hệ quả của Mệnh đề 29), do đó

$$
[h^0, x] =\sum_{\alpha\in B}b_{\alpha}\alpha (h^0)X_{\alpha}= 2x \tag{2}
$$

$$
[h^0, y] =\sum_{\alpha\in B}c_{\alpha}(-\alpha (h^0))X_{-\alpha}=-2y \tag{3}
$$

Mặt khác,

$$
[x, y] =\sum_{\alpha ,\beta\in B}b_{\alpha}c_{\beta}[X_{\alpha}, X_{-\beta}] =\sum_{\alpha\in B}b_{\alpha}c_{\alpha}[X_{\alpha}, X_{-\alpha}] =-\sum_{\alpha\in B}a_{\alpha}H_{\alpha}=-h^0 \tag{4}
$$

do đó tồn tại đồng cấu $\varphi$.

#### Mệnh đề 12 {#lie-viii-s7-prop-12 .statement tag=0144}

Cho E là một môđun đơn hữu hạn chiều của $\mathfrak{g}$, $\omega$ là trọng số cao nhất của nó, và $\mathscr{B}$ là không gian vectơ của các dạng song tuyến tính bất biến bởi $\mathfrak{g}$ trên E. Cho $m$ là số nguyên $\sum_{\alpha\in R_+}\omega (H_{\alpha})$, sao cho $m/2$ là tổng các tọa độ của $\omega$ đối với B (Ch. VI, §1, no. 10, Hệ quả của Mệnh đề 29). Cho $w_0$ là phần tử của W sao cho $w_0(B) =-B$.

(i) Nếu $w_0(\omega )\not=-\omega$, thì $\mathscr{B}= 0$.

(ii) Giả sử rằng $w_0(\omega ) =-\omega$. Khi đó $\mathscr{B}$ có chiều 1, và mọi phần tử khác không của $\mathscr{B}$ đều không suy biến. Nếu $m$ là chẵn (tương ứng lẻ), mọi phần tử của $\mathscr{B}$ đều đối xứng (tương ứng phản xứng).

$a)$ Cho $\Phi \in \mathscr{B}$. Ánh xạ $\varphi$ từ E vào $E^*$ được xác định, với $x, y\in E$, bởi $\varphi (x)(y) =$ $\Phi (x, y)$ là một đồng cấu của các $\mathfrak{g}$-môđun. Nếu $\Phi \not= 0$, thì $\varphi \not= 0$, do đó $\varphi$ là một đẳng cấu theo Bổ đề Schur, và do đó $\Phi$ không suy biến. Do đó, môđun $\mathfrak{g}$ E là đẳng cấu với môđun $\mathfrak{g}$ $E^*$, sao cho $w_0(\omega ) =-\omega$. Như vậy ta đã chứng minh (i).

$b)$ Từ đây giả sử rằng $w_0(\omega)=-\omega$. Khi đó E đẳng cấu với $E^*$. Không gian vectơ $\mathscr B$ đẳng cấu với $\operatorname{Hom}_{\mathfrak g}(E,E^*)$, và do đó với $\operatorname{Hom}_{\mathfrak g}(E,E)$ có chiều 1 (§6, no. 1, Mệnh đề 1 (iii)). Suy ra $\dim \mathscr B=1$. Mọi phần tử khác không $\Phi$ của $\mathscr B$ đều không suy biến theo a). Đặt $\Phi_1(x,y)=\Phi(y,x)$ với $x,y\in E$. Theo điều trên, tồn tại $\lambda\in k$ sao cho $\Phi_1(x,y)=\lambda\Phi(x,y)$ với mọi $x,y\in E$. Khi đó $\Phi(y,x)=\lambda\Phi(x,y)=\lambda^2\Phi(y,x)$, nên $\lambda^2=1$ và $\lambda=\pm1$. Do đó, $\Phi$ hoặc đối xứng hoặc phản xứng.

$c)$ Theo Chương VII, §1, no. 3, Mệnh đề 9 (v), $E^\lambda$ và $E^\mu$ là trực giao đối với $\Phi$ nếu $\lambda+\mu\ne0$. Vì $\Phi$ không suy biến, suy ra rằng $E^\omega,E^{-\omega}$ không trực giao đối với $\Phi$.

$d)$ Tồn tại một đồng cấu $\varphi$ từ $\mathfrak{sl}(2,k)$ lên một đại số con của $\mathfrak g$ biến $H$ thành
$$
\sum_{\alpha\in R_+}H_\alpha
$$
(Bổ đề 2). Xét E như một $\mathfrak{sl}(2,k)$-môđun qua đồng cấu này. Khi đó các phần tử của $E^\lambda$ có trọng số $\lambda\left(\sum_{\alpha\in R_+}H_\alpha\right)$. Nếu $\lambda\in P$ là sao cho $E^\lambda\ne0$ và $\lambda\ne\omega,\lambda\ne-\omega$, thì $-\omega<\lambda<\omega$, do đó
$$
-m=-\omega\left(\sum_{\alpha\in R_+}H_\alpha\right)<\lambda\left(\sum_{\alpha\in R_+}H_\alpha\right)<\omega\left(\sum_{\alpha\in R_+}H_\alpha\right)=m.
$$
Gọi G là thành phần đẳng kiểu kiểu V$(m)$ của $\mathfrak{sl}(2,k)$-môđun E. Theo điều trên, G có độ dài 1 và chứa $E^\omega,E^{-\omega}$. Theo c), hạn chế của $\Phi$ lên G là khác không. Theo §1, no. 3, Nhận xét 3, $\pi$ là chẵn hoặc lẻ tùy theo hạn chế này là đối xứng hay phản xứng. Theo b), điều này hoàn thành chứng minh.

#### Định nghĩa 2 {#lie-viii-s7-def-2 .statement tag=01J6}

Một biểu diễn bất khả quy hữu hạn chiều $\rho$ của $\mathfrak g$ được gọi là trực giao (tương ứng đối xứng symplectic) nếu trên E tồn tại một dạng song tuyến tính đối xứng (tương ứng phản xứng) không suy biến bất biến dưới $\rho$.

### 6. VÀNH BIỂU DIỄN

Cho $\mathfrak a$ là một đại số Lie hữu hạn chiều. Gọi $\mathscr F_{\mathfrak a}$ (tương ứng $\mathscr G_{\mathfrak a}$) là tập hợp các lớp của các $\mathfrak a$-môđun hữu hạn chiều (tương ứng hữu hạn chiều đơn). Gọi $\mathscr R(\mathfrak a)$ là nhóm Abel tự do $\mathbf Z^{(\mathscr G_{\mathfrak a})}$. Với mọi $\mathfrak a$-môđun đơn hữu hạn chiều E, ký hiệu lớp của nó là $[E]$. Cho F là một $\mathfrak a$-môđun hữu hạn chiều; gọi
$$
(F_n,F_{n-1},\ldots,F_0)
$$
là một chuỗi Jordan-Hölder của F; phần tử
$$
\sum_{i=1}^{n}[F_i/F_{i-1}]
$$
của $\mathscr R(\mathfrak a)$ chỉ phụ thuộc vào F chứ không phụ thuộc vào lựa chọn chuỗi Jordan-Hölder; ta ký hiệu nó là $[F]$. Nếu
$$
0\longrightarrow F'\longrightarrow F\longrightarrow F''\longrightarrow0
$$
là một dãy khớp của các $\mathfrak a$-môđun hữu hạn chiều, thì $[F]=[F']+[F'']$.

Cho F là một $\mathfrak{a}$-môđun nửa đơn hữu hạn chiều; với mọi $E\in \mathfrak{S}_{\mathfrak{a}}$, gọi $n_E$ là độ dài của thành phần đẳng kiểu của F kiểu E; khi đó [F] = $\sum_{E\in\mathfrak{S}_{\mathfrak{a}}}n_E.E$. Nếu $F,F'$ là các $\mathfrak{a}$-môđun nửa đơn hữu hạn chiều, và nếu [F] = $[F']$, thì F và $F'$ là đẳng cấu.

#### Bổ đề 3 {#lie-viii-s7-lem-3 .statement tag=0145}

Cho G là một nhóm Abel viết theo phép cộng, và $\varphi :\mathscr{F}_{\mathfrak{a}}\rightarrow G$ là một ánh xạ; bằng lạm dụng ký hiệu, ta ký hiệu bởi $\varphi (F)$ ảnh qua $\varphi$ của lớp của bất kỳ $\mathfrak{a}$-môđun hữu hạn chiều F nào. Giả sử rằng, với mọi dãy khớp

$$
0\longrightarrow F'\longrightarrow F\longrightarrow F''\longrightarrow 0
$$

các môđun $\mathfrak{a}$-hữu hạn chiều, ta có $\varphi (F) =\varphi (F') +\varphi (F'')$. Khi đó, tồn tại một đồng cấu duy nhất $\theta :\mathscr{R}(\mathfrak{a})\rightarrow G$ sao cho $\theta ([F]) =\varphi (F)$ với mọi môđun $\mathfrak{a}$-hữu hạn chiều F.

Tồn tại một đồng cấu duy nhất $\theta$ từ $\mathscr{R}(\mathfrak{a})$ đến G sao cho $\theta ([E]) =\varphi (E)$ với mọi môđun $\mathfrak{a}$ đơn hữu hạn chiều E. Cho F là một môđun $\mathfrak{a}$ hữu hạn chiều, và $(F_n,F_{n-1}, . . . ,F_0)$ là một chuỗi Jordan-Hölder của F; nếu $n >0$, ta có, theo quy nạp trên $n$,

$$
\theta ([F]) =\sum_{i=1}^n\theta ([F_i/F_{i-1}]) =\sum_{i=1}^n\varphi (F_i/F_{i-1}) =\varphi (F)
$$

Nếu $n= 0$ thì [F] = 0 nên $\theta ([F]) = 0$; mặt khác, bằng cách xét dãy khớp $0\longrightarrow 0\longrightarrow 0\longrightarrow 0\longrightarrow 0$ ta thấy rằng $\varphi (0) = 0$.

#### Ví dụ {#lie-viii-s7-n6-exa-1 .statement tag=0146}

Lấy $G =\mathbf{Z}$ và $\varphi (F) =$ dim F. Đồng cấu tương ứng từ $\mathscr{R}(\mathfrak{a})$ đến $\mathbf{Z}$ được ký hiệu là dim. Gọi $c$ là lớp của một môđun $\mathfrak{a}$ tầm thường có chiều 1, và gọi $\psi$ là đồng cấu $n \rightarrow nc$ từ $\mathbf{Z}$ đến $\mathscr{R}(\mathfrak{a})$. Điều này ngay lập tức cho thấy rằng

dim$\circ \psi =$ Id$_{\mathbf{Z}}$,

do đó $\mathscr{R}(\mathfrak{a})$ là tổng trực tiếp của Ker dim và $\mathbf{Z}c$.

#### Bổ đề 4 {#lie-viii-s7-lem-4 .statement tag=0147}

Trên nhóm cộng $\mathscr{R}(\mathfrak{a})$ tồn tại một phép nhân duy nhất phân phối đối với phép cộng sao cho $[E][F] = [E\otimes F]$ với mọi môđun $\mathfrak{a}$ hữu hạn chiều E, F. Theo cách này $\mathscr{R}(\mathfrak{a})$ được trang bị cấu trúc của một vành giao hoán. Lớp của môđun $\mathfrak{a}$ tầm thường có chiều 1 là phần tử đơn vị của vành này.

Tính duy nhất là rõ ràng. Tồn tại một phép nhân giao hoán trên $\mathscr{R}(\mathfrak{a}) =\mathbf{Z}^{(\mathfrak{S}_{\mathfrak{a}})}$ phân phối đối với phép cộng và sao cho $[E][F] = [E\otimes F]$ với mọi $E,F\in \mathfrak{S}_{\mathfrak{a}}$. Cho $E_1,E_2$ là các môđun $\mathfrak{a}$ hữu hạn chiều, $l_1$ và $l_2$ là độ dài của chúng; ta chứng minh rằng $[E_1][E_2] = [E_1\otimes E_2]$ bằng quy nạp trên $l_1+l_2$. Điều này là rõ ràng nếu $l_1+l_2\leq 2$. Mặt khác, cho $F_1$ là một môđun con của $E_1$ phân biệt với 0 và $E_1$. Khi đó

$[F_1][E_2] = [F_1\otimes E_2]$ và $[E_1/F_1][E_2] = [(E_1/F_1)\otimes E_2]$ theo giả thiết quy nạp. Mặt khác, $(E_1\otimes E_2)/(F_1\otimes E_2)$ đẳng cấu với $(E_1/F_1)\otimes E_2$. Do đó

$$
[E_1][E_2] = ([E_1/F_1] + [F_1]).[E_2] = [(E_1/F_1)\otimes E_2] + [F_1\otimes E_2] = [E_1\otimes E_2]
$$

điều này chứng minh mệnh đề của ta. Suy ra ngay lập tức rằng phép nhân được xác định ở trên là kết hợp, do đó $\mathscr{R}(\mathfrak{a})$ có cấu trúc của một vành giao hoán. Cuối cùng, rõ ràng rằng lớp của môđun $\mathfrak{a}$ tầm thường có chiều 1 là phần tử đơn vị của vành này.

#### Bổ đề 5 {#lie-viii-s7-lem-5 .statement tag=0148}

Tồn tại một tự đẳng cấu đối hợp duy nhất $X \rightarrow X^*$ của vành $\mathscr{R}(\mathfrak{a})$ sao cho $[E]^*= [E^*]$ với mọi $\mathfrak{a}$-môđun hữu hạn chiều E.

Tính duy nhất là rõ ràng. Theo Bổ đề 3, tồn tại một đồng cấu $X \rightarrow X^*$ từ nhóm cộng $\mathscr{R}(\mathfrak{a})$ vào chính nó sao cho $[E]^*= [E^*]$ với mọi $\mathfrak{a}$-môđun hữu hạn chiều E. Ta có $(X^*)^*= X$, do đó đồng cấu này là đối hợp. Nó là một tự đẳng cấu của vành $\mathscr{R}(\mathfrak{a})$ vì $(E\otimes F)^*$ đẳng cấu với $E^*\otimes F^*$ với mọi $\mathfrak{a}$-môđun hữu hạn chiều E và F. Q.E.D.

Gọi $U(\mathfrak{a})$ là đại số bao quanh của $\mathfrak{a}, U(\mathfrak{a})^*$ là không gian vectơ đối ngẫu của $U(\mathfrak{a})$. Nhắc lại (Chap. II, §1, no. 5) rằng cấu trúc đại số đối đồng của $U(\mathfrak{a})$ xác định trên $U(\mathfrak{a})^*$ một cấu trúc đại số giao hoán, kết hợp với phần tử đơn vị. Với mọi $\mathfrak{a}$-môđun hữu hạn chiều E, ánh xạ $u \rightarrow$ Tr($u_E$) từ $U(\mathfrak{a})$ vào $k$ là một phần tử $\tau_E$ của $U(\mathfrak{a})^*$. Nếu $0\longrightarrow E'\longrightarrow E\longrightarrow E''\longrightarrow 0$ là một dãy khớp của các $\mathfrak{a}$-môđun hữu hạn chiều, thì $\tau_E=\tau_{E'}+\tau_{E''}$. Do đó, theo Bổ đề 3 tồn tại một đồng cấu duy nhất, ký hiệu là Tr, từ nhóm cộng $\mathscr{R}(\mathfrak{a})$ vào nhóm $U(\mathfrak{a})^*$ sao cho Tr[E] $=\tau_E$ với mọi $\mathfrak{a}$-môđun hữu hạn chiều E. Nếu $k$ ký hiệu cho $\mathfrak{a}$-môđun tầm thường có chiều 1, thì dễ kiểm tra rằng Tr[$k]$ là phần tử đơn vị của $U(\mathfrak{a})^*$. Cuối cùng, cho E và F là các $\mathfrak{a}$-môđun hữu hạn chiều. Cho $u\in U(\mathfrak{a})$ và cho $c$ là đồng tích của $U(\mathfrak{a})$. Theo định nghĩa của U-môđun $E\otimes F$ (Chap. I, §3, no. 2), nếu $c(u) =\sum_iu_i\otimes u'_i$,

$$
u_{E\otimes F}=\sum_i(u_i)_E\otimes (u'_i)_F
$$

Do đó

$\tau_{E\otimes F}(u) =\sum_i$ Tr($u_i$)$_E$Tr($u'_i$)$_F=\sum_i\tau_E(u_i)\tau_F(u'_i)$

$$
= (\tau_E\otimes \tau_F)(c(u))
$$

Điều này có nghĩa là $\tau_E\tau_F=\tau_{E\otimes F}$. Vì vậy, Tr$:\mathscr{R}(\mathfrak{a})\rightarrow U(\mathfrak{a})^*$ là một đồng cấu của các vành.

Cho $\mathfrak{a}_1$ và $\mathfrak{a}_2$ là các đại số Lie, $f$ là một đồng cấu từ $\mathfrak{a}_1$ đến $\mathfrak{a}_2$. Mọi $\mathfrak{a}_2$-môđun hữu hạn chiều E xác định bằng $f$ một $\mathfrak{a}_1$-môđun, do đó các phần tử của $\mathscr{R}(\mathfrak{a}_2)$ và $\mathscr{R}(\mathfrak{a}_1)$ mà ta tạm thời ký hiệu lần lượt là $[E]_2$ và $[E]_1$. Theo Bổ đề 3, tồn tại một đồng cấu duy nhất, ký hiệu bởi $\mathscr{R}(f)$, từ nhóm $\mathscr{R}(\mathfrak{a}_2)$ đến nhóm $\mathscr{R}(\mathfrak{a}_1)$ sao cho $\mathscr{R}(f)[E]_2=[E]_1$ với mọi $\mathfrak{a}_2$-môđun hữu hạn chiều E. Hơn nữa, $\mathscr{R}(f)$ là một đồng cấu vành. Nếu U(f) là đồng cấu từ U($\mathfrak{a}_1$) đến U($\mathfrak{a}_2$) mở rộng $f$, biểu đồ sau là giao hoán

$$
\begin{array}{ccc}
\mathscr{R}(\mathfrak{a}_2) & \xrightarrow{\mathscr{R}(f)} & \mathscr{R}(\mathfrak{a}_1)\\
\Big\downarrow\scriptstyle{\operatorname{Tr}} & & \Big\downarrow\scriptstyle{\operatorname{Tr}}\\
U(\mathfrak{a}_2)^* & \xrightarrow{t_{U(f)}} & U(\mathfrak{a}_1)^*.
\end{array}
$$

Trong phần tiếp theo, ta lấy $\mathfrak{a}$ là đại số Lie nửa đơn tách được $\mathfrak{g}$. Vành $\mathscr{R}(\mathfrak{g})$ được gọi là *vành biểu diễn* của $\mathfrak{g}$. Với mọi $\lambda\in P_{++}$, ta ký hiệu bởi $[\lambda]$ lớp của $\mathfrak{g}$-môđun đơn E($\lambda$) có trọng số cao nhất $\lambda$.

### 7. CÁC ĐẶC TRƯNG CỦA $\mathfrak{g}$-MÔĐUN

Cho $\Delta$ là một nửa nhóm giao hoán được viết cộng tính, và $\mathbf{Z}[\Delta]=\mathbf{Z}^{(\Delta)}$ là đại số của nửa nhóm $\Delta$ trên $\mathbf{Z}$ (Đại số, Chương III, §2, no. 6). Ký hiệu bởi $(e^\lambda)_{\lambda\in\Delta}$ cơ sở chính tắc của $\mathbf{Z}[\Delta]$. Với mọi $\lambda,\mu\in\Delta$, ta có $e^{\lambda+\mu}=e^\lambda e^\mu$. Nếu 0 là phần tử trung hòa của $\Delta$, thì $e^0$ là phần tử đơn vị của $\mathbf{Z}[\Delta]$; nó được ký hiệu là 1.

Cho E là một không gian vectơ phân bậc theo $\Delta$ trên một trường $\kappa$, và $(E^\lambda)_{\lambda\in\Delta}$ là sự phân bậc của nó. Nếu mỗi $E^\lambda$ là hữu hạn chiều, đặc trưng của E, ký hiệu bởi ch(E), là phần tử $(\dim E^\lambda)_{\lambda\in\Delta}$ của $\mathbf{Z}^{\Delta}$. Nếu bản thân E là hữu hạn chiều,

$$
\operatorname{ch}(E)=\sum_{\lambda\in\Delta}(\dim E^\lambda)e^\lambda\in\mathbf{Z}[\Delta].
\tag{5}
$$

Cho E′, E, E″ là các không gian vectơ phân bậc theo $\Delta$ sao cho các E′${}^\lambda$, E${}^\lambda$, E″${}^\lambda$ là hữu hạn chiều trên $\kappa$, và $0\longrightarrow E'\longrightarrow E\longrightarrow E''\longrightarrow0$ là một dãy khớp các đồng cấu phân bậc có bậc 0. Ngay lập tức ta có

$$
\operatorname{ch}(E)=\operatorname{ch}(E')+\operatorname{ch}(E'').
\tag{6}
$$

Đặc biệt, nếu F$_1$, F$_2$ là các không gian vectơ phân bậc $\Delta$ sao cho F$_1^\lambda$ và F$_2^\lambda$ là hữu hạn chiều trên $\kappa$, thì

$$
\operatorname{ch}(F_1\oplus F_2)=\operatorname{ch}(F_1)+\operatorname{ch}(F_2).
\tag{7}
$$

Nếu F$_1$ và F$_2$ là hữu hạn chiều, ta cũng có

$$
\operatorname{ch}(F_1\otimes F_2)=\operatorname{ch}(F_1)\mathbin{.}\operatorname{ch}(F_2).
\tag{8}
$$

#### Ví dụ {#lie-viii-s7-n7-exa-1 .statement tag=01JX}

Giả sử rằng $\Delta=\mathbf{N}$. Gọi T là một phần tử bất định. Tồn tại một đẳng cấu duy nhất từ đại số $\mathbf{Z}[\mathbf{N}]$ vào đại số $\mathbf{Z}[T]$ biến $e^n$ thành $T^n$ với mọi $n\in\mathbf{N}$. Đối với mọi không gian vectơ phân bậc $\mathbf{N}$ hữu hạn chiều E, ảnh của ch(E) trong $\mathbf{Z}[T]$ là đa thức Poincaré của E (Chap. V, §5, no. 1).

Cho E là một $\mathfrak{g}$-môđun sao cho $E =\sum_{\lambda\in\mathfrak{h}^*}E^{\lambda}$ và sao cho mỗi $E^{\lambda}$ là

hữu hạn chiều. Ta biết rằng $(E^{\lambda})_{\lambda\in\mathfrak{h}^*}$ là một sự phân bậc của không gian vectơ E. Trong phần tiếp theo, ta dành ký hiệu ch(E) cho đặc trưng của E được xét như một không gian vectơ $\mathfrak{h}^*$-phân bậc. Như vậy, đặc trưng ch(E) là một phần tử của $\mathbf{Z}^{\mathfrak{h}^*}$. Nếu E là hữu hạn chiều, ch(E) $\in \mathbf{Z}[P]$. Theo công thức (6) và Bổ đề 3 của no. 6, tồn tại một đồng cấu duy nhất từ nhóm $\mathscr{R}(\mathfrak{g})$ vào $\mathbf{Z}[P]$ biến E thành ch(E), với mọi $\mathfrak{g}$-môđun hữu hạn chiều E; đồng cấu này sẽ được ký hiệu là ch. Quan hệ (8) chỉ ra rằng ch là một đồng cấu từ vành $\mathscr{R}(\mathfrak{g})$ vào vành $\mathbf{Z}[P]$.

#### Nhận xét {#lie-viii-s7-n7-rem-1 .statement tag=0149}

Mọi phần tử của P xác định một $\mathfrak{h}$-môđun đơn có chiều 1, do đó một đồng cấu từ nhóm $\mathbf{Z}[P]$ vào nhóm $\mathscr{R}(\mathfrak{h})$, là một đồng cấu đơn ánh của các vành. Hiển nhiên rằng ánh xạ hợp

$$
\mathscr{R}(\mathfrak{g})\longrightarrow \mathbf{Z}[P]\longrightarrow \mathscr{R}(\mathfrak{h})
$$

là đồng cấu được xác định bởi đơn ánh chính tắc của $\mathfrak{h}$ vào $\mathfrak{g}$ (no. 6).

Nhóm Weyl W tác động bởi các tự đẳng cấu lên nhóm P, và do đó tác động lên $\mathbf{Z}^P$. Với mọi $\lambda \in P$ và mọi $w\in W$, ta có $we^{\lambda}=e^{w\lambda}$. Gọi $\mathbf{Z}[P]^W$ là vành con của $\mathbf{Z}[P]$ gồm các phần tử bất biến dưới W.

#### Bổ đề 6 {#lie-viii-s7-lem-6 .statement tag=014A}

Nếu $\lambda \in P_{++}$, thì ch[$\lambda ]\in \mathbf{Z}[P]^W$. Số hạng cực đại duy nhất của ch[$\lambda ]$ (Chap. VI, §3, no. 2, Def. 1) là $e^{\lambda}$.

Mệnh đề đầu tiên suy ra từ no. 1, Hệ quả 2 của Mệnh đề 2, và mệnh đề thứ hai suy ra từ §6, no. 1, Mệnh đề 1 (ii).

#### Định lý 2 {#lie-viii-s7-thm-2 .statement tag=014B}

(i) Cho $(\varpi_{\alpha})_{\alpha\in B}$ là họ các trọng số cơ bản đối với B. Cho $(T_{\alpha})_{\alpha\in B}$ là một họ các phần tử bất định. Ánh xạ $f \rightarrow f(([\varpi_{\alpha}])_{\alpha\in B})$ từ $\mathbf{Z}[(T_{\alpha})_{\alpha\in B}]$ vào $\mathscr{R}(\mathfrak{g})$ là một đẳng cấu của các vành.

(ii) Đồng cấu ch từ $\mathscr{R}(\mathfrak{g})$ vào $\mathbf{Z}[P]$ cảm sinh một đẳng cấu từ vành $\mathscr{R}(\mathfrak{g})$ vào vành $\mathbf{Z}[P]^W$.

(iii) Cho E là một $\mathfrak{g}$-môđun hữu hạn chiều. Nếu ch $E =\sum_{\lambda\in P_{++}}m_{\lambda}$ch[$\lambda ]$, thành phần đẳng kiểu của E có trọng số cao nhất $\lambda$ có độ dài $m_{\lambda}$.

Họ $([\lambda ])_{\lambda\in P_{++}}$ là một cơ sở của $\mathbf{Z}$-môđun $\mathscr{R}(\mathfrak{g})$, và họ (ch[$\lambda ]$)$_{\lambda\in P_{++}}$ là một cơ sở của $\mathbf{Z}$-môđun $\mathbf{Z}[P]^W$ (Bổ đề 6, và Chương VI, §3, no. 4, Mệnh đề 3). Điều này chứng minh (ii) và (iii). Mệnh đề (i) suy ra từ (ii), Bổ đề 6 và Chương VI, §3, no. 4, Định lý 1.

#### Hệ quả {#lie-viii-s7-n7-cor-1 .statement tag=014C}

Cho $E,E'$ là các $\mathfrak{g}$-môđun hữu hạn chiều. Khi đó E đẳng cấu với $E'$ khi và chỉ khi ch E = ch $E'$.

Điều này suy ra từ Định lý 2 (ii) và sự kiện rằng $E,E'$ là nửa đơn.

### Bài tập {#lie-viii-s7-exercises}

Tất cả các $\mathfrak{g}$-môđun được xét (ngoại trừ các môđun trong Bài tập 14 và 15) được giả sử là hữu hạn chiều.

Xem [các bài tập cho § 7](exercises/s7/).
