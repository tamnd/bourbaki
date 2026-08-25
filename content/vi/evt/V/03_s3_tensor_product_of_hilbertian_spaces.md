---
book: evt
book_title: Topological Vector Spaces
chapter: V
chapter_title: HILBERTIAN SPACES (ELEMENTARY THEORY)
section: 3
section_title: Tensor product of hilbertian spaces
lang: vi
source: evt-i-v
book_pages: TVS V.25-TVS V.37
pdf_pages: 0283-0295, 0331-0368
extraction: ocr
subsections:
    - "no": 1
      title: Tensor product of prehilbertian spaces
      page: 25
      pdf_page: 283
    - "no": 2
      title: Hilbertian tensor product of hilbertian spaces
      page: 28
      pdf_page: 286
    - "no": 3
      title: Symmetric hilbertian powers
      page: 29
      pdf_page: 287
    - "no": 4
      title: Exterior hilbertian powers
      page: 33
      pdf_page: 291
    - "no": 5
      title: Exterior multiplication
      page: 35
      pdf_page: 293
statements: 20
exercises: 23
content_sha256: 8b99214f344288c753497fe643ac500d8dab7dcd03e408a489dac611530937df
translated_from: content/en/evt/V/03_s3_tensor_product_of_hilbertian_spaces.md
source_content_sha256: c097511d44f50c645d7fcf09bcd4d4b22d00be91e561c77b8ca07d794d412668
translation_model: gpt-5-6-mini, gpt-5.4-mini, gpt-5-6
translation_run: translate-vi-5b9a90dc
glossary_version: 34
glossary_terms_sha256: c2cc2596539425d7902d84d0208604cac76f3efe95aae5fccd392d4a62dbde9f
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 3. TÍCH TENXƠ CỦA CÁC KHÔNG GIAN HILBERT

### 1. Tích tenxơ của các không gian tiền Hilbert

Cho $ E_1 $ và $ E_2 $ là hai không gian tiền Hilbert và cho $ F = E_1 \otimes E_2 $ là tích tenxơ của các không gian vectơ $ E_1 $ và $ E_2 $. Cho $ x_1 \in E_1 $ và $ x_2 \in E_2 $; vì ánh xạ $ (y_1, y_2) \mapsto \langle x_1 | y_1 \rangle \langle x_2 | y_2 \rangle $ từ $ E_1 \times E_2 $ vào K là song tuyến tính, tồn tại một dạng tuyến tính $ \phi_{x_1, x_2} $ trên $ E_1 \otimes E_2 $ sao cho
$$
\phi_{x_1, x_2}(y_1 \otimes y_2) = \langle x_1 | y_1 \rangle \langle x_2 | y_2 \rangle
$$
với $ y_1 \in E_1 $ và $ y_2 \in E_2 $. Cho $ z \in F $. Ánh xạ $ (x_1, x_2) \mapsto \overline{\phi_{x_1, x_2}(z)} $ từ $ E_1 \times E_2 $ vào K là song tuyến tính; điều này có thể thấy được bằng cách viết $ z $ dưới dạng $ z = \sum_{i=1}^n y_{i,1} \otimes y_{i,2} $ với $ y_{i,1} \in E_1 $ và $ y_{i,2} \in E_2 $ với $ 1 \leq i \leq n $. Khi đó tồn tại một dạng tuyến tính $ \psi_z $ trên $ F = E_1 \otimes E_2 $ sao cho
$$
\psi_z(x_1 \otimes x_2) = \overline{\phi_{x_1, x_2}(z)} \quad (x_1 \in E_1, x_2 \in E_2).
$$
Ta đặt $ \Phi(z, t) = \psi_z(t) $ với $ z, t $ trong F. Ta thấy ngay lập tức rằng $ \Phi $ là một dạng nửa tuyến tính trên $ E_1 \otimes E_2 $ được đặc trưng bởi
$$
\Phi(x_1 \otimes x_2, y_1 \otimes y_2) = \langle x_1 | y_1 \rangle \langle x_2 | y_2 \rangle
$$
(xem A, IX, § 1, No. 11).

#### Mệnh đề 1 {#evt-v-s3-prop-1 .statement}

— Dạng nửa tuyến tính $ \Phi $ trên $ E_1 \otimes E_2 $ là Hermit và dương, do đó gán cấu trúc của một không gian tiền Hilbert cho $ E_1 \otimes E_2 $. Không gian này là Hausdorff nếu $ E_1 $ và $ E_2 $ là Hausdorff.

Công thức $ \Phi(z, t) = \overline{\Phi(t, z)} $ suy ra từ (3) khi $ z = x_1 \otimes x_2 $ và $ t = y_1 \otimes y_2 $. Trường hợp tổng quát thu được bằng tính tuyến tính, do đó $ \Phi $ là Hermit.

Giả sử $ E_1 $ và $ E_2 $ là Hausdorff; ta sẽ chứng minh rằng dạng Hermit $ \Phi $ là dương và tách. Cho $ z = \sum_{i=1}^n x_i \otimes y_i $ là một phần tử khác không của $ F = E_1 \otimes E_2 $. Cho $ (e_1, ..., e_n) $ là một cơ sở trực chuẩn của không gian con của $ E_1 $ sinh bởi $ x_1, ..., x_n $ (V, p. 23, cor. 1). Tồn tại các phần tử $ f_1, ..., f_m $ trong $ E_2 $, không phải tất cả đều không, sao cho $ z = \sum_{i=1}^n e_i \otimes f_i $, do đó
$$
\Phi(z, z) = \sum_{i,j=1}^m \Phi(e_i \otimes f_i, e_j \otimes f_j)
$$
$$
= \sum_{i,j} \langle e_i | e_j \rangle \langle f_i | f_j \rangle = \sum_{i=1}^m \| f_i \|^2 > 0.
$$

Trong trường hợp tổng quát, bây giờ ta chứng minh rằng $ \Phi $ là dương. Cho $ \tilde{E}_i $ là không gian prehilbert Hausdorff liên kết với $ E_i $ và cho $ \pi_i $ là ánh xạ chính tắc từ $ E_i $ lên $ \tilde{E}_i $ ($ i = 1, 2 $). Đặt $ \pi = \pi_1 \otimes \pi_2 $. Cho $ \tilde{\Phi} $ là dạng Hermit trên $ \tilde{E}_1 \otimes \tilde{E}_2 $ được xây dựng theo cùng cách như $ \Phi $. Ta có
$$
\Phi(z, t) = \Phi(\pi(z), \pi(t)) \quad (z \in F, \ t \in F),
$$
và vì $ \tilde{\Phi} $ là dương nên $ \Phi $ cũng là dương.

Không gian prehilbert được định nghĩa trong mệnh đề 1 được gọi là *tích tenxơ của các không gian prehilbert* $ E_1 $ và $ E_2 $ và được viết là $ E_1 \otimes E_2 $. Từ nay về sau ta sẽ viết $ \langle z|t \rangle $ cho $ \Phi(z, t) $, và do đó theo định nghĩa
$$
\langle x_1 \otimes x_2 | y_1 \otimes y_2 \rangle = \langle x_1 | y_1 \rangle \langle x_2 | y_2 \rangle;
$$
ta cũng sẽ viết $ \|z\|_2 $ hoặc $ \|z\| $ cho $ \langle z|z \rangle^{1/2} $. Từ (4), ta được
$$
\|x_1 \otimes x_2\|_2 = \|x_1\| \cdot \|x_2\|,
$$
suy ra ánh xạ song tuyến tính $ (x_1, x_2) \mapsto x_1 \otimes x_2 $ từ $ E_1 \times E_2 $ vào $ E_1 \otimes E_2 $ là liên tục.

Với $ i = 1, 2 $ cho $ F_i $ là một không gian con vectơ của $ E_i $, được trang bị cấu trúc prehilbert cảm sinh. Khi đó $ F_1 \otimes F_2 $ có thể được đồng nhất với một không gian con vectơ của $ E_1 \otimes E_2 $ (A, II, § 7, No. 7). Công thức (4) chỉ ra rằng $ F_1 \otimes F_2 $ với cấu trúc không gian prehilbert cảm sinh bởi cấu trúc của $ E_1 \otimes_2 E_2 $, chính là $ F_1 \otimes_2 F_2 $. Từ nay về sau ta sẽ đồng nhất $ F_1 \otimes_2 F_2 $ với một không gian con prehilbert của $ E_1 \otimes_2 E_2 $.

#### Mệnh đề 2 {#evt-v-s3-prop-2 .statement}

*Với $ i = 1, 2 $, cho $ E_i $ và $ F_i $ là hai không gian prehilbert Hausdorff và cho $ u_i \in \mathcal{L}(E_i; F_i) $. Ánh xạ tuyến tính $ u_1 \otimes u_2 $ từ $ E_1 \otimes_2 E_2 $ vào $ F_1 \otimes_2 F_2 $ là liên tục và ta có*
$$
\|u_1 \otimes u_2\| = \|u_1\| \cdot \|u_2\|.
$$

Xét dạng Hermit dương trên $ E_1 $ cho bởi
$$
f(x_1, y_1) = \|u_1\|^2 \langle x_1 | y_1 \rangle - \langle u_1(x_1) | u_1(y_1) \rangle.
$$

Nhờ Mệnh đề 1 (V, p. 25), tồn tại một dạng Hermit dương $ \Phi $ trên $ E_1 \otimes E_2 $ sao cho
$$
\Phi(x_1 \otimes x_2, y_1 \otimes y_2) = f(x_1, y_1) \langle x_2 | y_2 \rangle =
$$
$$
= \|u_1\|^2 \langle x_1 \otimes x_2 | y_1 \otimes y_2 \rangle - \langle (u_1 \otimes 1)(x_1 \otimes x_2) | (u_1 \otimes 1)(y_1 \otimes y_2) \rangle
$$
với $ x_1, y_1 $ trong $ E_1 $ và $ x_2, y_2 $ trong $ E_2 $. Theo tính tuyến tính ta có
$$
\Phi(z, t) = \|u_1\|^2 \langle z|t \rangle - \langle (u_1 \otimes 1)(z) | (u_1 \otimes 1)(t) \rangle
$$
với $ z, t $ trong $ E_1 \otimes E_2 $. Vì $ \Phi $ là dương, ta được $ \Phi(z, z) \geq 0 $, tức là $ \|(u_1 \otimes 1).z\|_2 $

$$
\leq \|u_1\| \cdot \|z\|_2 \text{ cho } z \in E_1 \otimes_2 E_2, \text{ hay } \|u_1 \otimes 1\| \leq \|u_1\|. \text{ Tương tự, ta chứng minh bất đẳng thức } \|1 \otimes u_2\| \leq \|u_2\|, \text{ và vì } u_1 \otimes u_2 = (u_1 \otimes 1) \circ (1 \otimes u_2), \text{ ta được}
$$
$$
\|u_1 \otimes u_2\| \leq \|u_1\| \cdot \|u_2\|.
$$
Mặt khác,
$$
\|u_1\| \cdot \|u_2\| = \sup_{\|x_1\| \leq 1, \|x_2\| \leq 1} \|u_1(x_1)\| \cdot \|u_2(x_2)\|
$$
$$
= \sup_{\|x_1\| \leq 1, \|x_2\| \leq 1} \|(u_1 \otimes u_2)(x_1 \otimes x_2)\|_2 \leq \|u_1 \otimes u_2\|.
$$
Điều này hoàn tất chứng minh của mệnh đề 2. Q.E.D.

Cho $E_1, ..., E_n$ là các không gian tiền Hilbert ($n \geq 2$). Ta định nghĩa tích tenxơ $E_1 \otimes_2 ... \otimes_2 E_n$ (còn ký hiệu là $\bigotimes_{i=1}^n E_i$) bằng quy nạp, bởi
$$
E_1 \otimes_2 ... \otimes_2 E_n = (E_1 \otimes_2 ... \otimes_2 E_{n-1}) \otimes_2 E_n.
$$
Do đó, theo định nghĩa của tích vô hướng, ta có
$$
\langle x_1 \otimes ... \otimes x_n | y_1 \otimes ... \otimes y_n \rangle = \prod_{i=1}^n \langle x_i | y_i \rangle,
$$
và nói riêng $^1$
$$
\|x_1 \otimes ... \otimes x_n\|_2 = \|x_1\| \cdots \|x_n\|,
$$
với $x_i, y_i$ trong $E_i$ ($1 \leq i \leq n$). Nếu các $E_i$ là Hausdorff, thì $E_1 \otimes_2 ... \otimes_2 E_n$ cũng là Hausdorff.

Cho $F_1, ..., F_n$ là các không gian tiền Hilbert và $u_i \in \mathcal{L}(E_i; F_i)$ với $1 \leq i \leq n$. Bằng quy nạp theo $n$, mệnh đề 2 suy ra rằng $u_1 \otimes ... \otimes u_n$ là một ánh xạ tuyến tính liên tục từ $E_1 \otimes_2 ... \otimes_2 E_n$ vào $F_1 \otimes_2 ... \otimes_2 F_n$ và rằng
$$
\|u_1 \otimes ... \otimes u_n\| = \|u_1\| \cdots \|u_n\|.
$$
Cho $\sigma \in S_n$ là một phép hoán vị của tập hợp $\{1, 2, ..., n\}$. Nhờ (6), ánh xạ tuyến tính $p_\sigma$ từ $E_1 \otimes_2 ... \otimes_2 E_n$ lên $E_{\sigma^{-1}(1)} \otimes_2 ... \otimes_2 E_{\sigma^{-1}(n)}$ được đặc trưng bởi
$$
p_\sigma(x_1 \otimes ... \otimes x_n) = x_{\sigma^{-1}(1)} \otimes ... \otimes x_{\sigma^{-1}(n)}
$$
là một đẳng cấu giữa các không gian tiền Hilbert ("tính giao hoán của tích tenxơ").

Tương tự, xét một phân hoạch của $\{1, 2, ..., n\}$ thành $m$ khoảng liên tiếp $I_1, ..., I_n$ với $I_k = [a_k, a_{k+1} - 1]$ với $1 \leq k \leq m$. Đặt
$$
F_k = \bigotimes_{i=a_k}^{a_{k+1}-1} E_i \quad (1 \leq k \leq m).
$$

$^1$ Ở đây một lần nữa ta đặt $\|z\|_2 = \langle z|z \rangle^{1/2}$ với $z$ trong $E_1 \otimes_2 ... \otimes_2 E_n$.

Đẳng cấu chính tắc từ $ F_1 \otimes ... \otimes F_m $ lên $ E_1 \otimes ... \otimes E_n $ biến $ \bigotimes_{k=1}^{m} \bigotimes_{i=a_k}^{a_{k+1}-1} x_i $ thành $ x_1 \otimes ... \otimes x_n $ (A, II, § 3, No. 9) là một đẳng cấu của không gian tiền Hilbert (« tính kết hợp của tích tenxơ »).

### 2. Tích tenxơ Hilbert của các không gian Hilbert

#### Định nghĩa 1 {#evt-v-s3-def-1 .statement}

Cho $ E_1, ..., E_n $ là các không gian hilbert. *Phép hoàn thiện của không gian tiền hilbert Hausdorff* $ E_1 \hat{\otimes}_2 ... \hat{\otimes}_2 E_n $ *được gọi là* tích tenxơ hilbert của các $ E_i $ và được ký hiệu bởi $ E_1 \hat{\otimes}_2 ... \hat{\otimes}_2 E_n $ (hoặc $ \hat{\otimes}_{2 \atop 1 \leq i \leq n} E_i $).

Cho $ F_1, ..., F_n $ là các không gian hilbert và $ u_i \in \mathcal{L}(E_i, F_i) $ với $ 1 \leq i \leq n $. Khi đó ánh xạ tuyến tính liên tục $ u_1 \otimes ... \otimes u_n $ mở rộng thành một ánh xạ tuyến tính liên tục $ u_1 \hat{\otimes}_2 ... \hat{\otimes}_2 u_n $ từ $ E_1 \hat{\otimes}_2 ... \hat{\otimes}_2 E_n $ vào $ F_1 \hat{\otimes}_2 ... \hat{\otimes}_2 F_n $. Ta có

$$
\|u_1 \hat{\otimes}_2 ... \hat{\otimes}_2 u_n\| = \|u_1\| ... \|u_n\|
$$

theo công thức (8) của V, p. 27. Hơn nữa, nếu $ 1_E $ ký hiệu ánh xạ đồng nhất của một không gian hilbert bất kỳ $ E $, ta có

$$
1_{E_1} \hat{\otimes}_2 ... \hat{\otimes}_2 1_{E_n} = 1_E \quad \text{với} \quad E = E_1 \hat{\otimes}_2 ... \hat{\otimes}_2 E_n .
$$

Cuối cùng, nếu $ G_1, ..., G_n $ là các không gian hilbert và $ v_i \in \mathcal{L}(F_i; G_i) $ với $ 1 \leq i \leq n $, ta được

$$
(v_1 \circ u_1) \hat{\otimes}_2 ... \hat{\otimes}_2 (v_n \circ u_n) = (v_1 \hat{\otimes}_2 ... \hat{\otimes}_2 v_n) \circ (u_1 \hat{\otimes}_2 ... \hat{\otimes}_2 u_n) .
$$

Ta để cho người đọc nhiệm vụ phát biểu « tính giao hoán » và « tính kết hợp » của tích tenxơ hilbert, tương tự như điều đã nói ở trên đối với các không gian tiền hilbert.

#### Nhận xét {#evt-v-s3-n2-rem-1 .statement}

Cho $ E_1, ..., E_n $ là các không gian tiền hilbert Hausdorff, và $ \hat{E}_1, ..., \hat{E}_n $ là các phần hoàn thiện tương ứng của chúng. Khi đó $ E_1 \otimes_2 ... \otimes_2 E_n $ là một không gian con tiền hilbert của $ \hat{E}_1 \otimes_2 ... \otimes_2 \hat{E}_n $. Vì ánh xạ $ (x_1, ..., x_n) \mapsto x_1 \otimes ... \otimes x_n $ từ $ \hat{E}_1 \times ... \times \hat{E}_n $ vào $ \hat{E}_1 \otimes_2 ... \otimes_2 \hat{E}_n $ là liên tục, nên $ E_1 \otimes_2 ... \otimes_2 E_n $ là trù mật trong $ \hat{E}_1 \otimes_2 ... \otimes_2 \hat{E}_n $. *A fortiori* phần hoàn thiện của $ E_1 \otimes_2 ... \otimes_2 E_n $ chính xác là không gian hilbert $ \hat{E}_1 \hat{\otimes}_2 ... \hat{\otimes}_2 \hat{E}_n $. Phần hoàn thiện này đôi khi được viết đơn giản là $ E_1 \hat{\otimes}_2 ... \hat{\otimes}_2 E_n $ (hoặc $ \hat{\otimes}_{2 \atop 1 \leq i \leq n} E_i $).

#### Mệnh đề 3 {#evt-v-s3-prop-3 .statement}

Cho $ E_1, ..., E_n $ là các không gian hilbert. Giả sử rằng với $ 1 \leq i \leq n $ không gian $ E_i $ là một tổng hilbert của một họ $ (E_{i,\alpha})_{\alpha \in A(i)} $ các không gian con vectơ đóng. Khi đó $ E_1 \otimes_2 ... \otimes_2 E_n $ là một tổng hilbert của họ các không gian con $ E_{1,\alpha_1} \hat{\otimes}_2 ... \hat{\otimes}_2 E_{n,\alpha_n} $ với $ (\alpha_1, ..., \alpha_n) $ chạy trên $ A(1) \times ... \times A(n) $.

Theo công thức (6) của V, p. 27, các không gian con $ E_{1,\alpha_1} \hat{\otimes}_2 ... \hat{\otimes}_2 E_{n,\alpha_n} $ của $ E_1 \hat{\otimes}_2 ... \hat{\otimes}_2 E_n $ đôi một trực giao. Với mọi số nguyên $ i $ giữa 1 và $ n $, tập hợp $ \bigcup_{\alpha \in A(i)} E_{i,\alpha} $ là toàn thể trong $ E_i $, và ánh xạ đa tuyến tính $ (x_1, ..., x_n) \mapsto x_1 \otimes ... \otimes x_n $ là liên tục.

Suy ra rằng hợp của các không gian con $ E_{1,\alpha_1} \hat{\otimes}_2 ... \hat{\otimes}_2 E_{n,\alpha_n} $ là toàn thể, do đó prop. 3.

#### Hệ quả 1 {#evt-v-s3-prop-3-cor-1 .statement}

— Với $ 1 \leq i \leq n $, cho $ (e_{i,\alpha})_{\alpha \in A(i)} $ là một cơ sở trực chuẩn của $ E_i $. Khi đó họ các vectơ $ e_{1,\alpha_1} \otimes \ldots \otimes e_{n,\alpha_n} $ khi $ (\alpha_1, \ldots, \alpha_n) $ chạy trên $ A(1) \times \cdots \times A(n) $ là một cơ sở trực chuẩn của $ E_1 \hat{\otimes}_2 \ldots \hat{\otimes}_2 E_n $.

#### Hệ quả 2 {#evt-v-s3-prop-3-cor-2 .statement}

— Cho $ E_1 $ và $ E_2 $ là hai không gian Hilbert, và $ (e_i)_{i \in I} $ là một cơ sở trực chuẩn của $ E_1 $. Cho $ (y_i)_{i \in I} $ là một họ các phần tử của $ E_2 $, sao cho $ \sum_{i \in I} \| y_i \| ^2 < + \infty $. Khi đó họ $ (e_i \otimes y_i)_{i \in I} $ là khả tổng trong $ E_1 \hat{\otimes}_2 E_2 $; hơn nữa, mọi phần tử của $ E_1 \otimes E_2 $ có thể được viết duy nhất dưới dạng $ \sum_{i \in I} e_i \otimes y_i $ với $ \sum_{i \in I} \| y_i \| ^2 < + \infty $.

Cho $ F_i $ là đường thẳng trong $ E_1 $ sinh bởi các $ e_i $ ($ i \in I $). Khi đó $ E_1 $ là tổng Hilbert của họ các không gian con $ (F_i)_{i \in I} $. Theo Mệnh đề 3, không gian $ E_1 \hat{\otimes}_2 E_2 $ là tổng Hilbert của họ các không gian con $ (F_i \hat{\otimes}_2 E_2)_{i \in I} $, do đó Hệ quả 2 được suy ra.

#### Ví dụ 1 {#evt-v-s3-n2-exa-1 .statement}

Theo Hệ quả 1, không gian $ \ell^2(I) \hat{\otimes}_2 \ell^2(J) $ đẳng cấu chính tắc với $ \ell^2(I \times J) $, tích tenxơ $ x \otimes y $ của $ x = (x_i)_{i \in I} $ và $ y = (y_j)_{j \in J} $ có thể được đồng nhất với họ $ (x_i y_j)_{i \in I, j \in J} $. Tương tự, theo Hệ quả 2, $ \ell^2(I) \hat{\otimes}_2 E $ có thể được đồng nhất với $ \ell^2_E(I) $, sao cho ta có $ (x_i)_{i \in I} \otimes y = (x_i y)_{i \in I} $ với mọi $ y $ trong không gian Hilbert $ E $.

#### Ví dụ 2 {#evt-v-s3-n2-exa-2 .statement}

Cho $ X $ là một không gian tôpô Hausdorff, và $ \mu $ là một độ đo dương trên $ X $. Cho $ E $ là một không gian Hilbert. Ta có thể đồng nhất $ L^2(X, \mu) \hat{\otimes}_2 E $ với $ L^2_E(X, \mu) $ một cách chính tắc : nếu $ f $ là lớp của hàm vô hướng khả tích bình phương $ f $ trên $ X $, và nếu $ a $ thuộc $ E $, thì $ f \otimes a $ là lớp của hàm $ x \mapsto f(x).a $ với các giá trị trong $ E $.

Cho $ Y $ là một không gian tôpô Hausdorff và $ \nu $ là một độ đo dương trên $ Y $. Theo một cách tương tự, ta có thể đồng nhất các không gian Hilbert $ L^2(X, \mu) \hat{\otimes}_2 L^2(Y, \nu) $ và $ L^2(X \times Y, \mu \otimes \nu) $; khi đó $ f \otimes g $ có thể được đồng nhất với lớp của hàm $ (x, y) \mapsto f(x)g(y) $ trên $ X \times Y $. \*

### 3. Các lũy thừa Hilbert đối xứng

Cho $ E $ là một không gian Hilbert, và cho $ n $ là một số nguyên dương. Ký hiệu $ \hat{T}^n(E) $ hoặc $ E^{\hat{\otimes} n} $ cho tích tenxơ của $ n $ không gian Hilbert, mỗi không gian đều bằng $ E $. Nói cách khác, $ \hat{T}^n(E) $ là sự hoàn thiện của không gian $ T^n(E) = E \otimes \ldots \otimes E $ ($ n $ thừa số) đối với cấu trúc không gian tiền Hilbert Hausdorff được xác định bởi

$$
\langle x_1 \otimes \ldots \otimes x_n | y_1 \otimes \ldots \otimes y_n \rangle = \prod_{i=1}^n \langle x_i | y_i \rangle .
$$

Nếu $ (e_i)_{i \in I} $ là một cơ sở trực chuẩn của $ E $, thì họ các vectơ $ e_{i_1} \otimes \ldots \otimes e_{i_n} $ với $ i_1, \ldots, i_n $ trong $ I $, là một cơ sở trực chuẩn của $ \hat{T}^n(E) $ (V, p. 29, hệ quả 1). Ta có $ \hat{T}^\circ(E) = K $.

Cho $ \sigma \in S_n $ là một phép hoán vị của tập $ \{ 1, 2, \ldots, n \} $. Theo V, p. 27, tồn tại một tự đẳng cấu $ p_\sigma $ của $ \hat{T}^n(E) $ được đặc trưng bởi

$$
p_\sigma(x_1 \otimes \ldots \otimes x_n) = x_{\sigma^{-1}(1)} \otimes \ldots \otimes x_{\sigma^{-1}(n)} .
$$

Ta có $ p_{\sigma \tau} = p_{\sigma} p_{\tau} $ với $ \sigma, \tau $ trong $ \mathfrak{S}_n $, và do đó tự đồng cấu $ \Pi_n = \frac{1}{n!} \sum_{\sigma \in \mathfrak{S}_n} p_{\sigma} $ của không gian vectơ $ \hat{\mathbf{T}}^n(E) $ là phép chiếu trực giao lên không gian con của tất cả các phần tử bất biến bởi $ \mathfrak{S}_n $. Tuy nhiên (A, III, § 6, No. 3), $ \Pi_n $ ánh xạ tích tenxơ « đại số » $ \mathbf{T}^n(E) $ lên không gian con $ \mathbf{TS}^n(E) $ của tất cả các tenxơ đối xứng bậc $ n $. Nói cách khác, ảnh của $ \Pi_n $ là sự hoàn thiện của không gian $ \mathbf{TS}^n(E) $ được trang bị một tích vô hướng cảm sinh bởi tích vô hướng của $ \mathbf{T}^n(E) $; sự hoàn thiện này sẽ được ký hiệu bởi $ \widetilde{\mathbf{TS}}^n(E) $.

Cho $ \mathbf{S}^n(E) $ là lũy thừa đối xứng thứ $ n $ của không gian vectơ $ E $ (A, III, § 6, No. 1). Ánh xạ chính tắc từ $ \mathbf{T}^n(E) $ lên $ \mathbf{S}^n(E) $ xác định bởi hạn chế một đẳng cấu $ \lambda_n $ từ $ \mathbf{TS}^n(E) $ lên $ \mathbf{S}^n(E) $. Ta kiểm tra ngay lập tức rằng đẳng cấu nghịch đảo được cho bởi

$$
\mu_n(x_1 \ldots x_n) = \Pi_n(x_1 \otimes \ldots \otimes x_n) = \frac{1}{n!} \sum_{\sigma \in \mathfrak{S}_n} x_{\sigma^{-1}(1)} \otimes \ldots \otimes x_{\sigma^{-1}(n)}
$$

với $ x_1, \ldots, x_n $ trong $ E $.

Ta định nghĩa một cấu trúc không gian tiền Hilbert Hausdorff trên $ \mathbf{S}^n(E) $ bằng cách đặt

$$
\langle u|v \rangle = n! \langle \mu_n(u)|\mu_n(v) \rangle .
$$

Khi đó ta có (so sánh với công thức (29) của A, III, § 11, No. 5)

$$
\langle x_1 \ldots x_n|y_1 \ldots y_n \rangle = \sum_{\sigma \in \mathfrak{S}_n} \prod_{i=1}^n \langle x_i|y_{\sigma(i)} \rangle ,
$$

và đặc biệt

$$
\langle x^n|y^n \rangle = n! \langle x|y \rangle^n .
$$

Ký hiệu $ \hat{\mathbf{S}}^n(E) $ là sự hoàn thiện của không gian tiền Hilbert $ \mathbf{S}^n(E) $ và $ \hat{\mathbf{S}}(E) $ là tổng Hilbert ngoài của các không gian Hilbert $ \hat{\mathbf{S}}^n(E) $. Ta có thể chứng minh (V, p. 73, bài tập 1) rằng phép nhân trong đại số $ \mathbf{S}(E) $ không thể được mở rộng liên tục đến $ \mathbf{S}(E) $, trừ khi $ E $ chỉ là 0.

#### Mệnh đề 4 {#evt-v-s3-prop-4 .statement}

*Cho $ (e_i)_{i \in I} $ là một cơ sở trực chuẩn của không gian Hilbert $ E $. Với mọi $ \alpha $ trong $ \mathbf{N}^{(I)} $, đặt*

$$
z_{\alpha} = \prod_{i \in I} e_i^{\alpha_i}/(\alpha_i!)^{1/2} .
$$

*Thì $ (z_{\alpha})_{\alpha \in \mathbf{N}^{(I)}} $ là một cơ sở trực chuẩn của $ \hat{\mathbf{S}}(E) $.*

Cho $ E_0 $ là không gian con vectơ của $ E $ sinh bởi các vectơ $ e_i $ với $ i $ chạy trên $ I $. Khi đó các $ z_{\alpha} $ tạo thành một cơ sở của không gian vectơ $ \mathbf{S}(E_0) $ (A, III, § 6, No. 6). Nhưng $ E_0 $ trù mật trong $ E $, và ánh xạ đa tuyến $ (x_1, \ldots, x_n) \mapsto x_1 \ldots x_n $ từ $ E \times \cdots \times E $ vào $ \mathbf{S}(E) $ là liên tục với mọi $ n \geqslant 1 $; do đó $ \mathbf{S}(E_0) $ trù mật trong $ \mathbf{S}(E) $. Bây giờ chỉ cần chứng minh rằng họ các $ z_\alpha $ là trực chuẩn. Trước hết nhận xét rằng $ \hat{S}^n(E) $ và $ \hat{S}^m(E) $ là trực giao khi $ n \neq m $. Do đó chỉ cần chứng minh công thức

$$
\langle z_\alpha | z_\beta \rangle = \left\{ \begin{array}{ll}
1 & \text{nếu } \alpha = \beta \\
0 & \text{nếu } \alpha \neq \beta
\end{array} \right.
$$

khi $ |\alpha| = \sum_{i \in I} \alpha_i $ và $ |\beta| = \sum_{i \in I} \beta_i $ bằng cùng một số nguyên $ n $.

Xét một phân hoạch $ (P_i)_{i \in I} $ của tập hợp $ \{ 1, 2, ..., n \} $ sao cho Card $ P_i = \alpha_i $ với mọi $ i \in I $. Đặt $ x_k = e_i $ nếu $ k $ thuộc $ P_i $, khi đó $ x_1 ... x_n = \prod_{i \in I} e_i^{\alpha_i} $. Tương tự ta định nghĩa $ (Q_i)_{i \in I} $ và $ y_k $ sao cho Card $ Q_i = \beta_i $ và $ y_1 ... y_n = \prod_{i \in I} e_i^{\beta_i} $. Vì các $ e_i $ đôi một trực giao, ta có $ \langle x_k | y_{\sigma(k)} \rangle = 0 $ trừ khi tồn tại một chỉ số $ i \in I $ sao cho $ k \in P_i $ và $ \sigma(k) \in Q_i $. Theo công thức (15), khi đó ta có $ \langle x_1 ... x_n | y_1 ... y_n \rangle = 0 $ trừ khi tồn tại một phép hoán vị $ \sigma \in \mathfrak{S}_n $ sao cho $ \sigma(P_i) = Q_i $ với mọi $ i \in I $, điều này suy ra $ \alpha = \beta $. Khi đó $ \langle z_\alpha | z_\beta \rangle = 0 $ đối với $ \alpha \neq \beta $. Cùng một lập luận chứng minh rằng $ \| x_1 ... x_n \| ^2 $ bằng số các $ \sigma \in \mathfrak{S}_n $ sao cho $ \sigma(P_i) = P_i $ với mọi $ i \in I $, do đó bằng $ \prod_{i \in I} \alpha_i ! $. Ta được $ \| z_\alpha \| = 1 $, và mệnh đề được chứng minh.

#### Hệ quả {#evt-v-s3-n3-cor-1 .statement}

— *Giả sử rằng không gian hilbert E là tổng trực tiếp của các không gian con trực giao M và N. Đẳng cấu chính tắc g từ $ S(M) \otimes S(N) $ lên $ S(E) $ (A, III, § 6, No. 6) mở rộng duy nhất thành một đẳng cấu không gian hilbert h từ $ \hat{S}(M) \hat{\otimes}_2 \hat{S}(N) $ lên $ \hat{S}(E) $.

Cho $ (e_i)_{i \in I} $ (tương ứng $ (f_j)_{j \in J} $) là một cơ sở trực chuẩn của không gian hilbert M (tương ứng N) và cho $ M_0 $ (tương ứng $ N_0 $) là không gian vectơ con của E sinh bởi các vectơ $ e_i $ (tương ứng $ f_j $). Đặt $ E_0 = M_0 + N_0 $ và cho $ g_0 $ là đẳng cấu chính tắc từ $ S(M_0) \otimes S(N_0) $ lên $ S(E_0) $. Đặt

$$
z_\alpha = \prod_{i \in I} e_i^{\alpha_i}/(\alpha_i!)^{1/2}, \quad t_\beta = \prod_{j \in J} f_j^{\beta_j}/(\beta_j!)^{1/2}
$$

với $ \alpha \in \mathbf{N}^{(I)} $ và $ \beta \in \mathbf{N}^{(J)} $. Theo mệnh đề 4, do đó ta đã xác định các cơ sở trực chuẩn $ (z_\alpha)_{\alpha \in \mathbf{N}^{(I)}} $ của $ \hat{S}(M) $, $ (t_\beta)_{\beta \in \mathbf{N}^{(J)}} $ của $ \hat{S}(N) $ và $ (z_\alpha t_\beta)_{\alpha \in \mathbf{N}^{(I)}, \beta \in \mathbf{N}^{(J)}} $ của $ \hat{S}(E) $. Vì ta có $ z_\alpha t_\beta = g_0(z_\alpha \otimes t_\beta) $, và vì các phần tử $ z_\alpha \otimes t_\beta $ lập thành một cơ sở trực chuẩn của $ \hat{S}(M) \hat{\otimes}_2 \hat{S}(N) $ (V, p. 29, hệ quả 1), ta thấy rằng $ g_0 $ mở rộng thành một đẳng cấu không gian hilbert $ h : \hat{S}(M) \hat{\otimes}_2 \hat{S}(N) \to \hat{S}(E) $. Theo phép dựng, ta có

$$
h(x_1 ... x_m \otimes y_1 ... y_n) = x_1 ... x_m y_1 ... y_n
$$

với mọi vectơ $ x_1, ..., x_m $ trong $ M_0 $ và $ y_1, ..., y_n $ trong $ N_0 $. Do tính liên tục, cùng một quan hệ cũng đúng đối với các vectơ $ x_1, ..., x_n $ trong M và các vectơ $ y_1, ..., y_n $ trong N; nói cách khác, $ h $ mở rộng $ g $. Tính duy nhất của $ h $ là rõ ràng.

Cho E và F là hai không gian hilbert và $ u \in \mathcal{L}(E; F) $. Ánh xạ tuyến tính $ \hat{T}^n(u) = u \hat{\otimes}_2 ... \hat{\otimes}_2 u $ ($ n $ thừa số) từ $ \hat{T}^n(E) $ vào $ \hat{T}^n(F) $ là liên tục với chuẩn $ \|u\|^n $ (V, p. 28, công thức (10)). Hơn nữa, các công thức (13) và (14) của V, p. 30, chỉ ra rằng tồn tại một đẳng cấu $ \phi_{n,E} $ từ $ \hat{S}^n(E) $ lên không gian con $ \widehat{T S^n}(E) $ của $ \hat{T}^n(E) $, và chỉ một, sao cho

$$
(18) \quad \phi_{n,E}(x_1 \ldots x_n) = \frac{1}{(n!)^{1/2}} \sum_{\sigma \in \mathfrak{S}_n} x_{\sigma(1)} \otimes \ldots \otimes x_{\sigma(n)} \quad (x_1, ..., x_n \text{ trong } E) .
$$

Do đó tồn tại một ánh xạ tuyến tính liên tục $ \hat{S}^n(u) $ từ $ \hat{S}^n(E) $ vào $ \hat{S}^n(F) $ và chỉ một ánh xạ làm cho biểu đồ sau giao hoán

$$
\begin{array}{ccc}
\hat{S}^n(E) & \xrightarrow{\phi_{n,E}} & \hat{T}^n(E) \\
\downarrow \hat{S}^n(u) & & \downarrow \hat{T}^n(u) \\
\hat{S}^n(F) & \xrightarrow{\phi_{n,F}} & \hat{T}^n(F)
\end{array}
$$

Bây giờ chứng minh công thức

$$
(19) \qquad \| \hat{S}^n(u) \| = \| u \|^{n} .
$$

Ta có rõ ràng $ \| \hat{S}^n(u) \| \leq \| \hat{T}^n(u) \| = \| u \|^{n} $. Hơn nữa, với mọi $ x \in E $, ta có $ \hat{S}^n(u)(x^n) = u(x)^n, \| x^n \| = (n!)^{1/2} \| x \|^{n} $ và $ \| u(x)^n \| = (n!)^{1/2} \| u(x) \|^{n} $, điều này cho

$$
\| \hat{S}^n(u) \| \cdot \| x \|^{n} \geq \| u(x) \|^{n} ;
$$

suy ra ngay lập tức rằng $ \| \hat{S}^n(u) \| \geq \| u \|^{n} $, do đó công thức (19).

Rõ ràng là ta có các công thức

$$
(20) \qquad \hat{S}^n(1_E) = 1_{\hat{S}_n(E)}
$$
$$
(21) \qquad \hat{S}^n(v \circ u) = \hat{S}^n(v) \circ \hat{S}^n(u) \quad \text{cho} \quad v \in \mathcal{L}(F ; G) .
$$

Cuối cùng, $ \hat{S}^n(u) $ trùng với trên $ S^n(E) $ với ánh xạ tuyến tính $ S^n(u) : S^n(E) \to S^n(F) $ được định nghĩa trong A, III, § 6, No. 2 vì nó biến $ x_1 ... x_n $ thành $ u(x_1) ... u(x_n) $ với mọi $ x_1, ..., x_n $ trong $ E $.

#### Ví dụ 1 {#evt-v-s3-n3-exa-1 .statement}

Cho $ d \geq 1 $ là một số nguyên và $ \omega $ là một hàm dương trên $ \mathbf{R}^d $, khả tích địa phương đối với độ đo Lebesgue $ \mu $. Cho $ E $ là không gian Hilbert $ L^2(\mathbf{R}^d, \omega.\mu) $, và đặt $ S = S(E) $. Khi đó $ S $ có thể được đồng nhất với không gian của mọi dãy $ f = (f_n)_{n \geq 0} $, trong đó mỗi $ f_n $ là một hàm trên $ (\mathbf{R}^d)^n $ đo được đối với độ đo Lebesgue $ \mu \otimes ... \otimes \mu $ ($ n $ thừa số) và *bất biến* dưới các hoán vị của $ n $ thừa số trong $ (\mathbf{R}^d)^n $, và sao cho

$$
(22) \qquad \| f \|^{2} = \sum_{n=0}^{\infty} n! \int_{\mathbf{R}^d} ... \int_{\mathbf{R}^d} |f_n(x_1, ..., x_n)|^2 \omega(x_1) ... \omega(x_n) dx_1 ... dx_n
$$

là hữu hạn. Chuẩn $ \| f \| $ trong $ S $ được định nghĩa bởi công thức (22). Không gian Hilbert $ S $ được định nghĩa ở trên được gọi là *không gian Fock đối xứng* tương ứng với *trọng số* $ \omega $.

#### Ví dụ 2 {#evt-v-s3-n3-exa-2 .statement}

Cho $ X $ là một không gian tôpô Hausdorff, $ \mu $ là một độ đo dương có chuẩn 1 trên $ X $ và $ E $ là một không gian con Hilbert của không gian Hilbert thực $ L^2_{\mathbf{R}}(X, \mu) $. Ta nói rằng $ E $ là một *không gian gaussian* nếu các điều kiện tương đương sau được thỏa mãn :

a) với mọi $ f \in E $, ta có $ \int_X e^{i f} d\mu = \exp(-\| f \|^{2}/2) ; $

b) với mọi $ f \in E $ có chuẩn 1, ảnh của độ đo $ \mu $ qua $ f $ là độ đo
$$
(2\pi)^{-1/2}\ e^{-x^2/2} dx .
$$
trên $ \mathbf{R} $.

*Giả sử $ E $ là một không gian gaussian.* Cho $ f_1, ..., f_n $ là các hàm mà các lớp $ f_i $ thuộc $ E $. Ta định nghĩa một hàm : $ f_1 ... f_n $ : trên X (gọi là « tích Wick » của $ f_1, ..., f_n $) bằng công thức
$$
(23)\quad :f_1 ... f_n: = \sum_{0 \leq 2p \leq n} (-1)^p \sum_{\sigma \in I_p} \prod_{i=1}^p \langle f_{\sigma(2i-1)}|f_{\sigma(2i)} \rangle \prod_{j=2p+1}^n f_{\sigma(j)},
$$
trong đó $ I_p $ là tập hợp các hoán vị $ \sigma $ của $ \{1, 2, ..., n\} $ sao cho ta có
$$
\begin{align*}
&\sigma(1) < \sigma(2), ..., \sigma(2p-1) < \sigma(2p) \\
&\sigma(1) < \sigma(3) < ... < \sigma(2p-1) \\
&\sigma(2p+1) < \sigma(2p+2) < ... < \sigma(n).
\end{align*}
$$

Khi đó tồn tại một *đẳng cấu* $ \phi $ *từ* $ \hat{S}(E) $ *onto một không gian con Hilbert của* $ L^2_R(X, \mu) $ *biến tích* $ f_1 ... f_n $ *của* $ f_1, ..., f_n $, *được tính trong* $ \hat{S}(E) $, *thành* $ (:f_1 ... f_n:) $. Giả sử rằng X là một không gian Souslin và rằng tồn tại một họ đếm được $ (f_n) $ các hàm mà các lớp của chúng thuộc E và phân biệt các điểm của X. Khi đó $ \phi $ là một đẳng cấu từ $ \hat{S}(E) $ onto $ L^2_R(X, \mu) $. \*

### 4. Các lũy thừa Hilbert ngoài

Cho E là một không gian Hilbert và $ n $ là một số nguyên dương. Với mỗi phép hoán vị $ \sigma \in \mathfrak{S}_n $, ký hiệu $ \varepsilon_\sigma $ là dấu của nó; đặt $ a_n = \frac{1}{n!} \sum_{\sigma \in \mathfrak{S}_n} \varepsilon_\sigma p_\sigma $ trong $ \mathcal{L}(\hat{T}^n(E)) $ (V, p. 29).

Hiển nhiên $ a_n $ là một phép chiếu trực giao, có ảnh $ \overline{\mathbf{A}'_n}(E) $ là bao đóng trong $ \hat{T}^n(E) $ của không gian $ \mathbf{A}'_n(E) $ gồm tất cả các tenxơ phản đối xứng cấp $ n $ (A, III, § 7, No. 4). Tồn tại một đẳng cấu $ \pi_n $ từ $ \Lambda^n(E) $ onto $ \mathbf{A}'_n(E) $ được đặc trưng bởi
$$
(24)\quad \pi_n(x_1 \wedge ... \wedge x_n) = a_n(x_1 \otimes ... \otimes x_n) = \frac{1}{n!} \sum_{\sigma \in \mathfrak{S}_n} \varepsilon_\sigma x_{\sigma(1)} \otimes ... \otimes x_{\sigma(n)}
$$
với $ x_1, ..., x_n $ trong E. Ta có thể định nghĩa một cấu trúc không gian tiền Hilbert Hausdorff trên $ \Lambda^n(E) $ bằng cách đặt
$$
(25)\quad \langle u|v \rangle = n!\langle \pi_n(u)|\pi_n(v) \rangle .
$$
Cụ thể hơn, ta có (so sánh với công thức (30) của A, III, § 11, No. 5).
$$
(26)\quad \langle x_1 \wedge ... \wedge x_n|y_1 \wedge ... \wedge y_n \rangle = \det(\langle x_i|y_j' \rangle)
$$
với mọi $ x_1, ..., x_n $ và $ y_1, ..., y_n $ trong E.

Ký hiệu $ \hat{\Lambda}^n(E) $ là sự hoàn tất của không gian tiền Hilbert $ \Lambda^n(E) $, và $ \hat{\Lambda}(E) $ là tổng Hilbert ngoài của các không gian Hilbert $ \hat{\Lambda}^n(E) $.

#### Ví dụ {#evt-v-s3-n4-exa-1 .statement}

— *Với các ký hiệu của ví dụ 1 của V, p. 32, ta có thể đồng nhất không gian Hilbert* $ \hat{\Lambda}(E) $ *với tập hợp tất cả các dãy* $ (f_n)_{n \geq 0} $ *các hàm đo được sao cho số* $ \|f\| $ *được định nghĩa trong* (22) *là hữu hạn, và trong đó mỗi hàm* $ f_n $ *là phản đối xứng*, *nghĩa là, thỏa mãn quan hệ*

$$
f_n(x_{\sigma(1)}, ..., x_{\sigma(n)}) = \varepsilon_\sigma f_n(x_1, ..., x_n)
$$

*với mọi phép hoán vị* $ \sigma \in \mathfrak{S}_n $. *Không gian Hilbert* $ \hat{\Lambda}(E) $ *được gọi là không gian Fock phản đối xứng tương ứng với* *trọng số* $ \omega $. \*

#### Mệnh đề 5 {#evt-v-s3-prop-5 .statement}

*Cho* $ (e_i)_{i \in I} $ *là một cơ sở trực chuẩn của không gian Hilbert* E. *Trang bị cho* I *một cấu trúc được sắp thứ tự toàn phần. Khi đó tập hợp tất cả các phần tử* $ e_{i_1} \wedge ... \wedge e_{i_n} $ *với* $ i_1 < ... < i_n $ *là một cơ sở trực chuẩn của* $ \hat{\Lambda}^n(E) $.

Ta biết (A, III, § 7, No. 8) rằng các phần tử đang xét tạo thành một cơ sở của không gian vectơ $ \Lambda^n(E_0) $ trong đó $ E_0 $ là không gian con vectơ của E được sinh bởi các vectơ $ e_i $. Hơn nữa, với $ i_1 < ... < i_n $, ma trận các tích vô hướng $ \langle e_{i_k}|e_{i_l} \rangle $ là ma trận đơn vị cấp n; theo (26), ta có $ \|e_{i_1} \wedge ... \wedge e_{i_n}\| = 1 $. Cuối cùng, nếu $ (i_1, ..., i_n) $ và $ (j_1, ..., j_n) $ là hai dãy khác nhau, tăng ngặt gồm các phần tử của I, thì tồn tại một phần tử $ j_\ell $ khác với $ i_1, ..., i_n $ nên ta có $ \langle e_{i_k}|e_{j_\ell} \rangle = 0 $ với $ 1 \leq k \leq n $, và theo (26), $ \langle e_{i_1} \wedge ... \wedge e_{i_n}|e_{j_1} \wedge ... \wedge e_{j_n} \rangle = 0 $. Nói cách khác, họ các phần tử $ e_{i_1} \wedge ... \wedge e_{i_n} $, với $ i_1 < ... < i_n $, là trực chuẩn.

Nhưng $ E_0 $ trù mật trong E, và ánh xạ $ (x_1, ..., x_n) \mapsto x_1 \wedge ... \wedge x_n $ từ $ E \times \cdots \times E $ vào $ \Lambda^n(E) $ là liên tục. Do đó, $ \Lambda^n(E_0) $ trù mật trong $ \Lambda^n(E) $, và mệnh đề 5 được suy ra.

#### Hệ quả {#evt-v-s3-n4-cor-1 .statement}

*Giả sử không gian Hilbert* E *là tổng trực tiếp của hai không gian con trực giao* M *và* N. *Đẳng cấu chính tắc* g *từ* $ \Lambda(M) \otimes \Lambda(N) $ *lên* $ \Lambda(E) $ *(A, III, § 7, No. 7)* *mở rộng một cách duy nhất thành một đẳng cấu không gian Hilbert từ* $ \hat{\Lambda}(M) \hat{\otimes}_2 \hat{\Lambda}(N) $ *lên* $ \hat{\Lambda}(E) $.

Chứng minh tương tự như chứng minh của hệ quả của mệnh đề 4 (V, p. 31).

Cho E và F là hai không gian Hilbert và $ u \in \mathcal{L}(E; F) $. Ta sẽ chỉ ra, như trong trường hợp của các lũy thừa đối xứng $ \hat{S}^n(E) $ (V, p. 32) rằng ánh xạ tuyến tính $ \hat{\Lambda}^n(u) $ từ $ \hat{\Lambda}^n(E) $ vào $ \hat{\Lambda}^n(F) $ (A, III, § 7, No. 4) mở rộng thành một ánh xạ tuyến tính liên tục $ \hat{\Lambda}^n(u) $ từ $ \hat{\Lambda}^n(E) $ vào $ \hat{\Lambda}^n(F) $. Ta có các hệ thức

$$
\hat{\Lambda}^n(1_E) = 1_{\hat{\Lambda}^n(E)} , \tag{27}
$$
$$
\hat{\Lambda}^n(v \circ u) = \hat{\Lambda}^n(v) \circ \hat{\Lambda}^n(u) \quad \text{nếu } v \text{ thuộc } \mathcal{L}(F; G) , \tag{28}
$$
$$
\|\hat{\Lambda}^n(u)\| \leq \|u\|^n . \tag{29}
$$

Nói chung ta không có đẳng thức trong công thức (29) (TS, IV, § 6). Cuối cùng, ta có một đẳng cấu $ \psi_n = \psi_{n,E} $ từ $ \hat{\Lambda}^n(E) $ lên không gian con $ \overline{\mathbf{A}}'_n(E) $ của $ \hat{T}^n(E) $ được xác định bởi

$$
\psi_n(x_1 \wedge ... \wedge x_n) = \frac{1}{(n!)^{1/2}} \sum_{\sigma \in \mathfrak{S}_n} \varepsilon_\sigma x_{\sigma(1)} \otimes ... \otimes x_{\sigma(n)} . \tag{30}
$$

### 5. Phép nhân ngoài

Cho E là một không gian Hilbert. Với mỗi số nguyên $ n \geqslant 0 $, ký hiệu $ \theta_n $ là ánh xạ chính tắc từ $ T^n(E) $ lên $ \Lambda^n(E) $; khi đó

$$
\theta_n(x_1 \otimes \ldots \otimes x_n) = x_1 \wedge \ldots \wedge x_n
$$

với $ x_1, \ldots, x_n $ trong E. Cho $ p $ và $ q $ là hai số nguyên dương; nhờ các công thức (30) và (31) ta có

$$
u \wedge v = \theta_{p+q}\left( \frac{1}{(p!)^{1/2}} \psi_p(u) \otimes \frac{1}{(q!)^{1/2}} \psi_q(v) \right)
$$

với $ u \in \Lambda^p(E) $ và $ v \in \Lambda^q(E) $. Vì $ \| \theta_n \| \leq (n!)^{1/2} $, ta được bất đẳng thức

$$
\| u \wedge v \| \leq \left( \frac{(p+q)!}{p! \ q!} \right)^{1/2} \| u \| \cdot \| v \|
$$

Do đó, ánh xạ $ (u, v) \mapsto u \wedge v $ mở rộng theo tính liên tục thành một ánh xạ song tuyến tính từ $ \hat{\Lambda}^p(E) \times \hat{\Lambda}^q(E) $ vào $ \hat{\Lambda}^{p+q}(E) $, với chuẩn không vượt quá $ \left( \frac{(p+q)!}{p! \ q!} \right)^{1/2} $ (xem V, p. 73, bài tập 2). Ta lại ký hiệu nó bởi $ (u, v) \mapsto u \wedge v $.

#### Mệnh đề 6 {#evt-v-s3-prop-6 .statement}

*Cho E là một không gian Hilbert. Ta có*

$$
\| x \wedge u \| \leq \| x \| \cdot \| u \|
$$

*với* $ x \in E $ *và* $ u \in \hat{\Lambda}(E) $.

Rõ ràng chỉ cần xét trường hợp $ \| x \| = 1 $.

Cho F là không gian con Hilbert của E gồm tất cả các vectơ vuông góc với x. Vì E là tổng Hilbert của F và đường thẳng K.x, suy ra từ hệ quả của V, p. 34 rằng ánh xạ $ (v, w) \mapsto v + x \wedge w $ là một đẳng cấu không gian Hilbert từ $ \hat{\Lambda}(F) \oplus \hat{\Lambda}(F) $ lên $ \hat{\Lambda}(E) $. Nếu $ u = v + x \wedge w $ với $ v, w $ trong $ \hat{\Lambda}(F) $, ta có $ x \wedge u = x \wedge v $, do đó $ \| x \wedge u \| = \| v \| \leq (\| v \|^2 + \| w \|^2)^{1/2} = \| u \| $.

#### Hệ quả 1 {#evt-v-s3-prop-6-cor-1 .statement}

*a)* *Cho* $ x_1, \ldots, x_n $ *là các phần tử của không gian Hilbert* E. *Ta có*

$$
\| x_1 \wedge \ldots \wedge x_n \| \leq \| x_1 \| \ldots \| x_n \|,
$$

*trong đó dấu bằng chỉ xảy ra nếu một trong các* $ x_i $ *bằng 0, hoặc nếu dãy* $ (x_1, \ldots, x_n) $ *là trực giao.*

*b)* *Cho* $ x_1, \ldots, x_n, y_1, \ldots, y_n $ *là các phần tử của không gian Hilbert* E. *Ta có*

$$
|\det(\langle x_i, y_j \rangle)| \leq \| x_1 \| \ldots \| x_n \| \cdot \| y_1 \| \ldots \| y_n \|;
$$

nếu các vectơ $ x_i $ và $ y_i $ đều khác 0; thì đẳng thức trong (36) xảy ra khi và chỉ khi $ (x_1, ..., x_n) $ và $ (y_1, ..., y_n) $ mỗi dãy là một cơ sở trực giao của cùng một không gian con vectơ của E.

Bất đẳng thức (35) suy ra từ mệnh đề 6 bằng quy nạp theo $ n $; bất đẳng thức (36) có thể suy ra bằng cách áp dụng bất đẳng thức Cauchy-Schwarz trong $ \Lambda^n(E) $ và công thức (26) của V, p. 33.

Giả sử dãy $ (x_1, ..., x_n) $ là trực giao. Khi đó

$$
\| x_1 \wedge ... \wedge x_n \|^2 = \det(\langle x_i | x_j \rangle) = \prod_{i=1}^n \| x_i \|^2
$$

vì $ \langle x_i | x_j \rangle = 0 $ với $ i \neq j $.

Bây giờ giả sử rằng các vectơ $ x_1, ..., x_n $ đều không bằng 0 và không tạo thành một dãy trực giao. Vì $ \| x_1 \wedge ... \wedge x_n \| $ phụ thuộc đối xứng vào các vectơ $ x_1, ..., x_n $, ta có thể giả sử rằng $ x_1 $ không vuông góc với không gian con F của E sinh bởi $ x_2, ..., x_n $, và rằng F không chỉ là 0. Ta có thể phân tích $ x_1 $ dưới dạng $ x'_1 + y $ với $ y \neq 0 $ trong F và $ x'_1 $ vuông góc với F; khi đó $ \| x'_1 \| < \| x_1 \| $. Nhưng

$$
x_1 \wedge x_2 \wedge ... \wedge x_n = x'_1 \wedge x_2 \wedge ... \wedge x_n,
$$

và do đó

$$
\begin{align*}
\| x_1 \wedge ... \wedge x_n \| &\leq \| x'_1 \| \| x_2 \| ... \| x_n \| \\
&< \| x_1 \| \| x_2 \| ... \| x_n \|.
\end{align*}
$$

Giả sử rằng các vectơ $ x_i $ và các vectơ $ y_i $ đều không bằng 0. Đẳng thức trong quan hệ (36) tương đương với việc đồng thời có các đẳng thức

(37) $$ |\langle x_1 \wedge ... \wedge x_n | y_1 \wedge ... \wedge y_n \rangle| = \| x_1 \wedge ... \wedge x_n \| \cdot \| y_1 \wedge ... \wedge y_n \| $$

(38) $$ \| x_1 \wedge ... \wedge x_n \| = \| x_1 \| ... \| x_n \| , \quad \| y_1 \wedge ... \wedge y_n \| = \| y_1 \| ... \| y_n \| . $$

Theo phần đầu của chứng minh, các đẳng thức (38) suy ra rằng mỗi dãy $ (x_1, ..., x_n) $ và $ (y_1, ..., y_n) $ đều trực giao, điều này lại suy ra rằng $ x_1 \wedge ... \wedge x_n \neq 0 $ và $ y_1 \wedge ... \wedge y_n \neq 0 $. Trong các điều kiện này, quan hệ (37) suy ra rằng tồn tại một vô hướng $ \lambda \neq 0 $ sao cho $ y_1 \wedge ... \wedge y_n = \lambda x_1 \wedge ... \wedge x_n $ (V, p. 3, Nhận xét 1); nói cách khác, $ (x_1, ..., x_n) $ và $ (y_1, ..., y_n) $ là các cơ sở của cùng một không gian con vectơ của E (A, III, § 11, No. 13).

#### Hệ quả 2 {#evt-v-s3-prop-6-cor-2 .statement}

— Cho $ (a_{ij})_{1 \leq i,j \leq n} $ là một ma trận Hermit, với các phần tử phức, và có định thức D. Giả sử rằng bất đẳng thức

$$
\sum_{i,j=1}^n a_{ij} \overline{z}_i z_j \geq 0
$$

đúng với mọi số phức $ z_1, ..., z_n $. Khi đó

$$
0 \leq D \leq a_{11} ... a_{nn}.
$$

Giả sử D khác không; đẳng thức $ D = a_{11} ... a_{nn} $ đúng khi và chỉ khi $ a_{ij} = 0 $ với mọi $ i \neq j $.

Cho $ \Phi $ là dạng Hermit trên không gian vectơ $ \mathbf{C}^n $ được cho bởi

$$
\Phi(\mathbf{z}, \mathbf{z}') = \sum_{i,j=1}^n a_{ij} \overline{z}_i z'_j
$$

với $ \mathbf{z} = (z_1, ..., z_n) $ và $ \mathbf{z}' = (z'_1, ..., z'_n) $ trong $ \mathbf{C}^n $. Theo giả thiết, $ \Phi $ là dương.

Trước hết giả sử rằng $ \Phi $ là phân biệt, tức là D khác không. Nếu $ (e_1, ..., e_n) $ là cơ sở chính tắc của $ \mathbf{C}^n $, ta có $ \Phi(e_i, e_j) = a_{ij} $, và hệ quả 2 suy ra ngay lập tức từ hệ quả 1, a) bằng cách lấy $ x_i = e_i $.

Vì $ a_{ii} = \Phi(e_i, e_i) \geq 0 $, ta cũng có bất đẳng thức (40) nếu $ D = 0 $.

#### Hệ quả 3 (« các bất đẳng thức của Hadamard ») {#evt-v-s3-prop-6-cor-3 .statement}

— Cho $ (a_{ij})_{1 \leq i, j \leq n} $ là một ma trận có phần tử phức, và có định thức D. Đặt

$$
c_i = \left( \sum_{j=1}^n |a_{ij}|^2 \right)^{1/2} \quad \text{với} \quad 1 \leq i \leq n,
$$

và $ m = \sup_{i,j} |a_{ij}| $. Khi đó ta có

$$
|D| \leq c_1 ... c_n \leq m^n \cdot n^{n/2}.
$$

Nếu $ D \neq 0 $, để $ |D| = c_1 ... c_n $ thì cần và đủ rằng các hàng $ y_i = (a_{ij})_{1 \leq j \leq n} $ của ma trận $ (a_{ij})_{1 \leq i, j \leq n} $ đôi một trực giao.

Cho không gian $ \mathbf{C}^n $ được trang bị một tích vô hướng xác định bởi

$$
\langle \mathbf{z}|\mathbf{z}' \rangle = \sum_{i=1}^n \overline{z}_i z'_i.
$$

Cho $ (\mathbf{x}_1, ..., \mathbf{x}_n) $ là cơ sở chính tắc của $ \mathbf{C}^n $ và $ \mathbf{y}_i $ là vectơ có các thành phần $ a_{ij} $ với $ 1 \leq j \leq n $. Ta có $ \| \mathbf{x}_i \| = 1 $ và $ \| \mathbf{y}_i \| = c_i $ với $ 1 \leq i \leq n $; đồng thời $ \langle \mathbf{x}_i|\mathbf{y}_j \rangle = a_{ji} $. Bất đẳng thức $ |D| \leq c_1 ... c_n $ và điều kiện xảy ra đẳng thức khi đó là các trường hợp riêng của V, p. 35, hệ quả 1. Hiển nhiên ta có $ c_i \leq m \cdot n^{1/2} $, do đó $ c_1 ... c_n \leq m^n \cdot n^{n/2} $.

### Bài tập {#evt-v-s3-exercises}

Xem [các bài tập cho § 3](exercises/s3/).
