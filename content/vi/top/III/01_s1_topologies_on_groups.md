---
book: top
book_title: General Topology
chapter: III
chapter_title: Topological Groups
section: 1
section_title: Topologies on groups
lang: vi
source: top-i-iv
pdf_pages: 0225-0231, 0302-0304
extraction: ocr
subsections:
    - "no": 1
      title: TOPOLOGICAL GROUPS
      page: 0
      pdf_page: 225
    - "no": 2
      title: NEIGHBOURHOODS OF A POINT IN A TOPOLOGICAL GROUP
      page: 0
      pdf_page: 227
    - "no": 3
      title: ISOMORPHISMS AND LOCAL ISOMORPHISMS
      page: 0
      pdf_page: 230
statements: 11
exercises: 9
content_sha256: 8fee9f67022015326d4e3a837e70b181399c0654e3e958317083cf7d19106f27
translated_from: content/en/top/III/01_s1_topologies_on_groups.md
source_content_sha256: affaabe14a2e0bad085ddd12018576d2fcad7b3610b4c325c8565f53e07ee793
translation_model: gpt-5.4
translation_run: translate-vi-e66c7828
glossary_version: 34
glossary_terms_sha256: 49f975cb2278dd4c8874686fb6b44d2969120636cebee567251607a136421b78
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 1. TÔPÔ TRÊN CÁC NHÓM

### 1. NHÓM TÔPÔ

Trong bốn tiết đầu của chương này, luật hợp thành của một nhóm nói chung sẽ được viết theo lối nhân, và e sẽ chỉ phần tử đơn vị; việc chuyển các kết quả sang ký hiệu cộng tính (mà ta nhắc lại là chỉ dành riêng cho các nhóm giao hoán) thường để cho người đọc.

#### Định nghĩa 1 {#top-iii-s1-def-1 .statement}

Một nhóm tôpô là một tập hợp G được trang bị một cấu trúc nhóm và một tôpô, đồng thời thỏa mãn hai tiên đề sau đây:

(GT_I). Ánh xạ $ (x, y) \to xy $ từ $ G \times G $ vào $ G $ là liên tục.

(GT_{II}). Ánh xạ $ x \to x^{-1} $ từ $ G $ vào $ G $ (phép đối xứng của nhóm G) là liên tục.

Người ta nói rằng một cấu trúc nhóm và một tôpô trên một tập hợp G là tương thích nếu chúng thỏa mãn (GT_I) và (GT_{II}).

#### Ví dụ 1 {#top-iii-s1-n1-exa-1 .statement}

Tôpô rời rạc trên một nhóm G là tương thích với cấu trúc nhóm. Một nhóm tôpô mà tôpô của nó là rời rạc được gọi là một nhóm rời rạc.

Mặt khác, tôpô thô nhất (Chương I, § 2, no. 2) trên G là tương thích với cấu trúc nhóm của G.

#### Ví dụ 2 {#top-iii-s1-n1-exa-2 .statement}

Trong Chương IV, ta sẽ thấy rằng tôpô của đường thẳng hữu tỉ Q (tương ứng, đường thẳng thực R) là tương thích với cấu trúc nhóm cộng của Q (tương ứng, R).

#### Ví dụ 3 {#top-iii-s1-n1-exa-3 .statement}

Nếu G là một nhóm tôpô, thì tôpô của nó tương thích với cấu trúc của nhóm $ G^0 $ là nhóm đối của G; $ G^0 $, với tôpô này, được gọi là nhóm tôpô đối của G.

Các tiên đề $ (\mathrm{GT}_\mathrm{I}) $ và $ (\mathrm{GT}_\mathrm{II}) $ tương đương với mệnh đề sau đây:

(GT'). *Ánh xạ* $ (x, y) \to xy^{-1} $ *từ* $ G \times G $ *vào* $ G $ *là liên tục*.

Rõ ràng $ (\mathrm{GT}_\mathrm{I}) $ và $ (\mathrm{GT}_\mathrm{II}) $ cùng nhau suy ra (GT'). Ngược lại, (GT') suy ra $ (\mathrm{GT}_\mathrm{II}) $, vì khi đó $ x \to ex^{-1} = x^{-1} $ liên tục; và (GT') cùng với $ (\mathrm{GT}_\mathrm{II}) $ suy ra $ (\mathrm{GT}_\mathrm{I}) $, vì khi đó $ (x, y) \to x(y^{-1})^{-1} = xy $ liên tục.

Nếu $ a $ là một phần tử bất kỳ của $ G $, thì *phép tịnh tiến trái* $ x \to ax $ (resp. *phép tịnh tiến phải* $ x \to xa $) liên tục, theo $ (\mathrm{GT}_\mathrm{I}) $, và do đó là một *phép đồng phôi* của $ G $ lên $ G $. Vì thế các ánh xạ $ x \to axb $, khi $ a $ và $ b $ chạy qua $ G $, tạo thành một *nhóm các phép đồng phôi* của $ G $; các ánh xạ $ x \to axa^{-1} $ (resp. $ x \to ax, x \to xa $), trong đó $ a $ chạy qua $ G $, tạo thành một nhóm con của nhóm các phép đồng phôi này. Hơn nữa, vì phép đối xứng $ x \to x^{-1} $ là một phép hoán vị đối hợp của $ G $, tiên đề $ (\mathrm{GT}_\mathrm{II}) $ cho thấy rằng ánh xạ này là một *phép đồng phôi* của $ G $ lên $ G $.

Nếu $ A $ là một tập con mở (tương ứng, đóng) của $ G $, và nếu $ x $ là một điểm bất kỳ của $ G $, thì các tập hợp $ x.A, A.x $ và $ A^{-1} (*) $ là mở (tương ứng, đóng), vì chúng là các ảnh của $ A $ qua một trong các phép đồng phôi ở trên. Nếu $ A $ là *mở* và $ B $ là một tập con bất kỳ của $ G $, thì $ AB $ và $ BA $ là *mở*, vì chúng là các hợp của các tập hợp mở [tiên đề $ (\mathrm{O}_\mathrm{I}) $]. Nếu $ V $ là một lân cận của $ e $ trong $ G $, thì $ VA $ và $ AV $ là các *lân cận* của $ A $; thật vậy, nếu $ W $ là một lân cận mở của $ e $ được chứa trong $ V $, thì $ WA $ và $ AW $ là mở và chứa $ A $.

Mặt khác, $ AB $ không nhất thiết đóng khi $ A $ đóng, ngay cả nếu $ B $ cũng đóng (x. § 4, no. 1, Hệ quả 1 của Mệnh đề 1).

\* Ví dụ, trong nhóm cộng của đường thẳng thực $ \mathbf{R} $, nhóm con $ \mathbf{Z} $ của các số nguyên hữu tỉ là đóng, và nhóm con $ \theta \mathbf{Z} $ gồm mọi bội số nguyên $ n\theta $ của một số *vô tỉ* $ \theta $ cũng vậy; nhưng nhóm con $ \mathbf{Z} + \theta \mathbf{Z} $ của $ \mathbf{R} $, là tập hợp mọi số thực $ m + n\theta $ (trong đó $ m $ và $ n $ nhận mọi giá trị nguyên) thì không đóng trong $ \mathbf{R} $, như ta sẽ thấy ở Chương V, § 1.

Lại cho $ A $ là tập con của nhóm cộng của $ \mathbf{R} \times \mathbf{R} $ gồm mọi cặp $ (x, y) $ sao cho $ x \geqslant 0 $ và $ 0 \leqslant y \leqslant 1 - \frac{1}{x+1} $; và cho $ B $ là tập hợp mọi cặp $ (x, 0) $, khi $ x $ chạy qua $ \mathbf{R} $. $ A $ và $ B $ là đóng, nhưng $ A + B $ là tập hợp mọi cặp $ (x, y) $ sao cho $ 0 \leqslant y < 1 $, và không đóng trong $ \mathbf{R} \times \mathbf{R} $. \*

Cho $ X $ là một không gian tôpô và $ f $ và $ g $ là hai ánh xạ từ $ X $ vào một nhóm tôpô $ G $. Nếu $ f $ và $ g $ liên tục tại một điểm $ x_0 $

(*) Ta nhắc lại rằng nếu $ A $ và $ B $ là hai tập hợp con của một nhóm $ G $, thì $ A.B $ hoặc $ AB $ ký hiệu tập hợp tất cả các tích $ xy $ với $ x \in A $ và $ y \in B $; $ A^{-1} $ ký hiệu tập hợp tất cả các phần tử $ x^{-1} $ với $ x \in A $. Nếu $ B $ chỉ gồm một phần tử $ x $, thì ta viết $ x.A $ hoặc $ xA $ (tương ứng, $ A.x $ hoặc $ Ax $) thay cho $ \{ x \}.A $ (tương ứng, $ A.\{ x \} $).

của X, thì $ f^{-1} $ và $ fg $ cũng vậy(*), theo Định lý 2 của Chương I, § 2, no. 1. Đặc biệt, các ánh xạ liên tục từ X vào G tạo thành một nhóm con của nhóm $ G^X $ gồm mọi ánh xạ từ X vào G.

Lại nữa, cho $ f $ và $ g $ là hai ánh xạ từ một tập hợp X, được lọc bởi một bộ lọc $ \mathfrak{F} $, vào một nhóm tôpô Hausdorff G. Nếu $ \lim_{\mathfrak{F}} f $ và $ \lim_{\mathfrak{F}} g $ tồn tại, thì $ \lim_{\mathfrak{F}} f^{-1} $ và $ \lim_{\mathfrak{F}} fg $ cũng tồn tại, và ta có (Chương I, § 7, no. 4, Mệnh đề 9, Hệ quả 1)

(1) $$
\lim_{\mathfrak{F}} f^{-1} = (\lim_{\mathfrak{F}} f)^{-1},
$$
(2) $$
\lim_{\mathfrak{F}} fg = (\lim_{\mathfrak{F}} f) (\lim_{\mathfrak{F}} g).
$$

Khi G là một nhóm giao hoán, được viết theo lối cộng, tiên đề (GT') cho biết rằng $ (x, y) \to x - y $ là một ánh xạ liên tục. Nếu $ f $ và $ g $ là các ánh xạ từ một không gian tôpô X vào G, liên tục tại một điểm $ x_0 $, thì $ f - g $ liên tục tại điểm đó. Các công thức (1) và (2) có thể được chép lại tương tự.

### 2. LÂN CẬN CỦA MỘT ĐIỂM TRONG MỘT NHÓM TÔPÔ

Cho $ \mathcal{B} $ là bộ lọc lân cận của phần tử đơn vị $ e $ trong một nhóm tôpô G, và cho $ a $ là một điểm bất kỳ của G. Vì $ x \to ax $ và $ x \to xa $ là các phép đồng phôi, suy ra bộ lọc lân cận của $ a $ là họ $ a.\mathcal{B} $ các tập hợp $ a.V $, trong đó V chạy qua $ \mathcal{B} $, và cũng là họ $ \mathcal{B}.a $ các tập hợp $ V.a $. Do đó ta biết bộ lọc lân cận của mọi điểm của một nhóm tôpô ngay khi ta biết bộ lọc lân cận của phần tử đơn vị $ e $ của nhóm.

Nếu ta nói rằng $ xy $ và $ x^{-1} $ liên tục tại $ x = y = e $, thì ta thu được (Chương I, § 2, no. 1):

(GV_I). *Với mọi* $ U \in \mathcal{B} $, *tồn tại* $ V \in \mathcal{B} $ *sao cho* $ V.V \subset U $.

(GV_{II}). *Với mọi* $ U \in \mathcal{B} $, *ta có* $ \overline{U} \in \mathcal{B} $.

Mọi bộ lọc $ \mathcal{B} $ trên G thỏa mãn (GV_I) và (GV_{II}) cũng thỏa mãn (GV_a). *Với mọi* $ U \in \mathcal{B} $, *tồn tại* $ V \in \mathcal{B} $ *sao cho* $ V.V^{-1} \subset U $. Thật vậy, theo (GV_I), tồn tại $ W \in \mathcal{B} $ sao cho $ W.W \subset U $, và theo (GV_{II}) tồn tại $ V \in \mathcal{B} $ sao cho $ V \subset W \cap W^{-1} $; do đó $ V^{-1} \subset W $ và vì thế $ V.V^{-1} \subset W.W \subset U $.

Ngược lại, nếu một bộ lọc $ \mathcal{B} $ trên G thỏa mãn (GV_a), trước hết suy ra rằng $ e $ thuộc mọi tập $ U \in \mathcal{B} $; thật vậy, nếu $ V \in \mathcal{B} $ sao cho $ V.V^{-1} \subset U $,

(*) Chúng tôi nhắc lại rằng $ f^{-1} $ là ánh xạ $ x \to (f(x))^{-1} $ và $ fg $ là ánh xạ $ x \to f(x)g(x) $; không nên nhầm chúng với $ f^{-1} $ và $ f \circ g $ (khi các ánh xạ này được xác định) (*Lý thuyết tập hợp*, R, § 2, số 6 và 11).

khi đó, vì $ V $ không rỗng, ta có $ x.x^{-1} = e \in U $ với mọi $ x \in V $. Do đó điều kiện $ (GV_a) $ suy ra $ V^{-1} \subset V.V^{-1} \subset U $, nên $ U^{-1} \in \mathcal{B} $ mỗi khi $ U \in \mathcal{B} $. Cuối cùng, nếu $ V \in \mathcal{B} $ sao cho $ V.V^{-1} \subset U $, và nếu $ W \in \mathcal{B} $ sao cho $ W \subset V \cap V^{-1} $, thì ta có $ W.W \subset U $. Như vậy ta thấy rằng $ (GV_a) $ là *tương đương* với phép hội của $ (GV_1) $ và $ (GV_{II}) $.

Cuối cùng, vì $ x \to axa^{-1} $ là một đồng phôi để lại $ e $ bất động, $ \mathcal{B} $ có tính chất sau:

$(GV_{III}).$ *Với mọi* $ a \in G $ *và mọi* $ V \in \mathcal{B} $, *ta có* $ a.Va^{-1} \in \mathcal{B} $.

Ba tính chất này của bộ lọc $ \mathcal{B} $ là *đặc số*:

#### Mệnh đề 1 {#top-iii-s1-prop-1 .statement}

*Cho* $ G $ *là một nhóm và cho* $ \mathcal{B} $ *là một bộ lọc trên* $ G $ *thỏa mãn các tiên đề* $ (GV_1) $, $ (GV_{II}) $ *và* $ (GV_{III}) $. *Khi đó tồn tại duy nhất một tôpô trên* $ G $, *tương thích với cấu trúc nhóm của* $ G $, *mà đối với tôpô này* $ \mathcal{B} $ *là bộ lọc lân cận của phần tử đơn vị* $ e $. *Đối với tôpô này, bộ lọc lân cận của mọi điểm* $ a \in G $ *trùng với mỗi một trong hai bộ lọc* $ a.\mathcal{B} $ *và* $ \mathcal{B}.a $.

Nếu có một tôpô với các tính chất được yêu cầu, thì theo điều đã nói ở trên, bộ lọc lân cận của $ a $ trùng với mỗi bộ lọc $ a.\mathcal{B} $ và $ \mathcal{B}.a $; do đó tôpô là duy nhất, nếu nó tồn tại. Sự tồn tại của nó sẽ được thiết lập nếu ta chỉ ra 1) rằng các bộ lọc $ a.\mathcal{B} $ là các bộ lọc lân cận của một tôpô trên $ G $, và 2) rằng tôpô này tương thích với cấu trúc nhóm của $ G $.

1) Bộ lọc $ a.\mathcal{B} $ thỏa mãn tiên đề $ (V_{III}) $ (xem Chương I § 1, no. 2) do $ (GV_1) $ và $ (GV_{II}) $, như ta đã thấy; vì thế để chỉ ra rằng $ a.\mathcal{B} $ là bộ lọc lân cận của $ a $ trong một tôpô trên $ G $, ta phải kiểm tra tiên đề $ (V_{IV}) $. Khi đó, lấy $ V $ là một tập hợp bất kỳ của $ \mathcal{B} $, và $ W $ là một tập hợp của $ \mathcal{B} $ sao cho $ W.W \subset V $; khi ấy với mọi $ x \in a.W $ ta có $ x.W \subset a.W.W \subset a.V $, nên $ a.V $ thuộc bộ lọc $ x.\mathcal{B} $; do đó $ (V_{IV}) $ được thỏa mãn.

2) Bây giờ ta hãy chứng minh rằng tôpô được xác định bởi các bộ lọc lân cận $ a.\mathcal{B} $ thỏa mãn $ (GT') $. Cho $ a, b $ là hai điểm bất kỳ của $ G $; nếu đặt $ x = au $ và $ y = bv $, thì ta phải chứng minh rằng $ xy^{-1} $ gần $ ab^{-1} $ tùy ý, mỗi khi $ u $ và $ v $ đủ gần $ e $. Mà $ (ab^{-1})^{-1}(xy^{-1}) = buv^{-1}b^{-1} $; cho $ U $ là một lân cận bất kỳ của $ e $, khi đó ta sẽ có $ buv^{-1}b^{-1} \in U $ nếu $ uv^{-1} \in b^{-1}Ub = V $, và $ V \in \mathcal{B} $ theo $ (GV_{III}) $. Nhưng theo $ (GV_1) $ và $ (GV_{II}) $ tồn tại $ W \in \mathcal{B} $ sao cho $ W.W^{-1} \subset V $; do đó chỉ cần lấy $ u \in W $ và $ v \in W $ thì có $ xy^{-1} \in (ab^{-1})U $. Điều này hoàn tất chứng minh.

Một phương pháp chung để định nghĩa một tôpô tương thích với một cấu trúc nhóm trên $ G $ là cho một bộ lọc thỏa mãn các tiên đề $ (GV_1) $, $ (GV_{II}) $ và $ (GV_{III}) $. Các điều kiện tương ứng đối với một *cơ sở bộ lọc* $ \mathcal{B} $ là như sau:

$(GV'_1).$ *Với mọi* $ U \in \mathcal{B} $, *tồn tại* $ V \in \mathcal{B} $ *sao cho* $ V.V \subset U $.

(GV_{II}). *Với mọi* $ U \in \mathcal{B} $, *tồn tại* $ V \in \mathcal{B} $ *sao cho* $ V^{-1} \subset U $.

(GV'_{III}). *Với mọi* $ a \in G $ *và mọi* $ U \in \mathcal{B} $, *tồn tại* $ V \in \mathcal{B} $ *sao cho* $ V \subset a . U . a^{-1} $.

Một lân cận của $ e $ trùng với ảnh của nó qua đối xứng $ x \to x^{-1} $ được gọi là *đối xứng*. Nếu $ V $ là một lân cận bất kỳ của $ e $, thì $ V \cup V^{-1} $, $ V \cap V^{-1} $ và $ V . V^{-1} $ là các lân cận đối xứng. Theo (GV_{II}), các lân cận đối xứng tạo thành một *hệ lân cận cơ bản* của $ e $. Cũng suy ra từ (GV_{I}) rằng khi $ V $ chạy qua một hệ lân cận cơ bản của $ e $, thì các tập hợp $ V^n $ (trong đó $ n $ là một số nguyên cố định $ \neq 0 $) tạo thành một hệ lân cận cơ bản của $ e $.

#### Nhận xét {#top-iii-s1-n2-rem-1 .statement}

Nếu $ G $ *giao hoán*, ta có $ x . A . x^{-1} = A $ với mọi tập con $ A $ của $ G $ và mọi $ x \in G $, và do đó (GV_{III}) [tương ứng, (GV'_{III})] được thỏa mãn một cách tự động đối với mọi bộ lọc (tương ứng, cơ sở bộ lọc) trên $ G $. Mặt khác, nếu $ G $ không Abel, thì (GV_{III}) không phải là một hệ quả của (GV_{I}) và (GV_{II}) [xem Bài tập 5].

Nếu $ G $ là một nhóm giao hoán, được viết *theo lối cộng*, thì các tiên đề đặc trưng cho bộ lọc $ \mathcal{B} $ các lân cận của phần tử không đối với một tôpô tương thích với cấu trúc nhóm của $ G $ do đó là như sau:

(GA_{I}). *Với mọi* $ U \in \mathcal{B} $, *tồn tại* $ V \in \mathcal{B} $ *sao cho* $ V + V \subset U $.

(GA_{II}). *Với mọi* $ U \in \mathcal{B} $, *ta có* $ -U \in \mathcal{B} $.

#### Mệnh đề 2 {#top-iii-s1-prop-2 .statement}

*Một nhóm tôpô* $ G $ *là Hausdorff khi và chỉ khi tập hợp* $ \{e\} $ *là đóng*.

Rõ ràng, nếu $ G $ là Hausdorff, thì $ \{e\} $ là đóng. Ngược lại, nếu $ \{e\} $ là đóng, thì đường chéo $ \Delta $ của $ G \times G $ là đóng, vì nó là ảnh ngược của $ \{e\} $ dưới ánh xạ liên tục $ (x, y) \to xy^{-1} $; do đó (Chương I, § 8, no. 1, Mệnh đề 1) $ G $ là Hausdorff.

#### Hệ quả {#top-iii-s1-n2-cor-1 .statement}

*Một nhóm tôpô* $ G $ *là Hausdorff khi và chỉ khi giao của các lân cận của* $ e $ *chỉ gồm điểm* $ e $.

Điều kiện ấy rõ ràng là cần thiết. Ngược lại, nếu giao của tất cả các lân cận của $ e $ chỉ là $ \{e\} $, thì với mọi $ x \neq e $ cho trước có một lân cận $ V $ của $ e $ sao cho $ x^{-1} \notin V $ và do đó $ e \notin xV $. Điều này chứng tỏ rằng $ x $ không thuộc bao đóng của $ \{e\} $, và vì thế $ \{e\} $ là đóng, nên $ G $ là Hausdorff.

#### Ví dụ {#top-iii-s1-n2-exa-1 .statement}

*Định nghĩa một tôpô trên một nhóm bằng một tập hợp các nhóm con.* Nếu $ \mathcal{B} $ là một *cơ sở lọc* trên một nhóm $ G $, được tạo thành từ các *nhóm con* của $ G $, thì thấy ngay lập tức rằng $ \mathcal{B} $ thỏa mãn các tiên đề (GV_{I}) và (GV_{II}), vì $ H . H^{-1} = H $ với mọi nhóm con $ H $ của $ G $. Do đó tập hợp $ \mathcal{B} $ sẽ là một *hệ cơ bản các lân cận* của $ e $ trong một tôpô tương thích với cấu trúc nhóm của $ G $, miễn là $ \mathcal{B} $ thỏa mãn (GV_{III}); điều này đặc biệt đúng nếu mọi nhóm con trong $ \mathcal{B} $ đều là chuẩn tắc, vì thế luôn luôn đúng nếu $ G $ là *giao hoán*. Tôpô được định nghĩa như vậy là *Hausdorff*, theo Mệnh đề 2, khi và chỉ khi *giao của tất cả các nhóm con trong $ \mathcal{B} $ chỉ gồm* $ e $. Những trường hợp đáng quan tâm nhất là các trường hợp trong đó nhóm con $ \{ e \} $ *không thuộc* $ \mathcal{B} $ (nếu không thì tôpô được định nghĩa bởi $ \mathcal{B} $ là tôpô *rời rạc*): nếu $ \{ e \} \notin \mathcal{B} $, tôpô được định nghĩa bởi $ \mathcal{B} $ chỉ là Hausdorff nếu $ \mathcal{B} $ là một *tập hợp vô hạn*.

Vì giao của hai nhóm con là một nhóm con, ta có thể định nghĩa một tôpô trên $ G $, tương thích với cấu trúc nhóm của nó, xuất phát từ *bất kỳ* tập hợp nào $ \mathfrak{F} $ các nhóm con của $ G $: đặt $ \mathfrak{G} $ là tập hợp của mọi nhóm con $ a.H.a^{-1} $, trong đó $ H \in \mathfrak{F} $ và $ a \in G $, và đặt $ \mathcal{B} $ là tập hợp của mọi giao *hữu hạn* của các nhóm con thuộc $ \mathfrak{G} $. Khi đó $ \mathcal{B} $ là một cơ sở bộ lọc và thỏa mãn (GV$_{\text{III}}$).

Xét riêng nhóm cộng của một *vành* $ A $. Mỗi tập hợp $ \mathfrak{F} $ các *iđêan* của $ A $ xác định một tôpô tương thích với cấu trúc nhóm cộng này. Tôpô này là Hausdorff nếu giao của tất cả các iđêan thuộc $ \mathfrak{F} $ là iđêan không, và nó không rời rạc nếu không có giao hữu hạn nào của các iđêan thuộc $ \mathfrak{F} $ là iđêan không. Các tôpô được xác định theo cách này giữ một vai trò quan trọng trong lý thuyết số (xem các Bài tập của §§ 6 và 7 của chương này).

### 3. ĐẲNG CẤU VÀ ĐẲNG CẤU ĐỊA PHƯƠNG

Phù hợp với các định nghĩa tổng quát (*Lý thuyết tập hợp*, Chương IV, § 1, no. 5), một *đẳng cấu* $ f $ của một nhóm tôpô $ G $ *lên trên* một nhóm tôpô $ G' $ là một ánh xạ song ánh từ $ G $ lên $ G' $ đồng thời là một *đẳng cấu của cấu trúc nhóm của* $ G $ lên cấu trúc nhóm của $ G' $, và một *đồng phôi của* $ G $ lên $ G' $. Nói cách khác, $ f $ là một đẳng cấu từ $ G $ lên $ G' $ khi và chỉ khi: 1) $ f $ là song ánh; 2) $ f(xy) = f(x)f(y) $ với mọi $ x, y \in G $; và 3) $ f $ là song liên tục.

Ví dụ, nếu $ a $ là một điểm bất kỳ của $ G $, ánh xạ $ x \to axa^{-1} $ là một đẳng cấu của $ G $ lên $ G $, tức là (*loc. cit.*), một *tự đẳng cấu* của nhóm tôpô $ G $. Nó được gọi là một *tự đẳng cấu trong*.

Nếu một tôpô $ \mathcal{C} $ tương thích với cấu trúc nhóm của một nhóm $ G $, thì $ \mathcal{C} $ cũng tương thích với cấu trúc nhóm *đối* của $ G $. Nếu $ G^0 $ ký hiệu nhóm tôpô nhận được bằng cách trang bị cho nhóm đối của $ G $ tôpô $ \mathcal{C} $, thì phép đối xứng $ x \to x^{-1} $ là một *đẳng cấu* của nhóm tôpô $ G $ lên nhóm tôpô $ G^0 $.

#### Định nghĩa 2 {#top-iii-s1-def-2 .statement}

*Nếu* $ G $ *và* $ G' $ *là hai nhóm tôpô, một đẳng cấu địa phương của* $ G $ *với* $ G' $ *là một đồng phôi* $ f $ *từ một lân cận* $ V $ *của phần tử đơn vị của* $ G $ *lên một lân cận* $ V' $ *của phần tử đơn vị của* $ G' $ *thỏa mãn các điều kiện sau đây:*

1) *Với mỗi cặp* $ x, y $ *điểm của* $ V $ *sao cho* $ xy \in V $,
$$
f(xy) = f(x)f(y).
$$

2) Nếu g là ánh xạ nghịch đảo của f, thì với mỗi cặp điểm x', y' của V' sao cho x'y' ∈ V', ta có g(x'y') = g(x') g(y').
Khi đó ánh xạ g là một đẳng cấu địa phương của G' với G.
Hai nhóm tôpô G, G' được gọi là đẳng cấu địa phương nếu tồn tại một đẳng cấu địa phương của G với G'.

Các nhóm tôpô đẳng cấu hiển nhiên là đẳng cấu địa phương. Đảo lại là sai.

\* Chẳng hạn, ta sẽ thấy trong Chương V, § 1, rằng các nhóm tôpô R và T là đẳng cấu địa phương nhưng không đẳng cấu. \*

Nếu f là một đẳng cấu địa phương của G với G', thì mọi hạn chế của f lên một lân cận của phần tử đơn vị của G lại vẫn là một đẳng cấu địa phương của G với G'.

Một đẳng cấu địa phương của G với G được gọi là một tự đẳng cấu địa phương của G.

Nói chung, nếu f là một đồng phôi từ một lân cận V của phần tử đơn vị của G lên một lân cận V' của phần tử đơn vị của G' thỏa mãn điều kiện 1) của Định nghĩa 2, thì f không nhất thiết thỏa mãn điều kiện 2) (xem Bài tập 7). Tuy nhiên, G và G' thực ra là đẳng cấu địa phương.

#### Mệnh đề 3 {#top-iii-s1-prop-3 .statement}

Cho G và G' là hai nhóm tôpô, và cho f là một đồng phôi từ một lân cận V của phần tử đơn vị của G lên một lân cận V' của phần tử đơn vị của G', thỏa mãn điều kiện 1) của Định nghĩa 2. Khi đó f là một mở rộng của một đẳng cấu địa phương của G với G'.

Thật vậy, không khó để thấy rằng nếu W là một lân cận của phần tử đơn vị của G sao cho W.W ⊂ V, thì hạn chế của f lên W là một đẳng cấu địa phương của G với G'.

### Bài tập {#top-iii-s1-exercises}

Xem [bài tập cho § 1](exercises/s1/).
