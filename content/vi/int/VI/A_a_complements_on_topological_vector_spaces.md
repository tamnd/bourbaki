---
book: int
book_title: Integration
chapter: VI
chapter_title: VECTORIAL INTEGRATION
section: 0
section_title: Complements on topological vector spaces
appendix: true
lang: vi
source: int-i-vi
pdf_pages: 0443-0447
extraction: ocr
subsections:
    - "no": 1
      title: Bilinear forms and linear mappings
      page: 0
      pdf_page: 443
    - "no": 2
      title: Some types of spaces having the property (GDF)
      page: 54
      pdf_page: 445
statements: 6
exercises: 0
content_sha256: ad99cf104d37deed8b6e313753fb8b48df44937572cdaadbafbf6f48329f536e
translated_from: content/en/int/VI/A_a_complements_on_topological_vector_spaces.md
source_content_sha256: 6c29684424d0e54d3567600bfd0da184a2868123d0169b2729df44f5b5c07f28
translation_model: gpt-5.4-mini
translation_run: translate-vi-8e8fb815
glossary_version: 34
glossary_terms_sha256: ec5b3f1c67f7153beea9f57289360fb414f8462a6da3eb5c829fbca7f21bb019
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## PHỤ LỤC

# Bổ sung về các không gian vectơ tôpô

### 1. Các dạng song tuyến tính và các ánh xạ tuyến tính

Cho $ (F_1, G_1), (F_2, G_2) $ là hai cặp không gian vectơ (thực hoặc phức) trong đối ngẫu tách biệt (TVS, II, §6, No. 1); giả sử mỗi không gian này được trang bị tôpô yếu tương ứng (*loc. cit.*, No. 2); nếu A và B là bất kỳ hai không gian nào trong các không gian này, như thường lệ ta ký hiệu $ \mathcal{L}(A; B) $ là không gian vectơ các ánh xạ tuyến tính liên tục của A vào B, và $ \mathfrak{B}(A, B) $ là không gian vectơ các dạng song tuyến tính *liên tục riêng rẽ* trên $ A \times B $.

Với mọi dạng song tuyến tính liên tục riêng rẽ $ \Phi $ trên $ F_1 \times F_2 $, $ x_1 \mapsto \Phi(x_1, x_2) $ là một dạng tuyến tính liên tục trên $ F_1 $, do đó tồn tại một và chỉ một phần tử $ {}^r\Phi(x_2) \in G_1 $ sao cho

$$
\Phi(x_1, x_2) = \langle x_1, {}^r\Phi(x_2) \rangle
$$

với $ x_1 \in F_1, x_2 \in F_2 $ (TVS, III, §5, No. 1, (1)). Hơn nữa, công thức này cho thấy ánh xạ $ x_2 \mapsto {}^r\Phi(x_2) $ là tuyến tính và liên tục đối với các tôpô (yếu) của $ F_2 $ và $ G_1 $. Ngược lại, với mọi ánh xạ tuyến tính liên tục $ u $ từ $ F_2 $ vào $ G_1 $, $ (x_1, x_2) \mapsto \Phi(x_1, x_2) = \langle x_1, u(x_2) \rangle $ là một dạng song tuyến tính liên tục riêng rẽ trên $ F_1 \times F_2 $, và $ {}^r\Phi = u $. Do đó ta định nghĩa một đẳng cấu $ r : \Phi \mapsto {}^r\Phi $ của $ \mathfrak{B}(F_1, F_2) $ lên $ \mathcal{L}(F_2; G_1) $, được gọi là *chính tắc*.

Tương tự, công thức

$$
\Phi(x_1, x_2) = \langle {}^l\Phi(x_1), x_2 \rangle
$$

xác định một *đẳng cấu chính tắc* $ l : \Phi \mapsto {}^l\Phi $ của $ \mathfrak{B}(F_1, F_2) $ lên $ \mathcal{L}(F_1; G_2) $; và hiển nhiên ta có biểu đồ giao hoán

$$
\begin{array}{ccc}
\mathcal{B}(F_1, F_2) & & \\
l & l^{-1} & r^{-1} \\
& & \\
\mathcal{L}(F_1; G_2) & \xleftarrow{t} & \mathcal{L}(F_2; G_1)
\end{array}
$$

trong đó $ t $ là đẳng cấu chuyển vị $ u \mapsto {}^t u $. Xét theo định nghĩa các tôpô yếu trên $ G_1 $ và $ G_2 $, hơn nữa hiển nhiên rằng khi $ \mathcal{B}(F_1, F_2) $, $ \mathcal{L}(F_1; G_2) $ và $ \mathcal{L}(F_2; G_1) $ được trang bị tôpô hội tụ điểm, các đẳng cấu trong biểu đồ trên là các đẳng cấu của cấu trúc không gian vectơ tôpô.

Bây giờ cho $ E, F $ là hai không gian lồi địa phương Hausdorff, $ E', F' $ là các không gian đối ngẫu tương ứng của chúng; ta ký hiệu $ E_\sigma, F_\sigma $ là các không gian $ E, F $ được trang bị các tôpô yếu hóa $ \sigma(E, E') $, $ \sigma(F, F') $, và $ E'_s, F'_s $ là các không gian $ E', F' $ được trang bị các tôpô yếu $ \sigma(E', E) $, $ \sigma(F', F) $. Vì thế, các nhận xét trên thiết lập các đẳng cấu chính tắc giữa ba không gian $ \mathcal{B}(E_\sigma, F'_s) $, $ \mathcal{L}(E_\sigma; F_\sigma) $ và $ \mathcal{L}(F'_s; E'_s) $, và cũng giữa ba không gian $ \mathcal{B}(E_\sigma, F_\sigma) $, $ \mathcal{L}(E_\sigma; F'_s) $ và $ \mathcal{L}(F_\sigma; E'_s) $. Ta sẽ nhận thấy rằng $ \mathcal{B}(E_\sigma, F_\sigma) $ cũng bằng không gian $ \mathcal{B}(E, F) $ các dạng song tuyến tính liên tục riêng rẽ trên $ E \times F $ ($ E $ và $ F $ được trang bị các tôpô ban đầu của chúng), vì mọi dạng tuyến tính liên tục trên $ E $ (resp. $ F $) đều liên tục trên $ E_\sigma $ (resp. $ F_\sigma $) và ngược lại (TVS, II, §6, No. 1 and No. 2, Mệnh đề 3).

Cho $ \mathcal{B}(E, F) $ là không gian các dạng song tuyến tính liên tục trên $ E \times F $ ($ E $ và $ F $ được trang bị với các tôpô ban đầu của chúng); thì $ \mathcal{B}(E, F) \subset \mathcal{B}(E, F) $.

#### Mệnh đề 1 {#int-vi-a0-prop-1 .statement}

*Để một dạng song tuyến tính $ \Phi \in \mathcal{B}(E, F) $ thuộc $ \mathcal{B}(E, F) $, điều cần và đủ là tồn tại một lân cận của 0 trong $ E $ mà ảnh của nó qua $ {}^l \Phi $ là một tập con đều liên tục của $ F' $.*

Thật vậy, nói rằng $ \Phi $ liên tục có nghĩa là tồn tại một lân cận lồi cân bằng $ V $ (resp. $ W $) của 0 trong $ E $ (resp. $ F $) sao cho $ |\Phi(x, y)| \leq 1 $ với $ x \in V $, $ y \in W $; điều này có thể viết là $ |\langle {}^l \Phi(x), y \rangle| \leq 1 $ với $ x \in V $, $ y \in W $, hoặc cũng có thể là $ {}^l \Phi(V) \subset W^\circ $; do đó suy ra mệnh đề, lưu ý rằng mọi tập con đều liên tục của $ F' $ đều được chứa trong đối cực của một lân cận của 0 trong $ F $.

#### Hệ quả {#int-vi-a0-n1-cor-1 .statement}

*Nếu $ \Phi $ là một dạng song tuyến tính liên tục trên $ E \times F $, thì $ {}^l \Phi $ là một ánh xạ tuyến tính liên tục của $ E $ vào đối ngẫu mạnh $ F'_b $ của $ F $. Nếu, hơn nữa, $ E $ và $ F $ là các không gian chuẩn, thì $ \|{}^l \Phi\| = \|\Phi\| $.*

Khẳng định thứ nhất suy ra từ Mđ. 1 và thực tế rằng mọi lân cận của 0 trong $ F'_b $ đều hấp thụ mọi tập con đều liên tục của $ F' $. Nếu $ E $ và $ F $ là các không gian chuẩn, thì

$$
\|\Phi\| = \sup_{\|x\| \leq 1, \|y\| \leq 1} |\Phi(x, y)| = \sup_{\|x\| \leq 1} \left( \sup_{\|y\| \leq 1} |\langle l \Phi(x), y \rangle| \right)
= \sup_{\|x\| \leq 1} \|l \Phi(x)\| = \|l \Phi\|,
$$

do đó khẳng định thứ hai.

Đổi chỗ vai trò của $ E $ và $ F $, ta thu được các kết quả tương tự với Mđ. 1 và hệ quả của nó cho các ánh xạ tuyến tính $ r \Phi $; chúng tôi để cho bạn đọc nêu ra chúng.

### 2. Một số kiểu không gian có tính chất (GDF)

Ta đã biết rằng mọi không gian Fréchet đều có tính chất (GDF) (TVS, I, §3, No. 3, Hệ quả 5 của Định lý 1).

#### Mệnh đề 2 {#int-vi-a0-prop-2 .statement}

— Cho E là một không gian vectơ, $(F_\alpha)_{\alpha \in A}$ là một họ các không gian địa phương compact có tính chất (GDF), và với mỗi $\alpha \in A$ cho $h_\alpha$ là một ánh xạ tuyến tính của $F_\alpha$ vào E. Nếu E được trang bị tôpô lồi địa phương mạnh nhất làm cho các $h_\alpha$ liên tục, thì E có tính chất (GDF).

Cho $u$ là một ánh xạ tuyến tính từ E vào một không gian Banach B, sao cho mọi giới hạn trong $E \times B$ của mọi dãy hội tụ các điểm của đồ thị $\Gamma$ của $u$ cũng thuộc $\Gamma$. Chỉ cần chứng minh rằng, với mọi $\alpha \in A$, $u \circ h_\alpha$ liên tục trên $F_\alpha$ (TVS, II, §4, No. 4, Mệnh đề 5). Bây giờ, cho $(x_n)$ là một dãy các phần tử của $F_\alpha$ có giới hạn $a$ và sao cho dãy $\left(u(h_\alpha(x_n))\right)$ có giới hạn $b \in B$. Vì $h_\alpha$ liên tục, $h_\alpha(a)$ là một giới hạn của dãy $(h_\alpha(x_n))$ trong E; do đó theo giả thiết $b = u(h_\alpha(a))$ và, vì $F_\alpha$ có tính chất (GDF), $u \circ h_\alpha$ liên tục.

#### Hệ quả {#int-vi-a0-n2-cor-1 .statement}

— Mọi không gian thương của một không gian lồi địa phương có tính chất (GDF) đều có tính chất (GDF).

#### Mệnh đề 3 {#int-vi-a0-prop-3 .statement}

— Đối ngẫu mạnh của một không gian Fréchet phản xạ có tính chất (GDF).

Đây là hệ quả của Mệnh đề 2 và bổ đề sau (hoặc TVS, IV, §3, No. 4, Mệnh đề 4):

#### Bổ đề {#int-vi-a0-n2-lem-1 .statement}

Cho F là một không gian Fréchet, $F'$ là đối ngẫu mạnh của nó, $F''$ là đối ngẫu kép của nó. Nếu mọi tập con của $F''$, bị chặn đối với $\sigma(F'', F')$, đều được chứa trong bao đóng (theo $\sigma(F'', F')$) của một tập con bị chặn của F, thì $F'$ là giới hạn trực tiếp của một dãy các không gian Banach.

Thật vậy, cho $ (V_n) $ là một dãy cơ sở giảm gồm các lân cận lồi, cân bằng và đóng của 0 trong F. Với mọi số nguyên $ n $, đặt $ G_n $ là không gian con tuyến tính của $ F' $ do cực $ V_n^\circ $ của $ V_n $ sinh ra. Trong $ G_n $, $ V_n^\circ $ là một tập hợp lồi hấp thụ, do đó hàm gauge $ p_n $ của nó là một chuẩn trên $ G_n $; hơn nữa, $ V_n^\circ $ là một tập con đầy đủ của đối ngẫu mạnh $ F' $ (TVS, III, §3, No. 8, Mệnh đề 11); vì thế $ G_n $, được trang bị chuẩn $ p_n $, là một không gian Banach (GT, III, §3, No. 5, Hệ quả 2 của Mệnh đề 9). Ta sẽ chứng minh rằng tôpô mạnh trên $ F' $ là giới hạn trực tiếp của các tôpô không gian Banach này trên các $ G_n $, hay nói cách khác, để một tập con đóng mạnh, cân bằng, lồi U của $ F' $ là một lân cận mạnh của 0, điều kiện cần và đủ là U hấp thụ từng $ V_n^\circ $. Hiển nhiên điều kiện này là cần; để thấy rằng nó là đủ, chỉ cần chứng minh rằng U chứa một thùng của $ F' $. Thật vậy, khi đó cực $ U^\circ $ của nó trong $ F'' $ sẽ bị chặn đối với $ \sigma(F'', F') $, do đó, theo giả thiết, sẽ được chứa trong bao đóng (theo $ \sigma(F'', F') $) của một tập con bị chặn B của F, từ đó suy ra rằng U (vốn đóng đối với $ \sigma(F', F'') $) chứa lân cận mạnh $ B^\circ $ của 0 (TVS, II, §6, No. 3, Định lý 1 và §8, No. 4).

Theo giả thiết, với mọi số nguyên $ n $ tồn tại một số $ \lambda_n > 0 $ sao cho $ \lambda_n V_n^\circ \subset \frac{1}{2}U $; đặt $ A_n $ là bao lồi của hợp các $ \lambda_i V_i^\circ $ với $ i \leq n $. Khi đó $ A_n \subset \frac{1}{2}U $ với mọi $ n $; đặt W là hợp của các $ A_n $; W là một tập lồi, cân bằng, hấp thụ được chứa trong $ \frac{1}{2}U $, và chỉ cần chứng minh rằng bao đóng mạnh của nó (là một thùng) được chứa trong U.

Khi đó, cho $ x' $ là một điểm của $ F' $ không thuộc U. Vì mỗi $ V_n^\circ $ đều compact đối với $ \sigma(F', F) $, nên điều đó cũng đúng cho các $ A_n $ (TVS, II, §2, No. 6, Mệnh đề 15), và vì $ x' \notin 2A_n $, tồn tại một phần tử $ x_n $ thuộc polar của $ A_n $ trong F sao cho $ \langle x', x_n \rangle = 2 $ (TVS, II, §5, No. 3, Mệnh đề 4). Dãy $ (x_n) $ bị chặn trong F: thật vậy, mọi $ y' \in F' $ thuộc về một $ V_k^\circ $ nào đó, do đó $ |\langle y', x_n \rangle| \leq \lambda_k^{-1} $ đối với $ n \geq k $, do đó có mệnh đề của chúng ta (TVS, IV, §1, No. 1, Mệnh đề 1). Cho C là một tập hợp lồi, cân bằng, bị chặn trong F chứa tất cả các $ x_n $; khi đó $ C^\circ $ là một lân cận của 0 trong $ F' $, và polar $ C^{\circ\circ} $ của $ C^\circ $ trong $ F'' $ là compact đối với $ \sigma(F'', F') $ (TVS, III, §3, No. 4, Hệ quả 2 của Mệnh đề 4 và No. 5, Mệnh đề 7). Do đó thấy rằng dãy $ (x_n) $ có một điểm tụ $ x'' $ trong $ F'' $ đối với $ \sigma(F'', F') $; hiển nhiên $ \langle x', x'' \rangle = 2 $ và, mặt khác, $ x'' $ thuộc polar của $ A_n $ trong $ F'' $ với mọi $ n $, nên thuộc polar $ W^\circ $ của W trong $ F'' $. Từ đó, suy ra rằng $ x' \notin W^{\circ\circ} $, do đó không thuộc bao đóng của W đối với $ \sigma(F', F'') $ (TVS, II, §6, No. 3, Định lý 1 và §8, No. 4), do đó *a fortiori* đối với tôpô mạnh, điều này hoàn thành chứng minh.

Bài tập
