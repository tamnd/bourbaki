---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 10
section_title: Modules over an Artinian Ring
lang: vi
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.173-A VIII.181
pdf_pages: 0190-0198
extraction: native
subsections:
    - "no": 1
      title: The Radical of an Artinian Ring
      page: 173
      pdf_page: 190
    - "no": 2
      title: Modules over an Artinian Ring
      page: 174
      pdf_page: 191
    - "no": 3
      title: Projective Modules over an Artinian Ring
      page: 175
      pdf_page: 192
statements: 12
exercises: 11
content_sha256: 976e60796d9a3ee8cd1441887ea663192d7a2373bb41d74954d5994bc4d8458d
translated_from: content/en/alg/VIII/10_s10_modules_over_an_artinian_ring.md
source_content_sha256: f88ff60a0976a0441aed75f5328135625983a714fc53ed6dc1504425eb26923f
translation_model: gpt-5.4
translation_run: translate-vi-d30757fd
glossary_version: 34
glossary_terms_sha256: 98cac96d18952bdfbc47b61b7a18e9db53dacc76fcfa72e6d84a6257c0fa262e
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 10. MÔĐUN TRÊN MỘT VÀNH ARTIN

### 1. Căn của một vành Artin

#### Mệnh đề 1 {#alg-viii-s10-prop-1 .statement tag=00C5}

Cho A là một vành Artin trái. Căn $\mathfrak{r}$ của A là iđêan hai phía lũy linh lớn nhất của A, và vành $A/\mathfrak{r}$ là nửa đơn.

Ta biết (VIII, p. 156, Định lý 1) rằng mọi iđêan hai phía lũy linh của A đều được chứa trong $\mathfrak{r}$. Ta hãy chứng minh rằng $\mathfrak{r}$ là lũy linh. Vì vành A là Artin trái và dãy các iđêan hai phía $\mathfrak{r}^n$ là giảm, nên tồn tại một số nguyên $p\geqslant 0$ sao cho ta có $\mathfrak{r}^p=\mathfrak{r}^{p+1}$. Vì A là Artin, A-môđun $A_s$ có độ dài hữu hạn (VIII, p. 6, Định lý 1) và do đó là Noether. Vậy iđêan trái $\mathfrak{r}^p$ là sinh hữu hạn. Theo Bổ đề Nakayama (Định lý 2 của VIII, p. 158), suy ra $\mathfrak{r}^p= 0$.

Vành $A/\mathfrak{r}$ không có căn (VIII, p. 155, Mệnh đề 5); vì nó là Artin trái, nên nó là nửa đơn (VIII, p. 154, Mệnh đề 4).

#### Hệ quả 1 {#alg-viii-s10-prop-1-cor-1 .statement tag=00C6}

Một vành là nửa đơn khi và chỉ khi nó là Artin trái và không có iđêan hai phía lũy linh nào khác 0.

Một vành nửa đơn là Artin trái và không có căn (VIII, p. 154, Mệnh đề 4); do đó nó không có iđêan hai phía lũy linh nào khác 0. Chiều đảo lại suy ra từ Mệnh đề 1.

#### Hệ quả 2 {#alg-viii-s10-prop-1-cor-2 .statement tag=00C7}

Trong một vành Artin trái A, căn gồm các phần tử $x$ sao cho ax lũy linh với mọi $a$ trong A.

Nếu A là Artin trái, thì căn là một iđêan hai phía lũy linh (Mệnh đề 1). Mọi iđêan nil trái đều được chứa trong căn theo định lý của Jacobson (VIII, p. 156, Định lý 1). Suy ra Hệ quả 2.

### 2. Môđun trên một vành Artin

#### Mệnh đề 2 {#alg-viii-s10-prop-2 .statement tag=00C8}

Cho A là một vành Artin trái. Với mọi A-môđun M, các tính chất sau là tương đương:

(i) M là nửa đơn.

(ii) M không có căn.

(iii) M bị triệt tiêu bởi căn $\mathfrak{r}$ của A.

Ta biết rằng (i) kéo theo (ii) (VIII, p. 153, Mệnh đề 3). Mặt khác, $\mathfrak{r}M$ được chứa trong căn của M (VIII, p. 158, Mệnh đề 6), nên (ii) kéo theo (iii).

Giả sử A-môđun M bị triệt tiêu bởi $\mathfrak{r}$. Ta có thể xem nó như một môđun trên vành $A/\mathfrak{r}$. Mà vành $A/\mathfrak{r}$ là nửa đơn (VIII, p. 173, Mệnh đề 1), và mọi môđun trên một vành nửa đơn đều là nửa đơn (VIII, p. 138, Mệnh đề 4). Do đó, M là một môđun nửa đơn trên vành $A/\mathfrak{r}$ và a fortiori trên vành A. Vậy (iii) suy ra (i).

#### Hệ quả {#alg-viii-s10-n2-cor-1 .statement tag=00C9}

Cho A là một vành Artin trái. Với mọi A-môđun M, căn của M bằng $\mathfrak{r}M$.

Căn $\mathfrak{R}(M)$ của M chứa $\mathfrak{r}M$ (VIII, p. 158, Mệnh đề 6). Hơn nữa, A-môđun $M/\mathfrak{r}M$ bị triệt tiêu bởi $\mathfrak{r}$. Bởi Mệnh đề 2, do đó nó không có căn, điều này suy ra $\mathfrak{R}(M)\subset \mathfrak{r}M$ (VIII, p. 152, Hệ quả 1, c)).

#### Mệnh đề 3 {#alg-viii-s10-prop-3 .statement tag=00CA}

Cho A và B là các vành và $f$ là một đồng cấu từ A vào B sao cho B được sinh bởi hợp của $f(A)$ và hoán tập $f(A)'$ của $f(A)$ trong B. Cho M là một B-môđun trái. Giả sử rằng hoặc vành A là Artin trái hoặc A-môđun $f_*(M)$ suy ra từ M bởi hạn chế vô hướng (II, §1, No. 13, p. 221) là sinh hữu hạn. Khi đó ta có $\mathfrak{R}_A(f_*(M))\subset \mathfrak{R}_B(M)$.

Cho S là một B-môđun đơn. Giả sử rằng hoặc A là Artin trái hoặc A-môđun $f_*(S)$ là sinh hữu hạn. Ta sẽ chứng minh rằng $f_*(S)$ không có căn. Với mọi $b\in f(A)'$, phép vị tự $b_S$ là một tự đồng cấu của A-môđun $f_*(S)$ và do đó bảo toàn $\mathfrak{R}_A(f_*(S))$ (VIII, p. 152, Mệnh đề 1). Vì B được sinh bởi $f(A)\cup f(A)'$, căn $\mathfrak{R}_A(f_*(S))$ là một B-môđun con của S, nên bằng 0 hoặc S. Nếu $f_*(S)$ là một A-môđun sinh hữu hạn, thì ta có $\mathfrak{R}_A(f_*(S))\not=f_*(S)$ (VIII, p. 153, Mệnh đề 2). Nếu vành A là Artin trái, thì ta có $\mathfrak{R}_A(f_*(S)) =f(\mathfrak{r})S$, trong đó $\mathfrak{r}$ là căn của A (VIII, p. 174, Hệ quả của Mệnh đề 2), và vì $\mathfrak{r}$ là một iđêan hai phía lũy linh của A (VIII, p. 173, Mệnh đề 1), ta không thể có $S =f(\mathfrak{r})S$. Vậy trong cả hai trường hợp ta đều có $\mathfrak{R}_A(f_*(S)) = 0$.

Cho $u$ là một ánh xạ B-tuyến tính khác không từ M vào một B-môđun đơn S. Ánh xạ $u$ là toàn ánh; do đó, nếu $f_*(M)$ là sinh hữu hạn, thì $f_*(S)$ cũng vậy. Dưới các giả thiết của Mệnh đề 3, A-môđun $f_*(S)$ không có căn và $u$ là một ánh xạ A-tuyến tính từ $f_*(M)$ vào $f_*(S)$. Vậy hạt nhân của $u$ chứa $\mathfrak{R}_A(f_*(M))$ theo Mệnh đề 1 của VIII, p. 152. Vì $u$ là tùy ý, ta có $\mathfrak{R}_A(f_*(M))\subset \mathfrak{R}_B(M)$.

#### Hệ quả {#alg-viii-s10-n2-cor-2 .statement tag=00CB}

Cho A là một vành giao hoán và B là một đại số trên A. Giả sử rằng hoặc vành A là Artin hoặc B là một A-môđun hữu hạn sinh. Khi đó ta có $\mathfrak{R}(A)B\subset \mathfrak{R}(B)$.

Theo Mệnh đề 3, căn $\mathfrak{R}_A(B_s)$ được chứa trong $\mathfrak{R}_B(B_s)$, mà không gì khác hơn là căn của vành B. Hơn nữa, ta có $\mathfrak{R}(A)B\subset \mathfrak{R}_A(B_s)$ theo Mệnh đề 6 của VIII, p. 158. Hệ quả suy ra.

### 3. Các môđun xạ ảnh trên một vành Artin

#### Mệnh đề 4 {#alg-viii-s10-prop-4 .statement tag=00CC}

Mọi môđun trên một vành Artin trái đều có một bao xạ ảnh.

Cho A là một vành Artin trái, và M là một môđun trên A. Căn $\mathfrak{r}$ của A là một iđêan hai phía lũy linh, và vành $A/\mathfrak{r}$ là nửa đơn (VIII, p. 173, Mệnh đề 1). Suy ra $A/\mathfrak{r}$-môđun $M/\mathfrak{r}M$ là xạ ảnh. Khi đó mệnh đề được suy ra từ Mệnh đề 11 của VIII, p. 164.

#### Mệnh đề 5 {#alg-viii-s10-prop-5 .statement tag=00CD}

Cho A là một vành Artin trái và $\mathfrak{r}$ là căn của nó.

a) Cho P là một A-môđun xạ ảnh. Ký hiệu ánh xạ chính tắc từ P đến $P/\mathfrak{r}P$ là $u$. Khi đó $(P, u)$ là một bao xạ ảnh của $P/\mathfrak{r}P$. Đặc biệt, A-môđun P sinh hữu hạn khi và chỉ khi $P/\mathfrak{r}P$ sinh hữu hạn.

b) Cho M là một môđun trên vành $A/\mathfrak{r}$. Khi đó M, được xem như một A-môđun, có một bao xạ ảnh. Nếu $(P, u)$ là một bao xạ ảnh như vậy, thì khi chuyển qua thương, $u$ cảm sinh một đẳng cấu từ $P/\mathfrak{r}P$ lên M. Hơn nữa, P không phân tích được khi và chỉ khi M là đơn.

c) Cho M và $M'$ là các môđun trên vành $A/\mathfrak{r}$. Cho $(P, u)$ và $(P', u')$ là các bao xạ ảnh của các A-môđun M và $M'$. Khi đó M và $M'$ đẳng cấu khi và chỉ khi P và $P'$ đẳng cấu.

Căn $\mathfrak{r}$ của A là một iđêan hai phía lũy linh (VIII, p. 173, Mệnh đề 1). Do đó mệnh đề a) suy ra từ Hệ quả 1 của VIII, p. 163 và Nhận xét 2 của VIII, p. 161.

Ta chứng minh mệnh đề b). Sự tồn tại của một bao xạ ảnh $(P, u)$ của M suy ra từ Mệnh đề 4 và đẳng cấu từ $P/\mathfrak{r}P$ lên M của Mệnh đề 9 trong VIII, p. 162. Vì vành $A/\mathfrak{r}$ là nửa đơn, một môđun trên vành này không phân tích được khi và chỉ khi nó là đơn. Khi đó khẳng định cuối cùng suy ra từ Hệ quả 2 của VIII, p. 160.

Ta hãy chứng minh c). Cho $f$ là một đẳng cấu từ P lên $P'$; nó cảm sinh một đẳng cấu $\overline{f}$ từ $P/\mathfrak{r}P$ lên $P'/\mathfrak{r}P'$. Theo b), các thương này lần lượt đẳng cấu với M và $M'$. Do đó, M đẳng cấu với $M'$. Ngược lại, theo Mệnh đề 8 của VIII, p. 161, mọi đẳng cấu $f$ từ M lên $M'$ đều nâng thành một đẳng cấu $\widetilde{f}$ từ P lên $P'$ sao cho $f\circ u=u'\circ \widetilde{f}$.

#### Hệ quả {#alg-viii-s10-n3-cor-1 .statement tag=00CE}

Với mỗi lớp P của các A-môđun xạ ảnh, gán lớp $\varphi (P)$ của môđun $P/\mathfrak{r}P$ trên vành $A/\mathfrak{r}$. Mọi lớp môđun (tương ứng, lớp môđun sinh hữu hạn) trên vành $A/\mathfrak{r}$ đều có dạng $\varphi (P)$ với một lớp P duy nhất của các A-môđun xạ ảnh (tương ứng, của các A-môđun xạ ảnh sinh hữu hạn).

Cho A là một vành Artin trái và $\mathfrak{r}$ là căn của nó. Ký hiệu tập hợp các lớp môđun đơn là $\mathscr{S}$; tập hợp này là hữu hạn (VIII, p. 51). Theo Mệnh đề 2 của VIII, p. 174, nó có thể được đồng nhất một cách chính tắc với tập hợp các lớp môđun đơn trên vành nửa đơn $A/\mathfrak{r}$. Với mọi $\lambda \in \mathscr{S}$, lấy $S_{\lambda}$ là một A-môđun đơn thuộc lớp $\lambda$, và chọn một bao xạ ảnh $(P_{\lambda}, u_{\lambda})$ của $S_{\lambda}$ (VIII, p. 175, Mệnh đề 4). Theo Mệnh đề 5, A-môđun $P_{\lambda}$ là xạ ảnh và không phân tích được, và $u_{\lambda}$ xác định một đẳng cấu từ $P_{\lambda}/\mathfrak{r}P_{\lambda}$ lên $S_{\lambda}$. Hơn nữa, nếu P là một A-môđun xạ ảnh và không phân tích được, thì tồn tại duy nhất một $\lambda \in \mathscr{S}$ sao cho P đẳng cấu với $P_{\lambda}:$ đó là $\lambda \in \mathscr{S}$ duy nhất sao cho $P/\mathfrak{r}P$ đẳng cấu với $S_{\lambda}$.

#### Mệnh đề 6 {#alg-viii-s10-prop-6 .statement tag=00CF}

Cho A là một vành Artin trái và $\mathfrak{r}$ là căn của nó. Cho P là một A-môđun xạ ảnh.

a) A-môđun $\overline{P}= P/\mathfrak{r}P$ là nửa đơn, và A-môđun P đẳng cấu với $\bigoplus_{\lambda\in\mathscr{S}}P^{([P:\lambda])}_{\lambda}$.

b) Cho $(Q_i)_{i\in I}$ là một họ các môđun con xạ ảnh không phân tích được của P có tổng trực tiếp là P. Khi đó với mọi $\lambda \in \mathscr{S}$, lực lượng của tập hợp $I(\lambda )$ các $i\in I$ sao cho $Q_i$ đẳng cấu với $P_{\lambda}$ bằng $[P :\lambda ]$.

Việc $\overline{P}$ là nửa đơn suy ra từ Mệnh đề 2 (VIII, p. 174). A-môđun $Q =\oplus_{\lambda\in\mathscr{S}}P^{([P:\lambda])}_{\lambda}$ là xạ ảnh. Vì $P_{\lambda}/\mathfrak{r}P_{\lambda}$ đẳng cấu với $S_{\lambda}$, nên thương $Q/\mathfrak{r}Q$ đẳng cấu với $\oplus_{\lambda\in\mathscr{S}}S^{([P:\lambda])}_{\lambda}$, tức là với $\overline{P}= P/\mathfrak{r}P$. Theo Mệnh đề 5, các A-môđun P và Q đẳng cấu với nhau.

Giả sử cho một họ $(Q_i)_{i\in I}$ các môđun con xạ ảnh và không phân tích được có tổng trực tiếp là P. Theo Mệnh đề 5, A-môđun $Q_i/\mathfrak{r}Q_i$ là đơn với mọi $i\in I$. Với $\lambda \in \mathscr{S}$, ký hiệu bởi $I(\lambda )$ tập hợp các $i\in I$ sao cho $Q_i/\mathfrak{r}Q_i$ đẳng cấu với $S_{\lambda}$, do đó với $P_{\lambda}/\mathfrak{r}P_{\lambda}$; đó cũng là tập hợp các $i\in I$ sao cho $Q_i$ đẳng cấu với $P_{\lambda}$. Vì $\overline{P}= P/\mathfrak{r}P$ là tổng trực tiếp của họ $(Q_i/\mathfrak{r}Q_i)_{i\in I}$, nên ta có Card(I($\lambda$ )) $= [P :\lambda ]$ theo Định lý 1 của VIII, p. 32.

#### Ví dụ {#alg-viii-s10-n3-exa-1 .statement tag=00CG}

Lấy P bằng $A_s$. Với $\lambda \in \mathscr{S}$, ký hiệu trường đối của hoán tập của A-môđun đơn $S_{\lambda}$ bởi $D_{\lambda}$ và chiều của $S_{\lambda}$ khi được xem như một không gian vectơ phải trên trường $D_{\lambda}$ bởi $m(\lambda )$. Ta biết rằng $m(\lambda )$ bằng bội số $[A_s/\mathfrak{r}A_s:\lambda ]$ (VIII, p. 143, Mệnh đề 11). Do đó, A-môđun $A_s$ đẳng cấu với $\oplus_{\lambda\in\mathscr{S}}P^{m(\lambda)}_{\lambda}$.

### Bài tập {#alg-viii-s10-exercises}

Xem [các bài tập cho § 10](exercises/s10/).
