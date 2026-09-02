---
book: alg
book_title: Algebra
chapter: IX
chapter_title: Formes sesquilinéaires et formes quadratiques
section: 4
section_title: Sous-espaces totalement isotropes. Théorème de Witt
lang: vi
source: alg-ix-fr
pdf_pages: 0061-0077
extraction: ocr
subsections:
    - "no": 1
      title: Sous-espaces isotropes.
      page: 0
      pdf_page: 62
    - "no": 2
      title: Décomposition de Witt.
      page: 0
      pdf_page: 63
    - "no": 3
      title: Théorème de Witt.
      page: 0
      pdf_page: 69
statements: 17
exercises: 0
content_sha256: cf0f0e2f6785aaa6b3e0de1e2bc22e884a5c735d2a302d0d4faff0a9ee403010
translated_from: content/en-mt/alg/IX/04_s4_sous_espaces_totalement_isotropes.md
source_lang: en-mt
translation_method: machine
source_content_sha256: c4d7dc0a8eceecac04306c2d8d160c199d10a6bf0f27b9e52f5313167fc907ac
translation_model: gpt-5.4
translation_run: translate-vi-38d41cce
glossary_version: 34
glossary_terms_sha256: 335390868a56e35bae23dfcff21916d5797c5ee0a7a518249ae0af87cd4640bc
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 4. Các không gian con hoàn toàn đẳng hướng. Định lý Witt

Trong đoạn này giả thiết rằng, trừ khi nói rõ ngược lại, A là một trường. Bởi Φ ta ký hiệu hoặc một dạng ε-Hermit trên E (đối với phản tự đẳng cấu đối hợp $λ \to \overline{λ}$ của A), hoặc dạng song tuyến tính đối xứng liên kết với một dạng toàn phương Q trên E (trong trường hợp sau giả thiết A giao hoán).

### 1. Các không gian con đẳng hướng.

#### Định nghĩa 1 {#alg-ix-s4-def-1 .statement}

Cho một môđun E trên vành A, một phần tử x của E được gọi là đẳng hướng nếu $\Phi(x, x) = 0$. Một môđun con F của E được gọi là
    1) đẳng hướng nếu tồn tại một phần tử $x \neq 0$ của F trực giao với F;
    2) hoàn toàn đẳng hướng nếu hạn chế của $\Phi$ lên F bằng không.

Khi môđun E được trang bị một dạng toàn phương Q, một phần tử của E sẽ được gọi là đẳng hướng (tương ứng, một môđun con của E được gọi là đẳng hướng, hoặc hoàn toàn đẳng hướng) nếu phần tử đó là đẳng hướng (tương ứng, nếu môđun con đó là đẳng hướng, hoặc hoàn toàn đẳng hướng) đối với dạng song tuyến tính liên kết với Q.

Một vectơ đẳng hướng đơn giản là một vectơ trực giao với chính nó. Nói rằng một môđun con F là đẳng hướng có nghĩa là $F \cap F^0 \neq \{0\}$, hay tương đương, hạn chế của $\Phi$ lên F là suy biến; do đó một môđun con G không đẳng hướng của E là một môđun con sao cho hạn chế của $\Phi$ lên G là không suy biến. Để một môđun con F của E là hoàn toàn đẳng hướng, điều kiện cần và đủ là $F \subset F^0$. Nếu F là một môđun con hoàn toàn đẳng hướng của E, thì mọi môđun con $F'$ được chứa trong F cũng có tính chất đó. Tổng của một họ các môđun con hoàn toàn đẳng hướng trực giao từng đôi một là một môđun con hoàn toàn đẳng hướng. Tập hợp các môđun con hoàn toàn đẳng hướng của E, được sắp thứ tự bởi quan hệ bao hàm, hiển nhiên là quy nạp; do đó mọi môđun con hoàn toàn đẳng hướng đều được chứa trong một môđun con hoàn toàn đẳng hướng cực đại.

#### Mệnh đề 1 {#alg-ix-s4-prop-1 .statement}

Giả sử A là một trường. Cho F là một không gian con hữu hạn chiều không đẳng hướng của E; khi đó E là tổng trực tiếp của F và $F^0$.

Thật vậy, vì hạn chế $\Phi'$ của $\Phi$ lên F là không suy biến theo giả thiết, ánh xạ $d_{\Phi'}$ từ F vào đối ngẫu của nó $F^*$ liên kết bên phải với $\Phi'$ là đơn ánh, nên là song ánh vì F và $F^*$ là hai không gian có cùng số chiều hữu hạn. Do đó, với mọi $y \in E$, tồn tại một và chỉ một phần tử $y_0$ của F sao cho $\Phi(x, y) = \Phi(x, y_0)$ với mọi $x \in F$, nghĩa là, $y - y_0 \in F^0$; điều này chứng tỏ rằng E là tổng trực tiếp của F và $F^0$.

#### Hệ quả {#alg-ix-s4-n1-cor-1 .statement}

Nếu F là một không gian con hữu hạn chiều của E, và nếu Φ là không suy biến, thì các điều kiện sau là tương đương:

a) F là không đẳng hướng.
b) F^0 là không đẳng hướng.
c) E là tổng trực tiếp của F và F^0.

Mệnh đề 1 thực vậy cho thấy rằng a) suy ra c), và c) suy ra a) và b). Sau cùng, nếu F^0 là không đẳng hướng, ta có F ∩ F^0 ⊂ F^0 ∩ F^{00} = {0}; do đó F là không đẳng hướng, điều này cho thấy rằng b) suy ra a).

#### Định nghĩa 2 {#alg-ix-s4-def-2 .statement}

Cho Q là một dạng toàn phương trên E. Một phần tử x của E được gọi là kì dị (đối với Q) nếu Q(x) = 0. Một môđun con F của E được gọi là:
1) kì dị nếu tồn tại một phần tử x ≠ 0 của F vừa kì dị vừa trực giao với F;
2) hoàn toàn kì dị nếu hạn chế của Q lên F bằng không.

Hạt nhân của môđun toàn phương (E, Q) (§ 3, n° 4) gồm các phần tử kì dị của E^0; để một môđun con F là kì dị, điều kiện cần và đủ là hạt nhân của nó ≠ {0}. Vì Φ(x, y) = Q(x + y) − Q(x) − Q(y), mọi môđun con hoàn toàn kì dị ≠ {0} đều là kì dị. Vì Φ(x, x) = 2Q(x), mọi vectơ kì dị đều là đẳng hướng và mọi môđun con kì dị (tương ứng môđun con hoàn toàn kì dị) đều là đẳng hướng (tương ứng hoàn toàn đẳng hướng); điều đảo lại là đúng nếu A là một trường có đặc số ≠ 2. Mọi môđun con được chứa trong một môđun con hoàn toàn kì dị thì bản thân nó cũng hoàn toàn kì dị. Tổng của một họ các môđun con hoàn toàn kì dị trực giao từng đôi một là một môđun con hoàn toàn kì dị. Tập hợp các môđun con hoàn toàn kì dị của E, được sắp thứ tự bởi quan hệ bao hàm, là quy nạp; do đó mọi môđun con hoàn toàn kì dị của E đều được chứa trong một môđun con hoàn toàn kì dị cực đại.

### 2. Phân tích Witt.

Vào các quy ước đã có hiệu lực từ đầu đoạn hiện tại, ta sẽ thêm quy ước sau đây:

Bourbaki XXIV.

ĐIỀU KIỆN (T). — Với mọi $x \in E$, tồn tại $\alpha \in A$ sao cho $\Phi(x, x) = \alpha + \varepsilon \bar{\alpha}$.

Điều kiện này luôn được thỏa mãn khi $\Phi$ là phản xứng, hoặc khi $\varepsilon = 1$ và $A$ là một trường có đặc số $\neq 2$, bằng cách lấy $\alpha = \frac{1}{2} \Phi(x, x)$ (x. bài tập 1 và 14).

#### Bổ đề 1 {#alg-ix-s4-lem-1 .statement}

Cho $\Phi$ là một dạng $\varepsilon$-Hermit thỏa mãn (T) (tương ứng dạng song tuyến tính liên kết với một dạng toàn phương Q) trên $E$, và cho F là một không gian con hoàn toàn đẳng hướng (tương ứng hoàn toàn kì dị) của $E$, không thu về 0. Với mọi $x \in E$ không trực giao với F và mọi $\alpha \in A$, tồn tại $y \in F$ sao cho

$$
\Phi(x + y, x + y) = \alpha + \varepsilon \bar{\alpha} \quad (\text{resp. } Q(x + y) = \alpha).
$$

Đặt $\Phi(x, x) = \beta + \varepsilon \bar{\beta}$ (tương ứng $Q(x) = \beta$). Khi đó với $y \in F$ ta có $\Phi(x + y, x + y) = (\beta + \Phi(x, y)) + \varepsilon (\beta + \Phi(x, y))$ vì $\Phi(y, y) = 0$ (tương ứng $Q(x + y) = \beta + \Phi(x, y)$ vì $Q(y) = 0$). Vì $x$ không trực giao với F, hàm afin tuyến tính $y \to \Phi(x, y) + \beta$ trên F không phải là hằng; do đó nó nhận giá trị $\alpha$ tại một phần tử nào đó $y$ của F, và vì thế trả lời được câu hỏi.

Người ta gọi là phân tích Witt của E mọi phân tích của E thành tổng trực tiếp của ba không gian con F, F', G sao cho F và F' là hoàn toàn đẳng hướng (tương ứng hoàn toàn kỳ dị) và G là không đẳng hướng và trực giao với $F + F'$; nếu E có chiều hữu hạn, ma trận của $\Phi$ đối với một cơ sở của E thích hợp với một phân tích Witt của E có dạng

$$
\begin{pmatrix}
0 & U & 0 \\
\varepsilon \overline{U} & 0 & 0 \\
0 & 0 & V
\end{pmatrix}
$$

(1)

Người ta nói rằng $\Phi$ là một dạng trung hòa nếu nó không suy biến và nếu E có chiều hữu hạn và là tổng trực tiếp của hai không gian con hoàn toàn đẳng hướng (tương ứng hoàn toàn kỳ dị). Tổng trực tiếp của hai dạng trung hòa là một dạng trung hòa.

#### Mệnh đề 2 {#alg-ix-s4-prop-2 .statement}

Cho $\Phi$ là một dạng $\varepsilon$-Hermite không suy biến thỏa mãn (T) (tương ứng dạng song tuyến tính gắn với một dạng toàn phương không suy biến Q), và F là một không gian con hoàn toàn đẳng hướng (tương ứng hoàn toàn kỳ dị) có chiều hữu hạn r.

a) Nếu $F'$ là một không gian con hoàn toàn đẳng hướng có chiều r sao cho $F' \cap F^0 = \{0\}$, thì $F + F'$ là không đẳng hướng và, với mọi cơ sở $(f_i)$ của F, tồn tại một cơ sở $(f'_i)$ của $F'$ sao cho $\Phi(f_i, f'_j) = \delta_{ij}$ (chỉ số Kronecker) với $i, j = 1, \ldots, r$.

b) Nếu G là một không gian con hoàn toàn đẳng hướng (tương ứng hoàn toàn kỳ dị) có chiều $\leq r$ sao cho $G \cap F^0 = \{0\}$, thì tồn tại một không gian con hoàn toàn đẳng hướng (tương ứng hoàn toàn kỳ dị) $F' \supset G$ có chiều r sao cho $F' \cap F^0 = \{0\}$.

Gọi $\Psi$ là hạn chế của $\Phi$ lên $F \times F'$; với $x' \in F'$, quan hệ «$\Phi(x, x') = 0$ với mọi $x \in F$ » kéo theo $x = 0$ vì $F' \cap F^0 = \{0\}$. Khi đó mệnh đề a) suy ra từ hệ quả của mệnh đề 6, § 1, No. 6, trừ việc $F + F'$ là không đẳng hướng. Mà không gian con $H = (F + F') \cap (F + F')^0$ bằng $(F + F') \cap F^0 \cap {F'}^0$. Vì $F \subset F^0$, ta có $(F + F') \cap F^0 = F + (F' \cap F^0) = F$, do đó $H = F \cap {F'}^0$; vậy nên $H = \{0\}$ vì ta đã thấy rằng $\Psi$ là không suy biến. Điều này chứng tỏ rõ rằng $F + F'$ là không đẳng hướng.

Để chứng minh b), ta sẽ tiến hành bằng quy nạp lùi theo $s = \dim G$. Như vậy chỉ cần chứng minh rằng, nếu $s < r$, thì tồn tại một không gian con hoàn toàn đẳng hướng (tương ứng hoàn toàn kỳ dị) $G'$ chứa G, có chiều $s + 1$, và sao cho $G' \cap F^0 = \{0\}$. Vì $\dim G < \dim F$, hạn chế của $\Phi$ lên $F \times G$ là suy biến, và vì $G \cap F^0$ bằng không, $F \cap G^0$ là khác không. Khi đó nếu ta có $G + F^0 \supset G^0$, thì khi lấy các không gian con trực giao và nhận thấy rằng $F = F^{00}$ và $G = G^{00}$ ($§ 1$, No. 6, hệ quả 1 của mệnh đề 4), ta sẽ suy ra $G^0 \cap F \subset G$, do đó

$$
G^0 \cap F \subset G \cap F \subset G \cap F^0 = \{0\},
$$

điều này là không thể được. Khi đó tồn tại một phần tử $x$ của $G^0$ sao cho $x \notin G + F^0$; vì $F \subset F^0$, ta có thể cộng vào $x$ một vectơ của $G^0 \cap F$ mà không làm thay đổi các tính chất ấy; vì $G^0 \cap F$ là hoàn toàn đẳng hướng (tương ứng hoàn toàn kỳ dị) và $\neq \{0\}$, bổ đề 1 cho thấy rằng có thể chọn $x$ đẳng hướng (tương ứng kỳ dị).

Khi đó không gian con $G' = G + Ax$ có chiều $s + 1$, và là hoàn toàn đẳng hướng (tương ứng, hoàn toàn kỳ dị); hơn nữa ta có $G' \cap F^0 = \{0\}$ vì, nếu $y = z + ax$ ($z \in G,\ a \in A$) thuộc $F^0$, thì ta có $a = 0$, nếu không thì $x \in F^0 + G$, trái với cách chọn $x$, do đó $y = z \in G \cap F^0 = \{0\}$ và $y = 0$. Vậy không gian con $G'$ trả lời câu hỏi.

#### Hệ quả 1 {#alg-ix-s4-prop-2-cor-1 .statement}

*Nếu F là một không gian con hoàn toàn đẳng hướng (tương ứng, hoàn toàn kỳ dị) có chiều r, thì tồn tại một không gian con hoàn toàn đẳng hướng (tương ứng, hoàn toàn kỳ dị) F' có chiều r sao cho $F \cap F' = \{0\}$ và $F + F'$ là không đẳng hướng.*

Chỉ cần lấy $G = \{0\}$ trong mệnh đề 2, b).

#### Hệ quả 2 {#alg-ix-s4-prop-2-cor-2 .statement}

*Hai dạng $\varepsilon$-Hermit trung hòa trên các không gian có cùng chiều trên A là tương đương.*

#### Nhận xét {#alg-ix-s4-n2-rem-1 .statement}

Trong các điều kiện của Hệ quả 1, E là tổng trực tiếp của $F + F'$ và trực giao của $F + F'$. Do đó ta có một phân tích Witt của E. Theo mệnh đề 2, a), tồn tại các cơ sở của F và F’ sao cho, trong ma trận (1) của $\Phi$, khối $U$ là ma trận đơn vị $1_r$.

#### Mệnh đề 3 {#alg-ix-s4-prop-3 .statement}

*Cho $\Phi$ là một dạng $\varepsilon$-Hermit không suy biến thỏa mãn (T) (tương ứng, dạng song tuyến tính liên kết với một dạng toàn phương không suy biến Q). Gọi $F_1$ và $F_2$ là hai không gian con cực đại hoàn toàn đẳng hướng (tương ứng, hoàn toàn kỳ dị) của E, trong đó một không gian là hữu hạn chiều. Đặt $F = F_1 \cap F_2$. Gọi $S_i \ (i = 1, 2)$ là một không gian con bù của $F$ trong $F_i$; đặt $S = S_1 + S_2$. Khi đó tồn tại hai không gian con G và H của E sao cho
a) Các không gian con $G + F, S$ và H là không đẳng hướng và trực giao từng đôi một;
b) E là tổng trực tiếp của F, S, G và H;
c) Không có vectơ đẳng hướng (tương ứng, kỳ dị) khác không nào trong H;
d) G là hoàn toàn đẳng hướng (tương ứng, hoàn toàn kỳ dị).
Hơn nữa $F_1$ và $F_2$ đều hữu hạn chiều và ta có dim $F_1 = \dim F_2, \dim G = \dim F, \dim S_1 = \dim S_2, \operatorname{codim} H = 2 \dim F_1$.

Trước hết hãy nhận thấy rằng, nếu $N$ là một không gian con cực đại hoàn toàn đẳng hướng (tương ứng, hoàn toàn kỳ dị), thì mọi vectơ đẳng hướng (tương ứng, kỳ dị) $x$ trực giao với $N$ đều là một phần tử của $N$, vì nếu không thì $N + Ax$ sẽ mâu thuẫn với tính chất cực đại của $N$. Vậy nếu, với $i = 1,\ 2,\ x_i$ là một vectơ đẳng hướng (tương ứng, kỳ dị) của $F_i^0$, thì ta có $x_i \in F_i$. Mặt khác, nếu $y$ là một phần tử của $S_1$ trực giao với $S_2$, thì nó trực giao với $F_1$ vì $F_1$ là hoàn toàn đẳng hướng, do đó trực giao với $F$, và vì thế trực giao với $F_2 = S_2 + F$. Vì $y$ là đẳng hướng (tương ứng, kỳ dị) và trực giao với $F_2$, nên ta có

$$
y \in S_1 \cap F_2 = S_1 \cap F_1 \cap F_2 = S_1 \cap F = \{0\}.
$$

Do đó ta có $S_1 \cap S_2^0 = \{0\}$, và tương tự $S_2 \cap S_1^0 = \{0\}$. Vì một trong hai không gian con $F_1, F_2$, chẳng hạn $F_1$, là hữu hạn chiều, nên $S_1$ là hữu hạn chiều, và do đó $S_1^0$ có đối chiều hữu hạn ($§ 1, \mathrm{n}^\circ 6, \mathrm{cor.\ 1\ de\ la\ prop.\ 4}$), và suy ra $S_2$ là hữu hạn chiều vì $S_2 \cap S_1^0 = \{0\}$; hơn nữa điều này cho thấy rằng $\dim S_2 \leqslant \operatorname{codim} S_1^0 = \dim S_1$; tương tự $\dim S_1 \leqslant \dim S_2$, do đó $\dim S_1 = \dim S_2$. Mệnh đề 2 a) khi đó cho thấy rằng $S = S_1 + S_2$ là không đẳng hướng.

Bây giờ trực giao $N$ của $S$ là không đẳng hướng ($\mathrm{n}^\circ 1, \mathrm{cor.\ de\ la\ prop.\ 1}$) và chứa $F$; do đó Hệ quả 1 của Mệnh đề 2 cho thấy rằng tồn tại một không gian con $G$ hoàn toàn đẳng hướng (tương ứng hoàn toàn kỳ dị) của $N$ sao cho $\dim G = \dim F$, $G \cap F = \{0\}$ và $G + F$ là không đẳng hướng. Vậy d) được thỏa mãn bởi $G$. Khi đó ta sẽ thỏa mãn a) và b) bằng cách lấy đối với $H$ trực giao của $G + F$ trong $N$. Còn đối với c), ta chú ý rằng, vì $H$ trực giao với $F_1 = S_1 + F$, nên không có vectơ đẳng hướng (tương ứng kỳ dị) khác không nào trong $H$ theo điều đã được ghi nhận ở đầu chứng minh và từ việc $H \cap F_1 = \{0\}$. Sau cùng một số mệnh đề về các chiều đã được chứng minh trong quá trình lập luận; các mệnh đề khác suy ra từ đó một cách hiển nhiên.

#### Hệ quả 1 {#alg-ix-s4-prop-3-cor-1 .statement}

Dưới các giả thiết của Mệnh đề 3, hai không gian con hoàn toàn đẳng hướng cực đại (tương ứng hoàn toàn kỳ dị cực đại) hữu hạn chiều có cùng chiều. Với mọi không gian con hoàn toàn đẳng hướng cực đại (tương ứng hoàn toàn kỳ dị cực đại) F hữu hạn chiều, tồn tại một F' khác sao cho F ∩ F' = {0}, và trong các điều kiện ấy F + F' là không đẳng hướng.

Nếu F ∩ F' = {0}, ta sẽ có G = {0} theo ký hiệu của Mệnh đề 3, và F + F' sẽ không đẳng hướng. Các mệnh đề khác suy ra hiển nhiên từ Mệnh đề 3 và Hệ quả 1 của Mệnh đề 2.

#### Hệ quả 2 {#alg-ix-s4-prop-3-cor-2 .statement}

Cho Q là một dạng toàn phương không suy biến trên một không gian vectơ E hữu hạn chiều n trên một trường đóng đại số A; khi đó tồn tại một cơ sở (e_i)_{1 \leq i \leq n} của E sao cho

(2)
$$
Q(\sum_{i=1}^{n} x_i e_i) = \sum_{i=1}^{\nu} x_i x_{i+\nu} \qquad si\ n = 2\nu,
$$

(3)
$$
Q(\sum_{i=1}^{n} x_i e_i) = \sum_{i=1}^{\nu} x_i x_{i+\nu} + x_{2\nu+1}^2 \qquad si\ n = 2\nu + 1.
$$

Thật vậy, cho $F_1$ và $F_2$ là hai không gian con hoàn toàn kỳ dị cực đại sao cho F_1 ∩ F_2 = {0} (Hệ quả 1) và gọi q là chiều của chúng. Khi đó ta có G = {0} theo ký hiệu của Mệnh đề 3. Lấy một cơ sở (e_i)_{1 \leq i \leq q} của F_1 và một cơ sở (e_i)_{q+1 \leq i \leq 2q} của F_2 sao cho Φ(e_i, e_{j+q}) = δ_{ij} với i, j = 1, ..., q (Mệnh đề 2 a)), ta thấy rằng chỉ cần chứng minh dim H ≤ 1. Bây giờ, nếu x ∈ H, y ∈ H và nếu x ≠ 0, phương trình Q(y - ax) = Q(y) - aΦ(x, y) + a^2 Q(x) = 0 có ít nhất một nghiệm a_0 vì Q(x) ≠ 0, và ta có y = a_0 x vì mọi vectơ kỳ dị của H đều bằng không.

#### Định nghĩa 3 {#alg-ix-s4-def-3 .statement}

Giả sử rằng E là hữu hạn chiều và Φ là một dạng ε-Hermit không suy biến thỏa mãn (T) (tương ứng dạng song tuyến tính liên kết với một dạng toàn phương không suy biến Q). Ta gọi chỉ số của Φ (tương ứng của Q) là chiều chung của các không gian con hoàn toàn đẳng hướng cực đại (tương ứng hoàn toàn kỳ dị cực đại) của E.

Nếu n là chiều của E và ν là chỉ số của Φ (tương ứng Q), Mệnh đề 3 cho thấy rằng

(4)
$$
n \geq 2\nu.
$$

Hơn nữa, vì mọi không gian con hoàn toàn đẳng hướng (tương ứng hoàn toàn kỳ dị) đều được chứa trong một không gian con hoàn toàn đẳng hướng cực đại (tương ứng hoàn toàn kỳ dị cực đại), nên các không gian con hoàn toàn đẳng hướng (tương ứng hoàn toàn kỳ dị) là cực đại chính là những không gian có chiều $v$. Mệnh đề rằng $\Phi$ (tương ứng Q) có chỉ số 0 có nghĩa là mọi vectơ đẳng hướng (tương ứng kỳ dị) của E đều bằng không. Trong một không gian có chiều chẵn $n$, các dạng trung hòa là những dạng có chỉ số $\frac{1}{2}n$; không có dạng trung hòa nào trong một không gian có chiều lẻ. Mệnh đề 3 cho thấy rằng mọi dạng đều là tổng trực tiếp của một dạng trung hòa và một dạng có chỉ số 0.

#### Mệnh đề 4 {#alg-ix-s4-prop-4 .statement}

*Cho một dạng toàn phương không suy biến Q trên E sao cho tồn tại một vectơ $x \neq 0$ của E sao cho $Q(x) = 0$, thì với mọi phần tử a của A, tồn tại $y \in E$ sao cho $Q(y) = a$.*

Thật vậy, theo Hệ quả 1 của Mệnh đề 2, tồn tại một không gian con $G = F + F'$ ($F, F'$: các không gian con hoàn toàn kỳ dị có chiều 1) của E, có chiều 2, sao cho hạn chế của Q lên G là trung hòa. Nếu $\{ e, e' \}$ ($e \in F, e' \in F'$) là một cơ sở của G, ta có
$$
Q(xe + x'e') = bxx' \quad (x \in A, x' \in A, b \in A, b \neq 0).
$$
Vì vậy chỉ cần lấy đối với $y$ vectơ $ae + b^{-1}e'$.

### 3. Định lý Witt.

Cho hai không gian vectơ E, $E'$ trên A được trang bị tương ứng với hai dạng sesquilinear $\Phi, \Phi'$ (tương ứng với hai dạng toàn phương Q, $Q'$), một *đồng cấu metric* từ E vào $E'$ là mọi ánh xạ tuyến tính $u$ từ E vào $E'$ sao cho $\Phi'(u(x), u(y)) = \Phi(x, y)$ (tương ứng $Q'(u(x)) = Q(x)$) với $x \in E, y \in E$. Nếu E và $E'$ có cùng số chiều hữu hạn và nếu $\Phi$ (tương ứng Q) không suy biến, thì mọi đồng cấu metric $u$ từ E vào $E'$ đều là một đẳng cấu, vì $u(x) = 0$ kéo theo $\Phi(x, y) = 0$ với mọi $y \in E$, do đó $x = 0$; vì thế $u$ là đơn ánh, nên song ánh vì E và $E'$ có cùng số chiều hữu hạn.

**Định lý 1** (Witt). — *Cho E và $E'$ là hai không gian vectơ có số chiều hữu hạn, được trang bị tương ứng với hai dạng $\varepsilon$-Hermit không suy biến $\Phi$ và $\Phi'$ thỏa mãn điều kiện (T) của No. 2* (tương ứng với hai dạng toàn phương không suy biến Q và Q'), và đẳng cấu đối với các cấu trúc ấy. Với một không gian con tùy ý F của E, mọi đồng cấu metric đơn ánh từ F vào E' đều mở rộng được thành một đẳng cấu metric từ E lên E'.

Dùng đẳng cấu đã cho từ E lên E', ta thấy rằng chỉ cần chứng minh rằng mọi đồng cấu metric đơn ánh u từ F vào E đều mở rộng được thành một tự đẳng cấu metric của E. Ta nhận xét rằng nếu, với i = 1, 2, $F_i$ là một không gian con của E và $u_i$ là một đồng cấu metric từ $F_i$ vào E, sao cho $F_1 \cap F_2 = {0}$ và $\Phi(u_1(x_1), u_2(x_2)) = \Phi(x_1, x_2)$ với $x_i \in F_i$ (i = 1, 2), thì đồng cấu ψ : $x_1 + x_2 \to u_1(x_1) + u_2(x_2)$ từ $F_1 + F_2$ vào E kéo dài $u_1$ và $u_2$ là metric: thật vậy, với mọi $x_i, y_i$ trong $F_i$ (i = 1, 2), khai triển của mỗi biểu thức $\Phi(x_1 + x_2, y_1 + y_2)$ và $\Phi(u_1(x_1) + u_2(x_2), u_1(y_1) + u_2(y_2))$ (tương ứng $Q(x_1 + x_2)$ và $Q(u_1(x_1) + u_2(x_2))$) chứa bốn (tương ứng ba) hạng tử bằng nhau từng đôi một theo các giả thiết đã đặt ra. Hơn nữa, nếu $u_1$ và $u_2$ là đơn ánh và nếu $u_1(F_1) \cap u_2(F_2) = {0}$, thì ψ là đơn ánh.

1) Trước hết ta chứng minh định lý Witt trong trường hợp tập hợp các phần tử bất biến bởi u là một siêu phẳng U của F. Khi đó tập hợp các vectơ có dạng $u(x) − x$ với $x ∈ F$ là một D phải. Nếu F' là một không gian con trực giao với D sao cho $F' ∩ F = F' ∩ u(F) = {0}$, thì ta sẽ có $\Phi(u(x), y) = \Phi(x, y)$ với $x ∈ F$ và $y ∈ F'$; do đó nhận xét ban đầu của ta áp dụng được cho u và cho ánh xạ đồng nhất từ F' vào E, và chỉ ra rằng u mở rộng được lên $F + F'$ bằng cách giữ cố định các điểm của F'; tập hợp các vectơ có dạng $u(x) − x$ ($x ∈ F + F'$) vẫn là D phải. Bây giờ, với $x ∈ F, y ∈ F$ ta có

(5) $\Phi(u(x), u(y) - y) = \Phi(u(x), u(y)) - \Phi(u(x), y) = \Phi(x - u(x), y)$,

điều này, khi $x ∈ U$ (nghĩa là khi $u(x) = x$), cho thấy rằng $x ∈ D^0$; nói cách khác ta có $U ⊂ D^0$. Ta sẽ phân biệt hai trường hợp:

a) $F \not\subset D^0$. Công thức (5) cho thấy rằng $u(F)$ không được chứa trong $D^0$, do đó $F \cap D^0 = u(F) \cap D^0 = U$. Khi đó có thể lấy cho F' một không gian con bù của U trong $D^0$; vì $F + F'$ chứa siêu phẳng $D^0$ và khác nó, nên ta có $F + F' = E$, và trong trường hợp này ta đã tìm được phép mở rộng cần thiết của u lên E.

b) F ⊂ D^0. Công thức (5) cho thấy rằng u(F) ⊂ D^0, và do đó

D ⊂ D^0 ; vì thế D phải là đẳng hướng (tương ứng kỳ dị, vì ta có $Q(u(x) − x) = Q(u(x)) − Φ(x, u(x)) + Q(x) = 2Q(x) − Φ(x, x) = 0$ với $x ∈ F$). Ta sẽ chỉ ra rằng, dưới các điều kiện này, tồn tại một không gian con F' của $D^0$ bù cho F và u(F) trong $D^0$. Điều này là ngay lập tức nếu F = u(F). Nếu không, lấy x và y là các vectơ sao cho $x ∈ F, x ∉ U, y ∈ u(F), y ∉ U$; khi đó ta có $F = U + Ax, u(F) = U + Ay$, và F không chứa $x + y$ vì nếu không thì $y = (x + y) − x$ sẽ thuộc $F ∩ u(F) = U$; tương tự ta thấy rằng $x + y$ không thuộc u(F); do đó A phải $(x + y)$ bù cho F và u(F) trong không gian con $F + u(F)$; khi đó chỉ cần đặt $F' = A(x + y) + G$ trong đó G bù cho $F + u(F)$ trong $D^0$. Khi đó, ta có $F + F' = u(F) + F' = D^0$, và, trong trường hợp này, điều đã nói ở đầu 1) cho thấy rằng tồn tại một phép mở rộng của u lên siêu phẳng $D^0$ của E, và $D^0$ ổn định đối với phép mở rộng này.

Vì vậy ta được đưa về trường hợp F là siêu phẳng $D^0$ và u là một tự đẳng cấu của F. Ta chứng minh rằng, với mọi $z ∈ E$, tồn tại $z' ∈ E$ sao cho

(6)
$$
\Phi(u(x), z') = \Phi(x, z)
$$
với mọi x ∈ F; thật vậy dạng tuyến tính $x → Φ(u^{-1}(x), z)$ trên F là hạn chế của một dạng tuyến tính trên E, một dạng có kiểu $x → Φ(x, z')$ vì Φ không suy biến; do đó (6) đúng. Hơn nữa, nếu $z ∉ F$, thì tồn tại một vectơ $z' ∈ E$ thỏa mãn (6) và sao cho $\Phi(z', z') = \Phi(z, z)$ (tương ứng $Q(z') = Q(z)$): thật vậy công thức (6) vẫn còn đúng nếu ta cộng vào z' một phần tử $u(y) − y$ ($y ∈ F$) của D vì $F = D^0$, và Bổ đề 1 của No. 2 cho phép kết luận vì z không trực giao với D. Nhận xét ban đầu của ta khi đó cho thấy rằng tồn tại một đồng cấu metric ϕ từ $F + Az = E$ vào E mở rộng u và biến đổi z thành z'. Vì Φ không suy biến, ϕ là tự đẳng cấu metric cần tìm của E.

2) Trong trường hợp tổng quát, ta lập luận bằng quy nạp theo $r = dim F$. Trường hợp $r = 0$ là tầm thường. Giả sử khi đó $r > 0$, nghĩa là $F ≠ {0}$, và gọi U là một siêu phẳng của F. Hạn chế $u_0$ của u lên U, theo giả thiết quy nạp, mở rộng được thành một tự đẳng cấu metric $\varphi_0$ của E. Nếu $\varphi_0$ mở rộng u, thì định lý được chứng minh. Nếu không, U là tập hợp các phần tử bất biến bởi $v_0^{-1}u$, và tồn tại, theo 1), một tự đẳng cấu metric $v_1$ của E mở rộng $v_0^{-1}u$. Tự đẳng cấu $v_0v_1$ khi đó là phép mở rộng cần thiết của u. QED.

#### Hệ quả 1 {#alg-ix-s4-prop-4-cor-1 .statement}

Cho, với i = 1, 2, $E_i$ là một không gian vectơ hữu hạn chiều, $\Phi_i$ là một dạng $\varepsilon$-Hermit không suy biến trên $E_i$ thỏa mãn (T) (tương ứng $Q_i$ là một dạng toàn phương không suy biến trên $E_i$), $E'_i$ và $E''_i$ là hai không gian con trực giao của $E_i$ mà tổng trực tiếp là $E_i$. Nếu các dạng $\Phi_1$ và $\Phi_2$ (tương ứng $Q_1$ và $Q_2$) là tương đương, và nếu các hạn chế của chúng lên $E'_1$ và $E'_2$ là tương đương, thì điều tương tự cũng đúng đối với các hạn chế của chúng lên $E''_1$ và $E''_2$.

Thật vậy, cho $u$ là một đẳng cấu metric từ $E'_1$ lên $E'_2$. Theo Định lý 1, $u$ kéo dài thành một đẳng cấu metric $\varphi$ từ $E_1$ lên $E_2$. Vì $\Phi_i$ không suy biến, $E''_i$ là trực giao của $E'_i$ trong $E_i$, do đó $\varphi$ ánh xạ $E''_1$ lên $E''_2$. Điều phải chứng minh.

#### Hệ quả 2 {#alg-ix-s4-prop-4-cor-2 .statement}

Với các giả thiết của Định lý 1, nhóm các tự đẳng cấu metric của E tác động bắc cầu trên các không gian con hoàn toàn đẳng hướng (tương ứng hoàn toàn kỳ dị) có chiều cho trước của E. Hơn nữa, nếu F là một không gian con hoàn toàn đẳng hướng (tương ứng hoàn toàn kỳ dị) của E, mọi ánh xạ tuyến tính song ánh từ F lên F đều được cảm sinh bởi một tự đẳng cấu metric của E.

#### Hệ quả 3 {#alg-ix-s4-prop-4-cor-3 .statement}

Cho Q là một dạng toàn phương không suy biến trên một không gian vectơ hữu hạn chiều E trên một trường đóng đại số A. Nhóm các tự đẳng cấu metric của E tác động bắc cầu trên các không gian con không đẳng hướng có chiều cho trước của E.

Điều này suy ra ngay lập tức từ Định lý 1 và Hệ quả 2 của Mệnh đề 3.

Bài tập. — 1) a) Cho K là một trường có đặc số 2, J : ξ → ¯ξ là một phản tự đẳng cấu đối hợp của K, Z là tâm của K. Chứng minh rằng nếu hạn chế của J lên Z không phải là đồng nhất, thì mọi phần tử μ của K sao cho ¯μ = μ đều có dạng λ + ¯λ (hãy nhận xét rằng tồn tại một phần tử ρ ≠ 0 trong Z có thể viết dưới dạng ζ + ¯ζ, với ζ ∈ Z); khi đó mọi dạng Hermit trên một không gian vectơ trên K đều thỏa mãn điều kiện (T).

b) Cho các ví dụ về những trường có đặc số 2, thừa nhận một phản tự đẳng cấu đối hợp ξ → ¯ξ khác với ánh xạ đồng nhất, và đối với đó tồn tại các phần tử $\mu = \bar{\mu}$ không có dạng $\lambda + \bar{\lambda}$ (xem Chương VIII, § 11, Bài tập 4).

2) Cho A là một trường, E là một không gian vectơ trên A, $\Phi$ (tương ứng Q) là một dạng $\varepsilon$-Hermit không suy biến trên E, thỏa mãn điều kiện (T) (tương ứng một dạng toàn phương không suy biến trên E, khi đó Φ ký hiệu dạng song tuyến tính đối xứng liên kết với Q).

a) Chứng minh rằng để một mặt phẳng P \subset E là đẳng hướng (tương ứng kỳ dị) mà không hoàn toàn đẳng hướng (tương ứng không hoàn toàn kỳ dị), điều kiện cần và đủ là nó chỉ chứa một đường thẳng đẳng hướng (tương ứng kỳ dị) duy nhất (xem Bài tập 14 e)).

b) Giả sử rằng dim $E \geqslant 3$, và rằng trong E tồn tại các vectơ đẳng hướng $\neq 0$. Chứng minh rằng nếu P là một mặt phẳng không hoàn toàn đẳng hướng trong E, thì tồn tại một không gian con vectơ không đẳng hướng V \subset E, có chiều 3, chứa các vectơ đẳng hướng $\neq 0$, và sao cho $P \subset V$.

3) Với các giả thiết như trong Bài tập 2, chứng minh rằng nếu dim $E \geqslant 3$, mọi đường thẳng đẳng hướng trong E đều là giao của hai mặt phẳng không đẳng hướng.

4) Các giả thiết là các giả thiết của Bài tập 2, và giả sử thêm rằng E là hữu hạn chiều.

a) Nếu chỉ số $\nu$ của $\Phi$ (tương ứng Q) là $\geqslant 1$, chứng minh rằng với mọi vectơ đẳng hướng (tương ứng kỳ dị) $a \neq 0$ trong E, tồn tại một cơ sở $(e_i)$ của E gồm các vectơ đẳng hướng (tương ứng kỳ dị), sao cho $e_1 = a$ (xem Bài tập 14 e)).

b) Cho V, W là hai không gian con hoàn toàn đẳng hướng (tương ứng hoàn toàn kỳ dị) cùng chiều $r \leqslant \nu$; chứng minh rằng tồn tại hai không gian con hoàn toàn đẳng hướng cực đại (tương ứng hoàn toàn kỳ dị cực đại) $V_1, W_1$, sao cho V \subset $V_1$, W \subset $W_1$, và $V_1 \cap W_1 = V \cap W$. (Nếu $U = V \cap W$, hãy lập luận trong $U^0/U$).

c) Cho V, W, $V_1, W_1$ là bốn không gian con hoàn toàn đẳng hướng (tương ứng hoàn toàn kỳ dị) cùng chiều, sao cho $V + W$ và $V_1 + W_1$ là không đẳng hướng. Chứng minh rằng tồn tại một tự đẳng cấu metric $u$ của E sao cho $u(V) = V_1$ và $u(W) = W_1$.

d) Cho $f$ là một dạng tuyến tính trên E, $\alpha$ là một phần tử của A có dạng $\lambda + \varepsilon \bar{\lambda}$ (tương ứng một phần tử của $\Lambda$). Xét dạng sesquilinear trên E

$$
(x, y) \to \Phi_1(x, y) = \Phi(x, y) + f(x)\overline{\alpha f(y)}
$$

(tương ứng dạng toàn phương

$$
x \to Q_1(x) = Q(x) + \alpha(f(x))^2).
$$

Chứng minh rằng nếu $\Phi_1$ (tương ứng $Q_1$) không suy biến và nếu $\nu_1$ ký hiệu chỉ số của nó, thì ta có $|\nu_1 - \nu| \leqslant 1$.

5) a) Cho B là một vành, $\xi \to \bar{\xi}$ là một phản tự đẳng cấu đối hợp của B, $\varepsilon$ là một phần tử của tâm của B sao cho $\varepsilon \bar{\varepsilon} = 1$. Chứng minh rằng nếu $\beta$ là một phần tử khả nghịch của B sao cho $\beta + \varepsilon \bar{\beta} \neq 0$, thì tồn tại một phần tử khả nghịch $\mu \neq 1$ trong B, sao cho $\mu(\beta + \varepsilon \bar{\beta})\mu = \beta + \varepsilon \bar{\beta}$. (Chứng minh rằng có thể lấy $\mu$ sao cho $\mu \beta \bar{\mu} = \beta$).

b) Cho A là một trường, E là một không gian vectơ trên A, $\Phi$ là một dạng sesquilinear $\varepsilon$-Hermit không suy biến trên E, thỏa mãn (T). Chứng minh rằng nếu $\Phi$ không phản xứng, thì với mọi siêu phẳng không đẳng hướng $H$ của E, tồn tại một tự đẳng cấu metric của E, khác với ánh xạ đồng nhất, để bất biến mọi phần tử của $H$ (dùng a).

6) Với các giả thiết của Bài tập 2, cho $a$ là một vectơ đẳng hướng $\neq 0$ trong $E$ (tương ứng một vectơ đẳng hướng không kỳ dị (chú ý rằng các vectơ như vậy chỉ tồn tại nếu $A$ có đặc số 2)). Cho $\lambda \in A$ sao cho $\lambda + \varepsilon \bar{\lambda} = 0$ (tương ứng $\lambda = (Q(a))^{-1}$); chứng minh rằng phép chuyển vị $x \to x + \Phi(x, a)\lambda a$ (Chương II, § 6, Bài tập 7) là một tự đẳng cấu metric của $E$; đảo lại.

7) Với các giả thiết như trong Bài tập 2, gọi $G$ là nhóm các tự đẳng cấu metric của $E$. Hãy chứng minh rằng các song ánh nửa tuyến tính duy nhất của $E$ lên chính nó giao hoán với mọi phần tử của $G$ là các phép vị tự của $E$, trừ trong ba trường hợp sau: dim $E = 2$, $G$ là nhóm các tự đẳng cấu metric tương ứng với một dạng toàn phương có chỉ số 1 trên $E$, và $A$ là một trong ba trường $\mathbf{F}_2, \mathbf{F}_3$ hoặc $\mathbf{F}_4$. (Dùng các Bài tập 5, 6 và 3; xét riêng trường hợp một dạng toàn phương trên một không gian vectơ chiều 2).

*8) Cho $A$ là một trường, $E$ là một không gian vectơ hữu hạn chiều $> 0$ trên $A$, $\Phi$ là một dạng sesquilinear $\varepsilon$-Hermit không suy biến trên $E$, thỏa mãn (T). Gọi $M(\Phi)$ là nhóm các nhân tử của các phép đồng dạng của $E$ đối với $\Phi$ ($§ 6, \mathrm{n}^o\ 5$).

a) Cho $V_1, V_2$ là hai không gian con vectơ của $E$, có cùng chiều, và gọi $\Phi_1, \Phi_2$ lần lượt là các hạn chế của $\Phi$ lên $V_1, V_2$. Để tồn tại một phép đồng dạng $u$ sao cho $u(V_1) = V_2$, điều kiện cần và đủ là tồn tại $\alpha \in M(\Phi)$ sao cho $\Phi_2$ tương đương với $\alpha \Phi_1$ (dùng định lý Witt).

b) Cho $(F, F', G)$ là một phân tích Witt của $E$ ($\mathrm{n}^o\ 2$), và gọi $\Phi_0$ là hạn chế của $\Phi$ lên không gian con không đẳng hướng $G$. Hãy chứng minh rằng $M(\Phi) = M(\Phi_0)$ nếu $G \neq \{0\}$. (Dùng định lý Witt và Mệnh đề 2 của $\mathrm{n}^o\ 2$).

c) Bây giờ chứng minh rằng nếu chỉ số $v$ của $\Phi$ sao cho dim $E = 2v$, thì $M(\Phi)$ là nhóm các phần tử $\zeta \neq 0$ của tâm của $A$ sao cho $\bar{\zeta} = \zeta$. Nếu dim $E = 2v + 1$, thì $M(\Phi)$ là nhóm các phần tử có dạng $\rho \bar{\rho}$, trong đó $\rho$ chạy qua nhóm nhân của các phần tử $\neq 0$ của tâm của $A$ (dùng định lý Witt). (Xem § 10, bài tập 18).*

*9) Cho $A$ là một trường giao hoán, $E$ là một không gian vectơ trên $A$, $Q$ là một dạng toàn phương không suy biến trên $E$. Một phép đồng dạng đối với $Q$ là mọi tự đẳng cấu $u$ của $E$ sao cho tồn tại một phần tử $\alpha \neq 0$ của $A$ mà $Q(u(x)) = \alpha Q(x)$ với mọi $x \in E$; khi đó $u$ cũng là một phép đồng dạng đối với dạng song tuyến tính liên kết với $Q$. Giả sử chiều của $E$ là hữu hạn và $> 0$, hãy phát biểu và bài tập chứng minh, đối với các phép đồng dạng tương đối với $Q$, các kết quả tương tự của bài tập 8.*

*10) Cho $A$ là một trường, $E$ là một không gian vectơ trên $A$ có chiều $> 2$, $\Phi_1$ (tương ứng $\Phi_2$) là một dạng sesquilinear không suy biến $\varepsilon_1$-Hermit (tương ứng $\varepsilon_2$-Hermit) trên $E$ đối với một phản tự đẳng cấu đối hợp $J_1$ (tương ứng $J_2$) của $A$, thỏa mãn điều kiện (T). Bây giờ chứng minh rằng nếu nhóm các tự đẳng cấu metric của $E$ đối với $\Phi_1$ là một nhóm con của nhóm các phép đồng dạng đối với $\Phi_2$, thì tồn tại $\alpha \in A$ sao cho $\Phi_2 = \Phi_1 \alpha$ (dùng bài tập 5 b) và 6).

Bài tập chứng minh tính chất tương tự khi A được giả sử là giao hoán, và khi $\Phi_1$ và $\Phi_2$ được thay thế trong mệnh đề bởi hai dạng toàn phương không suy biến $Q_1, Q_2$ trên E.*

11) Cho A là một vành, J là một phản tự đẳng cấu đối hợp của A, E là một A-môđun có một cơ sở hữu hạn $(e_i)$, $\Phi$ là một dạng $\varepsilon$-Hermit không suy biến trên E, R là ma trận của $\Phi$ đối với $(e_i)$; nhóm các tự đẳng cấu metric của $\Phi$ được đồng nhất với nhóm G các ma trận khả nghịch U sao cho $^tU . R . U^j = R$.

a) Giả sử rằng tồn tại một ma trận P sao cho $R = ^tP + \varepsilon P^j$. Bây giờ chứng minh rằng với mọi ma trận S sao cho $^tS + \varepsilon S^j = 0$, và sao cho $P + S$ khả nghịch, thì $U = (^tP^j - \varepsilon^j S)^{-1}(P + S)$ thuộc về G, và $\varepsilon I + U$ khả nghịch. Ngược lại (chứng minh rằng với mọi ma trận $U \in G$ sao cho $\varepsilon I + U$ khả nghịch, ta có

$$
\varepsilon(\varepsilon I + ^tU)^{-1}R + \varepsilon^j R (\varepsilon^j I + U^j)^{-1} = R.
$$

b) Chứng minh rằng điều kiện trong a) được thỏa mãn khi $\Phi$ thỏa mãn điều kiện (T). Trường hợp trong A phương trình $2\xi = \alpha$ có một và chỉ một nghiệm với mọi $\alpha \in A$.

¶ 12) Cho A là một trường giao hoán, E là một không gian vectơ hữu hạn chiều có chiều n trên A, $\Phi$ là một dạng sesquilinear $\varepsilon$-Hermit không suy biến trên E.

a) Cho u là một tự đồng cấu của E; chứng tỏ rằng nếu các $r_i (1 \leq i \leq m)$ là các bất biến tương tự của u (Chương VII, § 5, No. 1, Định nghĩa 1), thì các bất biến tương tự của liên hợp $u^*$ của u đối với $\Phi$ là các đa thức $\bar{r}_i (1 \leq i \leq m)$, trong đó $\bar{r}_i$ thu được từ $r_i$ bằng cách áp dụng tự đẳng cấu J cho mỗi hệ số (xem Chương VII, § 5, bài tập 2). Với mọi đa thức bất khả quy đơn nhất $p \in A[X]$ chia đa thức tối tiểu của u, gọi $F_k(u, p)$ là hạt nhân của $(p(u))^k$ trong E, và gọi $F(u, p)$ là hợp của các $F_k(u, p)$ với mọi số nguyên $k > 0$. Chứng tỏ rằng nếu p và q là các đa thức bất khả quy đơn nhất phân biệt chia đa thức tối tiểu của u, thì các không gian con $F(u, p)$ và $F(u^*, \bar{q})$ trực giao với nhau (dùng đồng nhất thức Bezout). Sau cùng, nếu G là một không gian con vectơ của E sao cho $u(G) \subset G$, thì ta có $u^*(G^0) \subset G^0$.

b) Giả sử rằng $uu^* = u^*u$ (trường hợp khi đó u được gọi là một tự đồng cấu chuẩn đối với $\Phi$; xem § 7, No. 3); chứng tỏ rằng khi đó ta có $u^*(F_k(u, p)) \subset F_k(u, p)$ với mọi k, và do đó $u^*(F(u, p)) \subset F(u, p)$. Nếu đặt $G(p, \bar{q}) = F(u, p) \cap F(u^*, \bar{q})$, hãy chứng tỏ rằng E là tổng trực tiếp của các không gian con $G(p, \bar{q})$, và rằng $G(p, \bar{q})$ và $G(p_1, \bar{q}_1)$ trực giao với nhau nếu $p \neq q_1$ hoặc nếu $p_1 \neq q$; đặc biệt $G(p, \bar{q})$ là hoàn toàn đẳng hướng nếu $p \neq q$. Chứng tỏ rằng $G(p, \bar{p})$ thu về 0 hoặc là không đẳng hướng, và rằng nếu $p \neq q$, không một vectơ khác không nào của $G(p, \bar{q})$ trực giao với $G(q, \bar{p})$ (dùng sự kiện $\Phi$ là không suy biến); suy ra rằng nếu $p \neq q$, $G(p, \bar{q})$ và $G(q, \bar{p})$ là các không gian con hoàn toàn đẳng hướng có cùng chiều, và rằng $G(p, \bar{q}) + G(q, \bar{p})$ là không đẳng hướng.

c) Giả sử rằng $J$ không phải là đồng nhất hoặc rằng $A$ không có đặc số 2, và rằng $u^* = u$. Gọi $\mathcal{M}$ là tập hợp các không gian con không đẳng hướng $M \subset G(p, \bar{p})$, ổn định dưới $u$ (do đó là các môđun con của $A[X]$-môđun $E_u$ (Chương VII, § 5, No. 1)). Bây giờ chứng minh rằng nếu $M$ là một phần tử cực tiểu của $\mathfrak{M}$, thì $M$ là một môđun con *không phân tích được* của $E_u$ (Chương VII, § 4, No. 7). (Giả sử rằng $M$ là tổng trực tiếp của một môđun con không phân tích được $M_1$ và một môđun con $M_2 \neq \{0\}$, các đa thức tối tiểu $p^h$ và $p^k$ của các hạn chế của $u$ lên $M_1$ và $M_2$ tương ứng thỏa mãn $h \geq k$. Khi đó hãy nhận xét rằng $M_1$ tất yếu là đẳng hướng và rằng mọi $z \neq 0$ trong $M_1$ sao cho $p(u).z = 0$ đều trực giao với $M_1$ (dùng sự kiện rằng mọi môđun con của $M_1$ đều đơn sinh); viết $z = (p(u))^{h-1}.x$ và rằng $z$ không trực giao với $M_2$, rồi suy ra rằng tất yếu $k = h$. Bây giờ chứng minh rằng tồn tại một môđun con không phân tích được $N_2$ của $M_2$ sao cho $p^h$ là đa thức tối tiểu của hạn chế của $u$ lên $N_2$, và rằng $M_1 + N_2$ là không đẳng hướng; kết luận rằng $M_2 = N_2$. Cuối cùng, nếu $y \in M_2$ không trực giao với $z$, hãy xét môđun con $P$ của $M$ sinh bởi $w = x + \lambda y$, trong đó $\lambda \in \mathbf{A}$, và chứng minh rằng có thể chọn $\lambda$ sao cho $P$ là không đẳng hướng, bằng cách chứng minh rằng $\Phi((p(u))^{h-1}.w, w) \neq 0$; điều này dẫn đến một mâu thuẫn).

d) Suy ra từ c) rằng $G(p, \overline{p})$ là tổng trực tiếp của các môđun con không phân tích được $H_i$ trực giao từng đôi một. Nếu $p^h$ là đa thức tối tiểu của hạn chế của $u$ lên $H_i$, và nếu $d$ là bậc của $p$, hãy chứng minh rằng tồn tại trong $H_i$ một không gian con hoàn toàn đẳng hướng có chiều $d.[h/2]$. Trường hợp $E$ không chứa vectơ đẳng hướng nào $\neq 0$ (xem § 7, No. 3).

e) Phát biểu và chứng minh các tính chất tương tự với các tính chất của c) và d) khi $u^* = -u$ hoặc $u^*u = 1$.

f) Cho một ví dụ trong đó $n = 4$, $\Phi$ đối xứng và có chỉ số 2, $p = \overline{p} = X - 1$, $u$ là chuẩn tắc, $E = G(p, \overline{p})$, nhưng $E$ không phải là tổng trực tiếp của các môđun con cực tiểu của $\mathfrak{M}$, và trong đó tồn tại một vectơ riêng của $u$ không phải là một vectơ riêng của $u^*$ (xem § 7, No. 3).

13) Các giả thiết là các giả thiết của Bài tập 2, và giả sử thêm rằng $E$ thừa nhận một cơ sở đếm được $(e_n)$. Cho $F$ là một không gian con hoàn toàn đẳng hướng (resp. hoàn toàn kỳ dị) của $E$ sao cho $F^{00} = F$; bây giờ chứng minh rằng tồn tại một không gian con hoàn toàn đẳng hướng (resp. hoàn toàn kỳ dị) $F'$ sao cho: $1^\circ \ F \cap F' = \{0\}$; $2^\circ$ tồn tại một cơ sở $(a_m)_{m \in I}$ của $F$ và một cơ sở $(a'_m)_{m \in I}$ của $F'$ (khoảng của $\mathbf{N}$ có gốc 0) sao cho $\Phi(a_i, a'_j) = \delta_{ij}$ với mọi cặp chỉ số; $3^\circ$ $(F + F')^{00} = F + F'$ và $E$ là tổng trực tiếp của $F + F'$ và $G = (F + F')^0$. (Lập bằng quy nạp một dãy tăng $(L_n)$ các không gian con không đẳng hướng, có hợp là $E$, sao cho $\dim L_{n+1} - \dim L_n = 2$, và áp dụng Mệnh đề 2 của No. 2 cho mỗi $L_n$; để lập dãy này, xét, với mỗi $n$, số nguyên nhỏ nhất $k$ sao cho $e_k \notin L_n$, và dùng Bài tập 9 b) của § 1).

14) Cho $A$ là một trường có đặc số 2, $E$ là một không gian vectơ hữu hạn chiều có chiều $n$ trên $A$, $\Phi$ là một dạng Hermit không suy biến trên $E$, không nhất thiết thỏa mãn điều kiện (T).

a) Chứng minh rằng tập hợp $V$ các $x \in E$ sao cho $\Phi(x, x)$ có dạng $\alpha + \overline{\alpha}$ là một không gian con vectơ của $E$.

b) Cho $V_1 = V \cap V^0$, $q = \dim V_1$, $V_2$ là một không gian bù của $V_1$ đối với $V$, $V_3$ là một không gian bù của $V_1$ đối với $V^0$. Bây giờ chứng minh rằng tồn tại một cơ sở $(e_i)_{1 \leq i \leq 2q}$ của $(V_2 + V_3)^0 = V_2^0 \cap V_3^0$ sao cho các vectơ $e_1, \ldots, e_q$ lập thành một cơ sở của $V_1$ và sao cho $\Phi(e_i, e_{q+j}) = \delta_{ij}$ với $1 \leq i \leq q, 1 \leq j \leq q$.

c) Gọi $G(\Phi)$ là nhóm các tự đẳng cấu metric của $E$ (đối với $\Phi$). Bây giờ chứng minh rằng với mọi $u \in G(\Phi)$, ta có $u(x) = x$ với mọi $x \in V^0$.

d) Với mọi $u \in G(\Phi)$, ta có $u(V) = V$; gọi $u_v$ là hạn chế của $u$ lên $V$, và gọi $G_v$ là nhóm tạo thành bởi các $u_v$. Bây giờ chứng minh rằng: $1^o$ hạt nhân của đồng cấu $u \to u_v$ từ $G(\Phi)$ lên $G_v$ là giao hoán; $2^o$ nếu $\Phi_2$ là hạn chế của $\Phi$ lên $V_2$ và $G(\Phi_2)$ là nhóm các tự đẳng cấu metric của $V_2$ đối với $\Phi_2$, thì tồn tại một đồng cấu từ $G_v$ lên $G(\Phi_2)$ mà hạt nhân là giao hoán (dùng $b$ và $c$).

e) Giả sử rằng $A$ là giao hoán và $J$ là đồng nhất; gọi $E$ là một không gian vectơ chiều 3 trên $A$, $(e_i)_{1 \leq i \leq 3}$ một cơ sở của $E$, $\Phi$ dạng đối xứng không suy biến trên $E$ mà ma trận đối với $(e_i)$ là

$$
\begin{pmatrix}
1 & 0 & 0 \\
0 & 0 & 1 \\
0 & 1 & 0
\end{pmatrix}.
$$

Hãy chỉ ra rằng mọi vectơ đẳng hướng trong $E$ đều được chứa trong siêu phẳng sinh bởi $e_2$ và $e_3$ (xem bài tập 4 a)). Hãy cho một ví dụ về một mặt phẳng không đẳng hướng chứa chỉ một phải đẳng hướng (xem bài tập 2 a)). Hãy chỉ ra rằng không có tự đẳng cấu nào $u \in G(\Phi)$ sao cho $u(e_1) = e_1 + e_2$, mặc dù ta có $\Phi(e_1, e_1) = \Phi(e_1 + e_2, e_1 + e_2)$.
