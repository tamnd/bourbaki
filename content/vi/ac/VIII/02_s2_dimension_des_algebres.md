---
book: ac
book_title: Commutative Algebra
chapter: VIII
chapter_title: DIMENSION
section: 2
section_title: Dimension des algèbres
lang: vi
source: ac-viii-ix-fr
book_pages: AC VIII.13-AC VIII.23
pdf_pages: 0017-0027, 0088-0090
extraction: ocr
subsections:
    - "no": 1
      title: Dimension et platitude
      page: 13
      pdf_page: 17
    - "no": 2
      title: Dimension d’une algèbre de type fini
      page: 16
      pdf_page: 20
    - "no": 3
      title: Dimension d’une algèbre entière
      page: 0
      pdf_page: 21
    - "no": 4
      title: Algèbres de type fini sur un corps
      page: 19
      pdf_page: 23
statements: 32
exercises: 18
content_sha256: ec5f5ee7ab2d50521a3dffdf01308cb0f163b9c7ab87830e3f0a6f147a5b53a9
translated_from: content/en-mt/ac/VIII/02_s2_dimension_des_algebres.md
source_lang: en-mt
translation_method: machine
source_content_sha256: b8e1ebd3e2fd9776cb8144b9349cd361f182844488973d9c0ece34efe2b398d8
translation_model: gpt-5.4
translation_run: translate-vi-3afa9944
glossary_version: 34
glossary_terms_sha256: 4393f9e476dfe4ddb8bf12c1118372ec16e3e594890377f3f5552b09be8a2eaa
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 2. CHIỀU CỦA CÁC ĐẠI SỐ

### 1. Chiều và tính phẳng

Cho $\rho : A \to B$ là một đồng cấu các vành. Ta ký hiệu bởi (PM) điều kiện sau:
(PM) Tồn tại một B-môđun N phẳng trung thành trên A sao cho, với mọi iđêan nguyên tố q của B, ta có $N \otimes_B \kappa(q) \neq 0$.

#### Nhận xét 1 {#ac-viii-s2-n1-rem-1 .statement}

Điều kiện (PM) được thỏa mãn khi tồn tại một B-môđun sinh hữu hạn, phẳng trung thành trên A và có giá bằng Spec(B). Đặc biệt, đây là trường hợp nếu A-môđun B là phẳng trung thành.

#### Nhận xét 2 {#ac-viii-s2-n1-rem-2 .statement}

Sự tồn tại của một B-môđun N phẳng trung thành trên A kéo theo tính đơn ánh của ρ (I, § 3, No. 5, mệnh đề 8), và tính toàn ánh của ánh xạ “ρ : Spec(B) → Spec(A) (II, § 2, No. 5, hệ quả 4 của mệnh đề 11).

#### Nhận xét 3 {#ac-viii-s2-n1-rem-3 .statement}

Giả sử rằng ρ : A → B là một đồng cấu địa phương của các vành địa phương và rằng tồn tại một B-môđun N phẳng trên A sao cho N ⊗_B κ(q) ≠ 0 với mọi iđêan nguyên tố q của B. Khi đó N là phẳng trung thành trên A và vì vậy ρ có tính chất (PM): thật vậy ta có N/m_B N = N ⊗_B κ(m_B) ≠ 0, do đó N ≠ m_B N và a fortiori N ≠ m_A N, và kết luận suy ra từ mệnh đề 1 của I, § 3, No. 1.

#### Mệnh đề 1 {#ac-viii-s2-prop-1 .statement}

Cho ρ : A → B là một đồng cấu các vành thỏa mãn điều kiện (PM).

a) Cho h : A → A′ là một đồng cấu các vành. Khi đó đồng cấu ρ′ : A′ → A′ ⊗_A B suy ra từ ρ thỏa mãn điều kiện (PM).

b) Cho q là một iđêan nguyên tố của B và p = ρ^{-1}(q). Đồng cấu chính tắc ρ_q : A_p → B_q thỏa mãn điều kiện (PM).

c) Cho q là một iđêan nguyên tố của B và p = ρ^{-1}(q). Với mọi iđêan nguyên tố p′ của A được chứa trong p, tồn tại một iđêan nguyên tố q′ của B nằm trên p′ và được chứa trong q.

Cho N là một B-môđun phẳng trung thành trên A và sao cho N ⊗_B κ(q) ≠ 0 với mọi iđêan nguyên tố q của B.

Chứng minh a). A′-môđun N′ = A′ ⊗_A N là phẳng trung thành (I, § 3, No. 3, mệnh đề 5); cho q′ là một iđêan nguyên tố của B′ = A′ ⊗_A B và q là ảnh ngược của nó trong B. Ta có các đẳng cấu

$$ N' \otimes_{B'} \kappa(q') \to N \otimes_B \kappa(q') \to (N \otimes_B \kappa(q)) \otimes_{\kappa(q)} \kappa(q'); $$

vì ta có N ⊗_B κ(q) ≠ 0, nên cũng có N′ ⊗_{B′} κ(q′) ≠ 0.

Chứng minh b). Theo các mệnh đề 13 và 14 của II, § 3, No. 4, A_p-môđun N_q là phẳng. Mặt khác, cho b′ là một iđêan nguyên tố của B_q; nó có dạng bB_q, trong đó b là một iđêan nguyên tố của B được chứa trong q (II, § 3, No. 1, mệnh đề 3); ta có N ⊗_B κ(b) ≠ 0 theo giả thiết đặt ra trên N, và vì N_q ⊗_{B_q} κ(b′) đẳng cấu với N ⊗_B κ(b′), nên ta có N_q ⊗_{B_q} κ(b′) ≠ 0. Nhận xét 3 cho phép kết luận.

Chứng minh c). Đồng cấu địa phương ρ_q : A_p → B_q suy ra từ ρ thỏa mãn điều kiện (PM) theo b). Do đó ánh xạ Spec(B_q) → Spec(A_p) là toàn ánh (Nhận xét 2), điều phải chứng minh.

#### Hệ quả {#ac-viii-s2-n1-cor-1 .statement}

Cho F là một tập con đóng của Spec(A). Nếu Y là một thành phần bất khả quy của ảnh ngược của F bởi ánh xạ “ρ : Spec(B) → Spec(A), thì bao đóng của “ρ(Y) là một thành phần bất khả quy của F.

Thật vậy, cho a là một iđêan của A sao cho F = V(a) và q là iđêan nguyên tố của B sao cho Y = V(q). Ảnh ngược của F bởi “ρ là tập con V(ρ(a)B) của Spec(B) và bao đóng của “ρ(Y) là tập con đóng bất khả quy V(ρ^{-1}(q)) của Spec(A).

Vấn đề là chứng minh rằng nếu q là cực tiểu trong số các iđêan nguyên tố của B chứa $\rho(a)$, thì $\rho^{-1}(q)$ là cực tiểu trong số các iđêan nguyên tố của A chứa a. Nếu không, sẽ tồn tại một iđêan nguyên tố $p'$ của A sao cho $a \subset p' \subset \rho^{-1}(q)$ và $p' \neq \rho^{-1}(q)$; theo mệnh đề 1, c), sẽ tồn tại một iđêan nguyên tố $q'$ của B sao cho $q' \subset q$ và $p' = \rho^{-1}(q')$, do đó $\rho(a) \subset q' \subset q$ và $q' \neq q$, trái với giả thiết đặt ra trên q.

#### Mệnh đề 2 {#ac-viii-s2-prop-2 .statement}

Cho $\rho : A \to B$ là một đồng cấu của các vành khác không có tính chất (PM). Ta có bất đẳng thức

(1)
$$
\dim(B) \geq \dim(A) + \inf_{m \in S} \dim(B/mB)
$$
trong đó S là tập hợp các iđêan cực đại của A.

Ta biết rằng $\dim(A) = \sup_{m \in S} \dim(A_m)$ (§ 1, No. 3, mệnh đề 8). Do đó chỉ cần thiết lập bất đẳng thức

(2)
$$
\dim(B) \geq \dim(A_m) + \dim(B/mB)
$$
với mọi iđêan cực đại m của A. Nói cách khác, vấn đề là chứng minh bất đẳng thức

(3)
$$
\dim(B) \geq n + r
$$
nếu $p_0 \subset ... \subset p_n$ là một dây chuyền các iđêan nguyên tố của A được chứa trong m và $\overline{q}_0 \subset ... \subset \overline{q}_r$ là một dây chuyền các iđêan nguyên tố của B/mB. Với $0 \leq i \leq r$, tồn tại một iđêan nguyên tố $q_{n+i}$ của B nằm trên m sao cho $\overline{q}_i = q_{n+i}/mB$, và $q_n \subset ... \subset q_{n+r}$ là một dây chuyền các iđêan nguyên tố của B. Đặt $p'_i = p_i$ với $0 \leq i \leq n-1$ và $p'_n = m$, sao cho $p'_0 \subset ... \subset p'_n$ là một dây chuyền các iđêan nguyên tố của A và q_n nằm trên $p'_n$. Nếu $q_i$ là một iđêan nguyên tố của B nằm trên $p'_i$ ($1 \leq i \leq n$), mệnh đề 1, c) chứng minh rằng tồn tại một iđêan nguyên tố $q_{i-1}$ của B nằm trên $p'_{i-1}$ và được chứa trong $q_i$. Bằng quy nạp đi xuống, do đó ta xây dựng được một dây chuyền $q_0 \subset ... \subset q_n$ các iđêan nguyên tố của B sao cho $q_i$ nằm trên $p_i$ với $0 \leq i \leq n$. Vì $q_0 \subset ... \subset q_{n+r}$ là một dây chuyền các iđêan nguyên tố của B, ta đã chứng minh bất đẳng thức (3).

#### Nhận xét 4 {#ac-viii-s2-n1-rem-4 .statement}

Cho $\rho : A \to B$ là một đồng cấu địa phương của các vành địa phương Noether thỏa mãn điều kiện (PM). Ta sẽ thấy về sau (§ 3, no 4, mệnh đề 7) rằng trong trường hợp này có đẳng thức trong (1). Trong trường hợp tổng quát có thể có bất đẳng thức ngặt (p. 84, bài tập 1).

#### Hệ quả {#ac-viii-s2-n1-cor-2 .statement}

Với mọi iđêan a của A, ta có $\mathrm{ht}(a) \leq \mathrm{ht}(\rho(a)B)$.

Cho q là một iđêan nguyên tố của B chứa $\rho(a)B$, và $p = \rho^{-1}(q)$. Theo mệnh đề 1, đồng cấu địa phương $\rho_q : A_p \to B_q$ suy ra từ $\rho$ thỏa mãn (PM), và do đó ta có $\dim(A_p) \leq \dim(B_q)$ theo mệnh đề 2. Theo mệnh đề 7 của § 7, số 3, ta có $\mathrm{ht}(a) \leq \dim(A_p)$ vì p chứa a, do đó $\mathrm{ht}(a) \leq \dim(B_q)$ đối với mọi iđêan nguyên tố q của B chứa $\rho(a)B$. Khi đó hệ quả được suy ra từ loc. cit.

#### Bổ đề 1 {#ac-viii-s2-lem-1 .statement}

Cho $\rho : A \to B$ là một đồng cấu vành và p là một iđêan nguyên tố của A. Ánh xạ liên tục $^a h : \mathrm{Spec}(B \otimes_A \kappa(p)) \to \mathrm{Spec}(B)$, liên kết với đồng cấu chính tắc $h : B \to B \otimes_A \kappa(p)$, *cảm sinh một đồng phôi của* $\mathrm{Spec}(B \otimes_A \kappa(p))$ *lên không gian con* $(\alpha\rho)^{-1}(p)$ *của* $\mathrm{Spec}(B)$ *được tạo thành bởi các iđêan nguyên tố của* $B$ *nằm trên* $p$.

Đồng cấu $h$ là hợp thành của đồng cấu chuyển qua thương từ $B$ vào $B/\rho(p)$ $B$ và của đồng cấu chính tắc từ $B/\rho(p)$ $B$ vào vành phân thức của nó $(\rho(A - p))^{-1}(B/\rho(p) \ B)$. Theo nhận xét và hệ quả của mệnh đề 13 của II, § 4, số 3, do đó $^a h$ cảm sinh một đồng phôi của $\mathrm{Spec}(B \otimes_A \kappa(p))$ lên không gian con của $\mathrm{Spec}(B)$ được tạo thành bởi các iđêan nguyên tố $q$ của $B$ chứa $\rho(p)$ và rời nhau với $\rho(A - p)$, tức là những iđêan nằm trên $p$.

#### Nhận xét 5 {#ac-viii-s2-n1-rem-5 .statement}

Theo mệnh đề 2 và Bổ đề 1, do đó ta có, dưới các giả thiết của mệnh đề 2, bất đẳng thức
$$
\dim(\mathrm{Spec}(B)) \geq \dim(\mathrm{Spec}(A)) + \inf_{p \in \mathrm{Spec}(A)} \dim(\alpha\rho^{-1}(p)) .
$$

### 2. Chiều của một đại số kiểu hữu hạn

#### Mệnh đề 3 {#ac-viii-s2-prop-3 .statement}

*Cho* $\rho : A \to B$ *là một đồng cấu vành*. *Đặt*
$n = \sup_{p \in \mathrm{Spec}(A)} \dim(B \otimes_A \kappa(p))$. *Ta có bất đẳng thức*
$$
\dim(B) + 1 \leq (\dim(A) + 1).(n + 1) .
$$

Ta có thể giả sử $\dim(A) \neq -\infty$ và $n < +\infty$. Cho $q_0 \subset ... \subset q_m$ là một dãy các iđêan nguyên tố của B; đặt $p_i = \rho^{-1}(q_i)$. Dãy các $p_i$ là tăng, vì thế tập hợp các giá trị của nó có lực lượng $\leq \dim(A) + 1$. Với mỗi $p \in \mathrm{Spec}(A)$, tập hợp các $q_j$ sao cho $p_j = p$ là một dãy của tập con $^a\rho^{-1}(p)$ của $\mathrm{Spec}(B)$, do đó có lực lượng nhỏ hơn $\dim(B \otimes_A \kappa(p)) + 1$ (số 1, Bổ đề 1), và do đó nhỏ hơn hoặc bằng $(n + 1)$. Suy ra $m + 1 \leq (\dim(A) + 1)(n + 1)$, do đó có mệnh đề.

#### Nhận xét 1 {#ac-viii-s2-n2-rem-1 .statement}

Nếu các vành $A$ và $B$ là Noether, ta sẽ thấy dưới đây (§ 3, số 4, hệ quả 2 của mệnh đề 7) rằng ta có bất đẳng thức $\dim(B) \leq \dim(A) + n$, mạnh hơn bất đẳng thức của mệnh đề 3.

#### Hệ quả 1 {#ac-viii-s2-prop-3-cor-1 .statement}

*Giả sử rằng ta có* $\dim(A) < +\infty$ *và rằng tồn tại một số nguyên* $n$ *sao cho* $\dim(B \otimes_A \kappa(p)) \leq n$ *với mọi* $p \in \mathrm{Spec}(A)$. *Khi đó ta có* $\dim(B) < +\infty$.

#### Hệ quả 2 {#ac-viii-s2-prop-3-cor-2 .statement}

*Cho* $A$ *là một vành và* $B = A[X]$ *là vành các đa thức theo một bất định với hệ số trong* $A$. *Ta có* :
$$
1 + \dim(A) \leq \dim(B) \leq 1 + 2\dim(A) .
$$

Bất đẳng thức thứ nhất đã được chứng minh (§ 1, No. 3, ví dụ 4). Hãy chứng minh bất đẳng thức thứ hai. Với mọi iđêan nguyên tố $p$ của $A$, vành $B \otimes_A \kappa(p)$, đẳng cấu với $\kappa(p)[X]$, là chính và không phải là một trường, do đó có chiều bằng 1 (§ 1, No. 3, ví dụ 2), và bất đẳng thức suy ra từ mệnh đề 3.

Tuy nhiên, dù các số nguyên n và q với n + 1 ≤ q ≤ 2n + 1 là thế nào, vẫn tồn tại một vành A có chiều n sao cho dim(A[X]) = q (xem p. 84, bài tập 7).

#### Hệ quả 3 {#ac-viii-s2-prop-3-cor-3 .statement}

Nếu A có số chiều hữu hạn, thì mọi đại số trên A sinh hữu hạn khác không đều có số chiều hữu hạn.

Thật vậy, từ hệ quả 2, bằng quy nạp theo n, suy ra rằng vành A[T₁, ..., Tₙ] có số chiều hữu hạn nếu A có số chiều hữu hạn; a fortiori, mọi vành thương khác không của A[T₁, ..., Tₙ] đều có số chiều hữu hạn (§ 1, No. 3, mệnh đề 6).

### 3. Chiều của một đại số nguyên

#### Bổ đề 2 {#ac-viii-s2-lem-2 .statement}

Cho ρ : A → B là một đồng cấu vành sao cho, với mọi iđêan nguyên tố p của A, đại số trên $\kappa(p)$ B ⊗ₓₐ κ(p) là nguyên (V, § 1, No. 1, định nghĩa 2). Gọi q và q’ là hai iđêan nguyên tố của B sao cho q ⊂ q’ và q ≠ q’. Khi đó ρ⁻¹(q) ≠ ρ⁻¹(q’).

Thật vậy, nếu q và q’ nằm trên cùng một iđêan nguyên tố p của A, thì ta có dim(B ⊗ₓₐ κ(p)) ≥ 1 theo Bổ đề 1 của No. 1, điều này mâu thuẫn với việc dim(B ⊗ₓₐ κ(p)) ≤ 0 (§ 1, No. 3, ví dụ 6).

#### Định lý 1 {#ac-viii-s2-thm-1 .statement}

Cho ρ : A → B là một đồng cấu vành biến B thành một đại số nguyên trên A.

a) Cho M là một A-môđun hữu hạn sinh. Khi đó ta có dim_B(M ⊗ₓₐ B) ≤ dim_A(M). Đặc biệt, ta có dim(B) ≤ dim(A). Nếu ánh xạ “ρ : Spec(B) → Spec(A) là toàn ánh, chẳng hạn (V, § 2, No. 1, định lý 1) nếu ρ là đơn ánh, thì ta có dim_B(M ⊗ₓₐ B) = dim_A(M), và đặc biệt dim(B) = dim(A).

b) Cho b là một iđêan của B và a = ρ⁻¹(b) là ảnh ngược của nó trong A. Ta có ht(b) ≤ ht(a) và dim(B/b) = dim(A/a). Nếu “ρ : Spec B → Spec A là toàn ánh, thì ta có ht(aB) ≤ ht(a) với mọi iđêan a của A.

c) Giả sử rằng B là hữu hạn trên A và cho N là một B-môđun hữu hạn sinh. Khi đó ta có dim_B(N) = dim_A(N). Đặc biệt, ta có dim(B) = dim_A(B).

Hãy chứng minh a). Theo mệnh đề 5 của V, § 1, No. 1, đại số trên $\kappa(p)$ B ⊗ₓₐ κ(p) là nguyên với mọi iđêan nguyên tố p của A. Cho q₀ ⊂ ... ⊂ qₘ là một dãy các iđêan nguyên tố của B; theo Bổ đề 2, các iđêan pᵢ = ρ⁻¹(qᵢ) phân biệt từng đôi một, do đó p₀ ⊂ ... ⊂ pₘ là một dãy các iđêan nguyên tố của A, do đó m ≤ dim(A). Vì thế dim(B) ≤ dim(A).

Bây giờ giả sử rằng ánh xạ “ρ là toàn ánh. Cho p₀ ⊂ ... ⊂ pₙ là một dãy các iđêan nguyên tố của A; do đó tồn tại một iđêan nguyên tố q₀ của B nằm trên p₀. Theo hệ quả 2 của định lý tồn tại thứ nhất (V, § 2, No. 1, định lý 1), bằng quy nạp theo n, ta có thể xây dựng một dãy q₀ ⊂ ... ⊂ qₙ các iđêan nguyên tố của B sao cho qᵢ nằm trên pᵢ với 0 ≤ i ≤ n. Vì thế n ≤ dim(B) và do đó dim(A) ≤ dim(B).

Điều này chứng minh $a$ trong trường hợp $M = A$. Trong trường hợp tổng quát, gọi $a$ là linh hóa tử của $M$, để giá của $M$ được đồng nhất với $\operatorname{Spec}(A/a)$, và ta có $\dim_A(M) = \dim(A/a)$. Theo II, § 4, No. 4, mệnh đề 19, giá của $M \otimes_A B$ là ảnh ngược bởi $^a\rho$ của giá của $M$, do đó được đồng nhất với $\operatorname{Spec}(B/\rho(a) B)$, và ta có $\dim_B(M \otimes_A B) = \dim(B/\rho(a) B)$. Còn lại chỉ cần nhận thấy rằng đồng cấu $\rho': A/a \to B/\rho(a) B$ suy ra từ $\rho$ biến $B/\rho(a) B$ thành một đại số nguyên trên $(A/a)$, và rằng “$\rho'$ là toàn ánh khi $^a\rho$ là như vậy.

Hãy chứng minh $b$. Theo mệnh đề 7 của § 1, No. 3, chỉ cần chứng minh rằng $\operatorname{ht}(b) \leq \dim(A_p)$ với mọi iđêan nguyên tố $p$ của $A$ chứa $a$; gọi $p$ là một iđêan như vậy. Theo V, § 2, No. 1, hệ quả 2 của định lý 1, tồn tại một iđêan nguyên tố $q$ của $B$ nằm trên $p$ và chứa $b$, và ta có $\operatorname{ht}(b) \leq \dim(B_q)$ theo mệnh đề 7 của § 1, No. 3.

Bây giờ $B_q$ đồng nhất với một vành phân thức của $A_p$-đại số $B \otimes_A A_p$, do đó
$$
\dim(B_q) \leq \dim(B \otimes_A A_p) \leq \dim(A_p)
$$
theo Mệnh đề 6 của § 1, No. 3 và mệnh đề $a$ ở trên. Như vậy ta đã chứng minh bất đẳng thức $\operatorname{ht}(b) \leq \operatorname{ht}(a)$. Hơn nữa, đồng cấu từ $A/a$ vào $B/b$ suy ra từ $\rho$ là đơn ánh và làm cho $B/b$ thành một $(A/a)$-đại số nguyên; do đó ta có $\dim(B/b) = \dim(A/a)$ theo $a$. Giả sử “$\rho$ là toàn ánh và cho $a$ là một iđêan của $A$ và $p$ là một iđêan nguyên tố của $A$ chứa $a$. Theo giả thiết, tồn tại một iđêan nguyên tố $q$ của $B$ nằm trên $p$. Ta có $aB \subset q$, do đó $\operatorname{ht}(aB) \leq \operatorname{ht}(q) \leq \operatorname{ht}(p)$ theo điều đi trước. Chuyển sang cận dưới lớn nhất, ta thu được $\operatorname{ht}(aB) \leq \operatorname{ht}(a)$.

Cuối cùng, $c$ suy ra từ $b$ áp dụng cho linh hóa tử $b$ của $N$.

#### Định lý 2 {#ac-viii-s2-thm-2 .statement}

Cho $A$ là một vành nguyên đóng, và $B$ là một vành chứa $A$, nguyên trên $A$. Giả sử rằng $B$ là một A-môđun không xoắn. Với mọi iđêan $a$ của $A$, ta có $\operatorname{ht}(a) = \operatorname{ht}(aB)$. Cho $b$ là một iđêan của $B$ và $a = b \cap A$; khi đó ta có $\operatorname{ht}(a) = \operatorname{ht}(b)$.

Gọi $\rho$ là ánh xạ chính tắc từ $A$ vào $B$. Gọi $a$ là một iđêan của $A$. Nếu $a = A$, đẳng thức thứ nhất là hiển nhiên. Giả sử $a \neq A$. Vì $\rho$ là đơn ánh, $^a\rho$ là toàn ánh (V, § 2, No. 1, Định lý 1). Do đó $aB \neq B$. Khi ấy lấy $q$ là một iđêan nguyên tố của $B$ chứa $aB$. Đặt $p = q \cap A$. Ta có $a \subset p$, suy ra $\operatorname{ht}(a) \leq \operatorname{ht}(p)$. Gọi $p_0 \subset ... \subset p_n$ là một chuỗi iđêan nguyên tố của $A$ với $p_n = p$. Theo định lý tồn tại thứ hai (V, § 2, No. 4, Định lý 3), ta xây dựng bằng quy nạp một chuỗi $q_0 \subset ... \subset q_n$ các iđêan nguyên tố của $B$ sao cho $q_n = q$ và $q_i$ nằm trên $p_i$ với $0 \leq i \leq n$. Ta có $n \leq \operatorname{ht}(q)$, suy ra $\operatorname{ht}(a) \leq \operatorname{ht}(q)$. Lấy cận dưới, ta được $\operatorname{ht}(a) \leq \operatorname{ht}(aB)$ ($§ 1$, No. 3, Mệnh đề 7). Bất đẳng thức $\operatorname{ht}(aB) \leq \operatorname{ht}(a)$ suy ra từ Định lý 1, do đó có đẳng thức thứ nhất. Gọi $b$ là một iđêan của $B$. Đặt $a = \rho^{-1}(b)$. Ta có $aB \subset b$, suy ra $\operatorname{ht}(a) = \operatorname{ht}(aB) \leq \operatorname{ht}(b)$. Bất đẳng thức $\operatorname{ht}(b) \leq \operatorname{ht}(a)$ suy ra từ Định lý 1, do đó được định lý.

#### Nhận xét {#ac-viii-s2-n3-rem-1 .statement}

Gọi $A$ là một miền nguyên và $B$ là một vành chứa $A$, nguyên trên $A$. Gọi $p$ là một iđêan nguyên tố của $A$ sao cho bao đóng nguyên của $A_p$ là một vành địa phương. Có thể chứng minh rằng, với mọi iđêan nguyên tố $q$ của $B$ nằm trên $p$, ta có $\operatorname{ht}(p) = \operatorname{ht}(q)$ (p. 85, Exer. 9) khi $B$ là một miền nguyên.

### 4. Các đại số kiểu hữu hạn trên một trường

Trong số này, $k$ ký hiệu một trường.

#### Bổ đề 3 {#ac-viii-s2-lem-3 .statement}

Cho $A$ là một $k$-đại số kiểu hữu hạn và $p_0 \subset ... \subset p_m$ là một dãy cực đại các iđêan nguyên tố của $A$. Tồn tại một số nguyên $n \geq m$, một dãy $(x_1, ..., x_n)$ các phần tử của $A$, tự do đại số trên $k$ (A, IV, p. 4), và sao cho :
a) $A$ là nguyên trên vành $B = k[x_1, ..., x_n]$;
b) với mọi $j$ sao cho $0 \leq j \leq m$, iđêan $p_j \cap B$ được sinh bởi các $x_k$ với $1 \leq k \leq n - m + j$.

Theo bổ đề chuẩn hóa (V, § 3, No. 1, th. 1), tồn tại một số nguyên $n \geq 0$, một dãy hữu hạn $(x_1, ..., x_n)$ các phần tử của $A$ tự do đại số và một dãy tăng $(h(j))_{0 \leq j \leq m}$ các số nguyên $\leq n$ sao cho iđêan $p_j \cap B$ bằng iđêan nguyên tố $q_j$ của $B$ được sinh bởi các $x_k$ với $1 \leq k \leq h(j)$, và sao cho $A$ là nguyên trên vành $B$. Cho $j$ là một số nguyên sao cho $0 \leq j < m$. Chuyển qua các thương, suy ra từ đơn ánh chính tắc của $B$ vào $A$ một đồng cấu đơn ánh của $B/q_j$ vào $A/p_j$ khiến $A/p_j$ là một $(B/q_j)$-đại số hữu hạn. Vì vành $B/q_j$ đẳng cấu với một đại số đa thức theo $n - h(j)$ bất định trên $k$, nên nó nguyên đóng (V, § 1, No. 3, Cor. 3 of Prop. 13). Theo th. 2 của No. 3, do đó có

$$
1 = \mathrm{ht}(p_{j+1}/p_j) = \mathrm{ht}(q_{j+1}/q_j) \geq h(j+1) - h(j) .
$$

Suy ra $h(j+1) \leq h(j) + 1$ và $q_{j+1} \neq q_j$, do đó $h(j+1) = h(j) + 1$. Nhưng ta có $h(m) = n$ vì $q_m$ là cực đại (V, § 2, No. 1, Prop. 1), do đó cuối cùng $h(j) = n - m + j$.

#### Định lý 3 {#ac-viii-s2-thm-3 .statement}

Cho $A$ là một $k$-đại số kiểu hữu hạn.
a) Với mọi iđêan nguyên tố cực tiểu $p$ của $A$, mọi dãy tối đại các iđêan nguyên tố của $A$ có gốc $p$ đều có độ dài bằng số nguyên $\deg.\mathrm{tr}_k \kappa(p)$.
b) Vành $A$ là catenary và chiều của nó là cận trên đúng của các số nguyên $\deg.\mathrm{tr}_k \kappa(p)$, khi $p$ chạy qua các iđêan nguyên tố cực tiểu của $A$.
c) Nếu $A$ là nguyên, thì mọi dãy tối đại các iđêan nguyên tố của $A$ đều có cùng độ dài, và chiều của $A$ là bậc siêu việt trên $k$ của trường phân thức của $A$.

Giả sử $A$ là nguyên và xét một dãy tối đại $p_0 \subset ... \subset p_m$ các iđêan nguyên tố của $A$. Ta có $p_0 = 0$. Khi đó, từ Bổ đề 3 ta suy ra sự tồn tại của một đơn cấu $\varphi : k[X_1, ..., X_m] \to A$ của các $k$-đại số, khiến $A$ trở thành một $k[X_1, ..., X_m]$-đại số hữu hạn. Do đó, bậc siêu việt trên $k$ của trường phân thức của $A$ bằng $m$, do đó suy ra c). Mệnh đề a) suy ra từ mệnh đề c) áp dụng cho vành $A/p$ và mệnh đề b) là một hệ quả ngay lập tức của a) và của Mệnh đề 5 của § 1, No. 2.

#### Hệ quả 1 {#ac-viii-s2-thm-3-cor-1 .statement}

Cho $n$ là một số nguyên dương. Ta có

$$
\dim(k[X_1, ..., X_n]) = n .
$$

Điều kiện cần và đủ để một k-đại số kiểu hữu hạn A có chiều n là tồn tại một k-đồng cấu đơn cấu $\varphi : k[X_1, ..., X_n] \to A$ khiến A trở thành một đại số hữu hạn trên $k[X_1, ..., X_n]$.

Điều này suy ra từ định lý 3, từ bổ đề chuẩn hóa (V, § 3, No. 1, định lý 1) và từ định lý 1, a) của No. 3.

#### Hệ quả 2 {#ac-viii-s2-thm-3-cor-2 .statement}

Cho A là một k-đại số nguyên kiểu hữu hạn. Với mọi iđêan nguyên tố p của A, ta có

$$
\operatorname{ht}(p) = \dim(A_p) = \dim(A) - \dim(A/p)
$$
$$
= \dim(A) - \deg.\operatorname{tr}_k\kappa(p).
$$

Đặc biệt, ta có $\operatorname{ht}(m) = \dim(A_m) = \dim(A)$ với mọi iđêan cực đại m của A.

Điều này suy ra từ định lý 3 và Nhận xét 4 của § 1, No. 3.

#### Hệ quả 3 {#ac-viii-s2-thm-3-cor-3 .statement}

Cho A là một k-đại số kiểu hữu hạn và cho f là một phần tử của A không thuộc iđêan nguyên tố cực tiểu nào của A (chẳng hạn một phần tử của A không phải là ước của không, xem IV, § 1, No. 1, Hệ quả 3 của Mệnh đề 2 và No. 3, Hệ quả 1 của Mệnh đề 7). Ta có $\dim(A) = \dim(A_f)$.

Ánh xạ $p \mapsto pA_f$ là một song ánh từ tập hợp các iđêan nguyên tố cực tiểu của A lên tập hợp các iđêan nguyên tố cực tiểu của $A_f$. Hơn nữa, các vành $A/p$ và $A_f/pA_f = (A/p)_f$ có cùng trường phân thức. Vì vậy chỉ cần áp dụng định lý 3, b).

#### Hệ quả 4 {#ac-viii-s2-thm-3-cor-4 .statement}

Cho A là một k-đại số kiểu hữu hạn và cho p là một iđêan nguyên tố của A.

a) Điều kiện cần và đủ để p là cực đại là trường phân thức của $A/p$ là một mở rộng hữu hạn của k.

b) Cho $f \in A - p$; iđêan p là một iđêan cực đại của A khi và chỉ khi $pA_f$ là một iđêan cực đại của $A_f$.

Nếu p là một iđêan cực đại của A, thì $A/p$ là một trường, do đó là một vành có chiều 0; đó là một mở rộng kiểu hữu hạn của k có bậc siêu việt bằng 0 (định lý 3, c)), vì vậy nó là một mở rộng hữu hạn của k. Ngược lại, nếu trường phân thức của $A/p$ là một mở rộng hữu hạn của k, thì ta có $\dim(A/p) = 0$ nên p là cực đại. Mệnh đề b) suy ra từ mệnh đề a), có tính đến việc $A/p$ và $A_f/pA_f$ có cùng trường phân thức.

Mệnh đề a) của Hệ quả 4 là một dạng của định lý không điểm (V, § 3, No. 3, Mệnh đề 1).

#### Hệ quả 5 {#ac-viii-s2-thm-3-cor-5 .statement}

Cho A là một k-đại số kiểu hữu hạn, p một iđêan nguyên tố của A và $(\mathfrak{p}_i)_{i \in I}$ là họ các iđêan nguyên tố cực tiểu của A được chứa trong p. Ta có:

$$
\dim_p(A) = \sup_{i \in I} \dim(A/\mathfrak{p}_i)
$$
$$
= \dim(A_p) + \dim(A/p)
$$
$$
= \dim(A_p) + \deg.\operatorname{tr}_k\kappa(p).
$$

Ta có $\dim_p(A) = \sup_{i \in I} \dim_{p/p_i}(A/p_i)$ (§ 1, No. 3, Mệnh đề 6). Nhưng, theo Hệ quả 3, ta có $\dim_{p/p_i}(A/p_i) = \dim(A/p_i)$, do đó suy ra đẳng thức thứ nhất. Theo Hệ quả 2, ta có $\dim(A/p_i) = \dim((A/p_i)_p) + \dim(A/p)$. Vì vậy đẳng thức thứ hai của hệ quả suy ra từ việc $\dim(A_p) = \sup_{i \in I} \dim((A/p_i)_p)$ và đẳng thức thứ ba suy ra từ định lý 3.

Vậy $\dim_p(A)$ là cận trên đúng của các độ dài của các dãy iđêan nguyên tố của $A$ mà p là một phần tử.

#### Hệ quả 6 {#ac-viii-s2-thm-3-cor-6 .statement}

*Cho A là một đại số trên k sinh hữu hạn không bằng 0, và cho n là một số nguyên $\geqslant 0$. Các điều kiện sau là tương đương:*

a) *Với mọi $p \in \operatorname{Ass}(A)$, ta có $\dim(A/p) = n$.*

b) *Mọi iđêan nguyên tố liên kết của A đều là cực tiểu và mọi thành phần bất khả quy của Spec(A) đều có chiều n.*

c) *Tồn tại một k-đồng cấu đơn ánh $\varphi : k[X_1, ..., X_n] \to A$ làm cho A thành một $k[X_1, ..., X_n]$-môđun kiểu hữu hạn không xoắn.*

Sự tương đương của a) và b) là ngay lập tức. Ta hãy chứng minh rằng a) suy ra c). Theo b), vành A có chiều n và do đó tồn tại (hệ quả 1) một k-đồng cấu đơn ánh $\varphi : k[X_1, ..., X_n] \to A$ làm cho A thành một $k[X_1, ..., X_n]$-môđun kiểu hữu hạn. Với mọi iđêan nguyên tố $p \in \operatorname{Ass}(A)$, vành $A/p$ khi đó là nguyên trên $k[X_1, ..., X_n]$, và vì thế ta có $n = \dim(A/p) = \dim(k[X_1, ..., X_n]/\varphi^{-1}(p))$ theo định lý 1, a) của no. 3, do đó $\varphi^{-1}(p) = 0$. Ảnh bởi đơn cấu $\varphi$ của một phần tử khác không của $k[X_1, ..., X_n]$ không phải là một ước của không trong A (IV, § 1, no. 1, hệ quả 3 của mệnh đề 2), do đó c).

Ngược lại, giả sử rằng điều kiện c) được thỏa mãn. Với mọi iđêan nguyên tố $p \in \operatorname{Ass}(A)$, đồng cấu $k[X_1, ..., X_n] \to A/p$ suy ra từ $\varphi$ là đơn ánh (*loc. cit.*). Do đó ta có $\dim(A/p) = n$ theo hệ quả 1.

#### Nhận xét 1 {#ac-viii-s2-n4-rem-1 .statement}

Theo hệ quả 5, các điều kiện a), b), c) của hệ quả 6 suy ra rằng ta có $\dim_p(A) = \dim(A)$ với mọi iđêan nguyên tố $p$ của A.

#### Mệnh đề 4 {#ac-viii-s2-prop-4 .statement}

*Cho A và B là hai đại số trên k sinh hữu hạn và $\rho : A \to B$ là một đồng cấu đại số. Giả sử rằng A là nguyên và A-môđun B là không xoắn, và ký hiệu K là trường các phân thức của A. Ta có*

$$
\dim(B) = \dim(A) + \dim(B \otimes_A K).
$$

Trước hết giả sử rằng B là nguyên. Đại số $B \otimes_A K$ khi đó là một vành các phân thức của B được xác định bởi một tập con nhân không chứa 0. Vậy nên nó có trường các phân thức là trường các phân thức L của B. Theo định lý 3, ta có

$$
\dim(B) = \deg.\mathrm{tr}_k L,\quad \dim(A) = \deg.\mathrm{tr}_k K,
$$
$$
\dim(B \otimes_A K) = \deg.\mathrm{tr}_K L.
$$

Bây giờ, theo hệ quả của A, V, p. 106

$$
\deg.\mathrm{tr}_k L = \deg.\mathrm{tr}_K L + \deg.\mathrm{tr}_k K,
$$

do đó có kết quả trong trường hợp này.

Ta chuyển sang trường hợp tổng quát. Mọi iđêan nguyên tố cực tiểu $p$ của $B$ đều được tạo thành bởi các ước của không trong $B$, và vì thế nằm trên iđêan 0 của $A$. Suy ra rằng ánh xạ $p \mapsto p . (B \otimes_A K)$ là một song ánh từ tập hợp các iđêan nguyên tố cực tiểu của $B$ lên tập hợp các iđêan nguyên tố cực tiểu của $B \otimes_A K$. Vậy mệnh đề được suy ra từ phần đầu của chứng minh và từ mệnh đề 6, c) của § 1, no 3.

#### Hệ quả {#ac-viii-s2-n4-cor-1 .statement}

*Cho $\rho : A \to B$ là một đồng cấu đơn ánh của các đại số trên k sinh hữu hạn.* *Ta có* $\dim(A) \leq \dim(B)$.

Thật vậy, cho $p$ là một iđêan nguyên tố cực tiểu của $A$ sao cho $\dim(A) = \dim(A/p)$. Tồn tại một iđêan nguyên tố $q$ của $B$ nằm trên $p$ (II, § 2, no 6, mệnh đề 16). Theo mệnh đề 4 áp dụng cho $A/p$ và $B/q$, ta có $\dim(A) = \dim(A/p) \leq \dim(B/q) \leq \dim(B)$, do đó có hệ quả.

*Bổ đề 4. — Cho $A$ và $B$ là hai đại số trên k nguyên, $M$ là một A-môđun không xoắn, $N$ là một B-môđun không xoắn. Nếu vành $A \otimes_k B$ là nguyên, thì $M \otimes_k N$ là một môđun không xoắn trên $A \otimes_k B$.*

Cho $K$ (resp. $L$) là trường các phân thức của $A$ (resp. $B$). Tồn tại một tập hợp $I$ (resp. $J$) sao cho $M$ (resp. $N$) đẳng cấu với một môđun con của $K^{(I)}$ (resp. $L^{(J)}$). Do đó $(A \otimes_k B)$-môđun $M \otimes_k N$ đẳng cấu với một môđun con của $K^{(I)} \otimes_k L^{(J)}$, môđun này đẳng cấu với $(K \otimes_k L)^{(I \times J)}$. Vì $K \otimes_k L$ là một vành phân thức của vành nguyên $A \otimes_k B$, nên nó là một môđun không xoắn trên $A \otimes_k B$, do đó suy ra bổ đề.

*MỆNH ĐỀ 5. — Cho $k'$ là một mở rộng của $k$, $A$ là một đại số trên k kiểu hữu hạn và $B$ là một đại số trên $k'$ kiểu hữu hạn.*

a) *Đại số trên $k'$ $A \otimes_k B$ là kiểu hữu hạn và ta có*
$$
\dim(A \otimes_k B) = \dim(A) + \dim(B).
$$

b) *Cho $r$ là một iđêan nguyên tố của $A \otimes_k B$; gọi $p$ (resp. $q$) là ảnh ngược của $r$ trong $A$ (resp. $B$). Ta có*
$$
\dim_r(A \otimes_k B) = \dim_p(A) + \dim_q(B).
$$

Đặt $n = \dim(A)$ và $m = \dim(B)$. Theo Hệ quả 1 của Định lý 3, tồn tại các đồng cấu đại số đơn ánh $\varphi : k[X_1, ..., X_n] \to A$ và $\psi : k'[Y_1, ..., Y_m] \to B$ khiến $A$ và $B$ lần lượt là các đại số hữu hạn trên $k[X_1, ..., X_n]$ và $k'[Y_1, ..., Y_m]$. Khi đó đồng cấu $\varphi \otimes \psi$ là đơn ánh và biến $A \otimes_k B$ thành một đại số hữu hạn trên đại số trên $k'$ $k[X_1, ..., X_n] \otimes_k k'[Y_1, ..., Y_m]$, đại số này được đồng nhất với $k'[X_1, ..., X_n, Y_1, ..., Y_m]$. Do đó $\dim(A \otimes_k B) = n + m$ theo Hệ quả 1 của Định lý 3, điều này chứng minh a).

Ta nhận thấy rằng khi $A$ và $B$ là nguyên, $A \otimes_k B$ là một $k'[X_1, ..., X_n, Y_1, ..., Y_m]$-môđun không xoắn theo Bổ đề 4, và do đó ta có
$$
\dim_r(A \otimes_k B) = n + m = \dim(A) + \dim(B)
$$
với mọi iđêan nguyên tố $r$ của $A \otimes_k B$ theo Nhận xét 1.

Chứng minh b) bây giờ. Cho $r_0$ là một iđêan nguyên tố cực tiểu của $A \otimes_k B$ được chứa trong $r$, và ký hiệu bởi $p_0$ (resp. $q_0$) ảnh ngược của $r_0$ trong $A$ (resp. $B$). Vành

(A \otimes_k B)/r_0 đẳng cấu với một thương của vành (A/p_0) \otimes_k (B/q_0). Do đó, theo $a$,

$$
\dim((A \otimes_k B)/r_0) \leq \dim(A/p_0) + \dim(B/q_0).
$$

Áp dụng hệ quả 5 cho định lý 3, ta suy ra bất đẳng thức

$$
\dim_r(A \otimes_k B) \leq \dim_p(A) + \dim_q(B).
$$

Ngược lại, cho $p_0$ (resp. $q_0$) là một iđêan nguyên tố cực tiểu của A (resp. B) được chứa trong $p$ (resp. q). Theo nhận xét đã nêu ở trên, ta có

$$
\dim(A/p_0) + \dim(B/q_0) = \dim_{\overline{r}}((A/p_0) \otimes_k (B/q_0))
$$

trong đó $\overline{r}$ là ảnh của r bởi toàn cấu chính tắc $A \otimes_k B \to (A/p_0) \otimes_k (B/q_0)$. Vế thứ hai của đẳng thức trên hiển nhiên nhỏ hơn $\dim_r(A \otimes_k B)$. Áp dụng hệ quả 5 cho định lý 3, ta suy ra bất đẳng thức

$$
\dim_p(A) + \dim_q(B) \leq \dim_r(A \otimes_k B),
$$

điều này hoàn tất chứng minh.

#### Hệ quả {#ac-viii-s2-n4-cor-2 .statement}

*Cho A là một đại số trên K sinh hữu hạn, k' là một mở rộng của k, và A' là đại số trên K A \otimes_k k'.*

a) *Ta có* $\dim(A') = \dim(A)$.

b) *Cho p' là một iđêan nguyên tố của A' và p là ảnh ngược của nó trong A; ta có* $\dim_{p'}(A') = \dim_p(A)$.

c) *Cho p' là một iđêan nguyên tố cực tiểu của A' và p là ảnh ngược của nó trong A. Khi đó p là cực tiểu và ta có* $\dim(A'/p') = \dim(A/p)$.

Các khẳng định a) và b) suy ra từ mệnh đề 5 bằng cách lấy $B = k'$. Hãy chứng minh c). Iđêan p là cực tiểu (No. 1, mệnh đề 1) và ta có

$$
\dim(A'/p') = \dim_{p'}(A') = \dim_p(A) = \dim(A/p).
$$

#### Nhận xét 2 {#ac-viii-s2-n4-rem-2 .statement}

*Giả sử rằng mở rộng k' của k là radicial. Khi đó ánh xạ chính tắc $f : \mathrm{Spec}(A') \to \mathrm{Spec}(A)$ là một đồng phôi.*

Thật vậy, cho $p \in \mathrm{Spec}(A)$. Theo Bổ đề 1 của No. 1, không gian $f^{-1}(\{p\})$ đồng phôi với $\mathrm{Spec}(\kappa(p) \otimes_k k')$. Bây giờ tập hợp a các phần tử lũy linh của $\kappa(p) \otimes_k k'$ là một iđêan nguyên tố (A, V, p. 134, hệ quả) và vành thương $(\kappa(p) \otimes_k k')/a$, nguyên và hữu hạn trên $\kappa(p)$, là một trường (A, V, p. 16, hệ quả 1 và p. 10, mệnh đề 1). Do đó $f^{-1}(\{p\})$ thu về một phần tử duy nhất. Suy ra ánh xạ $f$ là một song ánh tăng từ $\mathrm{Spec}(A')$ lên $\mathrm{Spec}(A)$, hai tập hợp này được sắp thứ tự bởi quan hệ bao hàm của các iđêan nguyên tố, và vì thế cảm sinh một song ánh giữa các tập con đóng bất khả quy của $\mathrm{Spec}(A)$ và các tập con đóng bất khả quy của $\mathrm{Spec}(A')$. Vì các tập con đóng của $\mathrm{Spec}(A)$ (resp. $\mathrm{Spec}(A')$) là các hợp hữu hạn của các tập con đóng bất khả quy, $f$ là một đồng phôi.

Để có một phép tổng quát hóa, xem bài tập 24, p. 98.

## BÀI TẬP {#ac-viii-s2-exercises}

Xem [các bài tập của § 2](exercises/s2/).
