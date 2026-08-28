---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IX
chapter_title: COMPACT REAL LIE GROUPS
section: 4
section_title: Root system associated to a compact group
lang: vi
source: lie-vii-ix
book_pages: 304-324, 396-405
pdf_pages: 0311-0331, 0403-0412
extraction: native+ocr
subsections:
    - "no": 1
      title: THE GROUP X(H)
      page: 304
      pdf_page: 311
    - "no": 2
      title: NODAL GROUP OF A TORUS
      page: 305
      pdf_page: 312
    - "no": 3
      title: WEIGHTS OF A LINEAR REPRESENTATION
      page: 307
      pdf_page: 314
    - "no": 4
      title: ROOTS
      page: 309
      pdf_page: 316
    - "no": 5
      title: NODAL VECTORS AND INVERSE ROOTS
      page: 311
      pdf_page: 318
    - "no": 6
      title: FUNDAMENTAL GROUP
      page: 314
      pdf_page: 321
    - "no": 7
      title: SUBGROUPS OF MAXIMAL RANK
      page: 316
      pdf_page: 323
    - "no": 8
      title: ROOT DIAGRAMS
      page: 317
      pdf_page: 324
    - "no": 9
      title: COMPACT LIE GROUPS AND ROOT SYSTEMS
      page: 319
      pdf_page: 326
    - "no": 10
      title: AUTOMORPHISMS OF A CONNECTED COMPACT LIE GROUP
      page: 322
      pdf_page: 329
statements: 60
exercises: 22
content_sha256: bd4bd4714daf2f27be94b6fc189301f123d5a4c8ef1e6ac4e4232ecfa1434b9f
translated_from: content/en/lie/IX/04_s4_root_system_associated_to_a_compact.md
source_content_sha256: e5b8a3582b57fb78f4dd12b6e9730ed0ae0bc70a11963071c72fa1b2877b4759
translation_model: gpt-5.4-mini, gpt-5-mini, gpt-5-6-mini
translation_run: translate-vi-edc7dde8
glossary_version: 34
glossary_terms_sha256: 2a41e4f0ca3ffbcdf3a86e587b8dec1ff4d4c5121ab51eb9aa6b4015476f5ceb
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 4. HỆ CĂN NGHIỆM LIÊN KẾT VỚI MỘT NHÓM COMPACT

Trong các đoạn 4 đến 8, ta ký hiệu bởi G một nhóm Lie compact liên thông và bởi T một xuyến cực đại của G. Ta ký hiệu bởi $\mathfrak{g}$ (resp. $\mathfrak{t}$) đại số Lie của G (resp. T), bởi $\mathfrak{g}_{\mathbf{C}}$ (resp. $\mathfrak{t}_{\mathbf{C}}$) đại số Lie phức hóa của $\mathfrak{g}$ (resp. $\mathfrak{t}$), và bởi W nhóm Weyl của G tương đối với T (§2, no. 5).

### 1. NHÓM X(H)

Cho H là một nhóm Lie compact. Ký hiệu X(H) là nhóm (giao hoán) các đồng cấu liên tục từ H đến nhóm tôpô $\mathbf{C}^*$. Theo Chương III, §8, no. 1, Định lý 1, các phần tử của X(H) là các cấu xạ của nhóm Lie; với mọi $a\in X(H)$, vi phân của $a$ là một ánh xạ tuyến tính trên $\mathbf{R}$ $L(a) : L(H)\rightarrow L(\mathbf{C}^*)$. Từ đây về sau ta đồng nhất đại số Lie của $\mathbf{C}^*$ với $\mathbf{C}$ sao cho ánh xạ mũ của $\mathbf{C}^*$ trùng với ánh xạ $z \rightarrow e^z$ từ $\mathbf{C}$ đến $\mathbf{C}^*$. Khi đó, với mỗi phần tử $a\in X(H)$, ta gắn một phần tử $L(a)\in$ Hom$_{\mathbf{R}}(L(H),\mathbf{C})$; ta ký hiệu $\delta (a)$ là phần tử của Hom$_{\mathbf{C}}(L(H)_{(\mathbf{C})},\mathbf{C})$ tương ứng với nó (nghĩa là, phần tử có hạn chế lên $L(H)\subset L(H)_{(\mathbf{C})}$ bằng $L(a)$).

Với mọi $x\in L(H)$ và mọi $a\in X(H)$, ta có

$a$(exp$_Hx$) $=e^{\delta(a)(x)}$,

theo tính hàm tử của ánh xạ mũ (Chương III, §6, no. 4, Mệnh đề 10).

Ta sẽ thường ký hiệu nhóm X(H) theo phép cộng; trong trường hợp đó, ta ký hiệu phần tử $a(g)$ của $\mathbf{C}^*$ bởi $g^a$. Với ký hiệu này, ta có các công thức

$$
g^{a+b}=g^ag^b,g\in H, a, b\in X(H)
$$

và

(exp$_Hx$)$^a=e^{\delta(a)(x)}, x\in L(H), a\in X(H)$.

Vì H compact, các phần tử của X(H) nhận giá trị trong nhóm con $\mathbf{U}=\mathbf{U}(1,\mathbf{C})$ gồm các số phức có môđun 1, do đó X(H) có thể được đồng nhất với nhóm các đồng cấu liên tục (hoặc giải tích) từ H đến $\mathbf{U}$. Suy ra rằng, với mọi $a\in L(H)$, ánh xạ $L(a)$ nhận giá trị trong không gian con $\mathbf{R}i$ của $\mathbf{C}$, nên $\delta (a)$ ánh xạ L(H) vào $\mathbf{R}i$.

Nếu H giao hoán, X(H) đơn giản là nhóm đối ngẫu (rời rạc) của H (Spectral Theories, Chương II, §1, no. 1). Nếu H giao hoán và hữu hạn, X(H) có thể được đồng nhất với nhóm đối ngẫu hữu hạn D(H) = Hom$_{\mathbf{Z}}(H,\mathbf{Q}/\mathbf{Z})$ (trong đó, như trong Algebra, Chương VII, §4, no. 9, Ví dụ 1, ta đồng nhất $\mathbf{Q}/\mathbf{Z}$ với một nhóm con của $\mathbf{C}^*$ bởi đồng cấu $r \rightarrow$ exp(2$\pi ir$)).

Với mọi cấu xạ $f: H\rightarrow H'$ của các nhóm Lie compact, ta ký hiệu $X(f)$ là đồng cấu $a \rightarrow a\circ f$ từ $X(H')$ đến X(H). Nếu K là một nhóm con chuẩn đóng của nhóm Lie compact H, ta có một dãy khớp của các $\mathbf Z$-môđun
$$
0\longrightarrow X(H/K)\longrightarrow X(H)\longrightarrow X(K).
$$

#### Mệnh đề 1 {#lie-ix-s4-prop-1 .statement tag=01JH}

— *Với mọi nhóm Lie compact* H, *$\mathbf Z$-*môđun* $X(H)$ *là hữu hạn kiểu. Nó là tự do nếu* H *liên thông.*

Trước hết giả sử rằng H liên thông; mọi phần tử của $X(H)$ triệt tiêu trên nhóm dẫn xuất $D(H)$ của H, do đó ta có một đồng cấu $X(H/D(H))\longrightarrow X(H)$. Nhưng $H/D(H)$ liên thông và giao hoán, nên là một xuyến, và $X(H/D(H))$ là một $\mathbf Z$-môđun tự do thuộc kiểu hữu hạn (*Spectral Theories*, Chap. II, §2, no. 1, Cor. 2 of Prop. 1). Trong trường hợp tổng quát, từ tính chính xác của dãy
$$
0\longrightarrow X(H/H_0)\longrightarrow X(H)\longrightarrow X(H_0),
$$
trong đó $X(H_0)$ là tự do thuộc kiểu hữu hạn và $X(H/H_0)$ là hữu hạn, suy ra rằng $X(H)$ thuộc kiểu hữu hạn.

#### Mệnh đề 2 {#lie-ix-s4-prop-2 .statement tag=01JI}

— *Cho* H *là một nhóm Lie compact giao hoán, và* $(a_i)_{i\in I}$ *là một họ các phần tử của* $X(H)$; *các* $a_i$ *sinh ra* $X(H)$ *khi và chỉ khi giao của các* $\operatorname{Ker}a_i$ *thu gọn thành phần tử đơn vị.*

Theo *Spectral Theories*, Chap. II, §1, no. 7, Th. 4, phần bù trực giao của hạt nhân của $a_i$ là nhóm con $A_i$ của $X(H)$ được sinh bởi $a_i$; theo *loc. cit.*, Cor. 2 of Th. 4, phần bù trực giao của $\bigcap\operatorname{Ker}a_i$ là nhóm con của $X(H)$ được sinh bởi các $A_i$, do đó có mệnh đề.

### 2. NHÓM NÚT CỦA MỘT XUYẾN

*Nhóm nút* của một xuyến S, ký hiệu bởi $\Gamma(S)$, là hạt nhân của ánh xạ mũ $\mathscr L(S)\longrightarrow S$. Đây là một nhóm con rời rạc của $\mathscr L(S)$, có hạng bằng chiều của S, và ánh xạ tuyến tính $\mathbf R$ $\mathbf R\otimes_{\mathbf Z}\Gamma(S)\longrightarrow\mathscr L(S)$ kéo dài đơn ánh chính tắc của $\Gamma(S)$ vào $\mathscr L(S)$ là song ánh. Nó cảm sinh, qua phép lấy thương, một đẳng cấu
$$
\mathbf R/\mathbf Z\otimes_{\mathbf Z}\Gamma(S)\longrightarrow S.
$$

Ví dụ, nhóm nút $\Gamma(\mathbf U)$ của $\mathbf U$ là nhóm con $2\pi i\mathbf Z$ của $\mathscr L(\mathbf U)=i\mathbf R$.

Đối với mọi cấu xạ của các xuyến $f:S\longrightarrow S'$, ký hiệu $\Gamma(f)$ là đồng cấu $\Gamma(S)\longrightarrow\Gamma(S')$ cảm sinh bởi $L(f)$. Ta có một biểu đồ giao hoán
$$
\begin{array}{ccccccccc}
0&\longrightarrow&\Gamma(S)&\longrightarrow&\mathscr L(S)&\xrightarrow{\exp_S}&S&\longrightarrow&0\\
&&\downarrow{\Gamma(f)}&&\downarrow{\mathscr L(f)}&&\downarrow f&&\\
0&\longrightarrow&\Gamma(S')&\longrightarrow&\mathscr L(S')&\xrightarrow{\exp_{S'}}&S'&\longrightarrow&0.
\end{array}
\tag{1}
$$

Cho $a\in X(S)$; áp dụng điều đã nói trước cho cấu xạ từ S đến $\mathbf U$ được định nghĩa bởi a, ta thấy rằng ánh xạ tuyến tính $\mathbf C$ $\delta(a):\mathscr L(S)_{\mathbf C}\longrightarrow\mathbf C$ ở no. 1 biến $\Gamma(S)$ thành $2\pi i\mathbf Z$. Vì vậy, ta có thể định nghĩa một dạng $\mathbf Z$-song tuyến tính trên $X(S)\times\Gamma(S)$ bằng cách đặt
$$
\langle a,X\rangle=\frac{1}{2\pi i}\delta(a)(X),\qquad a\in X(S),\quad X\in\Gamma(S).
\tag{2}
$$

#### Mệnh đề 3 {#lie-ix-s4-prop-3 .statement tag=01BP}

Dạng song tuyến tính $(a, X) \rightarrow  \langle a, X\rangle$ trên $X(S)\times \Gamma (S)$ là khả nghịch.

Nhắc lại (Algebra, Chap. IX) rằng, theo định nghĩa, điều này có nghĩa là các ánh xạ tuyến tính $X(S)\rightarrow$ Hom$_{\mathbf{Z}}(\Gamma (S),\mathbf{Z})$ và $\Gamma (S)\rightarrow$ Hom$_{\mathbf{Z}}(X(S),\mathbf{Z})$ liên kết với dạng song tuyến tính này là song ánh.

Hiển nhiên rằng nếu kết luận của mệnh đề đúng cho hai xuyến, thì nó cũng đúng cho tích của chúng. Vì mọi xuyến có chiều $n$ đều đẳng cấu với $\mathbf{U}^n$, ta quy về trường hợp $S =\mathbf{U}$. Trong trường hợp riêng này, mệnh đề là hiển nhiên.

Cho $f: S\rightarrow S'$ là một cấu xạ của các xuyến. Khi đó, mỗi ánh xạ tuyến tính $X(f) : X(S')\rightarrow X(S)$ và $\Gamma (f) :\Gamma (S)\rightarrow \Gamma (S')$ là chuyển vị của ánh xạ kia: với mọi $a'\in X(S')$ và mọi $X\in \Gamma$(S),

$$
\langle X(f)(a'), X\rangle =\langle a', \Gamma (f)(X)\rangle \tag{3}
$$

#### Mệnh đề 4 {#lie-ix-s4-prop-4 .statement tag=01BQ}

Cho S và $S'$ là các xuyến. Ký hiệu $M(S,S')$ là nhóm các cấu xạ của các nhóm Lie từ S đến $S'$. Các ánh xạ $f \rightarrow X(f)$ và $f \rightarrow \Gamma (f)$ là các đẳng cấu của các nhóm từ $M(S,S')$ đến Hom$_{\mathbf{Z}}(X(S'),X(S))$ và đến Hom$_{\mathbf{Z}}(\Gamma (S), \Gamma (S'))$, tương ứng.

Nếu $f$ là một cấu xạ của các nhóm Lie từ S đến $S'$, đồng cấu $X(f)$ chính là đối ngẫu của $f$ theo nghĩa của Spectral Theories, Chap. II, §1, no. 7. Ánh xạ $\varphi  \rightarrow \widehat{\varphi}$ từ Hom$_{\mathbf{Z}}(X(S'),X(S))$ đến $M(S,S')$ được định nghĩa trong loc. cit. là nghịch đảo của ánh xạ $f \rightarrow X(f)$ từ $M(S,S')$ đến Hom$_{\mathbf{Z}}(X(S'),X(S))$; ánh xạ sau do đó là song ánh. Nếu ta đồng nhất $\Gamma (S)$ (resp. $\Gamma (S')$) với môđun $\mathbf{Z}$ đối ngẫu của X(S) (resp. $X(S')$) (Prop. $3$)$,\Gamma (f)$ trùng với chuyển vị của đồng cấu $X(f)$, do đó có mệnh đề.

#### Nhận xét 1 {#lie-ix-s4-n2-rem-1 .statement tag=01BR}

Cho $f$ : S $\rightarrow S'$ là một cấu xạ của các xuyến. Biểu đồ rắn (Algebra, Chap. X, §1, no. 2) liên kết với (1) cho một dãy khớp

0 $\longrightarrow$ Ker$\Gamma (f)\longrightarrow$ Ker $L(f)\longrightarrow$ Ker $f\longrightarrow^d$ (4)

$\longrightarrow^d$ Coker $\Gamma (f)\longrightarrow$ Coker $L(f)\longrightarrow$ Coker $f\longrightarrow 0$.

Đặc biệt, giả sử rằng $f$ là toàn ánh, với hạt nhân hữu hạn N, sao cho ta có một dãy khớp

0 $\longrightarrow$ N $\longrightarrow^i$ S $\longrightarrow^fS'\longrightarrow 0$,

trong đó $i$ là đơn ánh chính tắc. Khi đó, $L(f)$ là song ánh, và (4) cho một đẳng cấu $N\rightarrow$ Coker $\Gamma (f)$, do đó có một dãy khớp

0 $\longrightarrow \Gamma (S)\overset{\Gamma(f)}{\longrightarrow}\Gamma (S')\longrightarrow$ N $\longrightarrow 0$. (5)

Ngoài ra, theo Spectral Theories, Chap. II, §1, no. 7, Th. 4, dãy

0 $\longrightarrow X(S')\overset{X(f)}{\longrightarrow}$ X(S) $\longrightarrow^{X(i)}$ X(N) $\longrightarrow$ 0 (6)

là khớp.

#### Nhận xét 2 {#lie-ix-s4-n2-rem-2 .statement tag=01BS}

Theo Mệnh đề 4, ánh xạ $f \rightarrow \Gamma (f)(2\pi i)$ từ $M(\mathbf{U},S)$ đến $\Gamma (S)$ là một đẳng cấu; nếu $a\in X(S) = M(S,\mathbf{U})$ và $f\in M(\mathbf{U},S)$, thì ánh xạ hợp $a\circ f\in M(\mathbf{U},\mathbf{U})$ là tự đồng cấu $u \rightarrow u^r$, trong đó $r=\langle a, \Gamma (f)(2\pi i)\rangle$. Từ nay ta sẽ đồng nhất $M(\mathbf{U},\mathbf{U}) = X(\mathbf{U})$ với $\mathbf{Z}$, phần tử $r$ của $\mathbf{Z}$ được liên kết với tự đồng cấu $u \rightarrow u^r$; do đó, với các ký hiệu ở trên,

$$
a\circ f=\langle a, \Gamma (f)(2\pi i)\rangle
$$

#### Nhận xét 3 {#lie-ix-s4-n2-rem-3 .statement tag=01BT}

Với dãy khớp $0\rightarrow \Gamma (S)\rightarrow L(S)\longrightarrow^{exp_S}S\rightarrow 0$ được liên kết một đẳng cấu từ $\Gamma (S)$ vào nhóm cơ bản của S, được gọi là chính tắc trong phần sau. Với mọi cấu xạ của các xuyến $f: S\rightarrow S',\Gamma (f)$ khi đó có thể được đồng nhất thông qua các đẳng cấu chính tắc $\Gamma (S)\rightarrow \pi_1(S)$ và $\Gamma (S')\rightarrow \pi_1(S')$ với đồng cấu $\pi_1(f) :\pi_1(S)\rightarrow \pi_1(S')$ cảm sinh bởi $f$. Chú ý rằng điều này cho một cách hiểu khác về dãy khớp (5) (xem Tôpô đại cương, Chương XI, đang chuẩn bị).

#### Nhận xét 4 {#lie-ix-s4-n2-rem-4 .statement tag=01BU}

Các đồng cấu của các $\mathbf{Z}$-môđun $\delta : X(S)\rightarrow$ Hom$_{\mathbf{C}}(L(S)_{(\mathbf{C})},\mathbf{C})$ và $\iota :\Gamma (S)\rightarrow L(S)_{(\mathbf{C})}(\iota$ được cảm sinh bởi đơn ánh chính tắc của $\Gamma (S)$ vào L(S)) mở rộng thành các đẳng cấu của các không gian vectơ $\mathbf{C}$

$u:\mathbf{C}\otimes X(S)\rightarrow$ Hom$_{\mathbf{C}}(L(S)_{(\mathbf{C})},\mathbf{C})$

$$
v:\mathbf{C}\otimes \Gamma (S)\rightarrow L(S)_{(\mathbf{C})}
$$

mà ta sẽ gọi là chính tắc trong phần sau. Chú ý rằng, nếu ta mở rộng cặp ghép giữa X(S) và $\Gamma (S)$ bởi tính $\mathbf{C}$-tuyến tính thành một dạng song tuyến tính $\ll ,\gg$ trên $(\mathbf{C}\otimes X(S))\times (\mathbf{C}\otimes \Gamma$(S)), thì

$$
\langle u(a), v(b)\rangle = 2\pi i\ll a, b\gg
$$

### 3. CÁC TRỌNG SỐ CỦA MỘT BIỂU DIỄN TUYẾN TÍNH

Trong số này $k$ ký hiệu một trong các trường $\mathbf{R}$ hoặc $\mathbf{C}$.

Cho V là một không gian vectơ hữu hạn chiều trên $k$, và $\rho : G\rightarrow \mathbf{G}\mathbf{L}(V)$ là một biểu diễn liên tục (do đó giải tích thực, Chương III, §8, no. 1, Định lý 1) của nhóm Lie compact liên thông G trên V. Định nghĩa một không gian vectơ phức $\widetilde{V}$ và một biểu diễn liên tục $\widetilde{\rho}: G\rightarrow \mathbf{G}\mathbf{L}( \widetilde{V})$ như sau: nếu $k=\mathbf{C}$, đặt $\widetilde{V} = V, \widetilde{\rho}=\rho$; nếu $k=\mathbf{R}$, đặt $\widetilde{V} = V_{(\mathbf{C})}$ và $\widetilde{\rho}$ là ánh xạ hợp của $\rho$ với đồng cấu chính tắc $\mathbf{G}\mathbf{L}(V)\rightarrow \mathbf{G}\mathbf{L}( \widetilde{V})$.

Với mọi $\lambda \in X(G)$, ký hiệu $\widetilde{V}_{\lambda}(G)$ là không gian con vectơ của $\widetilde{V}$ gồm các $v\in \widetilde{V}$ sao cho $\widetilde{\rho}(g)v=g^{\lambda}v$ với mọi $g\in G$ (xem Chương VII, §1, no. 1). Theo chỗ đã dẫn, Mệnh đề 3, tổng của các $\widetilde{V}_{\lambda}(G)$ (với $\lambda$ thuộc X(G)) là trực tiếp. Hơn nữa:

#### Bổ đề 1 {#lie-ix-s4-lem-1 .statement tag=01BV}

Nếu G giao hoán, $\widetilde{V}$ là tổng trực tiếp của các $\widetilde{V}_{\lambda}(G)$ với $\lambda \in X(G)$.

Vì $\rho$ là nửa đơn (§1, no. 1), chỉ cần chứng minh bổ đề trong trường hợp $\rho$ là đơn. Trong trường hợp đó, hoán tập Z của $\rho (G)$ trong End( $\widetilde{V}$) chỉ gồm các phép vị tự (Đại số, Chương VIII, §3, no. 2, Định lý 1); do đó, ảnh của đồng cấu $\widetilde{\rho}$ được chứa trong nhóm con $\mathbf{C}^*.1_V$ của GL( $\widetilde{V}$), và tồn tại $\lambda \in X(G)$ sao cho $\widetilde{V} = \widetilde{V}_{\lambda}(G)$.

#### Định nghĩa 1 {#lie-ix-s4-def-1 .statement tag=01BW}

Các trọng số của biểu diễn $\rho$ của G, đối với một xuyến cực đại T của G, là các phần tử $\lambda$ của X(T) sao cho $\widetilde{V}_{\lambda}(T)\not= 0$.

Ký hiệu bởi $P(\rho ,T)$, hoặc bởi $P(\rho )$ nếu không có khả năng nhầm lẫn về lựa chọn T, tập hợp các trọng số của $\rho$ đối với T. Theo Bổ đề 1,

$$
\widetilde{V} =\bigoplus_{\lambda\in P(\rho ,T)}\widetilde{V}_{\lambda}(T) \tag{7}
$$

Cho $T'$ là một xuyến cực đại khác của G và $g$ là một phần tử của G sao cho (Int $g$)$T = T'($§2, no. 2, Định lý 2). Với mọi $\lambda \in X(T)$,

$\widetilde{\rho}(g)( \widetilde{V}_{\lambda}(T)) = \widetilde{V}_{\lambda'}(T')$, trong đó $\lambda '=$ X(Int $g^{-1}$)$(\lambda )$. (8)

Do đó,

X(Int $g$)$(P(\rho ,T')) = P(\rho ,T)$. (9)

Nhóm Weyl $W = W_G(T)$ tác động bên trái trên $\mathbf{Z}$-môđun X(T) bởi $w \rightarrow X(w^{-1})$; do đó, với $t\in T, \lambda \in X(T), w\in W$, ta có $t^{w\lambda}= (w^{-1}(t))^{\lambda}$.

#### Mệnh đề 5 {#lie-ix-s4-prop-5 .statement tag=01BX}

Tập hợp $P(\rho ,T)$ ổn định dưới phép toán của nhóm Weyl W. Cho $n\in N_G(T)$, và cho $w$ là lớp của nó trong W; với $\lambda \in X(T)$, ta có $\rho (n)( \widetilde{V}_{\lambda}(T)) = \widetilde{V}_{w\lambda}(T)$ và dim $\widetilde{V}_{w\lambda}(T) =$ dim $\widetilde{V}_{\lambda}(T)$.

Công thức (9), với $T'= T, g=n$, suy ra rằng $P(\rho ,T)$ ổn định dưới $w$; hơn nữa, $\widetilde{\rho}(n)$ cảm sinh một đẳng cấu từ $\widetilde{V}_{\lambda}(T)$ đến $\widetilde{V}_{w\lambda}(T)$ (công thức (8)), do đó suy ra mệnh đề.

#### Mệnh đề 6 {#lie-ix-s4-prop-6 .statement tag=01BY}

Đồng cấu $\rho : G\rightarrow \mathbf{G}\mathbf{L}(V)$ là đơn ánh khi và chỉ khi $P(\rho ,T)$ sinh ra $\mathbf{Z}$-môđun X(T).

Đồng cấu $\rho$ là đơn ánh khi và chỉ khi hạn chế của nó vào T là đơn ánh (§2, no. 6, Mệnh đề 9). Hơn nữa, vì đồng cấu chính tắc $\mathbf{G}\mathbf{L}(V)\rightarrow \mathbf{G}\mathbf{L}( \widetilde{V})$ là đơn ánh, ta có thể thay thế $\rho$ bởi $\widetilde{\rho}$. Khi đó từ (7) suy ra rằng hạt nhân của hạn chế của $\rho$ vào T là giao của các hạt nhân của các phần tử của $P(\rho ,T)$. Do đó, kết luận suy ra từ Mệnh đề 2 của no. 1.

Biểu diễn tuyến tính $L(\rho )$ của $\mathfrak{t}$ trong $\mathfrak{g}\mathfrak{l}( \widetilde{V})$ mở rộng thành một đồng cấu của các đại số Lie-$\mathbf{C}$

$$
\widetilde{L}(\rho ) :\mathfrak{t}_{\mathbf{C}}\rightarrow \mathfrak{g}\mathfrak{l}( \widetilde{V})
$$

Hơn nữa, nhắc lại (no. 1) rằng ta đã liên kết với mỗi phần tử $\lambda$ của X(T) một dạng tuyến tính $\delta (\lambda )$ trên $\mathfrak{t}_{\mathbf{C}}$ sao cho

(exp$_Tx$)$^{\lambda}=e^{\delta(\lambda)(x)},x\in \mathfrak{t}$. (10)

Cuối cùng nhắc lại rằng (Chương VII, §1, no. 1), đối với mọi ánh xạ $\mu:\mathfrak{t}_{\mathbf{C}}\rightarrow \mathbf{C}$, ta ký hiệu bởi $\widetilde{V}_\mu(\mathfrak{t}_{\mathbf{C}})$ không gian vectơ con của $\widetilde{V}$ gồm các $v$ sao cho $(\widetilde{L}(\rho )(u))(v) =\mu(u).v$ với mọi $u\in \mathfrak{t}_{\mathbf{C}}$.

Bây giờ ta suy ra từ (7) và loc. cit., Mệnh đề 3:

#### Mệnh đề 7 {#lie-ix-s4-prop-7 .statement tag=01BZ}

a) Với mọi $\lambda \in X(T)$, ta có $\widetilde{V}_{\lambda}(T) = \widetilde{V}_{\delta(\lambda)}(\mathfrak{t}_{\mathbf{C}})$.

b) Ánh xạ $\delta : X(T)\rightarrow$ Hom$_{\mathbf{C}}(\mathfrak{t}_{\mathbf{C}},\mathbf{C})$ cảm sinh một song ánh từ $P(\rho ,T)$ lên tập hợp các trọng số của $\mathfrak{t}_{\mathbf{C}}$ trên $\widetilde{V}$.

Trước hết hãy lưu ý rằng, nếu W tác động trên $\mathfrak{t}_{\mathbf{C}}$ bằng cách liên kết với mỗi phần tử $w$ của W tự đồng cấu $L(w)_{(\mathbf{C})}$ của $\mathfrak{t}_{\mathbf{C}}$, thì ánh xạ $\delta$ tương thích với phép toán của W trên X(T) và Hom$_{\mathbf{C}}(\mathfrak{t}_{\mathbf{C}},\mathbf{C})$.

Bây giờ giả sử rằng $k=\mathbf{R}$. Ký hiệu bởi $\sigma$ phép liên hợp của $\widetilde{V}$ đối với V, được xác định bởi $\sigma (x+iy) =x-iy$ với $x, y$ thuộc V; đối với mỗi không gian vectơ phức con E của $\widetilde{V}$, không gian con nhỏ nhất của $\widetilde{V}$ hữu tỉ trên $\mathbf{R}$ và chứa E là $E +\sigma (E)$. Đặc biệt, với mọi $\lambda \in X(T)$, tồn tại một không gian vectơ thực con $V(\lambda )$ của V sao cho không gian con $V(\lambda )_{(\mathbf{C})}$ của $\widetilde{V}$ là $\widetilde{V}_{\lambda}(T) + \widetilde{V}_{-\lambda}(T)$ (lưu ý rằng $\sigma ( \widetilde{V}_{\lambda}(T)) = \widetilde{V}_{-\lambda}(T)$). Ta có $V(\lambda ) = V(-\lambda )$, và các $V(\lambda )$ là các thành phần đẳng kiểu của biểu diễn của T trên V cảm sinh bởi $\rho$.

### 4. CÁC NGHIỆM

Các nghiệm của G đối với T là các trọng số khác không của biểu diễn phụ hợp của G. Tập hợp các nghiệm của G đối với T được ký hiệu bởi $R(G,T)$, hoặc đơn giản bởi R nếu không có nguy cơ nhầm lẫn. Theo Mệnh đề 6, ánh xạ

$$
\delta : X(T)\rightarrow \mathfrak{t}^*_{\mathbf{C}}
$$

$(\mathfrak{t}^*_{\mathbf{C}}$ ký hiệu đối ngẫu của không gian vectơ phức $\mathfrak{t}_{\mathbf{C}})$ ánh xạ $R(G,T)$ song ánh lên tập hợp $R(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}})$ các nghiệm của đại số khả quy tách $(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}})$ (Chương VIII, §2, no. 2, Nhận xét 4). Nếu đặt

$$
\mathfrak{g}^{\alpha}= (\mathfrak{g}_{\mathbf{C}})_{\alpha}(T) = (\mathfrak{g}_{\mathbf{C}})_{\delta(\alpha)}(\mathfrak{t}_{\mathbf{C}}) \tag{11}
$$

với mọi $\alpha \in R$, thì mỗi $\mathfrak{g}^{\alpha}$ có chiều 1 trên $\mathbf{C}($loc. cit., Định lý 1) và

$$
\mathfrak{g}_{\mathbf{C}}=\mathfrak{t}_{\mathbf{C}}\oplus \bigoplus_{\alpha\in R}\mathfrak{g}^{\alpha} \tag{12}
$$

Với mỗi $\alpha \in R$, ký hiệu $V(\alpha )$ là không gian con 2 chiều của $\mathfrak{g}$ sao cho $V(\alpha )_{(\mathbf{C})}=\mathfrak{g}^{\alpha}+\mathfrak{g}^{-\alpha}$; các thành phần đẳng kiểu khác không của $\mathfrak{g}$ đối với biểu diễn phụ hợp của T là $\mathfrak{t}$ và các $V(\alpha )$. Hơn nữa, gọi K là dạng toàn phương liên kết với dạng Killing của $\mathfrak{g}$; nó âm (§1, no. 3, Mệnh đề 1) và hạn chế của nó $K(\alpha )$ trên $V(\alpha )$ là âm và tách. Với mỗi phần tử $t$ của T, Ad $t$ giữ $K(\alpha )$ ổn định, và do đó cho một cấu xạ của các nhóm Lie

$$
\iota_{\alpha}: T\rightarrow \mathbf{S}\mathbf{O}(K(\alpha ))
$$

Tồn tại một đẳng cấu duy nhất $\rho_{\alpha}:\mathbf{U}\rightarrow \mathbf{S}\mathbf{O}(K(\alpha ))$ sao cho $\iota_{\alpha}=\rho_{\alpha}\circ \alpha$. Thật vậy, cho $X$ là một phần tử khác không của $\mathfrak{g}^{\alpha}$, và gọi $Y$ là ảnh của $X$ qua phép liên hợp của $\mathfrak{g}_{\mathbf{C}}$ đối với $\mathfrak{g}$; khi đó $Y\in \mathfrak{g}^{-\alpha}$, và ta thu được một cơ sở $(U, V)$ của $V(\alpha )$ bằng cách đặt $U=X+Y, V=i(X-Y)$; ma trận của tự đồng cấu của $V(\alpha )$ cảm sinh bởi Ad $t,t\in T$, đối với cơ sở $(U, V)$ là

$$
(\mathscr{R}(t^{\alpha})-\mathscr{I}(t^{\alpha}))
$$

$$
\mathscr{I}(t^{\alpha})\mathscr{R}(t^{\alpha})
$$

do đó có mệnh đề.

#### Mệnh đề 8 {#lie-ix-s4-prop-8 .statement tag=01C0}

Cho Q(R) là nhóm con của X(T) sinh bởi các căn của G.

a) Tâm C(G) của G là một nhóm con đóng của T, bằng giao của các hạt nhân của các căn. Ánh xạ chính tắc $X(T/C(G))\rightarrow X(T)$ là đơn ánh với ảnh Q(R).

b) Nhóm compact C(G) đẳng cấu với đối ngẫu của nhóm rời rạc $X(T)/Q(R) ($Spectral Theories, Chap. II, §1, no. 1, Def. 2).

c) C(G) thu gọn về phần tử đơn vị khi và chỉ khi Q(R) bằng X(T).

Theo §2, no. 2, Hệ quả 2 của Định lý 2, C(G) được chứa trong T. Vì đây là hạt nhân của biểu diễn phụ hợp, nó là giao của các hạt nhân của các căn, nói cách khác là phần bù trực giao của nhóm con Q(R) của X(T). Do đó, mệnh đề suy ra từ Spectral Theories, Chap. II, §1, no. 7, Định lý 4 và no. 5, Định lý 2.

#### Mệnh đề 9 {#lie-ix-s4-prop-9 .statement tag=01C1}

Mọi tự đẳng cấu của nhóm Lie G cảm sinh đồng nhất trên T đều có dạng Int $t$, với $t\in T$.

Trước hết, giả sử rằng C(G) thu gọn về phần tử đơn vị, nói cách khác X(T) = Q(R) (Mệnh đề 8). Cho $f$ là một tự đẳng cấu của G cảm sinh đồng nhất trên T, và $\varphi = L(f)_{(\mathbf{C})}$; khi đó $\varphi$ là một tự đẳng cấu của $\mathfrak{g}_{\mathbf{C}}$ cảm sinh đồng nhất trên $\mathfrak{t}_{\mathbf{C}}$. Theo Chap. VIII, §5, no. 2, Mệnh đề 2, tồn tại một đồng cấu duy nhất $\theta : Q(R)\rightarrow \mathbf{C}^*$ sao cho $\varphi$ cảm sinh trên mỗi $\mathfrak{g}^{\alpha}$ phép vị tự với tỉ số $\theta (\alpha )$. Vì $\varphi$ giữ dạng thực $\mathfrak{g}$ của $\mathfrak{g}_{\mathbf{C}}$ ổn định, nó giao hoán với phép liên hợp $\sigma$ của $\mathfrak{g}_{\mathbf{C}}$ đối với $\mathfrak{g}$; nhưng $\sigma (\mathfrak{g}^{\alpha}) =\mathfrak{g}^{-\alpha}$, nên $\theta (-\alpha ) =\overline{\theta(\alpha)}$ với mọi $\alpha \in R$. Điều này suy ra rằng $\theta (\alpha )\theta (\alpha ) =\theta (\alpha )\theta (-\alpha ) = 1$. Suy ra $\theta$ nhận giá trị trong $\mathbf{U}$, và do đó tương ứng qua đối ngẫu với một phần tử $t$ của T sao cho (Ad $t$)$_{(\mathbf{C})}=\varphi$, vậy Int $t=f$.

Trong trường hợp tổng quát, điều nói trên áp dụng cho nhóm $G/C(G)$, có tâm thu gọn về phần tử đơn vị, và cho xuyến cực đại $T/C(G)$. Suy ra rằng, nếu $f$ là một tự đẳng cấu của G cảm sinh tự đồng nhất trên T, thì tồn tại một phần tử $t$ của T sao cho $f$ và Int $t$ cảm sinh qua phép đi qua thương cùng một tự đẳng cấu của $G/C(G)$. Nhưng, vì cấu xạ chính tắc $D(G)\rightarrow G/C(G)$ là một phủ hữu hạn (§1, no. 4, Hệ quả 1 của Mệnh đề 4), $f$ và Int $t$ cảm sinh cùng một tự đẳng cấu của D(G), do đó của $D(G)\times C(G)$, và do đó cũng của G (loc. cit.).

#### Hệ quả {#lie-ix-s4-n4-cor-1 .statement tag=01C2}

Cho $u$ là một tự đẳng cấu của G và H là nhóm con đóng của G gồm các điểm bất động của $u$. Khi đó, tự đẳng cấu $u$ là nội khi và chỉ khi $H_0$ có hạng cực đại.

Nếu $u$ bằng Int $g$, với $g\in G$, nhóm con $H_0= Z(g)_0$ có hạng cực đại (§2, no. 2, Hệ quả 3). Ngược lại, nếu H chứa một xuyến cực đại S, tự đẳng cấu $u$ có dạng Int $s$ với $s\in S$ (Mệnh đề 9).

### 5. VECTƠ NÚT VÀ CÁC CĂN NGHỊCH ĐẢO

#### Bổ đề 2 {#lie-ix-s4-lem-2 .statement tag=01C3}

Cho S là một nhóm con đóng của T và Z(S) là chuẩn hóa tử của nó trong G.

(i) $R(Z(S)_0,T)$ là tập hợp các $\alpha \in R(G,T)$ sao cho $\alpha (S) =\{1\}$.

(ii) Tâm của $Z(S)_0$ là giao của các Ker$\alpha$ với $\alpha \in R(Z(S)_0,T)$.

(iii) Nếu S liên thông, Z(S) liên thông.

Đại số Lie $L(Z(S))_{(\mathbf{C})}$ gồm các bất biến của S trên $\mathfrak{g}_{\mathbf{C}}$ (Chương III, §9, no. 3, Mệnh đề 8), và do đó là tổng trực tiếp của $\mathfrak{t}_{\mathbf{C}}$ và các $\mathfrak{g}^{\alpha}$ mà $\alpha (S) =\{1\}$, do đó suy ra (i). Mệnh đề (ii) suy ra từ Mệnh đề 8 (no. 4), và mệnh đề (iii) đã được chứng minh (§2, no. 2, Hệ quả 5 của Định lý 2).

#### Định lý 1 {#lie-ix-s4-thm-1 .statement tag=01C4}

Cho $\alpha \in R(G,T)$. Tâm hóa tử $Z_{\alpha}$ của hạt nhân của $\alpha$ là một nhóm con đóng liên thông của G; tâm của nó là Ker $\alpha$; nhóm dẫn xuất của nó $D(Z_{\alpha}) = S_{\alpha}$ là một nhóm con nửa đơn đóng liên thông của G có hạng 1. Ta có $R(Z_{\alpha},T) =\{\alpha ,-\alpha \}$ và dim $Z_{\alpha}=$ dim T + 2.

Gọi $Z'_{\alpha}$ là tâm hóa tử của (Ker $\alpha$ )$_0$. Theo Bổ đề 2, đây là một nhóm con đóng liên thông của G, và $R(Z'_{\alpha},T)$ là tập hợp các $\beta \in R(G,T)$ sao cho $\beta$((Ker$\alpha$ )$_0$) $=\{1\}$. Rõ ràng, $\{\alpha ,-\alpha \} \subset R(Z'_{\alpha},T)$. Ngược lại, cho $\beta \in R(Z'_{\alpha},T)$; vì (Ker $\alpha$ )$_0$ có chỉ số hữu hạn trong Ker $\alpha$, tồn tại một số nguyên $r\not= 0$ sao cho $t^{r\beta}= 1$ với $t\in$ Ker $\alpha$. Từ tính chính xác của dãy

$0\longrightarrow \mathbf{Z}\longrightarrow X(T)\longrightarrow$ X(Ker $\alpha$ )$\longrightarrow 0$

tương ứng theo đối ngẫu với dãy khớp

0 $\longrightarrow$ Ker$\alpha \longrightarrow$ T $\longrightarrow^{\alpha}\mathbf{U}\longrightarrow 0$,

suy ra rằng $r\beta$ là một bội của $\alpha$; theo Chương VIII, §2, no. 2, ĐL. 2 (i), điều này suy ra rằng $\beta \in  \{\alpha ,-\alpha \}$. Do đó, $R(Z'_{\alpha},T) =\{\alpha ,-\alpha \}$. Suy ra (Bổ đề 2) tâm của $Z'_{\alpha}$ là Ker$\alpha$, nên $Z'_{\alpha}= Z_{\alpha}$. Cuối cùng, theo Hệ quả 1 của Mệnh đề 4 (§1, no. 4), $D(Z_\alpha)$ là một nhóm con nửa đơn, đóng và liên thông của $G$; nó có hạng $1$ vì $\mathscr{L}(Z_\alpha)(\mathbf C)=\mathfrak{g}^\alpha+\mathfrak{g}^{-\alpha}+[\mathfrak{g}^\alpha,\mathfrak{g}^{-\alpha}]$.

#### Hệ quả {#lie-ix-s4-n5-cor-1 .statement tag=01C7}

— *Tồn tại một cấu xạ của nhóm Lie* $\nu:\mathbf{SU}(2,\mathbf C)\to G$ *với các tính chất sau:*

a) *Ảnh của* $\nu$ *giao hoán với hạt nhân của* $\alpha$.

b) *Với mọi* $a\in\mathbf U$, *ta có*
$$
\nu\begin{pmatrix}a&0\\0&\bar a\end{pmatrix}\in\mathbf T
\quad\text{và}\quad
\alpha\circ\nu\begin{pmatrix}a&0\\0&\bar a\end{pmatrix}=a^2.
$$

*Nếu* $\nu_1$ *và* $\nu_2$ *là hai cấu xạ từ* $\mathbf{SU}(2,\mathbf C)$ *đến* $G$ *thỏa các tính chất trên, thì tồn tại* $a\in\mathbf U$ *sao cho*
$$
\nu_2=\nu_1\circ\operatorname{Int}
\begin{pmatrix}a&0\\0&\bar a\end{pmatrix}.
$$

Theo ĐL. 1 và Mệnh đề 6 của §3, no. 6, tồn tại một cấu xạ của nhóm Lie
$$
\nu:\mathbf{SU}(2,\mathbf C)\to S_\alpha
$$
toàn ánh với hạt nhân rời rạc. Khi đó $\nu^{-1}(\mathbf T\cap S_\alpha)$ là một xuyến cực đại của $\mathbf{SU}(2,\mathbf C)$ (§2, no. 3, Mệnh đề 1). Vì các xuyến cực đại của $\mathbf{SU}(2,\mathbf C)$ là liên hợp (§2, no. 2, ĐL. 2), ta có thể giả sử, nếu cần thay $\nu$ bởi $\nu\circ\operatorname{Int}s$ (với $s\in\mathbf{SU}(2,\mathbf C)$), rằng $\nu^{-1}(\mathbf T\cap S_\alpha)$ là nhóm các ma trận đường chéo trong $\mathbf{SU}(2,\mathbf C)$. Khi đó
$$
\nu\begin{pmatrix}a&0\\0&\bar a\end{pmatrix}\in\mathbf T
$$
với mọi $a\in\mathbf U$, và ánh xạ
$$
\begin{pmatrix}a&0\\0&\bar a\end{pmatrix}
\longmapsto
\alpha\circ\nu\begin{pmatrix}a&0\\0&\bar a\end{pmatrix}
$$
là một nghiệm của $\mathbf{SU}(2,\mathbf C)$, và do đó bằng một trong hai ánh xạ
$$
\begin{pmatrix}a&0\\0&\bar a\end{pmatrix}\longmapsto a^2
$$
hoặc
$$
\begin{pmatrix}a&0\\0&\bar a\end{pmatrix}\longmapsto a^{-2}
$$
(§3, no. 6, các công thức (19)). Trong trường hợp thứ nhất, đồng cấu $\nu$ có các tính chất yêu cầu; trong trường hợp thứ hai, đồng cấu $\nu\circ\operatorname{Int}\theta$ có chúng (ở chỗ đã dẫn, các công thức (18)).

Nếu $\nu_1$ và $\nu_2$ là hai cấu xạ từ $\mathbf{SU}(2,\mathbf C)$ đến $G$ thỏa các điều kiện đã nêu, thì cả hai đều gửi $\mathbf{SU}(2,\mathbf C)$ vào $S_\alpha$ (điều kiện a)), do đó cả hai đều là các bao phủ phổ quát của $S_\alpha$. Suy ra, tồn tại một tự đẳng cấu $\varphi$ của $\mathbf{SU}(2,\mathbf C)$ sao cho $\nu_2=\nu_1\circ\varphi$, và ta kết luận bằng cách dùng Mệnh đề 9 của no. 4.

Từ hệ quả trước đó suy ra rằng đồng cấu $\nu_{\mathbf T}$ từ $\mathbf U$ đến $\mathbf T$, được xác định bởi
$$
\nu_{\mathbf T}(a)=\nu\begin{pmatrix}a&0\\0&\bar a\end{pmatrix}
$$
với $a\in\mathbf U$, không phụ thuộc vào lựa chọn của $\nu$. Ký hiệu $K_\alpha\in\Gamma(\mathbf T)$ là ảnh dưới $\Gamma(\nu_{\mathbf T})$ của phần tử $2\pi i$ của $\Gamma(\mathbf U)=2\pi i\mathbf Z$; nó được gọi là *vectơ nút liên kết với nghiệm* $\alpha$. Ta có $\langle\alpha,K_\alpha\rangle=2$, nói cách khác (no. 2, công thức (2)) $\delta(\alpha)(K_\alpha)=4\pi i$; vì $K_\alpha$ thuộc giao của $\mathfrak t$ và $\mathscr L(S_\alpha)(\mathbf C)$, ta có
$$
K_\alpha=2\pi iH_{\delta(\alpha)},
\tag{13}
$$
trong đó $H_{\delta(\alpha)}$ là *nghiệm nghịch đảo liên kết với nghiệm* $\delta(\alpha)$ của $(\mathfrak g_{\mathbf C},\mathfrak t_{\mathbf C})$ (Chap. VIII, §2, no. 2). Nói cách khác, khi $\Gamma(\mathbf T)\otimes\mathbf R$ được đồng nhất với đối ngẫu của $X(T)\otimes \mathbf{R}$ qua cặp $\langle ,\rangle$, $K_{\alpha}$ được đồng nhất với nghiệm nghịch đảo $\alpha^{\vee}\in (X(T)\otimes \mathbf{R})^*$.

#### Nhận xét {#lie-ix-s4-n5-rem-1 .statement tag=01C5}

Với mọi $x\in \mathbf{R}$, ta có

$($ exp(2$\pi ix$) 0 $)_{2\pi ix}$

$\nu$ 0 exp($-2\pi ix$)$=\nu_T(e$ ) = exp($xK_{\alpha}$). (14)

Đặc biệt:

$\nu (-0$1 $-01)=\nu_T(-1) =$ exp$(\frac{1}{2}K_{\alpha})$. (15)

Suy ra rằng $\nu$ là đơn ánh khi và chỉ khi $K_{\alpha}\notin2\Gamma$(T), nói cách khác nếu tồn tại $\lambda \in X(T)$ sao cho $\langle \lambda , K_{\alpha}\rangle \notin2\mathbf{Z}$. Khi $\mathfrak{g}_{\mathbf{C}}$ là đơn, $\nu$ là đơn ánh trừ khi $\mathfrak{g}_{\mathbf{C}}$ có kiểu $B_n, C(G) =\{1\}$ và $\alpha$ là một nghiệm ngắn (cf. Chap. VI, Plates).

Trong phần còn lại của đoạn này, ta ký hiệu $R^{\vee}(G,T)$ là tập hợp các vectơ nút $K_{\alpha}$ với $\alpha \in R(G,T)$. Đây là một tập con của $\Gamma (T)$ mà đơn ánh chính tắc của $\Gamma (T)$ vào $\mathfrak{t}_{\mathbf{C}}$ đồng nhất với phép vị tự có tỉ số $2\pi i$ của hệ nghiệm nghịch đảo $R^{\vee}(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}}) =\{H_{\delta(\alpha)}\}$ của $\delta (R)$. Suy ra rằng $R^{\vee}(G,T)$ sinh ra không gian vectơ $\mathbf{R}$ $L(T\cap D(G))$, và do đó rằng phần bù trực giao của nó trong X(T) là $X(T/(T\cap D(G)))$.

Kí hiệu Aut(T) là nhóm các tự đẳng cấu của nhóm Lie T; nhóm Weyl $W = W_G(T) ($§2, no. 5) có thể được đồng nhất với một nhóm con của Aut(T). Mặt khác, nhắc lại (Chương VIII, §2, no. 2, Nhận xét 4) rằng nhóm Weyl $W(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}})$ của đại số Lie reductive tách được $(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}})$ tác động lên $\mathfrak{t}_{\mathbf{C}}$, và do đó được đồng nhất một cách chính tắc với một nhóm con của $\mathbf{G}\mathbf{L}(\mathfrak{t}_{\mathbf{C}})$.

#### Mệnh đề 10 {#lie-ix-s4-prop-10 .statement tag=01C6}

Ánh xạ $u \rightarrow L(u)_{(\mathbf{C})}$ từ Aut(T) đến $\mathbf{G}\mathbf{L}(\mathfrak{t}_{\mathbf{C}})$ cảm sinh một đẳng cấu từ W đến nhóm Weyl của đại số Lie reductive tách được $(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}})$. Với mọi $\alpha \in R$, $W_{Z_{\alpha}}(T)$ có cấp 2, và ảnh của phần tử không đơn vị của $W_{Z_{\alpha}}(T)$ qua đẳng cấu nói trên là phép đối xứng $s_{H_{\delta(\alpha)}}$.

Ánh xạ đang xét là đơn ánh. Còn phải chứng minh rằng ảnh của nó bằng $W(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}})$.

Cho $g\in N_G(T)$. Với các kí hiệu trong Chương VIII, §5, no. 2, ta có Ad $g\in$ Aut($\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}}$)$\cap$ Int($\mathfrak{g}_{\mathbf{C}}$), nên Ad $g\in$ Aut$_0(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}}$) (loc. cit., no. 5, Mệnh đề 11). Theo loc. cit., no. 2, Mệnh đề 4, tự đẳng cấu của $\mathfrak{t}_{\mathbf{C}}$ được cảm sinh bởi Ad $g$ thuộc $W(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}})$. Do đó, ảnh của W trong $\mathbf{G}\mathbf{L}(\mathfrak{t}_{\mathbf{C}})$ được chứa trong $W(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}})$.

Cho $\alpha \in R(G,T)$, và cho $\nu :\mathbf{S}\mathbf{U}(2,\mathbf{C})\rightarrow G$ là một cấu xạ của nhóm Lie có các tính chất trong Hệ quả của Định lý 1. Ảnh qua $\nu$ của phần tử $\theta$ của $\mathbf{S}\mathbf{U}(2,\mathbf{C})$ có các tính chất sau (§3, no. 6, công thức (17)):

a) (Int$\nu (\theta )$)$(t) =t$ nếu $t\in$ Ker$\alpha$,

b) (Int$\nu (\theta )$)$(t) =t^{-1}$ nếu $t\in T\cap S_{\alpha}$.

Suy ra Ad $\nu (\theta )$ cảm sinh đồng nhất thức trên Ker $\delta (\alpha )\subset \mathfrak{t}_{\mathbf{C}}$, và cảm sinh ánh xạ $x \rightarrow  -x$ trên $[\mathfrak{g}^{\alpha},\mathfrak{g}^{-\alpha}]$, do đó trùng với phép đối xứng $s_{H_{\delta(\alpha)}}$. Do đó, ảnh của W chứa mọi $s_{H_{\delta(\alpha)}}$, và vì thế bằng $W(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}})$. Đặc biệt $W_{Z_{\alpha}}(T)$ có cấp 2, và do đó gồm phần tử đơn vị và Int $\nu (\theta )$. Điều đó kết thúc chứng minh mệnh đề.

#### Hệ quả {#lie-ix-s4-n5-cor-2 .statement tag=01JJ}

Giả sử G là nửa đơn. Khi đó mọi phần tử của G là giao hoán tử của hai phần tử của G.

Cho $c$ là một phép biến đổi Coxeter của nhóm Weyl $W(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}})$ (Chương V, §6, no. 1), và cho $n$ là một phần tử của $N_G(T)$ mà lớp của nó trong W được đồng nhất với $c$ bởi đẳng cấu được xác định trong mệnh đề. Kí hiệu $f_c$ là cấu xạ $t \rightarrow (n, t)$ từ T đến T; với $x\in \mathfrak{t}_{\mathbf{C}}$, ta có $L(f_c)_{(\mathbf{C})}(x) =$ (Ad $n$)$(x)-x=$ $c(x)-x$.

Theo Định lý 1 của Chương V, §6, no. 2, tự đồng cấu $c$ của $\mathfrak{t}_{\mathbf{C}}$ không có trị riêng bằng 1. Do đó, $L(f_c)$ là toàn ánh, và vì thế $f_c$ cũng toàn ánh. Suy ra mọi phần tử của T là giao hoán tử của hai phần tử của G, điều này suy ra hệ quả theo Định lý 2, §2, no. 2.

### 6. NHÓM CƠ BẢN

Trong mệnh đề sau, $f(G,T)$ ký hiệu đồng cấu từ $\Gamma (T)$ đến $\pi_1(G)$, là hợp thành của đẳng cấu chính tắc từ $\Gamma (T)$ đến $\pi_1(T)$ (no. 2, Nhận xét 3) và đồng cấu $\pi_1(\iota )$, trong đó $\iota$ là đơn ánh chính tắc $T\rightarrow G$.

#### Mệnh đề 11 {#lie-ix-s4-prop-11 .statement tag=01C8}

Đồng cấu $f(G,T) :\Gamma (T)\rightarrow \pi_1(G)$ là toàn ánh. Hạt nhân của nó là nhóm con $N(G,T)$ của $\Gamma (T)$ được sinh bởi họ các vectơ nút $(K_{\alpha})_{\alpha\in R(G,T)}$.

Đồng cấu $f(G,T)$ là toàn ánh theo Mệnh đề 3 (§2, no. 4). Ta ký hiệu $A(G,T)$ là mệnh đề: “hạt nhân của $f(G,T)$ được sinh bởi các $K_{\alpha}$”, điều còn phải chứng minh, và phân biệt một số trường hợp:

$a) G$ là đơn liên. Cho $\rho :\mathfrak{g}_{\mathbf{C}}\rightarrow \mathfrak{g}\mathfrak{l}(V)$ là một biểu diễn tuyến tính của $\mathfrak{g}_{\mathbf{C}}$ trên một không gian vectơ phức hữu hạn chiều V. Hạn chế xuống $\mathfrak{g}$, ta thu được một biểu diễn của $\mathfrak{g}$ trên không gian vectơ thực $V_{(\mathbf{R})}$; vì G đơn liên, tồn tại một biểu diễn tuyến tính giải tích $\pi$ của G trên $V_{(\mathbf{R})}$ sao cho $\rho = L(\pi )$. Suy ra từ Mệnh đề 7 của no. 3 rằng ảnh $\delta (X(T))$ của X(T) trong $\mathfrak{t}^*_{\mathbf{C}}$ chứa mọi trọng số của $\rho$ trên V. Vì điều này đúng với mọi biểu diễn $\rho$ của $\mathfrak{g}_{\mathbf{C}}$, suy ra từ Chương VIII, §7, no. 2, Định lý 1 rằng $\delta (X(T))$ chứa nhóm các trọng số của $\delta$(R), mà theo định nghĩa là tập hợp các $\lambda \in \mathfrak{t}^*_{\mathbf{C}}$ sao cho $\lambda (H_{\delta(\alpha)})\in \mathbf{Z}$ với mọi $\alpha \in R$, nói cách khác, $\lambda (K_{\alpha})\in 2\pi i\mathbf{Z}$ với mọi $\alpha \in R$. Do đó, nhóm X(T) chứa mọi phần tử $\lambda$ của $X(T)\otimes \mathbf{Q}$ sao cho $\langle \lambda , K_{\alpha}\rangle  \in \mathbf{Z}$ với mọi $\alpha \in R$, điều đó theo đối ngẫu suy ra rằng $\Gamma (T)$ được sinh bởi các $K_{\alpha}$, do đó mệnh đề $A(G,T)$.

$b) G$ là tích trực tiếp của một nhóm đơn liên thông $G'$ và một xuyến S. Khi đó T là tích trực tiếp của một xuyến cực đại $T'$ của $G'$ với $S,\Gamma (T)$ có thể được đồng nhất với $\Gamma (T')\times \Gamma$(S), $\pi_1(G)$ với $\pi_1(G')\times \pi_1$(S), và $f(G,T)$ với các đồng cấu có các thành phần $f(G',T')$ và $f(S,S)$. Vì $f(S,S)$ là song ánh, ánh xạ chính tắc $\Gamma (T')\rightarrow \Gamma (T)$ ánh xạ Ker $f(G',T')$ song ánh lên Ker $f(G,T)$. Hơn nữa, các $K_{\alpha}$ thuộc đại số Lie của nhóm dẫn xuất $G'$ của G, do đó thuộc ảnh của $\Gamma (T')$, nên suy ra ngay rằng $A(G',T')$ kéo theo $A(G,T)$, do đó mệnh đề $A(G,T)$, theo a).

c) Trường hợp tổng quát. Có một cấu xạ toàn ánh $p: G'\rightarrow G$ với hạt nhân hữu hạn, trong đó $G'$ là tích trực tiếp của một nhóm đơn liên thông bởi một xuyến (§1, no. 4, Mệnh đề 4). Nếu $T'$ là ảnh ngược của T trong $G'$ (đây là một xuyến cực đại của $G'$ theo §2, no. 3, Mệnh đề 1), và N là hạt nhân của $p$, ta có các dãy khớp $0\rightarrow N\rightarrow G'\rightarrow G\rightarrow 0$ và $0\rightarrow N\rightarrow T'\rightarrow T\rightarrow 0$, do đó một biểu đồ giao hoán với các hàng khớp (no. 2, Nhận xét 1 và General Topology, Chap. XI, in preparation)

0 $\longrightarrow \Gamma (T')\longrightarrow \Gamma (T)\longrightarrow$ N $\longrightarrow$ 0

$f(G',T')f(G,T)$ Id$_N$

0 $\longrightarrow \pi_1(G')\longrightarrow \pi_1(G)\longrightarrow$ N $\longrightarrow 0$.

Suy ra ngay từ biểu đồ con rắn (Algebra, Chap. X, p. 4, Mệnh đề 2) rằng $A(G',T')$ kéo theo $A(G,T)$, do đó mệnh đề, theo b).

#### Hệ quả 1 {#lie-ix-s4-prop-11-cor-1 .statement tag=01C9}

G là đơn liên thông khi và chỉ khi họ $(K_{\alpha})_{\alpha\in R(G,T)}$ sinh ra $\Gamma (T)$.

#### Hệ quả 2 {#lie-ix-s4-prop-11-cor-2 .statement tag=01CA}

Cho H là một nhóm con đóng liên thông của G chứa T; có một dãy khớp

$$
0\longrightarrow N(H,T)\longrightarrow N(G,T)\longrightarrow \pi_1(H)\longrightarrow \pi_1(G)\longrightarrow 0
$$

Điều này suy ra từ Algebra, Chap. X, p. 4, Mệnh đề 2 (biểu đồ con rắn), áp dụng cho biểu đồ giao hoán

0 $\longrightarrow N(H,T)\longrightarrow \Gamma (T)\longrightarrow \pi_1(H)\longrightarrow$ 0

0 $\longrightarrow N(G,T)\longrightarrow \Gamma (T)\longrightarrow \pi_1(G)\longrightarrow 0$.

#### Nhận xét {#lie-ix-s4-n6-rem-1 .statement tag=01CB}

Có thể chứng minh (xem Bài tập 2 của §5) rằng $\pi_2(G/H)$ bằng không. Tính khớp của dãy trước đó khi ấy cho một đẳng cấu từ $\pi_2(G/H)$ đến $N(G,T)/N(H,T)$.

#### Hệ quả 3 {#lie-ix-s4-prop-11-cor-3 .statement tag=01CC}

Đồng cấu $\pi_1(D(G))\rightarrow \pi_1(G)$ tương ứng với sự nhúng của D(G) vào G cảm sinh một đẳng cấu từ $\pi_1(D(G))$ lên nhóm con xoắn của $\pi_1(G)$.

Thật vậy, $T\cap D(G)$ là một xuyến cực đại của D(G) (§2, no. 3, Mệnh đề $1c$)); từ dãy khớp

$$
0\longrightarrow \Gamma (T\cap D(G))\longrightarrow \Gamma (T)\longrightarrow \Gamma (T/(T\cap D(G)))\longrightarrow 0
$$

và Mệnh đề 11, ta thu được một dãy khớp

$$
0\longrightarrow \pi_1(D(G))\longrightarrow \pi_1(G)\longrightarrow \Gamma (T/(T\cap D(G)))\longrightarrow 0
$$

do đó hệ quả, vì $\pi_1(D(G))$ là hữu hạn và $\Gamma (T/(T\cap D(G)))$ là tự do.

### 7. CÁC NHÓM CON CÓ HẠNG CỰC ĐẠI

Nhắc lại (Chương VI, §1, no. 7) rằng một tập con P của $R = R(G,T)$ được gọi là đóng nếu $(P + P)\cap R\subset P$, và đối xứng nếu $P =-P$.

#### Mệnh đề 12 {#lie-ix-s4-prop-12 .statement tag=01CD}

Giả sử $\mathscr{H}$ là tập hợp các nhóm con đóng liên thông của G chứa T, được sắp thứ tự bởi bao hàm. Ánh xạ $H \rightarrow R(H,T)$ là một song ánh tăng từ $\mathscr{H}$ tới tập hợp các tập con đóng đối xứng của $R(G,T)$, được sắp thứ tự bởi bao hàm.

Nếu $H\in \mathscr{H}$, thì $L(H)_{(\mathbf{C})}$ là tổng trực tiếp của $\mathfrak{t}_{\mathbf{C}}$ và các $\mathfrak{g}^{\alpha}$ với $\alpha \in R(H,T)$; vì đây là một đại số con khả quy trong $\mathfrak{g}_{\mathbf{C}}$, nên tập con $R(H,T)$ của R thỏa mãn các điều kiện đã nêu (Chương VIII, §3, no. 1, Bổ đề 2 và Mệnh đề 2). Ngược lại, nếu P là một tập con của R thỏa mãn các điều kiện này, thì $\mathfrak{t}_{\mathbf{C}}\oplus \sum_{\alpha\in P}\mathfrak{g}^{\alpha}$ là một đại số con

của $\mathfrak{g}_{\mathbf{C}}($loc. cit.) hữu tỉ trên $\mathbf{R}$ (no. 3), và do đó có dạng $\mathfrak{h}_{(\mathbf{C})}$, trong đó $\mathfrak{h}$ là một đại số con của $\mathfrak{g}$. Đặt H(P) là nhóm con nguyên của G được xác định bởi $\mathfrak{h}$; nó đóng (§2, no. 4, Nhận xét 1). Ta kiểm tra ngay rằng các ánh xạ $H \rightarrow R(H,T)$ và $P \rightarrow H(P)$ đều tăng và nghịch đảo của nhau.

#### Hệ quả 1 {#lie-ix-s4-prop-12-cor-1 .statement tag=01CE}

Chỉ có hữu hạn các nhóm con đóng của G chứa T.

Giả sử H là một nhóm con như vậy; khi đó $H_0\in \mathscr{H}$, và $\mathscr{H}$ là hữu hạn. Hơn nữa, H là một nhóm con của $N_G(H_0)$ chứa $H_0$, và $N_G(H_0)/H_0$ là hữu hạn (§2, no. 4, Mệnh đề 4 và Nhận xét 2).

#### Hệ quả 2 {#lie-ix-s4-prop-12-cor-2 .statement tag=01CF}

Giả sử H là một nhóm con đóng liên thông của G chứa T, và đặt $W^H_G(T)$ là nhóm ổn định trong $W_G(T)$ của tập con $R(H,T)$ của R. Nhóm $N_G(H)/H$ đẳng cấu với nhóm thương $W^H_G(T)/W_H(T)$.

Thật vậy, suy ra từ Mệnh đề 7 của §2, no. 5, áp dụng cho $N_G$(H), rằng $N_G(H)/H$ đẳng cấu với $W_{N(H)}(T)/W_H$(T), trong đó $W_{N(H)}(T)$ là tập hợp các phần tử của $W_G(T)$ mà các đại diện của chúng trong $N_G(T)$ chuẩn hóa H. Cho $n\in N_G$(T), và gọi $w$ là lớp của nó trong $W_G(T)$. Theo Chương III, §9, no. 4, Mệnh đề 11, $n$ chuẩn hóa H khi và chỉ khi (Ad $n$)$(L(H)) = L(H)$; xét theo Mệnh đề 5 của no. 3, điều đó cũng có nghĩa là tập con $R(H,T)$ của R ổn định dưới $w$, suy ra hệ quả.

#### Nhận xét 1 {#lie-ix-s4-n7-rem-1 .statement tag=01CG}

Nhóm $W^H_G(T)$ cũng là nhóm ổn định trong $W_G(T)$ của nhóm con C(H) của T: điều này suy ra từ Mệnh đề 8 của no. 4.

#### Mệnh đề 13 {#lie-ix-s4-prop-13 .statement tag=01CH}

Giả sử H là một nhóm con đóng liên thông của G có hạng tối đại, và C là tâm của nó. Khi đó C chứa tâm của G, và H là thành phần liên thông đơn vị của nhóm trung tâm hoá của C.

Cho S là một xuyến tối đại của H. Vì tâm của G được chứa trong S, nên nó được chứa trong C. Đặt $L = Z(C)_0$; đây là một nhóm con đóng liên thông của G chứa H, nên có hạng tối đại, và tâm của nó bằng C. Ký hiệu $R_H$ và $R_L$ lần lượt là các hệ nghiệm của H và L, tương ứng, đối với S; khi đó $R_H\subset R_L\subset R(G,S)$. Vì C(H) = C(L), Mệnh đề 8 (no. 4) suy ra đẳng thức $Q(R_H) = Q(R_L)$; nhưng $Q(R_H)\cap R_L= R_H$ (Chương VI, §1, no. 7, Mệnh đề 23), nên $R_H= R_L$ và H = L (Mệnh đề 12).

#### Nhận xét 2 {#lie-ix-s4-n7-rem-2 .statement tag=01CI}

Ta nói rằng một nhóm con C của G là căn nếu tồn tại một xuyến cực đại S của G và một tập con P của $R(G,S)$ sao cho $C =\bigcap_{\alpha\in P}$ Ker$\alpha$. Suy ra từ Mệnh đề 13 và Bổ đề 2 của no. 5 rằng ánh xạ $H \rightarrow C(H)$ cảm sinh một song ánh từ tập hợp các nhóm con đóng liên thông của hạng cực đại đến tập hợp các nhóm con căn của G. Song ánh ngược là ánh xạ $C \rightarrow Z(C)_0$.

#### Hệ quả {#lie-ix-s4-n7-cor-1 .statement tag=01CJ}

Tập các $g\in G$ sao cho $T\cap gTg^{-1}\not= C(G)$ là hợp của một số hữu hạn các đa tạp con giải tích đóng của G, khác G.

Thật vậy, đặt $A_g= T\cap gTg^{-1}$; ta có $T\subset Z(A_g)$ và $gTg^{-1}\subset Z(A_g)$. Do đó, tồn tại $x\in Z(A_g)$ sao cho $xTx^{-1}=gTg^{-1}($§2, no. 2, Định lý 2), điều này suy ra rằng $g\in Z(A_g).N_G(T)$. Ký hiệu $\mathscr{A}$ là tập hữu hạn (Hệ quả 1) các nhóm con đóng của G chứa T và khác G, và đặt X = $\bigcup_{H\in\mathscr{A}}H.N_G(T)$; đây là một hợp hữu hạn các đa tạp con đóng của G, khác G. Nếu $A_g\not= C(G)$, thì $Z(A_g)\in \mathscr{A}$, và $g$ thuộc X. Ngược lại, nếu $g\in H.N_G$(T), với $H\in \mathscr{A}$, thì $A_g$ chứa C(H), do đó $A_g\not= C(G)$ (Mệnh đề 13).

#### Mệnh đề 14 {#lie-ix-s4-prop-14 .statement tag=01CK}

Cho X là một tập con của T, và cho $R_X$ là tập các nghiệm $\alpha \in R(G,T)$ sao cho $\alpha (X) =\{1\}$. Nhóm $Z_G(X)/Z_G(X)_0$ đẳng cấu với thương của nhóm con của $W_G(T)$ giữ X cố định bởi nhóm con sinh bởi các phản xạ $s_{\alpha}$ với $\alpha \in R_X$.

Đặt $H = Z_G(X)$; vì $L(H)_{(\mathbf{C})}$ là tập hợp các điểm của $\mathfrak{g}_{\mathbf{C}}$ được Ad(X) cố định, nên nó là tổng của $\mathfrak{t}_{\mathbf{C}}$ và các $\mathfrak{g}^{\alpha}$ với $\alpha (X) =\{1\}$. Do đó, $R(H_0,T) =$ $R_X$, nên $W_{H_0}(T)$ được sinh bởi các phản xạ $s_{\alpha}$ với $\alpha \in R_X$. Bây giờ chỉ cần áp dụng Mệnh đề 7 của §2, no. 5.

Ta sẽ thấy dưới đây (§5, no. 3, Định lý 1) rằng nếu G là đơn liên và X rút về một điểm, thì nhóm trung tâm hóa Z(X) là liên thông.

### 8. BIỂU ĐỒ NGHIỆM

#### Định nghĩa 2 {#lie-ix-s4-def-2 .statement tag=01CL}

Một biểu đồ nghiệm (hay đơn giản là một biểu đồ, nếu không có nguy cơ nhầm lẫn) là một bộ ba $D = (M,M_0,R)$ trong đó:

(RD$_0$) $M$ là một $\mathbf{Z}$-môđun tự do hữu hạn sinh và môđun con $M_0$ là một nhân tử trực tiếp của M;

(RD$_I$) $R$ là một tập con hữu hạn của $M; R\cup M_0$ sinh ra không gian vectơ trên $\mathbf{Q}$ $\mathbf{Q}\otimes M$;

(RD$_{II}$) với mọi $\alpha \in R$, tồn tại một phần tử $\alpha^{\vee}$ của $M^*=$ Hom$_{\mathbf{Z}}(M,\mathbf{Z})$ sao cho $\alpha^{\vee}(M_0) = 0,\alpha^{\vee}(\alpha ) = 2$ và tự đồng cấu $x \rightarrow x-\alpha^{\vee}(x)\alpha$ của M giữ R ổn định.

Theo Chương VI, §1, no. 1, với mọi $\alpha \in R$ phần tử $\alpha^{\vee}$ của $M^*$ được xác định duy nhất bởi $\alpha$; ta ký hiệu bởi $s_{\alpha}$ tự đồng cấu $x \rightarrow x-\alpha^{\vee}(x)\alpha$ của M. Hơn nữa (loc. cit.), không gian $\mathbf{Q}$-vectơ $\mathbf{Q}\otimes M$ là tổng trực tiếp của $\mathbf{Q}\otimes M_0$ và không gian con vectơ V(R) sinh bởi R, và R là một hệ nghiệm trong V(R) (loc. cit., Định nghĩa 1).

Các phần tử của R được gọi là các nghiệm của biểu đồ nghiệm D, và các phần tử $\alpha^{\vee}$ của $M^*$ là các nghiệm nghịch đảo. Nhóm sinh bởi các tự đẳng cấu $s_{\alpha}$ của M được gọi là nhóm Weyl của D và được ký hiệu bởi W(D); các phần tử của W(D) cảm sinh đồng nhất trên $M_0$, và cảm sinh trên V(R) các phép biến đổi của nhóm Weyl của hệ nghiệm R.

#### Ví dụ 1 {#lie-ix-s4-n8-exa-1 .statement tag=01CM}

Với mọi $\mathbf{Z}$-môđun tự do hữu hạn sinh M, bộ ba $(M,M,\emptyset )$ là một biểu đồ nghiệm.

#### Ví dụ 2 {#lie-ix-s4-n8-exa-2 .statement tag=01CN}

Nếu $D = (M,M_0,R)$ là một biểu đồ nghiệm, hãy lấy $M^*_0$ là phần bù trực giao của V(R) trong $M^*$, và lấy $R^{\vee}$ là tập các nghiệm nghịch đảo của D. Khi đó $D^{\vee}= (M^*,M^*_0,R^{\vee})$ là một biểu đồ nghiệm, gọi là biểu đồ nghịch đảo của D. Với mọi $\alpha \in R$, phép đối xứng $s_{\alpha^{\vee}}$ của $M^*$ là tự đẳng cấu đối liên hợp của phép đối xứng $s_{\alpha}$ của M; ánh xạ $w \rightarrow^tw^{-1}$ là một đẳng cấu từ W(D) đến $W(D^{\vee})$. Hơn nữa, $V(R^{\vee})$ có thể được đồng nhất tự nhiên với đối ngẫu của không gian vectơ $\mathbf{Q}$ $V(R)$, khi đó $R^{\vee}$ được đồng nhất với hệ nghiệm nghịch đảo của R.

Nếu đối ngẫu của $M^*$ được đồng nhất với M, thì biểu đồ nghịch đảo của $D^{\vee}$ được đồng nhất với D.

#### Ví dụ 3 {#lie-ix-s4-n8-exa-3 .statement tag=01CO}

Cho $(\mathfrak{g},\mathfrak{h})$ là một đại số Lie $\mathbf{Q}$ khả quy tách, và $M\subset \mathfrak{h}$ là một dàn được phép (Chương VIII, §12, no. 6, Định nghĩa 1). Hãy lấy $M_0$ là nhóm con của M trực giao với các nghiệm của $(\mathfrak{g},\mathfrak{h})$ và $R^{\vee}$ là tập các $H_{\alpha},\alpha \in R(\mathfrak{g},\mathfrak{h})$. Khi đó $(M,M_0,R^{\vee})$ là một biểu đồ nghiệm, và $(M^*,M^*_0,R(\mathfrak{g},\mathfrak{h}))$ là biểu đồ nghịch đảo.

#### Ví dụ 4 {#lie-ix-s4-n8-exa-4 .statement tag=01CP}

Cho V là một không gian vectơ trên $\mathbf{Q}$ và R là một hệ nghiệm trong V; ký hiệu P(R) là nhóm các trọng số của R và Q(R) là nhóm các trọng số căn của R (Chương VI, §1, no. 9). Khi đó $(Q(R),0,R)$ và $(P(R),0,R)$ là các biểu đồ nghiệm. Một biểu đồ nghiệm $(M,M_0,S)$ đẳng cấu với một biểu đồ có dạng $(Q(R),0,R)$ (resp. $(P(R),0,R)$) khi và chỉ khi M được sinh bởi S (resp. $M^*$ được sinh bởi $S^{\vee}$).

Với mọi nhóm con X của P(R) chứa $Q(R), (X,0,R)$ là một biểu đồ nghiệm và, xét đến đẳng cấu, mọi biểu đồ $(M,M_0,S)$ sao cho $M_0= 0$, nói cách khác sao cho S sinh ra một nhóm con của M có chỉ số hữu hạn, đều xuất hiện theo cách này.

Biểu đồ nghiệm $(M,M_0,R)$ được gọi là rút gọn nếu hệ nghiệm R là rút gọn (nói cách khác (Chương VI, §1, no. 4) nếu các quan hệ $\alpha , \beta \in R,\lambda \in \mathbf{Z}$, $\beta =\lambda \alpha$ suy ra rằng $\lambda = 1$ hoặc $\lambda =-1$). Các biểu đồ trong Ví dụ 1) và 3) là rút gọn.

### 9. NHÓM LIE COMPACT VÀ HỆ NGHIỆM

Với thuật ngữ đã đưa vào ở số trước, một phần quan trọng của các kết quả ở các số 4 và 5 có thể được tóm tắt trong định lý sau:

#### Định lý 2 {#lie-ix-s4-thm-2 .statement tag=01CQ}

a) $(X(T),X(T/(T\cap D(G)),R(G,T)))$ là một biểu đồ nghiệm rút gọn; nhóm Weyl của nó gồm các $X(w)$ với $w\in W$; nhóm X(C(G)) đẳng cấu với thương của X(T) theo nhóm con sinh bởi R(G,T).

b) $(\Gamma (T), \Gamma (C(G)_0),R^{\vee}(G,T))$ là một biểu đồ nghiệm gốc rút gọn; nhóm Weyl của nó gồm các $\Gamma (w)$, với $w\in W$; nhóm $\pi_1(G)$ đẳng cấu với thương của $\Gamma (T)$ theo nhóm con được sinh bởi $R^{\vee}(G,T)$.

c) Nếu mỗi môđun $\mathbf{Z}$-môđun X(T) và $\Gamma (T)$ được đồng nhất với đối ngẫu của môđun kia (no. 2, Mệnh đề 3), thì mỗi biểu đồ nghiệm gốc trên được đồng nhất với nghịch đảo của biểu đồ kia.

Ký hiệu $D^*(G,T)$ là biểu đồ $(X(T),X(T/(T\cap D(G)),R(G,T)))$ và $D_*(G,T)$ là biểu đồ $(\Gamma (T), \Gamma (C(G)_0),R^{\vee}(G,T))$; các biểu đồ này lần lượt được gọi là biểu đồ phản biến và biểu đồ đồng biến của G (đối với T).

#### Ví dụ 1 {#lie-ix-s4-n9-exa-1 .statement tag=01CR}

Nếu G nửa đơn có hạng 1, thì $D^*(G,T)$ và $D_*(G,T)$ tất yếu đẳng cấu với một trong hai biểu đồ $\Delta_2= (\mathbf{Z},0,\{2,-2\})$, $\Delta_1= (\mathbf{Z},0,\{1,-1\})$. Nếu G đẳng cấu với $\mathbf{S}\mathbf{U}(2,\mathbf{C}), D_*(G,T)$ đẳng cấu với $\Delta_1$ (vì G đơn liên) nên $D^*(G,T)$ đẳng cấu với $\Delta_2$. Nếu G đẳng cấu với $\mathbf{S}\mathbf{O}(3,\mathbf{R}), D^*(G,T)$ đẳng cấu với $\Delta_1$ (vì $C(G) =\{1\}$), nên $D_*(G,T)$ đẳng cấu với $\Delta_2$.

#### Ví dụ 2 {#lie-ix-s4-n9-exa-2 .statement tag=01CS}

Nếu G và $G'$ là hai nhóm Lie compact liên thông, với các xuyến cực đại T và $T'$ tương ứng, và nếu $D^*(G,T) = (M,M_0,R)$ và $D^*(G',T') =$ $(M',M'_0,R')$, thì $D^*(G\times G',T\times T')$ có thể được đồng nhất với $(M\oplus M',M_0\oplus$ $M'_0,R\cup R')$. Tương tự đối với các biểu đồ đồng biến.

#### Ví dụ 3 {#lie-ix-s4-n9-exa-3 .statement tag=01CT}

Cho N là một nhóm con đóng của T, trung tâm trong G, và cho $(M,M_0,R)$ là biểu đồ phản biến của G tương đối với T. Khi đó biểu đồ phản biến của $G/N$ tương đối với $T/N$ có thể được đồng nhất với $(M',M'_0,R)$, trong đó $M'$ là nhóm con của M gồm các $\lambda$ sao cho $\lambda (N) =\{1\}$ và $M'_0= M'\cap M_0$.

#### Ví dụ 4 {#lie-ix-s4-n9-exa-4 .statement tag=01CU}

Tương tự, cho N là một nhóm Abel hữu hạn, và $\varphi :\pi_1(G)\rightarrow N$ là một đồng cấu toàn ánh. Cho $G'$ là phủ của G liên kết với đồng cấu này; đây là một nhóm Lie compact liên thông, trong đó N là một nhóm con trung tâm (Tôpô học tổng quát, Chương XI, đang soạn), và G có thể được đồng nhất tự nhiên với $G'/N$. Cho $T'$ là xuyến cực đại của $G'$ mà là ảnh ngược của T. Nếu $(P,P_0,S)$ là biểu đồ đồng biến của G tương đối với T, thì biểu đồ đồng biến của $G'$ tương đối với $T'$ có thể được đồng nhất với $(P',P'_0,S)$, trong đó $P'$ là hạt nhân của đồng cấu hợp thành $\varphi \circ f(G,T) : P\rightarrow N$ (x. no. 6, Mệnh đề 11), và $P'_0= P_0\cap P'$.

#### Nhận xét 1 {#lie-ix-s4-n9-rem-1 .statement tag=01CV}

Cho $\mathfrak{c}$ là tâm của $\mathfrak{g}_{\mathbf{C}}$; khi đó $\mathfrak{c}= L(C(G))_{(\mathbf{C})}$. Ta có các quan hệ sau giữa các biểu đồ của G tương đối với T và các hệ nghiệm gốc trực tiếp và nghịch đảo của đại số khả quy tách $(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}}):$

a) Đẳng cấu chính tắc từ $\mathbf{C}\otimes \Gamma (T)$ đến $\mathfrak{t}_{\mathbf{C}}$ cảm sinh một song ánh từ $\mathbf{C}\otimes \Gamma (C(G)_0)$ đến $\mathfrak{c}$ và một song ánh từ $1\otimes R^{\vee}(G,T)$ đến $2\pi i.R^{\vee}(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}})$.

b) Đẳng cấu chính tắc từ $\mathbf{C}\otimes X(T)$ đến đối ngẫu $\mathfrak{t}^*_{\mathbf{C}}$ của $\mathfrak{t}_{\mathbf{C}}$ cảm sinh một song ánh từ $\mathbf{C}\otimes X(T/(T\cap D(G)))$ đến phần bù trực giao của $\mathfrak{t}_{\mathbf{C}}\cap \mathscr{D}(\mathfrak{g})_{\mathbf{C}}$, và một song ánh từ $1\otimes R(G,T)$ đến $R(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}})$.

#### Nhận xét 2 {#lie-ix-s4-n9-rem-2 .statement tag=01CW}

Giả sử nhóm G là nửa đơn; ký hiệu R (tương ứng $R^{\vee}$) là hệ nghiệm $R(G,T)$ (tương ứng $R^{\vee}(G,T)$), do đó ta có các bao hàm

$$
Q(R)\subset X(T)\subset P(R)Q(R^{\vee})\subset \Gamma (T)\subset P(R^{\vee})
$$

Các nhóm Abel hữu hạn $P(R)/Q(R)$ và $P(R^{\vee})/Q(R^{\vee})$ ở trong đối ngẫu (Chap. VI, §1, no. 9); nếu $\widehat{M}$ ký hiệu nhóm đối ngẫu của nhóm Abel hữu hạn M, ta suy ra từ các đẳng cấu chính tắc trên

$$
\Gamma (T)/Q(R^{\vee})\rightarrow \pi_1(G)P(R^{\vee})/\Gamma (T)\rightarrow C(G)
$$

$$
P(R)/X(T)\rightarrow (\pi_1(G)\widehat{)}X(T)/Q(R)\rightarrow (C(G))\widehat{.}
$$

Đặc biệt, tích các bậc của $\pi_1(G)$ và C(G) bằng chỉ số liên kết $f$ của $R(G,T)$ ($loc. cit.$).

Bây giờ cho $G'$ là một nhóm Lie compact liên thông khác, $T'$ là một xuyến cực đại của $G'$. Cho $f: G\rightarrow G'$ là một đẳng cấu các nhóm Lie sao cho $f(T) = T'$; ký hiệu $f_T$ là đẳng cấu từ T đến $T'$ do nó xác định. Khi đó $X(f_T)$ là một đẳng cấu từ $D^*(G',T')$ đến $D^*(G,T)$, được ký hiệu bởi $D^*(f)$, và $\Gamma (f_T)$ là một đẳng cấu từ $D_*(G,T)$ đến $D_*(G',T')$, được ký hiệu bởi $D_*(f)$. Nếu $t\in T$, và nếu ta đặt $g=f\circ$ Int $t=$ (Int $f(t)$)$\circ f$, thì $D^*(g) = D^*(f), D_*(g) = D_*(f)$.

#### Mệnh đề 15 {#lie-ix-s4-prop-15 .statement tag=01CX}

Cho $\varphi$ là một đẳng cấu từ $D^*(G',T')$ đến $D^*(G,T)$ (tương ứng từ $D_*(G,T)$ đến $D_*(G',T')$). Tồn tại một đẳng cấu $f: G\rightarrow G'$ sao cho $f(T) = T'$ và $\varphi = D^*(f)$ (tương ứng $\varphi = D_*(f)$); nếu $f_1$ và $f_2$ là hai đẳng cấu như thế, thì tồn tại một phần tử $t$ của T sao cho $f_2=f_1\circ$ tự đẳng cấu trong $t$.

Mệnh đề thứ hai suy ra ngay từ Mệnh đề 9 (no. 4); chẳng hạn, ta chứng minh mệnh đề thứ nhất cho các sơ đồ đồng biến. Ký hiệu bởi $\mathfrak{g}'$ (tương ứng $\mathfrak{t}'$) đại số Lie của $G'$ (tương ứng $T'$), và bởi $\mathfrak{g}'_{\mathbf{C}}$ (tương ứng $\mathfrak{t}'_{\mathbf{C}}$) đại số Lie phức hóa của nó. Theo Chương VIII, §4, no. 4, Định lý 2 (i), tồn tại một đẳng cấu $\psi :\mathfrak{g}_{\mathbf{C}}\rightarrow \mathfrak{g}'_{\mathbf{C}}$ ánh xạ $\mathfrak{t}_{\mathbf{C}}$ thành $\mathfrak{t}'_{\mathbf{C}}$ và cảm sinh trên $\Gamma (T)\subset \mathfrak{t}_{\mathbf{C}}$ đẳng cấu đã cho $\varphi :\Gamma (T)\rightarrow \Gamma (T')$. Khi đó $\mathfrak{g}$ và $\psi^{-1}(\mathfrak{g}')$ là hai dạng compact của $\mathfrak{g}_{\mathbf{C}}$ có cùng giao $\mathfrak{t}$ với $\mathfrak{t}_{\mathbf{C}}$; theo §3, no. 2, Mệnh đề 3, tồn tại một tự đẳng cấu trong $\theta$ của $\mathfrak{g}_{\mathbf{C}}$ cảm sinh đồng nhất trên $\mathfrak{t}_{\mathbf{C}}$ và sao cho $\theta (\mathfrak{g}) =\psi^{-1}(\mathfrak{g}')$. Bằng cách thay thế $\psi$ bởi $\psi \circ \theta$, ta có thể giả sử rằng $\psi$ ánh xạ $\mathfrak{g}$ vào $\mathfrak{g}'$. Hơn nữa, theo Mệnh đề 4 của no. 2, tồn tại một cấu xạ duy nhất $f_T: T\rightarrow T'$ sao cho $\Gamma (f_T) =\varphi$. Khi đó, hạn chế của $\psi$ lên $\mathfrak{t}$ là $L(f_T)$, và theo §2, no. 6, Mệnh đề 8, tồn tại một cấu xạ duy nhất $f: G\rightarrow G'$ cảm sinh $f_T$ trên T và $\psi$ trên $\mathfrak{g}_{\mathbf{C}}$. Áp dụng điều trên cho $\varphi^{-1}$ và $\psi^{-1}$ ta thu được một cấu xạ nghịch đảo của $f$, do đó $f$ là một đẳng cấu. Khi đó $D_*(f) =\Gamma (f_T) =\varphi$, suy ra mệnh đề.

Chú ý rằng, nếu T và $T'$ là hai xuyến cực đại của G, thì các biểu đồ $D^*(G,T)$ và $D^*(G,T')$ đẳng cấu với nhau (nếu $g\in G$ sao cho $gTg^{-1}= T'$, thì Int $g$ là một đẳng cấu từ G đến G ánh xạ T thành $T'$). Kí hiệu $D^*(G)$ là lớp đẳng cấu của $D^*(G,T)$ (xem Lý thuyết tập hợp, Chương II, §6, no. 2); đây là một biểu đồ nghiệm chỉ phụ thuộc vào G và được gọi là biểu đồ phản biến của G. Biểu đồ đồng biến $D_*(G)$ của G được định nghĩa tương tự, và ta thu được:

#### Hệ quả {#lie-ix-s4-n9-cor-1 .statement tag=01CY}

Hai nhóm Lie compact liên thông G và $G'$ đẳng cấu khi và chỉ khi các biểu đồ $D^*(G)$ và $D^*(G')$ (tương ứng $D_*(G)$ và $D_*(G')$) bằng nhau.

#### Mệnh đề 16 {#lie-ix-s4-prop-16 .statement tag=01CZ}

Với mọi biểu đồ nghiệm rút gọn D, tồn tại một nhóm Lie compact liên thông G sao cho $D^*(G)$ (tương ứng $D_*(G)$) đẳng cấu với D.

a) Bằng cách thay thế D, nếu cần, bởi biểu đồ nghịch đảo của nó, ta quy về việc xây dựng G sao cho $D^*(G)$ đẳng cấu với D. Đặt $D = (M,M_0,R)$; khi đó $\mathbf{Q}\otimes M$ là tổng trực tiếp của $\mathbf{Q}\otimes M_0$ và không gian con vectơ V(R) sinh bởi R. Hơn nữa, vì các nghiệm nghịch đảo nhận các giá trị nguyên trên M, phép chiếu của M lên V(R) song song với $\mathbf{Q}\otimes M_0$ được chứa trong nhóm trọng số P(R) của R, do đó M là một nhóm con của $M_0\oplus P(R)$ có chỉ số hữu hạn. Kí hiệu $D'$ là biểu đồ $(M_0\oplus P(R),M_0,R)$.

b) Cho $\mathfrak{a}$ là một đại số Lie nửa đơn phức có hệ nghiệm chính tắc đẳng cấu với $R\subset \mathbf{C}\otimes V(R)$ (Ch. VIII, §4, no. 3), và cho $\mathfrak{g}_1$ là một dạng thực compact của $\mathfrak{a}($§3, no. 2, Định lý 1). Cho $G_1$ là một nhóm Lie thực đơn liên sao cho đại số Lie của nó đẳng cấu với $\mathfrak{g}_1$; khi đó $G_1$ là compact (§1, no. 4, Định lý 1). Cho $T_1$ là một xuyến cực đại của $G_1$. Theo Định lý 1, biểu đồ $D^*(G_1,T_1)$ đẳng cấu với $(P(R),0,R)$.

c) Cho $T_0$ là một xuyến có chiều bằng hạng của $M_0$; khi đó $D^*(T_0,T_0)$ đẳng cấu với $(M_0,M_0,\emptyset )$, do đó $D^*(G_1\times T_0,T_1\times T_0)$ đẳng cấu với $D'$ (Ví dụ 2).

d) Cuối cùng, cho N là nhóm con hữu hạn của $T_1\times T_0$ trực giao với M. Đặt $G = (G_1\times T_0)/N, T = (T_1\times T_0)/N$. Khi đó G là một nhóm Lie compact liên thông, T là một xuyến cực đại của G, và $D(G,T)$ đẳng cấu với D (Ví dụ 3).

#### Chú giải {#lie-ix-s4-n9-sch-1 .statement tag=01D0}

Việc phân loại các nhóm Lie compact liên thông theo đẳng cấu do đó được quy về việc phân loại các biểu đồ nghiệm rút gọn. Các nhóm Lie compact nửa đơn liên thông tương ứng với các biểu đồ nghiệm rút gọn $(M,M_0,R)$ sao cho $M_0= 0$; cho một biểu đồ như thế là tương đương với cho một hệ nghiệm rút gọn R trong một không gian vectơ V trên $\mathbf{Q}$ và một nhóm con M của V sao cho $Q(R)\subset M\subset P(R)$.

#### Nhận xét 3 {#lie-ix-s4-n9-rem-3 .statement tag=01D1}

Cho $T'$ là một xuyến cực đại khác của G, B (tương ứng $B'$) là một cơ sở của hệ nghiệm $R(G,T)$ (tương ứng $R(G',T')$) (Chương VI, §1, no. 5, Định nghĩa 2). Tồn tại các phần tử $g\in G$ sao cho Int $g$ ánh xạ T lên $T'$ và B lên $B'$, và các phần tử này tạo thành một lớp ghép duy nhất modulo Int(T) (vì T và $T'$ liên hợp, ta có thể giả sử rằng $T = T'$, và chỉ cần áp dụng Chương VI, §1, no. 5, Nhận xét 4 và Mệnh đề 9 của no. 4). Suy ra đẳng cấu từ T đến $T'$ cảm sinh bởi Int $g$ không phụ thuộc vào lựa chọn $g$; do đó điều tương tự cũng đúng cho $D_*$(Int $g$) và $D^*$(Int $g$). Diễn đạt lại Chương VIII, §5, no. 3, Nhận xét 2, với những thay đổi thích hợp, giờ đây ta có thể định nghĩa xuyến cực đại chính tắc của G, các biểu đồ nghiệm đồng biến và phản biến chính tắc của G, ...

### 10. TỰ ĐẲNG CẤU CỦA MỘT NHÓM LIE COMPACT LIÊN THÔNG

Kí hiệu Aut(G) là nhóm Lie các tự đẳng cấu của G (Chương III, §10, no. 2), và Aut(G$,T$) là nhóm con đóng của Aut(G) gồm các phần tử $u$ sao cho $u(T) = T$. Ta đã thấy (§1, no. 4, Hệ quả 5 của Mệnh đề 4) rằng thành phần liên thông đơn vị của Aut(G) là nhóm Int(G) của các tự đẳng cấu trong; kí hiệu Int$_G(H)$ là ảnh trong Int(G) của một nhóm con H của G.

Cho D là biểu đồ đồng biến của G đối với T; kí hiệu Aut(D) là nhóm các tự đẳng cấu của nó, và W(D) là nhóm Weyl của nó. Ánh xạ $u \rightarrow D_*(u)$ là một đồng cấu từ Aut(G$,T$) đến Aut(D). Mệnh đề 15 của no. 9 cho ngay:

#### Mệnh đề 17 {#lie-ix-s4-prop-17 .statement tag=01D2}

Đồng cấu Aut(G$,T$)$\rightarrow$ Aut(D) là toàn ánh, với hạt nhân Int$_G(T)$.

Chú ý rằng Aut(G$,T$)$\cap$ Int(G) = Int$_G(N_G(T))$ và ảnh của Int$_G(N_G(T))$ trong Aut(D) là W(D) (no. 5, Mệnh đề 10). Do đó, Mệnh đề 17 cho một đẳng cấu

Aut(G$,T$)$/$(Aut(G$,T$)$\cap$ Int(G)) $\rightarrow$ Aut(D)$/W(D)$.

Hơn nữa, Aut(G) = Int(G).Aut(G$,T$). Thật vậy, nếu $u$ thuộc Aut(G), $u(T)$ là một xuyến cực đại của T, nên liên hợp với T, và tồn tại một tự đẳng cấu trong $v$ của G sao cho $u(T) =v$(T), nói cách khác $v^{-1}u\in$ Aut(G$,T$). Suy ra Aut(G)$/$Int(G) có thể được đồng nhất với Aut(G$,T$)$/$(Aut(G$,T$)$\cap$Int(G)), nên theo điều trên ta có dãy khớp

$1\rightarrow$ Int(G) $\rightarrow$ Aut(G) $\rightarrow$ Aut(D)$/W(D)\rightarrow 1$. (16)

Do đó:

#### Mệnh đề 18 {#lie-ix-s4-prop-18 .statement tag=01K9}

Nhóm Aut(G)$/$Int(G) đẳng cấu với Aut(D)$/W(D)$.

Đặc biệt, giả sử G là nửa đơn; khi đó nhóm Aut(D) có thể được đồng nhất với nhóm con của $A(R(G,T))$ (Chương VI, §1, no. 1) gồm các phần tử $u$ sao cho $u(X(T))\subset X(T)$, và nhóm con W(D) có thể được đồng nhất với $W(R(G,T))$.

#### Hệ quả {#lie-ix-s4-n10-cor-1 .statement tag=01D3}

Nếu G liên thông đơn, hoặc nếu C(G) rút về phần tử đơn vị, thì nhóm Aut(G)$/$Int(G) đẳng cấu với nhóm các tự đẳng cấu của đồ thị Dynkin của $R(G,T)$.

Điều này suy ra từ phần trước và Chương VI, §4, no. 2, Hệ quả của Mệnh đề 1.

Bây giờ ta sẽ chứng minh rằng mở rộng (16) có các tiết diện.

Với mọi $\alpha \in R(G,T)$, ký hiệu $V(\alpha )$ là không gian con vectơ hai chiều của $\mathfrak{g}$ sao cho $V(\alpha )_{(\mathbf{C})}=\mathfrak{g}^{\alpha}+\mathfrak{g}^{-\alpha}$; ký hiệu K là dạng bậc hai liên kết với dạng Killing của $\mathfrak{g}$.

#### Định nghĩa 3 {#lie-ix-s4-def-3 .statement tag=01D4}

Một khung của $(G,T)$ là một cặp $(B,(U_{\alpha})_{\alpha\in B})$, trong đó B là một cơ sở của $R(G,T)$ (Chương VI, §1, no. 5, Định nghĩa 2) và trong đó, với mọi $\alpha \in B,U_{\alpha}$ là một phần tử của $V(\alpha )$ sao cho $K(U_{\alpha}) =-1$.

Một khung của G là một xuyến cực đại T của G cùng với một khung của $(G,T)$.

#### Bổ đề 3 {#lie-ix-s4-lem-3 .statement tag=01D5}

Cho $B_0$ là một cơ sở của $R(G,T)$. Nhóm Int$_G(T)$ tác động đơn bắc cầu trên tập hợp các khung của $(G,T)$ có dạng $(B_0,(U_{\alpha})_{\alpha\in B_0})$.

Với mọi $\alpha \in B_0$, ký hiệu $K(\alpha )$ là sự hạn chế của dạng bậc hai K lên $V(\alpha )$; phép toán của T trên $V(\alpha )$ xác định một cấu xạ $\iota_{\alpha}: T\rightarrow \mathbf{S}\mathbf{O}(K(\alpha ))$. Ta đã thấy ở no. 4 rằng $\mathbf{S}\mathbf{O}(K(\alpha ))$ có thể được đồng nhất với $\mathbf{U}$ sao cho $\iota_{\alpha}$ được đồng nhất với nghiệm $\alpha$. Vì $B_0$ là một cơ sở của R, nên nó là một cơ sở của $\mathbf{Z}$-môđun Q(R) được sinh bởi các nghiệm, do đó là một cơ sở của môđun con $X(T/C(G))$ của X(T). Suy ra tích của các cấu xạ $\iota_{\alpha}$ cảm sinh một đẳng cấu từ $T/C(G)$ tới tích của các nhóm $\mathbf{S}\mathbf{O}(K(\alpha ))$. Nhưng nhóm sau tác động đơn bắc cầu lên tập hợp các khung của $(G,T)$ có thành phần thứ nhất là $B_0$.

#### Mệnh đề 19 {#lie-ix-s4-prop-19 .statement tag=01D6}

Nhóm Int(G) tác động đơn bắc cầu trên tập hợp các khung của G.

Cho $e= (T,B,(U_{\alpha}))$ và $e'= (T',B',(U'_{\alpha}))$ là hai khung của G. Tồn tại các phần tử $g$ trong G sao cho (Int $g$)$(T) = T'$, và các phần tử này tạo thành một lớp ghép duy nhất modulo $N_G(T)$. Do đó, ta có thể giả sử rằng $T = T'$, và ta phải chứng minh rằng tồn tại một phần tử duy nhất của Int$_G(N_G(T))$ biến đổi $e$ thành $e'$. Theo Chương VI, §1, no. 5, Nhận xét 4, tồn tại một phần tử duy nhất $w$ của W(R) sao cho $w(B) = B'$. Vì W(R) có thể được đồng nhất với $N_G(T)/T$, nên tồn tại $n\in N_G(T)$ sao cho $w=$ Int $n$, và $n$ được xác định duy nhất modulo T. Do đó, ta có thể giả sử rằng $B = B'$, và ta phải chứng minh rằng tồn tại một phần tử duy nhất của Int$_G(T)$ biến đổi $e$ thành $e'$, mà đó chỉ là Bổ đề 3.

#### Hệ quả {#lie-ix-s4-n10-cor-2 .statement tag=01D7}

Let $e$ be a framing of $(G,T)$ và cho E là nhóm các tự đẳng cấu của G để $e$ ổn định. Khi đó Aut(G) là tích nửa trực tiếp của E bởi Int(G), và Aut(G$,T$) là tích nửa trực tiếp của E bởi Int(G) $\cap$ Aut(G$,T$) $=$ Int$_G(N_G(T))$.

Thật vậy, mọi phần tử của Aut(G) biến đổi $e$ thành một framing của G. Theo Mệnh đề 19, mọi lớp kề của Aut(G) modulo Int(G) đều gặp E tại đúng một điểm, suy ra mệnh đề thứ nhất. Mệnh đề thứ hai được chứng minh theo cùng cách.

#### Nhận xét {#lie-ix-s4-n10-rem-1 .statement tag=01D8}

Cho G và $G'$ là hai nhóm Lie compact liên thông, và cho $e=$ $(T,B,(U_{\alpha}))$ và $e'= (T',B',(U'_{\alpha}))$ lần lượt là các framing của G và $G'$. Cho X là tập hợp các đẳng cấu từ G đến $G'$ đưa $e$ thành $e'$. Ánh xạ $f \rightarrow D^*(f)$ (tương ứng $D_*(f)$) là một song ánh từ X lên tập các đẳng cấu từ $D^*(G',T')$ đến $D^*(G,T)$ (tương ứng từ $D_*(G,T)$ đến $D_*(G',T')$) đưa $B'$ thành B (tương ứng B thành $B'$). Quả vậy, điều này suy ra ngay từ Mệnh đề 15 và Bổ đề 3.

### Bài tập {#lie-ix-s4-exercises}

Xem [các bài tập của § 4](exercises/s4/).
