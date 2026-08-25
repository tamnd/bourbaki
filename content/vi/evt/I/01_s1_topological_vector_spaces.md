---
book: evt
book_title: Topological Vector Spaces
chapter: I
chapter_title: TOPOLOGICAL VECTOR SPACES OVER A VALUED DIVISION RING
section: 1
section_title: Topological vector spaces
lang: vi
source: evt-i-v
pdf_pages: 0009-0019, 0030-0033
extraction: ocr
subsections:
    - "no": 1
      title: Definition of a topological vector space
      page: 0
      pdf_page: 9
    - "no": 2
      title: Normed spaces on a valued division ring
      page: 3
      pdf_page: 11
    - "no": 3
      title: Vector subspaces and quotient spaces of a topological vector space; products of topological vector spaces; topological direct sums of subspaces
      page: 4
      pdf_page: 12
    - "no": 4
      title: Uniform structure and completion of a topological vector space
      page: 5
      pdf_page: 13
    - "no": 5
      title: Neighbourhoods of the origin in a topological vector space over a valued division ring
      page: 6
      pdf_page: 14
    - "no": 6
      title: Criteria of continuity and equicontinuity
      page: 8
      pdf_page: 16
    - "no": 7
      title: Initial topologies of vector spaces
      page: 9
      pdf_page: 17
statements: 27
exercises: 14
content_sha256: 097411c6adcad81a739a31e32d408e11f6f00b5dbd17505028b8384a58f763ee
translated_from: content/en/evt/I/01_s1_topological_vector_spaces.md
source_content_sha256: f0fe7522d5d70ea7ec263b1a50c064ff88e7fa4c451682bf647a4d2358aa9dc4
translation_model: gpt-5-6, gpt-5-6-mini
translation_run: translate-vi-52bd887b
glossary_version: 34
glossary_terms_sha256: 8e6288671426e65b346cdeb533a9c76d3902ae1665cb15d7531912bc1806762d
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 1. KHÔNG GIAN VECTƠ TÔPÔ

### 1. Định nghĩa không gian vectơ tôpô

#### Định nghĩa 1 {#evt-i-s1-def-1 .statement}

— *Cho một vành chia tôpô* $ \mathbf{K} $ (GT, III, § 6.7) *và một tập hợp* $ E $ *sao cho* $ E $ *có*
$ 1^\circ $ *cấu trúc của một không gian vectơ trái trên* $ \mathbf{K} $;
$ 2^\circ $ *một tôpô tương thích với cấu trúc nhóm cộng của* $ E $ (GT, III, § 1.1) *và ngoài ra thỏa mãn tiên đề sau:*
*(EVT)* *ánh xạ* $ (\lambda, x) \mapsto \lambda x $ *từ* $ \mathbf{K} \times E $ *vào* $ E $ *là liên tục,* *thì* $ E $ *được gọi là một không gian vectơ tôpô trái trên* (hoặc trên) $ \mathbf{K} $.

Điều này tương đương với nói rằng $ E $ là một *môđun trái tôpô* $ \mathbf{K}\text{-module} $ (GT, III, § 6.6).
Một cấu trúc không gian vectơ trái đối với $ \mathbf{K} $ và một tôpô đã cho trên một tập hợp $ E $ được gọi là *tương thích* nếu tôpô và cấu trúc nhóm cộng của $ E $ tương thích và nếu, ngoài ra, tiên đề (EVT) đúng. Điều này cũng chính là nói rằng hai ánh xạ $ (x, y) \mapsto x + y $ và $ (\lambda, x) \mapsto \lambda x $ từ $ E \times E $ và $ \mathbf{K} \times E $, tương ứng, vào $ E $ là liên tục, vì khi đó ánh xạ $ x \mapsto -x = (-1)x $, là liên tục và tôpô của $ E $ tương thích với cấu trúc nhóm cộng của nó.

Nếu $ E $ là một không gian vectơ tôpô trái trên $ \mathbf{K} $, ta nói rằng $ E $ chỉ được trang bị cấu trúc không gian vectơ của nó, *nằm dưới* không gian vectơ tôpô $ E $.

#### Ví dụ {#evt-i-s1-n1-exa-1 .statement}

— 1) Nếu $ E $ là một không gian vectơ trái trên một vành chia tôpô *rời rạc* $ \mathbf{K} $, tôpô *rời rạc* trên $ E $ tương thích với cấu trúc không gian vectơ của $ E $ (điều này không đúng nếu $ \mathbf{K} $ không rời rạc và $ E $ không phải là điểm duy nhất 0).
2) Cho $ A $ là một vành tôpô (GT, III, § 6.3) và cho $ \mathbf{K} $ là một vành con của $ A $ đồng thời cũng là một vành chia và sao cho tôpô cảm sinh trên $ \mathbf{K} $ bởi tôpô của $ A $ tương thích với cấu trúc vành chia của $ \mathbf{K} $; khi đó tôpô của $ A $ tương thích với cấu trúc không gian vectơ trái của nó trên $ \mathbf{K} $.
3) Cho $ \mathbf{K} $ là một vành chia tôpô tùy ý và $ I $ là một tập hợp tùy ý. Trên không gian vectơ tích $ K_s^I(A, II, § 1.5) $, tôpô tích tương thích với cấu trúc không gian vectơ (GT, III, § 6.4). Hoặc ta có thể nói rằng không gian $ K_s^I $ các ánh xạ từ $ I $ vào $ \mathbf{K} $ với tôpô *theo từng điểm* hoặc *hội tụ đơn* là một không gian vectơ tôpô trên $ \mathbf{K} $ (TG, X, p. 4).
4) Cho $ X $ là một không gian tôpô; trên tập hợp $ E = \mathcal{C}(X; \mathbf{R}) $ gồm các hàm thực *liên tục* hữu hạn xác định trên $ X $, tôpô *hội tụ compact* (GT, X, § 1.3) tương thích với cấu trúc không gian vectơ của E trên $ \mathbf{R} $. Thật vậy, cho $ u_0 $ là một điểm của E, cho H là một tập con compact của X và $ \varepsilon $ là một số dương ngặt tùy ý. Hàm thực $ u_0 $ bị chặn trên H ; đặt $ a = \sup_{t \in H} |u_0(t)| $; nếu $ u $ là một điểm bất kỳ của E thì với mọi $ t \in H $

$$
|\lambda u(t) - \lambda_0 u_0(t)| \leq |\lambda| \cdot |u(t) - u_0(t)| + a |\lambda - \lambda_0|.
$$

Do đó, nếu $ |\lambda - \lambda_0| \leq \varepsilon $ và $ |u(t) - u_0(t)| \leq \varepsilon $ với mọi $ t \in H $, thì với $ t \in H $,
$ |\lambda u(t) - \lambda_0 u_0(t)| \leq \varepsilon (\varepsilon + |\lambda_0| + a) $, điều này cho thấy tiên đề (EVT) được thỏa mãn; tương tự, có thể kiểm tra rằng tôpô hội tụ compact tương thích với cấu trúc nhóm cộng của E.

Mặt khác, nếu X không compact, tôpô *hội tụ đều* (trên X) không nhất thiết tương thích với cấu trúc không gian vectơ của E; chẳng hạn nếu $ X = \mathbf{R} $ và $ u_0 $ là một hàm liên tục không bị chặn trên $ \mathbf{R} $, thì ánh xạ $ \lambda \mapsto \lambda u_0 $ từ $ \mathbf{R} $ vào E không liên tục theo tôpô hội tụ đều trên E.

5) Cho E là một không gian vectơ có số chiều hữu hạn $ n $ trên một vành chia tôpô K; tồn tại một đẳng cấu $ u : K_s^n \to E $ của các không gian vectơ K và hơn nữa, nếu $ v $ là một đẳng cấu thứ hai của $ K_s^n $ lên E, thì ta có thể viết $ v = u \circ f $, trong đó $ f $ là một tự đẳng cấu của không gian vectơ K $ K_s^n $. Trên $ K_s^n $, xét tôpô *tích* tương thích với cấu trúc không gian vectơ của nó (*Ví dụ 3*); vì mọi ánh xạ tuyến tính từ $ K_s^n $ vào chính nó đều liên tục theo tôpô này, mọi tự đẳng cấu của không gian vectơ $ K_s^n $ đều *bicontinuous*. Do đó, nếu ta *chuyển* tôpô tích của $ K_s^n $ sang E, bằng một đẳng cấu bất kỳ nào của $ K_s^n $ lên E, thì tôpô nhận được trên E là *độc lập* với đẳng cấu cụ thể được sử dụng; ta gọi đó là *tôpô chính tắc* trên E; ta sẽ đặc trưng nó theo một cách khác (I, § 1.3) khi K là một vành chia đầy đủ, không rời rạc, có một định giá. Mọi ánh xạ tuyến tính từ E vào một không gian vectơ tôpô trên K đều *liên tục* theo tôpô chính tắc trên E.

Cũng như trong định nghĩa 1, có thể định nghĩa một không gian vectơ tôpô *phải* trên K, một vành chia tôpô; nhưng mọi không gian vectơ phải trên K có thể được xem như một không gian vectơ trái trên vành chia $ K^0 $ đối của K (A, II, § 1.1), và tôpô của K tương thích với cấu trúc của vành chia $ K^0 $. Vì lý do này, thông thường ta chỉ xét các không gian vectơ tôpô trái; khi nói « không gian vectơ tôpô » mà không có điều kiện bổ sung, cần hiểu rằng ta quy về một không gian vectơ trái.

Nếu K' là một vành chia con của K, và E là một không gian vectơ tôpô trên K, thì hiển nhiên tôpô của E vẫn tương thích với cấu trúc không gian vectơ của E đối với K', thu được bằng cách hạn chế trường vô hướng xuống K'; ta nói rằng không gian vectơ tôpô trên K', thu được theo thủ tục này, *nằm dưới* không gian vectơ tôpô E trên K.

Để một không gian vectơ tôpô E là *Hausdorff*, điều kiện cần và đủ là với mọi $ x \neq 0 $ của E, tồn tại một lân cận của 0 không chứa $ x $ (GT, III, § 1.2).

Xét một tôpô trên một không gian vectơ E trên một vành chia tôpô K, tương thích với cấu trúc nhóm cộng của E. Do đẳng thức

$$
\lambda x - \lambda_0 x_0 = (\lambda - \lambda_0) x_0 + \lambda_0 (x - x_0) + (\lambda - \lambda_0) (x - x_0)
$$

tiên đề (EVT) tương đương với hệ ba tiên đề sau.

*(EVT$_1'$)* *Với mọi* $ x_0 \in E $, *ánh xạ* $ \lambda \mapsto \lambda x_0 $ *liên tục tại* $ \lambda = 0 $.

*(EVT$_2'$)* *Với mọi* $ \lambda_0 \in K $, *ánh xạ* $ x \mapsto \lambda_0 x $ *liên tục tại* $ x = 0 $.

*(EVT$_3'$)* *Ánh xạ* $ (\lambda, x) \mapsto \lambda x $ *liên tục tại* $ (0, 0) $.

Đặc biệt:

#### Mệnh đề 1 {#evt-i-s1-prop-1 .statement}

— Với mọi $ \alpha \in K $ và mọi điểm $ b \in E $, ánh xạ $ x \mapsto \alpha x + b $ từ E vào chính nó là liên tục. Hơn nữa, nếu $ \alpha \neq 0 $, ánh xạ này là một phép đồng phôi của E lên chính nó.

Phần thứ hai của mệnh đề là hệ quả của sự kiện rằng nếu $ \alpha \neq 0 $, thì $ x \mapsto \alpha^{-1}x - \alpha^{-1}b $ là ánh xạ nghịch đảo của $ x \mapsto \alpha x + b $.

#### Hệ quả {#evt-i-s1-n1-cor-1 .statement}

— Nếu $ A $ là một tập hợp mở (tương ứng đóng) trong E, thì $ \alpha A $ là mở (tương ứng đóng) trong E với mọi $ \alpha \neq 0 $ trong K.

Cho $ E $ và $ F $ là hai không gian vectơ tôpô trên cùng một vành chia tôpô $ K $. Một song ánh $ f $ của $ E $ lên $ F $ là một đẳng cấu của không gian vectơ tôpô $ E $ lên không gian vectơ tôpô $ F $ khi và chỉ khi $ f $ là tuyến tính và song liên tục. Đặc biệt, nếu $ \gamma \neq 0 $ thuộc tâm của $ K $, phép vị tự $ x \mapsto \gamma x $ là một tự đẳng cấu của cấu trúc không gian vectơ tôpô của $ E $.

### 2. Các không gian chuẩn trên một vành chia có giá trị

Nhắc lại (GT, IX, § 3.2) rằng một giá trị tuyệt đối trên một vành chia $ K $ là một ánh xạ $ \xi \mapsto |\xi| $ của $ K $ vào $ \mathbf{R}_+ $, sao cho $ |\xi| = 0 $ khi và chỉ khi $ \xi = 0 $, và $ |\xi \eta| = |\xi| \cdot |\eta| $, và $ |\xi + \eta| \leq |\xi| + |\eta| $; một giá trị tuyệt đối định nghĩa một khoảng cách $ |\xi - \eta| $ trên $ K $, và do đó một tôpô Hausdorff tương thích với cấu trúc vành chia của $ K $. Nếu $ |\xi| = 1 $ với mọi $ \xi \neq 0 $, giá trị tuyệt đối được gọi là không thực, và tôpô mà nó định nghĩa trên $ K $ là tôpô rời rạc; mặt khác, nếu tồn tại $ \alpha \neq 0 $ trong $ K $ sao cho $ |\alpha| \neq 1 $, thì tồn tại $ \beta \neq 0 $ trong $ K $ sao cho $ |\beta| < 1 $ (chỉ cần lấy $ \beta = \alpha $ hoặc $ \beta = \alpha^{-1} $), và dãy $ (\beta^n)_{n \geq 1} $ hội tụ về 0, do đó tôpô của $ K $ không phải là rời rạc.

Mặt khác, ta nhắc lại (GT, IX, § 3.3) rằng nếu $ E $ là một không gian vectơ trên một vành chia có giá trị không rời rạc $ K $ thì một chuẩn trên $ E $ là một ánh xạ $ x \mapsto \|x\| $ của $ E $ vào $ \mathbf{R}_+ $, sao cho $ \|x\| = 0 $ khi và chỉ khi $ x = 0 $, và sao cho $ \|\lambda x\| = |\lambda| \cdot \|x\| $ với mọi vô hướng $ \lambda \in K $, và $ \|x + y\| \leq \|x\| + \|y\| $. Một khoảng cách $ \|x - y\| $, được định nghĩa trên $ E $ bởi chuẩn, và do đó một tôpô tương thích với cấu trúc không gian vectơ của $ E $ (loc. cit.). Trừ khi điều ngược lại được phát biểu rõ ràng, một không gian chuẩn được xét theo cấu trúc của không gian vectơ tôpô được định nghĩa bởi chuẩn của nó. Các không gian chuẩn là một trong những lớp quan trọng nhất của các không gian vectơ tôpô.

Đã biết (GT, IX, § 3.3) rằng hai chuẩn phân biệt trên $ E $ có thể định nghĩa cùng một tôpô trên $ E $; điều này xảy ra khi và chỉ khi hai chuẩn là tương đương (loc. cit.). Cấu trúc của các không gian chuẩn do đó phong phú hơn cấu trúc của các không gian vectơ tôpô; nếu $ E $ và $ F $ là hai không gian chuẩn, cần phải cẩn thận phân biệt giữa khái niệm đẳng cấu của cấu trúc không gian chuẩn của $ E $ với của $ F $, và khái niệm đẳng cấu của cấu trúc không gian vectơ tôpô của $ E $ với của $ F $.

#### Ví dụ {#evt-i-s1-n2-exa-1 .statement}

Cho I là một tập hợp chỉ số tùy ý; người ta biết (GT, X, § 3.2) rằng một chuẩn $ \|x\| $ có thể được định nghĩa, trên tập hợp các ánh xạ bị chặn $ x = (\xi_i) $ từ I vào K, $ \mathcal{B}(I; K) $ (cũng được viết là $ \mathcal{B}_K(I) $ hoặc $ \ell_K^\infty(I) $), bởi $ \|x\| = \sup_{i \in I} |\xi_i| $. Khi I là một không gian tôpô, tập hợp các ánh xạ liên tục, bị chặn từ I vào K là một không gian con đóng của không gian $ \mathcal{B}(I; K) $ (GT, X, § 3.1, hệ quả 2). Một không gian con khác của $ \mathcal{B}(I; K) $ là tập hợp $ \ell_K^1(I) $ của các họ cộng tuyệt đối $ x = (\xi_i) $ (GT, X, § 3.6); ta có thể định nghĩa trên không gian con này một chuẩn khác $ \|x\|_1 = \sum_{i \in I} |\xi_i| $, mà nói chung không tương đương với chuẩn $ \|x\| = \sup_{i \in I} |\xi_i| $ (I, p. 23, bài tập 6); khi xét $ \ell_K^1(I) $ như một không gian có chuẩn, không chỉ rõ chuẩn của nó, thì luôn hiểu đó là chuẩn $ \|x\| $. Ta viết $ \mathcal{B}(I) $ và $ \ell^1(I) $ thay cho $ \mathcal{B}(I; \mathbf{R}) $ và $ \ell_R^1(I) $.

### 3. Các không gian con vectơ và các không gian thương của một không gian vectơ tôpô; các tích của các không gian vectơ tôpô; các tổng trực tiếp tôpô của các không gian con

Mọi điều đã nói về các môđun tôpô (GT, III, § 6.6) đều áp dụng riêng cho các không gian vectơ tôpô. Nếu M là một không gian con vectơ của một không gian vectơ tôpô E, tôpô cảm sinh trên M bởi tôpô của E tương thích với cấu trúc không gian vectơ của M, và bao đóng $ \overline{M} $ của M trong E là một không gian con vectơ của E. Tôpô thương của tôpô của E theo M tương thích với cấu trúc không gian vectơ của E/M.

Nếu E là một không gian vectơ tôpô, bao đóng N của $ \{0\} $ trong E (giao của các lân cận của 0) là một không gian con vectơ đóng của E; không gian vectơ thương E/N, vốn nhất thiết là Hausdorff dù E có là Hausdorff hay không, được gọi là không gian vectơ Hausdorff liên kết với E.

Cho $ (E_i)_{i \in I} $ là một họ các không gian vectơ tôpô trên cùng một vành chia tôpô K, và cho E là không gian vectơ tích của các $ E_i $. Tôpô tích của các tôpô của các $ E_i $ tương thích với cấu trúc không gian vectơ của E. Trong không gian tích E, không gian con F, là tổng trực tiếp của các $ E_i $ là trù mật khắp nơi (GT, III, § 2.9, mệnh đề 25).

Đối với một số kiểu không gian vectơ tôpô trên trường $ \mathbf{R} $ hoặc trường $ \mathbf{C} $ ta định nghĩa (trong II, p. 29) một tôpô trên tổng trực tiếp của một họ $ (E_i) $ các không gian vectơ tôpô mà nói chung là phân biệt với tôpô cảm sinh bởi tôpô tích của các $ E_i $.

Mọi điều đã nói về các tổng trực tiếp hữu hạn của các nhóm con ổn định của các nhóm tôpô có toán tử (GT, III, § 6.2) đều áp dụng cho các không gian vectơ tôpô, bằng cách thay thế « nhóm con ổn định » khắp nơi bởi « không gian con vectơ ».

#### Nhận xét {#evt-i-s1-n3-rem-1 .statement}

Cho M là một không gian con vectơ đóng của một không gian vectơ tôpô Hausdorff E, không nhất thiết tồn tại một không gian con vectơ bù (đại số) của M đóng trong E (ngay cả khi E là một không gian có chuẩn; xem IV, p. 55, bài tập 16 (c)); a fortiori không nhất thiết tồn tại một không gian bù tôpô của M trong E (xem I, p. 26, bài tập 8). Tuy nhiên ta sẽ thấy trong § 2 rằng khi K là một vành chia có giá trị không rời rạc, thì mọi không gian con đóng M của E, với đối chiều hữu hạn, đều có một không gian bù tôpô trong E (I, p. 14, mệnh đề 3).

### 4. Cấu trúc đều và sự đầy đủ của một không gian vectơ tôpô

Vì tôpô của không gian vectơ tôpô E tương thích với cấu trúc nhóm cộng trên E, nó xác định một cấu trúc đều trên E (GT, III, § 3); khi ta nói về cấu trúc đều của một không gian vectơ tôpô, ta luôn hiểu cấu trúc này trừ khi có nêu rõ điều ngược lại. Mọi ánh xạ tuyến tính liên tục từ một không gian vectơ tôpô E vào một không gian vectơ tôpô F đều liên tục đều (GT, III, § 3.1, mệnh đề 3); mọi ánh xạ từ E vào chính nó có dạng $ x \mapsto \alpha x + b $ đều liên tục đều. Một tập hợp các ánh xạ tuyến tính liên tục đều từ E vào F là liên tục đều đồng đều (GT, X, § 2.2, mệnh đề 5).

#### Nhận xét 1 {#evt-i-s1-n4-rem-1 .statement}

Nếu B là một tập hợp tiền compact của K, thì với mọi lân cận V của 0 trong E, tồn tại một lân cận U của 0 trong E sao cho BU $ \subset $ V. Thật vậy, nếu W là một lân cận của 0 trong E sao cho W + W $ \subset $ V; thì từ (EVT$_{\text{III}}$) suy ra tồn tại một lân cận T$_0$ của 0 trong K và một lân cận U$_0$ của 0 trong E sao cho T$_0$U$_0$ $ \subset $ W. Vì B là tiền compact, tồn tại hữu hạn điểm $ \lambda_i \in B $ ($ 1 \leq i \leq n $) sao cho các $ \lambda_i + T_0 $ phủ B; từ (EVT$_{\text{II}}$) suy ra tồn tại một lân cận U $ \subset $ U$_0$ của 0 trong E, sao cho $ \lambda_i U \subset W $ với mọi $ i $; rõ ràng U có các tính chất cần thiết. Một cách tương tự (dùng (EVT$_{\text{I}}$) thay cho (EVT$_{\text{II}}$)) ta có thể chứng minh rằng nếu H là một tập hợp tiền compact của E, thì với mọi lân cận V của 0 trong E, tồn tại một lân cận T của 0 trong K sao cho TH $ \subset $ V.

#### Nhận xét 2 {#evt-i-s1-n4-rem-2 .statement}

Từ 1) suy ra rằng, nếu B là một tập hợp tiền compact của K và H là một tập hợp tiền compact của E, thì ánh xạ $ (\lambda, x) \mapsto \lambda x $ hạn chế trên B $ \times $ H là liên tục đều. Thật vậy, nếu V là một lân cận của 0 trong E thì tồn tại các lân cận T của 0 trong K, và U của 0 trong E sao cho TH + BU $ \subset $ V. Vì ta có thể viết $ \lambda x - \lambda' x' = (\lambda - \lambda') x + \lambda'(x - x') $, ta thấy rằng với $ \lambda, \lambda' $ trong B, x, x' trong H, $ \lambda - \lambda' \in T $ và $ x - x' \in U $, ta có $ \lambda x - \lambda' x' \in V $, điều này chứng minh mệnh đề của ta.

Một không gian vectơ tôpô được gọi là đầy đủ nếu, xét theo cấu trúc đều của nó, nó là một không gian đều đầy đủ.

#### Định nghĩa 2 {#evt-i-s1-def-2 .statement}

*Một không gian có chuẩn đầy đủ trên một vành chia có giá trị không rời rạc được gọi là một không gian Banach.*

#### Ví dụ {#evt-i-s1-n4-exa-1 .statement}

Nếu K là một vành chia có giá trị không rời rạc thì không gian $ \mathscr{B}(I ; K) $ (I, p. 4, Ví dụ) là đầy đủ (GT, X, § 3.1, cor. 1). Điều này cũng đúng cho không gian $ \ell_K^1(I) $ (I, p. 4, Ví dụ) với chuẩn $ \|x\|_1 = \sum_{i \in I} |\xi_i| $: vì, nếu $ x_n $ là một dãy Cauchy trong không gian này và $ x_n = (\xi_{m_i})_{i \in I} $, thì với mọi $ i \in I $

$$
|\xi_{m_i} - \xi_{n_i}| \leq \|x_m - x_n\|_1;
$$

do đó, với mỗi $ i \in I $, dãy $ (\xi_{m_i})_{n \geq 1} $ hội tụ đến một giới hạn $ \xi_i $ trong K. Hơn nữa, với mỗi tập con hữu hạn J của I

$$
\sum_{i \in J} |\xi_{m_i} - \xi_{n_i}| \leq \|x_m - x_n\|_1;
$$

và suy ra ngay lập tức rằng tồn tại một hằng $ a > 0 $, độc lập với J, m, n sao cho $ \sum_{i \in J} |\xi_{m_i} - \xi_{n_i}| \leq a $. Cho m tiến tới $ + \infty $, ta suy ra $ \sum_{i \in J} |\xi_i - \xi_{m_i}| \leq \varepsilon $ từ đó $ \sum_{i \in I} |\xi_i| \leq a + \|x_n\|_1 $, điều này cho thấy rằng $ z = (\xi_i)_{i \in I} $ thuộc về $ \ell_K^1(I) $; hơn nữa, với mọi $ \varepsilon > 0 $, tồn tại $ n_0 $ sao cho với $ n \geq n_0 $ và với mọi tập hợp hữu hạn J của I, ta có $ \sum_{i \in J} |\xi_i - \xi_{m_i}| \leq \varepsilon $; chuyển qua giới hạn theo tập có hướng gồm các tập con hữu hạn của I, ta thấy rằng $ \|z - x_n\|_1 \leq \varepsilon $ với $ n \geq n_0 $, điều này cho thấy rằng $ z $ là giới hạn của dãy $ (x_n) $ trong không gian định chuẩn $ \ell_K^1(I) $.

Cho $ K $ là một vành chia tôpô Hausdorff, $ E $ là một không gian vectơ tôpô trên $ K $ và giả sử rằng vành đầy đủ $ \hat{K} $ là một *vành chia* (điều này đúng khi $ K $ là một vành chia có giá trị, GT, IX, § 3.3) thì phần đầy đủ Hausdorff $ \hat{E} $ của $ E $ mang cấu trúc của một *không gian vectơ tôpô đầy đủ* trên $ \hat{K} $ (GT, III, § 6.5); ta nói rằng $ \hat{E} $, với cấu trúc này, là *phần đầy đủ Hausdorff* của không gian vectơ tôpô $ E $, hoặc đơn giản là *phần đầy đủ* của $ E $ khi $ E $ là *Hausdorff*.

### 5. Các lân cận của gốc trong một không gian vectơ tôpô trên một vành chia có giá trị

#### Định nghĩa 3 {#evt-i-s1-def-3 .statement}

*Cho $ K $ là một vành chia có giá trị và $ E $ là một không gian vectơ trái trên $ K $; ta nói rằng một tập con $ M $ của $ E $ là cân bằng nếu, với mọi $ x \in M $ và mọi $ \lambda \in K $ sao cho $ |\lambda| \leq 1 $, ta có $ \lambda x \in M $ (hay nói cách khác nếu $ \lambda M \subset M $ khi $ |\lambda| \leq 1 $).*

#### Mệnh đề 2 {#evt-i-s1-prop-2 .statement}

*Trong một không gian vectơ tôpô $ E $ trên một vành chia có giá trị $ K $, bao đóng của một tập cân bằng $ M $ là một tập cân bằng.*

Nếu $ B $ là tập hợp các $ \xi \in K $ với $ |\xi| \leq 1 $; thì $ B $ là đóng trong $ K $. Nhưng $ B \times M $ được ánh xạ vào $ M $ bởi ánh xạ liên tục $ (\lambda, x) \mapsto \lambda x $; và do đó $ B \times \overline{M} $ được ánh xạ vào $ \overline{M} $ (GT, I, § 2.1, th. 1), điều này chứng minh rằng $ \overline{M} $ là cân bằng.

Khi $ M $ là một tập hợp tùy ý trong không gian vectơ $ E $ trên một vành chia có giá trị $ K $, tập hợp $ M_1 $ của các $ \lambda x $ với $ x \in M $ và $ \lambda \in K $ sao cho $ |\lambda| \leq 1 $, rõ ràng là tập hợp cân bằng nhỏ nhất chứa $ M $; $ M_1 $ được gọi là *bao cân bằng* của $ M $.

#### Mệnh đề 3 {#evt-i-s1-prop-3 .statement}

*Cho $ K $ là một vành chia có giá trị compact địa phương và không rời rạc, và $ E $ là một không gian vectơ tôpô Hausdorff (tương ứng. một không gian vectơ tôpô) trên $ K $. Với mọi tập hợp compact (tương ứng. tiền compact) $ H $ trong $ E $, bao cân bằng của $ H $ là compact (tương ứng. tiền compact).

Nếu $ B $ ký hiệu quả cầu $ |\xi| \leq 1 $ trong $ K $, bao cân bằng của $ H $ là $ H_1 $, ảnh của $ B \times H $ qua ánh xạ liên tục $ m : (\lambda, x) \mapsto \lambda x $. Nếu $ E $ là Hausdorff, nếu $ B $ là compact và nếu $ H $ là compact thì $ B \times H $ cũng vậy và do đó $ H_1 $ cũng vậy. Nếu $ H $ là tiền compact thì hạn chế của $ m $ vào $ B \times H $ là liên tục đều (I, p. 5, *Nhận xét* 2) và vì $ B \times H $ là tiền compact, nên ảnh của nó qua $ m $ cũng là tiền compact (GT, II, § 4.2, prop. 2).

Chú ý rằng bao cân bằng của một tập hợp đóng không nhất thiết đóng. Ví dụ, trong $ \mathbf{R}^2 $, bao cân bằng của hyperbol xác định bởi phương trình $ xy = 1 $ không đóng.

Hợp của một họ các tập hợp cân bằng trong $ E $ là cân bằng, điều này suy ra rằng với mọi tập hợp $ M $ của $ E $ tồn tại một tập con cân bằng lớn nhất $ N $ của $ M $ được gọi là *lõi cân bằng của* $ M $; ngoài ra $ N $ không rỗng khi và chỉ khi $ 0 \in M $. Nói rằng $ x \in N $ có nghĩa là với mọi $ \lambda \in K $ sao cho $ |\lambda| \leq 1 $, ta có $ \lambda x \in M $, hay tương đương (nếu $ 0 \in M $) là, với mọi $ \mu \in K $ với |μ| ≥ 1, ta có x ∈ μM. Nếu 0 ∈ M, lõi cân bằng N của M do đó là giao $ \bigcap_{|\mu| \geq 1} \mu M $. Điều này đặc biệt cho thấy rằng nếu M đóng thì N cũng đóng.

#### Định nghĩa 4 {#evt-i-s1-def-4 .statement}

*Cho K là một vành chia định giá không rời rạc và E là một không gian vectơ trái trên K với hai tập con A và B. Ta nói rằng A hấp thụ B nếu tồn tại α > 0 sao cho λA ⊃ B với mọi λ ∈ K thỏa mãn |λ| ≥ α (hoặc tương đương nếu μB ⊂ A với μ ≠ 0 và |μ| ≤ α⁻¹). Một tập hợp A của E được gọi là hấp thụ nếu nó hấp thụ mọi tập hợp gồm một điểm.*

Cho A là một tập hợp cân bằng của E; để nó hấp thụ một tập hợp B của E thì chỉ cần tồn tại λ ≠ 0 sao cho λA ⊃ B; thật vậy, với |μ| ≥ |λ|, ta có λA = (λμ⁻¹) μA, và vì μA là cân bằng và |λμ⁻¹| ≤ 1, suy ra λA ⊂ μA, và do đó B ⊂ μA. Đặc biệt, để một tập hợp cân bằng A của E là hấp thụ, điều kiện cần và đủ là với mọi x ∈ E, tồn tại λ ≠ 0 trong K sao cho λx ∈ A. Mọi tập hợp hấp thụ của E đều sinh ra không gian vectơ E. Mọi giao hữu hạn của các tập hợp hấp thụ là một tập hợp hấp thụ.

#### Mệnh đề 4 {#evt-i-s1-prop-4 .statement}

*Trong một không gian vectơ tôpô E trên một vành chia định giá không rời rạc K tồn tại một hệ cơ sở $ \mathfrak{B} $ các lân cận đóng của 0 sao cho :
*(EV₁)* Mọi tập hợp V ∈ $ \mathfrak{B} $ đều cân bằng và hấp thụ.
*(EV₂)* Với mọi V ∈ $ \mathfrak{B} $ và λ ≠ 0 trong K, ta có λV ∈ $ \mathfrak{B} $ (tính bất biến của $ \mathfrak{B} $ đối với các phép vị tự có tỉ số khác không).
*(EV₃)* Với mọi V ∈ $ \mathfrak{B} $, tồn tại W ∈ $ \mathfrak{B} $ sao cho W + W ⊂ V.

Ngược lại, cho E là một không gian vectơ trên K, và cho $ \mathfrak{B} $ là một cơ sở lọc trên E thỏa mãn các điều kiện (EV₁), (EV₂) và (EV₃). Khi đó tồn tại một tôpô (và nó là duy nhất) trên E, tương thích với cấu trúc không gian vectơ của E, và sao cho $ \mathfrak{B} $ là một hệ cơ sở các lân cận của 0.

Theo tiên đề (EVT'₃) ta chứng minh trước hết rằng *lõi cân bằng*, V₁, của V, một lân cận của 0, bản thân nó là một lân cận của 0. Thật vậy, tồn tại α > 0 và một lân cận W của 0 sao cho, nếu |λ| ≤ α và x ∈ W, thì λx ∈ V. Vì K không rời rạc, tồn tại μ ≠ 0 trong K với |μ| ≤ α và μW là một lân cận của 0 sao cho μW ⊂ V. Ngoài ra nếu v ∈ K và |v| ≤ 1 thì |vμ| ≤ α và do đó vμW ⊃ V. Suy ra μW ⊃ V₁ và V₁ là một lân cận của 0. Hơn nữa vì V đóng nên V₁ cũng đóng. Như vậy tập hợp $ \mathfrak{B} $ các lân cận *đóng và cân bằng* của 0 tạo thành một hệ cơ sở các lân cận của 0 trong E. Theo (EVT₁') mọi lân cận của 0 đều *hấp thụ*; hơn nữa $ \mathfrak{B} $ thỏa mãn (EV₂) (*xem* I, p. 3, hệ quả); cuối cùng, do tính liên tục của (x, y) ↦ x + y tại điểm (0, 0), mọi hệ cơ sở các lân cận của 0 trong E đều thỏa mãn (EV₃). Tập hợp $ \mathfrak{B} $ thỏa mãn các điều kiện của mệnh đề.

Bây giờ cho E là một không gian vectơ trên K, và $ \mathfrak{B} $ là một cơ sở lọc trên E thỏa mãn (EV₁), (EV₂) và (EV₃). Tiên đề (EV₁) trước hết cho thấy rằng với mọi V ∈ $ \mathfrak{B} $, ta có −V = V và 0 ∈ V; các hệ thức này và tiên đề (EV₃) cho thấy rằng $ \mathfrak{B} $ là một hệ cơ sở các lân cận của 0, đối với một tôpô trên E tương thích với cấu trúc *nhóm cộng* của E (GT, III, § 1.2). Mặt khác các tiên đề (EVT'_I), (EVT'_II) và (EVT'_III) là các hệ quả ngay lập tức của (EV_I) và (EV_II), do đó tôpô được xác định ở trên thỏa mãn tiên đề (EVT), và mệnh đề được chứng minh.

#### Nhận xét 1 {#evt-i-s1-n5-rem-1 .statement}

Trong một không gian định chuẩn trên một vành chia định giá không rời rạc, tập hợp các quả cầu mở (tương ứng quả cầu đóng) có tâm 0 là một hệ cơ sở các lân cận của 0 thỏa mãn các điều kiện (EV_I), (EV_II) và (EV_III).

#### Nhận xét 2 {#evt-i-s1-n5-rem-2 .statement}

Khi vành chia của các vô hướng K là trường \mathbf{R} hoặc trường \mathbf{C}, mọi cơ sở lọc \mathfrak{B} trên E chỉ thỏa mãn hai tiên đề (EV_I) và (EV_III) là một hệ cơ sở các lân cận của 0 đối với một tôpô tương thích với cấu trúc không gian vectơ của E. Thật vậy, ta chỉ cần chứng minh rằng, trong các điều kiện này, với mọi $ \lambda \neq 0 $ trong K và mọi $ V \in \mathfrak{B} $ tồn tại $ W \in \mathfrak{B} $ sao cho $ \lambda W \subset V $. Bây giờ từ (EV_III) tồn tại $ W_1 \in \mathfrak{B} $ với $ 2\,W_1 \subset V $, và ta suy ra, bằng quy nạp, rằng với mọi số nguyên dương $ n $, tồn tại $ W_n \in \mathfrak{B} $ sao cho $ 2^n W_n \subset V $. Vì V là cân bằng, nếu lấy $ n $ đủ lớn sao cho $ 2^n = |2^n| > |\lambda| $, thì $ W = W_n $ thỏa mãn điều kiện, như cần phải chứng minh.

Kết quả này không đúng đối với mọi vành chia định giá không rời rạc K, vì trong một vành chia như vậy không còn nhất thiết đúng rằng $ |m\varepsilon| = m $ với mọi số nguyên dương $ m $ ($ \varepsilon $ chỉ phần tử đơn vị của vành chia ; xem I, p. 22, bt. 1).

#### Nhận xét 3 {#evt-i-s1-n5-rem-3 .statement}

Nếu $K$ là một vành chia rời rạc, các điều kiện (EVT'_I) và (EVT'_III) đúng với mọi tôpô trên $E$. Lập luận như trong mệnh đề 4, ta dễ dàng thấy rằng nếu $E$ là một không gian vectơ tôpô trên $K$, thì tồn tại $ \mathfrak{B} $, một hệ cơ sở các lân cận đóng của 0 trong $E$ thỏa mãn các điều kiện (EV_II) và (EV_III). Ngược lại, nếu một cơ sở lọc $ \mathfrak{B} $ trên một không gian vectơ $E$ trên $K$ sao cho 0 thuộc mọi tập hợp của $ \mathfrak{B} $ và (EV_II), (EV_III) đúng, thì $ \mathfrak{B} $ là một hệ cơ sở các lân cận của 0 trong một tôpô tương thích với cấu trúc không gian vectơ của $E$.

### 6. Các tiêu chuẩn về tính liên tục và tính liên tục đều

Cho $E$ và $F$ là các không gian vectơ tôpô trên cùng một vành chia $K$; để một ánh xạ tuyến tính $ f $ từ $E$ vào $F$ liên tục, chỉ cần nó liên tục tại gốc (GT, III, § 2.8, mệnh đề 23). Mệnh đề này được tổng quát hóa như sau:

#### Mệnh đề 5 {#evt-i-s1-prop-5 .statement}

— Cho $ E_i (1 \leq i \leq n) $ và $F$ là các không gian vectơ tôpô trên một trường định giá không rời rạc $K$. Để một ánh xạ đa tuyến tính $ f $ từ $ \prod_{i=1}^n E_i $ vào $F$ liên tục trong không gian tích $ \prod_{i=1}^n E_i $, chỉ cần nó liên tục tại $ (0, 0, ..., 0) $.

Cho $ (a_1, a_2, ..., a_n) $ là một điểm tùy ý của $ \prod_{i=1}^n E_i $; ta phải chứng minh rằng với mọi lân cận $W$ của 0 trong $F$, tồn tại các lân cận $ V_i $ của 0 trong $ E_i $ ($ 1 \leq i \leq n $) sao cho các hệ thức $ z_i \in V_i $ kéo theo

$$
f(a_1 + z_1, a_2 + z_2, ..., a_n + z_n) - f(a_1, a_2, ..., a_n) \in W .
$$

Bây giờ, ta có thể viết

$$
f(a_1 + z_1, ..., a_n + z_n) - f(a_1, ..., a_n) = \sum_H u_H
$$

trong đó $ H $ chạy qua $ 2^n - 1 $ tập con của tập hợp các số nguyên $ \{ 1, 2, ..., n \} $, loại trừ chính tập hợp $ \{ 1, 2, ..., n \} $, và trong đó $ u_H = f(y_1, y_2, ..., y_n) $, với $ y_i = a_i $ nếu $ i \in H $ và $ y_i = z_i $ nếu $ i \notin H $. Tồn tại $ 2^n - 1 $ lân cận cân bằng $ W_H $ của 0 trong $ F $ sao cho $ \sum_H W_H \subset W $; mặt khác, vì theo giả thiết $ f $ liên tục tại $ (0, 0, ..., 0) $, nên trong mỗi $ E_i $ tồn tại một lân cận $ U_i $ của 0 ($ 1 \leq i \leq n $) sao cho $ n $ hệ thức $ x_i \in U_i $ kéo theo $ f(x_1, ..., x_n) \in \bigcap_H W_H $. Vì $ U_i $ hấp thụ, tồn tại $ \lambda_i \neq 0 $ trong $ K $ sao cho $ \lambda_i a_i \in U_i $. Gọi $ \lambda $ là một phần tử của $ K $ sao cho $ |\lambda| \geq \prod_{i \in H} |\lambda_i|^{-1} $ với mỗi tập con $ H $; ta chứng minh rằng các lân cận $ V_i = \lambda^{-n} U_i $, thỏa mãn điều kiện cần thiết. Ta có thể viết $ u_H = \mu f(x_1, ..., x_n) $ trong đó $ x_i \in U_i $ với $ 1 \leq i \leq n $ và $ \mu = \lambda^{-np} (\prod_{i \in H} \lambda_i^{-1}) $, $ p $ là số các số nguyên của $ \{ 1, 2, ..., n \} $ không thuộc $ H $. Theo điều trên $ |\mu| \leq 1 $, do đó $ u_H \in \mu W_H \subset W_H $ vì $ W_H $ là cân bằng. Mệnh đề được chứng minh.

#### Mệnh đề 6 {#evt-i-s1-prop-6 .statement}

*Với cùng các giả thiết về $ E_i (1 \leq i \leq n) $ và về $ F $ như trong mệnh đề 5, để một tập hợp $ \mathcal{E} $ các ánh xạ đa tuyến tính của $ \prod_{i=1}^n E_i $ vào $ F $ là đều liên tục thì chỉ cần tập hợp đó đều liên tục tại $ (0, 0, ..., 0) $.*

Bởi vì, trong phép chứng minh của mệnh đề 5, các $ U_i (1 \leq i \leq n) $ có thể được chọn sao cho quan hệ $ x_i \in U_i (1 \leq i \leq n) $ kéo theo $ f(x_1, ..., x_n) \in \bigcap_H W_H $ đối với *mọi* ánh xạ $ f \in \mathcal{E} $.

### 7. Các tôpô ban đầu của các không gian vectơ

#### Mệnh đề 7 {#evt-i-s1-prop-7 .statement}

*Cho $ (E_v)_{v \in I} $ là một họ các không gian vectơ tôpô trên một vành chia tôpô $ K $. Cho $ E $ là một không gian vectơ trên $ K $ và với mỗi $ v \in I $, cho $ f_v $ là một ánh xạ tuyến tính của $ E $ vào $ E_v $. Khi đó tôpô thô nhất trên $ E $ làm cho mỗi hàm $ f_v $ liên tục, là một tôpô $ \mathcal{T} $ tương thích với cấu trúc không gian vectơ của $ E $. Hơn nữa, nếu với mọi $ x \in E $, $ \phi(x) $ ký hiệu điểm $ (f_v(x)) $ của không gian tích $ F = \prod_{v \in I} E_v $, thì tôpô $ \mathcal{T} $ là ảnh ngược của tôpô của không gian con $ \phi(E) $ của $ F $ qua ánh xạ tuyến tính $ \phi $.*

Phần cuối của mệnh đề là một trường hợp riêng của GT, I, § 4.1, mệnh đề 3. Mệnh đề sau đó suy ra từ bổ đề tiếp theo.

#### Bổ đề {#evt-i-s1-n7-lem-1 .statement}

— *Cho $ M $ và $ N $ là hai không gian vectơ, và $ g $ là một ánh xạ tuyến tính của $ M $ vào $ N $. Nếu $ \mathcal{T}_0 $ là một tôpô tương thích với cấu trúc không gian vectơ của $ N $, thì ảnh ngược của $ \mathcal{T}_0 $ qua $ g $ là tương thích với cấu trúc không gian vectơ của $ M $.*

Ta chứng minh, chẳng hạn, rằng $ (\lambda, x) \mapsto \lambda x $ là liên tục tại mỗi điểm $ (\lambda_0, x_0) $ của $ K \times M $. Đặt $ y_0 = g(x_0) $. Mọi lân cận của 0 trong $ M $ đều chứa một lân cận có dạng $ g(U) $ trong đó $ U $ là một lân cận của 0 trong $ N $; theo giả thiết tồn tại một lân cận $ V $ của 0 trong $ K $ và một lân cận $ W $ của 0 trong $ N $ sao cho các quan hệ $ \lambda - \lambda_0 \in V $, và $ y - y_0 \in W $ kéo theo $ \lambda y - \lambda_0 y_0 \in U $. Do đó các quan hệ $ \lambda - \lambda_0 \in V $, $ x - x_0 \in g(W) $ kéo theo $ \lambda x - \lambda_0 x_0 \in g(U) $. Ta cũng có thể chứng minh tương tự rằng $ (x, y) \mapsto x - y $ là liên tục trong $ M \times M $.

Với mỗi chỉ số $ i \in I $, cho $ \mathcal{B}_i $ là một hệ cơ bản các lân cận của 0 trong $ E_i $. Theo định nghĩa của tôpô $ \mathcal{T} $, bộ lọc các lân cận của 0 đối với tôpô này được sinh bởi các hợp của các tập thuộc các họ $ f_i^{-1}(\mathcal{B}_i) $; nói cách khác, các tập có dạng $ \bigcap_k f_{i_k}^{-1}(V_{i_k}) $ lập thành một hệ cơ bản các lân cận của 0 đối với $ \mathcal{T} $, trong đó $ (i_k)_{1 \leq k \leq n} $ là một dãy hữu hạn bất kỳ các chỉ số của I, và, với mỗi chỉ số $ k $, $ V_{i_k} $ là một tập bất kỳ của $ \mathcal{B}_{i_k} $.

#### Hệ quả 1 {#evt-i-s1-prop-7-cor-1 .statement}

*Một không gian vectơ tôpô G trên K. Để một tập hợp H các ánh xạ từ G vào E là liên tục đều, điều kiện cần và đủ là, với mọi $ i \in I $, tập hợp $ f_i \circ u $ trong đó u biến thiên trong H là liên tục đều.*

Đây là một trường hợp riêng của GT, X, § 2.2, prop. 3.

#### Hệ quả 2 {#evt-i-s1-prop-7-cor-2 .statement}

*Nếu các không gian $ E_i $ là Hausdorff, thì để $ \mathcal{T} $ là Hausdorff, điều kiện cần và đủ là, với mọi $ x \neq 0 $ trong E, tồn tại một chỉ số $ i \in I $, sao cho $ f_i(x) \neq 0 $.*

Vì khi đó $ \phi(E) $ là một không gian Hausdorff, và để $ \mathcal{T} $ là Hausdorff, hiển nhiên điều kiện cần và đủ là $ \phi $ đơn ánh; chú ý rằng khi đó ta có thể đồng nhất E (với $ \mathcal{T} $) với không gian con $ \phi(E) $ của $ \prod_{i \in I} E_i $ bởi ánh xạ $ \phi $.

#### Hệ quả 3 {#evt-i-s1-prop-7-cor-3 .statement}

*Giả sử các $ E_i $ đầy đủ và $ \phi(E) $ đóng trong $ F = \prod_{i \in I} E_i $. Khi đó E là đầy đủ đối với tôpô $ \mathcal{T} $.*

Vì không gian con $ \phi(E) $ của F khi đó là đầy đủ (GT, II, § 3.4, prop. 8 và § 3.5, prop. 10), do đó điều tương tự đúng với E đối với tôpô ảnh ngược (GT, I, § 7.6, prop. 10 và GT, II, § 3.1, prop. 4).

#### Ví dụ {#evt-i-s1-n7-exa-1 .statement}

— Cho $ \mathcal{D}'(\mathbf{R}) $ là không gian các phân phối trên $ \mathbf{R} $; với $ p $ là một số sao cho $ 1 \leq p \leq +\infty $, cho $ j : L^p(\mathbf{R}) \to \mathcal{D}'(\mathbf{R}) $ là đơn ánh chính tắc, liên tục (khi $ L^p(\mathbf{R}) $ mang tôpô không gian định chuẩn của nó và $ \mathcal{D}'(\mathbf{R}) $ mang tôpô mạnh). Với mọi phân phối $ f \in \mathcal{D}'(\mathbf{R}) $, ký hiệu đạo hàm của $ f $ bởi $ D(f) $; nhắc lại rằng $ f \mapsto D(f) $ là một tự đồng cấu liên tục của $ \mathcal{D}'(\mathbf{R}) $. Khi đó cho E là không gian con vectơ của $ L^p(\mathbf{R}) $ được tạo bởi các $ f \in L^p(\mathbf{R}) $ sao cho $ D(f) \in L^p(\mathbf{R}) $, và trang bị cho E tôpô yếu nhất làm cho đơn ánh chính tắc $ i : E \to L^p(\mathbf{R}) $ và ánh xạ $ D : E \to L^p(\mathbf{R}) $ liên tục ($ L^p(\mathbf{R}) $ mang tôpô không gian định chuẩn của nó). Đối với tôpô này, không gian E là *đầy đủ*. Thật vậy, ảnh của E trong $ F = L^p(\mathbf{R}) \times L^p(\mathbf{R}) $ bởi ánh xạ $ \phi : f \mapsto (f, D(f)) $ là *đóng*, vì nó là vết trên $ L^p(\mathbf{R}) \times L^p(\mathbf{R}) $ của ảnh G của $ \mathcal{D}'(\mathbf{R}) $ trong $ \mathcal{D}'(\mathbf{R}) \times \mathcal{D}'(\mathbf{R}) $ bởi ánh xạ

$$
\phi_0 : f \mapsto (f, D(f));
$$

bây giờ G là đồ thị của $ \phi_0 $, do đó đóng trong $ \mathcal{D}'(\mathbf{R}) \times \mathcal{D}'(\mathbf{R}) $ (GT, I, § 8.1, hệ quả 2 của mệnh đề 2), và vì $ \phi(E) $ là ảnh ngược của G bởi $ i \times i $, vốn liên tục, ta thấy rằng $ \phi(E) $ đóng trong F. \*

#### Hệ quả 4 {#evt-i-s1-prop-7-cor-4 .statement}

*Một không gian vectơ E trên một trường chia được tôpô K, và $ (\mathcal{T}_i)_{i \in I} $ là một họ các tôpô tương thích với cấu trúc không gian vectơ của E; khi đó cận trên $ \mathcal{T} $ của các tôpô $ \mathcal{T}_i $ tương thích với cấu trúc không gian vectơ của E.*

Thật vậy, nếu $ E_t $ ký hiệu không gian vectơ tôpô thu được từ $ E $ nhờ tôpô $ \mathcal{T}_t $, và $ f_t $ là ánh xạ đồng nhất từ $ E $ vào $ E_t $, thì $ \mathcal{T} $ là tôpô thô nhất làm cho các $ f_t $ liên tục.

### Bài tập {#evt-i-s1-exercises}

Xem [các bài tập của § 1](exercises/s1/).
