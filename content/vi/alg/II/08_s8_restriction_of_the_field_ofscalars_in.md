---
book: alg
book_title: Algebra
chapter: II
chapter_title: LINEAR ALGEBRA
section: 8
section_title: Restriction of the field ofscalars in vector spaces
lang: vi
source: alg-i-iii
source_edition: 1998, Springer
pdf_pages: 0341-0349, 0433-0434
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF K'-STRUCTURES
      page: 0
      pdf_page: 341
    - "no": 2
      title: Rationality for a subspace
      page: 0
      pdf_page: 342
    - "no": 3
      title: RATIONALITY FOR A LINEAR MAPPING
      page: 0
      pdf_page: 343
    - "no": 4
      title: RATIONAL LINEAR FORMS
      page: 0
      pdf_page: 344
    - "no": 5
      title: APPLICATION TO LINEAR SYSTEMS
      page: 0
      pdf_page: 345
    - "no": 6
      title: SMALLEST FIELD OF RATIONALITY
      page: 0
      pdf_page: 346
    - "no": 7
      title: CRITERIA FOR RATIONALITY
      page: 0
      pdf_page: 347
statements: 17
exercises: 5
content_sha256: 96945e45659c7d3584c3c69c30a2e33eb6c072c9c7d082f5d1af33b5ee0ae145
translated_from: content/en/alg/II/08_s8_restriction_of_the_field_ofscalars_in.md
source_content_sha256: 6810d0ad2d7a1ac57e96581b1b317b077f67da34f1fea1aceace9aa72bc903be
translation_model: gpt-5.4-mini, gpt-5-mini
translation_run: translate-vi-2f9cd8fa
glossary_version: 34
glossary_terms_sha256: 698bfe725ef5a091ed8296a5f24df6d97be7bc49f39c9ab48d374a42da00cf96
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 8. HẠN CHẾ TRƯỜNG VÔ HƯỚNG TRONG KHÔNG GIAN VECTƠ

Trong toàn bộ đoạn này, K ký hiệu một trường và K' một trường con của K. Trên một tập hợp V, một cấu trúc không gian vectơ phải (resp. trái) trên K xác định, bằng cách hạn chế trường vô hướng, một cấu trúc không gian vectơ phải (resp. trái) trên K'.

### 1. ĐỊNH NGHĨA CÁC CẤU TRÚC K'

#### Mệnh đề 1 {#alg-ii-s8-prop-1 .statement}

Cho V là một không gian vectơ phải trên K và V' là một tập con của V là một không gian con vectơ trên K'. Các điều kiện sau là tương đương:

(a) Ánh xạ K-tuyến tính $\lambda$ từ $V'_{(K)} = V' \otimes_{K'} K$ vào V sao cho $\lambda(x' \otimes \xi) = x'\xi$ với mọi $x' \in V', \xi \in K$, là song ánh.

(b) Mọi ánh xạ K'-tuyến tính $f'$ của V' vào một không gian K-vectơ W đều có thể được kéo dài duy nhất thành một ánh xạ K-tuyến tính f của V vào W.

(c) Mọi cơ sở của V' trên K' đều là một cơ sở của V trên K.

(d) Tồn tại một cơ sở của V' trên K' cũng là một cơ sở của V trên K.

(e) Không gian K-vectơ V được sinh bởi V' và mọi tập con của V' tự do trên K' đều tự do trên K.

Ta biết (§ 5, no. 1) rằng $V'_{(K)}$ có một cấu trúc không gian vectơ phải trên K theo đó $(x' \otimes \xi)\eta = x' \otimes (\xi\eta)$ ($\xi, \eta$ in K, $x' \in V'$) và rằng với mọi ánh xạ K'-tuyến tính $f'$ của V' vào một không gian K-vectơ W, tồn tại một và chỉ một ánh xạ K-tuyến tính $\bar{f}'$ của $V'_{(K)}$ vào W sao cho $\bar{f}'(x' \otimes 1) = f'(x')$ với $x' \in V'$. Nếu j là đơn ánh chính tắc của V' vào V, thì $\lambda$ chỉ là ánh xạ K-tuyến tính tương ứng $\bar{j}$. Nếu $\lambda$ là song ánh, thì với mọi ánh xạ K'-tuyến tính $f': V' \to W$, $\bar{f}' \circ \lambda^{-1}$ là ánh xạ K-tuyến tính duy nhất của V vào W kéo dài $f'$; nói cách khác, (a) suy ra (b). Ngược lại, nếu (b) đúng, thì đặc biệt tồn tại một ánh xạ K-tuyến tính $\mu$ của V vào $V'_{(K)}$ sao cho $\mu(x') = x' \otimes 1$ với mọi $x' \in V'$; rõ ràng $\mu \circ \lambda = 1_{V'_{(K)}}$; mặt khác, $\lambda(\mu(x')) = x'$ với mọi $x' \in V'$ và, vì theo giả thiết $j: V' \to V$ có thể được kéo dài duy nhất thành một tự đồng cấu của V, tất yếu $\lambda \circ \mu = 1_V$, điều đó hoàn tất chứng minh rằng (a) và (b) là tương đương.

Với mọi cơ sở B' của V' trên K', tập B gồm các phần tử $v' \otimes 1$ của $V'_{(K)}$, trong đó $v'$ chạy qua B', là một cơ sở của $V'_{(K)}$ trên K (§ 5, no. 1, Mệnh đề 4) và $\lambda(B) = B'$. Để $\lambda$ là song ánh, điều cần thiết là ảnh của mọi cơ sở của $V'_{(K)}$ qua $\lambda$ phải là một cơ sở của V trên K, và đủ là chỉ cần đúng với một cơ sở của $V'_{(K)}$ (§ 1, no. 11, Hệ quả 2 của Mệnh đề 17). Điều này chứng minh (a), (c) và (d) là tương đương.

Vì mọi tập con của V' tự do trên K' đều được chứa trong một cơ sở của V' trên K' (§ 7, no. 1, Định lý 2), nên (c) suy ra (e). Cuối cùng, giả sử rằng (e) đúng; nếu B' là một cơ sở của V' trên K', thì nó là một tập con tự do của V trên K; mặt khác B' sinh V' trên K' và do đó sinh V trên K theo giả thiết; vì vậy B' là một cơ sở của V trên K, điều đó chứng minh rằng (e) suy ra (c).

#### Định nghĩa 1 {#alg-ii-s8-def-1 .statement}

*Cho V là một không gian vectơ phải trên một trường K và K' là một trường con của K. Mọi không gian con K'-vectơ V' của V thỏa mãn các điều kiện tương đương của Mệnh đề 1 được gọi là một K'-cấu trúc trên V.*

#### Ví dụ {#alg-ii-s8-n1-exa-1 .statement}

Cho B là một cơ sở của V trên K. Với *mọi* trường con K' của K, không gian con K'-vectơ của V được sinh bởi B thừa nhận B làm một cơ sở trên K' và do đó là một K'-cấu trúc trên V. *Chẳng hạn, nếu K giao hoán và V được lấy là đại số đa thức K-algebra K[X_1, ..., X_n], thì với mọi trường con K' của K, K'[X_1, ..., X_n] là một K'-cấu trúc trên V.*

### 2. Tính hữu tỉ đối với một không gian con

#### Định nghĩa 2 {#alg-ii-s8-def-2 .statement}

*Cho V là một không gian vectơ phải trên K, với một K'-cấu trúc V'. Một vectơ của V được gọi là hữu tỉ trên K' nếu nó thuộc V'. Một không gian con K-vectơ W của V được gọi là hữu tỉ trên K' nếu nó được sinh (trên K) bởi các vectơ hữu tỉ trên K'._

Cho $(v'_i)_{i \in I}$ là một cơ sở của V' trên K', nên nó cũng là một cơ sở của V trên K (no. 1, Mệnh đề 1). Để một vectơ x = $\sum_i v'_i \xi_i$ của V là hữu tỉ trên K', điều cần và đủ là $\xi_i \in K'$ với mọi $i \in I$.

Nếu W là một không gian con K-vectơ của V mà *hữu tỉ* trên K', thì từ Định nghĩa 2 suy ra $W' = W \cap V'$ là một không gian con K'-vectơ của W, và nó *sinh* W trên K; mặt khác mọi tập con của W' tự do trên K' cũng tự do trên K vì nó được chứa trong V' (no. 1, Mệnh đề 1). Suy ra (no. 1, Mệnh đề 1) rằng W' là một *K'-cấu trúc* trên W, được gọi là *cảm sinh* bởi K'-cấu trúc V' trên V.

Với mọi không gian con K'-vectơ W' của V', ta sẽ ký hiệu W'.K là không gian con K-vectơ của V gồm các tổ hợp tuyến tính của các phần tử của W' với các hệ số trong K.

#### Mệnh đề 2 {#alg-ii-s8-prop-2 .statement}

*Cho V là một không gian vectơ phải trên K và V' là một K'-cấu trúc trên V. Ánh xạ W' \mapsto W'.K là một song ánh từ tập các không gian con K'-vectơ của V' lên tập các không gian con K-vectơ của V mà hữu tỉ trên K' và song ánh ngược là W \mapsto W \cap V'._

Rõ ràng song ánh $\lambda^{-1}: V \to V' \otimes_{\mathbf{K'}} \mathbf{K}$, nghịch đảo của song ánh $\lambda$ được định nghĩa ở no. 1, Mệnh đề 1, gửi mọi không gian con K'-vectơ W' của V' tới ảnh của nó qua đơn ánh chính tắc $x' \mapsto x' \otimes 1$ và W'.K tới W' $\otimes_{\mathbf{K'}} \mathbf{K}$; do đó các khẳng định của Mệnh đề 2 là hệ quả của Định nghĩa 2 và § 7, no. 9, Mệnh đề 19.

#### Hệ quả 1 {#alg-ii-s8-prop-2-cor-1 .statement}

*Mọi tổng và mọi giao của các không gian con K-vectơ của V hữu tỉ trên K' đều là một không gian con hữu tỉ trên K'*

Mệnh đề về các tổng là hiển nhiên. Mặt khác, nếu $(W'_i)_{i \in I}$ là một họ các không gian con vectơ-$\mathbf{K}'$ của $V'$, thì $\left( \bigcap_{i \in I} W'_i \right) \otimes_{\mathbf{K}'} \mathbf{K} = \bigcap_{i \in I} (W_i \otimes_{\mathbf{K}'} \mathbf{K})$ (§ 7, no. 7, Hệ quả của Mệnh đề 14), do đó chứng minh hệ quả.

Một cơ sở $B$ của $V$ trên $\mathbf{K}$ được gọi là *hữu tỉ trên $\mathbf{K}'$* nếu nó gồm các vectơ hữu tỉ trên $\mathbf{K}'$.

#### Hệ quả 2 {#alg-ii-s8-prop-2-cor-2 .statement}

*Mọi cơ sở của $V$ trên $\mathbf{K}$ hữu tỉ trên $\mathbf{K}'$ đều là một cơ sở của $V'$ trên $\mathbf{K}'$.*

Nếu $W'$ là không gian con vectơ-$\mathbf{K}'$ của $V'$ do $B$ sinh ra, thì $W'.\mathbf{K} = V = V'.\mathbf{K}$, do đó $V' = W'$ theo Mệnh đề 2.

### 3. TÍNH HỮU TỈ ĐỐI VỚI MỘT ÁNH XẠ TUYẾN TÍNH

#### Định nghĩa 3 {#alg-ii-s8-def-3 .statement}

*Cho $V_1, V_2$ là hai không gian vectơ phải trên $\mathbf{K}$ với các cấu trúc $\mathbf{K}'$ lần lượt là $V'_1, V'_2$. Một ánh xạ $\mathbf{K}$-tuyến tính $f : V_1 \to V_2$ được gọi là hữu tỉ trên $\mathbf{K}'$ nếu $f(V'_1) \subset V'_2$.*

Nếu $V_3$ là một không gian vectơ phải thứ ba trên $\mathbf{K}$, với một cấu trúc $\mathbf{K}'$ là $V'_3$ và một ánh xạ $\mathbf{K}$-tuyến tính $g : V_2 \to V_3$ hữu tỉ trên $\mathbf{K}'$, rõ ràng $g \circ f : V_1 \to V_3$ là hữu tỉ trên $\mathbf{K}'$.

#### Mệnh đề 3 {#alg-ii-s8-prop-3 .statement}

*Cho $V_1, V_2$ là hai không gian vectơ phải trên $\mathbf{K}$ và $V'_1, V'_2$ là các cấu trúc $\mathbf{K}'$ trên $V_1, V_2$ tương ứng. $V_1$ (resp. $V_2$) được đồng nhất một cách chính tắc với $V'_1 \otimes_{\mathbf{K}'} \mathbf{K}$ (resp. $V'_2 \otimes_{\mathbf{K}'} \mathbf{K}$) (no. 1, Mệnh đề 1).

(i) *Ánh xạ $f' \mapsto f' \otimes 1_{\mathbf{K}} = f'_{(\mathbf{K})}$ là một song ánh từ $\mathrm{Hom}_{\mathbf{K}'}(V'_1, V'_2)$ lên tập các ánh xạ $\mathbf{K}$-tuyến tính từ $V_1$ vào $V_2$ mà hữu tỉ trên $\mathbf{K}'$; song ánh ngược gán cho mỗi ánh xạ $\mathbf{K}$-tuyến tính $f : V_1 \to V_2$ hữu tỉ trên $\mathbf{K}'$ ánh xạ $\mathbf{K}'$-tuyến tính $f' : V'_1 \to V'_2$ có cùng đồ thị với hạn chế của $f$ lên $V'_1$.

(ii) *Đối với mọi ánh xạ tuyến tính $\mathbf{K}$ $f : V_1 \to V_2$ hữu tỉ trên $\mathbf{K}'$,

$$
f(V'_1) = f(V_1) \cap V'_2 \quad \text{và} \quad f^{-1}(V'_2) = V'_1 + \mathrm{Ker}(f).
$$

(i) Rõ ràng với các nhận dạng ở trên, nếu $f' : V'_1 \to V'_2$ là một ánh xạ tuyến tính $\mathbf{K}'$, $f'_{(\mathbf{K})} = f' \otimes 1_{\mathbf{K}}$ là hữu tỉ trên $\mathbf{K}'$ và $f'$ là ánh xạ có cùng đồ thị với hạn chế của $f'_{(\mathbf{K})}$ lên $V'_1$. Ngược lại, nếu $f : V_1 \to V_2$ là một ánh xạ tuyến tính $\mathbf{K}$ hữu tỉ trên $\mathbf{K}'$ và $f' : V'_1 \to V'_2$ có cùng đồ thị với hạn chế của $f$ lên $V'_1$, $f$ và $f'_{(\mathbf{K})}$ trùng nhau trên $V'_1$, mà đây là một hệ sinh của $V_1$ trên $\mathbf{K}$, do đó $f = f'_{(\mathbf{K})}$.

(ii) Nếu $f = f' \otimes 1_{\mathbf{K}}$, thì $f(V_1) = f(V'_1 \otimes_{\mathbf{K}'} \mathbf{K}) = f'(V'_1) \otimes_{\mathbf{K}'} \mathbf{K}$ và, vì $f'(V'_1) \subset V'_2, f(V'_1) = f'(V'_1) \cap V'_2$ (§ 7, no. 9, Mệnh đề 19); công thức $f^{-1}(V'_2) = V'_1 + \mathrm{Ker}(f)$ suy ra ngay lập tức.

#### Hệ quả 1 {#alg-ii-s8-prop-3-cor-1 .statement}

Theo ký hiệu của Mệnh đề 3, $\operatorname{Im}(f) = (\operatorname{Im}(f'))_{(\mathbf{K})}$,
$$
\operatorname{Ker}(f') = (\operatorname{Ker}(f'))_{(\mathbf{K})}, \quad \operatorname{Coker}(f) = (\operatorname{Coker}(f'))_{(\mathbf{K})}.
$$
Đặc biệt, để $f$ là đơn ánh (tương ứng toàn ánh, không), điều kiện cần và đủ là $f'$ cũng như vậy. Nếu $f$ là song ánh, ánh xạ nghịch đảo của nó là hữu tỉ trên $\mathbf{K}'$.

Đây là một trường hợp riêng của § 7, no. 9, Hệ quả của Mệnh đề 18.

#### Hệ quả 2 {#alg-ii-s8-prop-3-cor-2 .statement}

Cho $f : V_1 \to V_2$ là một ánh xạ tuyến tính $\mathbf{K}$ hữu tỉ trên $\mathbf{K}'$. Đối với mọi không gian con vectơ-$\mathbf{K}$ $W_1$ của $V_1$ (tương ứng $W_2$ của $V_2$) hữu tỉ trên $\mathbf{K}'$, $f(W_1)$ (tương ứng $f^{-1}(W_2)$) là một không gian con vectơ-$\mathbf{K}$ của $V_2$ (tương ứng $V_1$) hữu tỉ trên $\mathbf{K}'$.

Theo ký hiệu của Mệnh đề 3, với mọi không gian con vectơ-$\mathbf{K}'$ $W'_1$ của $V'_1$, $f'_{(\mathbf{K})}(W'_1 \otimes_{\mathbf{K}'} \mathbf{K}) = f'(W'_1) \otimes_{\mathbf{K}'} \mathbf{K}$; suy ra mệnh đề liên hệ đến $W_1$ (no. 2, Mệnh đề 2). Mặt khác, hãy lấy $W'_2$ là một không gian con vectơ-$\mathbf{K}'$ của $V'_2$ và gọi $g'$ là ánh xạ tuyến tính chính tắc $\mathbf{K}'$ $V'_2 \to V'_2/W'_2$; khi đó $f'(W'_2) = \operatorname{Ker}(g' \circ f')$; do đó, theo Hệ quả 1,
$$
{f'_{(\mathbf{K})}}^{-1}(W'_2 \otimes_{\mathbf{K}'} \mathbf{K}) = {f'}^{-1}(W'_2) \otimes_{\mathbf{K}'} \mathbf{K},
$$
suy ra mệnh đề liên hệ đến $W_2$.

Hãy cho $V_1, V_2$ là hai không gian vectơ phải $\mathbf{K}$ với các cấu trúc $\mathbf{K}'$ $V'_1, V'_2$ tương ứng. Hiển nhiên rằng $V'_1 \times V'_2$ là một cấu trúc $\mathbf{K}'$ trên $V_1 \times V_2$, gọi là tích của các cấu trúc $\mathbf{K}'$ $V'_1$ và $V'_2$.

#### Mệnh đề 4 {#alg-ii-s8-prop-4 .statement}

Để một ánh xạ tuyến tính $\mathbf{K}$ $f : V_1 \to V_2$ là hữu tỉ trên $\mathbf{K}'$, điều kiện cần và đủ là đồ thị $\Gamma$ của nó hữu tỉ trên $\mathbf{K}'$ đối với cấu trúc $\mathbf{K}'$ tích trên $V_1 \times V_2$.

Hãy cho $g$ là ánh xạ $x_1 \mapsto (x_1, f(x_1))$ từ $V_1$ đến $V_1 \times V_2$; đây là một ánh xạ tuyến tính $\mathbf{K}$ sao cho $\Gamma = g(V_1)$; nếu $f$ hữu tỉ trên $\mathbf{K}'$, thì $\Gamma$ cũng hữu tỉ nhờ Hệ quả 2 của Mệnh đề 3. Ngược lại, giả sử rằng $\Gamma$ hữu tỉ trên $\mathbf{K}'$ và hãy cho nó cấu trúc $\mathbf{K}'$ cảm sinh bởi cấu trúc đó trên $V_1 \times V_2$; suy ra ngay từ các định nghĩa rằng các hạn chế $p_1, p_2$ của các phép chiếu $\mathrm{pr}_1, \mathrm{pr}_2$ lên $\Gamma$, là các ánh xạ tuyến tính $\mathbf{K}$, hữu tỉ trên $\mathbf{K}'$ từ $\Gamma$ vào $V_1$ và $V_2$ tương ứng. Vì $p_1$ là song ánh, ánh xạ nghịch đảo của nó $q_1$ là hữu tỉ trên $\mathbf{K}'$ (Hệ quả 1 của Mệnh đề 3) và do đó $f = p_2 \circ q_1$ cũng vậy.

### 4. CÁC DẠNG TUYẾN TÍNH HỮU TỈ

### 5. ỨNG DỤNG VÀO CÁC HỆ PHƯƠNG TRÌNH TUYẾN TÍNH

Cho $V$ là một không gian vectơ phải trên $\mathbf{K}$ với một $\mathbf{K}'$-cấu trúc $V'$. Vì $K'_d$ là một $\mathbf{K}'$-cấu trúc trên không gian vectơ phải $\mathbf{K}$-không gian $K_d$, ta có thể định nghĩa các dạng tuyến tính $x^* \in V^*$, hữu tỉ trên $\mathbf{K}'$, như các ánh xạ tuyến tính của $V$ vào $K_d$, hữu tỉ trên $\mathbf{K}'$ đối với các $\mathbf{K}'$-cấu trúc trên $V$ và $K_d$. Nhờ no. 3, Mệnh đề 3, tập $R'$ gồm các dạng tuyến tính này là ảnh của đối ngẫu ${V'}^*$ của $V'$ qua ánh xạ hợp thành

(I) $$ {V'}^* \xrightarrow{\phi} K \otimes_{K'} {V'}^* \xrightarrow{\upsilon} V^* $$

trong đó $\phi({x'}^*) = 1 \otimes {x'}^*$ và $\upsilon(\xi \otimes {x'}^*)$ là dạng tuyến tính $y^*$ trên V sao cho $y^*(x') = \xi \langle {x'}^*, x' \rangle$ với mọi $x' \in V'$ (§ 5, no. 4). Ta biết rằng ánh xạ này là đơn ánh (§ 7, no. 9, Mệnh đề 20 và 19) và rõ ràng $R'$ là một không gian con vectơ trái trên $K'$ của $V^*$; hơn nữa mọi tập con của $R'$ tự do trên $K'$ đều tự do trên $K$. Nhưng nói chung $R'$ không nhất thiết sinh $V^*$ trên $K$ và do đó không xác định một $\mathbf{K}'$-cấu trúc trên $V^*$ (Bài tập 2). Tuy nhiên, nếu V có số chiều hữu hạn n trên K, thì ${V'}^*$ có chiều n trên $K'$ và khi đó $R'$ xác định một cách chính tắc một $\mathbf{K}'$-cấu trúc trên $V^*$.

#### Mệnh đề 5 {#alg-ii-s8-prop-5 .statement}

Cho V là một không gian vectơ phải trên K, V' một $\mathbf{K}'$-cấu trúc trên V và W là một không gian con $K$-vectơ của V. Để W hữu tỉ trên $K'$, điều kiện cần và đủ là tồn tại một tập $H \subset V^*$ gồm các dạng tuyến tính hữu tỉ trên $K'$ sao cho W là trực giao của H trong V (§ 2, no. 4).

Cho H là một tập con của $V^*$ mà các phần tử của nó là các dạng tuyến tính hữu tỉ trên $K'$. Với mọi $x^* \in H$, hạt nhân của $x^*$ là một không gian con $K$-vectơ của V, hữu tỉ trên $K'$ (no. 3, Hệ quả 2 của Mệnh đề 3); do đó giao của các hạt nhân này cũng là một không gian con $K$-vectơ của V, hữu tỉ trên $K'$ (no. 2, Hệ quả 1 của Mệnh đề 2).

Ngược lại, cho W là một không gian con $K$-vectơ của V hữu tỉ trên $K'$, do đó W được đồng nhất với $W' \otimes_{K'} K$, trong đó $W' = W \cap V'$ (no. 2, Mệnh đề 2). Để một dạng tuyến tính ${x'}^* \in {V'}^*$ triệt tiêu trên $W'$, điều kiện cần và đủ là dạng tuyến tính $x^* \in V^*$ tương ứng với nó qua (1) triệt tiêu trên W, vì theo no. 3, Hệ quả I của Mệnh đề 3,

$$
\operatorname{Ker}(x^*) = (\operatorname{Ker}({x'}^*)) \otimes_{K'} K \quad \text{and} \quad \operatorname{Ker}(x^{*\prime}) = (\operatorname{Ker}(x^*)) \cap V'.
$$

Cho H' là trực giao của W' trong ${V'}^*$; ta biết (§ 7, no. 5, Định lý 7) rằng W' là trực giao của H' trong V'; nếu H là ảnh của H' trong $V^*$ qua ánh xạ (1), thì từ điều trên suy ra rằng W là trực giao của H trong V, xét đến no. 7, Hệ quả của Mệnh đề 14.

#### Mệnh đề 6 {#alg-ii-s8-prop-6 .statement}

(i) Cho một hệ phương trình tuyến tính thuần nhất

(2)
$$
\sum_{i \in I} \alpha_{\mu i} \xi_i = 0 \quad (\mu \in M)
$$
có các hệ số $\alpha_{\mu i}$ thuộc K', mọi nghiệm $(\xi_i)$ của hệ này gồm các phần tử của K đều là một tổ hợp tuyến tính với hệ số trong K của các nghiệm $(\xi'_i)$ của (2) gồm các phần tử của K'.

(ii) *Cho một hệ phương trình tuyến tính*

$$
\sum_{i \in I} \alpha_{\mu i} \xi_i = \beta_\mu \quad (\mu \in M)
$$

*mà các hệ số* $\alpha_{\mu i}$ *và các vế phải* $\beta_\mu$ *thuộc* $K'$, *nếu tồn tại một nghiệm của hệ gồm các phần tử của* $K$, *thì cũng tồn tại một nghiệm gồm các phần tử của* $K'$.

(i) Với mỗi tập S, cho không gian vectơ phải $K$-không gian $K_d^{(S)}$ mang cấu trúc $K'$ $K_{d'}^{(S)}$. Cho $f$ là ánh xạ tuyến tính trên K của $K_d^{(I)}$ vào $K_d^{(M)}$, ánh xạ mỗi vectơ $(\xi_i)_{i \in I}$ tới vectơ $(\zeta_\mu)_{\mu \in M}$ được xác định bởi $\zeta_\mu = \sum_{i \in I} \alpha_{\mu i} \xi_i$ với mọi $\mu \in M$. Rõ ràng $f$ là hữu tỉ trên $K'$; hạt nhân V của nó, tức là tập các nghiệm trong K của hệ (2), là một không gian con của $K_d^{(I)}$ hữu tỉ trên $K'$ (no. 3, Hệ quả 2 của Mệnh đề 3) và do đó được sinh bởi các nghiệm của (2) trong $K'$.

(ii) Ta xét K như một không gian vectơ trái trên $K'$; tồn tại một phép chiếu $K'$-tuyến tính $p$ của K lên không gian con vectơ $K'_s$ của nó (§ 7, no. 3, Mệnh đề 4); nếu $(\xi_i)$ là một nghiệm của (3) trong K, thì $\sum_{i \in I} \alpha_{\mu i} p(\xi_i) = p \left( \sum_{i \in I} \alpha_{\mu i} \xi_i \right) = p(\beta_\mu) = \beta_\mu$, điều đó chứng tỏ rằng $(p(\xi_i))$ là một nghiệm của (3) trong $K'$.

==========

Đó là toàn bộ đoạn trích. Chỉ viết bản dịch của mọi thứ ở giữa hai dòng, và dừng ở đó.

Một vành K được gọi là (trái) *phẳng trung thành* trên một vành con $K'$ nếu Mệnh đề 6 đúng cho K và $K'$; ta sẽ khảo sát khái niệm này chi tiết hơn sau (*Commutative Algebra*, I, § 3).

### 6. TRƯỜNG HỮU TỈ NHỎ NHẤT

Cho V là một K-không gian vectơ phải với một $K'$-cấu trúc $V'$. Với mọi trường L sao cho $K' \subset L \subset K$, ta đặt $V_L = V'.L$; rõ ràng mọi cơ sở của $V'$ trên $K'$ đều là cơ sở của V trên K và là cơ sở của $V_L$ trên L. Do đó $V_L$ là một L-cấu trúc trên V và $V'$ là một $K'$-cấu trúc trên $V_L$.

#### Mệnh đề 7 {#alg-ii-s8-prop-7 .statement}

(i) *Cho V là một K-không gian vectơ phải với một $K'$-cấu trúc $V'$. Với mọi vectơ $x \in V$ (tương ứng với mọi không gian con vectơ trên K W của V), tập các trường con L của K chứa $K'$ và sao cho $x$ (tương ứng với W) là hữu tỉ trên L có một phần tử nhỏ nhất $K'(x)$ (tương ứng với $K'(W)$).

(ii) *Cho $V_1, V_2$ là hai K-không gian vectơ phải với các $K'$-cấu trúc $V_1', V_2'$ tương ứng. Với mọi ánh xạ K-tuyến tính f của $V_1$ vào $V_2$, tập các trường con L của K chứa $K'$ và sao cho f là hữu tỉ trên L có một phần tử nhỏ nhất $K'(f)$*.

Trước hết ta chứng minh mệnh đề (i) đối với một vectơ $x \in V$. Cho B là một cơ sở của V hữu tỉ trên $K'$; B là một cơ sở của $V'$ trên $K'$ và là một cơ sở của $V_L$ trên L với mọi trường L sao cho $K' \subset L \subset K$; để $x = \sum_{b \in B} b \xi_b$ hữu tỉ trên L, điều kiện cần và đủ là các $\xi_b$ thuộc L (no. 2), và do đó trường L nhỏ nhất có tính chất này là trường *sinh bởi* K' và các $\xi_b$ với $b \in B$.

Tiếp theo ta chứng minh (ii). Cho $B_1, B_2$ lần lượt là các cơ sở của $V_1, V_2$, hữu tỉ trên $K'$, và viết, với mọi $b_1 \in B_1$, $f(b_1) = \sum_{b_2 \in B_2} b_2 \alpha_{b_2 b_1}$ (*họ* $(\alpha_{b_2 b_1})$ chính là *ma trận* của $f$ theo các cơ sở $B_1$ và $B_2$; xem § 10, no. 4). Vì $B_1$ (tương ứng với $B_2$) là một cơ sở của $(V_1)_L$ (tương ứng với $(V_2)_L$) trên L với mọi trường sao cho $K' \subset L \subset K$, nên để $f$ hữu tỉ trên L, điều kiện cần và đủ là các $\alpha_{b_2 b_1}$ thuộc L; vì thế trường nhỏ nhất có tính chất này là trường *sinh bởi* K' và các $\alpha_{b_2 b_1}$ với $b_1 \in B_1, b_2 \in B_2$.

Sau cùng, để chứng minh mệnh đề (i) cho một không gian con W của V, trước hết ta chứng minh bổ đề sau:

#### Bổ đề 1 {#alg-ii-s8-lem-1 .statement}

*Cho V là một K-không gian vectơ phải với một $K'$-cấu trúc $V'$ và W là một không gian con vectơ trên K của V. Tồn tại hai không gian con vectơ trên K $W_1, W_2$ của V, hữu tỉ trên $K'$, sao cho V là tổng trực tiếp của $W_1$ và $W_2$ và, nếu đồng nhất V với $W_1 \times W_2$, thì W là đồ thị của một ánh xạ K-tuyến tính g từ $W_1$ vào $W_2$.*

Cho B là một cơ sở của V hữu tỉ trên K'. Áp dụng Định lý 2 của § 7, no. 1, cho một cơ sở của W trên K, xem như một tập con tự do của V, và cho hệ sinh là hợp của tập con tự do này và B, ta thấy rằng tồn tại một tập con C của B sao cho V là tổng trực tiếp của W và không gian con $W_2$ của V sinh bởi C. Đồng thời, đặt $W_1$ là không gian con của V sinh bởi $B - C$. Vì $B \subset V'$, rõ ràng $W_1$ và $W_2$ đều hữu tỉ trên K'. Hơn nữa, với mọi $x \in W_1$, tồn tại duy nhất một vectơ $g(x)$ của $W_2$ sao cho $x + g(x) \in W$, vì V là tổng trực tiếp của W và $W_2$; khi đó W là đồ thị của g và g là K-tuyến tính vì W là một không gian con vectơ K của V.

Sau khi chứng minh bổ đề này, ta biết rằng W hữu tỉ trên một trường con L của K chứa K' nếu và chỉ nếu g hữu tỉ trên L (no. 3, Mệnh đề 4). Vì vậy, trường nhỏ nhất $K'(g)$ sao cho g hữu tỉ trên $K'(g)$ cũng là trường nhỏ nhất mà W hữu tỉ trên đó.

### 7. CÁC TIÊU CHUẨN VỀ TÍNH HỮU TỈ

Với mọi trường con L của K, ký hiệu $\mathrm{End}_L(K)$ là vành tự đồng cấu của K, xét K như một *không gian vectơ trái* trên L; nếu L chứa K', thì $\mathrm{End}_L(K)$ là một vành con của $\mathrm{End}_{K'}(K)$. Với mọi tập con $\mathcal{M}$ của $\mathrm{End}_{K'}(K)$, tồn tại một *trường con lớn nhất* L của K chứa K' và sao cho $\mathcal{M}$ được chứa trong $\mathrm{End}_L(K)$, cụ thể là tập các $\xi \in K$ sao cho $\phi(\xi \eta) = \xi \cdot \phi(\eta)$ với mọi $\eta \in K$ và mọi $\phi \in \mathcal{M}$ (ngay lập tức kiểm tra được rằng tập này là một vành và, mặt khác, thay $\eta$ bởi $\xi^{-1} \eta$ trong quan hệ trên, ta thu được $\phi(\xi^{-1} \eta) = \xi^{-1} \cdot \phi(\eta)$ khi $\xi \neq 0$). Ta sẽ gọi trường này là *trường trung tâm hóa* của $\mathcal{M}$ trong K và ký hiệu nó là $\chi(\mathcal{M})$.

Bây giờ cho V là một không gian vectơ phải trên K với một cấu trúc K' là V'. Với mọi $\phi \in \mathrm{End}_{K'}(K)$, tồn tại duy nhất một tự đồng cấu $\phi_V$ của $\mathbf{Z}$-môđun V sao cho $\phi_V(x'.\xi) = x'.\phi(\xi)$ với $x' \in V'$ và $\xi \in K$: vì, ở no. 1, đã định nghĩa một đẳng cấu $\mathbf{Z}$ $\lambda$ của $V' \otimes_{K'} K$ lên V, ánh xạ $x' \otimes \xi$ thành $x'.\xi$, và $\phi_V$ tất yếu bằng $\lambda \circ (1_{V'} \otimes \phi) \circ \lambda^{-1}$.

#### Định lý 1 {#alg-ii-s8-thm-1 .statement}

*Cho $\mathcal{M}$ là một tập con của $\mathrm{End}_{K'}(K)$ và $L = \chi(\mathcal{M})$ là trường con của K, trường trung tâm hóa của $\mathcal{M}$.*

(i) *Cho V là một không gian vectơ phải trên K với một cấu trúc K'. Để một vectơ $x \in V$ hữu tỉ trên L, cần và đủ rằng $\phi_V(x.\eta) = x.\phi(\eta)$ với mọi $\phi \in \mathcal{M}$ và mọi $\eta \in K$. Để một không gian con vectơ K W của V hữu tỉ trên L, cần và đủ rằng $\phi_V(W) \subset W$ với mọi $\phi \in \mathcal{M}$.*

(ii) *Cho $V_1, V_2$ là hai không gian vectơ phải trên K, mỗi không gian có một cấu trúc K'. Để một ánh xạ K-tuyến tính f từ $V_1$ vào $V_2$ hữu tỉ trên L, cần và đủ rằng $f(\phi_{V_1}(x_1)) = \phi_{V_2}(f(x_1))$ với mọi $x_1 \in V_1$ và mọi $\phi \in \mathcal{M}$.*

Trước hết, ta chứng minh mệnh đề (i) đối với x. Cho B là một cơ sở của V hữu tỉ trên K' và viết $x = \sum_{b \in B} b.\xi_b$; khi đó, với $\phi \in \mathcal{M}$ và $\eta \in K$,

$$
\phi_V(x.\eta) - x.\phi(\eta) = \sum_{b \in B} b.(\phi(\xi_b\eta) - \xi_b.\phi(\eta))
$$

và do đó, các quan hệ

"với mọi $\phi \in \mathcal{M}$ và mọi $\eta \in K$, $\phi_V(x.\eta) = x.\phi(\eta)$"

và

"với mọi $\phi \in \mathcal{M}$, mọi $b \in B$ và mọi $\eta \in K$, $\phi(\xi_b\eta) = \xi_b.\phi(\eta)$"

là tương đương. Quan hệ thứ hai trong số đó có nghĩa là với mọi $b \in B$, $\xi_b \in \chi(\mathcal{M})$, điều này chứng minh mệnh đề thứ nhất của (i).

Tiếp theo, ta chứng minh (ii). Để f hữu tỉ trên L, điều cần và đủ là, với mọi $x'_1 \in V_1$ hữu tỉ trên K', $f(x'_1)$ là một vectơ trong $V_2$ hữu tỉ trên L; điều này sẽ kéo theo rằng $f(x_1)$ hữu tỉ trên L với mọi vectơ $x_1$ của $V_1$ hữu tỉ trên L, vì một vectơ như vậy là một tổ hợp tuyến tính với các hệ số trong L của các vectơ hữu tỉ trên K'. Điều kiện trên, theo phần đầu của lập luận, tương đương với quan hệ

$$
f(x'_1).\phi(\eta) = \phi_{V_2}(f(x'_1).\eta) \quad \text{với } \phi \in \mathcal{M} \text{ và } \eta \in K
$$

có thể cũng được viết

$$
f(\phi_{V_1}(x'_1.\eta)) = \phi_{V_2}(f(x'_1.\eta)) \quad \text{với } \phi \in \mathcal{M} \text{ và } \eta \in K.
$$

Vì mọi phần tử của $V_1$ là một tổ hợp tuyến tính với các hệ số trong K của các phần tử của $V_1$ hữu tỉ trên K', điều kiện (5) tương đương với

$$
f(\phi_{V_1}(x_1)) = \phi_{V_2}(f(x_1))
$$

với mọi $x_1 \in V_1$ và mọi $\phi \in \mathcal{M}$.

Cuối cùng, để chứng minh mệnh đề thứ hai trong (i), ta dùng no. 6, Bổ đề 1: W là đồ thị của một ánh xạ K-tuyến tính $g : W_1 \to W_2$ và W hữu tỉ trên nếu và chỉ nếu ánh xạ g hữu tỉ trên L (no. 3, Mệnh đề 4). Theo (ii), để g hữu tỉ trên L, điều cần và đủ là $g(\phi_{W_1}(x_1)) = \phi_{W_2}(g(x_1))$ với mọi $x_1 \in W_1$ và mọi $\phi \in \mathcal{M}$; vì $\phi_v = \phi_{W_1} \times \phi_{W_2}$, điều kiện trên có nghĩa là đồ thị W của g ổn định dưới $\phi_v$ với mọi $\phi \in \mathcal{M}$.

### Bài tập {#alg-ii-s8-exercises}

Xem [các bài tập cho § 8](exercises/s8/).
