---
book: ts
book_title: Théories spectrales
chapter: III
chapter_title: APPLICATIONS LINÉAIRES COMPACTES ET PERTURBATIONS
section: 5
section_title: Perturbation par une application linéaire compacte
lang: vi
source: ts-iii-v-fr
book_pages: TS III.71-TS III.82, TS III.125-TS III.128
pdf_pages: 0085-0096, 0139-0142
extraction: native
subsections:
    - "no": 1
      title: Morphismes stricts et propreté
      page: 71
      pdf_page: 85
    - "no": 2
      title: Perturbation des applications linéaires injectives ou surjectives
      page: 72
      pdf_page: 86
    - "no": 3
      title: Perturbation des applications de Fredholm
      page: 73
      pdf_page: 87
    - "no": 4
      title: Perturbation des endomorphismes de Riesz
      page: 75
      pdf_page: 89
    - "no": 5
      title: La théorie de Frédéric Riesz
      page: 77
      pdf_page: 91
    - "no": 6
      title: Alternative de Fredholm
      page: 79
      pdf_page: 93
statements: 19
exercises: 11
content_sha256: a15a730e6a6f6b9c7a8f8ad8dd0e1ae6b2f2efbd87f4cd136d6f999fa1af513b
translated_from: content/en-mt/ts/III/05_s5_perturbation_par_une_application.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 00c0f0e72c676ebd456b4c6b9377c906b9ac16d553f5dd1629b67d663477cbc7
translation_model: gpt-5.4
translation_run: translate-vi-12f45fca
glossary_version: 34
glossary_terms_sha256: 3b1dd58ec4b6eb011fb03b7c9ea0eaab27c193d55951f727b9acf22f6d7d12f2
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 5. NHIỄU LOẠN BỞI MỘT ÁNH XẠ TUYẾN TÍNH COMPACT

### 1. Cấu xạ ngặt và tính riêng

#### Bổ đề 1 {#ts-iii-s5-lem-1 .statement tag=02TK}

Cho E và F là các không gian vectơ tôpô, $u$ là một ánh xạ tuyến tính liên tục từ E vào F và U là một lân cận của 0 trong E. Giả sử rằng $u$ cảm sinh một đồng phôi của U lên một tập con đóng của F. Khi đó ảnh I của $u$ là đóng và $u$ cảm sinh một đồng phôi của E lên I.

Tập hợp $u(U)$ là một lân cận của 0 trong I; nó đóng trong F, do đó nhóm con I của F là địa phương đóng tại 0, và do đó nó là đóng (TG, III, p. 7, prop. 4).

Vì Ker($u$) chỉ giao với U tại 0, ta có Ker($u$) $=\{0\}$ và ánh xạ $u$ là đơn ánh. Cho V là một lân cận đóng của 0 trong E được chứa trong U. Vì $u(\mathring{V})$ là một lân cận của 0 trong $u$(V), tồn tại một lân cận cân bằng W của 0 trong F sao cho $u(V)\cap W\subset u(\mathring{V})$. Tập hợp $\overset{-1}{u}(W)$ là cân bằng, nên liên thông. Nó chứa 0 và được chứa trong $\mathring{V}\cup (E$ - V). Vì $\mathring{V}$ và E- V là các tập mở rời nhau của E, tập hợp $\overset{-1}{u}(W)$ được chứa trong $\mathring{V}$, do đó $W\cap I\subset u(\mathring{V})$. Do đó $u(\mathring{V})$ là một lân cận của 0 trong I. Điều này suy ra rằng $u$ cảm sinh một đồng phôi của E lên I.

#### Mệnh đề 1 {#ts-iii-s5-prop-1 .statement tag=02TL}

Cho E là một không gian lồi địa phương tách biệt, F là một không gian lồi địa phương và $u$ là một ánh xạ tuyến tính liên tục từ E vào F. Các điều kiện sau là tương đương:

(i) Ánh xạ $u$ là một cấu xạ ngặt, hạt nhân của nó có số chiều hữu hạn và ảnh của nó đóng trong F ;

(ii) Tồn tại một lân cận đóng V của 0 trong E sao cho hạn chế của $u$ lên V là riêng (TG, I, p. 72).

(i) $=\Rightarrow$ (ii) : Giả sử rằng $u$ thỏa mãn điều kiện (i). Vì hạt nhân của $u$ có số chiều hữu hạn, nó có một phần bù tôpô $E_1$ trong E (III, p. 55, prop. 1), và tồn tại một lân cận compact C của 0 trong Ker($u$). Đồng nhất E với $E_1\times$ Ker($u$); khi đó tập hợp $V = E_1\times C$ là một lân cận đóng của 0 trong E. Hạn chế của $u$ lên V là hợp thành của phép chiếu từ $E_1\times C$ lên $E_1$, phép chiếu này là riêng (TG, I, p. 77, cor. 5), và của hạn chế $u_1$ của $u$ lên $E_1$. Bây giờ $u_1$ là một đồng phôi của $E_1$ lên một không gian con đóng của F, nên là riêng (TG, I, p. 72, prop. 2). Hợp thành của hai ánh xạ riêng là riêng (TG, I, p. 73, prop. 5, a)), nên hạn chế của $u$ lên V là riêng.

(ii) $=\Rightarrow$ (i) : Cho V là một lân cận đóng của 0 trong E sao cho hạn chế $v$ của $u$ lên V là riêng. Khi đó tập hợp $V\cap$ Ker($u$) $=\overset{-1}{v}(\{0\})$ là compact (TG, I, p. 75, th. 1); do đó, không gian vectơ Ker($u$) là địa phương compact, nên có số chiều hữu hạn (EVT, I, p. 15, th. 3). Cho $E_1$ là một phần bù tôpô của Ker($u$) trong E (prop. 1 of III, p. 55); đặt $V_1= E_1\cap V$. Tập hợp $V_1$ là đóng trong V. Ánh xạ $u|V_1$ là riêng (TG, I, p. 74, cor. 1) và đơn ánh, nên là một đồng phôi của $V_1$ lên một tập con đóng của F (TG, I, p. 72, prop. 2). Theo Bổ đề 1, hạn chế của $u$ lên $E_1$ là một đồng phôi của $E_1$ lên một không gian con đóng của F, nên $u$ là một cấu xạ ngặt có ảnh đóng.

### 2. Nhiễu loạn của các ánh xạ tuyến tính đơn ánh hoặc toàn ánh

#### Định lý 1 {#ts-iii-s5-thm-1 .statement tag=02TM}

Cho E và F là các không gian lồi địa phương tách biệt và $u$ là một cấu xạ ngặt từ E vào F, với hạt nhân có số chiều hữu hạn và ảnh đóng. Cho $h$ là một ánh xạ tuyến tính compact từ E vào F. Ánh xạ tuyến tính $u+h$ là một cấu xạ ngặt, hạt nhân của nó có số chiều hữu hạn và ảnh của nó đóng.

Theo mệnh đề 1 của III, p. 71, tồn tại một lân cận đóng V của 0 trong E sao cho hạn chế của $u$ trên V là riêng. Vì $h$ là compact, tồn tại một lân cận đóng W của 0 được chứa trong V sao cho tập $h(W)$ là tương đối compact. Đặt $C =h(W)$. Hạn chế của $u$ trên W là riêng (TG, I, p. 74, hệ quả 1). Ánh xạ $\alpha :x\mapsto (u(x), h(x))$ từ W vào $F\times C$ là riêng vì ánh xạ pr$_1\circ \alpha =u|W$ từ W vào F là riêng (TG, I, p. 73, mệnh đề 5, d)). Ánh xạ $\beta : (y, z)\mapsto (y+z, z)$ từ $F\times C$ vào $F\times C$ là một đồng phôi, và ánh xạ pr$_1$ từ $F\times C$ vào F là riêng (TG, I, p. 77, hệ quả 5). Vậy ánh xạ hợp thành pr$_1\circ \beta \circ \alpha$ từ W vào F là riêng (TG, I, p. 73, mệnh đề 5, a)). Nhưng ánh xạ này không gì khác hơn là hạn chế của $u+h$ trên W. Theo mệnh đề 1 của III, p. 71$,u+h$ là một cấu xạ ngặt, hạt nhân của nó có số chiều hữu hạn và ảnh của nó đóng.

#### Bổ đề 2 {#ts-iii-s5-lem-2 .statement tag=02TN}

Cho E và F là các không gian Fréchet và $u\in \mathscr{L}(E; F)$. Các điều kiện sau là tương đương:

(i) Đối hạt nhân của $u$ có số chiều hữu hạn ;

(ii) Ánh xạ $^tu: F'_c\rightarrow E'_c$ là một cấu xạ ngặt có ảnh đóng và hạt nhân của nó có số chiều hữu hạn.

(i) $=\Rightarrow$ (ii) : Giả sử đối hạt nhân của $u$ có số chiều hữu hạn. Khi đó ánh xạ $u$ là một cấu xạ ngặt (bổ đề 6 của III, p. 52). Theo mệnh đề 2 của EVT, IV, p. 27, ảnh của $^tu$ đóng trong $E'$ được trang bị tôpô yếu, và a fortiori trong $E'_c$. Hạt nhân của $^tu$ là trực giao của ảnh của $u($loc. cit.) ; do đó nó có số chiều hữu hạn. Sau cùng, $^tu$ là một cấu xạ ngặt từ $F'_c$ vào $E'_c$ theo định lý 1 của EVT, IV, p. 28.

(ii) $=\Rightarrow$ (i) : Giả sử $^tu: F'_c\rightarrow E'_c$ là một cấu xạ ngặt. Theo EVT, IV, p. 28, định lý 1, ảnh của $u$ là đóng. Hạt nhân của $^tu$ là trực giao của Im($u$) (EVT, IV, p. 27, mệnh đề 2) ; nếu hạt nhân này có số chiều hữu hạn thì ảnh của $u$ có đối chiều hữu hạn trong F.

#### Định lý 2 {#ts-iii-s5-thm-2 .statement tag=02TO}

Cho E và F là các không gian Fréchet, $u: E\rightarrow F$ là một ánh xạ tuyến tính liên tục có đối hạt nhân số chiều hữu hạn, và $h: E\rightarrow F$ là một ánh xạ tuyến tính compact. Ánh xạ tuyến tính $u+h$ là một cấu xạ ngặt, đối hạt nhân của nó có số chiều hữu hạn và ảnh của nó đóng.

Theo bổ đề 6 của III, p. 52, chỉ cần chứng minh rằng đối hạt nhân của $u+h$ có số chiều hữu hạn. Bây giờ, theo mệnh đề 9 của III, p. 9, ánh xạ $^th$ từ $F'_c$ vào $E'_c$ là compact ; định lý 2 suy ra từ định lý 1 và bổ đề 2.

### 3. Nhiễu xạ của các ánh xạ Fredholm

#### Định lý 3 {#ts-iii-s5-thm-3 .statement tag=02TP}

Cho E là một không gian lồi địa phương, F là một không gian lồi địa phương tách biệt, $u$ là một ánh xạ Fredholm từ E vào F và $h$ là một ánh xạ tuyến tính compact từ E vào F. Khi đó $u+h$ là một ánh xạ Fredholm, và ta có ind($u+h$) $=$ ind($u$).

Chúng tôi sẽ chứng minh định lý thành ba bước.

A) Giả sử rằng E và F là các không gian Banach. Mệnh đề 2 của III, p. 42 cho thấy rằng ánh xạ tuyến tính $u$ là một cấu xạ ngặt có ảnh đóng, mà hạt nhân và đối hạt nhân có số chiều hữu hạn. Vì E và F là các không gian Banach, các Định lý 1 và 2 của III, p. 73 suy ra rằng, với mọi $t\in [0,1]$, ánh xạ tuyến tính $u_t=u+th$ có cùng các tính chất ấy, và do đó là một ánh xạ Fredholm (III, p. 42, Mệnh đề 2). Ánh xạ $t\mapsto u_t$ từ $[0,1]$ vào tập hợp $\mathscr{F}(E; F)$ các ánh xạ Fredholm từ E vào F là liên tục. Theo Định lý 1 của III, p. 58, ánh xạ $t\mapsto$ ind($u_t$) là hằng địa phương. Vì khoảng $[0,1]$ của $\mathbf{R}$ là liên thông, ánh xạ này là hằng. Do đó ind($u$) $=$ ind($u+h$).

B) Giả sử E = F và $u= 1_E$. Theo Mệnh đề 5 của III, p. 5, tồn tại một không gian Banach G, một ánh xạ tuyến tính liên tục $p: E\rightarrow G$ và một ánh xạ tuyến tính compact $q: G\rightarrow E$ sao cho $h=q\circ p$. Tự đồng cấu $p\circ q$ của G là compact. Theo A), $1_G+p\circ q$ là một tự đồng cấu Fredholm của G có chỉ số không. Nhưng khi đó $1_E+h= 1_E+q\circ p$ là một tự đồng cấu Fredholm của E có chỉ số không (III, p. 49, Mệnh đề 10, f )).

C) Trường hợp tổng quát. Gọi $v$ là một nghịch đảo giả của $u$. Các tự đồng cấu $u\circ v$ và $(u+h)\circ v$ của F sai khác với $1_F$ bởi các ánh xạ tuyến tính compact. Theo B), chúng là các tự đồng cấu Fredholm của F có chỉ số không. Suy ra rằng $u+h$ là một tự đồng cấu Fredholm (III, p. 40, n$^o2$) có cùng chỉ số như $u($III, p. 43, n$^o3$, công thức (2)).

#### Hệ quả 1 {#ts-iii-s5-thm-3-cor-1 .statement tag=02TQ}

Cho E và F là các không gian lồi địa phương tách và $u\in \mathscr{L}(E; F)$. Để $u$ là một ánh xạ Fredholm, điều kiện cần và đủ là tồn tại một ánh xạ $v\in \mathscr{L}(F; E)$ sao cho các ánh xạ tuyến tính $1_E-v\circ u$ và $1_F-u\circ v$ là compact.

Vì một ánh xạ tuyến tính liên tục có hạng hữu hạn là compact, điều kiện đã nêu là cần thiết.

Gọi $v$ là một phần tử của $\mathscr{L}(F; E)$ sao cho các ánh xạ tuyến tính $1_E-v\circ u$ và $1_F-u\circ v$ là compact. Theo Định lý 3$,v\circ u$ và $u\circ v$ là các ánh xạ Fredholm. Gọi $p$ và $q$ là các nghịch đảo giả của $v\circ u$ và $u\circ v$ tương ứng. Đặt $w=p\circ v$ và $w'=v\circ q$. Với các ký hiệu của No.$^o2$ ở III, p. 40, ta có $w\circ u\equiv 1_E$ và $u\circ w'\equiv 1_F$, do đó $w\equiv w\circ u\circ w'\equiv w'$. Suy ra rằng $w$ là một nghịch đảo giả của $u$.

#### Hệ quả 2 {#ts-iii-s5-thm-3-cor-2 .statement tag=02TR}

Cho E và F là các không gian lồi địa phương tách và $u\in \mathscr{L}(E; F)$. Các điều kiện sau là tương đương:

(i) Ánh xạ $u$ là một ánh xạ Fredholm có chỉ số không;

(ii) Tồn tại một đẳng cấu $v$ từ E lên F sao cho $u-v$ có hạng hữu hạn ;

(iii) Tồn tại một đẳng cấu $v$ từ E lên F sao cho $u-v$ là compact.

(i) $=\Rightarrow$ (ii) : Giả sử rằng $u$ là một ánh xạ Fredholm có chỉ số không. Tồn tại các phân tích thành các tổng trực tiếp tôpô $E = E_1\oplus E_2$ và $F = F_1\oplus F_2$ với $E_2$ và $F_2$ hữu hạn chiều sao cho $u$ triệt tiêu trên $E_2$ và xác định bởi hạn chế một đẳng cấu $u_1$ từ $E_1$ lên $F_1($III, p. 42, mệnh đề 2). Nếu ind($u$) $= 0$, thì các chiều của $E_2$ và $F_2$ bằng nhau và tồn tại một đẳng cấu $v$ từ E lên F mở rộng $u_1$. Hạt nhân của $u-v$ chứa $E_1$, do đó $u-v$ có hạng hữu hạn.

Ta có (ii) $=\Rightarrow$ (iii) vì mọi ánh xạ tuyến tính liên tục có hạng hữu hạn từ E vào F đều compact, và (iii) $=\Rightarrow$ (i) theo định lý 3.

### 4. Nhiễu của các tự đồng cấu Riesz

Cho E là một không gian Banach. Nhắc lại (xem III, p. 5, mệnh đề 3) rằng tập hợp $\mathscr{L}^c(E)$ các tự đồng cấu compact của E là một iđêan hai phía đóng của đại số Banach $\mathscr{L}(E)$. Đại số Banach thương được gọi là đại số Calkin của E; nó được ký hiệu bởi $\mathscr{C}$alk(E). Ta ký hiệu bởi $\pi$ đồng cấu chính tắc từ $\mathscr{L}(E)$ lên $\mathscr{C}$alk(E). Theo Hệ quả 1 của III, p. 74, một tự đồng cấu $u$ của E là một tự đồng cấu Fredholm khi và chỉ khi $\pi (u)$ khả nghịch trong đại số $\mathscr{C}$alk(E).

#### Mệnh đề 2 {#ts-iii-s5-prop-2 .statement tag=02TS}

Cho $u\in \mathscr{L}(E)$ sao cho $\|1_E-\pi (u)\|<1$ trong đại số $\mathscr{C}$alk(E). Khi đó $u$ là một tự đồng cấu Riesz của E.

Cho $r\geqslant 1$ là một số nguyên sao cho $\|1_E-\pi (u)\|^r<\frac{1}{2}$. Cho $P\in \mathbf{C}[X]$ là đa thức $\frac{1-(1-X)^r}{X}$. Đặt $v= 1_E-(1_E-u)^r$. Khi đó ta có $v=uP(u)$ và $\|1_E-\pi (v)\|<\frac{1}{2}$. Vì các tự đồng cấu $u$ và $P(u)$ của E giao hoán, chỉ cần chứng minh rằng $v$ là một tự đồng cấu Riesz của E (III, p. 49, mệnh đề 9).

Vì $\|1_E-\pi (v)\|<1/2$, nên theo định nghĩa của chuẩn thương trong không gian $\mathscr{C}$alk(E), tồn tại một tự đồng cấu compact $h$ của E và một tự đồng cấu $w$ của E sao cho $v= 1_E+h+w$ và $\|w\|<\frac{1}{2}$. Theo Hệ quả 1 của I, p. 22, phần tử $1_E+w$ là một tự đẳng cấu của E. Vì $h$ compact, $v= (1_E+w) +h$ là một tự đồng cấu Fredholm của E có chỉ số 0 (Hệ quả 2 của III, p. 74). Với mọi số nguyên $n\geqslant 0$, ký hiệu bởi $N_n$ hạt nhân của $v^n$. Để chứng minh rằng $v$ là một tự đồng cấu Riesz của E, chỉ cần chứng minh rằng tồn tại một số nguyên $n\geqslant 0$ sao cho $N_n= N_{n+1}($III, p. 46, định nghĩa 2 and III, p. 46, nhận xét).

Lập luận bằng phản chứng bằng cách giả sử dãy $(N_n)$ tăng ngặt. Với mọi $n\in \mathbf{N}$, gọi $p_n$ là ánh xạ chính tắc từ E lên không gian chuẩn $E/N_n$. Gọi $c$ là một số thực sao cho $2\|w\|< c <1$. Gọi $n\in \mathbf{N}$. Vì $N_{n+1}$ khác $N_n$, tồn tại một phần tử $x_n\in N_{n+1}$ sao cho $\|p_n(x_n)\|=c$ và sao cho $\|x_n\|<1$ (thật vậy, tồn tại $y\in N_{n+1}/N_n$ có chuẩn $c$ nên, với mọi $\varepsilon  >0$, tồn tại $x_n\in N_{n+1}$ sao cho $p_n(x_n) =y$ và $\|x_n\|\leqslant c+\varepsilon$ ).

Gọi $m,n$ là hai số nguyên sao cho $m > n\geqslant 0$. Ta có

$$
\|h(x_m)-h(x_n)\|=\|v(x_m-x_n)-(1_E+w)(x_m-x_n)\|
$$

$$
\geqslant \|(v-1_E)(x_m-x_n)\| - \|w(x_m-x_n)\|
$$

$$
\geqslant \|(v-1_E)(x_m-x_n)\| -2\|w\| \tag{1}
$$

vì $\|x_m\|\leqslant 1$ và $\|x_n\|\leqslant 1$. Hơn nữa, chú ý rằng

$$
(v-1_E)(x_m-x_n) =v(x_m-x_n) +x_n-x_m
$$

Nhưng vì $n < m$ và $v(N_{m+1})\subset N_m$, ta có $v(x_m-x_n) +x_n\in N_m$, do đó

$$
\|v(x_m-x_n) +x_n-x_m\|\geqslant \|p_m(x_m)\|=c
$$

Vậy bất đẳng thức (1) cho cận dưới

$$
\|h(x_m)-h(x_n)\|\geqslant c-2\|w\|>0 \tag{2}
$$

Do đó dãy $(h(x_m))_{m\in\mathbf{N}}$ không có giá trị bám nào trong E, điều này mâu thuẫn với việc ảnh của quả cầu đơn vị của E bởi $h$ là tương đối compắc, vì $h$ là compắc (nhận xét 1 của III, p. 2).

#### Hệ quả 1 {#ts-iii-s5-prop-2-cor-1 .statement tag=02TT}

Cho E là một không gian lồi địa phương tách và $u\in \mathscr{L}(E)$. Để $u$ là một tự đồng cấu Riesz, điều kiện cần và đủ là tồn tại một phần tử $v$ của $\mathscr{L}(E)$ giao hoán với $u$ và sao cho $1_E-u\circ v$ là compắc.

Vì mọi ánh xạ tuyến tính liên tục hạng hữu hạn đều compắc, điều kiện là cần (III, p. 47, prop. 6 d)). Ta hãy chứng minh rằng nó là đủ. Gọi $v$ là một phần tử của $\mathscr{L}(E)$ giao hoán với $u$ và sao cho tự đồng cấu $h= 1_E-u\circ v$ của E là compắc. Tồn tại một không gian Banach G, một ánh xạ tuyến tính liên tục $p: E\rightarrow G$ và một ánh xạ tuyến tính compắc $q: G\rightarrow E$ sao cho $h=q\circ p($III, p. 5, prop. 5). Tự đồng cấu $p\circ q$ của G là compắc. Theo mệnh đề 2, ánh xạ tuyến tính $1_G-p\circ q$ là một tự đồng cấu Riesz của G. Nhưng khi đó $u\circ v= 1_E-q\circ p$ là một tự đồng cấu Riesz của E (III, p. 49, prop. 10, g)). Vì $u$ và $v$ giao hoán, $u$ là một tự đồng cấu Riesz của E (III, p. 49, prop. 9).

#### Hệ quả 2 {#ts-iii-s5-prop-2-cor-2 .statement tag=02TU}

Cho E là một không gian lồi địa phương tách, $u$ là một tự đồng cấu Riesz của E và $h\in \mathscr{L}(E)$ là một ánh xạ tuyến tính compắc. Nếu $u$ và $h$ giao hoán, thì $u+h$ là một tự đồng cấu Riesz của E.

Cho $v$ là nghịch đảo giả chính tắc của $u$. Nó giao hoán với $u$ và với $h($III, p. 47, mệnh đề 6), nên cũng giao hoán với $u+h$. Tự đồng cấu $1_E-(u+h)\circ v$ của E là tổng của ánh xạ tuyến tính liên tục hạng hữu hạn $1_E-u\circ v$ và ánh xạ tuyến tính compact $-h\circ v$, nên là compact. Suy ra $u+h$ là một tự đồng cấu Riesz của E (hệ quả 1).

#### Mệnh đề 3 {#ts-iii-s5-prop-3 .statement tag=02TV}

Cho E là một không gian Banach. Cho $u$ là một tự đồng cấu của E, và cho A là hoán tập của nó trong $\mathscr{L}(E)$. Bao đóng B của $\pi (A)$ trong đại số $\mathscr{C}$alk(E) là một đại số Banach. Để $u$ là một tự đồng cấu Riesz của E, điều kiện cần và đủ là $\pi (u)$ khả nghịch trong B.

Vì $\pi (A)$ là một đại số con có đơn vị của $\mathscr{C}$alk(E), bao đóng B của nó là một đại số Banach. Nếu $u$ là một tự đồng cấu Riesz của E, phần tử $\pi (u)$ có một nghịch đảo trong $\pi (A)$ (hệ quả 1), nên trong B. Ngược lại, giả sử rằng $\pi (u)$ có một nghịch đảo $s$ trong B. Theo định nghĩa của B, tồn tại một phần tử $v$ của A sao cho

$$
\|s-\pi (v)\|<\frac{1}{\|\pi(u)\|}
$$

do đó $\|1_E-\pi (u\circ v)\|<1$. Theo mệnh đề 2, ánh xạ tuyến tính $u\circ v$ là một tự đồng cấu Riesz của E. Điều này cũng đúng với $u$ vì $u$ và $v$ giao hoán (III, p. 49, mệnh đề 9).

### 5. Lý thuyết của Frédéric Riesz

Cho E là một không gian lồi địa phương tách và cho $h$ là một tự đồng cấu compact của E. Cho $\lambda \in K$. Tự đồng cấu $\lambda h$ là compact, nên $1_E-\lambda h$ là một tự đồng cấu Riesz của E (hệ quả 2 của mệnh đề 2 của III, p. 75); ký hiệu bởi $N_{\lambda}$ và $I_{\lambda}$ không gian nhân và không gian đồng nhân của nó. Theo mệnh đề 6 của III, p. 47, các tính chất sau đúng:

(i) Các không gian con vectơ $I_{\lambda}$ và $N_{\lambda}$ của E là đóng và ổn định dưới $h$;

(ii) Không gian lồi địa phương E là tổng trực tiếp tôpô của $I_{\lambda}$ và $N_{\lambda}$;

(iii) Ánh xạ $1_E-\lambda h$ xác định bằng hạn chế một tự đẳng cấu của $I_{\lambda}$;

(iv) Không gian vectơ $N_{\lambda}$ là hữu hạn chiều, và tồn tại một số nguyên $n_{\lambda}\geqslant 0$ sao cho $(1_E-\lambda h)^{n_{\lambda}}(x) = 0$ với mọi $x\in N_{\lambda}$.

Các tính chất này xác định các không gian $I_{\lambda}$ và $N_{\lambda}$ một cách duy nhất (A, VIII, p. 26, nhận xét 2).

#### Bổ đề 3 {#ts-iii-s5-lem-3 .statement tag=02TW}

Cho X là một không gian tôpô mà tôpô của nó có một cơ sở đếm được. Mọi tập con rời rạc của X đều đếm được.

Cho $\mathscr{B}$ là một cơ sở đếm được của tôpô của X và cho D là một tập con rời rạc của X. Với mỗi phần tử $x$ của D, tồn tại một phần tử $B_x$ của $\mathscr{B}$ sao cho $B_x\cap D =\{x\}$. Ánh xạ từ D vào $\mathscr{B}$ xác định bởi $x\mapsto B_x$ là đơn ánh, do đó có bổ đề.

#### Định lý 4 {#ts-iii-s5-thm-4 .statement tag=02TX}

Cho E là một không gian lồi địa phương tách và cho $h$ là một tự đồng cấu compact của E. Tập Σ các $\lambda \in K$ sao cho $1_E-\lambda h$ không phải là một tự đẳng cấu của E là một tập con đếm được, đóng và rời rạc của trường K.

Tập hợp Σ cũng là tập hợp các $\lambda \in K$ sao cho $1_E-\lambda h$ không đơn ánh và là tập hợp các $\lambda \in K$ sao cho $1_E-\lambda h$ không toàn ánh.

Tồn tại một không gian Banach G, một ánh xạ tuyến tính liên tục $p: E\rightarrow G$ và một ánh xạ tuyến tính compact $q: G\rightarrow E$ sao cho $h=q\circ p($III, p. 5, mệnh đề 5). Tự đồng cấu $h'=p\circ q$ của G là compact, và để $1_E-\lambda h$ là một tự đẳng cấu của E thì điều kiện cần và đủ là $1_G-\lambda h'$ là một tự đẳng cấu của G (mệnh đề 10 của III, p. 49, e)). Do đó, với chúng ta chỉ cần chứng minh định lý trong trường hợp E là một không gian Banach, và từ nay ta giả thiết như vậy.

Cho $\lambda \in K$. Vì chỉ số của một tự đồng cấu Riesz bằng không, nên việc nói rằng ánh xạ $1_E-\lambda h$ là một tự đẳng cấu của E, hay nó đơn ánh, hay lại nữa nó toàn ánh, đều tương đương nhau.

Tập hợp Σ là đóng trong K vì tập hợp các tự đẳng cấu của E là mở trong $\mathscr{L}(E)$. Cho $\lambda$ là một phần tử của Σ. Ta có $\lambda \not = 0$. Ký hiệu N là không gian lũy linh của $h$ và I là đối không gian lũy linh của nó, và ký hiệu $h_I$ và $h_N$ là các tự đồng cấu của I và N mà $h$ xác định khi chuyển qua các không gian con này. Khi đó $1_I-\lambda h_I$ là một tự đẳng cấu của I, và tồn tại một lân cận U của $\lambda$ trong K sao cho $1_I-\mu h_I$ là một tự đẳng cấu của I với mọi $\mu\in U$. Tự đồng cấu $1_N-\lambda h_N$ của N là lũy linh; với mọi $\mu\not =\lambda$, ta có

$$
1_N-\mu h_N=\frac{\lambda-\mu}{\lambda}(1_N+\frac{\mu}{\lambda-\mu}(1_N-\lambda h_N))
$$

do đó $1_N-\mu h_N$ là một tự đẳng cấu của N. Vì thế, tập hợp $U\cap \Sigma$ được rút gọn còn phần tử duy nhất $\lambda$ và tập hợp Σ là rời rạc. Nó là đếm được theo bổ đề 3.

### 6. Phương án Fredholm

#### Mệnh đề 4 (Phương án Fredholm) {#ts-iii-s5-prop-4 .statement tag=02TY}

Cho E là một không gian Banach và cho $h$ là một tự đồng cấu compact của E. Cho $\lambda$ là một phần tử của K $-\{0\}$. Gọi F là hạt nhân của $1_E-\lambda h$ và G là hạt nhân của $1_{E'}-\lambda^th$.

a) Các không gian F và G có cùng số chiều hữu hạn $n\geqslant 0$;

b) Với $y\in E$, tồn tại $x\in E$ sao cho $x-\lambda h(x) =y$ khi và chỉ khi $\langle y, \ell \rangle = 0$ với mọi $\ell \in G$;

c) Với $\ell \in E'$, tồn tại $f\in E'$ sao cho $f-\lambda^th(f) =\ell$ khi và chỉ khi $\langle x, f\rangle = 0$ với mọi $x\in F$.

Đặc biệt, chỉ một và chỉ một trong các điều kiện sau là đúng:

(i) Không gian F khác không ;

(ii) Với mọi $y\in E$, tồn tại $x\in E$ sao cho $x-\lambda h(x) =y$.

Thay thế $h$ bởi $\lambda h$, ta rút gọn về trường hợp $\lambda = 1$.

Tự đồng cấu $^th$ là compact theo hệ quả 1 của III, p. 9. Do đó các tự đồng cấu $w= 1_E-h$ của E và $w'= 1_{E'}-^th$ của $E'$ là các tự đồng cấu Riesz (hệ quả 2 của mệnh đề 2 của III, p. 75). Đặc biệt, các hạt nhân F và G của chúng có số chiều hữu hạn. Vì $w'=^tw$ và chỉ số của $w$ bằng không, nên chiều của F bằng chiều của G theo công thức (3) của III, p. 43.

Với một phần tử $y$ của E, phương trình $x-h(x) =y$ có một nghiệm $x\in E$ khi và chỉ khi $x$ thuộc ảnh của $w$. Vì đối ngẫu của đối hạt nhân của $w$ được đồng nhất với hạt nhân G của Ker($^tw$) (EVT, IV, p. 27, mệnh đề 2), điều này xảy ra khi và chỉ khi $\langle y, \ell \rangle = 0$ với mọi $\ell \in G$.

Với một phần tử $\ell$ của $E'$, phương trình $f-^th(f) =\ell$ có một nghiệm $f\in E'$ khi và chỉ khi $f$ thuộc ảnh của $w'$. Vì ảnh của $^tw$ là trực giao của hạt nhân F của $w$ (EVT, IV, p. 27, mệnh đề 2) điều này xảy ra khi và chỉ khi $\langle x, f\rangle = 0$ với mọi $x\in F$.

#### Ví dụ {#ts-iii-s5-n6-exa-1 .statement tag=02TZ}

Cho X là một không gian compact, $\mu$ một độ đo trên X, thực hoặc phức tùy theo K bằng $\mathbf{R}$ hay $\mathbf{C}$, và $N : X\times X\rightarrow K$ một hàm liên tục.

Ký hiệu E là không gian Banach $\mathscr{C}(X; K)$. Giả sử đã cho một hàm $a\in E$ và $\lambda \in K-\{0\}$. Ta khảo sát bài toán về sự tồn tại và tính duy nhất của các nghiệm $f\in E$ của phương trình tích phân

$$
f(x)-\lambda \int_XN(x, y)f(y)d\mu(y) =a(x)(x\in X) \tag{3}
$$

Để làm việc đó, đưa vào tập hợp $F_{\lambda}$ các nghiệm $f\in E$ của phương trình thuần nhất liên kết

$$
f(x)-\lambda \int_XN(x, y)f(y)d\mu(y) = 0(x\in X) \tag{4}
$$

và tập hợp $G_{\lambda}$ các nghiệm $g\in E$ của phương trình thuần nhất chuyển vị của (4), nghĩa là

$$
g(y)-\lambda \int_XN(x, y)g(x)d\mu(x) = 0(y\in X) \tag{5}
$$

Nếu không rỗng, tập hợp các nghiệm của (3) là một không gian con affine của E có phương là $F_{\lambda}$.

Với $f\in E$ và $x\in X$, đặt

$$
h(f)(x) =\int_XN(x, y)f(y)d\mu(y)
$$

ánh xạ $f\mapsto h(f)$ được định nghĩa như vậy là một tự đồng cấu compact của không gian Banach E (hệ quả của mệnh đề 2 của III, p. 26). Đối ngẫu $E'$ của E gồm các độ đo trên X, thực hoặc phức tùy theo K bằng $\mathbf{R}$ hay $\mathbf{C}$ (INT, III, p. 47, § 1, n$^o3$, định nghĩa 2). Chuyển vị $^th$ của $h$ là tự đồng cấu của $E'$ được đặc trưng bởi quan hệ $\langle f,^th(m)\rangle =\langle h(f), m\rangle$ với $f\in E$ và $m\in E'$, nghĩa là

$$
\int_Xf(x)d(^th(m))(x) =\int_Xh(f)(x)dm(x)
$$

$$
=\int_X(\int_XN(x, y)f(y)d\mu(y))dm(x)
$$

$$
=\int_X(\int_XN(x, y)dm(x))f(y)d\mu(y) \tag{6}
$$

với $m\in E'$ và $f\in E$ (INT, III, p. 84, § 4, n$^o1$, định lý 2).

#### Bổ đề 4 {#ts-iii-s5-lem-4 .statement tag=02U0}

Ánh xạ tuyến tính từ $G_{\lambda}$ vào $E'$ được xác định bởi $g\mapsto g\cdot \mu$ là đơn ánh, và ảnh của nó là hạt nhân của $1_{E'}-\lambda^th$.

Nếu $g\in G_{\lambda}$ thỏa mãn $g\cdot \mu= 0$, thì công thức (5) suy ra $g= 0$, do đó ánh xạ $g\mapsto g\cdot \mu$ là đơn ánh.

Cho $m\in E'$ là một độ đo thuộc hạt nhân của $1_{E'}-\lambda^th$. Theo quan hệ (6), ta có

$$
\int_Xf(x)dm(x) =\lambda \int_X(\int_XN(x, y)dm(x))f(y)d\mu(y) \tag{7}
$$

với mọi hàm liên tục $f: X\rightarrow K$. Vậy độ đo $m$ bằng độ đo $g\cdot \mu$, trong đó $g$ là hàm liên tục từ X vào K được xác định bởi

$$
g(y) =\lambda \int_XN(x, y)dm(x) \tag{8}
$$

với mọi $y\in X$. Khi đó công thức (8) suy ra rằng hàm $g$ thuộc $G_{\lambda}$.

Ngược lại, cho $g: X\rightarrow K$ là một hàm liên tục thuộc $G_{\lambda}$ và đặt $m=g\cdot \mu$. Với mọi hàm liên tục $f: X\rightarrow K$, do đó ta có

$$
\int_Xf(y)dm(y) =\int_Xg(y)f(y)d\mu(y)
$$

$$
=\lambda \int_X(\int_XN(x, y)g(x)d\mu(x))f(y)d\mu(y)
$$

$$
=\lambda \int_Xf(x)dm(x)
$$

sao cho $^th(m) =\lambda m$. Điều này chứng minh Bổ đề 4.

Bằng cách áp dụng Mệnh đề 4 và Định lý 4 của III, p. 78. cho tự đồng cấu $h$, khi đó ta thu được các mệnh đề sau.

#### Định lý 5 {#ts-iii-s5-thm-5 .statement tag=02U1}

Cho $\lambda \in K$.

a) Các tập hợp $F_{\lambda}$ và $G_{\lambda}$ là các không gian con vectơ hữu hạn chiều của $\mathscr{C}(X; K)$ và các chiều của chúng bằng nhau ;

b) Để phương trình (3) có ít nhất một nghiệm $f\in \mathscr{C}(X,K)$, điều kiện cần và đủ là ta có $\int_Xa(x)g(x)d\mu(x) = 0$ với mọi hàm $g\in G_{\lambda}$. Khi đó tập hợp các nghiệm của (3) là một không gian con afin của $\mathscr{C}(X; K)$ với phương là $F_{\lambda}$;

c) Một trong các điều kiện sau đây, loại trừ lẫn nhau, được thỏa mãn :

(i) Với mọi hàm $a\in \mathscr{C}(X; K)$, tồn tại một nghiệm duy nhất

$f\in \mathscr{C}(X; K)$ của phương trình tích phân (3) ;

(ii) Phương trình thuần nhất (4) có một nghiệm khác không

$$
f\in \mathscr{C}(X; K)
$$

#### Hệ quả {#ts-iii-s5-n6-cor-1 .statement tag=02U2}

Tập hợp các $\lambda \in K$ sao cho không gian $F_{\lambda}$ khác không là một tập con đếm được, đóng và rời rạc của K.

## BÀI TẬP {#ts-iii-s5-exercises}

Trong các bài tập sau, khi E là một không gian Banach, người ta ký hiệu bởi $\mathscr{C}$alk(E) đại số Calkin $\mathscr{L}(E)/\mathscr{L}^c(E)$. Người ta ký hiệu bởi $\pi$ phép chiếu chính tắc của $\mathscr{L}(E)$ lên $\mathscr{C}$alk(E).

Nếu E là một không gian Hilbert phức, $\mathscr{C}$alk(E) được trang bị phép đối hợp suy ra từ phép đối hợp của $\mathscr{L}(E)$ bằng cách chuyển qua thương.

Xem [các bài tập của § 5](exercises/s5/).
