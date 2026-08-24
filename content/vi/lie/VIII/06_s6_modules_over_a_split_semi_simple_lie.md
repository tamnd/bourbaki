---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VIII
chapter_title: SPLIT SEMI-SIMPLE LIE ALGEBRAS
section: 6
section_title: Modules over a split semi-simple Lie algebra
lang: vi
source: lie-vii-ix
book_pages: 115-123, 238
pdf_pages: 0123-0131, 0246-0246
extraction: native
subsections:
    - "no": 1
      title: WEIGHTS AND PRIMITIVE ELEMENTS
      page: 116
      pdf_page: 124
    - "no": 2
      title: SIMPLE MODULES WITH A HIGHEST WEIGHT
      page: 118
      pdf_page: 126
    - "no": 3
      title: EXISTENCE AND UNIQUENESS THEOREM
      page: 119
      pdf_page: 127
    - "no": 4
      title: COMMUTANT OF $\mathfrak{h}$ IN THE ENVELOPING ALGEBRA $\mathbf{O}\mathbf{F}\mathfrak{g}$
      page: 122
      pdf_page: 130
statements: 17
exercises: 5
content_sha256: 7f8854480f88cf4f4300cbdf394191b0c8856ed510604cce956cba7ddb3824b4
translated_from: content/en/lie/VIII/06_s6_modules_over_a_split_semi_simple_lie.md
source_content_sha256: 487388bd8ad7aeeaec7bc35a084734841a8e2e5b22d8bc35a3035539d1b008d8
translation_model: gpt-5.4
translation_run: translate-vi-5540fd17
glossary_version: 34
glossary_terms_sha256: 5c0c201e5cebbfa1782e47a26467f63f1931bee6c889ae37baa3326eebbf52df
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 6. MÔĐUN TRÊN MỘT ĐẠI SỐ LIE NỬA ĐƠN TÁCH

Trong đoạn này, $(\mathfrak{g},\mathfrak{h})$ ký hiệu một đại số Lie nửa đơn tách, R hệ nghiệm của nó, W nhóm Weyl của nó, B một cơ sở của R, $R_+$ (tương ứng $R_-$) tập hợp các nghiệm dương (tương ứng các nghiệm âm) đối với B. Đặt

$\mathfrak{n}_+=\sum_{\alpha\in R_+}\mathfrak{g}^{\alpha},\mathfrak{n}_-=\sum_{\alpha\in R_-}\mathfrak{g}^{\alpha},\mathfrak{b}_+=\mathfrak{h}+\mathfrak{n}_+$ và $\mathfrak{b}_-=\mathfrak{h}+\mathfrak{n}_-$.

Ta có $\mathfrak{n}_+= [\mathfrak{b}_+,\mathfrak{b}_+],\mathfrak{n}_-= [\mathfrak{b}_-,\mathfrak{b}_-]$.

Với mọi $\alpha \in R$, chọn một phần tử $X_{\alpha}\in \mathfrak{g}^{\alpha}$ sao cho

$$
[X_{\alpha}, X_{-\alpha}] =-H_{\alpha}
$$

(§2, no. 4); không một định nghĩa nào dưới đây phụ thuộc vào lựa chọn này.

### 1. TRỌNG SỐ VÀ CÁC PHẦN TỬ NGUYÊN THỦY

Cho V là một $\mathfrak{g}$-môđun. Với mọi $\lambda \in \mathfrak{h}^*$, ký hiệu $V^{\lambda}$ là không gian con nguyên sơ, ứng với $\lambda$, của V khi xem V như một $\mathfrak{h}$-môđun (Chương VII, §1, no. 1). Các phần tử của $V^{\lambda}$ được gọi là các phần tử có trọng số $\lambda$ của $\mathfrak{g}$-môđun V. Tổng của các $V^{\lambda}$ là trực tiếp (Chương VII, §1, no. 1, Mệnh đề 3). Với mọi $\alpha \in \mathfrak{h}^*$ và $\lambda \in \mathfrak{h}^*,\mathfrak{g}^{\alpha}V^{\lambda}\subset V^{\alpha+\lambda}$ (Chương VII, §1, no. 3, Mệnh đề 10 (ii)). Chiều của $V^{\lambda}$ được gọi là bội số của $\lambda$ trong V; nếu nó $\geq 1$, tức là nếu $V^{\lambda}\not= 0,\lambda$ được gọi là một trọng số của V. Nếu V hữu hạn chiều, thì các đồng dạng của V xác định bởi các phần tử của $\mathfrak{h}$ là nửa đơn, nên $V^{\lambda}$ là tập hợp các $x\in V$ sao cho $Hx=\lambda (H)x$ với mọi $H\in \mathfrak{h}$.

#### Bổ đề 1 {#lie-viii-s6-lem-1 .statement tag=012M}

Cho V là một $\mathfrak{g}$-môđun và $v\in V$. Các điều kiện sau là tương đương:

(i) $\mathfrak{b}_+v\subset kv$;

(ii) $\mathfrak{h}v\subset kv$ và $\mathfrak{n}_+v= 0$;

(iii) $\mathfrak{h}v\subset kv$ và $\mathfrak{g}^{\alpha}v= 0$ với mọi $\alpha \in B$.

(i) $=\Rightarrow$ (ii): Giả sử rằng $\mathfrak{b}_+v\subset kv$. Tồn tại $\lambda \in \mathfrak{h}^*$ sao cho $v\in V^{\lambda}$. Cho $\alpha \in R_+$. Khi đó $\mathfrak{g}^{\alpha}.v\subset V^{\lambda}\cap V^{\lambda+\alpha}= 0$. Do đó $\mathfrak{n}_+v= 0$.

(ii) $=\Rightarrow$ (iii): Điều này hiển nhiên.

(iii) $=\Rightarrow$ (i): Điều này suy ra từ việc $(X_{\alpha})_{\alpha\in B}$ sinh ra $\mathfrak{n}_+($§3, no. 3, Mệnh đề 9 (iii)).

#### Định nghĩa 1 {#lie-viii-s6-def-1 .statement tag=012N}

Cho V là một $\mathfrak{g}$-môđun và $v\in V$. Khi đó $v$ được gọi là một phần tử nguyên thủy của V nếu $v\not= 0$ và $v$ thỏa mãn các điều kiện của Bổ đề 1.

Một phần tử nguyên thủy thuộc một trong các $V^{\lambda}$. Với mọi $\lambda \in \mathfrak{h}^*, V_{\pi}^{\lambda}$ ký hiệu tập hợp các $v\in V^{\lambda}$ sao cho $\mathfrak{b}_+v\subset kv$. Do đó, các phần tử nguyên thủy có trọng số $\lambda$ là các phần tử khác không của $V_{\pi}^{\lambda}$.

#### Mệnh đề 1 {#lie-viii-s6-prop-1 .statement tag=012O}

Cho V là một $\mathfrak{g}$-môđun, $v$ là một phần tử nguyên thủy của V và $\omega$ là trọng số của $v$. Giả sử rằng V được sinh bởi $v$ như một $\mathfrak{g}$-môđun.

(i) Nếu $U(\mathfrak{n}_-)$ ký hiệu đại số bao đóng của $\mathfrak{n}_-$, thì ta có $V = U(\mathfrak{n}_-).v$.

(ii) Với mọi $\lambda \in \mathfrak{h}^*,V^{\lambda}$ là tập hợp các $x\in V$ sao cho $Hx=\lambda (H)x$ với mọi $H\in \mathfrak{h}$. Ta có $V =\bigoplus_{\lambda\in\mathfrak{h}^*}V^{\lambda}$, và mỗi $V^{\lambda}$ đều hữu hạn chiều. Không gian

$V^{\omega}$ có chiều 1, và mọi trọng số của V đều có dạng $\omega -\sum_{\alpha\in B}n_{\alpha}.\alpha$, trong đó các $n_{\alpha}$ là những số nguyên $\geq 0$.

(iii) V là một $\mathfrak{g}$-môđun không phân tích được, và hoán tập của nó chỉ gồm các vô hướng.

(iv) Gọi $U(\mathfrak{g})$ là đại số bao của $\mathfrak{g}$, và $\mathscr{Z}$ là tâm của $U(\mathfrak{g})$. Tồn tại một đồng cấu duy nhất $\chi$ từ $\mathscr{Z}$ vào $k$ sao cho, với mọi $z\in \mathscr{Z}$, $z_V$ là phép vị tự có tỉ số $\chi (z)$.

Gọi $U(\mathfrak{b}_+)$ là đại số bao của $\mathfrak{b}_+$. Ta có $U(\mathfrak{g}) = U(\mathfrak{n}_-).U(\mathfrak{b}_+)$ (Chương I, §2, no. 7, Hệ quả 6 của Định lý 1). Do đó

$$
V = U(\mathfrak{g}).v= U(\mathfrak{n}_-).U(\mathfrak{b}_+).v= U(\mathfrak{n}_-).v
$$

Ký hiệu bởi $\alpha_1, . . . , \alpha_n$ các phần tử phân biệt của $R_+$. Khi đó

$$
(X_{-\alpha_1}^{p_1}X_{-\alpha_2}^{p_2}. . . X_{-\alpha_n}^{p_n})_{(p_1,...,p_n)\in\mathbf{N}^n}
$$

là một cơ sở của $U(\mathfrak{n}_-)$, nên

V = $\sum kX_{-\alpha_1}^{p_1}. . . X_{-\alpha_n}^{p_n}v$. (1)

$(p_1,...,p_n)\in \mathbf{N}^n$

Với $\lambda \in \mathfrak{h}^*$, đặt

$$
T_{\lambda}=\sum kX_{-\alpha_1}^{p_1}. . . X_{-\alpha_n}^{p_n}v
$$

$(p_1,...,p_n)\in \mathbf{N}^n, \omega -p_1\alpha_1-\cdot \cdot \cdot -p_n\alpha_n=\lambda$

Theo Chương VII, §1, no. 1, Mệnh đề 2 (ii), nếu $h\in \mathfrak{h},h_V|T_{\lambda}$ là phép vị tự với tỉ số $\lambda (h)$. Vậy $T_{\lambda}\subset V^{\lambda}$. Mặt khác, (1) kéo theo rằng

V = $\sum T_{\lambda}$.

$\lambda \in \omega -\mathbf{N}\alpha_1-\cdot \cdot \cdot -\mathbf{N}\alpha_n$

Tổng của các $V^{\lambda}$ là trực tiếp (Chương VII, §1, no. 1, Mệnh đề 3). Từ những nhận xét này suy ra rằng $V^{\lambda}= T_{\lambda}$, rằng V là tổng trực tiếp của các $V^{\lambda}$, và rằng $V^{\lambda}$ là tập hợp các $x\in V$ sao cho $hx=\lambda (h)x$ với mọi $h\in \mathfrak{h}$. Mặt khác, chiều của $V^{\lambda}$ nhiều nhất bằng lực lượng của tập hợp các $(p_1, . . . , p_n)\in \mathbf{N}^n$ sao cho $p_1\alpha_1+\cdots +p_n\alpha_n=\omega -\lambda$. Điều này chứng tỏ rằng $V^{\lambda}= 0$ nếu $\omega -\lambda  \notin \sum_{\alpha\in B}\mathbf{N}\alpha$,

rằng chiều của $V^{\omega}= 1$, và rằng các $V^{\lambda}$ đều hữu hạn chiều.

Cho $c$ là một phần tử của hoán tập của V. Với mọi $h\in \mathfrak{h}$,

$$
hc(v) =ch(v) =\omega (h)c(v)
$$

nên $c(v)\in V^{\omega}$; do đó tồn tại $t\in k$ sao cho $c(v) =tv$. Bây giờ, với mọi $(p_1, . . . , p_n)\in \mathbf{N}^n$,

$$
cX_{-\alpha_1}^{p_1}. . . X_{-\alpha_n}^{p_n}v=X_{-\alpha_1}^{p_1}. . . X_{-\alpha_n}^{p_n}cv=tX_{-\alpha_1}^{p_1}. . . X_{-\alpha_n}^{p_n}v
$$

nên $c=t.1$. Vậy hoán tập của V thu về các vô hướng. Điều này suy ra (iv) và rằng V là không phân tích được.

#### Định nghĩa 2 {#lie-viii-s6-def-2 .statement tag=012P}

Đồng cấu $\chi$ của Mệnh đề 1 (iv) được gọi là đặc trưng trung tâm của $\mathfrak{g}$-môđun V.

#### Mệnh đề 2 {#lie-viii-s6-prop-2 .statement tag=012Q}

Cho V là một $\mathfrak{g}$-môđun sinh bởi một phần tử nguyên thủy $e$ có trọng số $\omega$, và X là một $\mathfrak{g}$-môđun nửa đơn. Gọi $\Phi$ là tập hợp các đồng cấu từ $\mathfrak{g}$-môđun V đến $\mathfrak{g}$-môđun X. Khi đó $\varphi  \rightarrow \varphi (e)$ là một đẳng cấu từ không gian vectơ $\Phi$ lên không gian vectơ $X^{\omega}_{\pi}$.

Hiển nhiên là $\varphi (e)\in X^{\omega}_{\pi}$ với mọi $\varphi \in \Phi$. Nếu $\varphi \in \Phi$ và $\varphi (e) = 0$, thì $\varphi = 0$ vì $e$ sinh $\mathfrak{g}$-môđun V. Ta chứng minh rằng, nếu $f$ là một phần tử khác không của $X^{\omega}_{\pi}$, thì tồn tại $\varphi \in \Phi$ sao cho $\varphi (e) =f$. Gọi $X'$ là môđun con của X sinh bởi $f$. Theo Mệnh đề $1, X'$ là không phân tích được, do đó là đơn vì X là nửa đơn. Phần tử $(e, f)$ là nguyên thủy trong $\mathfrak{g}$-môđun $V\times X$. Gọi N là môđun con của $V\times X$ sinh bởi $(e, f)$. Khi đó $N\cap X\subset$ pr$_2(N) = X'$, nên $N\cap X = 0$ hoặc $X'$; nếu $N\cap X = X', N$ chứa các phần tử độc lập tuyến tính $(e, f)$ và $(0, f)$ là nguyên thủy có trọng số $\omega$; điều này vô lý (Mệnh đề 1), nên $N\cap X = 0$. Do đó pr$_1|N$ là một ánh xạ đơn ánh $h$ từ N vào V; ánh xạ này là toàn ánh vì ảnh của nó chứa $e$. Vậy $\varphi =$ pr$_2\circ h^{-1}$ là một đồng cấu từ $\mathfrak{g}$-môđun V vào $\mathfrak{g}$-môđun X sao cho $\varphi (e) =f$.

### 2. MÔĐUN ĐƠN VỚI MỘT TRỌNG SỐ CAO NHẤT

Nhắc lại rằng việc cố định B xác định một quan hệ thứ tự trên $\mathfrak{h}^*_{\mathbf{Q}}$ (Chương VI, §1, no. 6). Các phần tử của $\mathfrak{h}^*_{\mathbf{Q}}$ mà $\geq 0$ là các tổ hợp tuyến tính của các phần tử của B với các hệ số hữu tỉ $\geq 0$.

Tổng quát hơn, ta sẽ xét quan hệ thứ tự sau giữa các phần tử $\lambda , \mu\in \mathfrak{h}^*:$

$\lambda -\mu$ là một tổ hợp tuyến tính của các phần tử của B với các hệ số hữu tỉ $\geq 0$.

#### Bổ đề 2 {#lie-viii-s6-lem-2 .statement tag=012R}

Cho V là một $\mathfrak{g}$-môđun đơn, $\omega$ một trọng số của V. Các điều kiện sau là tương đương:

(i) mọi trọng số của V đều có dạng $\omega -\mu$ trong đó $\mu$ là một trọng số căn $\geq 0$;

(ii) $\omega$ là trọng số cao nhất của V;

(iii) với mọi $\alpha \in B,\omega +\alpha$ không là một trọng số của V;

(iv) tồn tại một phần tử nguyên thủy có trọng số $\omega$.

(i) $=\Rightarrow$ (ii) $=\Rightarrow$ (iii): Điều này là hiển nhiên.

(iii) $=\Rightarrow$ (iv): Giả sử rằng điều kiện (iii) được thỏa mãn. Với mọi $h\in \mathfrak{h}$,

Ker($h_V-\omega (h)$)

là khác không, được chứa trong $V^{\omega}$, và ổn định dưới tác dụng của $\mathfrak{h}_V$. Bằng quy nạp theo dim $\mathfrak{h}$, ta thấy rằng tồn tại một $v$ khác không trong $V^{\omega}$ sao cho $\mathfrak{h}v\subset kv$. Điều kiện (iii) suy ra $\mathfrak{n}_+v= 0$, nên $v$ là nguyên thủy.

(iv) $=\Rightarrow$ (i): Cho $v$ là một phần tử nguyên thủy có trọng số $\omega$. Vì V là đơn, V được sinh bởi $v$ như một $\mathfrak{g}$-môđun. Mệnh đề (i) khi đó suy ra từ Mệnh đề 1.

Điều phải chứng minh.

Vì thế, đối với mọi $\mathfrak{g}$-môđun đơn, sự tồn tại của một phần tử nguyên thủy là tương đương với sự tồn tại của một trọng số cao nhất, hoặc với sự tồn tại của một trọng số cực đại. Có những $\mathfrak{s}\mathfrak{l}(2,\mathbf{C}$)-môđun đơn V không có trọng số nào đối với bất kỳ đại số con Cartan $\mathfrak{h}$ nào của $\mathfrak{s}\mathfrak{l}(2,\mathbf{C}) ($§1, Bài tập $14f))$. Các môđun này có chiều vô hạn trên $\mathbf{C}($§1, no. 3, Định lý 1).

#### Mệnh đề 3 {#lie-viii-s6-prop-3 .statement tag=012S}

Cho V là một $\mathfrak{g}$-môđun đơn có trọng số cao nhất $\omega$.

(i) Các phần tử nguyên thủy của V là các phần tử khác không của $V^{\omega}$.

(ii) V là nửa đơn như một $\mathfrak{h}$-môđun.

(iii) Ta có $V =\bigoplus_{\lambda\in\mathfrak{h}^*}V^{\lambda}$. Với mọi $\lambda \in \mathfrak{h}^*,V^{\lambda}$ là hữu hạn chiều. Ta

có dim $V^{\omega}= 1$.

(iv) $\mathfrak{g}$-môđun V là đơn tuyệt đối.

Các mệnh đề (i), (ii) và (iii) suy ra từ Mệnh đề 1 và Bổ đề 2. Mệnh đề (iv) suy ra từ Mệnh đề 1 (iii) và Đại số, Chương VIII, §7, no. 3.

#### Hệ quả {#lie-viii-s6-n2-cor-1 .statement tag=012T}

Nếu V là hữu hạn chiều, đồng cấu chính tắc $U(\mathfrak{g})\rightarrow$ End(V) là toàn ánh.

Điều này suy ra từ (iv), xem Đại số, Chương VIII, §3, no. 3.

#### Mệnh đề 4 {#lie-viii-s6-prop-4 .statement tag=012U}

Cho V là một $\mathfrak{g}$-môđun đơn có trọng số cao nhất $\omega$, X là một $\mathfrak{g}$-môđun nửa đơn, và $X'$ là thành phần đẳng kiểu kiểu V trong X. Khi đó $X'$ là môđun con của X sinh bởi $X^{\omega}_{\pi}$. Độ dài của nó bằng chiều của $X^{\omega}_{\pi}$.

Gọi $X''$ là môđun con của X sinh bởi $X^{\omega}_{\pi}$. Rõ ràng mọi môđun con của X đẳng cấu với V đều được chứa trong $X''$. Do đó $X'\subset X''$. Mặt khác, gọi $\Phi$ là tập hợp các đồng cấu từ $\mathfrak{g}$-môđun V tới $\mathfrak{g}$-môđun X. Độ dài của $X'$ là dim$_k\Phi ($Đại số, Chương VIII, §4, no. 4), tức là dim$_kX^{\omega}_{\pi}$ (Mệnh đề 2).

### 3. ĐỊNH LÝ TỒN TẠI VÀ DUY NHẤT

Cho $\lambda \in \mathfrak{h}^*$. Vì $\mathfrak{b}_+=\mathfrak{h}\oplus \mathfrak{n}_+$ và vì $\mathfrak{n}_+= [\mathfrak{b}_+,\mathfrak{b}_+]$, ánh xạ $h+n \rightarrow \lambda (h)$ (trong đó $h\in \mathfrak{h},n\in \mathfrak{n}_+$) từ $\mathfrak{b}_+$ vào $k$ là một biểu diễn 1 chiều của $\mathfrak{b}_+$. Ký hiệu bởi $L_{\lambda}$ không gian vectơ trên $k$ là $k$ được trang bị cấu trúc môđun trên $\mathfrak{b}_+$ xác định bởi biểu diễn này. Gọi $U(\mathfrak{g}), U(\mathfrak{b}_+)$ là các đại số bao của $\mathfrak{g},\mathfrak{b}_+$, sao cho $U(\mathfrak{b}_+)$ là một đại số con của $U(\mathfrak{g})$; nhắc lại rằng $U(\mathfrak{g})$ là một $U(\mathfrak{b}_+$)-môđun phải tự do (Chap. I, §2, no. 7, Hệ quả 5 của Định lý 1). Đặt

$$
Z(\lambda ) = U(\mathfrak{g})\otimes_{U(\mathfrak{b}_+)}L_{\lambda} \tag{2}
$$

Khi đó $Z(\lambda )$ là một $\mathfrak{g}$-môđun trái. Ký hiệu bởi $e$ phần tử $1\otimes 1$ của $Z(\lambda )$.

#### Mệnh đề 5 {#lie-viii-s6-prop-5 .statement tag=012V}

(i) Phần tử $e$ của $Z(\lambda )$ là nguyên thủy, có trọng số $\lambda$ và sinh ra $\mathfrak{g}$-môđun $Z(\lambda )$.

(ii) Đặt $Z^+(\lambda ) =\sum_{\lambda\not=\mu}Z(\lambda )^\mu$. Mọi môđun con của $Z(\lambda )$ phân biệt với $Z(\lambda )$

đều được chứa trong $Z^+(\lambda )$.

(iii) Tồn tại một môđun con lớn nhất $F_{\lambda}$ của $Z(\lambda )$ phân biệt với $Z(\lambda )$. Môđun thương $Z(\lambda )/F_{\lambda}$ là đơn và có trọng số cao nhất $\lambda$.

Rõ ràng là $e$ sinh ra $\mathfrak{g}$-môđun $Z(\lambda )$. Nếu $x\in \mathfrak{b}_+$,

$$
x.e= (x.1)\otimes 1 = (1.x)\otimes 1 = 1\otimes x.1 =\lambda (x)(1\otimes 1) =\lambda (x)e
$$

do đó suy ra (i).

$\mathfrak{h}$-môđun $Z(\lambda )$ là nửa đơn (Mệnh đề 1). Nếu G là một $\mathfrak{g}$-môđun con của $Z(\lambda )$, thì $G =\sum_{\mu\in\mathfrak{h}^*}(G\cap Z(\lambda )^\mu)$. Giả thiết $G\cap Z(\lambda )^{\lambda}\not= 0$ kéo theo

rằng $G = Z(\lambda )$, vì dim $Z(\lambda )^{\lambda}= 1$ và $e$ sinh ra $\mathfrak{g}$-môđun $Z(\lambda )$. Nếu $G\not= Z(\lambda )$, thì $G =\sum_{\mu\not=\lambda}G\cap Z(\lambda )^\mu\subset Z^+(\lambda )$.

Gọi $F_{\lambda}$ là tổng của các môđun con $\mathfrak{g}$ của $Z(\lambda )$ phân biệt với $Z(\lambda )$. Theo (ii), $F_{\lambda}\subset Z^+(\lambda )$. Do đó $F_{\lambda}$ là môđun con lớn nhất của $Z(\lambda )$ phân biệt với $Z(\lambda )$. Rõ ràng $Z(\lambda )/F_{\lambda}$ là đơn và ảnh chính tắc của $e$ trong $Z(\lambda )/F_{\lambda}$ là nguyên thủy có trọng số $\lambda$.

Trong phần còn lại của chương này, $\mathfrak{g}$-môđun $Z(\lambda )/F_{\lambda}$ của Mệnh đề 5 sẽ được ký hiệu là $E(\lambda )$.

#### Định lý 1 {#lie-viii-s6-thm-1 .statement tag=012W}

Cho $\lambda \in \mathfrak{h}^*$. $\mathfrak{g}$-môđun $E(\lambda )$ là đơn và có trọng số cao nhất $\lambda$. Mọi $\mathfrak{g}$-môđun đơn có trọng số cao nhất $\lambda$ đều đẳng cấu với $E(\lambda )$.

Mệnh đề thứ nhất suy ra từ Mệnh đề 5 (iii). Mệnh đề thứ hai suy ra từ Mệnh đề 4.

#### Mệnh đề 6 {#lie-viii-s6-prop-6 .statement tag=012X}

Cho V là một $\mathfrak{g}$-môđun, $\lambda$ là một phần tử của $\mathfrak{h}^*$ và $v$ là một phần tử nguyên thủy của V có trọng số $\lambda$.

(i) Tồn tại một đồng cấu duy nhất của các $\mathfrak{g}$-môđun $\psi : Z(\lambda )\rightarrow V$ sao cho $\psi (e) =v$.

(ii) Giả sử rằng $v$ sinh V. Khi đó $\psi$ là toàn ánh. Hơn nữa, $\psi$ là song ánh khi và chỉ khi, với mọi phần tử khác không $u$ của $U(\mathfrak{n}_-),u_V$ là đơn ánh.

(iii) Ánh xạ $u \rightarrow u\otimes 1$ từ $U(\mathfrak{n}_-)$ vào $Z(\lambda )$ là song ánh.

Cho K là hạt nhân của biểu diễn của $U(\mathfrak{b}_+)$ trên $L_{\lambda}$; nó có đối chiều 1 trong $U(\mathfrak{b}_+)$. Đặt $J = U(\mathfrak{g})K$ là iđêan trái của $U(\mathfrak{g})$ sinh bởi K; khi đó $L_{\lambda}$ có thể được đồng nhất với $U(\mathfrak{b}_+)/K$ như một $U(\mathfrak{b}_+$)-môđun trái, và $Z(\lambda )$ có thể được đồng nhất với $U(\mathfrak{g})/J$ như một $U(\mathfrak{g}$)-môđun trái. Ta có $K.v= 0$, nên $J.v= 0$, điều này chứng minh (i).

Bây giờ giả sử rằng $v$ sinh ra V. Rõ ràng là $\psi$ toàn ánh.

Theo định lý Poincaré-Birkhoff-Witt (Chương I, §2, no. 7, Hệ quả 6 của Định lý 1), một cơ sở của $U(\mathfrak{n}_-)$ trên $k$ cũng là một cơ sở của $U(\mathfrak{g})$ như một môđun phải trên $U(\mathfrak{b}_+)$. Do đó ánh xạ $\varphi :u \rightarrow u\otimes 1$ từ $U(\mathfrak{n}_-)$ đến $U(\mathfrak{g})\otimes_{U(\mathfrak{b}_+)}L_{\lambda}$ là song ánh. Cho $u\in U(\mathfrak{n}_-)$. Khi đó $\varphi^{-1}\circ u_{Z(\lambda)}\circ \varphi$ là phép nhân trái bởi $u$ trên $U(\mathfrak{n}_-)$. Theo Chương I, §2, no. 7, Hệ quả 7 của Định lý $1,u_{Z(\lambda)}$ là đơn ánh nếu $u\not= 0$. Do đó, nếu $\psi$ là song ánh, thì $u_V$ là đơn ánh đối với $u$ khác không trong $U(\mathfrak{n}_-)$.

Giả sử rằng $\psi$ không đơn ánh. Tồn tại $u\in U(\mathfrak{n}_-)$ sao cho $u\not= 0$ và $\psi (\varphi (u)) = 0$. Khi đó

$$
u_V.v=u_V.\psi (1\otimes 1) =\psi (u\otimes 1) =\psi (\varphi (u)) = 0
$$

#### Hệ quả 1 {#lie-viii-s6-prop-6-cor-1 .statement tag=012Y}

Cho $\lambda \in \mathfrak{h}^*$ và $\alpha \in B$ sao cho $\lambda (H_{\alpha}) + 1\in \mathbf{N}$. Khi đó $Z(-\alpha +s_{\alpha}\lambda )$ đẳng cấu với một $\mathfrak{g}$-môđun con của $Z(\lambda )$.

Đặt $m=\lambda (H_{\alpha})$. Cho $x= X^{m+1}_{-\alpha}.e\in Z(\lambda )$, và gọi V là môđun con của $Z(\lambda )$ sinh bởi $x$. Khi đó $x\not= 0$ (Mệnh đề 6). Mặt khác, $x\in Z(\lambda )^{\lambda-(m+1)\alpha}$. Với $\beta \in B$ và $\beta \not=\alpha , [\mathfrak{g}^{-\alpha},\mathfrak{g}^{\beta}] = 0$ và $\mathfrak{g}^{\beta}.e= 0$, nên $\mathfrak{g}^{\beta}.x= 0$. Sau cùng, vì $[X_{\alpha},X_{-\alpha}] =-H_{\alpha}$, ta có

$$
[X_{\alpha}, X_{-\alpha}^{m+1}] = (m+ 1)X_{-\alpha}^m(-H_{\alpha}+m)
$$

(§1, no. 1, Bổ đề 1 (ii)), nên

$$
X_{\alpha}.x=X_{\alpha}X_{-\alpha}^{m+1}.e= [X_{\alpha}, X_{-\alpha}^{m+1}].e= (m+ 1)X_{-\alpha}^m(me-\lambda (H_{\alpha})e) = 0
$$

Vậy $x$ là nguyên thủy có trọng số $\lambda -(m+ 1)\alpha$. Theo Mệnh đề 6, $\mathfrak{g}$-môđun V đẳng cấu với $Z(-\alpha +\lambda -m\alpha ) = Z(-\alpha +s_{\alpha}\lambda )$.

#### Hệ quả 2 {#lie-viii-s6-prop-6-cor-2 .statement tag=012Z}

Cho $\rho =\frac{1}{2}\sum_{\alpha\in R_+}\alpha$, và $\lambda , \mu\in \mathfrak{h}^*$. Giả sử rằng $\lambda +\rho$ là một trọng số trội trong R, và rằng tồn tại $w\in W$ sao cho $\mu+\rho =w(\lambda +\rho )$. Khi đó $Z(\mu)$ đẳng cấu với một môđun con của $Z(\lambda )$.

Mệnh đề là hiển nhiên khi $w= 1$. Giả sử rằng nó đã được thiết lập mỗi khi $w$ có độ dài $< q$. Nếu $w$ có độ dài $q$, tồn tại $\alpha \in B$ sao cho $w=s_{\alpha}w^{'-1}$, với $l(w') =q-1$. Ta có $w'(\alpha )\in R_+$ (Chương VI, §1, no. 6, Hệ quả 2 của Mệnh đề 17), và do đó $w^{'-1}(\lambda +\rho )(H_{\alpha}) = (\lambda +\rho )(H_{w'\alpha})$ là một số nguyên $\geq 0$. Đặt

$$
\mu'=w^{'-1}(\lambda +\rho )-\rho
$$

Theo giả thiết quy nạp, $Z(\mu')$ đẳng cấu với một môđun con của $Z(\lambda )$. Mặt khác, theo Chương VI, §1, no. 10, Mệnh đề 29 (ii),

$$
-\alpha +s_{\alpha}\mu'=-\alpha +s_{\alpha}w^{'-1}(\lambda +\rho )-s_{\alpha}\rho =w(\lambda +\rho )-\rho =\mu
$$

Hơn nữa, $\rho (H_{\alpha}) = 1$ (Chương VI, §1, Mệnh đề 29 (iii)), nên $\mu'(H_{\alpha})+1\in \mathbf{N}$. Hệ quả 1 khi đó kéo theo rằng $Z(\mu)$ đẳng cấu với một môđun con của $Z(\mu')$, và do đó cũng với một môđun con của $Z(\lambda )$.

### 4. HOÁN TẬP CỦA $\mathfrak{h}$ TRONG ĐẠI SỐ BAO $\mathbf{O}\mathbf{F}\mathfrak{g}$

Cho U là đại số bao của $\mathfrak{g}, V\subset U$ đại số bao của $\mathfrak{h}$. Đại số V có thể được đồng nhất với đại số đối xứng $\mathbf{S}(\mathfrak{h})$ của $\mathfrak{h}$, và cũng với đại số các hàm đa thức trên $\mathfrak{h}^*$. Ký hiệu bởi $\alpha_1, . . . , \alpha_n$ các căn dương phân biệt từng đôi một. Cho $(H_1, . . . , H_l)$ là một cơ sở của $\mathfrak{h}$. Theo định lý Poincaré-Birkhoff-Witt, các phần tử

$$
u((q_i),(m_i),(p_i)) =X_{-\alpha_1}^{q_1}. . . X_{-\alpha_n}^{q_n}H_1^{m_1}. . . H_l^{m_l}X_{\alpha_1}^{p_1}. . . X_{\alpha_n}^{p_n}
$$

$(q_i, m_i, p_i$ là các số nguyên $\geq 0)$ tạo thành một cơ sở của không gian vectơ U. Với mọi $h\in \mathfrak{h}$, ta có

$$
[h, u((q_i),(m_i),(p_i))] = ((p_1-q_1)\alpha_1+\cdots +(p_n-q_n)\alpha_n)(h)u((q_i),(m_i),(p_i)).(3)
$$

Không gian vectơ U là một $\mathfrak{g}$-môđun (do đó cũng là một $\mathfrak{h}$-môđun) dưới biểu diễn kề. Nếu $\lambda \in \mathfrak{h}^*$, các không gian con $U^{\lambda}$ và $U_{\lambda}$ được xác định (Chương VII, §1, no. 3); công thức (3) cho thấy rằng $U^{\lambda}= U_{\lambda}$ và rằng $U =\bigoplus_{\lambda\in Q}U^{\lambda}$

(trong đó Q là nhóm các trọng căn của R). Đặc biệt, $U^0$ là hoán tập của $\mathfrak{h}$, hay của V, trong U.

#### Bổ đề 3 {#lie-viii-s6-lem-3 .statement tag=0130}

Đặt $L = (\mathfrak{n}_-U)\cap U^0$.

(i) Ta có $L = (U\mathfrak{n}_+)\cap U^0$, và L là một iđêan hai phía của $U^0$.

(ii) Ta có $U^0= V\oplus L$.

Hiển nhiên $\mathfrak{n}_-U$ (tương ứng, $U\mathfrak{n}_+$) là tập hợp các tổ hợp tuyến tính của các phần tử $u((q_i),(m_i),(p_i))$ sao cho $\sum q_i>0$ (tương ứng, $\sum p_i>0$). Mặt khác

$$
u((q_i),(m_i),(p_i))\in U^0\Leftarrow \Rightarrow p_1\alpha_1+\cdots +p_n\alpha_n=q_1\alpha_1+\cdots +q_n\alpha_n
$$

Điều này kéo theo $(\mathfrak{n}_-U)\cap U^0= (U\mathfrak{n}_+)\cap U^0$. Sau cùng, $(\mathfrak{n}_-U)\cap U^0$ (resp. $(U\mathfrak{n}_+)\cap U^0$) là một iđêan phải (resp. trái) của $U^0$, do đó suy ra (i). Hơn nữa, một phần tử $u((q_i),(m_i),(p_i))$ thuộc $U^0$ thuộc về V (resp. thuộc về L) khi và chỉ khi $p_1=\cdots =p_n=q_1=\cdots =q_n= 0$ (resp. $p_1+\cdots +p_n+q_1+\cdots +q_n>0$), do đó suy ra (ii). Q.E.D.

Theo Bổ đề 3, phép chiếu của $U^0$ lên V với hạt nhân là L là một đồng cấu đại số. Nó được gọi là đồng cấu Harish-Chandra từ $U^0$ vào V (đối với B). Nhắc lại rằng V có thể được đồng nhất với đại số các hàm đa thức trên $\mathfrak{h}^*$.

#### Mệnh đề 7 {#lie-viii-s6-prop-7 .statement tag=0131}

Cho $\lambda \in \mathfrak{h}^*$, E là một $\mathfrak{g}$-môđun được sinh bởi một phần tử nguyên thủy có trọng số $\lambda ,\chi$ là đặc trưng trung tâm của E, và $\varphi$ là đồng cấu Harish-Chandra từ $U^0$ vào V. Khi đó, $\chi (z) = (\varphi (z))(\lambda )$ với mọi $z$ trong tâm của U.

Cho $v$ là một phần tử nguyên thủy của E có trọng số $\lambda$, và $z$ là một phần tử của tâm của U. Tồn tại $u_1, . . . , u_p\in U$ và $n_1, . . . , n_p\in \mathfrak{n}_+$ sao cho $z=\varphi (z) +u_1n_1+\cdots +u_pn_p$. Khi đó

$$
\chi (z)v=zv=\varphi (z)v+u_1n_1v+\cdots +u_pn_pv=\varphi (z)v= (\varphi (z))(\lambda )v
$$

#### Hệ quả {#lie-viii-s6-n4-cor-1 .statement tag=0132}

Cho $\langle  \cdot ,\cdot  \rangle$ là một dạng song tuyến tính đối xứng bất biến không suy biến trên $\mathfrak{g}$, và C là phần tử Casimir liên kết với $\langle  \cdot ,\cdot  \rangle$. Cũng ký hiệu bởi $\langle  \cdot ,\cdot  \rangle$ dạng nghịch đảo trên $\mathfrak{h}^*$ của hạn chế của $\langle  \cdot ,\cdot  \rangle$ lên $\mathfrak{h}($§2, no. 3, Mệnh đề 5). Khi đó $\chi (C) =\langle \lambda , \lambda + 2\rho \rangle$, trong đó $\rho =\frac{1}{2}\sum_{\alpha\in R_+}\alpha$.

Ta nhắc lại các ký hiệu của §2, no. 3, Mệnh đề 6. Ta có

1 1

C = $\sum X_{\alpha}X_{-\alpha}+\sum X_{-\alpha}X_{\alpha}$

$$
_{\alpha\in R_-}\overline{\langle X_{\alpha}, X_{-\alpha}\rangle}\alpha^{\in}_{R_+}\overline{\langle X_{\alpha}, X_{-\alpha}\rangle}
$$

1 $'$

$$
+\sum[X_{\alpha}, X_{-\alpha}] +\sum H_iH
$$

$$
_{\alpha\in R_+}\overline{\langle X_{\alpha}, X_{-\alpha}\rangle}i_{\in I}^i
$$

do đó

$$
\varphi (C) =\sum_{\alpha\in R_+}\frac{1}{\langle X_{\alpha}, X_{-\alpha}\rangle}[X_{\alpha}, X_{-\alpha}] +\sum_{i\in I}H_iH'_i
$$

Theo Mệnh đề 7,

1 $'$

$$
\chi (C) =\sum\lambda ([X_{\alpha}, X_{-\alpha}]) +\sum\lambda (H_i)\lambda (H)
$$

$$
_{\alpha\in R_+}\overline{\langle X_{\alpha}, X_{-\alpha}\rangle}i_{\in I}i
$$

Gọi $h_{\lambda}$ là phần tử của $\mathfrak{h}$ sao cho $\langle h_{\lambda}, h\rangle =\lambda (h)$ với mọi $h\in \mathfrak{h}$. Theo §2, no. 2, Mệnh đề 1,

$($ 1 $)\langle$ 1 $\rangle$

$\lambda [X_{\alpha}, X_{-\alpha}]$ = $h_{\lambda},[X_{\alpha}, X_{-\alpha}]=\alpha (h_{\lambda}) =\langle \lambda , \alpha \rangle$.

$$
\overline{\langle X_{\alpha}, X_{-\alpha}\rangle}\overline{\langle X_{\alpha}, X_{-\alpha}\rangle}
$$

Do đó

$$
\chi (C) =((\sum_{\alpha\in R_+}\langle \lambda , \alpha \rangle )+\langle \lambda , \lambda \rangle =\langle \lambda , \lambda + 2\rho \rangle
$$

### Bài tập {#lie-viii-s6-exercises}

Xem [các bài tập cho § 6](exercises/s6/).
