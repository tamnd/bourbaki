---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: II
chapter_title: FREE LIE ALGEBRAS
section: 0
section_title: Möbius function
appendix: true
lang: vi
source: lie-i-iii
pdf_pages: 0194-0195, 0225-0225
extraction: ocr
statements: 1
exercises: 2
content_sha256: e9591387a446c5339a56838ea8622db48ac9f757b7d6e89d06584b8b05f0b043
translated_from: content/en/lie/II/A_a_mobius_function.md
source_content_sha256: d802f3bf7d9f7f09e088205f36806c5e4782b38de7866dc8943e4c4407e3ee59
translation_model: gpt-5.4
translation_run: translate-vi-de0b6f62
glossary_version: 34
glossary_terms_sha256: ec637e199dda4ad0d9c147ea0bfa7241912f24615d90bb3a1fba5542d6759542
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## PHỤ LỤC

# HÀM MÖBIUS

Cho n là một số nguyên $ \geq 1 $. Nếu n chia hết cho bình phương của một số nguyên tố, ta viết $ \mu(n) = 0 $. Nếu n không chia hết cho bình phương của một số nguyên tố, ta viết $ \mu(n) = (-1)^k $, trong đó k là số các ước nguyên tố của n. Hàm $ \mu : \mathbf{N}^* \to \{-1, 0, 1\} $ được xác định như vậy được gọi là hàm Möbius.

Nhắc lại rằng với hai số nguyên $ n_1 \geq 1, n_2 \geq 1 $, ta viết $ n_1 | n_2 $ nếu $ n_1 $ chia $ n_2 $.

#### Mệnh đề {#lie-ii-a0-n0-prop-1 .statement}

(i) *Hàm $ \mu $ là ánh xạ duy nhất từ $ \mathbf{N}^* $ vào $ \mathbf{Z} $ sao cho $ \mu(1) = 1 $ và*
$$
\sum_{d|n} \mu(d) = 0
$$
*đối với mọi số nguyên $ n > 1 $.*

(ii) *Cho s và t là hai ánh xạ từ $ \mathbf{N}^* $ vào một nhóm giao hoán viết theo lối cộng. Để có*
$$
s(n) = \sum_{d|n} t(d) \quad \text{với mọi số nguyên } n \geq 1,
$$
*thì điều kiện cần và đủ là*
$$
t(n) = \sum_{d|n} \mu(d) s\left(\frac{n}{d}\right) \quad \text{với mọi số nguyên } n \geq 1.
$$

Mệnh đề về tính duy nhất trong (i) là hiển nhiên, vì (1) cho phép ta xác định $ \mu(n) $ bằng quy nạp theo n. Ta chỉ ra rằng hàm $ \mu $ thỏa mãn (1). Cho n là một số nguyên $ > 1 $. Gọi P là tập hợp các ước nguyên tố của n và đặt $ n = \prod_{p \in P} p^{\nu_p(n)} $ là phân tích của n thành các thừa số nguyên tố. Nếu d là một ước của n, thì $ \mu(d) = 0 $ trừ khi d có dạng $ \prod_{p \in H} p $, trong đó H là một tập con của P. Khi đó
$$
\sum_{d|n} \mu(d) = \sum_{H \subset P} (-1)^{\mathrm{Card}\ H}
= \sum_{k=0}^{\mathrm{Card}\ P} \binom{n}{k} (-1)^k = (1 - 1)^{\mathrm{Card}\ P} = 0.
$$

Cho s và t là hai ánh xạ từ $ \mathbf{N}^* $ vào một nhóm giao hoán viết theo lối cộng. Cho $ n \in \mathbf{N}^* $. Nếu (2) đúng, thì
$$
\sum_{d|n} \mu(d)s\left(\frac{n}{d}\right) = \sum_{d|n} \mu(d) \sum_{\delta|(n/d)} t(\delta) = \sum_{d|n} \mu(d)t(\delta)
$$
$$
= \sum_{\delta|n} t(\delta) \sum_{d|(n/\delta)} \mu(d) = t(n).
$$
Ngược lại, nếu (3) đúng, thì
$$
\sum_{d|n} t(d) = \sum_{d|n} \sum_{\delta|d} \mu(\delta)s\left(\frac{d}{\delta}\right) = \sum_{d|n} s(d) \sum_{\delta|(n/d)} \mu(\delta) = s(n),
$$
điều đó kết thúc chứng minh.

Công thức (3) được gọi là công thức đảo Möbius.

### Bài tập {#lie-ii-a0-exercises}

Xem [bài tập của Phụ lục 0](exercises/a0/).
