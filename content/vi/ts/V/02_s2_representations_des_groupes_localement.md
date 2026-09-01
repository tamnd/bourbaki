---
book: ts
book_title: Théories spectrales
chapter: V
chapter_title: REPRÉSENTATIONS UNITAIRES
section: 2
section_title: Représentations des groupes localement compacts
lang: vi
source: ts-iii-v-fr
book_pages: TS V.399-TS V.431, TS V.486-TS V.492
pdf_pages: 0412-0444, 0499-0505
extraction: native
subsections:
    - "no": 1
      title: Continuité de certaines représentations
      page: 399
      pdf_page: 412
    - "no": 2
      title: Extension de représentations à des espaces de mesures
      page: 400
      pdf_page: 413
    - "no": 3
      title: Critère de semi-simplicité
      page: 402
      pdf_page: 415
    - "no": 4
      title: Représentations régulières
      page: 405
      pdf_page: 418
    - "no": 5
      title: Fonctions équivariantes
      page: 407
      pdf_page: 420
    - "no": 6
      title: Représentations induites
      page: 415
      pdf_page: 428
    - "no": 7
      title: Cas d’un sous-groupe fermé central
      page: 416
      pdf_page: 429
    - "no": 8
      title: Représentations de carré intégrable
      page: 419
      pdf_page: 432
    - "no": 9
      title: Sous-représentations de la représentation régulière d’un groupe commutatif
      page: 425
      pdf_page: 438
    - "no": 10
      title: Représentations unitaires du groupe R
      page: 427
      pdf_page: 440
statements: 45
exercises: 20
content_sha256: 50c6cc05b2ccc2095e50498f73abfff21dc821eb67be70898687f9eaa7f42d47
translated_from: content/en-mt/ts/V/02_s2_representations_des_groupes_localement.md
source_lang: en-mt
translation_method: machine
source_content_sha256: c28075aaca88e73a217d743e0f90dd1d3d6c62e0ddbc8b6f5c6252e65c430bf4
translation_model: gpt-5-6, gpt-5-6-mini, gpt-5-mini
translation_run: translate-vi-2f2eba27
glossary_version: 34
glossary_terms_sha256: 454022f824d62c73304ad6881a06bdbe8207e0e335f139de22ceb17b3c0b2cf3
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 2. BIỂU DIỄN CỦA CÁC NHÓM COMPACT ĐỊA PHƯƠNG

Trong đoạn này, các không gian vectơ là trên trường $K =\mathbf{R}$ hoặc $\mathbf{C}$. Ta ký hiệu G là một nhóm compact địa phương được trang bị một độ đo Haar trái $\mu$. Ta sẽ viết $\mathscr{L}^p(G) =\mathscr{L}_{\mathbf{C}}^p(G, \mu)$ và $L^p(G) = L^p_{\mathbf{C}}(G, \mu)$ với mọi $p\in [1,+\infty ]$.

### 1. Tính liên tục của một số biểu diễn

#### Mệnh đề 1 {#ts-v-s2-prop-1 .statement tag=03A4}

Cho H là một nhóm compact địa phương. Cho $\varrho_1$ (tương ứng $\varrho_2$) là một biểu diễn liên tục của G (tương ứng của H) trong một không gian vectơ lồi địa phương K tách được $E_1$ (tương ứng $E_2$). Cho F là không gian $\mathscr{L}(E_1; E_2)$ được trang bị tôpô hội tụ compact. Biểu diễn $\varrho$ của $G\times H$ trong F được xác định bởi $\varrho (g, h)u=\varrho_2(h)\circ u\circ \varrho_1(g^{-1})$ với $(g, h)\in G\times H$ là liên tục.

Cho $\mathscr{L}_c(E_1; E_2)$ là không gian $\mathscr{L}(E_1; E_2)$ được trang bị tôpô hội tụ compact. Cho $\mathfrak{F}_1$ (tương ứng $\mathfrak{F}_2,\mathfrak{F}_3$) là một cơ sở lọc trong G hội tụ đến $e$ (tương ứng một cơ sở lọc trong $\mathscr{L}_c(E_1; E_2)$ hội tụ đến 0, một cơ sở lọc trong H hội tụ đến $e$). Vì G và H là compact địa phương, tồn tại các phần tử $C\in \mathfrak{F}_1$ và $D\in \mathfrak{F}_3$ tương đối compact. Tập hợp $\varrho_1(C^{-1})$ là đẳng liên tục trong $\mathscr{L}(E_1) ($cf. INT, VIII, p. 129, § 2, n$^o1$, rem. 2, a$'))$. Theo prop. 9 của EVT, III, p. 33 và prop. 4 của EVT, III, p. 31, ánh xạ được xác định bởi $(u, v)\mapsto u\circ v$ từ $\mathscr{L}_c(E_1; E_2)\times \varrho_1(C^{-1})$ vào $\mathscr{L}_c(E_1; E_2)$ là liên tục. Cơ sở lọc $\mathfrak{F}_2\circ \varrho_1(\mathfrak{F}^{-1}_1)$ do đó hội tụ đến 0 trong $\mathscr{L}_c(E_1; E_2)$. Tập hợp $\varrho_2(D)$ là đẳng liên tục trong $\mathscr{L}(E_2) ($cf. INT, VIII, p. 129, § 2, n$^o1$, rem. 2), và với mọi $x\in E_2$, tập hợp $\varrho_2(D)x\subset E_2$ là tương đối compact. Do đó, $\varrho_2(D)$ là tương đối compact trong $\mathscr{L}(E_2)$ được trang bị tôpô hội tụ compact (TG, X, p. 18, cor. 1). Ánh xạ được xác định bởi $(u, v)\mapsto u\circ v$ từ $\overline{\varrho_2(D)}\times \mathscr{L}_c(E_1; E_2)$ vào $\mathscr{L}_c(E_1; E_2)$ là liên tục theo prop. 9 của EVT, III, p. 33 và prop. 4 của EVT, III, p. 31. Vì vậy cơ sở lọc $\varrho (\mathfrak{F}_1\times \mathfrak{F}_3)(\mathfrak{F}_2)$ hội tụ đến 0 trong $\mathscr{L}_c(E_1; E_2)$. Điều này kéo theo mệnh đề.

#### Hệ quả {#ts-v-s2-n1-cor-1 .statement tag=03A5}

Cho $\varrho$ là một biểu diễn liên tục của G trong một không gian vectơ lồi địa phương K tách được E. Biểu diễn đối ngẫu contragredient $\breve{\varrho}$ là liên tục khi $E'$ được trang bị tôpô hội tụ compact.

Điều này suy ra từ mệnh đề bằng cách lấy $H =\{e\},\varrho_1=\varrho$ và $\varrho_2$ là biểu diễn tầm thường trên K.

#### Nhận xét {#ts-v-s2-n1-rem-1 .statement tag=03A6}

Biểu diễn đối ngẫu contragredient không nhất thiết liên tục khi $E'$ được trang bị tôpô mạnh (cf. INT, VIII, p. 191, § 2, exercise 3, d)). Ta có thể chứng minh rằng nó là như vậy nếu không gian E là nửa phản xạ (loc. cit., c)).

### 2. Mở rộng các biểu diễn đến các không gian độ đo

Trong số này, giả sử rằng $K =\mathbf{C}$.

Cho $\varrho$ là một biểu diễn tuyến tính liên tục của G trong một không gian lồi địa phương tựa đầy đủ tách được E. Cho $\mathscr{M}_c(G)$ là không gian các độ đo có giá compact trên G được trang bị tôpô hội tụ compact; đây là đối ngẫu của không gian $\mathscr{C}(G)$. Với mỗi độ đo $\nu \in \mathscr{M}_c$(G), đặt

$$
\varrho (\nu ) =\int_G\varrho (g)d\nu (g)
$$

Đây là một phần tử của $\mathscr{L}(E)$. Đặc biệt, ta có $\varrho (\varepsilon_g) =\varrho (g)$ với mọi $g\in G$.

Theo INT, VIII, p. 136, § 2, n$^o6$, ánh xạ $\nu \mapsto \varrho (\nu )$ là một ánh xạ tuyến tính liên tục từ $\mathscr{M}_c(G)$ vào không gian $\mathscr{L}(E)$ được trang bị tôpô hội tụ compact. Theo INT, VIII, p. 145, § 3, n$^o3$, prop. 11, nó là một cấu xạ của các đại số có đơn vị.

Cho $x\in E$. Ánh xạ từ $\mathscr{M}_c(G)$ vào E được xác định bởi $\nu \mapsto \varrho (\nu )x$ là liên tục khi $\mathscr{M}_c(G)$ được trang bị tôpô hội tụ compact (INT, VI, p. 27, § 1, n$^o$ 7, prop. 16 và EVT, III, p. 31, prop. 4).

Đối với $f\in \mathscr{L}^1(G)$ triệt tiêu bên ngoài một tập con compact của G, độ đo $f\cdot \mu$ có giá compact và ta sẽ ký hiệu bởi $\varrho^\mu(f)$, hoặc bởi $\varrho (f)$ khi không thể có sự nhầm lẫn, tự đồng cấu $\varrho (f\cdot \mu)$ của E. Tự đồng cấu này chỉ phụ thuộc vào lớp $\widetilde{f}$ của $f$ trong $L^1$(G), và nó cũng sẽ được ký hiệu bởi $\varrho^\mu(\widetilde{f})$ hoặc $\varrho (\widetilde{f})$.

Tương tự, cho $\varrho$ là một biểu diễn tuyến tính liên tục và bị chặn của G trong một không gian Banach E. Với mọi độ đo bị chặn $\nu \in \mathscr{M}^1$(G), đặt

$$
\varrho (\nu ) =\int_G\varrho (g)d\nu (g)
$$

Theo INT, VIII, loc. cit., ánh xạ $\nu \mapsto \varrho (\nu )$ là một cấu xạ có đơn vị liên tục của các đại số Banach từ đại số $\mathscr{M}^1(G)$ của các độ đo phức bị chặn trên G vào đại số Banach $\mathscr{L}(E)$.

Cho $\rho$ là hàm $g\mapsto  \|\varrho (g)\|$ trên G; đại số được ký hiệu $\mathscr{M}^{\rho}$ trong INT, VIII, p. 145, prop. 11 (các phần tử của nó là các độ đo $\nu$ sao cho $\rho \in \mathscr{L}^1(\nu )$) trùng với đại số Banach $\mathscr{M}^1(G)$. Thật vậy, đặt M = sup $\rho$. Ta có $M>0$ vì $\rho (e) = 1$, và $M^{-1}\leqslant \rho \leqslant M$ vì $\|\varrho (e)\|\leqslant \|\varrho (g)\| \|\varrho (g^{-1})\|$ với mọi $g\in G$; do đó $\rho \in \mathscr{L}^1(\nu )$ khi và chỉ khi $\nu$ là một độ đo bị chặn.

Nếu $f\in \mathscr{L}^1$(G), ta cũng sẽ ký hiệu bởi $\varrho^\mu(f)$ hoặc đơn giản là $\varrho (f)$ tự đồng cấu $\varrho (f\cdot \mu)$, và tương tự đối với lớp $\widetilde{f}$ của $f$ trong $L^1(G)$.

#### Bổ đề 1 {#ts-v-s2-lem-1 .statement tag=03A7}

Cho $\varrho$ là một biểu diễn unita của G trong một không gian Hilbert E. Ánh xạ $\nu \mapsto \varrho (\nu )$ từ $\mathscr{M}^1(G)$ vào $\mathscr{L}(E)$ là một cấu xạ có đơn vị của các đại số Banach đối hợp.

Từ những điều đã nêu trên, chỉ cần chứng minh rằng cấu xạ $\nu \mapsto \varrho (\nu )$ là đối hợp. Cho $\nu \in \mathscr{M}^1(G)$. Độ đo $\nu^*$ là độ đo liên hợp của độ đo $\check{\nu}($I, p. 99, ví dụ 4). Theo định nghĩa của độ đo liên hợp (INT, III, p. 52, § 1, n$^o5$), ta tính được

$$
\langle x|\varrho (\nu )y\rangle =\int\langle x|\varrho (g)y\rangle d\nu (g)
$$

$$
=\int^G_G\langle \varrho (g^{-1})x|y\rangle d\nu (g) =\int_G\langle \varrho (g)x|y\rangle d\check{\nu}(g)
$$

$$
=\int_G\langle y|\varrho (g)x\rangle d\nu^*(g) =\langle \varrho (\nu^*)x|y\rangle
$$

với mọi $x$ và $y$ trong E, do đó $\varrho (\nu )^*=\varrho (\nu^*)$.

Cho $\varrho$ là một biểu diễn tuyến tính liên tục (tương ứng liên tục và bị chặn) của G trong một không gian lồi địa phương gần đầy đủ E (tương ứng một không gian Banach E). Nếu F là một không gian con đóng của E xác định một biểu diễn con $\varrho_F$ của $\varrho$, thì với mọi độ đo $\nu \in \mathscr{M}_c(G)$ (tương ứng $\nu \in \mathscr{M}^1(G)$), ánh xạ tuyến tính $\varrho (\nu )$ giữ ổn định không gian con F và trùng với $\varrho_F(\nu )$ trên F.

Ngược lại, cho $F\subset E$ là một không gian con đóng, ổn định dưới các ánh xạ tuyến tính $\varrho (f)$ với mọi hàm $f\in \mathscr{K}(G)$. Khi đó F xác định một biểu diễn con của $\varrho$ (INT, VIII, p. 139, § 2, n$^o7$, mệnh đề 10).

Nhắc lại (A, VIII, p. 388) rằng một hàm $f: G\rightarrow \mathbf{C}$ được gọi là trung tâm nếu, với mọi $g$ và $h$ trong G, ta có $f(gh) =f(hg)$. Điều này tương đương với việc nói rằng $f$ là bất biến qua phép liên hợp.

#### Định nghĩa 1 {#ts-v-s2-def-1 .statement tag=03A8}

Một độ đo bị chặn $\nu \in \mathscr{M}^1(G)$ được gọi là trung tâm nếu ta có $\varepsilon_g*\nu =\nu *\varepsilon_g$ với mọi $g\in G$.

Nếu G là đơn môđula và $f\in \mathscr{C}(G)$ là $\mu$-khả tích, độ đo $f\cdot \mu$ là trung tâm khi và chỉ khi $f$ là trung tâm.

Cho $\varrho$ là một biểu diễn liên tục bị chặn của G trong một không gian Banach E (tương ứng một biểu diễn liên tục của G trong một không gian lồi địa phương tách được gần đầy đủ E). Với mọi độ đo trung tâm bị chặn $\nu$ trên G (tương ứng mọi độ đo trung tâm có giá compact $\nu$ trên G), ánh xạ tuyến tính $\varrho (\nu )$ là một cấu xạ G từ $\varrho$ vào $\varrho$. Thật vậy, với mọi $g\in G$, ta có

$$
\varrho (\nu )\varrho (g) =\varrho (\nu *\varepsilon_g) =\varrho (\varepsilon_g*\nu ) =\varrho (g)\varrho (\nu )
$$

### 3. Tiêu chuẩn cho tính nửa đơn

#### Mệnh đề 2 {#ts-v-s2-prop-2 .statement tag=03A9}

Cho $\varrho$ là một biểu diễn unita của G trong một không gian Hilbert phức E. Cho $\mathfrak{F}$ là một cơ sở của bộ lọc trên $\mathscr{M}_c(G)$ hội tụ đến độ đo $\varepsilon_e$ đối với tôpô hội tụ compact. Giả sử rằng tồn tại $M\in \mathfrak{F}$ sao cho $\varrho (\nu )$ là một tự đồng cấu compact của E với mọi $\nu \in M$.

Khi đó biểu diễn unita $\varrho$ là nửa đơn và mọi biểu diễn unita bất khả quy của G có bội số hữu hạn trong $\varrho$.

Trước hết ta hãy chứng minh một bổ đề.

#### Bổ đề 2 {#ts-v-s2-lem-2 .statement tag=03AA}

Cho $\varrho_1$ là một biểu diễn unita khác không của G đẳng cấu với một biểu diễn con của $\varrho$. Tồn tại một độ đo $\nu \in M$ sao cho $\varrho_1(\check{\nu}*\nu )$ là một tự đồng cấu compact Hermit khác không của không gian của $\varrho_1$. Đặc biệt, tồn tại một số thực khác không $\lambda$ sao cho không gian con riêng của $\varrho_1(\check{\nu}*\nu )$ tương ứng với $\lambda$ là khác không.

Ta có thể giả sử rằng $\varrho_1$ là một biểu diễn con của $\varrho$. Cho $E_1$ là không gian của nó. Với mọi độ đo $\nu \in M$, tự đồng cấu $\varrho_1(\nu )$ được suy ra từ $\varrho (\nu )$ bằng cách chuyển qua các không gian con. Giả thiết và mệnh đề 3 của III, p. 5 do đó suy ra rằng $\varrho_1(\nu )$ là compact.

Vì $\mathfrak{F}$ hội tụ đến độ đo $\varepsilon_e$ trong $\mathscr{M}_c(G)$ được trang bị tôpô của sự hội tụ compact và vì không gian $E_1$ là khác không, tồn tại $\nu \in M$ sao cho $v=\varrho_1(\nu )$ là một tự đồng cấu khác không của $E_1$ (xem No.$^o2$ của V, p. 400). Tự đồng cấu $u=\varrho_1(\check{\nu}*\nu )$ bằng $v^*\circ v$ (bổ đề 1 của V, p. 401); do đó nó khác không (EVT, V, p. 39, mệnh đề 2), Hermit và compact, vì $v$ là compact.

Vì $u$ là Hermit và khác không, phổ của nó không thu gọn về không (ví dụ 1 của I, p. 110). Cuối cùng, vì $u$ là compact, mọi $\lambda \in$ Sp($u$)$-\{0\}$ là một trị riêng của $u$ (mệnh đề 2 của III, p. 83).

Bây giờ chứng minh mệnh đề.

Ta sẽ dùng mệnh đề 7 của V, p. 391 để thiết lập rằng $\varrho$ là nửa đơn. Cho $\varrho_1$ là một biểu diễn con khác không của $\varrho$, và $E_1\subset E$ là không gian của nó; ta phải chứng minh rằng $\varrho_1$ chứa một biểu diễn con bất khả quy.

Cho $\nu \in M$ sao cho $u=\varrho_1(\check{\nu}*\nu )$ là một tự đồng cấu Hermit compact khác không của không gian của $\varrho_1$, và cho $\lambda$ khác không sao cho không gian con riêng F của $u$ ứng với $\lambda$ là khác không (bổ đề 2). Không gian F có số chiều hữu hạn (mệnh đề 5 của III, p. 90). Tồn tại một biểu diễn con $\varrho_2$ của $\varrho_1$ trên một không gian con $E_2$ của $E_1$ sao cho $E_2\cap F$ là khác không và có chiều cực tiểu. Cho $x$ là một phần tử khác không của $E_2\cap F$, và cho $E_3$ là biểu diễn con của $\varrho_1$ sinh bởi $x$. Khi đó $E_3\subset E_2$, do đó $E_3\cap F = E_2\cap F$ bởi tính cực tiểu của chiều của $E_2\cap F$.

Ta chứng minh rằng biểu diễn $E_3$ là bất khả quy. Cho $E_4\subset E_3$ là một không gian con đóng ổn định dưới G. Ta có $E_2\cap F = (E_4\cap F)\oplus (E^{\circ}_4\cap F)$, trong đó $E^{\circ}_4$ chỉ phần trực giao của $E_4$ trong $E_3$ (thực vậy, nếu $y\in E_2\cap F$, gọi $y_4\in E_4$ là phép chiếu trực giao của nó trên $E_4$; vì $E_4$ và $E^{\circ}_4$ ổn định dưới $u$, vectơ $u(y_4)$ là phép chiếu trực giao của $u(y) =\lambda y$ trên $E_4$, do đó $u(y_4) =\lambda y_4$, điều này có nghĩa là $y_4\in E_4\cap F$, và mệnh đề được suy ra). Tính cực tiểu của chiều của $E_2\cap F$ khi đó suy ra rằng hoặc là $E_4\cap F = E_2\cap F$, hoặc là $E^{\circ}_4\cap F = E_2\cap F$. Trong trường hợp thứ nhất, ta có $x\in E_4$, do đó $E_4= E_3$, và trong trường hợp thứ hai, ta có $x\in E^{\circ}_4$, do đó $E^{\circ}_4= E_3$ và $E_4=\{0\}$. Biểu diễn $E_3$ do đó là bất khả quy.

Suy ra từ Mệnh đề 7 của V, p. 391 rằng biểu diễn $\varrho$ là nửa đơn.

Cho $\pi$ là một biểu diễn đơn vị bất khả quy của G có bội số trong $\varrho$ khác không; gọi $E_{\pi}$ là không gian của nó. Tồn tại một độ đo $\nu \in M$ và một số thực khác không $\lambda$ sao cho $u=\pi (\check{\nu}*\nu )$ là một tự đồng cấu Hermit compact khác không của $E_{\pi}$ và không gian con thực sự của $u$ tương ứng với $\lambda$ là khác không (Bổ đề 2). Gọi F là không gian con thực sự của $v=\varrho (\check{\nu}*\nu )$ tương ứng với $\lambda$. Với mọi biểu diễn con $E_1$ của E đẳng cấu với $\pi$, tự đồng cấu của $E_1$ suy ra từ $v$ bằng cách chuyển qua các không gian con được đồng nhất với $u$, do đó giao của $E_1$ và F là khác không. Vì vậy, bội số của $\pi$ trong $\varrho$ nhỏ hơn chiều của không gian F, là hữu hạn (Mệnh đề 5 của III, p. 90).

#### Ví dụ {#ts-v-s2-n3-exa-1 .statement tag=03AB}

Giả sử rằng G là đơn môđula, chẳng hạn rằng G là một nhóm Lie nửa đơn thực. Cho $\Gamma \subset G$ là một nhóm con rời rạc sao cho thương $X = \Gamma \backslash G$ là compact. Nhóm G tác động bên phải bằng phép nhân trên X. Gọi $\beta$ là độ đo đếm trên Γ và đặt $\widetilde{\mu}=\mu/\beta$ (INT, VII, p. 44, § 2, No.$^o2$, Def. 1); nó là một độ đo G-bất biến bị chặn trên X.

Với mọi $f\in \mathscr{L}^2(X,\widetilde{\mu})$ và mọi $g\in$ G, ta định nghĩa hàm $\varrho (g)f\in \mathscr{L}^2(X,\widetilde{\mu})$ bởi $\varrho (g)f(x) =f(x\cdot g)$. Ánh xạ $\varrho (g)$ là một ánh xạ tuyến tính liên tục, ánh xạ này cảm sinh qua phép chuyển qua các thương một ánh xạ unita trên $L^2(X,\widetilde{\mu})$, vẫn được ký hiệu là $\varrho (g)$. Ánh xạ $\varrho$ là một biểu diễn unita của G trong $L^2(X,\widetilde{\mu})$ (INT, VII, p. 135, § 2, No.$^o5$, Prop. 8).

Cho $\varphi \in \mathscr{K}(G)$. Với mọi tập compact $L_1$ và $L_2$ của G, giao T của Γ và tập compact $L_1$Supp($\varphi$ )$L^{-1}_2$ là hữu hạn. Với mọi $(g, h)\in L_1\times L_2$, chuỗi $\sum_{\gamma\in\Gamma}\varphi (g^{-1}\gamma h)$ trùng với tổng

hữu hạn $\sum_{\gamma\in T}\varphi (g^{-1}\gamma h)$. Vì G là địa phương compact, tổng của

chuỗi này, được ký hiệu bởi $k_{\varphi}(g, h)$, là một hàm liên tục trên $G\times G$.

Cho $g\in G$ và $(\gamma , \eta )\in \Gamma \times \Gamma$. Ta có $k_{\varphi}(\gamma g, \eta h) =k_{\varphi}(g, h)$, do đó $k_{\varphi}$ xác định qua phép chuyển qua thương một hàm liên tục trên $X\times X$, được ký hiệu là $\widetilde{k}_{\varphi}$. Ngoài ra ta có $\widetilde{k}_{\varphi}\in \mathscr{L}^2(X\times X,\widetilde{\mu}\otimes \widetilde{\mu})$, vì không gian X được giả thiết là compact.

Ta ký hiệu bởi $\dot{x}$ ảnh trong X của một phần tử $x$ của G qua phép chiếu chính tắc. Cho $\varphi \in \mathscr{K}(G)$. Với $f\in \mathscr{L}^2(X,\widetilde{\mu})$ và $x\in G$, ta có

$$
\varrho (\varphi )f( \dot{x}) =\int_G\varphi (g) (\varrho (g)f)( \dot{x})d\mu(g) =\int_G\varphi (g)f( \dot{x}\cdot g)d\mu(g)
$$

$$
=\int_G\varphi (x^{-1}y)f( \dot{y})d\mu(y) =\int_{\Gamma\backslash G}((\sum_{\gamma\in\Gamma}\varphi (x^{-1}\gamma y))f( \dot{y})d\widetilde{\mu}( \dot{y})
$$

(INT, VII, p. 46, § 2, No.$^o3$, Prop. 5). Vì $\widetilde{k}_{\varphi}$ thuộc không gian $\mathscr{L}^2(X\times X,\widetilde{\mu}\otimes \widetilde{\mu})$, suy ra tự đồng cấu $\varrho (\varphi )$ của $L^2(X,\widetilde{\mu})$ trùng với tự đồng cấu Hilbert-Schmidt có hạt nhân $\widetilde{k}_{\varphi}$; tự đồng cấu này do đó là compact (Cor. 1 of III, p. 33)

Tồn tại một dãy $(\varphi_n)_{n\in\mathbf{N}}$ các hàm trong $\mathscr{K}_+(G)$ có tích phân 1 sao cho $\varphi_n\cdot \mu$ hội tụ đến $\varepsilon_e$ trong $\mathscr{M}_c(G)$ được trang bị tôpô của hội tụ compact (INT, VIII, p. 139, § 2, No.$^o7$, Cor. 2). Mệnh đề 2 do đó suy ra rằng biểu diễn $\varrho$ là nửa đơn và các bội số của các biểu diễn unita bất khả quy của G trong $\varrho$ là hữu hạn.

Các biểu diễn unita bất khả quy của G mà bội số của chúng trong $\varrho$ không bằng không được gọi là các biểu diễn Γ-automorphic của nhóm G.

### 4. Các biểu diễn chính quy

Cho $p$ là một số thực $\geqslant 1$ và $\mu'$ là một độ đo Haar phải trên G.

Với mọi $g\in G$ và mọi hàm $f\in \mathscr{L}^p(G, \mu)$, ta ký hiệu bởi $\boldsymbol{\gamma }^{(p)}_G(g)f$ hàm $x\mapsto f(g^{-1}x)$ trên G. Ánh xạ $g\mapsto \boldsymbol{\gamma }^{(p)}_G(g)$ là một biểu diễn tuyến tính liên tục của G trong $\mathscr{L}^p(G)$. Chuyển qua các thương, nó cảm sinh một biểu diễn tuyến tính đẳng cự liên tục của G trong $L^p(G)$ (INT, VIII, p. 135, § 2, n$^o5$, Prop. 8), được ký hiệu bởi $\boldsymbol{\gamma }^{(p)}_G$.

Tương tự, với mọi $g\in G$ và mọi hàm $f\in \mathscr{L}^p(G, \mu')$, ta ký hiệu bởi $\boldsymbol{\delta }^{(p)}_G(g)f$ hàm $x\mapsto f(xg)$ trên G. Ánh xạ $g\mapsto \boldsymbol{\delta }^{(p)}_G(g)$ là một biểu diễn tuyến tính liên tục của G trong $\mathscr{L}^p(G, \mu')$. Chuyển qua các thương, nó cảm sinh một biểu diễn tuyến tính đẳng cự liên tục của G trong $L^p(G, \mu') ($cf. INT, VIII, p. 136, § 2, n$^o5)$.

Ta nói rằng $\boldsymbol{\gamma }_G^{(p)}$ là biểu diễn chính quy trái của G trong $\mathscr{L}^p(G)$ hoặc $L^p(G)$ và rằng $\boldsymbol{\delta }^{(p)}_G$ là biểu diễn chính quy phải của G trong $\mathscr{L}^p(G, \mu')$ hoặc $L^p(G, \mu')$.

#### Bổ đề 3 {#ts-v-s2-lem-3 .statement tag=03AC}

Cho $p$ là một số thực $\geqslant 1$. Biểu diễn chính quy trái (tương ứng phải) của G trong $L^p(G, \mu) ($tương ứng trong $L^p(G, \mu'))$ là trung thành.

Chính xác hơn, cho $q$ là số mũ liên hợp của $p$ và cho $g$ là một phần tử của G sao cho $g\not =e$.

a) Tồn tại một hàm $\varphi \in \mathscr{K}(G)$, dương và khác không trong $L^q(G, \mu)$, sao cho $\langle \varphi ,\boldsymbol{\gamma }^{(p)}_G(g)\varphi \rangle = 0$;

b) Tồn tại một hàm $\varphi \in \mathscr{K}(G)$, dương và khác không trong $L^q(G, \mu')$, sao cho $\langle \varphi ,\boldsymbol{\delta }^{(p)}_G(g)\varphi \rangle = 0$.

Ta xét trường hợp của biểu diễn chính quy trái $\boldsymbol{\gamma }^{(p)}_G$, trường hợp của biểu diễn chính quy phải là tương tự. Mệnh đề a) suy ra rằng $\boldsymbol{\gamma }^{(p)}_G$ là trung thành, vì nếu $g\not =e$ là một phần tử của G, và nếu $\varphi$ là như trong a), thì ta có $\varphi \not =\boldsymbol{\gamma }^{(p)}_G(g)\varphi$ vì $\langle \varphi , \varphi \rangle =\int_G\varphi^2>0$.

Do đó ta hãy chứng minh a). Cho $g\not =e$ trong G. Cho C là một lân cận compact đối xứng của $e$ sao cho $g \notin C^2$ và cho $\varphi \in \mathscr{K}(G)$ là một hàm liên tục dương có nguyên bằng 1 với giá chứa trong C; hàm $\varphi$ là khác không trong $L^p(G, \mu)$. Vì $C\cap g^{-1}C =\emptyset$, ta có

$$
\langle \varphi ,\boldsymbol{\gamma }^{(p)}_G(g)\varphi \rangle =\int_G\varphi (x)\varphi (g^{-1}x)d\mu(x) = 0
$$

Cho $\varrho$ là một biểu diễn bị chặn liên tục của G trong một không gian Banach E. Với mọi $f\in L^1(G)$ (tương ứng $f'\in L^1(G, \mu')$) và mọi $g\in G$, ta có

(1) $\varrho (g)\varrho (f\cdot \mu) =\varrho (\varepsilon_g*(f\cdot \mu)) =\varrho (\boldsymbol{\gamma }$[^1]$_G(g)f\cdot \mu)$,

(2) $\varrho (f'\cdot \mu')\varrho (g) =\varrho ((f'\cdot \mu')*\varepsilon_g) =\varrho (\boldsymbol{\delta }$[^1]$_G(g^{-1})f'\cdot \mu')$

(INT, VIII, p. 144, § 3, n$^o2$, công thức (5)).

Giả sử G đơn môđula, và đặt $\mu'=\mu$. Biểu diễn chính quy hai bên của G trong $\mathscr{L}^p(G)$ (tương ứng trong $L^p(G)$) là biểu diễn $\boldsymbol{\varrho }^{(p)}_G$ của $G\times G$ trong $\mathscr{L}^p(G)$ (tương ứng trong $L^p(G)$) sao cho

$$
\boldsymbol{\varrho }_G^{(p)}(g_1, g_2) =\boldsymbol{\gamma }_G^{(p)}(g_1)\boldsymbol{\delta }_G^{(p)}(g_2) =\boldsymbol{\delta }_G^{(p)}(g_2)\boldsymbol{\gamma }_G^{(p)}(g_1)
$$

Đó là một biểu diễn tuyến tính liên tục (Bổ đề 1 của V, p. 377). Nó thỏa mãn

$$
(\boldsymbol{\varrho }_G^{(p)}(g_1, g_2)f)(x) =f(g_1^{-1}xg_2)
$$

với mọi $f\in \mathscr{L}^p$(G), mọi $(g_1, g_2)\in G\times G$ và mọi $x\in G$.

#### Nhận xét {#ts-v-s2-n4-rem-1 .statement tag=03AD}

Biểu diễn chính quy hai bên của G trong $L^p(G, \mu)$ không nhất thiết trung thành; hạt nhân của nó là ảnh của tâm của G qua ánh xạ $g\mapsto (g, g)$ (bài tập 4 của V, p. 487).

Khi $p= 2$, biểu diễn chính quy trái $\boldsymbol{\gamma }$[^2]$_G$ của G trong không gian Hilbert phức $L^2(G, \mu)$ là unita, vì nó đẳng cự. Tương tự, biểu diễn chính quy phải $\boldsymbol{\delta }_G$[^2] trong $L^2(G, \mu')$ là unita.

Ta sẽ viết đơn giản $\boldsymbol{\gamma }_G=\boldsymbol{\gamma }$[^2]$_G$ và $\boldsymbol{\delta }_G=\boldsymbol{\delta }$[^2]$_G$, và ta sẽ gọi các biểu diễn này là các biểu diễn chính quy trái và phải của G.

Nếu G là đơn môđula, biểu diễn chính quy hai bên $\boldsymbol{\varrho }$[^2]$_G$ của $G\times G$ trong $L^2(G, \mu)$ là unita. Ta sẽ viết nó đơn giản là $\boldsymbol{\varrho }_G$.

#### Bổ đề 4 {#ts-v-s2-lem-4 .statement tag=03AE}

Cho $p$ là một số thực $\geqslant 1$. Với $f\in \mathscr{L}^1(G)$, ánh xạ tuyến tính $\boldsymbol{\gamma }^{(p)}_G(f)$ trùng với tự đồng cấu của $L^p(G)$ được xác định bởi $\varphi \mapsto f*^\mu\varphi$.

Điều này suy ra từ INT, VIII, p. 157, § 4, No.$^o2$, Mệnh đề 6, có tính đến công thức (14) của INT, VIII, p. 165.

#### Nhận xét {#ts-v-s2-n4-rem-2 .statement tag=03AF}

Nhắc lại rằng, với mọi hàm $f$ trên G, người ta định nghĩa hàm $\check{f}$ trên G bởi $\check{f}(g) =f(g^{-1})$ với mọi $g\in G$ (INT, VII, p. 12, § 1, No.$^o1$, công thức (12)).

Người ta kiểm tra rằng nếu $f\in \mathscr{L}^1$(G), ánh xạ tuyến tính $u=\boldsymbol{\delta }^{(p)}_G(f)$ thỏa mãn quan hệ

$$
u(\widecheck{\varphi}) =f*\check{\varphi}
$$

với mọi $\varphi \in L^p(G, \mu')$.

### 5. Các hàm hiệp biến

Trong số này, một nhóm con đóng H của G được cố định. Người ta ký hiệu bằng $\varpi$ phép chiếu chính tắc của G lên $G/H$.

Ngoài độ đo Haar $\mu$ trên G, một độ đo Haar trái $\beta$ trên H được cố định.

Theo INT, VII, p. 56, § 2, n$^o5$, th. 2, tồn tại một hàm liên tục $\kappa : G\rightarrow \mathbf{R}_+^*$ sao cho $\kappa (xh) = \Delta_H(h)\Delta_G(h)^{-1}\kappa (x)$ với mọi $(x, h)\in G\times H$. Ta cố định một hàm $\kappa$ như vậy. Ta ký hiệu bởi $\nu$ độ đo $(\kappa \cdot \mu)/\beta$ trên $G/H$; theo loc. cit., đây là một độ đo dương khác không gần bất biến bởi G. Giá đỡ của nó bằng $G/H$ (INT, VII, p. 10, § 1, n$^o1$). Theo INT, VII, p. 43, § 2, n$^o2$, Mệnh đề 4, độ đo $\nu$ là độ đo duy nhất trên $G/H$ sao cho độ đo $\nu^{\sharp}$ trên G bằng $\kappa \cdot \mu$. Ta trang bị không gian $G/H$ với độ đo $\nu$ (sao cho ta viết, chẳng hạn, $\mathscr{L}^p(G/H) =\mathscr{L}^p(G/H, \nu )$).

Ta sẽ nói rằng một tập hợp $S\subset G$ là không đáng kể modulo H nếu $\varpi (S)$ là $\nu$-không đáng kể. Điều kiện này không phụ thuộc vào sự lựa chọn các độ đo Haar trên G và trên H. Nó kéo theo rằng S là $\mu$-không đáng kể địa phương (INT, VII, p. 47, § 2, n$^o3$, Mệnh đề 6, a)). Ta sẽ nói rằng một tính chất của một phần tử của G là đúng hầu khắp nơi modulo H nếu tập hợp các phần tử của G mà tính chất này không đúng là không đáng kể modulo H.

Cho $\pi$ là một biểu diễn unita của H trong một không gian Hilbert E. Ta ký hiệu bởi $\mathscr{F}_{\pi}(G)$ không gian vectơ của các hàm $f$ trên G với các giá trị trong E sao cho $f(xh) =\pi (h)f(x)$ với mọi $(x, h)\in G\times H$. Các phần tử của $\mathscr{F}_{\pi}(G)$ được gọi là các hàm $\pi$-tương biến trên G.

Không gian $\mathscr{F}_1(G)$ liên kết với biểu diễn tầm thường của G trên $\mathbf{C}$ được đồng nhất với không gian $\mathscr{F}(G/H)$ của các hàm có giá trị phức trên $G/H$ bởi ánh xạ $f\mapsto f\circ \varpi$ từ $\mathscr{F}(G/H)$ vào $\mathscr{F}_1(G)$.

Với mỗi hàm $f$ trong $\mathscr{F}_{\pi}$(G), hàm $\|f\|$ thuộc về $\mathscr{F}_1(G)$ vì $\pi$ là unita. Điều này cho phép đồng nhất $\|f\|$ với một hàm trên $G/H$, và ta sẽ viết chẳng hạn $\|f(xH)\|$ cho giá trị của hàm này tại một phần tử $xH$ của $G/H$.

Một hàm $f$ của $\mathscr{F}_{\pi}(G)$ sẽ được gọi là bằng không ngoài một tập compact modulo H nếu $\|f\|$ bằng không ngoài một tập con compact của $G/H$. Điều này tương đương với việc nói rằng tồn tại một tập con compact K của G sao cho $f$ bằng không ngoài $K\cdot H$ (TG, III, p. 33, Mệnh đề 10).

Ta ký hiệu bởi $\mathscr{K}_{\pi}(G)$ không gian của các hàm liên tục trên G thuộc về $\mathscr{F}_{\pi}(G)$ và có giá compact modulo H.

Một không gian tương tự như $\mathscr{K}_{\pi}(G)$ đã được định nghĩa trong INT, VII, p. 39, §2, n$^o1$, khi $\pi$ là một đồng cấu liên tục của H vào $\mathbf{R}^*_+$.

Cho $p\in [1,+\infty [$. Với mọi $f\in \mathscr{F}_{\pi}$(G), ta đặt

$$
N_p(f) =(\int_{G/H}^*\|f\|^pd\nu )^{1/p}
$$

Đây là một số thực hoặc $+\infty$. Ta ký hiệu bởi $\mathscr{F}_{\pi}^p(G, \nu )$, hoặc đơn giản là $\mathscr{F}_{\pi}^p$(G), không gian con của các hàm $f\in \mathscr{F}_{\pi}(G)$ sao cho $N_p(f)$ là hữu hạn. Không gian $\mathscr{F}_{\pi}^p(G)$ được trang bị ánh xạ $N_p$ là một không gian nửa chuẩn.

Không gian $\mathscr{K}_{\pi}(G)$ được chứa trong $\mathscr{F}_{\pi}^p(G)$. Bao đóng của nó trong $\mathscr{F}_{\pi}^p(G)$ được ký hiệu bởi $\mathscr{L}_{\pi}^p(G, \nu )$, hoặc đơn giản là $\mathscr{L}_{\pi}^p(G)$; ta nói rằng đây là không gian các hàm $\pi$-tương biến trên G mà lũy thừa $p^e$ của chúng khả tích modulo H.

Các mệnh đề sau đây, khi $\pi$ là biểu diễn tầm thường có chiều 1, là hệ quả của INT, IV, p. 128, § 3, n$^o3$, prop. 6 và p. 131, §3, n$^o4$, th. 3.

#### Mệnh đề 3 {#ts-v-s2-prop-3 .statement tag=03AG}

a) Cho $(f_n)_{n\in\mathbf{N}}$ là một dãy trong $\mathscr{F}_{\pi}^p(G)$ sao cho chuỗi

$$
\sum_{n=0}^{+\infty}N_p(f_n)
$$

hội tụ. Khi đó chuỗi với số hạng tổng quát $f_n(g)$ hội tụ tuyệt đối đối với $g$ nằm ngoài một tập hợp T không đáng kể modulo H. Cho $f$ là hàm trên G nhận giá trị trong E bằng tổng của chuỗi này trên G - T và bằng 0 trên T. Khi đó ta có $f\in \mathscr{F}_{\pi}^p(G)$ và chuỗi với số hạng tổng quát $f_n$ hội tụ về $f$ trong không gian $\mathscr{F}_{\pi}^p(G)$;

b) Cho $(f_n)$ là một dãy hội tụ trong $\mathscr{L}_{\pi}^p(G)$ về một hàm $f$. Tồn tại một dãy con $(f_{n_k})$ được trích ra từ $(f_n)$ sao cho $f_{n_k}(g)$ hội tụ về $f(g)$ với mọi $g$ nằm ngoài một tập hợp không đáng kể modulo H;

c) Các không gian nửa chuẩn $\mathscr{F}_{\pi}^p(G)$ và $\mathscr{L}_{\pi}^p(G)$ là đầy đủ.

Trong mệnh đề a), nói rằng chuỗi với số hạng tổng quát $f_n$ hội tụ về $f$ trong không gian $\mathscr{F}_{\pi}^p(G)$ có nghĩa là dãy các tổng riêng phần $f_0+\cdots +f_n$ hội tụ về $f$ trong $\mathscr{F}_{\pi}^p(G)$. Khi đó người ta cũng nói rằng $f$ là một tổng của chuỗi này.

Ta chứng minh a). Theo prop. 6 của INT, IV, p. 128, § 3, n$^o3$, tồn tại một tập hợp S không đáng kể đối với $\nu$ trong $G/H$ sao cho chuỗi với số hạng tổng quát $\|f_n(gH)\|$ hội tụ tuyệt đối đối với $gH\notin S$. Hơn nữa, hàm $h$ bằng tổng của chuỗi này đối với $gH\notin S$ và bằng không đối với $gH\in S$ thỏa mãn $N_p(h)<+\infty$.

Tập hợp $T =\overset{-1}{\varpi}(S)$ là không đáng kể modulo H. Với mọi $g \notin T$, chuỗi có số hạng tổng quát $f_n(g)$ hội tụ tuyệt đối trong E. Định nghĩa $f(g) =\sum f_n(g)$ với $g \notin T$ và $f(g) = 0$ trong trường hợp ngược lại. Ta có $f\in$ $\mathscr{F}_{\pi}(G)$. Chú ý rằng $\|f(gH)\|\leqslant h(gH)$ với mọi $g\in G$, do đó $N_p(f)\leqslant$ $N_p(h)<+\infty$. Vậy $f\in \mathscr{F}_{\pi}^p(G)$. Tương tự, ta thu được

$$
N_p(f-\sum_{n=0}^kf_n)\leqslant \sum_{n=k+1}^{+\infty}N_p(f_n)
$$

với mọi $k\in \mathbf{N}$, do đó chuỗi $\sum f_n$ hội tụ tới $f$ trong $\mathscr{F}_{\pi}^p(G)$. Mệnh đề a) được chứng minh.

Ta chứng minh b). Dãy $(\|f_n-f\|)_{n\in\mathbf{N}}$ hội tụ tới 0 trong không gian $\mathscr{L}^p(G/H)$. Theo INT, IV, p. 131, § 4, n$^o3$, đl. 3, tồn tại một dãy con $(\|f_{n_k}-f\|)_{k\in\mathbf{N}}$ hội tụ $\nu$-hầu khắp nơi tới 0. Khi đó dãy $(f_{n_k}(g))_{k\in\mathbf{N}}$ hội tụ tới $f(g)$ với mọi $g$ nằm ngoài một tập hợp không đáng kể modulo H.

Cuối cùng, ta chứng minh c). Cho $(f_n)_{n\in\mathbf{N}}$ là một dãy Cauchy trong $\mathscr{F}_{\pi}^p(G)$. Tồn tại một dãy tăng ngặt các số nguyên $(n_k)_{k\in\mathbf{N}}$ sao cho $N_p(f_{n_{k+1}}-f_{n_k})\leqslant 2^{-k}$ với mọi $k\in \mathbf{N}$. Với mọi $k\in \mathbf{N}$, đặt $h_k$ = $f_{n_{k+1}}-f_{n_k}\in \mathscr{F}_{\pi}^p(G)$. Theo a), chuỗi có số hạng tổng quát $h_k$ hội tụ trong $\mathscr{F}_{\pi}^p(G)$; ký hiệu $h$ là tổng của nó. Với mọi $\ell \in \mathbf{N}$, ta có

$$
f_{n_0}+\sum_{k=0}^{\ell}h_k=f_{n_{\ell+1}}
$$

do đó $f_{n_0}+h$ là một giá trị cụm của dãy $(f_n)$. Nó vì thế hội tụ (TG, II, p. 14, hệ quả 2 của mệnh đề 5). Vậy không gian $\mathscr{F}_{\pi}^p(G)$ là đầy đủ; vì không gian $\mathscr{L}_{\pi}^p(G)$ là đóng trong $\mathscr{F}_{\pi}^p$(G), nó cũng đầy đủ.

#### Hệ quả {#ts-v-s2-n5-cor-1 .statement tag=03AH}

Cho $(f_n)_{n\in\mathbf{N}}$ là một dãy Cauchy trong $\mathscr{L}_{\pi}^p(G)$ và cho $f\in \mathscr{F}_{\pi}(G)$ sao cho $f_n(g)$ hội tụ tới $f(g)$ hầu khắp nơi modulo H. Khi đó $f\in \mathscr{L}_{\pi}^p(G)$ và $(f_n)_{n\in\mathbf{N}}$ hội tụ tới $f$ trong $\mathscr{L}_{\pi}^p(G)$.

Thật vậy, hàm $f$ trùng hầu khắp nơi modulo H với giới hạn của dãy $(f_n)$ trong $\mathscr{L}_{\pi}^p(G)$.

Ta ký hiệu bởi $L^p_{\pi}(G)$ không gian vectơ tôpô định chuẩn tách liên kết của không gian nửa chuẩn $\mathscr{L}_{\pi}^p(G)$; nó là một không gian Banach.

Cho $f$ là một hàm trên G với các giá trị trong E. Ký hiệu $S_f$ là tập hợp các $x\in G$ sao cho hàm $h\mapsto f(xh)$ trên H không thuộc $\mathscr{L}_E^1(H)$. Ta có $S_f\cdot h= S_f$ với mọi $h\in H$.

Cho $x\in$ G - $S_f$. Vì $\pi$ là một biểu diễn unita, hàm $h\mapsto \pi (h)^*f(xh)$ là đo được (vì là hợp thành của ánh xạ $h\mapsto (h, f(xh))$ từ H vào $H\times E$, ánh xạ này là đo được, và ánh xạ liên tục $(g, x)\mapsto \pi (g)^*x$ từ $H\times E$ vào E, xem INT, IV, p. 174, § 5, n$^o3$, Th. 1), và nó khả tích trên H.

Ta định nghĩa một hàm $f^{\pi}$ trên G bằng cách đặt

$$
f^{\pi}(x) =\int_H\pi (h)^*f(xh)d\beta (h) \tag{3}
$$

với $x\in G$ - $S_f$ và $f^{\pi}(x) = 0$ nếu $x\in S_f$.

#### Mệnh đề 4 {#ts-v-s2-prop-4 .statement tag=03AI}

Cho $f\in \mathscr{L}_E^1(G)$.

a) Tập hợp $S_f$ là không đáng kể modulo H và $f^{\pi}\in \mathscr{F}_{\pi}(G)$;

b) Cho C là một tập con compact của G. Nếu $f$ liên tục và có giá được chứa trong C, thì $S_f$ là rỗng, hàm $f^{\pi}$ thuộc $\mathscr{K}_{\pi}(G)$ và giá của nó được chứa trong $C\cdot H$.

Phần thứ nhất của a) suy ra từ INT, VII, p. 57, § 2, n$^o5$, c). Cho $w\in H$. Nếu $x\in G$ - $S_f$, thì $xw\in G$ - $S_f$ và

$$
f^{\pi}(xw) =\int_H\pi (h)^*f(xwh)d\beta (h)
$$

$$
=\int_H\pi (w^{-1}y)^*f(xy)d\beta (y) =\pi (w)f^{\pi}(x)
$$

trong khi nếu $x\in S_f$, thì $f^{\pi}(xw) = 0 =\pi (w)^*f^{\pi}(x)$. Do đó hàm $f^{\pi}$ thuộc $\mathscr{F}_{\pi}(G)$.

Giả sử bây giờ rằng $f$ liên tục và có giá được chứa trong C. Với mọi $x\in G$, ánh xạ $h\mapsto f(xh)$ khi đó thuộc $\mathscr{K}$ (H), do đó khả tích, điều này chứng minh rằng $S_f=\emptyset$.

Ta hãy chứng minh rằng $f^{\pi}$ liên tục. Cho $x\in G$. Cho U là một lân cận mở tương đối compact của $x$ trong G.

Với mọi $y\in U$, ta có

$$
\|f^{\pi}(y)-f^{\pi}(x)\|\leqslant \int_H\|f(yh)-f(xh)\|d\beta (h)
$$

$$
=\int\|f(yh)-f(xh)\|d\beta (h)
$$

$H\cap (y^{-1}C\cup x^{-1}C)$

$\leqslant \beta (H\cap U^{-1}C)$ sup$_{h\in U^{-1}C}\|f(yh)-f(xh)\|$,

và tính liên tục của $f^{\pi}$ khi đó suy ra từ tính liên tục đều của $f$ trên G.

Cuối cùng, nếu $x\in G$ thỏa mãn $f^{\pi}(x)\not = 0$, tồn tại $h\in H$ sao cho $f(xh)\not = 0$; do đó $xh$ thuộc C và $x$ thuộc $C\cdot H$. Vì $C\cdot H$ đóng trong G, ta kết luận rằng giá của $f^{\pi}$ được chứa trong $C\cdot H$.

Cho C là một tập con compact của G. Cho $u\in \mathscr{K}_+(G)$ là một hàm sao cho $u(x)>0$ với mọi $x\in C$. Cho $v$ là hàm trên G được xác định bởi

$$
v(x) =\int_Hu(xh)d\beta (h) \tag{4}
$$

với mọi $x\in G$; với ký hiệu trước đó, ta có $v=u^1$, tương ứng với biểu diễn tầm thường chiều 1 của H. Hàm $v$ liên tục và dương; nó thuộc $\mathscr{F}_1$(G), giá của nó được chứa trong Supp($u$)$\cdot H$ và ta có

(5) $x$inf$^{\in}_{C\cdot H}v(x)>0$

(INT, VII, p. 39–40, § 2, n$^o1$, mệnh đề 1 và bổ đề 1, a)).

#### Bổ đề 5 {#ts-v-s2-lem-5 .statement tag=03AJ}

Cho $f\in \mathscr{F}_{\pi}(G)$ là một hàm $\mu$-đo được bằng không bên ngoài $C\cdot H$ sao cho hàm $\|f\|$ là $\nu$-tích phân được trên $G/H$. Cho $s$ là hàm nhận giá trị trong E trên G sao cho

$v(x)^{-1}f(x)$ if $x\in C\cdot H$

$$
s(x) =
$$

0 if $x\in G$ - $C\cdot H$.

a) Hàm $s$ là $\mu$-đo được; nó thuộc $\mathscr{F}_{\pi}(G)$ và bằng không bên ngoài $C\cdot H$;

b) Hàm $us$ thuộc $\mathscr{L}^1(G)$ và $(us)^{\pi}=f$ hầu khắp nơi modulo H.

Theo định nghĩa, hàm $s$ bằng không bên ngoài $C\cdot H$; nó là $\mu$-đo được vì hàm $f$ là $\mu$-đo được và $v(x)>0$ với mọi $x\in C\cdot H$ (INT, IV, p. 193, § 5, n$^o10$, mệnh đề 16). Ta có $s\in \mathscr{F}_{\pi}(G)$ vì $v\in \mathscr{F}_1(G)$.

Hàm $f$ khả tích $\mu$ địa phương, vì $\|f\|$ là một hàm khả tích $\nu$ (INT, VII, p. 47, § 2, No.$^o3$, mệnh đề 6, c), nhận xét rằng độ đo $\nu^{\sharp}=\kappa \cdot \mu$ tương đương với $\mu)$, do đó hàm $s$ cũng như vậy theo công thức (5). Hàm $us$ đo được và bằng không bên ngoài một tập con compact của G; vì $u$ bị chặn, suy ra $us$ là $\mu$-khả tích.

Với mọi $x\in G$ - $S_{us}$, ta có

$$
(us)^{\pi}(x) =\int_H\pi (h)^*(u(xh)s(xh))d\beta (h)
$$

$$
=\int_Hu(xh)s(x)d\beta (h) =v(x)s(x)
$$

vì $s(xh) =\pi (h)s(x)$; khẳng định cuối cùng suy ra từ mệnh đề 4, a).

Khi $H =\{e\}$ và $\pi$ có chiều 1, mệnh đề sau đây không gì khác hơn INT, IV, p. 184, § 5, No.$^o6$, định lý 5.

#### Mệnh đề 5 {#ts-v-s2-prop-5 .statement tag=03AK}

Cho $p\in [1,+\infty [$. Không gian $\mathscr{L}_{\pi}^p(G)$ là không gian của các hàm $f\in \mathscr{F}_{\pi}(G)$ sao cho $f$ là $\mu$-đo được và hàm $\|f\|$ thuộc $\mathscr{L}^p(G/H)$.

Cho $f\in \mathscr{L}_{\pi}^p(G)$. Nó là giới hạn trong $\mathscr{L}_{\pi}^p(G)$ của một dãy các phần tử của $\mathscr{K}_{\pi}(G)$. Theo mệnh đề 3, b) và định lý Egoroff (INT, IV, p. 175, § 5, No.$^o4$, định lý 2), hàm $f$ do đó là $\mu$-đo được; do đó, hàm $\|f\|$ trên $G/H$ là $\nu$-đo được (INT, VII, p. 47, § 2, No.$^o3$, mệnh đề 6, b)). Vì $N_p(f)$ là hữu hạn, hàm $\|f\|$ thuộc $\mathscr{L}^p(G/H)$ (INT, IV, p. 184, § 5, No.$^o6$, định lý 5).

Ta hãy chứng minh mệnh đề đảo lại. Cho $f$ là một hàm $\mu$-đo được thuộc $\mathscr{F}_{\pi}(G)$ sao cho $\|f\| \in \mathscr{L}^p(G/H)$. Cho $\varepsilon  >0$. Ta hãy chứng minh rằng tồn tại $\widetilde{f}\in \mathscr{K}_{\pi}(G)$ sao cho

$$
N_p(f-\widetilde{f})^p=\int_{G/H}^*\|f-\widetilde{f}\|^pd\nu \leqslant \varepsilon
$$

điều này sẽ kết luận chứng minh.

Trước hết, giả sử rằng tồn tại một tập con compact C của G sao cho $f$ bằng không bên ngoài $C\cdot H$. Cho $u\in \mathscr{K}_+(G)$ là một hàm sao cho $u(x)>0$ với mọi $x\in C$ và định nghĩa $v=u^1$ như trên. Ta ký hiệu $\varphi$ là hàm đặc số của giá của $u$.

Cho $q$ là số mũ liên hợp của $p$. Nếu $p= 1$, đặt $w$ là hàm hằng trên G bằng sup$_{x\in G}u(x)$. Nếu $p >1$, định nghĩa

$$
w(x)=\left(\int_Hu(xh)^q\,d\beta(h)\right)^{1/q}
$$

với mọi $x\in G$. Trong cả hai trường hợp, hàm $w$ liên tục và dương; nó thuộc $\mathscr{K}_1(G)$ (Mệnh đề 4 áp dụng cho biểu diễn tầm thường có chiều 1 và cho hàm $u^q$), do đó nó bị chặn trên G. Đặt W = sup$_{x\in G}w(x)$.

Cho $s$ là hàm trên G có các giá trị trong E được xác định bởi Bổ đề 5 áp dụng cho $f$. Đặt $g=\varphi s$. Hàm $g$ là $\mu$-đo được, và thỏa mãn $\|g\|\leqslant \|f\|/$ inf$_{x\in C\cdot H}v(x)$. Vì $g$ triệt tiêu bên ngoài giá của $u$ và $\kappa$ liên tục, ta có $g\in \mathscr{L}_E^p(G, \kappa \cdot \mu)$. Cho $\widetilde{g}$ là một hàm trong $\mathscr{K}_E(G)$ sao cho

$$
\int^*\|g-\widetilde{g}\|^p\kappa  d\mu\leqslant \varepsilon_p
$$

$_G$ W

Ta có $us=ug$, do đó $f= (us)^{\pi}= (ug)^{\pi}$ hầu khắp nơi modulo H (Bổ đề 5, b)). Đặt $\widetilde{f}= (u\widetilde{g})^{\pi}$; ta có $\widetilde{f}\in \mathscr{K}_{\pi}(G)$ (Mệnh đề 4, b)). Với mọi $x\in G$ - $S_{ug}$, ta thu được

$$
\|(ug)^{\pi}(x)-(u\widetilde{g})^{\pi}(x)\|\leqslant \int_H^*u(xh)\|g(xh)-\widetilde{g}(xh)\|d\beta (h)
$$

do đó

$$
\|(ug)^{\pi}(x)-(u\widetilde{g})^{\pi}(x)\|^p\leqslant w(x)^p\int_H^*\|g(xh)-\widetilde{g}(xh)\|^pd\beta (h)
$$

theo bất đẳng thức Hölder trong trường hợp $p >1$. Vì $S_{ug}$ là không đáng kể modulo H, suy ra

$$
\int_{G/H}^*\|f-\widetilde{f}\|^pd\nu \leqslant W^p\int_{G/H}^*(\int_H^*\|g(xh)-\widetilde{g}(xh)\|d\beta (h))^pd\nu (xH)
$$

$$
= W^p\int_G^*\|g-\widetilde{g}\|^p\kappa  d\mu\leqslant \varepsilon
$$

theo INT, VII, p. 46, § 2, n$^o3$, Mệnh đề 5, b), áp dụng được vì $g-\widetilde{g}$ triệt tiêu bên ngoài một tập compact của G. Điều này suy ra tính chất cần thiết khi $f$ triệt tiêu bên ngoài một tập compact modulo H.

Xét bây giờ trường hợp tổng quát. Vì $\|f\| \in \mathscr{L}^p(G/H)$ theo giả thiết, tồn tại một tập compact L của $G/H$ sao cho

$$
\int^*p\varepsilon
$$

$$
\|f\|d\nu \leqslant
$$

$(G/H)-L$ 2

(xem INT, IV, p. 152, § 4, n$^o6$, th. 4). Gọi $\varphi_L$ là hàm đặc trưng của L và đặt $f_L= (\varphi_L\circ \varpi )f$. Ta có

$$
\int^*p\int^*p\varepsilon
$$

$$
\|f-f_L\|d\nu =\|f\|d\nu \leqslant
$$

$G/H(G/H)-L$ 2

Hàm $f_L$ là $\mu$-đo được và triệt tiêu bên ngoài một tập compact modulo H. Nó thuộc $\mathscr{L}_{\pi}^p$(G), do đó theo trường hợp trước, tồn tại $\widetilde{f}\in \mathscr{K}_{\pi}(G)$ sao cho $N_p(f_L-\widetilde{f})\leqslant (\frac{\varepsilon}{2})^{1/p}$, do đó

$$
\int_{G/H}^*\|f-\widetilde{f}\|^pd\nu \leqslant \varepsilon
$$

như mong muốn.

Xét trường hợp $p= 2$. Với $f_1$ và $f_2$ thuộc $\mathscr{F}_{\pi}$(G), hàm $x\mapsto  \langle f_1(x)|f_2(x)\rangle$ thuộc $\mathscr{F}_1(G)$ vì biểu diễn $\pi$ là unita, và do đó xác định qua phép chuyển qua thương một hàm trên $G/H$, hàm này được đồng nhất như trên với $\langle f_1|f_2\rangle$. Ta có bất đẳng thức major hóa $|\langle f_1|f_2\rangle |\leqslant \|f_1\|\|f_2\|$ trong $\mathscr{F}(G/H)$.

Nếu $f_1$ và $f_2$ thuộc $\mathscr{L}_{\pi}^2$(G), thì hàm $\langle f_1|f_2\rangle$ thuộc $\mathscr{L}_1^1(G)$. Đặc biệt, nó khả tích trên $G/H$. Ánh xạ

$$
(f_1, f_2)\mapsto \int_{G/H}\langle f_1|f_2\rangle d\nu
$$

là một dạng Hermit dương trên $\mathscr{L}_{\pi}^2(G)$; nửa chuẩn liên kết là nửa chuẩn $N_2$. Đặc biệt, không gian $\mathscr{L}_{\pi}^2(G)$ là một không gian tiền Hilbert và $L^2_{\pi}(G)$ là không gian Hilbert liên kết với $\mathscr{L}_{\pi}^2(G)$.

### 6. Các biểu diễn cảm sinh

Ta giữ lại các ký hiệu và quy ước của số trước liên quan đến các độ đo $\beta$ trên H và $\nu$ trên $G/H$, cũng như hàm $\kappa : G\rightarrow \mathbf{R}^*_+$.

Tồn tại một hàm liên tục $\eta$ từ $G\times G/H$ vào $\mathbf{R}_+^*$ sao cho

$$
\eta (x, yH) =\frac{\kappa(xy)}{\kappa(x)}
$$

với mọi $(x, y)\in G\times G$, và $\boldsymbol{\gamma }_{G/H}(x)\nu = (y\mapsto \eta (x^{-1}, y))\cdot \nu$ với $x\in G$ (INT, VII, p. 56, § 2, n$^o5$, đl. 2, c)).

Cho $p\in [1,+\infty [$ và cho $\pi$ là một biểu diễn unita của H trong một không gian Hilbert phức E.

#### Bổ đề 6 {#ts-v-s2-lem-6 .statement tag=03AL}

Cho $f\in \mathscr{K}_{\overline{\pi}}(G)$. Với mọi $g\in G$, hàm

$$
\widetilde{f}:x\mapsto \eta (g^{-1}, xH)^{1/p}f(g^{-1}x)
$$

từ G vào E thuộc $\mathscr{K}_{\overline{\pi}}(G)$ và thỏa mãn $N_p(\widetilde{f}) = N_p(f)$.

Ta kiểm tra không khó khăn rằng $\widetilde{f}\in \mathscr{K}_{\overline{\pi}}(G)$. Vì

$$
N_p(\widetilde{f})^p=\int_{G/H}^*\|\widetilde{f}\|^pd\nu =\int_{G/H}^*\gamma_{G/H}(g)(\|f\|^p)(y)\eta (g^{-1}, y)d\nu (y)
$$

và vì $(y\mapsto \eta (g^{-1}, y))\cdot \nu =\boldsymbol{\gamma }_{G/H}(g)\nu$, ta thu được $N_p(\widetilde{f}) = N_p(f)$.

Từ bổ đề này suy ra rằng tồn tại một biểu diễn đẳng cự liên tục $\widetilde{\pi}$ của G trong $L^p_{\overline{\pi}}(G)$ sao cho với $f\in \mathscr{K}_{\pi}(G)$ và $g\in G$, phần tử $\widetilde{\pi}(g)f$ là lớp của hàm $\widetilde{f}$ được xác định ở trên. Nếu $p= 2$, thì biểu diễn này là unita.

#### Định nghĩa 2 {#ts-v-s2-def-2 .statement tag=03AM}

Người ta nói rằng biểu diễn unita của G trong không gian $L^2_{\overline{\pi}}(G)$ được định nghĩa như vậy là biểu diễn unita của G cảm sinh bởi biểu diễn $\pi$ của H đối với $\kappa$. Nó được ký hiệu bởi Ind$^G_H(\pi , \kappa )$, hoặc đơn giản là Ind$^G_H(\pi )$.

#### Nhận xét 1 {#ts-v-s2-n6-rem-1 .statement tag=03AN}

Cho $\varrho$ là một biểu diễn unita của H trong một không gian Hilbert phức F và cho $u:\pi \rightarrow \varrho$ là một cấu xạ H. Với mọi hàm $f\in \mathscr{K}_{\overline{\pi}}$(G), gọi $v(f)$ là hàm $g\mapsto u(f(g))$ từ G vào F; nó thuộc về $\mathscr{K}_{\overline{\varrho}}(G)$ và thỏa mãn $N_p(v(f))\leqslant \|u\|N_p(f)$. Ánh xạ tuyến tính từ $\mathscr{K}_{\overline{\pi}}(G)$ vào $\mathscr{K}_{\overline{\varrho}}(G)$ gắn $v(f)$ với $f$ do đó mở rộng thành một cấu xạ H liên tục từ Ind$^G_H(\pi )$ vào Ind$^G_H(\varrho )$ được ký hiệu là Ind$^G_H(u)$. Ta có Ind$^G_H(1_{\pi}) = 1_{Ind^G_H(\pi)}$. Cho $\sigma$ là một biểu diễn unita của H và cho $v:\varrho \rightarrow \sigma$ là một cấu xạ H; ta có Ind$^G_H(v\circ u) =$ Ind$^G_H(v)\circ$ Ind$^G_H(u)$.

*Nói cách khác, phép dựng gắn Ind$^G_H(\pi )$ với $\pi$ và Ind$^G_H(u)$ với $u$ là một hàm tử từ phạm trù các biểu diễn unita của H vào phạm trù các biểu diễn unita của G (xem CAT, I, § 2, đang chuẩn bị).*

#### Nhận xét 2 {#ts-v-s2-n6-rem-2 .statement tag=03AO}

Cho $\kappa ': G\rightarrow \mathbf{R}_+^*$ sao cho

$$
\frac{\kappa'(xh)}{\kappa'(x)}=\frac{\Delta_H(h)}{\Delta_G(h)}=\frac{\kappa(xh)}{\kappa(x)}
$$

với mọi $(x, h)\in G\times H$. Gọi $\nu '$ là độ đo quasi-bất biến $(\kappa '\cdot \mu)/\beta$ trên $G/H$. Hàm $\kappa '\kappa^{-1}$ xác định, bằng cách chuyển qua các thương, một hàm liên tục $\xi : G/H\rightarrow \mathbf{R}_+^*$ sao cho $\nu '=\xi \cdot \nu$. Tự đồng cấu $\alpha$ của $\mathscr{K}_{\pi}(G)$ được xác định bởi $f\mapsto (\kappa '\kappa^{-1})^{1/p}f$ thỏa mãn

$$
\int_{G/H}^*\|f\|^pd\nu '=\int_{G/H}^*\|\alpha (f)\|^pd\nu
$$

và cho phép đồng nhất các không gian $\mathscr{L}_{\pi}^p(G, \nu ')$ và $\mathscr{L}_{\pi}^p(G, \nu )$, cũng như các không gian $L^p_{\pi}(G, \nu ')$ và $L^p_{\pi}(G, \nu )$. Hơn nữa, $\alpha$ cảm sinh một đẳng cấu đẳng cự của các biểu diễn Ind$^G_H(\pi , \kappa ')$ và Ind$^G_H(\pi , \kappa )$.

### 7. Trường hợp của một nhóm con đóng trung tâm

Trong No. này, giả thiết rằng nhóm G là đơn môđula.

Xét một nhóm con đóng Z của tâm của G, và gọi $dz$ là một độ đo Haar trên Z. Nhóm thương $G/Z$ được trang bị độ đo Haar $\nu =\mu/dz$. Cho $\chi$ là một đặc trưng unita của Z. Nhóm thương $G/Z$ là đơn môđula theo INT, VII, p. 61, § 2, n$^o7$, hệ quả của mệnh đề 11.

#### Bổ đề 7 {#ts-v-s2-lem-7 .statement tag=03AP}

Ta có

$$
N_1(\check{f}) = N_1(f),\langle f_1|f_2\rangle =\langle \check{f}_1|\check{f}_2\rangle \tag{6}
$$

với mọi $f\in \mathscr{F}_{\chi}(G)$ và mọi $f_1$ và $f_2$ trong $\mathscr{L}_{\chi}^2(G)$.

Các công thức này là những hệ quả của các định nghĩa.

Với mọi $g\in G$ và mọi $f\in \mathscr{F}_{\chi}$(G), các hàm $x\mapsto f(g^{-1}x)$ và $x\mapsto f(xg)$ thuộc về $\mathscr{F}_{\chi}(G)$. Chúng lần lượt được ký hiệu bởi $\boldsymbol{\gamma }_{G,\chi}(g)f$ và $\boldsymbol{\delta }_{G,\chi}(g)f$. Các ánh xạ $\boldsymbol{\gamma }_{G,\chi}$ và $\boldsymbol{\delta }_{G,\chi}$ là các biểu diễn tuyến tính của G trong $\mathscr{F}_{\chi}(G)$. Với mọi $z\in Z$, ta có

$$
\boldsymbol{\gamma }_{G,\chi}(gz) =\overline{\chi(z)}\boldsymbol{\gamma }_{G,\chi}(g),\boldsymbol{\delta }_{G,\chi}(gz) =\chi (z)\boldsymbol{\delta }_{G,\chi}(g) \tag{7}
$$

Cho $f\in \mathscr{F}_{\chi}(G)$ và $g\in G$; ta có

$$
|\boldsymbol{\gamma }_{G,\chi}(g)f|=\boldsymbol{\gamma }_{G/Z}(gZ)|f|,|\boldsymbol{\delta }_{G,\chi}(g)f|=\boldsymbol{\delta }_{G/Z}(gZ)|f| \tag{8}
$$

trong đó tất cả các hàm xuất hiện trong các đẳng thức này được đồng nhất với các hàm trên $G/Z$.

Không gian con $\mathscr{K}_{\chi}(G)$ của $\mathscr{F}_{\chi}(G)$ ổn định dưới $\boldsymbol{\gamma }_{G,\chi}$ và $\boldsymbol{\delta }_{G,\chi}$. Cho $p$ là một số thực $\geqslant 1$. Các công thức (8) suy ra rằng các biểu diễn $\boldsymbol{\gamma }_{G,\chi}$ và $\boldsymbol{\delta }_{G,\chi}$, hạn chế vào $\mathscr{K}_{\chi}$(G), mở rộng thành các biểu diễn tuyến tính đẳng cự liên tục của G trong $\mathscr{L}_{\chi}^p$(G), được ký hiệu bởi $\boldsymbol{\gamma }^{(p)}_{G,\chi}$ và $\boldsymbol{\delta }^{(p)}_{G,\chi}$. Bằng cách chuyển qua các thương, các biểu diễn này cũng xác định các biểu diễn đẳng cự của G trong $L^p_{\chi}$(G), được ký hiệu theo cùng cách.

Các biểu diễn $\boldsymbol{\gamma }_G$[^2]$_{,\chi}$ và $\boldsymbol{\delta }_G$[^2]$_{,\chi}$ trong $L_{\chi}^2(G)$ là unita, và sẽ được ký hiệu đơn giản là $\boldsymbol{\gamma }_{G,\chi}$ và $\boldsymbol{\delta }_{G,\chi}$, tương ứng, bất cứ khi nào không thể có sự nhầm lẫn với các biểu diễn trong $\mathscr{F}_{\chi}(G)$. Ta cũng ký hiệu bởi $\boldsymbol{\varrho }_{G,\chi}$ biểu diễn liên tục của $G\times G$ trong $\mathscr{L}_{\chi}^2(G)$ hoặc $L^2_{\chi}(G)$ được xác định bởi

$$
\boldsymbol{\varrho }_{G,\chi}(g, h) =\boldsymbol{\gamma }_{G,\chi}(g)\circ \boldsymbol{\delta }_{G,\chi}(h) =\boldsymbol{\delta }_{G,\chi}(h)\circ \boldsymbol{\gamma }_{G,\chi}(g)
$$

với mọi $(g, h)\in G\times G ($xem Bổ đề 1 của V, p. 377).

Biểu diễn $\boldsymbol{\gamma }_{G,\chi}$ trên $L^2_{\chi}(G)$ không gì khác ngoài biểu diễn cảm sinh Ind$^G_Z(\overline{\chi})$.

Khi $Z =\{e\}$, bổ đề sau là hệ quả của INT, VIII, p. 166, § 4, n$^o5$, Mệnh đề 12, vì G là đơn môđula.

#### Bổ đề 8 {#ts-v-s2-lem-8 .statement tag=03AQ}

Cho $f_1\in \mathscr{K}_{\chi}(G)$ và $f_2\in \mathscr{L}_{\chi}^2(G)$.

a) Hàm $f$ trên G được xác định bởi $f(g) =\langle f_1|\boldsymbol{\gamma }_{G,\chi}(g)f_2\rangle$ với mọi $g\in G$ thuộc về $\mathscr{L}_{\overline{\chi}}^2(G)$ và thỏa mãn $N_2(f)\leqslant N_1(f_1)N_2(f_2)$;

b) Hàm $f$ trên G được xác định bởi $f(g) =\langle f_1|\boldsymbol{\delta }_{G,\chi}(g)f_2\rangle$ với mọi $g\in G$ thuộc về $\mathscr{L}_{\chi}^2(G)$ và thỏa mãn $N_2(f)\leqslant N_1(f_1)N_2(f_2)$.

Ta chứng minh a), chứng minh của mệnh đề b) tương tự. Hàm $f$ liên tục, do đó $\mu$-đo được. Với mọi $z\in Z$ và mọi $g\in G$, ta có

$$
f(gz) =\langle f_1|\boldsymbol{\gamma }_{G,\chi}(gz)f_2\rangle =\overline{\chi(z)}\langle f_1|\boldsymbol{\gamma }_{G,\chi}(g)f_2\rangle
$$

(công thức (7), p. 417), do đó $f\in \mathscr{F}_{\overline{\chi}}(G)$. Mệnh đề 5 của V, p. 413 suy ra rằng bây giờ chỉ cần chứng minh $N_2(f)\leqslant N_1(f_1)N_2(f_2)$.

Trước hết giả sử rằng $f_2$ thuộc $\mathscr{K}_{\chi}(G)$. Với mọi $g\in G$, theo định nghĩa ta có

$$
f(g) =\int_{G/Z}\overline{f_1}\boldsymbol{\gamma }_{G,\chi}(g)f_2d\nu
$$

trong đó hàm $\overline{f_1}\boldsymbol{\gamma }_{G,\chi}(g)f_2$ được đồng nhất với một hàm trên $G/Z$.

Định nghĩa một hàm $f_3$ trên G bằng cách đặt $f_3(g) = 0$ nếu $f_1(g) = 0$ và $f_3(g) =f_1(g)|f_1(g)|^{-1/2}$ trong trường hợp ngược lại. Hàm $f_3$ thuộc $\mathscr{F}_{\chi}(G)$ và thỏa mãn $f_1=|f_1|^{1/2}f_3$; nó là $\mu$-đo được và bằng không bên ngoài một tập compact modulo Z, vì $f_1$ có tính chất đó. Vì $|f_1|^{1/2}\in \mathscr{K}_1$(G), suy ra rằng

$$
\overline{f_1}\boldsymbol{\gamma }_{G,\chi}(g)f_2=|f_1|^{1/2}\overline{f_3}\boldsymbol{\gamma }_{G,\chi}(g)f_2
$$

$$
|\overline{f_3}\boldsymbol{\gamma }_{G,\chi}(g)f_2|=|f_3| |\boldsymbol{\gamma }_{G,\chi}(g)f_2|
$$

với mọi $g\in G$.

Cho $g\in G$. Theo bất đẳng thức Cauchy-Schwarz, ta có

$$
|f(g)|^2\leqslant (\int_{G/Z}|f_1|^{1/2}|f_3| |\boldsymbol{\gamma }_{G,\chi}(g)f_2|d\nu )^2
$$

$$
\leqslant (\int_{G/Z}|f_1|d\nu )(\int_{G/Z}|f_3|^2|\boldsymbol{\gamma }_{G,\chi}(g)f_2|^2d\nu )
$$

Vì ta có $|f_3|^2=|f_1|$ trong $\mathscr{K}(G/Z)$, nên khi lấy tích phân trên $G/Z$, suy ra rằng

$$
\int_{G/Z}|f(g)|^2d\nu (g)\leqslant N_1(f_1)\int_{G/Z}(\int_{G/Z}|f_1(x)| |f_2(g^{-1}x)|^2d\nu (x))d\nu (g)
$$

Hàm trên $G/Z\times G/Z$ suy ra từ hàm

$$
(g, x)\mapsto  |f_1(x)| |f_2(g^{-1}x)|^2
$$

bằng cách chuyển qua các thương là $(\nu \otimes \nu$)-đo được và có giá compact, do đó nó là $(\nu \otimes \nu$)-điều hòa (INT, V, p. 4, § 5, No.$^o2$, Định nghĩa 2). Theo Mệnh đề 7 của INT, V, p. 93, § 8, No.$^o3$, suy ra rằng

$$
\int_{G/Z}(\int_{G/Z}|f_1(x)| |f_2(g^{-1}x)|^2d\nu (x))d\nu (g)
$$

$$
=\int_{G/Z}|f_1(x)|(\int_{G/Z}|f_2(g^{-1}x)|^2d\nu (g))d\nu (x) = N_1(f_1)N_2(f_2)^2
$$

Do đó, ta có $N_2(f)^2\leqslant N_1(f_1)^2N_2(f_2)^2$, điều này thiết lập tính chất cần chứng minh trong trường hợp này.

Xét trường hợp tổng quát. Gọi $u$ là ánh xạ tuyến tính từ $\mathscr{K}_{\chi}(G)$ vào $\mathscr{L}_{\overline{\chi}}^2(G)$ gán $f$ với $f_2$. Cho $f_2\in \mathscr{L}_{\chi}^2(G)$ và cho $(f_{2,n})_{n\in\mathbf{N}}$ là một dãy trong $\mathscr{K}_{\chi}(G)$ hội tụ tới $f_2$ trong $\mathscr{L}_{\chi}^2(G)$. Đặt $f_n=u(f_{2,n})$; dãy $(f_n)_{n\in\mathbf{N}}$ là một dãy Cauchy trong $\mathscr{L}_{\overline{\chi}}^2(G)$ vì trường hợp trước suy ra rằng $N_2(f_n-f_m)\leqslant N_1(f_1)N_2(f_{2,n}-f_{2,m})$ với mọi $n$ và $m$ trong $\mathbf{N}$. Cho $f\in \mathscr{L}_{\overline{\chi}}^2(G)$ sao cho $(f_n)$ hội tụ tới $f$ (Mệnh đề 3, c) của V, p. 409). Vì $N_2(f_n)\leqslant N_1(f_1)N_2(f_{2,n})$ với mọi $n\in \mathbf{N}$, nên suy ra rằng $N_2(f)\leqslant N_1(f_1)N_2(f_2)$.

Tồn tại một dãy con $(f_{n_k})_{k\in\mathbf{N}}$ sao cho $f_{n_k}(g)$ hội tụ tới $f(g)$ với mọi $g\in G$ nằm ngoài một tập con của G không đáng kể modulo Z (loc. cit., b)). Nhưng mặt khác, với mọi $g\in G$, ta có

$$
f_{n_k}(g) =\langle f_1|\boldsymbol{\gamma }_{G,\chi}(g)f_{2,n_k}\rangle  \rightarrow  \langle f_1|\boldsymbol{\gamma }_{G,\chi}(g)f_2\rangle
$$

Do đó, ta có $f(g) =\langle f_1|\boldsymbol{\gamma }_{G,\chi}(g)f_2\rangle$ với mọi $g$ nằm ngoài một tập con của G không đáng kể modulo Z. Vì $f\in \mathscr{L}_{\overline{\chi}}^2(G)$ và $N_2(f)\leqslant N_1(f_1)N_2(f_2)$, bổ đề được chứng minh.

### 8. Các biểu diễn khả tích bình phương

Trong số này, các không gian Hilbert được xét là phức. Giả sử rằng G là đơn môđula, và C là tâm của nó. Với mọi nhóm con đóng Z của C, gọi $\beta_Z$ là một độ đo Haar trên Z, và trang bị cho $G/Z$ độ đo Haar $\nu_Z=\mu/\beta_Z$ (INT, VII, p. 44, § 2, n$^o2$, Định nghĩa 1).

Cho $\pi$ là một biểu diễn unita bất khả quy của G trong một không gian Hilbert E, và cho $\chi \in \widehat{C}$ là đặc trưng trung tâm của nó (Định nghĩa 6 của V, p. 390). Với mọi $x$ và $y$ trong E, gọi $f_{x,y}$ là hệ số ma trận $g\mapsto  \langle x|\pi (g)y\rangle$; đây là một hàm liên tục có giá trị phức trên G.

Cho $x$ và $y$ thuộc E. Với $z\in C$ và $g\in G$, ta có

$$
f_{x,y}(zg) =\langle x|\pi (zg)y\rangle =\langle x|\chi (z)\pi (g)y\rangle =\chi (z)f_{x,y}(g) \tag{9}
$$

do đó $f_{x,y}$ thuộc không gian $\mathscr{F}_{\chi}(G) ($V, p. 408). Hơn nữa, với mọi $(g_1, h_1)\in G\times G$ và mọi $g\in G$, ta có

$$
f_{\pi(g_1)x,\pi(h_1)y}(g) =\langle \pi (g_1)x|\pi (g)\pi (h_1)y\rangle =f_{x,y}(g_1^{-1}gh_1) \tag{10}
$$

Quan hệ (9) biện minh cho định nghĩa sau.

#### Định nghĩa 3 {#ts-v-s2-def-3 .statement tag=03AR}

Cho $\pi$ là một biểu diễn unita bất khả quy của G trong một không gian Hilbert E. Ta nói rằng $\pi$ là khả tích bình phương modulo tâm nếu hàm trên $G/C$ suy ra từ hàm $|f_{x,y}|$ bằng cách chuyển qua thương thuộc $\mathscr{L}^2(G/C)$ với mọi $(x, y)\in E\times E$.

Điều kiện này không phụ thuộc vào lựa chọn một độ đo Haar trên $G/C$.

Nếu các hệ số ma trận của $\pi$ thuộc về $\mathscr{L}^2$(G), ta nói rằng $\pi$ là khả tích bình phương; sự tồn tại của một biểu diễn unita bất khả quy khả tích bình phương của G kéo theo rằng tâm của G là compact (bài tập 5 của V, p. 487).

Có những nhóm G không nhận một biểu diễn khả tích bình phương nào, ngay cả modulo tâm (xem bài tập 32 của V, p. 516).

#### Mệnh đề 6 {#ts-v-s2-prop-6 .statement tag=03AS}

Cho $\pi$ là một biểu diễn unita bất khả quy của G trong một không gian Hilbert E. Cho $\chi$ là đặc trưng trung tâm của $\pi$. Khi đó $\pi$ là khả tích bình phương modulo tâm khi và chỉ khi tồn tại các phần tử khác không $x_0$ và $y_0$ của E sao cho hàm trên $G/C$ suy ra từ $|f_{x_0,y_0}|$ bằng cách chuyển qua thương thuộc về $\mathscr{L}^2(G/C)$.

Giả sử tồn tại các phần tử khác không $x_0$ và $y_0$ của E sao cho $|f_{x_0,y_0}| \in \mathscr{L}^2(G/C)$. Chỉ cần chứng minh rằng khi đó $\pi$ là khả tích bình phương modulo tâm.

Cho F là tập hợp các phần tử $x\in E$ sao cho $|f_{x,y_0}|$ thuộc về $\mathscr{L}^2(G/C)$. Nó là một không gian con vectơ của E; nó chứa $x_0$, do đó khác không. Quan hệ (10) ở trên kéo theo rằng F ổn định dưới $\pi$; vì biểu diễn $\pi$ là bất khả quy, không gian F do đó trù mật trong E.

Cho $x\in F$. Vì $f_{x,y_0}$ thuộc về $\mathscr{F}_{\chi}(G)$ và là $\mu$-đo được, và vì $|f_{x,y_0}| \in \mathscr{L}^2(G/C)$, ta có $f_{x,y_0}\in \mathscr{L}_{\chi}^2(G)$ (Mệnh đề 5 của V, p. 413 áp dụng cho Z = C). Gọi $u$ là toán tử từng phần từ E vào $L^2_{\chi}(G)$ có miền xác định là F và gán cho $x\in F$ lớp của $f_{x,y_0}$ trong $L^2_{\chi}(G)$.

Hãy chứng minh rằng toán tử từng phần $u$ là đóng. Cho $(x_n, u(x_n))_{n\in\mathbf{N}}$ là một dãy các phần tử của đồ thị của $u$ hội tụ trong $E\times L^2_{\chi}(G)$. Cho $x$ là giới hạn của $(x_n)$ và cho $f\in \mathscr{L}_{\chi}^2(G)$ là một hàm mà lớp của nó là giới hạn của dãy $(u(x_n))$.

Hàm $u(x_n)$ là lớp của hệ số ma trận $f_{x_n,y_0}$. Với mọi $g\in G$, ta có

$$
f_{x_n,y_0}(g) =\langle x_n|\pi (g)y_0\rangle  \rightarrow  \langle x|\pi (g)y_0\rangle =f_{x,y_0}(g)
$$

khi $n\rightarrow +\infty$. Do đó $f_{x,y_0}\in \mathscr{L}_{\chi}^2(G)$ và $f=f_{x_0,y}$ hầu khắp nơi modulo C (hệ quả của Mệnh đề 3 của V, p. 409); điều này có nghĩa là $u(x)$ là lớp của $f$ trong $L^2_{\chi}(G)$. Như vậy ta đã chứng minh rằng $u$ là đóng.

Miền F của $u$ là ổn định đối với $\pi$, và quan hệ (10) chứng minh rằng $u$ thỏa mãn $u\circ \pi (g) =\boldsymbol{\gamma }_{G,\chi}(g)\circ u$ với mọi $g\in G$. Do đó người ta cũng có đẳng thức $u^*\circ \boldsymbol{\gamma }_{G,\chi}(g) =\pi (g)\circ u^*$ với mọi $g\in G$ (bổ đề 6 của V, p. 381), do đó $(u^*\circ u)\circ \pi (g) =\pi (g)\circ (u^*\circ u)$. Bây giờ toán tử từng phần $u^*\circ u$ là tự liên hợp (mệnh đề 12 của IV, p. 241), và đặc biệt là đóng (mệnh đề 7 của IV, p. 236), do đó hệ quả 1 của V, p. 387 suy ra rằng miền của $u^*\circ u$ bằng E. A fortiori, ta có F = E, nghĩa là hàm $|f_{x,y_0}|$ thuộc vào $\mathscr{L}^2(G/C)$ với mọi $x\in E$.

Cho $(x, y)\in E\times E$. Ta có $f_{x,y_0}\in \mathscr{L}_{\chi}^2(G)$. Người ta chứng minh, mutatis mutandis, bằng cách sử dụng biểu diễn $\boldsymbol{\delta }_{G,\chi}$ thay cho $\boldsymbol{\gamma }_{G,\chi}$, rằng tập hợp các $y\in E$ sao cho hàm $|f_{x,y}|$ thuộc vào $\mathscr{L}^2(G/C)$ bằng E. Mệnh đề được suy ra.

Trong phần còn lại của No. này, ta cố định một nhóm con đóng Z của C sao cho $C/Z$ là compact.

#### Bổ đề 9 {#ts-v-s2-lem-9 .statement tag=03AT}

Cho $\pi$ là một biểu diễn đơn vị bất khả quy của G trong một không gian Hilbert E là khả tích bình phương modulo tâm. Cho $\chi$ là hạn chế vào Z của đặc trưng trung tâm của $\pi$. Với mọi $x$ và $y$ trong E, ta có $f_{x,y}\in \mathscr{L}_{\chi}^2(G)$.

Hàm $f_{x,y}$ là liên tục, do đó $\mu$-đo được. Ta có $f_{x,y}\in \mathscr{F}_{\chi}(G)$ theo công thức (9), p. 420. Hơn nữa, theo INT, VII, p. 64, § 2, No.$^o8$, hệ quả 1, c), ta có $N_2(f_{x,y})<+\infty$ vì $C/Z$ là compact và $|f_{x,y}| \in \mathscr{L}^2(G/C)$. Mệnh đề do đó được suy ra từ mệnh đề 5 của V, p. 413.

#### Mệnh đề 7 {#ts-v-s2-prop-7 .statement tag=03AU}

Cho $\pi$ là một biểu diễn đơn vị bất khả quy của G trong một không gian Hilbert E là khả tích bình phương modulo tâm. Cho $\chi$ là hạn chế vào Z của đặc trưng trung tâm của $\pi$.

Tồn tại một số thực $c >0$ và một cấu xạ đẳng cự duy nhất $(G\times G)$-morphism $w$ của biểu diễn đơn vị $\overline{\pi}\boxtimes \pi$ vào $L^2_{\chi}(G)$ sao cho, với mọi $(x, y)\in \overline{E}\times E$, phần tử $w(x\otimes y)$ là lớp trong $L^2_{\chi}(G)$ của hàm $c^{1/2}f_{x,y}$.

Với mọi $(x, y)\in E\times E$, ta có $f_{x,y}\in \mathscr{L}_{\chi}^2(G)$ (bổ đề 9). Gọi $v$ là ánh xạ tuyến tính duy nhất từ $\overline{E}\otimes E$ vào $L^2_{\chi}(G)$ sao cho $v(x\otimes y)$ là lớp của $f_{x,y}$ với mọi $(x, y)\in E\times E$.

Ta sẽ chứng minh dưới đây bổ đề sau.

#### Bổ đề 10 {#ts-v-s2-lem-10 .statement tag=03AV}

Tồn tại một số thực $c >0$ sao cho ánh xạ tuyến tính $w=c^{1/2}v$ là đẳng cự.

Giả sử bổ đề này đúng, ta nhận xét rằng công thức (10), p. 420, có thể được viết

$$
v(\overline{\pi}(g_1)x\otimes \pi (h_1)y) =\boldsymbol{\varrho }_{G,\chi}(g_1, h_1)v(x\otimes y) \tag{11}
$$

với mọi $(g_1, h_1)\in G\times G$ và mọi $(x, y)\in \overline{E}\times E$. Ánh xạ tuyến tính đẳng cự $w$ của $\overline{E}\otimes E$ vào $L^2_{\chi}(G)$ thừa nhận một mở rộng liên tục, vẫn ký hiệu là $w$, tới $E\widehat{\otimes}_2E$. Theo tính liên tục và tính tuyến tính, công thức (11) suy ra rằng $w$ là một $(G\times$ G)-cấu xạ của $\overline{\pi}\boxtimes \pi$ vào $L^2_{\chi}$(G), điều này kết thúc chứng minh của mệnh đề.

Ta chứng minh bổ đề. Với mọi $x\in E$, ký hiệu $u_x$ là ánh xạ tuyến tính $y\mapsto v(x\otimes y) =f_{x,y}$ của E vào $L^2_{\chi}(G)$. Ta có $u_x\in$ Hom$_G(\pi ,\boldsymbol{\gamma }_{G,\chi})$ (công thức (10)). Theo hệ quả 5 của V, p. 388, tồn tại một số thực $\lambda_x\geqslant 0$ sao cho $\lambda_xu_x$ là đẳng cự.

Cho $x$ và $y$ thuộc E. Ta có

$$
\|f_{x,y}\|^2=\int_{G/Z}\overline{f}_{x,y}f_{x,y}d\nu_Z=\int_{G/Z}\overline{\check{f}}_{x,y}\check{f}_{x,y}d\nu_Z
$$

vì $G/Z$ là đơn môđula (bổ đề 7 của V, p. 417). Nhận xét rằng $\check{f}_{x,y}=f_{y,x}$, ta thu được

$$
\lambda_x\|y\|^2=\|f_{x,y}\|^2=\int_{G/Z}f_{y,x}\overline{f}_{y,x}d\nu_Z=\|f_{y,x}\|^2=\lambda_y\|x\|^2
$$

Điều này có nghĩa là số thực dương $\lambda_x/\|x\|^2$ độc lập với lựa chọn phần tử khác không $x$ của E. Nó dương ngặt vì, với mọi $x$ khác không, hàm $f_{x,x}$ liên tục và nhận giá trị $\|x\|^2>0$ tại $e$, do đó $\|u_x(x)\|=\|f_{x,x}\|>0$. Ta ký hiệu số thực này bởi $c^{-1}$.

Với mọi $(x, y)\in E\times E$, suy ra rằng

$$
\|v(x\otimes y)\|^2=\|f_{x,y}\|^2=\lambda_x\|y\|^2=c^{-1}\|x\|^2\|y\|^2=c^{-1}\|x\otimes y\|^2
$$

Dùng EVT, V, p. 29, hệ quả 1, ta suy ra rằng ánh xạ tuyến tính $w=c^{1/2}v$ của $\overline{E}\widehat{\otimes}_2E$ vào $L^2_{\chi}(G)$ là đẳng cự, như yêu cầu.

#### Hệ quả {#ts-v-s2-n8-cor-1 .statement tag=03AW}

Cho $\pi$ là một biểu diễn unita bất khả quy của G và cho $\chi$ là hạn chế vào Z của đặc trưng trung tâm của nó. Biểu diễn $\pi$ là khả tích bình phương modulo tâm khi và chỉ khi nó đẳng cấu với một biểu diễn con của biểu diễn $\boldsymbol{\gamma }_{G,\chi}$ của G trong $L^2_{\overline{\chi}}(G)$ (tương ứng của biểu diễn $\boldsymbol{\delta }_{G,\chi}$ của G trong $L^2_{\chi}(G)$).

Ta chứng minh mệnh đề liên quan đến $\boldsymbol{\gamma }_{G,\chi}$, trường hợp thứ hai được chứng minh theo cách tương tự.

Giả sử trước hết rằng tồn tại một biểu diễn con E của biểu diễn $\boldsymbol{\gamma }_{G,\chi}$ đẳng cấu với $\pi$. Vì không gian E là khác không, tồn tại một hàm $f_1\in \mathscr{K}_{\overline{\chi}}(G)$ mà lớp $\widetilde{f}_1$ không trực giao với E. Ta có $f_1\in \mathscr{L}_{\overline{\chi}}^1(G)$. Gọi $\widetilde{f}_{1,E}$ là phép chiếu trực giao của $\widetilde{f}_1$ lên E; đó là một phần tử khác không của E. Hơn nữa, cho $\widetilde{f}_2\in E$ là khác không. Ánh xạ $h:g\mapsto  \langle \widetilde{f}_{1,E}|\boldsymbol{\gamma }_{G,\chi}(g)\widetilde{f}_2\rangle$ là một hệ số ma trận của $\pi$. Với mọi $g\in G$, ta có $h(g) =\langle \widetilde{f}_1|\boldsymbol{\gamma }_{G\overline{,\chi}}(g)\widetilde{f}_2\rangle$ vì $\widetilde{f}_1-\widetilde{f}_{1,E}$ trực giao với E. Theo Bổ đề 8 của V, p. 418, hàm $h$ thuộc về $\mathscr{L}_{\chi}^2$(G), do đó Mệnh đề 6 suy ra rằng $\pi$ là khả tích bình phương modulo tâm.

Ngược lại, giả sử rằng $\pi$ là khả tích bình phương modulo tâm. Cho $x_0\in E$ là một vectơ khác không. Theo Mệnh đề 7 và công thức (10), ánh xạ $y\mapsto \check{f}_{x_0,y}$ là một cấu xạ G đơn ánh từ $\pi$ vào $\boldsymbol{\gamma }_{G,\chi}$.

#### Định nghĩa 4 {#ts-v-s2-def-4 .statement tag=03AX}

Cho Z là một nhóm con đóng của C sao cho $C/Z$ là compact. Cho $\pi$ là một biểu diễn unita bất khả quy của G là khả tích bình phương modulo tâm. Số thực duy nhất $c >0$ thỏa mãn tính chất của Mệnh đề 7 được gọi là bậc hình thức của $\pi$ đối với Z. Nó được ký hiệu bởi $c_Z(\pi )$.

Bậc hình thức phụ thuộc vào lựa chọn độ đo Haar trên Z. Nếu độ đo Haar $\beta_Z$ trên Z được nhân với một số thực $t >0$, thì độ đo $\nu_Z=\mu/\beta_Z$ trên $G/Z$ được nhân với $t^{-1}$, và bậc hình thức của $\pi$ được nhân với $t$.

Bậc hình thức được đặc trưng bởi tính chất sau:

#### Mệnh đề 8 (Các quan hệ trực giao) {#ts-v-s2-prop-8 .statement tag=03AY}

Cho $\pi$ là một biểu diễn unita bất khả quy của G trong một không gian Hilbert E là khả tích bình phương modulo tâm. Ta có

$$
c_Z(\pi )\int_{G/Z}\langle x|\pi (g)x'\rangle  \langle y|\pi (g)y'\rangle d\nu_Z(g) =\langle x|y\rangle \langle x'|y'\rangle
$$

với mọi $(x, y, x', y')\in E^4$.

Gọi $w$ là cấu xạ của Mệnh đề 7. Ta có

$$
\int_{G/Z}\langle x|\pi (g)x'\rangle  \langle y|\pi (g)y'\rangle d\nu_Z(g) =\langle f_{x,x'}|f_{y,y'}\rangle
$$

và theo loc. cit., suy ra rằng

$$
\langle f_{x,x'}|f_{y,y'}\rangle =\frac{1}{c_Z(\pi)}\langle w(x\otimes x')|w(y\otimes y')\rangle
$$

$$
=\frac{1}{c_Z(\pi)}\langle x\otimes x'|y\otimes y'\rangle =\frac{1}{c_Z(\pi)}\langle x|y\rangle_{\overline{E}}\langle x'|y'\rangle_E
$$

do đó có kết quả.

Bổ sung cho mệnh đề trước, ta cũng có các hệ thức sau đây đối với các biểu diễn bất khả quy khả tích bình phương không đẳng cấu.

#### Mệnh đề 9 {#ts-v-s2-prop-9 .statement tag=03AZ}

Cho $\pi_1$ và $\pi_2$ là các biểu diễn unita bất khả quy không đẳng cấu của G trong các không gian Hilbert $E_1$ và $E_2$. Giả sử rằng $\pi_1$ và $\pi_2$ là khả tích bình phương modulo tâm và rằng các hạn chế lên Z của các ký tự trung tâm của chúng trùng nhau. Khi đó

$$
\int_{G/Z}\langle x|\pi_1(g)x'\rangle  \langle y|\pi_2(g)y'\rangle d\nu_Z(g) = 0
$$

với mọi $(x, x', y, y')\in E^2_1\times E^2_2$.

Với $i= 1, 2$, gọi $w_i$ là cấu xạ của Mệnh đề 7 đối với biểu diễn $\pi_i$. Theo Bổ đề 8, b) của V, p. 384 và mệnh đề b) của Mệnh đề 8 của V, p. 394, ảnh của $w_i$ được chứa trong thành phần đẳng kiểu $\pi_i$ của $\boldsymbol{\delta }_{G,\chi}$. Theo mệnh đề a) của loc. cit., ảnh của $w_1$ do đó trực giao với ảnh của $w_2$. Do đó, ta có $\langle w_1(x\otimes x')|w_2(y\otimes y')\rangle = 0$ với mọi $(x, x', y, y')\in E^2_1\times E^2_2$, đó là công thức cần tìm.

#### Nhận xét {#ts-v-s2-n8-rem-1 .statement tag=03B0}

Các quan hệ trực giao của các Mệnh đề 8 và 9 tổng quát hóa các quan hệ của A, VIII, p. 399 (xem thêm trường hợp G compact trong § 2 của V, p. 457).

### 9. Các biểu diễn con của biểu diễn chính quy của một nhóm giao hoán

Trong số này, G là một nhóm giao hoán compact địa phương và $\mu$ là một độ đo Haar trên G. Ta ký hiệu bởi $\widehat{G}$ nhóm đối ngẫu của G (Định nghĩa 2 của II, p. 201) và bởi $\widehat{\mu}$ độ đo Haar đối ngẫu của $\mu$ trên $\widehat{G}$ (Định nghĩa 4 của II, p. 214). Các khái niệm về đo được sẽ luôn được hiểu tương đối với $\mu$ và $\widehat{\mu}$.

Ta đề xuất xác định tất cả các biểu diễn con của biểu diễn chính quy trái $\boldsymbol{\gamma }_G$ của G trong $L^2(G, \mu)$. Vì G là giao hoán, hơn nữa ta có $\boldsymbol{\delta }_G(g) =\boldsymbol{\gamma }_G(g^{-1})$, do đó các biểu diễn con này cũng là các biểu diễn con của biểu diễn chính quy phải.

Với mọi tập con đo được M của $\widehat{G}$, ta ký hiệu bởi $E_M$ tập hợp các $f\in L^2(G, \mu)$ sao cho biến đổi Fourier $\mathscr{F}_G(f)$ bằng không hầu khắp nơi trên M (xem No.$^o3$ của II, p. 210). Nó là hạt nhân của ánh xạ tuyến tính liên tục $f\mapsto \varphi_M\mathscr{F}_G(f)$ từ $L^2(G, \mu)$ vào $L^2(\widehat{G},\widehat{\mu})$, trong đó $\varphi_M$ ký hiệu hàm đặc trưng của M (xem Định lý 1 của II, p. 215), và do đó là một không gian con đóng của $L^2(G, \mu)$.

Ta nói rằng các tập con đo được M và N của $\widehat{G}$ bằng nhau sai khác một tập địa phương không đáng kể nếu $(M\cup N)$- $(M\cap N)$ là địa phương không đáng kể. Tương đương, các tập con đo được M và N bằng nhau sai khác một tập địa phương không đáng kể khi và chỉ khi các hàm đặc trưng của M và N bằng nhau trong $L^{\infty}(\widehat{G},\widehat{\mu})$.

#### Mệnh đề 10 {#ts-v-s2-prop-10 .statement tag=03B1}

a) Cho M là một tập con đo được của $\widehat{G}$. Không gian $E_M$ là một biểu diễn con của biểu diễn $\boldsymbol{\gamma }_G$;

b) Cho M và N là các tập con đo được của $\widehat{G}$. Ta có $E_M= E_N$ khi và chỉ khi M và N bằng nhau sai khác một tập địa phương không đáng kể;

c) Mọi biểu diễn con của $\boldsymbol{\gamma }_G$ đều có dạng $E_M$ với M là một tập con đo được của $\widehat{G}$.

Cho $\eta$ là ánh xạ chính tắc của G vào $\widehat{\widehat{G}} ($xem II, p. 216, Nhận xét 1). Vì $E_M$ là đóng, mệnh đề a) suy ra từ các công thức

$$
\boldsymbol{\gamma }_G(x)(f) =\varepsilon_x*f,\mathscr{F}_G(\varepsilon_x*f) =\eta (x)\mathscr{F}_G(f)
$$

với $x\in G$ và $f\in L^2(G, \mu)$.

Cho M và N là các tập con đo được bằng nhau sai khác một tập địa phương không đáng kể. Vì $\varphi_M$ khi đó bằng $\varphi_N$ trong $L^{\infty}(\widehat{G},\widehat{\mu})$, điều kiện này suy ra rằng $E_M= E_N$.

Ngược lại, giả sử rằng M và N không bằng nhau sai khác một tập địa phương không đáng kể. Có thể đổi chỗ vai trò của M và N, khi đó tồn tại một tập con compact K sao cho tập $L = K\cap (M$ - $(M\cap N))$ là không đáng kể. Gọi $\varphi_L\in L^2(\widehat{G},\widehat{\mu})$ là lớp của hàm đặc trưng của L, và đặt $f=\overline{\mathscr{F}}_{\widehat{G}}(\varphi_L)\in L^2(G, \mu)$; ta có $\mathscr{F}_G(f) =\varphi_L$ (Hệ quả của Định lý 2 của II, p. 220). Khi đó $f$ thuộc $E_N$, vì $L\cap N$ là rỗng, nhưng không thuộc $E_M$, vì $\varphi_M\mathscr{F}(f) =\varphi_M\varphi_L=\varphi_L$. Do đó $E_M\not = E_N$, điều này chứng minh b).

Bây giờ cho E là một biểu diễn con của $\boldsymbol{\gamma }_G$. Cho $p_E$ là phép chiếu trực giao của $L^2(G, \mu)$ có ảnh là E và cho $q_E=\mathscr{F}_G\circ p_E\circ \mathscr{F}_G^{-1}$. Phép chiếu $p_E$ thuộc Hom$_G(\boldsymbol{\gamma }_G,\boldsymbol{\gamma }_G)$ (mệnh đề 4 của V, p. 383), do đó nó giao hoán với $\boldsymbol{\gamma }_G(f)$ với mọi $f\in L^1(G, \mu) ($cf. V, p. 401). Điều này có nghĩa là nó giao hoán với các tự đồng cấu $\varphi \mapsto f*\varphi$ với $f\in L^1(G, \mu)$ (bổ đề 4 của V, p. 407). Do đó, tự đồng cấu $q_E$ của $L^2(\widehat{G},\widehat{\mu})$ giao hoán với tự đồng cấu phép nhân bởi g với mọi hàm $g\in \mathscr{C}_0(\widehat{G})$ thuộc ảnh của biến đổi Fourier của $L^1(G, \mu)$ trong $\mathscr{C}_0(\widehat{G})$ (mệnh đề 14 của II, p. 223). Vì ảnh của biến đổi Fourier là trù mật trong $\mathscr{C}_0(\widehat{G})$ (hệ quả của mệnh đề 5 của II, p. 209), tính liên tục của cấu xạ $g\mapsto m_g$ suy ra rằng $q_E$ giao hoán với $m_g$ với mọi hàm $g\in \mathscr{C}_0(\widehat{G})$.

Theo hệ quả của mệnh đề 7 của IV, p. 188, do đó tồn tại một hàm $\varphi \in \mathscr{L}^{\infty}(\widehat{G},\widehat{\mu})$ sao cho $q_E=m_{\varphi}$. Vì $q_E=q^2_E$, ta có $m_{\varphi}=m^2_{\varphi}=m_{\varphi^2}$, do đó $\varphi =\varphi^2$ trong $L^{\infty}(\widehat{G},\widehat{\mu})$ (mệnh đề 5 của IV, p. 186); điều này có nghĩa là $\varphi$ bằng trong $L^{\infty}(\widehat{G},\widehat{\mu})$ với lớp của hàm đặc trưng của một tập con đo được N của $\widehat{G}$. Đặt $M =\widehat{G}-$ N. Cho $f\in L^2(G, \mu)$. Ta có $f\in E$ khi và chỉ khi $p_E(f) =f$, khi và chỉ khi $\varphi \mathscr{F}_G(f) =\mathscr{F}_G(f)$, điều này tương đương với $f\in E_M$.

#### Nhận xét {#ts-v-s2-n9-rem-1 .statement tag=03B2}

Cho $\chi$ là một đặc trưng của G. Nếu G không compact, thành phần $\chi$-đẳng kiểu của biểu diễn chính quy của G trong $L^2(G)$ là tầm thường. Nếu G compact, thành phần $\chi$-đẳng kiểu của biểu diễn chính quy của G có chiều 1 và hàm $\chi \in L^2(G)$ là một cơ sở của nó.

### 10. Các biểu diễn unita của nhóm R

Trong số này, E chỉ một không gian Hilbert phức. Nhóm $\mathbf{R}$ được trang bị độ đo Lebesgue.

#### Bổ đề 11 {#ts-v-s2-lem-11 .statement tag=03B3}

Cho $u$ là một toán tử từng phần tự liên hợp trên E. Với $t\in \mathbf{R}$, đặt $\varrho (t) =e^{itu}\in \mathscr{L}(E)$. Khi đó ánh xạ $\varrho$ là một biểu diễn unita của $\mathbf{R}$.

Toán tử $\varrho (t)$ được xác định bởi phép tính phiếm hàm đo được phổ quát (định nghĩa 5 của IV, p. 272); nó là một tự đồng cấu của E vì hàm $x\mapsto e^{itx}$ bị chặn trên Sp($u$) (mệnh đề 5, a) của IV, p. 275).

Theo Mệnh đề 5 của IV, p. 275, ta có $\varrho (0) = 1_E,\varrho (t)^*=\varrho (-t)$ với mọi $t\in \mathbf{R}$ và $\varrho (t_1+t_2) =\varrho (t_1)\varrho (t_2)$ với mọi $t_1$ và $t_2$ trong $\mathbf{R}$. Đặc biệt, tự đồng cấu $\varrho (t)$ là unita với mọi $t\in \mathbf{R}$. Với mọi $x\in E$, ánh xạ từ $\mathbf{R}$ vào E xác định bởi $x\mapsto \varrho (t)x$ là liên tục tại $t= 0$ theo Mệnh đề 6 của IV, p. 276, do đó $\varrho$ là một biểu diễn unita của $\mathbf{R}$ trong E (V, p. 380, Bổ đề 4).

#### Bổ đề 12 {#ts-v-s2-lem-12 .statement tag=03B4}

Cho $\varrho$ là một biểu diễn unita của $\mathbf{R}$ trong E. Gọi D là tập hợp các phần tử $x$ của E sao cho ánh xạ $\psi_x:t\mapsto \varrho (t)x$ khả vi tại 0. Ánh xạ $u$ từ D vào E cho bởi $x\mapsto i^{-1}\psi '_x(0)$ xác định một toán tử bộ phận đối xứng trên E.

Cho $f\in \mathscr{D}(\mathbf{R})$ và $x\in E$. Đặt $y=\varrho (f)x$. Với mọi $h\in \mathbf{R}$, ta có

$$
\psi_y(h) =\varrho (h)\varrho (f)x=\varrho (f)\varrho (h)x
$$

$$
=\int_{\mathbf{R}}f(t)\varrho (t+h)x dt=\int_{\mathbf{R}}f(t-h)\psi_x(t)dt
$$

Hàm từ $\mathbf{R}^2$ vào $\mathbf{C}$ xác định bởi $(t, h)\mapsto f(t-h)$ là khả vi vô hạn; đạo hàm của nó theo $h$ là hàm được xác định bởi $(t, h)\mapsto$ $-f'(t-h)$, bị chặn bởi $\|f'\|_{\infty}$. Khi $h= 0$, đạo hàm này bằng không với $t$ nằm ngoài một tập compact. Vì $\|\psi_x(t)\|=\|x\|$ với mọi $t$, ta suy ra từ Mệnh đề 2 của IV, p. 197 rằng hàm $\psi_y$ khả vi tại 0 và đạo hàm của nó được cho bởi

$$
\psi '_y(0) =-\int_{\mathbf{R}}f'(t)\psi_x(t)dt=-\varrho (f')x
$$

Do đó $y\in D$. Vì không gian $\mathscr{D}(\mathbf{R})$ trù mật trong $L^1(\mathbf{R})$ (Mệnh đề 4 của IV, p. 202), ta suy ra từ INT, VIII, p. 139, § 2, n$^o7$, Mệnh đề 10 rằng không gian D trù mật trong E.

Cho $x_1$ và $x_2$ thuộc D. Ta tính

$$
i
$$

$\langle u(x_1)|x_2\rangle =$ lim $\langle (\varrho (h)-1_E)x_1|x_2\rangle$

$$
_{h\rightarrow 0}h
$$

$$
i
$$

= lim $\langle x_1|(\varrho (-h)-1_E)x_2\rangle =\langle x_1|u(x_2)\rangle$.

$$
_{h\rightarrow 0}h
$$

Do đó, toán tử bộ phận $u$ là đối xứng.

#### Định nghĩa 5 {#ts-v-s2-def-5 .statement tag=03B5}

Cho $\varrho$ là một biểu diễn unita của $\mathbf{R}$ trong E. Toán tử bộ phận đối xứng được xác định trong Bổ đề 12 được gọi là phần tử sinh vi phân của $\varrho$.

#### Định lý 1 (Stone) {#ts-v-s2-thm-1 .statement tag=03B6}

Ánh xạ $\sigma$ gán cho một biểu diễn unita $\varrho$ của $\mathbf{R}$ trong E phần tử sinh vô cùng bé $u$ của nó xác định một song ánh từ tập hợp các biểu diễn unita của $\mathbf{R}$ trong E lên tập hợp các toán tử bộ phận tự liên hợp trên E. Song ánh ngược $\tau$ gán cho một toán tử bộ phận tự liên hợp biểu diễn unita $t\mapsto e^{itu}$.

Trước hết ta hãy chứng minh một số bổ đề.

#### Bổ đề 13 {#ts-v-s2-lem-13 .statement tag=03B7}

Cho $\varrho$ là một biểu diễn unita của $\mathbf{R}$ trong E và cho $u$ là phần tử sinh vô cùng bé của nó.

a) Miền của $u$ là tập hợp các $x\in E$ sao cho ánh xạ $\psi_x:t\mapsto \varrho (t)x$ khả vi trên $\mathbf{R}$;

b) Với mọi $t\in \mathbf{R}$ và mọi $x\in$ dom($u$), ta có $\varrho (t)x\in$ dom($u$) và $\psi '_x(t) =iu(\varrho (t)x)$;

c) Toán tử bộ phận $u$ là tự liên hợp thiết yếu.

Với mọi $x\in E$, ta ký hiệu $\psi_x$ là ánh xạ từ $\mathbf{R}$ vào E được xác định bởi $\psi_x(t) =\varrho (t)x$. Với mọi $t\in \mathbf{R}$ và mọi $h\in \mathbf{R}$, ta có

$$
\psi_x(t+h)-\psi_x(t) =\varrho (t)(\psi_x(h)-\psi_x(0))
$$

điều này chứng minh rằng dom($u$) là không gian các phần tử $x\in E$ sao cho $\psi_x$ khả vi trên $\mathbf{R}$ và thiết lập rằng $\psi '_x(t) =\varrho (t)\psi '_x(0) =i\varrho (t)(u(x))$ với mọi $t\in \mathbf{R}$.

Cho $x\in$ E và $t\in \mathbf{R}$. Ta có $\psi_{\varrho(t)x}(s) =\psi_x(s+t)$ với mọi $s\in \mathbf{R}$. Do đó, ta có $\varrho (t)x\in$ dom($u$) nếu $x\in$ dom($u$), và hơn nữa $u(\varrho (t)x) =i^{-1}\psi '_x(t) =\varrho (t)u(x)$ theo a). Khi đó thu được mệnh đề b).

Ta hãy chứng minh c). Cho $x\in$ Ker($u^*-i1_E$). Ta hãy chứng minh rằng $x= 0$. Cho $y\in$ dom($u$), và cho $f$ là hàm trên $\mathbf{R}$ được xác định bởi $f(t) =\langle \psi_y(t)|x\rangle$ với $t\in \mathbf{R}$. Hàm $f$ bị chặn vì $\|\psi_y(t)\|=\|y\|$ với mọi $t\in \mathbf{R}$; nó khả vi trên $\mathbf{R}$ và, với mọi $t\in \mathbf{R}$, mệnh đề b) suy ra

$$
f'(t) =\langle \psi '_y(t)|x\rangle =\langle iu(\varrho (t)y)|x\rangle
$$

$$
=-i\langle \varrho (t)y|u^*(x)\rangle =-i\langle \psi_y(t)|ix\rangle =f(t)
$$

vì $u^*(x) =ix$. Do đó $f(t) =f(0)e^t$ với mọi $t\in \mathbf{R}$ (FVR, IV, p. 27). Vì $f$ bị chặn, hàm $f$ bằng không và, đặc biệt, ta có $\langle y|x\rangle =f(0) = 0$. Vì không gian dom($u$) là trù mật trong E, ta kết luận rằng $x= 0$. Tương tự, người ta chứng minh rằng Ker($u^*+i1_E$) được thu gọn về 0. Theo Hệ quả 3 của IV, p. 261, toán tử từng phần $u$ do đó là tự liên hợp thiết yếu.

#### Bổ đề 14 {#ts-v-s2-lem-14 .statement tag=03B8}

Cho $u$ là một toán tử từng phần tự liên hợp trên E và cho $\varrho (t) =e^{itu}$ là biểu diễn unita của $\mathbf{R}$ được xác định bởi $u$. Phần tử sinh vô cùng bé của $\varrho$ bằng $u$.

Cho $x\in$ dom($u$). Đặt $\psi_x(t) =\varrho (t)x$ với mọi $t\in \mathbf{R}$. Với mọi số thực khác không $h$, ta có

$$
\frac{1}{h}(\psi_x(t+h)-\psi_x(t)) =(\frac{1}{h}(e^{ihu}-1_E))e^{itu}x=(\frac{1}{h}(e^{ihu}-1_E))\varrho (t)x
$$

Khi $h$ tiến tới 0, ta có

1 $_{iht}$

$$
(e-1)\rightarrow it
$$

$$
h
$$

với mọi $t\in \mathbf{R}$. Hơn nữa,

$$
|\frac{1}{h}(e^{iht}-1)|=|t||\frac{1}{h}\int_0^he^{its}ds|\leqslant |t|
$$

Từ đó suy ra theo Mệnh đề 6 của IV, p. 276 rằng hàm $\psi_x$ khả vi trên $\mathbf{R}$ và thỏa mãn $\psi '_x(t) =iu(\varrho (t)x)$ với mọi $t\in \mathbf{R}$. Do đó, miền của $u$ được chứa trong tập hợp các $x\in E$ sao cho $\psi_x$ khả vi tại 0 và khi đó có $\psi '_x(0) =iu(x)$. Điều này có nghĩa theo định nghĩa rằng phần tử sinh vô cùng bé của $\varrho$ là một mở rộng của $u$. Hai toán tử này do đó bằng nhau vì chúng đối xứng và $u$ là tự liên hợp (IV, p. 238, Nhận xét 5).

#### Bổ đề 15 {#ts-v-s2-lem-15 .statement tag=03B9}

Cho $\varrho$ là một biểu diễn unita của $\mathbf{R}$ trong E. Khi đó phần tử sinh vô cùng bé $u$ của $\varrho$ là tự liên hợp và $\varrho (t) =e^{itu}$ với mọi $t\in \mathbf{R}$.

Theo Bổ đề 13, c), toán tử từng phần $u$ là tự liên hợp thiết yếu. Bao đóng của nó $\overline{u}$ do đó là một toán tử tự liên hợp. Gọi $\pi$ là biểu diễn unita của $\mathbf{R}$ được xác định bởi $\pi (t) =e^{itu}$ (Bổ đề 11).

Với mọi $x\in E$, gọi $\psi_x$ (tương ứng $\widetilde{\psi}_x$) là ánh xạ từ $\mathbf{R}$ vào E được xác định bởi $\psi_x(t) =\varrho (t)x$ (tương ứng bởi $\widetilde{\psi}_x(t) =\pi (t)x$).

Theo bổ đề 13, a) và b), không gian dom($u$) là không gian con của E gồm các phần tử $x\in E$ sao cho ánh xạ $\psi_x$ khả vi trên $\mathbf{R}$, và với mọi $x\in$ dom($u$) và mọi $t\in \mathbf{R}$, ta có $\psi '_x(t) =iu(\psi_x(t))$. Tương tự, không gian dom($\overline{u}$) là không gian con của E gồm các phần tử $x\in E$ sao cho ánh xạ $\widetilde{\psi}_x$ khả vi trên $\mathbf{R}$, và với mọi $x\in$ dom($\overline{u}$) và mọi $t\in \mathbf{R}$, ta có $\widetilde{\psi}'_x(t) =iu(\widetilde{\psi}_x(t))$.

Cho $x\in$ dom($u$)$\subset$ dom($\overline{u}$). Đặt $f=\psi_x-\widetilde{\psi}_x$. Đây là một hàm khả vi từ $\mathbf{R}$ vào E. Với mọi $t\in \mathbf{R}$, ta có

$$
f'(t) =iu(\psi_x(t))-iu(\widetilde{\psi}_x(t)) =iu(f(t))
$$

vì $\psi_x(t)\in$ dom($u$) và $u\subset \overline{u}$. Đặt $g=\|f\|^2$; đây là một ánh xạ khả vi từ $\mathbf{R}$ vào $\mathbf{R}$ sao cho $g(0) = 0$. Với $t\in \mathbf{R}$, từ FVR, I, p. 28, Prop. 2, ta thu được

$$
g'(t) =\langle f'(t)|f(t)\rangle +\langle f(t)|f'(t)\rangle
$$

$$
=\langle iu(f(t))|f(t)\rangle +\langle f(t)|iu(f(t))\rangle = 0
$$

vì $\overline{u}$ là tự liên hợp. Do đó $f= 0$, do đó $\varrho (t)x=\pi (t)x$ với mọi $t\in \mathbf{R}$. Các tự đồng cấu liên tục $\varrho (t)$ và $\pi (t)$ của E trùng nhau trên dom($u$), và do đó bằng nhau với mọi $t\in \mathbf{R}$. Vậy ta có $\pi =\varrho$; vì $\overline{u}$ là phần tử sinh vi phân của $\pi$ (bổ đề. 14), ta có $\overline{u}=u$, điều này chứng minh rằng $u$ là tự liên hợp.

Bây giờ ta chứng minh Định lý 1.

Các ánh xạ $\sigma$ và $\tau$ được xác định tốt (bổ đề 15 và bổ đề 11, tương ứng).

Cho $\varrho$ là một biểu diễn unita của $\mathbf{R}$. Gọi $u$ là phần tử sinh vi phân của nó. Quan hệ $\varrho (t) =e^{itu}$ với mọi $t\in \mathbf{R}$ (bổ đề 15) chứng minh rằng $\tau \circ \sigma$ là ánh xạ đồng nhất.

Cho $u$ là một toán tử bộ phận tự liên hợp trên E. Bổ đề 14 chứng minh rằng phần tử sinh vi phân của biểu diễn unita $t\mapsto e^{itu}$ bằng $u$, do đó $\sigma \circ \tau$ là ánh xạ đồng nhất.

Cho $u$ là một toán tử từng phần tự liên hợp trên E và cho $\varrho (t) =e^{itu}$ với $t\in \mathbf{R}$ là biểu diễn unita của $\mathbf{R}$ trong E liên kết với nó. Cho $x\in$ dom($u$). Phương trình $\partial_t\varrho (t)x=iu(\varrho (t)x)$ được thỏa mãn khi đó (Bổ đề 13, b)) được gọi là phương trình Schrödinger.

#### Hệ quả {#ts-v-s2-n10-cor-1 .statement tag=03BA}

Cho $\varrho$ là một biểu diễn unita của $\mathbf{R}$ trong một không gian Hilbert E. Tồn tại một không gian địa phương compact X, một độ đo dương $\mu$ trên X và một hàm liên tục $g$ trên X với các giá trị thực sao cho $\varrho$ đẳng cấu với biểu diễn $\pi$ của $\mathbf{R}$ trong $L^2(X, \mu)$ được xác định bởi $\pi (t)f=e^{itg}f$ với mọi $t\in \mathbf{R}$ và mọi $f\in L^2(X, \mu)$.

Cho $u$ là toán tử tự liên hợp trên E sao cho $\varrho (t) =e^{itu}$ với mọi $t\in \mathbf{R}$ (Định lý 1). Tồn tại một không gian địa phương compact X, một độ đo dương $\mu$ trên X, một đẳng cấu đẳng cự $\theta$ của $L^2(X, \mu)$ lên E và một hàm liên tục $g$ trên X với các giá trị thực sao cho $u=\theta \circ m_g\circ \theta^{-1}$ (Đl. 1 của IV, p. 266). Mệnh đề suy ra từ công thức $e^{itu}=\theta \circ e^{itm_g}\circ \theta^{-1}=\theta \circ m_{e^{itg}}\circ \theta^{-1}$ (Bổ đề 4 của IV, p. 269).

#### Nhận xét {#ts-v-s2-n10-rem-1 .statement tag=03BB}

Giả sử rằng $u$ là một tự đồng cấu của E. Biểu diễn unita của $\mathbf{R}$ trong E được xác định bởi $\varrho (t) =e^{itu}$ khi đó thỏa mãn bất đẳng thức $\|\varrho (t)-1_E\|\leqslant |t| \|u\|$ với mọi $t\in \mathbf{R}$, và ánh xạ $\varrho$ của $\mathbf{R}$ vào không gian Banach $\mathscr{L}(E)$ là nghiệm duy nhất của phương trình vi phân tuyến tính

$$
1d\varrho
$$

$$
=u\circ \varrho
$$

$$
idt
$$

(xem FVR, IV, p. 26, §6).

#### Ví dụ {#ts-v-s2-n10-exa-1 .statement tag=03BC}

Cho $\varrho$ là biểu diễn chính quy của $\mathbf{R}$ trong $L^2(\mathbf{R})$. Phần tử sinh vô cùng bé của $\varrho$ là bao đóng của toán tử vi phân với miền $\mathscr{D}(\mathbf{R})$ được xác định bởi $f\mapsto  -if'$.

## BÀI TẬP {#ts-v-s2-exercises}

Trong các bài tập của đoạn này, trừ khi có chỉ dẫn khác, G ký hiệu một nhóm tôpô địa phương compact, được trang bị một độ đo Haar trái ký hiệu bởi $\mu$.

Xem [các bài tập cho § 2](exercises/s2/).
