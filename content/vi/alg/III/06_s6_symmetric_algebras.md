---
book: alg
book_title: Algebra
chapter: III
chapter_title: TENSOR ALGEBRAS, EXTERIOR ALGEBRAS, SYMMETRIC ALGEBRAS
section: 6
section_title: Symmetric algebras
lang: vi
source: alg-i-iii
source_edition: 1998, Springer
pdf_pages: 0521-0530, 0656-0657
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF THE SYMMETRIC ALGEBRA OF A MODULE
      page: 0
      pdf_page: 521
    - "no": 2
      title: FUNCTORIAL PROPERTIES OF THE SYMMETRIC ALGEBRA
      page: 0
      pdf_page: 522
    - "no": 3
      title: n-th symmetric power of a module and symmetric multilinear mappings
      page: 0
      pdf_page: 524
    - "no": 4
      title: EXTENSION OF THE RING OF SCALARS
      page: 0
      pdf_page: 526
    - "no": 5
      title: DIRECT LIMIT OF SYMMETRIC ALGEBRAS
      page: 0
      pdf_page: 527
    - "no": 6
      title: SYMMETRIC ALGEBRA OF A DIRECT SUM. SYMMETRIC ALGEBRA OF A FREE MODULE. SYMMETRIC ALGEBRA OF A GRADED MODULE
      page: 0
      pdf_page: 527
statements: 17
exercises: 5
content_sha256: b0dd88bf19e9112fb553cd0fd8657415315aea872396765590b701bd3c87c0ed
translated_from: content/en/alg/III/06_s6_symmetric_algebras.md
source_content_sha256: 1c670a39292dbe1a46418f9f047277820d0abc0685853a99b28c564dad51b592
translation_model: gpt-5-6-mini, gpt-5.4-mini
translation_run: translate-vi-136a3468
glossary_version: 34
glossary_terms_sha256: d6dbfd0c638080e4c642c8c7c7e2fbc604abf11b2de1f9f15f1a38a2efbc3bca
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 6. ĐẠI SỐ ĐỐI XỨNG

### 1. ĐỊNH NGHĨA ĐẠI SỐ ĐỐI XỨNG CỦA MỘT MÔĐUN

#### Định nghĩa 1 {#alg-iii-s6-def-1 .statement}

*Cho A là một vành giao hoán và M là một A-môđun. Đại số đối xứng của M, ký hiệu là S(M), hoặc Sym(M), hoặc S_A(M), là đại số thương trên A của đại số tenxơ T(M) theo iđêan hai phía $ \mathfrak{J}' $ (cũng ký hiệu là $ \mathfrak{J}'_M $) sinh bởi các phần tử $ xy - yx = x \otimes y - y \otimes x $ của T(M), trong đó x và y chạy qua M.*

Vì iđêan $ \mathfrak{J}' $ được sinh bởi các phần tử thuần nhất có bậc 2, nên nó là một iđêan phân bậc (II, § 11, no. 3, Mệnh đề 2); ta viết $ \mathfrak{J}'_n = \mathfrak{J}' \cap T^n(M) $; khi đó đại số S(M) được phân bậc bởi phép phân bậc (gọi là chính tắc) gồm các $ S^n(M) = T^n(M)/\mathfrak{J}'_n $. Bây giờ $ \mathfrak{J}'_0 = \mathfrak{J}'_1 = \{0\} $ và do đó $ S^0(M) $ được đồng nhất một cách chính tắc với A và $ S^1(M) $ với $ T^1(M) = M $; từ đây về sau ta sẽ luôn thực hiện các sự đồng nhất này và ký hiệu bởi $ \phi' $ hoặc $ \phi'_M $ đơn ánh chính tắc $ M \to S(M) $.

#### Mệnh đề 1 {#alg-iii-s6-prop-1 .statement}

*Đại số S(M) là giao hoán.*

Theo định nghĩa $ \phi'(x)\phi'(y) = \phi'(y)\phi'(x) $ với $ x, y $ trong M và, vì các phần tử $ \phi'(x) $, khi x chạy qua M, sinh ra S(M), kết luận suy ra từ § 1, no. 7.

#### Mệnh đề 2 {#alg-iii-s6-prop-2 .statement}

*Cho E là một đại số trên A và $ f : M \to E $ là một ánh xạ A-tuyến tính thỏa mãn*
$$(1)$$
$$ f(x)f(y) = f(y)f(x) \text{ với mọi } x, y \text{ trong } M. $$
*Tồn tại một và chỉ một đồng cấu đại số trên A $ g : S(M) \to E $ sao cho $ f = g \circ \phi' $.*

Nói cách khác, $ (S(M), \phi') $ là một nghiệm của *bài toán ánh xạ phổ quát* (*Lý thuyết tập hợp*, IV, § 3, no. 1), trong đó $ \Sigma $ là loài cấu trúc đại số trên A, các ánh xạ $ \alpha $ là các ánh xạ tuyến tính của A-môđun M vào một đại số trên A thỏa mãn (1).

Tính duy nhất của g suy ra từ sự kiện $ \phi'(M) = M $ sinh ra S(M). Để chứng minh sự tồn tại của g, chú ý rằng theo § 5, No. 1, Mệnh đề 1 tồn tại một đồng cấu đại số trên A $ g_1 : T(M) \to E $ sao cho $ f = g_1 \circ \phi; $ tất cả những gì cần chứng minh là $ g_1 $ bằng không trên iđêan $ \mathfrak{J}' $, vì khi đó, nếu $ p : T(M) \to S(M) = T(M)/\mathfrak{J}' $ là đồng cấu chính tắc, ta có thể viết $ g_1 = g \circ p $, trong đó $ g : S(M) \to E $ là một đồng cấu đại số, và kết luận sẽ suy ra từ sự kiện rằng $ p \circ \phi = \phi' $. Bây giờ hạt nhân của $ g_1 $ là một iđêan hai phía mà, theo (1) và quan hệ $ g_1 \circ \phi = f $, chứa các phần tử $ x \otimes y - y \otimes x $ với $ x, y $ trong $ M $. Điều này hoàn tất chứng minh.

#### Nhận xét {#alg-iii-s6-n1-rem-1 .statement}

(1) Giả sử rằng $ E $ là một đại số trên $ A $ phân bậc kiểu $ \mathbf{Z} $, với phép phân bậc $ (E_n) $, và cũng giả sử rằng ánh xạ tuyến tính $ f $ (được giả thiết thỏa mãn (1)) là sao cho
(2)
$$
f(M) \subset E_1.
$$
Khi đó quan hệ $ g(x_1 x_2 \ldots x_p) = f(x_1) f(x_2) \ldots f(x_p) $ với các $ x_i \in M $ cho thấy rằng $ g(S^p(M)) \subset E_p $ với mọi $ p \geq 0 $ và do đó $ g $ là một đồng cấu đại số phân bậc.

(2) Mọi phần tử của $ S(M) $ là một tổng các tích có dạng $ x_1 x_2 \ldots x_n $, trong đó các $ x_i $ thuộc về $ M $; cần chú ý không nhầm lẫn các tích như vậy lấy trong $ S(M) $ với các tích tương tự lấy trong $ T(M) $.

(3) Nếu $ n!.1 $ khả nghịch trong $ A $, thì $ A $-môđun $ S^n(M) $ được sinh bởi các phần tử có dạng $ x^n $, với $ x \in M $; điều này suy ra từ nhận xét trên và I, § 8, no. 2, Mệnh đề 2.

### 2. CÁC TÍNH CHẤT HÀM CỦA ĐẠI SỐ ĐỐI XỨNG

#### Mệnh đề 3 {#alg-iii-s6-prop-3 .statement}

*Cho $ A $ là một vành giao hoán, $ M $ và $ N $ là hai $ A $-môđun và $ u : M \to N $ là một ánh xạ $ A $-tuyến tính. Tồn tại duy nhất một đồng cấu đại số $ A $-môđun $ u' : S(M) \to S(N) $ sao cho biểu đồ*

$$
\begin{array}{ccc}
M & \xrightarrow{u} & N \\
\downarrow \phi'_M & & \downarrow \phi'_N \\
S(M) & \xrightarrow{u'} & S(N)
\end{array}
$$

*giao hoán. Hơn nữa, $ u' $ là một đồng cấu đại số phân bậc.*

Sự tồn tại và tính duy nhất của $ u' $ suy ra từ no. 1, Mệnh đề 2 áp dụng cho đại số giao hoán $ S(N) $ và $ f = \phi'_N \circ u : M \to S(N) $; vì
$$
f(M) \subset S^1(N) = N,
$$
việc $ u' $ là một đồng cấu đại số phân bậc suy ra từ no. 1, *Nhận xét* 1.

Đồng cấu $ u' $ của Mệnh đề 3 từ nay sẽ được ký hiệu bởi $ S(u) $. Nếu $ P $ là một $ A $-môđun và $ v : N \to P $ là một ánh xạ $ A $-tuyến tính, thì
$$
S(v \circ u) = S(v) \circ S(u)
$$

vì $ S(v) \circ S(u) $ là một đồng cấu đại số làm cho biểu đồ sau giao hoán

$$
\begin{array}{ccc}
M & \xrightarrow{v \circ u} & P \\
\downarrow \phi'_M & & \downarrow \phi'_P \\
S(M) & \xrightarrow{S(v) \circ S(u)} & S(P)
\end{array}
$$

Vì $ S(M) $ chứa $ M = S^1(M) $, $ S(u) $ đôi khi được gọi là *phần mở rộng chính tắc* của $ u $ lên $ S(M) $. Hạn chế $ S^n(u): S^n(M) \to S^n(N) $ thỏa mãn
$$
S^n(u)(x_1 x_2 \ldots x_n) = u(x_1) u(x_2) \ldots u(x_n)
$$
trong đó $ x_i \in M $, vì $ S(u) $ là một đồng cấu đại số và $ S^1(u) = u $; hạn chế $ S^0(u) $ lên $ A $ là ánh xạ đồng nhất. Chú ý rằng $ S^n(u) $ có thể thu được từ $ T^n(u): T^n(M) \to T^n(N) $ bằng cách chuyển qua các thương.

#### Mệnh đề 4 {#alg-iii-s6-prop-4 .statement}

*Nếu $ u: M \to N $ là một ánh xạ $ A $-tuyến tính toàn ánh, thì đồng cấu $ S(u): S(M) \to S(N) $ là toàn ánh và hạt nhân của nó là iđêan của $ S(M) $ sinh bởi hạt nhân $ P \subset M \subset S(M) $ của $ u $.*

Ta viết $ v = T(u): T(M) \to T(N) $; ta biết (\S 5, no. 2, Mệnh đề 3) rằng $ v $ là toàn ánh và do đó suy ra từ các định nghĩa rằng $ v(\mathfrak{J}'_M) = \mathfrak{J}'_N $; nếu $ \mathfrak{R} $ là hạt nhân của $ v $, thì $ v^{-1}(\mathfrak{J}'_N) = \mathfrak{R} + \mathfrak{J}'_M $. Vì $ S(u): T(M)/\mathfrak{J}'_M \to T(N)/\mathfrak{J}'_N $ được dẫn xuất từ $ v $ bằng cách chuyển qua các thương, nó là một đồng cấu toàn ánh có hạt nhân là $ \mathfrak{R}' = (\mathfrak{R} + \mathfrak{J}'_M)/\mathfrak{J}'_M $. Vì $ \mathfrak{R} $ được sinh bởi hạt nhân $ P $ của $ u $ (\S 5, no. 2), nên $ \mathfrak{R}' $ cũng vậy.

Nếu $ u: M \to N $ là một ánh xạ tuyến tính *đơn ánh*, thì không phải lúc nào cũng đúng rằng $ S(u) $ là một ánh xạ đơn ánh (Bài tập 1). Tuy nhiên điều này đúng khi $ u $ là một đơn ánh sao cho $ u(M) $ là một *nhân tử trực tiếp* trong $ N $ và khi đó ảnh của $ S(u) $ (đẳng cấu với $ S(M) $) là một *nhân tử trực tiếp* của $ S(N) $; chứng minh cũng giống như chứng minh của các khẳng định tương tự đối với $ T(u) $ (\S 5, no. 2) khi thay $ T $ bởi $ S $.

#### Mệnh đề 5 {#alg-iii-s6-prop-5 .statement}

*Cho $ N $ và $ P $ là hai môđun con của một $ A $-môđun $ M $ sao cho tổng của chúng $ N + P $ là một nhân tử trực tiếp trong $ M $ và giao của chúng $ N \cap P $ là một nhân tử trực tiếp trong $ N $ và trong $ P $. Khi đó các đồng cấu $ S(N) \to S(M) $, $ S(P) \to S(M) $ và*
$$
S(N \cap P) \to S(M),
$$
*là các mở rộng chính tắc của các đơn ánh chính tắc, là đơn ánh; nếu $ S(N) $, $ S(P) $ và $ S(N \cap P) $ được đồng nhất với các đại số con của $ S(M) $ nhờ các đồng cấu này, thì*
$$
S(N \cap P) = S(N) \cap S(P).
$$
(4)

Chứng minh quy về chứng minh của \S 5, no. 2, Mệnh đề 4 bằng cách thay $ T $ bởi $ S $ trong toàn bộ. Các giả thiết của Mệnh đề 5 luôn thỏa mãn đối với các môđun con *tùy ý* $ N, P $ của $ M $ khi $ A $ là một trường.

#### Hệ quả {#alg-iii-s6-n2-cor-1 .statement}

*Cho K là một trường giao hoán và M là một không gian vectơ trên K. Với mọi phần tử $ z \in S(M) $ tồn tại một không gian vectơ N nhỏ nhất của M sao cho $ z \in S(N) $ và N là hữu hạn chiều.*

Chứng minh được dẫn xuất từ chứng minh của § 5, no. 2, Hệ quả của Mệnh đề 4 bằng cách thay T bởi S trong toàn bộ.

N được gọi là không gian con vectơ của M *liên kết* với z.

### 3. Lũy thừa đối xứng bậc n của một môđun và các ánh xạ đa tuyến tính đối xứng

Cho X, Y là hai tập hợp và $ n $ là một số nguyên $ \geqslant 1 $. Một *ánh xạ đối xứng* của $ X^n $ vào Y là một ánh xạ bất kỳ $ f : X^n \to Y $ sao cho, với mọi phép hoán vị $ \sigma \in \mathcal{S}_n $ và mọi phần tử $ (x_i) \in X^n $,

$$
f(x_{\sigma(1)}, x_{\sigma(2)}, \ldots, x_{\sigma(n)}) = f(x_1, x_2, \ldots, x_n).
$$

Vì các phép chuyển vị đổi chỗ hai số nguyên liên tiếp sinh ra nhóm $ \mathcal{S}_n $ (I, § 5, no. 7), nên chỉ cần điều kiện (5) đúng khi $ \sigma $ là một phép chuyển vị như vậy.

Khi Y là một *môđun* trên một vành giao hoán A, rõ ràng tập hợp các ánh xạ đối xứng từ $ X^n $ vào Y là một *môđun con* của A-môđun $ Y^{X^n} $ gồm tất cả các ánh xạ từ $ X^n $ vào Y.

#### Mệnh đề 6 {#alg-iii-s6-prop-6 .statement}

*Cho A là một vành giao hoán và M và N là hai A-môđun. Nếu với mỗi ánh xạ A-tuyến tính $ g : S^n(M) \to N $ ($ n \geqslant 1 $) được liên kết ánh xạ n-tuyến tính*

$$
(x_1, x_2, \ldots, x_n) \mapsto g(x_1 x_2 \ldots x_n)
$$

*(trong đó ở vế phải tích được lấy trong đại số $ S(M) $), ta thu được một ánh xạ A-tuyến tính song ánh từ A-môđun $ \operatorname{Hom}_A(S^n(M), N) $ lên A-môđun các ánh xạ n-tuyến tính đối xứng từ $ M^n $ vào N.*

Nhắc lại (II, § 3, no. 9) rằng có một song ánh chính tắc của A-môđun $ \operatorname{Hom}_A(T^n(M), N) $ lên A-môđun $ \mathcal{L}_n(M, \ldots, M; N) $ của *tất cả* các ánh xạ n-tuyến tính từ $ M^n $ vào N thu được bằng cách liên kết với mỗi ánh xạ A-tuyến tính $ f : T^n(M) \to N $ ánh xạ n-tuyến tính

$$
\tilde{f} : (x_1, x_2, \ldots, x_n) \mapsto f(x_1 \otimes x_2 \otimes \cdots \otimes x_n).
$$

Mặt khác, các ánh xạ A-tuyến tính $ g : S^n(M) \to N $ tương ứng một-một với các ánh xạ A-tuyến tính $ f : T^n(M) \to N $ sao cho $ f $ bằng không *trên* $ \mathfrak{J}'_n $, bằng cách liên kết với $ g $ ánh xạ $ f = g \circ p_n $, trong đó

$$
p_n : T^n(M) \to S^n(M) = T^n(M)/\mathfrak{J}'_n
$$

là đồng cấu chính tắc (II, § 2, no. 1, Định lý 1). Nhưng vì $ \mathfrak{J}'_n $ là một tổ hợp tuyến tính của các phần tử có dạng

$$
(u_1 \otimes u_2 \otimes \cdots \otimes u_p) \otimes (x \otimes y - y \otimes x) \otimes (v_1 \otimes \cdots \otimes v_{n-p-2})
$$

lũy thừa đối xứng bậc n

(x, y, u_i, v_j thuộc M), việc nói rằng hàm f có dạng g \circ p_n có nghĩa là hàm n-tuyến tính tương ứng $ \bar{f} $ thỏa mãn quan hệ

$$
\bar{f}(u_1, \ldots, u_p, x, y, v_1, \ldots, v_{n-p-2}) = \bar{f}(u_1, \ldots, u_p, y, x, v_1, \ldots, v_{n-p-2});
$$

nói cách khác, theo điều đã thấy ở trên, điều này có nghĩa là $ \bar{f} $ là *đối xứng*; do đó có mệnh đề, khi tính đến sự kiện rằng

$$
p_n(x_1 \otimes x_2 \otimes \cdots \otimes x_n) = x_1 x_2 \ldots x_n
$$

với $ x_i \in M $.

A-môđun $ S^n(M) $ được gọi là *lũy thừa đối xứng bậc n* của M. Với mỗi đồng cấu A-môđun $ u : M \to N $, ánh xạ $ S^n(u) : S^n(M) \to S^n(N) $ trùng với $ S(u) $ trên $ S^n(M) $ được gọi là *lũy thừa đối xứng bậc n của u*.

#### Nhận xét {#alg-iii-s6-n3-rem-1 .statement}

Cho $ \sigma $ là một phép hoán vị trong $ \mathfrak{S}_n $; vì ánh xạ

$$
(x_1, x_2, \ldots, x_n) \mapsto x_{\sigma^{-1}(1)} \otimes x_{\sigma^{-1}(2)} \otimes \cdots \otimes x_{\sigma^{-1}(n)}
$$

từ $ M^n $ vào $ T^n(M) $ là A-đa tuyến tính, nó có thể được viết duy nhất dưới dạng

$$
(x_1, \ldots, x_n) \mapsto u_\sigma(x_1 \otimes x_2 \otimes \cdots \otimes x_n),
$$

trong đó $ u_\sigma $ là một *tự đồng cấu* của A-môđun $ T^n(M) $, cũng được ký hiệu bởi $ z \mapsto \sigma . z $. Rõ ràng, nếu $ \sigma $ là phần tử đơn vị của $ \mathfrak{S}_n $, $ u_\sigma $ là đồng nhất; mặt khác, viết $ y_i = x_{\sigma^{-1}(i)} $, ta thu được, với mỗi phép hoán vị $ \tau \in \mathfrak{S}_n, y_{\tau^{-1}(i)} = x_{\sigma^{-1}(\tau^{-1}(i))} $ và do đó $ \tau . (\sigma . z) = (\tau \sigma) . z $; nói cách khác, A-môđun $ T^n(M) $ là một *tập hợp* trái $ \mathfrak{S}_n $ dưới phép toán $ (\sigma, z) \mapsto \sigma . z $ (I, § 5, no. 1). Các phần tử của $ T^n(M) $ sao cho $ \sigma . z = z $ với *mọi* $ \sigma \in \mathfrak{S}_n $ được gọi là (phản biến) *tenxơ đối xứng cấp n*; chúng tạo thành một A-môđun con $ S'_n(M) $ của $ T^n(M) $.

Với mọi $ z \in T^n(M) $, ta viết $ s . z = \sum_{\sigma \in \mathfrak{S}_n} \sigma . z $ và gọi $ s . z $ là *phép đối xứng hóa* của tenxơ $ z $; rõ ràng $ s . z $ là một tenxơ đối xứng và do đó $ z \mapsto s . z $ là một tự đồng cấu của $ T^n(M) $ mà ảnh $ S''_n(M) $ được chứa trong $ S'_n(M) $; nói chung, $ S''_n(M) \neq S'_n(M) $ (Bài tập 5). Nếu $ z $ là một tenxơ đối xứng, thì $ s . z = n! z $; do đó *khi n! là khả nghịch trong A*, tự đồng cấu $ z \mapsto (n!)^{-1} s . z $ là một *phép chiếu* của $ T^n(M) $ (II, § 1, no. 8), có ảnh là $ S'_n(M) = S''_n(M) $; hơn nữa hạt nhân của phép chiếu này chính là $ \mathfrak{J}'_n $. Thật vậy, hiển nhiên $ \sigma(\mathfrak{J}'_n) \subset \mathfrak{J}'_n $ với mọi $ \sigma \in \mathfrak{S}_n $ và $ \mathfrak{J}'_n $ theo định nghĩa được sinh bởi các tenxơ $ z - \rho . z $, trong đó $ \rho $ là một phép hoán vị đổi chỗ hai số liên tiếp trong $ \{1, n\} $; ngoài ra, nếu $ \sigma, \tau $ là hai phép hoán vị trong $ \mathfrak{S}_n $, thì $ z - (\sigma \tau) . z = z - \sigma . z + \sigma . (z - \tau . z) $, do đó suy ra (vì mọi phép hoán vị trong $ \mathfrak{S}_n $ là một tích của các phép hoán vị đổi chỗ hai số liên tiếp) rằng $ z - \sigma . z \in \mathfrak{J}'_n $ với mọi $ z \in T^n(M) $ và $ \sigma \in \mathfrak{S}_n $. Vì vậy (luôn giả sử rằng n! là khả nghịch trong A), ta thấy rằng

$$
z - (n!)^{-1} s . z = \sum_{\sigma \in \mathfrak{S}_n} (n!)^{-1} (z - \sigma . z) \in \mathfrak{J}'_n
$$

với mọi $ z \in T^n(M) $, điều này chứng minh mệnh đề của chúng ta.

Khi $ n! $ là khả nghịch trong $ A $, các môđun con $ S'_n(M) $ và $ \mathfrak{g}'_n $ của $ T^n(M) $ do đó là bù nhau và hạn chế vào $ S'_n(M) $ của đồng cấu chính tắc $ T^n(M) \to S^n(M) = T^n(M)/\mathfrak{g}'_n $ là một đẳng cấu $ A $-môđun, cho phép trong trường hợp đang xét đồng nhất các tenxơ đối xứng cấp $ n $ với các phần tử của lũy thừa đối xứng thứ $ n $ của $ M $. Tuy nhiên cần chú ý rằng sự đồng nhất này không tương thích với phép nhân, tích (trong $ T(M) $) của hai tenxơ đối xứng nói chung không phải là đối xứng và do đó không có ảnh trong $ S(M) $ là tích của các ảnh của các tenxơ đối xứng được xét.

### 4. MỞ RỘNG CỦA VÀNH CÁC VÔ HƯỚNG

Cho $ A, A' $ là hai vành giao hoán, $ \rho : A \to A' $ là một đồng cấu vành, $ M $ là một $ A $-môđun, $ M' $ là một $ A' $-môđun và $ f : M \to M' $ là một $ A $-đồng cấu (đối với $ \rho $) của $ M $ vào $ M' $. Ánh xạ hợp thành $ M \xrightarrow{f} M' \xrightarrow{\phi_{M'}} S_{A'}(M') $ là một ánh xạ $ A $-tuyến tính của $ M $ vào đại số giao hoán $ \rho_*(S_A(M')) $; khi đó tồn tại (no. 1, Mệnh đề 2) duy nhất một $ A $-đồng cấu đại số $ f' : S_A(M) \to S_{A'}(M') $ làm cho biểu đồ sau giao hoán

$$
\begin{array}{ccc}
M & \xrightarrow{f} & M' \\
\downarrow \phi_M' & & \downarrow \phi_{M'}' \\
S_A(M) & \xrightarrow{f'} & S_{A'}(M')
\end{array}
$$

Suy ra ngay lập tức rằng nếu $ \sigma : A' \to A'' $ là một đồng cấu vành khác, $ M'' $ là một $ A'' $-môđun, $ g : M' \to M'' $ là một $ A' $-đồng cấu (đối với $ \sigma $) và $ g' : S_{A'}(M') \to S_{A''}(M'') $ là $ A' $-đồng cấu đại số tương ứng, thì đồng cấu đại số $ A $ hợp thành

$$
S_A(M) \xrightarrow{f'} S_{A'}(M') \xrightarrow{g'} S_{A''}(M'')
$$

tương ứng với đồng cấu $ A $ hợp thành $ g \circ f : M \to M'' $ (đối với $ \sigma \circ \rho $).

#### Mệnh đề 7 {#alg-iii-s6-prop-7 .statement}

Cho $ A, B $ là hai vành giao hoán, $ \rho : A \to B $ là một đồng cấu vành và $ M $ là một $ A $-môđun. Mở rộng chính tắc

$$
\psi : S_B(B \otimes_A M) \to B \otimes_A S_A(M)
$$

của ánh xạ $ B $-tuyến tính $ l_B \otimes \phi_M' : B \otimes_A M \to B \otimes_A S_A(M) $ là một đẳng cấu đại số $ B $ phân bậc.

Chứng minh được dẫn xuất từ chứng minh của § 5, no. 3, Mệnh đề 5 bằng cách thay $ T $ bởi $ S $ và $ \phi_M $ bởi $ \phi_M' $.

### 5. GIỚI HẠN TRỰC TIẾP CỦA CÁC ĐẠI SỐ ĐỐI XỨNG

Cho $(A_\alpha, \phi_{\beta\alpha})$ là một hệ trực tiếp có hướng của các vành giao hoán, $(M_\alpha, f_{\beta\alpha})$ là một hệ trực tiếp của các $A_\alpha$-môđun, $A = \lim \rightarrow A_\alpha$ và $M = \lim \rightarrow M_\alpha$. Với $\alpha \leq \beta$, ta dẫn xuất một cách chính tắc từ $A_\alpha$-đồng cấu $f_{\beta\alpha}: M_\alpha \to M_\beta$ một đồng cấu đại số $A_\alpha$ (no. 4, công thức (8)) $f'_{\beta\alpha}: S_{A_\alpha}(M_\alpha) \to S_{A_\beta}(M_\beta)$ và suy ra từ (9) (no. 4) rằng $(S_{A_\alpha}(M_\alpha), f'_{\beta\alpha})$ là một *hệ trực tiếp của các $A_\alpha$-đại số*. Mặt khác, $f_\alpha: M_\alpha \to M$ là đồng cấu $A$ chính tắc; ta dẫn xuất (no. 4, công thức (8)) một đồng cấu đại số $A_\alpha$

$$
f'_\alpha: S_{A_\alpha}(M) \to S_A(M)
$$

và cũng suy ra từ (9) rằng các $f'_\alpha$ cấu thành một hệ trực tiếp các đồng cấu $A_\alpha$.

#### Mệnh đề 8 {#alg-iii-s6-prop-8 .statement}

*Đồng cấu $A$* $f' = \lim \rightarrow f'_\alpha : \lim \rightarrow S_{A_\alpha}(M_\alpha) \to S_A(M)$ *là một đẳng cấu đại số phân bậc.*

Chứng minh giống như của § 5, no. 5, Mệnh đề 6, thay toàn bộ $T$ bằng $S$ và $\phi$ bằng $\phi'$ và lưu ý rằng một giới hạn trực tiếp của các đại số giao hoán là giao hoán.

### 6. ĐẠI SỐ ĐỐI XỨNG CỦA MỘT TỔNG TRỰC TIẾP. ĐẠI SỐ ĐỐI XỨNG CỦA MỘT MÔĐUN TỰ DO. ĐẠI SỐ ĐỐI XỨNG CỦA MỘT MÔĐUN PHÂN BẬC

Cho $A$ là một vành giao hoán, $M = \bigoplus_{\lambda \in L} M_\lambda$ là tổng trực tiếp của một họ các $A$-môđun và $j_\lambda: M_\lambda \to M$ là đơn ánh chính tắc; ta suy ra một đồng cấu $A$-đại số $S(j_\lambda): S(M_\lambda) \to S(M)$. Vì $S(M)$ là giao hoán, có thể áp dụng Mệnh đề 8 của § 4, no. 5, cho các đồng cấu $S(j_\lambda)$ và do đó tồn tại duy nhất một đồng cấu đại số

$$
g: \bigotimes_{\lambda \in L} S(M_\lambda) \to S(M)
$$
(còn được ký hiệu bởi $g_M$) sao cho $S(j_\lambda) = g \circ f_\lambda$ với mọi $\lambda \in L$, trong đó

$$
f_\lambda: S(M_\lambda) \to \bigotimes_{\lambda \in L} S(M_\lambda)
$$

ký hiệu đồng cấu chính tắc.

#### Mệnh đề 9 {#alg-iii-s6-prop-9 .statement}

*Đồng cấu chính tắc* $g$ *(công thức (10))* *là một đẳng cấu đại số phân bậc* (cf. § 4, no. 8, *Nhận xét 1*).

Để chứng minh rằng $g$ là song ánh, ta định nghĩa một đồng cấu đại số

$$
h: S(M) \to \bigotimes_{\lambda \in L} S(M_\lambda)
$$

sao cho $ g \circ h $ và $ h \circ g $ lần lượt là các ánh xạ đồng nhất trên $ S(M) $ và $ \bigotimes_{\lambda \in L} S(M_\lambda) $. Với mỗi $ \lambda \in L $, đặt $ u_\lambda $ là ánh xạ tuyến tính hợp thành
$$
M_\lambda \xrightarrow{\phi'_M} S(M_\lambda) \xrightarrow{f_\lambda} \bigotimes_{\lambda \in L} S(M_\lambda).
$$
Tồn tại duy nhất một ánh xạ $ A $-tuyến tính $ u : M \to \bigotimes_{\lambda \in L} S(M_\lambda) $ sao cho $ u \circ j_\lambda = u_\lambda $ với mọi $ \lambda \in L $. Vì các $ S(M_\lambda) $ là giao hoán, nên tích tenxơ của chúng cũng giao hoán (\S 4, no. 5) và do đó (no. 1, Mệnh đề 2) tồn tại duy nhất một đồng cấu đại số $ h : S(M) \to \bigotimes_{\lambda \in L} S(M_\lambda) $ sao cho $ h \circ \phi'_M = u $; mặt khác, hiển nhiên $ u(M) $ được chứa trong môđun con các phần tử bậc 1 của đại số phân bậc $ \bigotimes_{\lambda \in L} S(M_\lambda) $ và do đó $ h $ là một đồng cấu đại số phân bậc. Với $ x_\lambda \in M_\lambda $,
$$
h(g(u_\lambda(x_\lambda))) = h(g(f_\lambda(\phi'_M(x_\lambda)))) = h(S(j_\lambda)(\phi'_M(x_\lambda))) = h(\phi'_M(j_\lambda(x_\lambda))) = u_\lambda(x_\lambda);
$$
vì các $ u_\lambda(x_\lambda) $ sinh ra đại số $ \bigotimes_{\lambda \in L} S(M_\lambda) $ (\S 4, no. 5, Mệnh đề 8), $ h \circ g $ chắc chắn là ánh xạ đồng nhất. Tương tự,
$$
g(h(\phi'_M(j_\lambda(x_\lambda)))) = g(u_\lambda(x_\lambda)) = g(f_\lambda(\phi'_M(x_\lambda))) = S(j_\lambda)(\phi'_M(x_\lambda)) = \phi'_M(j_\lambda(x_\lambda))
$$
và, vì các phần tử $ \phi'_M(j_\lambda(x_\lambda)) $ sinh ra đại số $ S(M) $, $ g \circ h $ chắc chắn là ánh xạ đồng nhất.

Nhận xét (1) Cho $ N = \bigoplus_{\lambda \in L} N_\lambda $ là tổng trực tiếp của một họ khác các $ A $-môđun với $ L $ làm tập chỉ số và, với mọi $ \lambda \in L $, cho $ v_\lambda : M_\lambda \to N_\lambda $ là một ánh xạ $ A $-tuyến tính, do đó có một ánh xạ $ A $-tuyến tính $ v = \bigoplus_\lambda v_\lambda : M \to N $ (II, \S 1, no. 6, Mệnh đề 6). Khi đó biểu đồ
$$
\begin{array}{ccc}
\bigotimes_{\lambda \in L} S(M_\lambda) & \xrightarrow{g_M} & S(M) \\
\downarrow & & \downarrow S(v) \\
\bigoplus_{\lambda \in L} S(v_\lambda) & \xrightarrow{g_N} & S(N)
\end{array}
$$
là giao hoán, như suy ra từ các định nghĩa (\S 4, no. 5, Hệ quả của Mệnh đề 8).

The A-môđun con của $ \bigotimes_{\lambda \in L} S(M_\lambda) $ mà qua đẳng cấu $ g $ $ S^n(M) $ được đồng nhất có thể được mô tả chính xác hơn. Với mọi tập con hữu hạn $ J $ của $ L $, ta viết $ E_J = \bigotimes_{\lambda \in J} S(M_\lambda) $, sao cho $ \bigotimes_{\lambda \in L} S(M_\lambda) = \varprojlim E_J $ tương ứng với tập có hướng $ \mathcal{F}(L) $ các tập con hữu hạn của $ L $, theo định nghĩa (\S 4, no. 5). Với mọi họ $ \nu = (n_\lambda) \in \mathbf{N}^{(L)} $ (do đó có giá hữu hạn) sao cho $ \sum_{\lambda \in L} n_\lambda = n $ và mọi tập con hữu hạn $ J $ của $ L $ chứa giá của họ $ \nu $, ta viết

$$
S^{J,\nu}(M) = \bigotimes_{\lambda \in J} S^{n_\lambda}(M_\lambda)
$$

sao cho môđun con $ E_{J,n} $ gồm các phần tử bậc $ n $ trong $ E_J $ là *tổng trực tiếp* của các $ S^{J,\nu}(M) $ theo mọi họ $ \nu $ có giá được chứa trong $ J $ và sao cho $ \sum_{\lambda \in L} n_\lambda = n $ (\S 4, no. 7, Mệnh đề 10 và \S 4, no. 8). Theo quy ước, ta viết $ S^{J,\nu}(M) = \{0\} $ cho các họ $ \nu $ có giá không được chứa trong $ J $; khi đó $ E_{J,n} $ cũng có thể được gọi là *tổng trực tiếp* của *mọi* $ S^{J,\nu}(M) $, trong đó $ \nu $ chạy qua tập $ H_n $ gồm *mọi* họ $ \nu = (n_\lambda)_{\lambda \in L} $ sao cho $ \sum_{\lambda \in L} n_\lambda = n $. Vì $ S^0(M_\lambda) $ được đồng nhất với $ A $, rõ ràng cũng vậy, với hai tập con hữu hạn $ J \subset J' $ của $ L $ và một họ $ \nu $ có giá được chứa trong $ J $, ánh xạ chính tắc $ S^{J,\nu}(M) \to S^{J',\nu}(M) $ (hạn chế của ánh xạ chính tắc $ E_J \to E_J $ lên $ S^{J,\nu}(M) $) là *song ánh*. Nếu ta viết, với mọi $ \nu \in H_n $,

$$
S^\nu(M) = \varprojlim S^{J,\nu}(M)
$$

thì thấy rằng, xét đến II, \S 6, no. 2, Mệnh đề 5:

#### Hệ quả {#alg-iii-s6-n6-cor-1 .statement}

*Môđun A* $ S^n(M) $ *là ảnh qua đẳng cấu* (10) *của môđun con của* $ \bigotimes_{\lambda \in L} S(M_\lambda) $ *là tổng trực tiếp của các môđun con* $ S^\nu(M) $ *ứng với mọi họ* $ \nu = (n_\lambda) \in \mathbf{N}^{(L)} $ *sao cho* $ \sum_{\lambda \in L} n_\lambda = n $; *nếu* $ J $ *là giá của* $ \nu $, $ S^\nu(M) $ *đẳng cấu chính tắc với* $ \bigotimes_{\lambda \in J} S^{n_\lambda}(M_\lambda) $.

Nói chung $ S^\nu(M) $, $ \bigotimes_{\lambda \in J} S^{n_\lambda}(M_\lambda) $ và ảnh của chúng trong $ S^n(M) $ được đồng nhất.

#### Định lý 1 {#alg-iii-s6-thm-1 .statement}

*Cho* $ A $ *là một vành giao hoán và* $ M $ *là một* $ A $-*môđun tự do với cơ sở* $ (e_\lambda)_{\lambda \in L} $. *Với mọi ánh xạ* $ \alpha : L \to \mathbf{N} $ *có giá hữu hạn, ta viết*

$$
e^\alpha = \prod_{\lambda \in L} e_\lambda^{\alpha(\lambda)}
$$

(*phép nhân trong đại số giao hoán* $ S(M) $). *Khi* $ \alpha $ *chạy qua tập* $ \mathbf{N}^{(L)} $ *gồm các ánh xạ của* $ L $ *vào* $ \mathbf{N} $, *có giá hữu hạn, thì các* $ e^\alpha $ *lập thành một cơ sở của* $ A $-*môđun* $ S(M) $.

Vì $ M $ là tổng trực tiếp của các $ M_\lambda = Ae_\lambda $, nên chỉ cần chứng minh định lý khi $ L $ thu về một phần tử duy nhất rồi áp dụng Mệnh đề 9. Nhưng khi $ M = Ae $ (*e* là một phần tử tự do), thì $ x \otimes y - y \otimes x = 0 $ với mọi $ x, y $ trong $ M $; do đó iđêan $ \mathfrak{g}' $ bằng không, nên $ T(Ae) = S(Ae) $ và định lý khi đó suy ra từ \S 5, no. 5, Định lý 1.

Bảng nhân của cơ sở (14) được cho bởi

(15)
$$
e^\alpha e^\beta = e^{\alpha + \beta}
$$
trong đó $ \alpha + \beta $ là ánh xạ $ \lambda \mapsto \alpha(\lambda) + \beta(\lambda) $ của $ L $ vào $ \mathbf{N} $. Nói cách khác, cơ sở $ (e^\alpha) $ của $ S(M) $, với luật nhân (15), là đẳng cấu chính tắc với monoid giao hoán tự do $ N^{(L)} $ dẫn xuất từ $ L $; suy ra (\S 2, no. 9) rằng đại số đối xứng $ S(M) $ của một môđun tự do $ M $ có cơ sở với tập chỉ số là $ L $, là đẳng cấu chính tắc với đại số đa thức $ A[(X_\lambda)_{\lambda \in L}] $, trong đó đẳng cấu chính tắc này được xác định bằng cách gửi $ e_\lambda $ tới $ X_\lambda $. Đặc biệt (\S 2, no. 7, Mệnh đề 7), với mọi ánh xạ $ f : L \to E $ của $ L $ vào một $ A $-đại số giao hoán $ E $, tồn tại một và chỉ một đồng cấu $ A $-đại số $ \tilde{f} : S(M) \to E $ sao cho $ \tilde{f}(e_\lambda) = f(\lambda) $.

Nhận xét (2). Các kết quả trên cũng có thể thu được như một hệ quả của các tính chất phổ quát của đại số đa thức và đại số đối xứng, có xét đến II, \S 1, no. 11, Hệ quả 3 của Mệnh đề 17.

#### Hệ quả {#alg-iii-s6-n6-cor-2 .statement}

*Nếu $ M $ là một $ A $-môđun xạ ảnh, thì $ S(M) $ là một $ A $-môđun xạ ảnh.*

Chứng minh giống như của \S 5, no. 5, Hệ quả của Định lý 1, thay $ T $ bằng $ S $.

#### Mệnh đề 10 {#alg-iii-s6-prop-10 .statement}

*Cho $ \Delta $ là một nửa nhóm giao hoán có đơn vị, $ M $ là một $ A $-môđun phân bậc kiểu $ \Delta $ và $ (M_\alpha)_{\alpha \in \Delta} $ là sự phân bậc của nó. Với mỗi cặp có thứ tự $ (\alpha, n) \in \Delta \times \mathbf{N} $, ký hiệu $ S^{\alpha, n}(M) $ là môđun con của $ S^n(M) $ bằng tổng trực tiếp của các môđun con $ \bigotimes_{\lambda \in J} S^{n_\lambda}(M_{\alpha_\lambda}) $, trong đó $ (n_\lambda)_{\lambda \in L} $ chạy qua tập hợp các họ số nguyên $ \geq 0 $ sao cho $ \sum_{\lambda \in L} n_\lambda = n $, $ J $ là giá đỡ của nó và, với mỗi $ (n_\lambda), (\alpha_\lambda)_{\lambda \in J} $ chạy qua tập hợp các họ của $ \Delta^J $ sao cho $ \sum_{\lambda \in J} \alpha_\lambda = \alpha $. Khi đó $ (S^{\alpha, n}(M))_{(\alpha, n) \in \Delta \times \mathbf{N}} $ là sự phân bậc duy nhất kiểu $ \Delta \times \mathbf{N} $ tương thích với cấu trúc đại số trên $ S(M) $ và cảm sinh trên $ M = S^1(M) $ sự phân bậc đã cho.*

Việc $ S(M) $ là tổng trực tiếp của các $ S^{\alpha, n}(M) $ suy ra từ Hệ quả của Mệnh đề 9; phần còn lại của chứng minh giống hệt với phần cuối của chứng minh ở \S 5, no. 5, Mệnh đề 7.

Giả sử cụ thể hơn rằng $ \Delta = \mathbf{Z} $ và cho $ S(M) $ được mang phân bậc toàn phần (kiểu $ \mathbf{Z} $) (II, \S 11, no. 1) tương ứng với sự phân bậc kiểu $ \mathbf{Z} \times \mathbf{N} $ (và do đó cũng kiểu $ \mathbf{Z} \times \mathbf{Z} $) đã định nghĩa ở trên; các phần tử thuần nhất bậc $ n \in \mathbf{Z} $ theo sự phân bậc này vì thế là những phần tử thuộc tổng trực tiếp của các $ S^{q, m}(M) $ với $ q + m = n $. Cho $ f $ là một *thuần nhất* ánh xạ tuyến tính *bậc* 0 của $ A $-môđun phân bậc $ M $ vào một *giao hoán* $ A $-đại số phân bậc $ F $ kiểu $ \mathbf{Z} $; khi đó đồng cấu đại số $ g : S(M) \to F $ sao cho $ f = g \circ \phi_M' $ là một *đồng cấu đại số phân bậc kiểu* $ \mathbf{Z} $, như suy ra từ công thức $ g(x_1 x_2 \ldots x_n) = f(x_1) f(x_2) \ldots f(x_n) $ đối với các $ x_i $ thuần nhất trong $ M $, từ giả thiết về $ f $ và từ định nghĩa của sự phân bậc kiểu $ \mathbf{Z} $ trên $ S(M) $.

### Bài tập {#alg-iii-s6-exercises}

Xem [các bài tập cho § 6](exercises/s6/).
