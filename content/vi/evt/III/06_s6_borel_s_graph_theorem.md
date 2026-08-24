---
book: evt
book_title: Topological Vector Spaces
chapter: III
chapter_title: SPACES OF CONTINUOUS LINEAR MAPPINGS
section: 6
section_title: Borel's graph theorem
lang: vi
source: evt-i-v
book_pages: TVS III.49-TVS III.50
pdf_pages: 0166-0169, 0181-0182
extraction: ocr
subsections:
    - "no": 1
      title: Borel’s graph theorem
      page: 34
      pdf_page: 166
    - "no": 2
      title: Locally convex Lusin spaces
      page: 34
      pdf_page: 166
    - "no": 3
      title: Measurable linear mappings on a Banach space $ ^1 $
      page: 36
      pdf_page: 168
statements: 8
exercises: 6
content_sha256: 38601c45c800a992891383f71d1cd8f4157c1a79ef12eb1c83841f6c50ec5014
translated_from: content/en/evt/III/06_s6_borel_s_graph_theorem.md
source_content_sha256: e17f21307f796721ccc0bb4982493d69710026c31234fab45b7a949a6c553437
translation_model: gpt-5.4
translation_run: translate-vi-37efe174
glossary_version: 34
glossary_terms_sha256: 82429cf98be4f83a844dbba3e47122ea163fa98b065056303187fde2e06bc49b
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 6. ĐỊNH LÝ ĐỒ THỊ CỦA BOREL

### 1. Định lý đồ thị của Borel

#### Định lý 1 {#evt-iii-s6-thm-1 .statement}

— Cho E là một không gian lồi địa phương là giới hạn quy nạp của các không gian Banach, F là một không gian lồi địa phương Souslin, chẳng hạn một không gian Lusin (GT, IX, § 6, No. 2 and No. 4), và u là một ánh xạ tuyến tính từ E vào F. Nếu đồ thị của u là một tập con Borel của E × F, thì u liên tục.

Cho E_i là một họ các không gian Banach, và (u_i) là một họ các ánh xạ tuyến tính liên tục u_i : E_i → E sao cho tôpô của E là tôpô lồi địa phương mịn nhất mà đối với nó các u_i là liên tục. Chỉ cần chứng minh rằng các ánh xạ hợp thành u ∘ u_i là liên tục, hoặc thực ra (GT, IX, § 2, No. 6, mđ. 10) rằng hạn chế của u ∘ u_i lên mọi không gian con đóng G của E_i thỏa mãn tiên đề đếm được thứ nhất là liên tục. Đồ thị của hạn chế này là ảnh ngược của đồ thị của u qua ánh xạ liên tục u_i × Id_F : G × F → E × F, do đó là một tập Borel trong G × F. Ngoài ra, G × F là một không gian Souslin và mọi tập con Borel của một không gian Souslin đều là một không gian Souslin (GT, IX, § 6, No. 3, mđ. 10). Định lý 1 khi đó suy ra từ đl. 4, GT, IX, § 6, No. 8.

#### Nhận xét {#evt-iii-s6-n1-rem-1 .statement}

— Nhắc lại (III, p. 12) rằng mọi không gian Hausdorff đồng điều và bán đầy đủ, chẳng hạn mọi không gian Fréchet, đều là giới hạn quy nạp của các không gian Banach. \* Điều này cũng đúng đối với đối ngẫu mạnh của một không gian Fréchet phản xạ (IV, p. 23, mđ. 4). \*

### 2. Các không gian Lusin lồi địa phương

#### Mệnh đề 1 {#evt-iii-s6-prop-1 .statement}

— Cho E là một không gian lồi địa phương Hausdorff. Giả sử rằng tồn tại một dãy (E_n)_{n \in \mathbf{N}} các không gian Fréchet thỏa mãn tiên đề đếm được thứ nhất, và các ánh xạ tuyến tính liên tục u_n : E_n → E sao cho E = \bigcup_{n \in \mathbf{N}} u_n(E_n). Khi đó E là một không gian Lusin.

Cho P_n là hạt nhân của u_n; khi đó u_n xác định một ánh xạ liên tục song ánh từ không gian thương E_n/P_n lên u_n(E_n). Vì E_n/P_n là một không gian Fréchet thỏa mãn tiên đề đếm được thứ nhất (GT, IX, § 3, No. 1), do đó là một không gian polish (GT, IX, § 6, No. 1, đn. 1), nên u_n(E_n) là một không gian con Lusin của E (GT, IX, § 6, No. 4, mđ. 11). Bởi vậy theo GT, IX, § 6, No. 7, hq. của đl. 3, không gian E, là chính quy (GT, III, § 3, No. 1), là một không gian Lusin.

#### Ví dụ 1 {#evt-iii-s6-n2-exa-1 .statement}

— Mọi không gian Fréchet thỏa mãn tiên đề đếm được thứ nhất đều là một không gian polish, do đó là một không gian Lusin. Do đó, các không gian $ \mathcal{C}(X) $ cũng vậy, trong đó X là địa phương compact và có một cơ sở đếm được (tôpô của $ \mathcal{C}(X) $ là tôpô hội tụ compact, xem GT, X, § 3, No. 3, hệ quả and § 1, No. 6, hq. 3); \* các không gian $ \mathcal{C}_0^\infty(U) $, trong đó U là một tập con mở của $ \mathbf{R}^n $ (III, p. 9) và $ \mathcal{H}(U) $, trong đó U là một tập con mở của $ \mathbf{C}^n $ (III, p. 10).

Mệnh đề 1 cho thấy rằng các không gian $ \mathcal{C}_0^\infty(U) $, trong đó U là một tập mở trong $ \mathbf{R}^n $, $ \mathcal{G}_s(I) $, trong đó I là một khoảng compact trong $ \mathbf{R} $ và $ s \geq 1 $, và $ \mathcal{H}(K) $, trong đó K là một tập con compact của $ \mathbf{C}^n $ đều là các không gian Lusin (III, p. 10). \*

#### Định lý 2 {#evt-iii-s6-thm-2 .statement}

— Cho E là một không gian lồi địa phương, là giới hạn quy nạp của một dãy tăng $ (E_n)_{n \in \mathbf{N}} $ các không gian con của E, được trang bị các tôpô của các không gian Fréchet thỏa mãn tiên đề đếm được thứ nhất. Giả sử rằng mọi tập con compact của E đều được chứa trong một trong các $ E_n $ và là compact trong không gian này. Cho F là một không gian Fréchet thỏa mãn tiên đề đếm được thứ nhất. Khi đó không gian $ \mathcal{L}_c(E; F) $ là một không gian Lusin.

Không gian E là bornological (III, p. 12), do đó không gian $ \mathcal{L}_c(E; F) $ là đầy đủ (III, p. 23, prop. 12). Ánh xạ tuyến tính $ j : f \mapsto (f|E_n)_{n \in \mathbf{N}} $ là một đơn ánh từ $ \mathcal{L}_c(E; F) $ vào không gian tích $ \prod_{n \in \mathbf{N}} \mathcal{L}_c(E_n; F) $; do giả thiết về các tập con compact của E và định nghĩa của các tôpô $ \mathfrak{S} $, $ j $ là một đẳng cấu từ $ \mathcal{L}_c(E; F) $ lên ảnh của nó (được trang bị tôpô cảm sinh bởi tôpô tích); hơn nữa, vì $ \mathcal{L}_c(E; F) $ là đầy đủ, ảnh này là một không gian con đóng của $ \prod_{n \in \mathbf{N}} \mathcal{L}_c(E_n; F) $ (GT, II, § 3, No. 4, prop. 8). Theo GT, IX, § 6, No. 4, do đó chỉ cần chứng minh rằng mỗi không gian $ \mathcal{L}_c(E; F) $ là một không gian Lusin. Trong phần còn lại của chứng minh, ta sẽ giả sử rằng E là một không gian Fréchet thỏa mãn tiên đề đếm được thứ nhất.

Vì F là một không gian Fréchet thỏa mãn tiên đề đếm được thứ nhất, nên nó đẳng cấu với một không gian con đóng của một tích đếm được các không gian Banach $ F_n $, mỗi không gian là một thương của F (II, p. 5), do đó thỏa mãn tiên đề đếm được thứ nhất. Ánh xạ tuyến tính $ j' : f \mapsto (\mathrm{pr}_n \circ f)_{n \in \mathbf{N}} $ là một đơn ánh từ $ \mathcal{L}_c(E; F) $ vào không gian tích $ \prod_{n \in \mathbf{N}} \mathcal{L}_c(E; F_n) $, và bằng cách dùng định nghĩa của các tôpô $ \mathfrak{S} $ và của các tập mở trong một tích, $ j' $ là một đẳng cấu từ $ \mathcal{L}_c(E; F) $ lên ảnh của nó; hơn nữa, vì $ \mathcal{L}_c(E; F) $ là đầy đủ, nên ảnh này là một không gian con đóng của $ \prod_{n \in \mathbf{N}} \mathcal{L}_c(E; F) $. Vậy chỉ cần chứng minh rằng mỗi không gian $ \mathcal{L}_c(E; F_n) $ là một không gian Lusin (GT, IX, § 6, No. 4), và do đó, ta có thể giả sử rằng F là một không gian Banach thỏa mãn tiên đề đếm được thứ nhất.

Không gian $ \mathcal{L}_c(E; F) $ là hợp của một họ đếm được các tập con đồng liên tục và đóng (III, p. 19, hệ quả 1 and GT, X, § 2, No. 3, mệnh đề 6). Nhưng mọi tập con đồng liên tục H của $ \mathcal{L}_c(E; F) $ đều khả mêtric hóa và thỏa mãn tiên đề đếm được thứ nhất (III, p. 18, mệnh đề 6 and GT, X, § 2, No. 4, định lý 1); nếu H đóng, thì nó là một không gian đầy đủ đối với cấu trúc đều cảm sinh bởi cấu trúc đều của $ \mathcal{L}_c(E; F) $, vì cấu trúc sau là đầy đủ. Nói cách khác, H là một không gian Ba Lan, và *a fortiori* là một không gian Lusin; do đó không gian chính quy $ \mathcal{L}_c(E; F) $ là một không gian Lusin (GT, IX, § 6, No. 7, hệ quả of định lý 3).

#### Hệ quả {#evt-iii-s6-n2-cor-1 .statement}

— *Với các giả thiết trên E như trong định lý 2, giả sử thêm rằng mọi tập con bị chặn của E đều compact tương đối. Khi đó đối ngẫu mạnh của E là một không gian Lusin.* *Đặc biệt, đối ngẫu mạnh của một không gian Fréchet thỏa mãn tiên đề đếm được thứ nhất, đồng thời cũng là một không gian Montel, là một không gian Lusin.*

\* Ví dụ 2. — Cho U là một tập con mở của $ \mathbf{R}^n $. Hệ quả áp dụng đặc biệt cho không gian Fréchet $ E = \mathcal{C}_c^\infty(U) $; đối ngẫu của nó $ \mathcal{C}_c^{-\infty}(U) $ (không gian các phân phối có giá compact trên U) khi đó là một không gian Lusin.

Không gian $ \mathcal{C}_c^\infty(U) $ là một giới hạn quy nạp ngặt của một dãy các không gian Fréchet $ \mathcal{C}_{K_n}^\infty(U) $ thỏa mãn tiên đề thứ nhất về tính đếm được (III, p. 9). Ta có thể chứng minh rằng mỗi không gian $ \mathcal{C}_{K_n}^\infty(U) $ là một không gian Montel; thêm nữa, mọi tập con bị chặn của $ \mathcal{C}_c^\infty(U) $ đều được chứa trong một trong các không gian $ \mathcal{C}_{K_n}^\infty(U) $ (III, p. 5, prop. 6). Khi đó ta có thể áp dụng hệ quả của đl. 2. Vậy đối ngẫu $ \mathcal{C}_c^{-\infty}(U) $ của $ \mathcal{C}_c^\infty(U) $ (không gian các phân phối trên U) là một không gian Lusin đối với tôpô mạnh.

Tương tự, ta chứng minh rằng với mọi tập con mở U của $ \mathbf{C}^n $, và với mọi tập con compact K của $ \mathbf{C}^n $, đối ngẫu mạnh của $ \mathcal{H}(U) $ và đối ngẫu mạnh của $ \mathcal{H}(K) $ là các không gian Lusin. \*

#### Nhận xét {#evt-iii-s6-n2-rem-1 .statement}

— Cho E như trong định lý 2; cho F là một không gian lồi địa phương Hausdorff là hợp của các ảnh của một dãy các ánh xạ tuyến tính liên tục $ u_n : F_n \to F $, trong đó mỗi $ F_n $ là một không gian Fréchet thỏa mãn tiên đề đếm được thứ nhất; khi đó $ \mathcal{L}_c(E ; F) $ là một không gian Lusin. Như trong mệnh đề 1, trước hết ta rút gọn về trường hợp mỗi $ u_n $ là đơn ánh; rồi, như trong chứng minh của định lý 2, ta có thể giả sử rằng E là một không gian Fréchet thỏa mãn tiên đề đếm được thứ nhất. Khi đó, theo I, p. 20, mệnh đề 1, $ \mathcal{L}(E ; F) $ là hợp của các $ \mathcal{L}(E ; F_n) $; hơn nữa, đơn ánh chính tắc $ \mathcal{L}_c(E ; F_n) \to \mathcal{L}_c(E ; F) $ là liên tục (GT, X, § 1, No. 4, mệnh đề 3). Vì mỗi không gian $ \mathcal{L}_c(E ; F_n) $ là một không gian Lusin theo định lý 2, nên $ \mathcal{L}(E ; F_n) $ cũng là một không gian Lusin đối với tôpô cảm sinh bởi tôpô của $ \mathcal{L}_c(E ; F) $ (GT, IX, § 6, No. 4, mệnh đề 11); do đó $ \mathcal{L}_c(E ; F) $ là một không gian Lusin theo GT, IX, § 6, No. 7, hệ quả của định lý 3.

### \*3. Các ánh xạ tuyến tính đo được trên một không gian Banach $ ^1 $

#### Mệnh đề 2 {#evt-iii-s6-prop-2 .statement}

— *Cho E là một không gian Banach, F là một không gian lồi địa phương và u là một ánh xạ tuyến tính từ E vào F. Giả sử rằng với mọi tập con đóng B của F, mọi tập con compact X của E và mọi độ đo $ \mu $ trên X, giao $ X \cap u^{-1}(B) $ là $ \mu $-đo được. Khi đó u là liên tục.*

Trước hết giả sử rằng F là trường cơ sở. Với mọi tập con compắc X của E và mọi độ đo $ \mu $ trên X, hạn chế của $ u $ trên X là $ \mu $-đo được (INT, IV). Giả sử rằng $ u $ không liên tục. Khi đó ta có thể tìm được một dãy điểm $ (x_n) $ trong E sao cho $ \sum_n \| x_n \| < \infty $ và $ |u(x_n)| \geq n $ với mọi số nguyên $ n $. Xét ánh xạ $ g : (t_n) \mapsto \sum_n t_n x_n $ từ lập phương $ C = [0, 1]^{\mathbf{N}} $ vào E; hiển nhiên $ g $ liên tục. Do đó $ f = u \circ g $ là đo được đối với mọi độ đo trên C (INT, V); đặc biệt đối với độ đo $ \mu $ là tích của các độ đo Lebesgue trên các thừa số của C. Vì vậy tồn tại một tập con compắc D của C sao cho $ \mu(D) > \frac{1}{2} $ và sao cho hạn chế của $ f $ trên D là liên tục, do đó cũng bị chặn. Gọi M là cận trên của $ |f| $ trên D và gọi $ p \in \mathbf{N} $ sao cho $ p \geq 4M $. Cho $ s = (s_n) $ và $ t = (t_n) $ là hai điểm của D sao cho $ s_n = t_n $ với mọi $ n \neq p $. Khi đó

$$
f(s) - f(t) = u(\sum_n s_n x_n - \sum_n t_n x_n) = (s_p - t_p) u(x_p) .
$$

Vì $ |f(s) - f(t)| \leq 2M $ và $ |u(x_p)| \geq p \leq 4M $, ta được

$$
|s_p - t_p| \leq \frac{1}{2} .
$$

Định lý Lebesgue-Fubini (INT, V, 2nd ed., § 8, No. 3, hệ quả 2 của mệnh đề 7) kéo theo $ \mu(D) \leq \frac{1}{2} $; điều này dẫn đến mâu thuẫn. Vậy $ u $ là liên tục.

Trong trường hợp tổng quát, với mọi $ v \in F' $, dạng tuyến tính $ v \circ u $ là liên tục, theo lập luận trước đó. Cho $ (x_n)_{n \in \mathbf{N}} $ là một dãy điểm của E tiến tới 0; khi đó dãy $ (u(x_n))_{n \in \mathbf{N}} $ tiến tới 0 trong F, nếu F được trang bị tôpô $ \sigma(F, F') $; do đó dãy này bị chặn đối với $ \sigma(F, F') $ và vì thế nó bị chặn trong F (III, p. 27, hệ quả 3). Vì E là bornological (III, p. 12, mệnh đề 2); ánh xạ tuyến tính $ u : E \to F $ là liên tục. \*

$ ^1 $ Các kết quả của tiết này phụ thuộc vào cuốn Tích phân.

Bài tập

### Bài tập {#evt-iii-s6-exercises}

Xem [các bài tập của § 6](exercises/s6/).
