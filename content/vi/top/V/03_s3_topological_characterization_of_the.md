---
book: top
book_title: General Topology
chapter: V
chapter_title: One-parameter groups
section: 3
section_title: Topological characterization of the groups R and T
lang: vi
source: top-v-x
pdf_pages: 0023-0025, 0031-0034
extraction: ocr
statements: 5
exercises: 1
content_sha256: 940a7bb177aaf90e669db985726dcb5688de84d177f82f406b20f25d559d64ca
translated_from: content/en/top/V/03_s3_topological_characterization_of_the.md
source_content_sha256: e083ecd8e6a72be8ff4cd629267067888014277bb5a1f7b1682d08f2f015472c
translation_model: gpt-5-6-mini
translation_run: translate-vi-700a49f5
glossary_version: 34
glossary_terms_sha256: ca9d4bb86f5c1591f284e7ca45aa8f993bad8afebc8143a363a97c92228e748c
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 3. ĐẶC TRƯNG HÓA TÔPÔ CỦA CÁC NHÓM $\mathbf{R}$ VÀ $\mathbf{T}$

#### Định lý 1 {#top-v-s3-thm-1 .statement}

*Một nhóm tôpô* $G$ *trong đó tồn tại một lân cận của phần tử đơn vị đẳng cấu đồng phôi với một khoảng mở của* $\mathbf{R}$ *là địa phương đẳng cấu với* $\mathbf{R}$.

Ý nghĩa của định lý này là nó cho phép ta suy ra, từ một tính chất tôpô thuần túy của một nhóm $G$, một tính chất của *cấu trúc nhóm* của $G$.

Ở đây ta quan tâm đến một hiện tượng đặc thù của nhóm $\mathbf{R}$ và không có tương tự nào đối với các nhóm $\mathbf{R}^n$ khi $n > 1$ (xem Chương VIII, § 1, no. 4). Các nhóm địa phương đẳng cấu với $\mathbf{R}$ đôi khi được gọi là *các nhóm một tham số*.

Để chứng minh Định lý 1 ta sẽ rút gọn nó về Mệnh đề 2 của § 2. Theo giả thiết, có một đồng phôi $\varphi$ của một lân cận mở $U$ của phần tử đơn vị $e$ của $G$ lên một khoảng mở trong $\mathbf{R}$. Bằng ánh xạ ngược của ánh xạ $\varphi$ ta có thể chuyển sang $U$ cấu trúc thứ tự tuyến tính của khoảng $\varphi(U)$; tôpô của $U$ (cảm sinh bởi tôpô của $G$) khi đó có một cơ sở gồm tất cả các khoảng mở của $U$ (Chương

Ta chứng minh rằng, nếu x, y, z thuộc V, thì quan hệ x < y kéo theo xz < yz và zx < zy. Thật vậy, các hàm f_1(z) = φ(yz) − φ(xz) và f_2(z) = φ(zy) − φ(zx) liên tục trên V; chúng > 0 với z = e và không triệt tiêu trong V [chẳng hạn, nếu ta có φ(yz) = φ(xz), thì ta sẽ có yz = xz và do đó y = x]. Vì f_1(V) và f_2(V) liên thông (Chương I, § 11, no. 2, Mệnh đề 4) và do đó là các khoảng trong R (Chương IV, § 2, no. 5, Định lý 4), và vì mỗi khoảng này đều chứa một số > 0 và không chứa 0, chúng được chứa trong R^*_+ : nghĩa là ta có f_1(z) > 0 và f_2(z) > 0 với mọi z ∈ V.

Nếu x và y là hai phần tử của V sao cho x ≥ e và y ≥ e, thì đặc biệt ta có xy ≥ e. Gọi E là tập hợp (có thứ tự tuyến tính) các phần tử của U thỏa mãn ≥ e, và gọi I là tập hợp các phần tử của V thỏa mãn ≥ e; khi đó các tiên đề (GR_I), (GR_{II}), (GR_{IIIa}) và (GR_{IVa}) của § 2 được thỏa mãn (lấy ω là phần tử e, và luật hợp thành là luật của nhóm G). Điều này hiển nhiên đối với (GR_I), (GR_{II}) và (GR_{IVa}), từ những điều trên. Đối với (GR_{IIIa}), chỉ cần nhận xét rằng, nếu e < x < y (x ∈ V, y ∈ V), thì ta có x^{-1} ∈ V, do đó x^{-1} < e < x^{-1}y và x^{-1}y < y; do đó z = x^{-1}y thuộc I và ta có xz = y. Theo Mệnh đề 2 của § 2, tồn tại vì thế một ánh xạ tăng ngặt f của I lên một khoảng của R, có điểm đầu bên trái 0, sao cho f(e) = 0 và f(xy) = f(x) + f(y) bất cứ khi nào x, y và xy thuộc I (điều này sẽ xảy ra bất cứ khi nào x và y thuộc W ∩ I, W là một lân cận của e sao cho W.W ⊂ V).

Với mọi phần tử x ∈ V không thuộc I ta có x < e, do đó x^{-1} > e; vì thế ta có thể mở rộng f thành một ánh xạ tăng ngặt $\overline{f}$ của V lên một khoảng của R bằng cách đặt $\overline{f}(x) = -f(x^{-1})$ với mọi x < e trong V. Ảnh ngược dưới $\overline{f}$ của một khoảng mở chứa trong $\overline{f}(V)$ là một khoảng mở của V, do đó $\overline{f}$ liên tục trên V; ngược lại, ảnh dưới $\overline{f}$ của một khoảng mở của V là một khoảng mở của $\overline{f}(V)$, và vì vậy $\overline{f}$ là một đồng phôi của V lên một lân cận của 0 trong nhóm R. Mặt khác, dễ dàng kiểm tra (như trong Mệnh đề 6 của § 1, no. 4, bằng cách xét các trường hợp có thể xảy ra) rằng ta có $\overline{f}(xy) = \overline{f}(x) + \overline{f}(y)$ bất cứ khi nào x, y và xy đều thuộc V; và do đó ta kết luận rằng $\overline{f}$, hạn chế trên một lân cận thích hợp của e trong G, là một đẳng cấu địa phương của G với R (Chương III, § 1, no. 3, Mệnh đề 3).

Q.E.D.

#### Định lý 2 {#top-v-s3-thm-2 .statement}

*Một nhóm liên thông* $G$ *trong đó tồn tại một lân cận của phần tử đơn vị đồng phôi với một khoảng mở của* $\mathbf{R}$ *là đẳng cấu với một trong hai nhóm* $\mathbf{R}$ *hoặc* $\mathbf{T}$.

Đây là một hệ quả ngay lập tức của định lý trước đó, cùng với Mệnh đề 7 của § 1, no. 4.

#### Nhận xét 1 {#top-v-s3-rem-1 .statement}

Để quyết định xem một nhóm $G$ thỏa mãn các điều kiện của Định lý 2 có đẳng cấu với $\mathbf{T}$ hay với $\mathbf{R}$, chỉ cần xem $G$ có compact hay không.

#### Nhận xét 2 {#top-v-s3-rem-2 .statement}

Định lý 2 chỉ ra đặc biệt rằng mọi nhóm tôpô *đồng phôi* với nhóm $\mathbf{R}$ *tất yếu là đẳng cấu* với $\mathbf{R}$.

#### Nhận xét 3 {#top-v-s3-rem-3 .statement}

Đặc trưng hóa tôpô trước đó của các nhóm $\mathbf{R}$ và $\mathbf{T}$ liên quan đến không gian tôpô $\mathbf{R}$ như một tập hợp phụ trợ. Có thể đặc trưng hóa các cấu trúc nhóm tôpô của $\mathbf{R}$ và $\mathbf{T}$ bằng các tiên đề không liên quan đến bất kỳ tập hợp phụ trợ nào (xem Các bài tập 4 và 5).

### Bài tập {#top-v-s3-exercises}

Xem [các bài tập cho § 3](exercises/s3/).
