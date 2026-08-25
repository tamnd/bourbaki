---
book: int
book_title: Integration
chapter: IX
chapter_title: MEASURES ON HAUSDORFF TOPOLOGICAL SPACES
section: 4
section_title: Inverse limits of measures
lang: vi
source: int-vii-ix
book_pages: INT IX.49-INT IX.55, INT IX.112-INT IX.113
pdf_pages: 0231-0237, 0294-0295
extraction: ocr
subsections:
    - "no": 1
      title: Complements on compact spaces and inverse limits
      page: 50
      pdf_page: 232
    - "no": 2
      title: Inverse systems of measures
      page: 50
      pdf_page: 232
    - "no": 3
      title: The case of countable inverse systems
      page: 54
      pdf_page: 236
statements: 7
exercises: 2
content_sha256: 94a888bdc5712bc68bbe1226b048bcf0c6046114c395d4390799779c159b730e
translated_from: content/en/int/IX/04_s4_inverse_limits_of_measures.md
source_content_sha256: aa4d547d2b59667d4b6a9c6560eb3a9d0270aca967cd7924b7b700b6cb81c4e8
translation_model: gpt-5.4
translation_run: translate-vi-145f2a6b
glossary_version: 34
glossary_terms_sha256: c38a0ce5cf634a91faa7a197e707a39a370bc534b9a93014348d4c316e88bd71
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 4. GIỚI HẠN NGHỊCH ĐẢO CỦA CÁC ĐỘ ĐO

*Trong suốt tiết này, I ký hiệu một tập hợp khác rỗng, được trang bị một quan hệ tiền thứ tự, ký hiệu là $i \leq j$, và có hướng đối với quan hệ này. Nhắc lại (GT, I, §4, No. 4) rằng một hệ ngược các không gian tôpô được đánh chỉ số bởi I là một họ $(T_i, p_{ij})$ trong đó $T_i$ là một không gian tôpô và $p_{ij}$ là một ánh xạ liên tục từ $T_j$ vào $T_i$ với $i \leq j$, trong đó $p_{ii}$ là ánh xạ đồng nhất của $T_i$, và trong đó $p_{ik} = p_{ij} \circ p_{jk}$ với $i \leq j \leq k$. Cho T là một không gian tôpô và $(p_i)_{i \in I}$ một họ các ánh xạ liên tục $p_i : T \to T_i$. Họ $(p_i)_{i \in I}$ được gọi là tương thích nếu $p_i = p_{ij} \circ p_j$ với $i \leq j$, và được gọi là phân ly nếu với mọi $x, y$ phân biệt trong T, tồn tại một $i \in I$ sao cho $p_i(x) \neq p_i(y)$. Khi $T = \varprojlim T_i$ và $p_i$ là ánh xạ chính tắc từ T vào $T_i$, thì họ $(p_i)_{i \in I}$ là tương thích và phân ly.*

(3) Trong một không gian Souslin, mọi tập Borel đều là một tập Souslin (GT, IX, §6, No. 3, Mệnh đề 11).
(4) Tổng quát hơn, nếu $f : X \to Y$ là một song ánh liên tục giữa các không gian Souslin, thì $\mu \mapsto f(\mu)$ là một ánh xạ song ánh từ tập hợp các độ đo bị chặn trên X lên tập hợp các độ đo bị chặn trên Y (\S2, No. 4, Mệnh đề 9).

### 1. Bổ túc về các không gian compắc và các giới hạn ngược

#### Mệnh đề 1 {#int-ix-s4-prop-1 .statement}

— Cho X và Y là hai không gian tôpô và f là một ánh xạ liên tục từ X vào Y. Cho $(K_\alpha)_{\alpha \in A}$ là một họ có hướng giảm các tập con compắc của X, với giao là K. Khi đó $f(K) = \bigcap_{\alpha \in A} f(K_\alpha)$.

Thật vậy, cho y là một điểm của $\bigcap_{\alpha \in A} f(K_\alpha)$; với mọi $\alpha \in A$, tập $L_\alpha = K_\alpha \cap f^{-1}(y)$ là compắc và khác rỗng. Họ $(L_\alpha)_{\alpha \in A}$ có hướng theo thứ tự giảm, do đó giao của nó là L khác rỗng. Bây giờ, $L = K \cap f^{-1}(y)$, do đó $y \in f(K)$. Vậy ta đã chứng minh được bao hàm $f(K) \supset \bigcap_{\alpha \in A} f(K_\alpha)$, và bao hàm ngược lại là hiển nhiên.

#### Mệnh đề 2 {#int-ix-s4-prop-2 .statement}

— Cho một hệ ngược $(T_i, p_{ij})$ các không gian tôpô được đánh chỉ số bởi I, một không gian tôpô T, và một họ kết hợp và phân biệt các ánh xạ liên tục $p_i : T \to T_i$. Khi đó:

a) Với mọi tập con compắc K của T, ta có $K = \bigcap_{i \in I} p_i^{-1}(p_i(K))$.

b) Cho K và L là hai tập con compắc rời nhau của T. Tồn tại một $i \in I$ sao cho $p_j(K)$ và $p_j(L)$ rời nhau với $j \geq i$.

a) Cho x là một điểm của $\bigcap_{i \in I} p_i^{-1}(p_i(K))$; với mọi $i \in I$, tập hợp $K_i$ gồm các điểm y của K sao cho $p_i(y) = p_i(x)$ là một tập con khác rỗng đóng của K. Với $i \leq j$ ta có $K_i \supset K_j$, và vì K compac, nên tập hợp $\bigcap_{i \in I} K_i$ do đó là khác rỗng. Cho y là một điểm của $\bigcap_{i \in I} K_i$; ta có $y \in K$ và $p_i(y) = p_i(x)$ với mọi $i \in I$, do đó $y = x$; sau cùng, $x \in K$, điều này chứng minh bao hàm thức $K \supset \bigcap_{i \in I} p_i^{-1}(p_i(K))$; bao hàm thức ngược lại là hiển nhiên.

b) Với mọi $i \in I$, đặt $M_i = p_i^{-1}(p_i(K)) \cap L$; đây là một tập con đóng của không gian compact L, ta có $M_i \supset M_j$ với $i \leq j$, và, theo a),

$$
\bigcap_{i \in I} M_i = K \cap L = \varnothing.
$$

Do đó, tồn tại một chỉ số i sao cho $M_i = \varnothing$. Với $j \geq i$, ta có $p_j^{-1}(p_j(K)) \cap L = M_j \subset M_i = \varnothing$, do đó $p_j(K) \cap p_j(L) = \varnothing$.

### 2. Hệ nghịch đảo các độ đo

#### Định nghĩa 1 {#int-ix-s4-def-1 .statement}

— Cho $\mathcal{T} = (T_i, p_{ij})$ là một hệ ngược các không gian tôpô được chỉ số hóa bởi I. Người ta gọi một hệ ngược (tương ứng, một hệ con ngược) các độ đo trên $\mathcal{T}$ là một họ $(\mu_i)_{i \in I}$, trong đó $\mu_i$ là một độ đo bị chặn trên $T_i$ với mọi $i \in I$, và trong đó $\mu_i = p_{ij}(\mu_j)$ (tương ứng, $\mu_i \geq p_{ij}(\mu_j)$) nếu $i \leq j$.

#### Mệnh đề 3 {#int-ix-s4-prop-3 .statement}

*Cho một hệ ngược các không gian tôpô $\mathcal{T} = (T_i, p_{ij})$ được đánh chỉ số bởi $I$, một không gian tôpô $T$, một họ kết hợp và tách biệt các ánh xạ liên tục $p_i : T \to T_i$ (với $i \in I$) và một hệ con ngược $(\mu_i)_{i \in I}$ các độ đo trên $\mathcal{T}$. Với mọi tập con compact K của $T$, đặt*

$$
J(K) = \inf_{i \in I} \mu_i^\bullet(p_i(K)).
$$

*Khi đó tồn tại một độ đo bị chặn $\pi$ trên $T$, và chỉ có một, sao cho $\pi^\bullet(K) = J(K)$ với mọi tập con compact $K$ của $T$. Ta có $\mu_i \geq p_i(\pi)$ với mọi $i \in I$, và $\pi$ là độ đo lớn nhất trên $T$ thỏa mãn điều kiện này.*

Trước hết ta hãy chứng minh rằng $J(K)$ là giới hạn của $\mu_i^\bullet((p_i(K)))$ đối với bộ lọc tiết diện $\mathfrak{F}$ của tập hợp tiền thứ tự có hướng $I$: để làm điều này, theo (GT, IV, §5, No. 2, Th. 2) chỉ cần chỉ ra rằng $\mu_i^\bullet(p_i(K)) \geq \mu_j^\bullet(p_j(K))$ với $i \leq j$; bây giờ, đặt $\mu_{ij}' = p_{ij}(\mu_j)$, ta có $\mu_{ij}' \leq \mu_i$ và $p_j(K) \subset \overline{p_{ij}}^{-1}(p_i(K))$, do đó

$$
\mu_j^\bullet(p_j(K)) \leq \mu_j^\bullet(\overline{p_{ij}}^{-1}(p_i(K))) = (\mu_{ij}')^\bullet(p_i(K)) \leq \mu_i^\bullet(p_i(K)).
$$

Bây giờ ta hãy chuyển sang nghiên cứu các tính chất của hàm $J$:
1) Rõ ràng là $J(K) \leq J(L)$ khi $K \subset L$.
2) Cho $K$ và $L$ là hai tập compact của $T$. Với mọi $i \in I$, ta có $p_i(K \cup L) = p_i(K) \cup p_i(L)$, do đó

$$
\mu_i^\bullet(p_i(K \cup L)) \leq \mu_i^\bullet(p_i(K)) + \mu_i^\bullet(p_i(L));
$$

chuyển qua giới hạn theo bộ lọc $\mathfrak{F}$, ta được $J(K \cup L) \leq J(K) + J(L)$.
3) Giả sử rằng các tập hợp compắc $K$ và $L$ rời nhau. Theo Mệnh đề 2 của No. 1, tồn tại một $i \in I$ sao cho $p_j(K) \cap p_j(L) = \varnothing$ với $j \geq i$. Do đó, với $j \geq i$ ta có

$$
\mu_j^\bullet(p_j(K \cup L)) = \mu_j^\bullet(p_j(K)) + \mu_j^\bullet(p_j(L)),
$$

do đó $J(K \cup L) = J(K) + J(L)$ khi chuyển qua giới hạn đối với bộ lọc $\mathfrak{F}$.
4) Cho $(K_\alpha)_{\alpha \in A}$ là một họ có hướng giảm các tập compact của $T$, với giao là $K$. Theo Mệnh đề 1 của No. 1, $p_i(K) = \bigcap_{\alpha \in A} p_i(K_\alpha)$ và do đó $\mu_i^\bullet(p_i(K)) = \inf_{\alpha \in A} \mu_i^\bullet(p_i(K_\alpha))$ với mọi $i \in I$ (\S1, No. 6, Hệ quả của Mệnh đề 5). Từ đó, suy ra
$$
J(K) = \inf_{i \in I} \mu_i^\bullet(p_i(K)) = \inf_{i \in I} \inf_{\alpha \in A} \mu_i^\bullet(p_i(K_\alpha))
= \inf_{\alpha \in A} \inf_{i \in I} \mu_i^\bullet(p_i(K_\alpha)) = \inf_{\alpha \in A} J(K_\alpha).
$$
5) Hãy chọn một $i \in I$ và đặt $c = \mu_i^\bullet(T_i)$. Khi đó $c$ là hữu hạn và $J(K) \leq \mu_i^\bullet(p_i(K)) \leq \mu_i^\bullet(T_i)$, vậy $J(K) \leq c$ với mọi tập compact $K$ trong $T$.

Các tính chất đi trước cho phép áp dụng Đl. 1 của \S3, No. 1; ta kết luận rằng tồn tại một và chỉ một độ đo bị chặn $\pi$ trên $T$ sao cho $\pi^\bullet(K) = J(K)$ với mọi tập con compắc $K$ của $T$. Với mỗi $i \in I$, ký hiệu bởi $\nu_i$ độ đo trên $T_i$ là ảnh của $\pi$ qua $p_i$. Cho $i \in I$, $A$ là một tập con compắc của $T_i$, và $\mathcal{L}$ là tập hợp các tập con compắc của $\overline{p_i^{-1}(A)}$. Theo Nhận xét 3 của \S1, No. 2, ta có $\pi^\bullet(\overline{p_i^{-1}(A)}) = \sup_{K \in \mathcal{L}} \pi^\bullet(K)$; hơn nữa, $\nu_i^\bullet(A) = \pi^\bullet(\overline{p_i^{-1}(A)})$ và $J(K) = \pi^\bullet(K)$ với $K \in \mathcal{L}$, do đó $\nu_i^\bullet(A) = \sup_{K \in \mathcal{L}} J(K)$.

Với $K \in \mathcal{L}$, ta có $p_i(K) \subset A$, do đó $J(K) \leq \mu_i^\bullet(p_i(K)) \leq \mu_i^\bullet(A)$ và cuối cùng $\nu_i^\bullet(A) \leq \mu_i^\bullet(A)$. Vì $A$ là một tập compact tùy ý trong $T_i$, ta kết luận rằng $\nu_i \leq \mu_i$. Khẳng định cuối cùng của mệnh đề là hiển nhiên.

Q.E.D.

#### Định lý 1 (Prokhorov) {#int-ix-s4-thm-1 .statement}

— *Cho $\mathcal{T} = (T_i, p_{ij})$ là một hệ ngược các không gian tôpô được đánh chỉ số bởi $I$, $T$ là một không gian tôpô và $(p_i)_{i \in I}$ là một họ tương thích và phân biệt các ánh xạ liên tục $p_i : T \to T_i$. Sau hết, giả sử $(\mu_i)_{i \in I}$ là một hệ ngược các độ đo trên $\mathcal{T}$.

Để tồn tại một độ đo bị chặn $\mu$ trên $T$ sao cho $p_i(\mu) = \mu_i$ với mọi $i \in I$, điều kiện cần và đủ là điều kiện sau được thỏa mãn:

(P) *với mọi $\varepsilon > 0$, tồn tại một tập con compact $K$ của $T$ sao cho $\mu_i^\bullet(T_i - p_i(K)) \leq \varepsilon$ với mọi $i \in I$.

Khi đó, độ đo $\mu$ được xác định duy nhất và*
$$
\mu^\bullet(K) = \inf_i \mu_i^\bullet(p_i(K))
$$
*đối với mọi tập compact $K$ trong $T$*.

Trước hết ta hãy chứng minh tính duy nhất của $\mu$. Cho $\mu$ là một độ đo bị chặn trên $T$ sao cho $p_i(\mu) = \mu_i$ với mọi $i \in I$. Gọi $K$ là một tập con compact của $T$; theo Mệnh đề 2 của No. 1, tập hợp $K$ là giao của họ có hướng giảm $(\overline{p_i^{-1}(p_i(K))})_{i \in I}$ các tập con *đóng* của $T$. Bởi Hệ quả của Mệnh đề 5 của \S1, No. 6, do đó ta có
$$
\mu^\bullet(K) = \inf_{i \in I} \mu^\bullet(\overline{p_i^{-1}(p_i(K))}) = \inf_{i \in I} \mu_i^\bullet(p_i(K)),
$$

điều này thiết lập công thức (2). Vì hai độ đo trùng nhau trên tập hợp các tập compact thì bằng nhau (\S 1, No. 2, Hệ quả của Mệnh đề 2), suy ra $\mu$ là duy nhất.

Theo Mệnh đề 3, tồn tại một độ đo bị chặn $\pi$ trên $T$ sao cho $\pi^\bullet(K) = \inf_{i \in I} \mu_i^\bullet(p_i(K))$ với mọi tập con compắc $K$ của $T$. Theo công thức (2), vì thế sự tồn tại của một độ đo bị chặn $\mu$ trên $T$ sao cho $p_i(\mu) = \mu_i$ với mọi $i \in I$ là tương đương với quan hệ:

(P') $p_i(\pi) = \mu_i$ với mọi $i \in I$.

Với $i \leq j$, ta có $\mu_i = p_{ij}(\mu_j)$, do đó $\mu_i^\bullet(T_i) = \mu_j^\bullet(T_j)$; vì $I$ có hướng, tồn tại một số hữu hạn $c \geq 0$ sao cho $\mu_i^\bullet(T_i) = c$ với mọi $i \in I$. Theo Mệnh đề 3, độ đo $\mu_i - p_i(\pi)$ là dương, do đó nó bằng không khi và chỉ khi khối lượng toàn phần của nó bằng không, nghĩa là khi $\mu_i(T_i) = p_i(\pi)^\bullet(T_i)$. Vì $p_i(\pi)^\bullet(T_i) = \pi^\bullet(T)$, nên điều kiện (P') do đó tương đương với $\pi^\bullet(T) = c$, tức là (\S 1, No. 2, Nhận xét 3) với tính chất:

(P'') $\sup_{K \in \mathcal{K}} \pi^\bullet(K) = c$, trong đó $\mathcal{K}$ là tập hợp các tập con compact của $T$.

Bây giờ, với $K \in \mathcal{K}$, ta có

$$
\pi^\bullet(K) = \inf_{i \in I} \mu_i^\bullet(p_i(K)) = c - \sup_{i \in I} \mu_i^\bullet(T_i - p_i(K))
$$

và công thức này ngay lập tức suy ra tính tương đương của (P) và (P'').

Q.E.D.

Cho $(T_i, p_{ij})$ là một hệ ngược các không gian tôpô. Đặt $T = \lim_{\leftarrow} T_i$ và ký hiệu bởi $p_i$ ánh xạ chính tắc từ $T$ vào $T_i$. Tổng quát hóa Định nghĩa 2 của Ch. III, \S 4, No. 5, ta sẽ nói rằng một độ đo bị chặn $\mu$ trên $T$ là *giới hạn ngược của một hệ ngược* $(\mu_i)_{i \in I}$ *các độ đo* nếu $\mu_i = p_i(\mu)$ với mọi $i \in I$. Định lý 1 cho một tiêu chuẩn về sự tồn tại của các giới hạn ngược của độ đo. Khi các không gian $T_i$ là *compact*, và các ánh xạ $p_{ij}$ toàn ánh, thì $T$ là compact và $p_i(T) = T_i$ với mọi $i \in I$; do đó điều kiện (P) được thỏa mãn, và trong trường hợp này ta thu lại Mệnh đề 8, (iv) của Ch. III, \S 4, No. 5.

#### Nhận xét {#int-ix-s4-n2-rem-1 .statement}

— Cho $(\mu_i)_{i \in I}$ là một hệ ngược các độ đo trên hệ ngược các không gian $\mathcal{T} = (T_i, p_{ij})$. Giả sử đã cho một không gian tôpô $T'$ và các ánh xạ liên tục $p'_i : T' \to T_i$; giả sử rằng họ $(p'_i)_{i \in I}$ là tương hợp, nhưng không nhất thiết phân biệt các điểm. *Nếu điều kiện Prokhorov (P) được thỏa mãn bởi họ* $(p'_i)_{i \in I}$, *thì tồn tại một độ đo* $\mu'$ (*không nhất thiết duy nhất*) *trên* $T'$ *sao cho* $p'_i(\mu') = \mu_i$ *với mọi* $i \in I$.

Thật vậy, đặt $T = \lim_{\leftarrow} T_i$ và $p' = (p'_i)_{i \in I}$, và ký hiệu bởi $p_i$ ánh xạ chính tắc từ $T$ vào $T_i$; điều kiện của Prokhorov được thỏa mãn bởi $T$ và các $p_i$, vì $p_i(p'(K')) = p'_i(K')$ và $p'(K')$ là compact trong $T$ với mọi tập con compact $K'$ của $T'$. Theo Định lý 1, tồn tại một độ đo bị chặn $\mu$ trên $T$ sao cho $p_i(\mu) = \mu_i$ với mọi $i \in I$. Cho $K'$ là một tập compact trong $T'$; khi đó $\mu^\bullet(p'(K')) = \inf_{i \in I} \mu_i^\bullet(p'_i(K'))$, do đó
$$
\mu^\bullet(T - p'(K')) = \sup_{i \in I} \mu_i^\bullet(T_i - p_i'(K')).
$$
Cho $\varepsilon > 0$; bởi vì điều kiện (P) của Prokhorov được thỏa mãn bởi các $p_i'$, do đó có thể tìm được một tập con compact $K'$ của $T'$ sao cho $\mu^\bullet(T - p'(K')) \leq \varepsilon$. Khi đó Mệnh đề 8 của §2, No. 4 thiết lập sự tồn tại của một độ đo bị chặn $\mu'$ trên $T'$ sao cho $\mu = p'(\mu')$, do đó $\mu_i = p_i(\mu) = p_i(p'(\mu')) = p_i'(\mu')$ với mọi $i \in I$.

### 3. Trường hợp các hệ ngược đếm được

#### Định lý 2 {#int-ix-s4-thm-2 .statement}

— *Giả sử tập tiền thứ tự có hướng I có một tập con đồng cuối đếm được. Cho $\mathcal{T} = (T_i, p_{ij})$ là một hệ ngược các không gian tôpô, $T = \lim_{\leftarrow} T_i$ và $p_i$ là ánh xạ chính tắc từ $T$ vào $T_i$. Khi đó mọi hệ ngược $(\mu_i)_{i \in I}$ các độ đo trên $\mathcal{T}$ đều thừa nhận một giới hạn ngược.*

Trước hết ta xét trường hợp $I = \mathbf{N}$ và đặt $q_n = p_{n,n+1}$. Cho $\varepsilon > 0$. Định nghĩa quy nạp một dãy các tập compact $L_n \subset T_n$ như sau: $L_0$ là một tập compact của $T_0$ sao cho $\mu_0^\bullet(T_0 - L_0) \leq \varepsilon/2$, và với $n \geq 0$ tập compact $L_{n+1}$ được chứa trong $\overline{q_n^{-1}(L_n)}$ và thỏa mãn
$$
\mu_{n+1}^\bullet(\overline{q_n^{-1}(L_n)} - L_{n+1}) \leq \varepsilon/2^{n+2}.
$$
Phép dựng này là có thể được nhờ *Nhận xét 3* của §1, No. 2. Ta có
$$
\begin{align*}
\mu_{n+1}^\bullet(T_{n+1} - L_{n+1}) &= \mu_{n+1}^\bullet(T_{n+1} - \overline{q_n^{-1}(L_n)}) + \mu_{n+1}^\bullet(\overline{q_n^{-1}(L_n)} - L_{n+1}) \\
&\leq \mu_{n+1}^\bullet(T_{n+1} - \overline{q_n^{-1}(L_n)}) + \varepsilon/2^{n+2} \\
&= \mu_n^\bullet(T_n - L_n) + \varepsilon/2^{n+2}
\end{align*}
$$
vì $\mu_n = q_n(\mu_{n+1})$; bằng quy nạp theo $p$, suy ra rằng
$$
\mu_p^\bullet(T_p - L_p) \leq \varepsilon(1 - 1/2^{p+1}) \leq \varepsilon.
$$
Vì $T$ là một không gian con đóng của $\prod_{n \in \mathbf{N}} T_n$ và không gian tích $\prod_{n \in \mathbf{N}} L_n$ là compact, tập con $L = T \cap \prod_{n \in \mathbf{N}} L_n = \bigcap_{n \in \mathbf{N}} \overline{p_n^{-1}(L_n)}$ của $T$ là compact. Cho $n \in \mathbf{N}$; ta có $p_n(L) = \bigcap_{m \geq n} p_{nm}(L_m)$ (GT, I, §9, No. 6, Mệnh đề 8) và $p_{nm}(L_m) \supset p_{nm'}(L_{m'})$ với $m' \geq m \geq n$, do đó
$$
\mu_n^\bullet(T_n - p_n(L)) = \lim_{m \to \infty} \mu_n^\bullet(T_n - p_{nm}(L_m)).
$$

Nhưng, với $m \geq n$, độ đo $\mu_n$ là ảnh của $\mu_m$ dưới $p_{nm}$, do đó

$$
\mu_n^\bullet(T_n - p_{nm}(L_m)) = \mu_m^\bullet(T_m - \overline{p}_{nm}(p_{nm}(L_m))) \leq \mu_m^\bullet(T_m - L_m) \leq \varepsilon;
$$

chuyển qua giới hạn theo $m$, ta được $\mu_n^\bullet(T_n - p_n(L)) \leq \varepsilon$. Nói cách khác, điều kiện (P) của Prokhorov được thỏa mãn, và tồn tại một độ đo bị chặn $\mu$ trên $T$ sao cho $\mu_n = p_n(\mu)$ với mọi $n \in \mathbf{N}$ (No. 2, Đl. 1).

Xét trường hợp tổng quát: tồn tại trong $I$ một dãy tăng đồng cuối $(i_n)_{n \in \mathbf{N}}$. Ánh xạ $t \mapsto (p_{i_n}(t))_{n \in \mathbf{N}}$ là một đồng phôi từ $T$ lên giới hạn ngược của hệ ngược $(T_{i_n}, p_{i_n i_m})$ (GT, I, §4, No. 4). Do phần đầu của chứng minh, do đó tồn tại một độ đo bị chặn $\mu$ trên $T$ sao cho $\mu_{i_n} = p_{i_n}(\mu)$ với mọi $n \in \mathbf{N}$. Lấy $i \in I$; tồn tại một $n \in \mathbf{N}$ sao cho $i \leq i_n$, do đó

$$
p_i(\mu) = p_{i i_n}(p_{i_n}(\mu)) = p_{i i_n}(\mu_{i_n}) = \mu_i.
$$

Q.E.D.

Định lý 2 thường được dùng trong tình huống sau: cho $D$ là một tập hợp đếm được và $(X_t)_{t \in D}$ là một họ các không gian tôpô. Gọi $\mathfrak{F}$ là tập hợp các tập con hữu hạn của $D$, có thứ tự theo bao hàm. Với $J$ thuộc $\mathfrak{F}$, đặt $X_J = \prod_{t \in J} X_t$, và với $J \subset J'$ gọi $p_{JJ'}$ là phép chiếu chính tắc của $X_{J'}$ lên tích bộ phận $X_J$. Cũng đặt $X = \prod_{t \in D} X_t$ và ký hiệu bởi $p_J$ phép chiếu chính tắc của $X$ lên tích bộ phận $X_J$. Ta dễ dàng chứng minh (xem S, III, §7, No. 2, Nhận xét 3) rằng họ $(p_J)_{J \in \mathfrak{F}}$ xác định một đồng phôi của $X$ lên $\lim_{\leftarrow} X_J$. Khi đó một hệ ngược các độ đo là một họ các độ đo bị chặn $\mu_J$ trên $X_J$ sao cho $\mu_J = p_{JJ'}(\mu_{J'})$ với $J \subset J'$. Tồn tại một và chỉ một độ đo bị chặn $\mu$ trên $X$ sao cho $\mu_J = p_J(\mu)$ với mọi tập con hữu hạn $J$ của $D$ (*định lý Kolmogoroff*). Đôi khi người ta nói rằng $\mu$ là độ đo trên $\prod_{t \in D} X_t$ có các *biên* $\mu_J$.

Đặc biệt, giả sử rằng, với mỗi $t \in D$, ta cho một độ đo $\nu_t$ trên $X_t$ có tổng khối lượng bằng 1. Đặt $\mu_J = \bigotimes_{t \in J} \nu_t$ với mọi tập con hữu hạn $J$ của $D$. Cho $J \subset J'$ là hai tập con hữu hạn của $D$ và đặt $K = J' - J$; khi đồng nhất $X_{J'}$ với $X_J \times X_K$, ta có $\mu_{J'} = \mu_J \otimes \mu_K$, và vì độ đo $\mu_K$ có tổng khối lượng bằng 1, phép chiếu của $\mu_J \otimes \mu_K$ lên $X_J$ bằng $\mu_J$. Độ đo trên $X$ nhận các biên $\mu_J$ được ký hiệu là $\bigotimes_{t \in D} \nu_t$ và được gọi là *tích của họ* $(\nu_t)_{t \in D}$. Khi các không gian $X_t$ là compắc, ta thu lại phép dựng của Ch. III, §4, No. 6.

### Bài tập {#int-ix-s4-exercises}

Xem [các bài tập của § 4](exercises/s4/).
