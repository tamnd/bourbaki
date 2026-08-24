---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VII
chapter_title: CARTAN SUBALGEBRAS AND REGULAR ELEMENTS
section: 1
section_title: Polynomial maps and Zariski topology
appendix: true
lang: vi
source: lie-vii-ix
book_pages: 45-47, 66
pdf_pages: 0055-0057, 0075-0075
extraction: native
subsections:
    - "no": 1
      title: ZARISKI TOPOLOGY
      page: 45
      pdf_page: 55
    - "no": 2
      title: DOMINANT POLYNOMIAL MAPS
      page: 46
      pdf_page: 56
statements: 7
exercises: 4
content_sha256: bf8891d25017fcf0101ae7b4677941603c38a2ab738a9b6995eaee0501f43988
translated_from: content/en/lie/VII/A1_a1_polynomial_maps_and_zariski_topology.md
source_content_sha256: 35b05a39838f20b88ddf3fc98b3fdd147867c98e1efaf99bb5c98caf247537a5
translation_model: gpt-5.4
translation_run: translate-vi-2839cc10
glossary_version: 34
glossary_terms_sha256: 84b4646e2f1b982a3fd497f4b3b8d2b4e39e27bee68e3b1227f6d86911623826
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## PHỤ LỤC I ÁNH XẠ ĐA THỨC VÀ TÔPÔ ZARISKI

Trong phụ lục này, giả thiết rằng $k$ là vô hạn.

### 1. TÔPÔ ZARISKI

Cho V là một không gian vectơ hữu hạn chiều. Ký hiệu $A_V$ là đại số các hàm đa thức trên V nhận giá trị trong $k($Đại số, Ch. IV, §5, no. 10, Đn. 4). Đây là một đại số phân bậc; thành phần bậc 1 của nó là đối ngẫu $V^*$ của V, và đơn ánh từ $V^*$ vào $A_V$ được mở rộng thành một đẳng cấu từ đại số đối xứng $\mathbf{S}(V^*)$ lên $A_V($Đại số, Ch. IV, §5, no. 11, Nhận xét 2).

Nếu $(e_1, . . . , e_n)$ là một cơ sở của V, và $(X_1, . . . ,X_n)$ là một dãy các ẩn, thì ánh xạ từ $k[X_1, . . . ,X_n]$ vào $A_V$ gán cho mọi phần tử $f$ của $k[X_1, . . . ,X_n]$ hàm

$$
\sum_{i=1}^n\lambda_ie_i \rightarrow f(\lambda_1, . . . , \lambda_n)
$$

là một đẳng cấu đại số (Đại số, Ch. IV, §5, no. 10, Hệ quả của Mệnh đề 19).

#### Mệnh đề 1 {#lie-vii-a1-prop-1 .statement tag=00XC}

Cho H là tập hợp các đồng cấu đại số từ $A_V$ đến $k$. Với mọi $x\in V$, gọi $h_x$ là đồng cấu $f \rightarrow f(x)$ từ $A_V$ đến $k$. Khi đó, ánh xạ $x \rightarrow h_x$ là một song ánh từ V lên H.

Thật vậy, gọi $H'$ là tập hợp các đồng cấu đại số từ $k[X_1, . . . ,X_n]$ đến $k$. Ánh xạ $\chi  \rightarrow (\chi (X_1), . . . , \chi (X_n))$ rõ ràng là một song ánh từ $H'$ lên $k^n$.

#### Hệ quả {#lie-vii-a1-n1-cor-1 .statement tag=00XD}

Với mọi $x\in V$, đặt $\mathfrak{m}_x=$ Ker($h_x$). Khi đó ánh xạ $x \rightarrow \mathfrak{m}_x$ là một song ánh từ V lên tập hợp các iđêan $\mathfrak{m}$ của $A_V$ sao cho $A_V/\mathfrak{m}=k$.

Một tập con F của V được gọi là đóng nếu tồn tại một họ $(f_i)_{i\in I}$ các phần tử của $A_V$ sao cho $x\in F\Leftarrow \Rightarrow x\in V$ và $f_i(x) = 0$ với mọi $i\in I$.

Hiển nhiên là $\emptyset$ và V là đóng, và giao tùy ý của các tập đóng là đóng. Nếu F được xác định bởi sự triệt tiêu của các $f_i$ và $F'$ bởi sự triệt tiêu của các $f'_j$, thì $F\cup F'$ được xác định bởi sự triệt tiêu của các $f_if'_j$, và do đó là đóng. Vậy tồn tại một tôpô trên V sao cho các tập đóng đối với tôpô này chính xác là các tập đóng theo nghĩa ở trên. Tôpô này được gọi là tôpô Zariski trên V. Với mọi $f\in A_V$, ta ký hiệu bởi $V_f$ tập hợp các $x\in V$ sao cho $f(x)\not= 0$; đó là một tập con mở của V. Hiển nhiên là các $V_f$ lập thành một cơ sở của tôpô Zariski. (Nếu $k$ là một trường tôpô, thì tôpô chính tắc của V mịn hơn tôpô Zariski.)

Ánh xạ $x \rightarrow \mathfrak{m}_x$ của Hệ quả của Mệnh đề 1 có thể được coi như một ánh xạ $\varepsilon$ từ V vào phổ nguyên tố Spec(A$_V$) của $A_V($Đại số giao hoán, Chương II, §4, no. 3, Định nghĩa 4). Ngay lập tức thấy rằng tôpô Zariski là ảnh ngược theo $\varepsilon$ của tôpô của Spec(A$_V$).

#### Mệnh đề 2 {#lie-vii-a1-prop-2 .statement tag=00XE}

Không gian vectơ V, được trang bị tôpô Zariski, là một không gian bất khả quy Noether. Đặc biệt, mọi tập con mở không rỗng của V đều trù mật.

Vì $A_V$ là Noether, Spec(A$_V$) là Noether (Đại số giao hoán, Chương II, §4, no. 3, Hệ quả 7 của Mệnh đề 11), và mọi không gian con của một không gian Noether đều là Noether (loc. cit., no. 2, Mệnh đề 8). Với ký hiệu của Hệ quả của Mệnh đề 1, giao của các $\mathfrak{m}_x$ là $\{0\}$, và $\{0\}$ là một iđêan nguyên tố của $A_V$; do đó V là bất khả quy (loc. cit., no. 3, Mệnh đề 14).

### 2. CÁC ÁNH XẠ ĐA THỨC TRỘI

Cho $V,W$ là các không gian vectơ hữu hạn chiều. Cho $f$ là một ánh xạ đa thức từ V vào W (Đại số, Chap. IV, §5, no. 10, Định nghĩa 4). Nếu $\psi \in A_W,\psi \circ f\in A_V$ (loc. cit., Mệnh đề 17). Ánh xạ $\psi  \rightarrow \psi \circ f$ là một đồng cấu từ $A_W$ vào $A_V$, được gọi là liên kết với $f$. Hạt nhân của nó gồm các hàm $\psi \in A_W$ triệt tiêu trên $f(V)$ (và do đó cả trên bao đóng của $f(V)$ trong tôpô Zariski).

#### Định nghĩa 1 {#lie-vii-a1-def-1 .statement tag=00XF}

Một ánh xạ đa thức $f: V\rightarrow W$ được gọi là trội nếu đồng cấu từ $A_W$ vào $A_V$ liên kết với $f$ là đơn ánh.

Theo điều đã nói trước đó, $f$ là trội khi và chỉ khi $f(V)$ trù mật trong W đối với tôpô Zariski.

#### Mệnh đề 3 {#lie-vii-a1-prop-3 .statement tag=00XG}

Giả sử rằng $k$ đóng đại số. Cho $f: V\rightarrow W$ là một ánh xạ đa thức trội. Ảnh qua $f$ của mọi tập con mở trù mật của V chứa một tập con mở trù mật của W.

Chỉ cần chứng minh rằng, với mọi phần tử khác không $\varphi$ của $A_V,f(V_{\varphi})$ chứa một tập con mở trù mật của W. Đồng nhất $A_W$ với một đại số con của $A_V$ bằng đồng cấu liên kết với $f$. Tồn tại một phần tử khác không $\psi$ của $A_W$ sao cho mọi đồng cấu $w: A_W\rightarrow k$ không triệt tiêu $\psi$ đều mở rộng thành một đồng cấu $v: A_V\rightarrow k$ không triệt tiêu $\varphi ($đại số giao hoán, Chap. V, §3, no. 1, Hệ quả 3 của Định lý 1). Khi đó một $w$ như vậy (resp. một $v$ như vậy) có thể được đồng nhất với một phần tử của $W_{\psi}$ (resp. của $V_{\varphi}$) và nói rằng $v$ mở rộng $w$ có nghĩa là $f(v) =w$. Do đó, $W_{\psi}\subset f(V_{\varphi})$. Q.E.D.

Cho $f: V\rightarrow W$ là một ánh xạ đa thức, và $x_0\in V$. Ánh xạ $h \rightarrow f(x_0+h)$ từ V đến W là đa thức. Phân tích nó thành một tổng hữu hạn các ánh xạ đa thức thuần nhất:

$$
f(x_0+h) =f(x_0) + D_1(h) + D_2(h) +\cdots
$$

trong đó $D_i: V\rightarrow W$ là thuần nhất bậc $i($Đại số, Chương IV, §5, no. 10, Mệnh đề 19). Ánh xạ tuyến tính $D_1$ được gọi là ánh xạ tuyến tính tiếp xúc của $f$ tại $x_0$. Ta ký hiệu nó bởi $Df(x_0)$.

#### Mệnh đề 4 {#lie-vii-a1-prop-4 .statement tag=00XH}

Cho $f: V\rightarrow W$ là một ánh xạ đa thức. Giả sử rằng tồn tại $x_0\in V$ sao cho $(Df)(x_0)$ là toàn ánh. Khi đó $f$ là trội.

Áp dụng một phép tịnh tiến trong V và một phép tịnh tiến trong W, ta có thể giả sử rằng $x_0= 0$ và $f(x_0) = 0$. Khi đó phân tích của $f$ thành một tổng các phần tử thuần nhất có thể được viết

$f=f_1+f_2+\cdots$ với bậc của $f_i=i$,

và ánh xạ tuyến tính $f_1$ là toàn ánh theo giả thiết. Giả sử rằng $f$ không trội. Khi đó tồn tại một phần tử khác không $\psi$ của $A_W$ sao cho $\psi \circ f= 0$. Gọi $\psi =\psi_m+\psi_{m+1}+\cdots$ là phân tích của $\psi$ thành các phần tử thuần nhất, với bậc của $\psi_i=i$ và $\psi_m\not= 0$. Khi đó

$$
0 =\psi \circ f=\psi_m\circ f+\psi_{m+1}\circ f+\cdots
$$

$$
=\psi_m\circ f_1+\rho
$$

trong đó $\rho$ là một tổng các ánh xạ đa thức thuần nhất bậc $> m$. Suy ra $\psi_m\circ f_1= 0$. Vì $f_1$ là toàn ánh, nên $\psi_m= 0$, mâu thuẫn.

#### Hệ quả {#lie-vii-a1-n2-cor-1 .statement tag=00XI}

Nếu $k$ đóng đại số và nếu $f$ thỏa mãn các giả thiết của Mệnh đề 4, thì ảnh qua $f$ của mọi tập con mở trù mật của V chứa một tập con mở trù mật của W.

Điều này suy ra từ các Mệnh đề 3 và 4.

### Bài tập {#lie-vii-a1-exercises}

Ký hiệu V là một không gian vectơ hữu hạn chiều trên $k$.

Xem [các bài tập của Phụ lục 1](exercises/a1/).
