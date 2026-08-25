---
book: evt
book_title: Topological Vector Spaces
chapter: III
chapter_title: SPACES OF CONTINUOUS LINEAR MAPPINGS
section: 3
section_title: Spaces of continuous linear mappings
lang: vi
source: evt-i-v
book_pages: TVS III.13-TVS III.23, TVS III.41-TVS III.43
pdf_pages: 0145-0155, 0173-0175
extraction: ocr
subsections:
    - "no": 1
      title: The spaces $ \mathcal{L}_\mathfrak{S}(E; F) $
      page: 13
      pdf_page: 145
    - "no": 2
      title: Condition for $ \mathcal{L}_\mathfrak{S}(E; F) $ to be Hausdorff
      page: 15
      pdf_page: 147
    - "no": 3
      title: Relations between $ \mathcal{L}(E; F) $ and $ \mathcal{L}(\hat{E}; F) $
      page: 15
      pdf_page: 147
    - "no": 4
      title: Equicontinuous subsets of $ \mathcal{L}(E; F) $
      page: 16
      pdf_page: 148
    - "no": 5
      title: Equicontinuous subsets of $ E' $
      page: 19
      pdf_page: 151
    - "no": 6
      title: The completion of a locally convex space
      page: 20
      pdf_page: 152
    - "no": 7
      title: $ \mathcal{S} $-bornologies on $ \mathcal{L}(E; F) $
      page: 21
      pdf_page: 153
    - "no": 8
      title: Complete subsets of $ \mathcal{L}_{\mathcal{S}}(E; F) $
      page: 22
      pdf_page: 154
statements: 39
exercises: 13
content_sha256: b3a33ab23e717bdd9441f724bcb244230641cd0459a9671e512b34c483e25410
translated_from: content/en/evt/III/03_s3_spaces_of_continuous_linear_mappings.md
source_content_sha256: aeea6217ee0e16e1a568bfe18558a479b66f5f96008067b42ed34a7e73ebf8f7
translation_model: gpt-5-6-mini, gpt-5-6
translation_run: translate-vi-23e90a2c
glossary_version: 34
glossary_terms_sha256: 597e567767ac2e633db64859aeec9cdae6a4f43c9e364126edd4f0afddd3a1af
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 3. CÁC KHÔNG GIAN CỦA CÁC ÁNH XẠ TUYẾN TÍNH LIÊN TỤC

### 1. Các không gian $ \mathcal{L}_\mathfrak{S}(E; F) $

Cho F là một không gian vectơ tôpô, E là một tập hợp tùy ý, và $ \mathfrak{S} $ là một họ các tập con của E. Xét không gian vectơ $ F^E $ với cấu trúc đều của sự hội tụ $ \mathfrak{S} $- (GT, X, § 1, No. 2). Ta biết rằng cấu trúc này tương thích với cấu trúc nhóm giao hoán của $ F^E $ (GT, X, § 1, No. 4, cor. 2). Tôpô suy ra được gọi là $ \mathfrak{S} $*-tôpô*. Nếu X là một tập con của $ F^E $, hoặc tổng quát hơn, là một tập hợp với một ánh xạ $ j : X \to F^E $, thì ảnh toàn phần theo j của $ \mathfrak{S} $*-tôpô* trên $ F^E $ được gọi là $ \mathfrak{S} $*-tôpô* trên X.

#### Nhận xét {#evt-iii-s3-n1-rem-1 .statement}

— 1) $ \mathfrak{S} $*-tôpô* đồng nhất với $ \mathfrak{S}' $*-tôpô*, trong đó $ \mathfrak{S}' $ ký hiệu tôpô sinh bởi $ \mathfrak{S} $ (III, p. 1).

2) Cho $ M \in \mathfrak{S} $ và cho V là một lân cận của 0 trong F; ký hiệu $ T(M, V) $ là tập hợp tất cả các $ f \in F^E $ sao cho $ f(x) \in V $ với mọi $ x \in M $. Nếu $ \mathfrak{S} $ ổn định đối với các hợp hữu hạn, các tập hợp $ T(M, V) $ tạo thành một hệ cơ sở các lân cận của 0 đối với $ \mathfrak{S} $*-tôpô* của $ F^E $.

#### Mệnh đề 1 {#evt-iii-s3-prop-1 .statement}

*Cho E là một tập hợp, $ \mathfrak{S} $ là một họ các tập con của E, F là một không gian vectơ tôpô và H là một không gian con vectơ của $ F^E $. Để $ \mathfrak{S} $*-tôpô* tương thích với cấu trúc không gian vectơ của H, điều kiện cần và đủ là $ u(M) $ bị chặn trong F với mọi $ u \in H $ và mọi $ M \in \mathfrak{S} $. Hơn nữa, nếu F là lồi địa phương, thì $ \mathfrak{S} $*-tôpô* trên H là lồi địa phương.*

Dựa vào các Nhận xét 1) và 2) ở trên, ta thấy rằng một điều kiện cần và đủ để $ \mathfrak{S} $*-tôpô* tương thích với cấu trúc không gian vectơ của H là các tập hợp $ H \cap T(M, V) $ là *hấp thụ* trong H (I, p. 7, prop. 4); nhưng điều này kéo theo rằng với mọi $ u \in H $, mọi tập con $ M \in \mathfrak{S} $, và mọi lân cận cân bằng V của 0 trong F, tồn tại $ \lambda \neq 0 $ sao cho $ u(M) \subset \lambda V $; nghĩa là (III, p. 2) rằng $ u(M) $ bị chặn trong F. Cuối cùng, khẳng định cuối cùng của mệnh đề suy ra từ sự kiện rằng nếu V là lồi, thì $ T(M, V) $ cũng vậy.

#### Hệ quả {#evt-iii-s3-n1-cor-1 .statement}

*Cho E và F là hai không gian lồi địa phương, $ \mathfrak{S} $ là một họ các tập con bị chặn của E, và $ \mathcal{L}(E; F) $ là không gian vectơ của các ánh xạ tuyến tính liên tục từ E vào F. Khi đó $ \mathfrak{S} $*-tôpô* tương thích với cấu trúc không gian vectơ của $ \mathcal{L}(E; F) $ và là lồi địa phương.*

Chỉ cần nhận xét rằng nếu $ u $ là một ánh xạ tuyến tính liên tục từ E vào F và M là một tập con bị chặn của E, thì $ u(M) $ bị chặn trong F (III, p. 4, cor. 1).

Cho hai không gian vectơ lồi địa phương E và F, và một họ $ \mathfrak{S} $ gồm các tập con bị chặn của E, ký hiệu $ \mathcal{L}_\mathfrak{S}(E; F) $ là không gian lồi địa phương thu được bằng cách gán $ \mathfrak{S} $*-tôpô* cho $ \mathcal{L}(E; F) $.

#### Ví dụ 1 {#evt-iii-s3-n1-exa-1 .statement}

Nếu $ \mathfrak{S} $ là tập hợp tất cả các tập con hữu hạn của E, thì $ \mathfrak{S} $-tôpô là tôpô của *hội tụ đơn giản* và không gian $ \mathcal{L}_{\mathfrak{S}}(E; F) $ cũng được ký hiệu bởi $ \mathcal{L}_s(E; F) $. Một tập con bị chặn của $ \mathcal{L}_s(E; F) $ được gọi là một tập con bị chặn đơn giản của $ \mathcal{L}(E; F) $.

#### Ví dụ 2 {#evt-iii-s3-n1-exa-2 .statement}

Nếu $ \mathfrak{S} $ là tập hợp các tập con *compact* (tương ứng *tiền compact*, *compact lồi*), thì tôpô $ \mathfrak{S} $ được gọi là tôpô của sự hội tụ *compact* (tương ứng *tiền compact*, *compact lồi*) và không gian $ \mathcal{L}_{\mathfrak{S}}(E; F) $ còn được ký hiệu bởi $ \mathcal{L}_c(E; F) $ (tương ứng $ \mathcal{L}_{pc}(E; F) $, $ \mathcal{L}_{cc}(E; F) $). (*Xem* IV, p. 48, Bài tập 7.)

#### Ví dụ 3 {#evt-iii-s3-n1-exa-3 .statement}

Nếu $ \mathfrak{S} $ là tập hợp tất cả các tập con *bị chặn* của E, ta nói rằng tôpô $ \mathfrak{S} $ là tôpô của sự hội tụ *bị chặn* và không gian $ \mathcal{L}_{\mathfrak{S}}(E; F) $ được ký hiệu bởi $ \mathcal{L}_b(E; F) $.

#### Ví dụ 4 {#evt-iii-s3-n1-exa-4 .statement}

Khi $ F = \mathbf{K} $, không gian $ \mathcal{L}(E; F) $ là đối ngẫu $ E' $ của E. Ta ký hiệu bởi $ E'_\mathfrak{S} $, $ E'_s $ v.v. không gian $ \mathcal{L}_{\mathfrak{S}}(E; \mathbf{K}) $, $ \mathcal{L}_s(E; \mathbf{K}) $ v.v. Không gian $ E'_s $ (tương ứng $ E'_b $) được gọi là đối ngẫu yếu (tương ứng đối ngẫu mạnh) của E. Một tập con bị chặn của $ E'_s $ (tương ứng $ E'_b $) được gọi là bị chặn yếu (tương ứng bị chặn mạnh). Ta nhận xét rằng tôpô yếu trên $ E' $ không gì khác ngoài $ \sigma(E', E) $ (II, p. 42).

Khi $ E = F $, ta ký hiệu bởi $ \mathcal{L}(E) $, $ \mathcal{L}_{\mathfrak{S}}(E) $ v.v. không gian $ \mathcal{L}(E; F) $, $ \mathcal{L}_{\mathfrak{S}}(E; F) $ v.v.

Cho $ p $ là một nửa chuẩn liên tục trên F và M là một tập con bị chặn của E. Đặt

$$
p_M(u) = \sup_{x \in M} p(u(x)) .
$$

Hiển nhiên $ p_M $ là một nửa chuẩn trên $ \mathcal{L}(E; F) $ và nếu $ \Gamma $ là một hệ cơ bản các nửa chuẩn trên F, họ các nửa chuẩn $ p_M $, trong đó $ p $ chạy qua $ \Gamma $ và M chạy qua một cơ sở của bornology được sinh bởi $ \mathfrak{S} $, là một hệ cơ bản các nửa chuẩn của $ \mathcal{L}_{\mathfrak{S}}(E; F) $.

Đặc biệt, nếu E và F là các không gian nửa chuẩn, và nếu $ p $ (tương ứng $ q $) ký hiệu nửa chuẩn của E (tương ứng F), thì tôpô của sự hội tụ bị chặn trên $ \mathcal{L}(E; F) $ được xác định bởi nửa chuẩn

$$
r(u) = \sup_{p(x) \leq 1} q(u(x))
$$

(*xem* GT, X, § 3, No. 2). Khi ta xem $ \mathcal{L}_b(E; F) $ như một không gian nửa chuẩn, ta sẽ luôn luôn, trừ khi điều ngược lại được nêu rõ, hiểu nửa chuẩn (2). Nếu F là một không gian chuẩn, nửa chuẩn (2) là một chuẩn.

#### Nhận xét {#evt-iii-s3-n1-rem-2 .statement}

— 3) Cho A là một tập con trù mật của quả cầu đơn vị của E. Do tính liên tục của $ u $, ta cũng có

$$
r(u) = \sup_{x \in A} q(u(x)) .
$$

Ví dụ

$$
r(u) = \sup_{p(x) < 1} q(u(x)) .
$$

Vì ta có $ u(tx) = tu(x) $ với $ t \in \mathbf{R} $, nên ta cũng có,

$$
r(u) = \sup_{p(x) = 1} q(u(x)) = \sup_{p(x) \neq 0} \frac{q(u(x))}{p(x)} .
$$

bất cứ khi nào $ p \neq 0 $.

4) Công thức (2) chỉ ra rằng ánh xạ $ u \mapsto r(u) $ là nửa liên tục dưới trên $ \mathcal{L}_s(E; F) $.

#### Mệnh đề 2 {#evt-iii-s3-prop-2 .statement}

— Cho E và F là hai không gian lồi địa phương và cho $ \mathfrak{S} $ là một tập hợp các tập con bị chặn của E.

1) Tôpô $ \mathfrak{S} $ trên $ \mathcal{L}(E; F) $ trùng với tôpô $ \tilde{\mathfrak{S}} $, trong đó $ \tilde{\mathfrak{S}} $ ký hiệu bornology thích nghi nhỏ nhất (III, p. 3) trên E chứa $ \mathfrak{S} $.

2) Giả sử rằng $ \{0\} $ không trù mật trong F và cho $ \mathfrak{S}' $ là một tập hợp khác gồm các tập con bị chặn của E. Khi đó tôpô $ \mathfrak{S}' $ thô hơn tôpô $ \mathfrak{S} $ khi và chỉ khi $ \mathfrak{S}' \subset \tilde{\mathfrak{S}} $.

Cho $ u \in \mathcal{L}(E; F) $, $ M \in \mathfrak{S} $ và cho $ p $ là một nửa chuẩn liên tục trên F. Vì $ p \circ u $ là một nửa chuẩn liên tục trên E, điều này tương đương với việc nói rằng $ p \circ u $ bị chặn trên bởi 1 trên M hoặc trên bao lồi cân bằng đóng $ \tilde{M} $ của M; nói cách khác, ta có $ p_M = p_{\tilde{M}} $. Hơn nữa, hiển nhiên rằng ta có $ p_{\lambda M} = \lambda p_M $ với mọi $ \lambda > 0 $ và $ p_{M \cup M'} = \sup(p_M, p_{M'}) $, từ đó suy ra mệnh đề đầu tiên, vì $ \tilde{\mathfrak{S}} $ có tập hợp các vị tự của các bao lồi cân bằng đóng của các hợp hữu hạn của các tập hợp thuộc $ \mathfrak{S} $ làm cơ sở.

Bây giờ chứng minh mệnh đề thứ hai: trước hết, nếu F là trường cơ sở, thì từ định nghĩa suy ra rằng tôpô $ \tilde{\mathfrak{S}} $ trên $ E' = \mathcal{L}(E; F) $ có hệ cơ sở các lân cận của 0 là tập hợp các đối cực của các tập hợp thuộc $ \tilde{\mathfrak{S}} $. Cho A là một tập con bị chặn của E, mà đối cực $ A^\circ $ là một lân cận của 0 đối với tôpô $ \tilde{\mathfrak{S}} $; khi đó tồn tại một tập hợp lồi cân bằng đóng $ B \in \tilde{\mathfrak{S}} $ sao cho $ A^\circ \supset B^\circ $, và do đó $ A \subset B^{\circ \circ} $; nhưng theo hệ quả 3 của II, p. 45, ta có $ B^{\circ \circ} = B $, và vì vậy $ A \subset B $ và $ A \in \tilde{\mathfrak{S}} $. Do đó nếu $ \mathfrak{S}' $ là một tập hợp các tập con bị chặn của E, thì tôpô $ \mathfrak{S}' $ thô hơn tôpô $ \mathfrak{S} $ trên $ E' $ khi và chỉ khi $ \mathfrak{S}' \subset \tilde{\mathfrak{S}} $. Trường hợp tổng quát suy ra ngay lập tức, vì nếu $ y \in F $ không thuộc bao đóng của 0, ta có thể kiểm tra rằng ánh xạ làm cho $ f \in E' $ tương ứng với ánh xạ $ x \mapsto f(x)\ y $ là một đẳng cấu của các không gian lồi địa phương $ E'_\mathfrak{S} $ lên ảnh của nó trong $ \mathcal{L}_{\tilde{\mathfrak{S}}}(E; F) $.

### 2. Điều kiện để $ \mathcal{L}_\mathfrak{S}(E; F) $ là Hausdorff

#### Mệnh đề 3 {#evt-iii-s3-prop-3 .statement}

— Cho E và F là hai không gian lồi địa phương, giả sử F là Hausdorff, và cho $ \mathfrak{S} $ là một họ các tập con bị chặn của E. Nếu hợp A của các tập hợp thuộc $ \mathfrak{S} $ là toàn phần trong E, thì không gian $ \mathcal{L}_\mathfrak{S}(E; F) $ là Hausdorff.

Cho $ u_0 $ là một phần tử khác không của $ \mathcal{L}(E; F) $; vì $ u_0 $ liên tục và A là toàn phần trong E, tồn tại một $ x_0 $ trong A sao cho $ u_0(x_0) \neq 0 $. Vì F là Hausdorff, tồn tại một lân cận V của 0 trong F sao cho $ u_0(x_0) \notin V $. Cho $ M \in \mathfrak{S} $ sao cho $ x_0 \in M $. Khi đó tập hợp U của mọi $ u \in \mathcal{L}(E; F) $ sao cho $ u(M) \subset V $ là một lân cận của 0 trong $ \mathcal{L}(E; F) $, và ta có $ u_0 \notin U $, do đó $ \mathcal{L}(E; F) $ là Hausdorff.

Đặc biệt, các tôpô sau đây trên $ \mathcal{L}(E; F) $ là Hausdorff bất cứ khi nào F là Hausdorff: hội tụ đơn giản, hội tụ compact, hội tụ tiền compact hoặc lồi compact, và hội tụ bị chặn.

### 3. Các quan hệ giữa $ \mathcal{L}(E; F) $ và $ \mathcal{L}(\hat{E}; F) $

Cho E và F là hai không gian lồi địa phương Hausdorff, và giả sử F đầy đủ; gọi $ \hat{E} $ là sự hoàn thành của E. Vì mọi ánh xạ tuyến tính liên tục $ u $ từ E vào F đều mở rộng duy nhất thành một ánh xạ tuyến tính liên tục $ \bar{u} $ từ $ \hat{E} $ vào F, ta có thể đồng nhất các không gian $ \mathcal{L}(E; F) $ và $ \mathcal{L}(\hat{E}; F) $ bởi ánh xạ $ u \mapsto \bar{u} $. Ngoài ra, cho $ \mathfrak{S} $ là một họ các tập con bị chặn của E; tôpô $ \mathfrak{S} $ trên $ \mathcal{L}(E; F) $ trùng với tôpô $ \mathfrak{S} $ trên $ \mathcal{L}(\hat{E}; F) $ và cũng trùng với tôpô $ \hat{\mathfrak{S}} $, trong đó $ \hat{\mathfrak{S}} $ chỉ họ các bao đóng trong $ \hat{E} $ của các tập thuộc $ \mathfrak{S} $.

Ví dụ, nếu E là *chuẩn*, tôpô hội tụ bị chặn trên $ \mathcal{L}(E; F) $ đồng nhất với tôpô hội tụ bị chặn trên $ \mathcal{L}(\hat{E}; F) $: vì mọi tập con bị chặn của $ \hat{E} $ đều được chứa trong bao đóng của một tập con bị chặn của E. Vì quả cầu đơn vị của $ \hat{E} $ là bao đóng của quả cầu đơn vị của E, suy ra từ công thức (3) (III, p. 14) rằng nếu F là một không gian Banach, ánh xạ $ u \mapsto \bar{u} $ là một đẳng cự từ $ \mathcal{L}(E; F) $ lên $ \mathcal{L}(\hat{E}; F) $.

Ta nhận xét rằng nếu E không phải là một không gian chuẩn, thì có thể tồn tại các tập con bị chặn của $ \hat{E} $ không được chứa trong bao đóng của bất kỳ tập con bị chặn nào của E (ví dụ, nếu E là đối ngẫu yếu của một không gian Banach vô hạn chiều); tuy nhiên, điều này đúng nếu E mêtric hóa được và thỏa mãn tiên đề đếm được thứ nhất (III, p. 39, exerc. 16).

### 4. Các tập con đẳng liên tục của $ \mathcal{L}(E; F) $

Cho E và F là hai không gian lồi địa phương. Đối với một tập con H của $ \mathcal{L}(E; F) $ là đẳng liên tục thì điều kiện cần và đủ là nó đẳng liên tục tại điểm 0 trong E (I, p. 9, prop. 6); điều này kéo theo rằng với mọi lân cận V của 0 trong F, tập $ \bigcap_{u \in H} u^{-1}(V) $ là một lân cận của 0 trong E; hoặc rằng với mọi nửa chuẩn liên tục $ p $ trên F, hàm $ \sup_{u \in H} (p \circ u) $ là một nửa chuẩn liên tục trên E. Hơn nữa (I, p. 5), H là đẳng liên tục đều. Ta chú ý rằng bao lồi cân bằng của một tập con đẳng liên tục là đẳng liên tục, vì nếu $ p $ là một nửa chuẩn liên tục trên F và $ \tilde{H} $ là bao lồi cân bằng của H, ta có, đối với các $ u_i $ trong H, bất đẳng thức $ p \circ (\sum_i \lambda_i u_i) \leq \sum_i |\lambda_i| \cdot (p \circ u_i) $, do đó $ \sup_{u \in H} (p \circ u) = \sup_{u \in \tilde{H}} (p \circ u) $.

Do đó, họ các tập con đẳng liên tục là một bornology lồi trên $ \mathcal{L}(E; F) $ (III, p. 2, def. 2).

#### Mệnh đề 4 {#evt-iii-s3-prop-4 .statement}

*Cho E, F là hai không gian lồi địa phương, và F là Hausdorff. Gán cho không gian $ F^E $ của tất cả các ánh xạ từ E vào F tôpô hội tụ đơn giản. Khi đó*

(i) *Tập các ánh xạ tuyến tính từ E vào F là đóng trong $ F^E $.*

(ii) *Nếu H là một tập con đẳng liên tục của $ \mathcal{L}(E; F) $, bao đóng $ \overline{H} $ của H trong $ F^E $ được chứa trong $ \mathcal{L}(E; F) $ và là đẳng liên tục.*

Ta biết rằng $ \overline{H} $ là đẳng liên tục (GT, X, § 2, No. 3, prop. 6). Còn lại cần chứng minh mệnh đề (i). Cho x, y thuộc E và $ \lambda, \mu $ thuộc K, và gọi $ A(x, y, \lambda, \mu) $ là tập tất cả các $ u \in F^E $ sao cho

$$
u(\lambda x + \mu y) - \lambda u(x) - \mu u(y) = 0 .
$$

Tập này là đóng trong $ F^E $ vì ánh xạ $ u \mapsto u(x) $ từ $ F^E $ vào F là liên tục với mọi $ x \in E $ và vì F là Hausdorff. Nhưng tập các ánh xạ tuyến tính từ E vào F bằng

$$
\bigcap_{x,y,\lambda,\mu} A(x, y, \lambda, \mu) .
$$

Do đó tập này là đóng trong $ F^E $.

#### Hệ quả 1 {#evt-iii-s3-prop-4-cor-1 .statement}

— *Đối với một tập con đẳng liên tục H của $ \mathcal{L}(E; F) $ để là tương đối compact trong $ \mathcal{L}_s(E; F) $, điều kiện cần và đủ là với mọi $ x \in E $, tập $ H(x) $ gồm tất cả các $ u(x) $ khi $ u $ chạy qua H, là tương đối compact trong F.*

Thực vậy, điều kiện này là cần và đủ để $ \overline{H} $ compact trong $ F^E $ (GT, I, § 9, No. 5, cor.).

#### Hệ quả 2 {#evt-iii-s3-prop-4-cor-2 .statement}

— *Mọi tập hợp con liên tục đều của đối ngẫu $ E' $ của E là tương đối compact đối với tôpô yếu $ \sigma(E', E) $ trên $ E' $* (III, p. 14, Ví dụ 4).

Thật vậy, nếu H là một tập hợp con liên tục đều của $ E' $, $ \sup_{u \in H} |u| $ là một bán chuẩn liên tục trên E; đặc biệt, với mọi $ x \in E $, tập hợp $ H(x) $ là bị chặn, do đó tương đối compact trong trường các vô hướng.

#### Hệ quả 3 {#evt-iii-s3-prop-4-cor-3 .statement}

— *Trong đối ngẫu mạnh $ E'_b $ của một không gian nửa chuẩn E, mọi quả cầu đóng đều compact đối với tôpô yếu $ \sigma(E', E) $.*

Quả cầu này cũng đóng đối với $ \sigma(E', E) $.

#### Mệnh đề 5 {#evt-iii-s3-prop-5 .statement}

— *Cho E và F là hai không gian lồi địa phương và cho T là một tập con toàn phần của E. Các cấu trúc đều sau đây trùng nhau trên mọi tập hợp con liên tục đều H của $ \mathcal{L}(E; F) $:*

1) *cấu trúc đều của sự hội tụ đơn giản trong T;*
2) *cấu trúc đều của sự hội tụ đơn giản trong E;*
3) *cấu trúc đều của sự hội tụ trong các tập con tiền compact của E.*

Ta nhắc lại (III, p. 15, prop. 2) rằng tôpô $ \mathfrak{S} $ trên $ \mathcal{L}(E; F) $ trùng với tôpô $ \tilde{\mathfrak{S}} $, trong đó $ \tilde{\mathfrak{S}} $ là bornologie nhỏ nhất thích nghi với E và chứa $ \mathfrak{S} $.

Trong mệnh đề của prop. 5, do đó ta có thể thay thế từ « toàn phần » bằng « trù mật khắp nơi ». Khi đó mệnh đề suy ra từ các tính chất tổng quát của các tập hợp con liên tục đều (GT, X, § 2, No. 4, th. 1).

#### Ví dụ {#evt-iii-s3-n4-exa-1 .statement}

— *1) Cho $ \mu $ là độ đo Lebesgue trên $ \mathbf{R} $, và cho E là không gian nửa chuẩn $ \mathcal{L}^p(\mu) $ ($ 1 \leq p < \infty $) (INT, IV). Với mọi hàm số $ f $ và mọi số thực $ h $, cho $ f_h $ là hàm $ x \mapsto f(x - h) $. Rõ ràng ánh xạ $ f \mapsto f_h $ xác định một đẳng cấu đẳng cự tuyến tính từ E lên chính nó. Nếu $ f $ liên tục và có giá compact, thì $ f_h $ hội tụ đến $ f $ đều, do đó cũng hội tụ theo trung bình cấp $ p $, khi $ h $ tiến đến 0. Vì tập hợp $ \mathscr{K}(\mathbf{R}) $ gồm tất cả các hàm liên tục có giá compact là trù mật trong E, và tập hợp các đẳng cấu đẳng cự tuyến tính của E là liên tục đều, nên suy ra từ prop. 5 rằng với mọi $ f \in E $, $ f_h $ hội tụ theo trung bình cấp $ p $ đến $ f $ khi $ h $ tiến đến 0.

Với $ p = 1 $, xét biến đổi Fourier, biến đổi này gán cho mỗi $ f \in \mathcal{L}^1(\mu) $ hàm $ \hat{f} $ trên $ \mathbf{R} $ được xác định bởi

$$
\hat{f}(y) = \int e^{-2i\pi xy} f(x) \, d\mu(x) .
$$

Tập hợp các dạng tuyến tính $ f \mapsto \hat{f}(y) $ là một tập hợp con liên tục đều của đối ngẫu của $ \mathcal{L}^1(\mu) $.

Mặt khác, ta biết rằng tập hợp T gồm tất cả các hàm đặc trưng của các khoảng đóng bị chặn là một tập con toàn phần của $ \mathcal{L}^1(\mu) $; và ta dễ dàng kiểm tra rằng với mọi $ f \in T $, biến đổi Fourier $ \hat{f} $ là một hàm liên tục tiến đến không tại vô cực. Ta suy ra rằng điều này đúng với mọi $ f \in \mathcal{L}^1(\mu) $ ("định lý Riemann-Lebesgue").

Quan hệ $ \sup_{y \in \mathbf{R}} |\hat{f}(y)| \leq \|f\|_1 $ chỉ ra rằng ánh xạ $ f \mapsto \hat{f} $ là một ánh xạ liên tục từ $ \mathcal{L}^1(\mu) $ vào không gian $ \mathcal{B}(\mathbf{R}) $ gồm tất cả các hàm bị chặn trên $ \mathbf{R} $, với cấu trúc hội tụ đều. Vì $ \hat{f} $ liên tục với mọi $ f \in T $, nên suy ra rằng $ \hat{f} $ liên tục với mọi $ f \in L^1(\mu) $. Việc $ \hat{f} $ tiến đến không tại vô cực suy ra từ việc không gian con $ C_0(\mathbf{R}) $ gồm tất cả các hàm liên tục tiến đến không tại vô cực là đóng trong $ \mathcal{B}(\mathbf{R}) $.

2) Cho E là không gian của tất cả các hàm số liên tục có giá trị số trên $ \mathbf{R} $ được trang bị tôpô hội tụ compact. Cho K là một tập compact của $ \mathbf{R} $ và cho $ (\mu_n) $ là một dãy các độ đo trên $ \mathbf{R} $ có giá đỡ nằm trong K. Giả sử $ \|\mu_n\| \leq 1 $ với mọi n. Tập hợp các $ \mu_n $ khi đó là một tập con liên tục đều của E'. Do đó, nếu với mọi hàm $ f \in E $, ta có $ \lim_{n \to \infty} \mu_n(f) = 0 $, thì dãy các hàm $ x \mapsto \int e^{itx} d\mu_n(t) $ hội tụ về 0, đều trên mọi tập con compact của $ \mathbf{R} $ (vì tập các hàm $ t \mapsto e^{itx} $, khi x chạy trên một tập compact của $ \mathbf{R} $, là compact trong E). \*

#### Hệ quả {#evt-iii-s3-n4-cor-1 .statement}

— *Giả sử F là Hausdorff. Cho H là một tập con liên tục đều của $ \mathcal{L}(E; F) $. Nếu một lọc $ \Phi $ trên H hội tụ đơn giản đến một ánh xạ $ u_0 $ từ E vào F, thì $ u_0 $ là một ánh xạ tuyến tính liên tục từ E vào F, và $ \Phi $ hội tụ đều đến $ u_0 $ trên mọi tập con tiềncompact của E.*

Khẳng định thứ nhất suy ra từ mệnh đề 4 (III, p. 16) và khẳng định thứ hai từ mệnh đề 5 (III, p. 17).

#### Mệnh đề 6 {#evt-iii-s3-prop-6 .statement}

— *Cho H là một tập con liên tục đều của $ \mathcal{L}(E; F) $. Nếu F là khả mêtric và nếu tồn tại một tập toàn phần đếm được trong E, thì cấu trúc đều trên H của hội tụ đơn giản trong E là khả mêtric. Nếu ngoài ra tồn tại một tập toàn phần đếm được trong F, thì tồn tại một tập trù mật khắp nơi đếm được trong H (đối với tôpô hội tụ đều trên các tập con compact của E).

Cho $ (a_n) $ là một dãy toàn phần trong E. Khi đó ánh xạ $ u \mapsto (u(a_n)) $ là một đẳng cấu từ $ \mathcal{L}(E; F) $, trong đó $ \mathcal{L}(E; F) $ có cấu trúc đều của hội tụ đơn giản trên tập hợp các $ a_n $, lên một không gian con đều của $ F^\mathbf{N} $. Nếu F là khả mêtric (tương ứng, khả mêtric và thỏa mãn tiên đề đếm được thứ nhất) thì điều này cũng đúng đối với $ F^\mathbf{N} $ (GT, IX, § 2, No. 4, hệ quả 2 và § 2, No. 8, hệ quả), và mệnh đề suy ra từ mệnh đề 5 (III, p. 17).*

#### Hệ quả 1 {#evt-iii-s3-prop-6-cor-1 .statement}

— *Cho E là một không gian lồi địa phương khả mêtric, và F là một không gian định chuẩn. Giả sử rằng E và F đều thỏa mãn tiên đề đếm được thứ nhất. Khi đó $ \mathcal{L}(E; F) $ là hợp của một họ đếm được các tập con liên tục đều và tồn tại một tập đếm được trong $ \mathcal{L}(E; F) $ trù mật đối với tôpô hội tụ đều trên các tập con tiềncompact của E.

Cho B là quả cầu đơn vị của F và $ (V_n) $ là một hệ cơ bản đếm được các lân cận của 0 trong E. Với mọi số nguyên n, tập $ H_n $ gồm tất cả các $ u \in \mathcal{L}(E; F) $ sao cho $ u(V_n) \subset B $ là liên tục đều và $ \mathcal{L}(E; F) $ là hợp của các $ H_n $. Hệ quả suy ra từ mệnh đề 6.*

#### Hệ quả 2 {#evt-iii-s3-prop-6-cor-2 .statement}

— *Mọi quả cầu đóng trong đối ngẫu E' của một không gian định chuẩn thỏa mãn tiên đề đếm được thứ nhất, là một không gian compact khả mêtric đối với tôpô yếu σ(E', E), và đối với tôpô này tồn tại một tập con trù mật đếm được trong E'*.

Điều này suy ra từ mệnh đề 6 và từ III, p. 17, hệ quả 3.

### 5. Các tập con liên tục đều của $ E' $

Trong tiết này, E ký hiệu một không gian lồi địa phương và $ E' $ là đối ngẫu của nó. Mỗi khi ta nói đến cực $ M^\circ $ của một tập M trong E (tương ứng, $ E' $), ta sẽ luôn luôn hiểu, trừ khi có quy định khác, là cực của M đối với đối ngẫu giữa E và $ E' $. Nhắc lại rằng nếu V là một lân cận lồi cân bằng đóng của 0 trong E, ta có $ V^{\circ\circ} = V $ (II, p. 45, hệ quả 3).

#### Mệnh đề 7 {#evt-iii-s3-prop-7 .statement}

— *Cho M là một tập con của $ E' $. Các điều kiện sau là tương đương :*

(i) $ M $ *là liên tục đều* ;
(ii) $ M $ *được chứa trong cực của một lân cận của 0 trong E* ;
(iii) *cực của M là một lân cận của 0 trong E*.

Nếu M là liên tục đều, tồn tại một lân cận lồi cân bằng V của 0 sao cho $ |u(x)| \leq 1 $ với mọi $ x \in V $ và mọi $ u \in M $; khi đó ta có $ M \subset V^\circ $ và (i) kéo theo (ii). Với cùng các ký hiệu đó, nếu $ M \subset V^\circ $ thì $ V \subset V^{\circ\circ} \subset M^\circ $ và (ii) kéo theo (iii). Cuối cùng, nếu $ M^\circ $ chứa một lân cận lồi cân bằng V của 0, thì $ M \subset M^{\circ\circ} \subset V^\circ $ và các quan hệ $ x \in \varepsilon V,\ u \in M $ kéo theo $ |u(x)| \leq \varepsilon $ với mọi $ \varepsilon > 0 $, điều này chứng minh rằng (iii) kéo theo (i).

Ta nhận xét rằng mọi $ x \in E $ xác định một ánh xạ $ j(x): u \mapsto u(x) $ từ $ E' $ vào K. Do đó ta có thể nói về tôpô $ \mathcal{S} $ trên E, trong đó $ \mathcal{S} $ là một họ các tập con của $ E' $: đây là ảnh ngược theo $ j $ của tôpô $ \mathcal{S} $ trên $ K^{E'} $. Ta kiểm tra ngay lập tức rằng nếu $ \mathcal{S} $ là một bao sinh lồi trên $ E' $, thì các cực của các tập hợp của $ \mathcal{S} $ tạo thành một hệ cơ bản các lân cận của 0 đối với tôpô $ \mathcal{S} $ trên E. Điều này đúng, đặc biệt, khi $ \mathcal{S} $ là họ các tập con liên tục đều của $ E' $ và mệnh đề 7 kéo theo :

#### Hệ quả 1 {#evt-iii-s3-prop-7-cor-1 .statement}

— *Tôpô của E đồng nhất với tôpô hội tụ đều trên các tập con liên tục đều của $ E' $*.

Tổng quát hơn, cho F là một không gian lồi địa phương; mọi $ u \in \mathcal{L}(E; F) $ xác định một ánh xạ $ j(u):(x, f) \mapsto f(u(x)) $ từ $ E \times F' $ vào K (*nghĩa là* vào $ \mathbf{R} $ hoặc $ \mathbf{C} $). Điều này cho phép ta định nghĩa, trên không gian $ \mathcal{L}(E; F) $, tôpô hội tụ đều trên một tập hợp các tập con của $ E \times F' $. Đặc biệt :

#### Hệ quả 2 {#evt-iii-s3-prop-7-cor-2 .statement}

— *Cho $ \mathcal{S} $ là một họ các tập con bị chặn của E. Tôpô $ \mathcal{S} $ trên $ \mathcal{L}(E; F) $ là tôpô hội tụ đều trên các tập hợp có dạng $ A \times B \subset E \times F' $, trong đó A thuộc $ \mathcal{S} $, và B thuộc họ các tập con liên tục đều của $ F' $*.

Với mọi $ u \in \mathcal{L}(E; F) $, mọi $ A \in \mathcal{S} $ và mọi lân cận lồi cân bằng đóng V của 0 trong F, quan hệ $ u(A) \subset V $ là tương đương với « $ j(u)(A \times V^\circ) $ được chứa trong quả cầu đơn vị của K ».

#### Mệnh đề 8 {#evt-iii-s3-prop-8 .statement}

— *Cho H là một họ các ánh xạ tuyến tính từ E vào một không gian lồi địa phương F. Để H là liên tục đều, điều kiện cần và đủ là với mọi tập con liên tục đều X trong đối ngẫu F' của F, tập hợp các dạng tuyến tính f \circ u, với f \in X và u \in H, là liên tục đều.

Điều kiện này rõ ràng là cần thiết. Giả sử nó được thỏa mãn, và cho V là một lân cận lồi cân bằng đóng của 0 trong F. Vì V^\circ là liên tục đều, tồn tại một lân cận W của 0 trong E sao cho |f(u(x))| \leq 1 với mọi x \in W, u \in H và f \in V^\circ; nói cách khác, u(W) \subset V^{\circ\circ} = V với mọi u \in H, do đó H là liên tục đều.

### 6. Sự hoàn thành của một không gian lồi địa phương

#### Định lý 1 (Grothendieck) {#evt-iii-s3-thm-1 .statement}

— Cho E là một không gian lồi địa phương, và cho \mathcal{S} là một bao sinh thích nghi và phủ trên E. Cho F \subset E^* là không gian của các dạng tuyến tính trên E mà hạn chế của chúng trên mỗi tập thuộc \mathcal{S} là liên tục. Nếu F được trang bị tôpô \mathcal{S}, thì đơn ánh chính tắc từ E'_\mathcal{S} vào F mở rộng thành một đẳng cấu từ sự hoàn thành \hat{E}'_\mathcal{S} của E'_\mathcal{S} lên F.

Vì mọi giới hạn đơn của các dạng tuyến tính trên E là một dạng tuyến tính (III, p. 16, mệnh đề 4) và vì bao sinh \mathcal{S} trên E là phủ, nên từ GT, X, § 1, No. 6, hệ quả 2 suy ra rằng không gian F với tôpô \mathcal{S} là Hausdorff và đầy đủ. Hiển nhiên rằng E'_\mathcal{S} là một không gian con vectơ tôpô của F; do đó chỉ cần chứng minh rằng E'_\mathcal{S} là trù mật khắp nơi trong F. Điều này suy ra từ bổ đề sau:

#### Bổ đề 1 {#evt-iii-s3-lem-1 .statement}

Cho A là một tập con lồi cân bằng đóng của E và cho u là một dạng tuyến tính trên E mà hạn chế của nó trên A là liên tục. Khi đó với mọi $ \varepsilon > 0 $, tồn tại một $ x' \in E' $ sao cho

$$ |u(x) - \langle x, x' \rangle| \leq \varepsilon \quad \text{với mọi} \quad x \in A . $$

Cho $ \varepsilon > 0 $. Tồn tại một lân cận lồi cân bằng đóng U của 0 trong E sao cho |u(x)| \leq \varepsilon với mọi x \in U \cap A. Ta biết rằng cực U^\circ của U trong E* được chứa trong E' và là compact đối với tôpô \sigma(E^*, E) (III, p. 17, hệ quả 2). Vì cực A^\circ của A trong E* là đóng đối với \sigma(E^*, E), nên suy ra A^\circ + U^\circ là một tập con lồi đóng của E* (GT, III, § 4, No. 1, hệ quả 1).

Cho C là một tập con lồi cân bằng đóng của E. Khi đó C là đóng đối với \sigma(E, E') (II, p. 45, hệ quả 3), do đó cũng đóng đối với \sigma(E, E^*), và do đó, ta có C = C^{\circ\circ} (đối với đối ngẫu giữa E và E*). Kết quả là, ta có

$$ A \cap U = A^{\circ\circ} \cap U^{\circ\circ} = (A^\circ \cup U^\circ)^\circ \supset (A^\circ + U^\circ)^\circ $$

từ đó, ta được

$$ (A \cap U)^\circ \subset (A^\circ + U^\circ)^{\circ\circ} = A^\circ + U^\circ . $$

Vì dạng tuyến tính $ \varepsilon^{-1}u $ thuộc (A \cap U)^\circ, tồn tại v \in A^\circ và w \in U^\circ sao cho u = \varepsilon(v + w). Do đó x' = \varepsilon w thuộc E' và u - x' = \varepsilon v bị chặn trên theo giá trị tuyệt đối bởi \varepsilon trên A; do đó bổ đề được chứng minh.

Bây giờ cho E là một không gian Hausdorff lồi địa phương và \hat{E} là sự hoàn thành của nó. Mọi dạng tuyến tính liên tục f trên E mở rộng đến \hat{E} bằng tính liên tục; do đó ta có (\hat{E})' = E'

(III, p. 16) và mọi phần tử của $ \hat{E} $ xác định một dạng tuyến tính trên $ E' $; nghĩa là, một phần tử của đối ngẫu đại số $ {E'}^* $ của $ E' $. Ngoài ra, đối ngẫu giữa $ E $ (tương ứng $ \hat{E} $) và $ E' $ là phân ly (II, p. 24, hệ quả 1). Do đó $ E $ và $ \hat{E} $ có thể được đồng nhất với các không gian con vectơ của $ {E'}^* $.

#### Định lý 2 {#evt-iii-s3-thm-2 .statement}

*Cho $ E $ là một không gian Hausdorff lồi địa phương và $ \hat{E} $ là sự hoàn thành của nó; ta đồng nhất $ E $ và $ \hat{E} $ với các không gian con vectơ của $ {E'}^* $. Khi đó để một phần tử $ f \in {E'}^* $ thuộc $ \hat{E} $, điều kiện cần và đủ là hạn chế của $ f $ trên mọi tập con liên tục đều của $ E' $ là liên tục đối với tôpô $ \sigma(E', E) $.*

Không gian $ E $ có thể được đồng nhất với đối ngẫu tôpô của $ E' $ khi $ E' $ được trang bị tôpô $ \sigma(E', E) $ (II, p. 43, Mệnh đề 3); mặt khác, nếu $ \mathcal{S} $ là tập hợp các tập con liên tục đều của $ E' $, tôpô đã cho trên $ E $ là tôpô $ \mathcal{S} $ (III, p. 19, Hệ quả 1). Khi đó, từ III, p. 13, Mệnh đề 1, suy ra các tập hợp của $ \mathcal{S} $ bị chặn đối với $ \sigma(E', E) $ (*xem* về sau, III, p. 22, Mệnh đề 9); nói cách khác, $ \mathcal{S} $ là một bornology thích nghi và phủ được đối với tôpô $ \sigma(E', E) $. Định lý 2 khi đó là một hệ quả của Định lý 1 nếu ta thay $ E $ bởi $ E' $ và $ E'_\mathcal{S} $ bởi $ E $.

#### Hệ quả 1 (Banach) {#evt-iii-s3-thm-2-cor-1 .statement}

— *Cho $ E $ là một không gian lồi địa phương Hausdorff và đầy đủ. Để một dạng tuyến tính trên $ E' $ liên tục đối với tôpô yếu $ \sigma(E', E) $ (tức là xuất phát từ một phần tử của $ E $), thì chỉ cần hạn chế của nó trên mọi tập con liên tục đều của $ E' $ liên tục đối với $ \sigma(E', E) $.*

#### Nhận xét {#evt-iii-s3-n6-rem-1 .statement}

— Giả sử thêm rằng tồn tại một tập toàn phần đếm được trong $ E $; khi đó mọi tập con liên tục đều của $ E' $ đều mêtric hóa được đối với tôpô $ \sigma(E', E) $ (III, p. 18, Mệnh đề 6); do đó, để kiểm tra rằng một dạng tuyến tính $ u $ trên $ E' $ là liên tục yếu, chỉ cần kiểm tra rằng với mọi *dãy liên tục đều* $ (x'_n) $ trong $ E' $ hội tụ về 0 đối với $ \sigma(E', E) $, ta có $ \lim_{n \to \infty} u(x'_n) = 0 $.

#### Hệ quả 2 {#evt-iii-s3-thm-2-cor-2 .statement}

*Cho $ (E_i)_{i \in I} $ là một họ các không gian lồi địa phương Hausdorff và cho $ E $ là tổng trực tiếp tôpô của chúng. Khi đó ánh xạ chính tắc từ tổng trực tiếp của các $ \hat{E}_i $ vào $ \hat{E} $ là một đẳng cấu. Đặc biệt, $ E $ đầy đủ khi và chỉ khi mọi $ E_i $ đều đầy đủ.*

Ta biết rằng đối ngẫu của $ E $ có thể được đồng nhất với tích của các đối ngẫu của các $ E_i $ (II, p. 30, công thức (1)). Cho $ u \in \hat{E} $, và cho $ u_i \in E_{i'}^* $ là hạn chế của $ u $ (được xem như một phần tử của $ {E'}^* $) trên $ E_i' \subset E' $. Ngay lập tức thấy rằng chỉ cần chứng minh $ u_i = 0 $ ngoại trừ một số hữu hạn chỉ số $ i \in I $. Giả sử ngược lại rằng tồn tại một dãy $ (i_n)_{n \in \mathbf{N}} $ gồm các chỉ số phân biệt sao cho $ u_{i_n} \neq 0 $. Khi đó tồn tại $ x_{i_n} \in E_{i_n}' $ sao cho $ u_{i_n}(x_{i_n}) = n $. Tập hợp $ H $ gồm tất cả các $ x_{i_n} $ là liên tục đều trong $ E' $ và hạn chế của $ u $ trên $ H $ không bị chặn, điều này là không thể.

### 7. Bornology $ \mathcal{S} $ trên $ \mathcal{L}(E; F) $

Cho $ E $ và $ F $ là hai không gian lồi địa phương và $ \mathcal{S} $ là một họ các tập con bị chặn của $ E $. Nói rằng một tập con $ H $ của $ \mathcal{L}(E; F) $ bị chặn đối với tôpô $ \mathcal{S} $ có nghĩa là *với* mọi $ M \in \mathcal{S} $, mọi lân cận $ V $ của 0 trong F đều hấp thụ tập $ H(M) = \bigcup_{u \in H} u(M) $; điều này cũng chính là nói rằng với mọi $ M \in \mathcal{S} $, tập $ H(M) $ bị chặn trong F. Tương đương, điều này có nghĩa là với mọi lân cận $ V $ của 0 trong F, tập $ \bigcap_{u \in H} u^{-1}(V) $ hấp thụ mọi tập con $ M $ của $ \mathcal{S} $.

#### Mệnh đề 9 {#evt-iii-s3-prop-9 .statement}

*Cho E và F là hai không gian lồi địa phương và $ \mathcal{S} $ là một họ các tập con bị chặn của E. Khi đó mọi tập con liên tục đều của $ \mathcal{L}(E; F) $ đều bị chặn đối với tôpô $ \mathcal{S} $.*

Thật vậy, nếu $ H $ là một tập con liên tục đều của $ \mathcal{L}(E; F) $ và $ V $ là một lân cận của 0 trong F, thì tập $ \bigcap_{u \in H} u^{-1}(V) $ là một lân cận của 0 trong E, do đó hấp thụ mọi tập con bị chặn của E.

Một tập con của $ \mathcal{L}(E; F) $ bị chặn đối với một tôpô $ \mathcal{S} $ không nhất thiết liên tục đều, ngay cả khi $ \mathcal{S} $ là phủ và $ \mathcal{S} $ là bornology chính tắc trên E (IV, p. 50, exerc. 17). Trong đoạn sau, ta sẽ nghiên cứu, dưới tên gọi các không gian *barrelled*, các không gian E sao cho mọi tập con bị chặn đơn giản của $ \mathcal{L}(E; F) $ đều liên tục đều. Hiện tại, chú ý kết quả sau:

#### Mệnh đề 10 {#evt-iii-s3-prop-10 .statement}

*Cho E là một không gian bornological (đặc biệt, một không gian lồi địa phương khả metric) và F là một không gian lồi địa phương. Mọi tập con H của $ \mathcal{L}(E; F) $ bị chặn đối với tôpô của hội tụ bị chặn đều liên tục đều.*

Với mọi lân cận lồi cân bằng $ V $ của 0 trong F, tập $ \bigcap_{u \in H} u^{-1}(V) $ hấp thụ mọi tập con bị chặn của E, do đó là một lân cận của 0 trong E; điều này chứng minh rằng H liên tục đều.

### 8. Các tập con đầy đủ của $ \mathcal{L}_{\mathcal{S}}(E; F) $

#### Mệnh đề 11 {#evt-iii-s3-prop-11 .statement}

*Cho E và F là hai không gian lồi địa phương, $ \mathcal{S} $ là một phủ của E gồm các tập con bị chặn. Nếu F là Hausdorff và quasi-đầy đủ (III, p. 8), thì mọi tập con H liên tục đều của $ \mathcal{L}(E; F) $ đóng đối với tôpô $ \mathcal{S} $ đều là một không gian con đều đầy đủ của $ \mathcal{L}_{\mathcal{S}}(E; F) $.*

Vì H bị chặn trong $ \mathcal{L}_{\mathcal{S}}(E; F) $ (III, p. 22, prop. 9) và đóng trong $ F^E $ đối với tôpô $ \mathcal{S} $ (III, p. 16, prop. 4), điều này suy ra từ hệ quả 3 của GT, X, § 1, No. 5.

#### Nhận xét 1 {#evt-iii-s3-n8-rem-1 .statement}

— Cho M là một không gian con đều *đầy đủ* của $ \mathcal{L}_{\mathcal{S}}(E; F) $. Với mọi tập các tập con bị chặn $ \mathcal{S}' \supset \mathcal{S} $ của E, tôpô $ \mathcal{S}' $ mịn hơn tôpô $ \mathcal{S} $ trên $ \mathcal{L}(E; F) $; mặt khác, tồn tại một hệ cơ bản các lân cận của 0 đối với tôpô $ \mathcal{S}' $ đóng đối với tôpô hội tụ đơn giản (III, p. 13, *Nhận xét 2*), và *a fortiori* đối với tôpô $ \mathcal{S} $. Ta kết luận (GT, III, § 3, No. 5, cor. 1) rằng M là *đầy đủ* đối với tôpô $ \mathcal{S}' $.

#### Hệ quả {#evt-iii-s3-n8-cor-1 .statement}

*Cho E và F là hai không gian lồi địa phương, H là một tập con liên tục đều của $ \mathcal{L}(E; F) $. Nếu F là Hausdorff và quasi-đầy đủ và nếu một bộ lọc $ \Phi $ trên H hội tụ* đơn giản tại mọi điểm của một tập con toàn T của E, thì tồn tại một ánh xạ tuyến tính liên tục u từ E vào F sao cho $ \Phi $ hội tụ đều đến u trên mọi tập con tiền compact của E.

Thật vậy, theo mệnh đề 5 (III, p. 17) $ \Phi $ là một bộ lọc Cauchy đối với cấu trúc đều của hội tụ tiền compact trong E; theo mệnh đề 11, bao đóng $ \overline{H} $ của H trong $ \mathcal{L}_{pc}(E; F) $ là đầy đủ và do đó $ \Phi $ hội tụ đều trên mọi tập con tiền compact của E đến một ánh xạ $ u \in \overline{H} $.

#### Nhận xét 2 {#evt-iii-s3-n8-rem-2 .statement}

Cho $ (u_n) $ là một dãy các ánh xạ tuyến tính liên tục từ một không gian Banach E vào một không gian Banach F; có thể xảy ra là $ (u_n(x)) $ có giới hạn tại mọi điểm của một không gian vectơ T trù mật khắp nơi trong E, mà dãy $ (u_n) $ lại không bị chặn trong không gian định chuẩn $ \mathcal{L}(E; F) $. Ví dụ, lấy E là không gian tất cả các hàm số liên tục trên $ \mathbf{R} $, tiến về không khi ra vô cực, với chuẩn $ \|f\| = \sup_{x \in \mathbf{R}} |f(x)| $ và lấy T là không gian con gồm các hàm số liên tục có giá compact. Dãy các ánh xạ tuyến tính liên tục $ f \mapsto nf(n) $ từ E vào $ \mathbf{R} $ hội tụ về 0 với mọi $ f \in T $, nhưng không bị chặn trong $ \mathcal{L}_b(E; \mathbf{R}) $. Cùng ví dụ đó cho thấy rằng trong không gian $ \mathcal{L}(T; \mathbf{R}) $, một dãy $ (v_n) $ có thể hội tụ đơn giản và không bị chặn đối với tôpô hội tụ bị chặn.

Mặt khác, dãy các ánh xạ tuyến tính liên tục $ f \mapsto \sum_{k=1}^n f(k) $ là một dãy Cauchy trong $ \mathcal{L}(T; \mathbf{R}) $ đối với tôpô hội tụ đơn giản, nhưng không tiến tới một giới hạn trong $ \mathcal{L}(T; \mathbf{R}) $ đối với tôpô này.

#### Mệnh đề 12 {#evt-iii-s3-prop-12 .statement}

— *Cho E là một không gian lồi địa phương bornological, F là một không gian Hausdorff lồi địa phương đầy đủ và $ \mathfrak{S} $ là một họ các tập con bị chặn của E chứa ảnh của mọi dãy hội tụ về 0. Khi đó không gian $ \mathcal{L}_{\mathfrak{S}}(E; F) $ là đầy đủ.*

Cho $ \Phi $ là một lọc Cauchy trong $ \mathcal{L}_{\mathfrak{S}}(E; F) $. Khi đó $ \Phi $ là một lọc Cauchy đối với tôpô hội tụ đơn giản, do đó hội tụ trong $ F^E $; hơn nữa, giới hạn $ u $ của nó là một ánh xạ tuyến tính từ E vào F và $ \Phi $ hội tụ đều về $ u $ trên mọi tập hợp thuộc $ \mathfrak{S} $ (GT, X, § 1, No. 5, mệnh đề 5). Suy ra ảnh bởi $ u $ của một dãy hội tụ về không là một dãy hội tụ về không, do đó $ u $ là *liên tục*, vì E là bornological (III, p. 11, mệnh đề 1, (iii)).

#### Hệ quả 1 {#evt-iii-s3-prop-12-cor-1 .statement}

— *Đối đối ngẫu mạnh của một không gian bornological là đầy đủ.*

#### Hệ quả 2 {#evt-iii-s3-prop-12-cor-2 .statement}

— *Cho E là một không gian nửa định chuẩn, và F là một không gian Banach (resp. Fréchet). Không gian $ \mathcal{L}_b(E; F) $ là một không gian Banach (resp. Fréchet). Đặc biệt, đối ngẫu của một không gian nửa định chuẩn là một không gian Banach.*

### Bài tập {#evt-iii-s3-exercises}

Xem [các bài tập cho § 3](exercises/s3/).
