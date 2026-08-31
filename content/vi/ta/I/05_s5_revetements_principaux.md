---
book: ta
book_title: Topologie algébrique
chapter: I
chapter_title: REVÊTEMENTS
section: 5
section_title: Revêtements principaux
lang: vi
source: ta-i-iv-fr
book_pages: TA I.91-TA I.119, TA I.147-TA I.149
pdf_pages: 0107-0135, 0163-0165
extraction: native
subsections:
    - "no": 1
      title: Espaces fibrés principaux
      page: 91
      pdf_page: 107
    - "no": 2
      title: Revêtements principaux
      page: 97
      pdf_page: 113
    - "no": 3
      title: Opérations propres et libres de groupes discrets
      page: 99
      pdf_page: 115
    - "no": 4
      title: Revêtements galoisiens
      page: 101
      pdf_page: 117
    - "no": 5
      title: Espaces fibrés associés
      page: 104
      pdf_page: 120
    - "no": 6
      title: Revêtements associés
      page: 108
      pdf_page: 124
    - "no": 7
      title: Espaces fibrés principaux définis par des cocycles
      page: 114
      pdf_page: 130
statements: 58
exercises: 4
content_sha256: 1b83c1cd7541d7e619984eecf8add07e1672e2f405223585c5f9aad797a490d0
translated_from: content/en-mt/ta/I/05_s5_revetements_principaux.md
source_lang: en-mt
translation_method: machine
source_content_sha256: b2aa9fda240c14a456e34d8b7b5d0b17468650d8303a0134aea07d1f327022fd
translation_model: gpt-5-6-mini, gpt-5-6
translation_run: translate-vi-5833cdb6
glossary_version: 34
glossary_terms_sha256: aaf6cbef7dd07dc7c9ba257f59cc0c46b9cf3517a7d0eb26d102028b28c5e2bb
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 5. KHÔNG GIAN SỢI CHÍNH

### 1. Không gian sợi chính

#### Định nghĩa 1 {#ta-i-s5-def-1 .statement tag=01Q5}

Cho G là một nhóm tôpô và B là một không gian tôpô. Một không gian sợi chính (phải) với cơ sở B và nhóm G là một không gian B $(E, p)$ được trang bị một phép toán phải của G trên E (A, I, p. 50) có tính chất sau:

(FP) Với mọi điểm $b$ của B, tồn tại một lân cận U của $b$ và một

đẳng cấu U $f: U\times G\rightarrow \overset{-1}{p}(U)$ sao cho với mọi $u\in U$

và $g,g'\in G$, ta có $f(u, gg') =f(u, g)\cdot g'$.

Thay vì nói rằng $(E, p)$ là một không gian sợi chính với cơ sở B và nhóm G, đôi khi người ta nói rằng bộ bốn $(E,G,B, p)$ là một phép phân thớ chính (xem VAR, R, § 6), hoặc, theo lối lạm dụng, rằng ánh xạ $p: E\rightarrow B$ là một phép phân thớ chính với cơ sở B và nhóm G.

Khi không thể có sự nhầm lẫn về cơ sở B, nhóm G và phép toán của G trên E, ta sẽ đơn giản nói rằng $(E, p)$ là một không gian sợi chính.

Cho G là một nhóm tôpô. Cho $(E, p)$ là một không gian B được trang bị một phép toán trái của G. Nếu, đối với phép toán phải của nhóm $G^{\circ}$ đối với phép toán đã cho (A, I, p. 50), $(E, p)$ là một không gian sợi chính phải với nhóm $G^{\circ}$, thì người ta nói rằng $(E, p)$ là một không gian sợi chính trái với nhóm G.

Một không gian sợi chính là một không gian sợi địa phương tầm thường (I, p. 68, def. 1).

Từ tính chất (FP) suy ra rằng nhóm G tác động liên tục (TG, III, p. 9) và tự do trên E, và các quỹ đạo của phép toán này là các sợi của không gian B $(E, p)$. Ánh xạ $p': E/G\rightarrow B$ suy ra từ $p$ là liên tục và song ánh. Lại từ tính chất (FP), ánh xạ $p$ là mở (TG, I, p. 30, prop. 2 và p. 26, prop. 5); do đó $p'$ là một phép đồng phôi (TG, I, p. 32, prop. 3).

Cho $(E, p)$ và $(E', p')$ là các không gian sợi chính với cơ sở B và nhóm G. Một ánh xạ $f: E\rightarrow E'$ được gọi là một cấu xạ của các không gian sợi chính (với cơ sở B và nhóm G) nếu $f$ là một cấu xạ B và nếu ta có $f(x\cdot g) =f(x)\cdot g$ với mọi $x\in E$ và mọi $g\in G$. Cho $(E'', p'')$ là một không gian sợi chính với cơ sở B và nhóm G. Nếu $f: E\rightarrow E'$ và $g: E'\rightarrow E''$ là các cấu xạ của các không gian sợi chính, thì ánh xạ $g\circ f: E\rightarrow E''$ là một cấu xạ của các không gian sợi chính. Phù hợp với các định nghĩa tổng quát (E, IV, p. 11), ta có thể lấy làm các cấu xạ của cấu trúc không gian sợi chính với cơ sở B và nhóm G các cấu xạ đã định nghĩa ở trên. Ta ký hiệu $\mathscr{C}_B^G(E; E')$ là tập hợp các cấu xạ của các không gian sợi chính từ $(E, p)$ vào $(E', p')$.

Một không gian sợi chính tầm thường với cơ sở B và nhóm G là không gian B $(B\times G$, pr$_1)$ được trang bị luật phép toán phải của G trên $B\times G$ xác định bởi $(b, g)\cdot h= (b, gh)$.

Một không gian sợi chính $(E, p)$ với cơ sở B và nhóm G được gọi là tầm thường hóa được nếu tồn tại một đẳng cấu của $(E, p)$ lên không gian sợi chính tầm thường $(B\times G$, pr$_1)$; một đẳng cấu như vậy được gọi là một phép tầm thường hóa của không gian sợi chính $(E, p)$. Tính chất (FP) phát biểu rằng tồn tại một phủ mở $(U_i)_{i\in I}$ của B sao cho, với mọi $i\in I$, không gian $U_i$ $(\overset{-1}{p}(U_i), p|U_i)$, được trang bị phép toán phải của G suy ra từ phép toán của G trên E, là một không gian sợi chính tầm thường hóa được.

#### Ví dụ 1 {#ta-i-s5-n1-exa-1 .statement tag=01Q6}

Cho $(E, p)$ là một không gian sợi chính với cơ sở B và nhóm G, và cho A là một không gian con của B. Không gian con $E_A=\overset{-1}{p}(A)$ của E ổn định đối với phép toán của G, và ánh xạ $p_A: E_A\rightarrow A$ biến nó thành một không gian sợi chính với cơ sở A và nhóm G. Người ta nói rằng $(E_A, p_A)$ là không gian sợi chính cảm sinh bởi $(E, p)$ trên A.

#### Ví dụ 2 {#ta-i-s5-n1-exa-2 .statement tag=01Q7}

Cho $(E, p)$ là một không gian sợi chính với cơ sở B và nhóm G; cho $(E', p')$ là một không gian sợi chính với cơ sở $B'$ và nhóm $G'$. Ta định nghĩa một luật phép toán ở bên phải của nhóm $G\times G'$ trên không gian $E\times E'$ bằng cách đặt $(x, x')\cdot (g, g') = (x\cdot g, x'\cdot g')$ với $x\in E,x'\in E',g\in G$ và $g'\in G'$; phép toán này là liên tục. Cho U là một tập con mở của B và $f: U\times G\rightarrow \overset{-1}{p}(U)$ là một sự tầm thường hóa của không gian U $(\overset{-1}{p}(U), p_U)$;

cho $U'$ là một tập con mở của $B'$ và $f': U'\times G'\rightarrow (^-{p'}^1)(U')$ là một sự tầm thường hóa của không gian $U'$ ($(^-{p'}^1)(U'), p'_U$). Ánh xạ $((b, b'),(g, g'))\mapsto$ $(f(b, g), f'(b', g'))$ là một đẳng cấu $(U\times U')$ $f''$ của $(U\times U')\times (G\times G')$

lên $\overset{-1}{p}(U)\times (^-{p'}^1)(U')$ và ta có

$$
f''((b, b'),(gh, g'h')) = (f(b, gh), f'(b', g'h')) =f''((b, b'),(g, g'))\cdot (h, h')
$$

Suy ra rằng không gian $(B\times B')$ $E\times E'$, được trang bị luật phép toán của $G\times G'$ đã định nghĩa ở trên, là một không gian sợi chính, được gọi là tích của các không gian sợi chính E và $E'$.

#### Ví dụ 3 {#ta-i-s5-n1-exa-3 .statement tag=01Q8}

Đặc biệt, khi $B = B'$, không gian B $E\times_BE'$ được đồng nhất với không gian sợi chính với nhóm $G\times G'$ cảm sinh bởi $E\times E'$ trên đường chéo $\Delta_B$ của $B\times B$. Được trang bị cấu trúc này của không gian sợi chính, không gian B $E\times_BE'$ được gọi là tích sợi của các không gian sợi chính E và $E'$.

#### Ví dụ 4 {#ta-i-s5-n1-exa-4 .statement tag=01Q9}

Cho E là một không gian sợi chính với cơ sở B và nhóm G và cho F là một không gian tôpô. Không gian $(B\times F)$ $E\times F$ được trang bị luật phép toán $(x, y)\cdot g= (x\cdot g, y)$, với $x\in E,y\in F$ và $g\in G$, là một không gian sợi chính với nhóm G. Đây là trường hợp riêng của Ví dụ 2, trong đó $p'$ là ánh xạ đồng nhất của F và $G'$ là một nhóm thu gọn về phần tử đơn vị.

#### Ví dụ 5 {#ta-i-s5-n1-exa-5 .statement tag=01QA}

Cho B là một không gian tôpô và $(E, p)$ là một không gian sợi chính với cơ sở B và nhóm G. Cho $B'$ là một không gian tôpô và $f: B'\rightarrow B$ là một ánh xạ liên tục. Nhóm G tác động ở bên phải trên tích sợi $B'\times_BE$ bởi luật $(b', x)\cdot g= (b', x\cdot g)$, với $b'\in B',x\in E$ và $g\in G$. Phép toán này là liên tục và tự do; các quỹ đạo là các thớ của ánh xạ pr$_1: B'\times_BE\rightarrow B'$. Suy ra từ các Ví dụ 1 và 4 ở trên và Nhận xét 2 của I, p. 16 rằng không gian $B'$ $B'\times_BE$ là một không gian sợi chính với nhóm G. Nó được gọi là không gian sợi chính suy ra từ $(E, p)$ bởi thay đổi cơ sở $f$, hoặc cũng là ảnh ngược của $(E, p)$ bởi $f$.

#### Mệnh đề 1 {#ta-i-s5-prop-1 .statement tag=01QB}

Mọi cấu xạ của các không gian sợi chính đều là một đẳng cấu.

Cho $f: B\times G\rightarrow B\times G$ là một cấu xạ của không gian sợi chính tầm thường $(B\times G$, pr$_1)$ vào chính nó và cho $\varphi : B\times G\rightarrow G$ là ánh xạ liên tục pr$_2\circ f$, sao cho $f(b, g) = (b, \varphi (b, g))$. Với mọi $b\in B$ và mọi $g,h\in G$, ta có $\varphi (b, gh) =\varphi (b, g)\cdot h$, do đó $\varphi (b, g) =\varphi (b, e)\cdot g$, trong đó $e$ ký hiệu phần tử đơn vị của G. Cấu xạ $f$ vì vậy là một đẳng cấu mà cấu xạ nghịch đảo $f^{-1}$ được xác định bởi $f^{-1}(b, g) =$ $(b, \varphi (b, e)^{-1}g)$ với $(b, g)\in B\times G$.

Bây giờ cho E và $E'$ là các không gian sợi chính và cho $f: E\rightarrow E'$ là một cấu xạ của các không gian sợi chính. Theo tính chất (FP), với mọi điểm $b\in B$, tồn tại một lân cận mở U của $b$ sao cho các không gian sợi chính $E_U$ và $E'_U$ là tầm thường hóa được. Bằng cách chuyển qua các không gian con, $f$ cảm sinh một cấu xạ $f_U: E_U\rightarrow E'_U$ của các không gian sợi chính; theo điều đã chứng minh ở trên, cấu xạ này $f_U$ là một đẳng cấu. Đặc biệt, $f_b: E_b\rightarrow E'_b$ là một song ánh. Khi đó tồn tại một ánh xạ duy nhất $g: E'\rightarrow E$ cảm sinh song ánh $f_b^{-1}$ bằng cách chuyển qua các không gian con. Theo Mệnh đề 4 của I, p. 19, ánh xạ $g$ là liên tục, do đó $f$ là một đẳng cấu của các không gian sợi chính.

#### Hệ quả {#ta-i-s5-n1-cor-1 .statement tag=01QC}

Cho G là một nhóm tôpô, $(E, p)$ và $(E', p')$ là các không gian sợi chính của nhóm G và có các cơ sở lần lượt là B và $B'$. Cho $f: B'\rightarrow$ B và $f': E'\rightarrow$ E là các ánh xạ liên tục sao cho $p\circ f'=f\circ p'$ và sao cho, với mọi $x'\in E'$ và mọi $g\in G$, $f'(x'\cdot g) =f'(x')\cdot g$. Khi đó bình phương

${E'}^{f'}$ E

$p'p$

${B'}^f$ B

là một bình phương Descartes.

Thật vậy, ánh xạ $h: E'\rightarrow B'\times_BE$ xác định bởi $h(x') =$ $(p'(x'), f'(x'))$ với $x'\in E'$, là một $B'$-cấu xạ của các phủ chính, do đó là một đẳng cấu; hơn nữa pr$_2\circ h=f'$, do đó có kết quả (I, p. 8, Mệnh đề 2).

Dưới các giả thiết của hệ quả trước, đôi khi người ta nói rằng $f'$ là một $f$-cấu xạ của các không gian sợi chính.

#### Mệnh đề 2 {#ta-i-s5-prop-2 .statement tag=01QD}

Cho $(E, p)$ là một không gian thớ chính với cơ sở B và nhóm G, và cho $\varepsilon$ là tiết diện $b\mapsto (b, e)$ của không gian thớ chính tầm thường $(B\times G$, pr$_1)$, trong đó $e$ ký hiệu phần tử đơn vị của G. Ánh xạ $h\mapsto h\circ \varepsilon$ là một song ánh của $\mathscr{C}_B^G(B\times G; E)$ lên tập hợp $\mathscr{S}(B; E)$ các tiết diện liên tục của $p$. Song ánh ngược gán cho một tiết diện liên tục $s$ của $p$ cấu xạ B $(b, g)\mapsto s(b)\cdot g$.

#### Hệ quả {#ta-i-s5-n1-cor-2 .statement tag=01QE}

Một không gian thớ chính là tầm thường hóa được khi và chỉ khi nó có một tiết diện liên tục.

#### Mệnh đề 3 {#ta-i-s5-prop-3 .statement tag=01QF}

Cho E và B là các không gian tôpô, $p: E\rightarrow B$ là một ánh xạ liên tục và G là một nhóm tôpô tác động bên phải trên E. Các điều kiện sau là tương đương:

(i) Được trang bị ánh xạ $p$, E là một không gian thớ chính với cơ sở B và nhóm G;

(ii) Với mọi $x\in E$ và mọi $g\in G$, ta có $p(x\cdot g) =p(x)$, ánh xạ $\theta : (x, g)\mapsto (x, x\cdot g)$ là một đồng phôi của $E\times G$ lên $E\times_BE$ và mọi điểm của B đều có một lân cận trên đó tồn tại một tiết diện liên tục của ánh xạ $p$.

(i)$\Rightarrow$(ii) : Giả sử rằng $(E, p)$ là một không gian thớ chính. Nhóm G tác động liên tục và tự do trong E, với các thớ của $p$ là các quỹ đạo. Do đó ánh xạ $\theta$ là song ánh và liên tục. Chính xác hơn, nếu $E\times_BE$ được trang bị phép toán của G xác định bởi $(x, y)\cdot g= (x, y\cdot g)$, ánh xạ $\theta$ là một cấu xạ E của không gian thớ chính tầm thường $E\times G$ vào không gian thớ chính $(E\times_BE\rightarrow E$, pr$_1)$ (ví dụ 5), do đó là một đẳng cấu (mệnh đề 1). Các khẳng định khác của (ii) suy ra ngay lập tức từ định nghĩa.

(ii)$\Rightarrow$(i) : Đặt $\varphi =$ pr$_2\circ \theta^{-1}$, sao cho, với mọi $(x, y)\in$ $E\times_BE$, ta có

$$
\theta^{-1}(x, y) = (x, \varphi (x, y)) \tag{1}
$$

Ánh xạ $\varphi : E\times_BE\rightarrow G$ là liên tục và, với $(x, y)\in E\times_BE$, phần tử $\varphi (x, y)$ là phần tử duy nhất $g$ của G sao cho $y=x\cdot g$. Cho $b$ là một điểm của B; cho U là một lân cận của $b$ và cho $s$ là một tiết diện liên tục của $p$ trên U. Với $(u, g)\in U\times G$, đặt $f(u, g) =s(u)\cdot$ $g$; ánh xạ $f$ là một cấu xạ U của $U\times G$ vào $\overset{-1}{p}(U)$. Với $y\in \overset{-1}{p}(U)$, đặt $f'(y) = (p(y), \varphi (s(p(y)), y))$. Ánh xạ $f'$ là một cấu xạ U của $\overset{-1}{p}(U)$ vào $U\times G$. Ta có

$$
(f\circ f')(y) =s(p(y))\cdot \varphi (s(p(y)), y) =y
$$

Mặt khác, với $(u, g)\in U\times G$, ta có

$$
(f'\circ f)(u, g) =f'(s(u)\cdot g) = (u, \varphi (s(u), s(u)\cdot g)) = (u, g)
$$

Do đó $f$ là một đẳng cấu U. Suy ra $(E, p)$ là một không gian bó chính với cơ sở B và nhóm G.

#### Nhận xét 1 {#ta-i-s5-n1-rem-1 .statement tag=01QG}

Cho $(E, p)$ là một không gian bó chính với cơ sở B và nhóm G. Với ký hiệu của mệnh đề 3, ánh xạ $\theta^{-1}: E\times_BE\rightarrow E\times G$ là một phép tầm thường hóa của không gian bó chính pr$_1: E\times_BE\rightarrow E$. Người ta gọi $\theta^{-1}$ là phép tầm thường hóa chính tắc của không gian bó chính này.

#### Hệ quả 1 {#ta-i-s5-prop-3-cor-1 .statement tag=01QH}

Cho G là một nhóm tôpô tác động liên tục bên phải trên một không gian tôpô E. Các điều kiện sau là tương đương:

(i) Không gian quỹ đạo $E/G$ là Hausdorff và không gian E, được trang bị ánh xạ chính tắc $p: E\rightarrow E/G$, là một không gian bó chính với nhóm G;

(ii) Nhóm G tác động đúng (TG, III, p. 27) và tự do trên E, và mọi điểm của $E/G$ đều có một lân cận trên đó tồn tại một tiết diện liên tục của ánh xạ $p$.

Đặt $B = E/G$. Dưới mỗi giả thiết (i) và (ii), nhóm G tác động liên tục và tự do trên E, do đó ánh xạ $\theta : (x, g)\mapsto (x, x\cdot g)$ là một song ánh liên tục từ $E\times G$ lên $E\times_BE$. Ta đặt mình dưới giả thiết này và ký hiệu $\varphi : E\times_BE\rightarrow G$ là ánh xạ pr$_2\circ \theta^{-1}$. Theo công thức (1), để $\theta$ là một đồng phôi, điều kiện cần và đủ là ánh xạ $\varphi$ liên tục. Mặt khác, vì quan hệ tương đương xác định bởi G là mở (TG, III, p. 10, bổ đề 2), để không gian $E/G$ là Hausdorff, điều kiện cần và đủ là đồ thị $E\times_BE$ của quan hệ tương đương này đóng trong $E\times E$ (TG, I, p. 55, mệnh đề 8). Cuối cùng (TG, III, p. 31, mệnh đề 6), để G tác động đúng trên E, điều kiện cần và đủ là $E\times_BE$ đóng trong $E\times E$ và ánh xạ $\varphi$ liên tục. Tính tương đương của các điều kiện (i) và (ii) khi đó suy ra từ mệnh đề 3.

#### Hệ quả 2 {#ta-i-s5-prop-3-cor-2 .statement tag=01QI}

Cho G là một nhóm tôpô, H là một nhóm con của G, và $p: G\rightarrow G/H$ là ánh xạ chính tắc. Nếu ánh xạ $p$ có một tiết diện liên tục trên một tập mở khác rỗng của $G/H$, thì ánh xạ $p$ biến G thành một không gian bó chính với cơ sở $G/H$ và nhóm H.

Bởi các phép tịnh tiến trái, mọi điểm của $G/H$ đều có một lân cận trên đó ánh xạ $p$ có một tiết diện liên tục. Mặt khác, với $(g, g')$ thuộc $G\times G$, đặt $\varphi (g, g') =$ $g^{-1}g'$. Nếu $p(g) =p(g'),\varphi (g, g')$ thuộc H. Ánh xạ $(g, g')\mapsto$ $(g, \varphi (g, g'))$ từ $G\times_{G/H}G$ vào $G\times H$ là liên tục và là ánh xạ nghịch đảo của ánh xạ liên tục $\theta : G\times H\rightarrow G\times_{G/H}G$ được xác định bởi $\theta (g, h) = (g, gh)$, do đó có hệ quả.

#### Nhận xét 2 {#ta-i-s5-n1-rem-2 .statement tag=01QJ}

Tình huống này đặc biệt xuất hiện khi G là một nhóm Lie thực, có chiều hữu hạn, đếm được tại vô cực, tác động bắc cầu và giải tích trên một đa tạp giải tích X. Nếu lấy H là nhóm ổn định của một điểm của X, thì ánh xạ $p$ là một phép chìm từ G lên không gian Lie thuần nhất $G/H$, đẳng cấu với X (LIE, III, p. 109, hệ quả). Do đó nó có các tiết diện địa phương (VAR, p. 50).

### 2. Các phủ chính

#### Định nghĩa 2 {#ta-i-s5-def-2 .statement tag=01QK}

Cho B là một không gian tôpô và G là một nhóm. Trang bị cho G tôpô rời rạc. Một không gian bó chính với cơ sở B và nhóm G được gọi là một phủ chính của B với nhóm G.

Thuật ngữ này là chính đáng, vì một B-không gian như vậy là một phủ của B.

Một phủ chính với nhóm G của một không gian tôpô khác rỗng có một bậc, bằng Card G.

#### Mệnh đề 4 {#ta-i-s5-prop-4 .statement tag=01QL}

Cho B là một không gian tôpô, $(E, p)$ là một B-không gian, và G là một nhóm tôpô rời rạc tác động bên phải trên E. Các khẳng định sau là tương đương:

(i) B-không gian E là một phủ chính với nhóm G;

(ii) Với mọi $g\in G$ và mọi $x\in E$, ta có $p(x\cdot g) =p(x)$, ánh xạ $p$ cảm sinh một đồng phôi từ $E/G$ lên B, và ánh xạ $\theta : (x, g)\mapsto (x, x\cdot g)$ là một đồng phôi từ $E\times G$ lên $E\times_BE$;

(iii) Nhóm G tác động liên tục và tự do trên E, ánh xạ $p$ là étale, và các thớ của nó là các quỹ đạo của G.

(i)$\Rightarrow$(ii) : Điều này suy ra từ I, p. 91 và từ mệnh đề 3 của I, p. 94.

(ii)$\Rightarrow$(iii): Theo giả thiết (ii), luật tác động của G là liên tục, và ánh xạ $p$ là toàn ánh và mở (TG, III, p. 10, bổ đề 2). Cho $x\in E$; ánh xạ $\theta$ cảm sinh một song ánh từ $\{x\} \times G$ lên $\{x\} \times$ $\overset{-1}{p}(p(x))$, do đó nhóm G tác động tự do và các quỹ đạo của nó là các thớ của $p$. Nếu $e$ là phần tử đơn vị của G, đường chéo của $E\times_BE$ là ảnh của $E\times  \{e\}$ qua đồng phôi $\theta$. Vì nhóm G rời rạc, tập hợp $\{e\}$ là mở trong G, do đó đường chéo $\Delta_E$ là mở trong $E\times_BE$. Theo mệnh đề 7 của I, p. 31, ánh xạ $p$ là étale.

(iii)$\Rightarrow$(i): Vì mọi thớ của $p$ đều là một quỹ đạo của phép toán của G trên E, ánh xạ $p$ là toàn ánh. Vì ánh xạ $p$ là étale, với mỗi điểm $b$ của B, tồn tại một lân cận mở U của $b$ và một tiết diện liên tục $s$ của $p$ trên U. Tập hợp $s(U)$ là mở trong E và $s$ cảm sinh một đồng phôi từ U lên $s(U)$ (I, p. 30, hệ quả 3). Với mọi $g\in G$, tập hợp $s(U)\cdot g$ là mở trong E và hợp của các tập hợp $s(U)\cdot g$, với mọi $g\in G$, bằng $\overset{-1}{p}(U)$. Nếu $g$ và $g'$ là hai phần tử phân biệt của G, các tập hợp $s(U)\cdot g$ và $s(U)\cdot g'$ rời nhau, vì G tác động tự do trên E. Do đó ánh xạ $f: U\times G\rightarrow$ $\overset{-1}{p}(U)$ xác định bởi $f(u, g) =s(u)\cdot g$ với $(u, g)\in U\times G$ là một đồng phôi từ $U\times G$ lên $\overset{-1}{p}(U)$, tương thích với các phép toán phải của G. Theo định nghĩa, E do đó là một phủ chính của B với nhóm G.

#### Ví dụ 1 {#ta-i-s5-n2-exa-1 .statement tag=01QM}

Cho E là một không gian tôpô, G là một nhóm tôpô rời rạc tác động liên tục và tự do trên E ở bên phải. Để ánh xạ chính tắc $p: E\rightarrow E/G$ làm cho E trở thành một phủ chính của $E/G$, điều kiện cần và đủ là nó étale (điều kiện (iii) của mệnh đề 4). Chẳng hạn, giả sử tồn tại một không gian tôpô X và một ánh xạ étale $q: E\rightarrow X$ tương thích với phép toán của G trên E; khi đó E là một phủ chính của $E/G$. Thật vậy, ký hiệu $q': E/G\rightarrow X$ là ánh xạ suy ra từ $q$; ta có $q=q'\circ p$, do đó $p$ là étale theo mệnh đề 6, d) của I, p. 29.

#### Ví dụ 2 {#ta-i-s5-n2-exa-2 .statement tag=01QN}

Cho $q: E\rightarrow$ X là một ánh xạ étale và tách được. Nhóm Aut$_X(E)$, được trang bị tôpô rời rạc, tác động liên tục lên E ở bên trái. Nếu không gian E liên thông, phép toán này là tự do (I, p. 34, hệ quả 2). Ký hiệu G là nhóm Aut$_X(E)^{\circ}$ và trang bị cho E phép toán phải đối với phép toán của Aut$_X(E)$. Theo ví dụ trên, không gian E, được trang bị ánh xạ chính tắc $p: E\rightarrow E/G$, là một phủ chính với nhóm G.

### 3. Các phép toán thực sự và tự do của các nhóm rời rạc

#### Định lý 1 {#ta-i-s5-thm-1 .statement tag=01QO}

Cho G là một nhóm rời rạc tác động liên tục ở bên phải trên một không gian tôpô E. Giả sử mỗi điểm của E có một lân cận U sao cho $U\cap (U\cdot g) =\emptyset$ với mọi phần tử $g$ của G khác phần tử đơn vị. Khi đó ánh xạ chính tắc $p: E\rightarrow E/G$ làm cho E trở thành một phủ chính của $E/G$ với nhóm G.

Phép toán của G trên E là tự do theo giả thiết, nên chỉ cần chứng minh rằng ánh xạ $p$ là étale (I, p. 98, ví dụ 1). Cho $x$ là một điểm của E và U là một lân cận mở của $x$ sao cho $U\cap U\cdot g=\emptyset$ với mọi phần tử $g$ của G phân biệt với phần tử đơn vị. Ánh xạ $p$ là mở (TG, III, p. 10, bổ đề 2) và cảm sinh một ánh xạ đơn ánh, liên tục và mở từ U lên $p(U)$, do đó là một đồng phôi, chứng tỏ rằng ánh xạ $p$ là étale.

#### Ví dụ 1 {#ta-i-s5-n3-exa-1 .statement tag=01QP}

Cho $n$ là một số nguyên $\geqslant 0$, cho $\mathbf{P}_n(\mathbf{R})$ là không gian xạ ảnh có chiều $n$ (TG, VI, p. 13) và cho $\mathbf{S}_n$ là mặt cầu đơn vị của $\mathbf{R}^{n+1}$ (TG, VI, p. 9). Ánh xạ chính tắc của $\mathbf{S}_n$ lên $\mathbf{P}_n(\mathbf{R})$ biến $\mathbf{S}_n$ thành một phủ chính với nhóm $\{1,-1\}$, nhóm này tác động bằng các phép vị tự; các quỹ đạo là các cặp điểm đối nhau qua tâm.

#### Ví dụ 2 {#ta-i-s5-n3-exa-2 .statement tag=01QQ}

Mọi phủ có bậc 2 đều có duy nhất một cấu trúc phủ chính với nhóm $\mathbf{Z}/2\mathbf{Z}$.

#### Ví dụ 3 {#ta-i-s5-n3-exa-3 .statement tag=01QR}

Cho X là một đa tạp khả vi tách được, địa phương có số chiều hữu hạn trên $\mathbf{R}$, và cho $\widetilde{X}$ là đa tạp các định hướng của bó tiếp xúc của X (VAR, R, 10.2.4). Không gian $\widetilde{X}$, được trang bị phép chiếu chính tắc lên X, là một phủ chính của X với nhóm $\{1,-1\}$.

#### Hệ quả 1 {#ta-i-s5-thm-1-cor-1 .statement tag=01QS}

Cho G là một nhóm tôpô rời rạc tác động liên tục bên phải trên một không gian tôpô E. Các điều kiện sau là tương đương:

(i) Nhóm G tác động đúng và tự do trên E;

(ii) Không gian $E/G$ là tách được và không gian E là một phủ chính với cơ sở $E/G$ và nhóm G.

Hơn nữa, dưới các điều kiện này, không gian E là tách được.

Giả sử điều kiện (i) được thỏa mãn. Khi đó các không gian E và $E/G$ là tách được (TG, III, p. 29, mệnh đề 3) và với mọi $x\in E$ tồn tại một lân cận mở U của $x$ trong E sao cho $U\cap (U\cdot g) =\emptyset$ với mọi phần tử $g$ của G khác với phần tử đơn vị (TG, III, p. 32, mệnh đề 8). Theo Định lý 1, khi đó điều kiện (ii) được thỏa mãn.

Hàm ý (ii)$\Rightarrow$(i) suy ra từ hệ quả 1 của I, p. 96.

#### Hệ quả 2 {#ta-i-s5-thm-1-cor-2 .statement tag=01QT}

Cho G là một nhóm tôpô và H là một nhóm con rời rạc của G. Cho H tác động trên G bằng các phép tịnh tiến phải. Khi đó ánh xạ chính tắc của G vào không gian $G/H$ các lớp trái modulo H trang bị cho G một cấu trúc phủ chính của $G/H$ với nhóm H.

Cho V là một lân cận của phần tử đơn vị $e$ của G sao cho $H\cap V =\{e\}$. Tồn tại một lân cận mở U của $e$ trong G sao cho $U^{-1}\cdot U\subset V$ (TG, III, p. 3) và do đó $U\cap U\cdot h=\emptyset$ với mọi $h\in H,h=\not e$. Hệ quả 2 của I, p. 100 do đó suy ra từ định lý 1.

#### Ví dụ 4 {#ta-i-s5-n3-exa-4 .statement tag=01QU}

Được trang bị ánh xạ chính tắc của $\mathbf{R}$ lên $\mathbf{T}=\mathbf{R}/\mathbf{Z}$ (TG, V, p. $2$)$,\mathbf{R}$ là một phủ chính của $\mathbf{R}/\mathbf{Z}$ với nhóm $\mathbf{Z}$.

#### Nhận xét 1 {#ta-i-s5-n3-rem-1 .statement tag=01QV}

Cho G là một nhóm tôpô tách được, K một nhóm con compact của G và H một nhóm con rời rạc của G. Nhóm G tác động liên tục và đúng bên phải trên không gian $K\backslash G$ các lớp phải modulo K (TG, III, p. 30, hệ quả). Vì nhóm H đóng trong G, nó cũng tác động đúng trên $K\backslash G$ (TG, III, p. 27, ví dụ 1). Hơn nữa, nếu $H\cap gKg^{-1}=\{e\}$ với mọi $g\in G$, thì nhóm H tác động tự do trên $K\backslash G$. Khi đó không gian $K\backslash G$ là một phủ chính với nhóm H của $K\backslash G/H$ theo hệ quả 1.

#### Hệ quả 3 {#ta-i-s5-thm-1-cor-3 .statement tag=01QW}

Cho G và $G'$ là các nhóm tôpô, và cho $\varphi : G\rightarrow G'$ là một đồng cấu liên tục, mở và toàn ánh. Giả sử hạt nhân H của $\varphi$ là rời rạc. Khi đó, đối với phép toán của H trên G bằng các phép tịnh tiến phải, $\varphi$ biến G thành một phủ chính của $G'$ với nhóm H.

Hơn nữa, nếu nhóm G liên thông, thì H được chứa trong tâm của G.

Đồng cấu $\varphi$ cảm sinh một đẳng cấu nhóm tôpô của $G/H$ lên $G'$ (TG, III, p. 16, prop. 24), do đó mệnh đề đầu tiên theo Hệ quả 2. Giả sử nhóm G liên thông. Với mọi $h\in H$, ánh xạ liên tục từ G vào H xác định bởi $g\mapsto ghg^{-1}$ là hằng, với giá trị $h$. Do đó nhóm H được chứa trong tâm của G.

#### Nhận xét 2 {#ta-i-s5-n3-rem-2 .statement tag=01QX}

Cho G và $G'$ là các nhóm tôpô và cho $\varphi : G\rightarrow G'$ là một đồng cấu mở liên tục. Nếu nhóm $G'$ liên thông, đồng cấu $\varphi$ là toàn ánh. Thực vậy, $\varphi (G)$ là một nhóm con mở, do đó đóng, của $G'$, và do đó bằng $G'$.

#### Nhận xét 3 {#ta-i-s5-n3-rem-3 .statement tag=01QY}

Cho G là một nhóm compact địa phương đếm được tại vô cực và cho $G'$ là một nhóm tôpô Hausdorff mà không gian nền của nó là một không gian Baire. Mọi đồng cấu toàn ánh liên tục từ G vào $G'$ đều là mở (TG, IX, p. 56, hệ quả và TG, III, p. 16, prop. 24).

#### Ví dụ 5 {#ta-i-s5-n3-exa-5 .statement tag=01QZ}

Với mọi số nguyên $n >$ 0, ký hiệu $\mu_n$ là nhóm các căn bậc $n$ của đơn vị trong $\mathbf{C}$ (A, V, p. 75). Ánh xạ $z\mapsto z^n$ biến $\mathbf{C}^*$ thành một phủ chính của $\mathbf{C}^*$ với nhóm $\mu_n$, nhóm này tác động trong $\mathbf{C}^*$ bằng phép nhân.

#### Ví dụ 6 {#ta-i-s5-n3-exa-6 .statement tag=01R0}

Được trang bị ánh xạ $z\mapsto e^{2\pi iz}$ (TG, VIII, p. 8, nhận xét), không gian $\mathbf{C}$ là một phủ chính của $\mathbf{C}^*$ với nhóm $\mathbf{Z}$. Ánh xạ $x\mapsto e^{2\pi ix}=\mathbf{e}(x)$ từ $\mathbf{R}$ lên $\mathbf{S}_1$ biến $\mathbf{R}$ thành một phủ chính của $\mathbf{S}_1$ với nhóm $\mathbf{Z}$.

### 4. Các phủ Galois

#### Định nghĩa 3 {#ta-i-s5-def-3 .statement tag=01R1}

Cho B là một không gian tôpô khác rỗng. Một phủ E của B được gọi là Galois nếu nó liên thông và nếu, với mọi điểm $b$ của B, phép toán của nhóm Aut$_B(E)$ gồm các tự đẳng cấu của E trên B trên thớ $E_b$ là bắc cầu.

Cho E là một phủ Galois của một không gian tôpô B và cho $p$ là phép chiếu của nó. Ánh xạ $p$ là toàn ánh (A, I, p. 56, def. 6); do đó không gian B là liên thông. Do đó, phủ $(E, p)$ có bậc khác không.

#### Mệnh đề 5 {#ta-i-s5-prop-5 .statement tag=01R2}

Cho B là một không gian tôpô khác rỗng và cho E là một phủ Galois của B. Ánh xạ $(h, x)\mapsto h(x)$ từ Aut$_B(E)\times E$ vào E là một luật phép toán phải của nhóm Aut$_B(E)^{\circ}$ trên E, biến E thành một phủ chính với nhóm Aut$_B(E)^{\circ}$.

Trang bị cho nhóm Aut$_B(E)^{\circ}$ tôpô rời rạc; khi đó luật phép toán $(h, x)\mapsto h(x)$ là liên tục. Phép toán này là tự do (I, p. 34, Hệ quả 2 của Mệnh đề 11). Vì E là một phủ Galois của B, các thớ của nó là các quỹ đạo của phép toán này. Theo Mệnh đề 4 của I, p. 97, E là một phủ chính với nhóm Aut$_B(E)^{\circ}$.

#### Định lý 2 {#ta-i-s5-thm-2 .statement tag=01R3}

Cho B là một không gian tôpô liên thông, cho E là một phủ của B, liên thông và khác rỗng. Các tính chất sau là tương đương:

(i) Phủ E là Galois;

(ii) Tồn tại một nhóm tôpô G rời rạc và một phép toán phải liên tục của G trên E biến E thành một phủ chính với nhóm G;

(iii) Phủ $E\times_BE$ của E xác định bởi phép chiếu pr$_1$ là tầm thường hóa được.

Khi các điều kiện này được thỏa mãn, ánh xạ chính tắc $G\rightarrow$ Aut$_B(E)^{\circ}$ xác định bởi phép toán của G là một đẳng cấu nhóm.

Nếu hơn nữa không gian B liên thông địa phương, các tính chất trên tương đương với tính chất sau:

(i$'$) Tồn tại một điểm $b$ của B sao cho phép toán của nhóm Aut$_B(E)$ trên thớ $E_b$ là bắc cầu.

Suy ra (i)$\Rightarrow$(ii) từ mệnh đề 5 và suy ra (ii)$\Rightarrow$(iii) từ nhận xét 1 của I, p. 95. Ta chứng minh (iii)$\Rightarrow$(i). Ký hiệu $p: E\rightarrow B$ là phép chiếu của phép phủ E. Vì B liên thông, phép phủ này có một bậc, và bậc này khác không vì E không rỗng. Cho $b$ là một điểm của B. Ta chứng minh rằng phép toán của Aut$_B(E)$ trên thớ $E_b$ là bắc cầu. Theo trên, thớ này không rỗng. Cho $x$ và $x'$ là các điểm của $E_b$. Các cấu xạ B $h: E\rightarrow E$ sao cho $h(x) =x'$ tương ứng song ánh với các tiết diện liên tục $s$ của ánh xạ pr$_1: E\times_BE\rightarrow E$ sao cho $s(x) = (x, x')$ (I, p. 9, prop. 3). Theo giả thiết (iii), một tiết diện như vậy tồn tại (I, p. 70, cor. 2) và là duy nhất (I, p. 34, cor. 1 of prop. 11) vì không gian E liên thông. Do đó, với mọi cặp $(x, x')\in E\times_BE$, tồn tại duy nhất một cấu xạ B $h: E\rightarrow E$ sao cho $h(x) =x'$. Nếu $h': E\rightarrow E$ là cấu xạ B duy nhất sao cho $h'(x') =x$, ta có $h'(h(x)) =x$ và $h(h'(x')) =x'$, do đó $h'\circ h=$ Id$_E$ và $h\circ h'=$ Id$_{E'}$. Điều này chứng minh rằng $h$ là một B-tự đẳng cấu của E. Vì vậy phép phủ E là Galois.

Ta đã chứng minh rằng các điều kiện (i), (ii), (iii) là tương đương. Giả sử chúng được thỏa mãn. Cho $\delta : G\rightarrow$ Aut$_B(E)$ là ánh xạ gán cho $g\in G$ tự đẳng cấu B $x\mapsto x\cdot g$ của E. Ánh xạ $\delta$ là một đồng cấu nhóm từ G vào Aut$_B(E)^{\circ}$. Vì G tác động tự do trên E, ánh xạ $\delta$ là đơn ánh. Cho $h\in$ Aut$_B(E)$, cho $x\in$ E và cho $g$ là phần tử duy nhất của G sao cho $x\cdot g=h(x)$. Các cấu xạ B $h$ và $\delta (g)$ trùng nhau tại $x$, do đó ở mọi nơi, vì không gian E liên thông (I, p. 34, cor. 1 of prop. 11), điều này chứng minh rằng $\delta$ là một đẳng cấu.

Bây giờ giả sử không gian B liên thông địa phương và ta chứng minh, dưới giả thiết (i$'$), rằng phép phủ E là Galois. Cho $E'$ là không gian thương của E theo phép toán phải của Aut$_B(E)^{\circ}$ và ký hiệu $q: E\rightarrow E'$ là ánh xạ chính tắc. Nó biến E thành một phép phủ toàn ánh của $E'$(I, p. 98, ví dụ 2); ánh xạ $p: E\rightarrow B$ xác định qua chuyển qua thương một ánh xạ liên tục $p': E'\rightarrow B$ sao cho $p'\circ q=p$. Vì không gian B liên thông địa phương, B-không gian $(E', p')$ là một phép phủ (I, p. 81, prop. 7). Theo giả thiết (i$'$), tồn tại một điểm $b$ của B sao cho thớ $E'_b$ có đúng một phần tử; vì không gian B liên thông, điều tương tự đúng với mọi điểm $b$ của B (I, p. 74, prop. 4), điều này chứng minh rằng E là một phép phủ Galois của B.

#### Mệnh đề 6 {#ta-i-s5-prop-6 .statement tag=01R4}

Cho B là một không gian tôpô và G là một nhóm. Cho $(E, p)$ là một phủ chính của B với nhóm G. Giả sử không gian B liên thông và liên thông địa phương. Cho $E_0$ là một thành phần liên thông của E và cho $G_0$ là nhóm con ổn định của G của $E_0$ (A, I, p. 51). Không gian B $(E_0, p|E_0)$ là một phủ chính đối với phép toán phải của $G_0$ trong $E_0$. Phủ này là Galois.

Vì không gian B liên thông địa phương, điều tương tự cũng đúng với E, do đó $E_0$ là một không gian con mở của E (TG, I, p. 85, prop. 11). Vì nó cũng đóng (TG, I, p. 83), không gian $E_0$ do đó là một phủ của B (I, p. 80, cor. 1). Vì B liên thông, phủ này có một bậc; vì $E_0$ không rỗng, mọi thớ của $p|E_0$ do đó đều không rỗng. Cho $x$ là một điểm của $E_0$, cho $x'\in E_0$ sao cho $p(x') =p(x)$; tồn tại một phần tử $g\in G$ sao cho $x\cdot g=x'$. Vì các thành phần liên thông $E_0$ và $E_0\cdot g$ khi đó có một điểm chung, chúng bằng nhau, do đó $g\in G_0$. Vậy nhóm $G_0$ tác động bắc cầu trên thớ của không gian B $E_0$ tại $p(x)$. Suy ra Mệnh đề 6.

#### Nhận xét {#ta-i-s5-n4-rem-1 .statement tag=01R5}

Nếu trong mệnh đề 6, không giả sử không gian B liên thông địa phương, có thể xảy ra rằng không gian $E_0$ không phải là một phủ của B (I, p. 147, exerc. 1).

### 5. Các không gian thớ liên kết

Cho E và F là các tập hợp và cho G là một nhóm tác động bên phải trên E và bên trái trên F. Nhóm G tác động bên phải trên tích $E\times F$ theo luật $(x, y)\cdot g= (x\cdot g, g^{-1}\cdot y)$, với $g\in G$, $(x, y)\in E\times F$. Tập thương của $E\times F$ theo phép toán này được ký hiệu là $E\times^GF$.

Khi E và F là các không gian tôpô, tập $E\times^GF$ được trang bị tôpô thương của tôpô trên $E\times F$. Ánh xạ chính tắc từ $E\times F$ lên $E\times^GF$ là liên tục. Nếu nhóm G tác động liên tục trong E và F, thì nó là mở.

Hơn nữa, cho $F'$ là một tập hợp trên đó G tác động bên trái và cho $h: F\rightarrow F'$ là một ánh xạ tương thích với các phép toán của G trên F và $F'$ (A, I, p. 50). Ánh xạ Id$_E\times h: E\times F\rightarrow E\times F'$ tương thích với các phép toán của G và định nghĩa, bằng cách chuyển qua các thương, một ánh xạ được ký hiệu là Id$_E\times^Gh$ từ $E\times^GF$ vào $E\times^GF'$.

Nếu $h: F\rightarrow F'$ là một ánh xạ liên tục (tương thích với các phép toán của G trên F và $F'$), ánh xạ Id$_E\times^Gh$ là liên tục (TG, I, p. 21, prop. 6).

#### Ví dụ 1 {#ta-i-s5-n5-exa-1 .statement tag=01R6}

Cho F là một không gian tôpô và cho G là một nhóm tôpô tác động liên tục bên trái trên F. Nếu không gian tôpô G được trang bị phép toán của G bởi các phép tịnh tiến phải, không gian $G\times^GF$ được đồng nhất một cách chính tắc với F theo cách sau. Các ánh xạ liên tục $\varphi : F\rightarrow G\times F$ và $\psi : G\times F\rightarrow$ F được định nghĩa bởi $\varphi (f) = (e, f)$ (trong đó $e$ ký hiệu phần tử đơn vị của G) và $\psi (g, f) =g\cdot f$ cảm sinh các ánh xạ liên tục $\overline{\varphi}: F\rightarrow G\times^GF$ và $\overline{\psi}: G\times^GF\rightarrow F$ là nghịch đảo của nhau.

#### Ví dụ 2 {#ta-i-s5-n5-exa-2 .statement tag=01R7}

Ví dụ 1 được tổng quát hóa như sau. Cho B và F là các không gian tôpô và cho G là một nhóm tôpô tác động liên tục bên trái trên F. Bằng cách chuyển qua các thương, ánh xạ từ $B\times F$ vào $(B\times G)\times F$ cho bởi $(b, f)\mapsto ((b, e), f)$ và ánh xạ từ $(B\times G)\times F$ vào $B\times F$ cho bởi $((b, g), f)\mapsto (b, gf)$ định nghĩa các B-đẳng cấu nghịch đảo nhau $B\times F\rightarrow (B\times G)\times^GF$ và $(B\times G)\times^GF\rightarrow B\times F$.

#### Ví dụ 3 {#ta-i-s5-n5-exa-3 .statement tag=01R8}

Tương tự, cho E là một không gian tôpô và G là một nhóm tôpô tác động liên tục bên phải trên E. Nếu không gian tôpô G được trang bị phép toán của G bởi các phép tịnh tiến trái, thì không gian $E\times^GG$ được đồng nhất với E.

Cho E và F là các không gian tôpô và G là một nhóm tôpô tác động liên tục bên phải trên E và bên trái trên F. Cho B là một không gian tôpô và cho $p: E\rightarrow B$ là một ánh xạ liên tục sao cho $p(x\cdot g) =p(x)$ với $x\in E$ và $g\in G$. Ánh xạ $p\circ$ pr$_1: E\times F\rightarrow B$ xác định, bằng cách chuyển qua thương, một ánh xạ liên tục $p^F: E\times^GF\rightarrow B$ và ánh xạ chính tắc $\pi : E\times F\rightarrow E\times^GF$ là một B-cấu xạ.

Cho $B'$ là một không gian tôpô và cho $h: B'\rightarrow B$ là một ánh xạ liên tục. Nhóm G tác động liên tục bên phải trên $B'\times_BE$ theo luật phép toán $((b', x), g)\mapsto (b', x\cdot g)$. Bằng cách hợp thành đẳng cấu chính tắc $((b', x), y)\mapsto (b',(x, y))$ của $(B'\times_BE)\times F$ lên $B'\times_B(E\times F)$ với ánh xạ Id$_{B'}\times \pi$ của $B'\times_B(E\times F)$ vào $B'\times_B(E\times^GF)$, ta thu được một ánh xạ liên tục $\lambda_0: (B'\times_BE)\times F\rightarrow B'\times_B(E\times^GF)$. Nó xác định, bằng cách chuyển qua thương, một ánh xạ liên tục

$$
\lambda : (B'\times_BE)\times^GF\rightarrow B'\times_B(E\times^GF)
$$

#### Bổ đề {#ta-i-s5-n5-lem-1 .statement tag=01R9}

Ánh xạ $\lambda$ là một phép đồng phôi.

Ánh xạ $\lambda_0$ là toàn ánh và hai phần tử của $(B'\times_BE)\times F$ có cùng ảnh qua $\lambda_0$ khi và chỉ khi chúng thuộc cùng một quỹ đạo đối với phép toán của G trên $(B'\times_BE)\times F$. Suy ra rằng ánh xạ $\lambda$ là song ánh. Vì ánh xạ $\pi$ là mở, điều tương tự cũng đúng với ánh xạ Id$_{B'}\times_B\pi ($I, p. 17, prop. 8), do đó đúng với $\lambda_0$ và $\lambda$ (TG, I, p. 32, prop. 3), điều này chứng minh rằng $\lambda$ là một phép đồng phôi.

#### Mệnh đề 7 {#ta-i-s5-prop-7 .statement tag=01RA}

Cho B là một không gian tôpô, cho G là một nhóm tôpô, cho $(E, p)$ là một không gian bó chính trên B với nhóm G và cho F là một không gian tôpô trên đó nhóm G tác động liên tục bên trái.

a) Không gian tôpô $E\times^GF$ được trang bị ánh xạ liên tục $p^F: E\times^GF\rightarrow B$ suy ra từ ánh xạ $p\circ$pr$_1: E\times F\rightarrow B$ bằng cách chuyển qua thương là một không gian bó địa phương tầm thường trên B kiểu thớ F; nó tầm thường hóa được nếu không gian bó trên B E tầm thường hóa được.

b) Cho $\pi : E\times F\rightarrow E\times^GF$ là toàn cấu chính tắc. Ánh xạ $\mu: E\times F\rightarrow E\times_B(E\times^GF)$ gán cho $(x, f)$ phần tử $(x, \pi (x, f))$ là một phép đồng phôi mà ánh xạ nghịch đảo của nó là một phép tầm thường hóa của không gian bó địa phương tầm thường trên E $(E\times_B(E\times^GF)$, pr$_1)$.

Trước hết, giả sử E là không gian bó chính tầm thường trên B $B\times G$. Theo ví dụ 2, khi đó không gian $E\times^GF$ được đồng nhất với $B\times F$ và ánh xạ $p^F$ với phép chiếu thứ nhất pr$_1: B\times F\rightarrow B$, điều này chứng minh rằng $(E\times^GF, p^F)$ là một không gian bó tầm thường hóa được trên B trong trường hợp này. Trong trường hợp tổng quát, mọi điểm của B đều có một lân cận U sao cho ánh xạ $p_U:\overset{-1}{p}(U)\rightarrow U$ biến $\overset{-1}{p}(U)$ thành một không gian bó chính tầm thường hóa được trên U. Từ những điều trên, $(\overset{-1}{p}(U)\times^GF\rightarrow U,(p_U)^F)$ là một không gian bó tầm thường hóa được trên U. Theo bổ đề trên, áp dụng cho trường hợp $B'= U$ và $h: U\rightarrow B$ là đơn ánh chính tắc, điều tương tự cũng

đúng đối với không gian bó trên U ($(p^{-F1})(U),(p^F)_U$) suy ra từ $(E\times^GF, p^F)$ bằng phép hạn chế trên U. Điều này chứng minh rằng $(E\times^GF, p^F)$ là một không gian bó địa phương tầm thường trên B và kết thúc chứng minh mệnh đề a).

Ánh xạ $\theta : E\times G\rightarrow E\times_BE$ được xác định bởi $\theta (x, g) = (x, x\cdot g)$ là một đồng phôi (I, p. 94, mệnh đề 3) tương thích với các phép toán của G trên $E\times G$ và trên $E\times_BE$ lần lượt được cho bởi $((x, g), g')\mapsto (x, gg')$ và $((x, y), g')\mapsto (x, yg')$. Do chuyển qua các thương, $\theta$ do đó cảm sinh một đồng phôi $\theta '$ của $(E\times G)\times^GF$ lên $(E\times_B$ $E)\times^GF$. Ánh xạ $\mu$ là hợp thành của đồng phôi $E\times F\rightarrow$ $(E\times G)\times^GF$ (ví dụ 2), của $\theta '$, và của đồng phôi chính tắc $(E\times_BE)\times^GF\rightarrow E\times_B(E\times^GF)$ (I, p. 105, bổ đề), do đó b).

Theo các giả thiết của mệnh đề 7, không gian B-xơ địa phương tầm thường ($E\times^GF, p^F$) được gọi là không gian xơ địa phương tầm thường kiểu xơ F liên kết với không gian xơ chính $(E, p)$. Tất cả các xơ của không gian B $E\times^GF$ đều đồng phôi với không gian F. Đặc biệt, nếu không gian F là rời rạc, ánh xạ $p^F$ là một phủ.

#### Ví dụ 4 {#ta-i-s5-n5-exa-4 .statement tag=01RB}

Cho B là một không gian tôpô, G là một nhóm tôpô, và $(E, p)$ là một không gian B-xơ chính với nhóm G. Cho H là một nhóm con của G.

Ký hiệu $\varphi : E\rightarrow E\times (G/H)$ và $\psi : E\times (G/H)\rightarrow E/H$ là các ánh xạ được xác định bởi $\varphi (x) = (x,H)$ và $\psi (x, gH) = (x\cdot g)H$. Chúng tương thích với các phép chiếu lên B và với các phép toán của G và xác định, bằng cách chuyển qua các thương, các cấu xạ của các không gian B $\overline{\varphi}: E/H\rightarrow E\times^G(G/H)$ và $\overline{\psi}: E\times^G(G/H)\rightarrow E/H$, nghịch đảo lẫn nhau. Người ta nói rằng $\overline{\varphi}$ là đồng phôi chính tắc của $E/H$ lên $E\times^G(G/H)$. Đặc biệt, không gian tôpô $E/H$ được trang bị với ánh xạ liên tục $p_H: E/H\rightarrow B$ là một không gian B-xơ địa phương tầm thường kiểu xơ $G/H$.

Nếu hơn nữa, H là một nhóm con chuẩn tắc của G, tác động của G trang bị cho không gian B $E/H$, bằng cách chuyển qua các thương, một cấu trúc của không gian xơ chính với nhóm $G/H$.

Đặc biệt, nếu E là một phủ chính của B với nhóm G, $E/H$ là một phủ của B; nếu H là chuẩn tắc trong G, nó là một phủ chính với nhóm $G/H$.

#### Ví dụ 5 {#ta-i-s5-n5-exa-5 .statement tag=01RC}

Cho B là một không gian tôpô, cho G là một nhóm tôpô, và cho E là một không gian B-xơ chính với nhóm G. Cho F là một không gian thuần nhất tôpô đối với G (TG, III, p. 12). Cho $y$ là một điểm của F và cho $G_y$ là nhóm ổn định của nó. Ánh xạ $\varphi_y:x\mapsto (x, y)$ từ E vào $E\times F$ xác định, bằng cách chuyển qua các thương, một đồng phôi $\overline{\varphi}_y$ của $E/G_y$ lên $E\times^GF$. Khi nhóm G là Abel, nhóm con $G_y$ không phụ thuộc vào điểm $y$, nhưng nói chung, đồng phôi $\overline{\varphi}_y$ lại phụ thuộc vào nó.

#### Ví dụ 6 {#ta-i-s5-n5-exa-6 .statement tag=01RD}

Cho B là một không gian tôpô, cho G là một nhóm tôpô, cho $(E, p)$ là một không gian B-xơ chính với nhóm G. Cho H là một nhóm tôpô và cho $f: G\rightarrow H$ là một cấu xạ của các nhóm tôpô; hãy trang bị cho H phép toán trái của G được cho bởi $g\cdot h=f(g)h$.

Cho $q: E\times H\rightarrow E\times^GH$ là ánh xạ chính tắc; nó là mở, do đó ngặt phổ quát (I, p. 20, hệ quả 11). Ánh xạ $m: (x, h, h')\mapsto q(x, hh')$ từ $E\times H\times H$ vào $E\times^GH$ là liên tục. Cho $(x, h)\in E\times H,h'\in H$ và $g\in G$; ta có $m(xg, f(g)^{-1}h, h') =$ $q(xg, f(g)^{-1}hh') =q(x, hh') =m(x, h, h')$. Do đó, tồn tại một ánh xạ duy nhất

$$
m': (E\times^GH)\times H\rightarrow E\times^GH
$$

sao cho $m'(q(x, h), h') =q(x, h, h')$ với mọi $x\in E$ và mọi $h, h'\in H$. Vì $q$ là ngặt một cách phổ quát, ánh xạ $m'$ liên tục. Đây là một phép toán phải của nhóm tôpô H trên B-không gian $E\times^GH$.

Cho U là một tập con mở của B sao cho $E_U$ đẳng cấu với bó sợi chính trên U, $U\times G$. Được trang bị phép toán của H, U-không gian $(E\times^GH)_U$ được đồng nhất với bó sợi chính $U\times H$. Điều này chứng minh rằng $E\times^GH$ là một bó sợi chính trên B với nhóm H.

#### Định nghĩa 4 {#ta-i-s5-def-4 .statement tag=01RE}

Cho B là một không gian tôpô và G là một nhóm tôpô. Một không gian sợi địa phương tầm thường X trên B được gọi là liên kết với một bó sợi chính E trên B với nhóm G nếu tồn tại một không gian tôpô F trên đó nhóm G tác động liên tục ở bên trái và một B-đẳng cấu từ $E\times^GF$ lên X.

Cho E là một bó sợi chính trên B với nhóm G và cho X là một không gian sợi địa phương tầm thường trên B liên kết với E. Nếu bó sợi chính E tầm thường hóa được, thì X tầm thường hóa được (Mệnh đề 7). Nếu $B'$ là một không gian tôpô và $h: B'\rightarrow B$ là một ánh xạ liên tục, thì không gian sợi địa phương tầm thường trên $B'$, $B'\times_BX$, suy ra từ X bởi phép thay đổi cơ sở là liên kết với bó sợi chính trên $B'$, $B'\times_BE$ (I, p. 105, bổ đề).

### 6. Các phủ liên kết

Cho B là một không gian tôpô, G là một nhóm tôpô rời rạc và E là một phủ chính của B với nhóm G. Cho F là một G-tập hợp; nếu F được trang bị tôpô rời rạc, nhóm G tác động liên tục trên F. Khi đó B-không gian $E\times^GF$ là một phủ. Nó được gọi là phủ của B với kiểu sợi F liên kết với phủ chính E.

#### Định nghĩa 5 {#ta-i-s5-def-5 .statement tag=01RF}

Cho B là một không gian tôpô, G là một nhóm tôpô rời rạc và E là một phủ chính của B với nhóm G. Một phủ X của B được gọi là liên kết với phủ chính E nếu tồn tại một G-tập hợp F và một B-đẳng cấu từ $E\times^GF$ lên X.

Cho B là một không gian tôpô, G là một nhóm tôpô rời rạc và E là một phủ của B, chính với nhóm G.

Với mọi phủ X của B, nhóm G tác động ở bên trái trên $\mathscr{C}_B(E; X)$ theo luật xác định bởi $(g\cdot h)(x) =h(x\cdot g)$ với $x\in E$, $g\in G,h\in \mathscr{C}_B(E; X)$.

Với mọi G-tập hợp F được trang bị tôpô rời rạc, ta định nghĩa một ánh xạ $\alpha_F: F\rightarrow \mathscr{C}_B(E; E\times^GF)$ bởi:

(2) $\alpha_F(y)(x) =\pi (x, y)$ với $y\in F$ và $x\in E$,

trong đó $\pi : E\times F\rightarrow E\times^GF$ là toàn cấu chính tắc. Ánh xạ $\alpha_F$ tương thích với các phép toán của G trên F và trên $\mathscr{C}_B(E; E\times^GF)$.

Với mọi phủ X của B, tồn tại một ánh xạ duy nhất $\beta_X$ từ $E\times^G\mathscr{C}_B(E; X)$ vào X sao cho:

(3) $\beta_X(\pi (x, h)) =h(x)$ với $h\in \mathscr{C}_B(E; X)$ và $x\in E$.

Thực vậy, ta có $(g^{-1}\cdot h)(x\cdot g) =h(x)$ với $x\in E,g\in G$ và $h\in \mathscr{C}_B(E; X)$, theo định nghĩa phép toán của G trên $\mathscr{C}_B(E; X)$. Khi tập hợp $\mathscr{C}_B(E; X)$ được trang bị tôpô rời rạc, ánh xạ $\beta_X$ là một B-cấu xạ của các phủ.

Khi $X = E\times^GF$, ta có

(4) $\beta_X(\pi (x, \alpha_F(y))) =\pi (x, y)$ với $x\in X$ và $y\in F$.

#### Mệnh đề 8 {#ta-i-s5-prop-8 .statement tag=01RG}

Cho B là một không gian tôpô liên thông khác rỗng. Cho G là một nhóm rời rạc và cho $(E, p)$ là một phủ chính của B với nhóm G. Giả sử E liên thông. Với ký hiệu trên, ta có:

a) Với mọi G-tập hợp F được trang bị tôpô rời rạc, ánh xạ $\alpha_F$ là một đẳng cấu của G-tập hợp F lên G-tập hợp $\mathscr{C}_B(E; E\times^GF)$.

b) Cho X là một phủ của B. B-cấu xạ $\beta_X$ là một đẳng cấu của $E\times^G\mathscr{C}_B(E; X)$ lên X khi và chỉ khi phủ $(E\times_BX$, pr$_1)$ của E tầm thường hóa được.

(a) Cho $y$ và $y'$ là các điểm của F sao cho $\alpha_F(y) =\alpha_F(y')$. Không gian E không rỗng; hãy chọn một điểm $x$ trong đó. Ta có $\pi (x, y) =\pi (x, y')$ trong $E\times^GF$. Do đó tồn tại $g\in G$ sao cho $x\cdot g=x$ và $g^{-1}\cdot y=y'$. Đẳng thức thứ nhất suy ra rằng $g$ là phần tử đơn vị $e$ của G, do đó $y=y'$. Vậy ánh xạ $\alpha_F$ là đơn ánh. Mặt khác, lấy $h\in$ $\mathscr{C}_B(E; E\times^GF)$ và lấy $x$ là một điểm của E. Lấy $x'\in E,y'\in F$ sao cho $h(x) =\pi (x', y')$. Đặc biệt, $p(x) =p(x')$; do đó tồn tại một phần tử $g$ của G sao cho $x'=x\cdot g$, và ta cũng có $h(x) =\pi (x, y)$, trong đó ta đặt $y=g\cdot y'$. Các cấu xạ B $h$ và $\alpha_F(y)$ trùng nhau tại điểm $x$ của E; do đó chúng bằng nhau vì không gian E liên thông (I, p. 34, Hệ quả 1 của Mệnh đề 11), và điều này chứng minh rằng ánh xạ $\alpha_F$ là toàn ánh.

(b) Theo mệnh đề 7, b) của I, p. 105 áp dụng cho $F =\mathscr{C}_B(E; X)$, phủ $p^*(E\times^G\mathscr{C}_B(E; X))$ của E là đẳng cấu với phủ tầm thường $E\times \mathscr{C}_B(E; X)$. Nếu $\beta_X$ là một đẳng cấu, thì phủ $p^*(X)$ của E do đó là tầm thường hóa được. Ngược lại, giả sử rằng phủ $p^*(X)$ là tầm thường hóa được và hãy chứng minh rằng cấu xạ B $\beta_X$ là song ánh; khi đó suy ra $\beta_X$ là một B-đẳng cấu (I, p. 30, Hệ quả 2 của Mệnh đề 6).

Ánh xạ $\beta_X$ được suy ra bằng cách chuyển qua thương từ ánh xạ $\gamma : E\times \mathscr{C}_B(E; X)\rightarrow X$ được xác định bởi $\gamma (x, h) =h(x)$. Hãy chứng minh rằng ánh xạ $\gamma$ là toàn ánh. Lấy $x$ là một điểm của X. Phép chiếu của không gian B E là toàn ánh, vì đó là một phủ chính; do đó tồn tại một điểm $y$ của E sao cho $(y, x)\in E\times_BX$. Khi đó tồn tại một tiết diện liên tục $s$ của phủ tầm thường hóa được pr$_1: E\times_BX\rightarrow E$ sao cho $s(y) = (y, x)$. Ánh xạ $h=$ pr$_2\circ s: E\rightarrow X$ là một cấu xạ B, và ta có $h(y) =x$, do đó ánh xạ $\gamma$ là toàn ánh và, do đó, ánh xạ $\beta_X$ cũng toàn ánh.

Cuối cùng, ta hãy chứng minh rằng $\beta_X$ là đơn ánh. Cho $(x, h)$ và $(x', h')$ là các phần tử của $E\times \mathscr{C}_B(E; X)$ sao cho $h(x) =h'(x')$. Nhận thấy rằng $x$ và $x'$ có cùng phép chiếu trong B; do đó tồn tại một phần tử $g$ của G sao cho $x'=x\cdot g$. Khi đó ta có $h(x) =h'(x\cdot g) = (g\cdot h')(x)$. Vì không gian E liên thông, ta có $h=g\cdot h'($I, p. 34, hệ quả 1 của mệnh đề 11). Do đó, $(x, h)$ và $(x', h')$ có cùng lớp trong $E\times^G\mathscr{C}_B(E; X)$, điều này chứng tỏ rằng ánh xạ $\beta_X$ là đơn ánh, và hoàn tất chứng minh.

#### Hệ quả 1 {#ta-i-s5-prop-8-cor-1 .statement tag=01RH}

Cho $(E, p)$ là một phủ chính của B với nhóm G; giả sử E liên thông và khác rỗng. Một phủ X của B liên kết được với E khi và chỉ khi phủ $p^*(X)$ tầm thường hóa được.

Nếu phủ $p^*(X)$ tầm thường hóa được, thì theo mệnh đề 8, b), phủ X liên kết được với E. Trong trường hợp này, ánh xạ $\beta_X$ đồng nhất phủ X với phủ kiểu thớ $\mathscr{C}_B(E; X)$ liên kết với E. Ngược lại, cho F là một G-tập hợp được trang bị tôpô rời rạc và giả sử ta có $X = E\times^GF$. Khi đó $\alpha_F$ là một đẳng cấu (loc. cit., a)) và công thức (4) suy ra rằng $\beta_X$ là một đẳng cấu. Do đó, phủ $p^*(X)$ tầm thường hóa được (mệnh đề 8, b)), do đó có hệ quả.

#### Hệ quả 2 {#ta-i-s5-prop-8-cor-2 .statement tag=01RI}

Cho B là một không gian tôpô liên thông và liên thông địa phương, cho $(E, p)$ là một phủ chính của B với nhóm G. Cho $E_0$ là một thành phần liên thông của E và cho $G_0$ là nhóm con của G ổn định $E_0$. Không gian B $(E_0, p|E_0)$ là một phủ chính với nhóm $G_0($I, p. 103, mệnh đề 6).

Mọi phủ X của B liên kết với phủ chính E đều liên kết với phủ chính $E_0$. Đặc biệt, phủ E liên kết với phủ chính $E_0$.

Thật vậy, nếu phủ X liên kết với E, thì phủ $p^*(X)$ tầm thường hóa được và phủ $p^*_0(X)$ cảm sinh bởi $p^*(X)$ trên $E_0$ do đó cũng tầm thường hóa được.

Chính xác hơn, chú ý rằng ánh xạ $(x, g)\mapsto x\cdot g$ từ $E_0\times G$ vào E cảm sinh, bằng cách chuyển qua thương, một B-đẳng cấu của các phủ chính từ $E_0\times^{G_0}G$ lên E.

#### Mệnh đề 9 {#ta-i-s5-prop-9 .statement tag=01RJ}

Cho B là một không gian tôpô, cho E là một phủ chính của B với nhóm G, liên thông và khác rỗng. Cho F là một G-tập hợp khác rỗng được trang bị tôpô rời rạc. Để không gian $E\times^GF$ liên thông, điều kiện cần và đủ là G tác động bắc cầu trên F.

Cho U là một tập con mở và đóng của $E\times^GF$. Nếu $\pi : E\times F\rightarrow$ $E\times^GF$ là toàn cấu chính tắc, thì $\overset{-1}{\pi}(U)$ là một tập con mở và đóng của $E\times F$ ổn định dưới G. Vì E liên thông, tồn tại một tập con $F'\subset F$, ổn định dưới G, sao cho $\overset{-1}{\pi}(U) = E\times F'$, do đó $U =\pi (E\times F')$. Cho $F'$ và $F''$ là các tập con của F ổn định dưới G sao cho $\pi (E\times F') =\pi (E\times F'')$; vì E không rỗng, ta có $F'= F''$. Ánh xạ $F'\mapsto \pi (E\times F')$ là một song ánh từ tập hợp các tập con của F ổn định dưới G lên tập hợp các tập con mở và đóng của $E\times^GF$. Mệnh đề được chứng minh.

#### Mệnh đề 10 {#ta-i-s5-prop-10 .statement tag=01RK}

Cho B là một không gian tôpô, cho $(E, p)$ là một phủ chính của B với nhóm G và cho X là một phủ của B. Giả sử E và X liên thông và khác rỗng. Các tính chất sau là tương đương:

(i) Phủ X liên kết được với phủ chính E;

(ii) Tồn tại một nhóm con H của G sao cho X B-đẳng cấu với $E/H$;

(iii) Tồn tại một B-cấu xạ toàn ánh $h: E\rightarrow X$;

(iv) Với mọi điểm $(y, x)$ của $E\times_BX$, tồn tại một B-cấu xạ $r: E\rightarrow X$ sao cho $r(y) =x$.

Giả sử các điều kiện này được thỏa mãn và cho H là một nhóm con của G sao cho X đẳng cấu B với $E/H$. Phủ X là Galois khi và chỉ khi nhóm con H là chuẩn trong G.

(i)$\Rightarrow$(ii) : Cho F là một G-tập rời rạc sao cho phủ $E\times^GF$ là đẳng cấu B với X. Tập hợp F là khác rỗng và không gian $E\times^GF$ là liên thông, do đó nhóm G tác động bắc cầu trên F (mệnh đề 9). Khi đó không gian $E\times^GF$ là đẳng cấu B với $E/H$, trong đó H là nhóm con của G cố định một điểm của F (I, p. 106, ví dụ 4).

(ii)$\Rightarrow$(iii) : Thực vậy, toàn cấu chính tắc từ E lên $E/H$ là một B-cấu xạ toàn ánh.

(iii)$\Rightarrow$(iv) : Cho $(y, x)$ là một điểm của $E\times_BX$. Vì ánh xạ $h$ là toàn ánh, tồn tại một điểm $y'$ của E sao cho $h(y') =x$. Các điểm $y$ và $y'$ có cùng phép chiếu trong B. Vì phủ E là chính với nhóm G, tồn tại $g\in G$ sao cho $y\cdot g=y'$. Ánh xạ $r: E\rightarrow X$ được xác định bởi $z\mapsto h(z\cdot g)$ là một B-cấu xạ và ta có $r(y) =x$.

(iv)$\Rightarrow$(i) : Vì X khác rỗng và phép chiếu của E lên B là toàn ánh, không gian $E\times_BX$ là khác rỗng. Do đó tồn tại một B-cấu xạ $r$ từ E vào X. Ánh xạ (Id$_E, r$)$: E\rightarrow E\times_BX$ là một tiết diện của phủ $p^*(X)$ của E. Vì không gian E là liên thông, suy ra từ Hệ quả 2 của mệnh đề 1 của I, p. 69 rằng phủ $p^*(X)$ là khả vi tầm thường, điều này chứng minh rằng phủ X là liên hợp với phủ Galois $p$ (mệnh đề 8).

Bây giờ giả sử rằng các điều kiện này được thỏa mãn. Ta ký hiệu X là B-không gian $E/H$, q là phép chiếu của nó, và $h: E\rightarrow E/H$ là ánh xạ chính tắc.

Nếu nhóm H là chuẩn trong G, thì X là một phủ chính với nhóm $G/H$ (I, p. 106, ví dụ 4). Vì X và B là liên thông và khác rỗng, X là một phủ Galois của B (I, p. 102, định lý 2). Ngược lại, giả sử rằng $E/H$ là một phủ Galois của B và đặt K = Aut$_B(E/H)^{\circ}$. Ta xác định một ánh xạ $\alpha : E\times G\rightarrow K$ bằng cách gán cho $(t, g)\in E\times G$ phần tử duy nhất $k$ của K sao cho $h(t\cdot g) =h(t)\cdot k$. Ánh xạ này liên tục vì nó nhận được bằng cách hợp thành ánh xạ liên tục $(t, g)\mapsto (h(t), h(t\cdot g))$ từ $E\times G$ vào $X\times_BX$ với phép tầm thường hóa chính tắc (I, p. 95, nhận xét 1) $X\times_BX\rightarrow X\times K$ của $q^*(X)$. Vì E là liên thông và K là một nhóm rời rạc, ánh xạ liên tục $t\mapsto \alpha (t, g)$ là hằng, với mọi $g\in G$; ta ký hiệu giá trị của nó bởi $\alpha (g)$. Nếu $t\in E,g\in G$ và $g'\in H$, khi đó ta có

$$
h(t) =h(t\cdot g^{-1}g) =h(t\cdot g^{-1})\cdot \alpha (g) =h(t\cdot g^{-1}\cdot g')\cdot \alpha (g) =h(t\cdot (g^{-1}g'g))
$$

Suy ra rằng $g^{-1}g'g$ thuộc H và do đó H là chuẩn trong G.

#### Hệ quả {#ta-i-s5-n6-cor-1 .statement tag=01RL}

Cho E là một phủ Galois của B và cho X là một phủ của B, liên thông và khác rỗng. Giả sử rằng X là một phủ hữu hạn hoặc không gian B là liên thông địa phương. Nếu tồn tại một B-cấu xạ $h: E\rightarrow X$, thì phủ X là liên hợp với phủ chính E.

Trong cả hai trường hợp, B-cấu xạ $h$ là một phủ (I, p. 77, Hệ quả 3 của định lý 1, và I, p. 78, mệnh đề 5), và một phủ khác rỗng của một không gian liên thông là toàn ánh (I, p. 68).

#### Định lý 3 {#ta-i-s5-thm-3 .statement tag=01RM}

Cho B là một không gian tôpô khác rỗng, liên thông và liên thông địa phương. Mọi phủ của B đều liên hợp với một phủ Galois; mọi phủ hữu hạn của B đều liên hợp với một phủ Galois hữu hạn.

Cho X là một phủ của B, và ký hiệu $q$ là phép chiếu của nó. Vì không gian B liên thông và khác rỗng, phủ X có một bậc; ký hiệu bậc này là F và trang bị cho tập hợp F tôpô rời rạc. Vì không gian B liên thông địa phương, bó $\mathscr{I}$ = $\mathscr{I}$som$_B(B\times F; X)$ là hằng địa phương và tại mọi điểm $b$ của B, thớ $\mathscr{I}_b$ của nó là đẳng cấu chính tắc với tập hợp $\mathscr{B}(F; X_b)$ các song ánh của F lên thớ $X_b($I, p. 89, Mệnh đề 12). Đặt $E = E_{\mathscr{I}}$ là phủ liên kết với bó hằng địa phương $\mathscr{I}($I, p. 86, hệ quả).

Cho G là nhóm các hoán vị của F. Với mỗi $g\in G$, ta định nghĩa như sau một cấu xạ $\gamma '(g)$ của bó $\mathscr{I}$ vào chính nó: với mỗi tập con mở U của B, ánh xạ $\gamma '(g)_U$ liên kết với một U-đẳng cấu $\varphi : U\times F\rightarrow \overset{-1}{q}(U)$ U-đẳng cấu được xác định bởi $(b, f)\mapsto \varphi (b, g(f))$ với $b\in U$ và $f\in F$. Ta có $\gamma '$(Id$_F$) $=$ Id$_{\mathscr{I}}$ và $\gamma '(g\circ g') =\gamma '(g')\circ \gamma '(g)$, với $g,g'\in G$, do đó với mọi $g\in G,\gamma '(g)$ là một tự đẳng cấu của bó $\mathscr{I}$. Cấu xạ B $\gamma (g): E\rightarrow E$ liên kết với $\gamma '(g)$ là một tự đẳng cấu (I, p. 50). Nếu $x= [U, \varphi , b]$ là một phần tử của E, trong đó U là một tập con mở của B$,b$ là một điểm của U và $\varphi$ là một U-đẳng cấu của $U\times F$ lên $\overset{-1}{q}(U)$, thì ta có $\gamma (g)(x) = [U, \psi , b]$, trong đó $\psi$ được xác định bởi $\psi (a, f) =\varphi (a, g(f))$, với $a\in$ U và $f\in$ F. Nếu $g$ và $g'$ là các phần tử của G, thì ta có $\gamma (g\circ g') =\gamma (g')\circ \gamma (g)$. Ta có $\gamma$(Id$_F$) $=$ Id$_E$. Do đó ta định nghĩa một luật phép toán phải liên tục của G trên E bằng cách đặt $x\cdot g=\gamma (g)(x)$, với $x\in E$ và $g\in G$. Nhóm G tác động đơn giản bắc cầu trên mỗi thớ của E, do đó phủ E được trang bị phép toán này là một phủ chính với nhóm G (I, p. 97, prop. 4). Cho $h$ là ánh xạ từ $E\times F$ vào X được xác định bởi $h([U, \varphi , b], f) =\varphi (b, f)$ với mọi tập con mở U của B, mọi điểm $b$ của U và mọi U-đẳng cấu $\varphi$ của $U\times F$ lên $\overset{-1}{q}(U)$. Theo định nghĩa của tôpô của E, nó liên tục; nó là một cấu xạ B. Với mọi phần tử $g$ của G và mọi điểm $(x, f)$ của $E\times F$, ta có $h(x, g(f)) =h(x\cdot g, f)$. Do đó, ánh xạ $h$ xác định, bằng cách chuyển qua thương, một cấu xạ B $h': E\times^GF\rightarrow X$. Với mỗi điểm $b$ của B, ánh xạ $h_b: E_b\times F\rightarrow X_b$ đồng nhất với ánh xạ $(\varphi , f)\mapsto \varphi (f)$ từ $\mathscr{B}(F; X_b)\times F$ vào $X_b$, do đó ánh xạ $h'_b$ là song ánh. Do đó, $h'$ là một B-đẳng cấu của $E\times^GF$ lên X (I, p. 30, cor. 2 of prop. 6).

Vì không gian B liên thông, liên thông địa phương và khác rỗng, phủ X, liên kết với phủ chính E, được liên kết với một phủ Galois (I, p. 110, corollary 2). Nếu phủ X hữu hạn, điều tương tự cũng đúng đối với phủ E, do đó X được liên kết với một phủ Galois hữu hạn (loc. cit.).

### 7. Các không gian thớ chính được xác định bởi các cocycle

#### Định nghĩa 6 {#ta-i-s5-def-6 .statement tag=01RN}

Cho B là một không gian tôpô, G là một nhóm tôpô, và $\mathscr{U}= (U_i)_{i\in I}$ là một phủ mở của B. Một 1-cocycle liên tục trên B với các giá trị trong G, phụ thuộc vào $\mathscr{U}$, theo định nghĩa là dữ liệu, với mỗi cặp $(i, j)$ các phần tử của I, của một ánh xạ liên tục $g_{i,j}$ từ $U_i\cap U_j$ vào G, sao cho với mọi bộ ba $(i, j, k)\in I\times I\times I$ và mọi điểm $b$ của $U_i\cap U_j\cap U_k$, ta có

$$
g_{i,k}(b) =g_{i,j}(b)g_{j,k}(b)
$$

Ta ký hiệu $Z^1_{cont}(B,\mathscr{U},G)$ là tập hợp các 1-cocycle liên tục trên B với các giá trị trong G, phụ thuộc vào phủ $\mathscr{U}$.

Trong tiết diện này, ta sẽ đơn giản gọi là cocycle thay cho 1-cocycle liên tục.

Cho $(E, p)$ là một không gian sợi chính trên B của nhóm G, và cho $\mathscr{U}$ = $(U_i)_{i\in I}$ là một phủ của B bởi các tập mở $U_i$. Người ta nói rằng E khả vi tầm thường trên $\mathscr{U}$ nếu, với mọi $i\in I$, E khả vi tầm thường trên $U_i$. Khi đó, người ta gọi một phép tầm thường hóa $\mathscr{U}$ của E là một họ $(f_i)_{i\in I}$, trong đó $f_i:\overset{-1}{p}(U_i)\rightarrow U_i\times G$ là một phép tầm thường hóa của E trên $U_i$.

Cho $\mathscr{U}= (U_i)_{i\in I}$ là một phủ của B bởi các tập mở, và cho $(E, p)$ là một không gian sợi chính trên B của nhóm G được trang bị một phép tầm thường hóa $\mathscr{U}$ $(f_i)_{i\in I}$. Với mỗi cặp $(i, j)\in I\times I$, ta ký hiệu $g_{ij}$ là ánh xạ từ $U_i\cap U_j$ vào G được xác định bởi

$$
(b, g_{ij}(b)) =f_i\circ f_j^{-1}(b, e)
$$

trong đó $e$ ký hiệu phần tử đơn vị của G. Ánh xạ này liên tục.

Vì $f_i$ và $f_j$ tương thích với các phép toán của G, ta có

$$
(f_i\circ f_j^{-1})(b, g) = (b, g_{ij}(b)g)
$$

với $b\in U_i\cap U_j$ và $g\in G$. Nếu $b$ là một điểm của $U_i\cap U_j\cap U_k$ (trong đó $i,j$, $k\in I$), ta có

$$
(f_i\circ f_k^{-1})(b, e) = (b, g_{ik}(b))
$$

và

$$
(f_i\circ f_k^{-1})(b, e) = (f_i\circ f_j^{-1})\circ (f_j\circ f_k^{-1})(b, e)
$$

$$
= (f_i\circ f_j^{-1})(b, g_{jk}(b)) = (b, g_{ij}(b)g_{jk}(b))
$$

Suy ra rằng

$$
g_{ik}(b) =g_{ij}(b)g_{jk}(b)
$$

do đó họ $(g_{ij})$ là một cocycle trên B với các giá trị trong G, phụ thuộc vào phủ $\mathscr{U}$. Nó được gọi là cocycle xác định bởi họ các phép tầm thường hóa $(f_i)_{i\in I}$.

Cho B, G và $\mathscr{U}$ như trong định nghĩa 6, và cho $(g_{ij})\in$ $Z^1_{cont}(B,\mathscr{U},G)$ là một cocycle. Với mỗi cặp $(i, j)\in I\times I$, ánh xạ $\gamma_{ij}: (U_i\cap U_j)\times G\rightarrow (U_i\cap U_j)\times G$ được xác định bởi

(5) $\gamma_{ij}(b, g) = (b, g_{ij}(b)g)$ với $b\in U_i\cap U_j$ và $g\in G$

là một đẳng cấu của các không gian sợi chính có cơ sở $U_i\cap U_j$. Với mọi bộ ba $(i, j, k)\in I\times I\times I$ và mọi cặp $(b, g)\in (U_i\cap U_j\cap U_k)\times G$, ta có :

$$
\gamma_{ik}(b, g) =\gamma_{ij}\circ \gamma_{jk}(b, g)
$$

Cho F là không gian tôpô thu được bằng cách dán các không gian $U_i\times G$ theo các $(U_i\cap U_j)\times G$ nhờ các song ánh $\gamma_{ij}$ (TG, I, p. 16). Với mỗi $i\in I$, ảnh của $U_i\times G$ trong F là một tập mở của F (TG, I, p. 17, Mệnh đề 9). Các phép chiếu chính tắc $p_i: U_i\times G\rightarrow U_i$ dán lại với nhau để cho một ánh xạ liên tục $p$ của F vào B. Vì các ánh xạ $\gamma_{ij}$ tương thích với các phép toán phải của G trong các không gian $U_i\times G$, suy ra một luật phép toán liên tục của G ở bên phải trong F, biến F thành một không gian bó sợi chính với cơ sở B và nhóm G, được trang bị một phép tầm thường hóa trên mỗi $U_i$. Ta nói rằng F là không gian bó sợi chính được xác định bởi cocycle $(g_{ij})$.

#### Định nghĩa 7 {#ta-i-s5-def-7 .statement tag=01RO}

Cho B là một không gian tôpô, G là một nhóm tôpô và $\mathscr{U}= (U_i)_{i\in I}$ là một phủ mở của B. Hai cocycle $(g_{ij})$ và $(g'_{ij})$ của $Z^1_{cont}(B,\mathscr{U},G)$ được gọi là đồng điều nếu tồn tại một họ $(h_i)_{i\in I}$ các ánh xạ liên tục $h_i: U_i\rightarrow G$ sao cho

$$
g'_{ij}(b) =h_i(b)g_{ij}(b)h_j(b)^{-1} \tag{6}
$$

với mọi cặp $(i, j)\in I\times I$ và mọi $b\in U_i\cap U_j$.

Quan hệ “$(g_{ij})$ đồng điều với $(g'_{ij})$” là một quan hệ tương đương trong tập hợp $Z^1_{cont}(B,\mathscr{U},G)$. Ta ký hiệu $H^1_{cont}(B,\mathscr{U},G)$ là tập thương của $Z^1_{cont}(B,\mathscr{U},G)$ theo quan hệ tương đương này.

#### Mệnh đề 11 {#ta-i-s5-prop-11 .statement tag=01RP}

Cho B là một không gian tôpô, G là một nhóm tôpô và $\mathscr{U}= (U_i)_{i\in I}$ là một phủ mở của B.

a) Mọi không gian bó sợi chính trên B với nhóm G có thể tầm thường hóa trên $\mathscr{U}$ đều đẳng cấu với một không gian bó sợi chính được xác định bởi một cocycle của $Z^1_{cont}(B,\mathscr{U},G)$.

b) Cho $(E, p)$ và $(E', p')$ là các không gian bó sợi chính trên B có thể tầm thường hóa trên $\mathscr{U}$. Gọi $(f_i)_{i\in I}($ resp. $(f'_i)_{i\in I})$ là một phép tầm thường hóa của $(E, p)$ ( resp. của $(E', p')$) thích nghi với $\mathscr{U}$, và ký hiệu $(g_{ij})_{(i,j)\in I\times I}$ ( resp. $(g'_{i,j})_{(i,j)\in I\times I}$) là cocycle được xác định bởi phép tầm thường hóa này. Khi đó các không gian bó sợi chính $(E, p)$ và $(E', p')$ là đẳng cấu khi và chỉ khi các cocycle này đồng điều.

Ta chứng minh b). Cho $\varphi : E\rightarrow E'$ là một đẳng cấu của các không gian bó sợi chính với cơ sở B và nhóm G. Với mỗi $i\in I$, gọi $h_i$ là ánh xạ liên tục của $U_i$ vào G được xác định bởi

$$
(b, h_i(b)) =f'_i\circ \varphi \circ f_i^{-1}(b, e)
$$

Vì, với mỗi $i\in I,f_i$ và $f'_i$ tương thích với các phép toán của G, ta có với mọi $b\in U_i$ và mọi $g\in G$,

$$
(f'_i\circ \varphi \circ f_i^{-1})(b, g) = (b, h_i(b)g)
$$

và

$$
(f_i\circ \varphi^{-1}\circ (f'_i)^{-1})(b, g) = (b, h_i(b)^{-1}g)
$$

Do đó, với mọi cặp $(i, j)\in I\times I$ và mọi điểm $b$ của $U_i\cap U_j:$ $f'_i\circ (f'_j)^{-1}(b, e) = (f'_i\circ \varphi \circ f_i^{-1})\circ (f_i\circ f_j^{-1})\circ (f_j\circ \varphi^{-1}\circ (f'_j)^{-1})(b, e)$

$$
= (b, h_i(b)g_{ij}(b)h_j(b)^{-1})
$$

suy ra

$$
g'_{ij}(b) =h_i(b)g_{ij}(b)h_j(b)^{-1}
$$

Điều này chứng minh rằng các cocycle $(g_{ij})$ và $(g'_{ij})$ là đồng điều.

Ngược lại, giả sử rằng các cocycle này đồng điều, và cho $(h_i)_{i\in I}$ là một họ các ánh xạ liên tục $h_i: U_i\rightarrow G$ sao cho $g'_{ij}(b) =h_i(b)g_{ij}(b)h_j(b)^{-1}$ với $i,j\in I$ và $b\in U_i\cap U_j$. Với

$i\in I$, đặt $\varphi_i:\overset{-1}{p}(U_i)\rightarrow (^-{p'}^1)(U_i)$ là ánh xạ được xác định bởi $f'_i\circ \varphi_i\circ$ $f_i^{-1}(b, g) = (b, h_i(b)g)$, với $b\in U_i$ và $g\in G$. Đó là một đẳng cấu của các không gian sợi chính với cơ sở $U_i$ và nhóm G. Với $(i, j)\in$ $I\times I$, ký hiệu $\gamma_{ij}$ và $\gamma '_{ij}$ là các đồng phôi ghép nối liên kết như trên với các cocycle $(g_{ij})$ và $(g'_{ij})$ tương ứng (I, p. 115, công thức (5)), sao cho $f_i(b, g) =\gamma_{ij}\circ f_j(b, g)$ và $f'_i(b, g) =\gamma '_{ij}\circ f'_j(b, g)$ với mọi $(b, g)\in (U_i\cap U_j)\times G$. Do đó, với $(i, j)\in I\times I$ và $(b, g)\in (U_i\cap U_j)\times G$, ta có các hệ thức

$$
f'_i\circ \varphi_j\circ f_i^{-1}(b, g) =\gamma '_{ij}\circ (f'_j\circ \varphi_j\circ f_j^{-1})(b, g_{ij}(b)^{-1}g)
$$

$$
=\gamma '_{ij}(b, h_j(b)g_{ij}(b)^{-1}g)
$$

$$
= (b, g'_{ij}(b)h_j(b)g_{ij}(b)^{-1}g)
$$

$$
= (b, h_i(b)g) =f'_i\circ \varphi_i\circ f_i^{-1}(b, g)
$$

Điều này chứng minh rằng $\varphi_i$ và $\varphi_j$ trùng nhau trên $\overset{-1}{p}(U_i\cap U_j)$. Do đó, các cấu xạ $\varphi_i$ ghép lại thành một cấu xạ B của các không gian sợi chính từ E đến $E'$. Mệnh đề b) được suy ra, vì mọi cấu xạ của các không gian sợi chính có cơ sở B và nhóm G đều là một đẳng cấu (I, p. 93, Mệnh đề 1).

Bây giờ chứng minh a). Cho $(E, p)$ là một không gian sợi chính với nhóm G được trang bị, với mỗi $i\in I$, một phép tầm thường hóa $f_i:\overset{-1}{p}(U_i)\rightarrow$ $U_i\times G$ trên $U_i$. Cho $(g_{ij})$ là cocycle được xác định bởi họ này, và khi đó cho F là không gian sợi chính được xác định bởi cocycle $(g_{ij})$. Theo phép dựng, không gian sợi chính F được trang bị một phép tầm thường hóa trên $\mathscr{U}$; phép tầm thường hóa này xác định cocycle $(g_{ij})$. Theo mệnh đề b), không gian sợi chính $(E, p)$ đẳng cấu với F.

Cho B là một không gian tôpô và G là một nhóm tôpô. Cho $(E, p)$ là một không gian sợi chính có cơ sở B và nhóm G. Cho $s$ là một tiết diện của ánh xạ toàn ánh $p$ (E, II, p. 19, Mệnh đề 8). Ánh xạ $f: B\times G\rightarrow E$ xác định bởi $f(b, g) =s(b)\cdot g$ là một song ánh tương thích với tác động của G. Trang bị cho $B\times G$ tôpô nhận được bởi phép chuyển cấu trúc; $(B\times G$, pr$_1)$ khi đó là một không gian sợi chính có cơ sở B và nhóm G đẳng cấu với E. Do đó tồn tại một tập hợp T các không gian sợi chính có cơ sở B và nhóm G sao cho mọi không gian sợi chính có cơ sở B và nhóm G đều đẳng cấu với một phần tử của T. Ký hiệu $P(B,G)$ là tập hợp các lớp đẳng cấu của các không gian sợi chính có cơ sở B và nhóm G (E, II, p. 47).

Cho $\mathscr{U}= (U_i)_{i\in I}$ là một phủ mở của B. Ký hiệu $P(B,\mathscr{U},G)$ là tập con của $P(B,G)$ gồm các lớp đẳng cấu của các bó chính khả vi tầm thường trên $\mathscr{U}$. Theo mệnh đề 11, tồn tại một ánh xạ $r_{\mathscr{U}}$ từ $H^1_{cont}(B,\mathscr{U},G)$ vào $P(B,\mathscr{U},G)$, ánh xạ lớp của một cocycle $(g_{ij})\in Z^1_{cont}(B,\mathscr{U},G)$ vào lớp đẳng cấu của không gian sợi chính được xác định bởi cocycle này; đó là một song ánh (loc. cit.). Song ánh ngược $s_{\mathscr{U}}$ ánh xạ lớp đẳng cấu trong $H^1_{cont}(B,\mathscr{U},G)$ của một không gian sợi chính E, khả tầm thường trên $\mathscr{U}$, vào lớp của cocycle được xác định bởi một họ tùy ý các phép tầm thường hóa của E trên $\mathscr{U}$. Theo sự tương ứng này, lớp đẳng cấu của không gian sợi chính tầm thường $B\times G$ tương ứng với lớp đối đồng điều của cocycle hằng $g_{ij}=e$, còn được gọi là cocycle tầm thường.

Theo định nghĩa của một không gian sợi chính, tập hợp $P(B,G)$ là hợp của các tập hợp có dạng $P(B,\mathscr{U},G)$, trong đó $\mathscr{U}$ là một phủ mở của B.

Cho $\mathscr{U}= (U_i)_{i\in I}$ là một phủ mở của B và $\mathscr{V}= (V_k)_{k\in K}$ là một phủ mở của B mịn hơn $\mathscr{U}$. Ta có $P(B,\mathscr{U},G)\subset$ $P(B,\mathscr{V},G)$; ký hiệu $i_{\mathscr{V} \mathscr{U}}$ là đơn ánh chính tắc được xác định bởi phép bao hàm này. Chọn một ánh xạ $\varphi : K\rightarrow I$ sao cho $V_k\subset U_{\varphi(k)}$ với mọi $k\in K$. Cho một cocycle $(g_{ij})\in Z^1_{cont}(B,\mathscr{U},G)$, đặt, với mọi cặp $(k, \ell )\in K\times K,\overline{g}_{k\ell}=g_{\varphi(k)\varphi(\ell)}|V_k\cap V_{\ell}$.

Họ $(\overline{g}_{k\ell})$ là một cocycle trên B, nhận giá trị trong G, thuộc $\mathscr{V}$. Nếu $(g'_{ij})\in Z^1_{cont}(B,\mathscr{U},G)$ là một cocycle đồng luân với cocycle $(g_{ij})$, thì cocycle $(\overline{g}'_{k\ell})$ suy ra từ $(g'_{k\ell})$ đồng luân với cocycle $(\overline{g}_{k\ell})$. Do đó tồn tại một ánh xạ

$$
c(\varphi ): H^1_{cont}(B,\mathscr{U},G)\rightarrow H^1_{cont}(B,\mathscr{V},G)
$$

ánh xạ lớp của $(g_{ij})$ vào lớp của $(\overline{g}_{k\ell})$.

Cho E là một không gian sợi chính có cơ sở B và nhóm G và, với mọi $i\in$ I, cho $f_i: E_{U_i}\rightarrow U_i\times G$ là một phép tầm thường hóa của bó chính $U_i$-bundle $E_{U_i}$. Với mọi $k\in$ K, cho $f'_k: E_{V_k}\rightarrow V_k\times G$ là phép tầm thường hóa suy ra từ $f_{\varphi(k)}$ bằng cách chuyển qua các tập con. Cho $(g_{ij})\in Z^1_{cont}(B,\mathscr{U},G)$ là cocycle được xác định bởi họ $(f_i)$; cocycle được xác định bởi họ $(f'_k)$ chính xác là cocycle $(\overline{g}_{k\ell})$ đã định nghĩa ở trên. Do đó, biểu đồ sau là giao hoán:

$$
H^1_{cont}(B,\mathscr{U},G)^{c(\varphi)}H^1_{cont}(B,\mathscr{V},G)
$$

$r_{\mathscr{U}}r_{\mathscr{V}}$

$$
P(B,\mathscr{U},G)^{i_{\mathscr{V} \mathscr{U}}}P(B,\mathscr{V},G)
$$

Vì các ánh xạ $r_{\mathscr{U}}$ và $r_{\mathscr{V}}$ là các song ánh, ánh xạ $c(\varphi )$, tương tự như $i_{\mathscr{V} \mathscr{U}}$, là một đơn ánh và không phụ thuộc vào lựa chọn $\varphi$. Từ nay về sau, ta sẽ viết $c_{\mathscr{V} \mathscr{U}}$ thay cho $c(\varphi )$.

Cho $\mathscr{R}$ là tập hợp các phần tử của $\mathfrak{P}(\mathfrak{P}(B))$ là các phủ mở của B. Với mọi phủ mở $\mathscr{U}$ của B, tồn tại một phủ mở $\mathscr{V}$ thuộc $\mathscr{R}$ sao cho $\mathscr{U}$ vừa mịn hơn vừa thô hơn $\mathscr{U}$. Tập hợp $\mathscr{R}$ có thứ tự và lọc theo quan hệ $\leqslant$ được định nghĩa bởi $\mathscr{U}\leqslant \mathscr{V}$ nếu $\mathscr{V}$ là một phủ mịn hơn $\mathscr{U}$. Theo những điều trên, một hệ quy nạp $(H^1_{cont}(B,\mathscr{U},G), c_{\mathscr{V} \mathscr{U}})$ đối với tập hợp có thứ tự lọc $\mathscr{R}$ đã được xác định và họ $(r_{\mathscr{U}})$ là một hệ quy nạp các ánh xạ song ánh từ $(H^1_{cont}(B,\mathscr{U},G), c_{\mathscr{V} \mathscr{U}})$ vào $(P(B,\mathscr{U},G), i_{\mathscr{V} \mathscr{U}})$. Nếu ký hiệu $H^1_{cont}(B,G)$ là giới hạn quy nạp của hệ $(H^1_{cont}(B,\mathscr{U},G), c_{\mathscr{V} \mathscr{U}})$ và $r: H^1_{cont}(B,G)\rightarrow P(B,G)$ là giới hạn quy nạp của họ $(r_{\mathscr{U}})$, thì ta có:

#### Định lý 4 {#ta-i-s5-thm-4 .statement tag=01RQ}

Ánh xạ $r: H^1_{cont}(B,G)\rightarrow P(B,G)$ là song ánh.

Cho $\mathscr{U}= (U_i)_{i\in I}$ là một phủ mở của B; ký hiệu $c_{\mathscr{U}}$ là ánh xạ chính tắc $H^1_{cont}(B,\mathscr{U},G)\rightarrow H^1_{cont}(B,G)$. Nếu $(g_{ij})$ là một cocycle trên B, lấy giá trị trong G, thuộc phủ mở $\mathscr{U}$, thì phần tử $c_{\mathscr{U}}((g_{ij}))$ của $H^1_{cont}(B,G)$ được gọi là lớp đối đồng điều của cocycle $(g_{ij})$.

## BÀI TẬP {#ta-i-s5-exercises}

Xem [các bài tập của § 5](exercises/s5/).
