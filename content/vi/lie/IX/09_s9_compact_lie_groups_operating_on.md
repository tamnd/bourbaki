---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IX
chapter_title: COMPACT REAL LIE GROUPS
section: 9
section_title: Compact Lie groups operating on manifolds
lang: vi
source: lie-vii-ix
book_pages: 369-381, 419-424
pdf_pages: 0376-0388, 0426-0431
extraction: native
subsections:
    - "no": 1
      title: EMBEDDING OF A MANIFOLD IN THE NEIGHBOURHOOD OF A COMPACT SET
      page: 369
      pdf_page: 376
    - "no": 2
      title: EQUIVARIANT EMBEDDING THEOREM
      page: 373
      pdf_page: 380
    - "no": 3
      title: TUBES AND TRANSVERSALS
      page: 375
      pdf_page: 382
    - "no": 4
      title: ORBIT TYPES
      page: 377
      pdf_page: 384
statements: 19
exercises: 21
errata:
    - says: §5, no. 2, Cor. of Prop. 2
      read: §5, no. 2, Cor. 1 of Prop. 2
      why: No. 2 of section 5 prints three numbered corollaries of Proposition 2 and the reference does not say which. The sentence citing it has G simply-connected and A an alcove, and says that the composite map from A to $G_r/$Int(G) is a homeomorphism. That is Corollary 1 b), whose homeomorphisms run $A/H_A$ to $T_r/W$ to $G_r/$Int(G) and whose $H_A$ is trivial for a simply-connected group. Corollary 2 is the same statement for the Lie algebra, over a chamber rather than an alcove, and Corollary 3 is about existence and uniqueness and names no map at all.
content_sha256: b9b976df2eab2351bd4474013c0db66fc16abc49f180ecfef1b343cdc1aebdce
translated_from: content/en/lie/IX/09_s9_compact_lie_groups_operating_on.md
source_content_sha256: dbd6a8fe77e36a2dde3d4d956d5fc6fd2a6bf284a5e6f34dca83531dabcebd7f
translation_model: gpt-5-6-mini, gpt-5-mini, gpt-5.4-mini
translation_run: translate-vi-79bcb0f4
glossary_version: 34
glossary_terms_sha256: b9ca2afa03f396c4168b4c28fdee4b4d7983e3ba259cadb3285bc9b99cd573d8
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 9. CÁC NHÓM LIE COMPACT TÁC ĐỘNG TRÊN CÁC ĐA TẠP

Trong đoạn này, X ký hiệu một đa tạp thực, tách được, hữu hạn chiều địa phương, thuộc lớp $C^r(1\leq r\leq \omega )$.

### 1. NHÚNG MỘT ĐA TẠP VÀO LÂN CẬN CỦA MỘT TẬP COMPACT

#### Bổ đề 1 {#lie-ix-s9-lem-1 .statement tag=01HE}

Cho T và $T'$ là hai không gian tôpô, A và $A'$ lần lượt là các tập con compact của T và $T'$, W là một lân cận của $A\times A'$ trong $T\times T'$. Tồn tại một lân cận mở U của A trong T và một lân cận mở $U'$ của $A'$ trong $T'$ sao cho $U\times U'\subset W$.

Cho $x\in A$; tồn tại các tập con mở $U_x$ của T và $U'_x$ của $T'$ sao cho $\{x\} \times A'\subset U_x\times U'_x\subset W:$ thật vậy, tập con compact $\{x\} \times A'$ của $T\times T'$ có thể được phủ bởi một số hữu hạn các tập mở chứa trong W, có dạng $U_i\times U'_i$, với $x\in U_i$; chỉ cần lấy $U_x=\bigcap_iU_i$ và $U'_x=\bigcup_iU'_i$.

Vì A compact, tồn tại các điểm $x_1, . . . , x_m$ của A sao cho $A\subset \bigcup_iU_{x_i}$; đặt $U =\bigcup_iU_{x_i}$ và $U'=\bigcap_iU'_{x_i}$. Khi đó $A\times A'\subset U\times U'\subset W$, do đó có bổ đề.

Trong phần còn lại của số này, Y ký hiệu một đa tạp tách được thuộc lớp $C^r$.

#### Mệnh đề 1 {#lie-ix-s9-prop-1 .statement tag=01HF}

Cho $\varphi : X\rightarrow Y$ là một cấu xạ thuộc lớp $C^r$, A là một tập con compact của X. Các điều kiện sau là tương đương:

(i) Hạn chế của $\varphi$ lên A là đơn ánh, và $\varphi$ là một phép nhúng tại mọi điểm của A;

(ii) tồn tại một lân cận mở U của A sao cho $\varphi$ cảm sinh một phép nhúng của U vào Y.

Khi các điều kiện này được thỏa mãn, $\varphi$ được gọi là một phép nhúng trong lân cận của A.

Ta chứng minh rằng (i) kéo theo (ii), chiều ngược lại là hiển nhiên. Giả sử (i), tồn tại một lân cận mở V của X chứa A sao cho hạn chế của $\varphi$ lên V là một phép nhúng (Differentiable and Analytic Manifolds, Results, 5.7.1). Ký hiệu $\Gamma$ là tập hợp các điểm $(x, y)$ trong $V\times V$ sao cho $\varphi (x) =\varphi (y)$, và ký hiệu $\Delta$ là đường chéo trong $V\times V$. Khi đó $\Delta$ là một tập con mở của $\Gamma :$ thật vậy, với mọi $x\in V$, tồn tại một lân cận mở $U_x$ của $x$ sao cho hạn chế của $\varphi$ lên $U_x$ là đơn ánh, nghĩa là, sao cho $\Gamma \cap (U_x\times U_x) =$ $\Delta \cap (U_x\times U_x)$.

Vì Y là tách được, $\Gamma$ là đóng trong $V\times V$; do đó phần bù W của $\Gamma$ **--** $\Delta$ trong $V\times V$ là mở. Theo giả thiết, W chứa $A\times A$; Bổ đề 1 suy ra rằng tồn tại một tập con mở $U'$ của V chứa A sao cho $U'\times U'\subset W$, nghĩa là sao cho hạn chế của $\varphi$ trên $U'$ là đơn ánh. Hơn nữa, tồn tại một lân cận mở U của A có bao đóng compact và được chứa trong $U'($Tôpô đại cương, Chương I, §9, no. 7, Mệnh đề 10). Khi đó $\varphi$ cảm sinh một đồng phôi từ U vào $\varphi$(U), và do đó từ U vào $\varphi (U)$; suy ra rằng hạn chế của $\varphi$ trên U là một phép nhúng (Đa tạp khả vi và giải tích, Kết quả, 5.8.3).

#### Mệnh đề 2 {#lie-ix-s9-prop-2 .statement tag=01HG}

Giả sử đa tạp Y là paracompact; cho A là một tập con của X, và cho $\varphi :X\rightarrow Y$ là một cấu xạ thuộc lớp $C^r$ cảm sinh một đồng phôi từ A vào $\varphi (A)$, và là étale tại mọi điểm của A. Khi đó tồn tại một lân cận mở U của A sao cho $\varphi$ cảm sinh một đẳng cấu từ U vào một đa tạp con mở của Y.

Nếu cần, hạn chế X và Y, ta có thể giả sử rằng $\varphi$ là étale và toàn ánh. Ký hiệu $\sigma :\varphi (A)\rightarrow A$ là đồng phôi nghịch đảo của $\varphi |A$. Vì Y là mêtric hóa được (Đa tạp khả vi và giải tích, Kết quả, 5.1.6), $\varphi (A)$ thừa nhận một hệ cơ bản các lân cận paracompact; do đó, theo Tôpô đại cương, Chương XI, tồn tại một lân cận mở V của $\varphi (A)$ trong Y và một ánh xạ liên tục $s: V\rightarrow X$, trùng với $\sigma$ trên $\varphi (A)$ và sao cho $\varphi (s(y)) =y$ với mọi $y\in V$. Hơn nữa, $s$ là étale theo tôpô, do đó $s(V)$ là một tập mở U chứa A. Khi đó $\varphi$ cảm sinh một đồng phôi $\varphi '$ từ U vào V; theo Đa tạp khả vi và giải tích, Kết quả$, 5.7.8,\varphi '$ là một đẳng cấu.

Trong phần còn lại của số này, ta giả sử rằng $r\not=\omega$.

#### Mệnh đề 3 {#lie-ix-s9-prop-3 .statement tag=01HH}

Cho A là một tập con compact của X. Tập hợp $\mathscr{P}$ các cấu xạ $\varphi \in \mathscr{C}^r(X;Y)$ là các phép nhúng trong một lân cận của A là mở trong $\mathscr{C}^r(X;Y)$ đối với tôpô hội tụ $C^r$ compact (§ 6, no. 4).

Rõ ràng, chỉ cần chứng minh mệnh đề với $r= 1$.

a) Trước hết ta chứng minh rằng tập con J của $\mathscr{C}^1(X;Y)$ gồm các cấu xạ là các phép dìm tại mọi điểm của A là mở. Xét ánh xạ $j_A:\mathscr{C}^1(X;Y)\times A\rightarrow J^1(X;Y)$ sao cho $j_A(\varphi , x) =j_x^1(\varphi ) ($Đa tạp khả vi và giải tích, Kết quả, 12.1).

Theo định nghĩa của tôpô trên $\mathscr{C}^1$(X;Y), ánh xạ $\widetilde{j}_A:\varphi \rightarrow j_A(\varphi , .)$ từ $\mathscr{C}^1(X;Y)$ vào $\mathscr{C}(A;J^1(X;Y))$ là liên tục; từ đó suy ra theo Tôpô đại cương, Chương X, §3, no. 4, Định lý 3, rằng $j_A$ là liên tục.

Mặt khác, cho M là tập hợp các mầm $j$ trong $J^1(X;Y)$ mà ánh xạ tiếp xúc $T(j) : T_{\mathbf{s}(j)}(X)\rightarrow T_{\mathbf{b}(j)}(Y) ($Đa tạp khả vi và giải tích, Kết quả, 12.3.4) là đơn ánh. Tập M là mở trong $J^1(X;Y)$; thực vậy, chỉ cần kiểm tra mệnh đề này khi X là một tập con mở của một không gian vectơ hữu hạn chiều E, và Y là một tập con mở của một không gian Banach F; khi đó ta quy về (Đa tạp khả vi và giải tích, Kết quả, 12.3.1) việc chứng minh rằng tập hợp các ánh xạ tuyến tính liên tục đơn ánh là mở trong $\mathscr{L}$(E;F), điều này suy ra từ Lý thuyết phổ, Chương III, §2, no. 7, Mệnh đề 16.

Ta kết luận từ điều đã nêu trước đó rằng tập hợp $j_A^{-1}(M)$ là mở trong $\mathscr{C}^1(X;Y)\times A$, do đó phần bù của nó $\mathscr{F}$ là đóng. Vì A là compact, phép chiếu pr$_1:\mathscr{C}^1(X;Y)\times A\rightarrow \mathscr{C}^1(X;Y)$ là một cấu xạ thực sự, do đó đóng; vì vậy, tập hợp J, bằng $\mathscr{C}^1(X;Y)$ **--** pr$_1(\mathscr{F})$, là mở trong $\mathscr{C}^1(X;Y)$.

b) Gọi H là tập con của $J\times A\times A$ gồm các phần tử $(f, x, y)$ sao cho $f(x) =f(y)$. Rõ ràng H chứa $J\times \Delta$, trong đó $\Delta$ ký hiệu đường chéo trong tích $A\times A$; ta chứng minh rằng $H'= H$ **--** $(J\times \Delta )$ là đóng trong $J\times A\times A$. Vì $\mathscr{P}$ là phần bù trong J của ảnh của $H'$ qua phép chiếu thực sự pr$_1: J\times A\times A\rightarrow J$, điều này sẽ suy ra mệnh đề.

Tôpô của $\mathscr{C}^1(X;Y)$ mịn hơn tôpô hội tụ compact, nên ánh xạ $(\varphi , x) \rightarrow \varphi (x)$ từ $\mathscr{C}^1(X;Y)\times A$ đến Y là liên tục (General Topology, Chap. X, §3, no. 4, Cor. 1 of Th. 3); do đó H là đóng trong $J\times A\times A$. Vì vậy, chỉ cần chứng minh rằng $J\times \Delta$ là mở trong H, nói cách khác, rằng với mọi $\varphi \in J$ và mọi $x\in A$ tồn tại một lân cận $\Omega$ của $\varphi$ trong J và một lân cận B của $x$ trong X sao cho, với mọi cấu xạ $\psi$ trong $\Omega$, hạn chế của $\psi$ trên $A\cap B$ là đơn ánh.

Do đó, mệnh đề suy ra từ bổ đề sau:

#### Bổ đề 2 {#lie-ix-s9-lem-2 .statement tag=01HI}

Cho $x$ là một điểm của X$,\varphi : X\rightarrow Y$ là một cấu xạ thuộc lớp $C^1$ và là một phép nhúng tại $x$. Tồn tại một lân cận $\Omega$ của $\varphi$ trong $\mathscr{C}^1(X;Y)$ và một lân cận B của $x$ trong X sao cho, với mọi $\psi \in \Omega$, hạn chế của $\psi$ trên B là đơn ánh.

Cho U là một lân cận mở tương đối compact của $x$ đẳng cấu với một không gian vectơ hữu hạn chiều, và sao cho $\varphi (U)$ được chứa trong miền V của một biểu đồ. Tập hợp $\Omega_0$ gồm các $\psi \in \mathscr{C}^1(X;Y)$ sao cho $\psi (U)\subset V$ là mở trong $\mathscr{C}^1$(X;Y), và ánh xạ hạn chế $\Omega_0\rightarrow \mathscr{C}^1(U;V)$ là liên tục; do đó ta được quy về việc chứng minh bổ đề khi X = U và Y = V, nói cách khác, ta có thể giả sử rằng X là một không gian vectơ hữu hạn chiều và Y là một không gian Banach. Chọn các chuẩn trên X và Y.

Ánh xạ tuyến tính $D\varphi (x) : X\rightarrow$ Y là đơn ánh; ký hiệu đối chuẩn của nó là $q($Spectral Theory, Chap. III, §2, no. 6), sao cho, theo định nghĩa, ta có $\|D\varphi (x).t\| \geq q\|t\|$ với mọi $t\in X$. Cho $\varepsilon \in \mathbf{R}$ sao cho $0< \varepsilon  < q/2$, và cho B là một quả cầu đóng có tâm $x$ sao cho $\|D\varphi (u)-D\varphi (x)\| \leq \varepsilon$ với mọi $u\in B$. Ký hiệu $\Omega$ là tập con của $\mathscr{C}^1(X;Y)$ gồm các cấu xạ $\psi$ sao cho $\|D\psi (u)-D\varphi (u)\| \leq \varepsilon$ với mọi $u\in B$; nó là mở theo định nghĩa của tôpô của $\mathscr{C}^1(X;Y)$. Với $\psi \in \Omega$, đặt $\psi_0=\psi -D\varphi (x)$. Ta có $\|D\psi_0(u)\| \leq 2\varepsilon$ với mọi $u\in B$, và do đó $\|\psi_0(u)-\psi_0(v)\| \leq 2\varepsilon \|u-v\|$ với mọi $u$ và $v$ trong B (Differentiable and Analytic Manifolds, Results, 2.2.3). Suy ra rằng

$$
\|\psi (u)-\psi (v)\| \geq  \|D\varphi (x).(u-v)\| - \|\psi_0(u)-\psi_0(v)\| \geq (q-2\varepsilon )\|u-v\|
$$

Do đó, hạn chế của $\psi$ trên B là đơn ánh, vậy nên bổ đề được chứng minh.

#### Mệnh đề 4 {#lie-ix-s9-prop-4 .statement tag=01HJ}

Cho A là một tập con compact của X. Tồn tại một không gian vectơ hữu hạn chiều E và một cấu xạ $\varphi \in \mathscr{C}^r(X;E) (r\not=\omega )$ là một phép nhúng trong một lân cận của A.

Cho $(U_i, \varphi_i,E_i)_{i\in I}$ là một họ hữu hạn các bản đồ tọa độ của X có các miền xác định phủ A. Ta mở rộng $\varphi_i$ thành một ánh xạ từ X vào $E_i$ (cũng ký hiệu là $\varphi_i$) bằng cách đặt $\varphi_i(x) = 0$ với $x \notin U_i$. Cho $(V_i)_{i\in I}$ là một phủ của A bởi các tập con mở của X sao cho $\overline{V}_i\subset U_i$ với mọi $i\in I$ (sự tồn tại của một phủ như vậy suy ra từ General Topology, Chap. IX, §4, no. 3, Cor. 1 of Th. 3, áp dụng cho không gian compact $X'$ thu được bằng cách thêm vào X một điểm ở vô cực và phủ của $X'$ gồm các tập mở $U_i(i\in I)$ và $X'$ **--** A). Với mọi $i\in I$, cho $\alpha_i$ là một hàm số thuộc lớp $C^r$ trên X, bằng 1 tại mọi điểm của $V_i$, và có giá được chứa trong $U_i($Differentiable and Analytic Manifolds, Results, 5.3.6).

Xét ánh xạ $\varphi : X\rightarrow \bigoplus_{i\in I}(E_i\oplus \mathbf{R})$ được xác định bởi

$$
\varphi (x) = (\alpha_i(x)\varphi_i(x), \alpha_i(x))_{i\in I}
$$

### 2. ĐỊNH LÝ NHÚNG ĐẲNG BIẾN

Trong số này, ta giả sử rằng $r\not=\omega$.

#### Bổ đề 3 {#lie-ix-s9-lem-3 .statement tag=01HK}

Cho G là một nhóm tôpô compact tác động liên tục trên một không gian tôpô X; cho A là một tập con của X, ổn định dưới G, và W là một lân cận của A. Khi đó, tồn tại một lân cận mở V của A ổn định dưới G và được chứa trong$_{\circ}W$.

Đặt F = X **--** W và V = X**--** GF. Khi đó V mở (Tôpô học đại cương, Chương III, §4, no. 1, Hệ quả 1 của Mệnh đề 1), ổn định dưới G, và $A\subset V\subset W$.

#### Định lý 1 {#lie-ix-s9-thm-1 .statement tag=01HL}

Cho G là một nhóm Lie compact, $(g, x) \rightarrow gx$ là một luật tác động trái lớp $C^r$ của G trên X, và A là một tập compact của X. Tồn tại một biểu diễn tuyến tính giải tích $\rho$ của G trên một không gian vectơ hữu hạn chiều E, một cấu xạ $\varphi : X\rightarrow E$ lớp $C^r$, tương thích với các tác động của G, và một lân cận mở U của A, ổn định dưới G, sao cho hạn chế của $\varphi$ trên U là một phép nhúng.

Thay A bởi tập compact GA, ta được quy về trường hợp A ổn định dưới G.

Lấy E là không gian Hom$_{\mathbf{R}}(E_1,E_0)$, $\rho$ là biểu diễn của G trên E cảm sinh bởi tác động trên $E_1$, và $\varphi : X\rightarrow E$ là ánh xạ gán cho $x\in X$ ánh xạ tuyến tính $\psi  \rightarrow \psi (x)$ từ $E_1$ đến $E_0$. Đây là một cấu xạ lớp $C^r$; với $x\in X,g\in G,\psi \in E_1$, ta có (ký hiệu $\tau (g)$ là tự đẳng cấu $x \rightarrow gx$ của X):

$$
\varphi (gx)(\psi )-\psi (gx) =\varphi (x)(\psi \circ \tau (g)) = (\rho (g)\varphi (x))(\psi )
$$

Với mọi $i\in I$, ánh xạ $\alpha_i\varphi_i$ có lớp $C^r$ (vì các hạn chế của nó lên $U_i$ và lên phần bù của giá đỡ của $\alpha_i$ đều như vậy), và hạn chế của nó lên $V_i$ là một phép nhúng; suy ra $\varphi$ là một cấu xạ lớp $C^r$ và là một phép nhúng ngập tại mọi điểm của A. Ta chứng minh rằng hạn chế của $\varphi$ lên A là đơn ánh. Cho $x, y$ là hai điểm của A sao cho $\varphi (x) =\varphi (y)$, và cho $i\in I$ sao cho $x\in V_i$. Khi đó $\alpha_i(x) = 1$, suy ra $\alpha_i(y) = 1$, điều đó kéo theo $y\in U_i$; nhưng ta cũng có $\varphi_i(x) =\varphi_i(y)$, nên $x=y$ vì $\varphi_i$ cảm sinh một phép nhúng của $U_i$ vào $E_i$.

Có thể chứng minh được$^9$ rằng mọi đa tạp tách biệt, đếm được ở vô cực và có chiều thuần túy $n$, được nhúng vào $\mathbf{R}^{2n}$; đối với một kết quả yếu hơn, xem Bài tập 2.

$^9$ Xem H. WHITNEY, Các giao tự của một $n$-đa tạp trơn trong không gian $2n$-chiều, Ann. of Math., 45 (1944), pp. 220-246.

Cho $\alpha :$ Hom$_{\mathbf{R}}(E_1,E_0)\rightarrow E_0$ là ánh xạ tuyến tính $u \rightarrow u(\varphi_0)$; ta có $\alpha \circ \varphi =\varphi_0$, do đó $\varphi$ là một phép nhúng trong một lân cận của A vì $\varphi_0$ là một phép nhúng. Suy ra tồn tại một lân cận mở U của A sao cho hạn chế của $\varphi$ trên U là một phép nhúng; ta có thể chọn U ổn định dưới G theo Bổ đề 3, do đó có định lý.

#### Hệ quả 1 {#lie-ix-s9-thm-1-cor-1 .statement tag=01HM}

Giả sử X là compact. Tồn tại một biểu diễn tuyến tính giải tích $\rho$ của G trên một không gian vectơ hữu hạn chiều E và một phép nhúng $\varphi : X\rightarrow E$ sao cho $\varphi (gx) =\rho (g)\varphi (x)$ với $g\in G, x\in X$.

#### Hệ quả 2 {#lie-ix-s9-thm-1-cor-2 .statement tag=01HN}

Cho H là một nhóm con đóng của G. Tồn tại một biểu diễn tuyến tính giải tích của G trên một không gian vectơ hữu hạn chiều E và một điểm $v\in E$ với nhóm cố định H.

Áp dụng Hệ quả 1 cho phép toán chính tắc của G trên đa tạp compact $G/H$. Điều này cho một biểu diễn tuyến tính giải tích $\rho : G\rightarrow \mathbf{G}\mathbf{L}(E)$ và một phép nhúng $\varphi : G/H\rightarrow E$ sao cho $\varphi (gx) =\rho (g)\varphi (x),g\in G, x\in G/H$. Gọi $\overline{e}\in G/H$ là lớp của $e\in G$, và $v=\varphi (\overline{e})$ là ảnh của nó. Với mọi $g\in G$, ta có $\rho (g)v=v\Leftarrow \Rightarrow \varphi (g\overline{e}) =\varphi (\overline{e})\Leftarrow \Rightarrow g\overline{e}= \overline{e}\Leftarrow \Rightarrow g\in H$.

#### Hệ quả 3 {#lie-ix-s9-thm-1-cor-3 .statement tag=01HO}

Giả sử X là paracompact. Tồn tại một không gian Hilbert thực E, một biểu diễn đơn vị liên tục $^{10}\rho$ của G trên E và một phép nhúng $\varphi : X\rightarrow E$ thuộc lớp $C^r$ sao cho $\varphi (gx) =\rho (g)\varphi (x)$ với mọi $g\in G$ và mọi $x\in X$.

Không gian $X/G$ là compact địa phương (General Topology, Chap. III, §4, no. 5, Prop. 11). Các thành phần liên thông của nó là các ảnh của các thành phần liên thông của X, vốn đếm được ở vô cực (General Topology, Chap. I, §9, no. 10, Th. 5); do đó, chính chúng cũng đếm được ở vô cực, điều này suy ra rằng $X/G$ là paracompact (loc. cit.). Vì vậy, tồn tại một phủ hữu hạn địa phương $(U'_{\alpha})_{\alpha\in I}$ của $X/G$ bởi các tập mở tương đối compact, và một phủ $(V'_{\alpha})_{\alpha\in I}$ sao cho $\overline{V}'_{\alpha}\subset U'_{\alpha}$ với mọi $\alpha \in I ($General Topology, Chap. IX, §4, no. 3, Cor. 1 of Th. 3); lấy ảnh ngược, ta thu được hai phủ hữu hạn địa phương $(U_{\alpha})_{\alpha\in I}$ và $(V_{\alpha})_{\alpha\in I}$ của X bởi các tập mở tương đối compact ổn định dưới G, sao cho $\overline{V}_{\alpha}\subset U_{\alpha}$ với mọi $\alpha \in I$.

Với mọi $\alpha \in I$, tồn tại một biểu diễn $\rho_{\alpha}$ của G trên một không gian vectơ thực hữu hạn chiều $E_{\alpha}$ và một cấu xạ $\varphi_{\alpha}\in \mathscr{C}^r(X;E_{\alpha})$, tương thích với các phép toán của G, mà hạn chế của nó trên $U_{\alpha}$ là một phép nhúng (Th. 1). Với $\alpha \in I$, cho $a_{\alpha}$ là một hàm số thuộc lớp $C^r$ trên X, bằng 1 trên $V_{\alpha}$ và bằng 0 bên ngoài $U_{\alpha}($Differentiable and Analytic Manifolds, Results, 5.3.6). Đặt $b_{\alpha}(x) =\int_Ga_{\alpha}(gx)dg$ với $x\in X$. Hàm $b_{\alpha}$ thuộc lớp $C^r$, bất biến dưới G (§6, no. 4, Cor. 2), bằng 1 trên $V_{\alpha}$ và bằng 0 bên ngoài $U_{\alpha}$. Trang bị cho mỗi $E_{\alpha}$ một tích vô hướng Hilbert bất biến dưới G (§1, no. 1), và $\mathbf{R}$ cấu trúc Hilbert chính tắc của nó; gọi E là tổng Hilbert của họ $(E_{\alpha}\oplus \mathbf{R})_{\alpha\in I}$, và gọi $\rho$ là biểu diễn của G trên E cảm sinh bởi các $\rho_{\alpha}$ và tác động tầm thường của G trên $\mathbf{R}$. Với $x\in X$, đặt $\varphi (x) = (b_{\alpha}(x)\varphi_{\alpha}(x), b_{\alpha}(x))_{\alpha\in I}$. Khi đó $\varphi$ là một cấu xạ thuộc lớp $C^r$ từ X vào E, tương thích với các phép toán của G; ta kiểm chứng như trong chứng minh của Mệnh đề 4 (no. 1) rằng $\varphi$ là một phép nhúng, điều này suy ra hệ quả.

$^{10}$Đó là (Spectral Theory, in preparation) một biểu diễn tuyến tính liên tục (Integration, Chap. VIII, §2, no. 1) sao cho toán tử $\rho (g)$ là unita với mọi

$$
g\in G
$$

### 3. ỐNG VÀ CÁC ĐƯỜNG CẮT NGANG

#### Bổ đề 4 {#lie-ix-s9-lem-4 .statement tag=01HP}

Cho H là một nhóm Lie compact, $\rho : H\rightarrow \mathbf{G}\mathbf{L}(V)$ là một biểu diễn liên tục (do đó giải tích) của H trên một không gian vectơ thực hữu hạn chiều, và W là một lân cận của gốc trong V. Tồn tại một lân cận mở B của gốc, được chứa trong W và ổn định dưới H, và một đẳng cấu giải tích $u: V\rightarrow B$, tương thích với các phép toán của H, sao cho $u(0) = 0$ và $Du(0) =$ Id$_V$.

Chọn một tích vô hướng trên V bất biến dưới H (§1, no. 1). Tồn tại một số thực $r >0$ sao cho quả cầu mở B bán kính $r$ được chứa trong W; rõ ràng nó ổn định dưới H. Đặt $u(v) =r(r^2+\|v\|^2)^{-1/2}v$ với mọi $v\in V$; khi đó $u$ là một ánh xạ giải tích song ánh từ V vào B, tương thích với các phép toán của H, và ánh xạ ngược của nó $w \rightarrow r(r^2- \|w\|^2)^{-1/2}w$ là giải tích. Hơn nữa, $u(0) = 0$ và $Du(0) =$ Id$_V$.

#### Mệnh đề 5 {#lie-ix-s9-prop-5 .statement tag=01HQ}

Cho H là một nhóm Lie compact, $(h, x) \rightarrow hx$ là một luật tác động trái thuộc lớp $C^r$ của H trên X, và $x$ là một điểm của X cố định dưới tác động của H. Khi đó nhóm H tác động tuyến tính trên không gian vectơ $T = T_x(X)$; tồn tại một phép nhúng mở $\varphi : T\rightarrow X$ thuộc lớp $C^r$, tương thích với các phép toán của H, sao cho $\varphi (0) =x$ và $T_0(\varphi )$ là ánh xạ đồng nhất của T.

Cho $(U, \psi ,E)$ là một biểu đồ của X tại $x$, sao cho U ổn định dưới H (no. 2, Bổ đề 3) và sao cho $\psi (x) = 0$. Đồng nhất E với T bằng $T_x(\psi )$, và đặt

$\psi^{\sharp}(y) =\int_Hh.\psi (h^{-1}y)dh$ với $y\in U$,

trong đó $dh$ là độ đo Haar trên H có khối lượng toàn phần 1.

Khi đó (§6, no. 4, Hệ quả $1$)$\psi^{\sharp}$ là một cấu xạ lớp $C^r$ từ U vào T, tương thích với các phép toán của H, sao cho $\psi^{\sharp}(x) = 0$ và $d_x\psi^{\sharp}=$ Id$_T$. Do đó, tồn tại một tập mở $U'\subset U$ chứa $x$, và một lân cận mở V của 0 trong T, sao cho $\psi^{\sharp}$ cảm sinh một đẳng cấu $\theta : U'\rightarrow V$. Nếu cần hạn chế $U'$ và V, ta có thể giả sử rằng chúng ổn định đối với H và rằng tồn tại một đẳng cấu $u: T\rightarrow V$ tương thích với các phép toán của H (Bổ đề 4). Bây giờ chỉ cần lấy $\varphi =\theta^{-1}\circ u$.

Nhắc lại (Đa tạp khả vi và giải tích, Các kết quả, 6.5.1) rằng nếu G là một nhóm Lie, H là một nhóm con Lie của G và Y là một đa tạp trên đó H tác động bên trái, ta ký hiệu bởi $G\times^HY$ thương của đa tạp tích $G\times Y$ bởi phép toán bên phải $((g, y), h) \rightarrow (gh, h^{-1}y)$ của H; đây là một đa tạp trên đó nhóm Lie G tác động một cách tự nhiên bên trái; phép chiếu $G\times^HY\rightarrow G/H$ là một bó với thớ Y. Hơn nữa, nếu Y là một không gian vectơ hữu hạn chiều trên đó H tác động tuyến tính, $G\times^HY$ có một cấu trúc tự nhiên của một G-bó vectơ với cơ sở $G/H ($Đa tạp khả vi và giải tích, Các kết quả, 7.10.2).

Cho G là một nhóm Lie tác động đúng trên đa tạp X (Tôpô đại cương, Chương III, §4, no. 1, Định nghĩa 1) sao cho luật tác động $(g, x) \rightarrow gx$ là lớp $C^r$. Khi đó, với mọi điểm $x$ của X, quỹ đạo $Gx$ của $x$ là một đa tạp con đóng của X, đẳng cấu với không gian thuần nhất Lie $G/G_x$, trong đó $G_x$ là bộ ổn định của $x$ trong G (xem Chương III, §1, no. 7, Mệnh đề 14 (ii), và Tôpô đại cương, Chương III, §4, no. 2, Mệnh đề 4); đây là một nhóm Lie compact (tại chỗ đã dẫn).

#### Mệnh đề 6 {#lie-ix-s9-prop-6 .statement tag=01HR}

Giả sử rằng đa tạp X là compact địa phương; cho $x$ là một điểm của X, $G_x$ là bộ ổn định của nó. Tồn tại một biểu diễn tuyến tính giải tích hữu hạn chiều $\tau : G_x\rightarrow \mathbf{G}\mathbf{L}(W)$, và một phép nhúng mở $\alpha : G\times^{G_x}W\rightarrow X$ lớp $C^r$, tương thích với các phép toán của G, ánh xạ lớp của $(e,0)\in G\times W$ vào $x$.

Đặt $T = T_x(X)$. Cho W là một không gian con bù của $T_x(Gx)$ trong T, ổn định dưới tác động của $G_x$ (chẳng hạn, không gian con trực giao của $T_x(Gx)$ đối với một tích vô hướng trên T bất biến dưới tác động của $G_x$). Mặt khác, cho $\varphi : T\rightarrow X$ là một cấu xạ với các tính chất đã nêu trong Mệnh đề 5 (đối với $H = G_x$). Xét cấu xạ $\lambda : G\times W\rightarrow X$ được xác định bởi $\lambda (g, w) =g\varphi (w)$. Nó cảm sinh qua phép chuyển sang thương một cấu xạ $\mu: G\times^{G_x}W\rightarrow X$ lớp $C^r$, tương thích với các phép toán của G, ánh xạ lớp $z$ của $(e,0)$ vào $x$.

Ta chứng minh rằng $\mu$ là étale tại điểm $z$. Ta có

dim(G $\times^{G_x}W$) $=$ dim(G) + dim(W) $-$ dim(G$_x$)

= dim(G$x$) $+$ dim(W) = dim(T),

suy ra chỉ cần chứng minh rằng $\mu$ đầy đủ hạng tại $z$, hay tương đương rằng $\lambda$ đầy đủ hạng tại $(e,0)$. Nhưng ánh xạ tiếp tuyến $T_{(e,0)}(\lambda ) : T_e(G)\oplus W\rightarrow T$ bằng $T_e(\rho (x)) +i$, trong đó $\rho (x)$ là ánh xạ quỹ đạo $g \rightarrow gx$ và $i$ là đơn ánh chính tắc từ W vào T; vì Im $T_e(\rho (x)) = T_x(Gx)$, ánh xạ $T_{(e,0)}(\lambda )$ là toàn ánh, và $\mu$ là étale tại $z$.

Ta sẽ chứng minh rằng tồn tại một lân cận mở $\Omega$ của $Gz$ trong $G\times^{G_x}W$, ổn định dưới G, sao cho $\mu$ cảm sinh một đẳng cấu từ $\Omega$ lên một tập con mở của X. Điều này sẽ suy ra mệnh đề: thật vậy, ảnh ngược của $\Omega$ trong $G\times W$ ổn định dưới G, và do đó có dạng $G\times B$, trong đó B là một tập con mở của W chứa gốc và ổn định dưới $G_x$; nếu cần, thu hẹp $\Omega$, ta có thể giả sử rằng tồn tại một đẳng cấu $u: W\rightarrow B$, tương thích với các phép toán của $G_x$ (Bổ đề 4). Rõ ràng cấu xạ hợp thành $\alpha : G\times^{G_x}W\overset{(Id,u)}{\longrightarrow}G\times^{G_x}B\longrightarrow^\mu$ X thỏa mãn các điều kiện trong mệnh đề.

Do đó, mệnh đề là hệ quả của bổ đề sau:

#### Bổ đề 5 {#lie-ix-s9-lem-5 .statement tag=01HS}

Cho Z là một đa tạp tách biệt lớp $C^r$, được trang bị một luật tác động trái $m: G\times Z\rightarrow Z$ lớp $C^r$, và $\mu: Z\rightarrow X$ là một cấu xạ (lớp $C^r$) tương thích với các phép toán của G. Cho z là một điểm của Z, và $x=\mu(z)$. Giả sử rằng $\mu$ là étale tại $z$, và nhóm cố định của $z$ trong G bằng với nhóm cố định $G_x$ của $x$. Khi đó, tồn tại một lân cận mở $\Omega$ của quỹ đạo $Gz$, ổn định dưới G, sao cho $\mu$ cảm sinh một đẳng cấu từ $\Omega$ lên một tập con mở của X.

Vì $\mu$ tương thích với các phép toán của G, nên nó là étale tại mọi điểm của $Gz$; vì ánh xạ chính tắc $G/G_x\rightarrow Gx$ là một đồng phôi, nên ánh xạ từ $Gz$ đến $Gx$ cảm sinh bởi $\mu$ cũng vậy. Do đó, từ Mệnh đề 2 của no. 1 suy ra rằng tồn tại một lân cận mở U của $Gz$ trong Z sao cho $\mu$ cảm sinh một nhúng mở của U vào X.

Vì G tác động thực sự lên X, tồn tại một lân cận mở V của $x$ và một tập con compact K của G sao cho $gV\cap V =\emptyset$ với $g \notin K ($General Topology, Chap. III, §4, no. 4, Mệnh đề 7); đặc biệt, $e\in K$. Tập $W_1$ gồm các điểm $y\in Z$ sao cho $Ky\subset U$ là mở trong Z: thật vậy, Z**--** $W_1$ là ảnh của tập đóng $(K\times Z)$ **--** $m^{-1}(U)$ qua phép chiếu thực sự pr$_2: K\times Z\rightarrow Z$. Đặt $W = W_1\cap \mu^{-1}(V)$; đây là một tập con mở của Z, chứa $z$, và thỏa mãn các điều kiện sau:

(i) KW $\subset U$, và đặc biệt $W\subset U$;

(ii) $\mu(W)\subset V$.

Đặt $\Omega =$ GW và xét hạn chế của $\mu$ lên $\Omega$. Đây là một cấu xạ étale, vì mọi điểm của $\Omega$ đều liên hợp dưới G với một điểm của U. Ta chứng minh rằng nó đơn ánh: cho $g, h$ trong G và $u, v$ trong W sao cho $\mu(gu) =$ $\mu(hv)$. Đặt $k=g^{-1}h$; khi đó $\mu(u) =k\mu(v)$, do đó $k\in K$ theo (ii). Nhưng $kv$ và $u$ thuộc U theo (i); do đó, $u=kv$ vì hạn chế của $\mu$ lên V là đơn ánh, suy ra $gu=hv$. Vậy, hạn chế của $\mu$ lên $\Omega$ là đơn ánh, và do đó (Differentiable and Analytic Manifolds, Kết quả, 5.7.8) là một đẳng cấu lên một phân đa tạp con mở của X, điều này hoàn tất chứng minh.

Theo các điều kiện của Mệnh đề 6, ảnh của $\alpha$ là một lân cận mở T của quỹ đạo A của $x$, được trang bị cấu trúc bó vectơ với cơ sở A, trong đó tiết diện không chính là quỹ đạo A. Một lân cận như thế được gọi là một ống tuyến tính (quanh quỹ đạo đang xét). Với mỗi điểm $a\in A$, sợi $Y_a$ của bó vectơ này là một phân đa tạp con của X, ổn định dưới nhóm ổn định $G_a$ của $a$, và sao cho cấu xạ từ $G\times^{G_a}Y_a$ đến X ánh xạ lớp của $(g, y)\in G\times Y_a$ thành $gy\in X$ cảm sinh một cấu xạ lớp $C^r$ từ $G\times^{G_a}Y_a$ đến T. Khi đó $Y_a$ được gọi là tiết diện ngang tại $a$ của ống T. Ta nhận xét rằng không gian tiếp tuyến tại $a$ của $Y_a$ đẳng cấu chính tắc với $Y_a$ và rằng nó là một bổ sung của $T_a(A)$ trong $T_a(X)$; do đó, bó vectơ T với cơ sở A đẳng cấu chính tắc với bó pháp tuyến của A trong X (Differentiable and Analytic Manifolds, Results, 8.1.3).

### 4. CÁC KIỂU QUỸ ĐẠO

Cho G là một nhóm tôpô tác động liên tục lên một không gian tôpô tách biệt E. Với mọi điểm $x$ của E, ký hiệu $G_x$ là nhóm ổn định của $x$ trong G, và giả sử rằng ánh xạ chính tắc $G/G_x\rightarrow Gx$ là một đồng phôi; điều này đặc biệt đúng trong hai trường hợp sau:

a) tôpô của G và E là rời rạc;

$b) G$ tác động thực sự lên E (General Topology, Chap. III, §4, no. 2, Mệnh đề 4), ví dụ, G là compact (General Topology, Chap. III, §4, no. 1, Mệnh đề 2).

Đặt $\mathscr{T}$ là tập hợp các lớp liên hợp của các nhóm con đóng của G. Với mọi $x\in E$, ta gọi kiểu quỹ đạo của $x$, hay đôi khi gọi là kiểu của $x$, là lớp của $G_x$ trong $\mathscr{T}$; hai điểm của cùng một quỹ đạo có cùng kiểu quỹ đạo (Đại số, Chương I, §5, no. 2, Mệnh đề 2); hai quỹ đạo có cùng kiểu khi và chỉ khi chúng đẳng cấu với tư cách là G-tập hợp (Đại số, Chương I, §5, no. 5, Định lý 1). Với mọi $t\in \mathscr{T}$, đặt $E_{(t)}$ là tập hợp các điểm của E có kiểu $t$, tức là, hợp của các quỹ đạo có kiểu $t$; đây là một tập con ổn định của E. Với $H\in t$, ta cũng viết $E_{(H)}$ cho $E_{(t)}$; chẳng hạn, $E_{(G)}$ là không gian con đóng của E gồm các điểm cố định bởi G.

Cho $\mathscr{T}$ quan hệ tiền thứ tự sau:

$t\leq t'\Leftarrow \Rightarrow$ tồn tại $H\in t$ và $H'\in t'$ sao cho $H\supset H'$.

Cho $\Omega$ và $\Omega '$ là hai quỹ đạo của G trên $E,t$ và $t'$ là các kiểu của chúng; khi đó $t\leq t'$ khi và chỉ khi tồn tại một G-cấu xạ (tất nhiên toàn ánh và liên tục) từ $\Omega '$ đến $\Omega$.

Cho $x, x'$ thuộc E, và $t, t'$ là các kiểu của chúng; khi đó $t\leq t'$ khi và chỉ khi tồn tại $a\in G$ sao cho $aG_{x'}a^{-1}\subset G_x$.

#### Bổ đề 6 {#lie-ix-s9-lem-6 .statement tag=01HT}

Cho G là một nhóm Lie.

a) Mọi dãy giảm các nhóm con compact của G đều dừng.

b) Cho H và $H'$ là hai nhóm con compact của G sao cho $H\subset H'$ và sao cho tồn tại một đẳng cấu (của các nhóm tôpô) từ $H'$ đến H. Khi đó $H = H'$.

c) Với quan hệ $t\leq t'$, tập hợp $\mathscr{T}$ là một tập có thứ tự Noether (Lý thuyết tập hợp, Chương III, §6, no. 5, văn bản trước Mệnh đề 7).

a) Cho $(H_i)_{i\geq 1}$ là một dãy giảm các nhóm con compact của G; đây là các nhóm con Lie của G (Chương III, §8, no. 2, Định lý 2). Dãy các số nguyên (dim $H_i$)$_{i\geq 1}$ là giảm, do đó dừng, nên tồn tại một số nguyên N sao cho các nhóm con $H_i$ có cùng thành phần liên thông đơn vị với mọi $i\geq N$. Khi đó dãy giảm các số nguyên dương $(H_i: (H_i)_0)_{i\geq N}$ là dừng, nên $H_i= H_{i+1}$ với mọi $i$ đủ lớn.

b) Cho $f$ là một đẳng cấu từ $H'$ đến H. Dãy $(f^n(H))_{n\geq 0}$ là một dãy giảm các nhóm con compact của G, nên $f^n(H) =f^{n+1}(H)$ với mọi $n$ đủ lớn, theo a). Vì $f$ là một đẳng cấu, điều này suy ra $f(H) = H =f(H')$, do đó $H = H'$.

==========

Đó là toàn bộ đoạn văn. Hãy viết bản dịch của mọi thứ nằm giữa hai dòng đó, và dừng ở đó.

c) Cho $t, t'\in \mathscr{T}$ sao cho $t\leq t'$ và $t'\leq t$. Khi đó, tồn tại $H,H_1\in t$ và $H',H'_1\in t'$ sao cho $H\supset H'$ và $H_1\subset H'_1$. Gọi $g$ và $g'$ là hai phần tử của G sao cho $H_1=gHg^{-1}$ và $H'_1=g'H'g^{'-1}$; đặt $u=g^{'-1}g$. Khi đó

$$
uHu^{-1}\subset H'\subset H
$$

theo b), điều này suy ra rằng $uHu^{-1}= H$, do đó $H'= H$ và $t'=t$. Vậy, tập hợp $\mathscr{T}$ có thứ tự, và nó là Noether theo a).

#### Định lý 2 {#lie-ix-s9-thm-2 .statement tag=01HU}

Cho G là một nhóm Lie tác động đúng lên X, sao cho luật tác động $(g, x) \rightarrow gx$ thuộc lớp $C^r$. Giả sử X là paracompact.

a) Ánh xạ gán cho mỗi điểm của X kiểu quỹ đạo của nó có tính chất nửa liên tục sau đây: cho $x\in X$ và cho $t\in \mathscr{T}$ là kiểu quỹ đạo của nó; tồn tại một lân cận mở ổn định U của $x$ sao cho, với mọi $u\in U$, kiểu của $u$ là $\geq t$.

b) Với mọi $t\in \mathscr{T},X_{(t)}$ là một đa tạp con của X, quan hệ tương đương trên $X_{(t)}$ cảm sinh bởi tác động của G là chính quy (Differentiable and Analytic Manifolds, Results, 5.9.5), và cấu xạ $X_{(t)}\rightarrow X_{(t)}/G$ là một bó.

c) Giả sử $X/G$ liên thông. Khi đó tập hợp các kiểu quỹ đạo của các phần tử của X có một phần tử lớn nhất $\tau$; hơn nữa, $X_{(\tau)}$ là một tập con mở trù mật của X và $X_{(\tau)}/G$ liên thông.

Cho $x$ là một điểm của X và $t\in \mathscr{T}$ là kiểu của nó. Để chứng minh a) và b), ta có thể thay X bởi một tập mở ổn định chứa $x$, và do đó (Mệnh đề 6) có thể giả sử rằng X có dạng $G\times^HW$, trong đó W là không gian của một biểu diễn tuyến tính giải tích hữu hạn chiều của một nhóm con compact H của G, còn điểm $x$ là ảnh $p(e,0)$ của $(e,0)\in G\times W$ qua phép chiếu chính tắc $p: G\times W\rightarrow G\times^HW$. Nếu $u=p(g, y)\in G\times^HW$ và $a\in G$, thì $au=u$ khi và chỉ khi tồn tại $h\in H$ sao cho $(ag, y) = (gh^{-1}, hy)$, tức là, nếu $a\in gH_yg^{-1}$. Do đó, $G_u=gH_yg^{-1}$; nói riêng, $G_x= H$, nên $G_u$ liên hợp với một nhóm con của $G_x$, điều này chứng minh rằng kiểu của $u$ là $\geq t$, suy ra a).

Hơn nữa, $u$ có kiểu $t$ khi và chỉ khi $G_u$ liên hợp với H trong G, hoặc tương đương là $H_y$ liên hợp với H trong G; theo Bổ đề $6b)$, điều này có nghĩa là $H_y= H$, và do đó $y$ bị H cố định. Nếu $W'$ là không gian con vectơ của W gồm các phần tử bị H cố định, suy ra $X_{(t)}$ có thể được đồng nhất với $G\times^HW'$, và do đó cũng với $G/H\times W'$, suy ra b).

Để chứng minh c), xét rằng giả thiết $X/G$ liên thông ngụ ý rằng X thuần có số chiều hữu hạn: thật vậy, với mọi $k\geq 0$, ký hiệu bởi $X_k$ tập các điểm $x\in X$ sao cho dim$_xX =k$; khi đó $X_k$ mở và đóng trong X, và ổn định dưới tác dụng của G, nên X bằng một trong các $X_k$.

Ta nay chứng minh c) bằng quy nạp theo chiều của X, mệnh đề hiển nhiên khi dim X = 0. Cho $\tau$ là một phần tử cực đại trong số các kiểu quỹ đạo của các điểm của X (một phần tử như vậy tồn tại theo Bổ đề $6c$)). Ta sẽ chứng minh điều sau:

$c')$ Với mọi tập con A của $X_{(t)}$, mở và đóng trong $X_{(\tau)}$ và ổn định dưới tác dụng của G, bao đóng $\overline{A}$ của A trong X là mở.

Mệnh đề này suy ra c). Thật vậy, trước hết chú ý rằng $X_{(\tau)}$ mở trong X, theo a); mệnh đề $c')$ suy ra rằng $\overline{X}_{(\tau)}$ mở và đóng trong X, do đó bằng X vì nó ổn định dưới tác dụng của G và $X/G$ liên thông. Cho A là một tập con không rỗng, mở và đóng của $X_{(\tau)}$ ổn định dưới tác dụng của G; theo $c')$, $\overline{A}$ mở và đóng trong X và ổn định dưới tác dụng của G, do đó bằng X; điều này ngụ ý rằng A trù mật trong $X_{(\tau)}$, do đó bằng $X_{(\tau)}$. Do đó, mọi tập con không rỗng, mở và đóng của $X_{(\tau)}/G$ đều bằng $X_{(\tau)}/G$, điều đó chứng tỏ rằng $X_{(\tau)}/G$ liên thông. Cuối cùng, vì $X_{(\tau)}$ trù mật trong X, suy ra từ a) rằng mọi điểm của X đều có kiểu $\leq \tau$; nói cách khác, $\tau$ là phần tử lớn nhất trong số các kiểu quỹ đạo của các điểm của X.

Bây giờ chứng minh $c')$. Có thể giả sử rằng A không rỗng; lấy $x\in A$. Chỉ cần chứng minh rằng A là một lân cận của x. Để làm điều đó, như trên, có thể giả sử rằng $X = G\times^HW$ với H compact, x là ảnh chính tắc của $(e,0)$. Giả sử trước hết rằng H tác động tầm thường lên W: khi đó X có thể được đồng nhất với $(G/H)\times W$, và $X_{(\tau)}/G = X/G$ đồng phôi với W, do đó liên thông; vì vậy, $A/G = X/G$, suy ra A = X. Từ đây giả sử rằng H không tác động tầm thường lên W. Chọn một tích vô hướng trên W bất biến dưới nhóm compact H; lấy S là mặt cầu đơn vị trong W (tập hợp các vectơ có chuẩn 1). Chú ý rằng $S/H$ liên thông: thật vậy, nếu dim(W) $\geq 2$, S liên thông, và nếu dim(W) = 1, S là một không gian gồm hai điểm mà H tác động không tầm thường. Đặt $Y = G\times^HS$; đây là một đa tạp con đóng của X, ổn định dưới G, có đồng chiều 1, và $Y/G$, vốn đồng phôi với $S/H$, là liên thông. Do đó, theo giả thiết quy nạp, tồn tại một kiểu quỹ đạo cực đại $\theta$ cho Y, tập $Y_{(\theta)}$ mở và trù mật trong Y, và $Y_{(\theta)}/G$ liên thông.

Xét phép toán của $\mathbf{R}^*_+$ trên X cảm sinh bởi việc qua thương theo luật phép toán $(\lambda ,(g, w)) \rightarrow (g, \lambda w)$ của $\mathbf{R}^*_+$ trên $G\times W$. Hai điểm của X liên hợp dưới phép toán này thì cùng kiểu quỹ đạo; do đó, $X_{(\theta)}$ chứa $\mathbf{R}^*_+Y_{(\theta)}$, là một tập con mở trù mật của X. Nhưng $X_{(\tau)}$ mở theo a), nên giao với $X_{(\theta)}$, suy ra $\theta =\tau$.

Mặt khác, đồng phôi $(\lambda , w) \rightarrow \lambda w$ từ $\mathbf{R}^*_+\times S$ đến W **--** $\{0\}($General Topology, Chap. VI, §2, no. 3, Mệnh đề 3) cảm sinh một đồng phôi từ $\mathbf{R}^*_+\times (S/H)$ đến $(\mathbf{R}^*_+S)/H$, do đó cũng từ $\mathbf{R}^*_+\times (Y/G)$ đến $(\mathbf{R}^*_+Y)/G$, và từ $\mathbf{R}^*_+\times (Y_{(\theta)}/G)$ đến $(\mathbf{R}^*_+Y_{(\theta)})/G$. Vì vậy, $(\mathbf{R}^*_+Y_{(\theta)})/G$ liên thông, và $X_{(\tau)}/G$, vốn chứa một tập con trù mật liên thông, tự nó liên thông (General Topology, Chap. I, §11, no. 1, Mệnh đề 1). Do đó, A bằng $X_{(\tau)}$, suy ra trù mật trong X, và A là một lân cận của x. Điều này hoàn tất chứng minh định lý.

Với ký hiệu trong Định lý $2c)$, các điểm của $X_{(\tau)}$ được gọi là các điểm chính và các quỹ đạo của chúng được gọi là các quỹ đạo chính. Nếu $x$ là một điểm của X, và nếu $G\times^{G_x}W$ là một ống tuyến tính trong X quanh quỹ đạo của $x$, thì điểm $x$ là chính khi và chỉ khi $G_x$ tác động tầm thường trên W, tức là nếu ống có dạng $(G/G_x)\times W$.

#### Ví dụ 1 {#lie-ix-s9-n4-exa-1 .statement tag=01HV}

Cho G là một nhóm Lie compact liên thông, tác động lên chính nó bởi các tự đẳng cấu nội. Nhóm ổn định của một phần tử $x$ của G đơn giản là tập trung hóa $Z(x)$ của $x$ trong G; nó chứa mọi xuyến cực đại chứa $x$. Do đó kiểu quỹ đạo lớn nhất $\tau$ là lớp liên hợp của các xuyến cực đại của G. Tập mở $G_{(\tau)}$ là tập các phần tử rất chính quy của G (§5, no. 1, Nhận xét). Giả sử rằng G là đơn liên thông. Khi đó $G_{(\tau)}$ bằng với tập $G_r$ của các phần tử chính quy của G (§5, no. 2, Nhận xét 2); nếu A là một alcove của một đại số con Cartan $\mathfrak{t}$ của $\mathfrak{g}= L(G)$, thì ánh xạ hợp thành $\pi : A\longrightarrow^{exp}G_r\longrightarrow G_r/$Int(G) là một đẳng cấu của các đa tạp giải tích. Thật vậy, đây là một đồng phôi (§5, no. 2, Hệ quả của Mệnh đề 2); lấy $a\in A$, đặt $t=$ exp $a$ và đồng nhất $T_t(G)$ với $\mathfrak{g}$ bằng phép tịnh tiến $\gamma (t)$. Khi đó, ánh xạ tiếp tuyến $T_a(\pi )$ có thể được đồng nhất với hợp thành của đơn ánh chính tắc $\mathfrak{t}\rightarrow \mathfrak{g}$ và ánh xạ thương $\mathfrak{g}\rightarrow \mathfrak{g}/$Im(Ad $t^{-1}-1$). Vì $t$ là chính quy, $T_a(\pi )$ là một đẳng cấu, do đó có kết quả đã nêu (Differentiable and Analytic Manifolds, Kết quả, 5.7.8).

#### Ví dụ 2 {#lie-ix-s9-n4-exa-2 .statement tag=01HW}

Cho E là một không gian affine Euclid thực, $\mathfrak{H}$ một tập hợp các siêu phẳng của E, W là nhóm các phép dời của E được sinh bởi các phép phản xạ trực giao đối với các siêu phẳng của $\mathfrak{H}$. Giả sử rằng $\mathfrak{H}$ ổn định dưới W và rằng nhóm W, với tôpô rời rạc, tác động đúng lên E.

Phần trên có thể được áp dụng cho phép tác động của W lên E. Nhóm ổn định của một điểm $x$ của E là nhóm con của W được sinh bởi các phép phản xạ đối với các siêu phẳng của $\mathfrak{H}$ chứa $x$ (Chương V, §3, no. 3, Mệnh đề 2). Do đó, kiểu quỹ đạo lớn nhất $\tau$ là lớp của nhóm con $\{$Id$_E\}$, và $E_{(\tau)}$ là hợp của các buồng của E. Chú ý rằng trong trường hợp này, phủ $E_{(\tau)}\rightarrow E_{(\tau)}/W$ là tầm thường, và đặc biệt $E_{(\tau)}$ không liên thông nếu $\mathfrak{H}$ không rỗng.

### Bài tập {#lie-ix-s9-exercises}

Xem [các bài tập cho § 9](exercises/s9/).
