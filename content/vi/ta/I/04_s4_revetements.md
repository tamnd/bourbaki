---
book: ta
book_title: Topologie algébrique
chapter: I
chapter_title: REVÊTEMENTS
section: 4
section_title: Revêtements
lang: vi
source: ta-i-iv-fr
book_pages: TA I.68-TA I.90, TA I.145-TA I.147
pdf_pages: 0084-0106, 0161-0163
extraction: native
subsections:
    - "no": 1
      title: Espaces fibrés localement triviaux
      page: 68
      pdf_page: 84
    - "no": 2
      title: Revêtements
      page: 69
      pdf_page: 85
    - "no": 3
      title: Produits et produits fibrés
      page: 71
      pdf_page: 87
    - "no": 4
      title: Degré d’un revêtement
      page: 73
      pdf_page: 89
    - "no": 5
      title: Revêtements finis
      page: 75
      pdf_page: 91
    - "no": 6
      title: Revêtements des espaces localement connexes
      page: 79
      pdf_page: 95
    - "no": 7
      title: Revêtements d’un espace paracompact
      page: 84
      pdf_page: 100
    - "no": 8
      title: Faisceaux localement constants
      page: 86
      pdf_page: 102
    - "no": 9
      title: Produits de faisceaux localement constants
      page: 87
      pdf_page: 103
    - "no": 10
      title: Morphismes de faisceaux localement constants sur un espace localement connexe
      page: 89
      pdf_page: 105
statements: 50
exercises: 9
content_sha256: 5497bd8b97667b103e1cd4c6c81910bab606a87bba03884b7347fb2b9c188209
translated_from: content/en-mt/ta/I/04_s4_revetements.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 28a8ab4dfdce641c77cb1c35e6e3d45d59595535573c27956687c039fb452550
translation_model: gpt-5-6, gpt-5-mini
translation_run: translate-vi-1a210324
glossary_version: 34
glossary_terms_sha256: bbeecd5787f7cc872f91ee42e43d9cffbb88096d4a70c9c3c9b3ae06f9f6597d
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 4. KHÔNG GIAN PHỦ

### 1. Không gian sợi địa phương tầm thường

Cho B là một không gian tôpô. Nếu F là một không gian tôpô, B-không gian $(B\times F$, pr$_1)$ được gọi là một B-không gian sợi tầm thường kiểu sợi F.

Cho E là một B-không gian. Nếu tồn tại một không gian tôpô F và một B-đẳng cấu $u: E\rightarrow B\times F$, ta nói rằng B-không gian E là một B-không gian sợi có thể tầm thường hóa và $u$ là một phép tầm thường hóa của nó kiểu sợi F.

#### Định nghĩa 1 {#ta-i-s4-def-1 .statement tag=01OR}

Cho B là một không gian tôpô. Cho E là một B-không gian và $p$ là phép chiếu của nó. Ta nói rằng E là một B-không gian sợi địa phương tầm thường nếu mọi điểm của B đều có một lân cận V sao cho $(\overset{-1}{p}(V), p_V)$ là một V-không gian sợi có thể tầm thường hóa.

Thay vì nói "B-không gian sợi địa phương tầm thường", ta cũng nói "không gian sợi địa phương tầm thường với cơ sở B". Nếu E là một B-không gian sợi địa phương tầm thường, đôi khi ta nói rằng $(E,B, p)$ là một phân thớ địa phương tầm thường, hoặc, theo lối nói không chính xác, rằng $p$ là một phân thớ địa phương tầm thường. Ta cũng nói rằng một B-không gian $(E, p)$ có thể tầm thường hóa trên một tập con A của B nếu A-không gian $E_A$ cảm sinh bởi $(E, p)$ trên A là một không gian sợi có thể tầm thường hóa.

Cho E là một B-không gian sợi địa phương tầm thường; ký hiệu $p$ là phép chiếu của nó.

Tập hợp các điểm $a$ của B sao cho sợi $\overset{-1}{p}(a)$ là rỗng (resp. khác rỗng) là mở. Do đó, ảnh của p là một tập con vừa mở vừa đóng của B.

Cho F là một không gian tôpô. Nếu mọi sợi của E đều đồng phôi với F, ta nói rằng E là một B-không gian sợi địa phương tầm thường kiểu sợi F.

#### Nhận xét 1 {#ta-i-s4-n1-rem-1 .statement tag=01OS}

Cho $(E, p)$ là một B-không gian sợi địa phương tầm thường và A là một tập con của B. A-không gian $E_A= (\overset{-1}{p}(A), p_A)$ suy ra từ E bằng cách chuyển qua các không gian con là một không gian sợi địa phương tầm thường. Nếu E có thể tầm thường hóa, điều tương tự cũng đúng với $E_A$.

Thật vậy, với mọi điểm $a$ của A, tồn tại một lân cận mở U của $a$ trong B, một không gian tôpô F và một U-đẳng cấu $g:\overset{-1}{p}(U)\rightarrow$ $U\times F$. Ánh xạ f cảm sinh một $(A\cap U)$-đẳng cấu của $p^{-1}_A(A\cap U)$ lên $(A\cap U)\times F$, điều này chứng minh rằng $E_A$ là một A-không gian sợi địa phương tầm thường.

#### Nhận xét 2 {#ta-i-s4-n1-rem-2 .statement tag=01OT}

Cho $(E, p)$ là một B-không gian và $(E_i)_{i\in I}$ là một phân hoạch của E gồm các tập mở.

Nếu mỗi B-không gian $(E_i, p|E_i)$ là một không gian sợi có thể tầm thường hóa, thì E là một B-không gian sợi có thể tầm thường hóa. Thật vậy, với mỗi $i\in I$, cho $F_i$ là một không gian tôpô sao cho các B-không gian $(E_i, p|E_i)$ và $(B\times F_i$, pr$_1)$ là đẳng cấu. Khi đó B-không gian $(E, p)$ đẳng cấu với $(B\times F$, pr$_1)$, trong đó F là không gian tôpô tổng của họ $(F_i)_{i\in I}$.

Giả sử tập hợp I hữu hạn. Nếu mỗi B-không gian $(E_i, p|E_i)$ là một B-không gian sợi địa phương tầm thường, điều tương tự cũng đúng với B-không gian E. Thật vậy, vì tập hợp I hữu hạn, mọi điểm của B đều có một lân cận U phía trên đó các B-không gian sợi $E_i$ đều có thể tầm thường hóa. Theo điều vừa nêu, U-không gian $(\overset{-1}{p}(U), p_U)$ khi đó là một không gian sợi có thể tầm thường hóa.

### 2. Không gian phủ

#### Định nghĩa 2 {#ta-i-s4-def-2 .statement tag=01OU}

Một không gian phủ là một không gian sợi địa phương tầm thường mà mọi sợi của nó đều rời rạc.

Thay vì nói rằng B-không gian E là một không gian phủ, ta cũng nói rằng E là một không gian phủ của B.

Cho E là một B-không gian, và ký hiệu $p$ là phép chiếu của nó; cho A là một tập con của B. Nếu E là một không gian phủ của B, các sợi của p rời rạc, do đó các sợi của $p_A:\overset{-1}{p}(A)\rightarrow A$ cũng rời rạc, và A-không gian sợi địa phương tầm thường $(\overset{-1}{p}(A), p_A)$ là một không gian phủ.

#### Mệnh đề 1 {#ta-i-s4-prop-1 .statement tag=01OV}

Cho B và E là các không gian tôpô và cho $p: E\rightarrow B$ là một ánh xạ. Các điều kiện sau là tương đương:

(i) Ánh xạ $p$ liên tục và B-không gian $(E, p)$ là một không gian phủ có thể tầm thường hóa;

(ii) Tồn tại một phân hoạch $(V_i)_{i\in I}$ của E gồm các tập mở sao cho, với mọi $i\in I$, ánh xạ $p|V_i: V_i\rightarrow B$ là một đồng phôi.

Giả sử điều kiện (i) được thỏa mãn, và cho $g: E\rightarrow B\times F$ là một phép tầm thường hóa của B-không gian $(E, p)$, kiểu sợi F. Khi đó F là một không gian tôpô rời rạc và các tập $V_i=\overset{-1}{g}(B\times  \{i\})$, với $i\in F$, tạo thành một phân hoạch của E gồm các tập mở. Với mọi $i$, ánh xạ $p|V_i: V_i\rightarrow B$ là một đồng phôi, với đồng phôi ngược là ánh xạ $x\mapsto g^{-1}(x, i)$, do đó điều kiện (ii).

Ngược lại, giả sử điều kiện (ii) được thỏa mãn. Ánh xạ $p$ khi đó là liên tục. Xét ánh xạ từ E vào $B\times I$ gán cho $x\in E$ cặp $(p(x), i)$, trong đó $i$ là phần tử duy nhất của I sao cho $x\in V_i$. Nếu I được trang bị tôpô rời rạc, điều kiện (ii) có nghĩa là ánh xạ này là một đẳng cấu B và không gian B $(E, p)$ là một phủ tầm thường hóa.

#### Hệ quả 1 {#ta-i-s4-prop-1-cor-1 .statement tag=01OW}

Cho B và E là các không gian tôpô và cho $p: E\rightarrow B$ là một ánh xạ. Để E, được trang bị ánh xạ $p$, là một phủ của B, điều kiện cần và đủ là, với mọi điểm $a$ của B, tồn tại một lân cận mở U của $a$ và một phân hoạch $(V_i)_{i\in I}$ của $\overset{-1}{p}(U)$ gồm các tập hợp mở của E sao cho, với mọi $i\in I$, ánh xạ $p$ cảm sinh một phép đồng phôi của $V_i$ lên U.

#### Nhận xét {#ta-i-s4-n2-rem-1 .statement tag=01OX}

Cho B là một không gian tôpô. Cho E là một không gian B và cho $p$ là phép chiếu của nó. Nếu E là một phủ của B, từ hệ quả 1 ở trên suy ra rằng ánh xạ $p$ là étale (I, p. 28, Định. 2) và tách (I, p. 25, Mệnh đề 1, (iii)). Tuy nhiên, các điều kiện này không đủ để bảo đảm rằng E là một phủ. Xét, chẳng hạn, một tập hợp mở U của B. Đơn ánh chính tắc $i: U\rightarrow B$ là étale và tách. Để không gian B $(U, i)$ là một phủ, điều kiện cần và đủ là tập hợp mở U cũng đóng.

#### Hệ quả 2 {#ta-i-s4-prop-1-cor-2 .statement tag=01OY}

Cho B là một không gian tôpô, cho E là một không gian B và cho $p$ là phép chiếu của nó. Giả sử rằng $p$ là étale và tách và rằng không gian B là liên thông. Để E là một phủ tầm thường hóa của B, điều kiện cần và đủ là, với mọi điểm $x$ của E, tồn tại một tiết diện liên tục $s: B\rightarrow E$ của $p$ sao cho $s\circ p(x) =x$.

Điều này hiển nhiên là cần thiết. Ngược lại, với mọi tiết diện liên tục $s$ của $p$, tập hợp $s(B)$ là mở và ánh xạ $p$ cảm sinh một phép đồng phôi của $s(B)$ lên B (I, p. 30, Hệ quả 3 của Mệnh đề 6). Hơn nữa, khi $s$ chạy qua tập hợp $\mathscr{S}(B; E)$ các tiết diện của $p$, các tập hợp $s(B)$ rời nhau từng đôi một, vì B là liên thông (I, p. 34, Hệ quả 1 của Mệnh đề 11). Khi đó từ mệnh đề 1 suy ra rằng nếu các tập hợp $s(B)$ phủ E, không gian E là một phủ tầm thường hóa của B.

### 3. Các tích và các tích có thớ

#### Mệnh đề 2 {#ta-i-s4-prop-2 .statement tag=01OZ}

Cho B và $B'$ là các không gian tôpô, cho $(E, p)$ là một không gian B và cho $(E', p')$ là một không gian $B'$. Giả sử rằng E và $E'$ là các không gian thớ địa phương tầm thường ( resp. các phủ). Không gian $E\times E'$, được trang bị ánh xạ $p\times p': E\times E'\rightarrow B\times B'$, khi đó là một không gian thớ địa phương tầm thường ( resp. một phủ) với cơ sở $B\times B'$. Nếu E và $E'$ là tầm thường hóa, thì $E\times E'$ cũng vậy.

Trước hết giả sử rằng không gian B E và không gian $B'$ $E'$ thừa nhận các phép tầm thường hóa $g: E\rightarrow B\times F,g': E'\rightarrow B'\times F'$; hợp thành của phép đồng phôi $g\times g'$ của $E\times E'$ lên $(B\times F)\times (B'\times F')$ và của phép đồng phôi chính tắc của $(B\times F)\times (B'\times F')$ lên $(B\times B')\times (F\times F')$ là một phép tầm thường hóa của không gian $B\times B'$ $E\times E'$, có kiểu thớ $F\times F'$. Nếu F và $F'$ là các không gian rời rạc, không gian $F\times F'$ cũng là rời rạc.

Trong trường hợp tổng quát, với mọi điểm $(a, a')$ của $B\times B'$, tồn tại một lân cận U của $a$ trong B và một lân cận $U'$ của $a'$ trong $B'$ sao cho không gian U $E_U$ và không gian $U'$ $E'_{U'}$ có thể tầm thường hóa. Theo những điều trên, không gian $B\times B'$ $E\times E'$ có thể tầm thường hóa trên $U\times U'$. Do đó nó là một không gian sợi địa phương tầm thường với cơ sở $B\times B'$. Các sợi của nó rời rạc nếu E và $E'$ là các phủ, do đó có mệnh đề.

Cần nhận thấy rằng, nếu $(p_i: E_i\rightarrow B_i)_{i\in I}$ là một họ các không gian sợi địa phương tầm thường, hoặc thậm chí các phủ, thì không gian tích $\prod_{i\in I}E_i$ được trang bị ánh xạ $(p_i)_{i\in I}$ không nhất thiết là một không gian sợi địa phương tầm thường với cơ sở $\prod_{i\in I}B_i($I, p. 145, Bài tập 3).

#### Hệ quả 1 {#ta-i-s4-prop-2-cor-1 .statement tag=01P0}

Cho A là một không gian tôpô, B, $B'$ là các A-không gian. Cho E và $E'$ là các không gian sợi địa phương tầm thường ( resp. các phủ) với các cơ sở B và $B'$; gọi p và $p'$ là các phép chiếu của chúng. Không gian $B\times_AB'$ $E\times_AE'$ thu được từ $p\times p'$ bằng cách chuyển qua các không gian con khi đó là một không gian sợi địa phương tầm thường ( resp. một phủ). Nó có thể tầm thường hóa nếu E và $E'$ có thể tầm thường hóa.

Vì tập hợp $E\times_AE'$ là ảnh ngược của $B\times_AB'$ qua ánh xạ $p\times p': E\times E'\rightarrow B\times B'$, hệ quả suy ra từ mệnh đề 2 và nhận xét 1 (I, p. 68).

#### Hệ quả 2 {#ta-i-s4-prop-2-cor-2 .statement tag=01P1}

Cho

${E'}^{f'}$ E

$p'p$

${B'}^f$ B

là một bình phương Descartes. Nếu $(E, p)$ là một không gian sợi B địa phương tầm thường ( resp. một phủ), thì $(E', p')$ là một không gian sợi địa phương tầm thường ( resp. một phủ) với cơ sở $B'$, có thể tầm thường hóa nếu $(E, p)$ có thể tầm thường hóa.

Điều này suy ra từ hệ quả 1, áp dụng với B = A và $E'= B'$.

#### Hệ quả 3 {#ta-i-s4-prop-2-cor-3 .statement tag=01P2}

Cho B là một không gian tôpô. Cho E và $E'$ là các không gian sợi B địa phương tầm thường ( resp. các phủ). Khi đó $E\times_BE'$ là một không gian sợi B địa phương tầm thường ( resp. một phủ của B). Nó có thể tầm thường hóa nếu E và $E'$ có thể tầm thường hóa.

Điều này suy ra từ hệ quả 1, áp dụng vào trường hợp A, B và $B'$ bằng nhau.

#### Mệnh đề 3 {#ta-i-s4-prop-3 .statement tag=01P3}

Cho

${E'}^{f'}$ E

$$
p'p \tag{1}
$$

${B'}^f$ B

là một bình phương Descartes. Giả sử rằng trong một lân cận của mỗi điểm của B, ánh xạ $f$ có một tiết diện liên tục. Khi đó, nếu $(E', p')$ là một không gian sợi $B'$ địa phương tầm thường ( resp. một phủ), không gian B $(E, p)$ là một không gian sợi địa phương tầm thường ( resp. một phủ).

Cần chứng minh rằng mỗi điểm $a$ của B có một lân cận U sao cho không gian U cảm sinh bởi $(E, p)$ trên U là một không gian sợi địa phương tầm thường (resp. một phủ). Lấy U là một lân cận của $a$ trên đó tồn tại một tiết diện liên tục $s$ của $f$. Gọi $i: U\rightarrow B$ và $j:\overset{-1}{p}(U)\rightarrow E$ là các phép nhúng chính tắc. Vì bình phương (1) là Descartes, tồn tại duy nhất một ánh xạ liên tục $s':\overset{-1}{p}(U)\rightarrow E'$ sao cho $f'\circ s'=j$ và $p'\circ s'=s\circ p_U$. Bình phương

$$
\overset{-1}{p}(U)^{s'}E'
$$

$$
p_{_U}p' \tag{2}
$$

U $^sB'$

do đó là giao hoán và hợp của nó với bình phương (1) là bình phương Descartes

$\overset{-1}{p}(U)^j$ E

$p_Up$

U $^iB$.

Theo mệnh đề 7 của I, p. 15, bình phương (2) là Descartes. Hệ quả 2 cho phép kết luận.

#### Nhận xét {#ta-i-s4-n3-rem-1 .statement tag=01P4}

Nếu, trong mệnh đề 3, ta làm yếu giả thiết về ánh xạ $f$ bằng cách chỉ giả sử nó ngặt phổ quát và toàn ánh, và nếu $p'$ là một phủ, thì ánh xạ $p$ là étale (I, p. 31, mệnh đề 8) và tách được (I, p. 27, mệnh đề 4), nhưng E không nhất thiết là một phủ của B. Chẳng hạn, có thể tìm một không gian tôpô B và một phủ đóng hữu hạn địa phương $(A_i)_{i\in I}$ của B, một B-không gian $(E, p)$ không phải là một phủ nhưng sao cho, với mọi $i\in I$, B-không gian $E_{A_i}$ cảm sinh là một phủ của $A_i($I, p. 146, bài tập 5). Tuy nhiên, để có một điều kiện đủ, xem hệ quả 4 của I, p. 77.

### 4. Bậc của một phủ

Cho B là một không gian tôpô, E là một phủ của B, và ký hiệu $p$ là phép chiếu của nó. Ký hiệu C là tập hợp các lực lượng Card($\overset{-1}{p}(b)$), trong đó $b$ chạy trên B. Ánh xạ $b\mapsto$ Card($\overset{-1}{p}(b)$) là một ánh xạ hằng địa phương từ B vào C. Ta nói rằng phủ E có một bậc nếu B khác rỗng và nếu ánh xạ $b\mapsto$ Card($\overset{-1}{p}(b)$) là hằng. Giá trị chung của các lực lượng Card($\overset{-1}{p}(b)$), với $b\in B$, khi đó được gọi là bậc của phủ E và được ký hiệu là deg(E$, p$), hoặc cũng là [E: B] nếu không thể có sự nhầm lẫn nào về ánh xạ $p$.

Nếu B khác rỗng, phủ tầm thường có cơ sở B và kiểu thớ F có bậc bằng Card(F).

Nếu B liên thông, hàm $b\mapsto$ Card($\overset{-1}{p}(b)$) là hằng. Do đó:

#### Mệnh đề 4 {#ta-i-s4-prop-4 .statement tag=01P5}

Mọi phủ của một không gian liên thông khác rỗng đều có một bậc.

Cho G là một không gian tôpô, $(F, g)$ là một phủ của G và $(E, f)$ là một phủ của F; giả sử các phủ này có một bậc. Nếu G-không gian $(E, g\circ f)$ là một phủ, thì nó có một bậc và ta có deg(E$, g\circ f$) $=$ deg(F$, g$) deg(E$, f$), điều này cũng có thể viết

$$
[E : G] = [E : F] [F : G]
$$

Thật vậy, nếu $z$ là một điểm của G, mọi thớ của ánh xạ

$$
f_{\overset{-1}{g}(z)}:\overset{-1}{f}(\overset{-1}{g}(z))\rightarrow \overset{-1}{g}(z)
$$

đều có lực lượng deg(E$, f$), và $\overset{-1}{g}(z)$ có lực lượng deg(F$, g$). Mệnh đề trên do đó suy ra từ nguyên lý người chăn cừu (E, III, p. 41, mệnh đề 9).

Cho B và $B'$ là các không gian tôpô, $(E, p)$ là một phủ của B và $(E', p')$ là một phủ của $B'$. Giả sử các phủ này có một bậc; khi đó phủ $(E\times E', p\times p')$ của $B\times B'$ (I, p. 71, mệnh đề 2) có một bậc và ta có:

deg(E $\times E', p\times p'$) $=$ deg(E$, p$) deg(E$', p'$).

Thật vậy, với mọi cặp $(b, b')\in B\times B'$, thớ $(E\times E')_{(b,b')}$ là tích $E_b\times E'_{b'}$.

Cho B và $B'$ là các không gian tôpô, $(E, p)$ là một phủ của B, $(E', p')$ là một phủ của $B'$ và cho

${E'}^{f'}$ E

$p'p$

${B'}^f$ B

a hình vuông Descartes. Nếu $B'$ khác rỗng và nếu phủ $(E, p)$ có một bậc, thì phủ $(E', p')$ có một bậc, bằng bậc của E, theo I, p. 10, hệ quả của mệnh đề 4.

### 5. Các phủ hữu hạn

Một phủ được gọi là hữu hạn địa phương nếu lực lượng của mọi thớ của nó đều hữu hạn. Một phủ được gọi là hữu hạn nếu tập hợp các lực lượng của các thớ của nó bị chặn trên bởi một lực lượng hữu hạn.

#### Định lý 1 {#ta-i-s4-thm-1 .statement tag=01P6}

Cho E, B là các không gian tôpô và $p: E\rightarrow B$ là một ánh xạ. Các điều kiện sau là tương đương:

(i) Không gian E, được trang bị ánh xạ $p$, là một phủ hữu hạn địa phương của B;

(ii) Ánh xạ $p$ là étale, thực sự và tách được;

(iii) Ánh xạ $p$ liên tục, mở và tách được, các thớ của nó hữu hạn, và hàm số $b\mapsto$ Card($\overset{-1}{p}(b)$) là nửa liên tục trên trên B (TG, IV, p. 28).

Ta sẽ sử dụng bổ đề sau trong chứng minh:

#### Bổ đề {#ta-i-s4-n5-lem-1 .statement tag=01P7}

Cho X và Y là các không gian tôpô. Để một ánh xạ $f: X\rightarrow Y$ là đóng, điều kiện cần và đủ là với mọi điểm $y$ của Y và mọi lân cận W của thớ $\overset{-1}{f}(y)$, tồn tại một lân cận V

của $y$ sao cho W chứa $\overset{-1}{f}(V)$.

Trong mệnh đề này, ta chỉ cần xét các lân cận W của $\overset{-1}{f}(y)$ là mở. Gọi F là phần bù của W trong Y, khi đó ta có thể phát biểu lại mệnh đề theo cách sau: để một ánh xạ $f: X\rightarrow Y$ là đóng, điều kiện cần và đủ là với mọi tập con đóng F của X, mọi điểm $y$ của Y không thuộc $f(F)$ đều có một lân cận V rời nhau với $f(F)$. Bây giờ mệnh đề này suy ra ngay lập tức từ định nghĩa của một ánh xạ đóng (TG, I, p. 30, định nghĩa 1).

Bây giờ chứng minh định lý 1. Mỗi một trong ba điều kiện đều kéo theo rằng ánh xạ $p$ liên tục, mở và tách được, và các thớ của $p$ đều hữu hạn. Điều này là hiển nhiên dưới các giả thiết (i) và (iii); dưới giả thiết (ii), các thớ của $p$ rời rạc (I, p. 29, nhận xét 2) và quasi-compact (TG, I, p. 75, định lý 1), do đó hữu hạn (TG, I, p. 60, ví dụ 1).

(i)$\Rightarrow$(ii) : chỉ cần chứng minh rằng $p$ là thực sự và, để làm điều đó, rằng với mọi tập mở U mà trên đó phủ $(E, p)$ có thể tầm thường hóa được, ánh xạ $p_U:\overset{-1}{p}(U)\rightarrow U$ là thực sự (TG, I, p. 72, mệnh đề 3). Vì các thớ của $p_U$ là hữu hạn, mệnh đề sau suy ra từ Hệ quả 5 của TG, I, p. 77.

(ii)$\Rightarrow$(iii) : cho $b$ là một điểm của B và, với mọi $x\in \overset{-1}{p}(b)$, cho $W_x$ là một lân cận mở của $x$ trong E sao cho $p|W_x$ là đơn ánh. Tập hợp $W =\bigcup_{x\in\overset{-1}{p}(b)}W_x$ là một lân cận mở của $\overset{-1}{p}(b)$. Vì ánh xạ $p$ là đóng, theo bổ đề trên tồn tại một lân cận mở U của $b$ sao cho $\overset{-1}{p}(U)\subset W$. Với mọi $a\in U$, ta có $\overset{-1}{p}(a)\subset W$; vì hạn chế của $p$ lên mỗi $W_x$ là đơn ánh, suy ra Card($\overset{-1}{p}(a)$)$\leqslant$ Card($\overset{-1}{p}(b)$), điều này chứng minh tính nửa liên tục trên của ánh xạ $a\mapsto$ Card($\overset{-1}{p}(a)$).

proves the upper semicontinuity of the mapping $a\mapsto$ Card($\overset{-1}{p}(a)$).

(iii)$\Rightarrow$(i): cho $b$ là một điểm của B. Vì thớ $E_b=\overset{-1}{p}(b)$ là hữu hạn và ánh xạ $p$ là tách được, có thể chọn, với mỗi $x\in E_b$, một lân cận mở $V'_x$ của $x$ sao cho các $V'_x$ từng đôi một rời nhau (I, p. 26, nhận xét 4). Vì ánh xạ $p$ là mở và tập hợp $E_b$ hữu hạn, tập hợp $U'=\bigcap_{x\in E_b}p(V'_x)$ là một lân cận mở của $b$ trong B. Cho U là một lân cận mở của $b$ trong B, được chứa trong $U'$ và sao cho với mọi $a\in U$, Card(E$_a$)$\leqslant$ Card(E$_b$). Với mỗi $x\in E_b$, đặt $V_x= V'_x\cap \overset{-1}{p}(U)$. Cho $a$ là một điểm của U; các tập hợp $E_a\cap V_x$, với $x\in E_b$, khác rỗng và từng đôi một rời nhau. Do đó mỗi tập hợp này chứa một phần tử duy nhất và chúng tạo thành một phân hoạch của $E_a$. Điều này cho thấy rằng, với mỗi $x\in E_b$, ánh xạ $p|V_x$ là đơn ánh và ta có $\overset{-1}{p}(U) =\bigcup_{x\in E_b}V_x$. Vì ánh xạ $p$ là mở, nó cảm sinh một đồng phôi của $V_x$ lên U và do đó, $(E, p)$ là một phủ của B (I, p. 70, hệ quả 1 của mệnh đề 1).

#### Nhận xét {#ta-i-s4-n5-rem-1 .statement tag=01P8}

Một ánh xạ liên tục, tách được, mở, thực sự với các thớ hữu hạn không nhất thiết là một phủ. Đây là trường hợp của ánh xạ $x\mapsto x^2$ của $\mathbf{R}$ vào $[0; +\infty [$.

#### Hệ quả 1 {#ta-i-s4-thm-1-cor-1 .statement tag=01P9}

Cho E và B là các không gian tôpô và cho $p: E\rightarrow B$ là một ánh xạ thực sự và tách được. Tập hợp U gồm các điểm $b$ của B sao cho $p$ là étale tại mọi điểm của thớ $E_b$ là mở trong B. Không gian U cảm sinh bởi $(E, p)$ trên U là một phủ hữu hạn địa phương.

Tập hợp F gồm các điểm của E tại đó ánh xạ $p$ không étale là đóng trong E (I, p. 29, nhận xét 1). Ảnh của nó $p(F)$ là đóng vì ánh xạ $p$ là thực sự; phần bù U của $p(F)$ do đó là mở. Ánh xạ $p_U$ là tách được (I, p. 27, mệnh đề 4) và thực sự (TG, I, p. 72, mệnh đề 3). Theo phép dựng, ánh xạ $p_U$ là étale; do đó nó thỏa mãn điều kiện (ii) của định lý 1.

#### Hệ quả 2 {#ta-i-s4-thm-1-cor-2 .statement tag=01PA}

Cho B là một không gian tôpô tách được và E là một B-không gian. Giả sử E là compact và phép chiếu $p: E\rightarrow B$ là étale. Khi đó, E là một phủ hữu hạn của B.

Ánh xạ $p$ là tách được (I, p. 26, nhận xét 2) và thực sự (TG, I, p. 76, hệ quả 2). Theo hệ quả 1, do đó E là một phủ hữu hạn địa phương của B. Vì E là compact, $p(E)$ là một tập con quasi-compact của B; ánh xạ từ $p(E)$ vào $\mathbf{N}$ cho bởi $b\mapsto$ Card $\overset{-1}{p}(b)$ là hằng địa phương, nên bị chặn trên (TG, IV, p. 30, hệ quả).

#### Hệ quả 3 {#ta-i-s4-thm-1-cor-3 .statement tag=01PB}

Cho B là một không gian tôpô, cho $(E, p)$ và $(E', p')$ là các B-không gian và cho $f: E'\rightarrow E$ là một B-cấu xạ. Giả sử rằng $E'$ là một phủ hữu hạn địa phương của B.

a) Nếu ánh xạ $p$ là étale và tách được, B-không gian $(E', f)$ là một phủ.

b) Nếu ánh xạ $f$ là toàn ánh và làm cho không gian $E'$ thành một phủ của E, thì E là một phủ của B.

Dưới giả thiết a), các ánh xạ $p$ và $p'$ là étale và tách được, và ánh xạ $p'$ là thực sự (định lý 1). Do đó ánh xạ $f$ là étale (I, p. 30, hệ quả 1 của mệnh đề 6), tách được (I, p. 25, mệnh đề 2 b)) và thực sự (I, p. 28, mệnh đề 5). Theo định lý 1, $(E', f)$ là một phủ của E.

Bây giờ giả sử rằng $f$ là toàn ánh và $(E', f)$ là một phủ của E. Khi đó nó hữu hạn địa phương, do đó ánh xạ $f$ là thực sự và toàn ánh (định lý 1). Theo I, p. 25, mệnh đề 2, c), ánh xạ $p$ là tách được, vì $p'=p\circ f$ và $p'$ là tách được. Ánh xạ $p$ là étale (I, p. 29, mệnh đề 6, d)), thực sự (TG, I, p. 73, mệnh đề 5, b)) và các thớ của nó là hữu hạn. Theo định lý 1, không gian B $(E, p)$ khi đó là một phủ của B.

#### Hệ quả 4 {#ta-i-s4-thm-1-cor-4 .statement tag=01PC}

Cho

${E'}^{f'}$ E

$p'p$

${B'}^f$ B là một bình phương Descartes. Giả sử $(E', p')$ là một phủ hữu hạn địa phương của $B'$ và ánh xạ $f$ là ngặt một cách phổ dụng và toàn ánh. Khi đó $(E, p)$ là một phủ hữu hạn địa phương của B.

Thật vậy, ánh xạ $p$ là étale (I, p. 31, mệnh đề 8), thực sự (I, p. 21, mệnh đề 11) và tách được (I, p. 27, mệnh đề 4).

#### Hệ quả 5 {#ta-i-s4-thm-1-cor-5 .statement tag=01PD}

Cho B là một không gian tôpô liên thông và $(E, p)$ là một phủ hữu hạn của B. Không gian E chỉ có một số hữu hạn các thành phần liên thông, và mỗi thành phần trong số đó là một phủ của B.

Kết quả đúng nếu B rỗng; từ nay về sau ta giả sử nó khác rỗng.

Nếu X là một tập con vừa mở vừa đóng của E, hạn chế của $p$ lên X là một ánh xạ tách được (I, p. 25, mệnh đề 2, a) và I, p. 26, nhận xét 1), étale và thực sự (TG, I, p. 74, hệ quả 1); theo định lý 1, $(X, p)$ là một phủ hữu hạn địa phương của B. Vì B liên thông, phủ này có bậc hữu hạn. Nếu X phân biệt với E, tồn tại một điểm $b\in B$ sao cho $X_b(E_b$, do đó $[X : B]<[E : B]$ vì B liên thông. Suy ra mọi dãy giảm các tập hợp vừa mở vừa đóng trong E đều dừng.

Cho $x\in E$; khi đó tồn tại một tập con nhỏ nhất X vừa mở vừa đóng của E chứa $x$ (E, III, p. 51, mệnh đề 6). Tập hợp X như vậy là liên thông; do đó nó là thành phần liên thông của $x$ trong E. Điều này cho thấy các thành phần liên thông của E vừa mở vừa đóng và mỗi thành phần trong số đó là một phủ của B. Vì B liên thông, mỗi thành phần liên thông của E gặp mỗi thớ của $p$; do đó các thành phần liên thông của E có số lượng hữu hạn.

#### Mệnh đề 5 {#ta-i-s4-prop-5 .statement tag=01PE}

Cho B là một không gian tôpô, cho E và $E'$ là các không gian B, và cho $f: E'\rightarrow E$ là một B-cấu xạ. Ta giả sử rằng E là một phủ hữu hạn địa phương và không gian $E'$, được trang bị ánh xạ $f$, là một không gian E phân thớ địa phương tầm thường ( resp. một phủ). Khi đó, $E'$ là một không gian B phân thớ địa phương tầm thường ( resp. một phủ).

Ký hiệu $p$ và $p'$ lần lượt là các phép chiếu của các không gian B E và $E'$. Cho $b$ là một điểm của B. Tồn tại một lân cận mở U của $b$ trong B và một phân hoạch hữu hạn $(V_i)_{i\in I}$ của $\overset{-1}{p}(U)$ tạo bởi các tập mở của E sao cho, với mọi $i\in I$, ánh xạ $p$ cảm sinh một phép đồng phôi từ

$V_i$ lên U. Đặt $V'_i=\overset{-1}{f}(V_i)$. Các tập hợp $V'_i$ là mở trong $E'$,

tạo thành một phân hoạch của $(^-{p'}^1)(U)$ và ánh xạ từ $V'_i$ đến U suy ra từ $p'$ bằng cách chuyển qua các không gian con biến $V'_i$ thành một không gian U phân thớ địa phương tầm thường. Do đó không gian $(^-{p'}^1)(U)$, được trang bị ánh xạ

$p'_U:(^-{p'}^1)(U)\rightarrow U$, là một không gian U phân thớ địa phương tầm thường (I, p. 69, nhận xét 2). Nếu $(E', f)$ là một phủ của E, các thớ của $p'_U$ là rời rạc vì giao của chúng với mỗi tập mở $V'_i$ đều như vậy. Chứng minh được hoàn tất.

#### Nhận xét {#ta-i-s4-n5-rem-2 .statement tag=01PF}

Nếu $(E, p)$ là một phủ của B và nếu $(E', f)$ là một phủ của E, ánh xạ $p\circ f$ là étale (I, p. 29, mệnh đề 6, a)) và tách được (I, p. 25, mệnh đề 2, a)). Tuy nhiên, có thể xảy ra, xem bài tập 5, b) của I, p. 146, rằng không gian $E'$, được trang bị ánh xạ $p\circ f$, không phải là một phủ của B. Tuy nhiên, xem IV, p. 342, mệnh đề 3.

### 6. Các phủ của các không gian liên thông địa phương

Cho B là một không gian tôpô và E là một B-không gian. Giả sử phép chiếu $p$ của nó là một ánh xạ étale và tách được.

Nếu không gian B liên thông địa phương thì không gian E liên thông địa phương. Nếu không gian E liên thông địa phương thì tập con mở $p(E)$ của B (xem I, p. 29, nhận xét 2) liên thông địa phương.

Ảnh $s(B)$ của mọi tiết diện $s$ của $p$ đều mở (I, p. 30, hệ quả 3) và đóng trong B (I, p. 27, mệnh đề 3). Nếu B liên thông và khác rỗng, thì do đó nó là một thành phần liên thông của E; nói chung, nó là một hợp của các thành phần liên thông của E.

Nếu B liên thông địa phương, thì hợp các ảnh của các tiết diện của $p$ do đó là một tập con mở và đóng của E (xem TG, I, p. 85).

Giả sử E là một phủ tầm thường hóa được của B và cho $g: E\rightarrow B\times F$ là một phép tầm thường hóa. Nếu không gian B liên thông, các tập hợp $V_x=\overset{-1}{g}(B\times  \{x\})$, với $x$ chạy trên F, là các thành phần liên thông của E (xem mệnh đề 1 của I, p. 69).

#### Mệnh đề 6 {#ta-i-s4-prop-6 .statement tag=01PG}

Cho B là một không gian tôpô và E là một B-không gian; ký hiệu $p$ là phép chiếu của nó. Giả sử không gian E liên thông địa phương. Để E là một phủ của B, điều kiện cần và đủ là mọi điểm của B đều có một lân cận mở U sao cho ánh xạ $p$ cảm sinh một phép đồng phôi từ mỗi thành phần liên thông của $\overset{-1}{p}(U)$ lên U.

Cho $b$ là một điểm của B. Nếu E là một phủ của B, mọi lân cận mở U của $b$ liên thông và trên đó phủ E tầm thường hóa được đều thỏa mãn các điều kiện nêu trong mệnh đề. Ngược lại, cho U là một lân cận mở của $b$ thỏa mãn các điều kiện này. Tập hợp $\overset{-1}{p}(U)$ là mở; các thành phần liên thông của nó là các tập con mở của E (TG, I, p. 85, mệnh đề 11) và tạo thành một phân hoạch của $\overset{-1}{p}(U)$. Do đó mệnh đề suy ra từ hệ quả 1 (I, p. 70) của mệnh đề 1.

#### Hệ quả 1 {#ta-i-s4-prop-6-cor-1 .statement tag=01PH}

Cho B là một không gian tôpô liên thông địa phương, $(E, p)$ là một phủ của B và $E'$ là một tập con mở và đóng của E. B-không gian $(E', p|E')$ là một phủ và $p(E')$ là mở và đóng trong B.

Các không gian E và $E'$ đều liên thông địa phương. Với mọi tập con mở U của B, tập hợp $E'\cap \overset{-1}{p}(U)$ là mở và đóng trong $\overset{-1}{p}(U)$, do đó là một hợp của các thành phần liên thông của $\overset{-1}{p}(U)$. Các tập con mở U của B sao cho $p$ cảm sinh một phép đồng phôi từ mỗi thành phần liên thông của $\overset{-1}{p}(U)$ lên U phủ B. Theo mệnh đề, $p|E'$ biến $E'$ thành một phủ của B. Mệnh đề thứ hai suy ra từ điều này (xem I, p. 68).

#### Hệ quả 2 {#ta-i-s4-prop-6-cor-2 .statement tag=01PI}

Cho B là một không gian tôpô liên thông địa phương, $(E, p)$, $(E', p')$ là các phủ của B và $f, g: E'\rightarrow E$ là các B-đồng cấu. Với mọi điểm $b$ của B, ký hiệu $f_b, g_b: E_b\rightarrow E'_b$ là các ánh xạ suy ra từ $f$ và $g$, tương ứng. Tập hợp các điểm $b$ của B sao cho $f_b=g_b$ là mở và đóng trong B.

Cho X là tập hợp các điểm $x$ của $E'$ sao cho $f(x) =g(x)$. Nó là tập hợp các điểm tại đó các phép nâng $f$ và $g$ của $p'$ lên E trùng nhau; do đó X là mở và đóng trong $E'$ (mệnh đề 11 của I, p. 34). Phần bù Y của X cũng mở và đóng; do đó $p(Y)$ là mở và đóng trong B (hệ quả 1). Phần bù của nó, tức là tập hợp các điểm $b$ của B sao cho $f_b=g_b$, do đó cũng như vậy.

#### Hệ quả 3 {#ta-i-s4-prop-6-cor-3 .statement tag=01PJ}

Cho B là một không gian tôpô liên thông và liên thông địa phương, $(E, p)$ và $(E', p')$ là các phủ của B. Với mọi điểm $b$ của B, ánh xạ $f\mapsto f_b$ từ $\mathscr{C}_B(E'; E)$ vào $\mathscr{C}(E'_b; E_b)$ là đơn ánh.

Cho $b$ là một điểm của B. Cho $f$ và $g$ là các B-cấu xạ từ $E'$ vào E sao cho $f_b=g_b$. Tập hợp các điểm $a$ của B sao cho $f_a=g_a$ là mở và đóng trong B (Hệ quả 2) và chứa $b$. Do đó nó bằng B, và $f$ bằng $g$.

#### Hệ quả 4 {#ta-i-s4-prop-6-cor-4 .statement tag=01PK}

Cho B là một không gian tôpô liên thông và liên thông địa phương, cho $(E, p)$ là một phủ của B, và cho $b$ là một điểm của B. Để E là một phủ tầm thường hóa được, điều kiện cần và đủ là mọi điểm của thớ $E_b$ thuộc ảnh của một tiết diện liên tục của $p$.

Điều kiện này là cần. Gọi $E'$ là hợp của các ảnh của các tiết diện liên tục của $p$, và gọi $E''$ là phần bù của nó trong E. Tập hợp $E'$ mở và đóng trong E (xem I, p. 79). Do đó $(E', p|E')$ là một phủ của B (Hệ quả 1), và phủ này tầm thường hóa được theo Hệ quả 2 (I, p. 70). Giả sử $E'$ chứa $E_b$ và hãy chứng minh rằng $E''$ rỗng. Vì $E''$ mở và đóng trong E, $p(E'')$ mở và đóng trong B (Hệ quả 1). Vì B liên thông và $b$ không thuộc $p(E''),p(E'') =\emptyset$, do đó $E''=\emptyset$.

#### Hệ quả 5 {#ta-i-s4-prop-6-cor-5 .statement tag=01PL}

Cho

${E'}^{f'}$ E

$p'p$

${B'}^f$ B

là một hình vuông Descartes. Giả sử rằng không gian B $(E, p)$ là một phủ và không gian $B'$ liên thông và liên thông địa phương. Cho $b'$ là một điểm của $B'$. Để không gian $B'$ $(E', p')$ là một phủ tầm thường hóa được, điều kiện cần và đủ là với mọi điểm $x$ của E sao cho $p(x) =f(b')$, tồn tại một phép nâng liên tục $g: B'\rightarrow E$ của $f$ sao cho $g(b') =x$.

Ta nhắc lại rằng $(E', p')$ là một phủ của $B'($I, p. 71, Hệ quả 2) và ánh xạ $f'$ cảm sinh một song ánh $E'_{b'}\rightarrow E_{f(b')}($I, p. 10, Hệ quả). Theo Mệnh đề 3 của I, p. 9, ánh xạ $s\mapsto f'\circ s$ xác định một song ánh giữa tập hợp các tiết diện liên tục của $p'$ và tập hợp các phép nâng liên tục của $f$ vào E. Do đó hệ quả suy ra từ Hệ quả 4.

#### Mệnh đề 7 {#ta-i-s4-prop-7 .statement tag=01PM}

Cho B là một không gian tôpô, cho E và $E'$ là các không gian B, và cho $f: E'\rightarrow E$ là một B-cấu xạ. Giả thiết rằng $E'$ là một phủ của B và không gian B liên thông địa phương.

a) Nếu phép chiếu của không gian B E là một ánh xạ étale và tách, $(E', f)$ là một phủ của E.

b) Nếu $f$ là toàn ánh, thì E là một phủ của B.

Gọi $p$ và $p'$ lần lượt là các phép chiếu của các không gian B E và $E'$. Theo giả thiết a$),f$ là étale (I, p. 29, Mệnh đề 6, c)). Theo giả thiết b$),p$ là étale (loc. cit., d)). Do đó, theo một trong hai giả thiết này, E liên thông địa phương; đặc biệt, các thành phần liên thông của nó mở và đóng trong E (TG, I, p. 85, Mệnh đề 11).

Trước hết ta chứng minh Mệnh đề 7 dưới giả thiết bổ sung rằng B liên thông, liên thông địa phương, và $E'$ là phủ tầm thường $(B\times F'$, pr$_1)$.

#### Bổ đề {#ta-i-s4-n6-lem-1 .statement tag=01PN}

Nếu U là một thành phần liên thông của $E'$, hạn chế của $f$ lên U cảm sinh một phép đồng phôi từ U lên một thành phần liên thông của E.

Cho $x\in F'$ sao cho $U = B\times  \{x\}($xem I, p. 79). Ánh xạ từ B vào E gán cho $b\in B$ phần tử $f(b, x)$ là một tiết diện liên tục của $p$. Do đó, ảnh X của nó là liên thông và mở trong E, vì $p$ là etale (I, p. 30, Hệ quả 3). Hơn nữa nó đóng theo giả thiết a), vì $p$ là tách (I, p. 27, Mệnh đề 3). Nó cũng đóng theo giả thiết b) theo Hệ quả 1 của I, p. 80, vì U mở và đóng trong $E'$. Do đó, X là một thành phần liên thông của E.

Vì $f|U: U\rightarrow X$ là song ánh và mở, nên nó là một phép đồng phôi lên ảnh của nó, điều này chứng minh bổ đề.

Ta giữ lại các giả thiết trước bổ đề và bây giờ chứng minh mệnh đề a). Cho V là một thành phần liên thông của E. Nó là một

tập hợp mở và đóng trong E và $\overset{-1}{f}(V)$ là hợp của các thành phần liên thông của $E'$ mà theo bổ đề $f$ ánh xạ đồng phôi lên V. Theo Mệnh đề 6 của I, p. 79, suy ra rằng $(E', f)$ là một phủ.

Ta chứng minh b). Vì $f$ là toàn ánh, theo bổ đề suy ra rằng mọi thành phần liên thông V của E là ảnh đồng phôi của một thành phần liên thông $U = B\times \{x\}$ của $E'$. Khi đó ánh xạ $p$ cảm sinh một phép đồng phôi từ V lên B. Theo Mệnh đề 6, E là một phủ của B.

Do đó điều này chứng minh mệnh đề, dưới giả thiết bổ sung rằng B liên thông và $E'$ là một phủ tầm thường hóa được của B. Ta chứng minh nó trong trường hợp tổng quát.

Tồn tại một phủ $(U_i)_{i\in I}$ của B, gồm các tập hợp mở liên thông trên đó phủ $E'$ tầm thường hóa được. Cho $i\in I$.

Ta chứng minh a). Nếu ánh xạ $p$ là etale và tách, thì điều tương tự cũng đúng đối với ánh xạ $p_{U_i}: U_i\times_BE\rightarrow U_i$, với $i\in I$, theo các Mệnh đề 8 của I, p. 31 và 4 của I, p. 27. Do đó theo trường hợp riêng đã xét, ta có,

với mọi $i\in I$, $U_i$-không gian ($(^-{p'}^1)(U_i), f_{U_i}$) là một phủ. Ký hiệu A là không gian tổng của các $U_i$ và $q: A\rightarrow B$ là ánh xạ chính tắc. Khi đó không gian $A\times_BE'$, được trang bị ánh xạ $f_A: A\times_BE'\rightarrow A\times_BE$ là một phủ của $A\times_BE$. Ánh xạ $q$ có một tiết diện liên tục trong một lân cận của mỗi điểm của B và Mệnh đề 3 của I, p. 72, áp dụng vào bình phương Descartes

$$
A\times_BE'E'
$$

$$
_{f_A}f
$$

$A\times_BE$ E

suy ra rằng $E'$ là một phủ của E.

Ta chứng minh b). Giả sử $f$ là toàn ánh. Khi đó, với mọi phần tử $i$ của I, ánh xạ $f_{U_i}: U_i\times_BE'\rightarrow U_i\times_BE$ là toàn ánh và không gian $U_i\times_BE'$, được trang bị ánh xạ $f_{U_i}$, là một phủ của $U_i\times_BE$ (I, p. 71, Hệ quả 2 của Mệnh đề 2). Theo trường hợp riêng đã xét ở trên, $U_i$-không gian $(\overset{-1}{p}(U_i), p_{U_i})$ là một phủ. Do đó, E là một phủ của B.

Cho B là một không gian tôpô, cho E và $E'$ là các phủ của B, và cho $f: E\rightarrow E'$ là một B-cấu xạ. Ta đã thấy rằng $(E, f)$ là một phủ dưới mỗi một trong hai giả thiết sau: 1) phủ E có bậc hữu hạn địa phương (I, p. 76, Hệ quả 1); 2) không gian B liên thông địa phương (I, p. 81, Mệnh đề 7). Hiện tượng này có thể được giải thích như sau.

Cho F và $F'$ là các không gian tôpô rời rạc và cho $f: B\times F\rightarrow$ $B\times F'$ là một cấu xạ B. Ánh xạ $\widetilde{f}:a\mapsto$ pr$_2\circ f(b,\cdot )$ từ B vào không gian $\mathscr{C}_c(F; F')$ là liên tục (TG, X, p. 28, th. 3). Nếu U là một tập mở của B sao cho ánh xạ $\widetilde{f}$ là hằng trên U, thì ánh xạ $f_U: U\times$ $F\rightarrow U\times F'$ suy ra từ $f$ là một phủ tầm thường hóa được (I, p. 69, prop. 1).

Không gian $\mathscr{C}_c(F; F')$ không gì khác hơn là tập hợp $\mathscr{F}(F; F')$ các ánh xạ từ F vào $F'$ được trang bị tôpô suy ra từ tôpô của không gian tích $(F')^F$ bởi phép đồng nhất chính tắc. Đối với tôpô này, không gian $\mathscr{F}(F; F')$ hoàn toàn không liên thông (I, p. 84, prop. 10). Do đó, nếu không gian B liên thông, ánh xạ $\widetilde{f}$ là hằng (I, p. 82, prop. 4); nếu không gian B liên thông địa phương, ánh xạ $\widetilde{f}$ là hằng địa phương. Khi tập hợp F hữu hạn, không gian $\mathscr{F}(F; F')$ rời rạc và ánh xạ $\widetilde{f}$ là hằng địa phương.

#### Nhận xét {#ta-i-s4-n6-rem-1 .statement tag=01PO}

Cho B là một không gian tôpô, cho $(E, p)$ và $(E', p')$ là các không gian B và cho $f: E'\rightarrow E$ là một cấu xạ B.

a) Nếu E và $E'$ là các phủ của B, ánh xạ $f$ là étale (I, p. 29, prop. 6) và tách được (I, p. 25, prop. 2). Nhưng nói chung, không đúng rằng $(E', f)$ là một phủ của E nếu không gian B không liên thông địa phương (I, p. 145, exerc. 4).

b) Nếu $(E', p')$ là một phủ của B, $f$ là toàn ánh và biến $E'$ thành một phủ của E, thì ánh xạ $p$ là étale (I, p. 29, prop. 6). Nhưng nói chung, không đúng rằng nó tách được nếu không gian B không liên thông địa phương (I, p. 145, exerc. 4). Đặc biệt, E không nhất thiết là một phủ của B.

#### Hệ quả {#ta-i-s4-n6-cor-1 .statement tag=01PP}

Cho B là một không gian tôpô liên thông và liên thông địa phương. Cho E và $E'$ là các phủ của B. Cho $b$ là một điểm của B. Cho $f: E'\rightarrow E$ là một cấu xạ B và cho $f_b: E'_b\rightarrow E_b$ là ánh xạ suy ra từ $f$ bằng cách hạn chế lên các thớ. Nếu ánh xạ $f_b$ là đơn ánh ( resp. toàn ánh, resp. song ánh), thì điều tương tự cũng đúng với ánh xạ $f$.

Ta ký hiệu $p$ là phép chiếu của không gian B E. Theo mệnh đề, $(E', f)$ là một phủ của E; ảnh $f(E')$ của nó là mở và đóng trong E. Gọi U là phần bù của $f(E')$ trong E, sao cho không gian B $(U, p|U)$ là một phủ của B (I, p. 80, corollary 1). Nếu ánh xạ $f_b$ là toàn ánh, thớ tại $b$ của phủ này là rỗng. Vì B là một không gian liên thông, khi đó U rỗng, do đó $f$ là toàn ánh.

Tập hợp V các điểm của E tại đó thớ của $f$ có đúng một phần tử là mở và đóng. Các không gian B $(V, p|V)$ và $(f(E'), p|f(E'))$ là các phủ của B (loc. cit.) và ánh xạ chính tắc $i: V\rightarrow$ $f(E')$ là một cấu xạ B. Nếu ánh xạ $f_b$ là đơn ánh, ánh xạ $i_b$ là toàn ánh, do đó $i$ là toàn ánh theo điều vừa chứng minh, và ta có $V =f(E')$. Do đó, ánh xạ $f$ là đơn ánh.

### 7. Các phủ của một không gian tựa compact

#### Mệnh đề 8 {#ta-i-s4-prop-8 .statement tag=01PQ}

Một phủ của một không gian tựa compact ( I, p. 69) là một không gian tựa compact.

Trước hết, ta chứng minh một bổ đề.

#### Bổ đề {#ta-i-s4-n7-lem-1 .statement tag=01PR}

Cho E là một không gian tôpô tách được. Giả sử E có một phủ mở hữu hạn địa phương $(V_i)_{i\in I}$ sao cho, với mọi $i\in I,\overline{V_i}$ là một không gian tựa compact. Khi đó không gian E là tựa compact.

Cho $(W_j)_{j\in J}$ là một phủ mở của E; ta sẽ chứng minh rằng tồn tại một phủ mở hữu hạn địa phương $(A_k)_{k\in K}$ của E mịn hơn phủ $(W_j)_{j\in J}$. Với mỗi $i\in I$, cho $(A'_{\ell})_{\ell\in K_i}$ là một phủ hữu hạn địa phương của $\overline{V_i}$ bởi các tập mở của $\overline{V_i}$, mịn hơn phủ $(W_j\cap \overline{V_i})_{j\in J}$. Cho K là tổng của họ $(K_i)_{i\in I}$ (E, II, p. 30, Def. 8). Với mỗi phần tử $k= (\ell , i)$ của K, đặt $A_k= A'_{\ell}\cap V_i$. Khi đó $A_k$ mở trong E và ta có $\bigcup_{k\in K}A_k=\bigcup_{i\in I}V_i= E$; hơn nữa, với mỗi $k\in K$, tồn tại một chỉ số $j\in J$ sao cho $A_k\subset W_j$. Do đó, họ $(A_k)_{k\in K}$ là một phủ mở của E mịn hơn $(W_j)_{j\in J}$. Còn phải chứng minh rằng họ $(A_k)_{k\in K}$ là hữu hạn địa phương. Cho $x\in E$; tồn tại một lân cận mở U của $x$ chỉ gặp $V_i$ với $i$ thuộc một tập con hữu hạn $I'$ của I. Với mỗi $i\in I'$, $x$ có một lân cận mở $U_i\subset U$ chỉ gặp một số hữu hạn các tập mở $A_k$, với $k\in K_i\times \{i\}$: điều này hiển nhiên nếu $x$ không thuộc $\overline{V_i}$, còn nếu $x$ thuộc $\overline{V_i}$, thì điều này suy ra từ tính chất hữu hạn địa phương của phủ $(A'_{\ell})_{\ell\in K_i}$ của $\overline{V_i}$. Suy ra rằng $V'=\bigcap_{i\in I'}U_i$ là một lân cận mở của $x$ chỉ gặp một số hữu hạn các $A_k,k\in K$, và phủ $(A_k)_{k\in K}$ là hữu hạn địa phương.

Ta hãy chứng minh mệnh đề. Cho E là một phủ của B, ký hiệu $p$ là phép chiếu của nó, và giả sử rằng không gian B là paracompact. Cho $(A_i)_{i\in I}$ là một phủ mở hữu hạn địa phương của B sao cho, với mỗi $i\in I$, phủ E là tầm thường hóa được trên $A_i$. Với mỗi $i\in I$, cho $F_i$ là một không gian tôpô rời rạc và cho $g_i:\overset{-1}{p}(A_i)\rightarrow A_i\times F_i$ là một phép tầm thường hóa của E trên $A_i$. Cho $(B_i)_{i\in I}$ là một phủ mở của B sao cho, với mỗi $i\in I$, ta có $\overline{B_i}\subset A_i$ (TG, IX, p. 49, Prop. 4 và p. 48, Cor. 1). Với mỗi $i\in I$, đặt $V_i=\overset{-1}{p}(B_i)$; ta có $\overline{V_i}\subset \overset{-1}{p}(B_i)\subset \overset{-1}{p}(A_i)$ và $V_i=\overset{-1}{g_{i}}(B_i\times F_i)$, do đó $\overline{V_i}\subset \overset{-1}{g_{i}}(B_i\times F_i)$. Vì B là paracompact, $\overline{B_i}$ là paracompact (TG, I, p. 69, Prop. 16) và $\overline{B_i}\times F_i$ là paracompact (TG, I, p. 70, Prop. 18). Suy ra $\overset{-1}{g_{i}}(B_i\times F_i)$ là paracompact, do đó $\overline{V_i}$ cũng vậy (TG, I, p. 69, Prop. 16). Họ $(V_i)_{i\in I}$, theo phép dựng, là một phủ mở hữu hạn địa phương của E. Cuối cùng, không gian E là tách được (I, p. 26, Remark 3). Do đó nó thỏa mãn các giả thiết của bổ đề, do đó mệnh đề.

#### Nhận xét {#ta-i-s4-n7-rem-1 .statement tag=01PS}

Có thể chứng minh rằng một phủ của một không gian khả mêtric là khả mêtric (I, p. 145, Exer. 1) và một phủ liên thông của một không gian địa phương compact đếm được tại vô hạn cũng là địa phương compact đếm được tại vô hạn (I, p. 145, Exer. 2).

### 8. Các bó hằng địa phương

Cho B là một không gian tôpô và F là một tập hợp; trang bị cho F tôpô rời rạc. Bó trên B gồm các ánh xạ hằng địa phương nhận giá trị trong F được gọi là bó hằng trên B với kiểu thớ F (I, p. 45, Ví dụ 2). Bó này đôi khi được ký hiệu bởi F, khi không có nguy cơ nhầm lẫn về không gian B. Nó được đồng nhất với bó trên B gồm các thiết diện liên tục của B-không gian étalé $(B\times F$, pr$_1$): công thức $i([U, s, a]) = (a, s(a))$ thực sự xác định một đẳng cấu chính tắc $i$ từ không gian étalé liên kết với F lên $(B\times F$, pr$_1)$. Với mọi $a\in B$, ánh xạ $[U, s, a]\mapsto s(a)$ là một song ánh chính tắc từ thớ $F_a$ của F tại $a$ lên tập hợp F.

Cho $\mathscr{P}= (\mathscr{P}(U), r_{UV})$ là tiền bó trên B sao cho $\mathscr{P}(U) = F$ với mọi tập mở U của B và $r_{UV}=$ Id$_F$ với mọi cặp $(U,V)$ các tập mở của B sao cho $U\subset V$. Khi đó bó $\widetilde{\mathscr{P}}$ liên kết với $\mathscr{P}$ là đẳng cấu chính tắc với bó hằng F (I, p. 52, Ví dụ 1).

#### Định nghĩa 3 {#ta-i-s4-def-3 .statement tag=01PT}

Một bó $\mathscr{F}$ trên một không gian tôpô B được gọi là hằng địa phương nếu mọi điểm của B đều có một lân cận mở U sao cho bó cảm sinh $\mathscr{F}|U$ là đẳng cấu với một bó hằng trên U.

#### Mệnh đề 9 {#ta-i-s4-prop-9 .statement tag=01PU}

Để một bó là hằng địa phương, điều kiện cần và đủ là không gian étalé liên kết với nó là một phủ.

Cho B là một không gian tôpô và $\mathscr{F}$ là một bó trên B. Bó $\mathscr{F}$ là hằng khi và chỉ khi không gian étalé $E_{\mathscr{F}}$ là B-đẳng cấu với một phủ tầm thường $(B\times F$, pr$_1)$, trong đó F là một không gian tôpô rời rạc. Nếu U là một tập mở của B, không gian étalé liên kết với bó cảm sinh $\mathscr{F}|U$ được đồng nhất với U-không gian étalé cảm sinh nhận được từ $E_{\mathscr{F}}$ trên U (cf. I, p. 51). Mệnh đề được suy ra.

#### Hệ quả {#ta-i-s4-n8-cor-1 .statement tag=01PV}

Để một B-không gian étalé là một phủ, điều kiện cần và đủ là bó các thiết diện của nó là hằng địa phương.

Điều này suy ra từ mệnh đề và từ Ví dụ 2 của I, p. 52.

### 9. Tích của các bó hằng địa phương

Cho B là một không gian tôpô và $(\mathscr{F}_i)_{i\in I}$ là một họ các bó trên B. Ký hiệu $\mathscr{F}$ là bó tích $\prod_{i\in I}\mathscr{F}_i$ và, với $i\in I$, cho pr$_i:\mathscr{F}\rightarrow \mathscr{F}_i$ là cấu xạ phép chiếu có chỉ số $i($I, p. 46, Ví dụ 7). Gọi $(E, p)$ và $(E_i, p_i)$ lần lượt là các B-không gian étalé liên kết với các bó $\mathscr{F}$ và $\mathscr{F}_i$, và $\varphi_i: E\rightarrow E_i$ là B-cấu xạ liên kết với pr$_i($I, p. 50). Cuối cùng, ký hiệu $(E', p')$ là B-tích $\prod_BE_i$. Theo tính chất phổ quát của B-không gian tích (I, p. 5), tồn tại duy nhất một B-cấu xạ $\Phi : E\rightarrow E'$ sao cho, với mọi $i\in I$, pr$_i\circ \Phi  =\varphi_i$.

#### Mệnh đề 10 {#ta-i-s4-prop-10 .statement tag=01PW}

Nếu tập hợp I là hữu hạn, B-cấu xạ Φ là một đẳng cấu.

Theo hệ quả của I, p. 32, B-không gian $E'$ là étalé, và chỉ cần chứng minh rằng B-cấu xạ Φ là song ánh ( I, p. 30, Cor. 2). Với mọi điểm $b$ của B, hạn chế $\Phi_b: E_b\rightarrow E'_b$ của Φ lên các thớ tại b được đồng nhất với ánh xạ chính tắc từ lim$\longrightarrow \prod^{i\in I}\mathscr{F}_i(U)$ vào $\prod_{i\in I}$ lim$\longrightarrow \mathscr{F}_i(U)$, trong đó U chạy qua tập hợp các tập mở của B chứa $b($cf. I, p. 50). Theo Prop. 10 của E, III, p. 67, ánh xạ này là một song ánh.

Bây giờ xét trường hợp các bó hằng địa phương trên một không gian tôpô B. Cho $(F_i)_{i\in I}$ là một họ các tập hợp và đặt $F =\prod_{i\in I}F_i$. Một cấu xạ chính tắc $\psi = (\psi_U)$ từ bó hằng F vào tích $\prod_{i\in I}F_i$ của các bó hằng $F_i$ được xác định bằng cách đặt, với mọi tập mở U của B và mọi hàm hằng địa phương $f: U\rightarrow F,\psi_U(f) =$ (pr$_i\circ f$)$_{i\in I}$.

#### Mệnh đề 11 {#ta-i-s4-prop-11 .statement tag=01PX}

i_U(f) =$ (pr$_i\circ f$)$_{i\in I}$.

Nếu tập hợp I là hữu hạn, hoặc nếu không gian B liên thông địa phương, thì cấu xạ chính tắc $\psi : F\rightarrow \prod F_i$ là một đẳng cấu.

Cho U là một tập mở của B. Rõ ràng ánh xạ $\psi_U$ là đơn ánh. Hãy chứng minh rằng nó là toàn ánh. Cần chứng minh rằng với mọi họ $(f_i)_{i\in I}$ trong đó $f_i$ là một ánh xạ hằng địa phương từ U vào $F_i$, và mọi điểm $a$ của U, tồn tại một lân cận V của $a$ trong U sao cho với mọi $i\in I$, ánh xạ $f_i|V$ là hằng. Khi tập hợp I là hữu hạn, sự tồn tại của một lân cận như vậy là rõ ràng. Khi không gian B liên thông địa phương, chỉ cần lấy V là một lân cận liên thông của $a$ trong U. Điều này chứng minh mệnh đề.

#### Hệ quả 1 {#ta-i-s4-prop-11-cor-1 .statement tag=01PY}

Một tích hữu hạn các bó hằng địa phương là hằng địa phương.

Cho $(\mathscr{F}_i)_{i\in I}$ là một họ hữu hạn các bó hằng địa phương trên B. Mỗi điểm $a$ của B có một lân cận mở U trong B sao cho, với mọi $i\in I$, bó $\mathscr{F}_i|U$ đẳng cấu với một bó hằng. Khi đó điều tương tự cũng đúng với bó $((\prod\mathscr{F}_i)|U$, là bó bằng $\prod ((\mathscr{F}_i|U)$.

#### Hệ quả 2 {#ta-i-s4-prop-11-cor-2 .statement tag=01PZ}

Cho $(\mathscr{F}_i)_{i\in I}$ là một họ các bó trên B. Giả sử không gian B liên thông địa phương và mọi điểm của B có một lân cận mở U sao cho, với mọi $i\in I$, bó $\mathscr{F}_i|U$ đẳng cấu với một bó hằng. Khi đó bó tích $\prod\mathscr{F}_i$ là hằng địa phương.

#### Nhận xét 1 {#ta-i-s4-n9-rem-1 .statement tag=01Q0}

Cho $(E_i, p_i)_{i\in I}$ là một họ các phủ của không gian tôpô B. Giả sử không gian B liên thông địa phương và tồn tại một phủ mở $(U_j)_{j\in J}$ của B sao cho, với mọi $j\in J$ và mọi $i\in I$, phủ $E_i$ là tầm thường hóa được trên $U_j$. Với $i\in I$, gọi $\mathscr{F}_i$ là bó hằng địa phương các thiết diện của $E_i$ và gọi $\mathscr{F}$ là bó tích $\prod_i\mathscr{F}_i$. Theo hệ quả trước, $\mathscr{F}$ là một bó hằng địa phương và không gian B-étalé E liên kết với nó do đó là một phủ (I, p. 86, mệnh đề 8). Với $i\in I$, gọi pr$_i: E\rightarrow E_i$ là B-cấu xạ cảm sinh bởi cấu xạ phép chiếu có chỉ số $i,\mathscr{F}\rightarrow \mathscr{F}_i$.

Bây giờ xét một phủ $(Y, q)$ của B và, với mọi $i\in$ I, gọi $f_i: Y\rightarrow E_i$ là một B-cấu xạ. Nếu $\mathscr{G}$ ký hiệu bó hằng địa phương các thiết diện của $q$, thì các B-cấu xạ $f_i$ cảm sinh các cấu xạ bó $\widetilde{f}_i:\mathscr{G}\rightarrow \mathscr{F}_i$. Gọi $\widetilde{f}:\mathscr{G}\rightarrow \mathscr{F}$ là cấu xạ bó duy nhất sao cho $\widetilde{f}_i=$ pr$_i\circ \widetilde{f}$ với mọi $i\in I$. Khi đó tồn tại duy nhất một B-cấu xạ $f: Y\rightarrow E$ sao cho $f_i$ = pr$_i\circ f$ với mọi $i:$ đó là B-cấu xạ cảm sinh $\widetilde{f}$.

Đôi khi người ta nói rằng E là phủ tích của họ $(E_i)_{i\in I}$.

#### Nhận xét 2 {#ta-i-s4-n9-rem-2 .statement tag=01Q1}

Với các ký hiệu trên, cấu xạ B chính tắc $\Phi : E\rightarrow \prod_BE_i$ là song ánh. Thực ra, vấn đề có tính chất địa phương trên B, và ta có thể giả sử rằng, với mọi $i\in I$, không gian B $E_i$ là đẳng cấu với không gian B $(B\times F_i$, pr$_1$), trong đó $F_i$ là một không gian tôpô rời rạc, sao cho bó $\mathscr{F}_i$ là đẳng cấu với bó $F_i$. Theo Mệnh đề 11, bó $\mathscr{F}$ được đồng nhất với bó F, trong đó F là tập hợp $\prod F_i$, được trang bị tôpô rời rạc, và ánh xạ Φ được đồng nhất với ánh xạ chính tắc $B\times F\rightarrow B\times (\prod_iF_i)$, là song ánh.

### 10. Các cấu xạ của các bó hằng địa phương trên một không gian liên thông địa phương

Cho B là một không gian tôpô, và $(E, p)$ và $(E', p')$ là các không gian B. Ta ký hiệu $\mathscr{M}$ = $\mathscr{M}$or$_B(E; E')$ là bó trên B gồm các cấu xạ B của $(E, p)$ vào $(E', p')$ (I, p. 45, Ví dụ 4). Nếu U là một tập mở của B và $b$ là một điểm của U, ta ký hiệu $\theta_{b,U}:\mathscr{M}(U)\rightarrow \mathscr{C}(E_b; E'_b)$ là ánh xạ chính tắc thu được bằng cách chuyển qua các thớ tại $b$. Người ta ký hiệu $\theta_b:\mathscr{M}_b\rightarrow$ $\mathscr{C}(E_b; E'_b)$ là ánh xạ duy nhất sao cho $\theta_{b,U}$ là hợp thành của $\theta_b$ và ánh xạ chính tắc $\mathscr{M}(U)\rightarrow \mathscr{M}_b$ với mọi tập mở U của B chứa $b$ (E, III, p. 62).

Ngoài ra, cho $\mathscr{I}=\mathscr{I}$som$_B(E; E')$ là bó trên B gồm các đẳng cấu B của $(E, p)$ vào $(E', p')$. Ta ký hiệu $i:\mathscr{I}\rightarrow \mathscr{M}$ là cấu xạ chính tắc. Với mọi $b\in B$, ánh xạ $\theta_b\circ i_b$ cảm sinh một ánh xạ $\theta '_b$ từ $\mathscr{I}_b$ vào tập hợp các song ánh liên tục của $E_b$ lên $E'_b$.

#### Mệnh đề 12 {#ta-i-s4-prop-12 .statement tag=01Q2}

Giả sử không gian B là liên thông địa phương và các không gian B E và $E'$ là các phủ. Khi đó bó $\mathscr{M}$or$_B(E; E')$ là hằng địa phương và, với mọi $b\in B$, ánh xạ $\theta_b$ là một song ánh từ thớ của nó tại $b$ lên tập hợp các ánh xạ từ $E_b$ vào $E'_b$.

Tương tự, bó $\mathscr{I}$som$_B(E; E')$ là hằng địa phương và, với mọi điểm $b$ của B, ánh xạ $\theta '_b$ là một song ánh từ thớ của nó tại $b$ lên tập hợp các song ánh từ $E_b$ lên $E'_b$.

Ta sẽ ký hiệu $\mathscr{M}=\mathscr{M}$or$_B(E; E')$ và $\mathscr{I}=\mathscr{I}$som$_B(E; E')$. Các mệnh đề cần chứng minh có tính chất địa phương trên B; do đó ta có thể giả sử rằng $E = B\times F$ và $E'= B\times F'$ là các phủ tầm thường, trong đó F và $F'$ là các không gian tôpô rời rạc.

Trước hết, ta chứng minh rằng, với mọi tập mở liên thông U của B và mọi điểm $b$ của U, ánh xạ $\theta_{b,U}$ là một song ánh. Cho $f: U\times F\rightarrow$ $U\times F'$ là một cấu xạ của các không gian U; khi đó $\theta_{b,U}(f)$ là ánh xạ $y\mapsto$ pr$_2(f(b, y))$ từ F vào $F'$. Với mọi $y\in F$, ánh xạ $x\mapsto$ pr$_2(f(x, y))$ là một ánh xạ liên tục từ không gian liên thông U vào không gian rời rạc $F'$, và do đó là hằng, bằng pr$_2(f(b, y))$. Vậy $f(x, y) = (x, \theta_{b,U}(f)(y))$. Suy ra $\theta_{b,U}$ là một song ánh; song ánh ngược của nó liên kết với mỗi ánh xạ $\varphi : F\rightarrow F'$ cấu xạ U từ $U\times F$ vào $U\times F'$ cho bởi $(x, y)\mapsto (x, \varphi (y))$.

Theo giả thiết, mỗi điểm $b\in B$ có một cơ sở các lân cận mở liên thông; do đó ánh xạ $\theta_b$ là một song ánh. Các ánh xạ $\theta^{-1}_{b,U}$, với U là một tập mở liên thông khác rỗng của B và b là một điểm bất kỳ của b, định nghĩa một cấu xạ của các tiền bó (đối với cơ sở các tập mở liên thông của B) từ bó hằng kiểu thớ ${F'}^F$ vào bó $\mathscr{M}$. Theo điều vừa chứng minh, cấu xạ này cảm sinh một song ánh trên các thớ; do đó nó là một đẳng cấu.

Các khẳng định liên quan đến bó $\mathscr{I}$ được chứng minh tương tự.

#### Hệ quả 1 {#ta-i-s4-prop-12-cor-1 .statement tag=01Q3}

Cho B là một không gian tôpô và A là một không gian con của B. Giả sử các không gian A và B liên thông địa phương. Cho E và $E'$ là các phủ của B. Khi đó các cấu xạ chính tắc $\psi :\mathscr{M}$or$_B(E; E')_A\rightarrow \mathscr{M}$or$_A(E_A; E'_A)$ và $\psi ':\mathscr{I}$som$_B(E; E')_A\rightarrow$ $\mathscr{I}$som$_A(E_A; E'_A)$ (I, p. 45, ví dụ 4) là các đẳng cấu.

Với mọi điểm $a\in A$, từ mệnh đề trước và từ ví dụ 2 của I, p. 63, áp dụng cho các không gian $\{a\}$, A, B và các phép nhúng chính tắc, suy ra rằng cấu xạ chính tắc $\psi$ cảm sinh, khi chuyển qua các thớ, đồng nhất của $E^{E'_a}_a$. Do đó nó là một đẳng cấu. Việc $\psi '$ là một đẳng cấu được chứng minh tương tự.

#### Hệ quả 2 {#ta-i-s4-prop-12-cor-2 .statement tag=01Q4}

Cho B là một không gian tôpô và A là một không gian con của B. Giả sử các không gian A và B liên thông địa phương và cặp $(B,A)$ có tính chất (PCV) của I, p. 37. Cho E và $E'$ là các phủ của B, và ký hiệu các phép chiếu của chúng lần lượt là $p$ và $p'$. Cho

$g:\overset{-1}{p}(A)\rightarrow (^-{p'}^1)(A)$ là một cấu xạ A ( resp. một đẳng cấu A). Khi đó tồn tại một lân cận U của A trong B và một cấu xạ U ( resp. một

đẳng cấu U) $f:\overset{-1}{p}(U)\rightarrow (\overset{-1}{p}')(U)$ sao cho $f_A=g$.

Ta giữ nguyên ký hiệu của hệ quả 1. Theo chính hệ quả đó, một cấu xạ A $g: E_A\rightarrow E'_A$ được đồng nhất với một tiết diện $s_0$ trên A của không gian étalé $E_{\mathscr{M}}$ liên kết với $\mathscr{M}$. Theo giả thiết đặt trên cặp $(B,A)$ và bổ đề 3 của I, p. 39, tồn tại một lân cận mở U của A trong B và một tiết diện liên tục $s$ của $E_{\mathscr{M}}$ trên U mở rộng $s_0$. Tiết diện $s`

Trường hợp $g$ là một A-đẳng cấu được xử lý tương tự bằng cách xét, thay cho bó $\mathscr{M}$, bó $\mathscr{I}$.

## BÀI TẬP {#ta-i-s4-exercises}

Xem [các bài tập cho § 4](exercises/s4/).
