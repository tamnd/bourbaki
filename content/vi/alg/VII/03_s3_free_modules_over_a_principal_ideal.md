---
book: alg
book_title: Algebra
chapter: VII
chapter_title: MODULES OVER PRINCIPAL IDEAL DOMAINS
section: 3
section_title: Free modules over a principal ideal domain
lang: vi
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A VII.14-A VII.15, A VII.59-A VII.62
pdf_pages: 0373-0374, 0418-0421
extraction: ocr
statements: 6
exercises: 11
content_sha256: 189c57f58cd23f0952a4af9369619052b4c7779ceac70e1a36d6a5d35b0733c8
translated_from: content/en/alg/VII/03_s3_free_modules_over_a_principal_ideal.md
source_content_sha256: 066133593c0e8a083eeae9d05d1754b642bc50b68931b431ed70f46e8f995177
translation_model: gpt-5.4
translation_run: translate-vi-40e2123e
glossary_version: 34
glossary_terms_sha256: 0e3eadd09e3ca45f08d856eecac1880d4006fd5557b013f992ba0d680884e27f
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 3. MÔĐUN TỰ DO TRÊN MỘT MIỀN IĐÊAN CHÍNH

#### Định lý 1 {#alg-vii-s3-thm-1 .statement}

— *Cho $A$ là một vành sao cho mọi iđêan trái của $A$ đều xạ ảnh (II, p. 231, Định nghĩa 1) như một $A$-môđun. Khi đó mọi môđun con $M$ của một $A$-môđun trái tự do $L$ là một tổng trực tiếp của các môđun đẳng cấu với các iđêan của $A$.*

Cho $(e_i)_{i \in I}$ là một cơ sở của $L$, và cho $p_i$ là các hàm tọa độ tương ứng với cơ sở này. Chọn một *thứ tự tốt* (*Lý thuyết tập hợp*, III, p. 153) trên $I$ và ký hiệu $L_\alpha$ là môđun con sinh bởi các $e_i$, với $\alpha \leq i$; đặt $M_\alpha = M \cap L_\alpha$. Hàm tọa độ $p_i$ ánh xạ $M_\alpha$ lên một iđêan $a_\alpha$ của $A$; vì $a_\alpha$ là một $A$-môđun xạ ảnh, nên tồn tại (II, p. 231, Prop. 4) một môđun con $N_\alpha$ của $M$, sao cho ánh xạ $x \mapsto p_i(x)$ từ $N_\alpha$ vào $a_\alpha$ là song ánh. Gọi $M'_\alpha$ là môđun con của $L$ sinh bởi các $N_\alpha$, với $\alpha \leq i$; ta sẽ chứng minh rằng $M'_\alpha = M_\alpha$ với mọi $\alpha$, điều này sẽ suy ra rằng $M$ được sinh bởi họ $(N_\alpha)_{\alpha < i}$. Thật vậy, giả sử $M'_\lambda = M_\lambda$ với mọi $\lambda < i$; khi đó $p_\lambda(x) \in a_\lambda$, với mọi $x \in M_\lambda$; do đó tồn tại $y \in N_\lambda$ sao cho $x - y$ là một tổ hợp tuyến tính của hữu hạn phần tử $e_i$, với $\alpha < \lambda$; nói cách khác $x - y$ là một phần tử của $M_\alpha$, với một $\lambda < i$ nào đó; giả thiết quy nạp cho thấy $x - y \in M'_\lambda \subset M'_\alpha$, nghĩa là $x \in M'_\alpha$, và do đó $M'_\alpha = M_\alpha$. Còn phải chứng minh rằng tổng của các $N_\alpha$ là trực tiếp; bây giờ giả sử tồn tại một quan hệ tuyến tính $\sum a_\alpha = 0$, với $a_\alpha \in N_\alpha$, trong đó các $a_\alpha$ (trừ hữu hạn phần tử đều bằng không) không đồng thời bằng không. Gọi $p$ là chỉ số lớn nhất $\alpha$ sao cho $a_\alpha \neq 0$; vì $p_\mu(a_\lambda) = 0$ với $\lambda < \mu$, ta có $p_\mu(a_\mu) = p_\mu\left( \sum a_\alpha \right) = 0$, nên $a_\mu = 0$, mâu thuẫn với lựa chọn $p$.

#### Hệ quả 1 {#alg-vii-s3-thm-1-cor-1 .statement}

— *Nếu mọi iđêan trái của $A$ đều xạ ảnh, thì mọi môđun con của một $A$-môđun trái xạ ảnh đều xạ ảnh.*

Thật vậy mọi $A$-môđun xạ ảnh đều là một môđun con của một $A$-môđun tự do (II, p. 231, Mệnh đề 4), và Định lý 1 áp dụng được.

#### Hệ quả 2 {#alg-vii-s3-thm-1-cor-2 .statement}

— *Mọi môđun con của một môđun tự do trên một miền iđêan chính đều tự do.*
    Điều này suy ra ngay lập tức từ Định lý 1, vì mọi iđêan của một miền iđêan chính đều tự do.

#### Hệ quả 3 {#alg-vii-s3-thm-1-cor-3 .statement}

— *Mọi môđun xạ ảnh trên một miền iđêan chính đều tự do.*
*Nhận xét.* — Chứng minh của Định lý 1 cho thấy rằng mọi môđun con của $A^{(1)}$ đều đẳng cấu với một tổng trực tiếp $\bigoplus a_i$, trong đó mỗi $a_i$ là một iđêan của $A$.

MỆNH ĐỀ I. — *Nếu L là một môđun tự do hạng hữu hạn n trên một miền iđêan chính A, thì mọi môđun con M của L đều là một môđun tự do hạng $\leq n$.*
    Thật vậy M là một môđun tự do theo Hệ quả 2 của Định lý 1, và nó có hạng $\leq n$ theo nhận xét trước, hoặc theo bổ đề sau:

#### Bổ đề 1 {#alg-vii-s3-lem-1 .statement}

— *Cho L là một môđun trên một vành giao hoán A, sinh bởi n phần tử, và cho M là một môđun con tự do của L; khi đó M có hạng $\leq n$.*
    Trước hết giả sử L là tự do. Gọi i là đơn ánh chính tắc của M vào L. Theo III, p. 520, Hệ quả, đồng cấu $\bigwedge^n i : \bigwedge^n M \to \bigwedge^n L$ là đơn ánh; theo III, p. 511, Mệnh đề 6, $\bigwedge^n L = \{0\}$, nên $\bigwedge^n M = \{0\}$; suy ra M có hạng $\leq n$ (III, p. 518, Hệ quả 1). Bây giờ xét trường hợp tổng quát; môđun L là một thương của một môđun tự do L' có hạng n. Tồn tại một môđun con M' của L' đẳng cấu với M (II, p. 218, Mệnh đề 21). Theo phần đầu của lập luận, M' có hạng $\leq n$, và kết quả suy ra.

#### Hệ quả {#alg-vii-s3-n0-cor-1 .statement}

— *Cho E là một môđun trên một miền iđêan chính A, sinh bởi n phần tử. Khi đó mọi môđun con F của E đều có thể sinh bởi nhiều nhất n phần tử.*
    Thật vậy tồn tại một đồng cấu f từ $A^n$ lên E (II, p. 216, Hệ quả 3), và $f^{-1}(F)$, là một môđun tự do có hạng $m \leq n$, được sinh bởi n phần tử; các ảnh của những phần tử này qua f sinh ra F.

### Bài tập {#alg-vii-s3-exercises}

Xem [các bài tập cho § 3](exercises/s3/).
