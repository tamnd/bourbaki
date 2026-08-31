---
book: hist
book_title: Elements of the History of Mathematics
chapter: "1"
chapter_title: ELEMENTS OF THE HISTORY OF MATHEMATICS
section: 19
section_title: The Gamma Function
lang: vi
source: hist
pdf_pages: 0205-0205
extraction: ocr
statements: 0
exercises: 0
content_sha256: 911e048672e7d3094668ccc3f1127a614ee8eafb57cb5d4f77a8d84e51c8007f
translated_from: content/en/hist/1/19_s19_the_gamma_function.md
source_content_sha256: 7092fa519a4f115973a096a09aabbecb5a46cdac0f410b2a08e230e4c0142ff8
translation_model: gpt-5.4
translation_run: translate-vi-9891b17b
glossary_version: 34
glossary_terms_sha256: 002e2f329b1f2b02743908adfd19a771b4902f465cea3a14fa3e2f641575d3b3
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 19. HÀM GAMMA.

Ý tưởng "nội suy" một dãy $(u_n)$ bằng các giá trị của một tích phân phụ thuộc vào một tham số thực $\lambda$ và bằng $u_n$ khi $\lambda = n$, bắt nguồn từ Wallis (xem tr. 187 tt.). Chính ý tưởng này đã là phương hướng chủ yếu dẫn dắt Euler khi, vào năm 1730 ([108 a], (1), v. XIV, tr. 1-24), ông nảy ra ý tưởng nội suy dãy các giai thừa. Ông bắt đầu bằng cách nhận thấy rằng $n!$ bằng tích vô hạn $\prod_{k=1}^{\infty} \left( \frac{k+1}{k} \right)^n \frac{k}{k+n}$, rằng tích này được xác định với mọi giá trị của $n$ (nguyên hay không), và đặc biệt, với $n = \frac{1}{2}$ nó nhận giá trị $\frac{1}{2} \sqrt{\pi}$ theo công thức của Wallis. Sự tương tự của kết quả này với các kết quả của Wallis dẫn ông đến chỗ xét lại tích phân $\int_0^1 x^e (1-x)^n dx$ ($n$ là một số nguyên, $e$ tùy ý), vốn đã được chính Wallis khảo sát. Euler thu được giá trị của nó là $\frac{n!}{(e+1)(e+2)\cdots(e+n)}$ bằng khai triển nhị thức; khi đó một phép đổi biến cho ông thấy rằng $n!$ là giới hạn, khi $z$ tiến tới 0, của tích phân $\int_0^1 \left( \frac{1-x^z}{z} \right)^n dx$, do đó có "tích phân Euler thứ hai" $n! = \int_0^1 (\log \frac{1}{x})^n dx$; bằng cùng phương pháp ấy và việc dùng công thức của Wallis, ông thu được công thức $\int_0^1 \sqrt{\log \frac{1}{x}} dx = \frac{1}{2} \sqrt{\pi}$. Trong các công trình về sau, Euler thường xuyên quay lại các tích phân này; theo cách đó, ông khám phá ra quan hệ về các phần bù ([108 a], (1), v. XV, p. 82 và v. XVII, p. 342), công thức $B(p, q) = \Gamma(p) \Gamma(q) / \Gamma(p + q)$ ([108 a], (1), v. XVII, p. 355), và trường hợp riêng của công thức Legendre-Gauss ứng với $x = 1$ ([108 a], (1), v. XIX, p. 483); tất nhiên, trong tất cả những điều ấy ông không bận tâm đến các vấn đề hội tụ.

Gauss tiếp tục nghiên cứu hàm $\Gamma$ liên hệ với các nghiên cứu của ông về hàm siêu bội, mà hàm $\Gamma$ là một trường hợp giới hạn ([124 a], v. III, tr. 125-162); chính trong nghiên cứu này mà ông thu được công thức tổng quát về phép nhân (mà Legendre đã lưu ý trước đó không lâu trong trường hợp $p = 2$). Các công trình tiếp theo về $\Gamma$ chủ yếu nhằm mở rộng hàm này sang miền phức. Chỉ gần đây người ta mới nhận thấy rằng tính chất lồi lôgarit đặc trưng cho $\Gamma(x)$ (trong miền thực) tới một nhân tử giữa mọi nghiệm của phương trình phiếm hàm $f(x+1) = x f(x)$ ([26], tr. 149-164); và Artin đã chỉ ra [7 d] rằng mọi kết quả cổ điển về $\Gamma(x)$ đều có thể được liên kết một cách đơn giản với tính chất ấy.
