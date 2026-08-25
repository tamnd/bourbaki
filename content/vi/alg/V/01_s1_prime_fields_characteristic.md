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
content_sha256: b93fe2a197f1a111f8ecc47e62d605b987be4553ca39172ad49d30e234f841c7
translated_from: content/en/alg/V/01_s1_prime_fields_characteristic.md
source_content_sha256: 1386d6b11c452c9e28fae816dceda271a73d913c580b11b29f309d049d175b40
translation_model: gpt-5-6-mini
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
