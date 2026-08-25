---
book: alg
book_title: Algebra
chapter: III
chapter_title: TENSOR ALGEBRAS, EXTERIOR ALGEBRAS, SYMMETRIC ALGEBRAS
section: 0
section_title: TENSOR ALGEBRAS, EXTERIOR ALGEBRAS, SYMMETRIC ALGEBRAS
kind: front
lang: vi
source: alg-i-iii
source_edition: 1998, Springer
pdf_pages: 0451-0451
extraction: ocr
statements: 0
exercises: 0
content_sha256: b65e4591269c836a04babe0718dcc1a21b5faa55be8ecf5e0103ceff5966becc
translated_from: content/en/alg/III/00_frontmatter.md
source_content_sha256: 6265d61279faab9dcf08066eb99e498297b3d05106b7e1efab665fe26a7b784b
translation_model: gpt-5-6-mini
translation_run: translate-vi-67965beb
glossary_version: 34
glossary_terms_sha256: b3e838741fd10fbba3c7ca2a24655a282163de96e96d383094e0a94a28f4d886
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## CHƯƠNG III

# Đại số tenxơ, Đại số ngoài, Đại số đối xứng

Nhắc lại ký hiệu mũ đưa vào trong Chương I, mà ta sẽ sử dụng thường xuyên (I, § 7, no. 8):

Cho $(x_\lambda)_{\lambda \in L}$ là một họ các phần tử từng đôi một hoán vị được của một vành $A$; với mọi ánh xạ $\alpha : L \to N$ có giá hữu hạn, ta sẽ viết

$$
x^\alpha = \prod_{\lambda \in L} x_\lambda^{\alpha(\lambda)}.
$$

Nếu $\beta$ là một ánh xạ khác của $L$ vào $N$ có giá hữu hạn, $\alpha + \beta$ ký hiệu ánh xạ

$$
\lambda \mapsto \alpha(\lambda) + \beta(\lambda)
$$

của $L$ vào $N$; với luật hợp thành này, tập hợp $N^{(L)}$ các ánh xạ của $L$ vào $N$ có giá hữu hạn là mônoit giao hoán tự do dẫn xuất từ $L$ và

$$
x^\alpha x^\beta = x^{\alpha + \beta}.
$$

Với mọi $\alpha \in N^{(L)}$, ta viết $|\alpha| = \sum_{\lambda \in L} \alpha(\lambda) \in N$; khi đó $|\alpha + \beta| = |\alpha| + |\beta|$; $|\alpha|$ được gọi là cấp của "đa chỉ số" $\alpha$. Với mọi $\lambda \in L$, gọi $\delta_\lambda$ là phần tử của $N^{(L)}$ sao cho $\delta_\lambda(\lambda) = 1$, $\delta_\lambda(\mu) = 0$ với $\mu \neq \lambda$ (chỉ số Kronecker); các $\delta_\lambda$ với $\lambda \in L$ là những phần tử duy nhất của $N^{(L)}$ có cấp 1. $N^{(L)}$ được trang bị quan hệ thứ tự cảm sinh bởi quan hệ thứ tự tích trên $N^L$, sao cho quan hệ $\alpha \leq \beta$ tương đương với "$\alpha(\lambda) \leq \beta(\lambda)$ với mọi $\lambda \in L$"; khi đó đa chỉ số $\lambda \mapsto \beta(\lambda) - \alpha(\lambda)$ được ký hiệu bởi $\beta - \alpha$, sao cho nó là đa chỉ số duy nhất thỏa mãn $\alpha + (\beta - \alpha) = \beta$. Với mọi $\alpha \in N^{(L)}$, chỉ có một số hữu hạn đa chỉ số $\beta \leq \alpha$; các $\delta_\lambda$ là các phần tử cực tiểu của tập hợp $N^{(L)} - \{0\}$; quan hệ $\alpha \leq \beta$ kéo theo $|\alpha| \leq |\beta|$ và nếu đồng thời $\alpha \leq \beta$ và $|\alpha| = |\beta|$, thì $\alpha = \beta$.

Cuối cùng, ta viết $\alpha! = \prod_{\lambda \in L} (\alpha(\lambda))!$, điều này có nghĩa vì $0! = 1$.

Từ § 4 đến § 8 kể cả, $A$ ký hiệu một vành giao hoán và, trừ khi có chỉ dẫn khác, các đại số được xét được giả thiết là kết hợp và có đơn vị và các đồng cấu đại số được giả thiết là có đơn vị.
