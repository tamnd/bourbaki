---
book: ts
book_title: Théories spectrales
chapter: V
chapter_title: REPRÉSENTATIONS UNITAIRES
section: 1
section_title: Représentations unitaires
lang: vi
source: ts-iii-v-fr
book_pages: TS V.373-TS V.398, TS V.483-TS V.486
pdf_pages: 0386-0411, 0496-0499
extraction: native
subsections:
    - "no": 1
      title: Rappels concernant les représentations linéaires continues
      page: 374
      pdf_page: 387
    - "no": 2
      title: Un critère de continuité
      page: 377
      pdf_page: 390
    - "no": 3
      title: Représentations continues de dimension finie
      page: 378
      pdf_page: 391
    - "no": 4
      title: Représentations irréductibles
      page: 378
      pdf_page: 391
    - "no": 5
      title: Représentations unitaires
      page: 379
      pdf_page: 392
    - "no": 6
      title: Somme directe hilbertienne et produit tensoriel de représentations unitaires
      page: 383
      pdf_page: 396
    - "no": 7
      title: Coefficients matriciels
      page: 385
      pdf_page: 398
    - "no": 8
      title: Le lemme de Schur
      page: 386
      pdf_page: 399
    - "no": 9
      title: Semi-simplicité
      page: 390
      pdf_page: 403
    - "no": 10
      title: Classes de représentations unitaires
      page: 392
      pdf_page: 405
    - "no": 11
      title: Composantes isotypiques
      page: 394
      pdf_page: 407
statements: 50
exercises: 7
content_sha256: 1d555f5b27e834c0f17f9f00487272d615e71239341b52d1ed56868cdad09ab1
translated_from: content/en-mt/ts/V/01_s1_representations_unitaires.md
source_lang: en-mt
translation_method: machine
source_content_sha256: f1149d81aaad2860301eff5572205d32a2e9786cc132ddd1dbc63f7daad65029
translation_model: gpt-5-mini, gpt-5-6, gpt-5-6-mini
translation_run: translate-vi-7b233af3
glossary_version: 34
glossary_terms_sha256: 82f9ffa966aefff9aa148e8e2003b278e88e33285046304bfe1791caef8b49e0
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 1. BIỂU DIỄN UNITA

Trong đoạn này, các không gian vectơ là trên $K =\mathbf{R}$ hoặc $\mathbf{C}$.

Nhắc lại rằng một biểu diễn tuyến tính của một nhóm G trong một không gian vectơ trên K E là một đồng cấu $\varrho$ của G vào nhóm $\mathbf{G}\mathbf{L}(E)$ các tự đẳng cấu của E (A, VIII, p. 387, Định nghĩa 1). Người ta nói rằng E là không gian của biểu diễn $\varrho$, và rằng chiều của E là chiều của $\varrho$, cũng được ký hiệu là dim($\varrho$ ).

Người ta có thể đồng nhất một biểu diễn của G trong một không gian vectơ trên K với một K[G]-môđun (loc. cit.), và thuật ngữ tương ứng sẽ được sử dụng, chẳng hạn đối với các tổng trực tiếp của các biểu diễn, các cấu xạ của các biểu diễn, hoặc biểu diễn trên $\mathbf{C}$ thu được từ một biểu diễn trong một không gian vectơ trên $\mathbf{R}$ bằng mở rộng vô hướng.

Một biểu diễn $\varrho : G\rightarrow \mathbf{G}\mathbf{L}(E)$ được gọi là trung thành nếu nó là một đơn cấu.

Cần chú ý rằng điều này không có nghĩa là K[G]-môđun liên kết với $\varrho$ là một K-môđun trung thành (A, II, p. 28).

Đặc trưng của một biểu diễn của G trong một không gian vectơ trên K hữu hạn chiều là ánh xạ $\chi_{\varrho}$ của G vào K sao cho $\chi_{\varrho}(g) =$ Tr($\varrho (g)$) với mọi $g\in G$, cf. A, VIII, p. 388.

### 1. Các nhắc lại liên quan đến các biểu diễn tuyến tính liên tục

Cho G là một nhóm tôpô. Nhắc lại rằng một biểu diễn tuyến tính liên tục của G trong một không gian vectơ tôpô trên K E là một biểu diễn tuyến tính $\varrho$ của G trong E sao cho ánh xạ từ $G\times E$ vào E xác định bởi $(g, x)\mapsto \varrho (g)x$ là liên tục (INT, VIII, p. 128, § 2, No.$^o1$, Định nghĩa 1). Ánh xạ này xác định một tác động của G trên E và ảnh của $\varrho$ được chứa trong $\mathscr{L}(E)$. Một biểu diễn liên tục $\varrho$ được gọi là bị chặn nếu ảnh của nó bị chặn trong không gian $\mathscr{L}(E)$ được trang bị tôpô hội tụ bị chặn.

#### Nhận xét {#ts-v-s1-n1-rem-1 .statement tag=038J}

Nếu $K =\mathbf{R}$ và nếu $\varrho$ là một biểu diễn tuyến tính liên tục của G trong một không gian vectơ trên $\mathbf{R}$ E, thì ánh xạ $\varrho_{(\mathbf{C})}:g\mapsto 1\otimes \varrho (g)$ là một biểu diễn tuyến tính liên tục của G trong $E_{(\mathbf{C})}$; nếu $\varrho$ bị chặn, thì $\varrho_{(\mathbf{C})}$ bị chặn.

Đối với mọi không gian vectơ tôpô trên K E, đồng cấu gắn $1_E$ với mọi $g\in G$ là một biểu diễn tuyến tính liên tục của G trong E, được gọi là biểu diễn tầm thường của G trong E.

Cho H là một nhóm con của G. Hạn chế của $\varrho$ lên H là một biểu diễn tuyến tính liên tục của H trong E, ký hiệu là Res$^G_H(\varrho )$.

Cho $\varrho_1$ và $\varrho_2$ là các biểu diễn tuyến tính liên tục của G trong các không gian vectơ tôpô trên K $E_1$ và $E_2$. Một G-cấu xạ $u$ của $\varrho_1$ vào $\varrho_2$ là một cấu xạ của các biểu diễn tuyến tính liên tục, nghĩa là một ánh xạ tuyến tính liên tục $u: E_1\rightarrow E_2$ sao cho $u\circ \varrho_1(g) =\varrho_2(g)\circ u$ với mọi $g\in G$. Không gian vectơ các G-cấu xạ của $\varrho_1$ vào $\varrho_2$ được ký hiệu bởi Hom$_G(\varrho_1, \varrho_2)$. Nó là một không gian con đóng của không gian $\mathscr{L}(E_1; E_2)$ được trang bị tôpô hội tụ đơn giản.

Cho $\varrho$ là một biểu diễn tuyến tính liên tục của một nhóm G trong một không gian vectơ tôpô trên K E. Ánh xạ đồng nhất $1_E$ của E là một G-cấu xạ của $\varrho$ vào $\varrho$, ký hiệu bởi $1_{\varrho}$. Nếu $\varrho_1,\varrho_2$ và $\varrho_3$ lần lượt là các biểu diễn tuyến tính liên tục của G trong các không gian vectơ tôpô trên K $E_1, E_2, E_3$, và nếu $u: E_1\rightarrow E_2$ và $v: E_2\rightarrow E_3$ là các G-cấu xạ, thì $v\circ u$ là một G-cấu xạ.

Một cấu xạ G $u$ từ $\varrho_1$ vào $\varrho_2$ là một G-đẳng cấu nếu tồn tại một cấu xạ G $v$ từ $\varrho_2$ vào $\varrho_1$ sao cho $v\circ u= 1_{\varrho_1}$ và $u\circ v= 1_{\varrho_2}$. Điều này tương đương với việc $u$ là một cấu xạ G và là một đẳng cấu của các không gian vectơ tôpô từ không gian của $\varrho_1$ lên không gian của $\varrho_2$; nghịch đảo $v=u^{-1}$ của nó khi đó thực sự là một cấu xạ G. Nếu tồn tại một G-đẳng cấu từ $\varrho_1$ lên $\varrho_2$, ta nói rằng các biểu diễn này là đẳng cấu.

#### Định nghĩa 1 {#ts-v-s1-def-1 .statement tag=038K}

Cho $\varrho$ là một biểu diễn tuyến tính liên tục của một nhóm tôpô G trong một không gian vectơ tôpô E. Một biểu diễn tuyến tính liên tục $\pi$ của G trong F là một biểu diễn con của $\varrho$ nếu F là một không gian con đóng của E và nếu, với mọi $g\in G$, không gian F ổn định dưới $\varrho (g)$ và $\pi (g)$ là tự đồng cấu của F suy ra từ $\varrho (g)$ bằng cách chuyển qua các không gian con.

Cho $\varrho$ là một biểu diễn tuyến tính liên tục của một nhóm tôpô G trong một không gian vectơ tôpô E. Bao đóng của $\{0\}$ trong E là một biểu diễn con của $\varrho$. Tổng quát hơn, bao đóng của một không gian con ổn định dưới các tự đồng cấu $\varrho (g)$ là một biểu diễn con của $\varrho$.

Một biểu diễn con $\pi$ của $\varrho$ được xác định một cách duy nhất bởi một không gian con đóng F, ổn định dưới mọi tự đồng cấu $\varrho (g)$. Điều kiện sau này thường được phát biểu dưới dạng “F là một không gian con G-bất biến của E”. Khi đó người ta cũng nói rằng F xác định một biểu diễn con của $\varrho$, hoặc đôi khi, do lạm dụng ngôn ngữ, rằng F là một biểu diễn con của $\varrho$, hoặc của E.

Cho F là một không gian con của E xác định một biểu diễn con $\pi$ của $\varrho$. Với mọi $g\in G$, ánh xạ tuyến tính $\varrho (g)$ xác định, bằng cách chuyển qua thương, một tự đồng cấu $\widetilde{\varrho}(g)$ của $E/F$. Ánh xạ $g\mapsto \widetilde{\varrho}(g)$ là một biểu diễn tuyến tính liên tục của G trong $E/F$ và phép chiếu chính tắc của E lên $E/F$ là một cấu xạ G. Người ta nói rằng $\widetilde{\varrho}$ là biểu diễn thương của G trên $E/F$; nó cũng được ký hiệu là $\varrho /\pi$.

Không gian con của các phần tử của E bất biến dưới tác động của G là một biểu diễn con tầm thường của $\varrho$. Nó được ký hiệu là $\varrho^G$ hoặc $E^G$.

Cho A là một tập con của E. Không gian con đóng F sinh bởi các phần tử $\varrho (g)x$, trong đó $g\in G$ và $x\in A$, là một biểu diễn con của $\varrho$, được gọi là biểu diễn con của $\varrho$ sinh bởi A; nếu F = E, người ta nói rằng A sinh $\varrho$. Nếu biểu diễn con F là hữu hạn chiều, người ta nói rằng tập con A là G-hữu hạn.

Giả sử rằng A rút gọn thành một phần tử duy nhất $x\in E$. Nếu A sinh $\varrho$, người ta nói rằng $x$ là một vectơ chu kỳ của $\varrho$ và rằng $\varrho$ là một biểu diễn chu kỳ; người ta nói rằng $x$ là một vectơ G-hữu hạn nếu A là G-hữu hạn.

Tập hợp các vectơ G-hữu hạn của $\varrho$ là một không gian con vectơ của E ổn định dưới $\varrho$; nó không nhất thiết đóng.

Cho $(\varrho_i)_{i\in I}$ là một họ các biểu diễn tuyến tính liên tục của G trong các không gian vectơ K tôpô lồi địa phương $(E_i)_{i\in I}$. Gọi E là không gian tổng trực tiếp của các không gian $E_i$. Ánh xạ $g\mapsto (\varrho_i(g))$ là một biểu diễn tuyến tính của G trong E, được gọi là tổng, hay tổng trực tiếp, của các biểu diễn $\varrho_i$. Nếu I là hữu hạn, nó liên tục.

Nếu các biểu diễn $\varrho_i$ đều bằng một biểu diễn $\varrho$ với mọi $i\in I$, người ta nói rằng tổng trực tiếp của các biểu diễn $\varrho_i$ là tổng của Card(I) bản sao của biểu diễn $\varrho$, và nó cũng được ký hiệu là $\varrho^{Card(I)}$, hoặc Card(I) $\varrho$.

Cho $(\varrho_i)_{i\in I}$ và $(\pi_j)_{j\in J}$ là các họ hữu hạn các biểu diễn tuyến tính liên tục của G trong các không gian vectơ K tôpô $(E_i)_{i\in I}$ và $(F_j)_{j\in J}$, tương ứng. Đẳng cấu chính tắc của các không gian vectơ K

Hom$_K(\bigoplus_{i\in I}E_i,\bigoplus_{j\in J}F_j)\rightarrow \bigoplus_{(i,j)\in I\times J}$ Hom$_K(E_i,F_j)$ (A, II, p. 13, Hệ quả 1) cảm sinh, bằng cách chuyển qua các không gian con, một đẳng cấu

(1) Hom$_G(\bigoplus_{i\in I}\varrho_i,\bigoplus_{j\in J}\pi_j)\rightarrow \bigoplus_{(i,j)\in I\times J}$ Hom$_G(\varrho_i, \pi_j)$

mà cũng được gọi là chính tắc.

Cho $\varrho_1$ và $\varrho_2$ là các biểu diễn tuyến tính của G trong các không gian vectơ K tôpô $E_1$ và $E_2$. Với $u\in \mathscr{L}(E_1; E_2)$ và $g\in G$, người ta đặt $\varrho (g)u=\varrho_2(g)\circ u\circ \varrho_1(g^{-1})$. Ánh xạ $g\mapsto \varrho (g)$ là một biểu diễn tuyến tính của G trong $\mathscr{L}(E_1; E_2)$. Không gian của các phần tử bất biến đối với biểu diễn này trùng với Hom$_G(\varrho_1, \varrho_2)$.

Cho $\varrho$ là một biểu diễn tuyến tính liên tục của G trong một không gian lồi địa phương E. Nhắc lại (INT, VIII, p. 131, § 2, n$^o2$) rằng biểu diễn đối ngẫu $\breve{\varrho}$ của $\varrho$ là biểu diễn tuyến tính của G trong không gian đối ngẫu $E'$ của E được xác định bởi $\breve{\varrho}(g) =^t\varrho (g^{-1})$.

### 2. Một tiêu chuẩn về tính liên tục

Kết quả sau đây cho phép kiểm tra rằng một số biểu diễn tuyến tính của một tích trực tiếp các nhóm tôpô là liên tục.

#### Bổ đề 1 {#ts-v-s1-lem-1 .statement tag=038L}

Cho G và H là các nhóm tôpô và E là một không gian Banach. Cho $\varrho$ là một biểu diễn bị chặn của G trong E và $\pi$ là một biểu diễn bị chặn của H trong E. Giả sử rằng $\varrho (g)$ giao hoán với $\pi (h)$ với mọi $(g, h)\in G\times H$. Ánh xạ $\varpi$ từ $G\times H$ vào $\mathbf{G}\mathbf{L}(E)$ được xác định bởi $(g, h)\mapsto \varrho (g)\circ \pi (h)$ là một biểu diễn tuyến tính liên tục bị chặn của $G\times H$ trong E.

Ánh xạ $\varpi$ là một biểu diễn tuyến tính của $G\times H$ trong E; ta hãy kiểm tra rằng nó liên tục. Vì $\|\varpi (g, h)\|\leqslant \|\varrho (g)\|\|\pi (h)\|$ với mọi $(g, h)\in G\times H$, biểu diễn $\varpi$ bị chặn, và do đó ảnh của nó là đẳng liên tục trong $\mathscr{L}(E)$. Khi đó chỉ cần chứng minh rằng, với mọi $x\in E$, ánh xạ $(g, h)\mapsto \varpi (g, h)x$ là liên tục (Nhận xét 2 của INT, VIII, p. 129, § 2, n$^o1$). Cho $(g_0, h_0)\in G\times H$. Đặt $y=\pi (h_0)x$. Với mọi $(g, h)\in G\times H$, ta có

$$
\|\varpi (g, h)x-\varpi (g_0, h_0)x\|\leqslant \|\varrho (g)(\pi (h)x-y)\|+\|\varrho (g)y-\varrho (g_0)y\|
$$

$$
\leqslant \|\varrho (g)\| \|\pi (h)x-y\|+\|\varrho (g)y-\varrho (g_0)y\|
$$

Vì $\varrho$ bị chặn và vì $\varrho$ và $\pi$ liên tục, điều này suy ra mệnh đề.

### 3. Các biểu diễn hữu hạn chiều liên tục

Cho $\varrho$ là một biểu diễn tuyến tính liên tục của một nhóm tôpô G trong một không gian vectơ tôpô K tách được E có số chiều hữu hạn. Ta trang bị cho $\mathscr{L}(E)$ cấu trúc duy nhất của không gian vectơ tôpô tách được trên K; cấu xạ $\varrho : G\rightarrow \mathbf{G}\mathbf{L}(E)$ khi đó là liên tục vì tôpô của $\mathbf{G}\mathbf{L}(E)$ được cảm sinh bởi tôpô của $\mathscr{L}$ (E), tôpô này trùng với tôpô hội tụ đơn giản (TVS, I, p. 14, Định lý 2). Do đó, đặc trưng của $\varrho$ là liên tục. Nếu G là một nhóm Lie thực, thì đặc trưng của $\varrho$ là một hàm giải tích trên G (LIE, III, p. 225, § 8, No. $^o1$, Định lý 1). Biểu diễn đối ngẫu cũng liên tục khi $E'$ được trang bị tôpô duy nhất của không gian vectơ tôpô tách được trên K. Hơn nữa, với mọi số nguyên $n\geqslant 0$, các biểu diễn $\mathsf{T}^n(\varrho ),\mathsf{S}^n(\varrho )$ và $\wedge^n(\varrho ) ($loc. cit.) là liên tục, khi các không gian tương ứng được trang bị các tôpô của các không gian vectơ tôpô tách được trên K.

Cho $\varrho_1$ và $\varrho_2$ là các biểu diễn liên tục của một nhóm tôpô G trong các không gian vectơ tôpô tách được $E_1$ và $E_2$ có số chiều hữu hạn. Biểu diễn tuyến tính $\varrho_1\otimes \varrho_2$ của G trong $E_1\otimes E_2$ (LIE, III, p. 256, Phụ lục) là liên tục, không gian $E_1\otimes E_2$ được trang bị tôpô của không gian vectơ tôpô tách được trên K.

### 4. Các biểu diễn bất khả quy

Trong No. này, G là một nhóm tôpô.

#### Định nghĩa 2 {#ts-v-s1-def-2 .statement tag=038M}

Một biểu diễn $\varrho$ của G trong một không gian vectơ tôpô K E được gọi là bất khả quy nếu $\{0\}$ không trù mật trong E và nếu các biểu diễn con duy nhất của $\varrho$ là $\varrho$ và biểu diễn trong bao đóng của $\{0\}$.

Nếu $\varrho$ là một biểu diễn bất khả quy của G trong một không gian vectơ tôpô tách được E, thì mọi phần tử khác không của E là một vectơ cyclic của $\varrho$.

#### Bổ đề 2 {#ts-v-s1-lem-2 .statement tag=038N}

Cho $\pi$ và $\varrho$ là các biểu diễn tuyến tính liên tục của G trong các không gian vectơ tôpô K tách được. Giả sử rằng $\pi$ là bất khả quy. Mọi G-cấu xạ khác không từ $\pi$ vào $\varrho$ đều là đơn ánh, và mọi G-cấu xạ khác không từ $\varrho$ vào $\pi$ đều có ảnh trù mật.

Đặc biệt, nếu $\pi$ và $\varrho$ là bất khả quy và hữu hạn chiều, thì mọi G-cấu xạ khác không từ $\pi$ vào $\varrho$ đều là một đẳng cấu.

Vì không gian của $\varrho$ là tách được, hạt nhân của một G-cấu xạ $u$ từ $\pi$ vào $\varrho$ là đóng, và tạo ra một biểu diễn con của $\pi$. Nếu cấu xạ $u$ khác không, hạt nhân của nó do đó phải được rút gọn về 0, vì $\pi$ là một biểu diễn bất khả quy trong một không gian vectơ tôpô tách được. Tương tự, bao đóng của ảnh của một G-cấu xạ khác không từ $\varrho$ vào $\pi$ là một biểu diễn con khác không của $\pi$, và do đó bằng không gian của $\pi$.

Khẳng định cuối cùng suy ra từ điều trên.

#### Bổ đề 3 {#ts-v-s1-lem-3 .statement tag=038O}

Cho $\varrho$ là một biểu diễn tuyến tính liên tục của G trong một không gian vectơ tôpô K tách được E có số chiều hữu hạn. Nếu E khác không, thì tồn tại một biểu diễn con bất khả quy của $\varrho$.

Vì E hữu hạn chiều và khác không, tồn tại một không gian con bất biến G F của E khác không và có chiều cực tiểu. Không gian con này đóng trong E và xác định một biểu diễn con của E; mọi biểu diễn con của F cũng là một biểu diễn con của E, và do đó biểu diễn F là bất khả quy theo tính cực tiểu.

#### Nhận xét {#ts-v-s1-n4-rem-1 .statement tag=038P}

Một biểu diễn khác không E của G không phải lúc nào cũng chứa một biểu diễn con bất khả quy (cf. V, p. 426, nhận xét). Tuy nhiên, ta sẽ thấy rằng điều này đúng nếu G compact và nếu $K =\mathbf{C}$ và nếu E là một không gian lồi địa phương khác không đầy đủ quasi tách được trên K (Mệnh đề 7 của V, p. 464).

### 5. Các biểu diễn unita

#### Định nghĩa 3 {#ts-v-s1-def-3 .statement tag=038Q}

Cho G là một nhóm tôpô và E là một không gian Hilbert trên K. Một biểu diễn unita của G trong E là một biểu diễn tuyến tính liên tục $\varrho$ của G trong E sao cho, với mọi $g$ trong G, tự đồng cấu $\varrho (g)$ của E là một tự đồng cấu unita (TVS, V, p. 40) của E.

Nói cách khác, một biểu diễn unita là một biểu diễn đẳng cự trong một không gian Hilbert. Đặc biệt, một biểu diễn unita bị chặn.

Biểu diễn tầm thường của một nhóm tôpô trong một không gian Hilbert là unita. Mọi biểu diễn con của một biểu diễn unita là unita. Hạn chế của một biểu diễn unita vào một nhóm con là unita.

#### Định nghĩa 4 {#ts-v-s1-def-4 .statement tag=038R}

Cho G là một nhóm tôpô, và cho $\varrho$ và $\pi$ là các biểu diễn unita của G trong các không gian Hilbert E và F tương ứng. Một dạng sesquiline bất biến theo G trên $E\times F$ là một dạng sesquiline liên tục $q$ trên $E\times F$ sao cho

$$
q(x, y) =q(\varrho (g)x, \pi (g)y)
$$

với mọi $g\in G$ và mọi $(x, y)\in E\times F$.

Không gian vectơ của các dạng sesquiline bất biến theo G trên $E\times F$ được ký hiệu bởi Sesq$_G(\varrho , \pi )$ hoặc Sesq$_G(E,F)$.

#### Ví dụ {#ts-v-s1-n5-exa-1 .statement tag=038S}

Cho G là một nhóm tôpô, và cho $\varrho$ là một biểu diễn unita của G trong E. Tích vô hướng $q$ trên E là một dạng sesquiline bất biến theo G trên $E\times E$.

#### Bổ đề 4 {#ts-v-s1-lem-4 .statement tag=038T}

Cho G là một nhóm tôpô, và cho $\varrho$ là một đồng cấu của G vào nhóm unita $\mathbf{U}(E)$ của một không gian Hilbert E. Khi đó $\varrho$ là một biểu diễn unita của G khi và chỉ khi $\varrho$ liên tục tại phần tử $e$ của G đối với tôpô hội tụ đơn giản trên $\mathbf{U}(E)$. Chỉ cần tính chất này đúng với mọi $x$ trong một tập con toàn phần của E.

Điều kiện này hiển nhiên là cần thiết. Nó đủ theo Nhận xét 2 của INT, VIII, p. 129, § 2, n$^o1$, vì ảnh của $\varrho$ là liên tục đều trong $\mathscr{L}(E)$ và vì tính liên tục của ánh xạ $g\mapsto \varrho (g)x$ tại $e$ kéo theo tính liên tục của nó trên G.

Cho G là một nhóm tôpô. Nếu $\varrho_1$ và $\varrho_2$ là các biểu diễn unita của G và nếu $u$ thuộc Hom$_G(\varrho_1, \varrho_2)$, thì $u^*$ thuộc Hom$_G(\varrho_2, \varrho_1)$. Thật vậy, vì $\varrho_1$ và $\varrho_2$ là các biểu diễn unita, ta có với mọi $g\in G$

$$
u^*\circ \varrho_2(g) =u^*\circ \varrho_2(g^{-1})^*= (\varrho_2(g^{-1})\circ u)^*
$$

$$
= (u\circ \varrho_1(g^{-1}))^*=\varrho_1(g)\circ u^*
$$

#### Bổ đề 5 {#ts-v-s1-lem-5 .statement tag=038U}

Cho G là một nhóm tôpô, và cho $\varrho$ là một biểu diễn unita của G trong một không gian Hilbert phức E. Không gian Hom$_G(\varrho , \varrho )$ là một đại số con có đơn vị, có đối hợp của $\mathscr{L}(E)$.

Điều đã trình bày trước đó cho thấy Hom$_G(\varrho , \varrho )$ là một đại số con tự liên hợp có đơn vị của $\mathscr{L}(E)$. Vì nó đóng trong $\mathscr{L}$ (E), nên nó là một đại số con có đối hợp của $\mathscr{L}(E)$.

#### Bổ đề 6 {#ts-v-s1-lem-6 .statement tag=038V}

Cho $\pi$ và $\varrho$ là các biểu diễn unita của một nhóm tôpô G trong các không gian Hilbert E và F tương ứng. Cho D là một không gian con trù mật của E ổn định theo $\pi$. Cho $u$ là một toán tử bộ phận đóng từ E vào F với miền xác định D sao cho $u\circ \pi (g) =\varrho (g)\circ u$ với mọi $g\in G$. Khi đó miền xác định của $u^*$ ổn định theo $\varrho$ và ta có quan hệ $u^*\circ \varrho (g) =\pi (g)\circ u^*$ với mọi $g\in G$.

Cho $g\in G$ và $x\in$ dom($u^*$). Với mọi $y\in$ dom($u$), ta có

$$
\langle \varrho (g)x|u(y)\rangle =\langle x|\varrho (g^{-1})u(y)\rangle =\langle x|u(\pi (g^{-1})y)\rangle
$$

$$
=\langle u^*(x)|\pi (g^{-1})y\rangle =\langle \pi (g)(u^*(x))|y\rangle
$$

vì $\varrho (g)^*=\varrho (g)^{-1}=\varrho (g^{-1})$. Điều này chứng minh rằng $\varrho (g)x\in$ dom($u^*$) và rằng $u^*(\varrho (g)x) =\pi (g)(u^*(x))$. Đặc biệt, miền của $u^*\circ \varrho (g)$ chứa miền của $u^*$, và $\pi (g)\circ u^*\subset u^*\circ \varrho (g)$.

Nhưng hơn nữa, nếu $x\in$ dom($u^*\circ \varrho (g)$), thì $x=\varrho (g^{-1})(\varrho (g)x)$ thuộc dom($u^*$) theo điều đã nói trước áp dụng cho $g^{-1}$. Suy ra rằng $u^*\circ \varrho (g) =\pi (g)\circ u^*$.

#### Mệnh đề 1 {#ts-v-s1-prop-1 .statement tag=038W}

Cho $\varrho_1$ và $\varrho_2$ là các biểu diễn unita của một nhóm tôpô G trong các không gian Hilbert $E_1$ và $E_2$. Ánh xạ từ Hom$_G(\varrho_1, \varrho_2)$ vào Sesq$_G(\varrho_2, \varrho_1)$, gán cho $u$ dạng song tuyến tính nửa xác định $q_u$ được định nghĩa bởi $q_u(x, y) =\langle x|u(y)\rangle$, là một đẳng cấu của các không gian vectơ.

Nếu $u$ là một G-cấu xạ, thì ta có

$$
q_u(\varrho_2(g)x, \varrho_1(g)y) =\langle \varrho_2(g)x|u(\varrho_1(g))y\rangle
$$

$$
=\langle \varrho_2(g)x|\varrho_2(g)u(y)\rangle =\langle x|u(y)\rangle =q_u(x, y)
$$

với mọi $g\in G$ và mọi $(x, y)\in E_2\times E_1$, do đó ánh xạ đã chỉ ra là một ánh xạ tuyến tính từ Hom$_G(\varrho_1, \varrho_2)$ vào Sesq$_G(\varrho_2, \varrho_1)$. Theo EVT, V, p. 16, Hệ quả 2, nó là đơn ánh.

Ngược lại, cho $q$ là một dạng song tuyến tính nửa xác định G-bất biến và $u$ là ánh xạ tuyến tính duy nhất từ $E_1$ vào $E_2$ sao cho $q(x, y) =\langle x|u(y)\rangle$ với mọi $(x, y)\in E_2\times E_1($loc. cit.). Với mọi $g$ trong G và mọi $(x, y)$ trong $E_2\times E_1$, ta có

$$
\langle x|(\varrho_2(g)\circ u\circ \varrho_1(g^{-1}))(y)\rangle =\langle \varrho_2(g^{-1})x|u(\varrho_1(g^{-1})y)\rangle
$$

$$
=q(\varrho_2(g^{-1})x, \varrho_1(g^{-1})y) =q(x, y) =\langle x|u(y)\rangle
$$

do đó $u=\varrho_2(g)\circ u\circ \varrho_1(g^{-1})$. Do đó, $u\in$ Hom$_G(\varrho_2, \varrho_1)$. Mệnh đề được suy ra.

Cho $\varrho$ là một biểu diễn unita của một nhóm tôpô G trong một không gian Hilbert E. Nếu $K =\mathbf{C}$, ký hiệu $\overline{E}$ là không gian liên hợp của E (EVT, V, p. 6). Nếu $K =\mathbf{R}$, đặt $\overline{E}= E$. Biểu diễn liên hợp $\overline{\varrho}$ là biểu diễn của G trong $\overline{E}$ được định nghĩa bởi $\overline{\varrho}(g) =\varrho (g)$ với mọi $g\in G$. Nó là một biểu diễn unita của G; theo định nghĩa, một không gian con của $\overline{E}$ là một biểu diễn con của $\overline{E}$ khi và chỉ khi nó là một biểu diễn con của E.

#### Mệnh đề 2 {#ts-v-s1-prop-2 .statement tag=038X}

Cho $\varrho$ là một biểu diễn unita của một nhóm tôpô G trong một không gian Hilbert E. Gọi $u$ là đẳng cấu đẳng cự của $\overline{E}$ lên $E'$ liên kết với $x$ dạng tuyến tính $y\mapsto  \langle x|y\rangle$.

a) Ánh xạ $u$ là một đẳng cấu của biểu diễn liên hợp $\overline{\varrho}$ lên biểu diễn đối ngẫu đối nghịch $\breve{\varrho}$;

b) Trang bị cho $E'$ cấu trúc của một không gian Hilbert thu được bởi phép chuyển cấu trúc bằng $u$; biểu diễn đối ngẫu đối nghịch $\breve{\varrho}$ là một biểu diễn unita của G trong $E'$.

Theo EVT, V, p. 15, Định lý 3 và nhận xét sau đó, ánh xạ $u$ là một đẳng cấu đẳng cự.

Với mọi $g$ trong G, mọi $x$ trong $\overline{E}$ và mọi $y$ trong E, ta có

$$
\langle y,( \breve{\varrho}(g)\circ u)(x)\rangle =\langle \varrho (g^{-1})y, u(x)\rangle
$$

$$
=\langle x|\varrho (g^{-1})y\rangle =\langle \varrho (g)x|y\rangle =\langle y, u(\overline{\varrho}(g)x)\rangle
$$

do đó $\breve{\varrho}(g)\circ u=u\circ \overline{\varrho}(g)$, điều này chứng minh a); mệnh đề b) suy ra ngay lập tức.

#### Hệ quả {#ts-v-s1-n5-cor-1 .statement tag=038Y}

Cho $\varrho$ là một biểu diễn unita của một nhóm tôpô G trong một không gian Hilbert E. Các điều kiện sau là tương đương:

(i) Biểu diễn $\varrho$ là bất khả quy;

(ii) Biểu diễn đối ngẫu đối nghịch $\breve{\varrho}$ là bất khả quy;

(iii) Biểu diễn liên hợp $\overline{\varrho}$ là bất khả quy.

Điều này suy ra từ Mệnh đề 2, và từ nhận xét đứng trước nó liên quan đến các biểu diễn con của E.

#### Mệnh đề 3 {#ts-v-s1-prop-3 .statement tag=038Z}

Cho $\varrho$ là một biểu diễn unita của một nhóm tôpô G trong một không gian Hilbert E. Gọi $\pi$ là một biểu diễn con của E và F là không gian của $\pi$. Phần bù trực giao $F^{\circ}$ của F trong E là một biểu diễn con của E sao cho $E = F\oplus F^{\circ}$ và $F^{\circ}$ là đẳng cấu với $E/F$.

Không gian $F^{\circ}$ là đóng. Với mọi $x\in F^{\circ}$, mọi $g\in G$ và mọi $y\in F$, ta có $\langle \varrho (g)x|y\rangle =\langle x|\varrho (g^{-1})y\rangle = 0$ vì $\varrho$ là unita và F là một biểu diễn con. Do đó $\varrho (g)x\in F^{\circ}$.

Phép chiếu chính tắc của E lên $E/F$ là một G-cấu xạ, do đó ánh xạ của $F^{\circ}$ vào $E/F$ được suy ra từ nó bằng cách chuyển qua không gian con là một G-cấu xạ của $F^{\circ}$ vào $E/F$; theo EVT, V, p. 13, nó là một đẳng cấu đẳng cự.

Ta cũng sẽ ký hiệu bởi $\pi^{\circ}$ biểu diễn của G trong $F^{\circ}$.

#### Mệnh đề 4 {#ts-v-s1-prop-4 .statement tag=0390}

Cho $\varrho$ là một biểu diễn unita của một nhóm tôpô G trong một không gian Hilbert E. Một không gian con đóng F của E là một biểu diễn con của $\varrho$ khi và chỉ khi phép chiếu trực giao $p$ của E có ảnh F là một G-cấu xạ của $\varrho$ vào $\varrho$.

Giả sử rằng F là một biểu diễn con của $\varrho$. Cho $x\in E$ và viết $x=p(x) +y$ với $y\in F^{\circ}$. Với mọi $g$ trong G, ta có

$$
\varrho (g)x=\varrho (g)(p(x)) +\varrho (g)y
$$

và vì $\varrho (g)(p(x))$ thuộc F và $\varrho (g)y$ thuộc $F^{\circ}$ (Mệnh đề 3), ta có $p(\varrho (g)x) =\varrho (g)(p(x))$. Do đó $p$ thuộc Hom$_G(\varrho , \varrho )$.

Ngược lại, nếu $p\in$ Hom$_G(\varrho , \varrho )$ thì $1_E-p$ là một cấu xạ G, do đó F = Ker(1$_E-p$) là một biểu diễn con của $\varrho$.

### 6. Tổng trực tiếp Hilbert và Tích tenxơ của các biểu diễn unita

Cho G là một nhóm tôpô. Cho $(\varrho_i)_{i\in I}$ là một họ các biểu diễn unita của G trong các không gian Hilbert $E_i$. Cho E là không gian tổng trực tiếp Hilbert ngoài của các $E_i$ (EVT, V, p. 18, Định. 1). Với mọi $g$ trong G và mọi $x= (x_i)_{i\in I}$ trong E, ta có

$$
\sum_i\|\varrho_i(g)x_i\|^2=\sum_i\|x_i\|^2=\|x\|^2
$$

điều này chứng minh rằng $(\varrho_i(g)x_i)_{i\in I}$ thuộc E và có cùng chuẩn với $x$. Do đó phần tử $\varrho (g) : (x_i)_{i\in I}\mapsto (\varrho_i(g)x_i)_{i\in I}$ là một phần tử unita của $\mathscr{L}(E)$.

#### Bổ đề 7 {#ts-v-s1-lem-7 .statement tag=0391}

Ánh xạ $g\mapsto \varrho (g)$ là một biểu diễn unita của G trong E.

Theo Bổ đề 4 của V, p. 380, chỉ cần chứng minh rằng với mọi $i$ trong I và mọi $x$ trong $E_i$, ánh xạ $g\mapsto \varrho (g)x$ liên tục tại phần tử đơn vị $e$ của G. Ánh xạ này là hợp thành của ánh xạ liên tục $g\mapsto \varrho_i(g)x_i$ và đơn ánh chính tắc của $E_i$ vào E. Do đó nó liên tục.

Biểu diễn $\varrho$ được gọi là tổng Hilbert của các biểu diễn unita $(\varrho_i)_{i\in I}$; nó được ký hiệu bởi $\varrho =\bigoplus_{i\in I}\varrho_i$.

Cho G và H là các nhóm tôpô. Cho $\varrho_1$ (tương ứng $\varrho_2$) là một biểu diễn unita của G (tương ứng H) trong một không gian Hilbert $E_1$ (tương ứng $E_2$). Cho $E = E_1\widehat{\otimes}_2E_2$ là không gian tích tenxơ Hilbert của $E_1$ và $E_2$ (EVT, V, p. 28, Định. 1). Với $(g, h)\in G\times H$, cho $\varrho (g, h)$ là tự đồng cấu liên tục $\varrho_1(g)\widehat{\otimes}_2\varrho_2(h)$ của E (EVT, V, p. 28) ; nó sẽ được ký hiệu đơn giản là $\varrho_1(g)\otimes \varrho_2(h)$ khi không có nguy cơ nhầm lẫn.

#### Bổ đề 8 {#ts-v-s1-lem-8 .statement tag=0392}

a) Ánh xạ $\varrho : (g, h)\mapsto \varrho (g, h)$ là một biểu diễn unita của $G\times H$ trong E ;

b) Với mọi cơ sở trực chuẩn $(e_i)_{i\in I}$ của $E_1$, ánh xạ từ tổng Hilbert $\bigoplus_{i\in I}E_2$ vào E được xác định bởi $(y_i)_{i\in I}\mapsto \sum_{i\in I}e_i\otimes y_i$ là một đẳng cấu H-đẳng cự của tổng Hilbert $\bigoplus_{i\in I}\varrho_2$ lên Res$^{G\times H}_{\{e\}\times H}(\varrho )$;

c) Với mọi cơ sở trực chuẩn $(f_j)_{j\in J}$ của $E_2$, ánh xạ từ tổng Hilbert $\bigoplus_{j\in J}E_1$ vào E được xác định bởi $(x_j)_{j\in J}\mapsto \sum_{j\in J}x_j\otimes f_j$ là một đẳng cấu G-đẳng cự của tổng Hilbert $\bigoplus_{j\in J}\varrho_1$ lên Res$^{G\times H}_{G\times \{e\}}(\varrho )$.

Ánh xạ $(g, h)\mapsto \varrho (g, h)$ là một đồng cấu của G vào $\mathbf{G}\mathbf{L}(E) ($cf. EVT, V, p. 28, n$^o2)$. Cho $(e_i)_{i\in I}$ là một cơ sở trực chuẩn của $E_1$. Theo EVT, V, p. 29, Mệnh đề 3 và Hệ quả 2, ánh xạ

$$
u: (y_i)\mapsto \sum_{i\in I}e_i\otimes y_i
$$

là một đẳng cự từ tổng trực tiếp Hilbert $F_2=\bigoplus_{i\in I}E_2$ lên E. Nhờ đẳng cự này, biểu diễn $\varrho_H:h\mapsto \varrho (e, h)$ của H trong E được đồng nhất với biểu diễn tổng trực tiếp của các biểu diễn $(\varrho_2)_{i\in I}$ trong $F_2$. Đặc biệt, nó là một biểu diễn unita của H trong E (bổ đề 7). Tương tự, đồng cấu $\varrho_G:g\mapsto \varrho (g, e)$ là một biểu diễn unita của G trong E.

Cho $(g, h)\in G\times H$. Ta có $\varrho (g, h) =\varrho_G(g)\circ \varrho_H(h)$; do đó $\varrho (g, h)$ là unita; hơn nữa, $\varrho_G(g)$ và $\varrho_H(h)$ giao hoán, suy ra bổ đề 1 của V, p. 377 kéo theo rằng $\varrho$ là một biểu diễn unita của $G\times H$.

Cuối cùng, các khẳng định liên quan đến hạn chế của $\varrho$ lên các nhóm con $\{e\} \times H$ và $G\times  \{e\}$ đã thu được trong quá trình lập luận trước đó.

Biểu diễn $(g, h)\mapsto \varrho_1(g)\otimes \varrho_2(h)$ của $G\times H$ được gọi là tích tenxơ ngoài của các biểu diễn unita $\varrho_1$ và $\varrho_2$, và được ký hiệu bởi $\varrho_1\boxtimes \varrho_2$.

Cho $n\in \mathbf{N}$ và cho $(G_i)_{1\leqslant i\leqslant n}$ là một họ hữu hạn các nhóm tôpô. Cho $\varrho_i$ là một biểu diễn unita của $G_i$ trong một không gian Hilbert $E_i$ với $1\leqslant i\leqslant n$. Người ta định nghĩa tương tự một biểu diễn

$$
\varrho_1\boxtimes \cdots \boxtimes \varrho_n
$$

của $G_1\times  \cdots  \times G_n$ trong không gian Hilbert $E = E_1\widehat{\otimes}_2\cdots \widehat{\otimes}_2E_n$ (EVT, V, p. 27).

Giả sử rằng $G_i= G$ với $1\leqslant i\leqslant n$. Cho $\Delta_n: G\rightarrow G^n$ là đồng cấu được xác định bởi $g\mapsto (g, . . . , g)$ với mọi $g\in G$. Người ta ký hiệu bởi $\varrho_1\otimes  \cdots  \otimes \varrho_n$ biểu diễn unita $(\varrho_1\boxtimes \cdots \boxtimes \varrho_n)\circ \Delta_n$ của G. Người ta nói rằng đó là tích tenxơ của các biểu diễn unita $\varrho_i$.

Với mọi phép hoán vị $\sigma$ của $\{1, . . . , n\}$, đẳng cấu chính tắc

$$
E_1\widehat{\otimes}_2\cdots \widehat{\otimes}_2E_n\rightarrow E_{\sigma(1)}\widehat{\otimes}_2\cdots \widehat{\otimes}_2E_{\sigma(n)}
$$

(EVT, V, p. 28) là một đẳng cấu đẳng cự

$$
\varrho_1\otimes  \cdots  \otimes \varrho_n\rightarrow \varrho_{\sigma(1)}\otimes  \cdots  \otimes \varrho_{\sigma(n)}
$$

của các biểu diễn của G.

Nếu $\varrho_i=\varrho$ với $1\leqslant i\leqslant n$, trong đó $\varrho$ là một biểu diễn unita của G, người ta cũng ký hiệu bởi $\varrho^{\otimes n}$ biểu diễn tích-tenxơ của các $\varrho_i$, và người ta nói rằng đó là lũy thừa tenxơ thứ $n^e$ của $\varrho$.

### 7. Các hệ số ma trận

#### Định nghĩa 5 {#ts-v-s1-def-5 .statement tag=0393}

Cho G là một nhóm tôpô và cho $\varrho$ là một biểu diễn unita của G trong một không gian Hilbert E. Cho $x$ và $y$ là các phần tử của E. Hàm từ G vào K cho bởi $g\mapsto  \langle x|\varrho (g)y\rangle$ được gọi là một hệ số ma trận của $\varrho$, hoặc một hàm đại diện. Nếu $x=y$, nó được gọi là một hệ số ma trận đường chéo. Nếu $\varrho$ là hữu hạn chiều, nó được gọi là một hệ số ma trận hữu hạn chiều.

Các hệ số ma trận của $\varrho$ là các hàm liên tục bị chặn trên G. Ta ký hiệu bởi Υ(G) (tương ứng Θ(G)) tập hợp các hệ số ma trận của các biểu diễn unita phức (tương ứng các biểu diễn unita phức hữu hạn chiều) của G.

#### Mệnh đề 5 {#ts-v-s1-prop-5 .statement tag=0394}

Cho G là một nhóm tôpô. Các tập hợp Θ(G) và Υ(G) là các đại số con có đơn vị đối hợp của $\mathscr{C}_b(G)$.

Hàm hằng 1 là một hệ số ma trận của biểu diễn tầm thường của G trên $\mathbf{C}$. Cho $\varrho$ là một biểu diễn unita của G và cho $x$ và $y$ là các vectơ của không gian của $\varrho$. Với mọi $\lambda \in \mathbf{C}$ và mọi $g\in G$, ta có $\lambda \langle x|\varrho (g)y\rangle =\langle x|\varrho (g)(\lambda y)\rangle$. Hơn nữa, ta có

$$
\langle x|\varrho (g)y\rangle =\langle \varrho (g^{-1})x|y\rangle =\overline{\langle y|\varrho(g^{-1})x\rangle}
$$

với mọi $g\in G$. Do đó, các tập hợp Θ(G) và Υ(G) ổn định đối với phép nhân với các vô hướng và đối với phép liên hợp.

Cho $\varrho_1$ và $\varrho_2$ là các biểu diễn unita của G; cho $(x_1, y_1)$ là các vectơ của không gian của $\varrho_1$ và $(x_2, y_2)$ là các vectơ của không gian của $\varrho_2$. Với mọi $g\in G$, khi đó ta có

$$
\langle x_1|\varrho_1(g)y_1\rangle +\langle x_2|\varrho_2(g)y_2\rangle =\langle (x_1, x_2)|(\varrho_1\oplus \varrho_2)(g)(y_1, y_2)\rangle
$$

$$
\langle x_1|\varrho_1(g)y_1\rangle \langle x_2|\varrho_2(g)y_2\rangle =\langle x_1\otimes x_2|(\varrho_1\otimes \varrho_2)(g)(y_1\otimes y_2)\rangle
$$

điều này chứng minh rằng Θ(G) và Υ(G) ổn định đối với phép cộng và phép nhân. Mệnh đề được suy ra.

### 8. Bổ đề Schur

Trong Số này, các không gian Hilbert là phức.

#### Mệnh đề 6 (Bổ đề Schur) {#ts-v-s1-prop-6 .statement tag=0395}

Cho $\varrho$ là một biểu diễn unita của một nhóm tôpô G trong một không gian Hilbert khác không E. Khi đó $\varrho$ là bất khả quy khi và chỉ khi Hom$_G(\varrho , \varrho )$ là bằng $\mathbf{C}\cdot 1_E$.

Không gian Hom$_G(\varrho , \varrho )$ là một đại số con sao có đơn vị của $\mathscr{L}(E)$ (bổ đề 5 của V, p. 380). Với mọi biểu diễn con F của E, phép chiếu trực giao $p$ có ảnh F là một phần tử lũy đẳng của đại số sao Hom$_G(\varrho , \varrho )$ (mệnh đề 4 của V, p. 383). Nếu đại số sau bằng $\mathbf{C}\cdot 1_E$, điều này có nghĩa là $p= 0$ hoặc $p= 1_E$, nghĩa là F = 0 hoặc F = E. Do đó $\varrho$ là bất khả quy.

Ngược lại, giả sử $\varrho$ bất khả quy. Cho $u$ và $v$ là các phần tử giao hoán được của đại số sao Hom$_G(\varrho , \varrho )$ sao cho $uv= 0$. Giả sử $u$ khác không. Khi đó hạt nhân F của $u$ xác định một biểu diễn con của $\varrho$ khác E, do đó F được rút gọn về 0; vì F chứa ảnh của $v$, suy ra $v= 0$. Theo mệnh đề 10 của I, p. 113, do đó ta có Hom$_G(\varrho , \varrho ) =\mathbf{C}\cdot 1_E$.

#### Hệ quả 1 {#ts-v-s1-prop-6-cor-1 .statement tag=0396}

Cho $\pi$ là một biểu diễn unita bất khả quy của một nhóm tôpô G trong một không gian Hilbert E. Cho $u$ là một toán tử bộ phận đóng trên E. Giả sử rằng $u$ có miền xác định trù mật, rằng dom($u$) ổn định dưới $\pi$ và rằng $u\circ \pi (g) =\pi (g)\circ u$ với mọi $g\in G$. Khi đó dom($u$) $= E$ và $u$ là một phép vị tự.

Toán tử bộ phận $u^*\circ u$ là một toán tử bộ phận tự liên hợp dương trên E (Mệnh đề 12 của IV, p. 241); điều tương tự đúng với $v= 1_E+u^*\circ u$, và toán tử sau là đơn ánh vì $-1\notin$ Sp($u^*\circ u$) (Mệnh đề 17 của IV, p. 248). Ta có $u^*\circ \pi (g) =\pi (g)\circ u^*$ với mọi $g\in G$ (Bổ đề 6 của V, p. 381), do đó $v\circ \pi (g) =\pi (g)\circ v$ với mọi $g\in G$. Vì $v$ là đơn ánh, suy ra rằng $v^{-1}\circ \pi (g) =\pi (g)\circ v^{-1}$ với mọi $g\in G$. Nhưng $v^{-1}$ thuộc về $\mathscr{L}$ (E), do đó theo Mệnh đề 6 tồn tại $\lambda \in \mathbf{C}$ sao cho $v^{-1}=\lambda 1_E$. Tất nhiên $\lambda \not = 0$, điều này suy ra rằng E = Im($v^{-1}$) $=$ dom($v$)$\subset$ dom($u$), do đó dom($u$) $= E$. Vì $u$ đóng, ta có $u\in \mathscr{L}(E)$ (TVS, I, p. 19, Hệ quả 5), do đó $u\in$ Hom$_G(\pi , \pi )$ và $u$ là một phép vị tự theo Mệnh đề 6.

#### Hệ quả 2 {#ts-v-s1-prop-6-cor-2 .statement tag=0397}

Cho $\varrho$ và $\pi$ là các biểu diễn unita bất khả quy của một nhóm tôpô G trong các không gian Hilbert E và F tương ứng. Không gian Hom$_G(\varrho , \pi )$ có chiều 1 nếu $\varrho$ đẳng cấu với $\pi$, và bằng không trong trường hợp ngược lại. Đặc biệt, nếu $\varrho$ đẳng cấu với $\pi$, mọi cấu xạ G khác không từ $\varrho$ vào $\pi$ đều là một đẳng cấu.

Giả sử tồn tại một cấu xạ G khác không $u$ từ $\varrho$ vào $\pi$. Ánh xạ tuyến tính $u^*\circ u$ là một phần tử của Hom$_G(\varrho , \varrho )$, do đó tồn tại một số phức $\lambda$ sao cho $u^*\circ u=\lambda \cdot 1_E$ (Mệnh đề 6). Khi đó ta có

$$
\langle u(x)|u(y)\rangle =\langle x|u^*u(y)\rangle =\lambda \langle x|y\rangle
$$

với mọi $x$ và $y$ trong E. Đặc biệt, $\lambda \not = 0$ vì $u$ là khác không. Vì $|u(x)|=|\lambda |^{1/2}|x|$ với mọi $x\in E$, ánh xạ tuyến tính $u$ là đơn ánh, và ảnh của $u$ là đóng trong F (Bổ đề 8 của I, p. 107); do đó nó là một biểu diễn con khác không của biểu diễn bất khả quy $\pi$, do đó suy ra rằng $u$ là toàn ánh. Vậy $u$ là một đẳng cấu của $\varrho$ lên $\pi$. Ánh xạ $v\mapsto u^*\circ v$ khi đó là một đẳng cấu của không gian Hom$_G(\varrho , \pi )$ lên không gian Hom$_G(\varrho , \varrho )$, có chiều 1 (Mệnh đề 6).

#### Hệ quả 3 {#ts-v-s1-prop-6-cor-3 .statement tag=0398}

Cho $\varrho$ là một biểu diễn unita của một nhóm tôpô G trong một không gian Hilbert E. Biểu diễn $\varrho$ là bất khả quy khi và chỉ khi không gian Sesq$_G(\varrho , \varrho )$ có chiều 1. Khi đó không gian này được sinh bởi tích vô hướng trên E.

Theo Mệnh đề 1 của V, p. 381, điều này suy ra từ Mệnh đề 6.

#### Hệ quả 4 {#ts-v-s1-prop-6-cor-4 .statement tag=0399}

Cho $\varrho_1$ và $\varrho_2$ là các biểu diễn unita bất khả quy không đẳng cấu của một nhóm tôpô G trong các không gian Hilbert $E_1$ và $E_2$. Không gian Sesq$_G(\varrho_1, \varrho_2)$ là không.

Theo Mệnh đề 1 của V, p. 381, điều này suy ra từ Hệ quả 2.

#### Hệ quả 5 {#ts-v-s1-prop-6-cor-5 .statement tag=039A}

Cho $\varrho$ là một biểu diễn unita của một nhóm tôpô G trong một không gian Hilbert E. Cho $\pi$ là một biểu diễn unita bất khả quy của G trong một không gian Hilbert F.

a) Với mọi cấu xạ G khác không $u$ của $\pi$ vào $\varrho$, tồn tại $\lambda \in \mathbf{R}^*_+$ sao cho $\lambda u$ là đẳng cự;

b) Mọi cấu xạ G $u$ của $\pi$ vào $\varrho$ đều có ảnh đóng;

c) Mọi cấu xạ G khác không $v$ của $\varrho$ vào $\pi$ đều là toàn ánh.

Ta chứng minh mệnh đề a), mệnh đề này kéo theo mệnh đề b) (Bổ đề 8 của I, p. 107). Vì cấu xạ $u$ là khác không, nó là đơn ánh (Bổ đề 2 của V, p. 378). Công thức $q(x, y) =\langle u(x)|u(y)\rangle$ với $x$ và $y$ trong F khi đó xác định một dạng song tuyến tính sesqui liên tục trên F. Vì $u$ là một cấu xạ G, ta có $q(\pi (g)x, \pi (g)y) =q(x, y)$ với mọi $g$ trong G và $(x, y)\in F\times F$, do đó $q$ là G-bất biến. Theo Hệ quả 3, tồn tại $\alpha \in \mathbf{R}^*_+$ sao cho

q(x,y)=⟨u(x)∣u(y)⟩=α⟨x∣y⟩

với mọi $(x, y)\in F\times F$, và do đó $\alpha^{-1/2}u$ là đẳng cự.

Cuối cùng ta chứng minh mệnh đề c). Vì $\pi$ là bất khả quy, ảnh của $v$ là trù mật trong F (Bổ đề 2 của V, p. 378), do đó ánh xạ đối phụ hợp $v^*$ là đơn ánh (TVS, V, p. 41, Mệnh đề 4). Theo b), ảnh H của $v^*$ là một không gian con đóng của E; do đó nó là một biểu diễn con của $\varrho$, và $v^*$ cảm sinh qua phép chuyển qua các không gian con một G-đẳng cấu của F lên H. Hạn chế $w$ của $v$ trên H xác định một G-cấu xạ từ H vào F, là đơn ánh vì hạt nhân của nó là giao của H và Ker($v$) $= H^{\circ}$ (loc. cit.). Ánh xạ $w$ do đó là một đẳng cấu (Hệ quả 2); đặc biệt, $v$ là toàn ánh.

#### Hệ quả 6 {#ts-v-s1-prop-6-cor-6 .statement tag=039B}

Cho $G_1$ và $G_2$ là các nhóm tôpô. Cho $\varrho_1$ là một biểu diễn unita bất khả quy của $G_1$ trong một không gian Hilbert $E_1$ và $\varrho_2$ là một biểu diễn unita bất khả quy của $G_2$ trong một không gian Hilbert $E_2$. Tích tenxơ ngoài $\varrho_1\boxtimes \varrho_2$ là một biểu diễn unita bất khả quy của $G_1\times G_2$ trong $E_1\widehat{\otimes}_2E_2$.

Tích tenxơ ngoài $\varrho =\varrho_1\boxtimes \varrho_2$ là một biểu diễn unita của $G = G_1\times G_2$ trong không gian $E = E_1\widehat{\otimes}_2E_2$ theo Bổ đề 8 của V, p. 384.

Cho $q$ là một dạng sesquilinear $(G_1\times G_2$)-bất biến trên E. Với mọi cặp $(x_1, y_1)\in E^2_1$, ánh xạ $(x_2, y_2)\mapsto q(x_1\otimes x_2, y_1\otimes y_2)$ thuộc về Sesq$_{G_2}(\varrho_2, \varrho_2)$. Ta ký hiệu bởi $b(x_1, y_1)$ số phức duy nhất sao cho

$$
q(x_1\otimes x_2, y_1\otimes y_2) =b(x_1, y_1)\langle x_2|y_2\rangle
$$

với mọi $(x_2, y_2)\in E^2_2$ (Hệ quả 3). Cho $\varepsilon \in E_2$ có chuẩn 1, sao cho $b(x_1, y_1) =q(x_1\otimes \varepsilon , y_1\otimes \varepsilon )$ với mọi $(x_1, y_1)\in E^2_1$. Công thức này suy ra rằng ánh xạ $b$ là sesquilinear trên $E_1$. Hơn nữa

$$
\|b(x_1, y_1)\|\leqslant \|q\| \|x_1\otimes \varepsilon \| \|y_1\otimes \varepsilon \|=\|q\| \|x_1\| \|y_1\|
$$

với mọi $(x_1, y_1)\in E^2_1$ (TVS, V, p. 26, công thức (5)), do đó $b$ là liên tục.

Cho $g\in G$ và $(x_1, y_1)\in E^2_1$. Vì $\varrho_2$ là unita và $q$ là bất biến, ta có

$$
b(\varrho_1(g)x_1, \varrho_1(g)y_1) =q(x_1\otimes \varrho_2(g^{-1})\varepsilon , y_1\otimes \varrho_2(g^{-1})\varepsilon ) =b(x_1, y_1)
$$

suy ra $b\in$ Sesq$_{G_1}(\varrho_1, \varrho_1)$. Do đó tồn tại một $\lambda \in \mathbf{C}$ duy nhất sao cho $b(x_1, y_1) =\lambda \langle x_1|y_1\rangle$ với mọi $(x_1, y_1)\in E^2_1$ (Hệ quả 3), nghĩa là

$$
q(x_1\otimes x_2, y_1\otimes y_2) =\lambda \langle x_1|y_1\rangle \langle x_2|y_2\rangle
$$

với mọi $(x_1, y_1, x_2, y_2)\in E^2_1\times E^2_2$. Suy ra rằng không gian Sesq$_{G_1\times G_2}(\varrho , \varrho )$ có chiều 1, điều này kéo theo rằng biểu diễn $\varrho =\varrho_1\boxtimes \varrho_2$ là bất khả quy (loc. cit.).

Ta nhắc lại rằng $\mathbf{U}$ ký hiệu nhóm các số phức có môđun bằng 1.

#### Hệ quả 7 {#ts-v-s1-prop-6-cor-7 .statement tag=039C}

Cho $\pi$ là một biểu diễn unita bất khả quy của một nhóm tôpô G trong một không gian Hilbert E. Tồn tại một đồng cấu liên tục $\chi$ của tâm C của G vào $\mathbf{U}$ sao cho $\pi (z) =\chi (z)\cdot 1_E$ với mọi $z\in C$. Đặc biệt, nếu G giao hoán, ta có dim(E) = 1.

Với $z\in C$, ánh xạ $\pi (z)$ thuộc Hom$_G(\pi , \pi )$; do đó nó có dạng $\chi (z)\cdot 1_E$ với một số phức $\chi (z)$ nào đó (mệnh đề 6). Vì $\pi (z)$ là một ánh xạ unita, ta có $|\chi (z)|= 1$. Hơn nữa, vì $\pi$ là một đồng cấu, ánh xạ $z\mapsto \chi (z)$ là một đồng cấu. Ta cố định $v\not = 0$ trong E; ánh xạ $z\mapsto \chi (z)v=\pi (z)v$ của C vào $\mathbf{U}$ là liên tục, và do đó đồng cấu $\chi$ là liên tục.

Cuối cùng, nếu G giao hoán, ta có C = G, do đó $\pi (g) =\chi (g)\cdot 1_E$ với mọi $g$ trong G; mọi không gian con chiều 1 của E khi đó là một biểu diễn con của $\pi$, và vì $\pi$ là bất khả quy, không gian E phải có chiều 1.

#### Định nghĩa 6 {#ts-v-s1-def-6 .statement tag=039D}

Cho $\pi$ là một biểu diễn unita bất khả quy của một nhóm tôpô G trong một không gian Hilbert E. Đồng cấu $\chi$ của tâm C của G vào $\mathbf{U}$ sao cho $\pi (z) =\chi (z)\cdot 1_E$ với mọi $z$ trong C được gọi là đặc trưng trung tâm của $\pi$.

#### Nhận xét {#ts-v-s1-n8-rem-1 .statement tag=039E}

Cho $\pi$ (tương ứng. $\varrho$ ) là một biểu diễn unita bất khả quy của một nhóm tôpô G (tương ứng. H) trong một không gian Hilbert E (tương ứng. F). Gọi $\chi$ (tương ứng. $\eta$ ) là đặc trưng trung tâm của $\pi$ (tương ứng. $\varrho$ ). Đặc trưng trung tâm của biểu diễn $\overline{\pi}$ là $\overline{\chi}$, và đặc trưng trung tâm của biểu diễn unita bất khả quy $\pi \boxtimes \varrho$ của $G\times H$ (hệ quả 6) là đặc trưng $\chi \boxtimes \eta : (g, h)\mapsto \chi (g)\eta (h)$ của $G\times H$.

### 9. Tính nửa đơn

#### Định nghĩa 7 {#ts-v-s1-def-7 .statement tag=039F}

Cho $\varrho$ là một biểu diễn unita của một nhóm tôpô G trong một không gian Hilbert E. Ta nói rằng $\varrho$ là nửa đơn nếu tồn tại một họ $(F_i)_{i\in I}$ các biểu diễn con bất khả quy của $\varrho$ sao cho E là tổng Hilbert của các không gian con $F_i$.

Đôi khi người ta cũng nói rằng một biểu diễn unita nửa đơn có một phân tích rời rạc hoặc là phân tích được một cách rời rạc.

Nếu $(\varrho_i)_{i\in I}$ là một họ các biểu diễn unita nửa đơn của một nhóm tôpô G, thì tổng Hilbert của các biểu diễn $\varrho_i$ là nửa đơn.

#### Mệnh đề 7 {#ts-v-s1-prop-7 .statement tag=039G}

Cho G là một nhóm tôpô và cho $\varrho$ là một biểu diễn unita của G trong một không gian Hilbert phức E. Biểu diễn $\varrho$ là nửa đơn khi và chỉ khi mọi biểu diễn con khác không của $\varrho$ chứa một biểu diễn con bất khả quy.

Giả sử rằng $\varrho$ là nửa đơn. Cho $(F_i)_{i\in I}$ là một họ các biểu diễn con bất khả quy của $\varrho$ sao cho E là tổng Hilbert của các không gian con $F_i$. Cho F là một biểu diễn con khác không của E. Tồn tại $i\in I$ sao cho hạn chế vào F của phép chiếu trực giao có ảnh $F_i$ là khác không. Phép chiếu trực giao này khi đó xác định bằng cách chuyển qua các không gian con một cấu xạ G khác không $p_i$ từ F vào $F_i$ (Mệnh đề 4 của V, p. 383). Theo Bổ đề Schur, cấu xạ G $p_i$ là toàn ánh (Hệ quả 5 của V, p. 388). Phần bù trực giao trong F của hạt nhân của $p_i$ là một biểu diễn con của F đẳng cấu với $F_i$ (Mệnh đề 3 của V, p. 383), do đó bất khả quy.

Ta hãy chứng minh mệnh đề đảo lại. Cho $\mathscr{F}$ là tập hợp các không gian con đóng F của E ổn định dưới G sao cho biểu diễn con của $\varrho$ trong F là bất khả quy. Cho $\mathscr{O}$ là tập hợp các tập con $\mathscr{G}$ của $\mathscr{F}$ sao cho các không gian con thuộc $\mathscr{G}$ trực giao từng đôi một.

Tập hợp $\mathscr{O}$ có đặc trưng hữu hạn (E, III, p. 34, Định nghĩa 2). Khi đó cho $\mathscr{G}$ là một phần tử cực đại của $\mathscr{O}$ (E, III, p. 35, Định lý 1). Cho $E_1$ là không gian con của E là tổng Hilbert của các biểu diễn con bất khả quy F của $\mathscr{G}$. Nếu có $E_1\not = E$, phần bù trực giao của $E_1$ sẽ khác không, và biểu diễn con của G trong $E^{\circ}_1$ sẽ chứa theo giả thiết một biểu diễn con bất khả quy. Không gian F của biểu diễn sau sẽ trực giao với các phần tử của $\mathscr{G}$, do đó $\mathscr{G}\cup  \{F\} \in \mathscr{O}$; điều này mâu thuẫn với tính cực đại của $\mathscr{G}$, vậy $E = E_1$, điều này hoàn thành chứng minh.

#### Hệ quả 1 {#ts-v-s1-prop-7-cor-1 .statement tag=039H}

Cho G là một nhóm tôpô và cho $\varrho$ là một biểu diễn unita nửa đơn của G trong một không gian Hilbert phức E. Mọi biểu diễn con của $\varrho ($resp. mọi biểu diễn thương của $\varrho )$ đều nửa đơn.

Nếu $\varrho_1$ là một biểu diễn con của $\varrho$, thì mọi biểu diễn con khác không của $\varrho_1$ chứa một biểu diễn con bất khả quy (Mệnh đề 7), do đó $\varrho_1$ là nửa đơn (loc. cit.).

Theo Mệnh đề 3 của V, p. 383, mọi biểu diễn thương của $\varrho$ đẳng cấu với một biểu diễn con của $\varrho$, do đó là nửa đơn.

#### Hệ quả 2 {#ts-v-s1-prop-7-cor-2 .statement tag=039I}

Mọi biểu diễn unita hữu hạn chiều $\varrho$ của một nhóm tôpô G đều nửa đơn.

Điều này suy ra từ Mệnh đề 7 và Bổ đề 3 của V, p. 379.

#### Hệ quả 3 {#ts-v-s1-prop-7-cor-3 .statement tag=039J}

Cho $\varrho_1$ và $\varrho_2$ là các biểu diễn unita hữu hạn chiều của một nhóm tôpô G. Các biểu diễn $\varrho_1$ và $\varrho_2$ đẳng cấu khi và chỉ khi $\chi_{\varrho_1}=\chi_{\varrho_2}$.

Điều này suy ra từ Hệ quả 2 và A, VIII, p. 389, Mệnh đề 1, b).

### 10. Các lớp của các biểu diễn unita

#### Bổ đề 9 {#ts-v-s1-lem-9 .statement tag=039K}

Cho E là một không gian Hilbert trên K. Cho $F\subset E$ là một không gian vectơ con trù mật trong E. Khi đó chiều Hilbert của E nhỏ hơn hoặc bằng chiều của F.

Nếu E có chiều Hilbert hữu hạn, điều này bằng chiều của E. Giả sử rằng E có chiều Hilbert vô hạn. Khi đó không gian con F có chiều vô hạn. Cho B là một cơ sở trực chuẩn của E và cho $B'$ là một cơ sở của F. Với mọi $x\in B$, tồn tại một phần tử $f(x)\in B'$ sao cho $\langle x|f(x)\rangle  \not = 0$, vì nếu không thì sẽ có $x\in F^{\circ}=\{0\}$. Do đó ta xác định một ánh xạ $f: B\rightarrow B'$.

Với mọi $y\in B'$, tập hợp $\overset{-1}{f}(y)$ được chứa trong tập hợp các $x\in B$ sao cho $\langle x|y\rangle  \not = 0$, do đó là đếm được (EVT, V, p. 21, Mệnh đề 4). Theo E, III, p. 50, Mệnh đề 4, ta thu được Card(B) = Card($f(B)$)$\leqslant$ Card(B$'$).

Ta ký hiệu bởi $Is_G(\pi_1, \pi_2)$ quan hệ

“G là một nhóm tôpô và $\pi_1,\pi_2$ là các biểu diễn unita đẳng cấu

của G trong các không gian Hilbert trên K”.

Với $\pi_1$ và $\pi_2$, đây là một quan hệ tương đương. Với mọi biểu diễn unita $\pi$ của G trong một không gian Hilbert trên K, ta ký hiệu cl($\pi$ ) là lớp tương đương của $\pi ($cf. E, II, p. 47); do đó nó là một biểu diễn unita của G đẳng cấu với $\pi$; người ta nói rằng cl($\pi$ ) là lớp của $\pi$. Hai biểu diễn unita $\pi_1$ và $\pi_2$ trong các không gian Hilbert trên K là đẳng cấu khi và chỉ khi cl($\pi_1$) $=$ cl($\pi_2$).

Cho G là một nhóm tôpô. Cho $\mathfrak{c}$ là một lực lượng. Quan hệ

" $\lambda$ là một lớp của biểu diễn unita của G trong

một không gian Hilbert phức có chiều Hilbert $\leqslant \mathfrak{c}$ "

là xác định tập theo $\lambda$ (E, II, p. 3). Thật vậy, mọi không gian Hilbert trên K có chiều $\leqslant \mathfrak{c}$ đều đẳng cấu đẳng cự với một không gian con Hilbert của $\ell^2(\mathfrak{c})$ (EVT, V, p. 23, cor. 2), và mệnh đề này suy ra từ E, II, p. 47.

Cho $\pi$ là một biểu diễn unita bất khả quy của G trong một không gian Hilbert E. Cho $x$ là một phần tử khác không của E. Vì $\pi$ là bất khả quy, vectơ $x$ là một vectơ chu kỳ của $\pi$, điều này kéo theo rằng chiều Hilbert của E là $\leqslant$ Card(G) (bổ đề 9, áp dụng cho không gian con trù mật sinh bởi các phần tử $\pi (g)x$ với $g\in G$). Các lớp của các biểu diễn unita bất khả quy của G trong một không gian Hilbert trên K do đó thuộc về tập hợp các lớp của các biểu diễn unita của G trong một không gian Hilbert trên K có chiều Hilbert $\leqslant$ Card(G) ; do đó, chúng tạo thành một tập hợp.

#### Định nghĩa 8 {#ts-v-s1-def-8 .statement tag=039L}

Ta ký hiệu bởi $\widehat{G}$ tập hợp các lớp của các biểu diễn unita bất khả quy của G trong một không gian Hilbert phức. Người ta nói rằng $\widehat{G}$ là đối ngẫu unita của G.

Với mọi biểu diễn unita bất khả quy $\pi$ của G trong một không gian Hilbert phức, do đó ta có cl($\pi$ )$\in \widehat{G}$.

#### Nhận xét 1 {#ts-v-s1-n10-rem-1 .statement tag=039M}

Giả sử rằng G là một nhóm giao hoán. Theo hệ quả 7 của V, p. 390, mọi biểu diễn unita bất khả quy của G trong một không gian Hilbert phức đều có chiều 1. Nếu G là compact địa phương, tập hợp $\widehat{G}$ được đồng nhất với tập hợp các đặc trưng unita của G (định nghĩa 1 của II, p. 201), và ký hiệu $\widehat{G}$ do đó tương thích với ký hiệu được đưa vào trong định nghĩa 2 của II, p. 201.

#### Nhận xét 2 {#ts-v-s1-n10-rem-2 .statement tag=039N}

Nếu G là hữu hạn, tập hợp $\widehat{G}$ song ánh với tập hợp các lớp của các $\mathbf{C}$[G]-môđun đơn (A, VIII, p. 47), tập hợp này cũng được ký hiệu bởi $\widehat{G}$ trong A, VIII, p. 396.

#### Nhận xét 3 {#ts-v-s1-n10-rem-3 .statement tag=039O}

Với $\pi \in \widehat{G}$, ta sẽ đồng nhất $\overline{\pi}$ với lớp trong $\widehat{G}$ của biểu diễn liên hợp của $\pi$.

#### Nhận xét 4 {#ts-v-s1-n10-rem-4 .statement tag=039P}

Nếu $\pi$ là một biểu diễn unita bất khả quy của G trong một không gian Hilbert phức hữu hạn chiều, đặc trưng $\chi_{\pi}$ của nó chỉ phụ thuộc vào lớp của $\pi$. Do đó người ta có thể nói về tập hợp các đặc trưng của các biểu diễn unita bất khả quy phức hữu hạn chiều của G.

### 11. Các thành phần đẳng kiểu

#### Định nghĩa 9 {#ts-v-s1-def-9 .statement tag=039Q}

Cho G là một nhóm tôpô và cho $\pi$ là một biểu diễn liên tục của G. Cho $\varrho$ là một biểu diễn liên tục của G trong một không gian lồi địa phương tách E. Thành phần $\pi$-đẳng kiểu của $\varrho$ là bao đóng trong E của tổng các không gian của tất cả các biểu diễn con của $\varrho$ đẳng cấu với $\pi$. Không gian con này được ký hiệu bởi $M_{\pi}(\varrho )$.

Không gian $M_{\pi}(\varrho )$ là một không gian con đóng của E, xác định một biểu diễn con của $\varrho$. Không gian này chỉ phụ thuộc vào lớp của $\pi$ trong $\widehat{G}$.

#### Mệnh đề 8 {#ts-v-s1-prop-8 .statement tag=039R}

Cho G là một nhóm tôpô. Cho $\varrho$ là một biểu diễn unita của G trong một không gian Hilbert phức E.

a) Cho $\pi_1$ và $\pi_2$ là các biểu diễn unita bất khả quy không đẳng cấu của G. Các không gian con $M_{\pi_1}(\varrho )$ và $M_{\pi_2}(\varrho )$ trực giao;

b) Cho $\varrho '$ là một biểu diễn unita của G và $u$ là một cấu xạ G của $\varrho$ vào $\varrho '$. Với mọi biểu diễn unita bất khả quy $\pi$ của G, ta có $u(M_{\pi}(\varrho ))\subset M_{\pi}(\varrho ')$.

Cho $E_1$ và $E_2$ là các không gian con của E xác định các biểu diễn con đẳng cấu với $\pi_1$ và $\pi_2$ tương ứng. Phép chiếu trực giao của E có ảnh $E_2$ xác định, bằng cách chuyển qua các không gian con, một phần tử của Hom$_G(\pi_1, \pi_2)$, bằng không (Hệ quả 2 của V, p. 387), và điều này chứng minh rằng $E_2$ trực giao với $E_1$. Điều này kéo theo mệnh đề a).

Đối với mệnh đề b), chú ý rằng $M_{\pi}(\varrho )$ theo định nghĩa là bao đóng trong E của không gian sinh bởi các phần tử $x\in E$ thuộc một không gian con đóng $F\subset E$ ổn định đối với $\varrho$ sao cho biểu diễn con $\varrho_F$ của $\varrho$ trong F đẳng cấu với $\pi$. Do đó chỉ cần chứng minh rằng, trong trường hợp này, ta có $u(x)\in M_{\pi}(\varrho ')$. Đặt $H =u(F)$; nó là một không gian con đóng của không gian của $\varrho '$ (Hệ quả 5 của V, p. 388) ổn định đối với $\varrho '$, và $u$ cảm sinh, bằng cách chuyển qua các không gian con, một cấu xạ G toàn ánh từ F lên H. Nếu H khác không, thì cấu xạ G này là một đẳng cấu theo Hệ quả 2 của V, p. 387. Biểu diễn của G trên H do đó đẳng cấu với $\pi$, do đó suy ra rằng $u(x)$ thuộc $M_{\pi}(\varrho ')$.

Với mọi không gian vectơ H và mọi họ $(H_i)_{i\in I}$ các không gian con của H, ta nói rằng các không gian $(H_i)_{i\in I}$ là tổng trực tiếp nếu họ $(H_i)_{i\in I}$ thỏa mãn các điều kiện tương đương của Mệnh đề 11 của A, II, p. 18.

#### Mệnh đề 9 {#ts-v-s1-prop-9 .statement tag=039S}

Cho G là một nhóm tôpô và cho $\varrho$ là một biểu diễn unita của G trong một không gian Hilbert phức E. Cho $\pi$ là một biểu diễn unita bất khả quy của G trong một không gian Hilbert phức $E_{\pi}$. Ký hiệu $v$ là ánh xạ tuyến tính từ Hom$_G(\pi , \varrho )\otimes E_{\pi}$ vào E sao cho $v(u\otimes x) =u(x)$ với mọi $(u, x)\in$ Hom$_G(\pi , \varrho )\times E_{\pi}$.

Ánh xạ tuyến tính $v$ là đơn ánh, và ảnh của nó là tổng của các không gian của tất cả các biểu diễn con của $\varrho$ đẳng cấu với $\pi$. Đặc biệt, ảnh của $v$ là trù mật trong $M_{\pi}(\varrho )$.

Hệ quả 5 của V, p. 388 suy ra rằng ảnh của $v$ là tổng của các không gian của tất cả các biểu diễn con của $\varrho$ đẳng cấu với $\pi$.

Ta hãy chứng minh rằng $v$ là đơn ánh. Cho $(u_i)_{i\in I}$ là một cơ sở của không gian vectơ Hom$_G(\pi , \varrho )$. Với $i\in I$, ký hiệu $F_i$ là ảnh của $u_i$ và $\widetilde{u}_i: E_{\pi}\rightarrow F_i$ là đẳng cấu G suy ra từ $u_i$ bằng cách chuyển qua các không gian con.

Trước hết ta chứng minh, bằng quy nạp theo lực lượng của một tập con hữu hạn J của I, rằng các không gian con $(F_i)_{i\in J}$ nằm trong tổng trực tiếp.

Trường hợp J rỗng là ngay lập tức. Giả sử rằng J khác rỗng và tính chất cần chứng minh đúng đối với các tập con của I có lực lượng nhiều nhất là Card(J) $-1$.

Cho $j$ là một phần tử cố định của J. Giả thiết quy nạp suy ra rằng các không gian con $F_i$ với $i\in J-\{j\}$ nằm trong tổng trực tiếp. Gọi $F'$ là tổng của chúng; bây giờ còn phải chứng minh rằng $F_j\cap F'=\{0\}$.

Giả sử giao của $F_j$ và $F'$ không thu gọn về 0; giao này là một biểu diễn con của $F_j$, và vì không gian sau là bất khả quy, do đó ta có $F_j\cap F'= F_j$, do đó $F_j\subset F'$.

Với $i\in J-\{j\}$, ký hiệu pr$_i: F'\rightarrow F_i$ là phép chiếu và $\iota_i: F_i\rightarrow F'$ là phép nhúng. Ta có một đẳng cấu chính tắc

Hom$_G(F_j,F')\rightarrow \bigoplus_{i\in J-\{j\}}$ Hom$_G(F_j,F_i)$

(công thức (1), p. 377) sao cho $u: F_j\rightarrow F'$ có ảnh là họ (pr$_i\circ u$)$_{i\in J-\{j\}}$ (A, II, p. 13, hệ quả 1). Hệ quả 2 của V, p. 387 suy ra rằng $\widetilde{u}_i\circ \widetilde{u}^{-1}_j$, là khác không, là một cơ sở của không gian Hom$_G(F_j,F_i)$. Do đó, họ các G-đồng cấu $(\iota_i\circ \widetilde{u}_i\circ \widetilde{u}^{-1}_j)_{i\in J-\{j\}}$ là một cơ sở của Hom$_G(F_j,F')$.

Ký hiệu $\iota$ là phép nhúng của $F_j$ vào $F'$; nó là một phần tử của Hom$_G(F_j,F')$, do đó nó là một tổ hợp tuyến tính của các G-đồng cấu $\iota_i\circ \widetilde{u}_i\circ \widetilde{u}^{-1}_j$ với $i\in J-\{j\}$. Suy ra rằng $u_j$ là một tổ hợp tuyến tính của các ánh xạ $u_i$ với $i\not =j$, điều này mâu thuẫn với tính độc lập tuyến tính của họ $(u_i)_{i\in I}$. Mệnh đề này do đó được chứng minh bằng quy nạp.

Bây giờ ta chứng minh rằng $v$ là đơn ánh. Cho $w$ là một phần tử của Hom$_G(\pi , \varrho )\otimes E_{\pi}$. Có một họ duy nhất $(x_i)_{i\in I}$ trong $E_{\pi}$ có giá hữu hạn sao cho

$$
w=\sum_{i\in I}u_i\otimes x_i
$$

(A, II, p. 62, hệ quả 1) và khi đó ta có

$$
v(w) =\sum_{i\in I}u_i(x_i)
$$

Từ những điều trên, điều kiện $v(w) = 0$ do đó suy ra rằng $u_i(x_i) = 0$ với mọi $i\in I$, do đó $x_i= 0$ với mọi $i$ vì $u_i$ là đơn ánh, và vì vậy $w= 0$.

#### Mệnh đề 10 {#ts-v-s1-prop-10 .statement tag=039T}

Cho G là một nhóm tôpô. Cho $\pi$ là một biểu diễn unita bất khả quy của G trong một không gian Hilbert phức $E_{\pi}$ và cho $\varrho$ là một biểu diễn unita của G trong một không gian Hilbert phức E.

Tồn tại các họ $(E_i)_{i\in I}$ gồm các không gian con bất biến đóng của E sao cho biểu diễn con của $\varrho$ trong $E_i$ là đẳng cấu với $\pi$ với mọi $i\in I$ và sao cho $M_{\pi}(\varrho )$ là tổng Hilbert của các không gian $E_i$. Hơn nữa, lực lượng của I là độc lập với họ $(E_i)_{i\in I}$ thỏa mãn các tính chất này.

Hãy chứng minh sự tồn tại của các họ thỏa mãn các điều kiện đã chỉ ra. Gọi $\mathscr{O}$ là tập hợp các tập con C của Hom$_G(\pi , \varrho )-\{0\}$ sao cho các không gian con $u(E_{\pi})$ với $u\in C$ trực giao từng đôi một. Tập hợp $\mathscr{O}$ có thứ tự bởi quan hệ bao hàm. Nó khác rỗng vì tập rỗng là một phần tử, và nó có đặc trưng hữu hạn (E, III, p. 34, Định nghĩa 2) vì C thuộc $\mathscr{O}$ khi và chỉ khi các tập chứa hai phần tử của C thuộc $\mathscr{O}$. Theo E, III, p. 35, Định lý 1, tồn tại một phần tử cực đại C của $\mathscr{O}$. Gọi F là bao đóng của không gian con sinh bởi các không gian $u(E_{\pi})$ với $u\in C$; nó là tổng Hilbert của các không gian $u(E_{\pi})$ với $u\in C$. Ta sẽ chứng minh rằng $F = M_{\pi}(\varrho )$, điều này sẽ chứng minh rằng họ $(u(E_{\pi}))_{\pi\in C}$ có các tính chất yêu cầu.

Theo định nghĩa, $u(E_{\pi})\subset M_{\pi}(\varrho )$ với mọi $u\in C$, do đó F được chứa trong $M_{\pi}(\varrho )$. Để chứng minh bao hàm đảo lại, chỉ cần chứng minh rằng nếu $v$ là một G-cấu xạ từ $\pi$ vào $\varrho$, thì ảnh của nó được chứa trong F. Gọi $p$ là phép chiếu trực giao của E có ảnh $F^{\circ}$; nó là một G-cấu xạ, vì F là một biểu diễn con của E (Mệnh đề 4 của V, p. 383). Ảnh của G-cấu xạ $p\circ v$ trực giao với F; do đó nó bằng không (nếu không thì $C\cup  \{p\circ v\} \in \mathscr{O}$, điều này mâu thuẫn với tính cực đại của C), và do đó ảnh của $v$ được chứa trong F.

Bây giờ hãy cho $(E_i)_{i\in I}$ và $(F_j)_{j\in J})$ là các họ các không gian con đóng bất biến của E, trực giao từng đôi một, sao cho biểu diễn con của G trong $E_i$ (tương ứng trong $F_j$) là đẳng cấu với $\pi$ với mọi $i\in I$ (tương ứng với mọi $j\in J$), và sao cho $M_{\pi}(\varrho )$ là tổng Hilbert của họ $(E_i)_{i\in I}$ và của họ $(F_j)_{j\in J}$.

Nếu I là hữu hạn, thì

dim Hom$_G(\pi ,M_{\pi}(\varrho )) =$ dim Hom$_G(E_{\pi},\bigoplus_{i\in I}E_i)=$ Card(I)

(công thức (1) của V, p. 377 và Hệ quả 2 của V, p. 387). Với mọi tập con hữu hạn L của J, ta có

Card(L) = dim Hom$_G(E_{\pi},\bigoplus_{i\in L}F_j)$

$\leqslant$ dim Hom$_G(\pi ,M_{\pi}(\varrho )) =$ Card(I)

(loc. cit.). Điều này chứng minh rằng J khi đó là hữu hạn và rằng Card(I) = Card(J), như mong muốn. Tương tự, nếu J là hữu hạn, thì I là hữu hạn và có cùng lực lượng.

Giả sử bây giờ rằng I và J là vô hạn. Với $j\in J$, gọi $p_j$ là phép chiếu trực giao của E có ảnh $F_j$. Với $i\in I$, gọi $x_i$ là một phần tử khác không của $E_i$; nó là một vectơ chu kỳ của $E_i$. Nhận xét rằng vì $p_j$ cảm sinh qua phép chuyển qua các không gian con một G-cấu xạ từ $E_i$ vào $F_j$, không gian $p_j(E_i)$ bằng không khi và chỉ khi $p_j(x_i) = 0$ (thực vậy, không gian $E_i\cap$Ker($p_j$) hoặc là không, hoặc bằng $E_i$).

For every $j\in J$, tồn tại một phần tử $f(j)\in I$ sao cho $p_j(E_{f(j)})$ không thu gọn về 0 (nếu không, phép chiếu trực giao $p_j$ sẽ bằng không trên $M_{\pi}(\varrho )$). Do đó một ánh xạ $f$ từ J vào I đã được xác định. Đối với

$-1$

mọi $i\in I$, tập hợp $f(i)$ là đếm được. Thật vậy, tập hợp này được chứa trong tập hợp các $j\in J$ sao cho $p_j(E_i)$ khác không, tức là sao cho $p_j(x_i)\not = 0$. Bây giờ (EVT, V, p. 20, hệ quả 2), ta có

$$
\sum_{j\in J}\|p_j(x_i)\|^2=\|x_i\|^2
$$

do đó tập hợp các $j\in J$ sao cho $p_j(x_i)\not = 0$ là đếm được. Theo E, III, p. 50, mệnh đề 4, suy ra rằng Card(J) = Card($f(J)$)$\leqslant$ Card(I). Bằng cách đổi chỗ vai trò của I và J, ta kết luận rằng Card(I) = Card(J).

#### Hệ quả {#ts-v-s1-n11-cor-1 .statement tag=039U}

Cho G là một nhóm tôpô và $\varrho$ là một biểu diễn unita của G trong một không gian Hilbert phức E. Tổng Hilbert của các thành phần đẳng kiểu $\pi$ của G đối với $\pi \in \widehat{G}$ là biểu diễn con nửa đơn lớn nhất của $\varrho$.

Thật vậy, các thành phần đẳng kiểu $\pi$ của G đối với $\pi \in \widehat{G}$ là trực giao từng đôi một (mệnh đề 8, a)), và mỗi thành phần là nửa đơn (mệnh đề 10, a)); do đó tổng Hilbert F của các không gian $M_{\pi}(\varrho )$ đối với $\pi \in \widehat{G}$ xác định một biểu diễn con nửa đơn của $\varrho$. Hơn nữa, vì mọi biểu diễn con bất khả quy của $\varrho$ đều là một biểu diễn con của một thành phần đẳng kiểu của $\varrho$, hệ quả được suy ra.

#### Định nghĩa 10 {#ts-v-s1-def-10 .statement tag=039V}

Cho G là một nhóm tôpô. Cho $\varrho$ là một biểu diễn unita của G trong một không gian Hilbert phức E và $\pi$ là một biểu diễn unita bất khả quy của G trong một không gian Hilbert phức.

**Bội số** của $\pi$ trong $\varrho$ được định nghĩa là lực lượng của tập hợp I đối với mọi họ $(E_i)_{i\in I}$ các không gian con đóng của E ổn định dưới G sao cho biểu diễn con của $\varrho$ cảm sinh trong $E_i$ là đẳng cấu với $\pi$ đối với mọi I và sao cho $M_{\pi}(\varrho )$ là tổng Hilbert của các không gian con $E_i$.

Nếu bội số của $\pi$ trong $\varrho$ là hữu hạn, thì nó bằng chiều của không gian Hom$_G(\pi , \varrho )$ (tương ứng bằng chiều của Hom$_G(\varrho , \pi )$) theo công thức (1) của V, p. 377 và hệ quả 2 của V, p. 387. Điều này nói chung không phải lúc nào cũng đúng.

#### Nhận xét {#ts-v-s1-n11-rem-1 .statement tag=039W}

Có thể xảy ra rằng một biểu diễn unita $\varrho$ khác không, nhưng tất cả các thành phần đẳng kiểu của $\varrho$ đối với tất cả các biểu diễn bất khả quy của G đều bằng không (xem V, p. 426, nhận xét).

## BÀI TẬP {#ts-v-s1-exercises}

Xem các [bài tập của § 1](exercises/s1/).
