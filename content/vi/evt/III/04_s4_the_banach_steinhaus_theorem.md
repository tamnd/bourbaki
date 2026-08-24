---
book: evt
book_title: Topological Vector Spaces
chapter: III
chapter_title: SPACES OF CONTINUOUS LINEAR MAPPINGS
section: 4
section_title: The Banach-Steinhaus theorem
lang: vi
source: evt-i-v
book_pages: TVS III.23-TVS III.28, TVS III.43-TVS III.46
pdf_pages: 0155-0160, 0175-0178
extraction: ocr
subsections:
    - "no": 1
      title: Barrels and barrelled spaces
      page: 24
      pdf_page: 156
    - "no": 2
      title: The Banach-Steinhaus theorem
      page: 25
      pdf_page: 157
    - "no": 3
      title: Bounded subsets of $ \mathcal{L}(E; F) $ (quasi-complete case)
      page: 27
      pdf_page: 159
statements: 18
exercises: 21
content_sha256: 4d55acb658f52079addc051a3b555cd43d764e8610348f6f66a817bd0471e4c8
translated_from: content/en/evt/III/04_s4_the_banach_steinhaus_theorem.md
source_content_sha256: a2edee71db4e593e68f89a39e51758bcfe1e509cba48f52ecbb2195db6722cea
translation_model: gpt-5.4
translation_run: translate-vi-7c7bdc75
glossary_version: 34
glossary_terms_sha256: 11c1a5f481edd3409e288af902ee1d8be20c90147f86e5c3780748b49f54ebfb
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 4. ĐỊNH LÝ BANACH-STEINHAUS

*Trong đoạn này, E chỉ một không gian lồi địa phương và E' là đối ngẫu của nó. Mỗi khi nói đến tôpô yếu trên E', ta sẽ hiểu là $ \sigma(E', E) $.*

### 1. Các thùng và các không gian thùng

Mệnh đề 1. — Cho T là một tập con của E. Các điều kiện sau là tương đương:

(i) T là lồi, cân bằng, đóng và thấm hút.

(ii) T là cực của một tập M lồi, cân bằng và bị chặn yếu trong E'.

(iii) Tồn tại một nửa chuẩn nửa liên tục dưới p trên E sao cho T là tập hợp mọi x ∈ E thỏa mãn p(x) ≤ 1.

(i) ⇒ (ii) : dưới giả thiết của (i), đặt M = T°; khi đó M là lồi và cân bằng trong E'. Với mọi x ∈ E, tồn tại một số thực r > 0 sao cho rx ∈ T, do đó |u(x)| ≤ $ \frac{1}{r} $ với mọi u ∈ M; nói cách khác, M bị chặn yếu. Theo hệ quả 3 của II, p. 45, ta có T = M°, vậy T thỏa mãn (ii).

(ii) ⇒ (iii) : dưới giả thiết của (ii), đặt $ p(x) = \sup_{u \in M} |u(x)| $ với mọi x ∈ E. Hiển nhiên T = M° gồm tất cả các x ∈ E sao cho p(x) ≤ 1. Nửa chuẩn p trên E' là nửa liên tục dưới, vì nó là bao trên của một họ các hàm liên tục (GT, IV, § 6, No. 2, hệ quả).

(iii) ⇒ (i) : điều này là rõ ràng.

Hệ quả. — Các điều kiện sau là tương đương:

(i) mọi tập con bị chặn yếu của E' đều là đẳng liên tục;

(ii) mọi tập lồi, cân bằng, đóng và thấm hút trong E đều là một lân cận của 0;

(iii) mọi nửa chuẩn nửa liên tục dưới trên E đều liên tục.

Định nghĩa 1. — Một tập T thỏa mãn các điều kiện tương đương của mệnh đề 1 được gọi là một thùng trong E.

Định nghĩa 2. — Một không gian E được gọi là không gian thùng nếu nó thỏa mãn các điều kiện tương đương của hệ quả của mệnh đề 1.

Ta biết (III, p. 22, mệnh đề 9) rằng mọi tập con đẳng liên tục của đối ngẫu E' của E đều bị chặn mạnh và bị chặn yếu. Do đó ta có thể phát biểu lại định nghĩa các không gian thùng như sau:

#### Chú giải {#evt-iii-s4-n1-sch-1 .statement}

— Trong đối ngẫu của một không gian thùng, lớp các tập đẳng liên tục, lớp các tập bị chặn mạnh, lớp các tập bị chặn yếu và lớp các tập tương đối compắc đối với tôpô yếu đều trùng nhau. Nếu E là Hausdorff và là không gian thùng, và nếu E'_b là đối ngẫu mạnh của nó, thì các cực của các lân cận của 0 trong một trong hai không gian tạo thành một cơ sở của bornology chính tắc của không gian kia, và các cực của các tập con bị chặn của một trong hai không gian tạo thành một cơ sở của bộ lọc các lân cận của 0 của không gian kia.

Mệnh đề 2. — Mọi không gian lồi địa phương E là một không gian Baire (GT, IX, § 5, No. 3) đều là không gian thùng.

Cho T là một thùng trong E; vì T là thấm hút, E là hợp của các tập đóng nT (n là số nguyên > 0); vì E là một không gian Baire, ít nhất một trong các tập ấy chứa một điểm trong, do đó chính T có một điểm trong x. Nếu $ x \neq 0 $, vì $-x \in T$, và 0 là một điểm của đoạn mở có hai đầu mút x và $-x$, nên 0 là một điểm trong của tập lồi T (II, p. 14, mệnh đề 16). Vậy T là một lân cận của 0.

#### Hệ quả {#evt-iii-s4-n1-cor-1 .statement}

— *Mọi không gian Fréchet (và đặc biệt, mọi không gian Banach) đều là không gian thùng.* Điều này suy ra từ định lý Baire (GT, IX, § 5, No. 3, định lý 1).

#### Mệnh đề 3 {#evt-iii-s4-prop-3 .statement}

— *Cho $(F_i)_{i \in I}$ là một họ các không gian thùng, và với mọi $i \in I$, cho $f_i$ là một ánh xạ tuyến tính từ $F_i$ vào một không gian vectơ E. Không gian E, được trang bị tôpô lồi địa phương mịn nhất sao cho các $f_i$ liên tục (II, p. 27, mệnh đề 5), là một không gian thùng.*

Cho T là một thùng trong E. Vì $f_i$ liên tục, $f_i^{-1}(T)$ là một tập lồi, cân bằng, đóng và hút được trong $F_i$; nói cách khác, một thùng trong $F_i$; vì $F_i$ là chùng, $f_i^{-1}(T)$ là một lân cận của 0 trong $F_i$, với mọi $i \in I$. Điều này suy ra rằng T là một lân cận của 0 trong E (II, p. 27, mệnh đề 5).

#### Hệ quả 1 {#evt-iii-s4-prop-3-cor-1 .statement}

— *Mọi không gian thương của một không gian chùng đều là chùng.*

#### Hệ quả 2 {#evt-iii-s4-prop-3-cor-2 .statement}

— *Cho $(E_i)_{i \in I}$ là một họ các không gian lồi địa phương và E là tổng trực tiếp tôpô của họ này. Để E là chùng, điều kiện cần và đủ là mỗi $E_i$ đều chùng.*

Điều kiện ấy hiển nhiên là đủ theo mệnh đề 3; nó cũng là cần, theo hệ quả 1, vì mỗi $E_i$ đẳng cấu với một không gian thương của E (II, p. 31, mệnh đề 8).

#### Hệ quả 3 {#evt-iii-s4-prop-3-cor-3 .statement}

— *Mọi giới hạn quy nạp của các không gian chùng là một không gian chùng.*

Sau này chúng tôi sẽ chứng minh (IV, p. 14, hệ quả) rằng mọi tích của các không gian chùng đều là chùng.

### 2. Định lý Banach-Steinhaus

#### Định lý 1 {#evt-iii-s4-thm-1 .statement}

— *Cho E là một không gian chùng, F một không gian lồi địa phương. Mọi tập con bị chặn đơn H của $\mathcal{L}(E; F)$ đều liên tục đều.*

Thật vậy, cho $p$ là một nửa chuẩn liên tục trên F; đặt $q = \sup_{u \in H} (p \circ u)$. Vì H bị chặn đơn giản, ta có $q(x) < +\infty$ với mọi $x \in E$ và $q$ là một nửa chuẩn nửa liên tục dưới, vì nó là bao trên hữu hạn của các nửa chuẩn liên tục. Vì E là vành thùng, $q$ là một nửa chuẩn liên tục và do đó H là đồng liên tục.

#### Hệ quả 1 {#evt-iii-s4-thm-1-cor-1 .statement}

— *Cho E và F là hai không gian Banach, H là một họ các ánh xạ tuyến tính liên tục từ E vào F; nếu, với mọi $x \in E$, ta có $\sup_{u \in H} \|u(x)\| < +\infty$, thì ta cũng có $\sup_{u \in H} \|u\| < +\infty$.*

Thật vậy, giả thiết nói rằng H bị chặn đơn giản và kết luận nói rằng nó đồng liên tục. Ngoài ra, mọi không gian Banach đều là vành thùng (III, p. 25).

#### Hệ quả 2 {#evt-iii-s4-thm-1-cor-2 .statement}

— (định lý Banach-Steinhaus). — *Cho E là một không gian vành thùng, F là một không gian lồi địa phương Hausdorff, và cho $(u_n)$ là một dãy các ánh xạ tuyến tính liên tục* từ E vào F, hội tụ đơn giản tới một ánh xạ u từ E vào F. Khi đó $ u \in \mathcal{L}(E; F) $, và $ (u_n) $ hội tụ tới u đều trên mọi tập con tiền compắc của E.

Thật vậy, dãy $ (u_n) $ bị chặn đơn giản, do đó đồng liên tục, và hệ quả suy ra từ hệ quả của mệnh đề 5 của III, p. 18.

#### Nhận xét {#evt-iii-s4-n2-rem-1 .statement}

— 1) Tính chất được phát biểu bởi hệ quả 2 không kéo theo rằng E là vành thùng: ta sẽ thấy sau này rằng đối ngẫu mạnh của một không gian Fréchet có tính chất này, trong khi không nhất thiết là vành thùng (IV, p. 23, hệ quả của mệnh đề 2 và p. 58, bài tập.

2) Cho E và F là hai không gian Banach, và $ (u_n) $ là một dãy các ánh xạ tuyến tính liên tục từ E vào F sao cho $ \sup \|u_n\| = + \infty $. Khi đó tập hợp X gồm mọi $ x \in E $ sao cho $ \sup \|u_n(x)\| = + \infty $ là trù mật trong E và là giao của một dãy các tập hợp mở trong E. Thật vậy, ký hiệu $ X_k $ là tập hợp mọi $ x \in E $ sao cho $ \sup \|u_n(x)\| > k $ (với k là số nguyên $ > 0 $). Mỗi $ X_k $ là mở và X là giao của các $ X_k $. Vì E là một không gian Baire, chỉ cần chứng minh rằng mỗi $ X_k $ đều trù mật trong E. Nhưng, nếu phần bù của $ X_k $ chứa một tập hợp mở không rỗng U, thì ta sẽ có $ \|u_n(x)\| \leq 2k $ với $ x \in U - U $ và, vì $ U - U $ là một lân cận của 0, ta sẽ có $ \sup \|u_n\| < + \infty $.

#### Hệ quả 3 {#evt-iii-s4-thm-1-cor-3 .statement}

— *Cho E là một không gian thùng, F là một không gian lồi địa phương Hausdorff và $ \Phi $ là một bộ lọc trên $ \mathcal{L}(E; F) $ hội tụ đơn giản trong E tới một ánh xạ u từ E vào F. Nếu $ \Phi $ chứa một tập con bị chặn đơn giản của $ \mathcal{L}(E; F) $, hoặc nếu $ \Phi $ có một cơ sở đếm được, thì u là một ánh xạ tuyến tính liên tục từ E vào F và $ \Phi $ hội tụ đều tới u trên mọi tập con tiền compắc của E.*

Trước hết giả sử rằng $ \Phi $ chứa một tập H bị chặn đơn giản; vì H là đồng liên tục (đl. 1), hệ quả suy ra từ hệ quả của mệnh đề 5 (III, p. 18). Nếu $ \Phi $ có một cơ sở đếm được, thì mọi bộ lọc sơ cấp $ \Psi $ liên kết với một dãy $ u_n $ (GT, I, § 6, No. 8) mịn hơn $ \Phi $ đều hội tụ đơn giản tới u trong E và từ hệ quả 2 suy ra rằng u là một ánh xạ tuyến tính liên tục từ E vào F, và rằng $ \Psi $ hội tụ tới u đối với tôpô hội tụ đều trên các tập con tiền compắc của E. Do đó điều tương tự cũng đúng với $ \Phi $, vì bộ lọc sau là giao của các bộ lọc sơ cấp, mỗi bộ lọc đều mịn hơn $ \Phi $ (GT, I, § 6, No. 8).

Ta nhận thấy rằng một bộ lọc trên $ \mathcal{L}(E; F) $ hội tụ đơn và có một cơ sở đếm được không nhất thiết chứa một tập hợp bị chặn đơn nào: để thấy điều đó, hãy xét ví dụ bộ lọc các lân cận của 0 trong $ \mathcal{L}(K; F) $ khi tôpô của F là khả mêtric, nhưng không thể được xác định bởi một chuẩn duy nhất.

#### Ví dụ {#evt-iii-s4-n2-exa-1 .statement}

— Cho E là không gian Banach (trên $ \mathbf{C} $) gồm các hàm phức liên tục, tuần hoàn chu kỳ 1 trên $ \mathbf{R} $, với chuẩn $ \|f\| = \sup_x |f(x)| $.

Với mọi số nguyên $ n \in \mathbf{Z} $ và mọi hàm $ f \in E $, đặt $ c_n(f) = \int_0^1 f(x) e^{-2i\pi nx} dx $ (hệ số Fourier thứ $ n $ của $ f $) ; mỗi một trong các ánh xạ $ f \mapsto c_n(f) $ là một dạng tuyến tính liên tục trên E. Gọi $ (\alpha_n) $ là một dãy số phức sao cho, với mọi hàm $ f \in E $, chuỗi có số hạng tổng quát $ \alpha_n c_n(f) + \alpha_{-n} c_{-n}(f) $ là hội tụ. Trong các điều kiện ấy, ánh xạ $ u : f \mapsto \alpha_0 c_0(f) + \sum_{n \geq 1} [\alpha_n c_n(f) + \alpha_{-n} c_{-n}(f)] $ là một dạng tuyến tính liên tục trên E ; \* nói cách khác, tồn tại một độ đo $ \mu $ trên $[0, 1]$ sao cho $ u(f) = \int f(x) d\mu(x) $ với mọi hàm $ f \in E $, và $ \alpha_n $ là hệ số Fourier thứ $ n $ của $ \mu $.* Thật vậy, với mọi số nguyên $ m > 0 $, ánh xạ $ f \mapsto \sum_{k = -m}^m \alpha_k c_k(f) $ là một dạng tuyến tính liên tục $ u_m $ trên E, và với mọi $ f \in E $, dãy $ (u_m(f)) $ hội tụ đến $ u(f) $, theo giả thiết. Khi đó mệnh đề suy ra từ định lý Banach-Steinhaus, vì E là không gian thùng.

#### Hệ quả 4 {#evt-iii-s4-thm-1-cor-4 .statement}

— *Cho E và F là hai không gian lồi địa phương, $ \mathfrak{S} $ là một phủ của E gồm các tập con bị chặn. Nếu E là đầy thùng và F Hausdorff và gần đầy đủ, thì không gian $ \mathcal{L}_{\mathfrak{S}}(E; F) $ là Hausdorff và gần đầy đủ.*

Thật vậy, mọi tập con bị chặn và đóng của $ \mathcal{L}_{\mathfrak{S}}(E; F) $ đều đơn giản bị chặn (vì $ \mathfrak{S} $ là một phủ của E), do đó là đồng liên tục (III, p. 25, định lý 1) và vì thế là một không gian con đầy đủ của $ \mathcal{L}_{\mathfrak{S}}(E; F) $ theo mệnh đề 11 (III, p. 22).

#### Hệ quả 5 {#evt-iii-s4-thm-1-cor-5 .statement}

— *Đối ngẫu mạnh và đối ngẫu yếu của một không gian đầy thùng là gần đầy đủ.*

### 3. Các tập con bị chặn của $ \mathcal{L}(E; F) $ (trường hợp gần đầy đủ)

#### Định lý 2 {#evt-iii-s4-thm-2 .statement}

— *Cho E là một không gian lồi địa phương Hausdorff, F là một không gian lồi địa phương và $ \mathfrak{S} $ là một họ các tập con đóng, lồi, cân bằng, bị chặn và nửa đầy đủ của E (III, p. 7). Mọi tập con đơn giản bị chặn H của $ \mathcal{L}(E; F) $ đều bị chặn đối với $ \mathfrak{S} $-tôpô.*

Cho $ A \in \mathfrak{S} $. Khi đó không gian $ E_A $ là một không gian Banach (III, p. 8, hệ quả), do đó là không gian thùng. Mặt khác, ảnh chính tắc của H trong $ \mathcal{L}(E_A; F) $ đơn giản là bị chặn, do đó đồng liên tục (III, p. 25, định lý 1). Do đó, tập hợp tất cả các $ u(x) $ với $ u \in H $ và $ x \in A $ là bị chặn trong F, điều này chứng minh rằng H bị chặn đối với tôpô $ \mathfrak{S} $.

#### Hệ quả 1 {#evt-iii-s4-thm-2-cor-1 .statement}

— *Cho E là một không gian Hausdorff lồi địa phương, F là một không gian lồi địa phương, và $ \mathfrak{S} $ là một họ các tập con bị chặn của E. Nếu E là nửa đầy đủ, thì mọi tập con bị chặn đơn của $ \mathcal{L}(E; F) $ đều bị chặn đối với tôpô $ \mathfrak{S} $.*

Chỉ cần áp dụng định lý 2, sau khi thay thế các tập hợp của $ \mathfrak{S} $ bởi các bao đóng, lồi, cân bằng của chúng, vì điều đó không thay đổi tôpô $ \mathfrak{S} $.

Khi E là nửa đầy đủ (chẳng hạn giả đầy đủ), ta có thể nói đến các *tập con bị chặn* của $ \mathcal{L}(E; F) $ mà không cần chỉ rõ tôpô $ \mathfrak{S} $, vì các tập này là như nhau đối với mọi tôpô $ \mathfrak{S} $ mỗi khi $ \mathfrak{S} $ là một phủ của E.

#### Hệ quả 2 {#evt-iii-s4-thm-2-cor-2 .statement}

— *Mọi không gian bornological nửa đầy đủ đều là thùng.*

Mọi tập con bị chặn đơn giản của đối ngẫu của một không gian như vậy đều bị chặn mạnh (hệ quả 1), do đó đồng liên tục (III, p. 22, mệnh đề 10).

#### Hệ quả 3 {#evt-iii-s4-thm-2-cor-3 .statement}

— *Cho E là một không gian lồi địa phương. Mọi tập con của E bị chặn đối với $ \sigma(E, E') $ đều bị chặn.*

Cho A là một tập con của E. Nói rằng A bị chặn đối với $ \sigma(E, E') $ có nghĩa là mọi dạng tuyến tính liên tục trên E đều bị chặn trên A ; nói rằng A bị chặn có nghĩa là mọi nửa chuẩn liên tục trên E đều bị chặn trên A. Gọi N là bao đóng của 0 trong E và $ \pi $ là ánh xạ chính tắc từ E lên E/N. Các dạng tuyến tính liên tục trên E là các ánh xạ có dạng $ f \circ \pi $ với $ f \in (E/N)' $ và ta có một đặc trưng hóa tương tự đối với các nửa chuẩn liên tục trên E. Do đó, bằng cách thay thế E bởi E/N và A bởi $ \pi(A) $, ta có thể giới hạn vào trường hợp E là Hausdorff.

Cho $ \mathfrak{S} $ là tập hợp các tập con đồng liên tục của $ E' $; khi gán cho $ E' $ tôpô $ \sigma(E', E) $, $ E $ có thể được đồng nhất với $ (E')_{\mathfrak{S}}' $ (III, p. 19, hệ quả 1). Mọi tập con đồng liên tục đóng của $ E' $ đều compact đối với $ \sigma(E', E) $ (III, p. 17, hệ quả 2), do đó đầy đủ đối với $ \sigma(E', E) $. Bây giờ chỉ cần áp dụng định lý 2.

### Bài tập {#evt-iii-s4-exercises}

Xem [bài tập của § 4](exercises/s4/).
