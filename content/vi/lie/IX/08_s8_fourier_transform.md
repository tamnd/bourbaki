---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IX
chapter_title: COMPACT REAL LIE GROUPS
section: 8
section_title: Fourier transform
lang: vi
source: lie-vii-ix
book_pages: 359-369, 417-418
pdf_pages: 0366-0376, 0424-0425
extraction: native
subsections:
    - "no": 1
      title: FOURIER TRANSFORMS OF INTEGRABLE FUNCTIONS
      page: 360
      pdf_page: 367
    - "no": 2
      title: FOURIER TRANSFORMS OF INFINITELY-DIFFERENTIABLE FUNCTIONS
      page: 362
      pdf_page: 369
    - "no": 3
      title: FOURIER TRANSFORMS OF CENTRAL FUNCTIONS
      page: 366
      pdf_page: 373
    - "no": 4
      title: CENTRAL FUNCTIONS ON G AND FUNCTIONS ON T
      page: 368
      pdf_page: 375
statements: 9
exercises: 6
content_sha256: 0e5ede1a2f9e3fa34eac4c19ec9fe6f8444157d7832c554639657a8d0ed1abc6
translated_from: content/en/lie/IX/08_s8_fourier_transform.md
source_content_sha256: 7146b47c4591798a6237702fc9df4724c46d7ba060e5bca3cd680259b2af702e
translation_model: gpt-5-mini, gpt-5-6-mini, gpt-5-6
translation_run: translate-vi-33b0919e
glossary_version: 34
glossary_terms_sha256: 26ab8e3ec0754df4390b5a0c8c063fa1c4c78028700404467b845d40bfef57e8
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 8. BIẾN ĐỔI FOURIER

Ta giữ lại các ký hiệu và quy ước của đoạn trước.

$^5$ Chứng minh của loc. cit., vốn chỉ được phát biểu cho các đại số Lie nửa đơn tách,

vẫn đúng không thay đổi trong trường hợp các đại số Lie khả quy tách.

### 1. CÁC BIẾN ĐỔI FOURIER CỦA CÁC HÀM KHẢ TÍCH

Trong số này, ta nhắc lại một số định nghĩa và kết quả từ Các lý thuyết phổ$^6$.

Ký hiệu $\widehat{G}$ là tập hợp các lớp của các biểu diễn bất khả quy của G (trên các không gian vectơ phức hữu hạn chiều). Với mọi $u\in \widehat{G}$, ký hiệu $Eu$ là không gian của $u$ và $d(u)$ là chiều của nó. Tồn tại các dạng Hermit dương tách được trên $E_u$ bất biến dưới $u$, và hai dạng như vậy bất kỳ đều tỉ lệ. Ký hiệu $A^*$ (tương ứng $\|A\|_{\infty}$) là ánh xạ liên hợp (tương ứng chuẩn) của một phần tử A của End(E$_u$) đối với một trong các dạng này; với mọi $g\in G$, ta có $u(g)^*=u(g)^{-1}=u(g^{-1})$ và $\|u(g)\|_{\infty}= 1$; với mọi $x\in \mathfrak{g}$, ta có $u(x)^*=-u(x) =u(-x)$.

Trang bị cho End(E$_u$) cấu trúc không gian Hilbert sao cho tích vô hướng là

$\langle A|B\rangle =d(u$)Tr(A$^*B$) $=d(u$)Tr(BA$^*$), (1)

và đặt

$\|A\|_2=\langle A|A\rangle^{1/2}= (d(u$)Tr(A$^*A$))$^{1/2}$. (2)

Ta có

$$
\surd\overline{d(u)}\|A\|_{\infty}\leq  \|A\|_2\leq d(u)\|A\|_{\infty} \tag{3}
$$

do đó

$$
|\langle A|B\rangle | \leq d(u)^2\|A\|_{\infty}\|B\|_{\infty} \tag{4}
$$

Với mọi $g\in G$, ta có $\|u(g)\|_2=d(u)$.

Ký hiệu $F( \widehat{G})$ là đại số $\prod_{u\in\widehat{G}}$ End(E$_u$). Ký hiệu $L^2( \widehat{G})$ là tổng Hilbert của các không gian Hilbert End(E$_u$); đây là không gian của các họ $A= (A_u)\in F( \widehat{G})$ sao cho $\sum_u\|A_u\|^2_2<\infty$, với tích vô hướng

$\langle A|B\rangle =\sum_{u\in\widehat{G}}\langle A_u|B_u\rangle =\sum_{u\in\widehat{G}}d(u$)Tr(A$^*_uB_u$). (5)

Ký hiệu chuẩn Hilbert trên $L^2( \widehat{G})$ cũng bởi $\| \|_2$, sao cho $\|A\|^2_2=\sum_{u\in\widehat{G}}\|A_u\|^2_2$ với $A\in L^2( \widehat{G})$.

Nếu $f$ là một hàm phức khả tích trên G, đặt

$u(f) =\int_Gf(g)u(g)dg\in$ End(E$_u$) (6)

với mọi $u\in \widehat{G}$. Ta có $\|u(f)\|_{\infty}\leq \int_G|f(g)|dg=\|f\|_1$. Biến đổi đối Fourier của $f$, ký hiệu bởi $\mathscr{F}(f)$, là họ $(u(f))_{u\in\widehat{G}}\in F( \widehat{G})$. Nếu $f\in L^2( \widehat{G})$,

$^6$ Xem chú ý $^1$, §7, p. 66.

$$
\|f\|^2_2=\sum_{u\in\widehat{G}}\langle u(f)|u(f)\rangle =\|\overline{\mathscr{F}}(f)\|^2_2
$$

do đó $\overline{\mathscr{F}}$ cảm sinh một ánh xạ tuyến tính đẳng cự từ không gian Hilbert $L^2(G)$ đến không gian Hilbert $L^2( \widehat{G}):$ nói cách khác, với $f$ và $f'$ trong $L^2$(G), ta có

$\int_G\overline{f(g)}f'(g)dg=\langle \overline{\mathscr{F}}(f)|\overline{\mathscr{F}}(f')\rangle =\sum_{u\in\widehat{G}}d(u$)Tr($u(f)^*u(f')$). (7)

Với $f$ và $f'$ thuộc $L^1$(G), tích chập $f*f'$ của $f$ và $f'$ được định nghĩa bởi

$$
(f*f')(h) =\int_Gf(hg^{-1})f'(g)dg=\int_Gf(g)f'(g^{-1}h)dg
$$

(nguyên có nghĩa đối với hầu khắp mọi $h\in G$).

Ta có $f*f'\in L^1(G)$ và, với mọi $u\in \widehat{G},u(f*f') =u(f)u(f')$, do đó

$$
\overline{\mathscr{F}}(f*f') =\overline{\mathscr{F}}(f).\overline{\mathscr{F}}(f') \tag{8}
$$

Ngược lại, cho $A = (A_u)_{u\in\widehat{G}}$ là một phần tử của $F( \widehat{G})$; với mọi $u\in \widehat{G}$, gọi $\mathscr{F}_uA$ là hàm (giải tích) trên G được xác định bởi

$(\mathscr{F}_uA)(g) =\langle u(g)|A_u\rangle =d(u$)Tr(A$_uu(g)^{-1}$). (9)

Nếu $A\in L^2( \widehat{G})$, họ $(\mathscr{F}_uA)_{u\in\widehat{G}}$ là khả tổng trong $L^2(G)$; biến đổi Fourier của A, được ký hiệu bởi $\mathscr{F}$(A), là tổng của họ này. Các ánh xạ $\mathscr{F}$ và $\mathscr{F}$ là các đẳng cấu ngược nhau giữa các không gian Hilbert $L^2(G)$ và $L^2( \widehat{G})$.

Nói cách khác:

#### Mệnh đề 1 {#lie-ix-s8-prop-1 .statement tag=01GZ}

Mọi hàm phức bình phương khả tích $f$ trên G là tổng trong không gian Hilbert $L^2(G)$ của họ $(f_u)_{u\in\widehat{G}}$ trong đó, với mọi $h\in G$ và mọi $u\in \widehat{G}$,

$$
f_u(h) =\langle u(h)|u(f)\rangle
$$

$=d(u)\int_Gf(g$)Tr($u(gh^{-1})$)$dg=d(u)\int_Gf(gh$)Tr($u(g)$)$dg$. (10)

Với mọi $u\in \widehat{G}$ chọn một cơ sở trực chuẩn $Bu$ của $E_u$, và ký hiệu bởi $(u_{ij}(g))$ ma trận của $u(g)$ trong cơ sở này. Mệnh đề 1 cũng có nghĩa là họ các hàm $\surd\overline{d(u)}u_{ij}$, với $u$ trong $\widehat{G}$ và $i, j$ trong $B_u$, là một cơ sở trực chuẩn của không gian $L^2(G)$.

Nếu $f$ là một hàm khả tích trên G sao cho họ $(f_u)$ là khả tổng đều, thì tổng của họ này là một hàm liên tục trùng với $f$ hầu khắp mọi nơi; nói cách khác, nếu ta giả sử thêm rằng $f$ là liên tục, thì với mọi $h\in G$, $f(h) =\sum_{u\in\widehat{G}}d(u)\int_Gf(gh$)Tr($u(g)$)$dg$. (11)

Ngược lại, cho $A\in F( \widehat{G})$; nếu họ $(\mathscr{F}_uA)_{u\in\widehat{G}}$ là khả tổng đều, hàm

$g \rightarrow \sum_{u\in\widehat{G}}(\mathscr{F}_uA)(g) =\sum_{u\in\widehat{G}}d(u$)Tr(A$_uu(g)^{-1}$)

là một hàm liên tục trên G mà biến đổi Fourier ngược của nó là A.

Cho $f$ là một hàm khả tích trên G, và cho $s\in G$. Ký hiệu $\gamma (s)f$ và $\delta (s)f$ là các hàm trên G được xác định bởi $\gamma (s)f=\varepsilon_s*f,\delta (s)f=f*\varepsilon_{s^{-1}}$, nghĩa là,

$(\gamma (s)f)(g) =f(s^{-1}g),(\delta (s)f)(g) =f(gs)$ với $g\in G$,

(Chương III, §3, no. 4 và Tích phân, Chương VII, §1, no. 1). Ta có

$$
u(\gamma (s)f) =\int_Gf(s^{-1}g)u(g)dg=\int_Gf(g)u(sg)dg
$$

do đó

$$
u(\gamma (s)f) =u(s)u(f) \tag{12}
$$

và tương tự

$$
u(\delta (s^{-1})f) =u(f)u(s) \tag{13}
$$

Khi G giao hoán, $\widehat{G}$ là tập nền của nhóm đối ngẫu của G (Các lý thuyết phổ, Chương II, §1, số $1$)$,d(u) = 1$ với mọi $u\in \widehat{G}$, và ta thu được lại các định nghĩa của biến đổi Fourier đã cho trong Các lý thuyết phổ, Chương II.

### 2. BIẾN ĐỔI FOURIER CỦA CÁC HÀM KHẢ VI VÔ HẠN

Nhắc lại (Chương III, §3, no. 1, Định nghĩa 2) rằng U(G) ký hiệu đại số các phân bố trên G có giá được chứa trong $\{e\}$. Đơn ánh chính tắc của $\mathfrak{g}$ vào U(G) mở rộng thành một đẳng cấu từ đại số bao của đại số Lie $\mathfrak{g}$ lên U(G) (đã dẫn, no. 7, Mệnh đề 25); từ nay ta đồng nhất hai đại số này bởi đẳng cấu này. Nếu $f$ là một hàm phức khả vi vô hạn trên G và nếu $t\in U(G)$, ta ký hiệu $L_tf$ và $R_tf$ là các hàm trên G được xác định bởi

$$
L_tf(g) =\langle \varepsilon_g*t, f\rangle ,R_tf(g) =\langle t*\varepsilon_g, f\rangle
$$

(xem đã dẫn, no. 6). Với mọi $g\in G$,

$$
L_t\circ \gamma (g) =\gamma (g)\circ L_t,R_t\circ \delta (g) =\delta (g)\circ R_t
$$

Cho $u\in \widehat{G}$; ký hiệu $Eu$ là không gian của $u$. Cấu xạ của các nhóm Lie $u: G\rightarrow \mathbf{G}\mathbf{L}(E_u)$ cho bởi phép vi phân một đồng cấu của các đại số Lie (thực) $\mathfrak{g}\rightarrow$ End(E$_u$), do đó là một đồng cấu của các đại số, cũng được ký hiệu bởi $u$, từ U(G) vào End(E$_u$). Nếu $t\in U(G)$ và nếu $f$ là một hàm khả vi vô hạn trên G, thì

$$
u(L_tf) =u(f)u(t^{\vee}), u(R_tf) =u(t^{\vee})u(f) \tag{14}
$$

trong đó $t^{\vee}$ ký hiệu ảnh của $t$ qua tự phản tự đẳng cấu chính của U(G) (Chương I, §2, no. 4); thực vậy, chỉ cần kiểm tra điều này với $t\in \mathfrak{g}$, trong trường hợp đó điều này suy ra bởi phép vi phân từ các công thức (12) và (13) (xem Chương III, §3, no. 7, Mệnh đề 27).

Với mọi $u\in \widehat{G}$, ký hiệu $\lambda (u)$ là trọng số cao nhất của $u($§7, no. 2, Định lý 1), do đó $u \rightarrow \lambda (u)$ là một ánh xạ song ánh từ $\widehat{G}$ lên tập hợp $X_{++}$ gồm các phần tử trội của X(T).

Cho $\Gamma \in U(G)$ là một phần tử Casimir của G (§7, no. 6); với mọi $u\in \widehat{G}$, tự đồng cấu $u(\Gamma )$ của $E_u$ là một phép vị tự, có tỷ số được ký hiệu bởi $\widetilde{\Gamma}(u)$, do đó ta có một ánh xạ $u \rightarrow \widetilde{\Gamma}(u)$ từ $\widehat{G}$ vào $\mathbf{C}$.

Nếu $\varphi$ và $\psi$ là hai hàm trên $\widehat{G}$ có các giá trị thực dương, ký hiệu quan hệ “$\varphi \preccurlyeq \psi$” hoặc “$\varphi (u)\preccurlyeq \psi (u$)” là quan hệ “tồn tại $M>0$ sao cho $\varphi (u)\leq M\psi (u)$ với mọi $u\in \widehat{G}$”; đây là một quan hệ tiền thứ tự trên tập hợp các hàm trên $\widehat{G}$ có các giá trị thực dương.

#### Mệnh đề 2 {#lie-ix-s8-prop-2 .statement tag=01H0}

Cho $m \rightarrow  \|m\|$ là một chuẩn trên không gian vectơ $\mathbf{R}$- $\mathbf{R}\otimes X(T)$ và $\Gamma$ là một phần tử Casimir của G. Cho $\varphi$ là một hàm trên $\widehat{G}$ có các giá trị thực dương.

a) Các điều kiện sau là tương đương:

(i) Tồn tại một số nguyên $n >0$ sao cho $\varphi (u)\preccurlyeq (\|\lambda (u)\|+ 1)^n$ (tương ứng, với mọi số nguyên $n >0$, ta có $\varphi (u)\preccurlyeq (\|\lambda (u)\|+ 1)^{-n}$).

(ii) Tồn tại một số nguyên $n >0$ sao cho $\varphi (u)\preccurlyeq ( \widetilde{\Gamma}(u) + 1)^n$ (tương ứng, với mọi số nguyên $n >0$, ta có $\varphi (u)\preccurlyeq ( \widetilde{\Gamma}(u) + 1)^{-n}$).

b) Nếu G là nửa đơn, các điều kiện (i) và (ii) cũng tương đương với:

(iii) Tồn tại một số nguyên $n >0$ sao cho $\varphi (u)\preccurlyeq d(u)^n$ (tương ứng, với mọi số nguyên $n >0$, ta có $\varphi (u)\preccurlyeq d(u)^{-n}$).

Trước hết chú ý rằng điều kiện (i) rõ ràng độc lập với lựa chọn chuẩn. Do đó ta có thể dùng chuẩn được xác định bởi dạng toàn phương $Q_{\Gamma}$ liên kết với $\Gamma ($§7, no. 6, Prop. 4). Khi đó

$$
0\leq \widetilde{\Gamma}(u) =\|\lambda (u) +\rho \|^2- \|\rho \|^2
$$

nên $\widetilde{\Gamma}(u) + 1\preccurlyeq (\|\lambda (u)\|+ 1)^2\preccurlyeq \widetilde{\Gamma}(u) + 1$, do đó suy ra a).

Hơn nữa, nếu G là nửa đơn,

$\|\lambda (u) +\rho \|\preccurlyeq d(u)\preccurlyeq \|\lambda (u) +\rho \|^N$, trong đó $N = 1/$2(dim $G-$ dim T)

(§7, no. 5, Cor. 1 of Th. 3), nên $\|\lambda (u)\|+ 1\preccurlyeq d(u)\preccurlyeq (\|\lambda (u)\|+ 1)^N$, do đó suy ra b).

Từ Mệnh đề 2 suy ra rằng điều kiện (i) độc lập với lựa chọn xuyến cực đại, buồng, và chuẩn, và rằng điều kiện (ii) độc lập với lựa chọn phần tử Casimir. Một hàm $\varphi$ thỏa mãn các điều kiện (i) và (ii) được gọi là tăng vừa phải (tương ứng, giảm nhanh). Tích của hai hàm tăng vừa phải là tăng vừa phải; tích của một hàm tăng vừa phải và một hàm giảm nhanh là giảm nhanh. Nếu $\varphi$ giảm nhanh, họ $(\varphi (u))_{u\in\widehat{G}}$ là tổng được.

#### Ví dụ {#lie-ix-s8-n2-exa-1 .statement tag=01H1}

Hàm $u \rightarrow d(u)$ là tăng vừa phải (§7, no. 5, Cor. 1 of Th. 3); với mọi chuẩn $\| \|$ trên $\mathbf{R}\otimes X(T)$, hàm $u \rightarrow  \|\lambda (u)\|$ là tăng vừa phải. Với mọi phần tử Casimir $\Gamma$, hàm $u \rightarrow \widetilde{\Gamma}(u)$ là tăng vừa phải; tổng quát hơn:

#### Mệnh đề 3 {#lie-ix-s8-prop-3 .statement tag=01H2}

Với mọi $t\in$ U(G), các hàm $u \rightarrow  \|u(t)\|_{\infty}$ và $u \rightarrow  \|u(t)\|_2$ trên $\widehat{G}$ là tăng vừa phải.

Vì tích của hai hàm tăng vừa phải là tăng vừa phải, chỉ cần chứng minh điều này khi $t\in \mathfrak{g}:$ trong trường hợp đó mệnh đề suy ra từ Nhận xét trong §7, no. 6 và bất đẳng thức

$$
\|u(t)\|_2\leq d(u)\|u(t)\|_{\infty}
$$

#### Định lý 1 {#lie-ix-s8-thm-1 .statement tag=01H3}

a) Cho $f$ là một hàm phức khả vi vô hạn trên G. Khi đó họ $(f_u)_{u\in\widehat{G}}$, trong đó $f_u(g) =\langle u(g)|u(f)\rangle$, là tổng được đều trên G và, với mọi $h\in G$,

$f(h) =\sum_{u\in\widehat{G}}\langle u(h)|u(f)\rangle =\sum_{u\in\widehat{G}}d(u)\int_Gf(g$)Tr($u(gh^{-1})$)$dg$.

(b) Cho $f$ là một hàm khả tích trên G; khi đó $f$ bằng hầu khắp nơi với một hàm khả vi vô hạn khi và chỉ khi hàm $u \rightarrow  \|u(f)\|_{\infty}$ giảm nhanh trên $\widehat{G}$.

Cho $f$ là một hàm khả vi vô hạn trên G, và cho $\Gamma$ là một phần tử Casimir đối với G; theo công thức (14),

$$
\widetilde{\Gamma}(u)^nu(f) =u(f)u(\Gamma )^n=u((L_{\Gamma})^nf)
$$

với mọi $n\geq 0$, và do đó

$\widetilde{\Gamma}(u)^n\|u(f)\|_{\infty}\leq  \|(L_{\Gamma})^nf\|_1\leq$ sup$_{g\in G}|((L_{\Gamma})^nf)(g)|$; (15)

do đó, hàm $u \rightarrow  \|u(f)\|_{\infty}$ thực sự giảm nhanh.

Ngược lại, cho $A = (A_u)_{u\in\widehat{G}}$ là một phần tử của $F( \widehat{G})$ sao cho hàm $u \rightarrow  \|A_u\|_{\infty}$ giảm nhanh. Đặt $f_u(g) =\langle u(g)|A_u\rangle$; hàm $g \rightarrow f_u(g)$ là giải tích, do đó khả vi vô hạn. Theo Chap. III, §3, no. 7, Prop. 27,

$$
(L_xf_u)(g) =\langle u(g)u(x)|A_u\rangle
$$

với mọi $x\in \mathfrak{g}$. Cho $t\in U(G)$; theo công thức trước đó,

$$
(L_tf_u)(g) =\langle u(g)u(t)|A_u\rangle
$$

và do đó

$$
|(L_tf_u)(g)|=|\langle u(g)u(t)|A_u\rangle  \leq d(u)^2\|u(t)\|_{\infty}\|u(g)\|_{\infty}\|A_u\|_{\infty}
$$

$$
=d(u)^2\|u(t)\|_{\infty}\|A_u\|_{\infty}
$$

Vì $d(u)$ và $\|u(t)\|_{\infty}$ tăng vừa phải (Prop. 3) và $\|A_u\|_{\infty}$ giảm nhanh, hàm $u \rightarrow$ sup$_g|(L_tf_u)(g)|$ giảm nhanh; do đó, họ $(L_tf_u)_{u\in\widehat{G}}$ khả tổng đều. Suy ra$^7$ rằng tổng của họ $(f_u)$ là một hàm khả vi vô hạn trên G, có đối biến đổi Fourier là $(A_u)$, do đó định lý được chứng minh.

Ký hiệu $\mathscr{S}( \widehat{G})$ là không gian con vectơ của $L^2( \widehat{G})$ gồm các họ $A = (A_u)_{u\in\widehat{G}}$ sao cho hàm $u \rightarrow  \|A_u\|_{\infty}$ giảm nhanh trên $\widehat{G}$. Theo định lý, các ánh xạ $\mathscr{F}:f \rightarrow (u(f))_{u\in\widehat{G}}$ và $\mathscr{F}: A \rightarrow \sum_{u\in\widehat{G}}\langle u(g)|A_u\rangle$ cảm sinh các đẳng cấu nghịch đảo giữa các không gian vectơ phức $\mathscr{C}^{\infty}(G;\mathbf{C})$ và $\mathscr{S}( \widehat{G})$. Trang bị cho không gian $\mathscr{C}^{\infty}(G;\mathbf{C})$ tôpô của sự hội tụ đều $C^{\infty}$ (§6, no. 4), có thể được xác định bởi họ các nửa chuẩn $f \rightarrow$ sup$_{g\in G}|L_tf(g)|$ với $t\in U(G)$, và cho không gian $\mathscr{S}( \widehat{G})$ tôpô được xác định bởi dãy các nửa chuẩn $p_n: A \rightarrow$ sup$_{u\in\widehat{G}}( \widetilde{\Gamma}(u) + 1)^n\|A_u\|_{\infty}$. Công thức (15) của chứng minh trước cho thấy rằng $\overline{\mathscr{F}}$ là liên tục. Cho $t\in U(G)$, và cho $A = (A_u)_{u\in\widehat{G}}$ là một phần tử của $\mathscr{S}( \widehat{G})$; đặt $f_n(g) =\langle u(g)|A_u\rangle$. Cho $p$ là một số nguyên sao cho $\sum_{u\in\widehat{G}}\widetilde{\Gamma}(u)^{-p}= M<\infty$. Theo chứng minh trước, tồn tại một số nguyên dương $m$ sao cho, với mọi $g\in G$,

$$
|(L_tf_u)(g)| \leq d(u)^2\|u(t)\|_{\infty}\|A_u\|_{\infty}\leq m.(1 + \widetilde{\Gamma}(u))^m\widetilde{\Gamma}(u)^{-p}\|A_u\|_{\infty}
$$

do đó $|(L_t\mathscr{F}(A))(g)| \leq mMp_m(A)$; điều này chứng minh rằng $\mathscr{F}$ là liên tục. Do đó:

#### Hệ quả {#lie-ix-s8-n2-cor-1 .statement tag=01H4}

Các ánh xạ $\overline{\mathscr{F}}:f \rightarrow (u(f))_{u\in\widehat{G}}$ và $\mathscr{F}: A \rightarrow \sum_{u\in\widehat{G}}\langle u(g)|A_u\rangle$ cảm sinh các đẳng cấu nghịch đảo giữa các không gian vectơ tôpô $\mathscr{C}^{\infty}(G;\mathbf{C})$ và $\mathscr{S}( \widehat{G})$.

$^7$ Điều này suy ra từ sự kiện rằng không gian $\mathscr{C}^{\infty}(G;\mathbf{C})$, với tôpô của sự hội tụ đều

$C^{\infty}$ (§6, no. 4), là đầy đủ.

### 3. BIẾN ĐỔI FOURIER CỦA CÁC HÀM TRUNG TÂM

Với mọi $u\in \widehat{G}$, ký hiệu $\chi_u$ là đặc trưng của $u$; do đó,

$\chi_u(g) =$ Tr($u(g)$)$,(g\in G)$. (16) Nhắc lại từ Lý thuyết Phổ các công thức

$$
\chi_u*\chi_v= 0(u, v\in \widehat{G}, u\not=v) \tag{17}
$$

$$
\chi_u*\chi_u=\frac{1}{d(u)}\chi_u(u\in \widehat{G}) \tag{18}
$$

Với mọi $u\in \widehat{G}$, ký hiệu $\varepsilon_u$ là ánh xạ đồng nhất của $E_u$. Nhắc lại (§7, no. 4) rằng ZL$^2(G)$ chỉ không gian con của $L^2(G)$ gồm các lớp của các hàm $f$ là trung tâm, nghĩa là sao cho $f\circ$ Int $s=f$ với mọi $s\in G$, hoặc tương đương là $\gamma (s)f=\delta (s^{-1})f$ với mọi $s\in G$.

#### Mệnh đề 4 {#lie-ix-s8-prop-4 .statement tag=01H5}

Cho $f\in L^2(G)$. Khi đó $f$ là trung tâm khi và chỉ khi $u(f)$ là một phép vị tự với mọi $u\in \widehat{G}$. Trong trường hợp đó

$$
u(f) =\frac{\varepsilon_u}{d(u)}\int_Gf(g)\chi_u(g)dg \tag{19}
$$

Theo Mệnh đề 1 (no. 1), nói rằng $f$ là trung tâm có nghĩa là $u(\gamma (s)f) =$ $u(\delta (s^{-1})f)$ với mọi $s\in G$ và mọi $u\in \widehat{G}$; nhưng điều này cũng có thể được viết thành $u(s)u(f) =u(f)u(s)$ với mọi $s\in G$ và mọi $u\in \widehat{G}$ (các công thức (12) và (13)), do đó suy ra mệnh đề đầu tiên của Mệnh đề 4 (Bổ đề Schur). Nếu $u(f)$ là một phép vị tự, thì $u(f) =\lambda_u\varepsilon_u$ với

$\lambda_u=\frac{1}{d(u)}$ Tr($u(f)$) $=\frac{1}{d(u)}\int_Gf(g$)Tr($u(g)$)$dg=\frac{1}{d(u)}\int_Gf(g)\chi_u(g)dg$.

Do đó, với $f\in$ ZL$^2(G)$ ta có

$$
u(f) =\langle \overline{\chi}_u|f\rangle \frac{\varepsilon_u}{d(u)}\rangle \tag{20}
$$

nên

$$
\overline{\mathscr{F}}(f) =(\langle \overline{\chi}_u|f\rangle \frac{\varepsilon_u}{d(u)})_{u\in\widehat{G}} \tag{21}
$$

với

$$
\|\overline{\mathscr{F}}(f)\|^2_2=\sum||||\langle \overline{\chi}_u|f\rangle \frac{\varepsilon_u}{d(u)}||||^{22}=\sum|\langle \overline{\chi}_u|f\rangle |^2
$$

$uu$

Ngược lại, nếu $\varphi$ là một hàm phức khả tích bình phương trên $\widehat{G}$, phần tử $(\frac{\varphi(u)}{d(u)}\varepsilon_u)_{u\in\widehat{G}}$ của $F( \widehat{G})$ thuộc về $L^2( \widehat{G})$, và ta có (công thức (9)) $(\mathscr{F}_u(\frac{\varphi(u)}{d(u)}\varepsilon_u))(g) =d(u$)Tr $(\frac{\varphi(u)}{d(u)}\varepsilon_uu(g)^{-1})=\varphi (u)\overline{\chi}_u(g)$,

do đó

$$
\mathscr{F}((\frac{\varphi(u)}{d(u)}\varepsilon_u))=\sum\varphi (u)\overline{\chi}_u \tag{22}
$$

$u\in \widehat{G}$

Đặc biệt, chú ý rằng các công thức (20) và (21) cho, với $u, v$ trong $\widehat{G},^8$

$u(\overline{\chi}_v) = 0$ nếu $u\not=v$, (23)

$u(\overline{\chi}_u) =\frac{\varepsilon_u}{d(u)}\in$ End(E$_u$), (24)

$\overline{\mathscr{F}}(\chi_u) =\frac{\varepsilon_u}{d(u)}\in$ End(E$_u$)$\subset F( \widehat{G})$. (25)

#### Mệnh đề 5 {#lie-ix-s8-prop-5 .statement tag=01H6}

Cho $f$ là một hàm trung tâm liên tục trên G. Khi đó $f$ khả vi vô hạn khi và chỉ khi hàm $u \rightarrow  |\langle \chi_u|f\rangle |$ là giảm nhanh trên $\widehat{G}$; trong trường hợp đó,

$$
f(g) =\sum_{u\in\widehat{G}}\langle \chi_u|f\rangle \chi_u(g)
$$

với mọi $g\in G$.

Theo Th. $1b)$, hàm $\overline{f}$ khả vi vô hạn khi và chỉ khi hàm $u \rightarrow  \|u(\overline{f})\|_{\infty}$ là giảm nhanh; nhưng, theo (20),

$$
\|u(\overline{f})\|_{\infty}=\frac{1}{d(u)}|\langle \chi_u|f\rangle |
$$

suy ra mệnh đề đầu tiên, vì các hàm $d(u)$ và $\frac{1}{d(u)}$ là tăng vừa phải.

Giả sử rằng $f$ khả vi vô hạn; theo Th. $1a),f(g) =\sum_{u\in\widehat{G}}f_u(g)$ với mọi $g\in G$, do đó

$f_u(g) =\langle u(g)|u(f)\rangle =d(u$)Tr($u(g)^{-1}.u(f)$) $=d(u$)Tr$(u(g)^{-1}\langle \overline{\chi}_u|f\rangle \frac{\varepsilon_u}{d(u)})$

$=\langle \overline{\chi}_u|f\rangle$Tr($u(g)^{-1}$) $=\langle \overline{\chi}_u|f\rangle \overline{\chi}_u(g)$.

Do đó, $f(g) =\sum_{u\in\widehat{G}}\langle \overline{\chi}_u|f\rangle \overline{\chi}_u(g)$; nhưng, với mọi $u\in \widehat{G}$, biểu diễn đối ngẫu của biểu diễn $u$ là $u'$ thỏa mãn $\overline{\chi}_u=\chi_{u'}$ và ánh xạ $u \rightarrow u'$ là một phép hoán vị của $\widehat{G}$; vì vậy ta cũng có $f(g) =\sum_{u\in\widehat{G}}\langle \chi_u|f\rangle \chi_u(g)$, do đó có mệnh đề.

$^8$ Ta nhúng End(E$_u$) vào tích $F( \widehat{G}) =\prod_{v\in\widehat{G}}$ End(E$_v$) bằng cách gán cho mỗi

$A\in$ End(E$_u$) họ $(A_v)_{v\in\widehat{G}}$ sao cho $A_u= A$ và $A_v= 0$ với $v\not=u$.

#### Hệ quả {#lie-ix-s8-n3-cor-1 .statement tag=01H7}

Cho $f$ là một hàm trung tâm liên tục trên G. Khi đó $f$ khả vi vô hạn khi và chỉ khi hạn chế của $f$ trên T là khả vi vô hạn.

Thật vậy, theo Hệ quả 4 của §7, no. 4,

$\langle \chi_u|f\rangle =\int_G\overline{\lambda(u)(t)}\varphi (t)dt$, trong đó $\varphi (t) =\prod_{\alpha >0}(1-\alpha (t)^{-1})f(t)$.

Nếu $f|T$ là khả vi vô hạn, thì $\varphi$ cũng vậy; theo Mệnh đề 5, áp dụng cho nhóm T, hàm $\mu \rightarrow \int_T\overline{\mu(t)}\varphi (t)dt$ trên $\widehat{T} = X(T)$ khi đó giảm nhanh, và hàm $u \rightarrow  \langle \chi_u|f\rangle$ cũng vậy; do đó hàm $f$ là khả vi vô hạn (Mệnh đề 5). Điều đảo lại là hiển nhiên.

### 4. CÁC HÀM TRUNG TÂM TRÊN G VÀ CÁC HÀM TRÊN T

Ký hiệu $\mathscr{C}(G)$ là không gian các hàm phức liên tục trên G và $\mathscr{C}^{\infty}(G)$ là không gian con của các hàm khả vi vô hạn. Khi đó ta có một dãy các phép bao hàm

$$
\Theta (G)\subset \mathscr{C}^{\infty}(G)\subset \mathscr{C}(G)\subset L^2(G)
$$

Ký hiệu lần lượt $Z\Theta (G),Z\mathscr{C}^{\infty}(G),Z\mathscr{C}(G)$, ZL$^2$(G), là các không gian con gồm các hàm trung tâm trong những không gian khác nhau này. Tương tự, đưa vào các không gian $\Theta (T),\mathscr{C}^{\infty}(T),\mathscr{C}(T),L^2(T)$; với mọi không gian E trong danh sách này, ký hiệu $E^W$ (resp. $E^{-W}$) là không gian con gồm các phần tử bất biến (resp. phản bất biến) đối với phép toán của nhóm Weyl W. Ta có một biểu đồ giao hoán

$$
Z\mathscr{C}(G)\longrightarrow^{a_c}\mathscr{C}(T)^W
$$

$$
Z\mathscr{C}^{\infty}(G)\longrightarrow^{a_{\infty}}\mathscr{C}^{\infty}(T)^W
$$

$$
Z\Theta (G)\longrightarrow^{a_{\Theta}}\Theta (T)^W
$$

trong đó các mũi tên đứng biểu diễn các phép nhúng chính tắc, và các ánh xạ $a_c, a_{\infty}, a_{\Theta}$ được cảm sinh bởi ánh xạ hạn chế từ $\mathscr{C}(G)$ đến $\mathscr{C}(T)$.

Các ánh xạ $a_c, a_{\infty}, a_{\Theta}$ là song ánh (§2, no. 5, Hệ quả 1 của Mệnh đề 5, §8, no. 3, Hệ quả của Mệnh đề 5, và §7, no. 3, Hệ quả của Mệnh đề 2).

Giả sử bây giờ rằng nửa tổng $\rho$ của các nghiệm dương thuộc về X(T) và xét ánh xạ $b$ ánh xạ mỗi hàm liên tục $\varphi$ trên T vào $\varphi .J(\rho )$. Ta có một biểu đồ giao hoán

ZL$^2(G)--------------------\longrightarrow^uL^2(T)^{-W}$

$$
Z\mathscr{C}(G)\longrightarrow^{a_c}\mathscr{C}(T)^W\longrightarrow^{b_c}\mathscr{C}(T)^{-W}
$$

$$
Z\mathscr{C}^{\infty}(G)\longrightarrow^{a_{\infty}}\mathscr{C}^{\infty}(T)^W\longrightarrow^{b_{\infty}}\mathscr{C}^{\infty}(T)^{-W}
$$

$$
Z\Theta (G)\longrightarrow^{a_{\Theta}}\Theta (T)^W\longrightarrow^{b_{\Theta}}\Theta (T)^{-W}
$$

trong đó các mũi tên đứng là các phép nhúng chính tắc, các ánh xạ $b_c, b_{\infty}, b_{\Theta}$ được cảm sinh bởi $b$, và $u$ mở rộng $b_c\circ a_c$ bởi tính liên tục (§7, no. 4, Hệ quả 3 của Định lý 2). Các ánh xạ $u$ và $b_{\Theta}$ là song ánh (loc. cit.); $b_{\infty}$ cũng vậy (Bài tập 5); mặt khác, $b_c$ nói chung không toàn ánh (Bài tập 6).

### Bài tập {#lie-ix-s8-exercises}

Xem các [bài tập cho § 8](exercises/s8/).
