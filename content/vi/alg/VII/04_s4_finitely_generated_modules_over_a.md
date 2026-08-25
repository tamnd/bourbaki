---
book: alg
book_title: Algebra
chapter: VII
chapter_title: MODULES OVER PRINCIPAL IDEAL DOMAINS
section: 4
section_title: Finitely generated modules over a principal ideal domain
lang: vi
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A VII.15-A VII.28, A VII.62-A VII.70
pdf_pages: 0374-0387, 0421-0429
extraction: ocr
subsections:
    - "no": 1
      title: Direct sums of cyclic modules
      page: 15
      pdf_page: 374
    - "no": 2
      title: Content of an element of a free module
      page: 16
      pdf_page: 375
    - "no": 3
      title: Invariant factors of a submodule
      page: 18
      pdf_page: 377
    - "no": 4
      title: Structure of finitely generated modules
      page: 19
      pdf_page: 378
    - "no": 5
      title: Calculation of invariant factors
      page: 20
      pdf_page: 379
    - "no": 6
      title: Linear mappings of free modules, and matrices over a principal ideal domain
      page: 21
      pdf_page: 380
    - "no": 7
      title: Finitely generated abelian groups
      page: 22
      pdf_page: 381
    - "no": 8
      title: Indecomposable modules. Elementary divisors
      page: 23
      pdf_page: 382
    - "no": 9
      title: Duality in modules of finite length over a principal ideal domain
      page: 25
      pdf_page: 384
statements: 40
exercises: 9
content_sha256: 2f7720288bd9b795f6504075d079e8e53bb04c01e53038eaebd8b565da7c7b59
translated_from: content/en/alg/VII/04_s4_finitely_generated_modules_over_a.md
source_content_sha256: 47e1f7b20c598278d3283f70227fe7863b421a8ea32d75c1e037bb13db45ff08
translation_model: gpt-5.4-mini, gpt-5-6-mini, gpt-5-6
translation_run: translate-vi-00516c9d
glossary_version: 34
glossary_terms_sha256: e192c0d24755ab7aa2e4eaaf30c953af00edf0cc460f76dac42a54aa0927393e
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 4. CÁC MÔĐUN HỮU HẠN SINH TRÊN MỘT MIỀN IĐÊAN CHÍNH

### 1. Tổng trực tiếp của các môđun cyclic

Cho $A$ là một vành giao hoán. Nhắc lại (II, p. 220, Mệnh đề 22) rằng một $A$-môđun cyclic đẳng cấu với một *môđun thương* $ A/a $, trong đó $a$ là một iđêan của $A$. Sau này ta sẽ thấy (Mục 4) rằng mọi môđun hữu hạn sinh trên một miền iđêan chính đều là một tổng trực tiếp của hữu hạn nhiều môđun cyclic.

#### Mệnh đề 1 {#alg-vii-s4-prop-1 .statement}

— *Cho $E$ là một môđun trên một vành giao hoán $A$; giả sử $E$ là một tổng trực tiếp của $n$ môđun cyclic $ \Lambda/\mathfrak{a}_k $ ($ 1 \leq k \leq n $), trong đó các $ \mathfrak{a}_k $ là các iđêan của $A$;*

thì, với mỗi số nguyên $ p > 0 $, $A$-môđun $ \bigwedge^p E $ đẳng cấu với tổng trực tiếp của các môđun $ A / a_H $, trong đó với mỗi tập con gồm $p$ phần tử $ H = \{ k_1, \ldots, k_p \} $ của $ [1, n] $, iđêan $ a_H $ là $ \sum_{j=1}^p a_{k_j} $.

Cho $ x_k $ là phần tử sinh chính tắc của $ A / a_k $, tức là ảnh của phần tử đơn vị của $A$, sao cho $ E $ là tổng trực tiếp của các $ Ax_i $ ($ 1 \leq i \leq n $). Khi đó ta biết (III, p. 515, Mệnh đề 10) rằng đại số ngoài $ \bigwedge^n E $ đẳng cấu với tư cách một $ A $-môđun với tích tenxơ $ \bigotimes_{i=1}^n (\bigwedge (Ax_i)) $. Lúc này $ \bigwedge (Ax_i) $ chỉ là tổng trực tiếp $ A \oplus Ax_i $, vì tích ngoài của bất kỳ hai phần tử nào của $ Ax_i $ đều bằng không, và do đó $ \bigwedge^p E $ là tổng trực tiếp của các môđun $ M_H = (Ax_{k_1}) \otimes \ldots \otimes (Ax_{k_p}) $ khi $ H = \{ k_1, \ldots, k_p \} $ chạy qua tập các tập con $p$ phần tử của $ [1, n] $ (với $ k_1 < \ldots < k_p $) ; nay $ M_H $ được biết là đẳng cấu với $ A / a_{11} $ (II, p. 257, Hệ quả 4), điều này hoàn tất chứng minh.

Ta thấy ngay rằng, theo ký hiệu của Mệnh đề 1, nếu các iđêan $ a_k $ tạo thành một dãy tăng, thì chúng được xác định hoàn toàn bởi môđun $ E $. Chính xác hơn :

#### Mệnh đề 2 {#alg-vii-s4-prop-2 .statement}

— *Cho $ A $ là một vành giao hoán, và cho $ E $ là một tổng trực tiếp của $ n $ môđun cyclic $ A / a_k $, trong đó các $ a_k $ thỏa mãn $ a_1 \subset a_2 \subset \ldots \subset a_n $. Khi đó, với $ 1 \leq p \leq n $, iđêan $ a_p $ là linh hóa tử của $ \bigwedge^p E $; nếu $ a_n \neq A $ thì $ \bigwedge^p E \neq 0 $ với $ 1 \leq p \leq n $ và $ \bigwedge^m E = 0 $ với $ m > n $.*

Theo ký hiệu của Mệnh đề 1, ta có $ a_p = a_{s(H)} $, trong đó $ s(H) $ là phần tử lớn nhất của tập con $ H $. Vì $ s(H) \geq p $ với mọi tập con gồm $ p $ phần tử $ H $, và vì $ s(H) = p $ đối với $ H = \{ 1, \ldots, p \} $, suy ra $ a_p $ là giao của các $ a_r $, khi $ H $ biến thiên trên tập hợp các tập con gồm $ p $ phần tử của $ (1, n) $; do đó iđêan $ a_p $ quả thật là linh hóa tử của $ \bigwedge^p E $, theo Mệnh đề 1.

#### Hệ quả {#alg-vii-s4-n1-cor-1 .statement}

— *Trong ký hiệu của Mệnh đề 2, nếu $ a_n \neq A $, và nếu $ E $ cũng đẳng cấu với tổng trực tiếp của $ m $ môđun cyclic $ A / a'_j $ với $ a'_1 \subset a'_2 \subset \ldots \subset a'_m \neq A $, thì $ m = n $ và $ a_k = a'_k $ với $ 1 \leq k \leq n $ (*tính duy nhất của $ a_k *$).

### 2. Nội dung của một phần tử của một môđun tự do

Cho $ A $ là một miền iđêan chính, cho $ L $ là một $ A $-môđun tự do, và cho $ x $ là một phần tử của $ L $. Khi $ f $ chạy qua tập hợp $ L^* $ các dạng tuyến tính trên $ L $, các phần tử $ f(x) $ tạo thành một iđêan $ c_L(x) $ của $ A $, được gọi là *nội dung* của $ x $ trong $ L $. Một phần tử $ c $ của $ A $ được gọi là một *nội dung* của $ x $ trong $ L $ nếu nó sinh ra iđêan $ c_{L}(x) $; điều này tương đương với việc nói rằng tồn tại một dạng tuyến tính $ f $ trên $ L $ sao cho $ f(x) = c $ và $ c $ chia hết $ g(x) $ với mọi dạng tuyến tính $ g $ trên $ L $. Cho $ (e_i)_{i \in I} $ là một cơ sở của $ L $; đặt $ x = \sum a_i e_i, a_i \in A $; khi đó iđêan $ c_L(x) $ gồm các tổng $ \sum a_i b_i $, khi $ (b_i) $ chạy qua tập hợp $ A' $; suy ra ngay lập tức rằng một phần tử $ c $ của $ A $ là một nội dung của $ x $ trong $ L $ khi và chỉ khi nó là một ước chung lớn nhất của họ $ (a_i) $ các tọa độ của $ x $.

Ta nói rằng $ x $ là *không thể chia được* nếu $ c_L(x) = A $, nghĩa là nếu các tọa độ của $ x $ đối với một cơ sở của $ L $ là nguyên tố cùng nhau từng đôi một.

#### Bổ đề 1 {#alg-vii-s4-lem-1 .statement}

*Cho $ L $ là một môđun tự do trên một miền iđêan chính $ A $ và cho $ x $ là một phần tử của $ L $. Khi đó các điều kiện sau là tương đương*:

(i) $ x $ là không thể chia được ;
(ii) *tồn tại một dạng tuyến tính $ f $ trên $ L $ sao cho $ f(x) = 1$ ;
(iii) $ x $ là khác không và môđun con $ Ax $ là một nhân tử trực tiếp của $ L $ ;
(iv) $ x $ là một phần tử của một cơ sở nào đó của $ L $.

(i) $ \Rightarrow $ (ii) : điều này suy ra từ định nghĩa.
(ii) $ \Rightarrow $ (iii) : cho $ f $ là một dạng tuyến tính trên $ L $ sao cho $ f(x) = 1$ ; khi đó $ x \neq 0 $ và ánh xạ $ y \mapsto f(y)x $ là một phép chiếu của $ L $, với ảnh $ Ax $.
(iii) $ \Rightarrow $ (iv) : cho $ L' $ là một phần bù của $ Ax $ trong $ L $, và cho $ B' $ là một cơ sở của $ L' $ (*VII*, p. 15, Hệ quả 2) ; khi đó $ B' \cup \{x\} $ là một cơ sở của $ L $.
(iv) $ \Rightarrow $ (i) : tầm thường.

#### Nhận xét {#alg-vii-s4-n2-rem-1 .statement}

— 1) Nếu $ x $ là một phần tử khác không của $ L $ và $ c $ là một nội dung của $ x $, thì tồn tại một phần tử duy nhất $ y $ của $ L $ sao cho $ x = cy $ ; ký hiệu phần tử này là $ x/c $ ; khi đó $ x/c $ là một phần tử không phân chia được của $ L $.
2) Nội dung $ c_L(x) $ là linh hóa tử của môđun xoắn của $ L/Ax $.

Cho $ L $ là một môđun tự do trên một miền iđêan chính $ A $ và cho $ M $ là một môđun con của $ L $ ; theo *VII*, p. 4, Bổ đề 1, họ $ c_L(x), x \in M $, có một phần tử cực đại ; nếu $ M \neq \{0\} $ thì một phần tử cực đại như vậy là khác không.

#### Mệnh đề 3 {#alg-vii-s4-prop-3 .statement}

*Cho $ L $ là một môđun tự do trên một miền iđêan chính $ A $ và cho $ M $ là một môđun con khác không của $ L $. Cho $ x $ là một phần tử của $ M $ sao cho $ c_L(x) $ là cực đại trong số các nội dung của các phần tử của $ M $, cho $ c $ là một nội dung của $ x $ trong $ L $, và cho $ f $ là một dạng tuyến tính trên $ L $ sao cho $ f(x) = c$.

a) $ L $ là tổng trực tiếp của $ A(x/c) $ và hạt nhân $ K $ của $ f $.
b) $ M $ là tổng trực tiếp của $ Ax $ và $ K \cap M $.
c) $ g(M) \subset Ac $ đối với mọi dạng tuyến tính $ g $ trên $ L $.*

Đặt $ y = x/c $ ; rõ ràng $ Ay \cap K = \{0\} $, vì $ f(y) = 1 $. Hơn nữa, với mỗi $ u \in L $ ta có
$$
u = f(u)\,y + (u - f(u)\,y),
$$
với $ f(u)y \in Ay $ và $ u - f(u)y \in K $ ; điều này chứng minh *a)*. Bây giờ chú ý rằng với $ u \in M $ ta có $ f(u) \in Ac $ : thật vậy, cho $ u \in M $, và cho $ d $ là một ước chung lớn nhất của $ f(u) $ và $ c $ ; khi đó tồn tại $ \lambda, \mu \in A $ sao cho $ d = Xf(u) + \mu c = f(Xu + \mu x) $ ; do đó nội dung của phần tử $ \lambda u + \mu x $ của $ M $ chia hết $ d $ ; bởi tính cực đại của $ c $, điều này suy ra rằng $ d $ là một phần tử liên kết của $ c $, vậy $ f(u) \in Ac $. Vì thế với mọi $ u $ trong $ M $, ta có thể viết
$$
u = (f(u)/c)\,x + (u - (f(u)/c)\,x) \in Ax + (K \cap M),
$$
điều này chứng minh *b)*. Cuối cùng, cho $ g $ là một dạng tuyến tính trên $ L $ ; theo *a)* tồn tại một vô hướng $ \alpha \in A $ và một dạng tuyến tính $ h $ trên $ K $ sao cho $ g(u) = \alpha f(u) + h(u - f(u)\,y) $ ; do đó theo

b) ta có $ g(M) \subset Ac + h(K \cap M) $. Để chứng minh c), do đó chỉ cần chứng minh rằng $ h(K \cap M) \subset Ac $ với mọi dạng tuyến tính $ h $ trên $ K $, hay tương đương với mọi dạng tuyến tính $ h $ trên $ L $ sao cho $ h(x) = 0 $; bây giờ, nếu $ u \in K \cap M $ và $ d $ là một ước chung lớn nhất của $ h(u) $ và $ c $, thì tồn tại $ A, \mu \in A $ với $ d = \lambda h(u) + \mu c $; khi đó $ (f + h)(Au + \mu x) = d $, điều này suy ra như trên rằng $ h(u) \in Ac $, và c) được suy ra.

### 3. Các nhân tử bất biến của một môđun con

#### Định lý 1 {#alg-vii-s4-thm-1 .statement}

— Cho $ L $ là một môđun tự do trên một miền iđêan chính $ A $, và cho $ M $ là một môđun con của $ L $ có hạng hữu hạn $ n $. Khi đó tồn tại một cơ sở $ B $ của $ L $, $ n $ phần tử $ e_i $ của $ B $, và $ n $ phần tử khác không $ \alpha_i $ của $ A $ ($ 1 \leq i \leq n $) sao cho:
a) các $ \alpha_i e_i $ lập thành một cơ sở của $ M $;
b) $ a_i $ chia hết cho $ \alpha_{i-1} $, với $ 1 \leq i \leq n-1 $.

Hơn nữa môđun $ M' $ sinh bởi các $ (e_i) $ và các iđêan chính $ A\alpha_i $ được xác định duy nhất bởi các điều kiện trên; môđun $ M'/M $ là môđun con xoắn của $ L/M $, và đẳng cấu với tổng trực tiếp của các $ A $-môđun $ A/A\alpha_i $; cuối cùng $ L/M $ là tổng trực tiếp của $ M'/M $ và một môđun tự do đẳng cấu với $ L/M' $.

1) Sự tồn tại của các $ e_i $ và các $ \alpha_i $.

Nếu $ M = \{0\} $ thì định lý là tầm thường. Nếu $ M \neq \{0\} $ thì từ Mệnh đề 3 suy ra rằng tồn tại một phần tử $ e_1 $ của $ L $, một phần tử khác không $ a $, của $ A $, và một môđun con $ L_1 $ của $ L $, sao cho $ L $ là tổng trực tiếp của $ Ae_1 $ và $ L_1 $, sao cho $ M $ là tổng trực tiếp của $ A\alpha_1 e_1 $ và môđun con $ M_1 = M \cap L_1 $ của $ L $, và sao cho $ g(M) \subset A\alpha_1 $ với mọi dạng tuyến tính $ g $ trên $ L $.

Bây giờ ta có thể tiến hành bằng quy nạp theo hạng $ n $ của $ M $. Vì $ L_1 $ là một môđun tự do (VII, p. 15, Hệ quả 2) và $ M_1 $ có hạng $ n-1 $, tồn tại một cơ sở $ B_1 $ của $ L_1 $, $ (n-1) $ phần tử $ e_2, \ldots, e_n $ của $ B_1 $, và các phần tử khác không $ \alpha_2, \ldots, a $, của $ A $ sao cho $ (\alpha_2 e_2, \ldots, \alpha_n e_n) $ là một cơ sở của $ M_1 $, và $ \alpha_i $ chia hết $ \alpha_{i+1} $ với $ 2 \leq i \leq n-1 $. Nếu $ L' $ là môđun con của $ L $, sinh bởi các phần tử của $ B_1 $ phân biệt với $ e_1, \ldots, e_n $, thì $ L $ là tổng trực tiếp của $ L' $ và môđun $ M' $ sinh bởi các phần tử $ e_1, \ldots, e_n $; khi đó $ (e_1, \ldots, e_n) $ là một cơ sở của $ M' $, và $ (\alpha_1 e_1, \ldots, \alpha_n e_n) $ là một cơ sở của $ M $. Bây giờ chỉ còn phải chứng minh rằng $ a_i $ chia hết $ a_i $; nhưng $ A\alpha_2 $ có dạng $ g(M_1) $, trong đó $ g $ là dạng tuyến tính trên $ L $ được xác định bởi $ g(e_2) = 1, g(e_i) = 0 $ với $ i \neq 2 $, và $ g(L') = (0) $; và ta đã thấy ở trên rằng $ g(M_1) \subset A\alpha_1 $.

2) Các tính chất về tính duy nhất.

Vì các $ a_i $ là khác không, môđun $ M' $ là tập hợp các $ x \in L $ sao cho $ \beta x \in M $ với một $ \beta \neq 0 $ nào đó trong $ A $; nói cách khác $ M'/M $ là môđun con xoắn của $ L/M $. Điều này xác định duy nhất $ M' $.

Rõ ràng rằng $ M'/M $ đẳng cấu với tổng trực tiếp của $ n $ môđun cyclic $ A/A\alpha_i $ (II, p. 204, công thức (26)). Gọi $ r $ là số các iđêan $ A\alpha $, khác với $ A $: do đó $ n-r $ iđêan đầu tiên $ A\alpha_i $ bằng $ A $, và $ r $ iđêan cuối cùng khác với $ A $. Khi đó $ M'/M $ cũng đẳng cấu với tổng trực tiếp của các môđun $ A/A\alpha_n, \ldots, A/A\alpha_{n-r+1} $, trong đó $ A\alpha_n \subset A\alpha_{n-1} \subset \ldots \subset A\alpha_{n-r+1} \neq A $.

Như vậy các điều kiện của Hệ quả của Mệnh đề 2 (VII, p. 16) được thỏa mãn: các iđêan $ Aa_i $ ($ 1 \leq i \leq n $) do đó được xác định duy nhất bởi môđun $ M'/M $.

Vì $ L $ là tổng trực tiếp của $ M' $ và $ L' $, suy ra $ L/M $ là tổng của $ M'/M $ và $ (L' + M)/M $, và tổng này là trực tiếp vì $ (L' + M) \cap M' = M $; mặt khác $ (L' + M)/M $ đẳng cấu với $ L'/(M \cap L') $ (I, p. 41, Định lý 4, c)), tức là với $ L' $, điều đó cho thấy rằng $ (L' + M)/M $ là một môđun tự do đẳng cấu với $ L/M' $.

#### Hệ quả {#alg-vii-s4-n3-cor-1 .statement}

— Một môđun con $ M $ có hạng hữu hạn trong một môđun tự do $ L $ trên một miền iđêan chính $ A $ có một phần bù trong $ L $ khi và chỉ khi $ L/M $ là môđun không xoắn.

Theo ký hiệu của Định lý 1, nếu $ L/M $ là môđun không xoắn, thì $ M = M' $, và $ M' $ có một phần bù $ L' $ trong $ L $. Ngược lại nếu $ M $ có một phần bù $ L' $ trong $ L $, thì $ L/M $ đẳng cấu với $ L' $, vốn là tự do (VII, p. 15, Hệ quả 2), và a fortiori không xoắn.

#### Nhận xét {#alg-vii-s4-n3-rem-1 .statement}

Có thể xảy ra rằng một môđun con $ M $ có hạng vô hạn trong một môđun tự do $ L $ sao cho $ L/M $ là môđun không xoắn, nhưng $ M $ không có phần bù nào trong $ L $ (VII, p. 60, Ex. 6, b)).

#### Định nghĩa 1 {#alg-vii-s4-def-1 .statement}

— Theo ký hiệu và các giả thiết của Định lý 1, các iđêan $ A\alpha_i $ của $ A $ được gọi là các thừa số bất biến của môđun con $ M $ đối với môđun $ L $.

Trong trường hợp $ A $ là hoặc vành $ \mathbf{Z} $ của các số nguyên, hoặc vành đa thức $ K[X] $ theo một ẩn trên một trường $ K $, có một cách chính tắc để chọn một phần tử sinh cho mỗi iđêan của $ A$: một số nguyên dương trong trường hợp của $ \mathbf{Z} $, hoặc một đa thức đơn khởi trong trường hợp của $ K[X] $ (VII, p. 5). Trong mỗi trường hợp này, phần tử sinh chính tắc của nhân tử bất biến $ Aa_i $ cũng được gọi là một nhân tử bất biến của $ M $ đối với $ L $, theo lối nói lạm dụng.

### 4. Cấu trúc của các môđun hữu hạn sinh

#### Định lý 2 {#alg-vii-s4-thm-2 .statement}

— Mọi môđun hữu hạn sinh $ E $ trên một miền iđêan chính $ A $ đều đẳng cấu với một tổng trực tiếp của một số hữu hạn $ m $ môđun cyclic $ A/a_k $, trong đó các $ a_k $ là các iđêan của $ A $ (một số trong đó có thể bằng không) sao cho $ a_1 \subset a_2 \subset \ldots \subset a_m \neq A $, và chúng được xác định duy nhất bởi các điều kiện này.

Nếu $ E $ có thể được sinh bởi $ q $ phần tử thì nó đẳng cấu với một môđun thương $ L/M $, trong đó $ L = A^q $ (II. p. 218). Vì $ M $ có hạng hữu hạn $ n \leq q $ (VII, p. 15, Mệnh đề 1), các điều kiện của Định lý 1 (VII, p. 18) được thỏa mãn. Khi đó, theo ký hiệu của Định lý 1, $ L/M $ đẳng cấu với một tổng trực tiếp của một phần bù $ L' $ của $ M' $ trong $ L $ và môđun xoắn $ M'/M $. Môđun $ L' $ là tự do có hạng hữu hạn $ p = q - n $, nên đẳng cấu với $ A^p $. Nếu $ r $ là chỉ số nhỏ nhất sao cho $ A\alpha_r \neq A $, thì $ M'/M $ đẳng cấu với tổng trực tiếp của các môđun $ A/A\alpha_i $ với $ r \leq i \leq n $. Các điều kiện đã nêu sẽ được thỏa mãn nếu ta lấy $ m = p + (n - r + 1) $, $ a_k = (0) $ với $ 1 \leq k \leq p $, và $ a_j = A\alpha_n , - , $ với $ 1 \leq j \leq n - r + 1 $. Tính duy nhất suy ra từ Hệ quả của VII, p. 16.

#### Hệ quả 1 {#alg-vii-s4-thm-2-cor-1 .statement}

— *Mọi môđun hữu hạn sinh E trên một miền iđêan chính đều là tổng trực tiếp của môđun con xoắn của E và một môđun tự do.*

Môđun con xoắn của $E$ nói chung có nhiều phần bù phân biệt. Chẳng hạn, nếu $ E = \mathbf{Z} \times (\mathbf{Z}/(2)) $ thì môđun con xoắn của $E$ là $ \{0\} \times (\mathbf{Z}/(2)) $; nó có làm một phần bù môđun con $ \mathbf{Z} \times (0) $, và cũng có môđun con gồm mọi phần tử $ (n, \overline{n}) $, trong đó $ n $ chạy qua $ \mathbf{Z} $ và $ \overline{n} $ là lớp thặng dư của $ n $ mod 2.

#### Hệ quả 2 {#alg-vii-s4-thm-2-cor-2 .statement}

— *Mọi môđun hữu hạn sinh không xoắn trên một miền iđêan chính đều tự do có hạng hữu hạn.*
Điều này suy ra ngay lập tức từ Hệ quả 1.

Điều kiện là môđun phải hữu hạn sinh là cốt yếu. Chẳng hạn, nhóm cộng của trường phân thức $K$ của $A$ là không xoắn như một A-môđun; tuy nhiên nó không phải là một môđun tự do nếu $ A \neq K $, vì một mặt bất kỳ hai phần tử nào của $K$ cũng có một ước chung, và mặt khác $K$ không phải là một môđun cyclic trên $A$, vì nếu không thì $ K = ab^{-1}A $ ($ a, b \in A $), do đó $ b^{-2} = acb^{-1} $ ($ c \in A $), suy ra $ b^{-1} = ac \in A $, và $ K = A $.

#### Định nghĩa 2 {#alg-vii-s4-def-2 .statement}

— *Trong ký hiệu và các giả thiết của Định lý 2, các iđêan $ a_k $ được gọi là các nhân tử bất biến của môđun E.*
Như trong Định nghĩa 1 (VII, p. 19), khi $ A = \mathbf{Z} $ hoặc $ A = K[X] $, phần tử sinh chính tắc của iđêan $ a_k $ (một số nguyên dương hoặc một đa thức đơn khởi) cũng được gọi, theo lối nói lạm dụng, là một *nhân tử bất biến* của môđun hữu hạn sinh E.

Cần cẩn thận để không nhầm các nhân tử bất biến của một môđun E với các nhân tử bất biến của một môđun con $ M $ của một môđun tự do $ L $ *đối với* môđun $ L $ (Định nghĩa I).

### 5. Tính toán các nhân tử bất biến

#### Mệnh đề 4 {#alg-vii-s4-prop-4 .statement}

— Cho A là một miền iđêan chính, cho L là một A-môđun tự do với cơ sở hữu hạn $ (u_j) $ ($ 1 \leq j \leq k $), cho M là một môđun con của L, cho $ (x_i) $ là một hệ sinh của M và cho $ A \alpha_i $ ($ 1 \leq i \leq n $) là các nhân tử bất biến của M đối với L. Khi đó với $ 1 \leq m \leq n $ tích $ \delta_m = \alpha_1 \ldots \alpha_m $ là một ước chung lớn nhất của các định thức con cấp m của ma trận có các cột là các vectơ tọa độ của $ x_i $ đối với cơ sở $ (u_j) $.

Theo Định lý 1, rõ ràng là $ M \subset \alpha_1 L $; do đó các tọa độ của mọi phần tử của M là các bội của $ a_1 $. Mặt khác, tồn tại một phần tử $ x $ của M sao cho $ a_1 $ là nội dung trong L. Biểu diễn $ x $ như một tổ hợp tuyến tính của các $ x_i $, suy ra rằng $ a_1 $ là một phần tử của iđêan sinh bởi các tọa độ của các $ x_i $. Vì tất cả các tọa độ này đều là các bội của $ a_1 $, suy ra rằng $ a_1 $ thực sự là ước chung lớn nhất của chúng, và mệnh đề của ta được chứng minh trong trường hợp $ m = 1 $.

Với $ m $ bất kỳ, xét *lũy thừa ngoài* cấp m $ \bigwedge^m M $ của M (III, p. 507). Theo ký hiệu của Định lý 1, tồn tại một cơ sở $ (a_i) $ cho M trong đó $ a_i = \alpha_i e_i $ ($ 1 \leq i \leq n $); do đó $ \bigwedge^m M $ có một cơ sở gồm các phần tử $ a_{i_1} \wedge \ldots \wedge a_{i_m} $, khi $ (i_1, \ldots, i_m) $ chạy qua tập hợp các dãy tăng ngặt gồm $ m $ phần tử của $(1, n)$. Bây giờ các phần tử $ e_{i_1} \wedge \ldots \wedge e_{i_m} $ thuộc một cơ sở $ B_m $ của $ \bigwedge^m L $. Vì vậy ánh xạ chính tắc từ $ \bigwedge^m M $ vào $ \bigwedge^m L $ là một đẳng cấu từ $ \bigwedge^m M $ lên môđun con của $ \bigwedge^m L $ có một cơ sở là các phần tử $ (\alpha_{i_1} \ldots \alpha_{i_m})\, e_{i_1} \wedge \ldots \wedge e_{i_m} $, và ta đồng nhất môđun con này với $ \bigwedge^m M $. Vì $ \alpha_j $ là một bội của $ \alpha_k $ với $ j \geq k $, các phần tử $ \alpha_{i_1} \ldots \alpha_{i_m} $ đều là các bội của $ \delta_m = \alpha_1 \ldots \alpha_m $, và một trong số chúng bằng $ \delta_m $; do đó $ \delta_m $ là một ước chung lớn nhất của các tọa độ đối với $ B_m $ của các phần tử của một hệ sinh của $ \bigwedge^m M $. Phần đầu của lập luận cho thấy rằng khi đó $ \delta_m $ là một ước chung lớn nhất của tập hợp các tọa độ của mọi hệ sinh của $ \bigwedge^m M $, đối với mọi cơ sở của $ \bigwedge^m L $. Lấy cơ sở cho $ \bigwedge^m L $ cảm sinh từ cơ sở $ (u_j) $ của $ L $, và hệ sinh cho $ \bigwedge^m M $ gồm các tích ngoài của các $ (x_i) $, biểu thức của các tọa độ của các tích này theo các định thức (III, p. 528, Mệnh đề 9) cho kết quả đã nêu.

### 6. Ánh xạ tuyến tính của các môđun tự do, và các ma trận trên một miền iđêan chính

Cho $ A $ là một miền iđêan chính. Xét một ánh xạ tuyến tính $ f $ từ một $ A $-môđun tự do $ L $ có hạng $ m $ vào một $ A $-môđun tự do $ L' $ có hạng $ n $. Các kết quả trước cho phép ta, bằng cách chọn các cơ sở thích hợp cho $ L $ và $ L' $, đưa ma trận của $ f $ về một dạng đặc biệt đơn giản, gọi là *dạng chính tắc* của ma trận.

#### Mệnh đề 5 {#alg-vii-s4-prop-5 .statement}

*Cho $ A $ là một miền iđêan chính, và $ f $ là một ánh xạ tuyến tính có hạng $ r $ từ một $ A $-môđun tự do $ L $ có hạng $ m $ vào một $ A $-môđun tự do $ L' $ có hạng $ n $. Khi đó tồn tại các cơ sở $ (e_i) $ ($ 1 \leq i \leq m $) của $ L $ và $ (e'_j) $ ($ 1 \leq j \leq n $) của $ L' $ sao cho $ f(e_i) = \alpha_i e'_i $ với $ 1 \leq i \leq r $ và $ f(e_i) = 0 $ với $ i > r $, trong đó các $ \alpha_i $ là các phần tử khác không của $ A $, mỗi phần tử chia hết phần tử tiếp theo; các iđêan $ A \alpha_i $ là các thừa số bất biến của $ f(L) $ trong $ L' $, và do đó được xác định duy nhất.*

Cho $ L_0 = f^{-1}(0) $ là hạt nhân của $ f $; môđun thương $ L/L_0 $ đẳng cấu với môđun $ f(L) $, là một môđun con của $ L' $ và do đó tự do (*VII*, p. 15, Hệ quả 2); vì vậy $ L_0 $ có một môđun bù $ L_1 $ trong $ L $ (*II*, p. 218, Mệnh đề 21), và hạn chế của $ f $ trên $ L_1 $ là một đẳng cấu từ $ L_1 $ lên $ f(L) = M' $. Nếu các iđêan $ A \alpha_i $ ($ 1 \leq i \leq r $) là các thừa số bất biến của $ M' $ trong $ L' $, thì Định lý 1 của *VII*, p. 18 cho thấy rằng tồn tại một cơ sở $ (e'_j) $ ($ 1 \leq j \leq n $) của $ L' $ sao cho $ (\alpha_i e'_i) $ ($ 1 \leq i \leq r $) là một cơ sở của $ M' $. Vì hạn chế của $ f $ trên $ L_1 $ là một đẳng cấu từ $ L_1 $ lên $ M' $, tồn tại một cơ sở $ (e_i) $ ($ 1 \leq i \leq r $) của $ L_1 $ sao cho $ f(e_i) = \alpha_i e'_i $. Cơ sở này mở rộng thành một cơ sở $ (e_s) $ ($ 1 \leq k \leq m $) của $ L $ bằng cách lấy $ (e_s) $ ($ r+1 \leq s \leq m $) là một cơ sở của hạt nhân $ L_0 $.

#### Hệ quả 1 {#alg-vii-s4-prop-5-cor-1 .statement}

— Cho X là một ma trận có hạng r, với n hàng và m cột, trên một miền iđêan chính A; khi đó tồn tại một ma trận $ X_0 $ tương đương với X (II, p. 354) có dạng

$$
\begin{pmatrix}
\alpha_1 & 0 & \ldots & 0 & 0 & \ldots & 0 \\
0 & \alpha_2 & \ldots & 0 & 0 & \ldots & 0 \\
0 & 0 & \ldots & \alpha_r & 0 & \ldots & 0 \\
0 & 0 & \ldots & 0 & 0 & \ldots & 0 \\
0 & 0 & \ldots & 0 & 0 & \ldots & 0
\end{pmatrix}
$$

trong đó $ \alpha_i $ là các phần tử khác không của A, mỗi phần tử chia hết phần tử tiếp theo. Với các điều kiện này, các $ \alpha_i $ được xác định duy nhất sai khác bởi phép nhân với các phần tử khả nghịch.

Cho hai ma trận X và $ X' $ là tương đương nếu tồn tại các ma trận vuông khả nghịch P và Q, có cấp n và m, trên A, sao cho $ X' = PXQ $, Hệ quả 1 chỉ là Mệnh đề 5 được biểu diễn theo các ma trận.

Theo ký hiệu của Mệnh đề 5 và Hệ quả 1, các iđêan (khác không) $ Au $, được gọi là các thừa số bất biến của ánh xạ tuyến tính f, hoặc của ma trận X. Khi đó suy ra ngay lập tức từ Hệ quả I rằng:

#### Hệ quả 2 {#alg-vii-s4-prop-5-cor-2 .statement}

— Hai ma trận X và $ X' $ có n hàng và m cột trên một miền iđêan chính A là tương đương khi và chỉ khi chúng có cùng các thừa số bất biến.

Chú ý rằng khi A là một trường ta có thể lấy các $ \alpha_i $ bằng 1, và khi đó ta thu được Mệnh đề 13 của II, p. 360.

Nếu X là ma trận của ánh xạ tuyến tính f đối với một cơ sở tùy ý của L và một cơ sở tùy ý của L', thì các cột của X là các vectơ tọa độ, đối với cơ sở của L', của các phần tử của L' tạo thành một hệ sinh của $ f(L) $. Kết quả sau đây do đó là một hệ quả ngay lập tức của Mệnh đề 4.

#### Mệnh đề 6 {#alg-vii-s4-prop-6 .statement}

— Cho X là một ma trận có hạng r trên một miền iđêan chính A, và cho $ A \alpha_i $ ($ 1 \leq i \leq r $) là dãy các thừa số bất biến của nó. Khi đó $ \alpha_1 $ là một ước chung lớn nhất của các phần tử của X; và tích $ \alpha_1 \ldots \alpha_q $ là một ước chung lớn nhất của các định thức con cấp q của X với $ q \leq r $.

### 7. Các nhóm Abel sinh hữu hạn

Trong trường hợp $ A = \mathbf{Z} $, các kết quả của tiết diện 4 có thể được biểu diễn

#### Định lý 3 {#alg-vii-s4-thm-3 .statement}

— Mọi nhóm Abel sinh hữu hạn G đều là tổng trực tiếp của nhóm con xoắn F của nó (nhóm con các phần tử có cấp hữu hạn trong G) và một nhóm Abel tự do có hạng hữu hạn p (đẳng cấu với $ \mathbf{Z}^p $). Nhóm F là một tổng trực tiếp của một số hữu hạn các nhóm cyclic có cấp $ n_1, n_2, \ldots, n_q $, trong đó các $ n_i $ là các số nguyên $ > 1 $, mỗi số chia hết số đứng trước nó; hơn nữa, các số nguyên $ p, q $ và $ n_i $ ($ 1 \leq i \leq q $) được xác định duy nhất bởi $ G $.

#### Nhận xét {#alg-vii-s4-n7-rem-1 .statement}

Trong khi các cấp $ n_1, \ldots, n_q $ của các nhóm chu trình mà F là tổng trực tiếp được xác định rõ bởi điều kiện chia hết của Định lý 3, thì điều đó *không* đúng với chính các nhóm: chẳng hạn, trong tích G của $ \mathbf{Z}/(p) $ với chính nó (với p nguyên tố), các nhóm con chính xác là các không gian con vectơ trên $ \mathbf{F}_p $, và G là tổng trực tiếp của hai không gian con một chiều theo $ p(p+1) $ cách khác nhau.

#### Hệ quả 1 {#alg-vii-s4-thm-3-cor-1 .statement}

— *Trong một nhóm Abel hữu hạn G, tồn tại một phần tử có cấp là bội chung nhỏ nhất của tất cả các cấp của các phần tử của G; cấp này n là nhân tử bất biến thứ nhất của G.*

#### Hệ quả 2 {#alg-vii-s4-thm-3-cor-2 .statement}

— *Bất kỳ nhóm Abel hữu hạn G nào có cấp không chia hết cho bình phương của bất kỳ số nguyên $ > 1 $ nào cũng là nhóm chu trình.*
Ta cứ theo ký hiệu của Định lý 3. Khi đó $ p = 0 $ vì G là hữu hạn, và $ q \leq 1 $, vì nếu không cấp của G sẽ chia hết cho $ n_q^2 $. Do đó G là nhóm chu trình.

#### Hệ quả 3 {#alg-vii-s4-thm-3-cor-3 .statement}

— *Cho L và M là hai $ \mathbf{Z} $-môđun tự do hạng n, cho $ (e_i) $ là một cơ sở của L và $ (f_i) $ là một cơ sở của M ($ 1 \leq i \leq n $), cho u là một đồng cấu từ L vào M, và cho U là ma trận của nó đối với các cơ sở $ (e_i) $ và $ (f_i) $. Khi đó $ \mathrm{Coker}\,u = M/u(L) $ là hữu hạn khi và chỉ khi $ \det(U) \neq 0 $, và khi ấy $ \mathrm{Card}(\mathrm{Coker}(u)) = |\det(U)| $.
Bằng cách đổi cơ sở trong L và M nếu cần, ta có thể giả sử U có dạng được mô tả trong VII, p. 22, Hệ quả 1 của Mệnh đề 5 (trong đó các $ a_i $ trong trường hợp này là các số nguyên); hệ quả đó khi ấy trở nên hiển nhiên, vì cấp của một tổng trực tiếp của các $ \mathbf{Z} $-môđun $ \mathbf{Z}/\alpha_i \mathbf{Z} $ ($ 1 \leq i \leq n $) là vô hạn nếu một trong các $ a_i $ bằng không, và bằng $ |\alpha_1 \alpha_2 \ldots a_n| $ nếu không.*

### 8. Môđun không phân tích được. Ước số sơ cấp

#### Định nghĩa 3 {#alg-vii-s4-def-3 .statement}

— *Một môđun trái M trên một vành A được gọi là phân tích được nếu nó là tổng trực tiếp của một họ các môđun con thực sự khác không. Nếu không thì nó được gọi là không phân tích được.*
Môđun không do đó là *phân tích được*, vì nó là tổng trực tiếp của họ rỗng các môđun con.
Cho $ \mathfrak{a} $ là một iđêan trái của vành A; các môđun con của $ A/\mathfrak{a} $ chỉ là các thương số $ b/\mathfrak{a} $, trong đó $ b $ là một iđêan của A chứa $ \mathfrak{a} $ (I, p. 41, Định lý 4); nếu $ b $ và $ c $ là hai iđêan của A chứa $ \mathfrak{a} $, thì môđun $ A/\mathfrak{a} $ là tổng trực tiếp của các môđun con $ b/\mathfrak{a} $ và $ c/\mathfrak{a} $ khi và chỉ khi $ A = b + c $ và $ b \cap c = \mathfrak{a} $. Từ đó suy ra:

#### Bổ đề 2 {#alg-vii-s4-lem-2 .statement}

— *Môđun $ A/\mathfrak{a} $ là không phân tích được khi và chỉ khi $ \mathfrak{a} \neq A $ và không có cặp $ (b, c) $ các iđêan của A, khác với A và $ \mathfrak{a} $, sao cho $ A = b + c $ và $ b \cap c = \mathfrak{a} $.*

#### Mệnh đề 7 {#alg-vii-s4-prop-7 .statement}

— Cho $ A $ là một vành giao hoán, cho $ \mathfrak{p} $ là một iđêan nguyên tố của $ A $ (I, p. 117, Định nghĩa 3), và cho $ q $ là một iđêan của $ A $ được chứa trong $ \mathfrak{p} $. Giả sử rằng với mọi $ x \in \mathfrak{p} $ đều tồn tại một số nguyên $ n > 0 $ sao cho $ x^n \in q $. Khi đó $ A $-môđun $ A/q $ là không phân tích được.

Cho $ b $ và $ c $ là hai iđêan của $ A $, sao cho $ A = b + c $ và $ b \cap c = q $. Khi đó $ bc \subset b \cap c = q \subset \mathfrak{p} $; nếu $ x \notin \mathfrak{p} $ và $ x \in c $, thì $ xb \subset p $, do đó $ b \subset \mathfrak{p} $ (I, p. 316, Mệnh đề 4); suy ra hoặc $ b \subset \mathfrak{p} $ hoặc $ c \subset p $. Giả sử chẳng hạn rằng $ c \subset \mathfrak{p} $, do đó $ b + p = A $; khi đó tồn tại $ x \in b $ và $ y \in \mathfrak{p} $ sao cho $ 1 = x + y $; lấy $ n \in \mathbf{N} $ sao cho $ y^n \in q $; khi đó $ 1 = (x + y)^n $. vậy $ 1 \in xA + y^nA \subset b + q \subset b $, do đó $ b = A $. Bổ đề 2 bây giờ cho thấy rằng $ A/q $ là không phân tích được.

Bây giờ giả sử rằng $ A $ là một miền iđêan chính; theo VII, p. 2, Mệnh đề 2, các iđêan nguyên tố của $ A $ là các iđêan $ (p) $, trong đó $ p $ là một phần tử bất khả quy của $ A $, và iđêan $ 0 $; theo mệnh đề trước, các môđun $ A $ và $ A/(p^n) $, với $ p $ bất khả quy và $ n > 0 $, là không phân tích được. Vì mọi môđun cyclic là một tổng trực tiếp của các môđun kiểu này (VII, p. 3, Mệnh đề 4) và vì mọi $ A $-môđun sinh hữu hạn là một tổng trực tiếp của các môđun cyclic (VII, p. 19, Định lý 2), ta suy ra:

#### Mệnh đề 8 {#alg-vii-s4-prop-8 .statement}

— Cho $ A $ là một miền iđêan chính và cho $ M $ là một $ A $-môđun sinh hữu hạn.

a) $ M $ là không phân tích được khi và chỉ khi nó đẳng cấu với $ A $ hoặc với một môđun có dạng $ A/(p^n) $, trong đó $ p $ là một phần tử bất khả quy của $ A $ và $ n > 0 $ là một số nguyên.

b) $ M $ là một tổng trực tiếp của một họ hữu hạn các môđun con không phân tích được.

Phần b) của mệnh đề trên có thể được làm chính xác hơn như sau:

#### Mệnh đề 9 {#alg-vii-s4-prop-9 .statement}

— Cho $ A $ là một miền iđêan chính, cho $ P $ là một hệ đại diện của các phần tử bất khả quy của $ A $ và cho $ M $ là một $ A $-môđun sinh hữu hạn. Khi đó tồn tại các số nguyên dương $ m(0) $ và $ m(p^n) $ ($ p \in P, n > 0 $), được xác định duy nhất bởi $ M $ và bằng không trừ một số hữu hạn trong chúng, sao cho $ M $ đẳng cấu với tổng trực tiếp của $ A^{m(0)} $ và các $ (A/(p^n))^{m(p^n)} $ ($ p \in P, n > 0 $).

Sự tồn tại của các số nguyên $ m(0) $ và $ m(p^n) $ ($ p \in P, n > 0 $) suy ra từ Mệnh đề 8. Số nguyên $ m(0) $ được xác định duy nhất: nó là hạng của môđun tự do là thương của $ M $ bởi môđun con xoắn của nó. Cuối cùng, thành phần $ p $-nguyên sơ của $ M $ đẳng cấu với tổng trực tiếp của các $ (A/(p^n))^{m(p^n)} $; vì họ các iđêan $ (p^n) $ ($ n \geq 1 $) được sắp thứ tự toàn phần bởi quan hệ bao hàm, tính duy nhất của $ m(p^n) $ suy ra từ Hệ quả của Mệnh đề 2 của VII, p. 16.

#### Định nghĩa 4 {#alg-vii-s4-def-4 .statement}

— Theo ký hiệu của Mệnh đề 9, các iđêan $ (p^n) $ ($ p \in P, n \geq 1 $ một số nguyên) sao cho $ m(p^n) > 0 $ được gọi là các ước sơ cấp của môđun $ M $, và các số nguyên $ m(p^n) $ được gọi là các bội số của chúng; nếu số nguyên $ m(0) $ là $ > 0 $, nó được gọi là bội số của ước sơ cấp 0.

Đối với các nhân tử bất biến (VII, p. 19, Định nghĩa 1), khi $ A = \mathbf{Z} $ hoặc $ A = K[X] $ (K là một trường giao hoán), thì phần tử sinh chính tắc của iđêan $ (p^n) $ (một số nguyên dương hoặc một đa thức đơn khởi) cũng được gọi, theo sự lạm dụng ngôn ngữ, là một ước sơ cấp của môđun sinh hữu hạn $ M $.

#### Nhận xét 1 {#alg-vii-s4-n8-rem-1 .statement}

Nếu $ M $ là một nhóm Abel hữu hạn, thì cấu trúc của nó có thể được mô tả bằng cách viết ra các ước sơ cấp của nó, mỗi ước được lặp lại số lần bằng bội số của nó. Chẳng hạn, ta sẽ nói rằng $ M $ là « kiểu $(2, 2, 4, 27, 27, 25)$ » (hoặc rằng nó là « một nhóm $(2, 2, 4, 27, 27, 25)$ ») nếu nó đẳng cấu với tích của hai nhóm $ \mathbf{Z}/(2) $, một nhóm $ \mathbf{Z}/(2^2) $, hai nhóm $ \mathbf{Z}/(3^3) $ và một nhóm $ \mathbf{Z}/(5^2) $.

#### Nhận xét 2 {#alg-vii-s4-n8-rem-2 .statement}

Nếu một môđun xoắn sinh hữu hạn $ M $ trên một miền iđêan chính $ A $ được cho dưới dạng tổng trực tiếp của các môđun cyclic đẳng cấu với $ A/(a_i) $ (đặc biệt nếu các nhân tử bất biến của $ M $ đã biết), thì các ước sơ cấp của $ M $, và các bội số của chúng, có thể được xác định bằng cách nhận xét rằng $ A/(a) $ đẳng cấu với tích của các $ A/(p^{n(p)}) $, trong đó $ a = e \prod_{p \in P} p^{n(p)} $ là phân tích của $ a $ thành các nhân tử bất khả quy ($ VII $, p. 3). Ta hãy nghiên cứu chẳng hạn nhóm nhân $ G(464\ 600) $, trong đó $ G(n) $ ký hiệu nhóm nhân $ (\mathbf{Z}/n\mathbf{Z})^* $ ($ VII $, p. 12). Vì $ 464\ 600 = 2^3 \cdot 5 \cdot 23 \cdot 101 $, nhóm này đẳng cấu với tích của các nhóm $ G(2^3) $, $ G(5^2) $, $ G(23) $ và $ G(101) $ ($ VII $, p. 13, Định lý 3); khi đó ba nhóm cuối là cyclic có các cấp 20, 22 và 100, và $ G(2^3) $ là tích của hai nhóm cyclic cấp 2 (\emph{loc. cit.}); vì $ 20 = 2^2 \cdot 5 $, $ 22 = 2 \cdot 11 $ và $ 100 = 2' \cdot 5^2 $, nhóm $ G(464\ 600) $ có kiểu $(2, 2, 2, 2^2, 2^2, 2^2, 5, 5^2, 11)$.

#### Nhận xét 3 {#alg-vii-s4-n8-rem-3 .statement}

Để tính các nhân tử bất biến của một môđun xoắn mà các ước sơ cấp đã biết, ta lại dựa vào sự kiện rằng, nếu $ a_i $ là các phần tử từng đôi một nguyên tố cùng nhau của $ A $, thì tích $ \prod A/(a_i) $ là một môđun cyclic đẳng cấu với $ A/(a_1 a_2 ... a_n) $ ($ VII $, p. 3, Mệnh đề 4). Ta minh họa phương pháp bằng cách xét ví dụ về nhóm $ G(464\ 600) = M $: viết các ước sơ cấp $ p^n $ của $ M $ là các lũy thừa của cùng một phần tử bất khả quy $ p $ trên cùng một dòng, bắt đầu bằng những ước có số mũ lớn nhất; kéo dài các dòng này thành những dòng có cùng độ dài bằng cách điền các số 1 khi cần thiết:

$$
\begin{array}{cccccc}
2^2 & 2^2 & 2 & 2 & 2 \\
5^2 & 5 & 1 & 1 & 1 \\
11 & 1 & 1 & 1 & 1 .
\end{array}
$$

Khi đó các nhân tử bất biến là các tích của các phần tử trong cùng một cột: $ 1100, 20, 2, 2, 2 $. Thật vậy, $ M $ đẳng cấu với một tích của các nhóm cyclic có cấp lần lượt là 1100, 20, 2, 2, 2 theo Mệnh đề 4 của $ VII $, p. 3; vì mỗi cấp trong số này là một bội của cấp tiếp theo, nên đây là các nhân tử bất biến của $ M $ ($ VII $, p. 22, Định lý 3).

#### Nhận xét 4 {#alg-vii-s4-n8-rem-4 .statement}

Một $ A $-môđun được gọi là đơn ($ I $, p. 37) nếu khác không và không có môđun con nào ngoài chính nó và $ 0 $; khi đó nó nhất thiết là cyclic, do đó sinh hữu hạn, và không phân tích được; vì các môđun $ A/(p^n) $ không đơn với $ n \neq 1 $, trong khi các môđun $ A/(p) $ là đơn, và vì $ A $ đơn khi và chỉ khi vành $ A $ là một trường, ta suy ra rằng các $ A $-môđun đơn là:
$ a) $ các môđun tự do hạng 1, khi $ A $ là một trường;
$ b) $ các môđun đẳng cấu với các thương $ A/(p) $, trong đó $ p $ là một phần tử bất khả quy của $ A $, khi $ A $ không phải là một trường.

### 9. Đối ngẫu trong các môđun có độ dài hữu hạn trên một miền iđêan chính

Trong tiết diện này $ A $ ký hiệu một miền iđêan chính không phải là một trường (và do đó có ít nhất một phần tử bất khả quy), và $ K $ là trường các phân thức của $ A $. Với mọi $ A $-môđun $ M $, đặt

$$
D(M) = \operatorname{Hom}_A(M, K/A);
$$

ta biết rằng $ D(M) $ được trang bị cấu trúc của một A-môđun theo một cách tự nhiên, cụ thể là với mọi đồng cấu $ u : M \to K/A $ và mọi $ \alpha \in A $, đồng cấu $ \alpha u $ ánh xạ $ x $ thành $ \alpha u(x) = u(\alpha x) $. Với mỗi đồng cấu $ f : M \to N $ của các A-môđun, ta có đồng cấu $ D(f) : D(N) \to D(M) $, trong đó $ D(f)(v) = v \circ f $ (II, p. 196). Với $ x \in M $ và $ x' \in D(M) $, đặt $ \langle x, x' \rangle = x'(x) \in K/A $ ; khi đó $ (x, x') \mapsto \langle x, x' \rangle $ là một ánh xạ *A-song tuyến tính* từ $ M \times D(M) $ vào $ K/A $, được gọi là *chính tắc*.

Nếu M và $ N $ là hai A-môđun, thì với mỗi ánh xạ A-song tuyến tính $ \varphi : M \times N \to K/A $ ta có các ánh xạ A-tuyến tính $ d_\varphi : N \to D(M) $ và $ s_\varphi : M \to D(N) $, trong đó $ d_\varphi(y)(x) = \varphi(x, y) = s_\varphi(x)(y) $ (II, p. 268, Hệ quả của Mệnh đề *1*). Đặc biệt, ánh xạ A-song tuyến tính chính tắc $ M \times D(M) \to K/A $ xác định một ánh xạ A-tuyến tính (cũng được gọi là *chính tắc*)

$$
c_M : M \to D(D(M))
$$

sao cho $ \langle x', c_M(x) \rangle = \langle x, x' \rangle $ với $ x \in M $ và $ x' \in D(M) $.

#### Mệnh đề 10 {#alg-vii-s4-prop-10 .statement}

— *Nếu $ M $ là một A-môđun có độ dài hữu hạn thì $ D(M) $ là* (nói chung không tự nhiên) *đẳng cấu với $ M $, và ánh xạ chính tắc $ c_M : M \to D(D(M)) $ là một đẳng cấu.*
Dùng VII, p. *19*, Định lý 2 và **II**, p. 203, Hệ quả 1, ta rút gọn về trường hợp $ M $ là đơn sinh. Vì vậy ta có thể giả sử rằng $ M = A/tA $ với $ t \neq 0 $. Chú ý rằng mọi đồng cấu $ u : A/tA \to K/A $ đều được xác định hoàn toàn bởi ảnh $ \xi \in K/A $ của lớp $ \varepsilon $ của *1* mod $ tA $ dưới $ u $, và phần tử này phải thỏa mãn quan hệ $ t\xi = 0 $ ; ngược lại, với mọi $ \xi \in K/A $ sao cho $ t\xi = 0 $, tồn tại một đồng cấu $ u : A/tA \to K/A $ sao cho $ u(\varepsilon) = \xi $. Suy ra $ D(M) $ đẳng cấu với $ t^{-1}A/A $, và vì phép vị tự bởi $ t $ là một song ánh trên K, ta cũng có $ D(M) $ đẳng cấu với $ A/tA $, điều đó chứng minh mệnh đề thứ nhất. Điều này chứng tỏ rằng $ M $ và $ D(D(M)) $ đẳng cấu, nên có cùng độ dài ; mặt khác $ c_M $ là đơn ánh, vì nếu $ y \in A $ sao cho quan hệ $ tz \in A $ (với $ z \in K $) kéo theo $ yz \in A $, thì lấy $ z = t^{-1} $ ta có $ y \in tA $. Suy ra ảnh $ c_M(M) $ tất yếu bằng $ D(D(M)) $.

#### Hệ quả {#alg-vii-s4-n9-cor-1 .statement}

— *Cho M, N là hai A-môđun có độ dài hữu hạn, và cho $ \varphi $ là một ánh xạ A-song tuyến tính từ $ M \times N $ vào $ K/A $, sao cho : 1) quan hệ $ \varphi(x, y) = 0 $ với mọi $ y \in N $ kéo theo $ x = 0 $ ; và 2) quan hệ $ \varphi(x, y) = 0 $ với mọi $ x \in M $ kéo theo $ y = 0 $. Khi đó các ánh xạ A-tuyến tính $ s_\varphi : M \to D(N) $ và $ d_\varphi : N \to D(M) $ liên kết với $ \varphi $ là các đẳng cấu.*
Thật vậy, các giả thiết về $ \varphi $ cho thấy $ s_\varphi $ và $ d_\varphi $ là *đơn ánh* và vì $ \mathrm{long}(D(N)) = \mathrm{long}(N) $ và $ \mathrm{long}(D(M)) = \mathrm{long}(M) $ theo Mệnh đề *10*, điều đó suy ra rằng $ \mathrm{long}(M) = \mathrm{long}(N) $, và do đó $ s_\varphi $ và $ d_\varphi $ là song ánh.

#### Mệnh đề 11 {#alg-vii-s4-prop-11 .statement}

— *Nếu $ M' \xrightarrow{u} M \xrightarrow{v} M'' $ là một dãy khớp các A-môđun có độ dài hữu hạn, thì dãy $ D(M'') \xrightarrow{D(v)} D(M) \xrightarrow{D(u)} D(M') $ là khớp* [^1].

Trước hết hãy chứng minh rằng, cho một dãy khớp

(1)
$$
0 \to M' \to M \to M'' \to 0
$$

thì dãy tương ứng

$$
0 \to D(M'') \to D(M) \to D(M') \to 0
$$

là khớp; thật vậy, ta biết rằng dãy

$$
0 \to D(M'') \to D(M) \to D(M')
$$

là khớp (II, p. 227, Định lý 1); mặt khác, từ (1) suy ra rằng

$$
\operatorname{long}(M) = \operatorname{long}(M') + \operatorname{long}(M'')
$$

(II, p. 212, Mệnh đề 16); theo Mệnh đề 10, do đó ta có

$$
\operatorname{long}(D(M)) = \operatorname{long}(D(M')) + \operatorname{long}(D(M''))
$$

nói cách khác $ \operatorname{long}(D(M')) = \operatorname{long}(D(M)/D(M'')) $. Vì $ D(M)/D(M'') $ được đồng nhất một cách tự nhiên với một môđun con của $ D(M') $, nó phải bằng $ D(M') $, điều này chứng minh mệnh đề của chúng ta.

Điều này suy ra ngay lập tức rằng nếu $ u : M' \to M $ là đơn ánh, thì $ D(u) : D(M) \to D(M') $ là toàn ánh; kết luận sau đó suy ra từ II, p. 199, nhận xét 4.

Với mọi A-môđun M, ký hiệu $ \mathfrak{S}(M) $ là tập hợp các môđun con của M. Với mọi môđun con N của M (tương ứng mọi môđun con N' của D(M)), ký hiệu $ N^0 $ (tương ứng $ {N'}^0 $) là môđun con của $ D(M) $ (tương ứng M) gồm các $ x' \in D(M) $ (tương ứng $ x \in M $) sao cho $ (y, x') = 0 $ với mọi $ y \in N $ (tương ứng $ (x, y') = 0 $ với mọi $ y' \in N' $).

#### Mệnh đề 12 {#alg-vii-s4-prop-12 .statement}

*Cho M là một A-môđun có độ dài hữu hạn. Khi đó ánh xạ gán cho mỗi môđun con N của M môđun $ N^0 $ là một song ánh từ $ \mathfrak{S}(M) $ lên $ \mathfrak{S}(D(M)) $, và song ánh ngược gán cho mỗi môđun con N' của D(M) môđun con $ {N'}^0 $ của M; môđun $ D(N) $ được đồng nhất một cách tự nhiên với $ D(M)/N^0 $ và $ D(M/N) $ với $ N^0 $. Hơn nữa, ta có*

(2)
$$
(N_1 + N_2)^0 = N_1^0 \cap N_2^0, \quad (N_1 \cap N_2)^0 = N_1^0 + N_2^0
$$

với mọi môđun con $ N_1, N_2 $ của M.

Với mỗi môđun con N của M, có một dãy khớp

$$
0 \to N \to M \to M/N \to 0
$$

và do đó (Mệnh đề 11) một dãy khớp

$$
0 \to D(M/N) \to D(M) \to D(N) \to 0
$$

và vì ảnh của $ D(M/N) $ trong $ D(M) $ hiển nhiên là $ N^0 $, ta thấy (Mệnh đề 10) rằng $ \operatorname{long}(N^0) = \operatorname{long}(M) - \operatorname{long}(N) $; vì $ M $ được đồng nhất với $ D(D(M)) $ bởi Mệnh đề 10, tương tự ta có

$$
\operatorname{long}(N^{00}) = \operatorname{long}(M) - \operatorname{long}(N^0) = \operatorname{long}(N);
$$

ngoài ra rõ ràng là $ N \subset N^{00} $, do đó $ N^{00} = N $. Hơn nữa quan hệ đầu tiên trong (2) là hiển nhiên, và bằng cách áp dụng nó cho các môđun con $ N_1^0 $ và $ N_2^0 $ của $ D(M) $, ta có $ (N_1^0 + N_2^0)^0 = N_1 \cap N_2 $, do đó $ N_1^0 + N_2^0 = (N_1^0 + N_2^0)^{00} = (N_1 \cap N_2)^0 $. Điều này hoàn tất chứng minh mệnh đề.

#### Ví dụ 1 {#alg-vii-s4-n9-exa-1 .statement}

Với $ A = \mathbf{Z} $, các $ \mathbf{Z} $-môđun có độ dài hữu hạn chính xác là các nhóm Abel hữu hạn; khi đó $ K = \mathbf{Q} $, nên $ K/A = \mathbf{Q}/\mathbf{Z} $. Khi đó để định nghĩa $ D(M) $, đôi khi ta lấy, thay vì $ \mathbf{Q}/\mathbf{Z} $, một $ \mathbf{Z} $-môđun đẳng cấu với nó, chẳng hạn như (V, p. 79, Mệnh đề 2) nhóm $ R $ các căn đơn vị (đối với phép nhân) trong một trường đóng đại số có đặc số 0 ; khi đó ta đặt $ D(M) = \operatorname{Hom}_{\mathbf{Z}}(M, R) $. Ta để cho độc giả viết lại các kết quả trước đó cho trường hợp riêng này bằng ký hiệu tương ứng.

#### Ví dụ 2 {#alg-vii-s4-n9-exa-2 .statement}

Cho $ a $ là một phần tử khác không của $ A $. Ánh xạ $ x \mapsto x/a $ từ $ A $ vào $ K $ xác định một đẳng cấu trên các môđun thương từ $ A/(a) $ lên môđun con $ (K/A)(a) $ của $ K/A $ gồm các phần tử bị triệt tiêu bởi $ a $. Nếu $ M $ là một $ A $-môđun bị triệt tiêu bởi $ a $, hay tương đương là một $ A/(a) $-môđun, thì $ A $-môđun $ D(M) $ được đồng nhất với $ \operatorname{Hom}_{A/(a)}(M, A/(a)) $. Chúng tôi để bạn đọc viết lại các kết quả trên cho trường hợp đặc biệt này trong ký hiệu tương ứng (xem V, p. 86).

### Bài tập {#alg-vii-s4-exercises}

Xem [các bài tập cho § 4](exercises/s4/).

[^1]: Sau này ta sẽ thấy (A, X, p. 18) rằng A-môđun K/A là đơn ánh. Suy ra Mệnh đề 11 vẫn đúng đối với các A-môđun tùy ý M, M' và M".
