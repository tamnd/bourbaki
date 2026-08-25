---
book: alg
book_title: Algebra
chapter: V
chapter_title: COMMUTATIVE FIELDS
section: 5
section_title: p-radical extensions
lang: vi
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A V.24-A V.26, A V.150-A V.151
pdf_pages: 0138-0140, 0264-0265
extraction: ocr
subsections:
    - "no": 1
      title: p-radical elements
      page: 24
      pdf_page: 138
    - "no": 2
      title: pradical extensions
      page: 25
      pdf_page: 139
statements: 8
exercises: 3
content_sha256: 196b614ab3102b402d49df0f873f92d0659fef6dca6e7dd98d503ecfd07ab7bc
translated_from: content/en/alg/V/05_s5_p_radical_extensions.md
source_content_sha256: a6aac90fb95dde1ede976db5b8a9e4ce3a61bf397137340698aadb5298fcb373
translation_model: gpt-5-6-mini
translation_run: translate-vi-7639faec
glossary_version: 34
glossary_terms_sha256: 58419569485a69f0d6d48e59947b20939d5d378c0a8a360188ef19dc741ae2e5
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 5. *p*-CĂN

*Trong suốt đoạn này, chữ p ký hiệu một số nguyên hoặc bằng 1 hoặc là một số nguyên tố. Tất cả các trường được xét đều có đặc số p. Tất cả các kết quả được phát biểu trong đoạn này đều tầm thường khi $ p = 1 $.*

### 1. Phần tử p-căn

#### Định nghĩa 1 {#alg-v-s5-def-1 .statement}

*Một phần tử x của một mở rộng E của trường K được gọi là p-căn trên K nếu tồn tại một số nguyên $ m \geq 0 $ sao cho $ x^{p^m} \in K $; số nguyên nhỏ nhất trong các số nguyên này được gọi là chiều cao của x (trên K).*

#### Mệnh đề 1 {#alg-v-s5-prop-1 .statement}

*Nếu E là một mở rộng của trường K và x là một phần tử p-căn có chiều cao e trên K; đặt $ a = x^{p^e} $. Khi đó $ a \in K $ và đa thức tối tiểu của x trên K là $ X^{p^e} - a $: Hơn nữa ta có $ [K(x):K] = p^e $.*

Chỉ cần chứng minh rằng đa thức $ X^{p^e} - a $ là bất khả quy trong $ K[X] $. Theo định nghĩa chiều cao của x, ta có $ a \notin K^p $, do đó mệnh đề suy ra từ bổ đề:

*Bổ đề 1. — Cho K là một trường và a là một phần tử của K sao cho $ a \notin K^p $. Khi đó, với mọi số nguyên $ e \geq 0 $, đa thức $ f(X) = X^{p^e} - a $ là bất khả quy trong $ K[X] $.*

Cho $ \Omega $ là một bao đóng đại số của $ K $ và cho b là phần tử $ a^{p^{-e}} $ của $ \Omega $; ta ký hiệu g là đa thức tối tiểu của b trên $ K $. Ta có $ f(X) = (X - b)^{p^e} $ và do đó mọi đa thức bất khả quy trong $ K[X] $ chia hết f đều nhận b làm nghiệm, và vì thế bằng g. Do đó tồn tại (*IV*, p. 13, Mệnh đề 13) một số nguyên $ q \geq 1 $ sao cho $ f = g^q $; vì q chia bậc $ p^e $ của f, nên tồn tại một số nguyên $ e' $ sao cho $ 0 \leq e' \leq e $ và $ q = p^{e'} $. Nếu c là số hạng hằng của g, ta có $ -a = c^q $; vì ta giả sử a không thuộc $ K^p $, nên phải có $ q = 1 $, tức là $ f = g $, và bổ đề được chứng minh.

### 2. Mở rộng p-căn

#### Định nghĩa 2 {#alg-v-s5-def-2 .statement}

Cho E là một mở rộng của trường K. Ta nói rằng E là p-căn $ ^1 $ (trên K) nếu mọi phần tử của E đều p-căn trên K. Khi đó, E được gọi là có chiều cao hữu hạn nếu tập hợp các chiều cao của các phần tử của E bị chặn trên, và ta gọi chiều cao của E là giá trị lớn nhất của các chiều cao của các phần tử của nó.

Ta chú ý rằng mọi mở rộng p-căn của một trường hoàn hảo (đặc biệt là của một trường có đặc số 0) đều tầm thường.

Cho K là một trường.. Các mở rộng p-căn có chiều cao 0 của K là các mở rộng tầm thường. Mọi mở rộng p-căn của K đều đại số. Nếu E là một mở rộng p-căn của K và F là một mở rộng p-căn của E, thì F là một mở rộng p-căn của K: thật vậy, với mọi $ x \in F $, tồn tại một số nguyên $ m \geq 0 $ sao cho $ x^{p^m} \in E $ và một số nguyên $ n \geq 0 $ sao cho $ (x^{p^m})^{p^n} \in K $, tức là $ x^{p^m + n} \in K $.

#### Mệnh đề 2 {#alg-v-s5-prop-2 .statement}

Cho E là một mở rộng của trường K. Với mỗi số nguyên $ n \geq 0 $, gọi $ E_n $ là tập hợp các phần tử của E là $ p\text{-căn} $ có chiều cao $ \leq n $ trên K, và gọi $ E_r $ là tập hợp tất cả các phần tử của E là p-căn trên K. Khi đó $ (E_n)_{n \geq 0} $ là một dãy tăng các mở rộng con của E mà hợp của chúng là $ E_\infty $, và $ E_r $ là mở rộng p-căn lớn nhất của K được chứa trong E.

Với mỗi số nguyên $ n \geq 0 $, tập hợp $ E_n $ gồm tất cả các phần tử $ x $ của E sao cho $ x^{p^n} \in K $; vì ánh xạ $ x \mapsto x^{p^n} $ là một tự đồng cấu của trường E, ta suy ra rằng $ E_n $ là một mở rộng con của E. Dãy $ (E_n)_{n \geq 0} $ tăng, có hợp là $ E_r $ và do đó $ E_r $ là một mở rộng con của E (V, p. 11, Mệnh đề 3). Rõ ràng $ E_r $ là một mở rộng p-căn của K và $ E_r $ chứa mọi mở rộng con của E là p-căn trên K.

#### Hệ quả {#alg-v-s5-n2-cor-1 .statement}

Nếu một mở rộng E của trường K được sinh bởi một tập hợp các phần tử $ p\text{-căn} $ trên K, thì nó là p-căn trên K.

Vì $ E_r $ là một mở rộng con của E và theo giả thiết $ E = K(E_\infty) $ do đó $ E = E_r $; vậy E là một mở rộng p-căn của K.

Dưới các điều kiện của Mệnh đề 2, $ E_r $ được gọi là bao đóng $ p\text{-căn} $ tương đối của K trong E.

Ta sẽ áp dụng Mệnh đề 2 đặc biệt cho trường hợp E là một mở rộng đóng đại số của K; khi đó E là hoàn hảo và ta có $ E_n = K^{p^{-n}} $ với mọi $ n \geq 0 $. Trong trường hợp này, ta ký hiệu $ K^{p^{-\infty}} $ là tập hợp các phần tử của E là p-căn trên K; đó là trường con của E là hợp của dãy tăng $ (K^{p^{-n}})_{n > 0} $ các trường con của E. Theo Mệnh đề 2, $ K^{p^{-\infty}} $ là mở rộng con lớn nhất của E là p-căn trên K; theo Mệnh đề 3 của V, p. 6, $ K^{p^{-\infty}} $ là một bao đóng hoàn hảo của K và nó cũng là trường con hoàn hảo nhỏ nhất của E chứa K. Khi K hoàn hảo, rõ ràng ta có $ K = K^{p^{-n}} = K^{p^{-\infty}} $ với mọi n. Nếu K không hoàn hảo, ta có $ K \neq K^P $, do đó

$ ^1 $ Một mở rộng p-căn còn được gọi là một mở rộng thuần túy không tách được, hoặc một mở rộng căn.

$$
K^{p^{-n}} \neq (K^p)^{p^{-n}} = K^{p^{-(n-1)}}
$$
với $ n \geq 1 $; khi đó các trường con $ K^{p^{-n}} $ của E từng đôi một phân biệt và $ K^{p^{-\infty}} $ là một mở rộng đại số có bậc vô hạn của K.

#### Mệnh đề 3 {#alg-v-s5-prop-3 .statement}

— Cho K là một trường, E là một trường mở rộng của K, p-căn trên K và $ u $ là một đồng cấu từ K vào một trường hoàn hảo F. Khi đó tồn tại một đồng cấu duy nhất $ v $ từ E vào F mở rộng u.

Gọi $ E_n $ là tập hợp các phần tử của E là p-căn có chiều cao $ \leq n $ trên K. Theo Mệnh đề 2, trường E là hợp của dãy tăng $ (E_n)_{n \geq 0} $ các trường con. Gọi $ v $ là một đồng cấu từ E vào F mở rộng u; với mọi $ x \in E_n $ ta có $ x^{p^n} \in K $, do đó $ v(x)^{p^n} = v(x^{p^n}) = u(x^{p^n}) $; do đó ta có $ v(x) = u(x^{p^n})^{p^{-n}} $ với mọi $ n \geq 0 $ và mọi $ x \in E_n $, do đó tính duy nhất của mở rộng của u lên E.

Cho $ n $ là một số nguyên dương; với mọi $ x \in E_n $ ta có $ x^{p^n} \in K $ và vì F hoàn hảo, ta có thể định nghĩa một phần tử $ v_n(x) $ của F bởi $ v_n(x) = u(x^{p^n})^{p^{-n}} $. Rõ ràng $ v_n $ là một đồng cấu từ $ E_n $ vào F, $ v_0 = u $ và $ v_{n+1} $ cảm sinh $ v_n $ trên $ E_n $. Do đó tồn tại một đồng cấu $ v $ từ E vào F cảm sinh $ v_n $ trên $ E_n $ với mọi $ n \geq 0 $ và, đặc biệt, trùng với $ v_0 = u $ trên $ E_0 = K $.

#### Hệ quả {#alg-v-s5-n2-cor-2 .statement}

— Để một mở rộng E của một trường K là một bao đóng hoàn hảo của K thì điều kiện cần và đủ là E phải là một mở rộng p-căn của K và trường E phải hoàn hảo.

Hệ quả là tầm thường khi $ p = 1 $; giả sử khi đó $ p \neq 1 $. Các điều kiện đã nêu là cần thiết theo V, p. 5, Định lý 3; chúng là đủ theo Mệnh đề 3.

#### Mệnh đề 4 {#alg-v-s5-prop-4 .statement}

— Cho E là một mở rộng p-căn *có bậc hữu hạn* của một trường K. Khi đó $[E : K]$ là một lũy thừa của số mũ đặc số p của K.

Vì E là một mở rộng p-căn có bậc hữu hạn của K, tồn tại các phần tử $ a,, \ldots, a, $ của E, p-căn trên K, sao cho $ E = K(a,, \ldots, a,) $. Cho i nhận các giá trị từ 1 đến m; vì $ a_i $ a fortiori là p-căn trên $ K(a,, \ldots, a_{i-1}) $, bậc
$$
n_i = [K(a_1, \ldots, a_i) : K(a_1, \ldots, a_{i-1})]
$$
là một lũy thừa của p (V, p. 24, Mệnh đề 1). Ta có $[E : K] = n_1 \ldots n_m$ theo V, p. 18, Định lý 2, do đó có kết quả.

### Bài tập {#alg-v-s5-exercises}

Xem [các bài tập của § 5](exercises/s5/).
