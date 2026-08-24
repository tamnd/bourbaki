---
book: alg
book_title: Algebra
chapter: V
chapter_title: COMMUTATIVE FIELDS
section: 12
section_title: Finite fields
lang: vi
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A V.166-A V.170
pdf_pages: 0207-0212, 0280-0284
extraction: ocr
subsections:
    - "no": 1
      title: The structure of finite fields
      page: 0
      pdf_page: 207
    - "no": 2
      title: Algebraic extensions of a finite field
      page: 94
      pdf_page: 208
    - "no": 3
      title: The Galois group of the algebraic closure of a finite field
      page: 96
      pdf_page: 210
    - "no": 4
      title: Cyclotomic polynomials over a finite field
      page: 97
      pdf_page: 211
statements: 11
exercises: 14
content_sha256: 0501211c878fc1eaf87afd5a38cdfe27944f3990ac7352b00458f597e468ae8f
translated_from: content/en/alg/V/12_s12_finite_fields.md
source_content_sha256: 1c18272a32e8d3405cf34f07429f1fb5d6f434b6e11f363b5880986e01e49860
translation_model: gpt-5.4, gpt-5-6
translation_run: translate-vi-826667eb
glossary_version: 34
glossary_terms_sha256: 7dd909fefb5c9d56cb9e506b028e5e4de13a43a739c0c6edbcae6328c8267140
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 12. TRƯỜNG HỮU HẠN

### 1. Cấu trúc của các trường hữu hạn

#### Mệnh đề 1 {#alg-v-s12-prop-1 .statement}

— Cho K là một trường hữu hạn có q phần tử.

a) Đặc số của K là một số nguyên tố p, và tồn tại một số nguyên f \geq 1 sao cho q = p^f.

b) Nhóm cộng của K là tổng trực tiếp của f nhóm cyclic cấp p.

c) Nhóm nhân của K là cyclic cấp q - 1.

Vì Z là vô hạn và K hữu hạn, đồng cấu vành duy nhất \varphi : Z \to K không là đơn ánh và hạt nhân của nó là một iđêan nguyên tố của Z khác 0. Do đó đặc số của K là một số nguyên tố và K là một đại số trên trường \mathbf{F}_p có p phần tử (V, p. 2). Gọi f là bậc của K trên \mathbf{F}_p. Nếu f là vô hạn, thì với mỗi số nguyên n \geq 0, K sẽ chứa một không gian con có chiều n trên \mathbf{F}_p, do đó q \geq p^n, điều này là vô lý. Vậy f là hữu hạn. Nhóm cộng của K do đó đẳng cấu với (\mathbf{F}_p)^f, do đó suy ra các mệnh đề a) và b).

Mệnh đề c) suy ra từ Bổ đề 1 (V, p. 78).

#### Mệnh đề 2 {#alg-v-s12-prop-2 .statement}

— Cho K là một trường hữu hạn có q phần tử. Trường K là một trường phân rã của đa thức X^q - X của \mathbf{F}_p[X] và nó là tập hợp tất cả các nghiệm của đa thức này.

1 Phù hợp với các quy ước của chương này, ở đây chúng ta sẽ chỉ xét các trường giao hoán hữu hạn. Thật vậy, mọi trường hữu hạn đều giao hoán, như ta sẽ thấy trong Chương VIII (x. V, p. 170, Bài tập 14).

Với mọi $ x \neq 0 $ trong $ K $ ta có $ x^{q-1} = 1 $ vì $ K^* $ là một nhóm hữu hạn cấp $ q-1 $ (I, p. 52). Suy ra $ x^q = x $ với mỗi $ x $ trong $ K $. Đa thức $ X^q - X $ của $ \mathbf{F}_p[X] $ có bậc $ q $ và có $ q $ nghiệm trong $ K $, do đó

$$
X^q - X = \prod_{\xi \in K} (X - \xi).
$$

Mệnh đề 2 suy ra ngay từ điều này.

#### Hệ quả {#alg-v-s12-n1-cor-1 .statement}

— *Hai trường hữu hạn có cùng lực lượng thì đẳng cấu.*

Cho $ K' $ là một trường hữu hạn có $ q $ phần tử; đặc số của nó là một số nguyên tố $ p' $ chia hết $ q = p^f $, do đó $ p' = p $. Vì vậy $ K' $ là một trường phân rã của đa thức $ X^q - X $ trong $ \mathbf{F}_p[X] $ (Mệnh đề 2), và do đó $ K $ và $ K' $ đẳng cấu (V, p. 22, Hệ quả).

Khi $ K = \mathbf{F}_p $, Công thức (1) thu gọn thành quan hệ

$$
X^p - X \equiv \prod_{i=0}^{p-1} (X - i) \mod p \mathbf{Z}[X]
$$

trong vành đa thức $ \mathbf{Z}[X] $.

Công thức (2) cũng có thể được viết là

$$
X^{p-1} - 1 \equiv \prod_{i=1}^{p-1} (X - i) \mod p \mathbf{Z}[X]
$$

Đặc biệt với $ X = 0 $ ta thu được (« công thức Wilson »)

$$
(p-1)! \equiv -1 \mod p
$$

### 2. Các mở rộng đại số của một trường hữu hạn

#### Mệnh đề 3 {#alg-v-s12-prop-3 .statement}

— *Cho $ K $ là một trường hữu hạn có $ q $ phần tử, $ \Omega $ là một mở rộng đóng đại số của $ K $ và $ m $ là một số nguyên $ \geqslant 1 $.
a) Tồn tại duy nhất một mở rộng con $ K_m $ của $ \Omega $ có bậc $ m $ trên $ K $.
b) Trường $ K_m $ có $ q^m $ phần tử và là tập hợp các phần tử bất động của tự đẳng cấu $ x \mapsto x^{q^m} $ của $ \Omega $.
c) Ta có $ K_m = K(\zeta) $ với mọi phần tử sinh $ \zeta $ của nhóm cyclic $ K_m^* $.
Cho $ p $ là đặc số của $ K $ và $ f $ là bậc của $ K $ trên $ \mathbf{F}_p $. Ta có $ q^m = p^{fm} $ và do đó ánh xạ $ x \mapsto x^{q^m} $ là một tự đẳng cấu của trường hoàn hảo $ \Omega $ (V, p. 7, Prop. 4). Vì thế tập hợp $ K_m $ các nghiệm của đa thức $ X^{q^m} - X $ thuộc $ K[X] $ là một trường con của $ \Omega $. Vì đạo hàm của $ X^{q^m} - X $ bằng $ -1 $, mọi nghiệm của đa thức này đều đơn (IV, p. 17, Prop. 7), và do đó $ K_m $ có $ q^m $ phần tử. Suy ra $ [K_m : K] = m $.

Bây giờ cho L là một mở rộng con của $ \Omega $, có bậc $ m $ trên $ K $. Với tư cách là không gian vectơ trên $ K $, $ L $ đẳng cấu với $ K^m $ nên có $ q^m $ phần tử. Do đó ta có $ x^{q^m} = x $ với mọi $ x \in L $ (Mệnh đề 2), do đó $ L \subset K_m $. Vì $[L : K] = [K_m : K] = m$, cuối cùng suy ra $ L = K_m $.

Vậy ta đã chứng minh các khẳng định $ a) $ và $ b) $, còn $ c) $ là tầm thường.

#### Hệ quả {#alg-v-s12-n2-cor-1 .statement}

— *Cho $ K $ là một trường hữu hạn và $ \Omega $ là một mở rộng đóng đại số của $ K $. Bao đóng đại số tương đối $ \overline{K} $ của $ K $ trong $ \Omega $ gồm có () và các căn của đơn vị và là một bao đóng đại số của $ K $.*

Ta biết $ K $ là một bao đóng đại số của $ K $ (V, p. 22, Ví dụ 2) và hiển nhiên mọi nghiệm của đơn vị trong $ \Omega $ đều thuộc $ K $. Hơn nữa, với $ x \neq 0 $ trong $ \overline{K} $, có bậc $ m $ trên $ K $, nếu $ K $ có $ q $ phần tử thì trường $ K(x) $ có $ q^m $ phần tử, do đó $ x^{q^m - 1} = 1 $, và vì thế $ x $ là một nghiệm của đơn vị trong $ \Omega $.

Cho $ p $ là một số nguyên tố và gọi $ \mathbf{F}_p = \mathbf{Z}/p\mathbf{Z} $ là trường có $ p $ phần tử. Chọn một bao đóng đại số $ \Omega $ của $ \mathbf{F}_p $, sự tồn tại của nó suy ra từ định lý của Steinitz (V, p. 23, Th. 2). Gọi $ f $ là một số nguyên dương và $ q = p^f $. Theo Mệnh đề 3 tồn tại một trường con duy nhất của $ \Omega $ có bậc $ f $ trên $ \mathbf{F}_p $; ta sẽ ký hiệu nó bởi $ \mathbf{F}_q(\Omega) $ hoặc, do lạm dụng ký hiệu, bởi $ \mathbf{F}_q $. Đó là trường con mở rộng duy nhất của $ \Omega $ có bậc $ f $ trên $ \mathbf{F}_p $. Đó là trường con duy nhất của $ \Omega $ có lực lượng $ q $, và mọi trường có lực lượng $ q $ đều đẳng cấu (không một cách chính tắc) với $ \mathbf{F}_q $ (Hệ quả của Mệnh đề 2). Chú ý rằng $ \mathbf{F}_q $ gồm các $ x $ thuộc $ \Omega $ sao cho $ x^q = x $ và rằng $ F, \subset \mathbf{F}_{q'} $ khi và chỉ khi $ q' $ là một lũy thừa của $ q $.

#### Mệnh đề 4 {#alg-v-s12-prop-4 .statement}

— *Cho $ \mathbf{K} $ là một trường hữu hạn có $ q $ phần tử và $ \mathbf{K}_m $ là một mở rộng bậc hữu hạn $ m $ của $ K $.

a) Trường $ \mathbf{K}_m $ là một mở rộng Galois của $ K $ mà nhóm Galois là nhóm cyclic cấp $ m $ sinh bởi tự đẳng cấu $ \sigma_q : x \mapsto x^q $.

b) Với mỗi $ x \in \mathbf{K}_m $, chuẩn của $ x $ đối với $ K $ bằng $ x^{(q^m - 1)/(q - 1)} $.

c) Mọi phần tử của $ K $ đều là vết (resp. chuẩn) của một phần tử của $ \mathbf{K}_m $.*

Cho $ \Gamma $ là nhóm cyclic các tự đẳng cấu của $ \mathbf{K}_m $ sinh bởi $ \sigma_q $. Trường bất biến của $ \Gamma $ gồm các phần tử $ x $ của $ \mathbf{K}_m $ sao cho $ x^q = x $, do đó bằng $ K $. Vậy $ \mathbf{K}_m $ là một mở rộng Galois của $ K $ với nhóm Galois $ \Gamma $, và nhóm sau có cấp bằng $[K_m : K] = m$ (V, p. 66, Định lý 3). Do đó suy ra $ a) $.

Ta có $ \Gamma = \{1, \sigma_q, \sigma_q^2, \ldots, \sigma_q^{m-1}\} $; do đó chuẩn của một phần tử $ x $ của $ \mathbf{K}_m $ đối với $ K $ là $ N(x) = \prod_{i=0}^{m-1} \sigma_q^i(x) = x^{1 + q + \cdots + q^{m-1}} $ và ta có $ 1 + q + \cdots + q^{m-1} = \frac{q^m - 1}{q - 1} $. Điều này chứng minh b). Cho $ \xi $ là một phần tử sinh của nhóm cyclic $ \mathbf{K}_m^* $; ảnh của chuẩn $ N : \mathbf{K}_m^* \to K^* $ là nhóm con cyclic của $ K^* $ được sinh bởi phần tử $ \xi = N(\xi) = \xi^{(q^m - 1)/(q - 1)} $; vì $ \xi $ có cấp $ q^m - 1 $, nên $ \xi $ có cấp $ q - 1 $, và do đó sinh ra $ K^* $. Điều này chứng minh rằng mọi phần tử khác không của K đều là chuẩn của một phần tử khác không của K; hơn nữa, ta có $ 0 = N(0) $.

Sau cùng, vì $ K_m $ là một mở rộng đại số tách được của K, vết là một dạng tuyến tính khác không trên không gian vectơ $ K_m $ trên K (V, p. 49, Hệ quả) ; do đó mọi phần tử của K đều là vết của một phần tử của $ K_m $.

### 3. Nhóm Galois của bao đóng đại số của một trường hữu hạn

Cho $ S \neq \{1\} $ là một tập hợp các số nguyên $ \geq 1 $ ổn định đối với phép nhân ; ta sẽ sắp thứ tự nó bởi quan hệ « m chia hết n ». Khi m chia hết n, ta có $ m\mathbf{Z} \supset n\mathbf{Z} $, do đó có một đồng cấu chính tắc $ \pi_{m,n} $ của vành $ \mathbf{Z}/n\mathbf{Z} $ lên vành $ \mathbf{Z}/m\mathbf{Z} $. Ta ký hiệu bởi $ A(S) $ giới hạn ngược của hệ ngược các vành $ (\mathbf{Z}/m\mathbf{Z}, \pi_{m,n}) $ được đánh chỉ số bởi S. Mỗi tập hợp hữu hạn $ \mathbf{Z}/m\mathbf{Z} $ được trang bị tôpô rời rạc và $ A(S) $ được trang bị tôpô cảm sinh bởi tôpô của tích $ \prod_{n \in S} (\mathbf{Z}/n\mathbf{Z}) $.

Khi đó $ A(S) $ là một vành tôpô compắc (Gen. Top. I, p. 64, Mệnh đề 8). Ta thấy ngay rằng đồng cấu vành duy nhất $ \varphi $ từ $ \mathbf{Z} $ vào $ A(S) $ là đơn ánh và có ảnh trù mật ; *ta sẽ đồng nhất $ \mathbf{Z} $ với ảnh của nó dưới $ \varphi $ trong $ A(S) $*. Đối với tôpô cảm sinh trên $ \mathbf{Z} $ bởi tôpô của $ A(S) $, *các tập hợp $ m\mathbf{Z} $ (với $ m \in S $) tạo thành một cơ sở các lân cận của 0*.

Khi $ S = \mathbf{N}^* $, $ A(S) $ được viết là $ \hat{\mathbf{Z}} $. Khi S gồm các lũy thừa của một số nguyên tố $ l $, $ A(S) $ được viết là $ \mathbf{Z}_l $ và được gọi là « vành các số nguyên I-adic ». Do đó ta có

$$
\hat{\mathbf{Z}} = \lim_{\leftarrow m \geq 1} \mathbf{Z}/m\mathbf{Z} , \quad \mathbf{Z}_l = \lim_{\leftarrow n \geq 0} \mathbf{Z}/l^n\mathbf{Z} .
$$

Khi S và T là hai tập hợp số nguyên ổn định đối với phép nhân sao cho $ S \supset T $, ta có một phép chiếu tự nhiên $ A(S) \to A(T) $ là một đồng cấu liên tục của các vành tôpô. Đặc biệt, với mọi số nguyên tố $ l $ ta có một đồng cấu liên tục $ \mathbf{Z} \to \mathbf{Z}_l $. Từ đó ta thu được một đồng cấu liên tục

$$
\hat{\mathbf{Z}} \to \prod_l \mathbf{Z}_l
$$

(tích lấy trên mọi số nguyên tố) ; đây là một *đẳng cấu của các vành tôpô*, như suy ra từ việc chuyển sang giới hạn ngược trong I, p. 112, Mệnh đề 11.

Cho K là một trường hữu hạn có q phần tử và K là một bao đóng đại số của K. Với mọi số nguyên $ m \geq 1 $ ta ký hiệu bởi $ K_m $ trường con duy nhất của K có bậc m trên K (Mệnh đề 3). Ta có $ \overline{K} = \bigcup_{m \geq 1} K_m $. Hơn nữa ta ký hiệu bởi $ \sigma_q $ tự đẳng cấu $ x \mapsto x^q $ của trường hoàn hảo $ \overline{K} $; nó được gọi là *tự đẳng cấu Frobenius* của K (đối với K).

#### Mệnh đề 5 {#alg-v-s12-prop-5 .statement}

— Tồn tại một đẳng cấu duy nhất của các nhóm tôpô $ \pi_K : \mathbf{Z} \to \mathrm{Gal}(\bar{K}/K) $ sao cho $ \pi_K(1) = \sigma_q $.

Cho $ \Gamma $ là nhóm con của $ \mathrm{Gal}(\bar{K}/K) $ sinh bởi $ \sigma_q $. Với mọi số nguyên $ m > 0 $ ta có $ \sigma_q^m(x) = x^{q^m} $ với mọi $ x \in \bar{K} $, do đó tập hợp các điểm bất động của $ \sigma_q^m $ bằng $ K $. Vì $ K \neq \bar{K} $, ta có $ \sigma_q^m \neq 1 $. Vậy tồn tại một đẳng cấu $ \pi_0 $ của $ \mathbf{Z} $ lên $ \Gamma $ gửi 1 tới $ \sigma_q $.

Trường bất biến của $ \Gamma $ gồm các $ x \in K $ sao cho $ x^q = x $, nên bằng $ K $. Do đó (V, p. 67, Bổ đề 2) nhóm $ \Gamma $ là trù mật trong $ \mathrm{Gal}(\bar{K}/K) $. Vì mọi mở rộng con của $ \bar{K} $ có bậc hữu hạn trên $ K $ đều là một trong các trường $ K_m $, các nhóm con $ \mathrm{Gal}(\bar{K}/K_m) $ tạo thành một hệ cơ bản các lân cận của 1 trong $ \mathrm{Gal}(\bar{K}/K) $. Rõ ràng $ \Gamma \cap \mathrm{Gal}(\bar{K}/K_m) $ là nhóm cyclic sinh bởi $ \sigma_q^m $, do đó bằng $ \pi_0(m\mathbf{Z}) $.

Từ các nhận xét ở trên về tôpô của $ \mathbf{Z} $, đẳng cấu $ \pi_0 : \mathbf{Z} \to \Gamma $ mở rộng theo một cách duy nhất thành một đẳng cấu của các nhóm tôpô $ \pi_K : \mathbf{Z} \to \mathrm{Gal}(\bar{K}/K) $.

Cho $ m \geq 1 $ là một số nguyên; hiển nhiên tự đẳng cấu Frobenius của $ \bar{K} $ đối với $ K $ là $ \sigma_q^m $. Do đó ta thu được quan hệ

$$
\pi_{K_m}(a) = \pi_K(ma) \quad \text{với } a \in \mathbf{Z}.
$$

### 4. Các đa thức cyclotomic trên một trường hữu hạn

Cho $ K $ là một trường hữu hạn có $ q $ phần tử, $ n \geq 1 $ là một số nguyên không chia hết cho đặc số $ p $ của $ K $ và $ R_n $, một mở rộng cyclotomic bậc $ n $ của $ K $ (V, p. 81). Ta biết rằng nhóm $ \mu_n(R_n) = \mu_n $ các căn bậc $ n $ của đơn vị trong $ R_n $ là cyclic cấp $ n $, rằng $ R_n = K(\mu_n) $ và rằng tồn tại một đơn cấu

$$
\varphi_n : \mathrm{Gal}(R_n/K) \to (\mathbf{Z}/n\mathbf{Z})^*
$$

sao cho $ \sigma(\zeta) = \zeta^j $ với $ \sigma \in \mathrm{Gal}(R_n/K) $, $ \zeta \in \mu_n $ và $ j \in \varphi_n(\sigma) $.

Hơn nữa, nếu $ f $ là bậc của $ R_n $ trên $ K $, thì nhóm Galois của $ R_n $ trên $ K $ là tuần hoàn cấp $ f $, sinh bởi tự đẳng cấu $ \sigma_q : x \mapsto x^q $ (V, p. 95, Prop. 4). Ta lập tức có:

#### Mệnh đề 6 {#alg-v-s12-prop-6 .statement}

— Ảnh qua $ \varphi_n $ của tự đẳng cấu Frobenius $ \sigma_q $ là lớp thặng dư của $ q \mod n $.

Vì vậy, có tính đến Mệnh đề 6 của V, p. 84 :

#### Hệ quả {#alg-v-s12-n4-cor-1 .statement}

— Bậc của $ R_n $ trên $ K $ là số nguyên nhỏ nhất $ f \geq 1 $ sao cho $ q^f \equiv 1 \pmod{n} $. Để đa thức cyclotomic $ \Phi_n $ là bất khả quy trên $ K $ thì điều kiện cần và đủ là nhóm $(\mathbf{Z}/n\mathbf{Z})^*$ phải được sinh bởi lớp thặng dư của $q$ modulo $n$.

#### Ví dụ 1 {#alg-v-s12-n4-exa-1 .statement}

Đa thức $\Phi_3(X) = X^2 + X + 1$ là bất khả quy trong $F_q[X]$ khi và chỉ khi $q \equiv 2 \pmod{3}$. Tương tự, $\Phi_4(X) = X^2 + 1$ là bất khả quy trong $F_q[X]$ khi và chỉ khi $q \equiv 3 \pmod{4}$ và đối với $\Phi_5 = X^4 + X^3 + X^2 + X + 1$, điều kiện bất khả quy được viết là $q \equiv 2,\ 3 \pmod{5}$.

#### Ví dụ 2 {#alg-v-s12-n4-exa-2 .statement}

Ta có $5^2 \equiv 1 \pmod{12}$, do đó lớp thặng dư của 5 (mod 12) không sinh $(\mathbf{Z}/12\mathbf{Z})^*$. Vì vậy đa thức $\Phi_{12}(X) = X^4 - X^2 + 1$ không bất khả quy trong $F_5[X]$; thực ra ta có
$$
\Phi_5(X) = (X^2 + 2X - 1)(X^2 - 2X - 1)
$$
trong $F_5[X]$.

### Bài tập {#alg-v-s12-exercises}

Xem [các bài tập cho § 12](exercises/s12/).
