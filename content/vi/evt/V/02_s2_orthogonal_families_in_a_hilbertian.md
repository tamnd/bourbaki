---
book: evt
book_title: Topological Vector Spaces
chapter: V
chapter_title: HILBERTIAN SPACES (ELEMENTARY THEORY)
section: 2
section_title: Orthogonal families in a hilbertian space
lang: vi
source: evt-i-v
book_pages: TVS V.17-TVS V.25, TVS V.70-TVS V.73
pdf_pages: 0275-0283, 0328-0331
extraction: ocr
subsections:
    - "no": 1
      title: External hilbertian sum of hilbertian spaces
      page: 17
      pdf_page: 275
    - "no": 2
      title: Hilbertian sum of orthogonal subspaces of a hilbertian space
      page: 18
      pdf_page: 276
    - "no": 3
      title: Orthonormal families
      page: 21
      pdf_page: 279
    - "no": 4
      title: Orthonormalisation
      page: 23
      pdf_page: 281
statements: 23
exercises: 16
content_sha256: 0668d86c47c676e2328cdf4b63a844f24bfd22c3c2158c28134f6b55fd187b3a
translated_from: content/en/evt/V/02_s2_orthogonal_families_in_a_hilbertian.md
source_content_sha256: 13b2d06e3e8c8872d9e3f91186077fdb068739451dbc3faf9b1d59434350b643
translation_model: gpt-5-6, gpt-5.4-mini, gpt-5-6-mini
translation_run: translate-vi-b27c62a3
glossary_version: 34
glossary_terms_sha256: 813b82c43d13a21606a63db86dcefd5f391fc498e2f45b54dbdca529840a03a4
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 2. CÁC HỌ TRỰC GIAO TRONG MỘT KHÔNG GIAN HILBERT

### 1. Tổng Hilbert ngoài của các không gian Hilbert

#### Mệnh đề 1 {#evt-v-s2-prop-1 .statement}

*Cho $(E_i)_{i \in I}$ là một họ các không gian Hilbert, P là không gian vectơ tích $\prod_{i \in I} E_i$ và E là tập con của P gồm tất cả các họ $x = (x_i)_{i \in I}$ sao cho $\sum_{i \in I} \|x_i\|^2$ là hữu hạn.

a) E là một không gian con vectơ của P.

b) Với mọi $x = (x_i)_{i \in I}$ và $y = (y_i)_{i \in I}$ trong E, họ $(\langle x_i|y_i \rangle)_{i \in I}$ là khả tổng. Nếu đặt $\langle x|y \rangle = \sum_{i \in I} \langle x_i|y_i \rangle$, ta định nghĩa một dạng Hermit dương tách được trên E.

c) Đối với tích vô hướng được định nghĩa như vậy, E là một không gian Hilbert; tổng trực tiếp S của các $E_i$ là trù mật trong E.

Với $x = (x_i)_{i \in I}$ và $y = (y_i)_{i \in I}$ trong E, ta có
$$
\|x_i + y_i\|^2 \leq 2(\|x_i\|^2 + \|y_i\|^2),
$$
suy ra $x + y = (x_i + y_i)_{i \in I}$ thuộc E. Điều này chứng minh a).

Theo bất đẳng thức Cauchy-Schwarz, ta có
$$
|\langle x_i|y_i \rangle| \leq \|x_i\| \cdot \|y_i\| \leq \frac{1}{2}(\|x_i\|^2 + \|y_i\|^2)
$$
suy ra $\sum_{i \in I} |\langle x_i|y_i \rangle| < +\infty$. Nếu $x \neq 0$, ta có $\langle x|x \rangle = \sum_{i \in I} \|x_i\|^2 > 0$, do đó mệnh đề b) được suy ra.

Ta nhắc lại rằng S là không gian con của P gồm tất cả các họ $x = (x_i)_{i \in I}$ sao cho tập hợp tất cả các $i \in I$ mà $x_i \neq 0$ là hữu hạn. Suy ra ngay lập tức rằng S trù mật trong E; do đó còn phải chứng minh rằng E là *đầy đủ* đối với tôpô $\mathcal{T}_1$ nhận được bởi chuẩn $\|x\| = \langle x|x \rangle^{1/2}$. Gọi $\mathcal{T}_2$ là tôpô cảm sinh trên E bởi tôpô tích trên $\prod_{i \in I} E_i$. Với mọi $r > 0$, gọi $B_r$ là tập hợp tất cả các $x \in E$ sao cho $\|x\| \leq r$. Quan hệ này kéo theo rằng ta có $\sum_{i \in J} \|x_i\|^2 \leq r^2$ với mọi tập con hữu hạn J của I, và do đó $B_r$ là một tập con đóng của $\prod_{i \in I} E_i$, vì vậy cũng đầy đủ. Sự kiện E đầy đủ đối với $\mathcal{T}_1$ giờ đây suy ra từ GT, III, § 3, No. 5, hệ quả 2 cho mệnh đề 10.

#### Định nghĩa 1 {#evt-v-s2-def-1 .statement}

*Cho* $(E_i)_{i \in I}$ *là một họ các không gian Hilbert. Không gian Hilbert E được định nghĩa trong mệnh đề 1 được gọi là tổng Hilbert ngoài của họ* $(E_i)_{i \in I}$ *và được viết là* $\bigoplus_{i \in I} E_i$ *hoặc* $\bigoplus_{i \in I} E_i$^1.

Gọi $f_i$ là ánh xạ từ $E_i$ vào E biến $z \in E_i$ thành một phần tử $(x_k) \in E$ sao cho $x_k = 0$ với mọi $k \neq i$ và $x_i = z$; rõ ràng rằng $f_i$ là một đẳng cấu từ không gian Hilbert $E_i$ lên một không gian con vectơ đóng của E. Ta nói rằng $f_i$ là *ánh xạ chính tắc* từ $E_i$ vào E và nói chung ta đồng nhất $E_i$ với ảnh của nó trong E qua đẳng cấu này. Với quy ước này, $E_i$ và $E_k$ là *trực giao* trong E đối với $i \neq k$, và E là không gian con vectơ đóng sinh bởi hợp của các không gian con $E_i$.

Khi I là hữu hạn, E là tổng trực tiếp của các $E_i$; vì phép chiếu chính tắc từ E lên $E_i$ là liên tục với mọi $i \in I$, E cũng là tổng trực tiếp tôpô của các $E_i$ (GT, III, § 6, No. 2, mệnh đề 2). Nếu $I = \{1, n\}$, ta cũng viết $E_1 \oplus E_2 \oplus ... \oplus E_n$ thay cho $\bigoplus_{i=1}^n E_i$.

#### Ví dụ {#evt-v-s2-n1-exa-1 .statement}

— Cho E là một không gian Hilbert và I là một tập chỉ số. Ký hiệu $\ell^2_E(I)$ là tổng Hilbert ngoài của họ $(E_i)_{i \in I}$, trong đó $E_i = E$ với mọi $i \in I$. Nói cách khác, $\ell^2_E(I)$ là không gian của mọi họ $x = (x_i)_{i \in I}$ gồm các phần tử của E sao cho $\sum_{i \in I} \|x_i\|^2 < +\infty$, được trang bị tích vô hướng $\langle x|y \rangle = \sum_{i \in I} \langle x_i|y_i \rangle$ (không gian các họ các phần tử của E khả tổng bình phương, được chỉ số hóa bởi I). Ta đặt $\ell^2(I) = \ell^2_K(I)$.

### 2. Tổng Hilbert của các không gian con trực giao của một không gian Hilbert

#### Định nghĩa 2 {#evt-v-s2-def-2 .statement}

*Một không gian Hilbert E được gọi là tổng Hilbert của một họ* $(E_i)_{i \in I}$ *các không gian con vectơ đóng của E khi* :

1) *với hai chỉ số phân biệt* $i, k$ *trong I, các không gian con* $E_i$ *và* $E_k$ *trực giao trong* E;
2) *không gian con vectơ đóng sinh bởi hợp của các* $E_i$ *là* E.

1 Cần chú ý không nhầm lẫn ký hiệu này với ký hiệu của tổng trực tiếp « đại số » của các không gian $E_i$ (A, II, § 1, No. 6).

#### Định lý 1 {#evt-v-s2-thm-1 .statement}

— Cho E là một không gian Hilbert là tổng Hilbert của một họ $(E_i)_{i \in I}$ các không gian con vectơ đóng của E. Tồn tại một đẳng cấu $f$ và chỉ một, từ E lên tổng Hilbert ngoài $\bigoplus_{i \in I} E_i = F$ của họ $(E_i)$ sao cho, với mọi $i \in I$, hạn chế của $f$ lên E là ánh xạ chính tắc $f_i$ từ $E_i$ vào F.

Cho $S \subset F$ là tổng trực tiếp « đại số » của các $E_i$, và cho $g$ là ánh xạ tuyến tính $(x_i)_{i \in I} \mapsto \sum_{i \in I} x_i$ từ S vào E. Ta sẽ chứng minh rằng $g$ là một đẳng cấu từ không gian tiền Hilbert S lên không gian con (tiền Hilbert) $g(S)$ của E, được sinh bởi hợp của các $E_i$ : vì, với hai phần tử $x = (x_i)_{i \in I}$, $y = (y_i)_{i \in I}$, ta có

$$
\langle g(x)|g(y) \rangle = \langle \sum_{i \in I} x_i|\sum_{i \in I} y_i \rangle = \sum_{(i,k) \in I \times I} \langle x_i|y_k \rangle .
$$

Nhưng nếu $i \neq k$, $\langle x_i|y_k \rangle = 0$ theo giả thiết, suy ra

$$
\langle g(x)|g(y) \rangle = \sum_{i \in I} \langle x_i|y_i \rangle = \langle x|y \rangle ;
$$

điều này chứng minh mệnh đề của chúng ta. Vì S trù mật trong F và $g(S)$ trù mật trong E, đẳng cấu $g$ được kéo dài thành một đẳng cấu $\overline{g}$ từ F lên E (V, p. 8, hệ quả). Hiển nhiên đẳng cấu nghịch đảo $f$ của $\overline{g}$ là ánh xạ cần tìm; tính duy nhất của nó suy ra từ việc không gian con đóng của E được sinh bởi hợp của các $E_i$ chính là E.

Khi E là tổng Hilbert của một họ $(E_i)_{i \in I}$ các không gian con, ta thường đồng nhất E với tổng Hilbert ngoài F của các $E_i$ nhờ đẳng cấu $f$. Nếu tập I hữu hạn, nói rằng E là tổng Hilbert của họ $(E_i)_{i \in I}$ có nghĩa là các $E_i$ từng đôi một trực giao và không gian vectơ E là tổng trực tiếp của họ $(E_i)_{i \in I}$ các không gian con.

#### Hệ quả 1 {#evt-v-s2-thm-1-cor-1 .statement}

— Cho E là một không gian Hilbert, là tổng Hilbert của một họ $(E_i)_{i \in I}$ các không gian con vectơ đóng của E; với mọi $i \in I$, ký hiệu $p_{E_i}$ là phép chiếu trực giao (V, p. 13) từ E lên $E_i$.

a) Với mọi $x \in E$, họ $(\|p_{E_i}(x)\|^2)_{i \in I}$ khả tổng trong $\mathbf{R}$, họ $(p_{E_i}(x))_{i \in I}$ khả tổng trong E, và ta có

$$
\|x\|^2 = \sum_{i \in I} \|p_{E_i}(x)\|^2 , \quad x = \sum_{i \in I} p_{E_i}(x) .
$$

b) Ngược lại, nếu $(x_i)_{i \in I}$ là một họ các phần tử của E sao cho $x_i \in E_i$ với mọi $i \in I$ và $\sum_{i \in I} \|x_i\|^2 < + \infty$, thì họ này là khả tổng, và tổng $x$ là điểm duy nhất của E sao cho $p_{E_i}(x) = x_i$ với mọi $i \in I$.

c) Với mọi cặp điểm $x, y$ của E, ta có

$$
\langle x|y \rangle = \sum_{i \in I} \langle p_{E_i}(x)|p_{E_i}(y) \rangle .
$$

Các tính chất này thực ra là hiển nhiên đối với tổng hilbert ngoài của các $E_i$, và có thể được chuyển sang E bởi đẳng cấu.

#### Hệ quả 2 {#evt-v-s2-thm-1-cor-2 .statement}

— Cho E là một không gian tiềnhilbert Hausdorff, $(E_i)_{i \in I}$ là một họ các không gian con vectơ đầy đủ của E sao cho, với mọi cặp chỉ số phân biệt $i, k$ trong I, các không gian con $E_i$ và $E_k$ là trực giao. Gọi V là không gian con vectơ đóng của E sinh bởi hợp của các $E_i$. Với mọi $i \in I$, gọi $p_{E_i}$ là phép chiếu trực giao từ E lên $E_i$. Gọi $x \in E$.

1) Ta có $\sum_{i \in I} \|p_{E_i}(x)\|^2 \leq \|x\|^2$.

2) Các điều kiện sau là tương đương : a) $x \in V$; b) $\sum_{i \in I} \|p_{E_i}(x)\|^2 = \|x\|^2$; c) họ $(p_{E_i}(x))_{i \in I}$ là khả tổng trong E, và ta có $x = \sum_{i \in I} p_{E_i}(x)$.

3) Giả sử V là đầy đủ. Khi đó họ $(p_{E_i}(x))_{i \in I}$ là khả tổng trong E, và
$$
p_V(x) = \sum_{i \in I} p_{E_i}(x), \quad \|p_V(x)\|^2 = \sum_{i \in I} \|p_{E_i}(x)\|^2,
$$
trong đó $p_V$ ký hiệu phép chiếu trực giao từ E lên V.

Cho $\hat{E}$ là sự hoàn thành không gian hilbert của E; ta đồng nhất E với một không gian con trù mật của $\hat{E}$; các $E_i$, vì đầy đủ, là các không gian con đóng của $\hat{E}$. Bao đóng $\overline{V}$ của V trong $\hat{E}$ là không gian con vectơ đóng của $\hat{E}$ sinh bởi hợp của các $E_i$, và $V = \overline{V} \cap E$. Không gian $\hat{E}$ là tổng hilbert của các $E_i$ và của không gian con W, phần bù trực giao của $\overline{V}$ trong $\hat{E}$; đặt $x_0 = p_W(x)$ và $x_i = p_{E_i}(x)$ với mọi $i \in I$. Theo hệ quả 1, ta có $\|x\|^2 = \|x_0\|^2 + \sum_{i \in I} \|x_i\|^2$, và $x = x_0 + \sum_{i \in I} x_i$ trong $\hat{E}$. Điều này kéo theo mệnh đề 1), và sự kiện rằng các điều kiện b) và c) của 2) tương đương với điều kiện $x_0 = 0$, do đó tương đương với điều kiện $x \in V$. Cuối cùng, nếu V là đầy đủ, và nếu đặt $x' = p_V(x)$, ta có $x' - x_i = (x - x_i) - (x - p_V(x))$, do đó $x' - x_i$ trực giao với $E_i$, và vì vậy $x_i = p_{E_i}(x')$ với mọi $i \in I$; bây giờ chỉ cần áp dụng tính chất 2) cho vectơ $x'$.

#### Nhận xét {#evt-v-s2-n2-rem-1 .statement}

Cho E là một không gian tiền Hilbert Hausdorff, $(V_i)_{i \in I}$ là một họ các không gian con vectơ của E sao cho với mọi cặp chỉ số phân biệt $i, k$, các không gian con $V_i$ và $V_k$ trực giao với nhau. Khi đó, với mọi $k \in I$, giao của $V_k$ và không gian con vectơ đóng $W_k$ sinh bởi hợp của các $V_i$ với mọi $i \neq k$ bằng $0$ vì nếu $x$ thuộc $V_k$ và đồng thời thuộc $W_k$, thì $x$ trực giao với mọi $V_i$ với $i \neq k$, suy ra trực giao với $W_k$. Đặc biệt, $x$ trực giao với chính nó, nên bằng không.

#### Mệnh đề 2 {#evt-v-s2-prop-2 .statement}

— Cho E là một không gian Hilbert và $(V_\lambda)_{\lambda \in L}$ là một họ các không gian con vectơ đóng của E; với mọi $\lambda \in L$, cho $(W_{\lambda \mu})_{\mu \in M_\lambda}$ là một họ các không gian con vectơ đóng của $V_\lambda$ sao cho $V_\lambda$ là không gian con vectơ đóng sinh bởi hợp của họ này. Để E là tổng Hilbert của họ $(W_{\lambda \mu})_{\lambda \in L, \mu \in M_\lambda}$, cần và đủ rằng E là tổng Hilbert của họ $(V_\lambda)_{\lambda \in L}$ và rằng, với mỗi $\lambda \in L$, $V_\lambda$ là tổng Hilbert của họ $(W_{\lambda \mu})_{\mu \in M_\lambda}$ ("tính kết hợp của tổng Hilbert").

Để chứng minh điều kiện này là cần thiết, chỉ cần thấy rằng $V_\alpha$ và $V_\beta$ trực giao nếu $\alpha \neq \beta$. Thật vậy, mọi phần tử của $W_{\alpha \mu}$ ($\mu \in M_\alpha$) đều trực giao với mọi $W_{\beta v}$ ($v \in M_\beta$), suy ra trực giao với không gian con vectơ đóng $V_\beta$ do chúng sinh ra; cùng một lập luận cho thấy mọi phần tử của $V_\beta$ đều trực giao với $V_\alpha$, vì nó trực giao với mọi $W_{\alpha \mu}$ ($\mu \in M_\alpha$).

Để chứng minh điều kiện này là đủ, chỉ cần kiểm tra rằng, nếu điều kiện ấy được thỏa mãn, thì E bằng không gian con vectơ đóng F sinh bởi hợp của các $W_{\lambda \mu}$ ($\lambda \in L$, μ ∈ M_λ); nhưng, với mỗi $\lambda \in L$, F chứa không gian con vectơ đóng sinh bởi hợp các $W_{\lambda\mu}$ sao cho $\mu \in M_\lambda$, tức là F chứa $V_\lambda$; do đó F là không gian con vectơ đóng sinh bởi hợp của các $V_\lambda$, mà theo giả thiết thì bằng E.

### 3. Các họ trực chuẩn

#### Định nghĩa 3 {#evt-v-s2-def-3 .statement}

Trong một không gian tiền Hilbert, một họ $(e_i)_{i∈I}$ các vectơ được gọi là trực giao nếu $e_i$ và $e_k$ trực giao với nhau với mọi $i \neq k$, và được gọi là trực chuẩn nếu thêm nữa $\|e_i\| = 1$ với mọi $i ∈ I$.

Một tập con S của E sao cho họ do ánh xạ đồng nhất từ S lên chính nó xác định là trực chuẩn được gọi là một tập trực chuẩn. Nếu $(e_i)_{i∈I}$ là một họ trực chuẩn, thì ánh xạ $i \mapsto e_i$ là đơn ánh; khi đó ta có thể nói không phân biệt về một họ trực chuẩn hay một tập trực chuẩn.

Nếu $(e_i)_{i∈I}$ là một họ trực chuẩn, thì các không gian con vectơ một chiều đầy đủ $D_i = Ke_i$ đôi một trực giao. Với mọi $x ∈ E$, phép chiếu trực giao của $x$ lên $D_i$ là $λ_i e_i$ với $⟨e_i|x - λ_i e_i⟩ = 0$, suy ra $⟨e_i|x⟩ = λ_i ⟨e_i|e_i⟩ = λ_i$. Các kết quả của No. 2 áp dụng cho các không gian con $D_i$ suy ra các mệnh đề sau:

#### Mệnh đề 3 {#evt-v-s2-prop-3 .statement}

Trong một không gian tiền Hilbert Hausdorff E, mọi họ trực chuẩn đều độc lập về mặt tôpô.

Ta lưu ý rằng tính chất này suy ra ngay lập tức từ đặc trưng hóa của các họ độc lập tôpô (IV, p. 1 and II, p. 43, cor. 2), do sự đồng nhất của đối ngẫu của E với sự hoàn tất của E hoặc với không gian liên hợp của E tùy theo K bằng R hay C (V, p. 17, Nhận xét).

#### Mệnh đề 4 {#evt-v-s2-prop-4 .statement}

Cho E là một không gian tiền Hilbert Hausdorff, $(e_i)_{i∈I}$ là một họ trực chuẩn trong E, V là không gian con vectơ đóng của E sinh bởi các $e_i$.

1) Với mọi $x ∈ E$, ta có

$$
\sum_{i∈I} |⟨e_i|x⟩|^2 \leq \|x\|^2
$$

(bất đẳng thức Bessel); ở đây tập hợp tất cả các $i ∈ I$ sao cho $⟨e_i|x⟩ \neq 0$ là đếm được. Hơn nữa, các điều kiện sau là tương đương : a) $x ∈ V$; b) $\|x\|^2 = \sum_{i∈I} |⟨e_i|x⟩|^2$; c) họ $⟨e_i|x⟩.e_i$ là khả tổng trong E, và $x = \sum_{i∈I} ⟨e_i|x⟩.e_i$.

2) Nếu V đầy đủ, thì họ tất cả các $⟨e_i|x⟩.e_i$ là khả tổng trong E với mọi $x ∈ E$, và $\sum_{i∈I} ⟨e_i|x⟩.e_i = p_V(x), \sum_{i∈I} |⟨e_i|x⟩|^2 = \|p_V(x)\|^2$.

3) Giả sử V đầy đủ. Với mọi họ $(\lambda_i)_{i∈I}$ của các số vô hướng sao cho $\sum_{i∈I} |\lambda_i|^2 < +∞$, tồn tại duy nhất một điểm $x ∈ V$ sao cho $⟨e_i|x⟩ = \lambda_i$ với mọi $i ∈ I$. Nếu $(\mu_i)_{i∈I}$ là một họ thứ hai các số vô hướng sao cho $\sum_{i∈I} |\mu_i|^2 < +∞$, và nếu $y ∈ V$ sao cho $⟨e_i|y⟩ = \mu_i$ với mọi $i ∈ I$, thì $⟨x|y⟩ = \sum_{i∈I} \overline{\lambda_i} \mu_i$.

#### Mệnh đề 5 {#evt-v-s2-prop-5 .statement}

— Cho $(e_i)_{i \in I}$ là một họ trực chuẩn trong một không gian tiền Hilbert Hausdorff E. Các tính chất sau là tương đương :
a) họ $(e_i)$ là toàn thể ;
b) với mọi $x \in E$, họ $\langle e_i | x \rangle \cdot e_i$ là khả tổng trong E, và ta có $x = \sum_{i \in I} \langle e_i | x \rangle \cdot e_i$;
c) với mọi $x \in E$,

$$
\|x\|^2 = \sum_{i \in I} |\langle e_i | x \rangle|^2
$$

(quan hệ Parseval).

Khi E là một không gian hilbert thì các điều kiện này cũng tương đương với :
d) các quan hệ $\langle e_i | x \rangle = 0$ với mọi $i \in I$ suy ra rằng $x = 0$.

Sự tương đương của các điều kiện a), b), c) suy ra ngay lập tức từ mệnh đề 4. Khi E là một không gian hilbert, sự tương đương của các điều kiện a) và d) suy ra từ hệ quả 1 của V, p. 16.

#### Định nghĩa 4 {#evt-v-s2-def-4 .statement}

— Một họ trực chuẩn và đầy đủ trong một không gian tiền Hilbert Hausdorff E được gọi là một cơ sở trực chuẩn của E.

Một cơ sở trực chuẩn của một không gian tiền Hilbert Hausdorff E cũng là một cơ sở trực chuẩn của phần hoàn thiện của E.

Cho $(e_i)_{i \in I}$ là một cơ sở trực chuẩn của E; với mọi $x \in E$, các số $⟨e_i | x⟩$ được gọi, lạm dụng ngôn ngữ, là các tọa độ của $x$ đối với cơ sở $(e_i)$. Với mọi $x$ và $y$ trong E, ta có

$$
\langle x | y \rangle = \sum_{i \in I} \overline{\langle e_i | x \rangle} \langle e_i | y \rangle .
$$

Một cơ sở trực chuẩn của E nói chung không phải là một cơ sở của E trên trường K theo nghĩa đã định trong A, II, p. 25; để tránh mọi lẫn lộn, ta sẽ luôn nói rằng một cơ sở của một không gian tiền Hilbert E theo nghĩa của chỗ dẫn trên là một cơ sở đại số của E trên K.

Cho E và F là hai không gian tiền Hilbert Hausdorff và $u$ là một ánh xạ tuyến tính liên tục từ E vào F. Cho $(e_i)_{i \in I}$ (tương ứng $(f_j)_{j \in J}$) là một cơ sở trực chuẩn của E (tương ứng F). Đặt

$$
u_{ji} = \langle f_j | u(e_i) \rangle
$$

với $i \in I,\ j \in J$. Họ $(u_{ji})_{(i,j) \in I \times J}$ được gọi là ma trận của $u$ đối với các cơ sở trực chuẩn $(e_i)$ và $(f_j)$. Cho $x \in E$ và $y = u(x)$; nếu ta viết $\xi_i = \langle e_i | x \rangle$ và $\eta_j = \langle f_j | y \rangle$ cho các tọa độ tương ứng của $x$ và $y$, ta được $\eta_j = \sum_{i \in I} u_{ji} \xi_i$ với mọi $j \in J$. Khi $(e_i)$ là một cơ sở đại số của E và $(f_j)$ là một cơ sở đại số của F, định nghĩa của chúng tôi phù hợp với định nghĩa ở A, II, § 10, No. 4.

#### Ví dụ {#evt-v-s2-n3-exa-1 .statement}

Cho E là không gian của mọi hàm liên tục nhận giá trị phức trên $\mathbf{R}$, sao cho $f(x + n) = f(x)$ với $x \in \mathbf{R}$ và $n \in \mathbf{Z}$. Ta gán cho E tích vô hướng được xác định bởi

$$
\langle f | g \rangle = \int_0^1 \overline{f(t)}\ g(t)\ dt .
$$

Khi đó E là một không gian tiền Hilbert Hausdorff, nhưng không đầy đủ. Với mỗi số nguyên $n \in \mathbf{Z}$, cho $e_n(x) \in \mathbf{e}(nx)$. Hiển nhiên họ $(e_n)_{n \in \mathbf{Z}}$ là trực chuẩn trong E. Hơn nữa, tôpô hội tụ đều trên E mịn hơn tôpô suy ra từ chuẩn $\|f\|_2 = \langle f|f \rangle^{1/2}$. Họ $(e_n)_{n \in \mathbf{Z}}$ là toàn thể trong E đối với sự hội tụ đều (GT, X, § 4, No. 4), và *a fortiori* trong không gian tiền Hilbert E. Do đó $(e_n)_{n \in \mathbf{Z}}$ là một cơ sở trực chuẩn của E.

### 4. Trực chuẩn hóa

#### Định lý 2 {#evt-v-s2-thm-2 .statement}

*Mọi tập trực chuẩn L trong một không gian hilbert E đều được chứa trong một cơ sở trực chuẩn B của E.*

Thật vậy, cho $\mathfrak{D}$ là họ tất cả các tập hợp trực chuẩn của E, được sắp thứ tự tuyến tính bởi phép bao hàm; hiển nhiên họ này có đặc trưng hữu hạn (S, III, § 4, No. 5). Do đó tồn tại một họ *cực đại* B trong $\mathfrak{D}$ chứa L, theo đl. 1 của S, III, § 4, No. 5. Còn phải chứng minh rằng B là một tập hợp toàn phần. Nếu không, sẽ tồn tại một vectơ $y \neq 0$ trực giao với mọi vectơ của B (V, p. 22, mệnh đề 5), và nhân y với một vô hướng thích hợp, ta có thể giả sử rằng $\|y\| = 1$; khi đó, $B \cup \{y\}$ sẽ là một tập hợp trực chuẩn khác B và chứa B; điều này mâu thuẫn với định nghĩa của B; vậy là định lý.

#### Hệ quả 1 {#evt-v-s2-thm-2-cor-1 .statement}

*Trong mọi không gian Hilbert, tồn tại một cơ sở trực chuẩn.*

Chỉ cần áp dụng định lý 2 cho trường hợp $L = \varnothing$.

#### Hệ quả 2 {#evt-v-s2-thm-2-cor-2 .statement}

*Mọi không gian Hilbert đều đẳng cấu với một không gian $\ell^2(I)$.*

Chính xác hơn, cho $(e_i)_{i \in I}$ là một cơ sở trực chuẩn của một không gian Hilbert E. Theo các mệnh đề 4 (V, p. 21) và 5 (V, p. 22), ánh xạ $\phi$ được xác định bởi
$$
\phi(x) = (\langle e_i|x \rangle)_{i \in I}
$$
là một đẳng cấu giữa các không gian Hilbert từ E lên $\ell^2(I)$. Đẳng cấu nghịch đảo $\psi$ được xác định bởi
$$
\psi((\lambda_i)_{i \in I}) = \sum_{i \in I} \lambda_i e_i .
$$

#### Mệnh đề 6 {#evt-v-s2-prop-6 .statement}

*Cho E là một không gian tiền Hilbert Hausdorff, và cho $(a_n)_{n \in I}$ (I là một khoảng của $\mathbf{N}$ có gốc 1) là một họ đếm được (hữu hạn hoặc không) độc lập các vectơ của E. Tồn tại một họ trực chuẩn $(e_n)_{n \in I}$, và chỉ một, trong E, có các tính chất sau:

1) với mọi số nguyên $p \in I$, không gian con vectơ của E do $e_1, e_2, ..., e_p$ sinh ra trùng với không gian con vectơ của E do $a_1, a_2, ..., a_p$ sinh ra;
2) với mọi số nguyên $p \in I$, số $\langle a_p|e_p \rangle$ là thực và $> 0$.

Thật vậy, cho $V_n$ là không gian con (có chiều n) do $a_1, a_2, ..., a_n$ sinh ra. Nếu $n + 1 \in I$ và $b_{n+1} = a_{n+1} - p_{V_n}(a_{n+1})$ (trong đó $p_{V_n}$ là phép chiếu trực giao lên không gian con đầy đủ $V_n$), thì đường thẳng $K b_{n+1}$ là phần trực giao của $V_n$ trong $V_{n+1}$. Nếu các $e_n$ thỏa mãn điều kiện 1) của mệnh đề, ta phải có $e_{n+1} = \lambda b_{n+1}$; điều kiện $\|e_{n+1}\| = 1$ khi đó suy ra $|\lambda|^2 \|b_{n+1}\|^2 = 1$ và điều kiện $\langle a_{n+1}|e_{n+1} \rangle > 0$ suy ra $\lambda \langle a_{n+1}|b_{n+1} \rangle > 0$; điều này xác định hoàn toàn $\lambda$, và ta đã chứng minh rằng ta có thể xác định, bằng quy nạp, một họ trực chuẩn $(e_n)_{n \in I}$, và chỉ một, sao cho thỏa mãn các điều kiện 1) và 2) của mệnh đề.

Dãy $(e_n)_{n \in I}$ được gọi là thu được bằng phép *trực chuẩn hóa* từ họ độc lập $(a_n)_{n \in I}$. Rõ ràng không gian con vectơ do họ $(e_n)$ sinh ra trùng với không gian con vectơ do họ $(a_n)$ sinh ra. Đặc biệt, nếu $(a_n)$ là một dãy toàn phần, thì $(e_n)$ cũng vậy, và khi đó nó là một cơ sở trực chuẩn của E; do đó ta có:

#### Hệ quả {#evt-v-s2-n4-cor-1 .statement}

*Trong mọi không gian tiền Hilbert Hausdorff E thỏa mãn tiên đề đếm được thứ nhất, tồn tại một cơ sở trực chuẩn đếm được.*

Nếu E thỏa mãn tiên đề đếm được thứ nhất, thì tồn tại một dãy toàn phần trong E, và ta luôn luôn có thể trích ra một họ độc lập toàn phần từ một dãy như vậy (A, II, § 7, No. 1, đl. 2).

Ta có thể nêu các ví dụ về những không gian tiền Hilbert Hausdorff không có cơ sở trực chuẩn nào (V, p. 70, bài tập 2).
*Ví dụ.* — Cho I là khoảng $(-1, 1)$ của $\mathbf{R}$ và E là không gian vectơ các hàm liên tục nhận giá trị thực trên I. Cho $x$ ký hiệu đơn ánh chính tắc từ I vào $\mathbf{R}$, xét như một phần tử của E. Theo định lý Stone-Weierstrass, dãy $(x^n)_{n \in \mathbf{N}}$ là toàn phần trong E đối với tôpô hội tụ đều GT, X, § 4, No. 2).
Xét E như một không gian tiền Hilbert Hausdorff thực trong đó tích vô hướng được cho bởi
$$
\langle f | g \rangle = \int_{-1}^{1} f(t) \, g(t) \, dt .
$$
Khi đó dãy $(x^n)_{n \in \mathbf{N}}$ là toàn phần trong không gian tiền Hilbert E. Cho $(\Pi_n)_{n \in \mathbf{N}}$ là dãy thu được bằng phép trực chuẩn hóa của dãy $(x^n)_{n \in \mathbf{N}}$. Ta có thể chứng minh rằng $\Pi_n = (n + \frac{1}{2})^{1/2} P_n$, trong đó đa thức Legendre $P_n$ được xác định bởi
$$
P_n(x) = \frac{1}{2^n n!} \left( \frac{d}{dx} \right)^n (x^2 - 1)^n .
$$

#### Mệnh đề 7 {#evt-v-s2-prop-7 .statement}

*Trong một không gian Hilbert E, hai cơ sở trực chuẩn là tương đương lực lượng.*

Let B và C là hai cơ sở trực chuẩn của E. Trường hợp một trong hai tập B, C hữu hạn là tầm thường, vì một cơ sở trực chuẩn hữu hạn là một cơ sở đại số của không gian. Vì vậy giả sử rằng B và C đều vô hạn. Với mọi $x \in B$, gọi $C_x$ là tập con của C gồm tất cả các $y \in C$ sao cho $\langle x | y \rangle \neq 0$. Tập $C_x$ là đếm được (V, p. 21, mệnh đề 4). Với mọi $y \in C$, tồn tại $x \in B$ sao cho $y \in C_x$, vì B là một cơ sở trực chuẩn và $y \neq 0$; nói cách khác C là hợp của các tập đếm được $C_x$ khi $x$ chạy trong B. Do đó lực lượng của C nhỏ hơn lực lượng của $\mathbf{N} \times B$, suy ra nhỏ hơn lực lượng của B (S, III, § 6, No. 3, hệ quả 4); tương tự, lực lượng của B nhỏ hơn lực lượng của C; điều này hoàn tất chứng minh.

Lực lượng của một cơ sở trực chuẩn tùy ý của một không gian Hilbert E được gọi là *chiều Hilbert* của E.

#### Hệ quả 1 {#evt-v-s2-prop-7-cor-1 .statement}

*Cho hai cơ sở trực chuẩn trong một không gian Hilbert E, tồn tại một tự đẳng cấu của E biến cơ sở thứ nhất thành cơ sở thứ hai.*

#### Hệ quả 2 {#evt-v-s2-prop-7-cor-2 .statement}

— Để cho các không gian Hilbert $\ell^2(I)$ và $\ell^2(J)$ đẳng cấu với nhau, điều kiện cần và đủ là I và J là hai tập có cùng lực lượng.

### Bài tập {#evt-v-s2-exercises}

Xem [các bài tập cho § 2](exercises/s2/).
