---
book: ts
book_title: Théories spectrales
chapter: III
chapter_title: APPLICATIONS LINÉAIRES COMPACTES ET PERTURBATIONS
section: 1
section_title: Applications linéaires compactes
lang: vi
source: ts-iii-v-fr
book_pages: TS III.2-TS III.23, TS III.103-TS III.118
pdf_pages: 0016-0037, 0117-0132
extraction: native
subsections:
    - "no": 1
      title: Applications linéaires compactes
      page: 2
      pdf_page: 16
    - "no": 2
      title: Applications linéaires compactes et topologies faibles
      page: 6
      pdf_page: 20
    - "no": 3
      title: Transposition
      page: 8
      pdf_page: 22
    - "no": 4
      title: Le théorème de Leray–Schauder
      page: 10
      pdf_page: 24
    - "no": 5
      title: Sous-espaces invariants par un opérateur compact
      page: 12
      pdf_page: 26
    - "no": 6
      title: Espaces d’approximation
      page: 14
      pdf_page: 28
    - "no": 7
      title: Exemples d’espaces d’approximation
      page: 20
      pdf_page: 34
statements: 57
exercises: 37
content_sha256: 638f4f6afd1ab2f37fc286808023c625d297a0eb9d7e2c7b2c096d6873347e92
translated_from: content/en-mt/ts/III/01_s1_applications_lineaires_compactes.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 92b75882bce16b6824c3479ff9597eedf1b6caa70b690c86dad0dce89c28a961
translation_model: gpt-5.4
translation_run: translate-vi-f16ad3e3
glossary_version: 34
glossary_terms_sha256: 4bb4a48b0232a0650b76b31c368998ce43a8d389305cd983708380e65fe5feaf
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 1. ÁNH XẠ TUYẾN TÍNH COMPACT

### 1. Ánh xạ tuyến tính compact

#### Định nghĩa 1 {#ts-iii-s1-def-1 .statement tag=02NY}

Cho E là một không gian vectơ tôpô và F là một không gian vectơ tôpô tách biệt. Một ánh xạ tuyến tính $u$ từ E vào F được gọi là compact nếu tồn tại một lân cận V của 0 trong E sao cho $u(V)$ là một tập con tương đối compact của F.

Ta ký hiệu bởi $\mathscr{L}^c(E; F)$ tập hợp các ánh xạ tuyến tính compact từ E vào F; ta cũng ký hiệu bởi $\mathscr{L}^c(F)$ tập $\mathscr{L}^c(F; F)$.

#### Nhận xét 1 {#ts-iii-s1-n1-rem-1 .statement tag=02NZ}

Một lân cận của 0 trong E hấp thụ mọi tập con bị chặn của E; do đó ảnh của một tập con bị chặn của E qua một ánh xạ tuyến tính compact từ E vào F là một tập con tương đối compact của F.

#### Nhận xét 2 {#ts-iii-s1-n1-rem-2 .statement tag=02O0}

Cho E là một không gian nửa chuẩn và B là quả cầu đơn vị của E. Để một ánh xạ tuyến tính $u$ từ E vào một không gian vectơ tôpô tách biệt F là compact, điều kiện cần và đủ là $u(B)$ là một tập con tương đối compact của F.

#### Nhận xét 3 {#ts-iii-s1-n1-rem-3 .statement tag=02O1}

Cho F là một không gian vectơ tôpô tách biệt. Để một không gian con vectơ E của F có số chiều hữu hạn, điều kiện cần và đủ là đơn ánh chính tắc của E vào F là compact (EVT, I, p. 15, th. 3).

#### Nhận xét 4 {#ts-iii-s1-n1-rem-4 .statement tag=02O2}

Với mọi không gian vectơ tôpô E trên trường $\mathbf{R}$, ta ký hiệu bởi $E_{(\mathbf{C})}$ không gian vectơ tôpô phức hoá của E (EVT, II, p. 65). Ta đồng nhất E với một không gian con vectơ tôpô thực của $E_{(\mathbf{C})}$ bởi ánh xạ $x\mapsto 1\otimes x$; khi đó không gian vectơ tôpô thực nền của $E_{(\mathbf{C})}$ là tổng trực tiếp tôpô của E và $iE$.

Cho $u$ là một ánh xạ tuyến tính từ E vào một không gian vectơ tôpô tách biệt F trên $\mathbf{R}$. Gọi $u_{(\mathbf{C})}$ là ánh xạ $\mathbf{C}$-tuyến tính từ $E_{(\mathbf{C})}$ vào $F_{(\mathbf{C})}$ kéo dài $u$. Các tập hợp dạng $V +iV$, trong đó V là một lân cận của 0 trong E, tạo thành một hệ cơ bản các lân cận của 0 trong $E_{(\mathbf{C})}$. Để tập $u_{(\mathbf{C})}(V +iV) =u(V) +iu(V)$ là tương đối compact trong $F_{(\mathbf{C})}$, điều kiện cần và đủ là $u(V)$ tương đối compact trong F. Do đó, để ánh xạ $\mathbf{C}$-tuyến tính $u_{(\mathbf{C})}$ là compact, điều kiện cần và đủ là ánh xạ $\mathbf{R}$-tuyến tính $u$ cũng vậy.

Theo cùng một ý tưởng, khi $v$ là một ánh xạ $\mathbf{C}$-tuyến tính liên tục từ $E_{(\mathbf{C})}$ vào một không gian vectơ tôpô $\mathbf{C}$ G, để $v$ là compact thì điều kiện cần và đủ là hạn chế của nó lên E là compact.

#### Nhận xét 5 {#ts-iii-s1-n1-rem-5 .statement tag=02O3}

Cho E là một không gian vectơ tôpô, F là một không gian vectơ tôpô tách biệt. Cho $F_1$ là một không gian con vectơ đóng của F và gọi $j$ là đơn ánh chính tắc của $F_1$ vào F. Để một ánh xạ tuyến tính $u$ từ E vào $F_1$ là compact, điều kiện cần và đủ là ánh xạ tuyến tính $j\circ u$ từ E vào F cũng vậy.

#### Nhận xét 6 {#ts-iii-s1-n1-rem-6 .statement tag=02O4}

Cho $(G_i)_{i\in I}$ là một họ các không gian vectơ tôpô tách biệt, và với mỗi $i\in I$, cho $u_i$ là một ánh xạ tuyến tính compact từ một không gian vectơ tôpô E vào $G_i$. Nếu tập I là hữu hạn, hoặc nếu E là một không gian nửa chuẩn, thì ánh xạ tuyến tính $x\mapsto (u_i(x))_{i\in I}$ từ E vào $\prod_{i\in I}G_i$ là compact (nhận xét 2 và TG, I, p. 63, th. 3).

#### Mệnh đề 1 {#ts-iii-s1-prop-1 .statement tag=02O5}

Cho E là một không gian vectơ tôpô và F là một không gian vectơ tôpô tách biệt.

a) Mọi ánh xạ tuyến tính compact từ E vào F đều liên tục ;

b) Mọi ánh xạ tuyến tính liên tục hạng hữu hạn từ E vào F đều compact;

c) Tập $\mathscr{L}^c(E; F)$ các ánh xạ tuyến tính compact từ E vào F là một không gian con vectơ của $\mathscr{L}(E; F)$.

Ta chứng minh a). Cho $v: E\rightarrow F$ là một ánh xạ tuyến tính compact và U là một lân cận của 0 trong F. Chọn một lân cận V của 0 trong E sao cho $v(V)$ tương đối compact trong F. Khi đó $v(V)$ bị chặn và do đó tồn tại một số thực $\lambda  >0$ sao cho tập $v(\lambda V)$ được chứa trong U; do đó, $v$ liên tục.

Cho $u: E\rightarrow F$ là một ánh xạ tuyến tính liên tục hạng hữu hạn. Vì ảnh $u(E)$ của $u$ là tách và có số chiều hữu hạn, tồn tại một lân cận compact A của 0 trong $u(E)$. Tập hợp $V =\overset{-1}{u}(A)$ là một lân cận của 0 trong E và ta có $u(V)\subset A$, do đó ánh xạ tuyến tính $u$ là compact. Điều này chứng minh mệnh đề b).

Cho $u_1$ và $u_2$ là các ánh xạ tuyến tính compact từ E vào F. Cho $V_1$ và $V_2$ là các lân cận của 0 trong E sao cho các tập hợp $u_1(V_1)$ và $u_2(V_2)$ là tương đối compact trong F. Đặt $V = V_1\cap V_2$ và $u=u_1+u_2$. Khi đó $u(V)$ được chứa trong $u_1(V_1) +u_2(V_2)$, do đó là tương đối compact trong F, và ánh xạ tuyến tính $u$ là compact. Ngay lập tức thấy rằng $\mathscr{L}^c(E; F)$ ổn định dưới phép vị tự. Điều này chứng minh rằng $\mathscr{L}^c(E; F)$ là một không gian con vectơ của $\mathscr{L}(E; F)$, do đó mệnh đề c).

#### Mệnh đề 2 {#ts-iii-s1-prop-2 .statement tag=02O6}

Cho E là một không gian nửa chuẩn và F là một không gian vectơ tôpô tách. Giả sử rằng mọi tập con đóng bị chặn của F đều đầy đủ. Khi đó không gian con vectơ $\mathscr{L}^c(E; F)$ của $\mathscr{L}(E; F)$ là đóng đối với tôpô hội tụ bị chặn.

Cho $u$ là một phần tử của $\mathscr{L}(E; F)$ thuộc bao đóng của $\mathscr{L}^c(E; F)$ đối với tôpô hội tụ bị chặn. Ký hiệu bởi B quả cầu đơn vị của E và bởi V một lân cận của 0 trong F. Chọn một lân cận W của 0 trong F sao cho $W + W\subset V$. Theo giả thiết, tồn tại một phần tử $v$ của $\mathscr{L}^c(E; F)$ sao cho $(u-v)(B)\subset W$. Vì tập hợp $v(B)$ là tương đối compact trong F, tồn tại một tập con hữu hạn M của F sao cho $v(B)\subset M + W$, do đó $u(B)\subset M + V$. Vì điều này đúng với mọi V, tập hợp $u(B)$ là tiền compact trong F, do đó bao đóng của nó cũng vậy (TG, II, prop. 1, p. 30). Vì tập sau là đóng và bị chặn, nó đầy đủ theo giả thiết đặt lên F, và do đó compact (TG, II, cor., p. 30). Suy ra rằng $u(B)$ là tương đối compact. Điều này chứng minh rằng $u$ thuộc $\mathscr{L}^c(E; F)$.

Nếu F lồi địa phương, giả thiết của mệnh đề có nghĩa là F là gần đầy đủ (EVT, III, p. 8, déf. 6).

#### Hệ quả {#ts-iii-s1-n1-cor-1 .statement tag=02O7}

Cho E và F là các không gian Banach. Tập hợp $\mathscr{L}^c(E; F)$ là một không gian con vectơ đóng của không gian Banach $\mathscr{L}(E; F)$. Nó chứa bao đóng của không gian $\mathscr{L}^f(E; F)$ gồm các ánh xạ tuyến tính liên tục hạng hữu hạn từ E vào F.

Điều này suy ra từ các Mệnh đề 1 và 2.

Tồn tại các không gian Banach E và F sao cho $\mathscr{L}^f(E; F)$ không trù mật trong $\mathscr{L}^c(E; F) ($cf. Nhận xét 6 của III, p. 16 và Định lý 4 của III, p. 19, b)).

#### Mệnh đề 3 {#ts-iii-s1-prop-3 .statement tag=02O8}

Cho $E_1$, E, F, $F_1$ là các không gian vectơ tôpô, trong đó F và $F_1$ được giả sử là tách. Cho $v: E_1\rightarrow E,u: E\rightarrow F$ và $w: F\rightarrow F_1$ là các ánh xạ tuyến tính. Nếu $v$ và $w$ liên tục và $u$ compact, thì $w\circ u\circ v$ là compact.

Theo giả thiết, tồn tại một lân cận V của 0 trong E sao cho $u(V)$ là tương đối compact trong F. Đặt $U =\overset{-1}{v}(V)$. Khi đó U là một lân cận của 0 trong $E_1$ và ảnh của nó bởi $w\circ u\circ v$ được chứa trong $w(u$(V)), do đó là tương đối compact trong $F_1$. Vậy ánh xạ tuyến tính $w\circ u\circ v$ là compact.

Cho E là một không gian vectơ tôpô tách được; theo các Mệnh đề 1 và 3, $\mathscr{L}^c(E)$ là một iđêan hai phía của đại số $\mathscr{L}(E)$. Khi E là một không gian Banach, $\mathscr{L}(E)$ là một đại số Banach và $\mathscr{L}^c(E)$ là một iđêan hai phía đóng của $\mathscr{L}(E)$ (hệ quả của Mệnh đề 2). Nó là một iđêan thực sự nếu E có chiều vô hạn (xem Nhận xét 3, p. 2).

#### Hệ quả {#ts-iii-s1-n1-cor-2 .statement tag=02O9}

Cho E là một không gian Hilbert. Không gian $\mathscr{L}^c(E)$ là một iđêan hai phía tự liên hợp đóng của $\mathscr{L}(E)$. Đặc biệt, nó là một đại số sao.

Thật vậy, không gian $\mathscr{L}^c(E)$ là một iđêan hai phía đóng, do đó tự liên hợp, của $\mathscr{L}(E)$ (Bổ đề 15 của I, p. 122).

#### Mệnh đề 4 {#ts-iii-s1-prop-4 .statement tag=02OA}

Cho E là một không gian vectơ tôpô, $\widehat{E}$ là hoàn thành tách được của nó và $j$ là ánh xạ chính tắc từ E vào $\widehat{E}$. Cho $u$ là một ánh xạ tuyến tính compact từ E vào một không gian vectơ tôpô tách được F. Khi đó tồn tại một ánh xạ tuyến tính compact duy nhất $v$ từ $\widehat{E}$ vào F sao cho $u=v\circ j$.

Đồng nhất F với một không gian con vectơ tôpô của $\widehat{F}$ và ký hiệu bởi $\widehat{u}:\widehat{E}\rightarrow \widehat{F}$ ánh xạ tuyến tính liên tục duy nhất sao cho $\widehat{u}\circ j$ trùng với $u$ trên E. Vì $u$ là compact, tồn tại một lân cận V của 0 trong E và một tập con compact A của F sao cho $u(V)\subset A$. Ta có $\widehat{u}(j(V))\subset A$, do đó $\widehat{u}(j(V))\subset A$. Bây giờ $j(V)$ là một lân cận của 0 trong $\widehat{E}$ (TG, III, p. 24, Mệnh đề 7). Suy ra ảnh của $\widehat{u}$ được chứa trong F và ánh xạ tuyến tính liên tục $v:\widehat{E}\rightarrow F$ suy ra từ $\widehat{u}$ bằng cách chuyển qua không gian con là compact. Vì $j(E)$ trù mật trong $\widehat{E}$, ánh xạ $v$ là ánh xạ tuyến tính liên tục duy nhất từ $\widehat{E}$ vào F sao cho $u=v\circ j$.

#### Mệnh đề 5 {#ts-iii-s1-prop-5 .statement tag=02OB}

Cho E là một không gian lồi địa phương, F là một không gian vectơ tôpô tách được và $u$ là một ánh xạ tuyến tính compact từ E vào F. Khi đó tồn tại một không gian Banach G, một ánh xạ tuyến tính liên tục $v$ từ E vào G và một ánh xạ tuyến tính compact $w$ từ G vào F sao cho $u=w\circ v$.

Cho V là một lân cận của 0 trong E sao cho $u(V)$ là compact tương đối trong F. Cho $p$ là một nửa chuẩn liên tục trên E sao cho V chứa quả cầu đơn vị của $p$ (EVT, II, p. 26, hệ quả). Ký hiệu bởi $E_p$ không gian nửa chuẩn nhận được bằng cách trang bị cho E nửa chuẩn $p$. Ánh xạ $u$ là một ánh xạ tuyến tính compact từ $E_p$ vào F. Hoàn thành tách được G của $E_p$ là một không gian Banach. Ký hiệu bởi $v$ ánh xạ tuyến tính chính tắc từ $E_p$ vào G. Theo Mệnh đề 4, tồn tại một ánh xạ tuyến tính compact $w: G\rightarrow F$ sao cho $u=w\circ v$. Mặt khác, $v$ là một ánh xạ liên tục từ E vào G vì tôpô của E mịn hơn tôpô của $E_p$.

### 2. Các ánh xạ tuyến tính compact và các tôpô yếu

Cho E là một không gian lồi địa phương, $E'$ là đối ngẫu của nó. Nhớ rằng tôpô $\sigma (E,E')$ trên E được gọi là tôpô yếu trên E (EVT, IV, p. 4). Trong số này, $E_{\sigma}$ ký hiệu không gian E được trang bị tôpô yếu.

#### Mệnh đề 6 {#ts-iii-s1-prop-6 .statement tag=02OC}

Cho E là một không gian lồi địa phương, F là một không gian lồi địa phương tách được, $u: E\rightarrow F$ là một ánh xạ tuyến tính compact và B là một tập con bị chặn của E. Hạn chế của $u$ lên B là một ánh xạ liên tục từ tập hợp B, được trang bị tôpô cảm sinh bởi $\sigma (E,E')$, vào không gian F.

Ánh xạ $u$ là một ánh xạ tuyến tính liên tục từ E vào F, và cũng từ $E_{\sigma}$ vào $F_{\sigma}$. Do đó hạn chế của nó lên B là một ánh xạ liên tục của tập hợp B, được trang bị tôpô cảm sinh bởi $\sigma (E,E')$, vào không gian $F_{\sigma}$. Bây giờ tập hợp $u(B)$ được chứa trong một tập con compact C của F (nhận xét 1 của III, p. 2) và không gian $F_{\sigma}$ là tách, nên các tôpô cảm sinh trên C bởi tôpô của F và của $F_{\sigma}$ trùng nhau. Mệnh đề được suy ra.

#### Hệ quả {#ts-iii-s1-n2-cor-1 .statement tag=02OD}

Cho $(x_n)_{n\in\mathbf{N}}$ là một dãy các điểm của E, hội tụ đến một điểm $x$ của E đối với tôpô yếu đi. Dãy $(u(x_n))_{n\in\mathbf{N}}$ hội tụ trong F đến $u(x)$.

Thật vậy, tập hợp gồm điểm $x$ và các điểm của dãy $(x_n)_{n\in\mathbf{N}}$ là một tập con bị chặn của E (EVT, III, p. 3, hệ quả của mệnh đề 2).

#### Mệnh đề 7 {#ts-iii-s1-prop-7 .statement tag=02OE}

Cho E là một không gian nửa chuẩn, $E'$ đối ngẫu của nó, B quả cầu đơn vị của $E'$ và $u$ là một ánh xạ tuyến tính từ $E'$ vào một không gian lồi địa phương tách F. Nếu hạn chế của $u$ lên B, được trang bị tôpô cảm sinh bởi $\sigma (E',E)$, là liên tục, thì $u(B)$ là một tập con compact của F và $u$ là một ánh xạ tuyến tính compact từ đối ngẫu mạnh $E'_b$ của E vào F.

Thật vậy tập hợp B, được trang bị tôpô cảm sinh bởi $\sigma (E',E)$, là compact (EVT, III, p. 17, hệ quả 2).

#### Hệ quả 1 {#ts-iii-s1-prop-7-cor-1 .statement tag=02OF}

Cho E là một không gian nửa chuẩn kiểu đếm được, cho $E'$ là đối ngẫu của nó và cho B là quả cầu đơn vị của $E'$. Cho $u$ là một ánh xạ tuyến tính từ $E'$ vào một không gian lồi địa phương tách F. Giả sử rằng với mọi dãy $(x_n)_{n\in\mathbf{N}}$ gồm các phần tử của B hội tụ đến 0 theo $\sigma (E',E)$, dãy $(u(x_n))_{n\in\mathbf{N}}$ hội tụ đến 0 trong F. Khi đó, $u(B)$ là một tập con compact của F và $u$ là một ánh xạ tuyến tính compact từ đối ngẫu mạnh $E'_b$ của E vào F.

Thật vậy, tôpô cảm sinh trên B bởi $\sigma (E',E)$ là mêtric hóa được (EVT, III, p. 19, hệ quả 2). Do đó giả thiết của hệ quả kéo theo rằng hạn chế của $u$ lên B là một ánh xạ liên tục từ B vào F, khi B được trang bị tôpô $\sigma (E',E)$, và hệ quả suy ra từ mệnh đề trước.

#### Hệ quả 2 {#ts-iii-s1-prop-7-cor-2 .statement tag=02OG}

Cho E là một không gian nửa chuẩn và $\mathfrak{S}$ là một tập hợp các tập con tiền compact của E mà hợp của chúng là trù mật trong E. Ký hiệu $E'_b$ là đối ngẫu mạnh của E và $E'_{\mathfrak{S}}$ là đối ngẫu của E được trang bị $\mathfrak{S}$-tôpô. Không gian $E'_{\mathfrak{S}}$ là tách và ánh xạ đồng nhất từ $E'_b$ vào $E'_{\mathfrak{S}}$ là compact.

Không gian $E'_{\mathfrak{S}}$ là tách theo TG, X, p. 8, mệnh đề 7; trên quả cầu đơn vị của $E'$, $\mathfrak{S}$-tôpô trùng với tôpô yếu $\sigma (E',E)$ (EVT, III, p. 17, mệnh đề 5), do đó có hệ quả.

#### Ví dụ {#ts-iii-s1-n2-exa-1 .statement tag=02OH}

Cho E là một không gian nửa chuẩn. Ánh xạ đồng nhất từ $E'_b$ vào không gian $E'$, được trang bị tôpô yếu, tôpô hội tụ compact hoặc tôpô hội tụ tiền compact, là compact.

#### Mệnh đề 8 {#ts-iii-s1-prop-8 .statement tag=02OI}

Cho E là một không gian Banach phản xạ, B quả cầu đơn vị của nó, F một không gian lồi địa phương tách và $u: E\rightarrow F$ là một ánh xạ tuyến tính. Các điều kiện sau là tương đương :

(i) Ánh xạ tuyến tính $u$ là compact ;

(ii) Tập hợp $u(B)$ là một tập con compact của F ;

(iii) Hạn chế của $u$ lên B là một ánh xạ liên tục của tập hợp B, được trang bị tôpô cảm sinh bởi $\sigma (E,E')$, vào F ;

(iv) Với mọi dãy $(x_n)_{n\in\mathbf{N}}$ các điểm của B hội tụ đến 0 đối với tôpô $\sigma (E,E')$, dãy $(u(x_n))_{n\in\mathbf{N}}$ hội tụ đến 0 trong F ;

(v) Từ mọi dãy vô hạn các điểm của $u(B)$, có thể trích ra một dãy hội tụ trong F ;

(vi) Mọi dãy vô hạn các điểm của $u(B)$ đều có một giá trị bám trong F.

Vì E là một không gian phản xạ, B là một tập con compact của $E_{\sigma}$ (TVS, IV, p. 17, mệnh đề 6), do đó (iii) suy ra (ii). Điều kiện (ii) suy ra (i) theo định nghĩa, và điều kiện (i) suy ra (iii) theo mệnh đề 6. Cũng là sơ cấp khi thấy rằng (iii) suy ra (iv) và (v) suy ra (vi).

Bây giờ chúng ta sẽ chứng minh rằng (iv) suy ra (v). Cho $(x_n)$ là một dãy vô hạn các điểm của B. Vì B là một tập con compact của $E_{\sigma}$, theo định lý của $\breve{S}$mulian (TVS, IV, p. 36, định lý 2), tồn tại một dãy $(y_n)$, trích từ dãy $(x_n)$, hội tụ trong $E_{\sigma}$ đến một giới hạn $y$. Dãy $(y_n-y)$ bị chặn trong $E_{\sigma}$, nên cũng bị chặn trong E (TVS, IV, p. 1, mệnh đề 1); do đó nó được chứa trong một tập vị tự của B. Nếu điều kiện (iv) được thỏa mãn, dãy $(u(y_n-y))$ hội tụ đến 0 trong F, và $(u(y_n))$, là một dãy trích từ $(u(x_n))$, hội tụ đến $u(y)$. Điều này chứng minh rằng (iv) suy ra (v).

Để kết luận, hãy chứng minh rằng (vi) suy ra (ii). Cho $j: F\rightarrow \widehat{F}$ là đơn ánh chính tắc của F vào không gian hoàn thành của nó. Dưới giả thiết (vi), $u(B)$ là một tập con tiền compact của F (TVS, IV, p. 32, mệnh đề 1), nên $j(u(B))$ là một tập con tương đối compact của $\widehat{F}$ (TG, II, n$^{\circ}2$, p. 29) và $j\circ u$ là một ánh xạ tuyến tính compact. Theo tính tương đương đã chứng minh ở trên của các điều kiện (i) và (ii), $j(u(B))$ là một tập con compact của $\widehat{F}$. Do đó, $u(B)$ là một tập con compact của F.

### 3. Chuyển vị

Cho E là một không gian lồi địa phương và $E'$ là đối ngẫu của nó. Nhắc lại rằng người ta ký hiệu bởi $E'_b$ và $E'_c$ các không gian lồi địa phương thu được bằng cách trang bị cho không gian vectơ $E'$ lần lượt tôpô hội tụ bị chặn và tôpô hội tụ compact (TVS, III, p. 14). Không gian $E'_b$ cũng được gọi là đối ngẫu mạnh của E (loc. cit., ví dụ 4).

#### Mệnh đề 9 {#ts-iii-s1-prop-9 .statement tag=02OJ}

Cho E là một không gian lồi địa phương, F là một không gian lồi địa phương tách và $u$ là một ánh xạ tuyến tính liên tục từ E vào F.

a) Nếu ánh xạ $u$ là compact, thì chuyển vị của nó $^tu$ là một ánh xạ tuyến tính compact từ $F'_c$ vào $E'_c$ và là một ánh xạ tuyến tính liên tục từ $F'_c$ vào $E'_b$;

b) Giả sử rằng không gian E là một không gian nửa chuẩn và không gian F là gần đầy đủ. Nếu chuyển vị $^tu$ là một ánh xạ liên tục từ $F'_c$ vào $E'_b$, thì ánh xạ tuyến tính $u$ là compact.

Trước hết giả sử rằng ánh xạ tuyến tính $u$ là compact. Khi đó tồn tại một lân cận V của 0 trong E mà ảnh của nó dưới $u$ được chứa trong một tập con compact C của F. Theo định nghĩa (TVS, II, p. 47, định nghĩa 2 and p. 68, định nghĩa 1), cực $C^{\circ}$ của C là một lân cận của 0 trong $F'_c$ và ta có $^tu(C^{\circ})\subset V^{\circ}$. Bây giờ $V^{\circ}$ là một tập con đồng liên tục của $E'$, đóng đối với tôpô yếu, nên compact trong $E'_c$ (TVS, III, p. 17, hệ quả 2 and mệnh đề 5). Điều này chứng minh rằng $^tu$ là một ánh xạ tuyến tính compact từ $F'_c$ vào $E'_c$.

Giữ các giả thiết trước đây và cho U là một lân cận của 0 trong $E'_b$. Nó chứa cực $A^{\circ}$ của một tập con bị chặn A của E. Vì ánh xạ tuyến tính $u$ là compact, tập $u(A)$ là tương đối compact trong F (nhận xét 1 của III, p. 2), và $(^tu)^{-1}(A^{\circ}) =u(A)^{\circ}$ là một lân cận của 0 trong $F'_c$. Điều này chứng minh rằng $^tu$ là một ánh xạ tuyến tính liên tục từ $F'_c$ vào $E'_b$.

Bây giờ ta đặt mình dưới các giả thiết của b) và ký hiệu bởi B quả cầu đơn vị của E. Đối cực $B^{\circ}$ của B là quả cầu đơn vị của $E'_b$ và ta có $(^tu)^{-1}(B^{\circ}) =u(B)^{\circ}$. Nếu $^tu$ là một ánh xạ liên tục từ $F'_c$ vào $E'_b$, thì tập $u(B)^{\circ}$ do đó là một lân cận của 0 trong $F'_c$; vì vậy nó chứa đối cực $C^{\circ}$ của một tập con compắc C của F. Theo định lý lưỡng cực (EVT, II, p. 49, cor. 3), tập $u(B)$ được chứa trong bao lồi đóng của $C\cup  \{0\}$; tập này compắc vì không gian F là gần đầy đủ (EVT, III, p. 8). Điều này chứng tỏ rằng ánh xạ tuyến tính $u$ là compắc.

#### Hệ quả 1 (Schauder) {#ts-iii-s1-prop-9-cor-1 .statement tag=02OK}

Cho E là một không gian nửa chuẩn, F một không gian Banach, $E'$ và $F'$ là các đối ngẫu mạnh tương ứng của chúng, và $u$ một ánh xạ tuyến tính liên tục từ E vào F. Các tính chất sau là tương đương:

(i) Ánh xạ tuyến tính $u$ từ E vào F là compắc;

(ii) Ánh xạ tuyến tính $^tu$ từ $F'$ vào $E'$ là compắc;

(iii) Ánh xạ tuyến tính $^tu$ từ $F'_c$ vào $E'$ là liên tục.

Sự tương đương của (i) và (iii) suy ra từ mệnh đề 9, a) và b); hệ quả (iii)$\Rightarrow$(ii) suy ra từ sự kiện rằng ánh xạ đồng nhất từ $F'$ vào $F'_c$ là compắc (hệ quả của mệnh đề 7 của III, p. 7).

Để kết luận, hãy chứng minh rằng điều kiện (ii) kéo theo (i). Giả sử rằng ánh xạ tuyến tính $^tu: F'\rightarrow E'$ là compắc. Từ hệ quả (i)$\Rightarrow$(ii), áp dụng cho $^tu$, suy ra rằng $^{tt}u$ là một ánh xạ tuyến tính compắc từ $E''$ vào $F''$. Ký hiệu bởi $v$ ánh xạ tuyến tính chính tắc từ E vào $E''$; nó liên tục. Vì F được đồng nhất với một không gian con vectơ đóng của $F''$ và vì $u$ trùng với $^t(^tu)\circ v$ trên E, nên từ nhận xét 5 của III, p. 3 suy ra rằng ánh xạ tuyến tính $u$ là compắc.

#### Hệ quả 2 {#ts-iii-s1-prop-9-cor-2 .statement tag=02OL}

Cho E là một không gian nửa chuẩn và F một không gian Banach kiểu đếm được. Cho $u$ là một ánh xạ tuyến tính liên tục từ E vào F. Giả sử rằng với mọi dãy $(y_n)$ các phần tử của $F'$ hội tụ yếu về 0, dãy $(^tu(y_n))$ hội tụ mạnh về 0 trong $E'$. Khi đó ánh xạ tuyến tính $u$ là compắc.

Ký hiệu bởi $B'$ quả cầu đơn vị của $F'$, được trang bị tôpô cảm sinh bởi tôpô $\sigma (F',F)$. Vì F là một không gian Banach kiểu đếm được, $B'$ là một không gian compắc khả mêtric (EVT, III, p. 19, cor. 2). Dưới giả thiết đã nêu, hạn chế của $^tu$ lên $B'$ là một ánh xạ liên tục từ $B'$ vào $E'$ và $^tu(B')$ là một tập con compắc của $E'$. Theo hệ quả 1, ánh xạ tuyến tính $u$ là compắc.

#### Nhận xét {#ts-iii-s1-n3-rem-1 .statement tag=02OM}

Cho E và F là các không gian lồi địa phương tách được. Chuyển vị của một ánh xạ tuyến tính compắc từ E vào F không phải luôn luôn là một ánh xạ tuyến tính compắc từ $F'_b$ vào $E'_b($cf. III, p. 108, exercise 15).

### 4. Định lý Leray-Schauder

Định lý sau sẽ được chứng minh trong TA, sẽ xuất hiện.

#### Định lý 1 (Brouwer) {#ts-iii-s1-thm-1 .statement tag=02ON}

Cho B là một tập con lồi compắc khác rỗng của một không gian vectơ chuẩn hữu hạn chiều. Mọi ánh xạ liên tục từ B vào B đều có một điểm bất động.

Ta sẽ suy ra từ đó kết quả sau đây.

#### Định lý 2 (Leray-Schauder) {#ts-iii-s1-thm-2 .statement tag=02OO}

Cho X là một không gian tôpô compắc khác rỗng, đồng phôi với một tập con lồi của một không gian lồi địa phương. Mọi ánh xạ liên tục từ X vào X đều có một điểm bất động.

Có thể giả sử rằng X là một tập con lồi của một không gian lồi địa phương E. Cho N là bao đóng của $\{0\}$ trong E và $\pi : E\rightarrow E/N$ là toàn cấu chính tắc. Vì X là một không gian tách được, hạn chế của $\pi$ lên X là đơn ánh; vì X compắc, nên do đó nó xác định một đồng phôi từ X lên một tập con lồi compắc khác rỗng của không gian lồi địa phương tách được $E/N$. Điều này cho phép ta giả sử rằng không gian E là tách được.

Cho $f: X\rightarrow X$ là một ánh xạ liên tục. Ánh xạ $h: X\rightarrow E$ được định nghĩa bởi $h(x) =f(x)-x$ là liên tục; vì X compắc, ảnh $h(X)$ là đóng. Do đó chỉ cần chứng minh rằng 0 là điểm bám của $h$(X), nghĩa là với mọi lân cận mở lồi U của 0 trong E, tồn tại một điểm $b$ của X sao cho $f(b)-b\in U$.

Cho U là một lân cận lồi của 0 trong E. Với mọi $a\in X$, ký hiệu $V_a$ là tập hợp các phần tử $x$ của X sao cho $f(x)-f(a)\in U$. Nó mở trong X và chứa $a$. Vì X compắc và khác rỗng, tồn tại một tập con hữu hạn khác rỗng A của X sao cho các tập $V_a$, với $a\in A$, phủ X. Cho $(\varphi_a)_{a\in A}$ là một phân hoạch đơn vị liên tục phụ thuộc vào phủ $(V_a)_{a\in A}$ (TG, IX, p. 43, prop. 1 and p. 47, th. 3). Cho F là không gian con vectơ của E sinh bởi $f(A)$. Với mọi $x\in F\cap X$, đặt

$$
g(x) =\sum_{a\in A}\varphi_a(x)f(a)
$$

Điều này xác định một ánh xạ liên tục $g: F\cap X\rightarrow E$. Ảnh của nó được chứa trong bao lồi của $f$(A), do đó trong $F\cap X$. Vì tập hợp $F\cap X$ là một tập con compắc lồi khác rỗng của một không gian vectơ hữu hạn chiều, ánh xạ $g$ có một điểm bất động $b\in F\cap X$ theo Định lý 1. Ta có

$$
f(b)-b=f(b)-g(b) =\sum_{a\in A}\varphi_a(b) (f(b)-f(a))
$$

Với mọi $a\in$ A sao cho $\varphi_a(b)\not = 0$, ta có $b\in V_a$ nên $f(b)-f(a)\in U$. Vì U là lồi, suy ra $f(b)-b\in U$, điều này hoàn tất chứng minh.

### 5. Các không gian con bất biến dưới một toán tử compắc

Định lý sau đây cần được so sánh với Bổ đề Schur (A, VIII, p. 43, cor. and V, p. 386, prop. 6) và Hệ quả 4 của I, p. 26.

#### Định lý 3 {#ts-iii-s1-thm-3 .statement tag=02OP}

Cho E là một không gian lồi địa phương tách trên $\mathbf{C}$ và A là một tập con của $\mathscr{L}(E)$. Đặt các giả thiết sau:

(i) Không tồn tại không gian con vectơ đóng nào của E, phân biệt với $\{0\}$ và E, ổn định dưới A;

(ii) Tập hợp A chứa một tự đồng cấu compắc khác không. Khi đó hoán tập của A được thu về các phép vị tự.

Thay thế A bởi đại số con có đơn vị của $\mathscr{L}(E)$ sinh bởi A, ta quy được về trường hợp A là một đại số con có đơn vị của $\mathscr{L}(E)$. Khi đó, cho $h$ là một tự đồng cấu compắc khác không của E thuộc A.

#### Bổ đề 1 {#ts-iii-s1-lem-1 .statement tag=02OQ}

Tồn tại một phần tử $a$ của A sao cho hạt nhân của $ha-1_E$ không thu về 0.

Tồn tại một phần tử $x_0$ của E sao cho $h(x_0)\not = 0$. Cho V là một lân cận đóng của $h(x_0)$ không chứa 0. Vì tự đồng cấu $h$ là compắc, có thể chọn một lân cận mở lồi U của $x_0$ sao cho $h(U)$ là một tập con tương đối compắc của V. Do đó bao đóng C của $h(U)$ là một tập con compắc lồi của E; vì nó được chứa trong V nên nó không chứa 0.

Cho $y$ là một điểm của C. Ký hiệu $Ay$ là tập hợp các ảnh của $y$ dưới các phần tử của A. Nó là một không gian con vectơ của E ổn định dưới A; nó khác không vì chứa $y$. Theo giả thiết (i) của định lý, tập $Ay$ trù mật trong E. Do đó tồn tại một phần tử $b$ của A sao cho $b(y)\in U$. Vì tập C là compắc, tồn tại một

$-1$

họ hữu hạn $(b_1, . . . , b_n)$ các phần tử của A sao cho các tập $b_i(U)$ phủ C. Tồn tại một phân hoạch đơn vị liên tục $(\varphi_1, . . . , \varphi_n)$ trên C phụ thuộc vào phủ này (TG, IX, p. 47, th. 3). Định nghĩa một ánh xạ $f: C\rightarrow E$ bằng cách đặt

$$
f(x) =\sum_{i=1}^n\varphi_i(x)b_i(x)
$$

với mọi $x\in C$; đó là một ánh xạ liên tục. Vì U lồi và $b_i(x)$ thuộc U khi $\varphi_i(x)$ khác không, ta có $f(C)\subset U$ và $h(f(C))\subset C$. Theo định lý Leray-Schauder (Định lý 2 của III, p. 11), tồn tại một phần tử $x\in C$ sao cho $h(f(x)) =x$. Khi đó đặt

$$
a=\sum_{i=1}^n\varphi_i(x)b_i
$$

Ta có $h(a(x)) =h(f(x)) =x$ và $x$ khác không vì 0 không thuộc C, do đó hạt nhân của $ha-1_E$ là khác không.

Hãy hoàn tất chứng minh của Định lý 3. Gọi $a$ là một phần tử của A sao cho hạt nhân T của $ha-1_E$ là khác không (Bổ đề 1). Gọi $i$ là đơn ánh chính tắc từ T vào E. Ánh xạ tuyến tính $i$ bằng $h\circ a\circ i$, và vì thế là compắc. Do đó chiều của T là hữu hạn (Nhận xét 3 của III, p. 2). Gọi $u$ là một phần tử của $\mathscr{L}(E)$ giao hoán với A. Vì $u$ giao hoán với $h\circ a$, ta có $u(T)\subset T$. Vì T có số chiều hữu hạn khác không trên trường đóng đại số $\mathbf{C}$, tự đồng cấu của T cảm sinh bởi $u$ có một trị riêng $\lambda$.

Đặt F = Ker($u-\lambda 1_E$). Đó là một không gian con vectơ đóng khác không của E; nó ổn định dưới A, vì $u$ giao hoán với các phần tử của A. Theo giả thiết (i), ta có F = E, do đó $u=\lambda 1_E$.

#### Hệ quả 1 {#ts-iii-s1-thm-3-cor-1 .statement tag=02OR}

Giữ các giả thiết của Định lý 3 và giả sử thêm rằng các phần tử của A giao hoán từng đôi một. Khi đó E có chiều bằng 1 trên $\mathbf{C}$.

Theo giả thiết (ii) của Định lý 3, không gian E khác không. Vì thế nó chứa một không gian con vectơ F có chiều bằng 1. Không gian con này là đóng vì E được giả thiết là phân ly. Theo Định lý 3, mọi phần tử của A đều là một phép vị tự, và do đó ổn định F. Khi đó từ giả thiết (i) của Định lý 3 suy ra F bằng E.

#### Hệ quả 2 (Lomonosov) {#ts-iii-s1-thm-3-cor-2 .statement tag=02OS}

Cho E là một không gian lồi địa phương phân ly có chiều ít nhất bằng 2 trên trường $\mathbf{C}$ và $u$ là một tự đồng cấu của E. Giả sử tồn tại một tự đồng cấu compắc $h\not = 0$ của E giao hoán với $u$. Khi đó tồn tại một không gian con vectơ đóng F của E, khác $\{0\}$ và khác E, sao cho $u(F)\subset F$.

Thật vậy, Hệ quả 1 cho thấy tập $A =\{u, h\}$ không thể thỏa mãn giả thiết (i) của Định lý 3.

#### Hệ quả 3 {#ts-iii-s1-thm-3-cor-3 .statement tag=02OT}

Cho E là một không gian lồi địa phương phân ly trên trường $\mathbf{C}$ và $u$ là một tự đồng cấu compắc của E. Nếu E có chiều ít nhất bằng 2, thì tồn tại một không gian con vectơ đóng F của E, khác $\{0\}$ và khác E, sao cho $u(F)\subset F$.

Trường hợp $u= 0$ là ngay lập tức. Trường hợp $u\not = 0$ suy ra từ Hệ quả 2 bằng cách lấy $h=u$.

### 6. Các không gian xấp xỉ

Cho các không gian lồi địa phương E và F, nhắc lại (EVT, III, p. 14, Ví dụ 2) rằng $\mathscr{L}_{pc}(E; F)$ ký hiệu không gian lồi địa phương nhận được bằng cách trang bị cho $\mathscr{L}(E; F)$ tôpô hội tụ tiền compắc. Ta cũng ký hiệu bởi $\mathscr{L}_{pc}(E)$ không gian lồi địa phương $\mathscr{L}_{pc}(E; E)$. Khi không gian lồi địa phương E là phân ly và gần đầy đủ (EVT, III, p. 8, định nghĩa 6), tôpô hội tụ tiền compắc trên $\mathscr{L}(E; F)$ trùng với tôpô hội tụ compắc, vì bao đóng của một tập con tiền compắc của E là compắc (EVT, III, p. 8).

#### Định nghĩa 2 {#ts-iii-s1-def-2 .statement tag=02OU}

Một không gian lồi địa phương E được gọi là có tính chất xấp xỉ, hay còn gọi là một không gian xấp xỉ, nếu ánh xạ đồng nhất $1_E$ của E thuộc bao đóng trong không gian $\mathscr{L}_{pc}(E)$ của tập $\mathscr{L}^f(E)$ các tự đồng cấu liên tục hạng hữu hạn của E.

Đặc biệt, mọi không gian lồi địa phương hữu hạn chiều đều là một không gian xấp xỉ.

#### Nhận xét 1 {#ts-iii-s1-n6-rem-1 .statement tag=02OV}

Để tổng trực tiếp tôpô của các không gian lồi địa phương E và F là một không gian xấp xỉ, điều kiện cần và đủ là E và F là các không gian xấp xỉ.

#### Nhận xét 2 {#ts-iii-s1-n6-rem-2 .statement tag=02OW}

Cho E là một không gian lồi địa phương. Gọi N là bao đóng của $\{0\}$ trong E và P là một không gian con bù đại số của N trong E. Khi đó P là một không gian con bù tôpô của N trong E, và đẳng cấu với không gian lồi địa phương $E/N$. Không gian N là một không gian xấp xỉ. Theo Nhận xét 1, để E là một không gian xấp xỉ, điều kiện cần và đủ là không gian lồi địa phương phân ly $E/N$ là một không gian như vậy.

#### Nhận xét 3 {#ts-iii-s1-n6-rem-3 .statement tag=02OX}

Cho E là một không gian lồi địa phương, A là một tập con đẳng liên tục của $\mathscr{L}^f(E)$ và T là một tập con toàn phần của E. Nếu $1_E$ thuộc bao đóng của A đối với tôpô hội tụ đơn giản trên T, thì $1_E$ thuộc bao đóng của A trong $\mathscr{L}_{pc}(E)$ (EVT, III, p. 16, Mệnh đề 4 và p. 17, Mệnh đề 5), và E là một không gian xấp xỉ.

#### Nhận xét 4 {#ts-iii-s1-n6-rem-4 .statement tag=02OY}

Cho E là một không gian lồi địa phương trên $\mathbf{C}$. Ký hiệu bởi $E_0$ không gian lồi địa phương trên $\mathbf{R}$ nằm dưới E. Để E là một không gian xấp xỉ, điều kiện cần và đủ là $E_0$ là một không gian như vậy. Thật vậy, điều kiện là cần; hãy chứng minh rằng nó là đủ. Vậy giả sử rằng $E_0$ là một không gian xấp xỉ. Cho C là một tập con tiền compact của E và U là một lân cận lồi cân bằng của 0 trong E. Đặt $C'= C\cup iC$. Tồn tại một ánh xạ $\mathbf{R}$-tuyến tính liên tục hạng hữu hạn $u$ từ $E_0$ vào $E_0$ sao cho $x-u(x)$ thuộc U với mọi $x\in C'$. Đặt $v(x) =\frac{1}{2}(u(x)-iu(ix))$ với mọi $x$ trong E. Khi đó ta xác định được một ánh xạ $\mathbf{C}$-tuyến tính liên tục hạng hữu hạn từ E vào E. Với mọi $x\in C$, ta có $x\in C',ix\in C'$ và $x-v(x) =\frac{1}{2}(x-u(x))-\frac{i}{2}(ix-u(ix))$, do đó $x-v(x)$ thuộc U. Điều này chứng minh rằng E là một không gian xấp xỉ.

#### Nhận xét 5 {#ts-iii-s1-n6-rem-5 .statement tag=02OZ}

Cho E là một không gian lồi địa phương trên $\mathbf{R}$. Để không gian lồi địa phương phức hóa $E_{(\mathbf{C})}$ của E là một không gian xấp xỉ, điều kiện cần và đủ là E là một không gian như vậy. Điều này suy ra từ các nhận xét 1 và 4, vì không gian lồi địa phương thực nằm dưới $E_{(\mathbf{C})}$ là đẳng cấu với $E\times E$.

#### Mệnh đề 10 {#ts-iii-s1-prop-10 .statement tag=02P0}

Cho E là một không gian Hilbert. Khi đó E là một không gian xấp xỉ.

Tập A các phép chiếu trực giao hạng hữu hạn trong E là đẳng liên tục. Cho $n\geqslant 1$ là một số nguyên và $(x_1, . . . , x_n)$ là một họ các phần tử của E. Gọi V là không gian con vectơ sinh bởi các $x_i$ và $p_V$ là phép chiếu trực giao có ảnh là V. Ta có $p_V(x_i) =x_i$ với $1\leqslant i\leqslant n$. Suy ra rằng $1_E$ thuộc bao đóng của A đối với tôpô hội tụ đơn, và do đó E là một không gian xấp xỉ (nhận xét 3).

Các ví dụ khác về không gian xấp xỉ sẽ được cho trong No.$^o7$ của III, p. 20.

#### Bổ đề 2 {#ts-iii-s1-lem-2 .statement tag=02P1}

Cho E là một không gian lồi địa phương. Khi đó E là một không gian xấp xỉ khi và chỉ khi, với mọi tập con tiền compact C của E và mọi lân cận U của 0 trong E, tồn tại một số nguyên $n\geqslant 0$, các phần tử $e_1, . . . , e_n$ của E, và các dạng tuyến tính liên tục $f_1, . . . , f_n$ trên E, sao cho $x-\sum^n_{i=1}f_i(x)e_i$ thuộc U với mọi $x\in C$.

Định nghĩa của tôpô hội tụ tiền compact cho thấy điều kiện là đủ. Ngược lại, giả sử rằng E là một không gian xấp xỉ. Cho P là một bổ sung tôpô trong E của bao đóng của $\{0\}($xem nhận xét 2). Khi đó tập A các $u\in \mathscr{L}^f(E)$ sao cho $u(E)\subset P$ là trù mật trong $\mathscr{L}^f(E)$. Vì P tách biệt, mọi phần tử $u$ của A đều có dạng $x\mapsto \sum^n_{i=1}f_i(x)e_i$, trong đó $n\in \mathbf{N},e_1, . . . , e_n$ là các phần tử của E và $f_1, . . . , f_n$ là các dạng tuyến tính liên tục trên E (EVT, I, p. 14, đl. 2). Điều này chứng minh rằng điều kiện là cần.

#### Nhận xét 6 {#ts-iii-s1-n6-rem-6 .statement tag=02P2}

Tồn tại các không gian Banach không có tính chất xấp xỉ, như đã được P. Enflo chứng minh (A counterexample to the approximation problem in Banach spaces, Acta Math. 130 (1973), p. 309–317 ; xem bài tập 25 của III, p. 112). Điều này trả lời một câu hỏi của S. Banach (Théorie des opérations linéaires, Monografje Matematyczne I, Warszawa, 1932, các nhận xét về Chương VI, §1). Xem thêm nhận xét ở p. 21.

#### Mệnh đề 11 {#ts-iii-s1-prop-11 .statement tag=02P3}

Cho E và F là các không gian lồi địa phương. Giả sử rằng E là một không gian xấp xỉ.

a) Tập $\mathscr{L}^f(E; F)$ là trù mật trong $\mathscr{L}_{pc}(E; F)$;

b) Tập $\mathscr{L}^f(F; E)$ là trù mật trong $\mathscr{L}_{pc}(F; E)$;

c) Cho $\mathfrak{S}$ là một tập các tập con bị chặn của F và $u\in \mathscr{L}(F; E)$. Giả sử rằng ảnh dưới $u$ của mọi tập con của F thuộc $\mathfrak{S}$ là tiền compact. Khi đó $u$ thuộc bao đóng của $\mathscr{L}^f(F; E)$ đối với $\mathfrak{S}$-tôpô (EVT, III, p. 13).

Cho $v$ là một phần tử của $\mathscr{L}(E; F)$. Ánh xạ $\varphi :w\mapsto v\circ w$ từ $\mathscr{L}_{pc}(E)$ vào $\mathscr{L}_{pc}(E; F)$ là liên tục (TG, X, p. 5, mệnh đề 3). Ta có $\varphi (1_E) =v$ và $\varphi (\mathscr{L}^f(E))\subset \mathscr{L}^f(E; F)$, do đó $v$ thuộc bao đóng của $\mathscr{L}^f(E; F)$ trong $\mathscr{L}_{pc}(E; F)$. Điều này chứng minh a).

Tương tự, dưới các giả thiết của c), ánh xạ $\psi :w\mapsto w\circ u$ từ $\mathscr{L}_{pc}(E)$ vào $\mathscr{L}_{\mathfrak{S}}(F; E)$ là liên tục (loc. cit.). Ta có $\psi (1_E) =u$ và $\psi (\mathscr{L}^f(E))\subset \mathscr{L}^f(F; E)$, do đó $u$ thuộc bao đóng của $\mathscr{L}^f(F; E)$ trong $\mathscr{L}_{\mathfrak{S}}(F; E)$.

Ảnh của một tập con tiền compact của F qua một ánh xạ tuyến tính liên tục từ F vào E là tiền compact, do đó b) suy ra từ c).

#### Hệ quả {#ts-iii-s1-n6-cor-1 .statement tag=02P4}

Cho E là một không gian xấp xỉ tách và F một không gian lồi địa phương. Mọi ánh xạ tuyến tính compact từ F vào E đều thuộc bao đóng của $\mathscr{L}^f(F; E)$ trong không gian $\mathscr{L}(F; E)$ được trang bị tôpô hội tụ trên các tập bị chặn.

Điều này suy ra từ mệnh đề 11, c), vì ảnh của một tập con bị chặn của F qua một ánh xạ tuyến tính compact từ F vào E là tương đối compact trong E (nhận xét 1 của III, p. 2), do đó tiền compact.

#### Mệnh đề 12 {#ts-iii-s1-prop-12 .statement tag=02P5}

Cho E là một không gian lồi địa phương, I một tập hợp, và với mỗi $i\in I$, cho $F_i$ là một không gian lồi địa phương và $v_i: E\rightarrow F_i$ một ánh xạ tuyến tính liên tục có ảnh trù mật. Giả sử rằng với mọi lân cận U của 0 trong E, tồn tại $i\in I$ và một lân cận V của 0 trong $F_i$ sao cho $\overset{-1}{v_{i}}(V)\subset U$. Nếu các $F_i$ là những không gian xấp xỉ, thì E cũng là một không gian như vậy.

Cho A là một tập con tiền compact của E và U một lân cận của 0 trong E. Theo giả thiết tồn tại $i\in I$ và một nửa chuẩn liên tục $p$ trên $F_i$ sao cho U chứa $(p\circ v_i)^{-1}([0,1])$. Đặt $F = F_i,v=v_i$ và $B =v$(A), và giả sử F là một không gian xấp xỉ. Tập hợp B là tiền compact trong F. Do đó tồn tại (bổ đề 2) một số nguyên $n\geqslant 1$, các phần tử $y_1, . . . , y_n$ của F và các dạng tuyến tính liên tục $f_1, . . . , f_n$ trên F, sao cho ta có, với mọi $y\in B$,

$$
p(y-\sum^nf_j(y)y_j)\leqslant \frac{1}{2}
$$

$j=1$

Vì B bị chặn (EVT, III, p. 3, mệnh đề 2), tồn tại một số thực $M>0$ sao cho $|f_j(y)|\leqslant M$ với mọi $j$ sao cho $1\leqslant j\leqslant n$ và mọi $y\in B$. Hơn nữa, vì $v(E)$ trù mật trong F, tồn tại, với mỗi số nguyên $j$ sao cho $1\leqslant j\leqslant n$, một phần tử $x_j$ của E sao cho $p(y_j-v(x_j))\leqslant (2nM)^{-1}$. Ánh xạ tuyến tính

$$
u:x\longmapsto \sum_{j=1}^nf_j(v(x))x_j
$$

thuộc $\mathscr{L}^f(E)$. Với mọi $x\in A$, ta có

$$
v(x-u(x)) =v(x)-\sum_{j=1}^nf_j(v(x))y_j+\sum_{j=1}^nf_j(v(x))(y_j-v(x_j))
$$

do đó $p(v(x-u(x)))\leqslant \frac{1}{2}+\frac{nM}{2nM}= 1$, và vì thế $x-u(x)\in U$. Mệnh đề được chứng minh.

#### Hệ quả 1 {#ts-iii-s1-prop-12-cor-1 .statement tag=02P6}

Một không gian con vectơ trù mật của một không gian xấp xỉ là một không gian xấp xỉ.

#### Hệ quả 2 {#ts-iii-s1-prop-12-cor-2 .statement tag=02P7}

Nếu hoàn thành tách của một không gian lồi địa phương E là một không gian xấp xỉ, thì E là một không gian xấp xỉ.

#### Hệ quả 3 {#ts-iii-s1-prop-12-cor-3 .statement tag=02P8}

Tích của một họ các không gian xấp xỉ là một không gian xấp xỉ.

Thật vậy, cho $(E_i)_{i\in I}$ là một họ các không gian xấp xỉ. Với mọi tập con hữu hạn J của I, đặt $E_J=\prod_{i\in J}E_i$ và ký hiệu $v_J$ là ánh xạ chính tắc từ $E =\prod_{i\in I}E_i$ vào $E_J$. Không gian lồi địa phương $E_J$ là một không gian xấp xỉ (Nhận xét 1). Khi đó hệ quả suy ra từ Mệnh đề 12 áp dụng cho không gian lồi địa phương E, cho họ $(E_J)$ các không gian lồi địa phương, và cho các ánh xạ tuyến tính liên tục $v_J: E\rightarrow E_J$.

#### Hệ quả 4 {#ts-iii-s1-prop-12-cor-4 .statement tag=02P9}

Cho E là một không gian lồi địa phương. Nếu mọi nửa chuẩn liên tục trên E đều bị chặn trên bởi một nửa chuẩn tiền Hilbert liên tục, thì E là một không gian xấp xỉ.

Cho $\mathscr{P}$ là tập hợp các nửa chuẩn tiền Hilbert liên tục trên E. Với mỗi $p\in \mathscr{P}$, giả thiết suy ra rằng không gian nửa chuẩn $E_p$ thu được bằng cách trang bị cho E nửa chuẩn $p$ là một không gian xấp xỉ (Hệ quả 2 và Mệnh đề 10), và ánh xạ đồng nhất từ E vào $E_p$ là liên tục. Vì thế hệ quả suy ra từ Mệnh đề 12.

#### Bổ đề 3 {#ts-iii-s1-lem-3 .statement tag=02PA}

Cho E là một không gian lồi địa phương khả mêtric và $(x_n)_{n\in\mathbf{N}}$ là một dãy các phần tử của E hội tụ về 0. Tồn tại một dãy $(y_n)_{n\in\mathbf{N}}$ các phần tử của E hội tụ về 0 và một dãy $(\lambda_n)_{n\in\mathbf{N}}$ các phần tử của khoảng $[0,1]$ hội tụ về 0 sao cho ta có $x_n=\lambda_ny_n$ với mọi $n\in \mathbf{N}$.

Vì E là khả mêtric, tồn tại một hệ cơ bản $(V_m)_{m\in\mathbf{N}}$ các lân cận cân bằng của 0 trong E sao cho $V_0= E$ và $2^{m+1}V_{m+1}\subset V_m$ với mọi $m\geqslant 0$. Vì $(x_n)$ hội tụ về 0, tồn tại một dãy tăng ngặt $(N_m)_{m\in\mathbf{N}}$ các số nguyên sao cho $N_0= 0$ và sao cho, với mọi $m\geqslant 0$, ta có $x_n\in V_m$ khi $n\geqslant N_m$. Với mọi số nguyên $n\geqslant 0$, tồn tại một số nguyên duy nhất $m\geqslant 0$ sao cho $N_m\leqslant n <N_{m+1}$, và khi đó đặt $\lambda_n= 2^{-m}$ và $y_n= 2^mx_n$. Dãy $(\lambda_n)$ được xác định như vậy hội tụ về 0. Hơn nữa, vì $y_n\in V_m$ với $n\geqslant N_{m+1}$, dãy $(y_n)$ hội tụ về 0 trong E. Cuối cùng, ta có $x_n=\lambda_ny_n$ với mọi $n$.

Nhắc lại (EVT, II, p. 28) rằng nếu E là một không gian vectơ và L là một tập con lồi cân bằng của E, thì người ta ký hiệu bởi $E_L$ không gian con vectơ của E sinh bởi L, được trang bị nửa chuẩn có quả cầu đơn vị là L. Khi tập hợp L không chứa đường thẳng nào, nửa chuẩn này là một chuẩn.

#### Bổ đề 4 {#ts-iii-s1-lem-4 .statement tag=02PB}

Cho E là một không gian Fréchet và A là một tập con compắc của E. Tồn tại một tập con lồi cân bằng compắc L của E chứa A sao cho các tôpô cảm sinh trên A bởi các tôpô của E và của $E_L$ là trùng nhau.

Tập A được chứa trong bao lồi cân bằng đóng của tập hợp các điểm của một dãy $(x_n)_{n\in\mathbf{N}}$ các phần tử của E hội tụ về 0 (EVT, IV, p. 24, Hệ quả 1). Cho $(y_n)_{n\in\mathbf{N}}$ và $(\lambda_n)_{n\in\mathbf{N}}$ là các dãy thỏa mãn kết luận của Bổ đề 3. Bao lồi cân bằng đóng L của các điểm của dãy $(y_n)$ chứa A và là một tập con compắc của E (EVT, III, p. 8). Do đó $E_L$ là một không gian Banach (EVT, III, p. 8, Hệ quả). Trong không gian Banach này, chuẩn của $x_n$ bị chặn trên bởi $\lambda_n$, vì vậy dãy $(x_n)$ tiến tới 0. Bao lồi cân bằng đóng $\widetilde{A}$ của dãy $(x_n)$ trong $E_L$ là một tập con compắc của $E_L$ (EVT, III, p. 8). Vì L là một tập con bị chặn của E, đơn ánh chính tắc từ $E_L$ vào E là liên tục. Các tôpô cảm sinh trên $\widetilde{A}$ bởi các tôpô của $E_L$ và của E là trùng nhau, và $\widetilde{A}$ là một tập con compắc, do đó đóng, của E. Vì tập hợp $\widetilde{A}$ là lồi, cân bằng, và chứa dãy $(x_n)$, nó chứa A. Điều này hoàn thành chứng minh.

#### Định lý 4 {#ts-iii-s1-thm-4 .statement tag=02PC}

Cho E là một không gian Fréchet.

a) Giả sử rằng E là một không gian xấp xỉ. Khi đó, với mọi không gian nửa định chuẩn F, không gian $\mathscr{L}^f(F; E)$ là trù mật trong $\mathscr{L}^c(F; E)$ đối với tôpô hội tụ bị chặn;

b) Ngược lại, giả sử rằng với mọi không gian Banach F, mọi ánh xạ tuyến tính compact từ F vào E thuộc bao đóng của $\mathscr{L}^f(F; E)$ đối với tôpô hội tụ bị chặn. Khi đó E là một không gian xấp xỉ.

Cho F là một không gian nửa định chuẩn. Bao đóng của $\mathscr{L}^f(F; E)$ trong $\mathscr{L}(F; E)$ được chứa trong $\mathscr{L}^c(F; E)$ (Mệnh đề 1 và 2 của III, p. 4). Nó bằng $\mathscr{L}^c(F; E)$ nếu E là một không gian xấp xỉ theo Hệ quả của Mệnh đề 11. Điều này chứng minh mệnh đề a).

Giả sử rằng giả thiết của b) được thỏa mãn. Cho $\varepsilon  >0$ là một số thực. Cho A là một tập con compact của E và $p$ một nửa chuẩn liên tục trên E. Cho L là một tập con compact lồi cân bằng của E sao cho A là một tập con compact của không gian định chuẩn $E_L$ (Bổ đề 4). Đơn ánh chính tắc $j: E_L\rightarrow E$ là compact và $E_L$ là một không gian Banach (TVS, III, p. 8, Cor.). Do đó theo giả thiết tồn tại một số nguyên $n\geqslant 1$, các phần tử $e_1, . . . , e_n$ của E, và các dạng tuyến tính liên tục $\ell_1, . . . , \ell_n$ trên $E_L$, sao cho ánh xạ $v$ từ $E_L$ vào E được xác định bởi $v(x) =\sum^n_{i=1}\ell_i(x)e_i$ thỏa mãn $p(x-v(x))\leqslant \frac{\varepsilon}{2}$ với $x\in A$. Ảnh của $^tj: E'\rightarrow (E_L)'$ là trù mật trong $(E_L)'$ đối với tôpô yếu (TVS, IV, p. 6, Prop. 5). Trên $(E_L)'$ tôpô hội tụ compact là tương thích với đối ngẫu giữa $(E_L)'$ và $E_L$ (TVS, IV, p. 3, Example). Vì vậy $^tj(E')$ là trù mật trong $(E_L)'$ đối với tôpô hội tụ compact (TVS, IV, p. 1, Prop. 1), và tồn tại các dạng tuyến tính liên tục $f_1, . . . , f_n$ trên E sao cho

$$
|\ell_i(x)-f_i(x)|p(e_i)\leqslant \frac{\varepsilon}{2n}
$$

với $x\in A$ và $1\leqslant i\leqslant n$. Tự đồng cấu $u:x\mapsto \sum^n_{i=1}f_i(x)e_i$ của E thuộc $\mathscr{L}^f(E)$, và với mọi $x\in A$, ta có

$$
p(x-u(x))\leqslant p(x-v(x)) +p(v(x)-u(x))\leqslant \frac{\varepsilon}{2}+n\times \frac{\varepsilon}{2n}=\varepsilon
$$

Từ đó suy ra rằng $1_E$ thuộc bao đóng của $\mathscr{L}^f(E)$ đối với tôpô hội tụ compact. Nhưng tôpô sau trùng với tôpô hội tụ tiền compact vì E là đầy đủ. Vậy E là một không gian xấp xỉ.

### 7. Các ví dụ về không gian xấp xỉ

Nhắc lại rằng mọi không gian Hilbert đều là một không gian xấp xỉ (III, p. 15, Prop. 10). Tiết này cho các ví dụ khác.

Nếu X là một không gian địa phương compact, người ta ký hiệu bởi $\mathscr{C}_0(X; K)$, hoặc đơn giản là $\mathscr{C}_0$(X), không gian Banach các ánh xạ liên tục từ X vào K tiến tới 0 ở vô cực, được trang bị chuẩn xác định bởi $\|f\|=$ sup$_{x\in X}|f(x)|$ với $f\in \mathscr{C}_0(X)$. Khi X compact, không gian này trùng với không gian $\mathscr{C}(X)$ các ánh xạ liên tục từ X vào K.

#### Bổ đề 5 {#ts-iii-s1-lem-5 .statement tag=02PD}

Cho X là một không gian tôpô compact, F một tập con hữu hạn của $\mathscr{C}(X)$ và $\varepsilon  >0$ một số thực.

Tồn tại một tập con hữu hạn $X_0\subset X$ và một ánh xạ tuyến tính $u:\mathscr{C}(X_0)\rightarrow \mathscr{C}(X)$ có chuẩn $\leqslant 1$ sao cho $\|u(f|X_0)-f\|\leqslant \varepsilon$ với mọi $f\in F$.

Vì tập hợp F là một tập con đẳng liên tục của $\mathscr{C}$ (X), tồn tại một phủ hữu hạn $(U_i)_{i\in I}$ của X sao cho, với mọi $i\in I$ và mọi $f\in F$, đường kính của $f(U_i)$ là $\leqslant \varepsilon$. Với $i$ thuộc I, chọn một điểm $x_i$ của $U_i$, và ký hiệu bởi $X_0$ tập hợp hữu hạn các $x_i$ với $i\in I$.

Cho $(\varphi_i)_{i\in I}$ là một phân hoạch đơn vị liên tục phục tùng $(U_i)_{i\in I}$ (TG, IX, p. 47, đl. 3). Định nghĩa một ánh xạ tuyến tính $u$ từ $\mathscr{C}(X_0)$ vào $\mathscr{C}(X)$ bằng cách đặt

$$
u(g) =\sum_{i\in I}g(x_i)\varphi_i
$$

với mọi $g\in \mathscr{C}(X_0)$. Ánh xạ tuyến tính $u$ có chuẩn $\leqslant 1$ và thỏa mãn $\|u(f|X_0)-f\|\leqslant \varepsilon$ với mọi $f$ thuộc F, do đó mệnh đề được chứng minh.

#### Mệnh đề 13 {#ts-iii-s1-prop-13 .statement tag=02PE}

Cho X là một không gian tôpô địa phương compact. Không gian Banach $\mathscr{C}_0(X)$ là một không gian xấp xỉ.

Trước hết giả sử X compact. Gọi $A\subset \mathscr{L}^f(\mathscr{C}(X))$ là tập hợp các ánh xạ có dạng $f\mapsto u(f|X_0)$, trong đó $X_0$ là một tập con hữu hạn của X và $u:\mathscr{C}(X_0)\rightarrow \mathscr{C}(X)$ là một ánh xạ tuyến tính có chuẩn $\leqslant 1$. Tập hợp A là đẳng liên tục. Theo Bổ đề 5, ánh xạ đồng nhất của $\mathscr{C}(X)$ thuộc bao đóng của A đối với tôpô hội tụ đơn trên $\mathscr{C}(X)$. Khi đó mệnh đề suy ra từ Nhận xét 3 của III, p. 14.

Xét trường hợp tổng quát. Gọi Y là phép compact hóa Alexandroff của X và $\omega$ là điểm ở vô cực của Y (TG, I, p. 67). Đồng nhất $\mathscr{C}_0(X)$ với tập hợp các phần tử của $\mathscr{C}(Y)$ triệt tiêu tại $\omega$. Khi đó $\mathscr{C}(Y)$ là tổng trực tiếp tôpô của $\mathscr{C}_0(X)$ và không gian vectơ các ánh xạ hằng trên Y. Vì $\mathscr{C}(Y)$ là một không gian xấp xỉ theo điều vừa nói trên, nên không gian $\mathscr{C}_0(X)$ là một không gian xấp xỉ (Nhận xét 1 của III, p. 14).

#### Hệ quả {#ts-iii-s1-n7-cor-1 .statement tag=02PF}

Mọi đại số sao giao hoán đều là một không gian xấp xỉ.

Thật vậy, một đại số như vậy đẳng cấu với đại số các hàm liên tục tiến tới 0 tại vô cực trên một không gian địa phương compact (I, p. 108, đl. 1).

#### Nhận xét {#ts-iii-s1-n7-rem-1 .statement tag=02PG}

Nếu E là một không gian Hilbert vô hạn chiều, đại số sao $\mathscr{L}(E)$ không có tính chất xấp xỉ (A. Szankowski, $\mathscr{B}(H)$ does not have the approximation property, Acta Math. 147 (1981), p. 89–108).

#### Bổ đề 6 {#ts-iii-s1-lem-6 .statement tag=02PH}

Cho X là một không gian tôpô địa phương compact. Cho $\mu$ là một độ đo dương trên X và $p\in [1,+\infty [$. Cho F là một tập con hữu hạn của $L^p_K(X, \mu)$ và $\varepsilon  >0$ là một số thực.

Tồn tại một phép chiếu hạng hữu hạn $u$ của $L^p_K(X, \mu)$ có chuẩn $\leqslant 1$ sao cho $\|u(f)-f\|\leqslant \varepsilon$ với mọi $f$ thuộc F.

Gọi $\mathscr{P}$ là tập hợp các phân hoạch hữu hạn $\pi = (K_1, . . . ,K_n,H)$ của X, trong đó $n\geqslant 1$ là một số nguyên và $K_1, . . . ,K_n$ là các tập con khả tích có độ đo khác không của X. Với mỗi phân hoạch $\pi = (K_1, . . . ,K_n,H)\in \mathscr{P}$, ta định nghĩa một tự đồng cấu $v_{\pi}$ của $\mathscr{L}^p(X, \mu)$ bằng cách đặt

$$
v_{\pi}(f) =\sum^n\frac{1}{\mu(K_i)}(\int_{K_i}f d\mu)\varphi_{K_i}
$$

$i=1$

với $f\in \mathscr{L}_K^p(X, \mu)$, trong đó $\varphi_{K_i}$ là hàm đặc trưng của $K_i$. Ánh xạ $v_{\pi}$ cảm sinh, khi chuyển qua các thương, một phép chiếu $u_{\pi}$ của $L^p_K(X, \mu)$. Dễ dàng kiểm tra rằng ảnh của $u_{\pi}$ là không gian các lớp của những hàm $f\in \mathscr{L}_K^p(X, \mu)$ sao cho $f$ triệt tiêu trên H và là hằng trên $K_i$ với $1\leqslant i\leqslant n$.

Ta hãy chứng minh rằng $\|u_{\pi}\|\leqslant 1$. Với $f\in \mathscr{L}_K^p(X, \mu)$, ta có

$$
\|u_{\pi}(f)\|^p_p=\sum_{i=1}^n\mu(K_i)^{1-p}|\int_{K_i}f d\mu|^p
$$

Theo bất đẳng thức Hölder (INT, IV, p. 208, § 6, No.$^o4$, Định lý 2), với mọi $i$ ta có bất đẳng thức

$$
|\int_{K_i}f d\mu|^p\leqslant \mu(K_i)^{p-1}\int_{K_i}|f|^pd\mu
$$

do đó $\|u_{\pi}(f)\|_p\leqslant \|f\|_p$.

Gọi $\mathscr{E}$ là tập hợp các lớp trong $L^p_K(X, \mu)$ của các hàm khả tích trên X chỉ nhận một số hữu hạn giá trị. Vì $\mathscr{E}$ trù mật trong $L^p_K(X, \mu)$ (INT, IV, p. 162, §4, No.$^o10$, Hệ quả 1), tồn tại một tập hợp hữu hạn $F'$ của $\mathscr{E}$ sao cho mọi phần tử của F đều cách một phần tử của $F'$ không quá $\varepsilon$. Khi xét phân hoạch hữu hạn $\pi$ tạo bởi các tập hợp có độ đo khác không, trên đó ánh xạ $x\mapsto (f(x))_{f\in F'}$ nhận một giá trị cho trước, ta thấy rằng tồn tại một phần tử $\pi$ của $\mathscr{P}$ sao cho $u_{\pi}(f) =f$ với mọi $f$ trong $F'$. Vậy phép chiếu $u_{\pi}$ có các tính chất cần có.

#### Mệnh đề 14 {#ts-iii-s1-prop-14 .statement tag=02PI}

Cho X là một không gian tôpô compact địa phương, $\mu$ là một độ đo dương trên X, và $p\in [1,+\infty ]$. Không gian $L^p_K(X, \mu)$ là một không gian xấp xỉ.

Nếu $p= +\infty$, thì không gian $L^{\infty}_{\mathbf{C}}(X, \mu)$ là một đại số stellar giao hoán (Ví dụ 4 của I, p. 103), do đó là một không gian xấp xỉ (Hệ quả của Mệnh đề 13), và điều tương tự cũng đúng với $L^{\infty}_{\mathbf{R}}(X, \mu)$ theo Nhận xét 5 của III, p. 15.

Giả sử $p$ là hữu hạn. Gọi $A\subset \mathscr{L}^f(L^p_K(X, \mu))$ là tập hợp các phép chiếu hạng hữu hạn và có chuẩn $\leqslant 1$. Theo Bổ đề 6, ánh xạ đồng nhất của $L^p_K(X, \mu)$ là điểm dính của A đối với tôpô hội tụ đơn giản, và mệnh đề khi đó suy ra từ Nhận xét 3 của III, p. 14.

## BÀI TẬP {#ts-iii-s1-exercises}

Chỉ trong các Bài tập 1 đến 5, K ký hiệu một trường định giá đầy đủ không Acsimet không rời rạc, mà định giá của nó được ký hiệu bởi $x\mapsto  |x|$. Ta cũng ký hiệu bởi $G\subset \mathbf{R}^*_+$ ảnh của $K^*$ dưới ánh xạ $x\mapsto  |x|$. Các không gian Banach được xét là các không gian Banach trên K.

Xem [các bài tập của § 1](exercises/s1/).
