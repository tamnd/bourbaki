---
book: ens
book_title: Theory of Sets
chapter: IV
chapter_title: STRUCTURES
section: 2
section_title: Morphisms and derived structures
lang: vi
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 271-283, 290-294
pdf_pages: 0276-0288, 0295-0299
extraction: ocr
subsections:
    - "no": 1
      title: MORPHISMS
      page: 271
      pdf_page: 276
    - "no": 2
      title: FINER STRUCTURES
      page: 273
      pdf_page: 278
    - "no": 3
      title: INITIAL STRUCTURES
      page: 274
      pdf_page: 279
    - "no": 4
      title: EXAMPLES OF INITIAL STRUCTURES
      page: 276
      pdf_page: 281
    - "no": 5
      title: FINAL STRUCTURES
      page: 280
      pdf_page: 285
    - "no": 6
      title: EXAMPLES OF FINAL STRUCTURES
      page: 281
      pdf_page: 286
statements: 12
exercises: 11
content_sha256: 38ab0c155c939c82f50b44d670c0b5ad1ab07d60e31858e124c0b5a315ef3675
translated_from: content/en/ens/IV/02_s2_morphisms_and_derived_structures.md
source_content_sha256: f3deeaa7f667542d82042b94967bb4d68d106fa3b1b0bdd6f7b4555f277bea62
translation_model: gpt-5-6-mini, gpt-5.4, gpt-5.4-mini, gpt-5-mini, gpt-5-6
translation_run: translate-vi-10c66441
glossary_version: 34
glossary_terms_sha256: f348b3bda3c3fd38fb2e806d1241ce9b7d0a293b1564809824de7ef754581cfe
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 2. CÁC CẤU XẠ VÀ CÁC CẤU TRÚC DẪN XUẤT

### 1. CÁC CẤU XẠ

Trong tiết này và tiết sau, để đơn giản hóa, ta sẽ giả thiết rằng loài cấu trúc đang xét chỉ có một tập hợp cơ sở (do đó là một tập hợp cơ sở chính). Người đọc sẽ không gặp khó khăn gì trong việc mở rộng các định nghĩa và kết quả cho trường hợp tổng quát.

Cho $\Sigma$ là một loài cấu trúc trong một lý thuyết $\mathscr{T}$ mạnh hơn lý thuyết tập hợp, và cho $x$, $y$, $s$, $t$ là bốn chữ cái phân biệt từng đôi một và khác với các hằng của $\mathscr{T}$. Ta nhắc lại rằng ký hiệu $\mathfrak{F}(x,y)$ biểu thị tập hợp các ánh xạ từ $x$ vào $y$ (Chương II, § 5, no. 2). Giả sử ta được cho một số hạng $\sigma\{x,y,s,t\}$ trong $\mathscr{T}$ thỏa mãn các điều kiện sau :

$(\mathrm{MO}_{\mathrm{I}})$ *Quan hệ “$s$ là một cấu trúc thuộc loài $\Sigma$ trên $x$, và $t$ là một cấu trúc thuộc loài $\Sigma$ trên $y$” kéo theo, trong E, quan hệ $\sigma\{x,y,s,t\}\subset\mathfrak{F}(x,y)$.*

$(\mathrm{MO}_{\mathrm{II}})$ *Nếu, trong một lý thuyết $\mathscr{T}'$ mạnh hơn $\mathscr{T}$, ta có ba tập hợp E, E′, E″ được trang bị tương ứng các cấu trúc $\mathscr{S}$, $\mathscr{S}'$, $\mathscr{S}''$ thuộc loài $\Sigma$, thì các quan hệ $f\in\sigma\{E,E',\mathscr{S},\mathscr{S}'\}$ và $g\in\sigma\{E',E'',\mathscr{S}',\mathscr{S}''\}$ kéo theo quan hệ*

$$
g\circ f\in\sigma\{E,E'',\mathscr{S},\mathscr{S}''\}.
$$

$(\mathrm{MO}_{\mathrm{III}})$ *Nếu, trong một lý thuyết $\mathscr{T}'$ mạnh hơn $\mathscr{T}$, ta có hai tập hợp E, E′ được trang bị tương ứng các cấu trúc $\mathscr{S}$, $\mathscr{S}'$ thuộc loài $\Sigma$, thì một song ánh $f$ từ E lên E′ là một đẳng cấu khi và chỉ khi $f\in\sigma\{E,E',\mathscr{S},\mathscr{S}'\}$ và $f^{-1}\in\sigma\{E',E,\mathscr{S}',\mathscr{S}\}$.*

Nếu $\Sigma$ và $\sigma$ được cho, quan hệ $f\in\sigma\{x,y,s,t\}$ được diễn đạt bằng cách nói rằng $f$ là một *cấu xạ* (hay một $\sigma$-*cấu xạ*) của $x$, được trang bị $s$, vào $y$, được trang bị $t$. Nếu (trong một lý thuyết $\mathscr{T}'$ mạnh hơn $\mathscr{T}$) E và E′ là hai tập hợp được trang bị các cấu trúc $\mathscr{S},\mathscr{S}'$ thuộc loài $\Sigma$, thì số hạng $\sigma\{E,E',\mathscr{S},\mathscr{S}'\}$ là *tập hợp các $\sigma$-cấu xạ từ E vào E′.*

*Ví dụ*

#### Ví dụ 1 {#ens-iv-s2-n1-exa-1 .statement tag=03VL}

Lấy $\Sigma$ là loài các cấu trúc thứ tự và cho $\sigma\{x,y,s,t\}$ ký hiệu tập hợp mọi ánh xạ $f$ của $x$ vào $y$ sao cho quan hệ $(u,v)\in s$ kéo theo $(f(u),f(v))\in t$. Theo ký hiệu của Chương III, § 1, điều này có nghĩa là $u \leqslant v$ kéo theo $f(u) \leqslant f(v)$, tức là $f$ là *tăng*. Việc kiểm tra các tiên đề $(\mathrm{MO_I})$, $(\mathrm{MO_{II}})$, và $(\mathrm{MO_{III}})$ là hiển nhiên.

#### Ví dụ 2 {#ens-iv-s2-n1-exa-2 .statement tag=03VM}

Lấy $\Sigma$ là một loài cấu trúc đại số chỉ có một luật hợp thành (trong) duy nhất, xác định khắp nơi (§1, no. 4, Example 2). Cho A, A$'$ là hai tập hợp được trang bị các cấu trúc thuộc loài $\Sigma$, và cho $p$, $p'$ là các luật hợp thành của hai cấu trúc đó. Xét các ánh xạ $f$ của A vào A$'$ sao cho $p'(f(x), f(y)) = f(p(x,\ y))$ với mọi $x \in \mathrm{A}$ và mọi $y \in \mathrm{A}$. Các ánh xạ này thỏa mãn $(\mathrm{MO_I})$, $(\mathrm{MO_{II}})$, và $(\mathrm{MO_{III}})$, và được gọi là các *đồng cấu* của A vào A$'$.

#### Ví dụ 3 {#ens-iv-s2-n1-exa-3 .statement tag=03VN}

Lấy $\Sigma$ là loài các cấu trúc tôpô (§1, no. 4, Example 3). Cho A, A$'$ là hai tập hợp được trang bị các tôpô V, V$'$, tương ứng. Xét các ánh xạ $f$ của A vào A$'$ sao cho quan hệ $\mathrm{X}' \in \mathrm{V}'$ kéo theo $\overset{-1}{f}(\mathrm{X}') \in \mathrm{V}$ (nói cách khác, sao cho ảnh ngược của mọi tập mở trong tôpô V$'$ là một tập mở trong tôpô V). Các ánh xạ này, thỏa mãn $(\mathrm{MO_I})$, $(\mathrm{MO_{II}})$, và $(\mathrm{MO_{III}})$, là các ánh xạ *liên tục* của A vào A$'$ (đối với các tôpô V và V$'$) (x. *General Topology*, Chương I, § 2).

#### Nhận xét {#ens-iv-s2-n1-rem-1 .statement tag=03VO}

Đối với một loài cấu trúc $\Sigma$ đã cho, có thể cần phải định nghĩa nhiều hạng thức khác nhau $\sigma \} x,\ y,\ s,\ t \{$ thỏa mãn các điều kiện $(\mathrm{MO_I})$, $(\mathrm{MO_{II}})$, và $(\mathrm{MO_{III}})$. Chẳng hạn, nếu $\Sigma$ là loài các cấu trúc tôpô, với ký hiệu của Ví dụ 3 ở trên, một ánh xạ $f$ của A vào A$'$ được gọi là *mở* nếu quan hệ $\mathrm{X} \in \mathrm{V}$ kéo theo $f(\mathrm{X}) \in \mathrm{V}'$ (nói cách khác, nếu ảnh qua $f$ của mọi tập mở là một tập mở). Dễ kiểm tra rằng các ánh xạ mở cũng thỏa mãn các điều kiện $(\mathrm{MO_I})$, $(\mathrm{MO_{II}})$, và $(\mathrm{MO_{III}})$ đối với loài $\Sigma$. \* Hơn nữa, có thể chỉ ra rằng một ánh xạ liên tục không nhất thiết là mở, và một ánh xạ mở không nhất thiết là liên tục. \* Do đó, một loài cấu trúc đã cho *không kéo theo* một khái niệm cấu xạ được xác định rõ.

☡

Khi nói đến các cấu trúc thứ tự, các cấu trúc đại số, và các cấu trúc tôpô, luôn luôn phải hiểu rằng các cấu xạ là những cấu xạ đã được định nghĩa trong các Ví dụ trên, trừ khi có nói rõ điều ngược lại.

Điều kiện $(\mathrm{MO_{III}})$ và đặc trưng hóa của các song ánh (Chương II, § 3, no. 8, Hệ quả của Mệnh đề 8) kéo theo tiêu chuẩn sau :

CST8. *Cho* E, E$'$ *là hai tập hợp, mỗi tập hợp được trang bị một cấu trúc thuộc loài cấu trúc $\Sigma$. Cho $f$ là một $\sigma$-cấu xạ của* E *vào* E$'$ *và cho $g$ là một $\sigma$-cấu xạ của* E$'$ *vào* E. *Nếu $g \circ f$ là ánh xạ đồng nhất của* E *lên chính nó, và nếu $f \circ g$ là ánh xạ đồng nhất của* E$'$ *lên chính nó, thì $f$ là một đẳng cấu của* E *lên* E$'$, *và $g$ là đẳng cấu nghịch đảo.*

Cần lưu ý rằng một song ánh của E lên E$'$ có thể là một $\sigma$-cấu xạ mà song ánh ngược không nhất thiết là một $\sigma$-cấu xạ. \* Chẳng hạn, một ánh xạ song ánh của một không gian tôpô A lên một không gian tôpô A$'$ có thể liên tục mà song ánh ngược không liên tục (*General Topology*, Chapter I, § 2, no. 1, Nhận xét 1). \*

☡

#### Nhận xét {#ens-iv-s2-n1-rem-2 .statement tag=03VP}

Khi một loài cấu trúc $\Sigma$ có nhiều tập cơ sở chính $x_1, \ldots, x_n$ và các tập cơ sở phụ trợ $\mathrm{A}_1, \ldots, \mathrm{A}_m$, thì một $\sigma$-cấu xạ là một hệ $(f_1, \ldots, f_n)$, trong đó $f_i$ là một ánh xạ của $x_i$ vào $y_i$ $(1 \leqslant i \leqslant n)$, và các hệ ánh xạ này thỏa mãn các điều kiện tương tự như $(\mathrm{MO_{II}})$ và $(\mathrm{MO_{III}})$, mà người đọc có thể dễ dàng tự phát biểu.

### 2. CÁC CẤU TRÚC MỊN HƠN

Trong phần còn lại của tiết diện này, ta sẽ giả sử rằng đã cho một loài cấu trúc $\Sigma$ và một khái niệm về $\sigma$-cấu xạ tương đối với loài cấu trúc này; *mọi khái niệm sẽ được đưa vào sẽ không những phụ thuộc vào $\Sigma$ mà còn phụ thuộc vào khái niệm về $\sigma$-cấu xạ đang xét.* Thông thường ta sẽ nói "cấu xạ" thay cho "$\sigma$-cấu xạ".

¶ Cho E là một tập hợp và cho $\mathscr{S}_1$, $\mathscr{S}_2$ là hai cấu trúc thuộc loài cấu trúc $\Sigma$ trên E. Cấu trúc $\mathscr{S}_1$ được gọi là *mịn hơn* $\mathscr{S}_2$ (và $\mathscr{S}_2$ *thô hơn* $\mathscr{S}_1$) nếu ánh xạ đồng nhất của E, được trang bị $\mathscr{S}_1$, lên E, được trang bị $\mathscr{S}_2$, là một cấu xạ.

Khi cần để tránh mơ hồ, ta sẽ nói rằng $\mathscr{S}_1$ mịn hơn $\mathscr{S}_2$ *tương đối với khái niệm về $\sigma$-cấu xạ đang xét*; và tương tự đối với mọi khái niệm khác sẽ được định nghĩa trong tiết diện này.

Giả sử rằng $\mathscr{S}_1$ mịn hơn $\mathscr{S}_2$. Nếu E$'$ là một tập hợp được trang bị một cấu trúc $\mathscr{S}'$ thuộc loài $\Sigma$, và nếu $f$ là một cấu xạ của E, được trang bị $\mathscr{S}_2$, vào E$'$, được trang bị $\mathscr{S}'$, thì $f$ cũng là một cấu xạ của E, được trang bị $\mathscr{S}_1$, vào E$'$, được trang bị $\mathscr{S}'$; điều này suy ra từ định nghĩa trước và từ $(\mathrm{MO_{II}})$. Tương tự, nếu $g$ là một cấu xạ của E$'$, được trang bị $\mathscr{S}'$, vào E, được trang bị $\mathscr{S}_1$, thì $g$ cũng là một cấu xạ của E$'$, được trang bị $\mathscr{S}'$, vào E, được trang bị $\mathscr{S}_2$.

Vì thế, cấu trúc (thuộc loài $\Sigma$) trên E càng *mịn hơn* thì càng có *nhiều* cấu xạ với E làm nguồn, và càng có *ít* cấu xạ với E làm đích.

Quan hệ "$\mathscr{S}_1$ thô hơn $\mathscr{S}_2$" là một *quan hệ thứ tự* giữa $\mathscr{S}_1$ và $\mathscr{S}_2$ trên tập hợp tất cả các cấu trúc thuộc loài $\Sigma$ trên E; vì nó phản xạ theo $(\mathrm{MO_{III}})$, bắc cầu theo $(\mathrm{MO_{II}})$, và nếu một cấu trúc thuộc loài $\Sigma$ vừa mịn hơn vừa thô hơn một cấu trúc khác, thì hai cấu trúc ấy trùng nhau theo $(\mathrm{MO_{III}})$. Phù hợp với các định nghĩa chung (Chương III, § 1, no. 14), hai cấu trúc thuộc loài $\Sigma$ trên E được gọi là *so sánh được* nếu một cấu trúc mịn hơn cấu trúc kia; một cấu trúc được gọi là *mịn hơn hẳn* (tương ứng *thô hơn hẳn*) một cấu trúc khác nếu nó *mịn hơn* (tương ứng *thô hơn*) cấu trúc kia và khác với nó.

*Ví dụ*

#### Ví dụ 1 {#ens-iv-s2-n2-exa-1 .statement tag=03VQ}

Một cấu trúc thứ tự với đồ thị $s$ trên một tập A mịn hơn một cấu trúc thứ tự với đồ thị $s'$ khi và chỉ khi $s \subset s'$. Nói cách khác, quan hệ $x \leqslant y$ đối với $s$ suy ra quan hệ $x \leqslant y$ đối với $s'$; điều này phù hợp với định nghĩa đã cho trong Chương III, § 1, no. 4, Ví dụ 3.

#### Ví dụ 2 {#ens-iv-s2-n2-exa-2 .statement tag=03VR}

Xét hai cấu trúc đại số F, F' cùng loài $\Sigma$ trên một tập A, trong đó F và F' là các đồ thị của các phép hợp thành (được xác định khắp nơi) của hai cấu trúc này. Từ định nghĩa về các cấu xạ trong trường hợp này (no. 1, Ví dụ 2), F mịn hơn F' khi và chỉ khi $F \subset F'$. Nhưng vì F và F' đều là các đồ thị phiếm hàm với cùng miền xác định $A \times A$, ta phải có $F = F'$. Nói cách khác, hai *so sánh được* cấu trúc thuộc loài $\Sigma$ tất yếu là *trùng nhau*.

#### Ví dụ 3 {#ens-iv-s2-n2-exa-3 .statement tag=03VS}

Cho V, V' là hai tôpô trên cùng một tập A. Nói rằng V mịn hơn V' nghĩa là, theo định nghĩa về các cấu xạ trong trường hợp này (no. 1, Ví dụ 3), rằng $V' \subset V$; nói cách khác, mọi tập con của A là một tập mở trong tôpô V' cũng là một tập mở trong tôpô V (và do đó, tôpô càng mịn hơn thì càng có nhiều tập mở).

#### Nhận xét {#ens-iv-s2-n2-rem-1 .statement tag=03VT}

Ta vừa gặp một ví dụ (Ví dụ 2) trong đó hai cấu trúc so sánh được cùng loài $\Sigma$ tất yếu trùng nhau. Có nhiều ví dụ tương tự khác: cấu trúc thứ tự tuyến tính, \* tôpô compact, cấu trúc không gian Fréchet (các cấu xạ là các ánh xạ tuyến tính liên tục), các tôpô được xác định bởi một giá trị tuyệt đối (hoặc một định giá) trên một vành chia, v.v. \*

Đối với một loài cấu trúc $\Sigma$ như vậy, một cấu xạ $f$ của E vào E' mà *song ánh* là một *đẳng cấu*; vì nếu ta chuyển sang E' cấu trúc $\mathscr{S}$ trên E bằng $f$, ta thu được một cấu trúc thuộc loài $\Sigma$ mịn hơn cấu trúc $\mathscr{S}'$ trên E' và do đó trùng với $\mathscr{S}'$.

### 3. CẤU TRÚC BAN ĐẦU

Xét một họ $(A_\iota)_{\iota \in I}$ các tập hợp, mỗi tập hợp trong đó được trang bị một cấu trúc $\mathscr{S}_\iota$ thuộc loài $\Sigma$. Cho E là một tập hợp, và với mỗi $\iota \in I$ cho $f_\iota$ là một ánh xạ *của* E *vào* $A_\iota$. Một cấu trúc $\mathscr{S}$ thuộc loài $\Sigma$ trên E được gọi là một *cấu trúc ban đầu đối với họ* $(A_\iota, \mathscr{S}_\iota, f_\iota)_{\iota \in I}$ nếu nó có tính chất sau :

(IN) Với mọi tập hợp E', mọi cấu trúc thuộc loài $\mathscr{S}'$ trên E', và mọi ánh xạ $g$ *của* E' *vào* E, quan hệ

"$g$ là một cấu xạ của E' vào E"

là *tương đương* với quan hệ

"với mỗi $\iota \in I, f_\iota \circ g$ là một cấu xạ của E' vào $A_\iota$".

CST9. *Nếu tồn tại một cấu trúc ban đầu trên* E *đối với họ* $(\mathrm{A}_\iota,\ \mathscr{S}_\iota,\ f_\iota)_{\iota \in \mathrm{I}}$, *thì nó là cấu trúc thô nhất trong tất cả các cấu trúc thuộc loài* $\Sigma$ *trên* E *mà mỗi ánh xạ* $f_\iota$ *là một cấu xạ, và do đó là duy nhất.*

Cho $\mathscr{I}$ là một cấu trúc ban đầu trên E, và cho $\mathscr{S}$ là một cấu trúc thuộc loài $\Sigma$ trên E sao cho mỗi $f_\iota$ là một cấu xạ. Nếu $i$ ký hiệu ánh xạ đồng nhất của E, được trang bị với $\mathscr{S}$, vào E, được trang bị với $\mathscr{I}$, thì $f_\iota \circ i$ là một cấu xạ với mọi $\iota \in \mathrm{I}$, và điều kiện (IN) chỉ ra rằng $i$ là một cấu xạ, điều này có nghĩa (no. 2) rằng $\mathscr{S}$ *mịn hơn* $\mathscr{I}$. Mặt khác, áp dụng (IN) vào trường hợp trong đó $g$ là ánh xạ đồng nhất của E (được trang bị với $\mathscr{I}$) lên chính nó, ta thấy (theo $(\mathrm{MO_{III}})$) rằng mỗi $f_\iota$ là một cấu xạ của E vào $\mathrm{A}_\iota$, điều này hoàn thành chứng minh.

Có thể xảy ra rằng tồn tại một cấu trúc thuộc loài $\Sigma$ trên E là thô nhất trong tất cả các cấu trúc thuộc loài $\Sigma$ mà các $f_\iota$ là các cấu xạ, nhưng cấu trúc này không phải là cấu trúc ban đầu đối với $(\mathrm{A}_\iota, \mathscr{S}_\iota, f_\iota)$ (Bài tập 6).

Ta có tiêu chuẩn *tính bắc cầu* sau :

CST10. *Cho* E *là một tập hợp, cho* $(\mathrm{A}_\iota)_{\iota \in \mathrm{I}}$ *là một họ các tập hợp, và với mỗi* $\iota \in \mathrm{I}$ *cho* $\mathscr{S}_\iota$ *là một cấu trúc thuộc loài* $\Sigma$ *trên* $\mathrm{A}_\iota$. *Cho* $(\mathrm{J}_\lambda)_{\lambda \in \mathrm{L}}$ *là một phân hoạch của* I, *và cho* $(\mathrm{B}_\lambda)_{\lambda \in \mathrm{L}}$ *là một họ các tập hợp được đánh chỉ số bởi* L. *Với mỗi* $\lambda \in \mathrm{L}$ *cho* $h_\lambda$ *là một ánh xạ của* E *vào* $\mathrm{B}_\lambda$, *và với mỗi* $\lambda \in \mathrm{L}$ *và mỗi* $\iota \in \mathrm{J}_\lambda$ *cho* $g_{\lambda\iota}$ *là một ánh xạ của* $\mathrm{B}_\lambda$ *vào* $\mathrm{A}_\iota$, *và cho* $f_\iota = g_{\lambda\iota} \circ h_\lambda$. *Giả sử rằng, với mỗi* $\lambda \in \mathrm{L}$, *tồn tại một cấu trúc ban đầu* $\mathscr{S}'_\lambda$ *trên* $\mathrm{B}_\lambda$ *đối với họ* $(\mathrm{A}_\iota, \mathscr{S}_\iota, g_{\lambda\iota})_{\iota \in \mathrm{J}_\lambda}$. *Khi đó các mệnh đề sau là tương đương* :

(a) *tồn tại một cấu trúc ban đầu* $\mathscr{I}$ *trên* E *đối với họ* $(\mathrm{A}_\iota, \mathscr{S}_\iota, f_\iota)_{\iota \in \mathrm{I}}$;

(b) *tồn tại một cấu trúc ban đầu* $\mathscr{I}'$ *trên* E *đối với họ* $(\mathrm{B}_\lambda, \mathscr{S}'_\lambda, h_\lambda)_{\lambda \in \mathrm{L}}$.

*Hơn nữa, các mệnh đề này kéo theo* $\mathscr{I} = \mathscr{I}'$.

Cho F là một tập hợp được trang bị một cấu trúc thuộc loài $\Sigma$, và cho $u$ là một ánh xạ từ F vào E. Hãy nhận thấy rằng theo định nghĩa, quan hệ "$h_\lambda \circ u$ là một cấu xạ từ F vào $\mathrm{B}_\lambda$" là tương đương với quan hệ "với mọi $\iota \in \mathrm{J}_\lambda$, $g_{\lambda\iota} \circ h_\lambda \circ u = f_\iota \circ u$ là một cấu xạ từ F vào $\mathrm{A}_\iota$". Do đó, quan hệ

(1)     "với mọi $\lambda \in \mathrm{L}$, $h_\lambda \circ u$ là một cấu xạ từ F vào $\mathrm{B}_\lambda$"

là tương đương với quan hệ

(2)     "với mọi $\iota \in \mathrm{I}$, $f_\iota \circ u$ là một cấu xạ từ F vào $\mathrm{A}_\iota$".

Bây giờ, nói rằng $\mathscr{I}'$ là cấu trúc ban đầu đối với họ $(\mathrm{B}_\lambda, \mathscr{S}'_\lambda, h_\lambda)_{\lambda \in \mathrm{L}}$ có nghĩa là quan hệ (1) tương đương với quan hệ "$u$ là một cấu xạ từ F vào E được trang bị $\mathscr{I}'$"; và nói rằng $\mathscr{I}$ là cấu trúc ban đầu đối với họ $(A_i,\,\mathscr{G}_i,\,f_i)_{i\in I}$ có nghĩa là quan hệ (2) tương đương với quan hệ “$u$ là một cấu xạ từ F vào E được trang bị $\Gamma$”. Do đó suy ra kết quả, theo tính chất duy nhất của cấu trúc ban đầu.

### 4. CÁC VÍ DỤ VỀ CẤU TRÚC BAN ĐẦU

I. *Ảnh ngược của một cấu trúc.* Khi I là một tập hợp gồm một phần tử duy nhất, cấu trúc ban đầu đối với $(A,\,\mathscr{G},\,f)$ được gọi là *ảnh ngược theo $f$ của cấu trúc $\mathscr{G}$* (khi nó tồn tại).

\* Một tôpô luôn luôn có ảnh ngược theo bất kỳ ánh xạ nào $f$; nhưng điều này không đúng đối với một cấu trúc thứ tự hoặc một cấu trúc đại số. \*

II. *Cấu trúc cảm sinh.* Cho A là một tập hợp được trang bị một cấu trúc $\mathscr{G}$ thuộc loài $\Sigma$, cho B là một tập con của A, và cho $j$ là đơn ánh chính tắc từ B vào A. Khi đó ảnh ngược theo $j$ của cấu trúc B (nếu nó tồn tại) được gọi là *cấu trúc do $\mathscr{G}$ cảm sinh trên B.*

Một cấu trúc thứ tự cảm sinh một cấu trúc cùng loài trên mọi tập con của tập hợp mà trên đó nó được xác định; nhưng điều này không đúng đối với cấu trúc của một tập có hướng. \* Một tôpô cảm sinh một tôpô trên mọi tập con của tập hợp mà trên đó nó được xác định, nhưng một tôpô compắc nói chung không cảm sinh một tôpô compắc. Một cấu trúc đại số trên một tập hợp A nói chung không cảm sinh một cấu trúc cùng loài trên một tập con tùy ý B; nếu cấu trúc đã cho trên A gồm các luật hợp thành được xác định khắp nơi, thì điều cần thiết là B phải ổn định đối với mỗi luật trong các luật ấy, nhưng điều kiện cần này không phải lúc nào cũng đủ. \*

Tiêu chuẩn tổng quát CST10 cho ta *tiêu chuẩn bắc cầu* sau đây đối với các cấu trúc cảm sinh:

CST11. *Cho B là một tập con của A, cho C là một tập con của B, và cho $\mathscr{G}$ là một cấu trúc thuộc loài $\Sigma$ trên A, cấu trúc này cảm sinh một cấu trúc $\mathscr{G}'$ cùng loài trên B. Khi đó $\mathscr{G}$ cảm sinh một cấu trúc thuộc loài $\Sigma$ trên C khi và chỉ khi $\mathscr{G}'$ cảm sinh một cấu trúc thuộc loài $\Sigma$ trên C, và khi ấy các cấu trúc do $\mathscr{G}$ và $\mathscr{G}'$ cảm sinh trên C là đồng nhất.*

CST12. *Cho A, A' là hai tập hợp được trang bị các cấu trúc $\mathscr{G}$, $\mathscr{G}'$ thuộc loài $\Sigma$. Cho B là một tập con của A, và B' là một tập con của A'. Giả sử rằng $\mathscr{G}$ (tương ứng $\mathscr{G}'$) cảm sinh một cấu trúc thuộc loài $\Sigma$ trên B (tương ứng B'). Nếu $f$ là một cấu xạ từ A vào A' sao cho $f(B)\subset B'$, thì ánh xạ từ B vào B' trùng với $f$ trên B là một cấu xạ (đối với các cấu trúc do $\mathscr{G}$ và $\mathscr{G}'$ cảm sinh).*

Cho $j$ (resp. $j'$) là đơn ánh chính tắc của B (resp. B') vào A (resp. A'). Theo định nghĩa ta có $f\circ j=j'\circ g$. Vì $f$ và $j$ là các cấu xạ, nên $f\circ j$ cũng vậy theo (MO$_{\mathrm{II}}$); nhưng khi đó, vì $j'\circ g$ là một cấu xạ, nên ánh xạ $g$ là một cấu xạ theo định nghĩa của cấu trúc ban đầu.

III. *Cấu trúc tích.* Cho $(A_i)_{i\in I}$ là một họ các tập hợp, và trên mỗi tập hợp $A_i$ cho $\mathscr{S}_i$ là một cấu trúc thuộc loài $\Sigma$. Cho $E=\prod_{i\in I}A_i$ là *tích* của họ $(A_i)_{i\in I}$ (Chương II, § 5), và ký hiệu $\operatorname{pr}_i$ là phép chiếu của $E$ lên $A_i$. Cấu trúc ban đầu (nếu tồn tại) đối với họ $(A_i,\mathscr{S}_i,\operatorname{pr}_i)_{i\in I}$ được gọi là *tích* của các cấu trúc $\mathscr{S}_i$.

\* Một họ các cấu trúc thứ tự luôn luôn thừa nhận một cấu trúc tích, nhưng điều tương tự không phải lúc nào cũng đúng đối với một họ các cấu trúc thứ tự toàn phần. Một họ các cấu trúc nhóm luôn luôn thừa nhận một cấu trúc tích, nhưng điều tương tự không nhất thiết đúng đối với một họ các cấu trúc vành chia. Một họ các tôpô luôn luôn thừa nhận một cấu trúc tích, nhưng điều này không phải lúc nào cũng đúng đối với một họ các cấu trúc không gian compact địa phương; trong trường hợp này, có một cấu trúc tích cùng loài nếu họ là *hữu hạn*, nhưng có thể không có nếu họ là *vô hạn* (xem *Topologie générale*, Chương I, § 9, no. 7, Mệnh đề 14). \*

Tiêu chuẩn CST10 dẫn đến *tiêu chuẩn kết hợp* sau đây đối với các cấu trúc tích :

CST13. *Cho $(A_i)_{i\in I}$ là một họ các tập hợp, và với mỗi chỉ số $i\in I$ cho $\mathscr{S}_i$ là một cấu trúc thuộc loài $\Sigma$ trên $A_i$. Cho $(J_\lambda)_{\lambda\in L}$ là một phân hoạch của $I$. Giả sử rằng trên mỗi tích bộ phận $B_\lambda=\prod_{i\in J_\lambda}A_i$, họ $(\mathscr{S}_i)_{i\in J_\lambda}$ thừa nhận một cấu trúc tích $\mathscr{S}'_\lambda$. Khi đó họ $(\mathscr{S}_i)_{i\in I}$ thừa nhận một cấu trúc tích $\mathscr{S}$ khi và chỉ khi họ $(\mathscr{S}'_\lambda)_{\lambda\in L}$ thừa nhận một cấu trúc tích $\mathscr{S}'$, và ánh xạ chính tắc từ $E=\prod_{i\in I}A_i$, được trang bị $\mathscr{S}$, lên $F=\prod_{\lambda\in L}B_\lambda$, được trang bị $\mathscr{S}'$ (Chương II, § 5, no. 5), khi đó là một đẳng cấu.*

Một ứng dụng khác của CST10 cho tiêu chuẩn sau đây liên quan đến các cấu trúc cảm sinh bởi một cấu trúc tích :

CST14. *Cho $(A_i)_{i\in I}$ là một họ các tập hợp, và với mỗi $i\in I$ cho $\mathscr{S}_i$ là một cấu trúc thuộc loài $\Sigma$ trên $A_i$. Với mỗi $i\in I$, cho $B_i$ là một tập con của $A_i$. Giả sử rằng mỗi $\mathscr{S}_i$ cảm sinh một cấu trúc $\mathscr{S}'_i$ trên $B_i$, và rằng trên tích $E=\prod_{i\in I}A_i$ tồn tại một cấu trúc $\mathscr{S}_0$ là tích của họ $(\mathscr{S}_i)$. Khi đó các mệnh đề sau là tương đương :*

(a) trên tập hợp $B=\prod_{i\in I}B_i\subset E$ tồn tại một cấu trúc $\mathscr{S}$ cảm sinh bởi $\mathscr{S}_0$;

(b) trên tập hợp $B$ tồn tại một cấu trúc $\mathscr{S}'$ là tích của họ các cấu trúc $(\mathscr{S}'_i)$.

*Hơn nữa, các mệnh đề này kéo theo $\mathscr{S}=\mathscr{S}'$.*

Cho $j_\iota$ là đơn ánh chính tắc của $\mathrm{B}_\iota$ vào $\mathrm{A}_\iota$, cho $j$ là đơn ánh chính tắc của B vào E, cho $p_\iota$ là phép chiếu của E lên $\mathrm{A}_\iota$, và cho $p'_\iota$ là phép chiếu của B lên $\mathrm{B}_\iota$. Khi đó ta có $p_\iota \circ j = j_\iota \circ p'_\iota$ với mọi $\iota \in \mathrm{I}$. Theo CST10, $\mathscr{S}$ là cấu trúc ban đầu đối với họ $(\mathrm{A}_\iota, \mathscr{S}_\iota, p_\iota \circ j)_{\iota \in \mathrm{I}}$, và $\mathscr{S}'$ là cấu trúc ban đầu đối với họ $(\mathrm{A}_\iota, \mathscr{S}_\iota, j_\iota \circ p'_\iota)_{\iota \in \mathrm{I}}$. Do đó có kết quả.

¶ Các khái niệm về ảnh ngược và tích liên quan với nhau bởi tiêu chuẩn sau đây :

CST15. *Cho $(\mathrm{A}_\iota)_{\iota \in \mathrm{I}}$ là một họ các tập hợp, và với mỗi $\iota \in \mathrm{I}$ cho $\mathscr{S}_\iota$ là một cấu trúc thuộc loài $\Sigma$ trên $\mathrm{A}_\iota$, và cho $f_\iota$ là một ánh xạ của một tập hợp E vào $\mathrm{A}_\iota$. Giả sử rằng trên tập hợp tích $\mathrm{A} = \prod_{\iota \in \mathrm{J}} \mathrm{A}_\iota$ tồn tại một cấu trúc tích $\mathscr{S}$ của họ $(\mathscr{S}_\iota)_{\iota \in \mathrm{I}}$. Khi đó tồn tại một cấu trúc ban đầu đối với họ $(\mathrm{A}_\iota, \mathscr{S}_\iota, f_\iota)_{\iota \in \mathrm{I}}$ khi và chỉ khi cấu trúc $\mathscr{S}$ có một ảnh ngược qua ánh xạ $x \to f(x) = (f_\iota(x))$ của E vào A, và khi đó hai cấu trúc này đồng nhất.*

Vì $f_\iota = \mathrm{pr}_\iota \circ f$, tiêu chuẩn này là một trường hợp riêng của CST10.

#### Nhận xét {#ens-iv-s2-n4-rem-1 .statement tag=03VU}

Cho $(\mathscr{S}_\lambda)_{\lambda \in \mathrm{L}}$ là một họ các cấu trúc thuộc loài $\Sigma$ trên cùng một tập hợp A; ký hiệu $\mathrm{A}_\lambda$ là tập hợp A được trang bị cấu trúc $\mathscr{S}_\lambda$, và ký hiệu $\mathrm{I}_\lambda$ là ánh xạ đồng nhất của A vào $\mathrm{A}_\lambda$. Cho B là tập hợp tích $\mathrm{A}^{\mathrm{L}} = \prod_{\lambda \in \mathrm{L}} \mathrm{A}_\lambda$, và cho $\Delta$ là đường chéo của tích này (Chương II, § 5, no. 3). Cho $h$ là ánh xạ đường chéo của A lên $\Delta$, sao cho $h(x)$ là phần tử $(x_\lambda)_{\lambda \in \mathrm{L}}$ thỏa mãn $x_\lambda = x$ với mọi $\lambda \in \mathrm{L}$. Giả sử rằng trên B tồn tại một cấu trúc tích $\mathscr{S}'$ của họ $(\mathscr{S}_\lambda)$. Vì $h$ là đơn ánh, tiêu chuẩn CST 15 chỉ ra rằng tồn tại một cấu trúc ban đầu $\mathscr{S}$ đối với họ $(\mathrm{A}_\lambda, \mathscr{S}_\lambda, \mathrm{I}_\lambda)_{\lambda \in \mathrm{L}}$ khi và chỉ khi tồn tại một cấu trúc $\mathscr{S}''$ trên $\Delta$ cảm sinh bởi $\mathscr{S}'$; khi đó $\mathscr{S}''$ đồng nhất với cấu trúc thu được bằng cách chuyển cấu trúc $\mathscr{S}$ sang $\Delta$ nhờ $h$. Đặc biệt, khi tất cả các cấu trúc $\mathscr{S}_\lambda$ đồng nhất, $h$ là một *đẳng cấu* của A (được trang bị cấu trúc này) lên $\Delta$.

Ta cũng có tiêu chuẩn sau đây :

CST16. *Cho $(\mathrm{A}_\iota)_{\iota \in \mathrm{I}}$, $(\mathrm{B}_\iota)_{\iota \in \mathrm{I}}$ là hai họ tập hợp được đánh chỉ số bởi cùng một tập hợp. Với mỗi $\iota \in \mathrm{I}$, cho $\mathscr{S}_\iota$ là một cấu trúc loài $\Sigma$ trên $\mathrm{A}_\iota$ và cho $\mathscr{S}'_\iota$ là một cấu trúc loài $\Sigma$ trên $\mathrm{B}_\iota$. Giả sử rằng tồn tại trên $\mathrm{A} = \prod_{\iota \in \mathrm{I}} \mathrm{A}_\iota \left( \text{resp. trên } \mathrm{B} = \prod_{\iota \in \mathrm{I}} \mathrm{B}_\iota \right)$ một cấu trúc tích $\mathscr{S}$ (resp. $\mathscr{S}'$) của họ $(\mathscr{S}_\iota)$ (resp. $(\mathscr{S}'_\iota)$). Với mỗi $\iota \in \mathrm{I}$, cho $f_\iota$ là một cấu xạ từ $\mathrm{A}_\iota$ vào $\mathrm{B}_\iota$. Khi đó ánh xạ $f = (f_\iota)_{\iota \in \mathrm{I}}$ là một cấu xạ từ A vào B.*

Cho $p_\iota$ (resp. $q_\iota$) là phép chiếu của A lên $\mathrm{A}_\iota$ (resp. của B lên $\mathrm{B}_\iota$). Khi đó ta có $q_\iota \circ f = f_\iota \circ p_\iota$. Vì $f_\iota$ và $p_\iota$ là các cấu xạ (tiêu chuẩn

CST9), $f_i \circ p_i$ là một cấu xạ theo (MO$_\Pi$); do đó $f$ là một cấu xạ theo (IN).

#### Nhận xét {#ens-iv-s2-n4-rem-2 .statement tag=03VV}

Đối với phần lớn các cấu trúc thông thường, điều kiện được cho trong CST16 không chỉ đủ mà còn cần thiết để $f$ là một cấu xạ (xem Bài tập 7). Đặc biệt, điều này đúng trong các trường hợp sau đây (xảy ra chẳng hạn nếu $\Sigma$ là loài của các cấu trúc thứ tự, \* hoặc loài của các cấu trúc nhóm, hoặc loài của các cấu trúc tôpô *, v.v.; xem Bài tập 8) :

☡

¶ Tồn tại một họ $(a_i)_{i\in I}$ sao cho $a_i\in A_i$ với mọi $i\in I$ và sao cho, nếu ta đặt $r_i(x)=(y_\lambda)$, trong đó $y_i=x_i$ và $y_\lambda=a_\lambda$ bất cứ khi nào $\lambda\ne i$, mỗi ánh xạ $r_i$ là một cấu xạ từ $A_i$ vào $A$. Thật vậy, nếu $f=(f_i)$ là một cấu xạ từ $A$ vào $B$, ta có thể viết $f_i=q_i\circ f\circ r_i$ với mọi $i\in I$, và chỉ cần áp dụng (MO$_\Pi$).

¶ Chú ý rằng $r_i$ là một cấu xạ nếu điều kiện sau được thỏa mãn :

(a) Với mọi tập hợp $E$ được trang bị một cấu trúc loài $\Sigma$, ánh xạ hằng $z\mapsto a_i$ là một cấu xạ từ $E$ vào $A_i$; cụ thể là, với mỗi $x\in I$, $p_x\circ r_i$ là một cấu xạ từ $A_i$ vào $A_x$, vì nó là ánh xạ đồng nhất khi $x=i$, và là ánh xạ hằng $z\mapsto a_x$ khi $x\ne i$; do định nghĩa cấu trúc tích, $r_i$ do đó là một cấu xạ từ $A_i$ vào $A$.

¶ Các ví dụ được liệt kê ở trên không chỉ thỏa mãn (a), mà còn thỏa mãn điều kiện sau:

(b) Trên mỗi tập hợp $A'_i=A_i\times\prod_{x\ne i}\{a_x\}$, cấu trúc $\mathscr{I}$ cảm sinh một cấu trúc loài $\Sigma$.

¶ Gọi $p'_i$ là hạn chế của $p_i$ trên $A'_i$. Nếu cả hai điều kiện (a) và (b) đều được thỏa mãn, thì $p'_i$ là một đẳng cấu từ $A'_i$ lên $A_i$. Thật vậy, vì $p'_i=p_i\circ j_i$, trong đó $j_i$ là đơn ánh chính tắc từ $A'_i$ vào $A$, nên $p'_i$ là một cấu xạ theo (MO$_\Pi$). Mặt khác, ta có $r_i=j_i\circ {p'_i}^{-1}$; do đó ${p'_i}^{-1}$ là một cấu xạ từ $A_i$ vào $A'_i$ theo định nghĩa cấu trúc cảm sinh.

Cuối cùng, ta có tiêu chuẩn sau đây, tiêu chuẩn này đặc trưng các cấu xạ trong nhiều trường hợp:

**CST17.** — Cho $A$ và $B$ là hai tập hợp, được trang bị các cấu trúc $\mathscr{S}_A$, $\mathscr{S}_B$ cùng loài $\Sigma$. Giả sử trên $A\times B$ tồn tại cấu trúc $\mathscr{S}_{A\times B}$, là tích của $\mathscr{S}_A$ và $\mathscr{S}_B$. Cho $f$ là một ánh xạ từ $A$ vào $B$, $F$ là đồ thị của nó, và $\pi$ là song ánh $x\mapsto (x,f(x))$ của $A$ lên $F$. Khi đó, để $f$ là một cấu xạ từ $A$ vào $B$, điều kiện cần và đủ là trên $F$ tồn tại một cấu trúc loài $\Sigma$ cảm sinh bởi $\mathscr{S}_{A\times B}$ và, khi $F$ được trang bị cấu trúc này, $\pi$ là một đẳng cấu của $A$ lên $F$.

Để chứng minh tính đủ, cho $j$ là đơn ánh chính tắc của $F$ vào $A\times B$. Ta có thể viết $f=\operatorname{pr}_2\circ j\circ\pi$, và khi đó theo giả thiết $f$ là hợp thành của ba cấu xạ.

¶ Để chứng minh tính cần, cho $\mathscr{S}_{\mathbf{F}}$ là cấu trúc loài $\Sigma$ thu được bằng cách chuyển cấu trúc $\mathscr{S}_{\mathbf{A}}$ lên F nhờ song ánh $\pi$ (§ 1, no. 5). Khi đó ta phải chứng minh rằng $\mathscr{S}_{\mathbf{F}}$ cảm sinh bởi $\mathscr{S}_{\mathbf{A} \times \mathbf{B}}$ trên F. Trước hết, ta nhận xét rằng $j$ là một cấu xạ từ F vào $\mathbf{A} \times \mathbf{B}$; vì $j \circ \pi$ là ánh xạ $x \to (x, f(x))$ từ A vào $\mathbf{A} \times \mathbf{B}$ và do đó là một cấu xạ theo giả thiết về $f$ và định nghĩa của cấu trúc tích; suy ra, theo định nghĩa của cấu trúc $\mathscr{S}_{\mathbf{F}}$, $j$ là một cấu xạ. Còn phải chứng minh rằng nếu E là một tập hợp được trang bị một cấu trúc loài $\Sigma$, và nếu $g$ là một ánh xạ từ E vào F sao cho $j \circ g$ là một cấu xạ từ E vào $\mathbf{A} \times \mathbf{B}$, thì $g$ là một cấu xạ; hay, tương đương, $g_1 = \overset{-1}{\pi} \circ g$ là một cấu xạ từ E vào A. Nhưng vì $g_1 = \mathrm{pr}_1 \circ (j \circ g)$, điều này suy ra từ giả thiết và định nghĩa của cấu trúc tích.

### 5. CẤU TRÚC CUỐI

Xét một họ các tập hợp $(\mathbf{A}_\iota)_{\iota \in \mathbf{I}}$, mỗi tập hợp đều được trang bị một cấu trúc $\mathscr{S}_\iota$ thuộc loài $\Sigma$. Cho E là một tập hợp, và với mỗi $\iota \in \mathbf{I}$, cho $g_\iota$ là một ánh xạ *từ* $\mathbf{A}_\iota$ *vào* E. Một cấu trúc $\mathscr{T}$ thuộc loài $\Sigma$ trên E được gọi là một *cấu trúc cuối cùng đối với họ* $(\mathbf{A}_\iota, \mathscr{S}_\iota, g_\iota)_{\iota \in \mathbf{I}}$ nếu nó có tính chất sau :

(FI) Cho bất kỳ tập hợp E′ nào, bất kỳ cấu trúc $\mathscr{S}'$ thuộc loài $\Sigma$ trên E, và bất kỳ ánh xạ $f$ *từ* E *vào* E′, quan hệ

$$\text{``}f \text{ là một cấu xạ từ E vào E'''}$$

là *tương đương* với quan hệ

$$\text{``với mọi } \iota \in \mathbf{I}, f \circ g_\iota \text{ là một cấu xạ từ } \mathbf{A}_\iota \text{ vào E'''}.$$

CST18. *Nếu tồn tại một cấu trúc cuối cùng trên* E *đối với họ* $(\mathbf{A}_\iota, \mathscr{S}_\iota, g_\iota)_{\iota \in \mathbf{I}}$, *thì nó là cấu trúc thuộc loài* $\Sigma$ *mịn nhất trên* E *sao cho mỗi ánh xạ* $g_\iota$ *là một cấu xạ, và do đó là duy nhất.*

Cho $\mathscr{T}$ là một cấu trúc cuối cùng trên E, và cho $\mathscr{S}$ là một cấu trúc thuộc loài $\Sigma$ trên E sao cho mỗi $g_\iota$ đều là một cấu xạ. Nếu $i$ ký hiệu ánh xạ đồng nhất của E, được trang bị $\mathscr{T}$, lên E, được trang bị $\mathscr{S}$, thì $i \circ g_\iota$ là một cấu xạ với mỗi $\iota \in \mathbf{I}$. Điều kiện (FI) khi đó cho thấy $i$ là một cấu xạ, nghĩa là (no. 2) $\mathscr{S}$ *thô hơn* $\mathscr{T}$. Áp dụng (FI) một lần nữa cho trường hợp trong đó $f$ là ánh xạ đồng nhất của E (được trang bị $\mathscr{T}$) lên chính nó, ta thấy (sử dụng $(\mathrm{MO_{III}})$) rằng mỗi $g_\iota$ là một cấu xạ từ $\mathbf{A}_\iota$ vào E. Điều này hoàn tất chứng minh.

Có thể xảy ra rằng tồn tại một cấu trúc thuộc loài $\Sigma$ trên E là cấu trúc mịn nhất trong tất cả các cấu trúc thuộc loài $\Sigma$ trên E sao cho các $g_\iota$ là các cấu xạ, nhưng cấu trúc này không phải là cấu trúc cuối cùng đối với họ $(\mathbf{A}_\iota, \mathscr{S}_\iota, g_\iota)$ (Exercise 6).

Ta có tiêu chuẩn *tính bắc cầu* sau :

CST19. *Cho* E *là một tập hợp, cho* $(\mathrm{A}_\iota)_{\iota \in \mathrm{I}}$ *là một họ các tập hợp, và với mỗi* $\iota \in \mathrm{I}$ *cho* $\mathscr{S}_\iota$ *là một cấu trúc thuộc loài* $\Sigma$ *trên* $\mathrm{A}_\iota$. *Cho* $(\mathrm{J}_\lambda)_{\lambda \in \mathrm{L}}$ *là một phân hoạch của* I, *và cho* $(\mathrm{B}_\lambda)_{\lambda \in \mathrm{L}}$ *là một họ các tập hợp được chỉ số bởi* L. *Với mỗi* $\lambda \in \mathrm{L}$, *cho* $h_\lambda$ *là một ánh xạ từ* $\mathrm{B}_\lambda$ *vào* E; *với mỗi* $\lambda \in \mathrm{L}$ *và mỗi* $\iota \in \mathrm{J}_\lambda$, *cho* $g_{\iota\lambda}$ *là một ánh xạ từ* $\mathrm{A}_\iota$ *vào* $\mathrm{B}_\lambda$, *và đặt* $f_\iota = h_\lambda \circ g_{\iota\lambda}$. *Giả sử rằng, với mỗi* $\lambda \in \mathrm{L}$, *tồn tại một cấu trúc cuối cùng* $\mathscr{S}'_\lambda$ *trên* $\mathrm{B}_\lambda$ *đối với họ* $(\mathrm{A}_\iota,\ \mathscr{S}_\iota,\ g_{\iota\lambda})_{\iota \in \mathrm{J}_\lambda}$. *Khi đó các mệnh đề sau là tương đương* :

(a) *Tồn tại một cấu trúc cuối cùng* $\mathscr{S}$ *trên* E *đối với họ* $(\mathrm{A}_\iota, \mathscr{S}_\iota, f_\iota)_{\iota \in \mathrm{I}}$.

(b) *Tồn tại một cấu trúc cuối cùng* $\mathscr{S}'$ *trên* E *đối với họ* $(\mathrm{B}_\lambda, \mathscr{S}'_\lambda, h_\lambda)_{\lambda \in \mathrm{L}}$.

*Hơn nữa các mệnh đề này kéo theo rằng* $\mathscr{S} = \mathscr{S}'$.

Cho F là một tập hợp được trang bị một cấu trúc loài $\Sigma$, và cho $u$ là một ánh xạ từ E vào F. Theo định nghĩa, quan hệ "$u \circ h_\lambda$ là một cấu xạ của $\mathrm{B}_\lambda$ vào F" tương đương với quan hệ

"với mọi $\iota \in \mathrm{J}_\lambda$, $u \circ h_\lambda \circ g_{\iota\lambda} = u \circ f_\iota$ là một cấu xạ của $\mathrm{A}_\iota$ vào F".

Do đó quan hệ

(3)             "với mọi $\lambda \in \mathrm{L}$,   $u \circ h_\lambda$ là một cấu xạ của $\mathrm{B}_\lambda$ vào F"

tương đương với quan hệ

(4)             "với mọi $\iota \in \mathrm{I}$,   $u \circ f_i$ là một cấu xạ của $\mathrm{A}_\iota$ vào F".

Nói rằng $\mathscr{S}'$ là cấu trúc cuối cùng đối với họ $(\mathrm{B}_\lambda, \mathscr{S}'_\lambda, h_\lambda)_{\lambda \in \mathrm{L}}$ có nghĩa là quan hệ (3) tương đương với quan hệ "$u$ là một cấu xạ của E (được trang bị $\mathscr{S}'$) vào F"; và nói rằng E là cấu trúc cuối cùng đối với họ $(\mathrm{A}_\iota, \mathscr{S}_\iota, f_\iota)_{\iota \in \mathrm{I}}$ có nghĩa là quan hệ (4) tương đương với quan hệ "$u$ là một cấu xạ của E (được trang bị $\mathscr{S}$) vào F"; do đó suy ra kết quả, xét đến tính chất duy nhất của cấu trúc cuối cùng.

### 6. CÁC VÍ DỤ VỀ CẤU TRÚC CUỐI CÙNG

I. *Ảnh trực tiếp của một cấu trúc.*   Khi I là một tập hợp gồm một phần tử duy nhất, cấu trúc cuối cùng đối với $(\mathrm{A}, \mathscr{S}, f)$ được gọi là *ảnh trực tiếp qua* $f$ *của cấu trúc* $\mathscr{S}$ (nếu nó tồn tại).

II. *Cấu trúc thương.*   Cho A là một tập hợp được trang bị một cấu trúc $\mathscr{S}$ của loài $\Sigma$, cho R là một quan hệ tương đương trên A, và cho $\varphi$ là ánh xạ chính tắc từ A lên tập thương $\mathrm{E} = \mathrm{A}/\mathrm{R}$ (Chương II, § 6, no. 2). Ảnh trực tiếp của cấu trúc $\mathscr{S}$ qua ánh xạ $\varphi$ được gọi là (nếu nó tồn tại) *thương* của cấu trúc $\mathscr{S}$ theo quan hệ R.

\* Nói chung, một cấu trúc thứ tự hoặc một cấu trúc đại số không thừa nhận các cấu trúc thương đối với các quan hệ tương đương tùy ý (cf. Chương III, § 1, Bài tập 2). Mặt khác, một tôpô luôn thừa nhận một cấu trúc thương đối với một quan hệ tương đương tùy ý, nhưng điều này không nhất thiết đúng đối với một tôpô Hausdorff. \*

Cho A, B là hai tập hợp được trang bị lần lượt các cấu trúc $\mathscr{S}$, $\mathscr{S}'$ thuộc loài $\Sigma$, và cho $f$ là một cấu xạ từ A vào B. Kí hiệu R là quan hệ tương đương $f(x) = f(y)$, kí hiệu $\varphi$ là ánh xạ chính tắc của A lên $\mathrm{A}/\mathrm{R}$, và kí hiệu $j$ là đơn ánh chính tắc của $f(\mathrm{A})$ vào B. Giả sử rằng $\mathscr{S}$ thừa nhận một cấu trúc thương $\mathscr{S}_0$ đối với R, và rằng $\mathscr{S}'$ cảm sinh một cấu trúc $\mathscr{S}'_0$ trên $f(\mathrm{A})$. Khi đó, trong *phân tích chính tắc* $f = j \circ g \circ \varphi$ của $f$ (Chapter II, § 6, no. 5), song ánh $g$ của $\mathrm{A}/\mathrm{R}$ lên $f(\mathrm{A})$ liên kết với $f$ là một *cấu xạ* (nhưng không nhất thiết là một đẳng cấu) khi $\mathrm{A}/\mathrm{R}$ được trang bị $\mathscr{S}_0$ và $f(\mathrm{A})$ với $\mathscr{S}'_0$. Vì $j \circ g$ là một cấu xạ của $\mathrm{A}/\mathrm{R}$ vào B theo định nghĩa của cấu trúc thương, và do đó $g$ là một cấu xạ của $\mathrm{A}/\mathrm{R}$ lên $f(\mathrm{A})$ theo định nghĩa của cấu trúc cảm sinh.

*Cho* A, A′ *là hai tập hợp được trang bị các cấu trúc* $\mathscr{S}$, $\mathscr{S}'$ *thuộc loài* $\Sigma$, *và cho* R (*resp.* R′) *là một quan hệ tương đương trên* A (*resp.* A′). *Giả sử tồn tại một cấu trúc thương* $\mathscr{S}_0$ (*resp.* $\mathscr{S}'_0$) *của* $\mathscr{S}$ *theo* R (*resp.* $\mathscr{S}'$ *theo* R′). *Nếu* $f$ *là một cấu xạ từ* A *vào* A′ *tương thích với các quan hệ tương đương* R *và* R′, *và nếu* $g$ *là ánh xạ thu được từ* $f$ *bằng cách chuyển qua thương, thì* $g$ *là một cấu xạ của* $\mathrm{A}/\mathrm{R}$ *vào* $\mathrm{A}'/\mathrm{R}'$.

Cho $\varphi$ (resp. $\varphi'$) là ánh xạ chính tắc của A lên $\mathrm{A}/\mathrm{R}$ (resp. của A′ lên $\mathrm{A}'/\mathrm{R}'$); khi đó ta có $g \circ \varphi = \varphi' \circ f$. Vì $\varphi'$ và $f$ là các cấu xạ, nên $\varphi' \circ f$ cũng là một cấu xạ theo ($\mathrm{MO_{II}}$). Nhưng khi đó, vì $g \circ \varphi$ là một cấu xạ, nên $g$ cũng là một cấu xạ theo định nghĩa của cấu trúc thương.

¶ Tiêu chuẩn tính bắc cầu CST19 nói riêng dẫn tới tiêu chuẩn sau :

CST21. *Cho* A *là một tập hợp được trang bị một cấu trúc* $\mathscr{S}$ *của loài* $\Sigma$, *và cho* R *là một quan hệ tương đương trên* A *sao cho trên* $\mathrm{A}/\mathrm{R}$ *tồn tại một cấu trúc thương* $\mathscr{S}'$ *của* $\mathscr{S}$ *theo* R. *Cho* S *là một quan hệ tương đương trên* A *thô hơn* R, *và cho* $\mathrm{S}/\mathrm{R}$ *ký hiệu quan hệ tương đương trên* $\mathrm{A}/\mathrm{R}$ *là thương của* S *theo* R *(Chương II, § 6, no. 7).* *Khi đó tồn tại trên* $(\mathrm{A}/\mathrm{R})/(\mathrm{S}/\mathrm{R})$ *một cấu trúc thương* $\mathscr{S}''$ *của* $\mathscr{S}'$ *theo* $\mathrm{S}/\mathrm{R}$ *khi và chỉ khi tồn tại trên* $\mathrm{A}/\mathrm{S}$ *một cấu trúc thương* $\mathscr{S}_0$ *của* $\mathscr{S}$ *theo* S, *và ánh xạ chính tắc của* $\mathrm{A}/\mathrm{S}$ *(được trang bị bởi* $\mathscr{S}_0$*) lên* $(\mathrm{A}/\mathrm{R})/(\mathrm{S}/\mathrm{R})$ *(được trang bị bởi* $\mathscr{S}''$*) là một đẳng cấu.*

Cho $\varphi$ là ánh xạ chính tắc của A lên $A/R$, và cho $\psi$ là ánh xạ của $A/R$ lên $(A/R)/(S/R)$. Nhờ CST19, $\mathscr{G}''$ là thương của $\mathscr{G}'$ theo $S/R$ khi và chỉ khi $\mathscr{G}''$ là cấu trúc cuối cùng đối với $(A,\mathscr{G},\psi\circ\varphi)$. Tiêu chuẩn đó suy ra từ việc quan hệ $\psi(\varphi(x))=\psi(\varphi(y))$ tương đương với S.

#### Nhận xét {#ens-iv-s2-n6-rem-1 .statement tag=03VW}

Cho A là một tập hợp được trang bị một cấu trúc $\mathscr{G}$ của loài $\Sigma$, và cho R là một quan hệ tương đương trên A sao cho tồn tại trên $E=A/R$ một cấu trúc thương $\mathscr{G}'$ của $\mathscr{G}$ theo R. Cho $\varphi$ là ánh xạ chính tắc của A lên E. Nói chung, không có *tiết diện* $s$ của $\varphi$ (Chương II, § 3, no. 8) nào là một *cấu xạ* từ E vào A. Giả sử rằng tồn tại một tiết diện như thế $s$, và hơn nữa tồn tại một cấu trúc $\mathscr{G}''$ được cảm sinh bởi $\mathscr{G}$ trên $s(E)$. Khi đó, nếu $j$ ký hiệu đơn ánh chính tắc của $s(E)$ vào A và nếu $s=j\circ f$, thì song ánh $f$ là một *đẳng cấu* từ E lên $s(E)$. Thật vậy, $f$ là một cấu xạ theo định nghĩa của cấu trúc được cảm sinh, và $g=\varphi\circ j$ là một cấu xạ của $s(E)$ lên E do (MO$_{\mathrm{II}}$). Vì $g\circ f$ và $f\circ g$ lần lượt là các ánh xạ đồng nhất của E và $s(E)$, nên mệnh đề này là một hệ quả của CST8.

### Bài tập {#ens-iv-s2-exercises}

Xem [các bài tập của § 2](exercises/s2/).
