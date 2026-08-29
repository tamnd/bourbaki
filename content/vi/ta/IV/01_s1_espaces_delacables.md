---
book: ta
book_title: Topologie algébrique
chapter: IV
chapter_title: ESPACES DÉLAÇABLES
section: 1
section_title: Espaces délaçables
lang: vi
source: ta-i-iv-fr
book_pages: TA IV.340-TA IV.351, TA IV.455-TA IV.457
pdf_pages: 0356-0367, 0471-0473
extraction: native
subsections:
    - "no": 1
      title: Espaces simplement connexes par arcs
      page: 340
      pdf_page: 356
    - "no": 2
      title: Espaces délaçables
      page: 340
      pdf_page: 356
    - "no": 3
      title: Revêtement universel d’un espace délaçable
      page: 342
      pdf_page: 358
    - "no": 4
      title: Exemples
      page: 346
      pdf_page: 362
statements: 20
exercises: 6
content_sha256: d0ea12d67933abbb664a2acc8cc94e05c2c0f025015f90179b63bd984cd22b11
translated_from: content/en-mt/ta/IV/01_s1_espaces_delacables.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 6fc423d8711798f8f570057261de9eb8f2b9492c8563a065ae96d37c64302106
translation_model: gpt-5-6-mini, gpt-5-mini
translation_run: translate-vi-9760c561
glossary_version: 34
glossary_terms_sha256: 5f62f89dd1099e144e468ebd83b9e3cc44f0561773f59b850d4235e978a90d71
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 1. KHÔNG GIAN ĐƠN LIÊN

### 1. Các không gian đơn liên theo cung

#### Định nghĩa 1 {#ta-iv-s1-def-1 .statement tag=0208}

Một không gian tôpô X được gọi là đơn liên theo cung nếu nó liên thông theo cung và nếu mọi vòng trong X là đồng luân nghiêm ngặt với một vòng hằng.

Không gian rỗng là đơn liên theo cung. Để một không gian liên thông theo cung X là đơn liên theo cung, điều kiện cần và đủ là nhóm $\pi_1(X, x)$ được thu gọn về phần tử đơn vị đối với mọi điểm $x$ của X (III, p. 292, prop. 2). Chỉ cần điều này đúng đối với một điểm $x$ của X là đủ (loc. cit.).

Mọi không gian tôpô đồng luân với một không gian đơn liên theo cung đều là đơn liên theo cung. Thật vậy, nó liên thông theo cung (III, p. 260) và, tại mọi điểm, nhóm Poincaré của nó được thu gọn về phần tử đơn vị (III, p. 296, cor. 2 of prop. 6). Đặc biệt, một không gian tôpô đồng luân với một điểm là đơn liên theo cung.

Một không gian tôpô đơn liên theo cung và liên thông theo cung địa phương là đơn liên (III, p. 309, cor. 2 of prop. 1).

### 2. Các không gian không cuộn được

#### Định nghĩa 2 {#ta-iv-s1-def-2 .statement tag=0209}

Một không gian tôpô B được gọi là không cuộn được nếu nó liên thông theo cung địa phương và nếu mọi điểm $b$ của B có một lân cận V sao cho đồng cấu của $\pi_1(V, b)$ vào $\pi_1(B, b)$ suy ra từ đơn ánh chính tắc có ảnh là phần tử đơn vị.

Một không gian tôpô liên thông theo cung địa phương là không cuộn được khi và chỉ khi mỗi thành phần liên thông của nó là như vậy.

Cho B là một không gian tôpô liên thông theo cung địa phương. Giả sử rằng mọi điểm của B có một lân cận V không cuộn được. Khi đó B là không cuộn được.

Mọi không gian tôpô liên thông theo cung địa phương và đơn liên theo cung đều là không cuộn được. Đây đặc biệt là trường hợp của một không gian liên thông theo cung địa phương đồng luân với một điểm.

#### Nhận xét 1 {#ta-iv-s1-n2-rem-1 .statement tag=020A}

Tồn tại các không gian tôpô B, liên thông và liên thông theo cung địa phương, sao cho một số điểm $a$ của B, nhưng không phải tất cả, có một lân cận V sao cho đồng cấu của $\pi_1(V, a)$ vào $\pi_1(B, a)$ là tầm thường (III, p. 336, exerc. 6).

#### Nhận xét 2 {#ta-iv-s1-n2-rem-2 .statement tag=020B}

Cho B là một không gian không cuộn được; mọi phép toán của groupoid $\varpi (B)$ trên một B-không gian đều không có đơn phương địa phương (cf. III, p. 313, remark). Đặc biệt, để một ánh xạ $p: E\rightarrow B$ biến E thành một phủ của B, điều kiện cần và đủ là nó étale, tách được và thỏa mãn tính chất nâng đường (III, p. 315, corollary 3).

#### Mệnh đề 1 {#ta-iv-s1-prop-1 .statement tag=020C}

Không gian tích của một họ hữu hạn các không gian không cuộn được là không cuộn được.

Chỉ cần chứng minh rằng, nếu A và B là hai không gian không cuộn được, thì điều tương tự cũng đúng với tích của chúng $A\times B$. Trong các điều kiện này, không gian $A\times B$ thực sự là liên thông theo cung địa phương (III, p. 261, prop. 9). Cho $(a, b)$ là một điểm của $A\times B$. Theo giả thiết tồn tại một lân cận U của $a$ (tương ứng, một lân cận V của $b$) sao cho ảnh của đồng cấu $i_*:\pi_1(U, a)\rightarrow \pi_1(A, a)$ suy ra từ đơn ánh chính tắc $i: U\rightarrow A$ (tương ứng, của đồng cấu $j_*:\pi_1(V, b)\rightarrow \pi_1(B, b)$ suy ra từ đơn ánh chính tắc $j: V\rightarrow B$) được thu gọn về phần tử đơn vị. Khi đó $U\times V$ là một lân cận của $(a, b)$ trong $A\times B$. Đồng cấu $\pi_1(U\times V,(a, b))\rightarrow \pi_1(A\times B,(a, b))$ đồng nhất với đồng cấu $(i_*, j_*)$ (III, p. 297, corollary of prop. 4). Ảnh của nó do đó được thu gọn về phần tử đơn vị. Điều này chứng minh rằng $A\times B$ là không cuộn được.

#### Mệnh đề 2 {#ta-iv-s1-prop-2 .statement tag=020D}

a) Mọi phủ của một không gian không cuộn được đều là không cuộn được.

b) Ngược lại, cho $p: E\rightarrow B$ là một ánh xạ étale và toàn ánh và giả sử rằng E là một không gian không cuộn được. Khi đó B là không cuộn được.

a) Cho B là một không gian tôpô không cuộn được và $(E, p)$ là một phủ của B. Khi đó không gian E liên thông theo cung địa phương. Cho $x$ là một điểm của E, đặt $b=p(x)$, và cho V là một lân cận của $b$ trong B sao cho đồng cấu chính tắc $\pi_1(V, b)\rightarrow \pi_1(B, b)$ là tầm thường. Gọi $i: V\rightarrow B$ và $j:\overset{-1}{p}(V)\rightarrow E$ là các đơn ánh chính tắc. Theo giả thiết, ảnh của đồng cấu $\pi_1(i, b)$ được thu gọn về phần tử đơn vị. Vì $p\circ i=j\circ p$ và $\pi_1(p, x)$ là đơn ánh, ảnh của đồng cấu $\pi_1(j, x)$ được thu gọn về phần tử đơn vị. Điều này chứng minh rằng E là không cuộn được.

b) Không gian B liên thông theo cung địa phương. Cho $b$ là một điểm của B và cho $x$ là một điểm của $E_b$. Vì $p$ là étale, tồn tại một lân cận U của $x$ trong E sao cho $p$ cảm sinh một đồng phôi từ U lên $p(U)$. Cho V là một lân cận của $x$ trong E được chứa trong U sao cho đồng cấu $\pi_1(j, x)$ là tầm thường, trong đó $j: V\rightarrow E$ là đơn ánh chính tắc. Cho $q: V\rightarrow p(V)$ là ánh xạ suy ra từ $p$ bằng cách chuyển qua các không gian con; nó là một đồng phôi. Cũng gọi $i$ là đơn ánh chính tắc của $p(V)$ vào B. Ta có $p\circ j=i\circ q$, do đó $\pi_1(i, b)\circ \pi_1(q, x) =\pi_1(p, x)\circ \pi_1(j, x)$ là đồng cấu tầm thường. Vì đồng cấu $\pi_1(q, x)$ là một đẳng cấu, đồng cấu $\pi_1(i, b)$ là tầm thường. Suy ra không gian B là không cuộn được.

#### Mệnh đề 3 {#ta-iv-s1-prop-3 .statement tag=020E}

Cho B là một không gian tôpô không cuộn được. Cho $(Y, q)$ là một phủ của B và $(Z, p)$ là một phủ của Y. Không gian tôpô Z, được trang bị bởi ánh xạ $q\circ p$, khi đó là một phủ của B.

Thực ra, ánh xạ $q\circ p$ là étale (I, p. 29, mệnh đề 6) và tách được (I, p. 25, mệnh đề 2). Theo Nhận xét 2 ở trên, do đó chỉ cần chứng minh rằng nó thỏa mãn tính chất nâng đường. Cho $z$ là một điểm của Z và cho $c:\mathbf{I}\rightarrow B$ là một đường trong B có gốc $q(p(z))$. Tồn tại một đường $c'$ có gốc $p(z)$ trong Y nâng $c$, vì Y là một phủ của B (III, p. 302, Hệ quả 2). Vì Z là một phủ của Y, tồn tại một đường $c''$ có gốc $z$ trong Z nâng $c'$; đường $c''$ nâng $c$. Điều này chứng minh mệnh đề.

### 3. Phủ phổ quát của một không gian không rối

Cho B là một không gian tôpô và cho $b$ là một điểm của B. Nhắc lại rằng $\Lambda_b(B)$ ký hiệu không gian con của $\mathscr{C}_c(\mathbf{I}; B)$ được tạo bởi các đường có gốc $b$, được trang bị tôpô thương của tôpô hội tụ compact. Ta ký hiệu bởi $e_B: \Lambda_b(B)\rightarrow$ B ánh xạ gán cho một đường điểm mút của nó; ánh xạ này liên tục. Ta ký hiệu bởi $\lambda_b(B)$ không gian thương của $\Lambda_b(B)$ theo quan hệ đồng luân ngặt và trang bị cho nó tôpô thương. Vì hai đường đồng luân ngặt có cùng điểm mút, ánh xạ $e_B$ xác định, bằng cách chuyển qua thương, một ánh xạ liên tục $\varepsilon_B:\lambda_b(B)\rightarrow B$, được gọi là ánh xạ điểm mút.

#### Định lý 1 {#ta-iv-s1-thm-1 .statement tag=020F}

Cho B là một không gian tôpô liên thông, địa phương liên thông theo cung, và cho $b$ là một điểm của B. Các tính chất sau là tương đương:

(i) Không gian B là không rối.

(ii) Tồn tại một phủ khác rỗng của B đơn liên theo cung.

(iii) Không gian $\lambda_b(B)$, được trang bị ánh xạ điểm mút $\varepsilon_B:\lambda_b(B)\rightarrow B$, là một phủ của B.

(iv) Nhóm $\pi_1(B, b)$ là rời rạc đối với tôpô khả dụng.

(v) Nhóm $\pi_1(B, b)$ là rời rạc đối với tôpô thương của tôpô hội tụ compact.

Hơn nữa, khi các điều kiện này được thỏa mãn, không gian $\lambda_b(B)$ là đơn liên theo cung, đơn liên, Galois với nhóm $\pi_1(B, b)^{\circ}$, và phủ có điểm $(\lambda_b(B), \varepsilon_b)$ là một phủ phổ quát của không gian có điểm $(B, b)$.

Từ định nghĩa của một không gian không rối suy ra rằng nhóm con của $\pi_1(B, b)$ rút gọn về phần tử đơn vị là khả dụng khi và chỉ khi B là không rối. Điều này chứng minh sự tương đương (i)$\Leftrightarrow ($iv). Hơn nữa, sự tương đương của các tính chất (iv) và (v) suy ra từ các Nhận xét 4 và 5 của III, p. 320.

(iv)$\Rightarrow ($ii). Theo III, p. 316, Mệnh đề 5, tồn tại một phủ $(E, p)$ của B và một điểm $x\in E_b$ sao cho $p_*(\pi_1(E, x)) =\{e\}$; đặc biệt, $\pi_1(E, x)$ rút gọn về phần tử đơn vị. Thành phần liên thông theo cung của $x$ trong E khi đó là một phủ khác rỗng của B (I, p. 80, Hệ quả 1 của Mệnh đề 6), đơn liên theo cung.

(ii)$\Rightarrow ($iii). Cho E là một phủ khác rỗng của B đơn liên theo cung. Cho $x$ là một điểm của $E_b$ (tồn tại một điểm như vậy vì B liên thông, I, p. 74, Mệnh đề 4). Phép chiếu $q: E\rightarrow$ B cảm sinh một phép đồng phôi $\Lambda_x(E)\rightarrow \Lambda_b(B)$ (III, p. 302, Hệ quả 2 của Mệnh đề 3), do đó, bằng cách chuyển qua các thành phần liên thông theo cung, một phép đồng phôi $q_*:\lambda_x(E)\simeq \lambda_b(B)$. Ánh xạ điểm mút $\Lambda_x(E)\rightarrow E$ liên tục và mở, vì E liên thông địa phương theo cung (III, p. 264, Hệ quả). Ánh xạ $\varepsilon_E:\lambda_x(E)\rightarrow E$ mà nó xác định bằng cách chuyển qua các thành phần liên thông theo cung do đó liên tục và mở. Ánh xạ $\varepsilon_E\circ (q_*)^{-1}:\lambda_b(B)\rightarrow E$ là song ánh, liên tục và mở. Điều này chứng minh rằng không gian tôpô $\lambda_b(B)$, được trang bị tôpô hội tụ compact và ánh xạ điểm mút, là một phủ của B.

(iii)$\Rightarrow ($v). Thực ra, tập hợp $\pi_1(B, b)$, được trang bị tôpô thương của tôpô hội tụ compact, được đồng nhất với thớ của không gian B $\lambda_b(B)$ trên lớp của vòng lặp hằng tại $b$. Nếu $\lambda_b(B)$ là một phủ của B, thì $\pi_1(B, b)$ là rời rạc đối với tôpô hội tụ compact.

Giả sử rằng các khẳng định này được kiểm chứng. Từ những điều trên, không gian $\lambda_b(B)$ khi đó là một phủ của B đơn liên theo cung, do đó đơn liên. Không gian có điểm $(\lambda_b(B), \varepsilon_b)$ do đó là một phủ phổ quát của $(B, b)$ (I, p. 126, hệ quả của Mệnh đề 3) và phủ $\lambda_b(B)$ là một phủ Galois của B (I, p. 120, Mệnh đề 1). Đồng cấu chính tắc $h_{(\lambda_b(B),\varepsilon_b)}:\pi_1(B, b)\rightarrow$ Aut$_B(\lambda_b(B))$ khi đó là một đẳng cấu (III, p. 306, Mệnh đề 5).

#### Nhận xét 1 {#ta-iv-s1-n3-rem-1 .statement tag=020G}

Cho B là một không gian liên thông tháo được và cho $b$ là một điểm của B. Từ Định lý 1, (iv), suy ra rằng mọi phép toán của nhóm $\pi_1(B, b)$ đều khả dụng. Do đó, mọi tập hợp $\pi_1(B, b)$ là đẳng cấu với một tập hợp $\pi_1(B, b)$ $E_b$, trong đó E là một phủ của B (III, p. 318, mệnh đề 7). Cũng nhắc lại (III, p. 310, mệnh đề 2) rằng nếu E và $E'$ là các phủ của B, ánh xạ $f\mapsto f_b$ cảm sinh một song ánh của tập hợp các cấu xạ của các không gian B từ E vào $E'$ lên tập hợp các cấu xạ của các tập hợp $\pi_1(B, b)$ từ $E_b$ vào $E'_b$.

*Trong ngôn ngữ của các phạm trù, người ta nói rằng hàm tử liên kết với một phủ E của B thớ $E_b$ là một tương đương của các phạm trù từ phạm trù các phủ của B vào phạm trù các tập hợp $\pi_1(B, b)$.*

#### Hệ quả 1 {#ta-iv-s1-thm-1-cor-1 .statement tag=020H}

Cho B là một không gian tôpô tháo được và cho $b$ là một điểm của B. Cho E là một phủ liên thông của B và cho $x$ là một điểm của thớ $E_b$. Các tính chất sau là tương đương:

(i) Nhóm $\pi_1(E, x)$ là tầm thường.

(ii) Không gian E là đơn liên.

(iii) Không gian có điểm $(E, x)$ là một phủ phổ quát của $(B, b)$.

Kéo theo (i)$\Rightarrow$(ii) đã được chứng minh dưới giả thiết duy nhất rằng không gian B là liên thông và liên thông địa phương theo cung (III, p. 309, hệ quả 2 của mệnh đề 1), và kéo theo (ii)$\Rightarrow$(iii) không cần bất kỳ giả thiết nào (I, p. 126, hệ quả).

Ta chứng minh (iii)$\Rightarrow$(i). Theo Định lý 1 của IV, p. 342, tồn tại một phủ $E'$ của B và một điểm $x'$ của thớ $E'_b$ sao cho nhóm $\pi_1(E', x')$ thu về phần tử đơn vị. Dưới giả thiết (iii), tồn tại một B-cấu xạ có điểm $f: (E, x)\rightarrow (E', x')$. Gọi $p: E\rightarrow$ B và $p': E'\rightarrow B$ là các phép chiếu của các phủ E và $E'$; ta có $p=p'\circ f$, do đó $\pi_1(p, x) =\pi_1(p', x')\circ \pi_1(f, x)$. Vì nhóm $\pi_1(E', x')$ là tầm thường, đồng cấu đơn cấu $\pi_1(p, x)$ có phần tử đơn vị làm ảnh. Điều này chứng minh rằng nhóm $\pi_1(E, x)$ thu về phần tử đơn vị.

#### Hệ quả 2 {#ta-iv-s1-thm-1-cor-2 .statement tag=020I}

Cho B là một không gian tôpô tháo được và cho $b$ là một điểm của B. Cho $(E, x)$ là một phủ phổ quát của không gian có điểm $(B, b)$. Với mọi phủ $E'$ của B và mọi điểm $x'$ của $E'_b$, B-cấu xạ duy nhất $f: E\rightarrow E'$ sao cho $f(x) =x'$ làm cho E là một phủ của $E'$. Không gian có điểm $(E, x)$ khi đó là một phủ phổ quát của $(E', x')$.

Theo mệnh đề 7 của I, p. 81, không gian E, được trang bị ánh xạ $f$, là một phủ của $E'$. Khẳng định cuối cùng khi đó suy ra từ Hệ quả 1.

Cho B là một không gian tôpô tháo được và cho $a,b$ là hai điểm của B. Không gian tôpô thương $\varpi_{a,b}(B)$ là đồng phôi với không gian $\pi_1(B, a)$, được trang bị tôpô thương của tôpô compact-mở (III, p. 293, nhận xét 3), và do đó là rời rạc theo Định lý 1 của IV, p. 342. Do đó, lớp đồng luân ngặt của mọi đường đi trong B nối $a$ với $b$ là một tập con mở của $\Lambda_{a,b}(B)$. Nói chung:

#### Mệnh đề 4 {#ta-iv-s1-prop-4 .statement tag=020J}

Cho B là một không gian tôpô tháo được. Quan hệ đồng luân ngặt là một quan hệ tương đương mở trong không gian tôpô $\mathscr{C}_c(\mathbf{I}; B)$.

Trước hết giả sử rằng không gian B là liên thông đơn theo cung. Gọi $\varphi : \Lambda (B)\rightarrow B\times B$ là ánh xạ liên kết với một đường đi $c$ trong B cặp $(c(0), c(1))$ được tạo bởi điểm đầu và điểm cuối của nó. Để hai đường đi trong B là đồng luân ngặt, điều kiện cần và đủ là chúng có cùng điểm đầu và cùng điểm cuối (III, p. 292, mệnh đề 2). Vì không gian B là liên thông và liên thông địa phương theo cung, ánh xạ $\varphi$ là toàn ánh, liên tục và mở (III, p. 262, mệnh đề 10). Do đó, quan hệ đồng luân ngặt là mở (TG, I, p. 32, mệnh đề 3).

Trong trường hợp tổng quát, cho E là một phủ liên thông đơn bởi các đường của B, khác rỗng nếu B $=\not\emptyset$. Phủ này là toàn ánh vì B liên thông (I, p. 74, mđ. 4). Ký hiệu $p$ là phép chiếu của không gian B E và gọi $\widetilde{p}: \Lambda (E)\rightarrow \Lambda (B)$ là ánh xạ gán cho một đường đi $c$ trong E đường đi $p\circ c$. Được trang bị ánh xạ $\widetilde{p}$, Λ(E) là một phủ của Λ(B) (III, p. 302, hệ quả 1 của mđ. 3). Để hai đường đi trong B đồng luân ngặt với nhau, điều kiện cần và đủ là chúng là ảnh qua ánh xạ $\widetilde{p}$ của hai đường đi đồng luân ngặt trong E (III, p. 302, mđ. 4). Cho U là một tập con mở của không gian Λ(B). Tập $(\overset{-1}{\widetilde{p}})(U)$ là mở trong Λ(E) ; theo phần đầu của

chứng minh, tập $U'$ bão hòa của $(\overset{-1}{\widetilde{p}})(U)$ đối với quan hệ đồng luân ngặt là mở trong Λ(E). Vì Λ(E) là một phủ của Λ(B), tập $\widetilde{p}(U')$ là mở trong Λ(B). Điều này chứng minh mệnh đề, vì $\widetilde{p}(U')$ là tập bão hòa của U đối với quan hệ đồng luân ngặt.

### 4. Ví dụ

1) Các không gian co được địa phương

#### Định nghĩa 3 {#ta-iv-s1-def-3 .statement tag=020K}

Một không gian tôpô B được gọi là co được địa phương nếu mọi điểm $b$ của B đều có một lân cận V sao cho không gian có điểm đánh dấu $(V, b)$ là co được (III, p. 234, ví dụ 3).

#### Mệnh đề 5 {#ta-iv-s1-prop-5 .statement tag=020L}

Một không gian tôpô co được địa phương là không thắt nút.

Cho B là một không gian co được địa phương. Cho $b$ là một điểm của B và V là một lân cận của $b$ sao cho $(V, b)$ là một không gian có điểm đánh dấu co được. Không gian V đồng luân với một điểm, do đó $\pi_1(V, b) =\{\varepsilon_b\}$(III, p. 296, hệ quả 3).

Để chứng minh mệnh đề, còn phải chứng minh rằng không gian B liên thông bởi các đường một cách địa phương. Cho $\sigma : V\times \mathbf{I}\rightarrow$ V là một đồng luân có điểm đánh dấu tại $b$ nối ánh xạ hằng có ảnh $b$ với ánh xạ Id$_V$. Với mọi lân cận W của $b$ được chứa trong V, tập $\sigma (W\times \mathbf{I})$ là một lân cận của $b$ vì nó chứa $W =\sigma (W\times  \{1\})$, và nó liên thông bởi các đường vì với mọi $(a, s)\in W\times \mathbf{I}$, ánh xạ $t\mapsto \sigma (a, ts)$ là một đường đi nối $b=\sigma (a,0)$ với $\sigma (a, s)$ trong $\sigma (W\times \mathbf{I})$. Ta hãy chứng minh rằng các tập có dạng $\sigma (W\times \mathbf{I})$ tạo thành một hệ cơ bản các lân cận của $b$. Cho $V'$ là một lân cận mở của $b$ trong B; khi đó, $\overset{-1}{\sigma}(V')$ là một lân cận mở của $\{b\} \times \mathbf{I}$ trong $V\times \mathbf{I}$. Vì không gian $\mathbf{I}$ là compact, phép chiếu pr$_1: V\times \mathbf{I}\rightarrow V$ là thực sự (TG, I, p. 77, hệ quả 5) và pr$_1(\complement \overset{-1}{\sigma}(V'))$ là một tập con đóng của V không chứa $b$. Phần bù của nó W do đó là một lân cận mở của $b$ trong V sao cho $W\times \mathbf{I}\subset \overset{-1}{\sigma}(V')$, do đó $\sigma (W\times \mathbf{I})\subset V'$.

Mọi tập con mở của một không gian số hoặc của một không gian xạ ảnh, thực hoặc phức, có chiều $n$ (xem các Chương VI và VIII) đều không thắt nút, cũng như các mặt cầu Euclid $\mathbf{S}_n$ (TG, VI, p. 11, mđ. 4). Tổng quát hơn, mọi đa tạp tôpô (VAR R, phần thứ hai, p. 7, Ký hiệu và Quy ước) đều không thắt nút. Thực vậy, các không gian này co được địa phương.

2) Nhóm Poincaré của đường tròn. — Không gian tôpô $\mathbf{R}$ đồng luân với một điểm (III, p. 234, ví dụ 4), do đó liên thông đơn bởi các đường (IV, p. 340). Toàn cấu chính tắc $p$ của $\mathbf{R}$ lên $\mathbf{T}=\mathbf{R}/\mathbf{Z}$ làm cho nó trở thành một phủ chính có nhóm $\mathbf{Z}($I, p. 100, ví dụ 4). Không gian tôpô $\mathbf{T}$ là không thắt nút và $(\mathbf{R},0)$ là một phủ phổ quát của $(\mathbf{T},0)$. Từ đó suy ra một đẳng cấu chính tắc của các nhóm $\pi_1(\mathbf{T},0)\rightarrow \mathbf{Z}:$ nó biến lớp của vòng $t\mapsto p(nt)$ tại 0 thành phần tử $n$ của $\mathbf{Z}$. Xét đến ví dụ 6 (I, p. 101), ta suy ra mệnh đề sau.

#### Mệnh đề 6 {#ta-iv-s1-prop-6 .statement tag=020M}

Ánh xạ $p:x\mapsto e^{2\pi ix}$ của $\mathbf{R}$ vào $\mathbf{S}_1$ làm cho $(\mathbf{R},0)$ là một phủ phổ quát của $(\mathbf{S}_1,1)$. Nhóm $\pi_1(\mathbf{S}_1,1)$ đẳng cấu với $\mathbf{Z}$; lớp của đường cong kín $t\mapsto e^{2\pi it}$ là một phần tử sinh của nó. Với mọi số nguyên $n >0$, ánh xạ $z\mapsto z^n$ làm cho $\mathbf{S}_1$ là một phủ Galois có nhóm $\mathbf{Z}/n\mathbf{Z}$ của $\mathbf{S}_1$. Mọi phủ liên thông khác rỗng của $\mathbf{S}_1$ đều đẳng cấu với một trong các phủ này.

Chỉ còn khẳng định cuối cùng cần được chứng minh. Sợi $E_1$ trên 1 của một phủ liên thông khác rỗng E của $\mathbf{S}_1$ được trang bị một phép toán bắc cầu của nhóm $\pi_1(§_1,1)$. Vì các nhóm con của $\mathbf{Z}$ là các tập hợp $n\mathbf{Z}$, với $n\geqslant 0$, ta thấy rằng $E_1$ đẳng cấu với một trong các tập hợp thuần nhất liên kết với các phủ được mô tả ở trên. Vì $\mathbf{S}_1$ liên thông và liên thông cung địa phương, E đẳng cấu với một trong các phủ này.

#### Hệ quả {#ta-iv-s1-n4-cor-1 .statement tag=020N}

Ánh xạ $z\mapsto e^z$ của $\mathbf{C}$ vào $\mathbf{C}^*$ làm cho $(\mathbf{C},0)$ là một phủ phổ quát của $(\mathbf{C}^*,1)$. Nhóm $\pi_1(\mathbf{C}^*,1)$ đẳng cấu với $\mathbf{Z}$; lớp của đường cong kín $t\mapsto e^{2\pi it}$ là một phần tử sinh của nó. Với mọi số nguyên $n >0$, ánh xạ $z\mapsto z^n$ làm cho $\mathbf{C}^*$ là một phủ Galois có nhóm $\mathbf{Z}/n\mathbf{Z}$ của $\mathbf{C}^*$. Mọi phủ liên thông khác rỗng của $\mathbf{C}^*$ đều đẳng cấu với một trong các phủ này.

Ánh xạ $z\mapsto (|z|, z/|z|)$ là một phép đồng phôi của không gian $\mathbf{C}^*$ lên không gian $\mathbf{R}^*_+\times \mathbf{S}^1$ (TG, VI, p. 10, prop. 3); đặc biệt, $\mathbf{C}^*$ là liên thông cung. Vì ánh xạ $x\mapsto e^x$ của $\mathbf{R}$ vào $\mathbf{R}_+^*$ là một phép đồng phôi, suy ra từ mệnh đề 6 rằng ánh xạ $(x, y)\mapsto e^xe^{2\pi iy}$ làm cho $\mathbf{R}^2$ là một phủ của $\mathbf{C}^*$. Khi nhận diện $\mathbf{R}^2$ với $\mathbf{C}$ nhờ ánh xạ $(x, y)\mapsto x+iy$, ta kết luận rằng không gian $\mathbf{C}$, được trang bị ánh xạ $z\mapsto e^z$, là một phủ của $\mathbf{C}^*$. Vì không gian $\mathbf{C}$ liên thông và liên thông cung đơn, phủ có điểm cơ sở $(\mathbf{C},0)$ là một phủ phổ quát của không gian có điểm cơ sở $(\mathbf{C}^*,1)$.

Cũng suy ra từ hệ quả, III, p. 297, rằng nhóm Poincaré của $\mathbf{C}^*$ tại 1 đẳng cấu với $\mathbf{Z}$ và lớp $\gamma$ của đường cong kín $t\mapsto e^{2\pi it}$ là một phần tử sinh của nó.

Cho $n$ là một số nguyên $>0$. Ánh xạ $x\mapsto x^n$ của $\mathbf{R}^*_+$ lên chính nó là một phép đồng phôi; suy ra như trên rằng ánh xạ $z\mapsto z^n$ làm cho $\mathbf{C}^*$ là một phép phủ bậc $n$ của $\mathbf{C}^*$. Nó là Galois với nhóm $\mathbf{Z}/n\mathbf{Z}$. Khẳng định cuối cùng được chứng minh như trong chứng minh của mệnh đề 6.

Với mọi số nguyên $n\geqslant 0$, xuyến $(\mathbf{S}_1)^n$ là một không gian không xoắn (IV, p. 341, mệnh đề 1) và nhóm Poincaré của nó tại mọi điểm là đẳng cấu với $\mathbf{Z}^n($III, p. 297, mệnh đề 4).

Ta sẽ tổng quát hóa các kết quả này trong đoạn 3 dành cho các phép phủ của các nhóm tôpô.

3) Các không gian xạ ảnh thực. --- Cho $n$ là một số nguyên $>0$. Các không gian $\mathbf{S}_n$ và $\mathbf{P}_n(\mathbf{R})$ là liên thông, không rỗng, và ánh xạ chính tắc (TG, VI, p. $13$)$\varphi :\mathbf{S}_n\rightarrow \mathbf{P}_n(\mathbf{R})$ làm cho $\mathbf{S}_n$ là một phép phủ chính của $\mathbf{P}_n(\mathbf{R})$ với nhóm $\{+1,-1\}($I, p. 99, ví dụ 1). Với $n\geqslant 2$, mặt cầu $\mathbf{S}_n$ là đơn liên (I, p. 127, ví dụ 3) và không xoắn, do đó đơn liên theo cung (IV, p. 344, hệ quả 1). Với $n= 1$, ánh xạ $z\mapsto z^2$ của $\mathbf{S}_1$ vào $\mathbf{S}_1$ xác định một quan hệ tương đương trong $\mathbf{S}_1$ mà các lớp của nó là các cặp điểm đối của $\mathbf{S}_1$. Ánh xạ $\varphi :\mathbf{S}_1\rightarrow \mathbf{P}_1(\mathbf{R})$ xác định qua phép chuyển qua thương một song ánh liên tục $\psi :\mathbf{S}_1\rightarrow \mathbf{P}_1(\mathbf{R})$ sao cho $\psi (z^2) =\varphi (z)$. Vì $\mathbf{S}_1$ là một không gian compact, ánh xạ $\psi$ là một phép đồng phôi (TG, I, p. 63, hệ quả 2).

#### Mệnh đề 7 {#ta-iv-s1-prop-7 .statement tag=020O}

Ánh xạ $x\mapsto \varphi (e^{2\pi ix})$ của $\mathbf{R}$ lên $\mathbf{P}_1(\mathbf{R})$ làm cho $(\mathbf{R},0)$ là một phép phủ phổ quát của $(\mathbf{P}_1(\mathbf{R}), \varphi (1))$. Cho $c:\mathbf{I}\rightarrow \mathbf{S}_1$ là đường đi $t\mapsto e^{\pi it}$; lớp của $\varphi (c)$ là một phần tử sinh của nhóm $\pi_1(\mathbf{P}_1(\mathbf{R}), \varphi (1))$, nhóm này đẳng cấu với $\mathbf{Z}$.

Với mọi số nguyên $n\geqslant$ 2 và mọi điểm $x$ của $\mathbf{S}_n$, ánh xạ chính tắc $\varphi :\mathbf{S}_n\rightarrow \mathbf{P}_n(\mathbf{R})$ làm cho $(\mathbf{S}_n, x)$ là một phép phủ phổ quát của $(\mathbf{P}_n(\mathbf{R}), \varphi (x))$. Với mọi đường đi $c$ trong $\mathbf{S}_n$ nối $x$ với $-x$, lớp của $\varphi \circ c$ sinh ra nhóm $\pi_1(\mathbf{P}_n(\mathbf{R}), \varphi (x))$, nhóm này đẳng cấu với $\mathbf{Z}/2\mathbf{Z}$.

4) Thương của một không gian bởi tác động thực sự của một nhóm rời rạc

#### Bổ đề 1 {#ta-iv-s1-lem-1 .statement tag=020P}

Cho X là một không gian tôpô, cho G là một nhóm rời rạc tác động thực sự trong X, và cho $p$ là phép chiếu chính tắc của X lên $X/G$.

Cho $x$ là một điểm của X, cho $K_x$ là nhóm ổn định của nó trong G. Cho $U_1$ là một lân cận của $x$ trong X; tồn tại một lân cận U của $x$ trong X, ổn định dưới $K_x$ và được chứa trong $U_1$ sao cho $g\cdot U\cap U =\emptyset$ nếu $g\notin K_x$ và sao cho ánh xạ chính tắc $p$ cảm sinh một phép đồng phôi từ $U/K_x$ lên một lân cận V của $p(x)$ trong $X/G$.

Theo mệnh đề 8 của TG, III, p. 32, tồn tại một lân cận $U_2$ của $x$ trong X, ổn định dưới $K_x$, sao cho $g\cdot U_2\cap U_2=\emptyset$ nếu $g\notin K_x$ và sao cho ánh xạ chính tắc $p$ cảm sinh một phép đồng phôi từ $U_2/K_x$ lên một lân cận của $p(x)$ trong $X/G$.

Vì ánh xạ chính tắc $U_2\rightarrow U_2/K_x$ là đóng (TG, III, p. 28, mệnh đề 2), tồn tại một lân cận mở U của $x$ được chứa trong $U_1\cap U_2$ và ổn định dưới $K_x($I, p. 75, bổ đề). Quan hệ tương đương trong $U_2$ được xác định bởi $K_x$ cũng là mở (TG, III, p. 10, bổ đề 2). Từ TG, I, p. 32, mệnh đề 4, suy ra rằng ánh xạ chính tắc cảm sinh một phép đồng phôi từ $U/K_x$ lên một lân cận mở của $p(x)$ trong $X/G$, do đó có bổ đề.

#### Mệnh đề 8 {#ta-iv-s1-prop-8 .statement tag=020Q}

Cho X là một không gian tôpô và cho G là một nhóm rời rạc tác động đúng trên X. Ta ký hiệu $p$ là phép chiếu chính tắc của X lên $X/G$.

a) Giả sử rằng X liên thông bằng cung và nhóm G được sinh bởi các nhóm ổn định của các điểm của X. Khi đó đồng cấu chính tắc $\pi_1(X, x)\rightarrow \pi_1(X/G, p(x))$ là toàn ánh với mọi điểm $x$ của X. Đặc biệt, $X/G$ là liên thông đơn bằng cung nếu X là như vậy.

b) Nếu không gian X là unloopable, không gian $X/G$ là unloopable.

a) Tập hợp N gồm các phần tử $g\in G$ sao cho tồn tại một đường đi $c_g:\mathbf{I}\rightarrow X$ thỏa mãn $c_g(0) =x,c_g(1) =g\cdot x$ và sao cho vòng $p\circ c_g$ trong $X/G$ đồng luân nghiêm ngặt với một vòng hằng là một nhóm con của G. Nếu $g\in G$ và nếu tồn tại một điểm $y$ của X sao cho $g\cdot y=y$, ta chọn một đường đi $c:\mathbf{I}\rightarrow X$ nối $x$ với $y$; khi đó đường đi $c'=c*$ $\overline{(g\cdot c)}$ thỏa mãn $c'(0) =x,c'(1) =g\cdot x$ và $[p\circ c'] = [p\circ c][p\circ (g\cdot c)]^{-1}=e_{p(x)}$, do đó $p\circ c'$ đồng luân nghiêm ngặt với một vòng hằng. Vì G được sinh bởi các nhóm ổn định của các điểm của X, suy ra rằng N = G.

Cho $c$ là một vòng trong $X/G$ tại $p(x)$. Theo Định lý 4 của III, p. 287, tồn tại một đường đi $\widetilde{c}:\mathbf{I}\rightarrow X$ nâng $c$ sao cho $\widetilde{c}(0) =x$. Vì $p(\widetilde{c}(1)) =c(1) =p(x)$, tồn tại $g\in G$ sao cho $\widetilde{c}(1) =g\cdot x$. Chọn một đường đi $c_g:\mathbf{I}\rightarrow X$ nối $x$ với $g\cdot x$ và sao cho $p\circ c_g$ đồng luân nghiêm ngặt với một vòng hằng. Khi đó đường đi $c'=\widetilde{c}*\overline{c_g}$ là một vòng tại $x$ trong X sao cho $[p\circ c'] = [c]$. Điều này chứng minh rằng đồng cấu $\pi_1(X, x)\rightarrow \pi_1(X/G, p(x))$ là toàn ánh. Mệnh đề khác suy ra ngay lập tức.

Bây giờ chứng minh mệnh đề b). Không gian $X/G$ là liên thông cung địa phương (III, p. 261, Mệnh đề 8).

Cho $x$ là một điểm của X và cho $K_x$ là nhóm ổn định của nó trong G. Cho $U_1$ là một lân cận mở của $x$, được chứa trong U, sao cho ảnh của đồng cấu chính tắc $\pi_1(U_1, x)\rightarrow \pi_1(X, x)$ được thu gọn về phần tử đơn vị. Theo Bổ đề 1 (IV, p. 349), tồn tại một lân cận U của $x$ trong X, được chứa trong $U_1$, ổn định dưới $K_x$, sao cho $g\cdot U\cap U =\emptyset$ nếu $g\notin K_x$ và sao cho ánh xạ chính tắc $p$ cảm sinh một đồng phôi từ $U/K_x$ lên một lân cận V của $p(x)$ trong $X/G$.

Cho $c$ là một vòng tại $x$ trong V; theo Định lý 4 (III, p. 287), áp dụng cho không gian tôpô U và nhóm $K_x$, tồn tại một đường đi $\widetilde{c}:\mathbf{I}\rightarrow U$ sao cho $\widetilde{c}(0) =x$ và nâng $c$. Tất yếu $\widetilde{c}(1) =x$, do đó $\widetilde{c}$ là một vòng tại $x$ trong U. Theo giả thiết, $\widetilde{c}$ đồng luân nghiêm ngặt với một vòng hằng trong X; do đó, điều tương tự đúng với $c$, và đồng cấu chính tắc $\pi_1(V, p(x))\rightarrow \pi_1(X/G, p(x))$ là tầm thường. Điều này chứng minh rằng $X/G$ là không tạo vòng nếu X là không tạo vòng.

5) Trong mặt phẳng Euclid $\mathbf{R}^2$, cho P là không gian tôpô bằng hợp của các đường tròn có tâm $(1/n,0)$ đi qua gốc (với $n\in \mathbf{N}^*$). Không gian P là compact, liên thông và liên thông cung địa phương, nhưng không là không tạo vòng. Nhóm $\pi_1(P,0)$, được trang bị tôpô thích hợp, là phân ly và không rời rạc (III, p. 337, Bài tập 7).

#### Nhận xét 1 {#ta-iv-s1-n4-rem-1 .statement tag=020R}

Định lý 4 của III, p. 287 và Mệnh đề 8 (IV, p. 349) vẫn đúng dưới giả thiết tổng quát hơn rằng G là một nhóm Lie hữu hạn chiều trên $\mathbf{R}$ tác động đúng trong X. Để biết thêm chi tiết, xem D. Montgomery và C. T. Yang, « The existence of a slice », Annals of mathematics 65 (1957), p. 108–116 ; R. Palais, « On the existence of slices for actions of non-compact Lie groups », Annals of mathematics 73 (1961), p. 295–323 ; và G. Bredon, Introduction to compact transformation groups, Academic Press, 1972.

## BÀI TẬP {#ta-iv-s1-exercises}

Xem [các bài tập cho § 1](exercises/s1/).
