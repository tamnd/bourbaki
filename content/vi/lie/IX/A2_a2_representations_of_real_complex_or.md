---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IX
chapter_title: COMPACT REAL LIE GROUPS
section: 2
section_title: Representations of real, complex or quaternionic type
appendix: true
lang: vi
source: lie-vii-ix
book_pages: 385-388
pdf_pages: 0392-0395
extraction: native
subsections:
    - "no": 1
      title: REPRESENTATIONS OF REAL ALGEBRAS
      page: 385
      pdf_page: 392
    - "no": 2
      title: REPRESENTATIONS OF COMPACT GROUPS
      page: 387
      pdf_page: 394
statements: 6
exercises: 0
content_sha256: 5b3522ce7f0ebfd846b40d68e702cd567d4af809ed79f729ed49f0a2d0d0ac77
translated_from: content/en/lie/IX/A2_a2_representations_of_real_complex_or.md
source_content_sha256: 166c8e4a3ff2601758b90e2cbc28e90c5ad2ac9dc57f18a2eb1d30f70fa6ca87
translation_model: gpt-5-6, gpt-5.4
translation_run: translate-vi-dced90e6
glossary_version: 34
glossary_terms_sha256: 9dbb7bcc047df64a2ced378885717f768a615524d7fd30c74f449fa2fd216117
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## PHỤ LỤC II

# CÁC BIỂU DIỄN KIỂU THỰC, PHỨC HOẶC QUATERNION

### 1. CÁC BIỂU DIỄN CỦA ĐẠI SỐ THỰC

Ký hiệu bởi $\sigma$ tự đẳng cấu $\alpha  \rightarrow \overline{\alpha}$ của $\mathbf{C}$; nếu W là một không gian vectơ phức, ký hiệu bởi W không gian vectơ trên $\mathbf{C}$ $\sigma_*(W)$ (nghĩa là, nhóm W với luật phép toán $(\alpha , w) \rightarrow \overline{\alpha w}$ đối với $\alpha \in \mathbf{C}, w\in W$).

#### Mệnh đề 1 {#lie-ix-a2-prop-1 .statement tag=01IS}

Cho A là một $\mathbf{R}$-đại số (kết hợp và có đơn vị) và V là một A-môđun đơn hữu hạn chiều trên $\mathbf{R}$. Khi đó, ta ở trong một trong ba tình huống sau:

$\alpha )$ Hoán tập của V (Đại số, Chương VIII, § 5, no. 1) đẳng cấu với $\mathbf{R}$, và $A_{(\mathbf{C})}$-môđun $V_{(\mathbf{C})}$ là đơn;

$\beta )$ hoán tập của V đẳng cấu với $\mathbf{C}$; $A_{(\mathbf{C})}$-môđun $V_{(\mathbf{C})}$ là tổng trực tiếp của hai $A_{(\mathbf{C})}$-môđun con đơn không đẳng cấu, bị hoán đổi bởi $\sigma \otimes 1_V$;

$\gamma )$ hoán tập của V đẳng cấu với $\mathbf{H}$; $A_{(\mathbf{C})}$-môđun $V_{(\mathbf{C})}$ là tổng trực tiếp của hai $A_{(\mathbf{C})}$-môđun con đơn đẳng cấu, bị hoán đổi bởi $\sigma \otimes 1_V$.

Hoán tập E của V là một trường, một mở rộng hữu hạn của $\mathbf{R}($Đại số, Chương VIII, §3, no. 2, Mệnh đề 2), do đó đẳng cấu với $\mathbf{R},\mathbf{C}$ hoặc $\mathbf{H}($Đại số, Chương VIII, §15). $A_{(\mathbf{C})}$-môđun $V_{(\mathbf{C})}$ là nửa đơn (Đại số, Chương VIII, §11, no. 4), và hoán tập của nó có thể được đồng nhất với $\mathbf{C}\otimes_{\mathbf{R}}E ($Đại số, Chương VIII, §11, no. 2, Bổ đề 1).

Nếu E đẳng cấu với $\mathbf{R}$, thì hoán tập của $V_{(\mathbf{C})}$ đẳng cấu với $\mathbf{C}$, và $V_{(\mathbf{C})}$ là một $A_{(\mathbf{C})}$-môđun đơn (Đại số, Chương VIII, §11, no. 4).

Nếu E không đẳng cấu với $\mathbf{R}$, thì nó chứa một trường đẳng cấu với $\mathbf{C}$; suy ra V có một cấu trúc $A_{(\mathbf{C})}$-môđun, ký hiệu là $V^c$. Khi đó $V^c$ là một $A_{(\mathbf{C})}$-môđun đơn, và ánh xạ $\mathbf{C}$-tuyến tính $\psi : V_{(\mathbf{C})}\rightarrow V^c\oplus \overline{V}^c$ sao cho $\psi (\alpha \otimes v) =$ $(\alpha v,\overline{\alpha v})$ với $\alpha \in \mathbf{C},v\in V$, là một đẳng cấu (Đại số, Chương V, §10, no. 4, Mệnh đề 8). Hơn nữa, $\sigma \otimes 1_V$ tương ứng qua đẳng cấu này với tự đẳng cấu $\mathbf{R}$ $(v, v') \rightarrow (v', v)$ của $V^c\oplus \overline{V}^c$, và do đó hoán đổi hai $A_{(\mathbf{C})}$-môđun con $\psi^{-1}(V^c)$ và $\psi^{-1}(V^c)$.

Hoán tập $E_{(\mathbf{C})}$ của $V_{(\mathbf{C})}$ do đó chứa $\mathbf{C}\times \mathbf{C}$, tác động bằng các phép vị tự trên $V^c\oplus \overline{V}^c$. Không tồn tại đẳng cấu nào của các $A_{(\mathbf{C})}$-môđun từ $V^c$ đến $\overline{V}^c$ khi và chỉ khi $E_{(\mathbf{C})}$ thu về $\mathbf{C}\times \mathbf{C}$, tức là, khi E đẳng cấu với $\mathbf{C}$. Điều này hoàn tất chứng minh.

#### Mệnh đề 2 {#lie-ix-a2-prop-2 .statement tag=01IT}

Cho A là một $\mathbf{R}$-đại số (kết hợp và có đơn vị), và W là một $A_{(\mathbf{C})}$-môđun đơn hữu hạn chiều trên $\mathbf{C}$. Khi đó, ta tất yếu ở trong một trong ba tình huống sau:

a) Tồn tại một $A_{(\mathbf{C})}$-đẳng cấu $\theta$ từ W lên $\overline{W}$ sao cho $\theta \circ \theta = 1_W$. Khi đó tập hợp V các điểm bất động của $\theta$ là một $\mathbf{R}$-cấu trúc trên W, và là một A-môđun đơn có hoán tập $\mathbf{R}.1_V$. Hơn nữa, $W_{[\mathbf{R}]}$ là tổng trực tiếp của hai A-môđun đơn đẳng cấu.

b) Các $A_{(\mathbf{C})}$-môđun W và $\overline{W}$ không đẳng cấu; khi đó $W_{[\mathbf{R}]}$ là một A-môđun đơn có hoán tập $\mathbf{C}.1_W$.

c) Tồn tại một $A_{(\mathbf{C})}$-đẳng cấu $\theta$ từ W đến $\overline{W}$ sao cho $\theta \circ \theta =-1_W$. Khi đó A-môđun $W_{[\mathbf{R}]}$ là đơn, và hoán tập của nó là trường $\mathbf{C}.1_W\oplus \mathbf{C}.\theta$, đẳng cấu với $\mathbf{H}$.

Không gian vectơ phức Hom$_{A_{(\mathbf{C})}}(W,W)$ có chiều $\leq 1 ($Đại số, Chương VIII, §3, no. 2); nếu $\theta \in$ Hom$_{A_{(\mathbf{C})}}(W,W)$, thì tự đồng cấu $\theta \circ \theta$ của W là một phép vị tự, có tỷ số $\alpha \in \mathbf{C}$. Với mọi $w\in W$, ta có $\alpha \theta (w) =\theta \circ \theta \circ \theta (w) =$ $\theta (\alpha w) = \overline{\alpha \theta}(w)$, nên $\alpha$ là thực. Nếu $\theta '=\lambda \theta$, với $\lambda \in \mathbf{C}$, thì $\theta '\circ \theta '=|\lambda |^2\theta \circ \theta$; do đó, chính xác một trong ba khả năng sau đây xảy ra:

a) Tồn tại $\theta \in$ Hom$_{A_{(\mathbf{C})}}(W,W)$ sao cho $\theta \circ \theta = 1_W$;

b) Hom$_{A_{(\mathbf{C})}}(W,W) =\{0\}$;

c) Tồn tại $\theta \in$ Hom$_{A_{(\mathbf{C})}}(W,W)$ sao cho $\theta \circ \theta =-1_W$.

Trong trường hợp a), tập hợp V các điểm bất động của $\theta$ là một cấu trúc $\mathbf{R}$ trên W (Đại số, Chương V, p. 61, Mệnh đề 7); vì $V_{(\mathbf{C})}$ đẳng cấu với W, A-môđun V là đơn với hoán tập $\mathbf{R}.1_V$ (Mệnh đề 1), và $W_{[\mathbf{R}]}$ không đơn.

Ngược lại, nếu $W_{[\mathbf{R}]}$ không đơn, cho V là một A-môđun con đơn của $W_{[\mathbf{R}]}$; vì $A_{(\mathbf{C})}$-môđun W là đơn, nên $V +iV = W$ và $V\cap iV =\{0\}$, nghĩa là $W = V\oplus iV$. Do đó, V là một cấu trúc $\mathbf{R}$ trên W, và đẳng cấu $\theta$ từ W đến $\overline{W}$ sao cho $\theta (v+iv') =v-iv'$ với $v$ và $v'$ trong V thỏa mãn $\theta \circ \theta = 1_W$.

Do đó, trong các trường hợp b) và c), A-môđun $W_{[\mathbf{R}]}$ là đơn; theo Mệnh đề 1, hoán tập E của nó đẳng cấu với $\mathbf{C}$ trong trường hợp b), và với $\mathbf{H}$ trong trường hợp c). Hơn nữa, hiển nhiên là E chứa $\mathbf{C}.1_W$, và chứa $\mathbf{C}.\theta$ trong trường hợp c), suy ra mệnh đề.

Với các giả thiết trong mệnh đề, $A_{(\mathbf{C})}$-môđun W được gọi là thuộc kiểu thực, kiểu phức hoặc kiểu quaternion (đối với A) tương ứng trong các trường hợp $a),b)$ hoặc c).

Đối với $K =\mathbf{R}$ hoặc $\mathbf{C}$, ký hiệu $\mathfrak{S}_K(A)$ là tập hợp các lớp của các $A_{(K)}$-môđun đơn hữu hạn chiều trên K. Nhóm $\Gamma =$ Gal($\mathbf{C}/\mathbf{R}$) tác động trên $\mathfrak{S}_{\mathbf{C}}(A)$; hai mệnh đề trước thiết lập một sự tương ứng song ánh giữa $\mathfrak{S}_{\mathbf{R}}(A)$ và tập thương $\mathfrak{S}_{\mathbf{C}}(A)/\Gamma$.

### 2. BIỂU DIỄN CỦA CÁC NHÓM COMPACT

Cho G là một nhóm tôpô compact, và cho $\rho : G\rightarrow \mathbf{G}\mathbf{L}(W)$ là một biểu diễn liên tục của G trên một không gian vectơ phức hữu hạn chiều. Ta sẽ nói rằng $\rho$ là bất khả quy kiểu thực, phức hoặc quaternion nếu điều này đúng đối với $\mathbf{C}^{(G)}$-môđun W (đối với đại số $A =\mathbf{R}^{(G)}$). Cho H là một dạng Hermit xác định dương trên W, bất biến dưới G.

#### Mệnh đề 3 {#lie-ix-a2-prop-3 .statement tag=01IU}

Giả sử rằng $\rho$ là bất khả quy.

a) Biểu diễn $\rho$ có kiểu thực nếu và chỉ nếu tồn tại một dạng song tuyến tính đối xứng khác không B trên W, bất biến dưới G. Trong trường hợp này dạng B là phân ly; tập hợp V gồm các $w\in W$ sao cho $H(w, x) = B(w, x)$ với mọi $x\in W$ là một cấu trúc $\mathbf{R}$ trên W bất biến dưới G.

b) Biểu diễn $\rho$ có kiểu phức nếu và chỉ nếu không tồn tại dạng song tuyến tính khác không nào trên W bất biến dưới G.

c) Biểu diễn $\rho$ có kiểu quaternion nếu và chỉ nếu tồn tại một dạng song tuyến tính phản xứng khác không trên W, bất biến dưới G; một dạng như vậy tất yếu là phân ly.

Với $\theta \in$ Hom$_{\mathbf{C}^{(G)}}(W,W)$ và $x, y\in W$, đặt $B_{\theta}(x, y) = H(\theta x, y)$. Khi đó $B_{\theta}$ là một dạng song tuyến tính trên W, bất biến dưới G, và phân ly nếu $\theta$ khác không. Ký hiệu bởi $\mathscr{B}(W)^G$ không gian các dạng song tuyến tính trên W bất biến dưới G; ánh xạ $\theta  \rightarrow B_{\theta}$ từ Hom$_{\mathbf{C}^{(G)}}(W,W)$ vào $\mathscr{B}(W)^G$ là một đẳng cấu của các $\mathbf{C}$-không gian vectơ. Điều này, đặc biệt, kéo theo mệnh đề b).

Cho $\theta$ là một $\mathbf{C}^{(G)}$-đẳng cấu từ W đến $\overline{W}$ sao cho $\theta \circ \theta =\alpha_W$, với $\alpha \in  \{-1,+1\}$ (Mệnh đề 2); vì $\mathscr{B}(W)^G$ có chiều bằng 1, nên tồn tại $\varepsilon \in \mathbf{C}$ sao cho

$B_{\theta}(y, x) =\varepsilon B_{\theta}(x, y)$ với mọi $x, y$ trong $W$.

Lặp lại, ta được $B_{\theta}(y, x) =\varepsilon B_{\theta}(x, y) =\varepsilon^2B_{\theta}(y, x)$, do đó $\varepsilon^2$ = 1 và $\varepsilon \in  \{-1,+1\}$. Hơn nữa, với $x$ trong W,

$$
H(\theta x, \theta x) = B_{\theta}(x, \theta x) =\varepsilon B_{\theta}(\theta x, x) =\varepsilon H(\theta \circ \theta (x), x) =\varepsilon \alpha H(x, x)
$$

vì vậy $\varepsilon \alpha  >0$ vì H là dương, nghĩa là $\varepsilon =\alpha$. Các khẳng định a) và c) bây giờ suy ra từ Mệnh đề 2.

Ký hiệu $dg$ là độ đo Haar có tổng khối lượng bằng 1 trên G.

#### Bổ đề 1 {#lie-ix-a2-lem-1 .statement tag=01IV}

Cho $W^G$ là không gian con của W gồm các phần tử bất biến dưới G. Tự đồng cấu $\int_G\rho (g)dg$ của W là một phép chiếu có ảnh là $W^G$, tương thích với các phép toán của G. Đặc biệt, dim $W^G=\int_G$ Tr $\rho (g)dg$.

Đặt $p=\int_G\rho (g)dg$; với $h\in G$,

$$
\rho (h)\circ p=\int_G\rho (hg)dg=\int_G\rho (g)dg=p
$$

và tương tự $p\circ \rho (h) =p$. Do đó, $p$ tương thích với các phép toán của G, và ảnh của nó được chứa trong $W^G$. Nếu $w\in W^G$, ta có $p(w) =\int_G\rho (g)w dg=w$, do đó bổ đề được chứng minh.

#### Bổ đề 2 {#lie-ix-a2-lem-2 .statement tag=01IW}

Cho $u$ là một tự đồng cấu của một không gian vectơ hữu hạn chiều E trên một trường K. Khi đó

Tr $u^2=$ Tr $\mathbf{S}^2(u)-$ Tr $\wedge \wedge^2(u)$.

Cho $\chi_u(X) =\prod_{i=1}^n(X-\alpha_i)$ là một phân tích của đa thức đặc trưng của $u$ thành các thừa số tuyến tính trong một mở rộng thích hợp của K. Ta có Tr $u^2=\sum_i\alpha^2_i$, Tr $\wedge \wedge^2(u) =\sum_{i<j}\alpha_i\alpha_j$, Tr $\mathbf{S}^2(u) =\sum_{i\leq j}\alpha_i\alpha_j$ (x. Đại số, Ch. VII, §5, no. 5, Hệ quả 3), do đó suy ra kết quả.

#### Mệnh đề 4 {#lie-ix-a2-prop-4 .statement tag=01IX}

Giả sử rằng $\rho$ là bất khả quy. Khi đó, $\rho$ thuộc kiểu thực (resp. phức, resp. quaternionic) nếu và chỉ nếu tích phân $\int_G$ Tr$\rho (g^2)dg$ bằng 1 (resp. 0, resp. $-1$).

Ký hiệu $\check{\rho}$ là biểu diễn phản biến của $\rho$ trên $W^*$ (được định nghĩa bởi $\check{\rho}(g) =^t\rho (g^{-1})$). Áp dụng Bổ đề 2 cho $\check{\rho}(g)$ và lấy tích phân trên G thu được

$\int_G$ Tr$\rho (g^2)dg=\int_G$ Tr $^t\rho (g^{-2})dg=\int_G$ Tr $\mathbf{S}^2( \check{\rho}(g))dg-\int_G$ Tr $\wedge \wedge^2( \check{\rho}(g))dg$

do đó, theo Bổ đề 1,

$\int_G$ Tr $\rho (g^2)dg=$ dim($\mathbf{S}^2W^*$)$^G-$ dim($\wedge \wedge^2W^*$)$^G$.

Nhưng $\mathbf{S}^2W^*$ (resp. $\wedge \wedge^2W^*$) có thể được đồng nhất với không gian các dạng song tuyến tính đối xứng (resp. phản xứng) trên W. Do đó, mệnh đề được suy ra ngay lập tức từ Mệnh đề 3.
