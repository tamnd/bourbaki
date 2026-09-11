---
book: ac
book_title: Commutative Algebra
chapter: X
chapter_title: Profondeur, régularité, dualité
section: 7
section_title: Algèbres lisses
lang: vi
source: ac-x-fr
book_pages: AC X.170-AC X.173
pdf_pages: 0082-0103, 0169-0172
extraction: ocr
subsections:
    - "no": 1
      title: Dérivations et relèvements d’homomorphismes
      page: 0
      pdf_page: 82
    - "no": 2
      title: Algèbres formellement lisses
      page: 84
      pdf_page: 83
    - "no": 3
      title: Exemples d’algèbres formellement lisses
      page: 87
      pdf_page: 86
    - "no": 4
      title: Relèvements d’homomorphismes dans les algèbres filtrées complètes
      page: 89
      pdf_page: 88
    - "no": 5
      title: Quotients formellement lisses d’algèbres
      page: 90
      pdf_page: 89
    - "no": 6
      title: Extension du corps de base dans les algèbres régulières (caractéristique non nulle)
      page: 0
      pdf_page: 91
    - "no": 7
      title: Un critère pour les algèbres locales formellement lisses
      page: 95
      pdf_page: 94
    - "no": 8
      title: Existence de rétractions pour les applications linéaires
      page: 0
      pdf_page: 96
    - "no": 9
      title: Le critère jacobien
      page: 98
      pdf_page: 97
    - "no": 10
      title: Algèbres lisses
      page: 102
      pdf_page: 101
statements: 39
exercises: 15
content_sha256: 36dc295b493999400fd3a8dc7dd1ab91360ca374a9facb9eee26d080435245e6
translated_from: content/en-mt/ac/X/07_s7_algebres_lisses.md
source_lang: en-mt
translation_method: machine
source_content_sha256: aaa34242d598f6821b0738736697b9b060d8724ab44b075a978f529e09bfce6c
translation_model: gpt-5.4
translation_run: translate-vi-65bb4a06
glossary_version: 34
glossary_terms_sha256: a5f8bb4f5717d2b9911457f7bb573517e88c7238cf3a01bcf6c21f9392f347e2
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 7. ĐẠI SỐ TRƠN

### 1. Các đạo hàm và các phép nâng của đồng cấu

Cho $k$ là một vành, $C$ là một $k$-đại số và $N$ là một iđêan của $C$ có bình phương bằng không. Gọi $\pi : C \to C/N$ là đồng cấu chính tắc; vì $N^2 = \{0\}$, cấu trúc $C$-môđun trên $N$ xuất phát từ một cấu trúc $C/N$-môđun.

Cho $A$ là một $k$-đại số và $\varphi : A \to C/N$ là một đồng cấu các $k$-đại số. Trang bị cho $N$ cấu trúc $A$-môđun suy ra từ $\varphi$. Một *phép nâng của $\varphi$* (lên $C$) được hiểu là mọi đồng cấu các $k$-đại số $\tilde{\varphi} : A \to C$ sao cho $\pi \circ \tilde{\varphi} = \varphi$. Cho $\tilde{\varphi}$ là một phép nâng như vậy, và $\delta$ là một ánh xạ từ $A$ vào $N$; gọi $\delta + \tilde{\varphi}$ là ánh xạ $x \mapsto \delta(x) + \tilde{\varphi}(x)$ từ $A$ vào $C$.

#### Mệnh đề 1 {#ac-x-s7-prop-1 .statement}

*Nếu $\varphi$ thừa nhận một phép nâng, thì ánh xạ $(\delta, \tilde{\varphi}) \mapsto \delta + \tilde{\varphi}$ xác định một phép toán đơn bắc cầu của nhóm các $k$-đạo hàm từ $A$ vào $N$ trên tập hợp các phép nâng của $\varphi$.*

Cho $\tilde{\varphi}_0 : A \to C$ là một phép nâng của $\varphi$. Ánh xạ $\delta \mapsto \delta + \tilde{\varphi}_0$ gây ra một song ánh từ tập hợp các ánh xạ từ $A$ vào $N$ lên tập hợp các ánh xạ $\tilde{\varphi} : A \to C$ sao cho $\pi \circ \tilde{\varphi} = \varphi$. Giữ cố định $\delta$, và đặt $\tilde{\varphi} = \delta + \tilde{\varphi}_0$. Để $\tilde{\varphi}$ là một đồng cấu các $k$-đại số, điều kiện cần và đủ là $\delta$ là một $k$-đạo hàm từ $A$ vào $N$: thật vậy, với $x, y$ trong $A$ và $\lambda$ trong $k$, ta có các đẳng thức

$$
\begin{align*}
\tilde{\varphi}(x + y) - \tilde{\varphi}(x) - \tilde{\varphi}(y) &= \delta(x + y) - \delta(x) - \delta(y) \\
\tilde{\varphi}(\lambda x) - \lambda \tilde{\varphi}(x) &= \delta(\lambda x) - \lambda \delta(x) \\
\tilde{\varphi}(xy) - \tilde{\varphi}(x)\tilde{\varphi}(y) &= \delta(xy) - \delta(x)\delta(y) - \delta(x)\tilde{\varphi}_0(y) - \tilde{\varphi}_0(x)\delta(y) \\
&= \delta(xy) - \varphi(x)\delta(y) - \varphi(y)\delta(x),
\end{align*}
$$

đẳng thức cuối cùng thu được từ sự kiện rằng $N$ có bình phương bằng không. Mệnh đề được suy ra từ đó.

#### Ví dụ {#ac-x-s7-n1-exa-1 .statement}

Cho $B$ là một $k$-đại số, $N$ là một $B$-môđun. Trang bị cho $k$-môđun $B \oplus N$ một cấu trúc $k$-đại số được xác định bởi $(b, x)(b', x') = (bb', bx' + b'x)$ (*xem* A, III, p. 127), sao cho $N$ là một iđêan bình phương-không của $B \oplus N$. Cho $\varphi : A \to B$ là một đồng cấu các $k$-đại số. Khi đó các phép nâng của $\varphi$ lên $B \oplus N$ là các ánh xạ $x \mapsto (\varphi(x), \delta(x))$, trong đó $\delta$ chạy qua tập hợp các $k$-đạo hàm từ $A$ vào $N$ (*xem loc. cit.*, mệnh đề 12).

Cho $\Omega_k(A)$ là môđun các $k$-vi phân của vành $A$, và cho $d : A \longrightarrow \Omega_k(A)$ là $k$-đạo hàm phổ quát (A, III, p. 133 and 134); ta nhắc lại (*loc. cit.*) rằng với mọi $A$-môđun $M$, ánh xạ $v \mapsto v \circ d$ là một đẳng cấu $A$-tuyến tính từ $\mathrm{Hom}_A(\Omega_k(A), M)$ lên $A$-môđun các $k$-đạo hàm từ $A$ vào $M$.

Cho J là một iđêan của A. Theo A, III, p. 137, ta có một dãy khớp các ánh xạ $A/J$-tuyến tính

$$
J/J^2 \xrightarrow{\bar{d}} (\Lambda/J) \otimes_A \Omega_k(\Lambda) \longrightarrow \Omega_k(A/J) \to 0,
$$

trong đó $\bar{d}$ là đồng cấu cảm sinh, bằng cách chuyển qua thương, từ hạn chế của $d$ lên J.

Kí hiệu $\rho : A \to A/J^2$ và $\pi : A/J^2 \to A/J$ là các toàn cấu chính tắc. Cho $v : (A/J) \otimes_A \Omega_k(A) \longrightarrow J/J^2$ là một ánh xạ $k$-tuyến tính; với nó ta kết hợp một ánh xạ $k$-tuyến tính $H_v : A \to A/J^2$ bằng cách đặt $H_v(x) = \rho(x) - v(1 \otimes dx)$. Nếu $v$ là một phân rã của $\bar{d}$, thì $H_v$ triệt tiêu trên J, do đó cảm sinh, bằng cách chuyển qua thương, một ánh xạ $k$-tuyến tính $h_v : A/J \to A/J^2$. Mặt khác, với một ánh xạ $k$-tuyến tính $h : A/J \to A/J^2$ đã cho, kí hiệu $\psi_h : A/J \oplus J/J^2 \longrightarrow A/J^2$ là ánh xạ $(x, y) \mapsto h(x) + y$.

#### Mệnh đề 2 {#ac-x-s7-prop-2 .statement}

Trang bị cho $k$-môđun $\Lambda/J \oplus J/J^2$ cấu trúc của một $k$-đại số được xác định như trong ví dụ trên. Các ánh xạ $v \mapsto h_v$ và $h \mapsto \psi_h$ cảm sinh các song ánh giữa các tập hợp sau :

(i) tập hợp các phép rút $A/J$-tuyến tính $v$ của $\bar{d}$ ;
(ii) tập hợp các đồng cấu $k$-đại số $h : A/J \to A/J^2$ sao cho $\pi \circ h = \mathrm{Id}_{A/J}$ ;
(iii) tập hợp các đẳng cấu $k$-đại số $\psi : A/J \oplus J/J^2 \longrightarrow A/J^2$ sao cho $\pi \circ \psi = \mathrm{pr}_1$ và $\psi(0, z) = z$ với $z \in J/J^2$.

Áp dụng Mệnh đề 1 với $C = A/J^2$ và $N = J/J^2$. Cho $\varphi : A \to A/J$ là toàn cấu chính tắc ; đồng cấu $\rho$ là một phép nâng của $\varphi$ lên $A/J^2$. A-môđun $\mathrm{Hom}_{A/J}((A/J) \otimes_A \Omega_k(A), J/J^2)$ được đồng nhất với $\mathrm{Hom}_A(\Omega_k(A), J/J^2)$ ; theo Mệnh đề 1, ánh xạ $v \mapsto H_v$ là một song ánh từ tập hợp này lên tập hợp các phép nâng của $\varphi$ lên $A/J^2$. Với $x \in J$, ta có $1 \otimes dx = \bar{d}(\rho(x))$ ; để $H_v$ triệt tiêu trên J, điều kiện cần và đủ là $v \circ \bar{d}$ là ánh xạ đồng nhất của $J/J^2$. Điều này chứng minh rằng ánh xạ $v \mapsto h_v$ gây ra một song ánh giữa hai tập hợp đầu được mô tả trong mệnh đề.

Ánh xạ $h \mapsto \psi_h$ là một song ánh từ tập hợp các đồng cấu $k$-tuyến tính của $A/J$ vào $A/J^2$ lên tập hợp các đồng cấu $k$-tuyến tính $\psi : A/J \oplus J/J^2 \longrightarrow A/J^2$ sao cho $\psi(0, z) = z$ với $z \in J/J^2$ ; hơn nữa, để có $\pi \circ \psi_h = \mathrm{pr}_1$, điều kiện cần và đủ là $\pi \circ h = \mathrm{Id}_{A/J}$, nghĩa là $z \equiv h(\pi(z)) \pmod{J/J^2}$ với mọi $z \in A/J^2$. Giả sử các điều kiện này được thỏa mãn. Để $h$ là một đồng cấu vành, điều kiện cần và đủ là điều tương tự đúng cho $\psi_h$ ; hơn nữa, đồng cấu $\psi_h$ là song ánh : ánh xạ nghịch đảo gắn cho một phần tử $z$ của $A/J^2$ cặp $(\pi(z), z - h(\pi(z)))$. Điều này chứng minh rằng ánh xạ $h \mapsto \psi_h$ gây ra một song ánh giữa hai tập hợp cuối được mô tả trong mệnh đề.

### 2. Các đại số trơn hình thức

Cho $k$ là một vành và $A$ là một $k$-đại số tôpô tuyến tính (III, § 4, No. 2, Def. 1).

#### Định nghĩa 1 {#ac-x-s7-def-1 .statement}

Người ta nói rằng $A$ là trơn hình thức trên $k$, hay là một $k$-đại số trơn hình thức, nếu nó thỏa mãn điều kiện sau: với mọi $k$-đại số $C$ và mọi iđêan bình phương-không $N$ của $C$, mọi đồng cấu liên tục từ $A$ vào $k$-đại số $C/N$, được trang bị tôpô rời rạc, đều có thể nâng lên thành một đồng cấu liên tục từ $A$ vào $k$-đại số $C$, được trang bị tôpô rời rạc.

Nhắc lại rằng một đồng cấu từ $A$ vào một $k$-đại số được trang bị tôpô rời rạc là liên tục khi và chỉ khi hạt nhân của nó là mở.

Cho $k$ là một vành, $A$ là một $k$-đại số và $J$ là một iđêan của $A$. Trang bị cho $A$ tôpô $J$-adic. Cho $C$ là một $k$-đại số, $N$ là một iđêan bình phương-không của $C$; trang bị cho $C$ và $C/N$ tôpô rời rạc. Cho $\varphi : A \to C/N$ là một đồng cấu đại số liên tục. Mọi phép nâng $\tilde{\varphi} : A \to C$ của $\varphi$ đều liên tục: thật vậy, tồn tại một số nguyên $n$ sao cho $\varphi(J^n)$ bằng không, và ta có $\tilde{\varphi}(J^n) \subset N$, do đó $\tilde{\varphi}(J^{2n}) \subset N^2 = 0$. Đặc biệt suy ra rằng, nếu $A$ là trơn hình thức đối với tôpô $J$-adic, thì nó cũng trơn hình thức đối với tôpô $J'$-adic với mọi iđêan $J'$ chứa $J$.

Ta sẽ nói rằng một $k$-đại số $A$ là trơn hình thức nếu nó trơn hình thức khi được trang bị tôpô rời rạc, nghĩa là tôpô $(0)$-adic; khi đó nó là trơn hình thức đối với tôpô $J$-adic, bất kể iđêan $J$ của $A$ là gì.

#### Nhận xét 1 {#ac-x-s7-n2-rem-1 .statement}

Cho $k$ là một vành, $A$ là một $k$-đại số và $J$ là một iđêan của $A$. Nếu $k$-đại số $A/J$ là trơn hình thức (đối với tôpô rời rạc), thì ánh xạ đồng nhất của $A/J$ chấp nhận một phép nâng lên $A/J^2$; do đó các tập hợp được mô tả trong Mệnh đề 2 là không rỗng. Đặc biệt, dãy

$$
0 \to J/J^2 \xrightarrow{\bar{d}} (A/J) \otimes_A \Omega_k(A) \longrightarrow \Omega_k(A/J) \to 0
$$

là khớp và tách.

#### Nhận xét 2 {#ac-x-s7-n2-rem-2 .statement}

Cho $k$ là một vành, $A$ là một $k$-đại số được tôpô hóa tuyến tính hình thức trơn, $M$ là một A-môđun mà linh hóa tử của nó là mở trong $A$. Khi đó mọi đạo hàm $\delta$ từ $k$ vào $M$ đều kéo dài được thành một đạo hàm từ $A$ vào $M$. Thật vậy, đặt $B = A/Ann(M)$; ánh xạ $\lambda \mapsto (\lambda 1_B, \delta(\lambda))$ xác định một đồng cấu vành từ $k$ vào $B \oplus M$ (No. 1, Ví dụ), tức là một cấu trúc $k$-đại số trên $B \oplus M$. Toàn cấu chính tắc $\varphi : A \to B$ là liên tục, và do đó nhận được một nâng $\tilde{\varphi} : A \to B \oplus M$; theo loc. cit., $pr_2 \circ \tilde{\varphi}$ là một đạo hàm từ $A$ vào $M$ kéo dài $\delta$.

#### Mệnh đề 3 {#ac-x-s7-prop-3 .statement}

Cho $k$ là một vành.

a) Cho $A$ và $B$ là các $k$-đại số được tôpô hóa tuyến tính và $\rho : A \to B$ là một đồng cấu liên tục các $k$-đại số. Nếu $A$ hình thức trơn trên $k$ và $B$ hình thức trơn trên $A$, thì $B$ hình thức trơn trên $k$.

b) Tích $k$-đại số của một họ hữu hạn các $k$-đại số được tôpô hóa tuyến tính hình thức trơn là hình thức trơn.

c) Cho $A$ là một $k$-đại số được tôpô hóa tuyến tính, và $\hat{A}$ là đại số hoàn thành tách của $A$; điều kiện cần và đủ để $A$ hình thức trơn trên $k$ là $\hat{A}$ cũng có tính chất đó.

Cho C là một $k$-đại số, N là một iđêan bình phương-không của C, và $\pi : C \to C/N$ là toàn cấu chính tắc. Trang bị cho C và C/N tôpô rời rạc.

a) Cho $\psi : B \to C/N$ là một đồng cấu liên tục các $k$-đại số. Vì A hình thức trơn trên $k$, tồn tại một đồng cấu liên tục các $k$-đại số $\tilde{\varphi} : A \to C$ sao cho $\pi \circ \tilde{\varphi} = \psi \circ \rho$.

$$
\begin{array}{ccc}
 & & C \\
 & \swarrow_{\tilde{\varphi}} & \\
A \xrightarrow{\rho} B \xrightarrow{\psi} C/N & & \downarrow^{\pi}
\end{array}
$$

Xem C và C/N như các A-đại số thông qua $\tilde{\varphi}$, để $\psi$ là một đồng cấu các A-đại số; vì B hình thức trơn trên A, tồn tại một đồng cấu liên tục các A-đại số $\tilde{\psi} : B \to C$ sao cho $\pi \circ \tilde{\psi} = \psi$, do đó a).

b) Chỉ cần chứng minh rằng tích của hai $k$-đại số trơn hình thức $A_1$ và $A_2$ là trơn hình thức. Cho $\varphi : A_1 \times A_2 \to C/N$ là một đồng cấu liên tục của các $k$-đại số. Đặt $e_1 = \varphi(1,0)$, $e_2 = \varphi(0,1)$, sao cho $e_1$ và $e_2$ là các phần tử lũy đẳng trực giao trong C/N. Gọi $\varphi_1 : A_1 \to (C/N)e_1$ và $\varphi_2 : A_2 \to (C/N)e_2$ là các ánh xạ được xác định bởi $\varphi_1(a_1) = \varphi(a_1,0)$ và $\varphi_2(a_2) = \varphi(0,a_2)$; đó là các đồng cấu liên tục của các $k$-đại số, và ta có $\varphi(a_1, a_2) = \varphi_1(a_1) + \varphi_2(a_2)$ với mọi $(a_1, a_2) \in A_1 \times A_2$. Tồn tại một phần tử lũy đẳng $\tilde{e}_1$ của C sao cho $\pi(\tilde{e}_1) = e_1$ (A, VIII, § 9, No. 4, Prop. 7); đặt $\tilde{e}_2 = 1 - \tilde{e}_1$, khi đó $\pi(\tilde{e}_2) = e_2$. Với $i = 1, 2$, đồng cấu $C\tilde{e}_i \to (C/N)e_i$ cảm sinh bởi $\pi$ là toàn ánh, với hạt nhân $N\tilde{e}_i$; vì $k$-đại số $A_i$ là trơn hình thức, đồng cấu $\varphi_i$ thừa nhận một nâng liên tục $\tilde{\varphi}_i$ lên $C\tilde{e}_i$. Ánh xạ $(a_1, a_2) \mapsto \tilde{\varphi}_1(a_1) + \tilde{\varphi}_2(a_2)$ là một nâng liên tục của $\varphi$ lên C.

c) Gọi $i : A \to \widehat{A}$ là đồng cấu chính tắc. Với mọi vành D, được trang bị tôpô rời rạc, ánh xạ liên kết với một đồng cấu liên tục $f : \widehat{A} \to D$ đồng cấu liên tục $f \circ i : A \to D$ là song ánh. Mệnh đề c) suy ra từ điều này.

Mệnh đề c) của mệnh đề áp dụng đặc biệt khi tôpô của $\Lambda$ là tôpô J-adic, trong đó J là một iđêan kiểu hữu hạn; bao đóng $\widehat{J}$ của J trong $\widehat{A}$ khi đó bằng $JA$ và tôpô của $\widehat{A}$ là tôpô $\widehat{J}$-adic (III, § 2, No. 12, Hệ quả 2 of Prop. 16). Do đó, nói rằng A là trơn hình thức đối với tôpô J-adic hay rằng hoàn thành tách của nó $\widehat{A}$ là trơn hình thức đối với tôpô J-adic là tương đương.

#### Mệnh đề 4 {#ac-x-s7-prop-4 .statement}

Cho k là một vành, A và B các $k$-đại số, J một iđêan của A, K một iđêan của B.

a) Cho S là một tập con nhân tính của A và T một tập con của k mà ảnh của nó trong A được chứa trong S. Nếu A là trơn hình thức trên k đối với tôpô J-adic, S $^1\Lambda$ là trơn hình thức trên $T^{-1}k$ đối với tôpô $S^{-1}J$-adic.

b) Cho $k'$ là một $k$-đại số. Nếu $A$ là trơn hình thức trên $k$ đối với tôpô $J$-adic, thì $k'$-đại số $A_{(k')}$ là trơn hình thức trên $k'$ đối với tôpô $JA_{(k')}$-adic.

c) Ký hiệu $I$ là iđêan của $A \otimes_k B$ sinh bởi các ảnh của $J \otimes_k B$ và $A \otimes_k K$. Nếu $A$ và $B$ hình thức trơn trên $k$ tương ứng đối với các tôpô $J$-adic và $K$-adic, thì $k$-đại số $A \otimes_k B$ hình thức trơn đối với tôpô $I$-adic.

a) Dưới các giả thiết của a), cho $C$ là một $T^{-1}k$-đại số, và $N$ là một iđêan bình phương bằng không của $C$; trang bị cho $C$ và $C/N$ tôpô rời rạc, và ký hiệu $\pi : C \to C/N$ là toàn cấu chính tắc. Cho $\varphi : S^{-1}A \longrightarrow C/N$ là một đồng cấu $T^{-1}k$-đại số, liên tục đối với tôpô $S^{-1}J$-adic. Ký hiệu $i$ là đồng cấu chính tắc của $A$ vào $S^{-1}A$. Ánh xạ $\varphi \circ i$ là một đồng cấu $k$-đại số, liên tục đối với tôpô $J$-adic, và do đó chấp nhận một phép nâng $\tilde{\varphi}_0 : A \to C$. Các phần tử của $\tilde{\varphi}_0(S)$ khả nghịch modulo $N$, nên khả nghịch vì $N$ có bình phương bằng không. Suy ra tồn tại một đồng cấu vành $\tilde{\varphi} : S^{-1}A \to C$ sao cho $\tilde{\varphi} \circ i = \tilde{\varphi}_0$ (II, § 2, No. 1, Mệnh đề 1); theo Hệ quả 3 của Mệnh đề 2 của loc. cit., $\tilde{\varphi}$ là $T^{-1}k$-tuyến tính. Ta có $\pi \circ \tilde{\varphi} \circ i = \varphi \circ i$, do đó $\pi \circ \tilde{\varphi} = \varphi$ (loc. cit., Mệnh đề 1), nên $\tilde{\varphi}$ là một phép nâng của $\varphi$.

b) Giả sử các giả thiết của b) được thỏa mãn. Cho $C$ là một $k'$-đại số, $N$ là một iđêan có bình phương bằng không của $C$; trang bị cho $C$ và $C/N$ tôpô rời rạc. Cho $\varphi : A_{(k')} \longrightarrow C/N$ là một đồng cấu $k'$-đại số, liên tục đối với tôpô $JA_{(k')}$-adic. Ký hiệu $i : A \to A_{(k')}$ là đồng cấu chính tắc. Ánh xạ $\varphi \circ i$ là một đồng cấu $k$-đại số từ $A$ vào $C/N$, liên tục đối với tôpô $J$-adic; nếu $A$ là trơn hình thức trên $k$ đối với tôpô $J$-adic, thì $\varphi \circ i$ nhận được một nâng $\tilde{\psi} : A \to C$. Đồng cấu $k'$-đại số $\tilde{\varphi} : A_{(k')} \longrightarrow C$ suy ra từ $\tilde{\psi}$ là một nâng của $\varphi$.

c) Giả sử các giả thiết của c) được thỏa mãn. $B$-đại số $A \otimes_k B$ là trơn hình thức đối với tôpô $J(A \otimes_k B)$-adic theo b), nên cũng trơn hình thức đối với tôpô $I$-adic; hơn nữa đồng cấu chính tắc $B \to A \otimes_k B$ là liên tục khi $B$ được trang bị tôpô $K$-adic và $A \otimes_k B$ được trang bị tôpô $I$-adic. Do đó mệnh đề c) suy ra từ mệnh đề 3, a).

### 3. Ví dụ về các đại số trơn hình thức

Cho $k$ là một vành.

1) Cho $P$ là một $k$-môđun xạ ảnh. $k$-đại số đối xứng $S_k(P)$ là trơn hình thức đối với tôpô rời rạc, và a fortiori đối với tôpô xác định bởi phân bậc của nó. Thật vậy, với mọi $k$-đại số $C$ và mọi iđêan $N$ của $C$, các đồng cấu đại số từ $S_k(P)$ vào $C$ (resp. $C/N$) tương ứng song ánh với các ánh xạ $k$-tuyến tính từ $P$ vào $C$ (resp. $C/N$), và ánh xạ chính tắc $\mathrm{Hom}_k(P, C) \to \mathrm{Hom}_k(P, C/N)$ là toàn ánh.

Do đó (mệnh đề 3, c)), $k$-đại số $\hat{S}_k(P) = \prod_{n \geq 0} S_k^n(P)$ là trơn hình thức (đối với tôpô tích của các tôpô rời rạc trên các $S_k^n(P)$): thật vậy nó là phép hoàn thành của $k$-đại số $S_k(P)$ đối với tôpô xác định bởi phân bậc.

2) Với mọi họ bất định $\mathbf{T} = (T_i)_{i \in I}$, đại số đa thức $k$ $k[\mathbf{T}]$, và đại số chuỗi lũy thừa hình thức $k$ $k[[\mathbf{T}]]$ được trang bị tôpô chính tắc của nó, đều là trơn hình thức; điều này suy ra từ ví dụ 1. Nếu $k$ là một trường, mở rộng siêu việt thuần túy $k(\mathbf{T})$ là trơn hình thức (No. 2, Mệnh đề 4 a)).

3) Cho $f \in k[T]$ là một đa thức theo một bất định. Nói rằng $k$-đại số $k[T]/(f)$ là trơn hình thức tức là nói rằng tính chất sau được thỏa mãn: *với mọi $k$-đại số $C$ và mọi iđêan bình phương bằng không $N$ của $C$, mọi nghiệm của $f$ trong $C/N$ đều có thể nâng thành một nghiệm của $f$ trong $C$*. Điều này đúng khi $f$ và đạo hàm $f'$ của nó sinh iđêan đơn vị. Thật vậy, giả sử $\alpha$ là một nghiệm của $f$ trong $C/N$ và $a$ là một phần tử của $C$ nâng $\alpha$. Khi đó $f(a)$ thuộc $N$ và do đó $f'(a)$ khả nghịch trong $C$; phần tử $b = a - f'(a)^{-1} f(a)$ nâng $\alpha$. Vì $f'(a)^{-1} f(a)$ có bình phương bằng không, ta có

$$
f(b) = f(a) - f'(a) f'(a)^{-1} f(a) = 0 .
$$

**Định lý 1** (I. S. Cohen). *Cho $k$ là một trường và $K$ là một mở rộng tách được của $k$. Khi đó $K$ là một $k$-đại số trơn hình thức.*

Cho $C$ là một $k$-đại số, $N$ là một iđêan bình phương bằng không của $C$, $\pi : C \to C/N$ là đồng cấu chính tắc và $\varphi : K \to C/N$ là một đồng cấu $k$-đại số. Ta phải xây dựng một phép nâng của $\varphi$. Ta phân biệt hai trường hợp.

A) Trước hết giả sử $k$ có đặc số 0. Xét các cặp $(K', \tilde{\varphi}')$, trong đó $K'$ là một mở rộng con của $K$ và $\tilde{\varphi}' : K' \to C$ là một nâng của hạn chế của $\varphi$ trên $K'$. Tập hợp các cặp ấy, được trang bị thứ tự xác định bởi quan hệ mở rộng, là quy nạp; theo định lý Zorn (E, III, p. 20, định lý 2), tồn tại một cặp cực đại $(K', \tilde{\varphi}')$. Ta hãy chứng minh rằng $K'$ bằng $K$. Lấy $x \in K - K'$. Nếu $x$ là siêu việt trên $K'$, thì $K'$-đại số $K'(x)$ là trơn hình thức (ví dụ 2). Nếu $x$ là đại số trên $K'$, thì đa thức tối tiểu của nó $f \in K'[T]$ nguyên tố cùng nhau với đạo hàm của nó (A, V, p. 37, mệnh đề 4), và $K'(x)$ được đồng nhất với $K'$-đại số $K'[T]/(f)$, do đó là một $K'$-đại số trơn hình thức (ví dụ 3). Trong cả hai trường hợp, $K'(x)$ là trơn hình thức trên $K'$, và tồn tại một mở rộng của $\tilde{\varphi}'$ đến $K'(x)$ nâng hạn chế của $\varphi$ trên $K'(x)$, điều này mâu thuẫn với tính chất cực đại của $(K', \tilde{\varphi}')$.

B) Giả sử rằng $k$ có đặc số $p \neq 0$. Xét đồng cấu vành $F : C \to C$ sao cho $F(x) = x^p$; ta có $F(x) = 0$ với $x \in N$, nên tồn tại một đồng cấu vành duy nhất $\lambda : C/N \to C$ sao cho $\lambda \circ \pi = F$. Ta có $\pi(\lambda(\pi(x))) = \pi(x^p) = \pi(x)^p$; vì $\pi$ là toàn ánh, do đó ta có $\pi(\lambda(z)) = z^p$ với mọi phần tử $z$ của $C/N$. Hơn nữa, ký hiệu $f : K \to K^p$ là đẳng cấu $y \mapsto y^p$ và $f^{-1} : K^p \to K$ là đẳng cấu nghịch đảo. Gọi $g : K^p \to C$ là hợp thành của dãy các đồng cấu vành

$$
\begin{array}{ccccccccc}
K^p & \xrightarrow{f^{-1}} & K & \xrightarrow{\varphi} & C/N & \xrightarrow{\lambda} & C .
\end{array}
$$

Với mọi $x \in K$, ta có $g(x^p) = \lambda(\varphi(x))$. Vì $\lambda(\alpha z) = \alpha^p \lambda(z)$ với $\alpha \in k$ và $z \in C/N$, ánh xạ $g$ là $k^p$-tuyến tính. Vì mở rộng $K$ của $k$ là tách được, $k(K^p)$ được đồng nhất với $k \otimes_{k^p} K^p$ (A, V, p. 119, nhận xét); do đó tồn tại một đồng cấu duy nhất các $k$-đại số $h : k(K^p) \to C$ trùng với $g$ trên $K^p$.

Cho $(a_i)_{i \in I}$ là một $p$-cơ sở của $K$ trên $k(K^p)$ (A, V, p. 98, định lý 2); với mọi $i \in I$, chọn một phần tử $b_i$ của $C$ sao cho $\pi(b_i) = \varphi(a_i)$. Ta có $h(a_i^p) = g(a_i^p) = \lambda(\varphi(a_i)) = \lambda(\pi(b_i)) = b_i^p$ với mọi $i \in I$. Theo A, V, p. 94, nhận xét, tồn tại một đồng cấu các $k$-đại số $\tilde{\varphi} : K \to C$, mở rộng $h$ và sao cho $\tilde{\varphi}(a_i) = b_i$ với mọi $i$. Ta có $\pi(\tilde{\varphi}(a_i)) = \pi(b_i) = \varphi(a_i)$ với mọi $i$ và $\pi(\tilde{\varphi}(x^p)) = \pi(h(x^p)) = \pi(g(x^p)) = \pi(\lambda(\varphi(x))) = \varphi(x^p)$ với mọi $x \in K$. Do đó $\pi \circ \tilde{\varphi} = \varphi$, điều này kết thúc chứng minh.

#### Hệ quả {#ac-x-s7-n3-cor-1 .statement}

Cho $k$ là một trường, $K$ là một mở rộng tách được của $k$ và $A$ là một $K$-đại số tôpô tuyến tính. Nếu $A$ trơn hình thức trên $K$ thì nó trơn hình thức trên $k$.

Điều này suy ra từ định lý và mệnh đề 3 a) của No. 2.

#### Nhận xét 1 {#ac-x-s7-n3-rem-1 .statement}

Cho $k$ là một trường. Mọi $k$-đại số étale (A, V, p. 28, def. 1) đều trơn hình thức (*loc. cit.*, p. 34, th. 4, d) và No. 2, prop. 3, b)).

#### Nhận xét 2 {#ac-x-s7-n3-rem-2 .statement}

Ta sẽ thấy dưới đây (hệ quả 2 của định lý 2 của No. 5) rằng một mở rộng trường trơn hình thức thì chính quy tuyệt đối, do đó tách được (§ 6, No. 4, ví dụ 2).

### 4. Nâng các đồng cấu trong các đại số lọc đầy đủ

Cho $k$ là một vành, $C$ là một $k$-đại số, $(C_n)_{n \in \mathbf{Z}}$ là một lọc giảm của $C$, tương thích với cấu trúc $k$-đại số và sao cho $C_0 = C$ (III, § 2, No. 1). Giả sử rằng $C$ tách biệt và đầy đủ đối với tôpô xác định bởi lọc này, để ánh xạ chính tắc $C \to \varprojlim C/C_n$ là một đồng phôi (*loc. cit.*, No. 6). Cho $m$ là một số nguyên $> 0$; ký hiệu bởi $\pi : C \to C/C_m$ toàn cấu chính tắc.

#### Mệnh đề 5 {#ac-x-s7-prop-5 .statement}

Cho $A$ là một đại số trên $k$ tôpô tuyến tính trơn hình thức. Mọi đồng cấu liên tục của các đại số trên $k$ $\varphi : \Lambda \to C/C_m$ đều có một nâng liên tục lên $C$.

Với mọi số nguyên $n > m$, ký hiệu $\pi_n : C/C_n \to C/C_{n-1}$ là toàn cấu chính tắc. Vì $C$ được đồng nhất với giới hạn xạ ảnh của các $C/C_n$, việc cho một nâng liên tục của $\varphi$ lên $C$ tương đương với việc cho một họ $(\varphi_n)_{n > m}$ các đồng cấu liên tục của các đại số trên $k$ $\varphi_n : A \to C/C_n$, thỏa mãn $\pi_n \circ \varphi_n = \varphi_{n-1}$. Điều này đưa ta, bằng quy nạp theo $m$, về việc chứng minh mệnh đề khi $C_{m+1} = 0$. Khi đó iđêan $C_m$ có bình phương bằng không (vì $2m \geq m+1$), do đó có mệnh đề này vì $A$ là trơn hình thức.

#### Ví dụ {#ac-x-s7-n4-exa-1 .statement}

Cho $C$ là một đại số trên $k$ và $N$ là một iđêan hai phía lũy linh của $C$. Mệnh đề áp dụng được cho đại số $C$ được trang bị lọc $N$-adic. Nếu $A$ là một đại số trên $k$ tôpô tuyến tính trơn hình thức, suy ra rằng mọi đồng cấu liên tục của $A$ vào đại số trên $k$ $C/N$, được trang bị tôpô rời rạc, đều nâng được thành một đồng cấu liên tục của $A$ vào đại số trên $k$ $C$, được trang bị tôpô rời rạc.

### 5. Thương trơn hình thức của các đại số

#### Định lý 2 {#ac-x-s7-thm-2 .statement}

Cho k là một vành, A là một đại số trên k, và J là một iđêan của A sao cho đại số trên k A/J là trơn hình thức. Trang bị cho A tôpô J-adic. Các điều kiện sau là tương đương:

(i) đại số trên k tôpô A là trơn hình thức;
(ii) $\Lambda/J$-môđun $J/J^2$ là xạ ảnh và đồng cấu chính tắc ($\S$ 5, n° 2)
$$
\beta : S_{A/J}(J/J^2) \to \mathrm{gr}_J(A)
$$
là song ánh;
(iii) $A/J$-môđun $J/J^2$ là xạ ảnh và tồn tại một đẳng cấu các đại số trên k tôpô từ hoàn thành tách biệt của A lên đại số hoàn thành của đại số phân bậc $S_{A/J}(J/J^2)$.

Nếu A là Noether, thì các điều kiện này còn tương đương với:

(iv) iđêan J là cát tuyến hoàn toàn.

Trước hết, ta nhận thấy rằng (iii) suy ra (i): thật vậy, dưới các giả thiết của (iii), đại số $S_{A/J}(J/J^2)$, được trang bị tôpô liên kết với phân bậc của nó, là trơn hình thức trên $A/J$ (No. 3, ví dụ 1), nên cũng trơn hình thức trên k (No. 2, mệnh đề 3, a)); khi đó mệnh đề (i) suy ra từ mệnh đề 3, c) của No. 2.

Ký hiệu $\hat{A}$ là bổ sung tách biệt của đại số A và $\hat{J}$ là bổ sung tách biệt của J. Đồng cấu chính tắc $i : A \to \hat{A}$ cảm sinh một đẳng cấu $A/J \to \hat{A}/\hat{J}$ (III, § 2, No. 12, công thức (21)). Ký hiệu $\varphi : A/J \to \hat{A}$ là một phép nâng của đẳng cấu này (No. 4, Mệnh đề 5). Ký hiệu $\lambda : \hat{J} \to J/J^2$ là toàn ánh suy ra từ đẳng cấu chính tắc $J/J^2 \to \hat{J}/\hat{J}^2$ (III, § 2, No. 12, công thức (21)). Cho $a$ là một phần tử của A, $\bar{a}$ là lớp của nó trong $A/J$, và $z$ là một phần tử của $\hat{J}$; ta có $\varphi(\bar{a}) \equiv i(a) \pmod{\hat{J}}$, do đó $\varphi(\bar{a})z \equiv i(a)z \pmod{\hat{J}^2}$ và $\lambda(\varphi(\bar{a})z) = \lambda(i(a)z) = \bar{a}\lambda(z)$. Nói cách khác, $\lambda$ là A/J-tuyến tính khi $\hat{J}$ được trang bị cấu trúc A/J-môđun suy ra từ $\varphi$.

Giả sử rằng đồng cấu $\lambda$ thừa nhận một tiết diện A/J-tuyến tính $\sigma : J/J^2 \to \hat{J}$. Ký hiệu S là đại số trên k phân bậc $S_{A/J}(J/J^2)$ và $\hat{S}$ là bổ sung của nó. Cho
$$
\theta : S \to \hat{A}
$$
là đồng cấu của các đại số trên k sao cho $\theta(x) = \varphi(x)$ với $x$ trong $S^0 = A/J$, và $\theta(x) = \sigma(x)$ với $x$ trong $S^1 = J/J^2$. Vì $\theta$ ánh xạ $S^1$ vào $\hat{J}$, nó ánh xạ $S^n$ vào $\hat{J}^n$ và do đó mở rộng thành một đồng cấu liên tục $\hat{\theta} : \hat{S} \to \hat{A}$. Ánh xạ $\mathrm{gr}_1(\theta) : J/J^2 \to \hat{J}/\hat{J}^2$ là hợp thành của $\sigma$ với toàn cấu chính tắc $\hat{J} \to \hat{J}/\hat{J}^2$; vì $\sigma$ là một tiết diện của $\lambda$, $\mathrm{gr}_1(\theta)$ trùng với đẳng cấu chính tắc từ $J/J^2$ lên $\hat{J}/\hat{J}^2$. Suy ra rằng $\mathrm{gr}(\theta) : S \to \mathrm{gr}_{\hat{J}}(\hat{A})$ là hợp thành của toàn cấu chính tắc $\beta$ với đẳng cấu chính tắc $\mathrm{gr}_J(A) \to \mathrm{gr}_{\hat{J}}(\hat{A})$ (III, § 2, No. 12, công thức (22)).

Bây giờ ta chứng minh hàm ý (ii) $\Rightarrow$ (iii). Dưới giả thiết (ii), A/J-môđun $J/J^2$ là xạ ảnh, và do đó $\lambda$ thừa nhận một tiết diện A/J-tuyến tính; đồng cấu $\hat{\theta} : \hat{S} \to \hat{A}$ gắn với tiết diện này bởi phép dựng trước cảm sinh bởi

Ta chứng minh (i) ⇒ (ii). Giả sử rằng đại số trên k tôpô A là trơn hình thức. Trước hết ta chứng minh rằng A/J-môđun $J/J^2$ là xạ ảnh. Cho M là một Λ/J-môđun và $f : M \to J/J^2$ là một ánh xạ A/J-tuyến tính toàn ánh; vấn đề là chứng minh rằng f thừa nhận một tiết diện Λ/J-tuyến tính.

Ký hiệu π là toàn cấu chính tắc $A/J^2 \to A/J$. Theo Nhận xét 1 của No. 2, tồn tại một đẳng cấu của các đại số trên k ψ : A/J ⊕ J/J^2 → A/J^2 sao cho π(ψ(y, z)) = y và ψ(0, z) = z với $y \in A/J$, $z \in J/J^2$. Xét đại số trên k (A/J) ⊕ M (No. 1, Ví dụ) và ánh xạ u : (A/J) ⊕ M → A/J^2 sao cho u(x, m) = ψ(x, f(m)). Đây là một đồng cấu toàn ánh của các đại số trên k, có hạt nhân là môđun con Ker f của M, và do đó có bình phương bằng không. Toàn cấu chính tắc ρ : A → A/J^2 là liên tục; vì đại số trên k tôpô A là trơn hình thức, tồn tại một đồng cấu của các đại số trên k ŝ : A → (A/J)⊕M sao cho u◦ŝ = ρ. Vì pr_1 = π◦ψ = π◦u, ta có pr_1◦ŝ = π◦u◦ŝ = π◦ρ, nên pr_1◦ŝ là toàn cấu chính tắc từ A lên A/J. Do đó ta có ŝ(J) ⊂ M và hệ quả là ŝ(J^2) = 0, nên ŝ cảm sinh một ánh xạ A/J-tuyến tính s : J/J^2 → M. Ta có u◦ŝ = ρ và pr_2◦ψ^{-1}◦u(y, m) = f(m) với $y \in A/J$ và $m \in M$. Cho $x \in J$, và ū là lớp của nó trong J/J^2; ta có f(s(ū)) = f(pr_2(ŝ(x))) = pr_2(ψ^{-1}(ū)) = ū. Vậy s là một tiết diện của f.

Còn phải chứng minh rằng đồng cấu β là đơn ánh. Vì A/J-môđun $J/J^2$ là xạ ảnh, λ thừa nhận một tiết diện A/J-tuyến tính; ký hiệu θ : S → Ā là đồng cấu gắn với tiết diện đó. Đồng cấu gr(θ) được đồng nhất với β. Cho m là một số nguyên; ký hiệu Σ_m là đại số trên k phân bậc thương của S theo iđêan $\sum_{i>m} S^i$ và $\theta_m : \Sigma_m \to A/J^{m+1}$ là đồng cấu suy ra từ θ. Hợp thành của θ_m với toàn cấu chính tắc A/J^{m+1} → A/J là phép chiếu chính tắc của Σ_m lên S^0 = A/J; vì thế hạt nhân của θ_m là một iđêan hai phía lũy linh. Theo ví dụ của No. 4, tồn tại một phép nâng ψ_m : A → Σ_m của toàn cấu chính tắc A → A/J^{m+1}. Vì hợp thành của ψ_m với phép chiếu chính tắc của Σ_m lên A/J là toàn cấu chính tắc, ψ_m(J) gồm các phần tử có bậc > 0. Chuyển qua các đại số liên kết phân bậc, ta suy ra từ ψ_m một ánh xạ K-tuyến tính phân bậc gr(ψ_m) : gr_J(A) → Σ_m sao cho gr_m(θ)◦gr_m(ψ_m) = Id_{J^m/J^{m+1}}. Suy ra gr_m(θ), do đó cả β_m, là đơn ánh, điều này hoàn tất chứng minh của (ii).

Sau cùng, khi A là Noether, các điều kiện (ii) và (iv) là tương đương (§ 5, No. 2, Định lý 1).

#### Hệ quả 1 {#ac-x-s7-thm-2-cor-1 .statement}

Cho k là một trường và A là một đại số địa phương Noether trên k sao cho mở rộng κ_A của k là tách được. Các điều kiện sau là tương đương:

(i) đại số trên k A là trơn hình thức đối với tôpô $m_A$-adic;
(ii) vành A là chính quy;
(iii) đại số trên k Λ là tuyệt đối chính quy (§ 6, No. 4, Định nghĩa 1) ;
(iv) đại số trên k Ā đẳng cấu với κ_A[[T_1, ..., T_n]], với n = dim A.

#### Hệ quả 2 {#ac-x-s7-thm-2-cor-2 .statement}

Cho $k$ là một trường, $A$ là một $k$-đại số Noether và $J$ là một iđêan của $A$ được chứa trong căn của $A$. Giả sử rằng $k$-đại số $A$ là trơn hình thức đối với tôpô $J$-adic. Khi đó nó là chính quy tuyệt đối.

Thật vậy, cho $k'$ là một mở rộng hữu hạn của $k$ và $A'$ là $A$-đại số $A_{(k')}$; cần chứng minh rằng, với mọi iđêan cực đại $m'$ của $A'$, vành địa phương Noether $A'_{m'}$ là chính quy. Mà ta có $JA' \subset m'$: thật vậy, ảnh ngược của $m'$ trong $A$ là một iđêan cực đại của $A$ (V, § 2, No. 1, prop. 1), nên chứa $J$. $k'$-đại số $A'$ là trơn hình thức đối với tôpô $JA'$-adic (No. 2, prop. 4, b)), và $k'$-đại số $A'_{m'}$ là trơn hình thức đối với tôpô $JA'_{m'}$-adic (No. 2, prop. 4, a)), do đó cũng trơn hình thức đối với tôpô $m'A'_{m'}$-adic. Cho $k_0$ là trường con nguyên tố của $k'$. Khi đó $A'_{m'}$ là trơn hình thức trên $k_0$ đối với tôpô $m'A'_{m'}$-adic (hệ quả của đ. lý 1 ở No. 3); vì $\kappa(m')$ tách được trên $k_0$, vành $A'_{m'}$ là chính quy (hệ quả 1).

#### Hệ quả 3 {#ac-x-s7-thm-2-cor-3 .statement}

Cho $k$ là một vành và $A$ là một $k$-đại số trơn hình thức.

a) $A$-môđun $\Omega_k(A)$ là xạ ảnh.

b) Giả sử rằng vành $A \otimes_k A$ là Noether. Kí hiệu $\mu : A \otimes_k A \to A$ là đồng cấu sao cho $\mu(x \otimes y) = xy$; khi đó iđêan $\mathrm{Ker}(\mu)$ là hoàn toàn cát tuyến.

Các $k$-đại số $A$ và $A \otimes_k A$ là trơn hình thức (No. 2, prop. 4, c)), và $A$ đẳng cấu với thương của $A \otimes_k A$ bởi hạt nhân $I$ của $\mu$. Theo định nghĩa ta có $\Omega_k(A) = I/I^2$. Vậy a) và b) suy ra từ đ. lý 2.

### 6. Mở rộng trường cơ sở trong các đại số chính quy (đặc số khác không)

Cho $k$ là một vành và $\rho : A \to B$ là một đồng cấu của các $k$-đại số. Từ $\rho$ suy ra một ánh xạ $A$-tuyến tính $\Omega(\rho) : \Omega_k(A) \to \Omega_k(B)$, và do đó một ánh xạ $B$-tuyến tính $\Omega_0(\rho) : B \otimes_A \Omega_k(A) \to \Omega_k(B)$ (A, III, p. 135). Cho $T = (T_i)_{i \in I}$ là một họ các bất định, và $t = (t_i)_{i \in I}$ là một họ các phần tử của $B$; với mọi đa thức $f = \sum_{\alpha \in \mathbf{N}^{(I)}} c_\alpha T^\alpha$ của $A[T]$, ký hiệu $d^\Lambda f(t)$ là phần tử $\sum_\alpha t^\alpha \otimes dc_\alpha$ của $B \otimes_A \Omega_k(A)$.

#### Bổ đề 1 {#ac-x-s7-lem-1 .statement}

Giả sử rằng $B$-đại số $A$ thừa nhận một họ sinh $t = (t_i)_{i \in I}$, với các quan hệ xác định $f_\lambda \in A[T]$ ($\lambda \in \Lambda$). Đồng cấu $B$-tuyến tính
$$
\psi : (B \otimes_A \Omega_k(A)) \oplus B^{(I)} \longrightarrow \Omega_k(B)
$$
được xác định bởi $\psi(\alpha, (b_i)) = \Omega_0(\rho)(\alpha) + \sum_{i \in I} b_i dt_i$, là toàn ánh; hạt nhân của nó được sinh bởi các phần tử $r_\lambda = \left( d^\Lambda f_\lambda(t), \left( \frac{\partial f_\lambda}{\partial T_i}(t) \right)_{i \in I} \right)$ với $\lambda \in \Lambda$.

Xét dãy các B-môđun và các ánh xạ B-tuyến tính

$$
B^{(\Lambda)} \xrightarrow{\varphi} (B \otimes_{\Lambda} \Omega_k(A)) \oplus B^{(1)} \xrightarrow{\psi} \Omega_k(B) \longrightarrow 0,
$$

trong đó $\varphi$ là đồng cấu sao cho $\varphi(e_\lambda) = n_\lambda$; vấn đề là chứng minh rằng dãy này là khớp. Theo A, II, p. 36, th. 1, chỉ cần chứng minh rằng, với mọi B-môđun M, dãy

$$
0 \to \mathrm{Hom}_B(\Omega_k(B), M) \xrightarrow{\mathrm{Hom}(\psi, 1)} \mathrm{Hom}_B((B \otimes_A \Omega_k(A)) \oplus B^{(1)}, M) \xrightarrow{\mathrm{Hom}(\varphi, 1)} \mathrm{Hom}_B(B^{(\Lambda)}, M)
$$

là khớp. Theo tính chất phổ quát của môđun vi phân (A, III, p. 134), dãy này được đồng nhất với

$$
0 \to D_k(B, M) \xrightarrow{\psi'} D_k(A, M) \oplus M^1 \xrightarrow{\varphi'} M^\Lambda
$$

trong đó $\psi'(D) = (D \circ \rho, (D(t_i)))$ và $\varphi'(\Delta, (m_i)) = (f^\Delta_\lambda(t) + \sum_i \frac{\partial f_\lambda}{\partial T_i}(t) m_i)_{\lambda \in \Lambda}$ (phù hợp với A, V, p. 121, với mọi đa thức $f = \sum_{\alpha \in \mathbf{N}^{(1)}} c_\alpha T^\alpha$ của $A[T]$, $f^\Delta(t)$ ký hiệu phần tử $\sum_\alpha t^\alpha \Delta(c_\alpha)$). Nhưng tính khớp của dãy này suy ra từ loc. cit., prop. 1, xét đến việc một đạo hàm $D : B \to M$ là $k$-tuyến tính khi và chỉ khi điều này đúng với $D \circ \rho$.

Cho A là một vành. Tồn tại duy nhất một cấu trúc $\mathbf{Z}$-đại số trên A; người ta viết đơn giản $\Omega(\Lambda)$ thay cho A-môđun $\Omega_{\mathbf{Z}}(A)$. Nếu $\rho : k \to A$ là một đồng cấu của các vành, thì có một dãy khớp chính tắc các A-môđun (A, III, p. 136, prop. 21)

$$
A \otimes_k \Omega(k) \to \Omega(A) \to \Omega_k(A) \to 0.
$$

Giả sử rằng A chứa một trường con, và cho P là trường con nguyên tố của A; khi đó $\Omega(P)$ bằng không và đồng cấu chính tắc của các A-môđun $\Omega(A) \to \Omega_P(A)$ là song ánh. Nếu hơn nữa A có đặc số $p \neq 0$ (theo định nghĩa có nghĩa là $p$ là một số nguyên tố, rằng $p1_A = 0$ và $1_A \neq 0$), thì P được đồng nhất với $\mathbf{F}_p$. Hơn nữa, mọi đạo hàm của A đều triệt tiêu trên vành con $A^p$; với mọi vành con $k$ của A được chứa trong $A^p$ (và, đặc biệt, với mọi trường con hoàn hảo $k$ của A), ánh xạ chính tắc $\Omega(A) \to \Omega_k(A)$ là song ánh.

Cho A là một vành có đặc số $p \neq 0$ và $(f_i)_{1 \leq i \leq n}$ một dãy hữu hạn các phần tử của A. Ký hiệu $A_n$ là vành thương của vành đa thức $A[T_1, \ldots, T_n]$ theo iđêan sinh bởi các đa thức $T_i^p - f_i$, với $1 \leq i \leq n$.

#### Bổ đề 2 {#ac-x-s7-lem-2 .statement}

Giả sử vành A là địa phương và Noether. Khi đó $A_n$ là địa phương và Noether. Các điều kiện sau là tương đương:

(i) $A_n$ là chính quy;
(ii) A là chính quy và các phần tử $1 \otimes df_i$ của không gian vectơ $\kappa_A$-vectơ $\kappa_A \otimes_A \Omega(A)$ độc lập tuyến tính.

A) Trước hết hãy xét trường hợp $n = 1$, đặt $T_1 = T$, $f_1 = f$. Ký hiệu $a$ là lớp của $f$ trong $\kappa_A$, và phân biệt hai trường hợp tùy theo $a$ có hoặc không thuộc $\kappa_A^p$. Nếu $a \notin \kappa_A^p$, thì đa thức $T^p - a$ là bất khả quy trong $\kappa_A$ (A, V, p. 24, bổ đề 1), và $\kappa_A \otimes_A A_1$ đẳng cấu với trường $\kappa_A[T]/(T^p - a)$. Do đó iđêan $m_A A_1$ của $A_1$ là cực đại, nên vành $A_1$ là địa phương (V, § 2, No. 1, mệnh đề 1). Nếu $A$ là chính quy, thì $A_1$ là chính quy (VIII, § 5, No. 1, mệnh đề 1). Theo A, V, p. 99, mệnh đề 6, phần tử $da$ của $\Omega(\kappa_A)$ khác không; vì nó là ảnh qua ánh xạ chính tắc $\kappa_A \otimes_A \Omega(A) \to \Omega(\kappa_A)$ của $1 \otimes df$, nên phần tử sau khác không. Điều đó chứng minh bổ đề trong trường hợp này.

Bây giờ giả sử rằng $a$ thuộc $\kappa_A^p$. Do đó tồn tại một phần tử $g$ của $A$ sao cho $f - g^p \in m_A$. Đặt $h = f - g^p$. Vì $T^p - f = (T - g)^p - h$, nên $A$-đại số $A_1$ đẳng cấu với $A[T]/(T^p - h)$. Theo VIII, § 5, No. 4, mệnh đề 4, vành $A_1$ là địa phương và, để nó là chính quy, điều kiện cần và đủ là $A$ là chính quy và $h$ không thuộc $m_A^2$. Bây giờ, vì $\kappa_A$ là trơn hình thức trên trường nguyên tố (No. 3, định lý 1), ánh xạ chính tắc

$$
\bar{d} : m_A / m_A^2 \to \kappa_A \otimes_A \Omega(A)
$$

là đơn ánh (No. 2, nhận xét 1); nhưng ảnh qua $\bar{d}$ của lớp của $h$ theo modulo $m_A^2$ bằng $1 \otimes dh = 1 \otimes d(f - g^p) = 1 \otimes df$. Điều đó chứng minh bổ đề trong trường hợp thứ hai này và hoàn tất chứng minh của trường hợp $n = 1$.

B) Giả sử $n > 1$. Vành $A_1$ là địa phương và Noether theo trường hợp đã xét. $A_1$-đại số $A_n$ được đồng nhất với thương của $A_1[T_2, \ldots, T_n]$ bởi iđêan sinh bởi các $T_i^p - f_i$, $i \geq 2$; theo giả thiết quy nạp, nó là một vành địa phương và điều kiện (i) tương đương với phép hội của hai điều kiện sau:

(i') $A_1$ là chính quy;
(ii') các phần tử $1 \otimes df_2, \ldots, 1 \otimes df_n$ của không gian vectơ $\kappa_{A_1}$ $\kappa_{A_1} \otimes_{A_1} \Omega(A_1)$ là độc lập tuyến tính.

Nhưng (i') tương đương, như ta vừa thấy, với
(ii'') $A$ là chính quy và phần tử $1 \otimes df_1$ của không gian vectơ $\kappa_A$ $\kappa_A \otimes_A \Omega(A)$ khác không.

Theo bổ đề 1, đồng cấu chính tắc $A_1 \otimes_A \Omega(A) \to \Omega(A_1)$ cảm sinh một đẳng cấu từ $((A_1 \otimes_A \Omega(A))/A_1(1 \otimes df_1)) \oplus A_1$ lên $\Omega(A_1)$, và do đó một đơn cấu của $(\kappa_{A_1} \otimes_A \Omega(A))/\kappa_{A_1}(1 \otimes df_1)$ vào $\kappa_{A_1} \otimes_{A_1} \Omega(A_1)$. Vì $\kappa_{A_1} \otimes_A \Omega(A)$ được đồng nhất với $\kappa_{A_1} \otimes_{\kappa_A} (\kappa_A \otimes_A \Omega(A))$, nên mệnh đề (ii'') do đó tương đương với:
(ii''') các phần tử $1 \otimes df_2, \ldots, 1 \otimes df_n$ là độc lập tuyến tính trong $(\kappa_A \otimes_A \Omega(A))/\kappa_A(1 \otimes df_1)$.

Nhưng phép hội của (ii') và (ii'') tương đương với (ii), điều đó chứng minh bổ đề.

#### Mệnh đề 6 {#ac-x-s7-prop-6 .statement}

Cho $k$ là một trường có đặc số $p \neq 0$, $k'$ là một mở rộng thuần túy không khả phân của $k$, bậc hữu hạn và chiều cao $\leqslant 1$, và $A$ là một $k$-đại số địa phương chính quy. Khi đó $A_{(k')}$ là một vành địa phương và các điều kiện sau là tương đương:

(i) vành $A_{(k')}$ là chính quy;
(ii) ánh xạ tuyến tính $\kappa_A$

$$
\kappa_A \otimes_{{k'}^p} \Omega_{{k'}^p}({k'}^p) \longrightarrow \kappa_A \otimes_A \Omega(A)
$$

suy ra từ đơn ánh chính tắc ${k'}^p \to A$ là đơn ánh.

Thật vậy, lấy $(x_i)_{i \in I}$ là một $p$-cơ sở hữu hạn của $k'$ trên $k$ (A, V, p. 98); với mỗi $i \in I$, đặt $f_i = x_i^p \in k$. $k$-đại số $k'$ được đồng nhất với thương của $k[(T_i)_{i \in I}]$ bởi iđêan sinh bởi các đa thức $T_i^p - f_i$, do đó $A$-đại số $A_{(k')}$ được đồng nhất với thương của $A[(T_i)_{i \in I}]$ bởi iđêan sinh bởi các đa thức $T_i^p - f_i 1_A$.

Hơn nữa, $(f_i)_{i \in I}$ là một $p$-cơ sở của ${k'}^p$ trên $k^p$, và không gian vectơ ${k'}^p$ $\Omega_{k^p}({k'}^p)$ có cơ sở là họ các $df_i$ (A, V, p. 97, Định lý 1). Khi đó Mệnh đề 6 suy ra từ bổ đề 2.

### 7. Một tiêu chuẩn cho các đại số địa phương trơn hình thức

#### Mệnh đề 7 {#ac-x-s7-prop-7 .statement}

Cho $k_0$ là một vành, $k$ là một $k_0$-đại số, $A$ là một $k$-đại số, $m$ là một iđêan cực đại của $A$. Giả sử rằng $k$ và $A/m$ là trơn hình thức trên $k_0$. Để $A$ là trơn hình thức trên $k$ đối với tôpô $m$-adic, điều kiện cần và đủ là hai điều kiện sau được thỏa mãn:

(i) đồng cấu chính tắc $S_{A/m}(m/m^2) \to \mathrm{gr}_m(A)$ là song ánh;
(ii) ánh xạ $A/m$-tuyến tính

$$
\omega : A/m \otimes_k \Omega_{k_0}(k) \longrightarrow A/m \otimes_A \Omega_{k_0}(A)
$$

suy ra từ ánh xạ chính tắc $k \to A$ là đơn ánh.

Ký hiệu bởi $d_k : k \to \Omega_{k_0}(k)$ và $d_A : A \to \Omega_{k_0}(A)$ các đạo hàm $k_0$-phổ quát.

Trước hết giả sử rằng $A$ là trơn hình thức trên $k$ đối với tôpô $m$-adic. Khi đó $A$ là trơn hình thức trên $k_0$ đối với tôpô $m$-adic (No. 2, Prop. 3, a)), điều này tương đương với (i) (No. 5, Định lý 2). Hơn nữa, đạo hàm $k_0$ $\lambda \mapsto 1 \otimes d_k(\lambda)$ của $k$ vào $A/m \otimes_k \Omega_{k_0}(k)$ có thể được mở rộng thành một đạo hàm $k_0$ của $A$ vào $A/m \otimes_k \Omega_{k_0}(k)$ (No. 2, Nhận xét 2). Do đó tồn tại một ánh xạ $A$-tuyến tính $u : \Omega_{k_0}(A) \to A/m \otimes_k \Omega_{k_0}(k)$ sao cho $u(d_A(\lambda 1_A)) = 1 \otimes d_k(\lambda)$ với mọi $\lambda \in k$. Ánh xạ $A/m$-tuyến tính $A/m \otimes_A \Omega_{k_0}(A) \longrightarrow A/m \otimes_k \Omega_{k_0}(k)$ suy ra từ $u$ là một phép co rút của $\omega$, điều này chứng minh (ii).

Ngược lại, giả sử rằng các điều kiện (i) và (ii) được thỏa mãn. Khi đó $A$ là trơn hình thức trên $k_0$ đối với tôpô $m$-adic (No. 5, Định lý 2) và $A$-môđun $\Omega_{k_0}(A)$ là xạ ảnh (No. 5, Hệ quả 3 của Định lý 2). Cố định một số nguyên $r \geqslant 0$ và xét ánh xạ $A/m^r$-tuyến tính

$$
\omega_r : A/m^r \otimes_k \Omega_{k_0}(k) \longrightarrow A/m^r \otimes_A \Omega_{k_0}(A)
$$

suy ra từ ánh xạ chính tắc $k \to A$. Cho $(\lambda_i)_{i \in I}$ là một họ các phần tử của $k$ sao cho các $d_k(\lambda_i)$ tạo thành một cơ sở của không gian vectơ $\Omega_{k_0}(k)$ trên $k$; theo (ii), các phần tử $1 \otimes d_A(\lambda_i 1_A)$ độc lập tuyến tính trong $A/\mathfrak{m} \otimes_{\Lambda} \Omega_{k_0}(A)$. Theo II, § 3, No. 2, Hệ quả 1 và 2 của Mệnh đề 5, các $1 \otimes d_A(\lambda_i 1_A)$ tạo thành một cơ sở của một nhân tử trực tiếp của $A/\mathfrak{m}^r$-môđun $A/\mathfrak{m}^r \otimes_{\Lambda} \Omega_{k_0}(A)$. Do đó tồn tại một ánh xạ $A/\mathfrak{m}^r$-tuyến tính
$$
u_r : A/\mathfrak{m}^r \otimes_{\Lambda} \Omega_{k_0}(A) \longrightarrow A/\mathfrak{m}^r \otimes_k \Omega_{k_0}(k)
$$
sao cho $u_r(1 \otimes d_A(\lambda_i 1_A)) = 1 \otimes d_k(\lambda_i)$ với mọi $i$, nên $u_r \circ \omega_r = \mathrm{Id}$.

Bây giờ ta hãy kiểm tra rằng $A$ là trơn hình thức trên $k$ đối với tôpô $\mathfrak{m}$-adic. Cho $C$ là một $k$-đại số, $N$ một iđêan bình phương bằng không của $C$, và $\pi : C \to C/N$ toàn cấu chính tắc; trang bị cho $C$ và $C/N$ tôpô rời rạc. Cho $\varphi : A \to C/N$ là một đồng cấu liên tục của các $k$-đại số. Vì $A$ là trơn hình thức trên $k_0$ đối với tôpô $\mathfrak{m}$-adic, tồn tại một đồng cấu liên tục của các $k_0$-đại số $\tilde{\varphi}_0 : A \to C$ sao cho $\pi \circ \tilde{\varphi}_0 = \varphi$. Theo Mệnh đề 1 của No. 1, các đồng cấu của $k_0$-đại số $\tilde{\varphi} : A \to C$ sao cho $\pi \circ \tilde{\varphi} = \varphi$ là các ánh xạ $x \mapsto v(d_A(x)) + \tilde{\varphi}_0(x)$, trong đó $v$ chạy qua $\mathrm{Hom}_{\Lambda}(\Omega_{k_0}(A), N)$. Còn phải chọn $v$ sao cho $\tilde{\varphi}$ là một đồng cấu của các $k$-đại số. Ánh xạ $\lambda \mapsto \lambda 1_C - \tilde{\varphi}_0(\lambda 1_A)$ là một đạo hàm $k_0$ của $k$ vào $N$ (*loc. cit.*), và do đó có thể viết dưới dạng $h \circ d_k$ với $h \in \mathrm{Hom}_k(\Omega_{k_0}(k), N)$.

Chọn một số nguyên $r$ sao cho hạt nhân của $\varphi$ chứa $\mathfrak{m}^r$. A-môđun $N$ bị triệt tiêu bởi $\mathfrak{m}^r$, và chỉ cần lấy cho $v$ hợp thành của dãy các đồng cấu
$$
\Omega_{k_0}(A) \longrightarrow A/\mathfrak{m}^r \otimes_{\Lambda} \Omega_{k_0}(A) \xrightarrow{u_r} A/\mathfrak{m}^r \otimes_k \Omega_{k_0}(k) \xrightarrow{h'} N ,
$$
trong đó $h'$ được suy ra từ $h$. Thật vậy, với $\lambda \in k$ ta có:
$$
v(d_A(\lambda 1_A)) = h'u_r(1 \otimes d_A(\lambda 1_A)) = h'(1 \otimes d_k(\lambda)) = h(d_k(\lambda)) = \lambda 1_C - \tilde{\varphi}_0(\lambda 1_A) .
$$

#### Nhận xét 1 {#ac-x-s7-n7-rem-1 .statement}

Khi $A$ là Noether, điều kiện (i) có nghĩa là vành địa phương $A_{\mathfrak{m}}$ là chính quy (VIII, § 5, No. 2, Định lý 1).

#### Mệnh đề 8 {#ac-x-s7-prop-8 .statement}

*Cho $k$ là một trường và $A$ là một đại số địa phương Noether trên $k$. Các điều kiện sau là tương đương*:

(i) *A là trơn hình thức trên $k$ đối với tôpô $\mathfrak{m}_A$-adic* ;
(ii) *A là chính quy và ánh xạ $\kappa_A$-tuyến tính*
$$
\omega : \kappa_A \otimes_k \Omega(k) \longrightarrow \kappa_A \otimes_{\Lambda} \Omega(A)
$$
*được suy ra từ đơn ánh chính tắc $k \to A$ là đơn ánh* ;
(iii) *A là chính quy tuyệt đối* ;
(iv) *với mọi mở rộng thuần bất khả phân $k'$ của $k$, có bậc hữu hạn và chiều cao $\leqslant 1$, vành địa phương $A_{(k')}$ là chính quy*.

(ii) $\Leftrightarrow$ (i): chỉ cần áp dụng Mđ. 7 và Nhận xét 1 ở trên, lấy cho $k_0$ trường con nguyên tố của $k$; thật vậy, $k$ và $\kappa_A$ đều trơn hình thức trên $k_0$ (No. 3, Định lý 1).
(i) $\Rightarrow$ (iii): điều này suy ra từ Hệ quả 2 của Định lý 2 (No. 5).

Nếu k có đặc số 0, từ Hệ quả 1 của Định lý 2 (No. 5) suy ra rằng (iv) kéo theo (i), do đó có mệnh đề trong trường hợp này. Giả sử k có đặc số $p \neq 0$ và chứng minh (iv) ⇒ (ii). Cho $k'$ là một mở rộng thuần bất khả phân của k, có bậc hữu hạn và chiều cao $\leq 1$. Nếu A và $A_{(k')}$ là chính quy, thì ánh xạ chính tắc $\kappa_A \otimes_{k'} \Omega_{k^p}({k'}^p) \longrightarrow \kappa_A \otimes_A \Omega(\Lambda)$ là đơn ánh (No. 6, Mđ. 6). Theo Định lý 1, b) của A, V, p. 97, áp dụng cho mở rộng k của $k^p$, không gian vectơ trên k $\Omega(k)$, trùng với $\Omega_{k^p}(k)$, là hợp lọc tăng của các không gian con $k \otimes_{{k'}^p} \Omega_{k^p}({k'}^p)$, trong đó $k'$ chạy qua tập hợp các mở rộng thuần bất khả phân hữu hạn của k có chiều cao $\leq 1$ được chứa trong một bao đóng đại số cố định của k. Mệnh đề (ii) được suy ra.

#### Nhận xét 2 {#ac-x-s7-n7-rem-2 .statement}

Cho k là một trường và A là một đại số trên k sao cho vành $A_{(k')}$ là chính quy với mọi mở rộng thuần bất khả phân $k'$ của k, có bậc hữu hạn và chiều cao $\leq 1$; khi đó A là chính quy tuyệt đối. Thật vậy, cho $k'$ là một mở rộng như thế; với mọi iđêan cực đại m của A, vành $k' \otimes_k A_m$ được đồng nhất với một vành phân thức của $A_{(k')}$, nên do đó là chính quy. Theo Mđ. 8 ở trên và Mđ. 6 của § 6, No. 4, đại số A là chính quy tuyệt đối.

### 8. Sự tồn tại của các phép rút đối với các ánh xạ tuyến tính

#### Mệnh đề 9 {#ac-x-s7-prop-9 .statement}

Cho A là một vành, M là một A-môđun hữu hạn sinh, N là một A-môđun xạ ảnh, và $u : M \to N$ là một ánh xạ A-tuyến tính.

a) Cho $\mathfrak{p}$ là một iđêan nguyên tố của A. Các điều kiện sau là tương đương :

(i) tồn tại $f \in A - \mathfrak{p}$ và $v \in \mathrm{Hom}_{A_f}(N_f, M_f)$ sao cho $v \circ u_f = \mathrm{Id}_{M_f}$;
(ii) tồn tại $v \in \mathrm{Hom}_{A_\mathfrak{p}}(N_\mathfrak{p}, M_\mathfrak{p})$ sao cho $v \circ u_\mathfrak{p} = \mathrm{Id}_{M_\mathfrak{p}}$;
(iii) ánh xạ $\kappa(\mathfrak{p})\text{-linear } 1 \otimes u : \kappa(\mathfrak{p}) \otimes_A M \to \kappa(\mathfrak{p}) \otimes_A N$ là đơn ánh;
(iv) tồn tại một số nguyên $m \geq 0$, các phần tử $x_1, \ldots, x_m$ của M và các dạng tuyến tính $y_1, \ldots, y_m$ trên N sao cho các ảnh của $x_i$ trong $M_\mathfrak{p}$ sinh ra $A_\mathfrak{p}$-môđun $M_\mathfrak{p}$ và sao cho ta có $\det(<y_j, u(x_i)>)\notin \mathfrak{p}$;

Nếu điều kiện (iv) được thỏa mãn, ta có $m = [\kappa(\mathfrak{p}) \otimes_A M : \kappa(\mathfrak{p})]$ và các phần tử $1 \otimes x_i$ lập thành một cơ sở của không gian vectơ $\kappa(\mathfrak{p})$-không gian vectơ $\kappa(\mathfrak{p}) \otimes_A M$.

b) Tập U các iđêan nguyên tố $\mathfrak{p}$ của A thỏa mãn các điều kiện của a) là một tập mở của Spec(A), và các điều kiện sau là tương đương:

(i) ta có $U = \mathrm{Spec}(A)$;
(ii) U chứa mọi iđêan cực đại của A;
(iii) tồn tại $v \in \mathrm{Hom}_A(N, M)$ sao cho $v \circ u = \mathrm{Id}_M$;
(iv) u là đơn ánh và Coker(u) là một A-môđun xạ ảnh.

Ta chứng minh a).

(i) ⇒ (ii) ⇒ (iii): các suy ra này là hiển nhiên.

(iii) ⇒ (iv): đặt $m = [\kappa(\mathfrak{p}) \otimes_A M : \kappa(\mathfrak{p})]$ và gọi $(x_1, \ldots, x_m)$ là một dãy các phần tử của M sao cho các phần tử $1 \otimes x_i$ lập thành một cơ sở của không gian vectơ $\kappa(\mathfrak{p})$-không gian vectơ $\kappa(\mathfrak{p}) \otimes_A M$. Các ảnh của $x_i$ trong $M_\mathfrak{p}$ sinh ra $A_\mathfrak{p}$-môđun $M_\mathfrak{p}$ (bổ đề Nakayama). Nếu điều kiện (iii) được thỏa mãn, các phần tử $1 \otimes u(x_i)$ của không gian vectơ $\kappa(\mathfrak{p})$-không gian vectơ $\kappa(\mathfrak{p}) \otimes_A N$ là độc lập tuyến tính.

Hơn nữa, tồn tại một A-môđun N', một tập hợp I, và một đẳng cấu các A-môđun $\theta : N \oplus N' \to A^{(I)}$, từ đó suy ra một đẳng cấu các không gian vectơ $\kappa(p)$-vectơ $$
\overline{\theta} : (\kappa(p) \otimes_{\Lambda} N) \oplus (\kappa(p) \otimes_A N') \to \kappa(p)^{(I)} .
$$ Các phần tử $t_i = \overline{\theta}(1 \otimes u(x_i), 0)$ của $\kappa(p)^{(I)}$ lập thành một họ tự do hữu hạn. Do đó tồn tại các phần tử $\alpha_1, \ldots, \alpha_m$ của I sao cho ta có $\det(\mathrm{pr}_{\alpha_j}(t_i)) \neq 0$; các dạng tuyến tính $y_j : z \mapsto \mathrm{pr}_{\alpha_j}(\theta(z, 0))$ trên N là thích hợp.

Giả sử điều kiện (iv) được thỏa mãn. Gọi $(a_{ij}) \in M_m(A)$ là ma trận hệ số $a_{ij} = <y_j, u(x_i)>$. Gọi g là một phần tử của $A - p$ sao cho các ảnh của $x_i$ sinh $\Lambda_g$-môđun $M_g$ (II, § 5, No. 1, Mệnh đề 2), và đặt $f = g \det(a_{ij})$. Vì $\det(a_{ij})$ khả nghịch trong $A_f$, các ảnh của các phần tử $u(x_i)$ trong $N_f$ độc lập tuyến tính; do đó các ảnh của $x_i$ trong $M_f$ tạo thành một cơ sở của $A_f$-môđun này. Điều này chứng minh mệnh đề cuối cùng của a). Bây giờ chứng minh (i). Gọi $w \in \mathrm{Hom}_A(N, M)$ là ánh xạ $z \mapsto \sum_j <y_j, z> x_j$. Ta có
$$
w \circ u(x_i) = \sum_j a_{ij} x_j ;
$$
vì các ảnh của $x_i$ tạo thành một cơ sở của $M_f$ và ma trận $(a_{ij})$ khả nghịch trong $M_m(A_f)$, tự đồng cấu $(w \circ u)_f$ của $M_f$ là song ánh, và ánh xạ $v = (w \circ u)_f^{-1} \circ w_f \in \mathrm{Hom}_{A_f}(N_f, M_f)$ thỏa mãn điều kiện (i).

Bây giờ chứng minh b). Việc U là mở suy ra từ điều kiện (i) của a).

(iii) $\Rightarrow$ (i) $\Rightarrow$ (ii): điều này rõ ràng.

(iv) $\Rightarrow$ (iii): dưới các giả thiết của (iv), dãy $0 \to M \xrightarrow{u} N \longrightarrow \mathrm{Coker}(u) \to 0$ là khớp và tách, do đó có (iii).

(ii) $\Rightarrow$ (iv): như trên, đưa vào một đẳng cấu các A-môđun $\theta : N \oplus N' \to A^{(I)}$. Gọi $u'$ là ánh xạ từ M vào $A^{(I)}$ được xác định bởi $u'(x) = \theta(u(x), 0)$. Tồn tại một tập con hữu hạn J của I sao cho ảnh của $u'$ được chứa trong môđun con $A^J$ của $A^{(I)}$. Gọi $u'' : M \to \Lambda^J$ là ánh xạ suy ra từ $u'$. Dưới giả thiết (ii), với mọi iđêan cực đại m của A, ánh xạ tuyến tính $A_m$-tuyến tính $u'_m$ từ $M_m$ vào $A_m^{(I)}$ thừa nhận một ánh xạ co rút, và vì vậy điều tương tự cũng đúng với $u''_m$; do đó $u''_m$ là đơn ánh và ảnh của nó là một nhân tử trực tiếp trong $A_m^J$, nên đối hạt nhân của nó là một $A_m$-môđun xạ ảnh. A-môđun $\mathrm{Coker}(u'')$ là hữu hạn trình bày theo phép dựng; vì vậy nó là xạ ảnh (II, § 5, No. 2, Định lý 1). Đồng cấu $u''$ là đơn ánh (II, § 3, No. 3, Định lý 1); do đó, $u$ là đơn ánh. A-môđun $\mathrm{Coker}(u')$ đẳng cấu, một mặt với $\mathrm{Coker}(u) \oplus N'$, mặt khác với $\mathrm{Coker}(u'') \oplus A^{(I-J)}$. Vì các A-môđun $A^{(I-J)}$, $\mathrm{Coker}(u'')$ và $N'$ là xạ ảnh, điều tương tự cũng đúng với $\mathrm{Coker}(u)$, điều này hoàn tất việc chứng minh (iv).

### 9. Tiêu chuẩn Jacobi

Cho k là một vành, A là một đại số trên K, J là một iđêan của A và $\bar{d} : J/J^2 \to \Lambda/J \otimes_A \Omega_k(A)$ là ánh xạ chính tắc. Với mỗi đại số trên A/J R, người ta ký hiệu bởi
$$
\bar{d}_R : R \otimes_{\Lambda/J} J/J^2 \longrightarrow R \otimes_A \Omega_k(A)
$$

ánh xạ R-tuyến tính cảm sinh bởi $\bar{d}$. Nếu $k$-đại số $A/J$ là trơn hình thức, thì $\bar{d}$ có một phép rút lại A-tuyến tính (No. 2, Nhận xét 1) và $\bar{d}_R$ có một phép rút lại R-tuyến tính đối với mọi R.

Tổng quát hơn:

#### Bổ đề 3 {#ac-x-s7-lem-3 .statement}

Cho K là một iđêan của A chứa J. Giả sử rằng tồn tại một số nguyên m sao cho $J \cap K^m$ được chứa trong JK (điều kiện này được thỏa mãn nếu A là Noether). Nếu $A/J$ là trơn hình thức trên k đối với tôpô K/J-adic, thì ánh xạ $\bar{d}_{A/K} : A/K \otimes_{A/J} J/J^2 \longrightarrow A/K \otimes_A \Omega_k(A)$ có một phép rút lại A-tuyến tính.

Ký hiệu C là $k$-đại số $A/(JK + K^m)$; iđêan N = $(J + K^m)/(JK + K^m)$ của C có bình phương bằng không và vành thương C/N được đồng nhất với $A/(J + K^m)$. Trang bị cho C và C/N tôpô rời rạc, và cho A/J tôpô K/J-adic. Đồng cấu chính tắc $A/J \to A/(J + K^m)$ là liên tục; do đó nó có một phép nâng $\varphi : A/J \to A/(JK + K^m)$.

Khi đó ánh xạ $a \mapsto a1_C - \varphi(a1_{A/J})$ từ A vào N là một k-đạo hàm (No. 1, Mệnh đề 1), nên được viết thành $a \mapsto u(da)$ với $u \in \mathrm{Hom}_A(\Omega_k(A), N)$. Nhưng giả thiết $J \cap K^m \subset JK$ kéo theo $J \cap (JK + K^m) = JK$, nên ánh xạ chính tắc $\psi : J/JK \to N$ là song ánh; do đó tồn tại $v \in \mathrm{Hom}_{A/K}(A/K \otimes_A \Omega_k(A), J/JK)$ sao cho, với a trong A, ta có $a1_C = \varphi(a1_{A/J}) + \psi(v(1 \otimes da))$. Lấy a trong J, ta thấy rằng $v(1 \otimes da)$ bằng lớp của a trong J/JK. Vì $A/K \otimes_{A/J} J/J^2$ được đồng nhất với $J/JK$, nên $v$ là phép rút lại cần tìm.

Việc điều kiện trên K được thỏa mãn khi đại số A là Noether suy ra từ III, § 3, No. 1, Hệ quả 2 của Mệnh đề 1.

#### Bổ đề 4 {#ac-x-s7-lem-4 .statement}

Giả sử rằng A là trơn hình thức trên k đối với tôpô J-adic. Để $A/J$ là trơn hình thức trên k, điều kiện cần và đủ là ánh xạ chính tắc $\bar{d}$ có một phép rút lại A-tuyến tính.

Người ta đã biết rằng nếu $A/J$ là trơn hình thức trên $k$, thì ánh xạ $\bar{d}$ thừa nhận một phép rút lại A-tuyến tính (No. 2, Nhận xét 1). Ngược lại, giả sử rằng $\bar{d}$ có một phép rút lại A-tuyến tính. Cho $\pi : A/J^2 \to A/J$ là toàn cấu chính tắc; theo Mệnh đề 2 của No. 1, tồn tại một đồng cấu vành $h : A/J \to A/J^2$ sao cho $\pi \circ h = \mathrm{Id}_{A/J}$. Cho C là một $k$-đại số, N một iđêan của C có bình phương bằng không, và $\rho : C \to C/N$ là toàn cấu chính tắc; trang bị cho C và C/N tôpô rời rạc. Cho $u : A/J \to C/N$ là một đồng cấu liên tục của các $k$-đại số. Vì A là trơn hình thức trên $k$ đối với tôpô J-adic, nên tồn tại một đồng cấu của các $k$-đại số $v : A \to C$ làm cho biểu đồ

$$
\begin{array}{ccc}
A & \xrightarrow{v} & C \\
\downarrow & & \downarrow \rho \\
A/J & \xrightarrow{u} & C/N
\end{array}
$$

giao hoán, trong đó các mũi tên thẳng đứng biểu thị các toàn cấu chính tắc. Ta có $v(J) \subset \mathbf{N}$, nên $v(J^2) \subset \mathbf{N}^2 = \{0\}$, và $v$ xác định, bằng cách chuyển qua các thương, một đồng cấu $\bar{v} : A/J^2 \to C$ thỏa mãn $\rho \circ \bar{v} = u \circ \pi$. Khi đó $\bar{v} \circ h$ là một phép nâng của $u$ lên $C$.

#### Định lý 3 {#ac-x-s7-thm-3 .statement}

Cho $k$ là một vành, $A$ là một $k$-đại số trơn hình thức, và $J$ là một iđêan sinh hữu hạn của $A$; đặt $B = A/J$.

a) Cho $\mathfrak{p}$ là một iđêan nguyên tố của $B$ và cho $q$ là iđêan (nguyên tố) của $A$ sao cho $\mathfrak{p} = q/J$. Các điều kiện sau là tương đương:
(i) $k$-đại số $B_{\mathfrak{p}}$ là trơn hình thức;
(ii) tồn tại $f \in B - \mathfrak{p}$ sao cho $k$-đại số $B_f$ là trơn hình thức;
(iii) ánh xạ tuyến tính trên $\kappa(\mathfrak{p})$
$$
\bar{d}_{\kappa(\mathfrak{p})} : \kappa(\mathfrak{p}) \otimes_B J/J^2 \to \kappa(\mathfrak{p}) \otimes_A \Omega_k(\Lambda)
$$
là đơn ánh;
(iv) tồn tại một số nguyên $m \geqslant 0$, các phần tử $f_1, \ldots, f_m$ của $J$, mà các ảnh $(f_1)_q, \ldots, (f_m)_q$ sinh iđêan $J_q$, và các $k$-đạo hàm $D_1, \ldots, D_m$ của $A$ sao cho $\det(D_j(f_i)) \notin q$.

b) Tập hợp các iđêan nguyên tố $\mathfrak{p}$ của $B$ thỏa mãn các điều kiện tương đương của a) là mở trong $\mathrm{Spec}(B)$. Để $B$ là trơn hình thức trên $k$, điều kiện cần và đủ là mọi iđêan nguyên tố (resp. cực đại) của $B$ đều thỏa mãn các điều kiện ấy.

c) Giả sử rằng $A$ là Noether. Các điều kiện của a) cũng tương đương với:
(v) $k$-đại số $B_{\mathfrak{p}}$ là trơn hình thức đối với tôpô $\mathfrak{p}B_{\mathfrak{p}}$-adic.
Hơn nữa, dưới các điều kiện của (iv), iđêan $J_q$ là hoàn toàn cát tuyến và dãy $((f_1)_q, \ldots, (f_m)_q)$ là hoàn toàn cát tuyến đối với $A_q$.

Đặt $M = J/J^2$ và $N = B \otimes_A \Omega_k(A)$. $B$-môđun $M$ là kiểu hữu hạn, và $B$-môđun $N$ là xạ ảnh (No. 5, Hệ quả 3 của Định lý 2). Với mọi tập con nhân $S$ của $A$, $k$-đại số $S^{-1}A$ là trơn hình thức (No. 2, Mệnh đề 4, a)). Theo Bổ đề 4, do đó các điều kiện (i) và (ii) lần lượt tương đương với
(i') ánh xạ $\bar{d}_{B_{\mathfrak{p}}} : M_{\mathfrak{p}} \to N_{\mathfrak{p}}$ có một phép co rút tuyến tính trên $B_{\mathfrak{p}}$;
(ii') tồn tại $f \in B - \mathfrak{p}$ sao cho ánh xạ $\bar{d}_{B_f} : M_f \to N_f$ có một phép co rút tuyến tính trên $B_f$.

Mệnh đề 9 của No. 8 áp dụng cho vành $B$ và cho đồng cấu $\bar{d} : M \to N$ suy ra tính tương đương của các điều kiện (i'), (ii'') và (iii), và cũng kéo theo các khẳng định của b) (lại dùng Bổ đề 4). Hơn nữa, (iii) tương đương với:
(iii') ánh xạ $\kappa(q) \otimes_A J \to \kappa(q) \otimes_A \Omega_k(A)$ suy ra từ $d : J \to \Omega_k(A)$ là đơn ánh,
còn (iv) có thể viết:
(iv') tồn tại một số nguyên $m \geqslant 0$, các phần tử $f_1, \ldots, f_m$ của $J$ mà các ảnh của chúng sinh iđêan $J_q$ của $A_q$, và các phần tử $y_1, \ldots, y_m$ của $\mathrm{Hom}_A(\Omega_k(A), A)$ sao cho $\det(<y_j, df_i>) \notin q$.

Vì $A$-môđun $\Omega_k(A)$ là xạ ảnh (No. 5, Hệ quả 3 của Định lý 2), Mệnh đề 9 của No. 8, áp dụng cho vành $A$ và cho đồng cấu $d : J \to \Omega_k(A)$, suy ra tính tương đương của (iii') và (iv').

Sau cùng, giả sử vành $A$ là Noether. Hiển nhiên (i) suy ra (v). Dưới giả thiết (v), Bổ đề 3 cho thấy rằng ánh xạ

$$
\bar{d}_{\kappa(q)} : \kappa(q) \otimes_{B_p} J_q / J_q^2 \longrightarrow \kappa(q) \otimes_{A_q} \Omega_k(A_q)
$$

là đơn ánh, do đó có (iii).

Dưới các điều kiện của (iv), ta có $m = [\kappa(q) \otimes_A J : \kappa(q)]$ (No. 9, Mệnh đề 8). Theo Định lý 2 của No. 5, iđêan $J_q$ là hoàn toàn cát tuyến, và dãy $((f_1)_q, \ldots, (f_m)_q)$ là hoàn toàn cát tuyến đối với $A_q$ ($§ 1$, No. 3, Hệ quả 2 của Định lý 1). Điều đó chứng minh c).

#### Hệ quả 1 {#ac-x-s7-thm-3-cor-1 .statement}

*Cho $k_0$ là một vành, $k$ là một $k_0$-đại số Noether trơn hình thức, và $B$ là một $k$-đại số địa phương essenxiellement hữu hạn kiểu. Nếu $k_0$-đại số $B$ là trơn hình thức đối với tôpô $\mathfrak{m}_B$-adic, thì nó là trơn hình thức.*

Tồn tại một số nguyên $n \geqslant 0$, một tập con nhân tính $S$ của $k[T_1, \ldots, T_n]$, và một $k$-đồng cấu toàn ánh $S^{-1} k[T_1, \ldots, T_n] \to B$. Đại số $S^{-1} k[T_1, \ldots, T_n]$ là Noether và trơn hình thức trên $k$ (No. 3, Ví dụ 2 và No. 2, Mệnh đề 4, a)), do đó trên $k_0$ (No. 2, Mệnh đề 3, a)). Khi đó hệ quả suy ra từ Định lý 3, c).

#### Hệ quả 2 {#ac-x-s7-thm-3-cor-2 .statement}

*Cho $k_0$ là một vành, $k$ là một $k_0$-đại số Noether trơn hình thức, và $B$ là một $k$-đại số essenxiellement hữu hạn kiểu. Tập $U$ các iđêan nguyên tố $\mathfrak{p}$ của $B$ sao cho $k_0$-đại số $B_{\mathfrak{p}}$ là trơn hình thức (đối với tôpô rời rạc hoặc tôpô $\mathfrak{p}B_{\mathfrak{p}}$-adic) là mở trong $\operatorname{Spec}(B)$ và các điều kiện sau là tương đương:

(i) *ta có* $U = \operatorname{Spec}(B)$ ;
(ii) $U$ *chứa mọi iđêan cực đại của* $B$ ;
(iii) *$k_0$*-đại số* $B$ *là trơn hình thức*.

Điều này suy ra như trên từ Định lý 3.

#### Nhận xét 1 {#ac-x-s7-n9-rem-1 .statement}

Các hệ quả 1 và 2 áp dụng đặc biệt khi $k_0$ là một trường và ta ở trong một trong hai trường hợp sau:
a) $B$ là một đại số về cơ bản thuộc kiểu hữu hạn trên một mở rộng tách được của $k_0$ (định lý 1 của No. 3);
b) $B$ là một $k_0$-đại số địa phương Noether đầy đủ mà trường thặng dư $\kappa_B$ của nó là một mở rộng tách được của $k_0$ (trong trường hợp này ta lấy cho $k$ một đại số chuỗi lũy thừa hình thức trên $\kappa_B$ mà $B$ là một thương của nó (No. 3 và IX, § 3, No. 3)).
Trong mỗi trường hợp ấy, suy ra từ hệ quả 2, có lưu ý đến mệnh đề 8 của No. 7 và mệnh đề 6, b) của § 6, No. 4, rằng $k_0$-đại số $B$ là trơn hình thức khi và chỉ khi nó là chính quy tuyệt đối.

**Hệ quả 3 (Zariski).** — *Cho $k$ là một trường, $A$ là một $k$-đại số địa phương chính quy, và $J$ là một iđêan của $A$ phân biệt với $A$. Giả sử rằng $k$-đại số $A$ về cơ bản thuộc kiểu hữu hạn hoặc đầy đủ. Để vành địa phương $A/J$ là chính quy, điều kiện cần và đủ là tồn tại một số nguyên $m \geqslant 0$, các phần tử $f_1, \ldots, f_m$ của $J$ sinh ra $J$, và các đạo hàm $D_1, \ldots, D_m$ của $A$ sao cho $\det(D_j(f_i)) \notin \mathfrak{m}_A$. Khi đó các phần tử $(f_1, \ldots, f_m)$ tạo thành một phần của một hệ tọa độ của $A$ và iđêan $J$ là nguyên tố.*

Cho $k_0$ là trường con nguyên tố của $k$. $k_0$-đại số $A$ là chính quy tuyệt đối ($§ 6$, No. 4, ví dụ 1), do đó trơn hình thức (nhận xét 1 ở trên). Vì những lý do như vậy, nói rằng $A/J$ là chính quy tương đương với nói rằng nó là một $k_0$-đại số trơn hình thức. Do đó khẳng định thứ nhất suy ra từ định lý 3, định lý này cũng kéo theo rằng dãy $(f_1, \ldots, f_m)$ là hoàn toàn cát tuyến đối với $A$. Khi đó ta áp dụng mệnh đề 2 của VIII, $§ 5$, No. 3.

#### Nhận xét 2 {#ac-x-s7-n9-rem-2 .statement}

Dưới các giả thiết của hệ quả 3, $A$-môđun $\Omega(A)$ là xạ ảnh (No. 5, hệ quả 3 của định lý 2), do đó tự do; vì vậy mọi đạo hàm của $A$ vào $\kappa_A$ đều nâng được thành một đạo hàm của $A$. Vì thế điều kiện của mệnh đề có thể được phát biểu như sau: tồn tại một hệ sinh $(f_1, \ldots, f_m)$ của $J$ và các đạo hàm $D_1, \ldots, D_m$ của $A$ vào $\kappa_A$, sao cho $\det(D_j(f_i)) \neq 0$.

#### Hệ quả 4 (Zariski) {#ac-x-s7-thm-3-cor-4 .statement}

*Cho $k$ là một trường và $A$ là một $k$-đại số về cơ bản thuộc kiểu hữu hạn hoặc một vành địa phương Noether đầy đủ. Tập hợp các iđêan nguyên tố $\mathfrak{p}$ của $A$ sao cho vành địa phương $A_{\mathfrak{p}}$ là chính quy là mở trong $\mathrm{Spec}(A)$*.

Chỉ cần áp dụng Nhận xét 1, lấy cho $k_0$ trường con nguyên tố của $k$.

### 10. Đại số trơn

#### Bổ đề 5 {#ac-x-s7-lem-5 .statement}

*Cho $\rho : A \to B$ là một đồng cấu địa phương của các vành địa phương Noether. Giả sử rằng $B$ là về bản chất kiểu hữu hạn trên $A$. Để $B$-đại số $B$ là trơn hình thức trên $A$, điều kiện cần và đủ là $B$-môđun $B$ phẳng và $\kappa_A$-đại số $\kappa_A \otimes_A B$ là chính quy tuyệt đối.*

Tồn tại một số nguyên $n \geqslant 0$, một iđêan nguyên tố $q$ của $A[T_1, \ldots, T_n]$, và một đồng cấu toàn ánh $h$ từ $A[T_1, \ldots, T_n]_q$ lên $B$. Gọi $C$ là $A$-đại số địa phương $A[T_1, \ldots, T_n]_q$; nó là trơn hình thức (No. 3, Ví dụ 2 và No. 2, Mệnh đề 4, a)) và phẳng trên $A$, và có thể đồng nhất $B$ với $A$-đại số $C/J$, trong đó $J = \mathrm{Ker}(h)$.

Đặt $\overline{C} = \kappa_A \otimes_A C$ và $\overline{B} = \kappa_A \otimes_A B$. Giả sử rằng $B$ là trơn hình thức trên $A$. Khi đó $\kappa_A$-đại số $\overline{B}$ là trơn hình thức (No. 2, Mệnh đề 4, b)), do đó chính quy tuyệt đối (No. 5, Hệ quả 2 của Định lý 2). Hơn nữa, vì $\overline{C}/J\overline{C}$ có thể đồng nhất với $\overline{B}$ và $\kappa_A$-đại số $\overline{C}$ là trơn hình thức, iđêan $J\overline{C}$ của $\overline{C}$ là hoàn toàn cát tuyến (No. 5, Định lý 2). Khi đó suy ra từ § 5, No. 6, Mệnh đề 6 rằng $A$-môđun $B$ là phẳng.

Ngược lại, giả sử rằng $B$ phẳng trên $A$ và $\kappa_A$-đại số $\overline{B}$ là chính quy tuyệt đối. Khi đó $\kappa_A$-đại số địa phương $\overline{B}$ là trơn hình thức (Nhận xét 1 của No. 9 với $k = k_0 = \kappa_A$). Đặt $\overline{J} = \kappa_A \otimes_A J$; vì $B$ là một $A$-môđun phẳng, ánh xạ chính tắc $\overline{J} \to J\overline{C}$ là song ánh và $\overline{B}$ có thể đồng nhất với $\overline{C}/\overline{J}$. Suy ra (Nhận xét 1 của No. 2) rằng ánh xạ chính tắc

$$
\overline{J}/\overline{J}^2 \longrightarrow \overline{B} \otimes_{\overline{C}} \Omega_{\kappa_A}(\overline{C})
$$

là đơn ánh và thừa nhận một phép co rút. Bây giờ $\overline{J}/\overline{J}^2$ được đồng nhất với $\kappa_A \otimes_A J/J^2$, do đó với $\overline{B} \otimes_B J/J^2$; mặt khác, $\overline{C}$-môđun $\Omega_{\kappa_A}(\overline{C})$ đẳng cấu chính tắc với $\overline{C} \otimes_C \Omega_A(C)$ (A, III, p. 136, mệnh đề 20), do đó $\overline{B} \otimes_{\overline{C}} \Omega_{\kappa_A}(\overline{C})$ đẳng cấu chính tắc với $\overline{B} \otimes_C \Omega_A(C)$. Chuyển qua thương theo iđêan cực đại của $\overline{B}$, ta thu được một đồng cấu đơn cấu

$$
\kappa_B \otimes_B J/J^2 \longrightarrow \kappa_B \otimes_C \Omega_A(C)
$$

không là gì khác ngoài $d_{\kappa_B}$. Vậy B là trơn hình thức trên A (định lý 3).

#### Định lý 4 {#ac-x-s7-thm-4 .statement}

Cho A là một vành Noether và B là một đại số trên A thuộc kiểu hữu hạn về bản chất. Các điều kiện sau là tương đương:

(i) đại số trên A B là trơn hình thức ;
(ii) với mọi $q \in \mathrm{Spec}(B)$, đại số trên A $B_q$ là trơn hình thức (resp. trơn hình thức đối với tôpô $qB_q$-adic) ;
(iii) A-môđun B là phẳng và, với mọi $p \in \mathrm{Spec}(A)$, $\kappa(p)\text{-đại số} \ \kappa(p) \otimes_A B$ là chính quy tuyệt đối ;
(iv) A-môđun B là phẳng và, với mọi đại số trên A chính quy R, vành $R \otimes_A B$ là chính quy ;
(v) A-môđun B là phẳng và hạt nhân của đồng cấu $\mu : B \otimes_A B \to B$ sao cho $\mu(x \otimes y) = xy$ là một iđêan cát hoàn toàn.

Sự tương đương của (i) và (ii) suy ra từ hệ quả 2 của định lý 3 (No. 9).

(i)⇒(v) : giả sử đại số trên A B là trơn hình thức. Cho q là một iđêan nguyên tố của B, và p là ảnh ngược của nó trong A. Đại số trên $A_p$ $B_q$ là trơn hình thức (mệnh đề 4, a) của No. 2), nên phẳng (bổ đề 5) ; do đó A-môđun B là phẳng (II, § 3, No. 4, mệnh đề 15). Mặt khác, vành $B \otimes_A B$ là Noether (§ 6, No. 1, hệ quả của mệnh đề 2), nên iđêan $\mathrm{Ker}\,\mu$ là cát hoàn toàn theo hệ quả 3 của định lý 2 (No. 5).

(v)⇒(iii) : giả sử điều kiện (v) được thỏa mãn. Đặt $I = \mathrm{Ker}(\mu)$. Cho $p \in \mathrm{Spec}(A)$. Ánh xạ

$$
1 \otimes \mu : \kappa(p) \otimes_A (B \otimes_A B) \to \kappa(p) \otimes_A B
$$

được đồng nhất với ánh xạ

$$
\mu_p : (\kappa(p) \otimes_A B) \otimes_{\kappa(p)} (\kappa(p) \otimes_A B) \to \kappa(p) \otimes_A B
$$

suy ra từ phép nhân của $\kappa(p)\text{-đại số} \ \kappa(p) \otimes_A B$. Iđêan $\mathrm{Ker}(\mu_p)$ được đồng nhất với $I(\kappa(p) \otimes_A (B \otimes_A B))$. Nó là cát hoàn toàn vì A-môđun B là phẳng (§ 5, No. 6, mệnh đề 6). Khi đó mệnh đề (iii) suy ra từ mệnh đề 8 của § 6, No. 5.

(iii)⇒(ii) : cho q là một iđêan nguyên tố của B, và p là ảnh ngược của nó trong A. Dưới các giả thiết của (iii), $A_p$-môđun $B_q$ là phẳng, và $\kappa(p)\text{-đại số} \ \kappa(p) \otimes_{A_p} B_q$, được đồng nhất với một vành phân thức của $\kappa(p) \otimes_A B$, là chính quy tuyệt đối (§ 6, No. 4, mệnh đề 6). Từ bổ đề 5 suy ra rằng $B_q$ là trơn hình thức trên $A_p$, nên trên A (No. 2, mệnh đề 3 và 4).

(iii)⇒(iv) : hãy đặt mình dưới các giả thiết của (iii). Cho R là một đại số trên A chính quy. R-môđun $R \otimes_A B$ là phẳng (I, § 2, No. 7, hệ quả 2 của mệnh đề 8). Cho r là một iđêan nguyên tố của R và p là ảnh ngược của nó trong A ; vành $\kappa(r) \otimes_R (R \otimes_A B)$, được đồng nhất với $\kappa(r) \otimes_{\kappa(p)} (\kappa(p) \otimes_A B)$, là chính quy (§ 6, No. 4, hệ quả 2 của mệnh đề 7). Vậy vành $R \otimes_A B$ là chính quy (§ 4, No. 5, hệ quả của mệnh đề 9).

(iv) ⇒ (iii) : cho $p$ là một iđêan nguyên tố của $A$ và cho $k$ là một mở rộng của $\kappa(p)$; dưới các giả thiết của (iv), vành $k \otimes_{\kappa(p)} (\kappa(p) \otimes_A B)$, được đồng nhất với $k \otimes_A B$, là chính quy, do đó có (iii).

#### Định nghĩa 2 {#ac-x-s7-def-2 .statement}

Cho $A$ là một vành Noether. Một đại số trên $A$ $B$ được gọi là trơn nếu nó thuộc kiểu hữu hạn về bản chất và nếu nó thỏa mãn các điều kiện tương đương của định lý 4.

#### Mệnh đề 10 {#ac-x-s7-prop-10 .statement}

Cho $A$ là một vành Noether.

a) Cho $A'$ là một đại số trên $A$ Noether và $B$ là một đại số trên $A$ trơn. Khi đó đại số trên $A'$ $A' \otimes_A B$ là trơn.

b) Cho $B$ là một $A$-đại số trơn và $C$ là một $B$-đại số trơn. Khi đó $A$-đại số $C$ là trơn.

c) Cho $B$ và $C$ là hai $A$-đại số trơn. Khi đó $A$-đại số $B \otimes_A C$ là trơn.

Điều này suy ra từ Mệnh đề 4 của No. 2 và từ các mệnh đề tương tự đối với các đại số cốt yếu kiểu hữu hạn (§ 6, No. 1).

#### Ví dụ 1 {#ac-x-s7-n10-exa-1 .statement}

Các đại số trơn trên một trường $k$ là các $k$-đại số cốt yếu kiểu hữu hạn và chính quy tuyệt đối.

#### Ví dụ 2 {#ac-x-s7-n10-exa-2 .statement}

Cho $A$ là một vành Noether, $T = (T_i)_{i \in I}$ là một họ hữu hạn các ẩn. $A$-đại số $A[T]$ là trơn. Tổng quát hơn, cho $F_1, \ldots, F_m$ là các phần tử của $A[T]$, và cho $B$ là $A$-đại số $A[T]/(F_1, \ldots, F_m)$. Nếu tại mọi iđêan cực đại $n$ của $B$, lớp (mod. $n$) của ma trận $\left( \frac{\partial F_j}{\partial T_i} \right)$ có hạng $m$, thì $A$-đại số $B$ là trơn (Định lý 3 của No. 9).

## BÀI TẬP {#ac-x-s7-exercises}

Xem [các bài tập của § 7](exercises/s7/).
