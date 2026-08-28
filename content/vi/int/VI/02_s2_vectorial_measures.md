---
book: int
book_title: Integration
chapter: VI
chapter_title: VECTORIAL INTEGRATION
section: 2
section_title: Vectorial measures . "
lang: vi
source: int-i-vi
book_pages: INT VI.18-INT VI.40, INT VI.62-INT VI.69
pdf_pages: 0409-0431, 0453-0460
extraction: ocr
subsections:
    - "no": 1
      title: Definition of a vectorial measure
      page: 18
      pdf_page: 409
    - "no": 2
      title: Integration with respect to a vectorial measure
      page: 20
      pdf_page: 411
    - "no": 3
      title: Majorizable vectorial measures
      page: 22
      pdf_page: 413
    - "no": 4
      title: Vectorial measures with base $\mu$
      page: 25
      pdf_page: 416
    - "no": 5
      title: The Dunford–Pettis theorem
      page: 27
      pdf_page: 418
    - "no": 6
      title: Dual of the space $L^1_F$ (F a separable Banach space)
      page: 32
      pdf_page: 423
    - "no": 7
      title: Integration of a vector-valued function with respect to a vectorial measure
      page: 33
      pdf_page: 424
    - "no": 8
      title: Complex measures
      page: 34
      pdf_page: 425
    - "no": 9
      title: Bounded complex measures⁶
      page: 37
      pdf_page: 428
    - "no": 10
      title: Image of a complex measure; induced complex measure; product of complex measures\footnote{Cf. Ch. V, §6, No. 4; Ch. IV, §5, No. 7 and Ch. V, §7; Ch. III, §4 and Ch. V, §8, Nos. 2–5.}
      page: 39
      pdf_page: 430
statements: 42
exercises: 18
content_sha256: b77bf541e3e518abb93045c369a3f6999436d7a2399899fc0be5bccd95724fc8
translated_from: content/en/int/VI/02_s2_vectorial_measures.md
source_content_sha256: b2224e3ba44c39c383bed9964f3920718fdcd7f727ed0fef49058dbd1cef0556
translation_model: gpt-5.4-mini
translation_run: translate-vi-d5713465
glossary_version: 34
glossary_terms_sha256: 35aad004b0b2a174d17d9a0fabe6d09fed206e8b47bc3227450c706b0ee26f84
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 2. ĐỘ ĐO VECTƠ

### 1. Định nghĩa về một độ đo vectơ

Định nghĩa về một độ đo đã nêu ở Ch. III, §1, No. 3 có thể được khái quát như sau:

#### Định nghĩa 1 {#int-vi-s2-def-1 .statement}

*Cho F là một không gian lồi địa phương Hausdorff trên R. Người ta gọi độ đo vectơ trên T với giá trị trong F là mọi ánh xạ tuyến tính liên tục của không gian $\mathcal{K}(T)$ vào F.*

Định nghĩa 1 cũng có thể phát biểu như sau: một độ đo vectơ trên T với giá trị trong F là một ánh xạ tuyến tính m của $\mathcal{K}(T)$ vào F sao cho, với mọi tập con compact K của T, hạn chế của m trên $\mathcal{K}(T, K)$ là liên tục đối với tôpô hội tụ đều. Nếu $f \in \mathcal{K}(T)$, người ta cũng viết $\int f dm$ hoặc $\int f(t)\,dm(t)$ thay cho $m(f)$. Các độ đo nhận giá trị trong $\mathbf{R}$ đôi khi được gọi là các độ đo *thực* (Ch. III, §1, No. 5) hoặc các độ đo *vô hướng* trên T.

#### Ví dụ {#int-vi-s2-n1-exa-1 .statement}

— 1) Ánh xạ đồng nhất của $\mathcal{K}(T)$ là một độ đo vectơ trên T với giá trị trong $\mathcal{K}(T)$.

2) *Cho H là một không gian Hilbert phức, $\mathcal{L}(H)$ là đại số chuẩn của các tự đồng cấu liên tục của H. Cho A là một đại số con của $\mathcal{L}(H)$, giao hoán, đóng, tự liên hợp và chứa ánh xạ đồng nhất; người ta chứng minh rằng tồn tại một không gian compact X và một đẳng cấu của đại số chuẩn A lên đại số $\mathcal{K}_\mathbf{C}(X) = \mathcal{C}_\mathbf{C}(X)$ gồm các hàm số phức liên tục trên X, được trang bị chuẩn $\|f\| = \sup_{x \in X} |f(x)|$. Đẳng cấu nghịch đảo, khi hạn chế trên $\mathcal{K}(X)$, là một độ đo vectơ m trên X, với giá trị trong $\mathcal{L}(H)$, sao cho $m(fg) = m(f)m(g)$.*_

#### Nhận xét {#int-vi-s2-n1-rem-1 .statement}

— 1) Để một ánh xạ tuyến tính m của $\mathcal{K}(T)$ vào F là một độ đo vectơ, điều kiện cần và đủ là, với mọi tập con compact K của T, ảnh qua m của quả cầu đơn vị $\|f\| \leq 1$ của $\mathcal{K}(T, K)$ bị chặn trong F. Do đó, khái niệm độ đo vectơ với giá trị trong F là như nhau đối với mọi tôpô lồi địa phương Hausdorff trên F có cùng các tập bị chặn, và đặc biệt đối với mọi tôpô tương thích với tính đối ngẫu giữa F và F' (TVS, IV, §1, No. 1, Mệnh đề 1).

2) Cho $T_1$ là một không gian compact địa phương, $F_1$ là một không gian lồi địa phương Hausdorff trên $\mathbf{R}$, u là một ánh xạ tuyến tính liên tục của $\mathcal{K}(T_1)$ vào $\mathcal{K}(T)$, và v là một ánh xạ tuyến tính liên tục của F vào $F_1$. Nếu m là một độ đo vectơ trên T với giá trị trong F, thì $v \circ m \circ u$ là một độ đo vectơ trên $T_1$ với giá trị trong $F_1$. Đặc biệt, nếu g là một hàm số số trị hữu hạn, liên tục trên T, thì $f \mapsto m(gf)$ là một độ đo vectơ trên T với giá trị trong F, được ký hiệu là $g \cdot m$; nếu h là một hàm số số trị hữu hạn, liên tục thứ hai trên T, thì $g \cdot (h \cdot m) = (gh) \cdot m$.

3) Vì không gian $\mathcal{K}(T)$ là giới hạn trực tiếp của các không gian Banach $\mathcal{K}(T, K)$, và đặc biệt là không gian đầy thùng (TVS, III, §4, No. 1, Hệ quả của Mệnh đề 2 và Hệ quả 3 của Mệnh đề 3), để một ánh xạ tuyến tính m của $\mathcal{K}(T)$ vào F là một độ đo vectơ, điều kiện cần và đủ là, với mọi $z' \in F'$, $z' \circ m$ là một độ đo vô hướng trên T (TVS, II, §6, No. 4, Mệnh đề 5 và IV, §1, No. 3, Mệnh đề 7).

4) Xét theo Nhận xét 1, Mệnh đề 1 của Ch. III, §2, No. 1 và chứng minh của nó vẫn đúng cho các độ đo vectơ. Do đó có thể định nghĩa *giá đỡ* của một độ đo vectơ m trên T là phần bù của tập mở lớn nhất $U \subset T$ sao cho hạn chế của m trên U là không.

### 2. Phép tích phân theo một độ đo vectơ

Cho $m$ là một độ đo vectơ trên $T$, với giá trị trong $F$. Với mọi $z' \in F'$, ánh xạ $z' \circ m$ là một độ đo vô hướng trên $T$, phụ thuộc tuyến tính vào $z'$. Nếu $f$ là một hàm số được xác định trên $T$, ta sẽ nói, theo lối nói rộng, rằng cặp $(f, m)$ có tính chất P nếu, với mọi $z' \in F'$, cặp $(f, |z' \circ m|)$ có tính chất P. Chẳng hạn, ta sẽ nói rằng $f$ *khả tích theo nghĩa thực chất đối với* $m$ nếu, với mọi $z' \in F'$, hàm số $f$ khả tích theo nghĩa thực chất đối với $|z' \circ m|$. Điều đó cũng tương đương với việc nói rằng $f$ khả tích theo nghĩa thực chất đối với từng trong các độ đo $(z' \circ m)^+$ và $(z' \circ m)^-$ (Ch. V, §2, No. 2, Hệ quả 2 của Mệnh đề 3).

#### Mệnh đề 1 {#int-vi-s2-prop-1 .statement}

*Cho $m$ là một độ đo vectơ trên $T$ với giá trị trong $F$, $f$ là một hàm số vô hướng trên $T$ gần như khả tích đối với $m$. Ánh xạ*
$$
z' \mapsto \int f \, d(z' \circ m)^+ - \int f \, d(z' \circ m)^-
$$
*là một dạng tuyến tính trên $F'$*.

Ký hiệu ánh xạ này là $\Phi$, ta hiển nhiên có $\Phi(\lambda z') = \lambda \Phi(z')$ với mọi $\lambda \in \mathbf{R}$. Mọi việc quy về chứng minh rằng $\Phi(y' + z') = \Phi(y') + \Phi(z')$. Đặt $\mu = |y' \circ m| + |z' \circ m|$; theo định lý Lebesgue–Nikodym, ta có thể viết $y' \circ m = g \cdot \mu$ và $z' \circ m = h \cdot \mu$, trong đó $g$ và $h$ là hai hàm số vô hướng bị chặn và địa phương $\mu$-khả tích (Ch. V, §5, No. 5, Định lý 2); mặt khác, $(y' \circ m)^+ = g^+ \cdot \mu$ và $(y' \circ m)^- = g^- \cdot \mu$, và các quan hệ tương tự đúng khi thay $y'$ bởi $z'$ (tương ứng $y' + z'$) và $g$ bởi $h$ (tương ứng $g + h$). Vì vậy, hiển nhiên $f$ gần như khả tích đối với $\mu$ (Ch. V, §2, No. 2, Hệ quả 1 của Mệnh đề 3), và quan hệ cần chứng minh quy về $(g + h)^+ - (g + h)^- = (g^+ - g^-) + (h^+ - h^-)$, điều này hiển nhiên.

#### Định nghĩa 2 {#int-vi-s2-def-2 .statement}

*Cho $m$ là một độ đo vectơ trên $T$ với giá trị trong $F$, $f$ là một hàm số vô hướng trên $T$ gần như khả tích đối với $m$. Người ta gọi tích phân của $f$ đối với $m$, và ký hiệu bởi $m(f)$ hay $\int f \, dm$ hay cũng $\int f(t) \, dm(t)$, phần tử của ${F'}^*$ được xác định bởi*

$$
\langle z', \int f \, dm \rangle = \int f \, d(z' \circ m)^+ - \int f \, d(z' \circ m)^-.
$$

Ta nhận thấy rằng nếu $f \in \mathcal{K}(T)$, thì phần tử $\int f \, dm$ được định nghĩa như vậy trùng với phần tử cũng được ký hiệu như thế ở No. 1, vì khi đó vế thứ hai của (1) là $\int f \, d(z' \circ m) = z'(m(f))$ theo định nghĩa. Hơn nữa, nếu đặc biệt áp dụng Định nghĩa 2 cho trường hợp $F = \mathbf{R}$, ta thấy rằng với mọi $z' \in F'$, $f$ gần như khả tích đối với độ đo thực $z' \circ m$, và vế thứ hai của (1) có thể viết là $\int f d(z' \circ m)$.

Giả sử nay $f$ gần như khả tích đối với $m$, và lấy $z' \in F'$. Đặt $\mu = |z' \circ m|$; theo định lý Lebesgue–Nikodym, ta có thể viết $z' \circ m = g \cdot \mu$, trong đó $g$ địa phương $\mu$-khả tích và $\|g\| \leq 1$, và chứng minh của Mệnh đề 1 cho thấy rằng $\int f d(z' \circ m) = \int fg d\mu$. Do đó,

$$
\left| \int f d(z' \circ m) \right| \leq \int |f| d|z' \circ m|.
$$

Rõ ràng là tập hợp các hàm số vô hướng hữu hạn khả tích theo nghĩa thiết yếu đối với $m$ là một không gian vectơ trên $\mathbf{R}$; ta sẽ ký hiệu không gian này bởi $\mathcal{L}(m)$, được trang bị tôpô lồi địa phương thô nhất làm cho mọi dạng tuyến tính $f \mapsto \int f d(z' \circ m)$, với $z'$ chạy qua $F'$, đều liên tục. Chú ý rằng nói chung không gian lồi địa phương $\mathcal{L}(m)$ *không Hausdorff*.

#### Ví dụ {#int-vi-s2-n2-exa-1 .statement}

— Ta lấy cho $m$ ánh xạ đồng nhất của $\mathscr{K}(T)$ lên chính nó. Vì không gian đối ngẫu của $\mathscr{K}(T)$ là không gian $\mathscr{M}(T)$ của các độ đo vô hướng trên $T$, các hàm $f \in \mathcal{L}(m)$ là những hàm khả tích theo nghĩa thiết yếu đối với *mọi* độ đo vô hướng $\mu$ (xem Bài tập 1), và tích phân $\int f dm$ là dạng tuyến tính $\mu \mapsto \int f d\mu$ trên $\mathscr{M}(T)$. Không thể có $\int f d\mu = 0$ với mọi độ đo $\mu \in \mathscr{M}(T)$ trừ khi $f = 0$, như thấy khi lấy $\mu = \varepsilon_t$, với $t$ tùy ý trong $T$; nói cách khác, ánh xạ $f \mapsto \int f dm$ là một *đơn ánh* từ $\mathcal{L}(m)$ vào đối ngẫu đại số của $\mathscr{M}(T)$, và nó mở rộng ánh xạ đồng nhất của $\mathscr{K}(T)$. Do đó, quan hệ $\int f dm \in F = \mathscr{K}(T)$ tương đương với $f \in \mathscr{K}(T)$.

Cho $u$ là một ánh xạ tuyến tính liên tục của $F$ vào một không gian lồi địa phương Hausdorff $G$, và cũng ký hiệu bằng $u$ phép mở rộng của nó bằng song chuyển vị thành một ánh xạ tuyến tính của ${F'}^*$ vào ${G'}^*$ (\S 1, No. 1). Với quy ước này:

#### Mệnh đề 2 {#int-vi-s2-prop-2 .statement}

*Mọi hàm số vô hướng* $f$ *khả tích theo nghĩa thiết yếu đối với* $m$ *đều khả tích theo nghĩa thiết yếu đối với* $u \circ m$, *và* $\int f d(u \circ m) = u(\int f dm)$.

Mệnh đề là hiển nhiên, do đẳng thức $y' \circ u \circ m = {}^t u(y') \circ m$ với mọi $y \in G'$.

Nói chung, nếu $f \in \mathcal{L}(m)$, thì tích phân $\int f dm$ thuộc ${F'}^*$ nhưng không thuộc $F$ (xem *Ví dụ* trên). Tuy nhiên:

#### Mệnh đề 3 {#int-vi-s2-prop-3 .statement}

*Nếu ảnh qua* $m$ *của tập hợp các* $f \in \mathscr{K}(T)$ *sao cho* $\sup_{t \in T} |f(t)| \leq 1$ *là tương đối compact yếu trong* $F$, *thì* $\int f dm \in F$ *với mọi hàm số vô hướng bị chặn* $f$ *khả tích theo nghĩa thiết yếu đối với* $m$.

Cho $A$ là tập hợp các $f \in \mathcal{L}(m)$ sao cho $\sup_{t \in T} |f(t)| \leq 1$, và cho $B = A \cap \mathscr{K}(T)$; theo giả thiết, $m(B)$ là tương đối compact yếu trong $F$, do đó đủ để chỉ ra rằng $m(A)$ được chứa trong bao đóng (trong ${F'}^*$) của $m(B)$ đối với tôpô $\sigma({F'}^*, F')$; vì $m(B)$ là lồi và cân bằng, đủ để chứng minh rằng đối cực của $m(B)$ trong $F'$ được chứa trong đối cực của $m(A)$ (TVS, II, §6, No. 3, ĐL. 1). Bây giờ, để một dạng tuyến tính $z' \in F'$ thuộc $(m(B))^\circ$, cần và đủ rằng $|\langle z', m(g)\rangle| = |\int g d(z'\circ m)| \leq 1$ đối với mọi hàm $g \in B$, điều đó có nghĩa là độ đo vô hướng $|z'\circ m|$ bị chặn và có chuẩn $\leq 1$ (Ch. III, §1, No. 8); nhưng theo (2) điều kiện sau suy ra rằng $|\langle z', m(f)\rangle| \leq 1$ đối với mọi hàm $f \in A$, suy ra $z' \in (m(A))^\circ$.

#### Hệ quả 1 {#int-vi-s2-prop-3-cor-1 .statement}

*Nếu, với mọi tập con compact K của T, ảnh của tập hợp các $f \in \mathcal{H}(T, K)$ sao cho $\sup_{t \in T} |f(t)| \leq 1$ qua m là tương đối compact yếu trong F, thì $\int f dm \in F$ đối với mọi hàm $f \in \mathcal{L}(m)$ bị chặn và có giá compact, và $\int f dm \in F''$ đối với mọi hàm $f \in \mathcal{L}(m)$.*

Mệnh đề đầu tiên có thể suy ra ngay lập tức từ Mệnh đề 3: nếu $f$ bị chặn và có giá compact, và nếu U là một lân cận mở tương đối compact của giá của $f$, thì phần hạn chế của $m$ lên không gian con $\mathcal{H}(U)$ là một độ đo $m_U$ trên U thỏa mãn các điều kiện của Mệnh đề 3, và $\int f dm_U = \int f dm$ (Ch. V, §7, No. 1, ĐL. 1), do đó $\int f dm \in F$.

Now let $f$ be any element of $\mathcal{L}(m)$; for every compact subset K of T and every integer $n > 0$, let $f_{n,K}$ be the numerical function on T defined as follows: if $t \notin K$, $f_{n,K}(t) = 0$; if $t \in K$ and $|f(t)| \leq n$, $f_{n,K}(t) = f(t)$; finally, if $t \in K$ and $|f(t)| > n$, $f_{n,K}(t) = nf(t)/|f(t)|$. It is clear that for every $t \in T$, $f(t)$ is the limit of $f_{n,K}(t)$ with respect to the product filter of the Fréchet filter by the section filter of the (increasing directed) ordered set of compact subsets of T. Since $|f_{n,K}| \leq |f|$, it follows from Lebesgue’s theorem and Prop. 10 of Ch. V, §1, No. 3, applied to each scalar measure $|z'\circ m|$, that $f_{n,K}$ converges to $f$ in $\mathcal{L}(m)$ with respect to the preceding filter. Consequently, the integral $\int f dm$ is in the closure in ${F'}^*$ (for the topology $\sigma({F'}^*, F')$) of the set M of $m(f_{n,K})$. But the first part of the corollary shows that $M \subset F$, and, on the other hand, for every $z' \in F'$ one has $|\langle z', m(f_{n,K})\rangle| \leq \int |f| d|z'\circ m|$, which shows that M is bounded in $F_\sigma$, hence also in F (TVS, IV, §1, No. 1, Prop. 1). Lemma 1 of §1, No. 2 therefore shows that $\int f dm \in F''$.

#### Hệ quả 2 {#int-vi-s2-prop-3-cor-2 .statement}

*Nếu F là bán phản xạ, thì $\int f dm \in F$ với mọi hàm số vô hướng $f$ khả tích thiết yếu đối với $m$.*

### 3. Các độ đo vectơ khả trù

Cho $q$ là một nửa chuẩn nửa liên tục dưới trên F. Ta sẽ ký hiệu $A'_q$ là tập hợp các $z' \in F'$ sao cho $|\langle z', x\rangle| \leq q(x)$ với mọi $x \in F$. Đây là

phần đối cực trong $F'$ của tập hợp các $x \in F$ sao cho $q(x) \leq 1$; với mọi $x \in F$,
$$
q(x) = \sup_{z' \in A'_q} |\langle x, z' \rangle|.
$$

#### Định nghĩa 3 {#int-vi-s2-def-3 .statement}

*Cho $m$ là một độ đo vectơ trên T nhận giá trị trong F. Nếu $q$ là một nửa chuẩn nửa liên tục dưới trên F, thì nói rằng $m$ là *q-khả trù* nếu tồn tại một độ đo dương $\mu$ sao cho $|z' \circ m| \leq \mu$ với mọi $z' \in A'_q$; cận trên đúng của các độ đo $|z' \circ m|$ khi $z'$ chạy trong $A'_q$ (Ch. III, §2, No. 4, Th. 3) được ký hiệu là $q(m)$. Nói rằng $m$ là *khả trù* nếu nó là *q-khả trù* với mọi nửa chuẩn liên tục trên F.*

Nếu $m$ và $m'$ đều *q-khả trội*, thì hiển nhiên $m + m'$ cũng *q-khả trội* và
$$
q(m + m') \leq q(m) + q(m').
$$

Khi $F$ là một không gian có chuẩn, với chuẩn ký hiệu $|x|$, nói rằng $m$ là khả trội do đó có nghĩa là các độ đo $|z' \circ m|$, với $|z'| \leq 1$, đều được chặn trên$^1$ bởi cùng một độ đo dương; rồi người ta ký hiệu supremum của họ các độ đo này là $|m|$.

Nếu $F = \mathbf{R}$, thì độ đo $|m|$ tương ứng với chuẩn Euclid $|x|$ trên $\mathbf{R}$ trùng với độ đo được ký hiệu bởi $|m|$ trong Chương III, §1, No. 5.

#### Mệnh đề 4 {#int-vi-s2-prop-4 .statement}

*Cho* $(F_i)_{1 \leq i \leq n}$ *là một họ hữu hạn các không gian lồi địa phương Hausdorff, $F = \prod_{i=1}^n F_i$ là tích của chúng, $q_i$ ($1 \leq i \leq n$) *là một nửa chuẩn bán liên tục dưới* trên $F_i$, *và* $q$ *là nửa chuẩn trên* $F$ *được xác định bởi* $q(x_1, \ldots, x_n) = \sum_{i=1}^n q_i(x_i)$. *Nếu* $m_i$ ($1 \leq i \leq n$) *là một độ đo vectơ trên* $T$ *nhận giá trị trong* $F_i$ *và là* $q_i$*-khả trội*, *thì độ đo* $m = (m_1, \ldots, m_n)$ *nhận giá trị trong* $F$ *là* *q-khả trội*.

Vì, không gian đối ngẫu $F'$ có thể được đồng nhất với $\prod_{i=1}^n F_i'$, sao cho nếu $x = (x_i) \in F$, $z' = (z_i') \in F'$, thì $\langle x, z' \rangle = \sum_{i=1}^n \langle x_i, z_i' \rangle$. Nếu $|\langle x, z' \rangle| \leq q(x)$ với mọi $x \in F$, thì đặc biệt $|\langle x_i, z_i' \rangle| \leq q_i(x_i)$ đối với $1 \leq i \leq n$, và điều ngược lại hiển nhiên, điều đó cho thấy rằng tập $A'_q$ là tích của các $A'_{q_i}$. Vì theo giả thiết $|z_i' \circ m_i| \leq q_i(m_i)$ với $z_i' \in A'_{q_i}$, suy ra rằng
$$
|z' \circ m| \leq \sum_{i=1}^n |z_i' \circ m_i| \leq \sum_{i=1}^n q_i(m_i)
$$
với mọi $z' \in A'_q$, điều đó chứng minh mệnh đề.

$^1$ Được chặn trên.

#### Hệ quả {#int-vi-s2-n3-cor-1 .statement}

— *Nếu không gian F là hữu hạn chiều, thì mọi độ đo vectơ m nhận giá trị trong F đều là khả trội. Để một hàm số thực khả tích thực chất đối với m, cần và đủ là nó khả tích thực chất đối với |m|* (trong đó |x| ký hiệu một chuẩn bất kỳ trên F).

#### Mệnh đề 5 {#int-vi-s2-prop-5 .statement}

— *Cho q là một nửa chuẩn bán liên tục dưới trên F. Cho m là một độ đo q-khả trội, và cho f là một hàm số khả tích thực chất đối với m và sao cho $\int f dm \in F$. Khi đó*

$$
q\left( \int f dm \right) \leq \int^\bullet |f| dq(m).
$$

Vì,

$$
q\left( \int f dm \right) = \sup_{z' \in A'_q} \left| \langle z', \int f dm \rangle \right| \leq \sup_{z' \in A'_q} \int |f| d|z' \circ m| \leq \int^\bullet |f| dq(m)
$$

nhờ (1) và hệ thức $|z' \circ m| \leq q(m)$ với $z' \in A'_q$.

#### Mệnh đề 6 {#int-vi-s2-prop-6 .statement}

— *Cho F là một không gian lồi địa phương Hausdorff gần đầy đủ, m là một độ đo khả trội trên T nhận giá trị trong F. Nếu f là một hàm số thực khả tích thực chất đối với mọi độ đo q(m) (trong đó q chạy trên tập các nửa chuẩn liên tục trên F), thì f khả tích thực chất đối với m, và $\int f dm \in F$.

Ta sẽ sử dụng kết quả phụ sau đây. Cho $(\mu_\iota)_{\iota \in I}$ là một họ các độ đo dương tăng và có hướng trên T. Ký hiệu $\mathcal{L}^1((\mu_\iota)_{\iota \in I})$ là không gian vectơ của các hàm số thực hữu hạn trên T, hầu như $\mu_\iota$-khả tích với mọi $\iota \in I$, được trang bị tôpô được xác định bởi các nửa chuẩn $f \mapsto \mu_\iota(|f|)$ ($\iota \in I$). Ký hiệu $\mathcal{L}_0$ là không gian con tuyến tính của $\mathcal{L}^1((\mu_\iota)_{\iota \in I})$ sinh bởi các tích $g \varphi_K$, trong đó g chạy trên tập các hàm số thực hữu hạn liên tục trên T, và K chạy trên tập các tập con compact của T.

#### Bổ đề 1 {#int-vi-s2-lem-1 .statement}

— *Khi $\mathcal{L}_0$ và $\mathcal{K}(T)$ được trang bị tôpô cảm sinh bởi tôpô của $\mathcal{L}^1((\mu_\iota)_{\iota \in I})$:
a) mỗi phần tử của $\mathcal{L}_0$ thuộc bao đóng của một tập con bị chặn nào đó của $\mathcal{K}(T)$;
b) mỗi phần tử của $\mathcal{L}^1((\mu_\iota)_{\iota \in I})$ thuộc bao đóng của một tập con bị chặn nào đó của $\mathcal{L}_0$.*

Để chứng minh a), ta có thể chỉ xét trường hợp một phần tử có dạng $f = g \varphi_K$ ($g \in \mathcal{C}(T)$, K compact trong T). Điều đó là hiển nhiên (nhờ định lý Urysohn) rằng $f$ thuộc bao đóng của tập B gồm các hàm có dạng $gh$, trong đó h chạy trên tập các ánh xạ liên tục của T vào $[0,1]$ bằng 1 trên K và bằng 0 trên phần bù của một lân cận compact cố định H của K. Hơn nữa, tập B bị chặn, vì $\mu_\iota(|gh|) \leq \mu_\iota(|f\varphi_H|)$ với mọi hàm h có các tính chất trên.

Bây giờ ta chứng minh b); ta có thể chỉ xét trường hợp một phần tử $f \geq 0$ của $\mathcal{L}^1((\mu_\iota)_\iota \in I)$. Với mọi $\iota \in I$ và mọi $\varepsilon > 0$, tồn tại một tập con compact $K(\iota, \varepsilon)$ của T sao cho hạn chế của $f$ lên $K(\iota, \varepsilon)$ là liên tục và $|\mu_\iota(|f - f\varphi_{K(\iota, \varepsilon)}|)| \leq \varepsilon$. Rõ ràng $f$ thuộc bao đóng của tập C gồm các $f\varphi_{K(\iota, \varepsilon)}$ (với $\iota \in I,\ \varepsilon > 0$). Nhờ định lý Urysohn, tập C được chứa trong $\mathcal{L}_0$; hơn nữa, tập này bị chặn, vì $\mu_\kappa(f\varphi_{K(\iota, \varepsilon)}) \leq \mu_\kappa(f)$ với mọi $\iota \in I,\ \kappa \in I$ và $\varepsilon > 0$.

Bây giờ ta chứng minh Mệnh đề 6: với mọi hàm $g \in \mathscr{K}(T)$ và mọi nửa chuẩn liên tục q trên F, $q\left( \int g\,dm \right) \leq \int |g|\,d(q(m))$ (Mệnh đề 5), điều này suy ra rằng ánh xạ $g \mapsto \int g\,dm$ từ $\mathscr{K}(T)$ vào F là liên tục khi $\mathscr{K}(T)$ được trang bị tôpô cảm sinh bởi tôpô của $\mathcal{L}^1((q(m))_{q \in Q})$ (Q là tập các nửa chuẩn liên tục trên F). Do đó, theo bổ đề trước và Mệnh đề 10 của TVS, III, §1, No. 6, ánh xạ này có thể được kéo dài liên tục, trước hết thành một ánh xạ tuyến tính liên tục $v_0$ từ $\mathcal{L}_0$ vào F, rồi thành một ánh xạ tuyến tính liên tục $v$ từ $\mathcal{L}^1((q(m))_{q \in Q})$ vào F. Hơn nữa, với mọi $z' \in F'$ thì quan hệ $\langle z', v(f) \rangle = \int f\,d(z' \circ m)$ đúng, theo định nghĩa của $v$, với mọi $f \in \mathscr{K}(T)$; vì $|z' \circ m| \leq q(m)$ với $q(z) = |\langle z', z \rangle|$, ánh xạ $f \mapsto \int f\,d(z' \circ m)$ là liên tục trên $\mathcal{L}^1((q(m))_{q \in Q})$, do đó lại theo tính liên tục, quan hệ $\langle z', v(f) = \int f\,d(z' \circ m)$ đúng với mọi hàm số $f \in \mathcal{L}^1((q(m))_{q \in Q})$. Suy ra $v(f) = \int f\,dm$, điều này hoàn tất chứng minh.

### 4. Độ đo vectơ với cơ sở $\mu$

#### Định nghĩa 4 {#int-vi-s2-def-4 .statement}

*Cho $\mu$ là một độ đo dương trên T. Một độ đo vectơ $m$ trên T, với giá trị trong F, được gọi là một độ đo có cơ sở $\mu$ nếu tồn tại một ánh xạ $f$ của T vào F, khả tích địa phương theo vô hướng theo $\mu$, sao cho $m(g) = \int gf\,d\mu$ với mọi hàm $g \in \mathscr{K}(T)$. Khi đó ta nói rằng $f$ là một mật độ của $m$ đối với $\mu$, và viết $m = f \cdot \mu$.*

Ngay lập tức thấy rằng nếu $f_1$ và $f_2$ là hai mật độ của $m$ đối với $\mu$, thì $f_1 - f_2$ là vô hướng địa phương $\mu$-không đáng kể (Ch. V, §5, No. 3, Hệ quả 2 của Mệnh đề 3); hãy nhớ rằng nói chung điều này không suy ra $f_1 - f_2$ bằng không ở khắp nơi địa phương hầu như mọi chỗ (cf. §1, Bài tập 12 và No. 1, *Nhận xét 2*).

Cho $m$ là một độ đo có cơ sở $\mu$, với mật độ $f$. Để một hàm số $g$ là khả tích theo nghĩa thiết yếu đối với $m$, điều kiện cần và đủ là $gf$ phải khả tích theo nghĩa thiết yếu theo vô hướng theo $\mu$ (Ch. V, §5, No. 3, Định lý 1).

#### Mệnh đề 7 {#int-vi-s2-prop-7 .statement}

— Cho $f$ là một ánh xạ khả tích địa phương theo vô hướng đối với một độ đo dương $\mu$ trên $T$, sao cho, với mọi hàm $g \in \mathcal{K}(T)$, ta có $\int gf\,d\mu \in F$. Khi đó ánh xạ $g \mapsto \int gf\,d\mu$ của $\mathcal{K}(T)$ vào $F$ là một độ đo vectơ trên $T$, với cơ sở $\mu$ và mật độ $f$ đối với $\mu$.

Đối với (No. 1, Nhận xét 3), chỉ cần chứng minh rằng, đặt $m(g) = \int gf\,d\mu$, thì $z' \circ m$ là một độ đo vô hướng với mọi $z' \in F'$. Nhưng vì $z'(m(g)) = \int g\langle z', f \rangle\,d\mu$, ta có $z' \circ m = \langle z', f \rangle \cdot \mu$, do đó mệnh đề của chúng ta.

#### Mệnh đề 8 {#int-vi-s2-prop-8 .statement}

— Cho $\mu$ là một độ đo dương trên $T$, $m$ là một độ đo trên $T$ nhận giá trị trong $F$, với cơ sở $\mu$ và mật độ $f$ đối với $\mu$. Cho $q$ là một nửa chuẩn nửa liên tục dưới trên $F$.

a) Nếu, với mọi tập con compact $K$ của $T$, tích phân trên $\int_K^*(q \circ f)\,d\mu$ là hữu hạn, thì $m$ là $q$-đại chặn được.

b) Nếu $m$ là $q$-khả trội, thì $q(m)$ có cơ sở $\mu$; nếu thêm rằng $f$ là $\mu$-khả đo như một ánh xạ từ $T$ vào $F_\sigma$, thì $q \circ f$ khả tích địa phương theo $\mu$ và $q(m) = (q \circ f) \cdot \mu$.

a) Với mọi tập con hữu hạn $J$ của $A'_q$, ký hiệu $\lambda_J$ là cận trên đúng của các độ đo $|z' \circ m|$, với $z'$ chạy qua $J$; nếu $g_J = \sup_{z' \in J} |\langle z', f \rangle|$ thì $\lambda_J = g_J \cdot \mu$ (Ch. V, §5, No. 2, Mệnh đề 2). Với mọi tập con mở tương đối compact $U$ của $T$, ký hiệu $\lambda_{J,U}$ là hạn chế của $\lambda_J$ lên $U$; trước hết hãy chứng minh rằng khi $J$ chạy qua tập có hướng $\mathfrak{F}$ của các tập con hữu hạn của $A'_q$, họ $(\lambda_{J,U})$ bị chặn trên trong $\mathcal{M}(U)$. Thật vậy, với mọi hàm $h \geq 0$ trong $K(U)$,

$$
\int h\,d\lambda_{J,U} = \int hg_J\,d\mu \leq \int^*(q \circ f)h\,d\mu \leq \|h\| \int_U^*(q \circ f)\,d\mu,
$$

do đó mệnh đề của chúng ta (Ch. II, §2, No. 2). Ký hiệu $\nu_U$ là cận trên đúng của họ các độ đo này trong $\mathcal{M}(U)$. Nếu $U'$ là một tập con mở tương đối compact thứ hai của $T$ sao cho $U \subset U'$, thì $\nu_U$ là hạn chế của $\nu_{U'}$ lên $U$, điều này suy ra ngay từ biểu thức của cận trên đúng của một tập có hướng tăng các độ đo (Ch. II, §2, No. 2) và từ sự kiện rằng $\lambda_{J,U}$ là hạn chế lên $U$ của $\lambda_{J,U'}$. Do đó tồn tại đúng một độ đo dương $\nu$ mà hạn chế của nó lên mỗi $U$ là $\nu_U$ (Ch. III, §2, No. 1, Mệnh đề 1), và hiển nhiên $\nu = q(m)$.

b) Vì các độ đo $\lambda_J$ có cơ sở $\mu$, nên cận trên đúng $q(m)$ của chúng cũng có cơ sở đó (Ch. V, §5, No. 5, Định lý 2). Nếu $f$ là $\mu$-khả đo đối với tôpô $\sigma(F, F')$ trên $F$, thì từ các định nghĩa suy ra ngay rằng ánh xạ $g : t \mapsto (g_J(t))_{J \in \mathfrak{F}}$ của $T$ vào không gian tích $\mathbf{R}^\mathfrak{F}$ là $\mu$-khả đo. Hạn chế của $q \circ f = \sup_{J \in \mathfrak{F}} g_J$ trên mọi tập con compact của $T$ mà trên đó $g$ liên tục là nửa liên tục dưới; do đó $q \circ f$ là $\mu$-khả đo (Ch. IV, §5, No. 5, Hệ quả của Mệnh đề 8 và No. 10, Mệnh đề 15). Cho $K$ là một tập con compact của T; nó có một phân hoạch gồm một tập $\mu$-không đáng kể và một dãy $(K_n)$ các tập compact mà trên đó $g$ liên tục. Khi đó $\int_{K_n}^*(q \circ f)\, d\mu = \sup_J \int_{K_n} g_J\, d\mu \leq \int_{K_n} dq(m)$ với mọi $n$ (Ch. IV, §1, No. 1, Định lý 1 và Ch. V, §7, No. 1, Mệnh đề 1), do đó $\int_K^*(q \circ f)\, d\mu = \sum_n \int_{K_n}^*(q \circ f)\, d\mu \leq \int_K dq(m)$. Nhưng điều này chứng tỏ rằng $q \circ f$ khả tích địa phương theo $\mu$ và rằng $\lambda_J \leq (q \circ f) \cdot \mu \leq q(m)$ với mọi $J \in \mathcal{F}$; do đó, theo định nghĩa, $q(m) = (q \circ f) \cdot \mu$.

#### Nhận xét {#int-vi-s2-n4-rem-1 .statement}

Giả sử rằng trong $A_q'$ có một tập con đếm được D trù mật đối với $\sigma(F', F)$; khi đó, hàm $q \circ f$ luôn luôn là $\mu$-khả đo, vì $q(f(t)) = \sup_{z' \in D} |\langle z', f(t) \rangle|$ (Ch. IV, §5, No. 4, Hệ quả 1 của Định lý 2). Khi đó, với mọi tập con compact K của T, $\int_K^*(q \circ f)\, d\mu = \sup_J \int_K g_J\, d\mu$, trong đó J chạy qua tập có hướng đếm được gồm các tập con hữu hạn của D (Ch. IV, §1, No. 1, Hệ quả của Định lý 3); do đó, ta thấy rằng trong trường hợp này điều kiện $\int_K^*(q \circ f)\, d\mu < +\infty$ với mọi tập con compact K của T là cần và đủ để m có thể major hóa bởi q.

#### Mệnh đề 9 {#int-vi-s2-prop-9 .statement}

— *Cho F là một không gian Banach hữu hạn chiều. Mọi độ đo m trên T nhận giá trị trong F đều là một độ đo có cơ sở $|m|$. Nếu $m = f \cdot |m|$, thì $|f(t)| = 1$ hầu khắp địa phương đối với $|m|$. Để m có cơ sở $\mu$, điều kiện cần và đủ là $|m|$ có cơ sở $\mu$, và nếu $m = g \cdot \mu$ thì $|m| = |g| \cdot \mu$.

Hãy lấy $(e_i)_{1 \leq i \leq n}$ và $(e'_i)_{1 \leq i \leq n}$ là các cơ sở đối ngẫu của F và F' (A, II, §2, No. 6) với $|e'_i| = 1$ với mọi i. Khi đó $|e'_i \circ m| \leq |m|$ với mọi chỉ số i, do đó (Ch. V, §5, No. 5, Định lý 2) $e'_i \circ m = h_i \cdot |m|$, trong đó $h_i$ bị chặn và $|m|$-khả đo. Đặt $h = \sum_{i=1}^n h_i \cdot e_i$, ta có $m = h \cdot |m|$. Nếu $m = f \cdot |m|$, Mệnh đề 8 cho thấy rằng $|m| = |f| \cdot |m|$, do đó $|f(t)| = 1$ hầu khắp địa phương đối với $|m|$ (Ch. V, §5, No. 3, Hệ quả 2 của Mệnh đề 3). Khẳng định cuối cùng suy ra ngay từ Mệnh đề 8.

#### Nhận xét {#int-vi-s2-n4-rem-2 .statement}

Nếu $z = \sum_{i=1}^n z_i e_i$ thì $\psi(z_1, \ldots, z_n) = |z|$ là một hàm liên tục thuần nhất dương trên $\mathbf{R}^n$. Đặt $\mu_i = e'_i \circ m = h_i \cdot |m|$, theo định nghĩa (Ch. V, §5, No. 9) $\psi(\mu_1, \ldots, \mu_n) = \psi(h_1, \ldots, h_n) \cdot |m| = |h| \cdot |m| = |m|$.

### 5. Định lý Dunford–Pettis

Cho $\mu$ là một độ đo dương trên T. Một độ đo vectơ m trên T, nhận giá trị trong F, được gọi là *có cơ sở theo nghĩa vô hướng* $\mu$ (hay có cơ sở $\mu$ theo nghĩa vô hướng) nếu, với mọi $z' \in F'$, độ đo vô hướng $z' \circ m$ có cơ sở $\mu$. Nếu một độ đo vectơ $m$ nhận giá trị trong $F$ có cơ sở $\mu$, thì nó có cơ sở $\mu$ theo nghĩa vô hướng: vì, nếu $m = f \cdot \mu$ thì $z' \circ m = \langle z', f \rangle \cdot \mu$ với mọi $z' \in F'$. Nhưng tồn tại những độ đo vectơ có cơ sở theo nghĩa vô hướng $\mu$ mà không có cơ sở $\mu$ (Bài tập 17), và, mặt khác, tồn tại những độ đo vectơ không có cơ sở theo nghĩa vô hướng là $\nu$ đối với bất kỳ độ đo dương $\nu$ nào; tuy nhiên, lưu ý rằng mọi độ đo có thể trội hóa $m$ nhận giá trị trong một không gian chuẩn đều có cơ sở theo nghĩa vô hướng là $|m|$, nhờ định lý Lebesgue–Nikodym.

#### Ví dụ {#int-vi-s2-n5-exa-1 .statement}

— Ta hãy lấy $m$ là ánh xạ đồng nhất của $\mathcal{H}(T)$. Nói rằng $m$ có cơ sở $\mu$ theo nghĩa vô hướng có nghĩa là mọi độ đo thực trên $T$ đều có cơ sở $\mu$. Đặc biệt, độ đo điểm $\varepsilon_t$ ($t \in T$) phải có cơ sở $\mu$, điều này đòi hỏi $\mu(\{t\}) > 0$ với mọi $t \in T$, và suy ra đặc biệt rằng mọi tập con compact của $T$ đều đếm được.

Trong số này chúng ta sẽ chứng minh một kết quả tổng quát hóa một trong các hệ quả của định lý Lebesgue–Nikodym, cụ thể là, đối ngẫu của $L^1(\mu)$ là $L^\infty(\mu)$ (Ch. V, §5, No. 8, Định lý 4), và cho một điều kiện đủ để một độ đo vectơ có cơ sở theo nghĩa vô hướng $\mu$ có cơ sở $\mu$.

Cho $\pi$ là ánh xạ chính tắc của $\mathcal{L}^\infty(\mu)$ lên $L^\infty(\mu)$. Ta sẽ nói rằng một không gian con tuyến tính $G$ của $L^\infty$ có *tính chất nâng* nếu tồn tại một ánh xạ tuyến tính $\rho$ từ $G$ vào $\mathcal{L}^\infty(\mu)$ (gọi là một *phép nâng* của $G$) sao cho $\pi \circ \rho$ là ánh xạ đồng nhất trên $G$ và $|\rho(f)(t)| \leq N_\infty(f)$ với mọi $t \in T$ và $f \in G$.

Người ta chứng minh rằng nếu $\mu$ là độ đo Lebesgue trên $\mathbf{R}^n$, thì toàn bộ không gian $L^\infty(\mathbf{R}^n, \mu)$ có tính chất nâng (Bài tập 18).

#### Bổ đề 2 {#int-vi-s2-lem-2 .statement}

*Mọi không gian con tách được* $G$ *của không gian Banach* $L^\infty(T, \mu)$ *đều có tính chất nâng*.

#### Định nghĩa 5 {#int-vi-s2-def-5 .statement}

Theo giả thiết, tồn tại một tập con đếm được trù mật $H$ của $G$ là một không gian con tuyến tính đối với trường số hữu tỉ $\mathbf{Q}$; hãy lấy $(h_n)$ làm một cơ sở (đếm được) của $H$ trên $\mathbf{Q}$. Với mọi số nguyên $n$, hãy lấy $h'_n$ là một phần tử của $\mathcal{L}^\infty$ sao cho $\pi(h'_n) = h_n$, và hãy lấy $\rho'$ là ánh xạ $\mathbf{Q}$-tuyến tính của $H$ vào $\mathcal{L}^\infty$ được xác định bởi $\rho'(h_n) = h'_n$; hiển nhiên $\pi \circ \rho'$ là đồng nhất trên $H$. Hơn nữa, với mọi $h \in H$ ta có $|\rho'(h)(t)| \leq N_\infty(h)$ trừ tại các điểm $t$ của một tập cục bộ không đáng kể $A(h)$. Gọi $A$ là hợp của các $A(h)$ khi $h \in H$, vốn cũng cục bộ không đáng kể. Với mọi $h \in H$, ký hiệu $\rho(h)$ là hàm $h'' \in \mathcal{L}^\infty$ sao cho $h''(t) = \rho'(h)(t)$ nếu $t \notin A$, và $h''(t) = 0$ nếu $t \in A$. Hiển nhiên $\rho$ là một ánh xạ $\mathbf{Q}$-tuyến tính của $H$ vào không gian con $\mathcal{B}$ của các hàm bị chặn trong $\mathcal{L}^\infty$, sao cho $\pi \circ \rho$ là đồng nhất trên $H$ và sao cho $|\rho(h)(t)| \leq N_\infty(h)$ với mọi $h \in H$ và $t \in T$. Vì $\mathcal{B}$ là một không gian Banach đối với chuẩn $\|f\| = \sup_{t \in T} |f(t)|$ (Ch. IV, §5, No. 4, Th. 2), $\rho$ có thể được mở rộng thành một ánh xạ $\mathbf{R}$-tuyến tính liên tục, vẫn ký hiệu là $\rho$, của $G$ vào $\mathcal{B}$, và đó hiển nhiên là một phép nâng của G.

Cho F là một không gian lồi địa phương Hausdorff, $F'_s$ là đối ngẫu của nó được trang bị tôpô $\sigma(F', F)$. Ký hiệu $\mathcal{L}_{F'_s}^\infty$ là không gian vectơ các ánh xạ $f$ của T vào $F'_s$, sao cho $f$ đo được theo vô hướng đối với $\mu$ và bằng theo vô hướng địa phương hầu khắp nơi (theo $\mu$) với một ánh xạ của T vào một tập con đều liên tục của $F'$. Ký hiệu $L_{F'_s}^\infty$ là không gian thương của $\mathcal{L}_{F'_s}^\infty$ bởi không gian các ánh xạ của T vào $F'_s$ không đáng kể theo vô hướng địa phương đối với $\mu$.

Khi F thỏa các giả thiết của §1, No. 5, Mệnh đề 13, các hàm trong $\mathcal{L}_{F'_s}^\infty$ là $\mu$-đo được đối với tôpô yếu $\sigma(F', F)$, nhưng không nhất thiết đo được đối với tôpô mạnh trên $F'$, ngay cả khi F là một không gian Banach (§1, Bài tập 17). Dưới cùng các điều kiện đó, các ánh xạ không đáng kể theo vô hướng địa phương đối với $\mu$ của T vào $F'_s$ trùng với các ánh xạ không đáng kể theo địa phương đối với $\mu$ của T vào $F'_s$ (§1, No. 1, Nhận xét 2).

Khi F là một không gian chuẩn tách được, các phần tử của $\mathcal{L}_{F'_s}^\infty$ là các ánh xạ $f$ của T vào $F'_s$ sao cho $f$ đo được theo vô hướng đối với $\mu$ và $|f|$ bị chặn theo độ đo; khi đó có thể định nghĩa một cấu trúc không gian chuẩn trên không gian $L_{F'_s}^\infty$, bằng cách trang bị cho nó chuẩn $N_\infty$ (Ch. IV, §6, No. 3).

#### Bổ đề 3 {#int-vi-s2-lem-3 .statement}

Cho F là một không gian lồi địa phương Hausdorff, $f$ là một phần tử của $\mathcal{L}_{F'_s}^\infty$. Với mọi $z \in F$, ta có $\langle z, f \rangle \in \mathcal{L}^\infty$, và ánh xạ tuyến tính $z \mapsto \pi(\langle z, f \rangle)$ của F vào $L^\infty$ là liên tục; hơn nữa, nếu F là một không gian chuẩn, thì $N_\infty(\langle z, f \rangle) \leq |z| \cdot \sup_{t \in T} |f(t)|$.

Hiển nhiên theo định nghĩa rằng $\langle z, f \rangle$ là $\mu$-đo được và bị chặn theo độ đo; nếu cần, thay $f$ bởi một hàm thuộc cùng một lớp của $L_{F'_s}^\infty$, ta có thể giả sử thêm rằng $f(T) \subset V^\circ$, trong đó V là một lân cận cân bằng lồi của 0 trong F (điều này không làm thay đổi $\langle z, f \rangle$ trừ trên một tập không đáng kể địa phương, phụ thuộc vào $z$). Khi đó quan hệ $z \in V$ suy ra $|\langle z, f(t) \rangle| \leq 1$ với mọi $t \in T$, điều này chứng minh tính liên tục của $z \mapsto \pi(\langle z, f \rangle)$. Khẳng định cuối cùng là hiển nhiên.

#### Bổ đề 4 {#int-vi-s2-lem-4 .statement}

Cho F là một không gian lồi địa phương Hausdorff, $f$ là một phần tử của $\mathcal{L}_{F'_s}^\infty$. Với mọi hàm số $g \in \overline{\mathcal{L}}^1$, hàm $gf$ khả tích thiết yếu theo vô hướng đối với $\mu$ và $\int gf\, d\mu \in F'$.

For every $z \in F$, $\langle z, f \rangle$ thuộc $\mathcal{L}^\infty$, do đó có mệnh đề đầu tiên. Hơn nữa, có thể giả sử, mà không làm thay đổi $\int gf\, d\mu$, rằng $f(T) \subset V^\circ$, trong đó V là một lân cận lồi cân bằng của 0 trong F. Khi đó quan hệ $z \in V$ suy ra $|\langle z, f(t) \rangle| \leq 1$ với mọi $t \in T$, do đó $|\langle z, \int gf\, d\mu \rangle| = |\int \langle z, f \rangle g\, d\mu| \leq \overline{N}_1(g)$, điều này chứng tỏ rằng $\int gf\, d\mu \in F'$.

#### Định lý 1 {#int-vi-s2-thm-1 .statement}

— Cho F là một không gian lồi địa phương Hausdorff chứa một tập con trù mật đếm được. Với mọi hàm $f \in \mathcal{L}_{F'_s}^\infty$ và mọi $z \in F$, đặt $v_f(z) = \pi(\langle z, f \rangle) \in L^\infty$; ánh xạ $f \mapsto v_f$ xác định, qua thương, một song ánh tuyến tính từ $L_{F'}^\infty$ lên không gian $\mathcal{L}(F; L^\infty)$ của các ánh xạ tuyến tính liên tục từ F vào $L^\infty$. *Nếu $F$ là một không gian có chuẩn, thì song ánh này là một đẳng cự.*

Do Bổ đề 3, mệnh đề đầu tiên sẽ được chứng minh nếu ta chứng minh rằng với mọi ánh xạ liên tục $u$ của F vào $L^\infty$, tồn tại một hàm $f \in \mathcal{L}_{F'}^\infty$ sao cho $\pi(\langle z, f \rangle) = u(z)$ với mọi $z \in F$, và rằng lớp của $f$ trong $L_{F'}^\infty$ được xác định duy nhất bởi điều kiện này. Điểm thứ hai là ngay lập tức, vì nếu $\pi(\langle z, f \rangle) = \pi(\langle z, f_1 \rangle)$ với mọi $z \in F$, thì $f_1 - f$ là vô hướng không đáng kể địa phương. Mặt khác, tồn tại một phép nâng $\rho$ của $u(F)$ vào $\mathcal{L}^\infty$ (Bổ đề 2). Với mọi $t \in T$, ánh xạ $z \mapsto \rho(u(z))(t)$ là một dạng tuyến tính liên tục trên F, tức là một phần tử $f(t)$ của $F'$. Hàm $f$ là khả đo theo vô hướng $\mu$ vì $\langle z, f \rangle = \rho(u(z)) \in \mathcal{L}^\infty$ với mọi $z \in F$; ta có $\pi(\langle z, f \rangle) = u(z)$; cuối cùng, với mọi $t \in T$ và mọi $z$ thuộc ảnh ngược $V$ qua $u$ của quả cầu đơn vị của $L^\infty$,

$$
|\langle z, f(t) \rangle| = |\rho(u(z))(t)| \leq N_\infty(u(z)) \leq 1,
$$

điều này cho thấy rằng $f(t) \in V^\circ$ với mọi $t \in T$.

Nếu, hơn nữa, $F$ là một không gian có chuẩn, thì điều trên cho thấy rằng

$$
\sup_{t \in T} |f(t)| \leq \|u\|.
$$

Nhưng mặt khác (Bổ đề 3), $N_\infty(u(z)) \leq |z| \cdot \sup_{t \in T} |f(t)|$, và bất đẳng thức này vẫn đúng khi $f$ được thay đổi tùy ý trên một tập không đáng kể địa phương. Suy ra $\|u\| = N_\infty(|f|)$.

#### Hệ quả 1 {#int-vi-s2-thm-1-cor-1 .statement}

*Cho $F$ là một không gian lồi địa phương Hausdorff chứa một tập con trù mật đếm được. Với mỗi hàm $f \in \mathcal{L}_{F'}^\infty$, mỗi $z \in F$ và mỗi hàm $g \in \mathcal{L}^1$, đặt $\Phi_f(z, \tilde{g}) = \int \langle z, f(t) \rangle g(t)\, d\mu(t)$. Ánh xạ $f \mapsto \Phi_f$ xác định, qua phép chuyển sang thương, một song ánh tuyến tính từ $L_{F'}^\infty$ lên không gian $\mathcal{B}(F, L^1)$ gồm các dạng song tuyến tính liên tục trên $F \times L^1$. *Nếu $F$ là một không gian chuẩn, thì song ánh này là một đẳng cự.*

Có thể giả sử rằng $f(T)$ là một tập con đều liên tục của $F'$. Khi đó hiển nhiên $\Phi_f$ là liên tục riêng rẽ, và, với các ký hiệu của Định lý 1 và Phụ lục, ta có (tính đến thực tế rằng $L^\infty$ là đối ngẫu của $L^1$ (Ch. V, §5, No. 8, Định lý 4)) $^l \Phi_f = v_f$. Hệ quả này suy ra từ Định lý 1 trên đây và từ Phụ lục, No. 1, Mệnh đề 1 và hệ quả của nó.

#### Hệ quả 2 (định lý Dunford–Pettis) {#int-vi-s2-thm-1-cor-2 .statement}

— *Cho $F$ là một không gian lồi địa phương Hausdorff chứa một tập con trù mật đếm được. Với mỗi hàm $f \in \mathcal{L}_{F'}^\infty$ và mỗi hàm $g \in \mathcal{L}^1$, đặt $w_f(\tilde{g}) = \int gf\, d\mu \in F'$ (Bổ đề 4). Ánh xạ $f \mapsto w_f$ xác định, qua phép chuyển sang thương, một song ánh tuyến tính* từ $L_{F_s}^\infty$ lên không gian $\mathcal{R}(L^1, F')$ gồm các ánh xạ tuyến tính $u$ của $L^1$ vào $F'$ sao cho ảnh của quả cầu đơn vị của $L^1$ qua $u$ là một tập con đều liên tục của $F'$. *Nếu $F$ là một không gian chuẩn (trong trường hợp đó $\mathcal{R}(L^1, F')$ là không gian các ánh xạ tuyến tính liên tục từ $L^1$ vào đối ngẫu mạnh của $F$), thì song ánh $f \mapsto w_f$ là một đẳng cự.*

Tính đến thực tế rằng $L^\infty$ là đối ngẫu của $L^1$, điều này suy ra từ hệ quả trước và từ Phụ lục, No. 1, Mệnh đề 1 và hệ quả của nó.

#### Nhận xét {#int-vi-s2-n5-rem-1 .statement}

— Điều hiển nhiên là các ánh xạ $u \in \mathcal{R}(L^1, F')$ đều liên tục đối với mọi $\mathcal{G}$-tôpô trên $F'$ ($\mathcal{G}$ là một phủ của $F$ bởi các tập con bị chặn). Ngược lại, nếu giả thiết thêm rằng $F$ là *barreled*, thì mọi ánh xạ tuyến tính liên tục của $L^1$ vào $F'$ được trang bị một tôpô $\mathcal{G}$ đều biến quả cầu đơn vị của $L^1$ thành một tập con bị chặn của $F'$, và do đó là đều liên tục (TVS, III, §4, No. 2, Định lý 1).

#### Hệ quả 3 {#int-vi-s2-thm-1-cor-3 .statement}

*Cho $F$ là một không gian lồi địa phương Hausdorff chứa một tập con trù mật đếm được, $m$ là một độ đo vectơ trên $T$ với giá trị trong đối ngẫu yếu $F'$ của $F$. Nếu ảnh qua $m$ của tập $B$ gồm các hàm $g$ trong $\mathcal{K}(T)$ sao cho $\mu(|g|) \leq 1$ được chứa trong một tập con đóng, lồi và đẳng liên tục $H'$ của $F'$, thì $m$ có cơ sở $\mu$ và tồn tại một mật độ $f$ của $m$ đối với $\mu$ sao cho $f(t) \in H'$ với mọi $t \in T$.*

Giả thiết suy ra rằng $m$ liên tục khi $\mathcal{K}(T)$ được trang bị tôpô cảm sinh bởi tôpô của $\mathcal{L}^1(\mu)$ (được định nghĩa bởi nửa chuẩn $N_1$); do đó nó có thể được mở rộng thành một ánh xạ tuyến tính liên tục $u$ của $\mathcal{L}^1(\mu)$ vào sự hoàn thành $G$ của đối ngẫu yếu của $F$; nhưng vì $H'$ là một tập con compact của $G$ và ảnh qua $u$ của tập $\overline{B}$ gồm các $f \in \mathcal{L}^1$ sao cho $N_1(f) \leq 1$ được chứa trong bao đóng của $H'$ trong $G$, nên có $u(\overline{B}) \subset H'$, do đó $u$ ánh xạ $\mathcal{L}^1$ vào $F'$. Vì quan hệ $N_1(f) \leq \varepsilon$ suy ra rằng $u(f) \in \varepsilon H'$, nên $u(g) = 0$ nếu $g$ là $\mu$-không đáng kể, và do đó có thể áp dụng Hệ quả 2 cho ánh xạ của $L^1$ vào $F'$ thu được từ $u$ bằng cách chuyển qua thương; do đó suy ra hệ quả.

#### Hệ quả 4 {#int-vi-s2-thm-1-cor-4 .statement}

*Cho $F$ là một không gian chuẩn tách được, và $m$ là một độ đo trên $T$ với giá trị trong đối ngẫu mạnh $F'$, bị chặn trên bởi chuẩn của $F'$. Khi đó $m$ là một độ đo với cơ sở $|m|$, và nếu $m = f \cdot |m|$ thì $|f(t)| = 1$ địa phương hầu khắp nơi đối với $|m|$.*

Do đó, với mọi $z \in F$ sao cho $|z| \leq 1$, ta có $|\langle z, m(g) \rangle| \leq |m|(|g|)$ với mọi hàm $g \in \mathcal{K}(T)$, do đó $|m(g)| \leq |m|(|g|)$ (TVS, IV, §2, No. 4, công thức (1)). Vì mọi quả cầu trong $F'$ đều đều liên tục, Hệ quả 3 áp dụng được và cho thấy rằng $m$ có cơ sở $|m|$; hơn nữa, nếu $m = f \cdot |m|$ thì $f$ là $|m|$-đo được đối với $\sigma(F', F)$ (§1, No. 5, Mệnh đề 13) và $|m| = |f| \cdot |m|$ (No. 4, Mệnh đề 8), điều đó chứng minh hệ quả này (Ch. V, §5, No. 3, Hệ quả 2 của Mệnh đề 3).

Nếu hệ quả này được áp dụng vào trường hợp $F$ hữu hạn chiều, ta thu được như một trường hợp riêng phần thứ nhất của Mệnh đề 9.

### 6. Đối ngẫu của không gian $L^1_F$ (F là một không gian Banach tách được)

#### Mệnh đề 10 {#int-vi-s2-prop-10 .statement}

— *Cho F là một không gian Banach tách được. Với mọi hàm $f \in \overline{\mathcal{L}}^1_F$ và mọi hàm $g \in \mathcal{L}_{F'_s}^\infty$, hàm số vô hướng $\langle f, g \rangle : t \mapsto \langle f(t), g(t) \rangle$ là gần như $\mu$-tích phân được, và*

$$
\left| \int \langle f, g \rangle \, d\mu \right| \leq \overline{N}_1(f) N_\infty(g) .
$$

*Với mỗi lớp $\dot{g} \in L_{F'_s}^\infty$, gọi $\theta(\dot{g})$ là dạng tuyến tính liên tục trên $L^1_F$ suy ra từ dạng tuyến tính $f \mapsto \int \langle f, g \rangle \, d\mu$ trên $\overline{\mathcal{L}}^1_F$ bằng cách chuyển xuống thương; khi đó $\theta$ là một đẳng cự tuyến tính từ $L_{F'_s}^\infty$ lên đối ngẫu mạnh $(L^1_F)'$ của không gian Banach $L^1_F$.

Với mọi tập con compact K của T và mọi $\varepsilon > 0$, tồn tại một tập con compact K' của K sao cho $\mu(K - K') \leq \varepsilon$ và sự hạn chế của $f$ (tương ứng $g$) trên K' là một ánh xạ liên tục từ K' vào F (tương ứng vào $F'_s$); do đó $g(K')$ là compact yếu, suy ra đều liên tục trên $F'$ (TVS, III, §4, No. 2, ĐL. 1 hoặc IV, §1, BT. 10). Bây giờ, hạn chế của dạng song tuyến tính chính tắc trên $F \times F'$ đối với tích của F và một tập con đều liên tục của $F'$ là liên tục đối với tôpô tích của tôpô của F và $\sigma(F', F)$ (GT, X, §2, No. 1, Hệ quả 4 của Mệnh đề 1); suy ra rằng hạn chế của $\langle f, g \rangle$ trên K' là liên tục, do đó $\langle f, g \rangle$ là $\mu$-đo được. Hơn nữa,

$$
|\langle f(t), g(t) \rangle| \leq |f(t)| \cdot |g(t)| \leq |f(t)| N_\infty(g)
$$

địa phương hầu khắp nơi, do đó $\langle f, g \rangle$ là gần như $\mu$-tích phân được và bất đẳng thức (3) đúng (Ch. IV, §5, No. 6, ĐL. 5 và Ch. V, §1, No. 3, Bổ đề).

Còn phải chứng minh rằng $\theta$ là một đẳng cự toàn ánh. Gọi $u$ là một dạng tuyến tính liên tục trên $L^1_F$. Ánh xạ $(\tilde{h}, z) \mapsto u(\tilde{h}z)$ là một dạng song tuyến tính liên tục trên $L^1 \times F$, vì

$$
|u(\tilde{h}z)| \leq \|u\| \cdot N_1(hz) \leq \|u\| \cdot |z| \cdot N_1(h) .
$$

Theo Hệ quả 1 của Định lý 1 ở No. 5, tồn tại một ánh xạ $g$ từ T vào $F'$, thuộc $\mathcal{L}_{F'_s}^\infty$, sao cho $|g(t)| \leq \|u\|$ với mọi $t \in T$ và sao cho $u(\tilde{h}z) = \int \langle hz, g \rangle \, d\mu$ với mọi hàm $h \in \mathcal{L}^1$ có lớp $\tilde{h}$ trong $L^1$ và mọi $z \in F$. Nói cách khác, các dạng tuyến tính $u$ và $\theta(\dot{g})$ trùng nhau trên không gian con của $L^1_F$ được sinh bởi các phần tử có dạng $\tilde{h}z$ ($\tilde{h} \in L^1, z \in F$). Vì không gian con này trù mật trong $L^1_F$ (Chương IV, §3, No. 5, Mệnh đề 10), suy ra $u = \theta(\dot{g})$, điều này đã chứng tỏ rằng $\theta$ là toàn ánh. Hơn nữa, theo (3), $\| \theta(\dot{g}) \| \leq N_\infty(g) \leq \| u \| = \| \theta(\dot{g}) \|$, do đó $\| \theta(\dot{g}) \| = N_\infty(g)$, và điều này kết thúc chứng minh.

### 7. Tích phân của một hàm nhận giá trị vectơ đối với một độ đo vectơ

#### Mệnh đề 11 {#int-vi-s2-prop-11 .statement}

— *Cho* $F, G, H$ *là ba không gian Banach*, $\Phi$ *là một ánh xạ song tuyến tính liên tục từ* $F \times G$ *vào* $H$. *Cho* $m$ *là một độ đo vectơ khả trội trên* $T$, *nhận giá trị trong* $G$. *Khi đó tồn tại một và chỉ một ánh xạ tuyến tính liên tục* $I_{\Phi,m}$ *từ* $\overline{\mathcal{L}}^1_F(|m|)$ *vào* $H$ *sao cho, với mọi* $z \in F$ *và mọi hàm vô hướng* $h$ *khả tích theo* $|m|$, *ta có* $I_{\Phi,m}(hz) = \Phi(z, \int h dm)$. *Hơn nữa,

$$
|I_{\Phi,m}(f)| \leq \| \Phi \| \int |f| d|m|
$$

*với mọi hàm* $f \in \overline{\mathcal{L}}^1_F(|m|)$.

Nếu tồn tại một ánh xạ như vậy, thì giá trị của nó đối với một hàm *bậc thang* $f$ trên các tập hợp khả tích theo $|m|$ được xác định duy nhất: vì biết rằng khi đó có thể viết $f = \sum_i a_i \varphi_{X_i}$, trong đó các $X_i$ là các tập hợp khả tích theo $|m|$ và rời nhau, còn $a_i \in F$ (Chương IV, §4, No. 9, Bổ đề). Do đó giá trị của $I_{\Phi,m}(f)$ phải bằng $\sum_i \Phi(a_i, \int \varphi_{X_i} dm)$. Bây giờ, ta có (No. 3, Mệnh đề 5)

$$
\left| \sum_i \Phi \left( a_i, \int \varphi_{X_i} dm \right) \right| \leq \| \Phi \| \cdot \sum_i |a_i| \cdot |m|(X_i) = \| \Phi \| \int |f| d|m|,
$$

which shows first of all that the element $\sum_i \Phi(a_i, \int \varphi_{X_i} dm)$ of $H$ does not depend on the particular expression of $f$ in the form $\sum_i a_i \varphi_{X_i}$, hence that we may denote it by $I_{\Phi,m}(f)$. Người ta kiểm tra ngay rằng ánh xạ $I_{\Phi,m}$ được định nghĩa như vậy là tuyến tính trên không gian $\mathcal{E}_F$ của các hàm bậc thang trên các tập hợp $|m|$-khả tích: vì thế, chỉ cần viết hai hàm $f, g$ của $\mathcal{E}_F$ dưới dạng $f = \sum_i a_i \varphi_{X_i}$ và $g = \sum_i b_i \varphi_{X_i}$ với cùng một họ hữu hạn các tập hợp $|m|$-khả tích rời nhau từng đôi một $X_i$ (điều này có thể làm được nhờ Bổ đề của Ch. IV, §4, No. 9). Bất đẳng thức (5) khi đó cho thấy $I_{\Phi,m}$ liên tục trên $\mathcal{E}_F$, và vì không gian con này trù mật trong $\overline{\mathcal{L}}^1_F$ (Ch. IV, §4, No. 10, Hệ quả 1 của Mệnh đề 19 và Ch. V, §1, No. 3), từ đó suy ra sự tồn tại và tính duy nhất của $I_{\Phi,m}$, cũng như bất đẳng thức (4).

Người ta nói rằng $I_{\Phi,m}(f)$ là tích phân của $f$ *đối với* $m$ (tương đối với ánh xạ song tuyến tính $\Phi$); khi giá trị của ánh xạ song tuyến tính $\Phi$ tại điểm $(x,y)$ được ký hiệu là $xy$, ta sẽ viết $\int f\,dm$ thay cho $I_{\Phi,m}(f)$.

Với các ký hiệu của No. 6, tích phân $\int \langle f, g \rangle\,d\mu$ chẳng qua là $I_{\Phi,m}(f)$ với $\Phi(x,x') = \langle x, x' \rangle$ và $m = g \cdot \mu$.

#### Hệ quả {#int-vi-s2-n7-cor-1 .statement}

*Nếu* $m$ *và* $m'$ *là hai độ đo khống chế trên* $T$, *với giá trị trong* $G$, *thì* $I_{\Phi,m+m'} = I_{\Phi,m} + I_{\Phi,m'}$ *và* $I_{\Phi,\lambda m} = \lambda I_{\Phi,m}$ *với mọi vô hướng* $\lambda$.

Mệnh đề thứ hai là ngay lập tức. Mệnh đề thứ nhất có nghĩa là với mọi hàm $f$ vừa $|m|$-khả tích vừa $|m'|$-khả tích,

$$
I_{\Phi,m+m'}(f) = I_{\Phi,m}(f) + I_{\Phi,m'}(f).
$$

Hàm $f$ là $(|m| + |m'|)$-khả tích (Ch. V, §2, No. 2, Hệ quả 1 của Mệnh đề 3), do đó *a fortiori* $(|m + m'|)$-khả tích, và vế thứ nhất của (6) quả thực có nghĩa. Để chứng minh (6), chỉ cần làm điều đó khi $f$ là một hàm bậc thang trên các tập hợp $(|m| + |m'|)$-khả tích, vì tập hợp các hàm như vậy trù mật trong $\mathcal{L}_F^1(|m| + |m'|)$ và hai vế của (6) là liên tục trong không gian sau, nhờ (4). Nhưng với $f = a \varphi_X$, trong đó $X$ là $(|m| + |m'|)$-khả tích, hai vế của (6) rút gọn thành $\Phi(a, \int \varphi_X\,dm) + \Phi(a, \int \varphi_X\,dm')$, do đó suy ra hệ quả.

#### Nhận xét {#int-vi-s2-n7-rem-1 .statement}

— Khi $m$ có dạng $b\mu$, trong đó $b \in G$ và $\mu$ là một độ đo thực trên $T$,

$$
I_{\Phi,m}(f) = \int \Phi(f(t), b)\,d\mu(t)
$$

for every function $f \in \mathcal{L}_F^1(\mu)$, vì cả hai biểu thức đều liên tục trên không gian này và trùng nhau khi $f$ là một hàm bậc thang trên các tập hợp khả tích theo $|\mu|$.

### 8. Độ đo phức

#### Định nghĩa 6 {#int-vi-s2-def-6 .statement}

*Người ta gọi độ đo phức trên* $T$ *mọi dạng tuyến tính liên tục trên không gian vectơ phức* $\mathscr{K}_C(T)$.\footnote{Xem Ch. III, §1, No. 3, Định nghĩa 2.}

Không gian $\mathscr{M}_C(T)$ các độ đo phức trên $T$ vì thế là *đối ngẫu* của không gian lồi địa phương Hausdorff $\mathscr{K}_C(T)$.

Nếu $m$ là một độ đo phức trên $T$, thì hạn chế của nó lên $\mathscr{K}(T)$ là một độ đo vectơ trên $T$ với giá trị trong $\mathbf{C}$ (được xem như một không gian vectơ trên $\mathbf{R}$);

$m$ được xác định bởi hạn chế này, vì nếu $f = f_1 + i f_2 \in \mathcal{H}_\mathbf{C}(T)$, thì phần thực $f_1$ và phần ảo $f_2$ của $f$ đều thuộc $\mathcal{H}(T)$, và $m(f) = m(f_1) + i m(f_2)$. Ngược lại, với mọi độ đo vectơ $m_0$ trên $T$ với giá trị trong $\mathbf{C}$, công thức $m(f) = m_0(f_1) + i m_0(f_2)$ xác định một độ đo phức $m$, là độ đo duy nhất trên $T$ có hạn chế lên $\mathcal{H}(T)$ bằng $m_0$. Vì vậy từ nay ta sẽ đồng nhất một độ đo phức với hạn chế của nó lên $\mathcal{H}(T)$; một độ đo như vậy $m$ có dạng $m = \mu_1 + i \mu_2$, trong đó $\mu_1$ và $\mu_2$ là hai độ đo thực trên $T$, và chúng được gọi lần lượt là phần thực và phần ảo của $m$. Giá đỡ của $m$ là hợp các giá đỡ của $\mu_1$ và $\mu_2$. Người ta biết rằng $m$ là majorizable (No. 3, Hệ quả của Mệnh đề 4); ta sẽ gọi giá trị tuyệt đối của $m$ là độ đo dương $|m|$ tương ứng với giá trị tuyệt đối $|x_1 + i x_2| = \sqrt{x_1^2 + x_2^2}$ trên $\mathbf{C}$. Ta có $|m| = (\mu_1^2 + \mu_2^2)^{1/2}$ (No. 4, Nhận xét sau Mệnh đề 9),$^3$ và $|\mu_1| \leq |m|$, $|\mu_2| \leq |m|$, $|m| \leq |\mu_1| + |\mu_2|$; hơn nữa, $m$ là một độ đo với cơ sở $|m|$, và có thể viết $m = h \cdot |m|$, trong đó $h \in \mathcal{L}_\mathbf{C}^\infty(|m|)$ và $|h(t)| = 1$ địa phương hầu như khắp nơi đối với $|m|$ (No. 4, Mệnh đề 9).$^4$ Giá đỡ của $m$ và $|m|$ là như nhau.

Đối với mọi ánh xạ $f$ từ T vào một không gian Banach phức F, khả tích một cách thiết yếu đối với $|m|$, ta có thể định nghĩa (No. 7) tích phân của $f$ đối với $m$ (tương ứng với ánh xạ song tuyến tính trên $\mathbf{R}$ $(x, \lambda) \mapsto \lambda x$ của $F \times \mathbf{C}$ vào F), được ký hiệu là $\int f \, dm$; suy ra ngay từ tính chất duy nhất của Mệnh đề 11 rằng (với các ký hiệu trên) $\int f \, dm = \int f \, d\mu_1 + i \int f \, d\mu_2 = \int f h \, d|m|$. Vì vậy ta có $m(f) = \int f \, dm$ với $f \in \mathcal{H}_\mathbf{C}(T)$. Ta nói rằng $f$ khả tích một cách thiết yếu đối với $m$ nếu nó như vậy đối với $|m|$;$^5$ các ánh xạ $m$-khả tích, $m$-đo được, địa phương $m$-khả tích, $m$-không đáng kể hoặc địa phương $m$-không đáng kể được định nghĩa tương tự. Ta viết
$$
\mathcal{L}_F^p(T, m) \quad \text{(tương ứng } \overline{\mathcal{L}}_F^p(T, m), \ L_F^p(T, m) \text{)}
$$
thay cho $\mathcal{L}_F^p(T, |m|)$ (tương ứng $\overline{\mathcal{L}}_F^p(T, |m|), \ L_F^p(T, |m|)$); đó là các không gian vectơ phức.

Để $f$ là $m$-khả tích (tương ứng khả tích một cách thiết yếu đối với $m$), thì điều kiện cần và đủ là $f$ khả tích (tương ứng khả tích một cách thiết yếu) đối với từng một trong bốn độ đo $\mu_1^+, \mu_1^-, \mu_2^+, \mu_2^-$, nhờ các bất đẳng thức giữa $|m|, |\mu_1|, |\mu_2|$ và các hệ thức $|\mu_k| = \mu_k^+ + \mu_k^-$ (Ch. V, §2, No. 2, Mệnh đề 3 và Hệ quả 1 của nó).

Nếu $f$ khả tích một cách thiết yếu đối với $m$ (tương ứng $m$-khả tích), thì $|f|$ là

---
$^3$Đặc biệt, định nghĩa này của $|m|$ trùng với định nghĩa trong Ch. III, §1, No. 6 (cf. Ch. V, §5, No. 9).
$^4$Xem Ch. V, §5, No. 5, Hệ quả 3 của Định lý 2 để có một mệnh đề sắc hơn.
$^5$Xem Ch. V, §1, các nhận xét ở cuối No. 3.

khả tích một cách thiết yếu đối với $|m|$ (tương ứng $|m|$-khả tích), và suy ra từ Mệnh đề 11 rằng

$$
\left| \int \mathbf{f}\, dm \right| \leq \int |\mathbf{f}| \, d|m|.
$$

Cho F và G là hai không gian Banach phức, $u$ là một ánh xạ tuyến tính liên tục từ F vào G. Nếu $\mathbf{f}$ là một ánh xạ khả tích một cách thiết yếu đối với $m$ (tương ứng $m$-khả tích) từ T vào F, thì $u \circ \mathbf{f}$ cũng khả tích một cách thiết yếu đối với $m$ (tương ứng $m$-khả tích) và $\int (u \circ \mathbf{f})\, dm = u(\int \mathbf{f}\, dm)$; điều này suy ra ngay từ các điều trên và mệnh đề tương ứng cho các hàm khả tích một cách thiết yếu đối với $|m|$ (Ch. IV, §4, No. 2, Định lý 1 và Ch. V, §1, No. 3, Bổ đề và Định nghĩa 3).

Cho $m$ là một độ đo phức trên T và cho $h$ là một hàm phức địa phương khả tích đối với $m$. Với mọi hàm $f \in \mathcal{K}_C(T)$, hàm $fh$ là $m$-khả tích và ánh xạ $f \mapsto \int fh\, dm$ là một độ đo phức, ký hiệu $h \cdot m$ và được gọi là độ đo *với mật độ* $h$ đối với $m$. Nếu $m = g \cdot |m|$, thì rõ ràng $h \cdot m = hg \cdot |m|$; hơn nữa, vì $|g(t)| = 1$ hầu khắp nơi địa phương đối với $|m|$, để $\mathbf{f}$ khả tích thiết yếu đối với $n = h \cdot m$ thì cần và đủ rằng $fh$ khả tích thiết yếu đối với $m$, trong trường hợp đó $\int \mathbf{f}\, dn = \int (\mathbf{f}h)\, dm$. Hơn nữa, $|h \cdot m| = |h| \cdot |m|$. Một lần nữa ta nói rằng mọi độ đo có dạng $h \cdot m$ là một độ đo phức *với cơ sở* $m$; hai độ đo phức $m, m'$ được gọi là *tương đương* nếu mỗi độ đo đều có một mật độ đối với độ đo kia, hay, điều đó tương đương, nếu $m' = h \cdot m$ với $h$ địa phương khả tích đối với $m$ và $h(t) \neq 0$ hầu khắp nơi địa phương đối với $|m|$. Rõ ràng $m$ và $|m|$ là tương đương và, để $m$ và $m'$ tương đương, cần và đủ rằng $|m|$ và $|m'|$ cũng như vậy.

Nếu $m$ và $m'$ là hai độ đo phức trên T, và $\mathbf{f}$ là một hàm lấy giá trị trong một không gian Banach phức F, khả tích thiết yếu (tương ứng khả tích) đối với cả $m$ và $m'$, thì, với mọi số phức $\lambda$ và $\lambda'$, $\mathbf{f}$ khả tích thiết yếu (tương ứng khả tích) đối với $\lambda m + \lambda' m'$, và

$$
\int \mathbf{f}\, d(\lambda m + \lambda' m') = \lambda \int \mathbf{f}\, dm + \lambda' \int \mathbf{f}\, dm'.
$$

Vì, điều này suy ra từ Hệ quả của Mệnh đề 11 của No. 7.

Ngoài ra, từ các định nghĩa suy ra rằng

$$
|\lambda m + \lambda' m'| \leq |\lambda| \cdot |m| + |\lambda'| \cdot |m'|.
$$

Ta gọi *độ đo liên hợp* của một độ đo phức $m$ là độ đo phức $\overline{m}$ được xác định bởi $\overline{m}(f) = m(\overline{f})$ với $f \in \mathcal{K}_C(T)$. Nếu $m = \mu_1 + i \mu_2$, trong đó $\mu_1$ và $\mu_2$ là các độ đo thực, thì $\overline{m} = \mu_1 - i \mu_2$ và $|\overline{m}| = |m|$; nếu $m = h \cdot |m|$ thì $\overline{m} = \overline{h} \cdot |m|$. Nếu $f$ là khả tích thiết yếu đối với $m$ (tương ứng

nếu $f$ là một hàm có giá trị phức, có thể tích phân theo $m$, thì $\overline{f}$ về bản chất là $\overline{m}$-có thể tích phân (resp. $\overline{m}$-có thể tích phân) và

$$
\int \overline{f}\, d\overline{m} = \overline{\int f\, dm}.
$$

#### Mệnh đề 12 {#int-vi-s2-prop-12 .statement}

*Cho m là một độ đo phức trên T, p và q là các số mũ liên hợp (Ch. IV, §6, No. 4). Dạng song tuyến tính $(f,g) \mapsto \int fg\, dm$ được xác định và liên tục trên tích $\mathcal{L}_C^p(m) \times \mathcal{L}_C^q(m)$; bất đẳng thức $|\int fg\, dm| \leq N_p(f)N_q(g)$ đúng, và $N_q(g)$ là chuẩn của dạng tuyến tính liên tục trên $\mathcal{L}_C^p(m)$ suy ra từ dạng tuyến tính $f \mapsto \int fg\, dm$ bằng phép chuyển sang thương.

Hơn nữa, nếu $1 \leq p < +\infty$, thì mọi dạng tuyến tính liên tục trên không gian vectơ phức $\mathcal{L}_C^p(m)$ đều có kiểu $f \mapsto \int fg\, dm$, trong đó $g$ là một hàm trong $\mathcal{L}_C^q(m)$, có lớp trong $\mathcal{L}_C^q(m)$ được xác định duy nhất.

Vì $m = h \cdot |m|$, với $|h(t)| = 1$ địa phương hầu khắp nơi, mệnh đề thứ nhất suy ra ngay từ bất đẳng thức Hölder (Ch. IV, §6, No. 4, Th. 2); mệnh đề thứ hai suy ra từ Mđ. 3 của Ch. IV, §6, No. 4. Cuối cùng, nếu $u$ là một dạng tuyến tính liên tục trên $\mathcal{L}_C^p$, thì hạn chế của nó lên không gian con (thực) $\mathcal{L}^p$ của $\mathcal{L}_C^p$ là một ánh xạ $\mathbf{R}$-tuyến tính liên tục của $\mathcal{L}^p$ vào $\mathbf{C}$; nếu $1 \leq p < +\infty$, thì do đó nó có kiểu $f \mapsto \int fg_1\, d|m| + i \int fg_2\, d|m|$, trong đó $g_1$ và $g_2$ thuộc $\mathcal{L}^q$ (Ch. V, §5, No. 8, Th. 4); do đó mệnh đề cuối cùng, khi đặt $g = (g_1 + ig_2)h^{-1}$.

### 9. Các độ đo phức bị chặn⁶

Với mọi độ đo phức $m$ trên $T$, ta đặt

$$
\|m\| = \sup_{\|f\| \leq 1,\, f \in \mathcal{H}_C(T)} |m(f)|.
$$

Người ta nói rằng $m$ là *bị chặn* nếu $\|m\| < +\infty$; điều đó tương đương với việc nói rằng $m$ liên tục trên $\mathcal{H}_C(T)$ được trang bị tôpô hội tụ đều, do đó có thể được mở rộng thành một dạng tuyến tính liên tục (có chuẩn $\|m\|$) trên không gian Banach $\mathcal{H}_C(T)$ của các hàm phức liên tục tiến tới 0 ở vô cực.

#### Bổ đề 5 {#int-vi-s2-lem-5 .statement}

*Cho m là một độ đo phức trên T, f là một hàm phức có thể tích phân theo m. Khi đó $\int |f|\, d|m| = \sup |\int fh\, dm|$, với h chạy qua tập các hàm trong $\mathcal{H}_C(T)$ sao cho $|h(t)| \leq 1$ với mọi $t \in T$*.

⁶Xem Ch. III, §1, No. 8.

Nếu $m = g \cdot |m|$, thì $\int |f| d|m| = \int |f g| d|m|$ và $\int f h \, dm = \int f g h \, d|m|$. Đặt $\zeta(t) = 0$ khi $f(t)g(t) = 0$, và $\zeta(t) = \frac{f(t)g(t)}{|f(t)g(t)|}$ khi $f(t)g(t) \neq 0$; $\zeta$ là $|m|$-đo được, do đó với mọi $\varepsilon > 0$ tồn tại một tập con compact K của T sao cho $\int_{T-K} |f| \, d|m| \leq \varepsilon$, hạn chế của $\zeta$ lên K là liên tục, và $|\zeta(t)| = 1$ trên K. Do đó, nhờ định lý Urysohn, tồn tại một hàm liên tục $\zeta_1$ xác định trên T, có giá trị phức, sao cho $\zeta_1 = \zeta$ trên K và sao cho $|\zeta_1(t)| \leq 2$ và $\zeta_1(t) \neq 0$ với mọi $t \in T$; đặt $h(t) = \zeta_1(t)/|\zeta_1(t)|$, ta thấy rằng h liên tục trên T, trùng với $\zeta$ trên K, và thỏa $|h(t)| = 1$ với mọi $t \in T$. Cuối cùng, cho u là một ánh xạ liên tục của T vào $[0,1]$, bằng 1 trên K và có giá compact; đặt $h_1 = h^{-1}u$, ta có
$$
\left| \int f h_1 \, dm - \int |f| \, d|m| \right| \leq 2 \int_{T-K} |f| \, d|m| \leq 2\varepsilon ,
$$
điều đó chứng minh bổ đề.

#### Mệnh đề 13 {#int-vi-s2-prop-13 .statement}

— *Cho m là một độ đo phức, và $\mu = |m|$. Để m bị chặn, điều kiện cần và đủ là $\mu$ bị chặn; khi đó $\|m\| = \|\mu\|$.*

Ta có $m = g \cdot \mu$, trong đó $g$ là $\mu$-đo được và $|g(t)| = 1$ với mọi $t \in T$. Nếu $\mu$ bị chặn thì, với mọi hàm $f \in \mathcal{K}_\mathbf{C}(T)$,
$$
|m(f)| = \left| \int f g \, d\mu \right| \leq N_\infty(fg)\|\mu\| = \|f\| \cdot \|\mu\|,
$$
do đó $m$ bị chặn và $\|m\| \leq \|\mu\|$. Nếu $m$ bị chặn thì, với mọi $f \in \mathcal{K}_\mathbf{C}(T)$ ta có, xét đến Bổ đề 5,
$$
|\mu(f)| \leq \|f\| \cdot \|m\|,
$$
do đó $\mu$ bị chặn và $\|\mu\| \leq \|m\|$. Suy ra mệnh đề.

#### Hệ quả {#int-vi-s2-n9-cor-1 .statement}

— *Cho m là một độ đo phức bị chặn. Khi đó mọi hàm $f \in \mathcal{L}_\mathbf{F}^\infty(m)$ đều khả tích theo m, và $\left| \int f \, dm \right| \leq N_\infty(f)\|m\|$.*

Vì, $f$ là $m$-đo được và, đặt $\mu = |m|$, ta có
$$
\int^* |f| \, d\mu \leq N_\infty(f)\|\mu\| = N_\infty(f)\|m\|,
$$
do đó $f$ khả tích theo $|m|$ (Ch. IV, §5, No. 6, ĐL. 5) và
$$
\left| \int f \, dm \right| \leq \int |f| \, d\mu \leq N_\infty(f)\|m\|.
$$

### 10. Ảnh của một độ đo phức; độ đo phức cảm sinh; tích của các độ đo phức\footnote{Xem Ch. V, §6, No. 4; Ch. IV, §5, No. 7 và Ch. V, §7; Ch. III, §4 và Ch. V, §8, Nos. 2–5.}

Cho $m$ là một độ đo phức trên $T$, và cho $\pi$ là một ánh xạ của $T$ vào một không gian địa phương compact $X$. Ta sẽ nói rằng $\pi$ là $m$-thực sự nếu $\pi$ là $|m|$-thực sự (Ch. V, §6, No. 1, Def. 1); khi đó hiển nhiên rằng với mọi hàm $f \in \mathcal{H}_C(X)$, hàm $f \circ \pi$ là khả tích theo nghĩa thiết yếu đối với $m$ và

$$
\left| \int (f \circ \pi)\, dm \right| \leq \int |f \circ \pi|\, d|m| = \int |f|\, d(\pi(|m|)),
$$

do đó ánh xạ $f \mapsto \int (f \circ \pi)\, dm$ là liên tục trên $\mathcal{H}_C(X)$, nói cách khác là một độ đo phức trên $X$, được ký hiệu là $\pi(m)$ và được gọi là *ảnh* của $m$ dưới $\pi$. Hơn nữa, suy ra từ (8) rằng $|\pi(m)| \leq \pi(|m|)$. Nếu $m$ và $m'$ là hai độ đo phức trên $T$ và nếu $\pi$ vừa là $m$-thực sự vừa là $m'$-thực sự, thì $\pi$ là $(\lambda m + \lambda' m')$-thực sự với mọi vô hướng phức $\lambda, \lambda'$, và $\pi(\lambda m + \lambda' m') = \lambda \pi(m) + \lambda' \pi(m')$.

Cho $Y$ là một không gian con địa phương compact của $T$. Với mọi hàm $f \in \mathcal{H}_C(Y)$, hàm $f'$ trên $T$, được xác định bởi $f'(t) = f(t)$ nếu $t \in Y$ và bởi $f'(t) = 0$ nếu $t \notin Y$, là khả tích đối với $m$ (Ch. IV, §5, No. 7); hiển nhiên rằng ánh xạ $f \mapsto \int f'\, dm$ là một độ đo phức trên $Y$, gọi là độ đo *được cảm sinh* trên $Y$ bởi $m$ và ký hiệu $m_Y$. Nếu $m = g \cdot |m|$, thì rõ ràng $m_Y = g_Y \cdot |m|_Y$, trong đó $g_Y$ là hạn chế lên $Y$ của hàm $g$, hàm này khả tích địa phương đối với $|m|_Y$ (Ch. V, §7, No. 1); hơn nữa, vì $|g_Y| = 1$ hầu như khắp nơi địa phương đối với $|m|_Y$ (Ch. V, §7, No. 1, Cor. 1 of Prop. 1), ta có $|m_Y| = |m|_Y$.\footnote{Xem Ch. IV, §5, No. 7, Bổ đề 3.}

Let $T$ và $T'$ là hai không gian compact địa phương, $m$ (resp. $m'$) là một độ đo phức trên $T$ (resp. $T'$). Viết $m = g \cdot |m|$ và $m' = g' \cdot |m'|$. Hàm $g \otimes g'$ là khả tích địa phương trên $T \times T'$ đối với độ đo dương $|m| \otimes |m'|$ (Ch. V, §8, No. 5, Mệnh đề 10), và ta kiểm tra ngay rằng nếu $g$ (resp. $g'$) được thay bởi một hàm $g_1$ (resp. $g'_1$) bằng $g$ (resp. $g'$) địa phương hầu khắp nơi đối với $|m|$ (resp. $|m'|$), thì $g_1 \otimes g'_1$ bằng $g \otimes g'$ địa phương hầu khắp nơi đối với $|m| \otimes |m'|$. Vì thế độ đo phức $(g \otimes g') \cdot (|m| \otimes |m'|)$ trên $T \times T'$ chỉ phụ thuộc vào $m$ và $m'$; nó được ký hiệu là $m \otimes m'$ và được gọi là độ đo *tích* của $m$ và $m'$. Vì $|g \otimes g'| = 1$ địa phương hầu khắp nơi đối với $|m| \otimes |m'|$ (Ch. V, §8, No. 2, Mệnh đề 4), ta có $|m \otimes m'| = |m| \otimes |m'|$.\footnote{Cf. Ch. III, §4, No. 2, Mệnh đề 3.}

Bạn đọc sẽ dễ dàng kiểm tra rằng mọi mệnh đề đã chứng minh ở Ch. V liên quan đến ảnh của một độ đo dương, độ đo cảm sinh bởi một độ đo dương, và tích của các độ đo dương, trừ những mệnh đề trong đó các tích phân trên hoặc các tích phân trên cốt yếu can dự, vẫn đúng khi các độ đo dương được thay bởi các độ đo phức tùy ý.

Sau cùng, người ta định nghĩa như ở §1 khái niệm hàm cốt yếu khả tích theo vô hướng đối với một độ đo phức $m$; để một hàm $f$ có tính chất này, điều kiện cần và đủ là $f$ phải cốt yếu khả tích theo vô hướng đối với $|\mu_1|$ và $|\mu_2|$, trong đó $\mu_1$ và $\mu_2$ là phần thực và phần ảo của $m$, khi đó $\int f dm = \int f d\mu_1 + i \int f d\mu_2$. Chúng tôi để cho bạn đọc nhiệm vụ chuyển các kết quả của §1 sang các độ đo phức.

### Bài tập {#int-vi-s2-exercises}

Xem [các bài tập cho § 2](exercises/s2/).
