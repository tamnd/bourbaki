---
book: alg
book_title: Algebra
chapter: V
chapter_title: COMMUTATIVE FIELDS
section: 1
section_title: Prime fields. Characteristic
lang: vi
source: alg-iv-vii
source_edition: 2003, Springer
pdf_pages: 0115-0123, 0259-0260
extraction: ocr
subsections:
    - "no": 1
      title: Prime fields
      page: 0
      pdf_page: 115
    - "no": 2
      title: Characteristic of a ring and of a field
      page: 2
      pdf_page: 116
    - "no": 3
      title: Commutative rings of characteristic p
      page: 3
      pdf_page: 117
    - "no": 4
      title: Perfect rings of characteristic p
      page: 5
      pdf_page: 119
    - "no": 5
      title: Characteristic exponent of a field. Perfect fields
      page: 7
      pdf_page: 121
    - "no": 6
      title: Characterization of polynomials with zero differential
      page: 7
      pdf_page: 121
statements: 23
exercises: 5
content_sha256: 5b7389368dc6bfa2fa03066bf4aac0a7b0cb23ef4c8cfcec89279baa644f5082
translated_from: content/en/alg/V/01_s1_prime_fields_characteristic.md
source_content_sha256: 1386d6b11c452c9e28fae816dceda271a73d913c580b11b29f309d049d175b40
translation_model: gpt-5-6-mini, gpt-5.4-mini
translation_run: translate-vi-78072c4e
glossary_version: 34
glossary_terms_sha256: 546dc1c2d6ff8e87cff78adc3bff2632b820bd6ba5ab15c2bd5a6b0d8f75034f
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 1. TRƯỜNG NGUYÊN TỐ. ĐẶC SỐ

### 1. Các trường nguyên tố

Trường phân thức của vành Z các số nguyên hữu tỉ được gọi là trường các số hữu tỉ và được ký hiệu bởi Q (I, p. 117). Với mọi số nguyên tố p, vành thương $ \mathbf{Z}/(p) $ là một trường hữu hạn $ ^1 $ gồm p phần tử, được ký hiệu bởi $ \mathbf{F}_p $ trong phần tiếp theo. Trường Q là vô hạn vì nó chứa Z, và do đó không đẳng cấu với bất kỳ trường nào $ \mathbf{F}_p $. Nếu p và $ p' $ là các số nguyên tố phân biệt, các trường $ \mathbf{F}_p $ và $ \mathbf{F}_{p'} $ có các lực lượng phân biệt và vì vậy không đẳng cấu.

#### Định nghĩa 1 {#alg-v-s1-def-1 .statement}

Một trường được gọi là nguyên tố nếu nó đẳng cấu hoặc với Q hoặc với một trong các trường $ \mathbf{F}_p $.

Mọi trường con của Q đều chứa vành Z và do đó chứa trường phân thức Q của Z; mọi vành con của $ \mathbf{F}_p $ nhất thiết bằng $ \mathbf{F}_p $. Vì vậy mọi trường con của một trường nguyên tố nhất thiết bằng nó (xem Hệ quả 2 của Định lý 1 dưới đây). Cho P là một trường nguyên tố và A là một vành; nếu f và $ f' $ là hai đồng cấu của P vào A, thì tập hợp của $ x \in P $ sao cho $ f(x) = f'(x) $ là một trường con của P, do đó theo điều đã nói ta phải có $ f = f' $. Đặc biệt, tự đồng cấu duy nhất của một trường nguyên tố là ánh xạ đồng nhất.

$ ^1 $ Do lạm dụng ngôn ngữ, người ta nói rằng một vành hoặc một trường là hữu hạn nếu tập hợp nền của nó là hữu hạn.

#### Định lý 1 {#alg-v-s1-thm-1 .statement}

— Cho $ A $ là một vành ; giả sử rằng tồn tại một trường con của $ A $. Khi đó $ A $ có một trường con duy nhất $ P $ là một trường nguyên tố. Hơn nữa, $ P $ được chứa trong tâm của $ A $ và trong mọi trường con của $ A $.

Cho $ K $ là một trường con của $ A $, $ C $ là tâm của $ A $, và đặt $ K' = K \cap C $; khi đó $ K' $ là một trường con của $ A $. Cho $ f $ là đồng cấu duy nhất của $ \mathbf{Z} $ vào $ A $ và $ p $ là hạt nhân của nó. Mọi vành con của $ A $, đặc biệt là $ K' $, đều chứa $ f(\mathbf{Z}) $; do đó iđêan $ p $ là nguyên tố (I, p. 116-117). Nếu $ p = (0) $, đồng cấu $ f $ của $ \mathbf{Z} $ vào $ K' $ là đơn ánh; do đó nó mở rộng (I, p. 116) thành một đẳng cấu $ \bar{f} $ của $ \mathbf{Q} $ lên một trường con $ P $ của $ K' $. Nếu $ p \neq (0) $, tồn tại một số nguyên dương $ p $ sao cho $ p = (p) $ (I, p. 111); nếu ta có $ p = ab $ với $ a > 1 $ và $ b > 1 $, điều này có nghĩa là $ a \notin p, b \notin p $ và $ ab \in p $ mâu thuẫn với sự kiện rằng $ p $ là nguyên tố. Số $ p $ do đó là nguyên tố và bằng cách chuyển qua thương, $ f $ xác định một đẳng cấu của $ F_p = \mathbf{Z}/p $ lên một trường con $ P $ của $ K' $. Trong cả hai trường hợp $ P $ là một trường con của $ A $ được chứa trong tâm $ C $ của $ A $, và nó là một trường nguyên tố. Cho $ L $ là một trường con của $ A $; khi đó $ P \cap L $ là một trường con của $ P $, và vì $ P $ là nguyên tố, ta có $ P \cap L = P $, do đó $ P \subset L $. Nếu $ P' $ là một trường con của $ A $ và là một trường nguyên tố, thì theo những gì đã nói, $ P \subset P' $, do đó $ P = P' $ vì $ P' $ là một trường nguyên tố.

#### Hệ quả 1 {#alg-v-s1-thm-1-cor-1 .statement}

— Cho $ K $ là một trường. Tồn tại một trường con duy nhất của $ K $ là một trường nguyên tố, và đây là trường con nhỏ nhất của $ K $.

#### Hệ quả 2 {#alg-v-s1-thm-1-cor-2 .statement}

— Để một trường là nguyên tố, điều kiện cần và đủ là nó không chứa trường con nào khác ngoài chính nó.

### 2. Đặc số của một vành và của một trường

Ta sẽ định nghĩa đặc số của một vành $ A $ chỉ khi $ A $ có một trường con. Khi điều này xảy ra, cho $ f $ là đồng cấu vành duy nhất từ $ \mathbf{Z} $ vào $ A $, và cho $ n $ là số nguyên dương duy nhất sinh iđêan của $ \mathbf{Z} $ là hạt nhân của $ f $ (I, p. 111); khi đó số nguyên $ n $ được gọi là đặc số của $ A $.

Cho $ A $ là một vành mà đặc số đã được định nghĩa; khi đó $ A $ không rút gọn về 0. Theo Định lý 1 tồn tại một trường con duy nhất $ P $ của $ A $ là một trường nguyên tố; ta sẽ gọi nó là trường con nguyên tố của $ A $. Theo chứng minh của Định lý 1 có hai khả năng sau:
$ a) $ đặc số của $ A $ là 0, $ P $ đẳng cấu với $ Q $,
$ b) $ đặc số của $ A $ là một số nguyên tố $ p $, $ P $ đẳng cấu với $ \mathbf{F}_p $.

Nếu đặc số của $ A $ là không, tồn tại một đồng cấu vành duy nhất từ $ Q $ vào $ A $; ảnh của nó là trường con nguyên tố của $ A $, được chứa trong tâm của $ A $. Do đó tồn tại một cấu trúc đại số $ Q $ duy nhất của $ A $ tương thích với cấu trúc vành. Khi đặc số của $ A $ là một số nguyên tố $ p $, ta có các tính chất tương ứng khi thay thế trường $ Q $ bởi trường $ \mathbf{F}_p $.

#### Mệnh đề 1 {#alg-v-s1-prop-1 .statement}

— Cho $ A $ là một vành không rút gọn về 0.
$ a) $ Để $ A $ có đặc số 0, điều kiện cần và đủ là ánh xạ $ x \mapsto n \cdot x $ từ $ A $ vào chính nó phải là song ánh, với mọi số nguyên $ n \neq $

b) Cho $ p $ là một số nguyên tố. Để $ A $ có đặc số $ p $, điều kiện cần và đủ là $ p \cdot x = 0 $ với mọi $ x \in A $.

Cho $ f $ là đồng cấu duy nhất của $ \mathbf{Z} $ vào $ A $; ta có $ n \cdot x = f(n)x $ với mọi số nguyên $ n $ và mọi $ x $ trong $ A $. Để $ A $ có đặc số 0, điều kiện cần và đủ là $ f $ mở rộng thành một đồng cấu của $ \mathbf{Q} $ vào $ A $, nghĩa là, $ f(n) $ khả nghịch trong $ A $ với mọi $ n \neq 0 $ (I, p. 113); điều này chứng minh $ a $. Tương tự, để $ A $ có đặc số $ p $ thì điều kiện cần và đủ là $ f $ triệt tiêu $ p\mathbf{Z} $, nghĩa là $ f(p) = 0 $, hoặc cũng là $ p \cdot x = 0 $ với mọi $ x \in A $; điều này chứng minh $ b $.

Xét $ A $ là một trường không nhất thiết giao hoán. Tâm của $ A $ là một trường (giao hoán); do đó đặc số và trường con nguyên tố của $ A $ được xác định.

#### Nhận xét 1 {#alg-v-s1-n2-rem-1 .statement}

Cho $ A $ và $ A' $ là hai vành không suy biến về 0. Giả sử đặc số của $ A $ được xác định và có một đồng cấu $ u $ của $ A $ vào $ A' $. Ảnh qua $ u $ của trường con nguyên tố của $ A $ là một trường con $ P' $ của $ A' $, đẳng cấu với $ P $, và do đó nguyên tố. Suy ra rằng đặc số của $ A' $ được xác định và bằng đặc số của $ A $. Nếu $ A $ và $ A' $ có đặc số 0 (tương ứng $ p \neq 0 $), ánh xạ $ u $ là một đồng cấu của các đại số trên $ \mathbf{Q} $ (tương ứng $ \mathbf{F}_p $).

#### Nhận xét 2 {#alg-v-s1-n2-rem-2 .statement}

Nhận xét 1 chỉ ra rằng nếu $ A $ là một vành có đặc số 0 (tương ứng $ p \neq 0 $), điều tương tự cũng đúng đối với mọi vành $ A' $ chứa $ A $ như vành con, hoặc đối với mọi thương của $ A $ bởi một iđêan hai phía $ a \neq A $. Đặc biệt, nếu $ K $ là một trường, mọi trường con của $ K $ và mọi mở rộng trường của $ K $ đều có cùng đặc số với $ K $.

#### Nhận xét 3 {#alg-v-s1-n2-rem-3 .statement}

Cho $ A $ là một đại số khác không trên một trường $ K $. Vì ánh xạ $ \lambda \mapsto \lambda \cdot 1 $ từ $ K $ vào $ A $ là một đồng cấu vành, Nhận xét 1 cho thấy đặc số của $ A $ được xác định và bằng đặc số của $ K $.

#### Nhận xét 4 {#alg-v-s1-n2-rem-4 .statement}

Vì trường $ \mathbf{Q} $ là vô hạn, mọi vành có đặc số 0 đều vô hạn; suy ra mọi trường hữu hạn đều có đặc số khác không.

#### Nhận xét 5 {#alg-v-s1-n2-rem-5 .statement}

Cho $ A $ là một vành khác không, có nhóm cộng là một $ \mathbf{Z} $-môđun không xoắn, và đặt $ B = \mathbf{Q} \otimes_{\mathbf{Z}} A $. Ánh xạ $ x \mapsto 1 \otimes x $ từ $ A $ vào $ B $ là đơn ánh (II, p. 314), do đó $ A $ đẳng cấu với một vành con của một vành có đặc số 0.

### 3. Các vành giao hoán có đặc số p

Trong Số này và Số tiếp theo, $ p $ ký hiệu một số nguyên tố.

#### Định lý 2 {#alg-v-s1-thm-2 .statement}

— Cho $ A $ là một vành giao hoán có đặc số $ p $. Ánh xạ $ a \mapsto a^p $ là một tự đồng cấu của vành $ A $, nghĩa là ta có các quan hệ

(1) $$(a + b)^p = a^p + b^p$$
(2) $$(ab)^p = a^p b^p$$

với $ a, b $ thuộc $ A $.

Công thức (2) suy ra từ tính giao hoán của $ A $. Để chứng minh (1), ta dùng công thức nhị thức $(a + b)^p = a^p + b^p + \sum_{i=1}^{p-1} \binom{p}{i} \cdot a^i b^{p-i}$; vì $ p \cdot x = 0 $ với mọi $ x \in A $, chỉ cần chứng minh bổ đề sau:

#### Bổ đề 1 {#alg-v-s1-lem-1 .statement}

Cho $ p $ là một số nguyên tố và $ i $ là một số nguyên trong khoảng từ 1 đến $ p - 1 $, khi đó hệ số nhị thức $ \binom{p}{i} $ là một số nguyên chia hết cho $ p $.

Ta lập luận bằng quy nạp theo $ i $, trường hợp $ i = 1 $ là ngay lập tức từ công thức $ \binom{p}{1} = p $. Giả sử $ 2 \leq i \leq p - 1 $ và $ \binom{i}{i-1} $ chia hết cho $ p $. Khi đó số nguyên $ i \binom{p}{i} = (p - i + 1) \binom{p}{i-1} $ thuộc iđêan nguyên tố $ p\mathbf{Z} $ của $ \mathbf{Z} $; vì $ i \notin p\mathbf{Z} $, ta có $ \binom{p}{i} \in p\mathbf{Z} $ và bổ đề được chứng minh.

Cho $ A $ là một vành giao hoán có đặc số $ p $ và $ f $ là một số nguyên $ \geq 0 $. Từ Định lý 2, ta suy ra bằng quy nạp theo $ f $ rằng ánh xạ $ a \mapsto a^{p^f} $ là một tự đồng cấu của vành $ A $. Đặc biệt ta có quan hệ

$$
(a_1 + \cdots + a_n)^{p^f} = a_1^{p^f} + \cdots + a_n^{p^f}
$$

với mọi $ a_1, \ldots, a_n $ thuộc $ A $. Ánh xạ $ a \mapsto a^p $ đôi khi được gọi là *tự đồng cấu Frobenius* của $ A $. Lấy $ A = \mathbf{F}_p $ và $ a_i = 1 $, ta thu được từ (3) quan hệ:

$$
n^{p^f} \equiv n \mod p \quad (n \in \mathbf{Z}, f \in \mathbf{N}) .
$$

Đối với mỗi tập con $ S $ của $ A $, ta ký hiệu $ S^{p^f} $ là tập hợp các phần tử của $ A $ có dạng $ x^{p^f} $ với $ x \in S $^1. Đặc biệt, nếu $ K $ là một vành con của $ A $, thì tập hợp $ K^{p^f} $ là một vành con của $ A $. Nếu $ K $ là một vành con của $ A $ và $ S $ là một tập con của $ A $, ta ký hiệu $ K[S] $ là vành con của $ A $ sinh bởi $ K \cup S $; khi $ A $ là một trường, ta ký hiệu $ K(S) $ là trường phân thức của $ K[S] $, nghĩa là trường con của $ A $ sinh bởi $ K \cup S $.

#### Mệnh đề 2 {#alg-v-s1-prop-2 .statement}

— *Cho $ A $ là một vành giao hoán có đặc số $ p $, $ K $ là một vành con của $ A $, $ S $ là một tập con của $ A $ và $ f $ là một số nguyên dương.*

a) *Ta có $ K[S]^{p^f} = K^{p^f}[S^{p^f}] $, và nếu $ A $ là một trường, $ K(S)^{p^f} = K^{p^f}(S^{p^f}) $.*

b) *Nếu môđun $ K $- $ K[S] $ được sinh bởi họ $ (a_i)_{i \in I} $ các phần tử của $ A $, thì môđun $ K $- $ K[S^{p^f}] $ được sinh bởi họ $ (a_i^{p^f})_{i \in I'} $*

Vì $ K[S] $ là vành con của $ A $ sinh bởi $ K \cup S $, ảnh $ KISlp^f $ của nó qua tự đồng cấu $ \pi : a \mapsto a^{p^f} $ của vành $ A $ là vành con của $ A $ sinh bởi ảnh $ K^{p^f} \cup S^{p^f} $ của $ K \cup S $ qua $ \pi $, do đó $ K[S]^{p^f} = K^{p^f}[S^{p^f}] $. Trường hợp các trường được xử lý tương tự; điều này chứng minh $ a) $.

Hiển nhiên họ $ (a_i^{p^f})_{i \in I} $ sinh $ K^{p^f} $-môđun $ K[S]^{p^f} $. $ K $-môđun $ K[S^{p^f}] $ được sinh bởi các tích có dạng $ x_1^{p^f} \cdots x_n^{p^f} = (x, \ldots x_n)^{p^f} $ với $ x_1, \ldots, x_n $ tùy ý trong $ S $, do đó cũng bởi tập hợp $ K[S]^{p^f} $. Mệnh đề $ b) $ suy ra trực tiếp từ điều này.

^1 Dĩ nhiên tập hợp $ S^{p^f} $ không được nhầm lẫn với tích tập hợp của $ p^f $ tập hợp bằng $ S $, cũng không với tập hợp các tích của $ p^f $ phần tử thuộc $ S $.

### 4. Các vành hoàn hảo có đặc số p

#### Định nghĩa 2 {#alg-v-s1-def-2 .statement}

— Một vành $ A $ có đặc số $ p \neq 0 $ được gọi là hoàn hảo nếu nó giao hoán và ánh xạ $ a \mapsto a^p $ là song ánh.

Nếu vành $ A $ là hoàn hảo có đặc số $ p $, ánh xạ $ a \mapsto a^{p^f} $ là một tự đẳng cấu của vành $ A $ với mọi số nguyên $ f \geq 0 $; tự đẳng cấu nghịch đảo được ký hiệu bởi $ a \mapsto a^{1/p^f} $ hoặc $ a \mapsto a^{p^{-f}} $ và ảnh của một tập con $ S $ của $ A $ qua tự đẳng cấu này được viết là $ S^{1/p^f} $ hoặc $ S^{p^{-f}} $. Hiển nhiên $ (a^{p^e})^{p^f} = a^{p^{e+f}} $ với mọi $ a \in A $ và mọi số nguyên $ e $ và $ f $ (với dấu tùy ý).

Cho $ A $ là một vành giao hoán có đặc số $ p $. Với mọi số nguyên $ f \geq 0 $ ta ký hiệu $ \mathfrak{n}_f $ là hạt nhân của tự đồng cấu $ a \mapsto a^p $ của vành $ A $. Khi đó $ (\mathfrak{n}_f)_{f \geq 0} $ là một dãy tăng các iđêan của $ A $; vì mọi số nguyên dương đều bị chặn trên bởi một lũy thừa của $ p $, iđêan $ \mathfrak{n} = \bigcup_{f \geq 0} \mathfrak{n}_f $ gồm tất cả các phần tử lũy linh của $ A $. Đặc biệt, nếu $ A $ hoàn hảo, mọi phần tử lũy linh của $ A $ đều bằng không.

#### Định nghĩa 3 {#alg-v-s1-def-3 .statement}

— Cho $ A $ là một vành giao hoán có đặc số $ p \neq 0 $. Ta gọi bao đóng hoàn hảo của $ A $ là một cặp $ (A, u) $ trong đó $ A $ là một vành hoàn hảo có đặc số $ p $ và $ u $ là một đồng cấu của $ A $ vào $ A $ thỏa mãn tính chất phổ quát sau:

(PC) *Nếu B là một vành hoàn hảo có đặc số p và v là một đồng cấu của A vào B, thì tồn tại một đồng cấu duy nhất h của A vào B sao cho $ v = h \circ u $.*

Tính chất phổ quát (PC) suy ra ngay tính duy nhất của bao hoàn hảo, theo nghĩa sau: nếu $ (A, u) $ và $ (A', u') $ là hai bao hoàn hảo của $ A $, thì tồn tại duy nhất một đẳng cấu $ h $ từ $ A $ lên $ A' $ sao cho $ u' = h \circ u $ (cf. *E, IV*, p. 23). Ta sẽ nay thiết lập *sự tồn tại* của bao hoàn hảo:

#### Định lý 3 {#alg-v-s1-thm-3 .statement}

— Cho $ A $ là một vành giao hoán có đặc số $ p \neq 0 $. Tồn tại một bao hoàn hảo $ (A, u) $ của $ A $. Hơn nữa, hạt nhân của $ u $ là tập hợp tất cả các phần tử lũy linh của $ A $ và với mỗi $ x \in A $ tồn tại một số nguyên $ n \geq 0 $ sao cho $ x^{p^n} \in u(A) $.

Với mỗi số nguyên $ n \geq 0 $, đặt $ A_n = A $; khi $ m \geq n $ ta định nghĩa một đồng cấu $ \pi_{m,n} $ của $ A_n $ vào $ A_m $ bởi $ \pi_{m,n}(a) = a^{p^{m-n}} $. Do đó ta thu được một hệ trực tiếp các vành $ (A_n, \pi_{m,n}) $ (I, p. 120); cho $ A $ là giới hạn trực tiếp của hệ này và $ u_n $ là đồng cấu chính tắc của $ A_n = A $ vào $ A $; ta cũng đặt $ u = u_0 $. Theo phép dựng giới hạn trực tiếp, hạt nhân $ \mathfrak{n} $ của $ u $ là hợp của các hạt nhân của các đồng cấu π_{n,0}: a \mapsto a^{p^n} của $ A $ vào $ A $, do đó nó gồm tất cả các phần tử lũy linh của $ A $. Vành $ A $ giao hoán có đặc số $ p $ theo Nhận xét 1 của V, p. 3.

Vành $ A $ là hợp của dãy tăng $ (u, (A))_n $ các vành con. Ta có $ u_n(A)^{p^n} = A $; suy ra với mỗi $ x \in \hat{A} $ tồn tại một số nguyên $ n \geq 0 $ sao cho $ x^{p^n} \in u(A) $. Ta cũng có $ u_n(A) = u_{n+1}(A)^p $, do đó $ \hat{A}^p = A $. Cho $ x \in A $ sao cho $ x^p = 0 $; chọn một số nguyên $ n \geq 1 $ và một phần tử $ a \in A $ sao cho $ x = u_n(a) $. Khi đó ta có $ u_{n-1}(a) = u_n(a)^p = 0 $; theo định nghĩa của giới hạn trực tiếp tồn tại một số nguyên $ m $ sao cho $ \pi_m^{1,n-1}(a) = 0 $, tức là $ a^{p^{m-n}} = 0 $. Do đó ta có $ \pi_{m,n}(a) = 0 $, suy ra $ u_n(a) = 0 $, tức là $ x = 0 $. Vì vậy vành $ A $ là vành hoàn hảo có đặc số $ p $.

Với mọi số nguyên $ n \geq 0 $, ánh xạ $ b \mapsto b^{p^n} $ là một tự đẳng cấu của $ B $ và do đó tồn tại một đồng cấu $ v_n $ của $ A, = A $ vào $ B $ được đặc trưng bởi $ v(a) = v_n(a)^{p^n} $. Khi đó ta có $ v_m \circ \pi_{m,n} = v_n $ với $ m \geq n \geq 0 $; theo định nghĩa của giới hạn trực tiếp tồn tại một đồng cấu $ h $ của $ A $ vào $ B $ sao cho $ v_n = h \circ u $, với mọi $ n \geq 0 $; đặc biệt ta có $ v = v_0 = h \circ u_0 = h \circ u $. Cuối cùng, cho $ h' $ là một đồng cấu của $ A $ vào $ B $ sao cho $ h' \circ u = v $. Lấy $ x \in A $; như ta đã thấy, tồn tại một số nguyên $ n \geq 0 $ và một phần tử $ a \in A $ sao cho $ x^{p^n} = u(a) $. Khi đó ta có

$$
h(x)^{p^n} = h(u(a)) = v(a) = h'(u(a)) = h'(x)^{p^n},
$$

và vì $ B $ hoàn hảo, ta suy ra $ h(x) = h'(x) $. Do đó ta có $ h' = h $, và điều này hoàn tất chứng minh rằng $ (A, u) $ là một bao đóng hoàn hảo của $ A $.

#### Mệnh đề 3 {#alg-v-s1-prop-3 .statement}

— *Cho $ B $ là một vành hoàn hảo có đặc số $ p $ và $ A $ là một vành con của $ B $. Viết $ \mathbf{A}^{p^{-\infty}} = \bigcup_{f \geq 0} \mathbf{A}^{p^{-f}} $ và ký hiệu $ j $ là đơn ánh chính tắc của $ A $ trong $ \mathbf{A}^{p^{-\infty}} $. Khi đó $ \mathbf{A}^{p^{-\infty}} $ là vành con hoàn hảo nhỏ nhất của $ B $ chứa $ A $ và $ (\mathbf{A}^{p^{-\infty}}, j) $ là một bao đóng hoàn hảo của $ A $.*

For mỗi số nguyên $ f \in \mathbf{Z} $ ký hiệu $ \pi_f $ là tự đẳng cấu $ b \mapsto b^{p^f} $ của $ B $. Dãy các vành con $ \pi_{-f}(A) $ của $ B $ (với $ f \geq 0 $) là tăng dần và hợp của chúng $ \mathbf{A}^{p^{-\infty}} $ do đó là một vành con của $ B $. Ta có $ \pi_1(\mathbf{A}^{p^{-\infty}}) = \bigcup_{f \geq 0} \pi_{-(f-1)}(A) = \mathbf{A}^{p^{-m}} $, do đó $ \mathbf{A}^{p^{-\infty}} $ là một vành con hoàn hảo của $ B $. Sau cùng, cho $ B_0 $ là một vành con hoàn hảo của $ B $ chứa $ A $; với mọi số nguyên $ f \geq 0 $ ta có $ \pi_{-f}(A) \subset \pi_{-f}(B_0) = B_0 $, do đó $ \mathbf{A}^{p^{-\infty}} \subset B_0 $.

Nếu $ v $ là một đồng cấu từ $ A $ vào một vành hoàn hảo $ B' $ có đặc số $ p $, thì với mọi số nguyên $ f \geq 0 $ ta có thể định nghĩa một đồng cấu $ h_f $ của $ \pi_{-f}(A) $ vào $ B' $ bởi $ h_f(\pi_{-f}(a)) = v(a)^{p^{-f}} $ với mọi $ a \in A $. Ta thấy ngay rằng $ h_{f+1} $ trùng với $ h_f $ trên $ \pi_{-f}(A) $; do đó tồn tại một đồng cấu $ h $ của $ \mathbf{A}^{p^{-\infty}} $ vào $ B' $ sao cho nó cảm sinh $ h_f $ trên $ \pi_{-f}(A) $ với mọi $ f \geq 0 $ và đặc biệt, $ h $ mở rộng $ h_0 = v $. Nếu $ h' $ là một mở rộng khác của $ v $ thành một đồng cấu của $ A^{p^{-\infty}} $ vào B, thì đẳng thức $ h' = h $ có thể được chứng minh như trong chứng minh của ĐL. 3.

### 5. Số mũ đặc số của một trường. Các trường hoàn hảo

Cho $ K $ là một trường. Theo *số mũ đặc số* của $ K $ ta hiểu số nguyên bằng *1* nếu $ K $ có đặc số 0, và bằng đặc số của $ K $ khi số này khác không.

#### Mệnh đề 4 {#alg-v-s1-prop-4 .statement}

— *Cho $ K $ là một trường có số mũ đặc số q. Với mọi số nguyên $ f \geq 0 $ ánh xạ $ x \mapsto x^{q^f} $ là một đẳng cấu của K lên một trong các trường con của nó (được ký hiệu bởi $ K^{q^f} $).*
Điều này suy ra từ ĐL. 2 khi q ≠ 1 và là tầm thường khi q = 1.
Tương tự, ta có thể mở rộng Mđ. 2 đến trường hợp $ A $ là một trường có số mũ đặc số q, trường hợp q = *1* là tầm thường.

#### Định nghĩa 4 {#alg-v-s1-def-4 .statement}

— *Một trường K có số mũ đặc số q được gọi là hoàn hảo nếu ta có $ K^q = K $. Khi $ K^q \neq K $, K được gọi là không hoàn hảo.*
Theo định nghĩa này, một trường là hoàn hảo nếu nó có đặc số 0, hoặc nếu nó là một vành hoàn hảo có đặc số $ p \neq 0 $ theo nghĩa của Định nghĩa 2. Nếu $ K $ là một trường có đặc số $ p \neq 0 $ và $ (K, u) $ là một bao đóng hoàn hảo của $ K $, thì K là một trường theo Mệnh đề 3 *(V, p. 6)* và $ u $ là một đẳng cấu của K lên một trường con của $ \hat{K} $. Thông thường người ta đồng nhất $ K $ với ảnh của nó qua $ u $ trong $ \hat{K} $, do đó ta có $ \hat{K} = K^{p^{-\infty}} $ (Mệnh đề **3**).
Cho K là một trường có đặc số *0* ; khi đó số mũ đặc số của $ K $ là *1*. Theo quy ước, ký hiệu $ x^{q^{-f}} $ và $ S^{q^{-f}} $ được hiểu lần lượt là x và S *(đối với một phần tử $ x $ của $ K $ và một tập con S của $ K$)*. Đặc biệt ta đặt $ K^{q^{-\infty}} = K $ và ta quy ước lấy bao đóng hoàn hảo của $ K $ là $ K $.

#### Mệnh đề 5 {#alg-v-s1-prop-5 .statement}

— *Nếu K là một trường có đặc số 0, hoặc hữu hạn, \* hoặc đóng đại số \*, thì nó hoàn hảo. Đặc biệt mọi trường nguyên tố đều hoàn hảo.*
Giả sử rằng $ K $ có đặc số $ p \neq 0 $. Nếu $ K $ hữu hạn, thì trường con $ K^p $ của $ K $ có cùng lực lượng với $ K $, do đó $ K^p = K $. \* Nếu $ K $ đóng đại số, thì đa thức $ X^p - a $ có một nghiệm $ x $ trong $ K $ đối với mỗi $ a \in K $ *(V, p. 20, Định nghĩa 1)* do đó $ x^p = a $ và suy ra $ K^p = K $. \* Cuối cùng một trường nguyên tố có đặc số *0* hoặc hữu hạn.
Cho $ K_0 $ là một trường có đặc số $ p \neq 0 $ và $ K = K_0(X) $ là trường phân thức hữu tỉ trong một ẩn $ X $ trên $ K_0 $. Khi đó $ K $ là *không hoàn hảo*, vì không có phần tử $ u(X)/v(X) $ nào của $ K $ *(u, v là các đa thức trong $ K_0[X] $)* sao cho $ (u(X)/v(X))^p = X $. Điều này có thể thấy bằng cách viết quan hệ này dưới dạng $ u(X)^p = Xv(X)^p $ và so sánh bậc của hai vế.

### 6. Đặc trưng hóa các đa thức có vi phân bằng không

#### Mệnh đề 6 {#alg-v-s1-prop-6 .statement}

— *Cho K là một vành giao hoán, A là đại số đa thức $ K[X_i]_{i \in I} $, và S là tập hợp các phần tử F của A sao cho $ dF = 0 $. \*

a) *Nếu K là một vành có đặc số 0, thì S = K.*
b) *Nếu K là một vành có đặc số $ p \neq 0 $, thì $ S = K[X_i^p]_{i \in I} $; nếu hơn nữa K hoàn hảo, thì $ K = A^P $. \*

Ánh xạ $ F \mapsto dF $ của A vào môđun $ \Omega_K(A) $ của các vi phân K của A là K-tuyến tính và thỏa mãn quan hệ

$$
d(FF') = F \cdot dF' + F' \cdot dF
$$

(III, p. 569). Do đó S là một đại số con.

Nếu K có đặc số $ p \neq 0 $, ta đặt $ T = K[X_i^p]_{i \in I} $; do đó ta có $ T = A^P $ nếu K hoàn hảo ($ V $, p. 4, Mệnh đề 2); hơn nữa, ta có $ d(X_i^p) = pX_i^{p-1} \cdot dX_i = 0 $ với mọi $ i \in I $, vì vậy đại số con S của A chứa T. Nếu K có đặc số 0, ta đặt $ T = K $, và vẫn thấy rằng $ T \subset S $. Còn lại là phải chứng minh rằng S được chứa trong T.

Với mọi tập con hữu hạn J của I, hãy đặt $ A_J $ là đại số con của A sinh bởi họ $ (X_j)_{j \in J} $. Ta có $ A_\emptyset = K $ và $ A = \bigcup_{J \in I} A_J $; vì vậy chỉ cần chứng minh hệ thức $ S \cap A_J \subset T $, điều mà ta sẽ thực hiện bằng quy nạp theo lực lượng của J. Do đó, hãy lấy J là một tập con hữu hạn của I sao cho $ S \cap A_J \subset T $, lấy i là một phần tử của $ I - J $ và $ J' = J \cup \{ i \} $. Mỗi phần tử F của A có thể được viết theo đúng một cách dưới dạng

$$
F = \sum_{n=0}^\infty F_n \cdot X_i^n,
$$

với $ F_n \in A_J $ với mọi $ n \geq 0 $, và khi đó

$$
dF = \sum_{n=0}^\infty X_i^n \cdot dF_n + \sum_{n=0}^\infty nX_i^{n-1}F_n \cdot dX_i.
$$

Giả sử F thuộc S; họ $ (dX_r)_{r \in J} $ là một cơ sở của A-môđun $ \Omega_K(A) $ (III, p. 570) và $ dF_n $ là một tổ hợp tuyến tính của các vi phân $ dX_j $ với $ j \in J $ vì $ F_n \in A_J = K[X_j]_{j \in J} $. Theo (6) ta có $ dF_n = 0 $ và $ nF_n = 0 $ với mọi số nguyên $ n \geq 0 $. Theo giả thiết quy nạp, $ F_n \in T $ với mọi $ n $, vì $ dF_n = 0 $.

a) Nếu K có đặc số 0, ta có $ nF_n = 0 $ với mọi $ n \geq 1 $, do đó $ F_n = 0 $ theo Mệnh đề 1 ($ V $, p. 2); vì vậy $ F = F_0 $, suy ra $ F \in T $.

b) Nếu K có đặc số $ p \neq 0 $, thì A là một đại số trên trường $ \mathbf{F}_p $ và hệ thức $ nF_n = 0 $ suy ra $ F_n = 0 $ với mọi số nguyên $ n $ không chia hết cho $ p $. Vì vậy ta có $ F = \sum_{m=0}^m F_{mp} X_i^{mp} $, suy ra $ F \in T $

#### Nhận xét {#alg-v-s1-n6-rem-1 .statement}

— Ta vẫn có $ S = K $ khi nhóm cộng của K không xoắn; điều này suy ra từ chứng minh trên hoặc từ Nhận xét 5 của V, p. 3.

#### Hệ quả {#alg-v-s1-n6-cor-1 .statement}

— Cho K là một trường và F(X) là một đa thức có hệ số trong K, có đạo hàm F'(X) bằng 0.
a) Nếu K có đặc số 0, thì F ∈ K.
b) Nếu K có đặc số p ≠ 0, tồn tại một đa thức G(X) sao cho F(X) = G(X^p).
Vì ta có dF = F . dX = 0.

### Bài tập {#alg-v-s1-exercises}

Xem [bài tập cho § 1](exercises/s1/).
