---
book: ens
book_title: Theory of Sets
chapter: IV
chapter_title: STRUCTURES
section: 3
section_title: Universal mappings
lang: vi
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 283-288, 294-295
pdf_pages: 0288-0293, 0299-0300
extraction: ocr
subsections:
    - "no": 1
      title: UNIVERSAL SETS AND MAPPINGS
      page: 283
      pdf_page: 288
    - "no": 2
      title: EXISTENCE OF UNIVERSAL MAPPINGS
      page: 284
      pdf_page: 289
    - "no": 3
      title: EXAMPLES OF UNIVERSAL MAPPINGS
      page: 286
      pdf_page: 291
statements: 0
exercises: 3
content_sha256: e0d6f1d3ac680784ebbba2ceccdd530739c71ccfe7de1f79dd906f6c3543a4ba
translated_from: content/en/ens/IV/03_s3_universal_mappings.md
source_content_sha256: 98de15070c6122f15d37cc5ed3db1f93782ce63e3a7bbc618529bef0a4082473
translation_model: gpt-5.4
translation_run: translate-vi-09555ffd
glossary_version: 29
glossary_terms_sha256: 5c1b2fc3a46a9ee4d0ce36fff1d95af737aa582b9c9ef2a9d1c855744febe162
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 3. ÁNH XẠ PHỔ QUÁT

### 1. TẬP HỢP PHỔ QUÁT VÀ ÁNH XẠ PHỔ QUÁT

Cho $\mathscr{T}$ là một lý thuyết mạnh hơn lý thuyết tập hợp, và cho E là một số hạng trong $\mathscr{T}$. Cho $\Sigma$ là một loài cấu trúc trong $\mathscr{T}$. Để đơn giản, trong toàn bộ phần này ta sẽ giả sử rằng $\Sigma$ được định nghĩa trên một tập cơ sở (chính) duy nhất, và để ngắn gọn ta sẽ nói “$\Sigma$-tập hợp” thay cho “tập hợp được trang bị một cấu trúc thuộc loài $\Sigma$”. Hơn nữa, ta sẽ giả sử rằng các $\sigma$-cấu xạ đã được định nghĩa cho loài $\Sigma$ (§ 2, no. 1; như trong § 2, ta sẽ nói “cấu xạ” thay cho “$\sigma$-cấu xạ”). Sau hết, vì loài $\Sigma$ được định nghĩa trên tập cơ sở $x$ và có $s$ làm cấu trúc tổng quát (§ 1, no. 4), ta hãy giả sử rằng một số hạng $\alpha\{x,s\}$ được định nghĩa trong $\mathscr{T}_{\Sigma}$, thỏa mãn các điều kiện sau :

(QM$_{\mathrm{I}}$) *Quan hệ $\alpha\{x,s\}\subset\mathscr{T}(E;x)$ là đúng trong $\mathscr{T}_{\Sigma}$.*

(QM$_{\mathrm{II}}$) *Nếu (trong một lý thuyết $\mathscr{T}'$ mạnh hơn $\mathscr{T}$) F và F′ là hai tập hợp được trang bị các cấu trúc $\mathscr{G},\mathscr{G}'$ thuộc loài $\Sigma$, và nếu $f$ là một cấu xạ từ F vào F′, thì quan hệ $\varphi\in\alpha\{F,\mathscr{G}\}$ suy ra $f\circ\varphi\in\alpha\{F',\mathscr{G}'\}$.*

Ta sẽ diễn đạt quan hệ $\varphi\in\alpha\{x,s\}$ bằng cách nói rằng $\varphi$ là một ánh xạ $\alpha$ của E vào $x$ ($s$ được trang bị trên đó).

Một tập hợp $\Sigma$ $F_E$ và một ánh xạ $\alpha$ $\varphi_E$ của E vào $F_E$ được gọi là *phổ quát* nếu điều kiện sau được thỏa mãn :

$(AU)$ *Với mỗi $\alpha$-ánh xạ $\varphi$ từ E vào một $\Sigma$-tập hợp F, tồn tại một cấu xạ duy nhất $f$ từ $F_E$ vào F sao cho $\varphi=f\circ\varphi_E$.*

Khi đó cặp $(F_E,\varphi_E)$ cũng được gọi là một *nghiệm của bài toán ánh xạ phổ quát* đối với E (tương đối với $\Sigma$, $\sigma$, và $\alpha$).

¶ Cho $(F'_E,\varphi'_E)$ và $(F''_E,\varphi''_E)$ là hai nghiệm của bài toán ánh xạ phổ quát đối với E. Điều kiện $(AU)$ khi đó cho thấy rằng tồn tại một cấu xạ duy nhất $f_1$ từ $F'_E$ vào $F''_E$ và một cấu xạ duy nhất $f_2$ từ $F''_E$ vào $F'_E$ sao cho $\varphi''_E=f_1\circ\varphi'_E$ và $\varphi'_E=f_2\circ\varphi''_E$. Do đó ta có $\varphi''_E=f_2\circ f_1\circ\varphi'_E$ và $\varphi'_E=f_1\circ f_2\circ\varphi''_E$. Áp dụng $(AU)$ cho trường hợp $F=F'_E$ và $\varphi=\varphi'_E$, ta thấy rằng $f_2\circ f_1$ là ánh xạ đồng nhất của $F'_E$ lên chính nó. Tương tự, $f_1\circ f_2$ là ánh xạ đồng nhất của $F''_E$ lên chính nó. Do đó (§ 2, no. 1, tiêu chuẩn CST8) $f_1$ là một *đẳng cấu* từ $F'_E$ lên $F''_E$, và $f_2$ là đẳng cấu nghịch đảo của nó. Kết quả này được phát biểu bằng cách nói rằng nghiệm của bài toán ánh xạ phổ quát đối với E là *duy nhất tới đẳng cấu*.

Để kiểm tra rằng một cặp $(F_E,\varphi_E)$ là một nghiệm của bài toán ánh xạ phổ quát đối với E, thường thuận tiện khi kiểm tra hai điều kiện sau :

$(AU'_{\mathrm I})$ *Với mọi $\Sigma$-tập hợp F và mọi $\alpha$-ánh xạ $\varphi$ từ E vào F, tồn tại một cấu xạ $f$ từ $F_E$ vào F sao cho $\varphi=f\circ\varphi_E$.*

$(AU'_{\mathrm{II}})$ *Với mọi $\Sigma$-tập hợp F, hai cấu xạ từ $F_E$ vào F trùng nhau trên $\varphi_E(E)$ thì bằng nhau.*

Thật vậy, nếu hai điều kiện này được thỏa mãn, thì cấu xạ $f$ mà sự tồn tại của nó được $(AU'_{\mathrm I})$ bảo đảm là duy nhất theo $(AU'_{\mathrm{II}})$. Ngược lại, hiển nhiên là $(AU)$ suy ra $(AU'_{\mathrm I})$; hơn nữa, nếu $f$ và $f'$ là hai cấu xạ của $F_E$ vào F trùng nhau trên $\varphi_E(E)$, thì ta có $f\circ\varphi_E=f'\circ\varphi_E$, do đó $f=f'$ khi áp dụng $(AU)$ cho ánh xạ $\alpha$ $f\circ\varphi_E$. Vậy $(AU)$ suy ra $(AU'_{\mathrm{II}})$.

### 2. SỰ TỒN TẠI CỦA CÁC ÁNH XẠ PHỔ QUÁT

Một bài toán ánh xạ phổ quát không tất yếu có nghiệm (Bài tập 1). Tuy nhiên, ta sẽ chỉ ra rằng các điều kiện sau kéo theo sự tồn tại của một nghiệm:

$(CU_{\mathrm I})$ *Trên mọi tích của một họ các $\Sigma$-tập hợp đều tồn tại một cấu trúc tích thuộc loài $\Sigma$ (§ 2, no. 4).*

$(CU_{\mathrm{II})}$ *Cho $(F_i)_{i\in I}$ là một họ các $\Sigma$-tập hợp, và với mỗi $i\in I$ cho $\varphi_i$ là một $\alpha$-ánh xạ từ E vào $F_i$. Khi đó ánh xạ $(\varphi_i)_{i\in I}$ từ E vào $\prod_{i\in I}F_i$ (được trang bị cấu trúc tích) là một $\alpha$-ánh xạ.*

Một tập con G của một $\Sigma$-tập hợp F sẽ được gọi là $\Sigma$-*chấp nhận được* nếu cấu trúc trên F cảm sinh một cấu trúc thuộc loài $\Sigma$ trên G ($\S\,2$, no. 4).

$(\mathrm{CU_{III}})$ *Tồn tại một lực lượng* $\mathfrak{a}$ *có các tính chất sau đây : với mọi* $\Sigma$-*tập hợp* F *và mọi* $\alpha$-*ánh xạ* $\varphi$ *từ* E *vào* F *đều tồn tại một* $\Sigma$-*tập con chấp nhận được* G *của* F *chứa* $\varphi(\mathrm{E})$, *có lực lượng* $\leqslant \mathfrak{a}$, *sao cho ánh xạ từ* E *vào* G *có cùng đồ thị với* $\varphi$ *là một* $\alpha$-*ánh xạ, và sao cho mọi cặp cấu xạ của* G *vào một* $\Sigma$-*tập hợp, trùng nhau trên* $\varphi(\mathrm{E})$, *thì bằng nhau.*

CST22. *Nếu các điều kiện* $(\mathrm{CU_I})$ *đến* $(\mathrm{CU_{III}})$ *được thỏa mãn, thì bài toán ánh xạ phổ quát đối với* E *có nghiệm.*

Trước hết ta sẽ chỉ ra rằng nếu tồn tại một cặp $(\mathrm{F_E},\ \varphi_\mathrm{E})$ thỏa mãn $(\mathrm{AU'_I})$, thì cũng tồn tại một nghiệm của bài toán ánh xạ phổ quát đối với E. Thật vậy, theo $(\mathrm{CU_{III}})$, tồn tại một tập con chấp nhận được đối với $\Sigma$ là $\mathrm{F'_E}$ của $\mathrm{F_E}$ chứa $\varphi_\mathrm{E}(\mathrm{E})$, sao cho ánh xạ $\varphi'_\mathrm{E}$ từ E vào $\mathrm{F'_E}$ có cùng đồ thị với $\varphi_\mathrm{E}$ là một $\alpha$-ánh xạ, và sao cho bất kỳ hai cấu xạ nào từ $\mathrm{F'_E}$ vào một $\Sigma$-tập hợp trùng nhau trên $\varphi_\mathrm{E}(\mathrm{E})$ đều bằng nhau. Gọi $j$ là đơn ánh chính tắc của $\mathrm{F'_E}$ vào $\mathrm{F_E}$, do đó $\varphi_\mathrm{E} = j \circ \varphi'_\mathrm{E}$. Với mọi cấu xạ $f$ từ $\mathrm{F_E}$ vào một $\Sigma$-tập hợp F, $f \circ j$ là một cấu xạ từ $\mathrm{F'_E}$ vào F, và ta có $f \circ \varphi_\mathrm{E} = (f \circ j) \circ \varphi'_\mathrm{E}$. Vì vậy hiển nhiên là $(\mathrm{F'_E},\ \varphi'_\mathrm{E})$ thỏa mãn $(\mathrm{AU'_I})$ và $(\mathrm{AU'_{II}})$.

Còn phải thiết lập sự tồn tại của một cặp $(\mathrm{F_E},\ \varphi_\mathrm{E})$ thỏa mãn $(\mathrm{AU'_I})$. Gọi $s \in \mathrm{S}(x)$ là đặc trưng hóa điển hình của loài cấu trúc $\Sigma$, và xét tập con L của $\mathfrak{P}(\mathfrak{a}) \times \mathrm{S}(\mathfrak{a}) \times \mathfrak{P}(\mathrm{E} \times \mathfrak{a})$ gồm tất cả các bộ ba $\lambda = (\mathrm{X},\ \mathrm{V},\ \mathrm{P})$ có tính chất sau : "V là một cấu trúc thuộc loài $\Sigma$ trên $\mathrm{X} \subset \mathfrak{a}$, và P là đồ thị của một $\alpha$-ánh xạ từ E vào X (đối với cấu trúc V)" (nhận thấy rằng ta có $\mathrm{S}(\mathrm{X}) \subset \mathrm{S}(\mathfrak{a})$, như dễ dàng thấy được khi lập luận từng bước theo độ dài của lược đồ phép dựng bậc thang S). Với mỗi $\lambda = (\mathrm{X},\ \mathrm{V},\ \mathrm{P}) \in \mathrm{L}$, ta ký hiệu bởi $\mathrm{X}_\lambda$ tập hợp X được trang bị cấu trúc V, và bởi $\varphi_\lambda$ ánh xạ từ E vào $\mathrm{X}_\lambda$ mà đồ thị là P.

Cho $\mathrm{F_E}$ là $\Sigma$-tập hợp là tích của các $\mathrm{X}_\lambda$ (nó tồn tại theo $(\mathrm{CU_I})$), và $\varphi_\mathrm{E}$ là ánh xạ $x \to (\varphi_\lambda(x))$ từ E vào $\mathrm{F_E}$, là một $\alpha$-ánh xạ theo $(\mathrm{CU_{II}})$. Ta sẽ chứng minh rằng cặp $(\mathrm{F_E},\ \varphi_\mathrm{E})$ thỏa mãn $(\mathrm{AU'_I})$. Cho một $\alpha$-ánh xạ $\varphi$ từ E vào một $\Sigma$-tập hợp F, gọi G là một tập con của F thỏa mãn các điều kiện đã phát biểu trong $(\mathrm{CU_{III}})$. Gọi $j$ là đơn ánh chính tắc của G vào F, và $\psi$ là ánh xạ từ E vào G có cùng đồ thị với $\varphi$, sao cho $\varphi = j \circ \psi$. Suy ra từ $(\mathrm{CU_{III}})$ rằng $\psi$ là một $\alpha$-ánh xạ từ E vào G. Vì Card (G) $\leqslant \mathfrak{a}$, tồn tại một tập con G$'$ của $\mathfrak{a}$ đẳng lực với G. Gọi $g$ là một song ánh từ G lên G$'$. Nếu ta dùng $g$ để chuyển cấu trúc loài $\Sigma$ trên G, thì theo định nghĩa tồn tại một phần tử $\lambda$ của L sao cho G$'$ (được trang bị cấu trúc được chuyển) bằng $\mathrm{X}_\lambda$ và sao cho $g \circ \psi = \varphi_\lambda$. Khi đó

$f = j \circ \overset{-1}{g} \circ \mathrm{pr}_\lambda$ là một cấu xạ từ $\mathrm{F_E}$ vào F sao cho $\varphi = f \circ \varphi_\mathrm{E}$, và chứng minh là đầy đủ.

CST23. *Cho* $(\mathrm{F_E},\ \varphi_\mathrm{E})$ *là một nghiệm của bài toán ánh xạ phổ quát đối với* E. *Khi đó* $\varphi_\mathrm{E}$ *là một đơn ánh của* E *vào* $\mathrm{F_E}$ *khi và chỉ khi, với mỗi cặp phần tử phân biệt* $x$, $y$ *của* E, *tồn tại một* $\alpha$-*ánh xạ* $\varphi$ *từ* E *vào một* $\Sigma$-*tập hợp* F *sao cho* $\varphi(x) \neq \varphi(y)$.

Vì $\varphi_\mathrm{E}$ là một $\alpha$-ánh xạ, tiêu chuẩn này là một hệ quả ngay lập tức của các định nghĩa.

¶ Trong trường hợp này, các $\alpha$-ánh xạ được gọi là *phân biệt* các phần tử của E, và theo thuật ngữ, thông thường ta không phân biệt giữa các phần tử của E và các ảnh của chúng qua $\varphi_\mathrm{E}$. Với quy ước này, nếu $(\mathrm{F_E},\ \varphi_\mathrm{E})$ là một nghiệm của một bài toán ánh xạ phổ quát, và nếu điều kiện $(\mathrm{CU_{III}})$ được thỏa mãn, thì mọi $\alpha$-ánh xạ từ E vào một $\Sigma$-tập hợp F *đều được mở rộng một cách duy nhất thành một cấu xạ từ* $\mathrm{F_E}$ *vào* F.

### 3. CÁC VÍ DỤ VỀ ÁNH XẠ PHỔ QUÁT

\* Phần lớn các ví dụ sau đây sẽ được khảo sát chi tiết ở chỗ khác trong chuỗi này.

I. *Các cấu trúc đại số tự do.* Cho E là một tập hợp và cho $\Sigma$ là một loài các cấu trúc đại số, được định nghĩa bởi một hoặc nhiều luật hợp thành. Ta lấy làm cấu xạ các *đồng cấu* đối với loài $\Sigma$ đang xét, và làm các ánh xạ $\alpha$ các ánh xạ *tùy ý* của E vào một $\Sigma$-tập hợp (nói cách khác, $\alpha \{ x,\ s \} = \mathscr{F}(\mathrm{E},\ x)$). Tất cả các loài thông thường của các cấu trúc đại số đều thỏa mãn $(\mathrm{CU_{III}})$; ngoại trừ các cấu trúc vành chia, chúng cũng thỏa mãn $(\mathrm{CU_I})$, và ở đây $(\mathrm{CU_{II}})$ là một hệ quả tầm thường của $(\mathrm{CU_I})$.

Vì nói chung tồn tại các cấu trúc thuộc loài $\Sigma$ được định nghĩa trên các tập hợp có ít nhất hai phần tử, các ánh xạ $\alpha$ tách biệt các phần tử của E, và do đó E có thể được xem như được nhúng vào $\mathrm{F_E}$. $\mathrm{F_E}$ được gọi là $\Sigma$-*tập hợp* *tự do sinh bởi* E. Vì vậy trong đại số ta nói đến *nửa nhóm tự do*, *nhóm tự do*, *môđun tự do*, và *đại số tự do*.

II. *Các vành và các trường phân thức.* Cho E là một vành giao hoán có phần tử đơn vị và cho S là một tập con đóng đối với phép nhân của E không chứa 0. Ta lấy $\Sigma$ làm loài cấu trúc của các vành giao hoán có phần tử đơn vị, và các cấu xạ là các đồng cấu vành biến đổi phần tử đơn vị thành phần tử đơn vị. Các ánh xạ $\alpha$ sẽ là các đồng cấu $\varphi$ của E vào một vành giao hoán A có phần tử đơn vị, sao cho $\varphi(1) = 1$ và $\varphi(\mathrm{S})$ chỉ chứa các *phần tử khả nghịch* của A. Các điều kiện $(\mathrm{QM_{II}})$, $(\mathrm{CU_I})$ đến $(\mathrm{CU_{III}})$ (với $\mathfrak{a} = \mathrm{Card}\ (\mathrm{E})\ \mathrm{Card}\ (\mathbf{N})$) được kiểm tra ngay lập tức. Do đó bài toán ánh xạ phổ quát luôn có một nghiệm $(\mathrm{F_E},\ \varphi_\mathrm{E})$, nhưng nói chung $\varphi_\mathrm{E}$

không đơn ánh. Trường hợp gặp thường xuyên nhất là trường hợp $E$ là một miền nguyên; trong trường hợp này, $\varphi_E$ là đơn ánh. Hơn nữa, nếu ta lấy $S = E - \{0\}$, thì $F_E$ là một trường, được gọi là *trường phân thức* của $E$.

III. *Tích tenxơ của hai môđun.* Cho $E$ là tích $A \times B$ của hai môđun trên một vành giao hoán $C$ có phần tử đơn vị. Lấy $\Sigma$ là loài các cấu trúc $C$-môđun, các cấu xạ là các ánh xạ tuyến tính, và các ánh xạ-$\alpha$ là các ánh xạ *song tuyến tính* từ $A \times B$ vào một $C$-môđun. Điều kiện $(QM_{II})$ hiển nhiên được thỏa mãn, và các điều kiện từ $(CU_I)$ đến $(CU_{III})$ cũng vậy (với $\mathfrak{a} = \mathrm{Card}\ (E)\ \mathrm{Card}\ (C)\ \mathrm{Card}\ (\mathbf{N})$). $C$-môđun phổ quát $F_E$ tương ứng với cặp $(A, B)$ được gọi là *tích tenxơ* của $A$ và $B$ và được ký hiệu là $A \otimes B$. Ánh xạ phổ quát $\varphi_E$ được viết là $(x,\ y) \to x \otimes y$; nó là song tuyến tính nhưng nói chung không đơn ánh.

IV. *Mở rộng vành các toán tử của một môđun.* Cho $A$ là một vành giao hoán với một phần tử đơn vị, cho $B$ là một vành con của $A$ chứa phần tử đơn vị của $A$, và cho $E$ là một $B$-môđun. Loài $\Sigma$ là loài các cấu trúc $A$-môđun, các cấu xạ là các ánh xạ $A$-*tuyến tính*, và các ánh xạ $\alpha$ là các ánh xạ $B$-*tuyến tính* từ $E$ vào một $A$-môđun. $A$-môđun phổ quát $F_E$ tương ứng với $B$-môđun $E$ được nói là thu được bằng cách *mở rộng lên* $A$ vành các toán tử $B$ của $E$.

V. *Sự hoàn thành của một không gian đều.* Cho $E$ là một không gian đều. Lấy $\Sigma$ là loài cấu trúc của các không gian đều Hausdorff đầy đủ, các cấu xạ là các ánh xạ liên tục đều, và các $\alpha$-ánh xạ là các ánh xạ liên tục đều từ $E$ vào một không gian đều Hausdorff đầy đủ. Các tập con $\Sigma$-chấp nhận được của một không gian đều Hausdorff đầy đủ ở đây là các tập con *đóng* (đối với tôpô của không gian), và các điều kiện $(QM_{II})$ và $(CU_I)$ đến $(CU_{III})$ được thỏa mãn (với $\mathfrak{a} = 2^{2^{\mathrm{Card}(E)}}$). Không gian đều Hausdorff đầy đủ này là (lên đến đẳng cấu) *sự hoàn thành* của không gian đều Hausdorff liên kết với $E$ (*Topologie générale*, Chương II, § 3, no. 7).

VI. *Compact hóa Stone-Čech.* Cho $E$ là một không gian hoàn toàn chính quy. $\Sigma$ là loài cấu trúc của các không gian compac, các cấu xạ là các ánh xạ liên tục (từ một không gian compac vào một không gian compac), và các ánh xạ $\alpha$ là các ánh xạ liên tục từ $E$ vào một không gian compac. Các tập con $\Sigma$-chấp nhận được lại là các tập *đóng*, và các điều kiện $(QM_{II})$, từ $(CU_I)$ đến $(CU_{III})$ được kiểm tra dễ dàng (với cùng lực lượng như trong Ví dụ V). Không gian compac $F_E$ là (sai khác đến đẳng cấu) "compact hóa Stone-Čech" thu được bằng cách hoàn thành $E$ đối với cấu trúc đều thô nhất sao cho mọi ánh xạ liên tục từ $E$ vào khoảng $[0,\ 1]$ của $\mathbf{R}$ đều liên tục đều (*Tôpô đại cương*, Chương IX, § 1, Bài tập 7); ánh xạ $\varphi_E$ là đơn ánh, vì bất kỳ

hai điểm phân biệt của E đều có thể được tách bởi một ánh xạ liên tục từ E vào $[0, 1]$.

VII. *Nhóm tôpô tự do*. Cho E là một không gian hoàn toàn chính quy, cho $\Sigma$ là loài các cấu trúc nhóm tôpô Hausdorff, các cấu xạ là các đồng cấu liên tục; và lấy các $\alpha$-ánh xạ là các ánh xạ liên tục của E vào một nhóm tôpô Hausdorff. Các điều kiện $(\mathrm{QM_{II}})$ và $(\mathrm{CU_I})$ đến $(\mathrm{CU_{III}})$ được kiểm tra dễ dàng, với

$$\mathfrak{a} = \mathrm{Card\ (E)\ Card\ (\mathbf{N})}.$$

Nhóm tôpô Hausdorff $\mathrm{F_E}$ là nghiệm của bài toán ánh xạ phổ quát này đối với E được gọi là *nhóm tôpô tự do sinh bởi không gian* E. Vì hai điểm phân biệt bất kỳ của E đều có thể được tách ra bởi một ánh xạ liên tục của E vào nhóm tôpô Hausdorff **R**, nên ánh xạ $\varphi_\mathrm{E}$ là đơn ánh; có thể chứng minh rằng $\varphi_\mathrm{E}$ là một đồng phôi của E lên không gian con $\varphi_\mathrm{E}(\mathrm{E})$ của $\mathrm{F_E}$ [^1]. Thay vì lấy $\Sigma$ là loài các cấu trúc nhóm tôpô Hausdorff, ta cũng có thể lấy các loài cấu trúc khác, chẳng hạn như các cấu trúc nhóm tôpô Hausdorff Abel, nhóm compact, vành tôpô Hausdorff, không gian vectơ tôpô Hausdorff (trên một vành phép chia tôpô, được xét như một tập hợp cơ sở phụ trợ), v.v.

VIII. *Các hàm hầu tuần hoàn trên một nhóm tôpô*. Cho E là một nhóm tôpô. Lấy $\Sigma$ là loài các cấu trúc nhóm compact, các cấu xạ là các đồng cấu liên tục, và các $\alpha$-ánh xạ là các đồng cấu liên tục từ E vào một nhóm compact. Các điều kiện $(\mathrm{QM_{II}})$, $(\mathrm{CU_I})$ đến $(\mathrm{CU_{III}})$ được thỏa mãn, với $\mathfrak{a} = 2^{2^{\mathrm{Card\,(E)}}}$. Nhóm compact $\mathrm{F_E}$ là nghiệm của bài toán ánh xạ phổ quát này đối với E được gọi là *nhóm compact liên kết* với E; ánh xạ $\varphi_\mathrm{E}$ không tất yếu đơn ánh. Mọi hàm thực liên tục trên E, có dạng $g \circ \varphi_\mathrm{E}$, trong đó $g$ là một hàm thực liên tục trên E, được gọi là một *hàm hầu tuần hoàn* trên E.

IX. *Đa tạp Albanese*. Cho E là một đa tạp đại số, và lấy $\Sigma$ là loài các cấu trúc của các đa tạp Abel trên cùng trường cơ sở với E (một đa tạp Abel là một đa tạp đại số đầy đủ được trang bị một cấu trúc nhóm đại số; nó tất yếu giao hoán). Các cấu xạ là các ánh xạ hữu tỉ từ một đa tạp Abel vào một đa tạp Abel khác (mỗi cấu xạ tất yếu là hợp thành của một đồng cấu và một phép tịnh tiến). Các $\alpha$-ánh xạ là các ánh xạ hữu tỉ từ E vào một đa tạp Abel. Điều kiện $(\mathrm{CU_I})$ không được thỏa mãn, tuy vậy bài toán ánh xạ phổ quát này đối với E vẫn có một nghiệm $\mathrm{F_E}$, được gọi là *đa tạp Albanese* của E. Nói chung, ánh xạ hữu tỉ $\varphi_\mathrm{E}$ không đơn ánh. ✳

### Bài tập {#ens-iv-s3-exercises}

Xem [các bài tập của § 3](exercises/s3/).

[^1]: Xem P. SAMUEL, "Về các ánh xạ phổ quát và các nhóm tôpô tự do", *Bull. Amer. Math. Soc.*, **54** (1948), pp. 591-598.
