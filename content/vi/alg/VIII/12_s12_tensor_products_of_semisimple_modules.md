---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 12
section_title: Tensor Products of Semisimple Modules
lang: vi
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.211-A VIII.228
pdf_pages: 0228-0245
extraction: native
subsections:
    - "no": 1
      title: Semisimple Modules over Tensor Products of Algebras
      page: 211
      pdf_page: 228
    - "no": 2
      title: Tensor Products of Simple Modules
      page: 213
      pdf_page: 230
    - "no": 3
      title: Tensor Products of Semisimple Commutative Algebras
      page: 215
      pdf_page: 232
    - "no": 4
      title: The Radical of a Tensor Product of Algebras
      page: 217
      pdf_page: 234
    - "no": 5
      title: Tensor Products of Semisimple Modules
      page: 218
      pdf_page: 235
    - "no": 6
      title: Tensor Products of Semisimple Algebras
      page: 221
      pdf_page: 238
    - "no": 7
      title: Extension of Scalars in Semisimple Modules
      page: 222
      pdf_page: 239
statements: 26
exercises: 17
content_sha256: c9069565ee8b1d1e34a816beec5ab78f90f2e454b6bf8a53c8e6f853bf30f6cb
translated_from: content/en/alg/VIII/12_s12_tensor_products_of_semisimple_modules.md
source_content_sha256: b311e3c926d1c35b21ba3909e0ec3e0584eb38f0337ee0f5d814716a0a8f67c8
translation_model: gpt-5.4, gpt-5-6
translation_run: translate-vi-74c08a00
glossary_version: 34
glossary_terms_sha256: 18b6f1f032f95ac5189aa8b750783d65afac1431c0b3d4370ab1843856692367
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 12. TÍCH TENXƠ CỦA CÁC MÔĐUN NỬA ĐƠN

Trong tiết diện này, chữ K chỉ một trường giao hoán. Nếu E và F là các không gian vectơ trên K, thì ta ký hiệu tích tenxơ $E\otimes_KF$ bởi $E\otimes F$.

### 1. Các Môđun Nửa Đơn trên Tích Tenxơ của các Đại số

Trong tiểu mục này, ta xét các K-đại số $A_1$ và $A_2$; ta ký hiệu đại số $A_1\otimes A_2$ bởi A.

#### Mệnh đề 1 {#alg-viii-s12-prop-1 .statement tag=00E6}

Cho $M_1$ là một $A_1$-môđun và $M_2$ là một $A_2$-môđun, cả hai đều không rút về 0. Nếu môđun $M = M_1\otimes M_2$ trên vành $A = A_1\otimes A_2$ là đơn (resp. đẳng kiểu, nửa đơn), thì $A_1$-môđun $M_1$ và $A_2$-môđun $M_2$ là đơn (resp. đẳng kiểu, nửa đơn).

Giả sử M là một A-môđun nửa đơn. Cho $N_1$ là một môđun con $A_1$ của $M_1$. Gọi N là ảnh chính tắc của $N_1\otimes M_2$ trong A-môđun M. Theo Hệ quả 2 của VIII, p. 56, tồn tại một phép chiếu A-tuyến tính $p$ trong M có ảnh là N. Theo giả thiết, ta có $M_2\not= 0$; do đó có thể chọn một phần tử $m$ của $M_2$ và một dạng tuyến tính $\varphi$ trên không gian vectơ trên K $M_2$ sao cho $\varphi (m) = 1$ (II, §7, No. 5, p. 302, Hệ quả 2). Gọi $u$ là ánh xạ từ $M_1$ vào M được xác định bởi $u(m_1) =m_1\otimes m$, và gọi $v$ là ánh xạ K-tuyến tính từ M vào $M_1$ được đặc trưng bởi $v(m_1\otimes m_2) =\varphi (m_2)m_1$. Đặt $q=v\circ p\circ u$. Ánh xạ $q: M_1\rightarrow M_1$ là $A_1$-tuyến tính, ảnh của nó được chứa trong $N_1$, và ta có $q(n) =n$ với mọi $n\in N_1$. Do đó, $q$ là một phép chiếu trong $M_1$ có ảnh là $N_1$. Ta đã chứng minh rằng $M_1$ là một $A_1$-môđun nửa đơn (VIII, p. 56, Hệ quả 2).

Giả sử rằng M là đơn và $M_1$ là tổng trực tiếp của hai $A_1$-môđun con $M'_1$ và $M''_1$. Đặt $M'= M'_1\otimes M_2$ và $M''= M''_1\otimes M_2$; khi đó M là tổng trực tiếp của các A-môđun con $M'$ và $M''$. Vì M là đơn, nên $M'$ hoặc $M''$ phải thu về 0; do theo giả thiết ta có $M_2\not= 0$, suy ra $M'_1= 0$ hoặc $M''_1= 0$ (II, §3, No. 7, p. 256, Hệ quả 2). Điều này chứng minh rằng $M_1$ là một $A_1$-môđun đơn.

Bây giờ giả sử rằng M là một A-môđun đẳng kiểu. Cho S và T là các $A_1$-môđun con đơn của $M_1$. Khi đó các A-môđun $S\otimes M_2$ và $T\otimes M_2$ có thể được đồng nhất với các môđun con khác không của M. Do đó chúng đẳng kiểu cùng một kiểu như M. Theo Nhận xét VIII, p. 61, tồn tại một ánh xạ A-tuyến tính khác không $f: S\otimes M_2\rightarrow T\otimes M_2$. Đặc biệt, ánh xạ $f$ là $A_1$-tuyến tính. Vì các $A_1$-môđun $S\otimes M_2$ và $T\otimes M_2$ đều khác không và đẳng kiểu lần lượt kiểu S và T, nên S và T đẳng cấu. Điều này chứng minh rằng $M_1$ là một $A_1$-môđun đẳng kiểu.

#### Mệnh đề 2 {#alg-viii-s12-prop-2 .statement tag=00E7}

Cho S là một môđun đơn trên vành $A = A_1\otimes A_2$, hữu hạn chiều trên K. Với $i\in  \{1,2\}$, tồn tại một $A_i$-môđun đơn $S_i$ sao cho $A_i$-môđun S là đẳng kiểu thuộc kiểu $S_i$. A-môđun S đẳng cấu với một thương của A-môđun $S_1\otimes S_2$.

Vì S là một $A_1$-môđun khác không hữu hạn chiều trên K, nên nó có độ dài hữu hạn trên $A_1$ và tồn tại một $A_1$-môđun đơn trái $S_1$ cùng một ánh xạ $A_1$-tuyến tính khác không từ $S_1$ vào S. Ta trang bị cho $M_2=$ Hom$_{A_1}(S_1,S)$ một cấu trúc $A_2$-môđun trái được xác định bởi phép toán ngoài $(a_2, u)\mapsto (a_2)_S\circ u$. Theo phép dựng, ta có $M_2\not= 0$, và $M_2$ hữu hạn chiều trên K. Do đó, ta có thể tìm một $A_2$-môđun đơn trái $S_2$ và một ánh xạ $A_2$-tuyến tính khác không $\varphi : S_2\rightarrow M_2$. Ta định nghĩa một ánh xạ A-tuyến tính khác không $\psi$ từ $S_1\otimes S_2$ vào S bởi

$$
\psi (s_1\otimes s_2) =\varphi (s_2)(s_1) \tag{1}
$$

với mọi $s_1\in S_1$ và $s_2\in S_2$. Vì S là một A-môđun đơn và $\psi$ khác không, nên $\psi$ là toàn ánh và S đẳng cấu với một thương của $S_1\otimes S_2$. Với $i\in  \{1,2\}$, $A_i$-môđun $S_1\otimes S_2$ là đẳng kiểu kiểu $S_i$, và do đó $A_i$-môđun S cũng vậy (VIII, p. 61, Mệnh đề 2).

Với mọi đại số trên K B, ta ký hiệu bởi $\mathscr{S}_K(B)$ tập hợp các lớp của các B-môđun trái đơn (VIII, p. 51) hữu hạn chiều trên K.

#### Định lý 1 {#alg-viii-s12-thm-1 .statement tag=00E8}

Giả sử rằng trường K đóng đại số.

a) Cho $M_1$ là một $A_1$-môđun và $M_2$ là một $A_2$-môđun, cả hai đều đơn (resp. nửa đơn) và hữu hạn chiều trên K. Khi đó $M_1\otimes M_2$ là một môđun đơn (resp. nửa đơn) trên vành $A_1\otimes A_2$ và hữu hạn chiều trên K.

b) Ánh xạ từ $\mathscr{S}_K(A_1)\times \mathscr{S}_K(A_2)$ vào $\mathscr{S}_K(A_1\otimes A_2)$ gửi (cl(S$_1$), cl(S$_2$)) tới cl(S$_1\otimes S_2$)), trong đó $S_1($resp. $S_2)$ là một $A_1$-môđun đơn (resp. $A_2$-môđun) hữu hạn chiều trên K, là song ánh.

Để chứng minh phần a), chỉ cần xét trường hợp $M_1$ và $M_2$ là đơn. Gọi $M'$ là một A-môđun con của $M = M_1\otimes M_2$; nó là một $A_1$-môđun con của $M_1\otimes M_2$, ổn định dưới tập hợp các nội cấu dạng $1_{M_1}\otimes u$, trong đó $u$ chạy qua tập hợp các phép vị tự của $A_2$-môđun $M_2$. Vì trường K đóng đại số, Bổ đề Schur (VIII, p. 47, Định lý 1) suy ra rằng hoán tập End$_{A_1}(M_1)$ của $M_1$ bằng K. Theo Hệ quả 2 của VIII, p. 63, A-môđun con $M'$ của $M_1\otimes M_2$ có dạng $M_1\otimes M'_2$, trong đó $M'_2$ là một $A_2$-môđun con của $M_2$. Ta đã giả thiết rằng $M_2$ là đơn; do đó $M'_2= 0$ hoặc $M'_2= M_2$, nghĩa là $M'= 0$ hoặc $M'= M$. Do đó, M là đơn.

Nếu S là một môđun đơn trên $A_1\otimes A_2$ hữu hạn chiều trên K, thì theo Mệnh đề 2 và phần a), suy ra S đẳng cấu với một môđun dạng $S_1\otimes S_2$, trong đó $S_1$ (resp. $S_2$) là một $A_1$-môđun đơn (resp. $A_2$-môđun đơn). Hơn nữa, như một $A_i$-môđun, S là đẳng kiểu kiểu $S_i$, nên lớp của $S_i$ chỉ phụ thuộc vào lớp của S. Điều này chứng minh phần b).

#### Nhận xét 1 {#alg-viii-s12-n1-rem-1 .statement tag=00E9}

Mệnh đề a) của Định lý 1 không còn đúng nữa khi không giả thiết trường K là đóng đại số. Ta có thể cho các ví dụ (VIII, p. 225, Bài tập 4) trong đó $M_i$ là một $A_i$-môđun đơn hữu hạn chiều trên K, với $i\in  \{1,2\}$, và trong đó A-môđun $M_1\otimes M_2$ không nửa đơn hoặc nửa đơn nhưng không đơn.

#### Nhận xét 2 {#alg-viii-s12-n1-rem-2 .statement tag=00EA}

Tồn tại một đồng cấu $\varphi$ từ $R_K(A_1)\otimes_{\mathbf{Z}}R_K(A_2)$ vào $R_K(A)$ được đặc trưng bởi quan hệ $\varphi ([M_1]\otimes [M_2]) = [M_1\otimes M_2]$. Điều này có thể được chứng minh theo cùng cách như Mệnh đề 9 của VIII, p. 196. Nếu trường K là đóng đại số, thì $\varphi$ là một đẳng cấu từ $R_K(A_1)\otimes_ZR_K(A_2)$ lên $R_K(A)$ theo Định lý 1, b) bởi vì với mọi K-đại số B, $\mathbf{Z}$-môđun $R_K(B)$ là tự do với cơ sở là họ $([S])_{S\in\mathscr{S}_K(B)}$ (VIII, p. 195).

### 2. Tích tenxơ của các môđun đơn

Cho $A_1$ và $A_2$ là các đại số trên trường giao hoán K. Ta ký hiệu K-đại số $A_1\otimes A_2$ bởi A.

#### Bổ đề 1 {#alg-viii-s12-lem-1 .statement tag=00RB}

Cho $M_1$ và $N_1$ là các $A_1$-môđun, và cho $M_2$ và $N_2$ là các $A_2$-môđun. Ta đưa ra các giả thiết sau:

(i) $A_1$-môđun $M_1$ sinh hữu hạn.

(ii) $A_2$-môđun $M_2$ sinh hữu hạn, hoặc $N_1$ hữu hạn chiều trên K.

Đặt $M = M_1\otimes M_2$ và $N = N_1\otimes N_2$, và xem chúng như các môđun trên vành $A = A_1\otimes A_2$. Đồng cấu chính tắc (II, §3, No. 5, p. 251)

$\lambda :$ Hom$_K(M_1,N_1)\otimes$ Hom$_K(M_2,N_2)\longrightarrow$ Hom$_K(M,N)$

khi đó cảm sinh một đẳng cấu của các không gian vectơ trên K

$\varphi :$ Hom$_{A_1}(M_1,N_1)\otimes$ Hom$_{A_2}(M_2,N_2)\longrightarrow$ Hom$_A(M,N)$.

Ánh xạ $\lambda$ là đơn ánh (II, §7, No. 7, p. 308, Mệnh đề 16) và biến không gian con tuyến tính Hom$_{A_1}(M_1,N_1)\otimes$ Hom$_{A_2}(M_2,N_2)$ vào Hom$_A(M,N)$. Do đó chỉ cần chứng minh rằng mọi ánh xạ A-tuyến tính từ M vào N đều thuộc ảnh của Hom$_{A_1}(M_1,N_1)\otimes$ Hom$_{A_2}(M_2,N_2)$ bởi $\lambda$. Cho $u: M\rightarrow N$ là một ánh xạ A-tuyến tính. Cho $x\in M_1$. Ký hiệu $u_x$ là ánh xạ $A_2$-tuyến tính $y\mapsto u(x\otimes y)$ từ $M_2$ vào $N_1\otimes N_2$. Đặt P = Hom$_{A_2}(M_2,N_2)$, và ký hiệu bởi $\nu$ đồng cấu chính tắc từ $N_1\otimes P$ vào Hom$_{A_2}(M_2,N_1\otimes N_2)$ (II, §4, No. 2, p. 269). Ánh xạ này là đơn ánh (II, §4, No. 2, p. 269, Mệnh đề 2, (i) áp dụng cho không gian vectơ trên K $N_1$). Theo giả thiết (ii), tồn tại một không gian con tuyến tính $V_x$ của $N_1$, hữu hạn chiều trên K, sao cho $u_x$ nhận giá trị trong $V_x\otimes N_2$. Suy ra $u_x$ là ảnh bởi $\nu$ của một phần tử duy nhất $v_x$ của $N_1\otimes P$. Ánh xạ $\widetilde{u}:x\mapsto v_x$ từ $M_1$ vào $N_1\otimes P$ là $A_1$-tuyến tính. Theo giả thiết (i), $A_1$-môđun $M_1$ là sinh hữu hạn. Một lập luận tương tự như trên cho thấy rằng $\widetilde{u}$ thuộc ảnh của Hom$_{A_1}(M_1,N_1)\otimes P$ trong Hom$_{A_1}(M_1,N_1\otimes P)$. Suy ra Bổ đề 1.

#### Định lý 2 {#alg-viii-s12-thm-2 .statement tag=00EB}

Cho $A_1$ và $A_2$ là các đại số trên trường giao hoán K; cho $S_1$ là một $A_1$-môđun đơn và $S_2$ là một $A_2$-môđun đơn. Cho $D_1$ và $D_2$ là các hoán tập tương ứng của $S_1$ và $S_2$. Đặt $M = S_1\otimes S_2,A = A_1\otimes A_2$, và $D = D_1\otimes D_2$. Xem M như một song môđun trái $(A,D)$.

a) Hoán tập của A-môđun M bằng $D_M$.

b) Ánh xạ $\mathfrak{a}\mapsto \mathfrak{a}M$ là một đẳng cấu từ tập hợp các iđêan phải của D, có thứ tự theo bao hàm, tới tập hợp các A-môđun con của M, có thứ tự theo bao hàm. Ánh xạ nghịch đảo gửi một môđun con N của M tới iđêan của D gồm các phần tử $d$ sao cho $dM\subset N$.

Mệnh đề a) suy ra từ Bổ đề 1 vì một môđun đơn là đơn sinh.

Cho T là song môđun $(A_1,D_2$)-$S_1\otimes (D_2)_d$. Ta đồng nhất $M = S_1\otimes S_2$ với $T\otimes_{D_2}S_2$ (II, §3, No. 8, p. 258); sự đồng nhất này tương thích với các cấu trúc môđun trái trên vành $A = A_1\otimes A_2$.

Cho N là một A-môđun con của M; nó là một $A_2$-môđun con của $T\otimes_{D_2}S_2$, ổn định dưới các nội cấu dạng $(a_1)_T\otimes 1_{S_2}$ khi $a_1$ chạy qua $A_1$. Từ Hệ quả 2 của VIII, p. 63 suy ra rằng tồn tại duy nhất một môđun con song $(A_1,D_2)$ của T sao cho $N = V\otimes_{D_2}S_2$.

Đẳng cấu $u$ từ $T = S_1\otimes (D_2)_d$ tới $((D_1)_d\otimes (D_2)_d)\otimes_{D_1}S_1$ được xác định bởi $u(s\otimes d) = 1\otimes d\otimes s$ là $(A_1,D_2$)-tuyến tính. Ta đồng nhất các $(A_1,D_2)$-song môđun này. Một lập luận tương tự như lập luận đã cho ở trên chứng minh sự tồn tại và tính duy nhất của một môđun con phải $(D_1\otimes D_2$) $\mathfrak{a}$ của $D_1\otimes D_2$ sao cho $V =\mathfrak{a}\otimes_{D_1}S_1$. Xét theo các sự đồng nhất đã thực hiện ở trên, $\mathfrak{a}$ là iđêan phải duy nhất của $D = D_1\otimes D_2$ sao cho $N =\mathfrak{a}M$.

Ta vừa chứng minh rằng ánh xạ $\mathfrak{a}\mapsto \mathfrak{a}M$ là song ánh; khẳng định cuối cùng suy ra từ đó.

#### Hệ quả 1 {#alg-viii-s12-thm-2-cor-1 .statement tag=00EC}

Môđun $S_1\otimes S_2$ trên vành $A_1\otimes A_2$ là nửa đơn (tương ứng, đẳng kiểu, đơn) khi và chỉ khi vành $D = D_1\otimes D_2$ là nửa đơn (tương ứng, đơn, một trường). Đặc biệt, $S_1\otimes S_2$ là đơn nếu hoán tập của $S_1$ hoặc của $S_2$ bằng K.

Theo Định lý 2, môđun $S_1\otimes S_2$ trên vành $D_1\otimes D_2$ là nửa đơn (tương ứng, đẳng kiểu, đơn) khi và chỉ khi D-môđun phải $(D_1\otimes D_2)_d$ là như vậy (VIII, p. 109, Mệnh đề 10). Bây giờ, D-môđun phải $D_d$ là đơn khi và chỉ khi D là một trường; nó là đẳng kiểu (tương ứng, nửa đơn) khi và chỉ khi vành D là đơn (tương ứng, nửa đơn) (VIII, p. 120, Định nghĩa 1; VIII, p. 121, Hệ quả 1; và VIII, p. 137, Mệnh đề 2).

#### Hệ quả 2 {#alg-viii-s12-thm-2-cor-2 .statement tag=00ED}

Ta có $\mathfrak{R}_A(M) =\mathfrak{R}(D)M$. A-môđun M không có căn khi và chỉ khi vành D không có căn.

Điều này suy ra từ Mệnh đề 8 của VIII, p. 108 và Định lý 2, b).

### 3. Tích tenxơ của các đại số giao hoán nửa đơn

#### Định lý 3 {#alg-viii-s12-thm-3 .statement tag=00EE}

Cho $Z_1$ và $Z_2$ là các đại số giao hoán nửa đơn trên K. Căn của vành $Z_1\otimes Z_2$ bằng tập hợp các phần tử lũy linh của nó.

Trước hết ta xét trường hợp $Z_1$ và $Z_2$ là các mở rộng $L_1$ và $L_2$ của trường K. Bằng cách đổi chỗ $L_1$ và $L_2$ nếu cần, ta rút gọn về trường hợp bậc siêu việt của $L_1$ trên K nhỏ hơn bậc siêu việt của $L_2$ trên K. Chọn một bao đóng đại số Ω của $L_2$; theo Hệ quả 1 của Định lý 5 của V, §14, No. 6, p. 114, ta có thể giả sử rằng $L_1$ là một mở rộng con của Ω.

A) Trước hết hãy chứng minh rằng căn của $L_1\otimes L_2$ được chứa trong căn của $L_1\otimes \Omega$. Đặt $\mathfrak{a}=\mathfrak{R}(L_1\otimes L_2)(L_1\otimes \Omega )$; đó là một iđêan của vành giao hoán $L_1\otimes \Omega$, và phải chứng minh rằng $\mathfrak{a}$ được chứa trong căn của $L_1\otimes \Omega$. Nói cách khác (VIII, p. 156, Định lý 1), phải chứng minh rằng với $x\in \mathfrak{a}$, phần tử $1 +x$ là khả nghịch trong $L_1\otimes \Omega$. Bây giờ, vì Ω là một mở rộng đại số của $L_2$, nên tồn tại một mở rộng $L_3$ của $L_2$, bậc hữu hạn, sao cho $x$ thuộc về $\mathfrak{R}(L_1\otimes L_2)(L_1\otimes L_3)$. Hiển nhiên chỉ cần chứng minh rằng $1 +x$ là khả nghịch trong $L_1\otimes L_3$. Bây giờ, $C = L_1\otimes L_3$ là một môđun hữu hạn sinh trên vành $B = L_1\otimes L_2$. Theo hệ quả của VIII, p. 175, ta có $\mathfrak{R}(B)C\subset \mathfrak{R}$(C), do đó $x$ thuộc căn của C và $1 +x$ là khả nghịch trong C.

B) Ta sẽ chứng minh rằng căn của $L_1\otimes \Omega$ gồm các phần tử lũy linh. Ký hiệu số mũ đặc số của K là $p$ và bao đóng $p$-căn tương đối (nghĩa là, thuần túy không tách được) của K trong Ω (V, §5, No. 2, p. 25) là P; trường P là hoàn hảo. Vì P là một mở rộng đại số của K, ta có $L_1(P) = L_1[P]$ (V, §3, No. 2, p. 18, Hệ quả 1). Gọi $\mathfrak{b}$ là hạt nhân của đồng cấu chính tắc từ $L_1\otimes P$ vào trường $P_1= L_1[P]$. Lấy $x\in \mathfrak{b}$; tồn tại các phần tử $y_1, . . . , y_n$ của $L_1$ và các phần tử $z_1, . . . , z_n$ của P sao cho $x=\sum^n_{i=1}y_i\otimes z_i$ và $\sum_{i=1}^ny_iz_i= 0$. Vì P là một mở rộng $p$-căn của K, tồn tại một lũy thừa $q$ của $p$ sao cho $z^q_1, . . . , z_n^q$ thuộc K. Khi đó ta có

$$
x^q=\sum_{i=1}^ny^q_i\otimes z_i^q=\sum_{i=1}^ny^q_iz_i^q\otimes 1 =(\sum_{i=1}^ny_iz_i)^q\otimes 1 = 0
$$

Vậy $\mathfrak{b}$ gồm các phần tử lũy linh.

Đặt $\mathfrak{c}=\mathfrak{b}\otimes_P\Omega$; đó là hạt nhân của đồng cấu chính tắc từ $(L_1\otimes P)\otimes_P\Omega$ vào $P_1\otimes_P\Omega$, và theo trên nó gồm các phần tử lũy linh. Bây giờ, Ω là một mở rộng đóng đại số của P, và $P_1$ là một mở rộng con của Ω. Vì trường P là hoàn hảo, $P_1$ là một mở rộng tách được của P (V, §15, No. 5, p. 125, Định lý 3). Theo Định lý 4 của V, p. 120, giao của các iđêan cực đại của vành giao hoán $P_1\otimes_P\Omega$ thu về 0. Nói cách khác, vành $P_1\otimes_P\Omega$, đẳng cấu với $((L_1\otimes P)\otimes_P\Omega )/\mathfrak{c}$, là không có căn. Điều này chứng minh (VIII, p. 155, Mệnh đề 5) rằng $\mathfrak{c}$ chứa căn của vành $(L_1\otimes P)\otimes_P\Omega$. Bây giờ, vành này đẳng cấu với $L_1\otimes \Omega$, và $\mathfrak{c}$ gồm các phần tử lũy linh. Do đó, căn của $L_1\otimes \Omega$ gồm các phần tử lũy linh.

C) Kết thúc chứng minh trong trường hợp riêng. Theo A) và B), căn $\mathfrak{r}$ của $L_1\otimes L_2$ được chứa trong tập hợp $\mathfrak{n}$ các phần tử lũy linh của vành giao hoán này. Hơn nữa, ta biết rằng $\mathfrak{n}$ được chứa trong $\mathfrak{r}$ (VIII, p. 157, Nhận xét 2).

Bây giờ xét trường hợp tổng quát. Vì một đại số giao hoán nửa đơn trên K là tích của hữu hạn mở rộng của trường K (VIII, p. 137, Mệnh đề 3) và căn của một tích các vành là tích của các căn (VIII, p. 156, Hệ quả 3), nên căn của $Z_1\otimes Z_2$ là tập hợp các phần tử lũy linh của vành này.

### 4. Căn của một tích tenxơ các đại số

Cho $A_1$ và $A_2$ là các đại số trên K, và đặt $A = A_1\otimes A_2$.

#### Mệnh đề 3 {#alg-viii-s12-prop-3 .statement tag=00EF}

Giả sử các đại số $A_1$ và $A_2$ là nửa đơn, với các tâm tương ứng $Z_1$ và $Z_2$. Đặt $Z = Z_1\otimes Z_2$.

a) Ánh xạ $\mathfrak{a}\mapsto \mathfrak{a}A$ là một đẳng cấu từ tập hợp các iđêan của Z, được sắp thứ tự bởi quan hệ bao hàm, lên tập hợp các iđêan hai phía của A, được sắp thứ tự bởi quan hệ bao hàm.

b) Căn của A bằng giao của các iđêan hai phía cực đại của A và bằng $\mathfrak{R}(Z)A$.

c) Nếu một trong các K-đại số $Z_1$ và $Z_2$ là tách được, đặc biệt nếu trường K là hoàn hảo, thì các căn của các vành Z và A đều bằng 0.

Mỗi đại số $A_i$ là tích của hữu hạn đại số đơn. Mà tâm của một tích các vành là tích của các tâm, và ta có các mệnh đề tương tự đối với các căn (VIII, p. 156, Hệ quả 3) và đối với các iđêan hai phía (I, §8, No. 10, p. 109, Mệnh đề 8). Vì thế chỉ cần chứng minh Mệnh đề 3 dưới giả thiết rằng $A_1$ và $A_2$ là các đại số đơn.

Với $i\in  \{1,2\}$, đặt $B_i= A_i\otimes A^o_i$, và xem $A_i$ như một $B_i$-môđun, trong đó các phép vị tự được cho bởi công thức

$$
(x\otimes y)z=xzy
$$

với $x,y$, và $z$ trong $A_i$. Hoán tập của $B_i$-môđun $A_i$ là $(Z_i)_{A_i}$, tập hợp các phép vị tự bởi các phần tử của $Z_i$; ta đồng nhất nó với $Z_i$. Hơn nữa, các môđun con $B_i$ của $A_i$ là các iđêan hai phía của $A_i$, và vì vành $A_i$ là đơn, các iđêan hai phía duy nhất là 0 và $A_i$. Do đó $A_i$ là một $B_i$-môđun đơn. Hơn nữa, các môđun con $(B_1\otimes B_2$) của $A_1\otimes A_2$ là các iđêan hai phía của vành $A_1\otimes A_2$.

Mệnh đề a) do đó suy ra từ VIII, p. 214, Định lý 2, b) áp dụng cho $B_1$-môđun đơn $A_1$, với hoán tập $Z_1$, và cho $B_2$-môđun đơn $A_2$, với hoán tập $Z_2$.

Hãy chứng minh mệnh đề b). Giao của các iđêan hai phía cực đại của A là căn của $(B_1\otimes B_2$)-môđun $A_1\otimes A_2$; theo Hệ quả 2 của VIII, p. 215, giao này trùng với $\mathfrak{R}(Z)A$. Các đại số $Z_1$ và $Z_2$ là giao hoán và nửa đơn. Do đó căn của vành Z gồm các phần tử lũy linh (VIII, p. 215, Định lý 3), và iđêan hai phía $\mathfrak{R}(Z)A$ của vành A được chứa trong căn $\mathfrak{R}(A)$ (VIII, p. 157, Nhận xét 1). Tuy nhiên, giao của các iđêan hai phía cực đại của A chứa $\mathfrak{R}(A)$ (VIII, p. 155, Mệnh đề 5, d)). Điều này chứng minh mệnh đề b).

Tích tenxơ của một đại số giao hoán tách được và một đại số giao hoán không nilpotent là một vành không nilpotent (V, §15, No. 2, p. 120, Mệnh đề 5). Các đại số $Z_1$ và $Z_2$ là giao hoán và nửa đơn, do đó không nilpotent. Nếu một trong hai đại số $Z_1$ và $Z_2$ là tách được, thì đại số Z là không nilpotent; vì thế nó không có căn theo Định lý 3 của VIII, p. 215, và ta có $\mathfrak{R}(A) =\mathfrak{R}(Z)A = 0$. Đặc biệt, đây là trường hợp khi trường K là hoàn hảo vì mọi đại số giao hoán không nilpotent trên một trường hoàn hảo đều tách được (V, §15, No. 5, p. 125, Định lý 3).

#### Hệ quả {#alg-viii-s12-n4-cor-1 .statement tag=00EG}

Giả sử rằng các đại số $A_1$ và $A_2$ là đơn và tâm $Z_1$ của $A_1$ thu về K. Khi đó vành $A_1\otimes A_2$ không có iđêan hai phía nào khác ngoài 0 và chính nó.

Theo giả thiết, ta có $Z_1= K$, và vì $A_2$ là đơn nên tâm $Z_2$ của nó là một trường (VIII, p. 121, Hệ quả 1, a)). Do đó vành $Z = Z_1\otimes Z_2$ là một trường, và hệ quả suy ra từ Mệnh đề 3, a).

### 5. Tích Tenxơ của các Môđun Nửa đơn

#### Mệnh đề 4 {#alg-viii-s12-prop-4 .statement tag=00EH}

Với $i\in  \{1,2\}$, cho $A_i$ là một đại số trên K, $M_i$ là một $A_i$-môđun nửa đơn, và $Z_i$ là tâm của hoán tập của $M_i$. Đặt $A = A_1\otimes A_2$, $M = M_1\otimes M_2$, và $Z = Z_1\otimes Z_2$. Ta có $\mathfrak{R}_A(M) =\mathfrak{R}(Z)M$. Nếu một trong hai đại số $Z_1$ và $Z_2$ tách được trên K, đặc biệt nếu trường K là hoàn hảo, thì A-môđun M không có căn.

Với $i\in  \{1,2\}$, cho $S_i$ là một $A_i$-môđun đơn, $D_i$ là hoán tập của nó, và $I(i)$ là một tập hợp. Trước hết ta xét trường hợp $M_i$ là $A_i$-môđun $S_i^{(I(i))}$. Ta đồng nhất tâm $Z_i$ của hoán tập của nó với tâm của $D_i$. Đặt $D = D_1\otimes D_2$. Ta có $\mathfrak{R}(D) =\mathfrak{R}(Z)D$ (Mệnh đề 3 của VIII, p. 217) và $\mathfrak{R}_A(S_1\otimes S_2) =$ $\mathfrak{R}(D)(S_1\otimes S_2)$ (VIII, p. 215, Hệ quả 2), do đó $\mathfrak{R}_A(S_1\otimes S_2) =\mathfrak{R}(Z)(S_1\otimes S_2)$. A-môđun M là tổng trực tiếp của một họ các A-môđun đẳng cấu với $S_1\otimes S_2$, và căn của tổng trực tiếp của một họ môđun là tổng trực tiếp của các căn (VIII, p. 152, Hệ quả 2). Vậy ta có $\mathfrak{R}_A(M) =\mathfrak{R}(Z)M$.

Bây giờ xét trường hợp tổng quát. Với $i\in  \{1,2\}$, ký hiệu giá của $A_i$-môđun $M_i$ bởi $\mathscr{S}_{M_i}$. Với $\lambda \in \mathscr{S}_{M_i}$, ký hiệu thành phần đẳng kiểu của $M_i$ thuộc kiểu $\lambda$ bởi $M_{i;\lambda}$ và tâm của hoán tập của nó bởi $Z_{i;\lambda}$. Ta đồng nhất vành $Z_i$ với tích của các vành $Z_{i;\lambda}$ với $\lambda \in \mathscr{S}_{M_i}$. Cho $\lambda \in \mathscr{S}_{M_1}$ và $\mu\in \mathscr{S}_{M_2}$. Ký hiệu bởi $i_{\lambda}: Z_{1;\lambda}\rightarrow Z_1$ ánh xạ K-tuyến tính duy nhất sao cho pr$_{\lambda}\circ i_{\lambda}$ là ánh xạ đồng nhất trên $Z_{1;\lambda}$ và pr$_{\lambda'}\circ i_{\lambda}$ là ánh xạ không với $\lambda '\in \mathscr{S}_{M_1}-\{\lambda \}$. Định nghĩa $i_\mu: Z_{2;\mu}\rightarrow Z_2$ tương tự. Đặt $Z_{\lambda ,\mu}= Z_{1;\lambda}\otimes Z_{2;\mu}$ và $i_{\lambda ,\mu}=i_{\lambda}\otimes i_\mu$, và ký hiệu ánh xạ pr$_{\lambda}\otimes$ pr$_\mu$ từ Z tới $Z_{\lambda ,\mu}$ bởi $\pi_{\lambda ,\mu}$. Ánh xạ $\pi_{\lambda ,\mu}$ là một đồng cấu vành toàn ánh; do đó ta có $\pi_{\lambda ,\mu}(\mathfrak{R}(Z))\subset \mathfrak{R}(Z_{\lambda ,\mu})$ (VIII, p. 155, Mệnh đề 5, b)). Ta hãy chứng minh bao hàm ngược lại. Cho $z$ là một phần tử của $\mathfrak{R}(Z_{\lambda ,\mu})$; vì $Z_{1;\lambda}$ và $Z_{2;\mu}$ là các trường, $z$ là lũy linh (Định lý 3 của VIII, p. 215). Ta có $i_{\lambda ,\mu}(xy) =i_{\lambda ,\mu}(x)\cdot i_{\lambda ,\mu}(y)$ với $x, y$ trong $Z_{\lambda ,\mu}$; do đó, $i_{\lambda ,\mu}(z)$ là lũy linh và vì thế thuộc $\mathfrak{R}(Z)$. Vì $\pi_{\lambda ,\mu}\circ i_{\lambda ,\mu}$ là ánh xạ đồng nhất trên $Z_{\lambda ,\mu}$, phần tử $z$ thuộc $\pi_{\lambda ,\mu}(\mathfrak{R}(Z))$. Như vậy ta đã chứng minh đẳng thức $\pi_{\lambda ,\mu}(\mathfrak{R}(Z)) =\mathfrak{R}(Z_{\lambda ,\mu})$.

Đặt $M_{\lambda ,\mu}= M_{1;\lambda}\otimes M_{2;\mu}$; đó là một môđun con của M ổn định dưới Z. Với $z\in Z$ và $m\in M_{\lambda ,\mu}$, ta có $zm=\pi_{\lambda ,\mu}(z)m$. Do đó, $\mathfrak{R}(Z)M_{\lambda ,\mu}$ bằng $\mathfrak{R}(Z_{\lambda ,\mu})M_{\lambda ,\mu}$ và vì thế bằng $\mathfrak{R}_A(M_{\lambda ,\mu})$ theo trường hợp đẳng kiểu. Vì căn của một tổng trực tiếp là tổng trực tiếp của các căn (VIII, p. 152, Hệ quả 2) và M là tổng trực tiếp của các môđun con $M_{\lambda ,\mu}$ với $(\lambda , \mu)\in \mathscr{S}_{M_1}\times \mathscr{S}_{M_2}$, đẳng thức $\mathfrak{R}_A(M) =\mathfrak{R}(Z)M$ được chứng minh. Khẳng định cuối cùng khi đó suy ra từ Mệnh đề 3 của VIII, p. 217.

#### Bổ đề 2 {#alg-viii-s12-lem-2 .statement tag=00EI}

Cho $A_1$ và $A_2$ là các đại số trên trường giao hoán K. Cho $M_1$ là một $A_1$-môđun hữu hạn chiều trên K và $M_2$ là một $A_2$-môđun có độ dài hữu hạn. Khi đó $A_1\otimes A_2$-môđun $M_1\otimes M_2$ có độ dài hữu hạn.

Đặt $M = M_1\otimes M_2$. Cho $(e_1, . . . , e_n)$ là một cơ sở của $M_1$ trên trường K. Ánh xạ $(x_1, . . . , x_n)\mapsto \sum^n_{i=1}e_i\otimes x_i$ là một đẳng cấu từ $A_2$-môđun $M^n_2$ lên $A_2$-môđun M. Vì $M_2$ là một $A_2$-môđun có độ dài hữu hạn, nên M cũng vậy. Hơn nữa, mọi A-môđun con của M đều là một $A_2$-môđun con; do đó, M là một A-môđun có độ dài hữu hạn.

#### Mệnh đề 5 {#alg-viii-s12-prop-5 .statement tag=00RC}

Cho $A_1$ và $A_2$ là các đại số trên trường giao hoán K. Cho $M_1$ là một $A_1$-môđun nửa đơn hữu hạn chiều trên K và $M_2$ là một $A_2$-môđun nửa đơn. Với $i\in  \{1,2\}$, ký hiệu hoán tập của $A_i$-môđun $M_i$ là $D_i$ và tâm của $D_i$ là $Z_i$. Đặt $A = A_1\otimes A_2$, M = $M_1\otimes M_2,D = D_1\otimes D_2$, và $Z = Z_1\otimes Z_2$.

a) Hoán tập của A-môđun M có thể được đồng nhất với D, và tâm của nó là Z. Nếu $A_2$-môđun $M_2$ có độ dài hữu hạn, thì A-môđun M có độ dài hữu hạn, vành D là Artin phải và trái, và vành Z là Artin.

b) Các tính chất sau là tương đương:

(i) A-môđun M là nửa đơn.

(ii) Vành Z đẳng cấu với tích của một họ các trường giao hoán.

(iii) Vành Z là rút gọn.

c) Các tính chất sau là tương đương:

(i) A-môđun M là đẳng kiểu và không bị thu về 0.

(ii) Vành Z là một trường.

(iii) Vành Z là một miền nguyên.

Theo giả thiết, $M_1$ hữu hạn chiều trên K. Do đó hoán tập của M có thể được đồng nhất với D (VIII, p. 213, Bổ đề 1), và tâm của nó là Z (III, §4, No. 4, p. 468, Hệ quả). Giả sử $A_2$-môđun $M_2$ có độ dài hữu hạn. A-môđun M có độ dài hữu hạn theo Bổ đề 2. Vì $M_2$ là nửa đơn và sinh hữu hạn, vành $D_2$ là nửa đơn (VIII, p. 139, Mệnh đề 6), và tâm của nó $Z_2$ là tích của một họ hữu hạn các trường giao hoán. Do đó, $D_2$-môđun $(D_2)_s$ và $Z_2$-môđun $(Z_2)_s$ đều có độ dài hữu hạn. Hơn nữa, vì $M_1$ hữu hạn chiều trên K, $D_1$ và $Z_1$ cũng vậy. Theo Bổ đề 2, môđun $(D_1\otimes D_2)_s$ có độ dài hữu hạn; do đó, vành $D_1\otimes D_2$ là Artin trái. Tương tự, ta chứng minh rằng vành $D_1\otimes D_2$ là Artin phải và vành $Z_1\otimes Z_2$ là Artin. Mệnh đề a) suy ra.

Hãy chứng minh b). Tâm của hoán tập của một môđun nửa đơn đẳng cấu với tích của một họ các trường giao hoán (VIII, p. 87, Mệnh đề 8, a)); điều này chứng minh rằng (i) kéo theo (ii). Suy ra (ii) $\Rightarrow$ (iii) là hiển nhiên.

Giả sử rằng vành Z là rút gọn. Khi đó ta có $\mathfrak{R}(Z) = 0$ (VIII, p. 215, Định lý 3) và $\mathfrak{R}_A(M) = 0$ (VIII, p. 218, Mệnh đề 4). Vì $A_2$-môđun $M_2$ là nửa đơn, tồn tại một họ $(S_i)_{i\in I}$ các $A_2$-môđun đơn và một đẳng cấu từ $M_2$ lên $\bigoplus S_i$. Do đó, A-môđun M đẳng cấu với $\bigoplus M_1\otimes S_i$. Với mọi $i\in I$, A-môđun $M_1\otimes S_i$ vì thế không có căn. Theo a), nó có độ dài hữu hạn; vì vậy nó là nửa đơn (VIII, p. 153, Mệnh đề 3, b)). Khi đó A-môđun M là tổng trực tiếp của một họ các môđun nửa đơn và do đó là nửa đơn. Điều này chứng minh rằng (iii) kéo theo (i) và kết thúc chứng minh của b).

Một A-môđun là đẳng kiểu và khác không khi và chỉ khi nó là nửa đơn và tâm của hoán tập của nó là một trường (VIII, p. 87, Mệnh đề 8, b)). Vậy c) suy ra từ b).

#### Hệ quả {#alg-viii-s12-n5-cor-1 .statement tag=00EJ}

Nếu $Z_1$ hoặc $Z_2$ là một đại số tách được trên trường K (chẳng hạn như khi K là hoàn hảo), thì A-môđun $M_1\otimes M_2$ là nửa đơn.

Các vành $Z_1$ và $Z_2$ đẳng cấu với các tích của các trường và vì thế là các vành thu gọn. Đặc biệt, nếu K là hoàn hảo, thì chúng là các đại số tách được trên K (V, §15, No. 5, p. 125, Định lý 3). Theo Mệnh đề 5 của V, §15, No. 2, p. 120, tích tenxơ của một đại số tách được và một đại số thu gọn là thu gọn. Vậy Z là một vành thu gọn, và hệ quả suy ra từ Mệnh đề 5, b).

### 6. Tích Tenxơ Của Các Đại Số Nửa Đơn

#### Mệnh đề 6 {#alg-viii-s12-prop-6 .statement tag=00EK}

Cho $A_1$ và $A_2$ là các K-đại số khác không. Nếu vành $A_1\otimes A_2$ là đơn (tương ứng, nửa đơn), thì các vành $A_1$ và $A_2$ là đơn (tương ứng, nửa đơn).

Một vành B là nửa đơn (tương ứng, đơn) khi và chỉ khi B-môđun $B_s$ là nửa đơn (tương ứng, đẳng kiểu và khác không). Do đó mệnh đề suy ra từ Mệnh đề 1 (VIII, p. 211).

#### Mệnh đề 7 {#alg-viii-s12-prop-7 .statement tag=00EL}

Cho $A_1$ và $A_2$ là các K-đại số nửa đơn, với các tâm tương ứng $Z_1$ và $Z_2$. Giả sử rằng $A_1$ có bậc hữu hạn trên K. Khi đó vành $A_1\otimes A_2$ là Artin trái, cũng như tâm của nó $Z_1\otimes Z_2$. Vành $A_1\otimes A_2$ là đơn (resp. nửa đơn) khi và chỉ khi vành $Z_1\otimes Z_2$ là một trường (resp. một vành rút gọn).

Đây là trường hợp $M_1= (A_1)_s, M_2= (A_2)_s$ của Mệnh đề 5 của VIII, p. 219.

#### Hệ quả 1 {#alg-viii-s12-prop-7-cor-1 .statement tag=00EM}

Cho $A_1$ và $A_2$ là các K-đại số nửa đơn; giả sử rằng $A_1$ hữu hạn chiều trên K. Giả sử rằng tâm của $A_1$ hoặc $A_2$ là một đại số tách được trên K; chẳng hạn, đó là trường hợp khi K hoàn hảo. Khi đó $A_1\otimes A_2$ là nửa đơn.

Đây là trường hợp $M_1= (A_1)_s, M_2= (A_2)_s$ của hệ quả ở VIII, p. 221.

#### Hệ quả 2 {#alg-viii-s12-prop-7-cor-2 .statement tag=00RD}

Cho $A_1$ và $A_2$ là các K-đại số đơn; giả sử rằng $A_1$ hữu hạn chiều trên K. Nếu tâm của $A_1$ hoặc $A_2$ bằng K, thì đại số $A_1\otimes A_2$ là đơn. Đặc biệt, đây là trường hợp khi K đóng đại số.

Các tâm $Z_1$ và $Z_2$ của $A_1$ và $A_2$, tương ứng, là các trường; nếu một trong các vành $Z_1$ và $Z_2$ bằng K, thì vành $Z_1\otimes Z_2$ là một trường. Do đó chỉ cần áp dụng Mệnh đề 7.

Nếu trường K đóng đại số, thì tâm của $A_1$ bằng K.

### 7. Mở rộng vô hướng trong các môđun nửa đơn

#### Mệnh đề 8 {#alg-viii-s12-prop-8 .statement tag=00EN}

Cho A là một đại số trên K, M là một A-môđun, và L là một mở rộng của trường K. Ký hiệu hoán tập của M là D và tâm của D là Z.

a) Giả sử rằng $A_{(L)}$-môđun $M_{(L)}$ là đơn (tương ứng, đẳng kiểu, nửa đơn). Khi đó A-môđun M là đơn (tương ứng, đẳng kiểu, nửa đơn).

b) Giả sử rằng A-môđun M là nửa đơn và M hoặc L là hữu hạn chiều trên K. A-môđun $A_{(L)}$ $M_{(L)}$ là nửa đơn khi và chỉ khi vành $Z_{(L)}$ là rút gọn. A-môđun $A_{(L)}$ $M_{(L)}$ là đẳng kiểu và khác không khi và chỉ khi vành $Z_{(L)}$ là một miền nguyên.

c) Giả sử rằng A-môđun M là đơn. A-môđun $A_{(L)}$ $M_{(L)}$ là nửa đơn (tương ứng, đẳng kiểu, đơn) khi và chỉ khi vành $D_{(L)}$ là nửa đơn (tương ứng, đơn, một trường).

Mệnh đề a) là một trường hợp riêng của Mệnh đề 1 (VIII, p. 211), mệnh đề b) là một trường hợp riêng của Mệnh đề 5 (VIII, p. 219), và mệnh đề c) là một trường hợp riêng của Hệ quả 1 của VIII, p. 215.

#### Hệ quả 1 {#alg-viii-s12-prop-8-cor-1 .statement tag=00EO}

a) Giả sử rằng A-môđun M là nửa đơn, rằng mở rộng L của K là tách được, và rằng M hoặc L là hữu hạn chiều trên K. Khi đó A-môđun $A_{(L)}$ $M_{(L)}$ là nửa đơn.

b) Giả sử rằng A-môđun M là đơn và hoán tập của nó bằng K. Khi đó A-môđun $A_{(L)}$ $M_{(L)}$ là đơn.

Mệnh đề a) suy ra từ Hệ quả VIII, p. 221. Mệnh đề b) là một trường hợp riêng của Mệnh đề 8, c).

#### Hệ quả 2 {#alg-viii-s12-prop-8-cor-2 .statement tag=00RE}

Cho L là một mở rộng của trường K. Ký hiệu tâm của đại số trên K A là Z.

a) Nếu đại số trên L $A_{(L)}$ là nửa đơn, thì đại số trên K A là nửa đơn.

b) Giả sử đại số trên K A là nửa đơn và L hoặc A là hữu hạn chiều trên K. Đại số trên L $A_{(L)}$ là nửa đơn khi và chỉ khi vành $Z_{(L)}$ là reduced; điều này, đặc biệt, đúng khi L là một mở rộng tách được của K. Đại số trên L $A_{(L)}$ là đơn khi và chỉ khi vành $Z_{(L)}$ là một miền nguyên; điều này, đặc biệt, đúng khi tâm của A bằng K.

Các khẳng định a) và b) suy ra từ Mệnh đề 8, a) và b) áp dụng cho A-môđun $A_s$.

#### Mệnh đề 9 {#alg-viii-s12-prop-9 .statement tag=00EP}

Cho A là một đại số trên K và L là một mở rộng tách được của K.

a) Nếu M là một A-môđun không có căn, thì $A_{(L)}$-môđun $M_{(L)}$ không có căn.

b) Nếu đại số trên K A không có căn, thì đại số trên L $A_{(L)}$ không có căn.

Hãy chứng minh mệnh đề a). Cho M là một A-môđun không có căn. Ta đồng nhất M với ảnh chính tắc của nó trong $M_{(L)}$. Cho N là một môđun con cực đại của M. Vì A-môđun $M/N$ là đơn, suy ra từ Mệnh đề 4 của VIII, p. 218 rằng $A_{(L)}$-môđun $(M/N)_{(L)}= M_{(L)}/N_{(L)}$ không có căn và do đó $\mathfrak{R}_{A_{(L)}}(M_{(L)})\subset N_{(L)}$ theo Hệ quả 1, c) của VIII, p. 152. Bây giờ, từ hệ quả của Mệnh đề 14 của II, §7, No. 7, p. 306 suy ra rằng giao của các $N_{(L)}$, trong đó N chạy qua tập hợp các môđun con cực đại của M, thu về 0. Do đó, $A_{(L)}$-môđun $M_{(L)}$ không có căn.

Mệnh đề b) suy ra từ mệnh đề a) áp dụng cho A-môđun $A_s$.

#### Mệnh đề 10 {#alg-viii-s12-prop-10 .statement tag=00EQ}

Cho A là một đại số trên K và L là một mở rộng của K. Cho M là một A-môđun.

a) Ta đặt một trong hai giả thiết sau:

(i) A-môđun M sinh hữu hạn và L đại số trên K.

(ii) Vành A là Artin trái.

Khi đó ta có bao hàm

$$
\mathfrak{R}_A(M)_{(L)}\subset \mathfrak{R}_{A_{(L)}}(M_{(L)})
$$

b) Nếu L là một mở rộng tách được của K, thì ta có bao hàm

$$
\mathfrak{R}_{A_{(L)}}(M_{(L)})\subset \mathfrak{R}_A(M)_{(L)}
$$

Hãy chứng minh mệnh đề a). Xét trường hợp (i). Trước hết giả sử rằng L có bậc hữu hạn trên K. Khi đó A-môđun $M_{(L)}$ là sinh hữu hạn. Ký hiệu đồng cấu chính tắc từ A vào $A_{(L)}$ là $f$; vành $A_{(L)}$ được sinh bởi hợp của tâm của nó và $f(A)$. Do đó ta có thể áp dụng Mệnh đề 3 của VIII, p. 174 cho $A_{(L)}$-môđun $M_{(L)}$. Điều này cho bao hàm $\mathfrak{R}_A(M_{(L)})\subset \mathfrak{R}_{A_{(L)}}(M_{(L)})$ và a fortiori $\mathfrak{R}_A(M)_{(L)}\subset \mathfrak{R}_{A_{(L)}}(M_{(L)})$ (VIII, p. 152, Hệ quả 1).

Bây giờ ta xét trường hợp tổng quát. Cho $x_1, . . . , x_n$ là các phần tử sinh A-môđun M và $x$ là một phần tử của $\mathfrak{R}_A(M)$. Cho $a_1, . . . , a_n$ là các phần tử của $A_{(L)}$; vì L là đại số trên K, tồn tại một mở rộng hữu hạn $L'$ của K được chứa trong L sao cho các $a_i$ thuộc $A_{(L')}$. Theo điều trên, $x$ thuộc căn của $A_{(L')}$-môđun $M_{(L')}$; từ hệ quả ở VIII, p. 153 suy ra rằng các phần tử $x_i+a_ix$ với $1\leqslant i\leqslant n$ sinh $A_{(L')}$-môđun $M_{(L')}$ và do đó sinh $A_{(L)}$-môđun $M_{(L)}$. Theo cùng hệ quả ấy, $x$ thuộc căn của $A_{(L)}$-môđun $M_{(L)}$.

Bây giờ ta xét trường hợp (ii). Gọi $\mathfrak{r}$ là căn của A, sao cho căn của A-môđun M bằng $\mathfrak{r}M$ (VIII, p. 174, Hệ quả). Căn $\mathfrak{r}$ của A là một iđêan hai phía lũy linh của A (VIII, p. 173, Mệnh đề 1); do đó, $\mathfrak{r}_{(L)}$ là một iđêan hai phía lũy linh của $A_{(L)}$. Suy ra $\mathfrak{r}_{(L)}\subset \mathfrak{R}(A_{(L)})$ (VIII, p. 156, Định lý 1), và Mệnh đề 6 của VIII, p. 158 kéo theo $\mathfrak{R}(A_{(L)})M_{(L)}\subset \mathfrak{R}_{A_{(L)}}(M_{(L)})$. Vậy ta có $\mathfrak{R}_A(M) =\mathfrak{r}M\subset$ $\mathfrak{R}_{A_{(L)}}(M_{(L)})$, điều này kết thúc chứng minh mệnh đề a).

Môđun $M/\mathfrak{R}_A(M)$ không có căn. Nếu L là một mở rộng tách được của K, thì từ Mệnh đề 9 của VIII, p. 223 suy ra rằng $A_{(L)}$-môđun $(M/\mathfrak{R}_A(M))_{(L)}$ không có căn. Do đó, ta có bao hàm

$$
\mathfrak{R}_{A_{(L)}}(M_{(L)})\subset \mathfrak{R}_A(M)_{(L)}
$$

#### Hệ quả {#alg-viii-s12-n7-cor-1 .statement tag=00ER}

Cho L là một mở rộng tách được của K. Ta có $\mathfrak{R}(A_{(L)}) =$ $\mathfrak{R}(A)_{(L)}$ nếu L đại số trên K hoặc nếu vành A là Artin trái.

Đây là trường hợp $M = A_s$ của Mệnh đề 10.

### Bài tập {#alg-viii-s12-exercises}

Xem [các bài tập cho § 12](exercises/s12/).
