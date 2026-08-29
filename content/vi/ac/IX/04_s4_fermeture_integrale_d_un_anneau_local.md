---
book: ac
book_title: Commutative Algebra
chapter: IX
chapter_title: ANNEAUX LOCAUX NOETHÉRIENS COMPLETS
section: 4
section_title: Fermeture intégrale d'un anneau local complet
lang: vi
source: ac-viii-ix-fr
book_pages: AC IX.78-AC IX.84
pdf_pages: 0142-0148, 0190-0196
extraction: ocr
subsections:
    - "no": 1
      title: Anneaux japonais
      page: 30
      pdf_page: 142
    - "no": 2
      title: Théorème de Nagata
      page: 0
      pdf_page: 143
    - "no": 3
      title: Quelques lemmes
      page: 33
      pdf_page: 145
    - "no": 4
      title: Anneaux de Nagata
      page: 0
      pdf_page: 146
statements: 25
exercises: 32
content_sha256: 923a9d4c9119e4dce0be1ba954e46e8882a8325f0c6eb5cecd8015888b444a55
translated_from: content/en-mt/ac/IX/04_s4_fermeture_integrale_d_un_anneau_local.md
source_lang: en-mt
translation_method: machine
source_content_sha256: c99f00ea92b0543993afc373c2da1ed8fe1a64884eee789c95c982869175bfae
translation_model: gpt-5-6-mini, gpt-5-mini
translation_run: translate-vi-017b3d2e
glossary_version: 34
glossary_terms_sha256: e63d0c3b1aa6a93dc2865a2c7a350b013d280af31d79f580f97549e58628a0dc
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 4. ĐÓNG NGUYÊN CỦA MỘT VÀNH ĐỊA PHƯƠNG ĐẦY ĐỦ

### 1. Các vành Nhật Bản

#### Định nghĩa 1 {#ac-ix-s4-def-1 .statement}

Cho $A$ là một vành nguyên Noether. Ta nói rằng $A$ là Nhật Bản nếu đóng nguyên của $A$ trong mọi mở rộng hữu hạn của trường phân thức của nó là một đại số hữu hạn trên $A$.

#### Nhận xét 1 {#ac-ix-s4-n1-rem-1 .statement}

Điều này tương đương với việc nói rằng $A$ thỏa mãn điều kiện sau: mọi đại số nguyên $A$ $B$ nguyên trên $A$, được chứa trong một mở rộng sinh hữu hạn của trường phân thức $K$ của $A$, là một đại số hữu hạn trên $A$. Thật vậy, trường phân thức $L$ của $B$ là một mở rộng đại số của $K$, và do đó có bậc hữu hạn trên $K$ (A, V, p. 112, hệ quả 1 của mệnh đề 17). Đại số trên $A$ $B$ được chứa trong đóng nguyên của $A$ trong $L$, và do đó là hữu hạn nếu cái sau là hữu hạn.

#### Ví dụ {#ac-ix-s4-n1-exa-1 .statement}

Mọi đại số nguyên sinh hữu hạn trên một trường đều là một vành Nhật Bản (V, § 3, No. 2, định lý 2).

#### Mệnh đề 1 {#ac-ix-s4-prop-1 .statement}

Cho A là một vành nguyên Noether, K là trường phân thức của nó. Giả sử rằng với mọi mở rộng radicial hữu hạn L của K, đóng nguyên của A trong L là một đại số hữu hạn trên A. Khi đó vành A là Nhật Bản.

Cho E là một mở rộng hữu hạn của K. Cho N là một mở rộng gần-Galois hữu hạn của K chứa E (A, V, p. 54, hệ quả 1), và L là trường các bất biến của nhóm các tự đẳng cấu K của N. Khi đó (A, V, p. 73, mệnh đề 13), L là một mở rộng radicial của K và N là một mở rộng tách được của L. Đóng nguyên B của A trong L do đó theo giả thiết là một đại số hữu hạn trên A; đóng nguyên C của B trong N là một đại số hữu hạn trên B (V, § 1, No. 6, hệ quả 1 của mệnh đề 18), do đó là một đại số hữu hạn trên A. Đóng nguyên của A trong E được chứa trong C, và do đó là một đại số hữu hạn trên A vì A là Noether.

#### Hệ quả {#ac-ix-s4-n1-cor-1 .statement}

Giả sử trường K hoàn hảo (chẳng hạn có đặc số 0). Khi đó A là Nhật Bản khi và chỉ khi đóng nguyên của nó là một đại số hữu hạn trên A.

#### Mệnh đề 2 {#ac-ix-s4-prop-2 .statement}

Cho B là một vành nguyên Noether và A là một vành con Noether của B, sao cho B là một đại số hữu hạn trên A. Để A là Nhật Bản, điều kiện cần và đủ là B là Nhật Bản.

Gọi K (tương ứng L) là trường phân thức của A (tương ứng B). Trước hết giả sử rằng A là Nhật Bản, và cho M là một mở rộng hữu hạn của L. Gọi C là đóng nguyên của B trong M. Theo V, § 1, No. 1, mệnh đề 6, C là đóng nguyên của A trong M, và do đó là một đại số hữu hạn trên A vì M là một mở rộng hữu hạn của K và A là Nhật Bản. A fortiori, C là một đại số hữu hạn trên B. Điều này chứng minh rằng B là Nhật Bản.

Ngược lại, giả sử B là Nhật Bản và cho N là một mở rộng hữu hạn của K. Gọi D là đóng nguyên của A trong N. Cho E là một mở rộng của K hợp thành bởi L và N; vì B là Nhật Bản, đóng nguyên D’ của B trong E là một đại số hữu hạn trên B, do đó là một đại số hữu hạn trên A; A-môđun D, là một môđun con của D’, do đó là sinh hữu hạn, do đó suy ra rằng A là Nhật Bản.

### 2. Định lý Nagata

#### Định lý 1 (Tate) {#ac-ix-s4-thm-1 .statement}

Cho A là một vành Noether đóng nguyên, a là một phần tử của A. Giả sử rằng iđêan $aA$ là nguyên tố, rằng vành $A/aA$ là Nhật Bản, và rằng A là đầy đủ đối với tôpô $aA$-adic. Khi đó vành A là Nhật Bản.

a) Gọi trường phân thức của A là K, vì mệnh đề là tầm thường khi K có đặc số 0 (No. 1, hệ quả của mệnh đề 1), ta có thể giả sử K có đặc số $p > 0$. Ta cũng có thể giả sử $a \neq 0$.

Cho L là một mở rộng radicial hữu hạn của K và q là một lũy thừa của p sao cho $L \subset K^{1/q}$. Đặt $x = a^{1/q}$ và $M = L(x)$. Theo mệnh đề 1 của No. 1, chỉ cần chứng minh rằng đóng nguyên B của A trong M là một đại số hữu hạn trên A.

b) Trước hết hãy chứng minh rằng iđêan $xB$ là iđêan nguyên tố duy nhất của B nằm trên $aA$. Thật vậy tồn tại ít nhất một iđêan nguyên tố của B nằm trên $aA$ (V, § 2, No. 1, định lý 1). Cho q là một trong các iđêan này. Ta có $x^q = a \in q$, do đó $xB \subset q$ vì q là nguyên tố. Ngược lại, cho y là một phần tử của q; phần tử $y^q$ của K là nguyên trên A, và do đó thuộc A vì A đóng nguyên. Vì $q \cap A = aA$, tồn tại một phần tử $\alpha$ của A sao cho $y^q = a\alpha = x^q\alpha$. Do đó phần tử $y/x$ của M là nguyên trên A, và do đó thuộc B; vậy ta có $y \in xB$, do đó $q = xB$, điều này chứng minh mệnh đề của chúng ta.

c) Suy ra rằng vành $B_{xB}$ là đóng nguyên trong M của vành $A_{aA}$ (V, § 1, No. 5, mệnh đề 16 và § 2, No. 1, mệnh đề 2). Theo VI, § 3, No. 6, mệnh đề 9, $A_{aA}$ là một vành định giá rời rạc; khi đó suy ra từ định lý Krull-Akizuki (VII, § 2, No. 5, mệnh đề 5) rằng trường $\kappa(xB)$ là một mở rộng hữu hạn của $\kappa(aA)$ và rằng $B_{xB}$ là Noether.

d) Vành $B/xB$ là nguyên trên vành Nhật Bản $A/aA$ và trường phân thức của nó là một mở rộng hữu hạn của trường phân thức của vành sau. Do đó, $B/xB$ là một $(A/aA)$-môđun sinh hữu hạn. Với mọi số nguyên $i \geq 0$, điều tương tự cũng đúng đối với môđun $x^iB/x^{i+1}B$; suy ra rằng $(A/aA)$-môđun $B/aB$ có một chuỗi hợp thành độ dài q mà các thương của nó là các $(A/aA)$-môđun sinh hữu hạn, và do đó bản thân nó là một $(A/aA)$-môđun sinh hữu hạn.

e) Ta trang bị cho vành A với lọc $(aA)$-adic và vành B với lọc $(aB)$-adic. Khi đó A là đầy đủ theo giả thiết; vì $B_{xB}$ là một miền nguyên và Noether, lọc $aB_{xB}$-adic của $B_{xB}$ là tách được (III, § 3, No. 2, hệ quả của mệnh đề 5); do đó ta có $\bigcap a^nB \subset \bigcap a^nB_{xB} = {0}$, và lọc $aB$-adic của B là tách được; môđun gr(A)-môđun gr(B) được sinh bởi gr_0(B), do đó là sinh hữu hạn theo d). Từ III, § 2, No. 9, hệ quả 1 của mệnh đề 12, suy ra rằng B là một A-môđun sinh hữu hạn, điều này hoàn tất chứng minh.

#### Hệ quả {#ac-ix-s4-n2-cor-1 .statement}

Cho R là một miền nguyên Noether và n là một số nguyên. Nếu R là Japanese, vành $R[[T_1, ..., T_n]]$ là Japanese.

Lập luận bằng quy nạp, ta có thể giả sử rằng $n = 1$. Gọi S là bao đóng nguyên của R; nếu R là Japanese, S là một đại số hữu hạn trên R, do đó là một vành Japanese (No. 1, mệnh đề 2). Vành S[[T]] là Noether và đóng nguyên (V, § 1, No. 4, mệnh đề 14); áp dụng Định lý 1 cho $A = S[[T]]$ và $a = T$, ta suy ra S[[T]] là Japanese. Do đó R[[T]] là Japanese (No. 1, mệnh đề 2).

#### Định lý 2 (Nagata) {#ac-ix-s4-thm-2 .statement}

Mọi miền nguyên Noether địa phương đầy đủ A đều là Japanese.

Theo Định lý 3 của § 2, No. 5 và Định lý 2 của § 3, No. 3, tồn tại một số nguyên $n \geq 0$, một vành R là một trường hoặc một vành định giá rời rạc với trường phân thức có đặc số 0, và một vành con B của A, đẳng cấu với R[[T₁, ..., Tₙ]] và sao cho A là một đại số hữu hạn trên B. Khi đó R là Japanese (No. 1, ví dụ và hệ quả của mệnh đề 1), do đó B là Japanese (hệ quả của Định lý 1), và A là Japanese (No. 1, mệnh đề 2).

#### Hệ quả {#ac-ix-s4-n2-cor-2 .statement}

Cho A là một vành Noether nửa địa phương có hoàn thành là giảm. Khi đó bao đóng nguyên A' của A trong vành phân thức toàn phần R của nó là một A-đại số hữu hạn.

Trước hết giả sử rằng A là địa phương và đầy đủ, và gọi p₁, ..., pₙ là các iđêan nguyên tố cực tiểu (phân biệt) của A; với i = 1, ..., n, gọi Kᵢ là trường phân thức của A/pᵢ và Aᵢ' là bao đóng nguyên của A/pᵢ. Vì A là giảm, R là tích của các vành Kᵢ và A' là tích của các vành Aᵢ' (V, § 1, No. 2, hệ quả 1 của mệnh đề 9). Vì các vành địa phương A/pᵢ là các miền nguyên và đầy đủ, chúng là Japanese (Định lý 2), do đó mỗi Aᵢ' là một A-đại số hữu hạn, và A' là một A-đại số hữu hạn.

Nếu A là nửa địa phương và đầy đủ, nó đẳng cấu với một tích hữu hạn của các vành địa phương đầy đủ (III, § 2, No. 13, hệ quả của mệnh đề 19), và ta kết luận ngay từ điều trước.

Ta chuyển sang trường hợp tổng quát, và nhận xét rằng hoàn thành Â của A là một vành Noether nửa địa phương, đầy đủ, phẳng trung thành trên A (III, loc. cit., § 3, No. 4, hệ quả của mệnh đề 8 và § 3, No. 5, mệnh đề 9). Gọi S là tập hợp các phần tử không là ước của không của A; ta có R = S⁻¹A. Vì Â phẳng trên A, các phần tử của S là các phần tử không là ước của không trong Â, và S⁻¹Â được đồng nhất với một vành con của vành phân thức toàn phần T của Â. Lại vì Â phẳng trên A, vành A' ⊗_A Â được đồng nhất với một vành con của R ⊗_A Â = S⁻¹Â, do đó cũng với một vành con của T nguyên trên Â. Theo phần đầu của chứng minh, A' ⊗_A Â vì thế là một Â-môđun sinh hữu hạn; do đó A' là một A-môđun sinh hữu hạn (I, § 3, No. 6, mệnh đề 11).

Nhắc lại (A, V, p. 114, định nghĩa 1) rằng một đại số E trên một trường K được gọi là tách được nếu vành L ⊗_K E là giảm với mọi mở rộng L của K; chỉ cần điều này đúng với mọi mở rộng hữu hạn của K. Mệnh đề sau đây mở rộng Định lý 2:

#### Mệnh đề 3 {#ac-ix-s4-prop-3 .statement}

Cho A là một miền nguyên Noether nửa địa phương, K là trường phân thức của nó. Nếu K-đại số K ⊗_A Â là tách được, vành A là Japanese.

Cho L là một mở rộng hữu hạn của K và B là bao đóng nguyên của A trong L. Cho F là một tập con hữu hạn của B sao cho L = K[F] (V, § 1, No. 5, hệ quả 2 của mệnh đề 16); gọi C là A-đại số (hữu hạn) được sinh bởi F. Vì L là trường phân thức của C, vành B là bao đóng nguyên của C (V, § 1, No. 1, mệnh đề 6) và chỉ cần chứng minh rằng B là một C-đại số hữu hạn. Bây giờ, C là một vành Noether nửa địa phương (IV, § 2, No. 5, hệ quả 3 của mệnh đề 9); hoàn thành của nó được đồng nhất với C ⊗_A Â (III, § 3, No. 4, định lý 3 (ii)), do đó cũng với một vành con của vành giảm L ⊗_A Â = L ⊗_K (K ⊗_A Â) và vì thế là giảm. Mệnh đề 3 do đó suy ra từ hệ quả của Định lý 2.

### 3. Một số bổ đề

#### Bổ đề 1 {#ac-ix-s4-lem-1 .statement}

Cho A là một vành Noether nửa địa phương và B là một A-đại số hữu hạn. Khi đó vành B là nửa địa phương và Noether; gọi m₁, ..., mₙ là các iđêan cực đại của nó.

Đồng cấu chính tắc của B vào $\prod_{i=1}^n \hat{B}_{m_i}$ mở rộng thành một đẳng cấu từ $\hat{A} \otimes_A B$ lên $\prod_{i=1}^n \hat{B}_{m_i}$.

Theo IV, § 2, No. 5, hệ quả 3 của mệnh đề 9, vành B là nửa địa phương và $m_A B$ là một iđêan định nghĩa của nó. Theo III, § 3, No. 4, định lý 3, (ii), vành $\hat{A} \otimes_A B$ là hoàn thành của B đối với tôpô được xác định bởi căn của nó; khi đó áp dụng III, § 2, No. 13, hệ quả của mệnh đề 19.

#### Bổ đề 2 {#ac-ix-s4-lem-2 .statement}

Cho A là một vành Noether và M là một A-môđun. Ánh xạ chính tắc của M vào tích $\prod_{p \in \mathrm{Ass}(M)} M_p$ là đơn ánh.

Thật vậy, cho m là một phần tử khác không của M; khi đó Ann(m) được chứa trong một iđêan nguyên tố p của A liên kết với M (IV, § 1, No. 1, mệnh đề 2), và ảnh của m trong $M_p$ là khác không (II, § 2, No. 2, mệnh đề 4).

#### Bổ đề 3 {#ac-ix-s4-lem-3 .statement}

Cho $A$ là một vành Noether, $x$ là một phần tử của $A$, $M$ là một A-môđun sinh hữu hạn, và $p$ là một iđêan nguyên tố của $A$ liên kết với $M$. Giả sử rằng phép vị tự $x_M$ là đơn ánh. Gọi $q$ là một iđêan nguyên tố của $A$, cực tiểu trong số các iđêan chứa $p + xA$. Khi đó $q$ liên kết với A-môđun $M/xM$.

Cho $N$ là môđun con của $M$ tạo bởi các phần tử $m$ sao cho $pm = 0$. Ta có $N \cap xM = xN$; thật vậy, nếu một phần tử $m$ của $M$ sao cho $pxm = 0$, thì $pm = 0$ vì $x_M$ là đơn ánh, do đó $m \in N$. Do đó, $A$-môđun $N/xN$ là đẳng cấu với môđun con $(N + xM)/xM$ của $M/xM$, và chỉ cần chứng minh rằng $q$ liên kết với $N/xN$. Vì $p$ liên kết với $M$, tồn tại một phần tử $m$ của $M$ sao cho $p = \mathrm{Ann}(m)$; ta có $m \in N$, do đó $p = \mathrm{Ann}(N)$ và vì vậy $\mathrm{Supp}(N/xN) = V(p + xA)$ theo II, § 4, No. 4, hệ quả của mệnh đề 18; do đó, $q$ liên kết với $N/xN$ (IV, § 1, No. 4, định lý 2).

#### Bổ đề 4 {#ac-ix-s4-lem-4 .statement}

Cho $A$ là một vành định giá rời rạc, $B$ là một vành địa phương Noether, và $\rho : A \to B$ là một đồng cấu địa phương và phẳng. Nếu vành $\kappa_A \otimes_A B$ là giảm, thì $B$ là giảm.

Giả sử tồn tại một phần tử lũy linh khác không $x$ của $B$, và gọi $\pi$ là một phần tử chuẩn hóa của $A$. Vì $\pi B \subset m_B$, vành $B$ là tách được đối với tôpô $\pi B$-adic. Do đó tồn tại $n \in \mathbf{N}$ và $y \in B$ sao cho $x = \pi^n y$ và $y \notin \pi B$. Vì $B$ là phẳng trên $A$, phép nhân bởi $\pi$ là đơn ánh trong $B$. Lớp của $y$ trong $B/\pi B$ do đó là một phần tử lũy linh khác không, điều này mâu thuẫn với giả thiết.

### 4. Vành Nagata

#### Định nghĩa 2 {#ac-ix-s4-def-2 .statement}

Một vành $A$ được gọi là một vành Nagata nếu nó là Noether và nếu, với mọi iđêan nguyên tố $p$ của $A$, vành nguyên Noether $A/p$ là Japanese (No. 1, định nghĩa 1).

#### Ví dụ 1 {#ac-ix-s4-n4-exa-1 .statement}

Mọi đại số sinh hữu hạn trên một trường đều là một vành Nagata (No. 1, ví dụ).

#### Ví dụ 2 {#ac-ix-s4-n4-exa-2 .statement}

Mọi vành địa phương Noether đầy đủ đều là một vành Nagata (No. 2, định lý 2).

#### Ví dụ 3 {#ac-ix-s4-n4-exa-3 .statement}

Vành $\mathbf{Z}$ là một vành Nagata (No. 1, ví dụ và hệ quả của mệnh đề 1).

#### Ví dụ 4 {#ac-ix-s4-n4-exa-4 .statement}

Có thể chứng minh (bài tập 30) rằng mọi đại số sinh hữu hạn trên một vành Nagata đều là một vành Nagata.

#### Mệnh đề 4 {#ac-ix-s4-prop-4 .statement}

Cho $A$ là một vành Nagata.
a) Mọi đại số $A$ hữu hạn đều là một vành Nagata.
b) Với mọi tập con nhân $S$ của $A$, vành $S^{-1}A$ là một vành Nagata.
a) Cho $B$ là một đại số $A$ hữu hạn, $\rho : A \to B$ là đồng cấu chính tắc. Với mọi iđêan nguyên tố $p$ của $B$, vành $B/p$, là một đại số hữu hạn trên vành Nhật $A/\rho^{-1}(p)$, là Nhật (No. 1, mệnh đề 2).
b) Cho $q$ là một iđêan nguyên tố của $S^{-1}A$; khi đó tồn tại một iđêan nguyên tố $p$ của $A$ sao cho $q = S^{-1}p$. Vành $(S^{-1}A)/q$ là một vành phân thức của vành Nhật $A/p$, và do đó là Nhật (No. 1, nhận xét 2).

#### Định lý 3 (Zariski-Nagata) {#ac-ix-s4-thm-3 .statement}

Cho $A$ là một vành Noether nửa địa phương. Các điều kiện sau là tương đương:
(i) $A$ là một vành Nagata;
(ii) với mọi iđêan nguyên tố $p$ của $A$, đại số $\kappa(p)$-$\kappa(p) \otimes_A \hat{A}$ là tách được;
(iii) với mọi đại số $A$-rút gọn $R$, vành $R \otimes_A \hat{A}$ là rút gọn.
Trước hết ta chứng minh sự tương đương của các điều kiện (ii) và (iii). Sự kéo theo (iii) $\Rightarrow$ (ii) là tầm thường; ngược lại, giả sử rằng $A$ thỏa mãn điều kiện (ii). Khi đó, với mọi đại số $A$- $K$ là một trường, vành $K \otimes_A \hat{A}$ là rút gọn. Bây giờ cho $C$ là một đại số $A$-rút gọn hữu hạn kiểu; vành $C$, vì là Noether, đẳng cấu với một vành con của một tích hữu hạn $K_1 \times \cdots \times K_n$ của các trường (IV, § 2, No. 5, Mệnh đề 10); vì $\hat{A}$ là phẳng trên $A$, vành $C \otimes_A \hat{A}$ đẳng cấu với một vành con của vành rút gọn $\prod_i (K_i \otimes_A \hat{A})$, do đó là rút gọn. Cuối cùng, cho $R$ là một đại số $A$-rút gọn bất kỳ; khi đó $R$ là hợp của họ lọc $(C_\alpha)$ gồm các đại số con hữu hạn kiểu của nó, và $R \otimes_A \hat{A}$ là giới hạn trực tiếp của họ lọc $(C_\alpha \otimes_A \hat{A})$ gồm các vành rút gọn, do đó là rút gọn.
Ta chứng minh rằng (ii) kéo theo (i). Cho $p$ là một iđêan nguyên tố của $A$; trường phân thức $K$ của vành $A/p$ được đồng nhất với $\kappa(p)$, và đại số $K$- $K \otimes_{A/p} (\widehat{A/p})$ được đồng nhất với $\kappa(p) \otimes_{A/p} \hat{A}/p\hat{A}$, do đó với $\kappa(p) \otimes_A \hat{A}$. Nếu $\kappa(p) \otimes_A \hat{A}$ là một đại số $\kappa(p)$-tách được, vành $A/p$ là Nhật Bản (No. 2, Mệnh đề 3).
Ta chứng minh sự kéo theo (i) $\Rightarrow$ (ii) bằng quy nạp theo $\dim(A)$. Điều này là hiển nhiên nếu $\dim(A) = 0$ vì khi đó $A$ là Artin, do đó đầy đủ. Cho $n$ là một số nguyên $> 0$; xét giả thiết sau:

(R$_n$) $\left\{ \begin{array}{l}
\text{với mọi vành Nagata Noether địa phương } C \text{ có chiều } < n \text{ và mọi iđêan nguyên tố } r \text{ của } C, \text{ vành } \kappa(r) \otimes_C \hat{C} \text{ là rút gọn.}
\end{array} \right.$

Cho $A$ là một vành Nagata Noether nửa địa phương có chiều $n$, cho $p$ là một iđêan nguyên tố của $A$ và $L$ là một mở rộng hữu hạn của trường $\kappa(p)$; chỉ cần chứng minh,

#### Hệ quả 1 {#ac-ix-s4-thm-3-cor-1 .statement}

*Hoàn thành của một vành Nagata địa phương rút gọn là rút gọn.*
Thực vậy, chỉ cần đặt R = A trong Định lý 3, (iii).

#### Hệ quả 2 (Chevalley) {#ac-ix-s4-thm-3-cor-2 .statement}

*Cho A là một đại số rút gọn hữu hạn kiểu trên một trường, và p là một iđêan nguyên tố của A. Hoàn thành của vành địa phương $A_p$ là rút gọn.*
Vì A là rút gọn, vành địa phương $A_p$ là rút gọn; hơn nữa A là một vành Nagata (ví dụ 1), do đó $A_p$ là một vành Nagata (Mệnh đề 4), và Hệ quả 2 suy ra từ Hệ quả 1, áp dụng cho vành $A_p$.

#### Hệ quả 3 {#ac-ix-s4-thm-3-cor-3 .statement}

*Cho $k$ là một trường có đặc số 0, và $A$ là một $k$-đại số địa phương Noether. Để $A$ là một vành Nagata, điều kiện cần và đủ là, với mọi iđêan nguyên tố $p$ của $A$, vành $(\widehat{A/p})$ là giảm.*
Thật vậy, vì các trường $\kappa(p)$ có đặc số 0, điều này tương đương với việc nói rằng các đại số $\kappa(p) \otimes_A \hat{A} = \kappa(p) \otimes_{A/p} (\widehat{A/p})$ là giảm hoặc chúng là tách được (A, V, p. 117, Định lý 1), điều này cho thấy điều kiện đã nêu là đủ (Định lý 3, (ii) ⇒ (i)); hơn nữa nó là cần thiết (Định lý 3, (i) ⇒ (iii) với R = A/p).

## BÀI TẬP {#ac-ix-s4-exercises}

Xem [các bài tập cho § 4](exercises/s4/).
