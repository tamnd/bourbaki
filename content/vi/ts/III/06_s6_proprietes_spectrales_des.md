---
book: ts
book_title: Théories spectrales
chapter: III
chapter_title: APPLICATIONS LINÉAIRES COMPACTES ET PERTURBATIONS
section: 6
section_title: Propriétés spectrales des endomorphismes des espaces de Banach
lang: vi
source: ts-iii-v-fr
book_pages: TS III.82-TS III.101, TS III.128-TS III.142
pdf_pages: 0096-0115, 0142-0156
extraction: native
subsections:
    - "no": 1
      title: Points isolés et points sensibles du spectre
      page: 82
      pdf_page: 96
    - "no": 2
      title: Une partition du spectre
      page: 85
      pdf_page: 99
    - "no": 3
      title: Spectre du transposé d’un endomorphisme
      page: 88
      pdf_page: 102
    - "no": 4
      title: Perturbation par un opérateur compact
      page: 89
      pdf_page: 103
    - "no": 5
      title: Spectre d’un opérateur compact
      page: 89
      pdf_page: 103
    - "no": 6
      title: Cas des espaces hilbertiens
      page: 92
      pdf_page: 106
    - "no": 7
      title: Le théorème de Krein–Rutman
      page: 93
      pdf_page: 107
statements: 36
exercises: 30
content_sha256: 23cb2155bf34ce03b002524186cf089c87366bbdb801c4ef808fb8241de6c55e
translated_from: content/en-mt/ts/III/06_s6_proprietes_spectrales_des.md
source_lang: en-mt
translation_method: machine
source_content_sha256: ccef81be0b51793e31aeb322d53ffa1bccb3187f62d1475d741e2c9c623ce0f4
translation_model: gpt-5.4
translation_run: translate-vi-a9d4f7c3
glossary_version: 34
glossary_terms_sha256: 36e2bacb3d5071358188aa93879d6278dfabed20cfa1dfa7d9bbf0523c63aa72
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 6. TÍNH CHẤT PHỔ CỦA CÁC TỰ ĐỒNG CẤU CỦA KHÔNG GIAN BANACH

Trừ khi có phát biểu ngược lại, các không gian vectơ được xét trong đoạn này là các không gian vectơ trên $\mathbf{C}$. Phổ của một tự đồng cấu của một không gian khả chuẩn đầy đủ E là phổ tương đối với đại số có đơn vị $\mathscr{L}(E) ($xem n$^o7$ của I, p. 127).

### 1. Các điểm cô lập và các điểm nhạy của phổ

Cho E là một không gian khả chuẩn đầy đủ và cho $u$ là một tự đồng cấu của E. Cho $\lambda$ là một điểm cô lập của phổ của $u$. Ta nhắc lại rằng $e_{\lambda}(u)$ ký hiệu phép chiếu phổ gắn với $u$ và với tập đóng và mở $\{\lambda \}$ của phổ của $u$ (n$^o3$ của I, p. 131). Tự đồng cấu $u-\lambda 1_E$ cảm sinh một tự đẳng cấu của Ker($e_{\lambda}(u)$) và một tự đồng cấu giả lũy linh của Im($e_{\lambda}(u)$) $($dẫn chiếu trên$)$.

#### Định nghĩa 1 {#ts-iii-s6-def-1 .statement tag=02UE}

Người ta nói rằng $\lambda$ có bội số phổ hữu hạn đối với $u$ nếu phép chiếu phổ $e_{\lambda}(u)$ có hạng hữu hạn; trong trường hợp đó, số nguyên $m_{\lambda}(u) =$ dim(Im($e_{\lambda}(u)$)) được gọi là bội số phổ của $\lambda$ đối với $u$.

#### Định nghĩa 2 {#ts-iii-s6-def-2 .statement tag=02UF}

Các điểm cô lập của Sp($u$) có bội số phổ hữu hạn được gọi là các điểm nhạy của phổ của $u$. Tập các điểm nhạy của Sp($u$) được gọi là phổ nhạy của $u$ và được ký hiệu bởi Sp$_s(u)$.[^1] Tập bù Sp($u$) - Sp$_s(u)$ được gọi là phổ cốt yếu của $u$ và được ký hiệu bởi Sp$_e(u)$.

Vì tập Sp$_s(u)$ gồm các điểm cô lập của Sp($u$), nó mở trong Sp($u$), rời rạc, và đếm được (III, p. 78, bổ đề 3); nó cũng bị chặn. Tập Sp$_e(u)$ đóng trong Sp($u$), do đó compắc.

Theo Mệnh đề 14 của III, p. 54, các điểm nhạy của phổ của $u$ là các số phức $\lambda$ sao cho $u-\lambda 1_E$ là một tự đồng cấu Riesz của E mà không phải là một tự đẳng cấu của E.

Với mọi số phức $\lambda$, ký hiệu $N_{\lambda}(u)$ và $I_{\lambda}(u)$ lần lượt là không gian nil và không gian conil của tự đồng cấu $u-\lambda 1_E$ của E. Vì E là một không gian Fréchet, $u-\lambda 1_E$ là một tự đồng cấu Riesz khi và chỉ khi $N_{\lambda}(u)$ có số chiều hữu hạn và $I_{\lambda}(u)$ có đối chiều hữu hạn (mệnh đề 13 của III, p. 53); khi điều này xảy ra, $u-\lambda 1_E$ khả nghịch khi và chỉ khi $N_{\lambda}(u)$ thu về 0 (III, p. 47, mệnh đề 6). Do đó, các điểm nhạy của phổ của $u$ là các số phức $\lambda$ sao cho $N_{\lambda}(u)$ có chiều hữu hạn khác không và $I_{\lambda}(u)$ có đối chiều hữu hạn trong E (III, p. 54, mệnh đề 14). Khi đó bội số phổ $m_{\lambda}(u)$ của $\lambda$ là chiều của $N_{\lambda}(u)$, tự đồng cấu $u-\lambda 1_E$ xác định bằng cách hạn chế một tự đẳng cấu của $I_{\lambda}(u)$ và một tự đồng cấu lũy linh của $N_{\lambda}(u)$. Vì $N_{\lambda}(u)$ không thu về 0, suy ra $\lambda$ là một trị riêng của $u$. Số nguyên nhỏ nhất $n\geqslant 1$ sao cho Ker(($u-\lambda 1_E$)$^n$) bằng $N_{\lambda}(u)$ là cấp của cực của hàm giải thức của $u$ tại điểm $\lambda$ (No.$^o3$ của I, p. 131), bị chặn trên bởi $m_{\lambda}(u)$.

Đặc biệt, do đó ta đã chứng minh:

#### Mệnh đề 1 {#ts-iii-s6-prop-1 .statement tag=02UG}

Các điểm nhạy của phổ của $u$ là các trị riêng có bội số phổ hữu hạn.

Phổ cốt yếu của $u$ gồm các số phức $\lambda$ sao cho $u-\lambda 1_E$ không phải là một tự đồng cấu Riesz của E. Đặc biệt, nếu $u$ compact, thì mọi $\lambda \in$ Sp($u$)$-\{0\}$ đều là một điểm nhạy của phổ (hệ quả 2 của III, p. 77).

#### Mệnh đề 2 {#ts-iii-s6-prop-2 .statement tag=02UH}

Cho E là một không gian khả chuẩn đầy đủ và $u$ một tự đồng cấu của E. Cho H là một tập con hữu hạn của Sp$_s(u)$. Tập H vừa mở vừa đóng trong Sp($u$). Phép chiếu phổ $e_H(u)$ có hạng hữu hạn, có ảnh là $\sum_{\lambda\in H}N_{\lambda}(u)$ và hạt nhân là $\bigcap_{\lambda\in H}I_{\lambda}(u)$.

Điều này suy ra từ No.$^o3$ của I, p. 131 vì, với mọi $\lambda \in$ Sp$_s(u)$, các không gian con $N_{\lambda}(u)$ và $I_{\lambda}(u)$ lần lượt là ảnh và hạt nhân của phép chiếu phổ $e_{\lambda}(u)$.

#### Hệ quả 1 {#ts-iii-s6-prop-2-cor-1 .statement tag=02UI}

Cho V là một lân cận của Sp$_e(u)$.

a) Tồn tại một phân tích của E thành một tổng trực tiếp tôpô $F\oplus$ G sao cho F có số chiều hữu hạn, sao cho F và G ổn định dưới mọi tự đồng cấu giao hoán với $u$, và sao cho phổ của tự đồng cấu của G cảm sinh bởi $u$ được chứa trong V;

b) Giả sử V khác rỗng. Tồn tại một phần tử $v$ của đối giao hoán tử kép của $u$ trong $\mathscr{L}(E)$ mà phổ được chứa trong V và sao cho $v-u$ có hạng hữu hạn.

Cho H = Sp($u$)$\cap (\mathbf{C}-\mathring{V})$. Tập hợp H được chứa trong Sp$_s(u)$, do đó là rời rạc; vì nó đóng trong không gian compắc Sp($u$), nên nó hữu hạn. Có thể lấy F và G lần lượt là ảnh và hạt nhân của phép chiếu phổ $e_H(u)$ (Mệnh đề 2).

Giả sử V khác rỗng. Lấy $\mu\in V$ và ký hiệu $v$ là tự đồng cấu của E trùng với phép vị tự tỉ số $\mu$ trên F và với $u$ trên G. Phổ của nó được chứa trong $\{\mu\} \cup$ (Sp($u$) - H), do đó trong V, và $v-u$ có hạng hữu hạn vì F là hữu hạn chiều.

Với mọi tập con compắc S của $\mathbf{C}$, ký hiệu $\mathscr{O}(S)$ là đại số các mầm hàm chỉnh hình trên một lân cận của S nhận giá trị trong $\mathbf{C}$ (I, p. 49, §4, No. $1$).

#### Hệ quả 2 {#ts-iii-s6-prop-2-cor-2 .statement tag=02UJ}

Cho $f\in \mathscr{O}$(Sp($u$)) và cho $\mu$ là một số phức. Gọi H là tập hợp các $\lambda \in$ Sp($u$) sao cho $f(\lambda ) =\mu$. Khi đó $\mu$ là một điểm của phổ rời rạc của $f(u)$ khi và chỉ khi H là hữu hạn, khác rỗng, và được chứa trong phổ rời rạc của $u$. Trong các điều kiện ấy, phép chiếu phổ $e_\mu(f(u))$ bằng phép chiếu $e_H(u)$ liên kết với $u$ và H. Ta có

$$
N_\mu(f(u)) =\bigoplus_{\lambda\in H}N_{\lambda}(u),I_\mu(f(u)) =\bigcap_{\lambda\in H}I_{\lambda}(u)
$$

và bội số phổ của $\mu$ đối với $f(u)$ là tổng các bội số phổ của các phần tử của H, nghĩa là

$$
m_\mu(f(u)) =\sum_{\lambda\in H}m_{\lambda}(u)
$$

Số phức $\mu$ thuộc $f$(Sp($u$)), và do đó thuộc phổ của $f(u)$ (Mệnh đề 8 của I, p. 75), khi và chỉ khi H khác rỗng. Khi đó ta có $e_\mu(f(u)) =e_H(u)$ (No. $1$ của I, p. 127). Các khẳng định khác suy ra từ điều này nhờ Mệnh đề 2.

#### Ví dụ 1 {#ts-iii-s6-n1-exa-1 .statement tag=02UK}

Cho E là một không gian vectơ hữu hạn chiều và $u$ là một tự đồng cấu của E. Phổ của $u$ là hữu hạn và trùng với Sp$_s(u)$. Các phần tử của nó là các nghiệm của đa thức đặc trưng $\chi_u$ của $u$; chúng là các giá trị riêng của $u$. Bội số phổ $m_{\lambda}(u)$ của một phần tử $\lambda \in$ Sp($u$) là bội số của $\lambda$ như một nghiệm của đa thức $\chi_u$ (A, VII, p. 36, hệ quả). Theo Hệ quả 2 ở trên, ta có

$$
\chi_{f(u)}(T) =\prod_{\lambda\in Sp(u)}(T-f(\lambda ))^{m_{\lambda}}
$$

với mọi $f\in \mathscr{O}$(Sp($u$)). Điều này tổng quát hóa Mệnh đề 10 của A, VII, p. 36.

#### Ví dụ 2 {#ts-iii-s6-n1-exa-2 .statement tag=02UL}

Cho X là một tập con compắc của $\mathbf{C}$, và $\mathscr{C}(X)$ là không gian Banach các hàm liên tục nhận giá trị phức trên X. Ký hiệu $u$ là tự đồng cấu của $\mathscr{C}(X)$ mà với $f\in \mathscr{C}(X)$ gán hàm $z\mapsto zf(z)$ của $\mathscr{C}(X)$. Phổ của $u$ bằng X, các điểm của phổ rời rạc của nó là các điểm cô lập của X, và bội số phổ của chúng đều bằng 1.

### 2. Một phân hoạch của phổ

Ký hiệu $\overline{\mathbf{Z}}$ là tập con $\mathbf{Z}\cup  \{-\infty ,+\infty \}$ của $\overline{\mathbf{R}}$. Nếu $u$ là một ánh xạ tuyến tính mà hạt nhân hoặc đối hạt nhân có số chiều hữu hạn, thì chỉ số của $u$ là phần tử ind($u$) của $\overline{\mathbf{Z}}$ được định nghĩa bởi

ind($u$) $=$ dim Coker($u$)$-$ dim Ker($u$)

(xem No$^o6$ của III, p. 67).

#### Định nghĩa 3 {#ts-iii-s6-def-3 .statement tag=02UM}

Cho E là một không gian khả chuẩn đầy đủ và $u$ một tự đồng cấu của E. Với mọi $n\in \overline{\mathbf{Z}}$, ký hiệu Sp$_n(u)$ là tập hợp các số phức $\lambda \in$ Sp$_e(u)$ sao cho $u-\lambda 1_E$ là một cấu xạ ngặt mà hạt nhân hoặc đối hạt nhân có số chiều hữu hạn, và có chỉ số bằng $n$. Ký hiệu Sp$_{\omega}(u)$ là phần bù trong Sp$_e(u)$ của hợp các tập con Sp$_n(u)$ với $n\in \mathbf{Z}$.

Các tập hợp Sp$_s(u)$, Sp$_n(u)$ với $n\in \overline{\mathbf{Z}}$, và Sp$_{\omega}(u)$ tạo thành một phân hoạch của phổ của $u$.

Mọi tự đồng cấu của E mà đối hạt nhân có số chiều hữu hạn đều là ngặt (III, p. 52, Bổ đề 6). Các tự đồng cấu Fredholm của E là các tự đồng cấu của E mà hạt nhân và đối hạt nhân có số chiều hữu hạn (III, p. 52, Mệnh đề 11). Tập hợp $\mathbf{C}-$ Sp$_e(u)$ gồm các $\lambda \in \mathbf{C}$ sao cho $u-\lambda 1_E$ là một tự đồng cấu Riesz của E, và một tự đồng cấu như thế là một tự đồng cấu Fredholm của E có chỉ số 0.

Do đó, với $\lambda \in \mathbf{C}$ và với $n\in \mathbf{Z}-\{0\}$, ta có:

$\lambda \in \mathbf{C}-$ Sp($u$)$\Leftarrow \Rightarrow u-\lambda 1_E$ là một tự đẳng cấu ;

$\lambda \in$ Sp$_s(u)\Leftarrow \Rightarrow u-\lambda 1_E$ là một tự đồng cấu Riesz, nhưng

không phải là một tự đẳng cấu ;

$\lambda \in$ Sp$_0(u)\Leftarrow \Rightarrow u-\lambda 1_E$ là một tự đồng cấu Fredholm

có chỉ số 0 của E nhưng không phải là một tự đồng cấu Riesz của E ;

$\lambda \in$ Sp$_n(u)\Leftarrow \Rightarrow u-\lambda 1_E$ là một tự đồng cấu Fredholm

$(n\not = 0)$ có chỉ số $n$ của E ;

$\lambda \in$ Sp$_{-\infty}(u)\Leftarrow \Rightarrow u-\lambda 1_E$ là ngặt, hạt nhân của nó có số chiều

vô hạn và đối hạt nhân của nó có số chiều hữu hạn ; $\lambda \in$ Sp$_{+\infty}(u)\Leftarrow \Rightarrow u-\lambda 1_E$ là ngặt, hạt nhân của nó có số chiều

hữu hạn và đối hạt nhân của nó có số chiều vô hạn ; $\lambda \in$ Sp$_{\omega}(u)\Leftarrow \Rightarrow$ hoặc là $u-\lambda 1_E$ không ngặt, hoặc hạt nhân

và đối hạt nhân của nó có số chiều vô hạn.

#### Nhận xét {#ts-iii-s6-n2-rem-1 .statement tag=02UN}

Ký hiệu $\pi$ là đồng cấu chính tắc của $\mathscr{L}(E)$ lên đại số Calkin $\mathscr{C}$alk(E) của E (x. No. 4 của III, p. 75). Phổ của $\pi (u)$ đối với đại số $\mathscr{C}$alk(E) đôi khi được gọi là phổ ổn định của $u$. Các phần tử của nó là các số phức $\lambda$ sao cho $u-\lambda 1_E$ không phải là một tự đồng cấu Fredholm của E (hệ quả 1 của định lý 3 của III, p. 73). Do đó nó bằng Sp$_{\omega}(u)\cup$ Sp$_{-\infty}(u)\cup$ Sp$_{+\infty}(u)$.

Gọi A là tập hợp các tự đồng cấu của E giao hoán với $u$. Bao đóng B của $\pi (A)$ trong $\mathscr{C}$alk(E) là một đại số đầy đủ khả chuẩn, và phổ của $\pi (u)$ đối với B là phổ cốt yếu Sp$_e(u)$ của $u$ (III, p. 77, mệnh đề 3). Theo hệ quả của mệnh đề 6 của I, p. 28, áp dụng cho đại số con B của $\mathscr{C}$alk(E), tập hợp Sp$_e(u)$ là hợp của Sp$_{\omega}(u)\cup$ Sp$_{-\infty}(u)\cup$ Sp$_{+\infty}(u)$ và của một số thành phần liên thông bị chặn của phần bù của nó.

#### Định lý 1 {#ts-iii-s6-thm-1 .statement tag=02UO}

Cho E là một không gian khả chuẩn đầy đủ và $u$ là một tự đồng cấu của E.

a) Tập hợp Sp$_{\omega}(u)$ là compắc. Nó không rỗng nếu E là vô hạn chiều;

b) Cho $n\in \overline{\mathbf{Z}}$. Tập hợp Sp$_n(u)$ là hợp của một họ các thành phần liên thông bị chặn của $\mathbf{C}-$ Sp$_{\omega}(u)$. Nó mở trong $\mathbf{C}$, và biên của nó trong $\mathbf{C}$ được chứa trong Sp$_{\omega}(u)$.

Tập hợp $\mathbf{C}-$ Sp$_{\omega}(u)$ gồm các số phức $\lambda \in \mathbf{C}$ sao cho $u-\lambda 1_E$ là một cấu xạ ngặt, mà hạt nhân hoặc đối hạt nhân có số chiều hữu hạn. Theo các mệnh đề 11 của III, p. 67 và 13 của III, p. 70, nó là mở. Do đó tập hợp Sp$_{\omega}(u)$ là đóng. Vì nó bị chặn, nó là compắc.

Hãy chứng minh b). Cho $n\in \overline{\mathbf{Z}}$. Tập hợp Sp$_n(u)$ được chứa trong $\mathbf{C}-$Sp$_{\omega}(u)$. Gọi U là một thành phần liên thông của $\mathbf{C}-$ Sp$_{\omega}(u)$ cắt Sp$_n(u)$. Vì ánh xạ $\lambda \mapsto$ ind($u-\lambda 1_E$) từ $\mathbf{C}-$ Sp$_{\omega}(u)$ vào $\overline{\mathbf{Z}}$ là địa phương hằng (hệ quả 1 của mệnh đề 12 của III, p. 68 và hệ quả 1 của mệnh đề 13 của III, p. 70), nên chỉ số của $u-\lambda 1_E$ bằng $n$ với mọi $\lambda \in U$. Nếu $n\not = 0$, điều này suy ra U được chứa trong Sp$_n(u)$. Nếu $n= 0$, nhận xét rằng tập hợp U là một thành phần liên thông của $\mathbf{C}-$ (Sp$_{\omega}(u)\cup$ Sp$_{-\infty}(u)\cup$ Sp$_{+\infty}(u)$). Vì U cắt Sp$_0(u)$ và do đó cắt Sp$_e(u)$, từ Nhận xét 2 suy ra tập hợp U được chứa trong Sp$_e(u)$, và do đó trong Sp$_0(u)$. Trong mọi trường hợp, ta kết luận rằng Sp$_n(u)$ là hợp của các thành phần liên thông của $\mathbf{C}-$ Sp$_{\omega}(u)$ cắt Sp$_n(u)$. Các thành phần ấy tất yếu bị chặn vì tập hợp Sp($u$) bị chặn. Do đó, Sp$_n(u)$ là mở trong $\mathbf{C}$ và biên của nó được chứa trong Sp$_{\omega}(u)$. Điều này chứng minh b).

Cuối cùng giả sử rằng tập hợp Sp$_{\omega}(u)$ là rỗng. Theo b), khi đó mỗi tập hợp Sp$_n(u)$, với $n\in \overline{\mathbf{Z}}$, đều rỗng. Vì vậy ta có Sp($u$) $=$ Sp$_s(u)$. Do đó phổ của $u$ là rời rạc và compac, nên hữu hạn, và vì mọi điểm của nó đều có bội số phổ hữu hạn, không gian vectơ E là hữu hạn chiều (III, p. 83, mệnh đề 2). Điều này hoàn thành chứng minh của a).

#### Hệ quả {#ts-iii-s6-n2-cor-1 .statement tag=02UP}

a) Gọi Ω là thành phần liên thông không bị chặn của $\mathbf{C}-$ Sp$_{\omega}(u)$. Ta có $\Omega \cap$ Sp($u$)$\subset$ Sp$_s(u)$;

b) Mọi điểm dính với Sp$_s(u)$ mà không thuộc Sp$_s(u)$ đều thuộc Sp$_{\omega}(u)$.

Mệnh đề a) là một hệ quả trực tiếp của mệnh đề b) của định lý 1. Gọi $\lambda$ là một điểm dính với Sp$_s(u)$ mà không thuộc Sp$_s(u)$. Nó thuộc phổ của $u$, vì phổ này đóng. Nó không thuộc bất kỳ tập hợp nào trong các tập hợp Sp$_n(u)$, với $n\in \overline{\mathbf{Z}}$, vì các tập hợp ấy đều mở (loc. cit.) và rời nhau với Sp$_s(u)$. Vì vậy ta có $\lambda \in$ Sp$_{\omega}(u)$, do đó b).

#### Mệnh đề 3 {#ts-iii-s6-prop-3 .statement tag=02UQ}

Cho E và F là các không gian định chuẩn đầy đủ, $u: E\rightarrow F$ và $v: F\rightarrow E$ là các ánh xạ tuyến tính liên tục.

a) Các vết trên $\mathbf{C}-\{0\}$ của các tập Sp($v\circ u$) và Sp($u\circ v$) $($tương ứng Sp$_s(v\circ u)$ và Sp$_s(u\circ v)$, tương ứng Sp$_n(v\circ u)$ và Sp$_n(u\circ v)$ với $n\in \overline{\mathbf{Z}}$, tương ứng Sp$_{\omega}(v\circ u)$ và Sp$_{\omega}(u\circ v))$ là bằng nhau;

b) Cho $\lambda$ là một phần tử của Sp$_s(v\circ u)$ phân biệt với 0. Các bội số phổ của $\lambda$ đối với $v\circ u$ và đối với $u\circ v$ là bằng nhau.

Cho $\mu$ là một số phức khác không và cho $n\in \overline{\mathbf{Z}}$. Điều kiện cần và đủ để $\mu1_E-v\circ u$ là một tự đẳng cấu (tương ứng một tự đồng cấu Riesz, tương ứng một cấu xạ ngặt mà hạt nhân hoặc đối hạt nhân có số chiều hữu hạn và có chỉ số bằng $n$) là $\mu1_F-u\circ v$ cũng là như vậy (III, p. 49, mệnh đề 10). Khi đó mệnh đề a) suy ra từ các định nghĩa.

Cho $\lambda$ là một điểm của Sp$_s(v\circ u)$ phân biệt với 0. Ta có

dim Ker(($\lambda 1_E-v\circ u$)$^n$) $=$ dim Ker(($\lambda 1_F-u\circ v$)$^n$)

với mọi $n\geqslant 0 ($loc. cit.), do đó các bội số phổ của $\lambda$ đối với $v\circ u$ và $u\circ v$ là bằng nhau.

### 3. Phổ của chuyển vị của một tự đồng cấu

#### Mệnh đề 4 {#ts-iii-s6-prop-4 .statement tag=02UR}

Cho E là một không gian định chuẩn đầy đủ, $E'$ là không gian đối ngẫu của E và $u$ là một tự đồng cấu của E.

a) Ta có Sp$_s(u) =$ Sp$_s(^tu)$, Sp$_n(u) =$ Sp$_{-n}(^tu)$ với mọi $n\in \overline{\mathbf{Z}}$ và Sp$_{\omega}(u) = Sp_{\omega}(^tu)$;

b) Mọi điểm của Sp$_s(u)$ đều có cùng bội số phổ đối với $u$ và đối với $^tu$.

Phần a) của mệnh đề 3 ở I, p. 131 chứng minh rằng Sp($u$) $=$ Sp($^tu$), và phần c) của loc. cit. kéo theo rằng Sp$_s(u) =$ Sp$_s(^tu)$ và rằng mệnh đề b) là đúng.

Với mọi $\lambda \in \mathbf{C}$, bổ đề 4 của III, p. 69 kéo theo rằng $u-\lambda 1_E$ là một cấu xạ ngặt khi và chỉ khi $^tu-\lambda 1_{E'}$ là như vậy, và rằng

dim Coker($^t(u-\lambda 1_E)$) $=$ dim Ker($u-\lambda 1_E$)

dim Ker($^t(u-\lambda 1_E)$) $=$ dim Coker($u-\lambda 1_E$)

trong $\overline{\mathbf{Z}}$. Mệnh đề a) suy ra từ điều này, có tính đến các định nghĩa của các phần khác nhau của phổ (định nghĩa 3 của III, p. 85).

### 4. Nhiễu loạn bởi một toán tử compact

#### Định lý 2 {#ts-iii-s6-thm-2 .statement tag=02US}

Cho E là một không gian chuẩn hoá đầy đủ, $u$ là một tự đồng cấu của E và $h$ là một tự đồng cấu compact của E. Ta có Sp$_{\omega}(u+h) =$ Sp$_{\omega}(u)$ và Sp$_n(u+h) =$ Sp$_n(u)$ với mọi $n\in \overline{\mathbf{Z}}-\{0\}$.

Cho $\lambda \in \mathbf{C}$. Để $u+h-\lambda 1_E$ là một cấu xạ ngặt mà hạt nhân (tương ứng, đối hạt nhân) có số chiều hữu hạn, điều kiện cần và đủ là $u-\lambda 1_E$ có tính chất đó, theo Định lý 1 của III, p. 72 (tương ứng, Định lý 2 của III, p. 73).

Các đẳng thức

Sp$_{-\infty}(u+h) =$ Sp$_{-\infty}(u)$, Sp$_{+\infty}(u+h) =$ Sp$_{+\infty}(u)$,

Sp$_{\omega}(u+h) =$ Sp$_{\omega}(u)$

suy ra từ điều này. Hơn nữa, ta có Sp$_n(u+h) =$ Sp$_n(u)$ theo Định lý 3 của III, p. 73 với mọi $n\in \mathbf{Z}-\{0\}$.

#### Hệ quả {#ts-iii-s6-n4-cor-1 .statement tag=02UT}

Giả sử rằng thành phần liên thông không bị chặn của phần bù của Sp$_{\omega}(u)$ chứa 0. Khi đó $u+h$ là một tự đồng cấu Riesz của E.

Ta có Sp$_{\omega}(u+h) =$ Sp$_{\omega}(u)$ (Định lý 2), do đó 0 thuộc thành phần liên thông không bị chặn của $\mathbf{C}-$ Sp$_{\omega}(u+h)$. Theo hệ quả của Định lý 1 của III, p. 87, hoặc 0 không thuộc phổ của $u+h$, hoặc là nó là một điểm nhạy của phổ này. Trong cả hai trường hợp, $u+h$ là một tự đồng cấu Riesz của E.

### 5. Phổ của một toán tử compact

#### Bổ đề 1 {#ts-iii-s6-lem-1 .statement tag=02UU}

Cho E là một không gian vectơ tôpô tách biệt có chiều $\geqslant 2$ trên $\mathbf{R}$, và cho X là một tập con đếm được của E. Tập hợp bù E - X là liên thông.

Trước hết giả sử E có chiều 2. Có thể giả sử rằng $E =\mathbf{R}^2$ được trang bị chuẩn Euclid (TVS, I, p. 14, Định lý 2). Vì X là đếm được, tồn tại một số thực $r\in \mathbf{R}_+^*$ sao cho đường tròn C tâm 0 bán kính $r$ không cắt X. Cho $x\in E$ - X; nếu $x \notin C$, tồn tại một điểm $y\in C$ sao cho đường thẳng $L_x$ nối $x$ với $y$ không cắt X, vì X là đếm được. Tập hợp E - X là hợp của C, là một tập hợp liên thông, và của các tập hợp liên thông $L_x\cup C$ với $x\in E$- $(X\cup C)$; các tập hợp này đều chứa C, và do đó E- X là liên thông (TG, I, p. 81, Mệnh đề 2).

Xét trường hợp tổng quát. Thay thế X bởi $X-x$ với một phần tử $x\in E$ - X, ta quy được về trường hợp $0\notin X$. Vì E - X là hợp của các tập hợp F - $(X\cap F)$ khi F chạy qua tập hợp các không gian con 2 chiều của E, và vì các tập hợp ấy liên thông theo trường hợp trước và chứa 0, nên tập hợp E - X là liên thông (loc. cit.).

#### Bổ đề 2 {#ts-iii-s6-lem-2 .statement tag=02UV}

Cho $S\subset \mathbf{C}$ là một tập hợp vô hạn, rời rạc, bị chặn và đóng trong $\mathbf{C}-\{0\}$. Khi đó S là tập hợp các giá trị của một dãy $(\lambda_n)_{n\in\mathbf{N}}$ các số phức khác không, từng đôi một phân biệt, sao cho dãy $(|\lambda_n|)_{n\in\mathbf{N}}$ giảm và hội tụ về 0.

Với mọi số nguyên $i\geqslant 1$, tập hợp $A_i$ các số phức $\lambda \in S$ sao cho $|\lambda |\geqslant \frac{1}{i}$ là compắc và rời rạc trong $\mathbf{C}$, nên hữu hạn. Gọi $a_i$ là lực lượng của nó. Vì S là vô hạn, dãy $(a_i)$ tiến tới $+\infty$. Đặt $A_0=\emptyset$ và $a_0= 0$. Với mọi $i\geqslant 1$, chọn một song ánh $n\mapsto \lambda_n$ từ khoảng $[a_{i-1}, a_i[$ của $\mathbf{N}$ lên $A_i-A_{i-1}$ sao cho ánh xạ $n\mapsto  |\lambda_n|$ giảm trên $[a_{i-1}, a_i[$. Dãy $(\lambda_n)_{n\in\mathbf{N}}$ thỏa mãn các tính chất cần có.

Cho E là một không gian khả chuẩn đầy đủ vô hạn chiều. Đại số $\mathscr{L}^c(E)$ là một đại số con không có đơn vị của $\mathscr{L}(E)$. Nhắc lại rằng với mọi tự đồng cấu compắc $u\in \mathscr{L}^c$(E), phổ Sp$'_{\mathscr{L}^c(E)}(u)$ là phổ của $u$ đối với đại số con có đơn vị $\mathscr{L}^c(E)\oplus \mathbf{C}1_E$ của $\mathscr{L}(E) ($I, p. 4, No.$^o4$).

#### Mệnh đề 5 {#ts-iii-s6-prop-5 .statement tag=02UW}

Cho E là một không gian khả chuẩn đầy đủ và cho $u$ là một tự đồng cấu compắc của E. Mọi phần tử của Sp$_s(u)$ là một trị riêng có bội số phổ hữu hạn. Hơn nữa:

a) Nếu E là hữu hạn chiều, thì Sp($u$) $=$ Sp$_s(u)$;

b) Nếu E là vô hạn chiều, thì Sp$_s(u) =$ Sp($u$)$-\{0\}$ và Sp$_{\omega}(u) =\{0\}$;

c) Nếu Sp$_s(u)$ là vô hạn, thì nó là tập hợp các giá trị của một dãy $(\lambda_n)_{n\in\mathbf{N}}$ các số phức khác không, từng đôi một phân biệt, sao cho dãy $(|\lambda_n|)_{n\in\mathbf{N}}$ giảm và hội tụ về 0 ;

d) Nếu E là vô hạn chiều, thì Sp($u$) $=$ Sp$'_{\mathscr{L}^c(E)}(u)$.

Mọi phần tử của Sp$_s(u)$ là một trị riêng có bội số phổ hữu hạn (mệnh đề 1 của III, p. 83).

Mệnh đề a) là sơ cấp (III, p. 85, ví dụ 1). Bây giờ giả sử E là vô hạn chiều.

Cho $\lambda \in$ Sp($u$)$-\{0\}$. Khi đó $u-\lambda 1_E$ là một tự đồng cấu Riesz của E (hệ quả 2 của mệnh đề 2 của III, p. 75), do đó $\lambda$ thuộc Sp$_s(u)$. Nếu E là vô hạn chiều, thì Sp$_{\omega}(u)$ không rỗng (III, p. 87, định lý 1, a)). Tất yếu có Sp$_{\omega}(u) =\{0\}$, do đó b).

Tập hợp Sp$_s(u)$ là rời rạc và bị chặn. Hơn nữa, theo b) ta có Sp$_s(u) =$ Sp($u$)$\cap (\mathbf{C}-\{0\})$, nên Sp$_s(u)$ là đóng trong $\mathbf{C}-\{0\}$. Vậy mệnh đề c) suy ra từ Bổ đề 2.

Phổ của $u$ là đếm được, và phần bù của nó trong $\mathbf{C}$ vì thế là liên thông (bổ đề 1). Theo hệ quả của mệnh đề 6 của I, p. 28, áp dụng cho đại số con có đơn vị $\mathscr{L}^c(E)\oplus \mathbf{C}1_E$ của $\mathscr{L}$ (E), suy ra rằng Sp($u$) $=$ Sp$'_{\mathscr{L}^c(E)}(u)$.

#### Mệnh đề 6 {#ts-iii-s6-prop-6 .statement tag=02UX}

Cho E là một không gian định chuẩn đầy đủ trên $\mathbf{C}$ và $u$ là một tự đồng cấu compact của E.

a) Cho $f\in \mathscr{O}$(Sp($u$)) sao cho $f(0) = 0$. Tự đồng cấu $f(u)$ là compact;

b) Giả sử rằng E là một không gian Hilbert phức và $u$ là chuẩn tắc. Cho $f$ là một hàm liên tục trên Sp($u$) sao cho $f(0) = 0$. Tự đồng cấu chuẩn tắc $f(u)$ là compact.

Hơn nữa, các mệnh đề đảo lại là đúng nếu E vô hạn chiều, và điều kiện $f(0) = 0$ là không cần thiết nếu E hữu hạn chiều.

Ta có thể giả sử rằng E là vô hạn chiều.

Ta hãy chứng minh a) và mệnh đề đảo lại của nó. Tự đồng cấu $u$ là một phần tử của đại số Banach $\mathscr{L}^c(E)$. Vì E vô hạn chiều, ta có đẳng thức Sp($u$) $=$ Sp$'_{\mathscr{L}^c(E)}(u)$ theo mệnh đề 5, d). Phần tử $f(u)$ của phép tính phiếm hàm chỉnh hình của đại số Banach có đơn vị suy ra từ $\mathscr{L}^c(E)$ bằng phép nối thêm một phần tử đơn vị thuộc về $\mathscr{L}^c(E)$ khi và chỉ khi $f(0) = 0$ (I, p. 88). Nhưng hơn nữa phần tử này trùng với phần tử $f(u)$ của $\mathscr{L}(E)$ (mệnh đề 7 của I, p. 75), do đó $f(u)$ là compact khi và chỉ khi $f(0) = 0$.

Chứng minh của mệnh đề b) và của mệnh đề đảo lại của nó hoàn toàn giống như vậy nếu ta xét phép tính phiếm hàm liên tục của đại số có phép đối hợp $\mathscr{L}^c(E)$ (I, p. 110, định nghĩa 5).

#### Hệ quả {#ts-iii-s6-n5-cor-1 .statement tag=02UY}

Cho E và F là các không gian Hilbert và cho $u$ là một ánh xạ tuyến tính liên tục từ E vào F. Ánh xạ tuyến tính $u$ là compact khi và chỉ khi tự đồng cấu $|u|$ của E là compact.

Cho $(j,|u|)$ là phân tích cực của $u$ (định nghĩa 4 của I, p. 140). Vì

$$
\surd
$$

$u=j|u|$ và $|u|=u^*u$ (mệnh đề 10 của I, p. 139), tính tương đương suy ra từ mệnh đề 3 của III, p. 5 và mệnh đề b) của mệnh đề trước.

### 6. Trường hợp các không gian Hilbert

Trong No. này, E chỉ một không gian Hilbert trên $\mathbf{C}$. Ta ký hiệu bởi $\pi$ đồng cấu chính tắc của $\mathscr{L}(E)$ lên đại số có phép đối hợp $\mathscr{C}$alk(E).

#### Mệnh đề 7 {#ts-iii-s6-prop-7 .statement tag=02UZ}

Cho $u\in \mathscr{L}(E)$.

a) Nếu $u$ là chuẩn tắc, thì $u$ là một tự đồng cấu Riesz khi và chỉ khi $u$ là một tự đồng cấu Fredholm có chỉ số 0.

b) Nếu $u$ là Hermit, thì $u$ là một tự đồng cấu Fredholm khi và chỉ khi $u$ là một tự đồng cấu Riesz.

Mọi tự đồng cấu Riesz đều là một tự đồng cấu Fredholm có chỉ số 0 (mệnh đề 5 của III, p. 46). Đảo lại, giả sử rằng $u$ là một tự đồng cấu Fredholm có chỉ số 0, và rằng $u$ là chuẩn tắc. Khi đó không gian không của nó trùng với hạt nhân của nó (EVT, V, p. 43, mệnh đề 8), và vì thế có số chiều hữu hạn. Khi đó suy ra từ bổ đề 2 của III, p. 45 và từ định nghĩa rằng $u$ là một tự đồng cấu Riesz.

Ta hãy chứng minh b). Theo a), chỉ cần kiểm tra rằng chỉ số của một tự đồng cấu Fredholm Hermit $u$ bằng không. Nhưng trực giao bù của ảnh của $u$ (là đóng) khi đó bằng hạt nhân của $u$ (EVT, V, p. 41, mệnh đề 4), do đó có mệnh đề phải chứng minh.

#### Hệ quả {#ts-iii-s6-n6-cor-1 .statement tag=02V0}

Cho $u\in \mathscr{L}(E)$. Nếu $u$ là chuẩn tắc, thì Sp$_0(u)$ là rỗng, và nếu $u$ là Hermit, thì Sp$_e(u)$ trùng với phổ của $\pi (u)$ đối với đại số $\mathscr{C}$alk(E).

Cả hai khẳng định đều suy ra từ mệnh đề và từ định nghĩa của các tập Sp$_n(u)$ với $n\in \overline{\mathbf{Z}}$ và của Sp$_{\omega}(u)$, các tập này tạo thành một phân hoạch của phổ cốt yếu của $u$ (định nghĩa 2 của III, p. 83).

#### Định lý 3 (Weyl) {#ts-iii-s6-thm-3 .statement tag=02V1}

Cho $u\in \mathscr{L}(E)$ là một tự đồng cấu chuẩn tắc của $u$. Phổ cốt yếu của $u$ là giao của các tập Sp($u+h$), khi $h$ chạy qua $\mathscr{L}^c(E)$.

Cho $h\in \mathscr{L}^c(E)$. Vì Sp$_0(u)$ là rỗng (hệ quả trên), Định lý 2 của III, p. 89 suy ra rằng Sp$_e(u+h) =$ Sp$_e(u)$. Do đó giao của các tập Sp($u+h$) chứa Sp$_e(u)$.

Cho $\lambda \in$ Sp$_s(u)$. Gọi $E_{\lambda}$ là không gian con riêng của $u$ ứng với $\lambda$, và $F_{\lambda}$ là ảnh của phép chiếu phổ liên kết với $u$ và $\mathbf{C}-\{\lambda \}$. Không gian E là tổng trực tiếp tôpô của $E_{\lambda}$ và $F_{\lambda}$. Cho $h$ là tự đồng cấu hạng hữu hạn của E bằng không trên $F_{\lambda}$ và trùng trên $E_{\lambda}$ với đồng nhất. Tự đồng cấu $u+h$ là khả nghịch, do đó $\lambda  \notin$ Sp($u+h$). Định lý được chứng minh.

Vì vậy, nếu $u$ là một tự đồng cấu chuẩn tắc của E, và nếu $h\in \mathscr{L}^c$(E), thì phổ của $u+h$ chỉ có thể khác phổ của $u$ ở các điểm cô lập có bội số phổ hữu hạn.

### 7. Định lý Krein-Rutman

#### Bổ đề 3 {#ts-iii-s6-lem-3 .statement tag=02V2}

Cho $(a_n)_{n\geqslant 0}$ là một dãy các số thực dương sao cho chuỗi lũy thừa

$$
f(z) =\sum_{n\geqslant 0}a_nz^n
$$

có bán kính hội tụ hữu hạn $r >0$. Cho $D\subset \mathbf{C}$ là đĩa mở tâm 0 bán kính $r$. Không tồn tại một hàm chỉnh hình $\widetilde{f}$ xác định trên một lân cận mở U của $r$ trong $\mathbf{C}$ mà trùng với $f$ trên $U\cap D$.

Giả sử tồn tại một hàm chỉnh hình như vậy $\widetilde{f}$ được xác định trên một lân cận mở U của $r$. Tồn tại các số thực $s < r$ và $\delta  >0$ sao cho $s+\delta  > r$ và sao cho đĩa mở $D'$ có tâm $s$ và bán kính $\delta$ được chứa trong U. Khai triển chuỗi lũy thừa của $\widetilde{f}$ tại điểm $s$ (VAR, R1, p. 26, 3.2.1) khi đó hội tụ với mọi $z$ trong đĩa có tâm 0 và bán kính $\delta$ (VAR, R1, p. 29, 3.3.4). Chuỗi này là

$+\infty (n)+\infty (n)$

$\widetilde{f}_s(z) =\sum\widetilde{f}n$!$(s)z^n=\sum fn$!$(s)z^n$

$n=0n=0$ (VAR, R1, p. 27, 3.2.4). Vì $s\in D$, ta có

$$
f^{(n)}(s) =\sum_{k=n}^{+\infty}k(k-1)\cdots (k-n+ 1)a_ks^{k-n}
$$

(VAR, R1, p. 28, 3.2.11). Lấy $z$ sao cho $0< z < \delta$. Vì $a_k\geqslant 0$, ta có

$\widetilde{f}_s(z) =\sum^{+\infty}(\sum^{+\infty}k(k-1)\cdots n($!$k-n+ 1)a_ks^{k-n})z^n$

$n=0k=n$ $+\infty k+\infty$

$=\sum(a_k\sum n$!($kk-$! $n$)! $s^{k-n}z^n)=\sum a_k(s+z)^k$

$k=0n=0k=0$

(TG, III, p. 40). Khi $s+z > r$, sự hội tụ của biểu thức này mâu thuẫn với giả thiết rằng bán kính hội tụ của chuỗi lũy thừa $f$ bằng $r$.

Cho E là một không gian Banach thực. Cho C là một nón lồi có đỉnh trong E. Không gian vectơ sinh bởi C bằng $C-C$ (EVT, II, p. 12, hệ quả 1). Đặc biệt, nón C là toàn phần trong E khi và chỉ khi $C-C$ trù mật trong E. Nhắc lại rằng C được gọi là nhọn nếu $C\cap (-C)$ thu về 0 (EVT, II, p. 11).

Đối cực $C^{\circ}$ của C là tập hợp các dạng tuyến tính liên tục $\ell \in E'$ sao cho $\ell (x)\geqslant 0$ với mọi $x\in C$ (EVT, II, p. 47, mệnh đề 4). Theo định lý lưỡng cực (EVT, II, p. 48, định lý 1), nếu C là một nón lồi có đỉnh đóng, thì ta có $C^{\circ \circ}= C$.

#### Bổ đề 4 {#ts-iii-s6-lem-4 .statement tag=02V3}

Cho E là một không gian Banach thực và $u\in \mathscr{L}(E_{(\mathbf{C})})$ là một tự đồng cấu khác không của $E_{(\mathbf{C})}$. Cho C là một nón lồi toàn phần trong E. Tồn tại $x\in C$ sao cho $u(x)\not = 0$.

Thật vậy, nếu $u$ triệt tiêu trên C, thì $u$ triệt tiêu trên $C-C$, do đó trên E, và vì thế trên $E_{(\mathbf{C})}$.

#### Định lý 4 (Krein–Rutman) {#ts-iii-s6-thm-4 .statement tag=02V4}

Cho E là một không gian định chuẩn đầy đủ trên $\mathbf{R}$. Cho C là một nón lồi nhọn toàn phần đóng trong E và cho $u\in \mathscr{L}(E)$ là một ánh xạ tuyến tính compact sao cho $u(C)\subset C$. Nếu bán kính phổ $\varrho (u)$ là $>0$, thì $\varrho (u)$ là một điểm cô lập của phổ của $u$, và tồn tại một vectơ riêng khác không $x\in C$ của $u$ ứng với trị riêng $\varrho (u)$.

Cho $E_{(\mathbf{C})}$ là không gian phức hóa của E và $u_{(\mathbf{C})}$ là tự đồng cấu của $E_{(\mathbf{C})}$ thu được bằng cách mở rộng vô hướng từ $u$. Bán kính phổ của $u_{(\mathbf{C})}$ bằng $\varrho (u) ($I, p. 86); ta ký hiệu đơn giản nó bởi $\varrho$. Vì $\varrho  >0$, phổ phức của $u$ không bị thu về 0. Do đó tồn tại $\lambda_0\in$ Sp$_s(u_{(\mathbf{C})})$ sao cho $|\lambda_0|=\varrho$ (Mệnh đề 5 của III, p. 90). Gọi $e_0$ là phép chiếu phổ của $u_{(\mathbf{C})}$ liên kết với $\lambda_0$.

Hàm giải thức $\lambda \mapsto R(u_{(\mathbf{C})}, \lambda ) = (\lambda -u_{(\mathbf{C})})^{-1}$ là chỉnh hình trên phần bù của phổ của $u_{(\mathbf{C})}$ (Định lý 1 của I, p. 24). Số phức $\lambda_0$ là một cực của hàm giải thức và thặng dư của nó là phép chiếu phổ $e_0($I, p. 131).

Cho $y$ và $y'$ là các phần tử của E sao cho $y+iy'\in E_{(\mathbf{C})}$ là một vectơ riêng của $u_{(\mathbf{C})}$ ứng với trị riêng $\lambda_0$. Vì $e_0(y+iy') =y+iy'\not = 0$, nên tồn tại một phần tử $x_0\in C$ sao cho $e_0(x_0)\not = 0$ (Bổ đề 4). Vì C đóng và nhọn, cực đối ngẫu của nó $C^{\circ}$ là toàn bộ (EVT, II, p. 48, Hệ quả 1), và khi đó tồn tại một dạng tuyến tính $\ell_0\in C^{\circ}$ sao cho $\langle e_0(x_0), \ell_0\rangle  \not = 0$.

Xét hàm $f$ được xác định bởi $f(0) = 0$ và bởi

$$
f(z) =\langle R(u_{(\mathbf{C})}, z^{-1})x_0, \ell_0\rangle
$$

với $z\in \mathbf{C}$ sao cho $z^{-1}\notin$ Sp($u_{(\mathbf{C})}$). Hàm này thỏa mãn

$$
f(z) =\ell_0((\sum^{+\infty}_{n=0}z^{n+1}u^n_{(\mathbf{C})})x_0)=\sum_{n=0}^{\infty}\langle u^n(x_0), \ell_0\rangle z^{n+1} \tag{1}
$$

với $|z|<1/\varrho$ (Định lý 1 của I, p. 24, d)) và do đó là chỉnh hình trong đĩa tâm 0 bán kính $1/\varrho$.

Tồn tại một hàm chỉnh hình $\widetilde{R}$ xác định trên một lân cận mở U của $\lambda_0$ và nhận giá trị trong $\mathscr{L}(E)$ sao cho với $z$ thuộc U$-\{\lambda_0\}$, ta có

$$
R(u_{(\mathbf{C})}, z) =\widetilde{R}(z) +\sum_{n=0}^{+\infty}(z-\lambda_0)^{-n-1}(u_{(\mathbf{C})}-\lambda_0)^ne_0
$$

(Mệnh đề 17 của I, p. 83). Do đó, với $z$ sao cho $z^{-1}\in U$ và $z\not = 1/\lambda_0$, ta có

$$
f(z) =\langle \widetilde{R}(z^{-1})x_0, \ell_0\rangle +\sum_{n=0}^{+\infty}(z^{-1}-\lambda_0)^{-n-1}\langle (u_{(\mathbf{C})}-\lambda_0)^ne_0(x_0), \ell_0\rangle
$$

Số hạng của chuỗi tương ứng với $n= 0$ là $(z^{-1}-\lambda_0)^{-1}\langle e_0(x_0), \ell_0\rangle$. Vì $\langle e_0(x_0), \ell_0\rangle  \not = 0$, tính duy nhất của khai triển Laurent (VAR, R1, p. 30, 3.3.9) suy ra rằng $f$ không thể được kéo dài thành một hàm chỉnh hình trong một lân cận của $1/\lambda_0$. Đặc biệt, bán kính hội tụ của khai triển thành chuỗi lũy thừa (1) của hàm $f$ tại điểm 0 bằng $1/\varrho$.

Các hệ số của chuỗi lũy thừa (1) là $\langle u^n(x_0), \ell_0\rangle \geqslant 0$ vì $u(C)\subset C$ và $\ell_0\in C^{\circ}$. Theo Bổ đề 3, hàm $f$ không thể được mở rộng thành một hàm chỉnh hình trong một lân cận của $1/\varrho$. Do đó phân giải thức của $u_{(\mathbf{C})}$ không thể được mở rộng thành một hàm chỉnh hình trong một lân cận của $\varrho$, nghĩa là $\varrho \in$ Sp($u$). Điều này suy ra rằng $\varrho$ là một trị riêng của $u_{(\mathbf{C})}$ (mệnh đề 5 của III, p. 90). Vì $\varrho$ là thực, nó cũng là một trị riêng của $u$.

Gọi $d\geqslant 1$ là cấp của cực của phân giải thức của $u_{(\mathbf{C})}$ tại $\varrho$. Gọi $e$ là tự đồng cấu

$e=$ lim$_{z\rightarrow\varrho}(z-\varrho )^dR(u_{(\mathbf{C})}, z)$.

Nó khác không và giao hoán với $u_{(\mathbf{C})}$, và ảnh của nó được chứa trong không gian riêng của $u_{(\mathbf{C})}$ tương ứng với $\varrho ($xem No.$^o3$ của I, p. 131). Bây giờ gọi $\ell$ là một phần tử của $C^{\circ}$ và $x$ là một phần tử của C. Theo Định lý 1 của I, p. 24, d), ta có

$\langle e(x), \ell \rangle =$ lim$_{zz>\varrho\rightarrow\varrho}(z-\varrho )^d\sum_{n\geqslant 0}\langle u^n(x), \ell \rangle z^{-n-1}\geqslant 0$.

Định lý lưỡng cực (EVT, II, p 48, đl. 1) suy ra rằng $e(x)\in C$ với mọi $x\in C$. Vì C là toàn phần, tồn tại $x\in C$ sao cho $e(x)\not = 0$ (Bổ đề 4), và khi đó $e(x)$ thuộc C và là một vectơ riêng của $u$ ứng với trị riêng $\varrho$, đúng như cần chứng minh.

#### Hệ quả {#ts-iii-s6-n7-cor-1 .statement tag=02V5}

Cho E là một không gian khả chuẩn đầy đủ trên $\mathbf{R}$. Cho C là một nón lồi đóng nhọn toàn phần trong E và $u\in \mathscr{L}(E)$ là một ánh xạ tuyến tính compắc sao cho $u(C)\subset C$. Nếu bán kính phổ $\varrho (u)$ của $u$ là $>0$, thì $\varrho (^tu) =\varrho (u)$ là một trị riêng của $^tu$, và $^tu$ thừa nhận một vectơ riêng ứng với $\varrho (u)$ trong $C^{\circ}$.

Ta có $\varrho (^tu) =\varrho (u)$ (mệnh đề 3 của I, p. 131). Theo Hệ quả 1 của III, p. 9, tự đồng cấu $^tu$ của $E'$ là compắc. Hơn nữa, ta có $^tu(C^{\circ})\subset C^{\circ}$; khi đó mệnh đề suy ra từ định lý Krein-Rutman áp dụng cho $^tu$, và cho nón lồi đóng $C^{\circ}$, vì nón sau là nhọn (do C là toàn phần) và toàn phần (do C là nhọn).

#### Nhận xét {#ts-iii-s6-n7-rem-1 .statement tag=02V6}

Nói chung, giả thiết $\varrho (u)>0$ không thể bỏ đi trong định lý Krein-Rutman. Chẳng hạn, gọi V là tự đồng cấu của không gian Banach $\mathscr{C}([0,1])$ được xác định bởi

$$
V(f)(x) =\int_0^xf(y)dy
$$

với $f\in \mathscr{C}([0,1])$. Ánh xạ V là compắc và bán kính phổ của nó bằng không (Bài tập 1 của I, p. 187). Nó bảo toàn nón lồi đóng nhọn toàn phần trong $\mathscr{C}([0,1])$ tạo bởi các hàm dương, và không có trị riêng nào (loc. cit.).

Mệnh đề sau mô tả một điều kiện đủ để một tự đồng cấu bảo toàn một nón có bán kính phổ dương ngặt, và khi đó làm sắc bén thêm định lý Krein-Rutman.

#### Mệnh đề 8 {#ts-iii-s6-prop-8 .statement tag=02V7}

Cho E là một không gian khả chuẩn đầy đủ khác không trên $\mathbf{R}$. Cho C là một nón lồi nhọn đóng có phần trong khác rỗng $\mathring{C}$ trong E, và cho $u\in \mathscr{L}(E)$ là một ánh xạ tuyến tính compắc sao cho $u(C-\{0\})\subset \mathring{C}$.

a) Ta có $\varrho (u)>0$ và tồn tại một vectơ riêng $x_0$ của $u$ trong $\mathring{C}$ ứng với trị riêng $\varrho (u)$;

b) Phép chiếu phổ của $u$ tương ứng với $\varrho (u)$ có hạng 1;

c) Với mọi trị riêng $\lambda \not =\varrho (u)$ của $u_{(\mathbf{C})}$, ta có $|\lambda |< \varrho (u)$;

d) Cho F là một không gian con của E ổn định dưới tác động của $u$ sao cho (C $-\{0\}$)$\cap F$ khác rỗng. Khi đó $x_0\in F$. Đặc biệt, các vectơ riêng duy nhất của $u$ trong C là các bội của $x_0$.

Ta hãy chứng minh hai bổ đề sơ bộ.

#### Bổ đề 5 {#ts-iii-s6-lem-5 .statement tag=02V8}

Cho E là một không gian Banach thực, C là một nón lồi trong E, và $u\in \mathscr{L}(E)$ sao cho $u(C-\{0\})\subset \mathring{C}$. Cho $\ell \in C^{\circ}$ là một vectơ riêng của $^tu$. Khi đó hạt nhân của $\ell$ ổn định dưới tác động của $u$ và không giao với C $-\{0\}$.

Cho $\lambda \in \mathbf{R}$ sao cho $^tu(\ell ) =\lambda \ell$. Với mọi $x\in$ Ker($\ell$ ), ta có

$$
\langle u(x), \ell \rangle =\langle x,^tu(\ell )\rangle =\lambda \langle x, \ell \rangle = 0
$$

do đó Ker($\ell$ ) ổn định dưới tác động của $u$.

Cho $x$ là một phần tử khác không của Ker($\ell$ ). Với mọi phần tử $y$ của E sao cho $\langle y, \ell \rangle <0$, ta có $\langle u(x) +y, \ell \rangle <0$, do đó suy ra rằng $u(x) +$ $y \notin C$ vì $\ell \in C^{\circ}$. Suy ra $u(x)$ không thuộc $\mathring{C}$. Vì $u(C-\{0\})\subset \mathring{C}$, điều này kéo theo $x \notin C$.

#### Bổ đề 6 {#ts-iii-s6-lem-6 .statement tag=02V9}

Cho E là một không gian vectơ thực hữu hạn chiều và B là một lân cận lồi compắc của 0 trong E. Cho $u$ là một tự đồng cấu của E sao cho $u(B)\subset \mathring{B}$. Khi đó phổ phức của $u$ được chứa trong đĩa đơn vị của $\mathbf{C}$ và, đặc biệt, không giao với đường tròn tâm 0 bán kính 1 trong $\mathbf{C}$.

Thay thế B bởi $B\cap (-B)$, ta được quy về trường hợp B là cân bằng. Phiếm hàm Minkowski $p$ của B (EVT, II, p. 28, ex. 3) khi đó là một chuẩn trên E, chuẩn này xác định tôpô của E (EVT, I, p. 14, th. 2). Giả thiết kéo theo rằng $p(u(x))< p(x)$ với mọi phần tử $x$ của E $-\{0\}$, do đó bán kính phổ của $u$ là $<1$; vì đó cũng là bán kính phổ của $u_{(\mathbf{C})}($cf. I, p. 86), kết luận suy ra.

Bây giờ ta chứng minh mệnh đề.

Kí hiệu bởi $x\preccurlyeq y$ quan hệ thứ tự trên E liên kết với nón lồi C (EVT, II, p. 13, n$^o5$), nghĩa là, $x\preccurlyeq y$ khi và chỉ khi $y-x\in C$. Ta có $u(x)\preccurlyeq u(y)$ nếu $x\preccurlyeq y$. Vì $\mathring{C}$ khác rỗng, không gian vectơ $C-C$ sinh bởi C (EVT, II, p. 12, hệ quả 1) chứa một lân cận của 0, do đó nón C là toàn phần.

Ta hãy chứng minh mệnh đề a). Đặt $\varrho =\varrho (u)$. Lấy $y_0$ là một phần tử của $\mathring{C}$. Ta có $y_0\not = 0$. Lấy $r >0$ sao cho quả cầu đóng tâm $y_0$ bán kính $r$ được chứa trong C. Với mọi $y\in E-\{0\}$, ta có $y_0-r\|y\|^{-1}y\in C$, do đó $y\preccurlyeq r^{-1}\|y\|y_0$ với mọi $y\in E$.

Vì $y_0\not = 0$, các giả thiết suy ra $u(y_0)\in \mathring{C}$. Do đó tồn tại $t >0$ sao cho $tu(y_0)-y_0\in C$. Đặt $v=tu$. Đó là một tự đồng cấu compact của E sao cho $v(C)\subset C$ và $v(y_0)\succcurlyeq y_0$. Với mọi số nguyên $n\geqslant 1$, ta có

$$
y_0\preccurlyeq v^n(y_0)\preccurlyeq r^{-1}\|v^n(y_0)\|y_0\preccurlyeq r^{-1}\|v^n\| \|y_0\|y_0
$$

do đó $(r^{-1}\|v^n\|\|y_0\| -1)y_0\in C$. Vì C là nhọn, điều này suy ra $t^n\|u^n\|=\|v^n\|\geqslant r/\|y_0\|$, do đó $\varrho \geqslant t^{-1}>0 ($I, p. 20, mệnh đề 1).

Theo định lý Krein-Rutman (định lý 4), số thực $\varrho$ là một trị riêng của $u$, và tồn tại một vectơ riêng $x_0$ của $u$ trong C ứng với trị riêng $\varrho$. Ta có $\varrho x_0=u(x_0)\in \mathring{C}$ theo giả thiết, do đó $x_0\in \mathring{C}$. Điều này chứng minh mệnh đề a).

Gọi K là giao của phổ của $u_{(\mathbf{C})}$ với đường tròn tâm 0 bán kính $\varrho$ trong $\mathbf{C}$. Vì $u$ là compact và $\varrho  >0$, tập hợp K là hữu hạn và ảnh của phép chiếu phổ $e_K$ là một không gian con của $E_{(\mathbf{C})}$ có số chiều hữu hạn (mệnh đề 2 của III, p. 83 và mệnh đề 5 của III, p. 90). Vì K ổn định dưới phép liên hợp phức, ảnh của $e_K$ là một không gian con của $E_{(\mathbf{C})}$ hữu tỉ trên $\mathbf{R}$ (A, V, p.60, mệnh đề 6) ; gọi F là không gian con của E sao cho $F_{(\mathbf{C})}$ bằng ảnh của $e_K$. Không gian F ổn định dưới $u$ và chứa không gian riêng của $u$ tương ứng với $\varrho$, do đó F khác không.

Để chứng minh các mệnh đề b) và c), chỉ cần chứng minh rằng F có chiều bằng 1.

Cho $v$ là tự đồng cấu của F suy ra từ $u$ bằng cách chuyển qua các không gian con. Đặt $C_F= C\cap F$. Đây là một nón lồi nhọn đóng có phần trong khác rỗng trong F (vì $x_0\in \mathring{C}\cap F$), do đó là toàn phần; nó thỏa mãn $v(C_F-\{0\})\subset \mathring{C}_F$, và đặc biệt ổn định dưới $v$. Vì $\varrho (v)\leqslant \varrho$ và $x_0\in F$, ta có $\varrho (v) =\varrho$. Từ hệ quả của Định lý 4, áp dụng cho $C_F$ và $v$, tồn tại một vectơ riêng $\ell$ của $^tv$ trong $C^{\circ}_F$ ứng với trị riêng $\varrho (v) =\varrho  >0$.

Không gian con Ker($\ell$ ) của F ổn định dưới $v$. Cho $w$ là tự đồng cấu của Ker($\ell$ ) suy ra từ $\varrho^{-1}v$ bằng cách chuyển qua các không gian con; phổ của nó được chứa trong đường tròn đơn vị. Tập hợp B gồm các $y\in$ Ker($\ell$ ) sao cho $x_0+y\in C_F$ là một lân cận lồi đóng của 0 trong Ker($\ell$ ). Với mọi $y\in B$ và mọi $z\in$ Ker($\ell$ ), ta có

$$
x_0+ (w(y) +z) =\varrho^{-1}(v(x_0+y) +\varrho z)
$$

vế này thuộc $C_F$ nếu chuẩn của $z$ đủ nhỏ, do đó $w(y)\in \mathring{B}$.

Tập hợp B bị chặn: thật vậy, nếu tồn tại một dãy $(y_n)_{n\in\mathbf{N}}$ trong Ker($\ell$ ) sao cho $\|y_n\| \rightarrow +\infty$ và $x_0+y_n\in C_F$ thì, bằng cách chuyển sang một dãy con nếu cần, ta sẽ có $y_n/\|y_n\| \rightarrow y$ với $y\in$ Ker($\ell$ ) khác không, và $y=$ lim $\|y_n\|^{-1}(x_0+y_n)$ sẽ thuộc $C_F$, trái với Bổ đề 5. Do đó tập hợp B là compact.

Khi đó suy ra từ Bổ đề 6, áp dụng cho Ker($\ell$ ), cho B và cho $w$, rằng phổ phức của $w$ không cắt đường tròn tâm 0 bán kính 1; điều này kéo theo rằng phổ của $w$ là rỗng, nghĩa là Ker($\ell$ ) thu về $\{0\}$, do đó F có chiều 1. Như vậy các khẳng định b) và c) được thiết lập.

Ánh xạ tuyến tính $^tu$ là compact (Hệ quả 1 của III, p. 9) và $^tu(C^{\circ})\subset C^{\circ}$; hơn nữa $\varrho (^tu) =\varrho  >0$ (mệnh đề 3 của I, p. 131). Từ hệ quả của Định lý 4, tồn tại trong $C^{\circ}$ một vectơ riêng $\ell \not = 0$ của $^tu$ ứng với trị riêng $\varrho$. Hạt nhân của $\ell$ ổn định dưới $u$ và không cắt C $-\{0\}$ (Bổ đề 5). Đặc biệt, ta có $x_0\notin$ Ker($\ell$ ).

Cho F là một không gian con của E ổn định bởi $u$. Ta có phân tích $F = (F\cap \mathbf{R}x_0)\oplus (F\cap$ Ker($\ell$ )). Nếu F không chứa $x_0$, thì do đó ta có $F\subset$ Ker($\ell$ ), suy ra F không cắt C$-\{0\}$. Điều này chứng minh d) và kết thúc chứng minh của mệnh đề.

#### Hệ quả {#ts-iii-s6-n7-cor-2 .statement tag=02VA}

Cho E là một không gian khả chuẩn đầy đủ khác không trên $\mathbf{R}$. Cho C là một nón lồi nhọn đóng có phần trong khác rỗng $\mathring{C}$ trong E, và cho $u$ là một tự đồng cấu compact của E sao cho $u(C)\subset C$. Giả sử tồn tại một số nguyên $k\geqslant 1$ sao cho $u^k(C-\{0\})\subset \mathring{C}$.

a) Ta có $\varrho (u)>0$ và tồn tại một vectơ riêng $x_0$ của $u$ trong $\mathring{C}$ ứng với trị riêng $\varrho (u)$;

b) Phép chiếu phổ của $u$ tương ứng với $\varrho (u)$ có hạng 1;

c) Với mọi trị riêng $\lambda \not =\varrho (u)$ của $u_{(\mathbf{C})}$, ta có $|\lambda |< \varrho (u)$;

d) Các vectơ riêng duy nhất của $u$ trong C là các bội của $x_0$.

Đặt $\varrho =\varrho (u)$. Ta có thể áp dụng Định lý 4 cho $u$ và Mệnh đề 8 cho $u^k$. Do đó tồn tại một vectơ riêng $x_0$ của $u$ trong C ứng với trị riêng $\varrho$. Vì $0< \varrho (u^k) =\varrho^k$ (công thức (4) của I, p. 21), nên đặc biệt ta có $\varrho  >0$, và vì $x_0$ là một vectơ riêng của $u^k$ ứng với trị riêng $\varrho (u^k)$, nên ta có $x_0\in \mathring{C}$.

Ta có Sp($u^k_{(\mathbf{C})}$) $=$ Sp($u_{(\mathbf{C})}$)$^k$ (nhận xét 4 của I, p. 2), do đó mọi trị riêng $\lambda \in \mathbf{C}$ của $u_{(\mathbf{C})}$ sao cho $|\lambda |=\varrho$ đều thỏa mãn $\lambda^k=\varrho^k$, và vì mọi vectơ riêng ứng với $\lambda$ đều là một vectơ riêng của $u^k$ ứng với $\varrho^k$, nên tỷ lệ với $x_0$, ta có $\lambda =\varrho$.

Nếu phép chiếu phổ của $u$ ứng với trị riêng $\varrho$ có hạng ít nhất bằng 2, thì điều tương tự cũng đúng với phép chiếu phổ của $u^k$ ứng với trị riêng $\varrho^k($xem No.$^o2$ của I, p. 129).

Sau cùng, nếu $x\in C$ là một vectơ riêng của $u$, thì nó cũng là một vectơ riêng của $u^k$, nên tỷ lệ với $x_0$.

Cho $n$ là một số nguyên $\geqslant 1$. Tập hợp $\mathbf{R}_+^n$ là một nón lồi đóng, nhọn và salient trong $\mathbf{R}^n$, có phần trong khác rỗng bằng $(\mathbf{R}_+^*)^n$.

Cho A $= (a_{i,j})$ là một ma trận thực kiểu $(n, n)$, và $u_A$ là tự đồng cấu $x\mapsto Ax$ của $\mathbf{R}^n$. Đặt $\varrho =\varrho (u_A)$ là bán kính phổ của nó.

#### Bổ đề 7 {#ts-iii-s6-lem-7 .statement tag=02VB}

Ta có $u_A(\mathbf{R}^n_+)\subset \mathbf{R}_+^n$ khi và chỉ khi $a_{i,j}\geqslant 0$ với mọi $i$ và $j$, và $u_A(\mathbf{R}^n_+-\{0\})\subset (\mathbf{R}_+^*)^n$ khi và chỉ khi $a_{i,j}>0$ với mọi $i$ và $j$.

Cho $(e_1, . . . , e_n)$ là cơ sở chính tắc của $\mathbf{R}^n$. Các vectơ $e_i$ thuộc $\mathbf{R}_+^n$ và $u_A(e_i)\in \mathbf{R}_+^n$ với mọi $i$ (resp. $u_A(e_i)\in (\mathbf{R}_+^*)^n$ với mọi $i$) khi và chỉ khi $a_{i,j}\geqslant 0$ với mọi $i$ và $j$ (resp. $a_{i,j}>0$ với mọi $i$ và $j$). Kết quả suy ra bởi tính tuyến tính.

#### Định lý 5 (Perron–Frobenius) {#ts-iii-s6-thm-5 .statement tag=02VC}

a) Nếu $a_{i,j}\geqslant 0$ với mọi $i$ và $j$ trong $\{1, . . . , n\}$, thì số thực $\varrho$ là một trị riêng của A;

b) Nếu $a_{i,j}>0$ với mọi $i$ và $j$ trong $\{1, . . . , n\}$, thì $\varrho  >0$ và không gian nguyên sơ của $u_A$ đối với $\varrho$, tức là không gian nil của $A-\varrho 1_{\mathbf{R}^n}$, có chiều 1 và được sinh bởi một vectơ $x_0\in (\mathbf{R}_+^*)^n$. Không tồn tại trị riêng nào khác của A có một vectơ riêng trong $\mathbf{R}^n_+$, và mọi trị riêng phức $\lambda \not =\varrho$ của A đều thỏa mãn $|\lambda |< \varrho$.

Nếu $\varrho = 0$, mệnh đề a) là sơ cấp, vì khi đó 0 là một trị riêng của A. Nếu $\varrho  >0$, mệnh đề a) suy ra từ định lý 4 theo bổ đề 7. Mệnh đề b), vì cùng một lý do, là một hệ quả của mệnh đề 8.

#### Nhận xét {#ts-iii-s6-n7-rem-2 .statement tag=02VD}

Giả sử rằng tồn tại một số nguyên $k\geqslant 1$ sao cho mọi hệ số của $A^k$ đều $>0$ (một ma trận như vậy đôi khi được gọi là nguyên thủy). Khi đó, theo hệ quả của Mệnh đề 8, bán kính phổ $\varrho$ là một trị riêng của A, không gian nguyên sơ của $u_A$ đối với $\varrho$ có chiều 1, và được sinh bởi một vectơ $x_0\in (\mathbf{R}^*_+)^n$. Hơn nữa, không tồn tại trị riêng phức nào khác của A nhận một vectơ riêng trong $\mathbf{R}_+^n$ và mọi trị riêng phức $\lambda \not =\varrho$ của A đều thỏa mãn $|\lambda |< \varrho$.

## BÀI TẬP {#ts-iii-s6-exercises}

Xem [các bài tập của § 6](exercises/s6/).

[^1]: Một số tác giả nói đến một "điểm hữu hạn" của phổ, hoặc một "phổ rời rạc".
