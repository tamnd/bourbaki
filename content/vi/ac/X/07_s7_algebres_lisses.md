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
content_sha256: 81fa7e7e411169ce5429ab6c417df000de35e2770aeb931704d7d8b046f9a852
translated_from: content/en-mt/ac/X/07_s7_algebres_lisses.md
source_lang: en-mt
translation_method: machine
source_content_sha256: aaa34242d598f6821b0738736697b9b060d8724ab44b075a978f529e09bfce6c
translation_model: gpt-5-mini, gpt-5-6-mini, gpt-5-6
translation_run: translate-vi-65bb4a06
glossary_version: 34
glossary_terms_sha256: a5f8bb4f5717d2b9911457f7bb573517e88c7238cf3a01bcf6c21f9392f347e2
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 7. ĐẠI SỐ TRƠN

### 1. Các đạo hàm và các phép nâng của các đồng cấu

Cho $k$ là một vành, $C$ là một $k$-đại số và $N$ là một iđêan của $C$ có bình phương bằng không. Gọi $\pi : C \to C/N$ là đồng cấu chính tắc; vì $N^2 = \{0\}$, cấu trúc môđun $C$ trên $N$ xuất phát từ một cấu trúc môđun $C/N$.

Cho $A$ là một $k$-đại số và $\varphi : A \to C/N$ là một đồng cấu của các $k$-đại số. Trang bị cho $N$ cấu trúc $A$-môđun suy ra từ $\varphi$. Một *phép nâng của $\varphi$* (lên $C$) được hiểu là bất kỳ đồng cấu nào của các $k$-đại số $\tilde{\varphi} : A \to C$ sao cho $\pi \circ \tilde{\varphi} = \varphi$. Cho $\tilde{\varphi}$ là một phép nâng như vậy, và $\delta$ là một ánh xạ của $A$ vào $N$; ký hiệu $\delta + \tilde{\varphi}$ là ánh xạ $x \mapsto \delta(x) + \tilde{\varphi}(x)$ của $A$ vào $C$.

#### Mệnh đề 1 {#ac-x-s7-prop-1 .statement}

*Nếu $\varphi$ thừa nhận một phép nâng, ánh xạ $(\delta, \tilde{\varphi}) \mapsto \delta + \tilde{\varphi}$ xác định một phép toán bắc cầu đơn của nhóm các $k$-đạo hàm của $A$ vào $N$ trên tập hợp các phép nâng của $\varphi$.*

Cho $\tilde{\varphi}_0 : A \to C$ là một phép nâng của $\varphi$. Ánh xạ $\delta \mapsto \delta + \tilde{\varphi}_0$ cảm sinh một song ánh của tập hợp các ánh xạ của $A$ vào $N$ lên tập hợp các ánh xạ $\tilde{\varphi} : A \to C$ sao cho $\pi \circ \tilde{\varphi} = \varphi$. Cố định $\delta$, và đặt $\tilde{\varphi} = \delta + \tilde{\varphi}_0$. Để $\tilde{\varphi}$ là một đồng cấu của các $k$-đại số, điều kiện cần và đủ là $\delta$ là một $k$-đạo hàm của $A$ vào $N$: thật vậy, với $x, y$ trong $A$ và $\lambda$ trong $k$, ta có các đẳng thức

$$
\begin{align*}
\tilde{\varphi}(x + y) - \tilde{\varphi}(x) - \tilde{\varphi}(y) &= \delta(x + y) - \delta(x) - \delta(y) \\
\tilde{\varphi}(\lambda x) - \lambda \tilde{\varphi}(x) &= \delta(\lambda x) - \lambda \delta(x) \\
\tilde{\varphi}(xy) - \tilde{\varphi}(x)\tilde{\varphi}(y) &= \delta(xy) - \delta(x)\delta(y) - \delta(x)\tilde{\varphi}_0(y) - \tilde{\varphi}_0(x)\delta(y) \\
&= \delta(xy) - \varphi(x)\delta(y) - \varphi(y)\delta(x),
\end{align*}
$$

đẳng thức cuối cùng suy ra từ sự kiện rằng $N$ có bình phương bằng không. Mệnh đề được chứng minh từ đây.

#### Ví dụ {#ac-x-s7-n1-exa-1 .statement}

Cho $B$ là một $k$-đại số, $N$ là một $B$-môđun. Trang bị cho $k$-môđun $B \oplus N$ cấu trúc của một $k$-đại số xác định bởi $(b, x)(b', x') = (bb', bx' + b'x)$ (*cf.* A, III, p. 127), sao cho $N$ là một iđêan bình phương bằng không của $B \oplus N$. Cho $\varphi : A \to B$ là một đồng cấu của các $k$-đại số. Khi đó các phép nâng của $\varphi$ lên $B \oplus N$ là các ánh xạ $x \mapsto (\varphi(x), \delta(x))$, trong đó $\delta$ chạy qua tập hợp các đạo hàm $k$-của $A$ vào $N$ (*cf. loc. cit.*, mệnh đề 12).

Cho $\Omega_k(A)$ là môđun các vi phân $k$ của vành $A$, và cho $d : A \longrightarrow \Omega_k(A)$ là đạo hàm $k$ phổ quát (A, III, p. 133 và 134); ta nhắc lại (*loc. cit.*) rằng với mọi $A$-môđun $M$, ánh xạ $v \mapsto v \circ d$ là một đẳng cấu $A$-tuyến tính từ $\mathrm{Hom}_A(\Omega_k(A), M)$ lên môđun $A$ của các đạo hàm $k$ của $A$ vào $M$.

Cho J là một iđêan của A. Theo A, III, p. 137, ta có một dãy khớp của các ánh xạ $A/J$-tuyến tính

$$
J/J^2 \xrightarrow{\bar{d}} (\Lambda/J) \otimes_A \Omega_k(\Lambda) \longrightarrow \Omega_k(A/J) \to 0,
$$

trong đó $\bar{d}$ là đồng cấu cảm sinh bởi chuyển qua thương từ hạn chế của $d$ lên J.

Cho $\rho : A \to A/J^2$ và $\pi : A/J^2 \to A/J$ lần lượt là các toàn ánh chính tắc. Cho $v : (A/J) \otimes_A \Omega_k(A) \longrightarrow J/J^2$ là một ánh xạ $k$-tuyến tính; với nó ta liên kết một ánh xạ $k$-tuyến tính $H_v : A \to A/J^2$ bằng cách đặt $H_v(x) = \rho(x) - v(1 \otimes dx)$. Nếu $v$ là một phép co của $\bar{d}$, $H_v$ triệt tiêu trên J, do đó cảm sinh bởi chuyển qua thương một ánh xạ $k$-tuyến tính $h_v : A/J \to A/J^2$. Mặt khác, cho một ánh xạ $k$-tuyến tính $h : A/J \to A/J^2$, ta ký hiệu bởi $\psi_h : A/J \oplus J/J^2 \longrightarrow A/J^2$ ánh xạ $(x, y) \mapsto h(x) + y$.

#### Mệnh đề 2 {#ac-x-s7-prop-2 .statement}

Trang bị cho $k$-môđun $\Lambda/J \oplus J/J^2$ cấu trúc của một $k$-đại số xác định trong ví dụ trên. Các ánh xạ $v \mapsto h_v$ và $h \mapsto \psi_h$ cảm sinh các song ánh giữa các tập hợp sau :

(i) tập hợp các phép rút tuyến tính theo $A/J$ $v$ của $\bar{d}$ ;
(ii) tập hợp các đồng cấu của các đại số $k$ $h : A/J \to A/J^2$ sao cho $\pi \circ h = \mathrm{Id}_{A/J}$ ;
(iii) tập hợp các đẳng cấu của các đại số $k$ $\psi : A/J \oplus J/J^2 \longrightarrow A/J^2$ sao cho $\pi \circ \psi = \mathrm{pr}_1$ và $\psi(0, z) = z$ với $z \in J/J^2$.

Áp dụng Mệnh đề 1 với $C = A/J^2$ và $N = J/J^2$. Cho $\varphi : A \to A/J$ là toàn cấu chính tắc ; đồng cấu $\rho$ là một phép nâng của $\varphi$ lên $A/J^2$. $A$-môđun $\mathrm{Hom}_{A/J}((A/J) \otimes_A \Omega_k(A), J/J^2)$ được đồng nhất với $\mathrm{Hom}_A(\Omega_k(A), J/J^2)$ ; sau Mệnh đề 1, ánh xạ $v \mapsto H_v$ là một song ánh từ tập hợp này lên tập hợp các phép nâng của $\varphi$ lên $A/J^2$. Với $x \in J$, ta có $1 \otimes dx = \bar{d}(\rho(x))$ ; để $H_v$ triệt tiêu trên J, điều kiện cần và đủ là $v \circ \bar{d}$ là ánh xạ đồng nhất của $J/J^2$. Điều này chứng minh rằng ánh xạ $v \mapsto h_v$ cảm sinh một song ánh giữa hai tập hợp đầu tiên được mô tả trong mệnh đề.

Ánh xạ $h \mapsto \psi_h$ là một song ánh từ tập hợp các đồng cấu tuyến tính theo $k$ của $A/J$ vào $A/J^2$ lên tập hợp các đồng cấu tuyến tính theo $k$ $\psi : A/J \oplus J/J^2 \longrightarrow A/J^2$ sao cho $\psi(0, z) = z$ với $z \in J/J^2$ ; hơn nữa, để $\pi \circ \psi_h = \mathrm{pr}_1$ đúng, điều kiện cần và đủ là $\pi \circ h = \mathrm{Id}_{A/J}$, nghĩa là $z \equiv h(\pi(z)) \pmod{J/J^2}$ với mọi $z \in A/J^2$. Giả sử các điều kiện này được thỏa mãn. Để $h$ là một đồng cấu vành, điều kiện cần và đủ là điều tương tự đúng đối với $\psi_h$ ; hơn nữa, đồng cấu $\psi_h$ là song ánh : ánh xạ nghịch đảo gán cho một phần tử $z$ của $A/J^2$ cặp $(\pi(z), z - h(\pi(z)))$. Điều này chứng minh rằng ánh xạ $h \mapsto \psi_h$ cảm sinh một song ánh giữa hai tập hợp cuối cùng được mô tả trong mệnh đề.

### 2. Các đại số trơn hình thức

Cho $k$ là một vành và $A$ là một đại số $k$ có tôpô tuyến tính (III, § 4, No. 2, Định nghĩa 1).

#### Định nghĩa 1 {#ac-x-s7-def-1 .statement}

Người ta nói rằng $A$ là trơn hình thức trên $k$, hay là một $k$-đại số trơn hình thức, nếu nó thỏa mãn điều kiện sau: bất kể $k$-đại số $C$ và iđêan bình phương không $N$ của $C$ là gì, mọi đồng cấu liên tục từ $A$ vào $k$-đại số $C/N$, được trang bị tôpô rời rạc, đều có thể được nâng lên thành một đồng cấu liên tục từ $A$ vào $k$-đại số $C$, được trang bị tôpô rời rạc.

Nhắc lại rằng một đồng cấu từ $A$ vào một $k$-đại số được trang bị tôpô rời rạc là liên tục khi và chỉ khi hạt nhân của nó là mở.

Cho $k$ là một vành, $A$ là một $k$-đại số và $J$ là một iđêan của $A$. Trang bị cho $A$ tôpô $J$-adic. Cho $C$ là một $k$-đại số, $N$ là một iđêan bình phương không của $C$; trang bị cho $C$ và $C/N$ tôpô rời rạc. Cho $\varphi : A \to C/N$ là một đồng cấu liên tục của các đại số. Mọi phép nâng $\tilde{\varphi} : A \to C$ của $\varphi$ đều liên tục: thực vậy tồn tại một số nguyên $n$ sao cho $\varphi(J^n)$ là không, và ta có $\tilde{\varphi}(J^n) \subset N$, do đó $\tilde{\varphi}(J^{2n}) \subset N^2 = 0$. Suy ra đặc biệt rằng, nếu $A$ là trơn hình thức đối với tôpô $J$-adic, thì nó cũng là trơn hình thức đối với tôpô $J'$-adic đối với mọi iđêan $J'$ chứa $J$.

Ta sẽ nói rằng một $k$-đại số $A$ là trơn hình thức nếu nó là trơn hình thức khi được trang bị tôpô rời rạc, nghĩa là, tôpô $(0)$-adic; khi đó nó là trơn hình thức đối với tôpô $J$-adic bất kể iđêan $J$ của $A$ là gì.

#### Nhận xét 1 {#ac-x-s7-n2-rem-1 .statement}

Cho $k$ là một vành, $A$ là một $k$-đại số và $J$ là một iđêan của $A$. Nếu $k$-đại số $A/J$ là trơn hình thức (đối với tôpô rời rạc), ánh xạ đồng nhất của $A/J$ có một phép nâng lên $A/J^2$; do đó các tập hợp được mô tả trong Mệnh đề 2 là không rỗng. Đặc biệt, dãy

$$
0 \to J/J^2 \xrightarrow{\bar{d}} (A/J) \otimes_A \Omega_k(A) \longrightarrow \Omega_k(A/J) \to 0
$$

là khớp và tách.

#### Nhận xét 2 {#ac-x-s7-n2-rem-2 .statement}

Cho $k$ là một vành, $A$ là một đại số $k$ trơn hình thức được tôpô tuyến tính, $M$ là một $A$-môđun có linh hóa tử là mở trong $A$. Khi đó mọi đạo hàm $\delta$ của $k$ vào $M$ mở rộng được thành một đạo hàm của $A$ vào $M$. Thật vậy, đặt $B = A/Ann(M)$; ánh xạ $\lambda \mapsto (\lambda 1_B, \delta(\lambda))$ xác định một đồng cấu vành từ $k$ vào $B \oplus M$ (No. 1, Ví dụ), nghĩa là, một cấu trúc đại số $k$ trên $B \oplus M$. Toàn cấu chính tắc $\varphi : A \to B$ là liên tục, và do đó thừa nhận một nâng $\tilde{\varphi} : A \to B \oplus M$; theo loc. cit., $pr_2 \circ \tilde{\varphi}$ là một đạo hàm của $A$ vào $M$ mở rộng $\delta$.

#### Mệnh đề 3 {#ac-x-s7-prop-3 .statement}

Cho $k$ là một vành.

a) Cho $A$ và $B$ là các đại số $k$ được tôpô tuyến tính và $\rho : A \to B$ là một đồng cấu liên tục của các đại số $k$. Nếu $A$ là trơn hình thức trên $k$ và $B$ là trơn hình thức trên $A$, thì $B$ là trơn hình thức trên $k$.

b) Đại số $k$ tích của một họ hữu hạn các đại số $k$ trơn hình thức được tôpô tuyến tính là trơn hình thức.

c) Cho $A$ là một đại số $k$ được tôpô tuyến tính, và $\hat{A}$ là đại số hoàn thành tách được của $A$; để $A$ là trơn hình thức trên $k$, điều kiện cần và đủ là điều này đúng với $\hat{A}$.

Cho C là một đại số $k$, N là một iđêan bình phương-không của C, và $\pi : C \to C/N$ là toàn cấu chính tắc. Trang bị cho C và C/N tôpô rời rạc.

a) Cho $\psi : B \to C/N$ là một đồng cấu liên tục của các đại số $k$. Vì A là trơn hình thức trên $k$, tồn tại một đồng cấu liên tục của các đại số $k$ $\tilde{\varphi} : A \to C$ sao cho $\pi \circ \tilde{\varphi} = \psi \circ \rho$.

$$
\begin{array}{ccc}
 & & C \\
 & \swarrow_{\tilde{\varphi}} & \\
A \xrightarrow{\rho} B \xrightarrow{\psi} C/N & & \downarrow^{\pi}
\end{array}
$$

Xét C và C/N như các đại số $A$ bằng cách dùng $\tilde{\varphi}$, sao cho $\psi$ là một đồng cấu của các đại số $A$; vì B là trơn hình thức trên A, tồn tại một đồng cấu liên tục của các đại số A $\tilde{\psi} : B \to C$ sao cho $\pi \circ \tilde{\psi} = \psi$, do đó a).

b) Chỉ cần chứng minh rằng tích của hai $k$-đại số trơn hình thức $A_1$ và $A_2$ là trơn hình thức. Cho $\varphi : A_1 \times A_2 \to C/N$ là một đồng cấu liên tục của các $k$-đại số. Đặt $e_1 = \varphi(1,0)$, $e_2 = \varphi(0,1)$, khi đó $e_1$ và $e_2$ là các phần tử lũy đẳng trực giao trong C/N. Gọi $\varphi_1 : A_1 \to (C/N)e_1$ và $\varphi_2 : A_2 \to (C/N)e_2$ là các ánh xạ được xác định bởi $\varphi_1(a_1) = \varphi(a_1,0)$ và $\varphi_2(a_2) = \varphi(0,a_2)$; đây là các đồng cấu liên tục của các $k$-đại số, và ta có $\varphi(a_1, a_2) = \varphi_1(a_1) + \varphi_2(a_2)$ với mọi $(a_1, a_2) \in A_1 \times A_2$. Tồn tại một phần tử lũy đẳng $\tilde{e}_1$ của C sao cho $\pi(\tilde{e}_1) = e_1$ (A, VIII, § 9, No. 4, Prop. 7); đặt $\tilde{e}_2 = 1 - \tilde{e}_1$, khi đó $\pi(\tilde{e}_2) = e_2$. Với $i = 1, 2$, đồng cấu $C\tilde{e}_i \to (C/N)e_i$ cảm sinh bởi $\pi$ là toàn ánh, với hạt nhân $N\tilde{e}_i$; vì $k$-đại số $A_i$ là trơn hình thức, đồng cấu $\varphi_i$ có một phép nâng liên tục $\tilde{\varphi}_i$ lên $C\tilde{e}_i$. Ánh xạ $(a_1, a_2) \mapsto \tilde{\varphi}_1(a_1) + \tilde{\varphi}_2(a_2)$ là một phép nâng liên tục của $\varphi$ lên C.

c) Gọi $i : A \to \widehat{A}$ là đồng cấu chính tắc. Với mọi vành D, được trang bị tôpô rời rạc, ánh xạ gán cho một đồng cấu liên tục $f : \widehat{A} \to D$ đồng cấu liên tục $f \circ i : A \to D$ là song ánh. Mệnh đề c) suy ra từ điều này.

Mệnh đề c) áp dụng riêng biệt trong trường hợp tôpô của $\Lambda$ là tôpô J-adic, trong đó J là một iđêan kiểu hữu hạn; bao đóng $\widehat{J}$ của J trong $\widehat{A}$ khi đó bằng $JA$ và tôpô của $\widehat{A}$ là tôpô $\widehat{J}$-adic (III, § 2, No. 12, Hệ quả 2 của Mệnh đề 16). Do đó, nói rằng A trơn hình thức đối với tôpô J-adic hay rằng hoàn thiện tách được của nó $\widehat{A}$ là trơn hình thức đối với tôpô J-adic là tương đương.

#### Mệnh đề 4 {#ac-x-s7-prop-4 .statement}

Cho k là một vành, A và B là các $k$-đại số, J là một iđêan của A, K là một iđêan của B.

a) Cho S là một tập con nhân của A và T là một tập con của k mà ảnh của nó trong A được chứa trong S. Nếu A trơn hình thức trên k đối với tôpô J-adic, thì S $^1\Lambda$ là trơn hình thức trên $T^{-1}k$ đối với tôpô $S^{-1}J$-adic.

b) Cho $k'$ là một $k$-đại số. Nếu $A$ trơn hình thức trên $k$ đối với tôpô $J$-adic, thì $k'$-đại số $A_{(k')}$ là trơn hình thức trên $k'$ đối với tôpô $JA_{(k')}$-adic.

c) Gọi $I$ là iđêan của $A \otimes_k B$ sinh bởi các ảnh của $J \otimes_k B$ và $A \otimes_k K$. Nếu $A$ và $B$ là trơn chính thức trên $k$ đối với các tôpô $J$-adic và $K$-adic tương ứng, thì đại số $k$-đại số $A \otimes_k B$ là trơn chính thức đối với tôpô $I$-adic.

a) Dưới các giả thiết của a), cho $C$ là một $T^{-1}k$-đại số, và $N$ là một iđêan bình phương bằng không của $C$; trang bị cho $C$ và $C/N$ tôpô rời rạc, và gọi $\pi : C \to C/N$ là toàn cấu chính tắc. Cho $\varphi : S^{-1}A \longrightarrow C/N$ là một đồng cấu của các $T^{-1}k$-đại số, liên tục đối với tôpô $S^{-1}J$-adic. Gọi $i$ là đồng cấu chính tắc của $A$ vào $S^{-1}A$. Ánh xạ $\varphi \circ i$ là một đồng cấu của các $k$-đại số, liên tục đối với tôpô $J$-adic, và do đó có một nâng $\tilde{\varphi}_0 : A \to C$. Các phần tử của $\tilde{\varphi}_0(S)$ là khả nghịch modulo $N$, do đó khả nghịch vì $N$ là bình phương bằng không. Suy ra rằng tồn tại một đồng cấu vành $\tilde{\varphi} : S^{-1}A \to C$ sao cho $\tilde{\varphi} \circ i = \tilde{\varphi}_0$ (II, § 2, No. 1, Mệnh đề 1); theo Hệ quả 3 đối với Mệnh đề 2 của tài liệu đã dẫn, $\tilde{\varphi}$ là $T^{-1}k$-tuyến tính. Ta có $\pi \circ \tilde{\varphi} \circ i = \varphi \circ i$, do đó $\pi \circ \tilde{\varphi} = \varphi$ (tài liệu đã dẫn, Mệnh đề 1), vì vậy $\tilde{\varphi}$ là một nâng của $\varphi$.

b) Ta đặt mình dưới các giả thiết của b). Cho $C$ là một $k'$-đại số, $N$ là một iđêan bình phương bằng không của $C$; trang bị cho $C$ và $C/N$ tôpô rời rạc. Cho $\varphi : A_{(k')} \longrightarrow C/N$ là một đồng cấu của các $k'$-đại số, liên tục đối với tôpô $JA_{(k')}$-adic. Ký hiệu $i : A \to A_{(k')}$ là đồng cấu chính tắc. Ánh xạ $\varphi \circ i$ là một đồng cấu của các $k$-đại số từ $A$ vào $C/N$, liên tục đối với tôpô $J$-adic; nếu $A$ trơn hình thức trên $k$ đối với tôpô $J$-adic, $\varphi \circ i$ có một phép nâng $\tilde{\psi} : A \to C$. Đồng cấu của các $k'$-đại số $\tilde{\varphi} : A_{(k')} \longrightarrow C$ suy ra từ $\tilde{\psi}$ là một phép nâng của $\varphi$.

c) Ta đặt mình dưới các giả thiết của c). $B$-đại số $A \otimes_k B$ là trơn hình thức đối với tôpô $J(A \otimes_k B)$-adic theo b), do đó đối với tôpô $I$-adic; hơn nữa đồng cấu chính tắc $B \to A \otimes_k B$ là liên tục khi $B$ được trang bị tôpô $K$-adic và $A \otimes_k B$ được trang bị tôpô $I$-adic. Do đó mệnh đề c) suy ra từ mệnh đề 3, a).

### 3. Các ví dụ về các đại số trơn hình thức

Cho $k$ là một vành.

1) Cho $P$ là một $k$-môđun xạ ảnh. $k$-đại số đối xứng $S_k(P)$ là trơn hình thức đối với tôpô rời rạc, và $a fortiori$ đối với tôpô được xác định bởi phép phân bậc của nó. Thật vậy, với mọi $k$-đại số $C$ và mọi iđêan $N$ của $C$, các đồng cấu đại số từ $S_k(P)$ vào $C$ (tương ứng $C/N$) có sự tương ứng song ánh với các ánh xạ $k$-tuyến tính từ $P$ vào $C$ (tương ứng $C/N$), và ánh xạ chính tắc $\mathrm{Hom}_k(P, C) \to \mathrm{Hom}_k(P, C/N)$ là toàn ánh.

Do đó (mệnh đề 3, c)), $k$-đại số $\hat{S}_k(P) = \prod_{n \geq 0} S_k^n(P)$ là trơn hình thức (đối với tôpô tích của các tôpô rời rạc trên các $S_k^n(P)$): thật vậy nó là hoàn thành của $k$-đại số $S_k(P)$ đối với tôpô được xác định bởi phép phân bậc.

2) Với mọi họ các phần tử bất định $\mathbf{T} = (T_i)_{i \in I}$, đại số đa thức $k$-đại số $k[\mathbf{T}]$, và đại số chuỗi lũy thừa hình thức $k$-đại số $k[[\mathbf{T}]]$ được trang bị tôpô chính tắc của nó, đều trơn hình thức; điều này suy ra từ ví dụ 1. Nếu $k$ là một trường, mở rộng siêu việt thuần túy $k(\mathbf{T})$ là trơn hình thức (No. 2, Mệnh đề 4 a)).

3) Cho $f \in k[T]$ là một đa thức theo một phần tử bất định. Nói rằng $k$-đại số $k[T]/(f)$ là trơn hình thức có nghĩa là tính chất sau đây được thỏa mãn: *với mọi $k$-đại số $C$ và mọi iđêan bình phương bằng không $N$ của $C$, mọi nghiệm của $f$ trong $C/N$ đều có thể được nâng lên thành một nghiệm của $f$ trong $C$*. Điều này đúng khi $f$ và đạo hàm của nó $f'$ sinh iđêan đơn vị. Thật vậy, cho $\alpha$ là một nghiệm của $f$ trong $C/N$ và cho $a$ là một phần tử của $C$ nâng $\alpha$. Khi đó $f(a)$ thuộc $N$ và do đó $f'(a)$ là khả nghịch trong $C$; phần tử $b = a - f'(a)^{-1} f(a)$ nâng $\alpha$. Vì $f'(a)^{-1} f(a)$ có bình phương bằng không, ta có

$$
f(b) = f(a) - f'(a) f'(a)^{-1} f(a) = 0 .
$$

**Định lý 1** (I. S. Cohen). *Cho $k$ là một trường và $K$ là một mở rộng tách được của $k$. Khi đó $K$ là một $k$-đại số trơn hình thức.*

Cho $C$ là một $k$-đại số, $N$ là một iđêan bình phương bằng không của $C$, $\pi : C \to C/N$ là đồng cấu chính tắc và $\varphi : K \to C/N$ là một đồng cấu của các $k$-đại số. Ta phải xây dựng một phép nâng của $\varphi$. Hãy phân biệt hai trường hợp.

A) Trước hết giả sử rằng $k$ có đặc số 0. Xét các cặp $(K', \tilde{\varphi}')$, trong đó $K'$ là một mở rộng con của $K$ và $\tilde{\varphi}' : K' \to C$ là một phép nâng của hạn chế của $\varphi$ lên $K'$. Tập hợp các cặp này, được trang bị cấp xác định bởi quan hệ mở rộng, là quy nạp; theo định lý Zorn (E, III, p. 20, đl. 2), tồn tại một cặp cực đại $(K', \tilde{\varphi}')$. Ta hãy chứng minh rằng $K'$ bằng $K$. Cho $x \in K - K'$. Nếu $x$ là siêu việt trên $K'$, đại số $K'$-đại số $K'(x)$ là trơn hình thức (ví dụ 2). Nếu $x$ là đại số trên $K'$, đa thức tối tiểu của nó $f \in K'[T]$ nguyên tố cùng nhau với đạo hàm của nó (A, V, p. 37, Mệnh đề 4), và $K'(x)$ được đồng nhất với $K'$-đại số $K'[T]/(f)$, do đó là một $K'$-đại số trơn hình thức (ví dụ 3). Trong cả hai trường hợp, $K'(x)$ là trơn hình thức trên $K'$, và tồn tại một mở rộng của $\tilde{\varphi}'$ lên $K'(x)$ nâng hạn chế của $\varphi$ lên $K'(x)$, điều này mâu thuẫn với đặc trưng cực đại của $(K', \tilde{\varphi}')$.

B) Giả sử rằng $k$ có đặc số $p \neq 0$. Xét đồng cấu vành $F : C \to C$ sao cho $F(x) = x^p$; ta có $F(x) = 0$ với $x \in N$, do đó tồn tại một đồng cấu vành duy nhất $\lambda : C/N \to C$ sao cho $\lambda \circ \pi = F$. Ta có $\pi(\lambda(\pi(x))) = \pi(x^p) = \pi(x)^p$; vì $\pi$ là toàn ánh, do đó ta có $\pi(\lambda(z)) = z^p$ với mọi phần tử $z$ của $C/N$. Hơn nữa, gọi $f : K \to K^p$ là đẳng cấu $y \mapsto y^p$ và $f^{-1} : K^p \to K$ là đẳng cấu ngược. Gọi $g : K^p \to C$ là hợp của dãy các đồng cấu vành

$$
\begin{array}{ccccccccc}
K^p & \xrightarrow{f^{-1}} & K & \xrightarrow{\varphi} & C/N & \xrightarrow{\lambda} & C .
\end{array}
$$

Với mọi $x \in K$, ta có $g(x^p) = \lambda(\varphi(x))$. Vì $\lambda(\alpha z) = \alpha^p \lambda(z)$ với $\alpha \in k$ và $z \in C/N$, ánh xạ $g$ là $k^p$-tuyến tính. Vì mở rộng $K$ của $k$ là tách được, $k(K^p)$ được đồng nhất với $k \otimes_{k^p} K^p$ (A, V, p. 119, nhận xét); do đó tồn tại một đồng cấu duy nhất của các $k$-đại số $h : k(K^p) \to C$ trùng với $g$ trên $K^p$.

Cho $(a_i)_{i \in I}$ là một cơ sở-$p$ của $K$ trên $k(K^p)$ (A, V, p. 98, định lý 2); với mọi $i \in I$, chọn một phần tử $b_i$ của $C$ sao cho $\pi(b_i) = \varphi(a_i)$. Ta có $h(a_i^p) = g(a_i^p) = \lambda(\varphi(a_i)) = \lambda(\pi(b_i)) = b_i^p$ với mọi $i \in I$. Theo A, V, p. 94, nhận xét, tồn tại một đồng cấu của các $k$-đại số $\tilde{\varphi} : K \to C$, mở rộng $h$ và sao cho $\tilde{\varphi}(a_i) = b_i$ với mọi $i$. Ta có $\pi(\tilde{\varphi}(a_i)) = \pi(b_i) = \varphi(a_i)$ với mọi $i$ và $\pi(\tilde{\varphi}(x^p)) = \pi(h(x^p)) = \pi(g(x^p)) = \pi(\lambda(\varphi(x))) = \varphi(x^p)$ với mọi $x \in K$. Do đó $\pi \circ \tilde{\varphi} = \varphi$, điều này hoàn tất chứng minh.

#### Hệ quả {#ac-x-s7-n3-cor-1 .statement}

Cho $k$ là một trường, $K$ là một mở rộng tách được của $k$ và $A$ là một $K$-đại số có tôpô tuyến tính. Nếu $A$ là trơn hình thức trên $K$, thì nó là trơn hình thức trên $k$.

Điều này suy ra từ định lý và mệnh đề 3 a) của No. 2.

#### Nhận xét 1 {#ac-x-s7-n3-rem-1 .statement}

Cho $k$ là một trường. Mọi $k$-đại số étale (A, V, p. 28, def. 1) đều trơn hình thức (*loc. cit.*, p. 34, th. 4, d) và No. 2, prop. 3, b)).

#### Nhận xét 2 {#ac-x-s7-n3-rem-2 .statement}

Ta sẽ thấy dưới đây (hệ quả 2 của định lý 2 của No. 5) rằng một mở rộng trường trơn hình thức là tuyệt đối chính quy, do đó tách được (§ 6, No. 4, ví dụ 2).

### 4. Các phép nâng của các đồng cấu trong các đại số lọc đầy đủ

Cho $k$ là một vành, $C$ là một $k$-đại số, $(C_n)_{n \in \mathbf{Z}}$ là một lọc giảm của $C$, tương thích với cấu trúc $k$-đại số và sao cho $C_0 = C$ (III, § 2, No. 1). Giả sử rằng $C$ tách được và đầy đủ đối với tôpô được xác định bởi lọc này, sao cho ánh xạ chính tắc $C \to \varprojlim C/C_n$ là một đồng phôi (*loc. cit.*, No. 6). Cho $m$ là một số nguyên $> 0$; ký hiệu $\pi : C \to C/C_m$ là toàn cấu chính tắc.

#### Mệnh đề 5 {#ac-x-s7-prop-5 .statement}

Cho $A$ là một đại số trên k được làm trơn hình thức với tôpô tuyến tính. Mọi đồng cấu liên tục của các đại số trên k $\varphi : \Lambda \to C/C_m$ đều có một phép nâng liên tục lên $C$.

Với mỗi số nguyên $n > m$, ta ký hiệu bởi $\pi_n : C/C_n \to C/C_{n-1}$ toàn cấu chính tắc. Vì $C$ được đồng nhất với giới hạn xạ ảnh của các $C/C_n$, việc cho một phép nâng liên tục của $\varphi$ lên $C$ tương đương với việc cho một họ $(\varphi_n)_{n > m}$ các đồng cấu liên tục của các đại số trên k $\varphi_n : A \to C/C_n$, thỏa mãn $\pi_n \circ \varphi_n = \varphi_{n-1}$. Điều này quy về, bằng quy nạp theo $m$, việc chứng minh mệnh đề khi $C_{m+1} = 0$. Khi đó iđêan $C_m$ có bình phương bằng không (vì $2m \geq m+1$), do đó suy ra mệnh đề vì $A$ được làm trơn hình thức.

#### Ví dụ {#ac-x-s7-n4-exa-1 .statement}

Cho $C$ là một đại số trên k và $N$ là một iđêan hai phía lũy linh của $C$. Mệnh đề áp dụng cho đại số $C$ được trang bị với lọc $N$-adic. Nếu $A$ là một đại số trên k được làm trơn hình thức với tôpô tuyến tính, ta thu được rằng mọi đồng cấu liên tục từ $A$ vào đại số trên k $C/N$, được trang bị với tôpô rời rạc, đều nâng lên thành một đồng cấu liên tục từ $A$ vào đại số trên k $C$, được trang bị với tôpô rời rạc.

### 5. Các thương làm trơn hình thức của các đại số

#### Định lý 2 {#ac-x-s7-thm-2 .statement}

Cho k là một vành, A là một đại số trên K, và J là một iđêan của A sao cho đại số trên k $A/J$ được làm trơn hình thức. Trang bị cho A tôpô J-adic. Các điều kiện sau là tương đương:

(i) đại số trên k tôpô A được làm trơn hình thức;
(ii) môđun $\Lambda/J$- $J/J^2$ là xạ ảnh và đồng cấu chính tắc ($\S$ 5, n° 2)
$$
\beta : S_{A/J}(J/J^2) \to \mathrm{gr}_J(A)
$$
là song ánh;
(iii) môđun $A/J$- $J/J^2$ là xạ ảnh và tồn tại một đẳng cấu của các đại số trên k tôpô từ phép hoàn thiện tách được của A lên đại số hoàn thiện của đại số phân bậc $S_{A/J}(J/J^2)$.

Nếu A là Noether, các điều kiện này cũng tương đương với:

(iv) iđêan J là hoàn toàn secant.

Trước hết ta nhận xét rằng (iii) suy ra (i): thật vậy, dưới các giả thiết của (iii), đại số $S_{A/J}(J/J^2)$, được trang bị với tôpô liên kết với phép phân bậc của nó, là làm trơn hình thức trên $A/J$ (No. 3, ví dụ 1), do đó trên k (No. 2, mệnh đề 3, a)); mệnh đề (i) khi đó suy ra từ mệnh đề 3, c) của No. 2.

Gọi $\hat{A}$ là phép hoàn thành tách được của đại số A và $\hat{J}$ là phép hoàn thành tách được của J. Đồng cấu chính tắc $i : A \to \hat{A}$ cảm sinh một đẳng cấu $A/J \to \hat{A}/\hat{J}$ (III, § 2, No. 12, công thức (21)). Gọi $\varphi : A/J \to \hat{A}$ là một phép nâng của đẳng cấu này (No. 4, Mệnh đề 5). Gọi $\lambda : \hat{J} \to J/J^2$ là toàn cấu suy ra từ đẳng cấu chính tắc $J/J^2 \to \hat{J}/\hat{J}^2$ (III, § 2, No. 12, công thức (21)). Cho $a$ là một phần tử của A, $\bar{a}$ là lớp của nó trong $A/J$, và $z$ là một phần tử của $\hat{J}$; ta có $\varphi(\bar{a}) \equiv i(a) \pmod{\hat{J}}$, do đó $\varphi(\bar{a})z \equiv i(a)z \pmod{\hat{J}^2}$ và $\lambda(\varphi(\bar{a})z) = \lambda(i(a)z) = \bar{a}\lambda(z)$. Nói cách khác, $\lambda$ là A/J-tuyến tính khi $\hat{J}$ được trang bị cấu trúc của một A/J-môđun suy ra từ $\varphi$.

Giả sử rằng đồng cấu $\lambda$ thừa nhận một tiết diện A/J-tuyến tính $\sigma : J/J^2 \to \hat{J}$. Gọi S là đại số phân bậc trên k $S_{A/J}(J/J^2)$ và $\hat{S}$ là phép hoàn thành của nó. Gọi
$$
\theta : S \to \hat{A}
$$
là đồng cấu của các đại số trên k sao cho $\theta(x) = \varphi(x)$ đối với $x$ trong $S^0 = A/J$, và $\theta(x) = \sigma(x)$ đối với $x$ trong $S^1 = J/J^2$. Vì $\theta$ biến $S^1$ vào $\hat{J}$, nó biến $S^n$ vào $\hat{J}^n$ và do đó mở rộng thành một đồng cấu liên tục $\hat{\theta} : \hat{S} \to \hat{A}$. Ánh xạ $\mathrm{gr}_1(\theta) : J/J^2 \to \hat{J}/\hat{J}^2$ là hợp thành của $\sigma$ với toàn cấu chính tắc $\hat{J} \to \hat{J}/\hat{J}^2$; vì $\sigma$ là một tiết diện của $\lambda$, $\mathrm{gr}_1(\theta)$ trùng với đẳng cấu chính tắc của $J/J^2$ lên $\hat{J}/\hat{J}^2$. Suy ra rằng $\mathrm{gr}(\theta) : S \to \mathrm{gr}_{\hat{J}}(\hat{A})$ là hợp thành của toàn cấu chính tắc $\beta$ với đẳng cấu chính tắc $\mathrm{gr}_J(A) \to \mathrm{gr}_{\hat{J}}(\hat{A})$ (III, § 2, No. 12, công thức (22)).

Bây giờ ta chứng minh kéo theo (ii) $\Rightarrow$ (iii). Theo giả thiết (ii), A/J-môđun $J/J^2$ là xạ ảnh, và do đó $\lambda$ thừa nhận một tiết diện A/J-tuyến tính; đồng cấu $\hat{\theta} : \hat{S} \to \hat{A}$ liên kết với tiết diện này bởi phép dựng trước đó cảm sinh bởi

Ta chứng minh (i) ⇒ (ii). Giả sử rằng đại số tôpô trên k A là trơn hình thức. Trước hết ta chứng minh rằng A/J-môđun $J/J^2$ là xạ ảnh. Cho M là một Λ/J-môđun và $f : M \to J/J^2$ là một ánh xạ A/J-tuyến tính toàn ánh; vấn đề là chứng minh rằng f thừa nhận một tiết diện Λ/J-tuyến tính.

Gọi π là toàn cấu chính tắc $A/J^2 \to A/J$. Theo Nhận xét 1 của No. 2, tồn tại một đẳng cấu của các đại số trên k ψ : A/J ⊕ J/J^2 → A/J^2 sao cho π(ψ(y, z)) = y và ψ(0, z) = z đối với $y \in A/J$, $z \in J/J^2$. Xét đại số trên k (A/J) ⊕ M (No. 1, Ví dụ) và ánh xạ u : (A/J) ⊕ M → A/J^2 sao cho u(x, m) = ψ(x, f(m)). Đây là một đồng cấu toàn ánh của các đại số trên k, có hạt nhân là môđun con Ker f của M, và do đó bình phương bằng không. Toàn cấu chính tắc ρ : A → A/J^2 là liên tục; vì đại số tôpô trên k A là trơn hình thức, tồn tại một đồng cấu của các đại số trên k ŝ : A → (A/J)⊕M sao cho u◦ŝ = ρ. Vì pr_1 = π◦ψ = π◦u, ta có pr_1◦ŝ = π◦u◦ŝ = π◦ρ, do đó pr_1◦ŝ là toàn cấu chính tắc của A lên A/J. Vì thế ta có ŝ(J) ⊂ M và do đó ŝ(J^2) = 0, nên ŝ cảm sinh một ánh xạ A/J-tuyến tính s : J/J^2 → M. Ta có u◦ŝ = ρ và pr_2◦ψ^{-1}◦u(y, m) = f(m) đối với $y \in A/J$ và $m \in M$. Cho $x \in J$, và ū là lớp của nó trong J/J^2; ta có f(s(ū)) = f(pr_2(ŝ(x))) = pr_2(ψ^{-1}(ū)) = ū. Do đó s là một tiết diện của f.

Còn lại là chứng minh rằng đồng cấu β là đơn ánh. Vì A/J-môđun $J/J^2$ là xạ ảnh, λ thừa nhận một tiết diện A/J-tuyến tính; gọi θ : S → Ā là đồng cấu liên kết. Đồng cấu gr(θ) được đồng nhất với β. Cho m là một số nguyên; gọi Σ_m là thương đại số trên k phân bậc của S bởi iđêan $\sum_{i>m} S^i$ và $\theta_m : \Sigma_m \to A/J^{m+1}$ là đồng cấu suy ra từ θ. Hợp thành của θ_m với toàn cấu chính tắc A/J^{m+1} → A/J là phép chiếu chính tắc của Σ_m lên S^0 = A/J; do đó hạt nhân của θ_m là một iđêan hai phía lũy linh. Theo ví dụ của No. 4, tồn tại một phép nâng ψ_m : A → Σ_m của toàn cấu chính tắc A → A/J^{m+1}. Vì hợp thành của ψ_m với phép chiếu chính tắc của Σ_m lên A/J là toàn cấu chính tắc, ψ_m(J) gồm các phần tử có bậc > 0. Bằng cách chuyển qua các đại số phân bậc liên kết, suy ra từ ψ_m một ánh xạ K-tuyến tính phân bậc gr(ψ_m) : gr_J(A) → Σ_m sao cho gr_m(θ)◦gr_m(ψ_m) = Id_{J^m/J^{m+1}}. Suy ra gr_m(θ), và do đó cả β_m, là đơn ánh, điều này hoàn tất chứng minh của (ii).

Cuối cùng, khi A là Noether, các điều kiện (ii) và (iv) là tương đương (§ 5, No. 2, Định lý 1).

#### Hệ quả 1 {#ac-x-s7-thm-2-cor-1 .statement}

Cho k là một trường và A là một đại số địa phương Noether trên k sao cho mở rộng κ_A của k là tách được. Các điều kiện sau là tương đương:

(i) đại số trên k A là trơn hình thức đối với tôpô $m_A$-adic;
(ii) vành A là chính quy;
(iii) đại số trên k Λ là tuyệt đối chính quy (§ 6, No. 4, Định nghĩa 1) ;
(iv) đại số trên k Ā là đẳng cấu với κ_A[[T_1, ..., T_n]], với n = dim A.

#### Hệ quả 2 {#ac-x-s7-thm-2-cor-2 .statement}

Cho $k$ là một trường, $A$ là một $k$-đại số Noether và $J$ là một iđêan của $A$ được chứa trong căn của $A$. Giả sử rằng $k$-đại số $A$ là trơn hình thức đối với tôpô $J$-adic. Khi đó nó là chính quy tuyệt đối.

Thật vậy, cho $k'$ là một mở rộng hữu hạn của $k$ và $A'$ là $A$-đại số $A_{(k')}$; cần chứng minh rằng, với mọi iđêan cực đại $m'$ của $A'$, vành địa phương Noether $A'_{m'}$ là chính quy. Bây giờ ta có $JA' \subset m'$: thực vậy, ảnh ngược của $m'$ trong $A$ là một iđêan cực đại của $A$ (V, § 2, No. 1, mệnh đề 1), do đó chứa $J$. $k'$-đại số $A'$ là trơn hình thức đối với tôpô $JA'$-adic (No. 2, mệnh đề 4, b)), và $k'$-đại số $A'_{m'}$ là trơn hình thức đối với tôpô $JA'_{m'}$-adic (No. 2, mệnh đề 4, a)), do đó cũng đối với tôpô $m'A'_{m'}$-adic. Gọi $k_0$ là trường con nguyên tố của $k'$. Khi đó $A'_{m'}$ là trơn hình thức trên $k_0$ đối với tôpô $m'A'_{m'}$-adic (hệ quả của định lý 1 của No. 3); vì $\kappa(m')$ là tách được trên $k_0$, vành $A'_{m'}$ là chính quy (hệ quả 1).

#### Hệ quả 3 {#ac-x-s7-thm-2-cor-3 .statement}

Cho $k$ là một vành và $A$ là một $k$-đại số trơn hình thức.

a) $A$-môđun $\Omega_k(A)$ là xạ ảnh.

b) Giả sử rằng vành $A \otimes_k A$ là Noether. Gọi $\mu : A \otimes_k A \to A$ là đồng cấu sao cho $\mu(x \otimes y) = xy$; khi đó iđêan $\mathrm{Ker}(\mu)$ là hoàn toàn cắt.

Các $k$-đại số $A$ và $A \otimes_k A$ là trơn hình thức (No. 2, mệnh đề 4, c)), và $A$ đẳng cấu với thương của $A \otimes_k A$ bởi hạt nhân $I$ của $\mu$. Theo định nghĩa ta có $\Omega_k(A) = I/I^2$. Do đó a) và b) suy ra từ định lý 2.

### 6. Mở rộng trường cơ sở trong các đại số chính quy (đặc số khác không)

Cho $k$ là một vành và $\rho : A \to B$ là một đồng cấu của các đại số $k$. Từ $\rho$ suy ra một ánh xạ tuyến tính $A$ $\Omega(\rho) : \Omega_k(A) \to \Omega_k(B)$, và do đó một ánh xạ tuyến tính $B$ $\Omega_0(\rho) : B \otimes_A \Omega_k(A) \to \Omega_k(B)$ (A, III, p. 135). Cho $T = (T_i)_{i \in I}$ là một họ các bất định, và $t = (t_i)_{i \in I}$ là một họ các phần tử của $B$; với mọi đa thức $f = \sum_{\alpha \in \mathbf{N}^{(I)}} c_\alpha T^\alpha$ của $A[T]$, ký hiệu $d^\Lambda f(t)$ là phần tử $\sum_\alpha t^\alpha \otimes dc_\alpha$ của $B \otimes_A \Omega_k(A)$.

#### Bổ đề 1 {#ac-x-s7-lem-1 .statement}

Giả sử rằng đại số $A$-$B$ nhận một họ sinh $t = (t_i)_{i \in I}$, với các hệ thức định nghĩa $f_\lambda \in A[T]$ ($\lambda \in \Lambda$). Đồng cấu tuyến tính $B$
$$
\psi : (B \otimes_A \Omega_k(A)) \oplus B^{(I)} \longrightarrow \Omega_k(B)
$$
được xác định bởi $\psi(\alpha, (b_i)) = \Omega_0(\rho)(\alpha) + \sum_{i \in I} b_i dt_i$, là toàn ánh; hạt nhân của nó được sinh bởi các phần tử $r_\lambda = \left( d^\Lambda f_\lambda(t), \left( \frac{\partial f_\lambda}{\partial T_i}(t) \right)_{i \in I} \right)$ với $\lambda \in \Lambda$.

Xét dãy các môđun $B$ và các ánh xạ tuyến tính $B$

$$
B^{(\Lambda)} \xrightarrow{\varphi} (B \otimes_{\Lambda} \Omega_k(A)) \oplus B^{(1)} \xrightarrow{\psi} \Omega_k(B) \longrightarrow 0,
$$

trong đó $\varphi$ là đồng cấu sao cho $\varphi(e_\lambda) = n_\lambda$; cần chứng minh rằng dãy này là khớp. Theo A, II, p. 36, th. 1, chỉ cần chứng minh rằng, với mọi môđun $B$ $M$, dãy

$$
0 \to \mathrm{Hom}_B(\Omega_k(B), M) \xrightarrow{\mathrm{Hom}(\psi, 1)} \mathrm{Hom}_B((B \otimes_A \Omega_k(A)) \oplus B^{(1)}, M) \xrightarrow{\mathrm{Hom}(\varphi, 1)} \mathrm{Hom}_B(B^{(\Lambda)}, M)
$$

là khớp. Theo tính chất phổ quát của môđun vi phân (A, III, p. 134), dãy này được đồng nhất với

$$
0 \to D_k(B, M) \xrightarrow{\psi'} D_k(A, M) \oplus M^1 \xrightarrow{\varphi'} M^\Lambda
$$

trong đó $\psi'(D) = (D \circ \rho, (D(t_i)))$ và $\varphi'(\Delta, (m_i)) = (f^\Delta_\lambda(t) + \sum_i \frac{\partial f_\lambda}{\partial T_i}(t) m_i)_{\lambda \in \Lambda}$ (phù hợp với A, V, p. 121, với mọi đa thức $f = \sum_{\alpha \in \mathbf{N}^{(1)}} c_\alpha T^\alpha$ của $A[T]$, $f^\Delta(t)$ ký hiệu phần tử $\sum_\alpha t^\alpha \Delta(c_\alpha)$). Nhưng tính khớp của dãy này suy ra từ loc. cit., prop. 1, xét đến sự kiện rằng một đạo hàm $D : B \to M$ là $k$-tuyến tính khi và chỉ khi điều này đúng với $D \circ \rho$.

Cho A là một vành. Tồn tại duy nhất một cấu trúc đại số $\mathbf{Z}$ trên A; người ta viết đơn giản $\Omega(\Lambda)$ cho môđun $A$ $\Omega_{\mathbf{Z}}(A)$. Nếu $\rho : k \to A$ là một đồng cấu của các vành, tồn tại một dãy khớp chính tắc của các môđun $A$ (A, III, p. 136, prop. 21)

$$
A \otimes_k \Omega(k) \to \Omega(A) \to \Omega_k(A) \to 0.
$$

Giả sử rằng A chứa một trường con, và cho P là trường con nguyên tố của A; khi đó $\Omega(P)$ bằng không và đồng cấu chính tắc của các môđun $A$ $\Omega(A) \to \Omega_P(A)$ là song ánh. Hơn nữa nếu A có đặc số $p \neq 0$ (điều này có nghĩa theo định nghĩa rằng $p$ là một số nguyên tố, rằng $p1_A = 0$ và $1_A \neq 0$), thì P được đồng nhất với $\mathbf{F}_p$. Ngoài ra, mọi đạo hàm của A triệt tiêu trên vành con $A^p$; với mọi vành con $k$ của A được chứa trong $A^p$ (và, đặc biệt, với mọi trường con hoàn hảo $k$ của A), ánh xạ chính tắc $\Omega(A) \to \Omega_k(A)$ là song ánh.

Cho A là một vành có đặc số $p \neq 0$ và $(f_i)_{1 \leq i \leq n}$ là một dãy hữu hạn các phần tử của A. Gọi $A_n$ là vành thương của vành đa thức $A[T_1, \ldots, T_n]$ theo iđêan sinh bởi các đa thức $T_i^p - f_i$, với $1 \leq i \leq n$.

#### Bổ đề 2 {#ac-x-s7-lem-2 .statement}

Giả sử vành A là địa phương và Noether. Khi đó $A_n$ là địa phương và Noether. Các điều kiện sau là tương đương:

(i) $A_n$ là chính quy;
(ii) A là chính quy và các phần tử $1 \otimes df_i$ của không gian vectơ $\kappa_A$- $ \kappa_A \otimes_A \Omega(A)$ là độc lập tuyến tính.

A) Trước hết ta xét trường hợp $n = 1$, đặt $T_1 = T$, $f_1 = f$. Gọi $a$ là lớp của $f$ trong $\kappa_A$, và phân biệt hai trường hợp tùy theo $a$ có thuộc hoặc không thuộc $\kappa_A^p$. Nếu $a \notin \kappa_A^p$, thì đa thức $T^p - a$ là bất khả quy trong $\kappa_A$ (A, V, p. 24, bổ đề 1), và $\kappa_A \otimes_A A_1$ đẳng cấu với trường $\kappa_A[T]/(T^p - a)$. Do đó iđêan $m_A A_1$ của $A_1$ là cực đại, vì vậy vành $A_1$ là địa phương (V, § 2, No. 1, mệnh đề 1). Nếu A là chính quy, thì $A_1$ là chính quy (VIII, § 5, No. 1, mệnh đề 1). Theo A, V, p. 99, mệnh đề 6, phần tử $da$ của $\Omega(\kappa_A)$ là khác không; vì nó là ảnh qua ánh xạ chính tắc $\kappa_A \otimes_A \Omega(A) \to \Omega(\kappa_A)$ của $1 \otimes df$, nên phần tử sau cũng khác không. Điều này chứng minh bổ đề trong trường hợp này.

Bây giờ giả sử $a$ thuộc $\kappa_A^p$. Do đó tồn tại một phần tử $g$ của A sao cho $f - g^p \in m_A$. Đặt $h = f - g^p$. Vì $T^p - f = (T - g)^p - h$, nên đại số $A$- $A_1$ đẳng cấu với $A[T]/(T^p - h)$. Theo VIII, § 5, No. 4, mệnh đề 4, vành $A_1$ là địa phương và, để nó là chính quy, điều kiện cần và đủ là A chính quy và $h$ không thuộc $m_A^2$. Bây giờ, vì $\kappa_A$ trơn hình thức trên trường nguyên tố (No. 3, định lý 1), ánh xạ chính tắc

$$
\bar{d} : m_A / m_A^2 \to \kappa_A \otimes_A \Omega(A)
$$

là đơn ánh (No. 2, nhận xét 1); nhưng ảnh qua $\bar{d}$ của lớp của $h$ modulo $m_A^2$ bằng $1 \otimes dh = 1 \otimes d(f - g^p) = 1 \otimes df$. Điều này chứng minh bổ đề trong trường hợp thứ hai này và hoàn tất chứng minh trường hợp $n = 1$.

B) Giả sử $n > 1$. Vành $A_1$ là địa phương và Noether theo trường hợp đã xét. Đại số $A_1$-đại số $A_n$ được đồng nhất với thương của $A_1[T_2, \ldots, T_n]$ theo iđêan sinh bởi các $T_i^p - f_i$, $i \geq 2$; theo giả thiết quy nạp, nó là một vành địa phương và điều kiện (i) tương đương với phép hội của hai điều kiện sau:

(i') $A_1$ là chính quy;
(ii') các phần tử $1 \otimes df_2, \ldots, 1 \otimes df_n$ của không gian vectơ $\kappa_{A_1}$-không gian $\kappa_{A_1} \otimes_{A_1} \Omega(A_1)$ là độc lập tuyến tính.

Nhưng (i') tương đương, như ta vừa thấy, với
(ii'') $A$ là chính quy và phần tử $1 \otimes df_1$ của không gian vectơ $\kappa_A$-không gian $\kappa_A \otimes_A \Omega(A)$ là không.

Theo bổ đề 1, đồng cấu chính tắc $A_1 \otimes_A \Omega(A) \to \Omega(A_1)$ cảm sinh một đẳng cấu từ $((A_1 \otimes_A \Omega(A))/A_1(1 \otimes df_1)) \oplus A_1$ lên $\Omega(A_1)$, và do đó một đồng cấu đơn cấu từ $(\kappa_{A_1} \otimes_A \Omega(A))/\kappa_{A_1}(1 \otimes df_1)$ vào $\kappa_{A_1} \otimes_{A_1} \Omega(A_1)$. Vì $\kappa_{A_1} \otimes_A \Omega(A)$ được đồng nhất với $\kappa_{A_1} \otimes_{\kappa_A} (\kappa_A \otimes_A \Omega(A))$, mệnh đề (ii'') do đó tương đương với:
(ii''') các phần tử $1 \otimes df_2, \ldots, 1 \otimes df_n$ là độc lập tuyến tính trong $(\kappa_A \otimes_A \Omega(A))/\kappa_A(1 \otimes df_1)$.

Nhưng phép hội của (ii') và (ii'') tương đương với (ii), điều này chứng minh bổ đề.

#### Mệnh đề 6 {#ac-x-s7-prop-6 .statement}

Cho $k$ là một trường có đặc số $p \neq 0$, $k'$ là một mở rộng thuần túy không tách được của $k$, có bậc hữu hạn và có chiều cao $\leqslant 1$, và $A$ là một $k$-đại số địa phương chính quy. Khi đó $A_{(k')}$ là một vành địa phương và các điều kiện sau là tương đương:

(i) vành $A_{(k')}$ là chính quy;
(ii) ánh xạ tuyến tính $\kappa_A$-tuyến tính

$$
\kappa_A \otimes_{{k'}^p} \Omega_{{k'}^p}({k'}^p) \longrightarrow \kappa_A \otimes_A \Omega(A)
$$

suy ra từ đơn ánh chính tắc ${k'}^p \to A$ là đơn ánh.

Thật vậy, hãy cho $(x_i)_{i \in I}$ là một cơ sở $p$ hữu hạn của $k'$ trên $k$ (A, V, p. 98); với mỗi $i \in I$, đặt $f_i = x_i^p \in k$. $k$-đại số $k'$ được đồng nhất với thương của $k[(T_i)_{i \in I}]$ theo iđêan sinh bởi các đa thức $T_i^p - f_i$, do đó $A$-đại số $A_{(k')}$ với thương của $A[(T_i)_{i \in I}]$ theo iđêan sinh bởi các đa thức $T_i^p - f_i 1_A$.

Hơn nữa, $(f_i)_{i \in I}$ là một cơ sở $p$ của ${k'}^p$ trên $k^p$, và không gian vectơ ${k'}^p$-không gian $\Omega_{k^p}({k'}^p)$ có họ các $df_i$ làm cơ sở (A, V, p. 97, đl. 1). Mệnh đề 6 khi đó suy ra từ bổ đề 2.

### 7. Một tiêu chuẩn cho các đại số địa phương trơn hình thức

#### Mệnh đề 7 {#ac-x-s7-prop-7 .statement}

Cho $k_0$ là một vành, $k$ là một $k_0$-đại số, $A$ là một $k$-đại số, $m$ là một iđêan cực đại của $A$. Giả sử rằng $k$ và $A/m$ là trơn hình thức trên $k_0$. Để $A$ là trơn hình thức trên $k$ đối với tôpô $m$-adic, điều kiện cần và đủ là hai điều kiện sau được thỏa mãn:

(i) đồng cấu chính tắc $S_{A/m}(m/m^2) \to \mathrm{gr}_m(A)$ là song ánh;
(ii) ánh xạ tuyến tính $A/m$-tuyến tính

$$
\omega : A/m \otimes_k \Omega_{k_0}(k) \longrightarrow A/m \otimes_A \Omega_{k_0}(A)
$$

suy ra từ ánh xạ chính tắc $k \to A$ là đơn ánh.

Ta ký hiệu bởi $d_k : k \to \Omega_{k_0}(k)$ và $d_A : A \to \Omega_{k_0}(A)$ các đạo hàm $k_0$-phổ quát.

Trước hết, giả sử rằng $A$ là trơn hình thức trên $k$ đối với tôpô $m$-adic. Khi đó $A$ là trơn hình thức trên $k_0$ đối với tôpô $m$-adic (No. 2, Mệnh đề 3, a)), điều này tương đương với (i) (No. 5, Định lý 2). Hơn nữa, đạo hàm $k_0$-$\lambda \mapsto 1 \otimes d_k(\lambda)$ của $k$ vào $A/m \otimes_k \Omega_{k_0}(k)$ có thể được mở rộng thành một đạo hàm $k_0$ của $A$ vào $A/m \otimes_k \Omega_{k_0}(k)$ (No. 2, Nhận xét 2). Do đó tồn tại một ánh xạ tuyến tính $A$ $u : \Omega_{k_0}(A) \to A/m \otimes_k \Omega_{k_0}(k)$ sao cho $u(d_A(\lambda 1_A)) = 1 \otimes d_k(\lambda)$ với mọi $\lambda \in k$. Ánh xạ tuyến tính $A/m$-tuyến tính $A/m \otimes_A \Omega_{k_0}(A) \longrightarrow A/m \otimes_k \Omega_{k_0}(k)$ suy ra từ $u$ là một phép rút gọn của $\omega$, điều này chứng minh (ii).

Ngược lại, giả sử rằng các điều kiện (i) và (ii) được thỏa mãn. Khi đó $A$ là trơn hình thức trên $k_0$ đối với tôpô $m$-adic (No. 5, Định lý 2) và $A$-môđun $\Omega_{k_0}(A)$ là xạ ảnh (No. 5, Hệ quả 3 của Định lý 2). Ta cố định một số nguyên $r \geqslant 0$ và xét ánh xạ tuyến tính $A/m^r$-tuyến tính

$$
\omega_r : A/m^r \otimes_k \Omega_{k_0}(k) \longrightarrow A/m^r \otimes_A \Omega_{k_0}(A)
$$

suy ra từ ánh xạ chính tắc $k \to A$. Cho $(\lambda_i)_{i \in I}$ là một họ các phần tử của $k$ sao cho các $d_k(\lambda_i)$ tạo thành một cơ sở của không gian vectơ $\Omega_{k_0}(k)$ trên $k$; theo (ii), các phần tử $1 \otimes d_A(\lambda_i 1_A)$ là độc lập tuyến tính trong $A/\mathfrak{m} \otimes_{\Lambda} \Omega_{k_0}(A)$. Theo II, § 3, No. 2, Hệ quả 1 và 2 của Mệnh đề 5, các $1 \otimes d_A(\lambda_i 1_A)$ tạo thành một cơ sở của một nhân tử trực tiếp của môđun $A/\mathfrak{m}^r$ $A/\mathfrak{m}^r \otimes_{\Lambda} \Omega_{k_0}(A)$. Do đó tồn tại một ánh xạ tuyến tính theo $A/\mathfrak{m}^r$
$$
u_r : A/\mathfrak{m}^r \otimes_{\Lambda} \Omega_{k_0}(A) \longrightarrow A/\mathfrak{m}^r \otimes_k \Omega_{k_0}(k)
$$
sao cho $u_r(1 \otimes d_A(\lambda_i 1_A)) = 1 \otimes d_k(\lambda_i)$ với mọi $i$, do đó $u_r \circ \omega_r = \mathrm{Id}$.

Bây giờ ta kiểm tra rằng $A$ trơn hình thức trên $k$ đối với tôpô $\mathfrak{m}$-adic. Cho $C$ là một đại số $k$, $N$ là một iđêan bình phương bằng không của $C$, và $\pi : C \to C/N$ là toàn cấu chính tắc; trang bị cho $C$ và $C/N$ tôpô rời rạc. Cho $\varphi : A \to C/N$ là một đồng cấu liên tục của các đại số $k$. Vì $A$ trơn hình thức trên $k_0$ đối với tôpô $\mathfrak{m}$-adic, tồn tại một đồng cấu liên tục của các đại số $k_0$ $\tilde{\varphi}_0 : A \to C$ sao cho $\pi \circ \tilde{\varphi}_0 = \varphi$. Theo Mệnh đề 1 của No. 1, các đồng cấu của các đại số $k_0$ $\tilde{\varphi} : A \to C$ sao cho $\pi \circ \tilde{\varphi} = \varphi$ là các ánh xạ $x \mapsto v(d_A(x)) + \tilde{\varphi}_0(x)$, trong đó $v$ chạy qua $\mathrm{Hom}_{\Lambda}(\Omega_{k_0}(A), N)$. Còn phải chọn $v$ sao cho $\tilde{\varphi}$ là một đồng cấu của các đại số $k$. Ánh xạ $\lambda \mapsto \lambda 1_C - \tilde{\varphi}_0(\lambda 1_A)$ là một đạo hàm $k_0$ của $k$ vào $N$ (*loc. cit.*), và do đó có thể viết được dưới dạng $h \circ d_k$ với $h \in \mathrm{Hom}_k(\Omega_{k_0}(k), N)$.

Chọn một số nguyên $r$ sao cho hạt nhân của $\varphi$ chứa $\mathfrak{m}^r$. A-môđun $N$ bị triệt tiêu bởi $\mathfrak{m}^r$, và chỉ cần lấy cho $v$ hợp của dãy các đồng cấu
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

*Cho $k$ là một trường và $A$ là một đại số Noether địa phương trên $k$. Các điều kiện sau là tương đương*:

(i) *$A$ trơn hình thức trên $k$ đối với tôpô $\mathfrak{m}_A$-adic* ;
(ii) *$A$ là chính quy và ánh xạ $\kappa_A$-tuyến tính*
$$
\omega : \kappa_A \otimes_k \Omega(k) \longrightarrow \kappa_A \otimes_{\Lambda} \Omega(A)
$$
*được suy ra từ đơn ánh chính tắc $k \to A$ là đơn ánh* ;
(iii) *$A$ là chính quy tuyệt đối* ;
(iv) *đối với mọi mở rộng thuần túy không phân ly $k'$ của $k$, có bậc hữu hạn và có chiều cao $\leqslant 1$, vành địa phương $A_{(k')}$ là chính quy*.

(ii) $\Leftrightarrow$ (i): chỉ cần áp dụng Mệnh đề 7 và Nhận xét 1 ở trên, lấy $k_0$ là trường con nguyên tố của $k$; thật vậy, $k$ và $\kappa_A$ trơn hình thức trên $k_0$ (No. 3, Định lý 1).
(i) $\Rightarrow$ (iii): điều này suy ra từ Hệ quả 2 của Định lý 2 (No. 5).

Nếu k có đặc số 0, suy ra từ Hệ quả 1 của Định lý 2 (No. 5) rằng (iv) kéo theo (i), do đó có mệnh đề trong trường hợp này. Giả sử k có đặc số $p \neq 0$ và chứng minh (iv) ⇒ (ii). Cho $k'$ là một mở rộng thuần túy không phân ly của k, có bậc hữu hạn và có chiều cao $\leq 1$. Nếu A và $A_{(k')}$ là chính quy, ánh xạ chính tắc $\kappa_A \otimes_{k'} \Omega_{k^p}({k'}^p) \longrightarrow \kappa_A \otimes_A \Omega(\Lambda)$ là đơn ánh (No. 6, Mệnh đề 6). Theo Định lý 1, b) của A, V, p. 97, áp dụng cho mở rộng k của $k^p$, không gian vectơ trên K $\Omega(k)$, trùng với $\Omega_{k^p}(k)$, là hợp lọc tăng của các không gian con $k \otimes_{{k'}^p} \Omega_{k^p}({k'}^p)$, trong đó $k'$ chạy qua tập hợp các mở rộng thuần túy không phân ly hữu hạn của k có chiều cao $\leq 1$ được chứa trong một bao đóng đại số cố định của k. Mệnh đề (ii) được suy ra.

#### Nhận xét 2 {#ac-x-s7-n7-rem-2 .statement}

Cho k là một trường và A là một đại số trên k sao cho vành $A_{(k')}$ là chính quy đối với mọi mở rộng thuần túy không phân ly $k'$ của k, có bậc hữu hạn và có chiều cao $\leq 1$; khi đó A là chính quy tuyệt đối. Thật vậy, cho $k'$ là một mở rộng như vậy; đối với mọi iđêan cực đại m của A, vành $k' \otimes_k A_m$ được đồng nhất với một vành phân thức của $A_{(k')}$, và do đó là chính quy. Theo Mệnh đề 8 ở trên và Mệnh đề 6 của § 6, No. 4, đại số A là chính quy tuyệt đối.

### 8. Sự tồn tại các phép rút đối với các ánh xạ tuyến tính

#### Mệnh đề 9 {#ac-x-s7-prop-9 .statement}

Cho A là một vành, M là một A-môđun sinh hữu hạn, N là một A-môđun xạ ảnh, và $u : M \to N$ là một ánh xạ A-tuyến tính.

a) Cho $\mathfrak{p}$ là một iđêan nguyên tố của A. Các điều kiện sau là tương đương :

(i) tồn tại $f \in A - \mathfrak{p}$ và $v \in \mathrm{Hom}_{A_f}(N_f, M_f)$ với $v \circ u_f = \mathrm{Id}_{M_f}$;
(ii) tồn tại $v \in \mathrm{Hom}_{A_\mathfrak{p}}(N_\mathfrak{p}, M_\mathfrak{p})$ với $v \circ u_\mathfrak{p} = \mathrm{Id}_{M_\mathfrak{p}}$;
(iii) ánh xạ $\kappa(\mathfrak{p})\text{-tuyến tính } 1 \otimes u : \kappa(\mathfrak{p}) \otimes_A M \to \kappa(\mathfrak{p}) \otimes_A N$ là đơn ánh;
(iv) tồn tại một số nguyên $m \geq 0$, các phần tử $x_1, \ldots, x_m$ của M và các dạng tuyến tính $y_1, \ldots, y_m$ trên N sao cho ảnh của các $x_i$ trong $M_\mathfrak{p}$ sinh A-môđun $M_\mathfrak{p}$ và ta có $\det(<y_j, u(x_i)>)\notin \mathfrak{p}$;

Nếu điều kiện (iv) được thỏa mãn, ta có $m = [\kappa(\mathfrak{p}) \otimes_A M : \kappa(\mathfrak{p})]$ và các phần tử $1 \otimes x_i$ tạo thành một cơ sở của không gian vectơ $\kappa(\mathfrak{p}) \otimes_A M$ trên $\kappa(\mathfrak{p})$.

b) Tập hợp U gồm các iđêan nguyên tố $\mathfrak{p}$ của A thỏa mãn các điều kiện của a) là một tập mở của Spec(A), và các điều kiện sau là tương đương:

(i) có $U = \mathrm{Spec}(A)$;
(ii) U chứa tất cả các iđêan cực đại của A;
(iii) tồn tại $v \in \mathrm{Hom}_A(N, M)$ với $v \circ u = \mathrm{Id}_M$;
(iv) u là đơn ánh và Coker(u) là một A-môđun xạ ảnh.

Ta chứng minh a).

(i) ⇒ (ii) ⇒ (iii): các kéo theo này là hiển nhiên.

(iii) ⇒ (iv): đặt $m = [\kappa(\mathfrak{p}) \otimes_A M : \kappa(\mathfrak{p})]$ và cho $(x_1, \ldots, x_m)$ là một dãy các phần tử của M sao cho các phần tử $1 \otimes x_i$ tạo thành một cơ sở của không gian vectơ $\kappa(\mathfrak{p}) \otimes_A M$ trên $\kappa(\mathfrak{p})$. Ảnh của các $x_i$ trong $M_\mathfrak{p}$ sinh A-môđun $M_\mathfrak{p}$ (bổ đề Nakayama). Nếu điều kiện (iii) được thỏa mãn, các phần tử $1 \otimes u(x_i)$ của không gian vectơ $\kappa(\mathfrak{p}) \otimes_A N$ trên $\kappa(\mathfrak{p})$ là độc lập tuyến tính.

Ngoài ra, tồn tại một A-môđun N', một tập hợp I, và một đẳng cấu của các A-môđun $\theta : N \oplus N' \to A^{(I)}$, từ đó suy ra một đẳng cấu của các không gian vectơ trên $\kappa(p)$
$$
\overline{\theta} : (\kappa(p) \otimes_{\Lambda} N) \oplus (\kappa(p) \otimes_A N') \to \kappa(p)^{(I)} .
$$
Các phần tử $t_i = \overline{\theta}(1 \otimes u(x_i), 0)$ của $\kappa(p)^{(I)}$ tạo thành một họ tự do hữu hạn. Do đó tồn tại các phần tử $\alpha_1, \ldots, \alpha_m$ của I sao cho có $\det(\mathrm{pr}_{\alpha_j}(t_i)) \neq 0$; các dạng tuyến tính $y_j : z \mapsto \mathrm{pr}_{\alpha_j}(\theta(z, 0))$ trên N là thích hợp.

Giả sử điều kiện (iv) được thỏa mãn. Gọi $(a_{ij}) \in M_m(A)$ là ma trận các hệ số $a_{ij} = <y_j, u(x_i)>$. Gọi g là một phần tử của $A - p$ sao cho các ảnh của các $x_i$ sinh $\Lambda_g$-môđun $M_g$ (II, § 5, No. 1, Prop. 2), và đặt $f = g \det(a_{ij})$. Vì $\det(a_{ij})$ khả nghịch trong $A_f$, các ảnh của các phần tử $u(x_i)$ trong $N_f$ là độc lập tuyến tính; do đó các ảnh của các $x_i$ trong $M_f$ lập thành một cơ sở của A-môđun $A_f$ này. Điều này chứng minh khẳng định cuối cùng của a). Bây giờ ta chứng minh (i). Gọi $w \in \mathrm{Hom}_A(N, M)$ là ánh xạ $z \mapsto \sum_j <y_j, z> x_j$. Ta có
$$
w \circ u(x_i) = \sum_j a_{ij} x_j ;
$$
vì các ảnh của các $x_i$ lập thành một cơ sở của $M_f$ và ma trận $(a_{ij})$ khả nghịch trong $M_m(A_f)$, tự đồng cấu $(w \circ u)_f$ của $M_f$ là song ánh, và ánh xạ $v = (w \circ u)_f^{-1} \circ w_f \in \mathrm{Hom}_{A_f}(N_f, M_f)$ thỏa mãn điều kiện (i).

Ta chứng minh b). Sự kiện U là mở suy ra từ điều kiện (i) của a).

(iii) $\Rightarrow$ (i) $\Rightarrow$ (ii): điều này là rõ ràng.

(iv) $\Rightarrow$ (iii): dưới các giả thiết của (iv), dãy $0 \to M \xrightarrow{u} N \longrightarrow \mathrm{Coker}(u) \to 0$ là khớp và tách, do đó (iii).

(ii) $\Rightarrow$ (iv): ta đưa vào, như trên, một đẳng cấu của các A-môđun $\theta : N \oplus N' \to A^{(I)}$. Gọi $u'$ là ánh xạ từ M vào $A^{(I)}$ được xác định bởi $u'(x) = \theta(u(x), 0)$. Tồn tại một tập con hữu hạn J của I sao cho ảnh của $u'$ được chứa trong môđun con $A^J$ của $A^{(I)}$. Gọi $u'' : M \to \Lambda^J$ là ánh xạ suy ra từ $u'$. Dưới giả thiết (ii), với mọi iđêan cực đại m của A, ánh xạ tuyến tính trên $A_m$ $u'_m$ từ $M_m$ vào $A_m^{(I)}$ có một ánh xạ rút, và do đó điều tương tự cũng đúng với $u''_m$; vì vậy $u''_m$ là đơn ánh và ảnh của nó là một nhân tử trực tiếp trong $A_m^J$, do đó đối hạt nhân của nó là một A-môđun $A_m$ xạ ảnh. A-môđun $\mathrm{Coker}(u'')$ là hữu hạn trình bày bởi phép dựng; do đó nó là xạ ảnh (II, § 5, No. 2, Th. 1). Đồng cấu $u''$ là đơn ánh (II, § 3, No. 3, Th. 1); do đó, $u$ là đơn ánh. A-môđun $\mathrm{Coker}(u')$ một mặt đẳng cấu với $\mathrm{Coker}(u) \oplus N'$, mặt khác đẳng cấu với $\mathrm{Coker}(u'') \oplus A^{(I-J)}$. Vì các A-môđun $A^{(I-J)}$, $\mathrm{Coker}(u'')$ và $N'$ là xạ ảnh, điều tương tự đúng với $\mathrm{Coker}(u)$, điều này hoàn tất việc chứng minh (iv).

### 9. Tiêu chuẩn Jacobian

Cho k là một vành, A là một đại số trên k, J là một iđêan của A và $\bar{d} : J/J^2 \to \Lambda/J \otimes_A \Omega_k(A)$ là ánh xạ chính tắc. Với mỗi đại số trên A/J R, ta ký hiệu bởi
$$
\bar{d}_R : R \otimes_{\Lambda/J} J/J^2 \longrightarrow R \otimes_A \Omega_k(A)
$$

ánh xạ R-tuyến tính cảm sinh bởi $\bar{d}$. Nếu $k$-đại số $A/J$ trơn hình thức, $\bar{d}$ có một phép co rút A-tuyến tính (No. 2, Nhận xét 1) và $\bar{d}_R$ có một phép co rút R-tuyến tính đối với mọi R.

Nói chung hơn:

#### Bổ đề 3 {#ac-x-s7-lem-3 .statement}

Cho K là một iđêan của A chứa J. Giả sử tồn tại một số nguyên m sao cho $J \cap K^m$ được chứa trong JK (điều kiện này được thỏa mãn nếu A là Noether). Nếu $A/J$ trơn hình thức trên k đối với tôpô K/J-adic, ánh xạ $\bar{d}_{A/K} : A/K \otimes_{A/J} J/J^2 \longrightarrow A/K \otimes_A \Omega_k(A)$ có một phép co rút A-tuyến tính.

Gọi C là $k$-đại số $A/(JK + K^m)$; iđêan N = $(J + K^m)/(JK + K^m)$ của C có bình phương bằng không và vành thương C/N đồng nhất với $A/(J + K^m)$. Trang bị cho C và C/N tôpô rời rạc, và cho A/J tôpô K/J-adic. Đồng cấu chính tắc $A/J \to A/(J + K^m)$ là liên tục; do đó nó có một phép nâng $\varphi : A/J \to A/(JK + K^m)$.

Ánh xạ $a \mapsto a1_C - \varphi(a1_{A/J})$ của A vào N khi đó là một k-đạo hàm (No. 1, Mệnh đề 1), do đó được viết $a \mapsto u(da)$ với $u \in \mathrm{Hom}_A(\Omega_k(A), N)$. Nhưng giả thiết $J \cap K^m \subset JK$ suy ra $J \cap (JK + K^m) = JK$, vì vậy ánh xạ chính tắc $\psi : J/JK \to N$ là song ánh; do đó tồn tại $v \in \mathrm{Hom}_{A/K}(A/K \otimes_A \Omega_k(A), J/JK)$ sao cho, với a trong A, ta có $a1_C = \varphi(a1_{A/J}) + \psi(v(1 \otimes da))$. Lấy a trong J, ta thấy rằng $v(1 \otimes da)$ bằng lớp của a trong J/JK. Vì $A/K \otimes_{A/J} J/J^2$ đồng nhất với J/JK, nên v là phép co rút cần tìm.

Sự kiện rằng điều kiện trên K được thỏa mãn khi đại số A là Noether suy ra từ III, § 3, No. 1, Hệ quả 2 của Mệnh đề 1.

#### Bổ đề 4 {#ac-x-s7-lem-4 .statement}

Giả sử rằng A trơn hình thức trên k đối với tôpô J-adic. Để $A/J$ là trơn hình thức trên k, điều kiện cần và đủ là ánh xạ chính tắc $\bar{d}$ có một phép co rút A-tuyến tính.

Đã biết rằng nếu $A/J$ trơn hình thức trên $k$, ánh xạ $\bar{d}$ nhận một phép co rút A-tuyến tính (No. 2, Nhận xét 1). Ngược lại, giả sử rằng $\bar{d}$ có một phép co rút A-tuyến tính. Gọi $\pi : A/J^2 \to A/J$ là toàn cấu chính tắc; theo Mệnh đề 2 của No. 1, tồn tại một đồng cấu vành $h : A/J \to A/J^2$ sao cho $\pi \circ h = \mathrm{Id}_{A/J}$. Gọi C là một $k$-đại số, N là một iđêan của C có bình phương bằng không, và $\rho : C \to C/N$ là toàn cấu chính tắc; trang bị cho C và C/N tôpô rời rạc. Gọi $u : A/J \to C/N$ là một đồng cấu liên tục của các $k$-đại số. Vì A trơn hình thức trên $k$ đối với tôpô J-adic, tồn tại một đồng cấu của các $k$-đại số $v : A \to C$ làm cho biểu đồ

$$
\begin{array}{ccc}
A & \xrightarrow{v} & C \\
\downarrow & & \downarrow \rho \\
A/J & \xrightarrow{u} & C/N
\end{array}
$$

giao hoán, trong đó các mũi tên đứng biểu diễn các toàn cấu chính tắc. Ta có $v(J) \subset \mathbf{N}$, do đó $v(J^2) \subset \mathbf{N}^2 = \{0\}$, và v xác định, bằng cách chuyển qua các vành thương, một đồng cấu $\bar{v} : A/J^2 \to C$ thỏa mãn $\rho \circ \bar{v} = u \circ \pi$. Khi đó $\bar{v} \circ h$ là một phép nâng của u lên C.

#### Định lý 3 {#ac-x-s7-thm-3 .statement}

Cho $k$ là một vành, A là một $k$-đại số trơn hình thức, và J là một iđêan sinh hữu hạn của A; đặt $B = A/J$.

a) Cho $\mathfrak{p}$ là một iđêan nguyên tố của $B$ và cho $q$ là iđêan (nguyên tố) của $A$ sao cho $\mathfrak{p} = q/J$. Các điều kiện sau là tương đương:
(i) $k$-đại số $B_{\mathfrak{p}}$ trơn hình thức;
(ii) tồn tại $f \in B - \mathfrak{p}$ sao cho $k$-đại số $B_f$ trơn hình thức;
(iii) ánh xạ tuyến tính $\kappa(\mathfrak{p})$
$$
\bar{d}_{\kappa(\mathfrak{p})} : \kappa(\mathfrak{p}) \otimes_B J/J^2 \to \kappa(\mathfrak{p}) \otimes_A \Omega_k(\Lambda)
$$
là đơn ánh;
(iv) tồn tại một số nguyên $m \geqslant 0$, các phần tử $f_1, \ldots, f_m$ của $J$, có các ảnh $(f_1)_q, \ldots, (f_m)_q$ sinh ra iđêan $J_q$, và các đạo hàm $k$-của $A$ $D_1, \ldots, D_m$ sao cho $\det(D_j(f_i)) \notin q$.

b) Tập hợp các iđêan nguyên tố $\mathfrak{p}$ của $B$ thỏa mãn các điều kiện tương đương của a) là mở trong $\mathrm{Spec}(B)$. Để $B$ trơn hình thức trên $k$, điều kiện cần và đủ là mọi iđêan nguyên tố (tương ứng cực đại) của $B$ thỏa mãn các điều kiện này.

c) Giả sử rằng $A$ là Noether. Các điều kiện của a) cũng tương đương với:
(v) $k$-đại số $B_{\mathfrak{p}}$ trơn hình thức đối với tôpô $\mathfrak{p}B_{\mathfrak{p}}$-adic.
Ngoài ra, dưới các điều kiện của (iv), iđêan $J_q$ là cắt hoàn toàn và dãy $((f_1)_q, \ldots, (f_m)_q)$ là cắt hoàn toàn đối với $A_q$.

Đặt $M = J/J^2$ và $N = B \otimes_A \Omega_k(A)$. $B$-môđun $M$ là hữu hạn kiểu, và $B$-môđun $N$ là xạ ảnh (No. 5, Hệ quả 3 của Định lý 2). Đối với mọi tập hợp nhân $S$ của $A$, $k$-đại số $S^{-1}A$ là trơn hình thức (No. 2, Mệnh đề 4, a)). Theo Bổ đề 4, các điều kiện (i) và (ii) do đó tương đương lần lượt với
(i') ánh xạ $\bar{d}_{B_{\mathfrak{p}}} : M_{\mathfrak{p}} \to N_{\mathfrak{p}}$ có một phép rút gọn tuyến tính $B_{\mathfrak{p}}$;
(ii') tồn tại $f \in B - \mathfrak{p}$ sao cho ánh xạ $\bar{d}_{B_f} : M_f \to N_f$ có một phép rút gọn tuyến tính $B_f$.

Mệnh đề 9 của No. 8 áp dụng cho vành $B$ và cho đồng cấu $\bar{d} : M \to N$ suy ra tính tương đương của các điều kiện (i'), (ii'') và (iii), và cũng kéo theo các khẳng định của b) (lại sử dụng Bổ đề 4). Hơn nữa, (iii) tương đương với:
(iii') ánh xạ $\kappa(q) \otimes_A J \to \kappa(q) \otimes_A \Omega_k(A)$ suy ra từ $d : J \to \Omega_k(A)$ là đơn ánh,
trong khi (iv) có thể viết:
(iv') tồn tại một số nguyên $m \geqslant 0$, các phần tử $f_1, \ldots, f_m$ của $J$ mà ảnh của chúng sinh iđêan $J_q$ của $A_q$, và các phần tử $y_1, \ldots, y_m$ của $\mathrm{Hom}_A(\Omega_k(A), A)$ sao cho $\det(<y_j, df_i>) \notin q$.

Vì $A$-môđun $\Omega_k(A)$ là xạ ảnh (No. 5, Hệ quả 3 của Định lý 2), Mệnh đề 9 của No. 8, áp dụng cho vành $A$ và cho đồng cấu $d : J \to \Omega_k(A)$, cho sự tương đương của (iii') và (iv').

Cuối cùng, giả sử vành $A$ Noether. Rõ ràng (i) suy ra (v). Dưới giả thiết (v), Bổ đề 3 chỉ ra rằng ánh xạ

$$
\bar{d}_{\kappa(q)} : \kappa(q) \otimes_{B_p} J_q / J_q^2 \longrightarrow \kappa(q) \otimes_{A_q} \Omega_k(A_q)
$$

là đơn ánh, do đó (iii).

Dưới các điều kiện của (iv), ta có $m = [\kappa(q) \otimes_A J : \kappa(q)]$ (No. 9, Mệnh đề 8). Theo Định lý 2 của No. 5, iđêan $J_q$ là hoàn toàn cát tuyến, và dãy $((f_1)_q, \ldots, (f_m)_q)$ là hoàn toàn cát tuyến đối với $A_q$ ($§ 1$, No. 3, Hệ quả 2 của Định lý 1). Điều này chứng minh c).

#### Hệ quả 1 {#ac-x-s7-thm-3-cor-1 .statement}

*Cho $k_0$ là một vành, $k$ là một $k_0$-đại số Noether chính quy hình thức, và $B$ là một $k$-đại số địa phương cốt yếu kiểu hữu hạn. Nếu $k_0$-đại số $B$ là chính quy hình thức đối với tôpô $\mathfrak{m}_B$-adic, thì nó là chính quy hình thức.*

Tồn tại một số nguyên $n \geqslant 0$, một tập con nhân $S$ của $k[T_1, \ldots, T_n]$, và một đồng cấu $k$ toàn ánh $S^{-1} k[T_1, \ldots, T_n] \to B$. Đại số $S^{-1} k[T_1, \ldots, T_n]$ là Noether và chính quy hình thức trên $k$ (No. 3, Ví dụ 2 và No. 2, Mệnh đề 4, a)), do đó trên $k_0$ (No. 2, Mệnh đề 3, a)). Hệ quả sau đó suy ra từ Định lý 3, c).

#### Hệ quả 2 {#ac-x-s7-thm-3-cor-2 .statement}

*Cho $k_0$ là một vành, $k$ là một $k_0$-đại số Noether chính quy hình thức, và $B$ là một $k$-đại số cốt yếu kiểu hữu hạn. Tập hợp $U$ các iđêan nguyên tố $\mathfrak{p}$ của $B$ sao cho $k_0$-đại số $B_{\mathfrak{p}}$ là chính quy hình thức (đối với tôpô rời rạc hoặc tôpô $\mathfrak{p}B_{\mathfrak{p}}$-adic) là mở trong $\operatorname{Spec}(B)$ và các điều kiện sau là tương đương:

(i) *ta có* $U = \operatorname{Spec}(B)$ ;
(ii) $U$ *chứa mọi iđêan cực đại của* $B$ ;
(iii) *$k_0$*-đại số* $B$ *là chính quy hình thức*.

Điều này suy ra như trên từ Định lý 3.

#### Nhận xét 1 {#ac-x-s7-n9-rem-1 .statement}

Hệ quả 1 và 2 áp dụng đặc biệt khi $k_0$ là một trường và ta ở trong một trong hai trường hợp sau:
a) $B$ là một đại số kiểu hữu hạn thiết yếu trên một mở rộng tách được của $k_0$ (đl. 1 của No. 3);
b) $B$ là một $k_0$-đại số địa phương Noether đầy đủ có trường thặng dư $\kappa_B$ là một mở rộng tách được của $k_0$ (trong trường hợp này lấy cho $k$ một đại số các chuỗi lũy thừa hình thức trên $\kappa_B$ mà $B$ là một thương của nó (No. 3 và IX, § 3, No. 3)).
Trong mỗi trường hợp này, từ hq. 2, xét đến mđ. 8 của No. 7 và mđ. 6, b) của § 6, No. 4, suy ra rằng $k_0$-đại số $B$ là trơn hình thức khi và chỉ khi nó là chính quy tuyệt đối.

**Hệ quả 3 (Zariski).** — *Cho $k$ là một trường, $A$ là một $k$-đại số địa phương chính quy, và $J$ là một iđêan của $A$ phân biệt với $A$. Giả sử rằng $k$-đại số $A$ là kiểu hữu hạn thiết yếu hoặc đầy đủ. Để vành địa phương $A/J$ là chính quy, điều kiện cần và đủ là tồn tại một số nguyên $m \geqslant 0$, các phần tử $f_1, \ldots, f_m$ của $J$ sinh ra $J$, và các đạo hàm $D_1, \ldots, D_m$ của $A$ sao cho $\det(D_j(f_i)) \notin \mathfrak{m}_A$. Khi đó các phần tử $(f_1, \ldots, f_m)$ tạo thành một phần của một hệ tọa độ của $A$ và iđêan $J$ là nguyên tố.*

Cho $k_0$ là trường con nguyên tố của $k$. $k_0$-đại số $A$ là chính quy tuyệt đối ($§ 6$, No. 4, ví dụ 1), do đó trơn hình thức (nhận xét 1 ở trên). Vì những lý do tương tự, nói rằng $A/J$ là chính quy tương đương với nói rằng nó là một $k_0$-đại số trơn hình thức. Mệnh đề thứ nhất do đó suy ra từ đl. 3, mệnh đề này cũng kéo theo rằng dãy $(f_1, \ldots, f_m)$ là hoàn toàn cắt ngang đối với $A$. Sau đó áp dụng mđ. 2 của VIII, $§ 5$, No. 3.

#### Nhận xét 2 {#ac-x-s7-n9-rem-2 .statement}

Dưới các giả thiết của hq. 3, $A$-môđun $\Omega(A)$ là xạ ảnh (No. 5, hq. 3 của đl. 2), do đó tự do; mọi đạo hàm của $A$ vào $\kappa_A$ vì thế nâng được thành một đạo hàm của $A$. Điều kiện của mệnh đề do đó có thể được biểu diễn như sau: tồn tại một hệ sinh $(f_1, \ldots, f_m)$ của $J$ và các đạo hàm $D_1, \ldots, D_m$ của $A$ vào $\kappa_A$, sao cho $\det(D_j(f_i)) \neq 0$.

#### Hệ quả 4 (Zariski) {#ac-x-s7-thm-3-cor-4 .statement}

*Cho $k$ là một trường và $A$ là một $k$-đại số kiểu hữu hạn thiết yếu hoặc một vành địa phương Noether đầy đủ. Tập hợp các iđêan nguyên tố $\mathfrak{p}$ của $A$ sao cho vành địa phương $A_{\mathfrak{p}}$ là chính quy là mở trong $\mathrm{Spec}(A)$*.

Chỉ cần áp dụng Nhận xét 1, lấy $k_0$ là trường con nguyên tố của $k$.

### 10. Các đại số trơn

#### Bổ đề 5 {#ac-x-s7-lem-5 .statement}

*Cho $\rho : A \to B$ là một đồng cấu địa phương của các vành địa phương Noether. Giả sử rằng $B$ là bản chất hữu hạn kiểu trên $A$. Để đại số $A$-đại số $B$ là trơn hình thức, điều kiện cần và đủ là $A$-môđun $B$ là phẳng và $\kappa_A$-đại số $\kappa_A \otimes_A B$ là chính quy tuyệt đối.*

Tồn tại một số nguyên $n \geqslant 0$, một iđêan nguyên tố $q$ của $A[T_1, \ldots, T_n]$, và một đồng cấu toàn ánh $h$ từ $A[T_1, \ldots, T_n]_q$ lên $B$. Ký hiệu $C$ là $A$-đại số địa phương $A[T_1, \ldots, T_n]_q$; nó là trơn hình thức (No. 3, Ví dụ 2 và No. 2, Mệnh đề 4, a)) và phẳng trên $A$, và ta có thể đồng nhất $B$ với $A$-đại số $C/J$, trong đó $J = \mathrm{Ker}(h)$.

Đặt $\overline{C} = \kappa_A \otimes_A C$ và $\overline{B} = \kappa_A \otimes_A B$. Giả sử rằng $B$ trơn hình thức trên $A$. Khi đó $\kappa_A$-đại số $\overline{B}$ là trơn hình thức (No. 2, Mệnh đề 4, b)), do đó chính quy tuyệt đối (No. 5, Hệ quả 2 của Định lý 2). Hơn nữa, vì $\overline{C}/J\overline{C}$ có thể được đồng nhất với $\overline{B}$ và $\kappa_A$-đại số $\overline{C}$ là trơn hình thức, iđêan $J\overline{C}$ của $\overline{C}$ là cắt hoàn toàn (No. 5, Định lý 2). Khi đó suy ra từ § 5, No. 6, Mệnh đề 6 rằng $A$-môđun $B$ là phẳng.

Ngược lại, giả sử rằng $B$ là phẳng trên $A$ và rằng $\kappa_A$-đại số $\overline{B}$ là chính quy tuyệt đối. Khi đó $\kappa_A$-đại số địa phương $\overline{B}$ là trơn hình thức (Nhận xét 1 của No. 9 với $k = k_0 = \kappa_A$). Đặt $\overline{J} = \kappa_A \otimes_A J$; vì $B$ là một $A$-môđun phẳng, ánh xạ chính tắc $\overline{J} \to J\overline{C}$ là song ánh và $\overline{B}$ có thể được đồng nhất với $\overline{C}/\overline{J}$. Suy ra (Nhận xét 1 của No. 2) rằng ánh xạ chính tắc

$$
\overline{J}/\overline{J}^2 \longrightarrow \overline{B} \otimes_{\overline{C}} \Omega_{\kappa_A}(\overline{C})
$$

là đơn ánh và thừa nhận một phép rút gọn. Khi đó $\overline{J}/\overline{J}^2$ được đồng nhất với $\kappa_A \otimes_A J/J^2$, do đó với $\overline{B} \otimes_B J/J^2$; mặt khác, $\overline{C}$-môđun $\Omega_{\kappa_A}(\overline{C})$ đẳng cấu chính tắc với $\overline{C} \otimes_C \Omega_A(C)$ (A, III, p. 136, mđ. 20), do đó $\overline{B} \otimes_{\overline{C}} \Omega_{\kappa_A}(\overline{C})$ đẳng cấu chính tắc với $\overline{B} \otimes_C \Omega_A(C)$. Chuyển qua thương theo iđêan cực đại của $\overline{B}$, ta thu được một đồng cấu đơn ánh

$$
\kappa_B \otimes_B J/J^2 \longrightarrow \kappa_B \otimes_C \Omega_A(C)
$$

không gì khác ngoài $d_{\kappa_B}$. Do đó B trơn hình thức trên A (đl. 3).

#### Định lý 4 {#ac-x-s7-thm-4 .statement}

Cho A là một vành Noether và B là một đại số trên A thiết yếu có kiểu hữu hạn. Các điều kiện sau là tương đương:

(i) đại số trên A B là trơn hình thức ;
(ii) với mọi $q \in \mathrm{Spec}(B)$, đại số trên A $B_q$ là trơn hình thức (tương ứng, trơn hình thức đối với tôpô $qB_q$-adic) ;
(iii) A-môđun B là phẳng và, với mọi $p \in \mathrm{Spec}(A)$, $\kappa(p)\text{-đại số} \ \kappa(p) \otimes_A B$ là chính quy tuyệt đối ;
(iv) A-môđun B là phẳng và, với mọi đại số trên A chính quy R, vành $R \otimes_A B$ là chính quy ;
(v) A-môđun B là phẳng và hạt nhân của đồng cấu $\mu : B \otimes_A B \to B$ sao cho $\mu(x \otimes y) = xy$ là một iđêan cắt hoàn toàn.

Sự tương đương của (i) và (ii) suy ra từ hệ quả 2 của định lý 3 (No. 9).

(i)⇒(v) : giả sử đại số trên A B trơn hình thức. Gọi q là một iđêan nguyên tố của B, và p là ảnh ngược của nó trong A. Đại số trên $A_p$ $B_q$ là trơn hình thức (mệnh đề 4, a) của No. 2), do đó phẳng (bổ đề 5) ; do đó A-môđun B là phẳng (II, § 3, No. 4, mđ. 15). Mặt khác, vành $B \otimes_A B$ là Noether (§ 6, No. 1, hệ quả của mđ. 2), do đó iđêan $\mathrm{Ker}\,\mu$ là cắt hoàn toàn theo hệ quả 3 của định lý 2 (No. 5).

(v)⇒(iii) : giả sử điều kiện (v) được thỏa mãn. Đặt $I = \mathrm{Ker}(\mu)$. Cho $p \in \mathrm{Spec}(A)$. Ánh xạ

$$
1 \otimes \mu : \kappa(p) \otimes_A (B \otimes_A B) \to \kappa(p) \otimes_A B
$$

được đồng nhất với ánh xạ

$$
\mu_p : (\kappa(p) \otimes_A B) \otimes_{\kappa(p)} (\kappa(p) \otimes_A B) \to \kappa(p) \otimes_A B
$$

suy ra từ phép nhân của $\kappa(p)\text{-đại số} \ \kappa(p) \otimes_A B$. Iđêan $\mathrm{Ker}(\mu_p)$ được đồng nhất với $I(\kappa(p) \otimes_A (B \otimes_A B))$. Nó là cắt hoàn toàn vì A-môđun B là phẳng (§ 5, No. 6, mđ. 6). Mệnh đề (iii) khi đó suy ra từ mđ. 8 của § 6, No. 5.

(iii)⇒(ii) : cho q là một iđêan nguyên tố của B, và p là ảnh ngược của nó trong A. Dưới các giả thiết của (iii), $A_p$-môđun $B_q$ là phẳng, và $\kappa(p)\text{-đại số} \ \kappa(p) \otimes_{A_p} B_q$, được đồng nhất với một vành các phân thức của $\kappa(p) \otimes_A B$, là chính quy tuyệt đối (§ 6, No. 4, mđ. 6). Suy ra từ bổ đề 5 rằng $B_q$ trơn hình thức trên $A_p$, do đó trên A (No. 2, mđ. 3 và 4).

(iii)⇒(iv) : ta đặt mình dưới các giả thiết của (iii). Cho R là một đại số trên A chính quy. R-môđun $R \otimes_A B$ là phẳng (I, § 2, No. 7, hệ quả 2 của mđ. 8). Gọi r là một iđêan nguyên tố của R và p là ảnh ngược của nó trong A ; vành $\kappa(r) \otimes_R (R \otimes_A B)$, được đồng nhất với $\kappa(r) \otimes_{\kappa(p)} (\kappa(p) \otimes_A B)$, là chính quy (§ 6, No. 4, hệ quả 2 của mđ. 7). Vành $R \otimes_A B$ do đó là chính quy (§ 4, No. 5, hệ quả của mđ. 9).

(iv) ⇒ (iii) : cho $p$ là một iđêan nguyên tố của $A$ và cho $k$ là một mở rộng của $\kappa(p)$; dưới các giả thiết của (iv), vành $k \otimes_{\kappa(p)} (\kappa(p) \otimes_A B)$, được đồng nhất với $k \otimes_A B$, là chính quy, do đó (iii).

#### Định nghĩa 2 {#ac-x-s7-def-2 .statement}

Cho $A$ là một vành Noether. Một đại số trên $A$ $B$ được gọi là trơn nếu nó thiết yếu có kiểu hữu hạn và nếu nó thỏa mãn các điều kiện tương đương của định lý 4.

#### Mệnh đề 10 {#ac-x-s7-prop-10 .statement}

Cho $A$ là một vành Noether.

a) Cho $A'$ là một đại số Noether trên A và $B$ là một đại số trơn trên A. Khi đó đại số trên $A'$ $A' \otimes_A B$ là trơn.

b) Cho $B$ là một $A$-đại số trơn và $C$ là một $B$-đại số trơn. Khi đó $C$ là một $A$-đại số trơn.

c) Cho $B$ và $C$ là hai $A$-đại số trơn. Khi đó $B \otimes_A C$ là một $A$-đại số trơn.

Điều này suy ra từ Mệnh đề 4 của No. 2 và từ các mệnh đề tương tự đối với các đại số thiết yếu là hữu hạn kiểu (§ 6, No. 1).

#### Ví dụ 1 {#ac-x-s7-n10-exa-1 .statement}

Các đại số trơn trên một trường $k$ là các $k$-đại số thiết yếu là hữu hạn kiểu và chính quy tuyệt đối.

#### Ví dụ 2 {#ac-x-s7-n10-exa-2 .statement}

Cho $A$ là một vành Noether, $T = (T_i)_{i \in I}$ là một họ hữu hạn các bất định. $A$-đại số $A[T]$ là trơn. Nói chung hơn, cho $F_1, \ldots, F_m$ là các phần tử của $A[T]$, và cho $B$ là $A$-đại số $A[T]/(F_1, \ldots, F_m)$. Nếu tại mọi iđêan cực đại $n$ của $B$ lớp (mod. $n$) của ma trận $\left( \frac{\partial F_j}{\partial T_i} \right)$ có hạng $m$, thì $A$-đại số $B$ là trơn (Định lý 3 của No. 9).

## BÀI TẬP {#ac-x-s7-exercises}

Xem các [bài tập cho § 7](exercises/s7/).
