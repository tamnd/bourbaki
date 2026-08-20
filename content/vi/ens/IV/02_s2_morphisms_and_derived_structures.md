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
content_sha256: 68a8f4bf0f517a7917776dffba6cfe2314663b75042a23ca9f231dcb23e43623
translated_from: content/en/ens/IV/02_s2_morphisms_and_derived_structures.md
source_content_sha256: 1df0116fa77b9eebc1d44429db56bb11c1cc04c82010063f9e8691600a51190e
translation_model: gpt-5.4
translation_run: translate-vi-362ea494
glossary_version: 29
glossary_terms_sha256: f6304d853f6e48a03c0ae16d58797bc66ff3a6760cefb52564504683c3573cd3
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 2. CÁC CẤU XẠ VÀ CÁC CẤU TRÚC DẪN XUẤT

### 1. CÁC CẤU XẠ

Trong tiết này và tiết sau, để cho đơn giản, ta sẽ giả thiết rằng loài cấu trúc đang xét chỉ có *một* tập hợp cơ sở (do đó là một tập hợp cơ sở chính). Người đọc sẽ không gặp khó khăn gì khi mở rộng các định nghĩa và các kết quả sang trường hợp tổng quát.

Cho $\Sigma$ là một loài cấu trúc trong một lý thuyết $\mathscr{T}$ mạnh hơn lý thuyết tập hợp, và $x$, $y$, $s$, $t$ là bốn chữ cái phân biệt, khác với các hằng của $\mathscr{T}$. Nhắc lại rằng ký hiệu $\mathscr{F}(x, y)$ biểu thị tập hợp các ánh xạ từ $x$ vào $y$ (Chương II, § 5, số 2). Giả sử ta được cho một số hạng $\sigma\{x, y, s, t\}$ trong $\mathscr{T}$ thỏa mãn các điều kiện sau :

(MO$_{\mathrm{I}}$) *Quan hệ* "$s$ *là một cấu trúc thuộc loài* $\Sigma$ *trên* $x$, *và* $t$ *là một cấu trúc thuộc loài* $\Sigma$ *trên* $y$" *kéo theo, trong* E, *quan hệ* $\sigma\{x, y, s, t\} \subset \mathscr{F}(x, y)$.

(MO$_{\mathrm{II}}$) *Nếu, trong một lý thuyết* $\mathscr{T}'$ *mạnh hơn* $\mathscr{T}$, *ta có ba tập hợp* E, E′, E″ *được trang bị tương ứng các cấu trúc* $\mathscr{S}$, $\mathscr{S}'$, $\mathscr{S}''$ *thuộc loài* $\Sigma$, *thì các quan hệ* $f \in \sigma\{\mathrm{E},\ \mathrm{E}',\ \mathscr{S},\ \mathscr{S}'\}$ *và* $g \in \sigma\{\mathrm{E}',\ \mathrm{E}'',\ \mathscr{S}',\ \mathscr{S}''\}$ *suy ra quan hệ*

$$g \circ f \in \sigma\{\mathrm{E},\ \mathrm{E}'',\ \mathscr{S},\ \mathscr{S}''\}.$$

(MO$_{\mathrm{III}}$) *Nếu, trong một lý thuyết* $\mathscr{T}'$ *mạnh hơn* $\mathscr{T}$, *ta có hai tập hợp* E, E′ *được trang bị lần lượt các cấu trúc* $\mathscr{S}$, $\mathscr{S}'$ *thuộc loài* $\Sigma$, *thì một song ánh* $f$ *của* E *lên* E′ *là một đẳng cấu khi và chỉ khi* $f \in \sigma\{\mathrm{E},\ \mathrm{E}',\ \mathscr{S},\ \mathscr{S}'\}$ *và* $\overset{-1}{f} \in \sigma\{\mathrm{E}',\ \mathrm{E},\ \mathscr{S}',\ \mathscr{S}\}$.

Nếu $\Sigma$ và $\sigma$ được cho, quan hệ $f \in \sigma\{x, y, s, t\}$ được diễn đạt bằng cách nói rằng $f$ là một *cấu xạ* (hoặc một *σ-cấu xạ*) *từ* $x$, *được trang bị* $s$, *vào* $y$, *được trang bị* $t$. Nếu (trong một lý thuyết $\mathscr{T}'$ mạnh hơn $\mathscr{T}$) E và E′ là hai tập hợp được trang bị các cấu trúc $\mathscr{S}$, $\mathscr{S}'$ thuộc loài $\Sigma$, thì số hạng $\sigma\{\mathrm{E}, \mathrm{E}', \mathscr{S}, \mathscr{S}'\}$ là *tập hợp các σ-cấu xạ từ* E *vào* E′.

*Ví dụ*

#### Ví dụ 1 {#ens-iv-s2-n1-exa-1 .statement tag=03VL}

Lấy $\Sigma$ là loài các cấu trúc thứ tự và ký hiệu $\sigma\{x,\ y,\ s,\ t\}$ là tập hợp mọi ánh xạ $f$ từ $x$ vào $y$ sao cho quan hệ $(u,\ v) \in s$ kéo theo $(f(u), f(v)) \in t$. Theo ký hiệu của Chương III, § 1,

điều này có nghĩa là $u \leqslant v$ kéo theo $f(u) \leqslant f(v)$, tức là $f$ là *tăng*. Việc kiểm tra các tiên đề $(\mathrm{MO_I})$, $(\mathrm{MO_{II}})$, và $(\mathrm{MO_{III}})$ là hiển nhiên.

#### Ví dụ 2 {#ens-iv-s2-n1-exa-2 .statement tag=03VM}

Lấy $\Sigma$ là một loài các cấu trúc đại số có một luật hợp thành (trong) duy nhất, được xác định khắp nơi (§1, no. 4, Ví dụ 2). Cho A, A$'$ là hai tập hợp được trang bị các cấu trúc thuộc loài $\Sigma$, và gọi $p$, $p'$ là các luật hợp thành của hai cấu trúc ấy. Xét các ánh xạ $f$ từ A vào A$'$ sao cho $p'(f(x), f(y)) = f(p(x,\ y))$ với mọi $x \in \mathrm{A}$ và mọi $y \in \mathrm{A}$. Các ánh xạ này thỏa mãn $(\mathrm{MO_I})$, $(\mathrm{MO_{II}})$, và $(\mathrm{MO_{III}})$, và được gọi là các *đồng cấu* từ A vào A$'$.

#### Ví dụ 3 {#ens-iv-s2-n1-exa-3 .statement tag=03VN}

Lấy $\Sigma$ là loài các cấu trúc tôpô (§1, no. 4, Ví dụ 3). Cho A, A$'$ là hai tập hợp được trang bị các tôpô V, V$'$, tương ứng. Xét các ánh xạ $f$ từ A vào A$'$ sao cho quan hệ $\mathrm{X}' \in \mathrm{V}'$ kéo theo $\overset{-1}{f}(\mathrm{X}') \in \mathrm{V}$ (nói cách khác, sao cho ảnh ngược của mọi tập hợp mở trong tôpô V$'$ là một tập hợp mở trong tôpô V). Các ánh xạ này, thỏa mãn $(\mathrm{MO_I})$, $(\mathrm{MO_{II}})$, và $(\mathrm{MO_{III}})$, là các ánh xạ *liên tục* từ A vào A$'$ (đối với các tôpô V và V$'$) (xem *Tôpô đại cương*, Chương I, § 2).

#### Nhận xét {#ens-iv-s2-n1-rem-1 .statement tag=03VO}

Đối với một loài cấu trúc $\Sigma$ đã cho, ta có thể cần định nghĩa nhiều thuật ngữ $\sigma \} x,\ y,\ s,\ t \{$ thỏa mãn các điều kiện $(\mathrm{MO_I})$, $(\mathrm{MO_{II}})$, và $(\mathrm{MO_{III}})$. Chẳng hạn, nếu $\Sigma$ là loài cấu trúc tôpô, với ký hiệu của Ví dụ 3 ở trên, một ánh xạ $f$ của A vào A$'$ được gọi là *mở* nếu quan hệ $\mathrm{X} \in \mathrm{V}$ kéo theo $f(\mathrm{X}) \in \mathrm{V}'$ (nói cách khác, nếu ảnh qua $f$ của mọi tập mở là một tập mở). Dễ dàng kiểm tra rằng các ánh xạ mở cũng thỏa mãn các điều kiện $(\mathrm{MO_I})$, $(\mathrm{MO_{II}})$, và $(\mathrm{MO_{III}})$ đối với loài $\Sigma$. \* Hơn nữa, có thể chỉ ra rằng một ánh xạ liên tục không tất yếu là mở, và rằng một ánh xạ mở không tất yếu liên tục. \* Vì vậy, một loài cấu trúc đã cho *không kéo theo* một khái niệm cấu xạ được xác định rõ ràng.

☡

Đối với các cấu trúc thứ tự, các cấu trúc đại số và các cấu trúc tôpô, luôn luôn phải hiểu rằng các cấu xạ là những cấu xạ đã được định nghĩa trong các Ví dụ ở trên, trừ khi điều ngược lại được phát biểu minh thị.

Điều kiện $(\mathrm{MO_{III}})$ và đặc trưng hóa của các song ánh (Chương II, § 3, no. 8, Hệ quả của Mệnh đề 8) suy ra tiêu chuẩn sau :

CST8. *Cho* E, E$'$ *là hai tập hợp, mỗi tập hợp được trang bị một cấu trúc thuộc loài $\Sigma$. Cho $f$ là một $\sigma$-cấu xạ từ* E *vào* E$'$ *và cho $g$ là một $\sigma$-cấu xạ từ* E$'$ *vào* E. *Nếu $g \circ f$ là ánh xạ đồng nhất của* E *lên chính nó, và nếu $f \circ g$ là ánh xạ đồng nhất của* E$'$ *lên chính nó, thì $f$ là một đẳng cấu từ* E *lên* E$'$, *và $g$ là đẳng cấu nghịch đảo.*

Cần lưu ý rằng một song ánh của E lên E$'$ có thể là một $\sigma$-cấu xạ mà song ánh ngược không tất yếu là một $\sigma$-cấu xạ. \* Chẳng hạn, một ánh xạ song ánh của một không gian tôpô A lên một không gian tôpô A$'$ có thể liên tục mà song ánh ngược không liên tục (*Tôpô đại cương*, Chương I, § 2, no. 1, Nhận xét 1). \*

☡

#### Nhận xét {#ens-iv-s2-n1-rem-2 .statement tag=03VP}

Khi một loài cấu trúc $\Sigma$ có nhiều tập hợp cơ sở chính $x_1, \ldots, x_n$, và các tập hợp cơ sở phụ $\mathrm{A}_1, \ldots, \mathrm{A}_m$, thì một $\sigma$-cấu xạ là một hệ $(f_1, \ldots, f_n)$, trong đó $f_i$ là một ánh xạ của $x_i$ vào $y_i$ $(1 \leqslant i \leqslant n)$, và các hệ ánh xạ này thỏa mãn những điều kiện tương tự như $(\mathrm{MO_{II}})$ và $(\mathrm{MO_{III}})$, mà người đọc có thể dễ dàng tự phát biểu.

### 2. CẤU TRÚC MỊN HƠN

Trong phần còn lại của tiết này, ta sẽ giả sử rằng đã cho một loài cấu trúc $\Sigma$ và một khái niệm về $\sigma$-cấu xạ tương đối đối với loài cấu trúc này; *mọi khái niệm sẽ được đưa vào đều phụ thuộc không những vào $\Sigma$ mà còn vào khái niệm $\sigma$-cấu xạ được xét đến.* Thông thường ta sẽ nói "cấu xạ" thay cho "$\sigma$-cấu xạ".

¶ Cho E là một tập hợp và $\mathscr{S}_1$, $\mathscr{S}_2$ là hai cấu trúc thuộc loài $\Sigma$ trên E. Cấu trúc $\mathscr{S}_1$ được gọi là *mịn hơn* $\mathscr{S}_2$ (và $\mathscr{S}_2$ *thô hơn* $\mathscr{S}_1$) nếu ánh xạ đồng nhất của E, được trang bị $\mathscr{S}_1$, lên E, được trang bị $\mathscr{S}_2$, là một cấu xạ.

Khi cần thiết để tránh mọi nhập nhằng, ta sẽ nói rằng $\mathscr{S}_1$ mịn hơn $\mathscr{S}_2$ *tương đối với khái niệm $\sigma$-cấu xạ đang xét*; và tương tự như vậy đối với mọi khái niệm khác sẽ được định nghĩa trong tiết diện này.

Giả sử rằng $\mathscr{S}_1$ mịn hơn $\mathscr{S}_2$. Nếu E$'$ là một tập hợp được trang bị một cấu trúc $\mathscr{S}'$ thuộc loài $\Sigma$, và nếu $f$ là một cấu xạ từ E, được trang bị $\mathscr{S}_2$, vào E$'$, được trang bị $\mathscr{S}'$, thì $f$ cũng là một cấu xạ từ E, được trang bị $\mathscr{S}_1$, vào E$'$, được trang bị $\mathscr{S}'$; điều này suy ra từ định nghĩa trước đó và từ $(\mathrm{MO_{II}})$. Tương tự, nếu $g$ là một cấu xạ từ E$'$, được trang bị $\mathscr{S}'$, vào E, được trang bị $\mathscr{S}_1$, thì $g$ cũng là một cấu xạ từ E$'$, được trang bị $\mathscr{S}'$, vào E, được trang bị $\mathscr{S}_2$.

Do đó, cấu trúc (thuộc loài $\Sigma$) trên E càng *mịn hơn* thì càng có *nhiều* cấu xạ lấy E làm nguồn, và càng có *ít* cấu xạ lấy E làm đích.

Quan hệ "$\mathscr{S}_1$ thô hơn $\mathscr{S}_2$" là một *quan hệ thứ tự* giữa $\mathscr{S}_1$ và $\mathscr{S}_2$ trên tập hợp mọi cấu trúc của loài $\Sigma$ trên E; thật vậy, nó phản xạ theo $(\mathrm{MO_{III}})$, bắc cầu theo $(\mathrm{MO_{II}})$, và nếu một cấu trúc thuộc loài $\Sigma$ vừa mịn hơn vừa thô hơn một cấu trúc khác, thì hai cấu trúc ấy là đồng nhất theo $(\mathrm{MO_{III}})$. Phù hợp với các định nghĩa tổng quát (Chương III, § 1, no. 14), hai cấu trúc của loài $\Sigma$ trên E được gọi là *so sánh được* nếu một cấu trúc mịn hơn cấu trúc kia; một cấu trúc được gọi là *mịn hơn nghiêm ngặt* (resp. *thô hơn nghiêm ngặt*) một cấu trúc khác nếu nó *mịn hơn* (resp. *thô hơn*) cấu trúc kia và phân biệt với cấu trúc ấy.

*Ví dụ*

#### Ví dụ 1 {#ens-iv-s2-n2-exa-1 .statement tag=03VQ}

Một cấu trúc thứ tự có đồ thị $s$ trên một tập hợp A mịn hơn một cấu trúc thứ tự có đồ thị $s'$ khi và chỉ khi $s \subset s'$. Nói cách khác, quan hệ $x \leqslant y$ đối với $s$ kéo theo $x \leqslant y$ đối với $s'$; điều này phù hợp với định nghĩa đã cho trong Chương III, § 1, no. 4, Ví dụ 3.

#### Ví dụ 2 {#ens-iv-s2-n2-exa-2 .statement tag=03VR}

Xét hai cấu trúc đại số F, F' cùng loài $\Sigma$ trên một tập hợp A, trong đó F và F' là các đồ thị của các luật hợp thành (được định nghĩa mọi nơi) của hai cấu trúc này. Từ định nghĩa của các cấu xạ trong trường hợp này (no. 1, Ví dụ 2), F mịn hơn F' khi và chỉ khi $F \subset F'$. Nhưng vì F và F' đều là các đồ thị phiếm hàm có cùng miền xác định $A \times A$, nên ta phải có $F = F'$. Nói cách khác, hai cấu trúc *so sánh được* của loài $\Sigma$ tất yếu *đồng nhất*.

#### Ví dụ 3 {#ens-iv-s2-n2-exa-3 .statement tag=03VS}

Cho V, V' là hai tôpô trên cùng một tập hợp A. Nói rằng V mịn hơn V' có nghĩa là, do định nghĩa của các cấu xạ trong trường hợp này (no. 1, Ví dụ 3), ta có $V' \subset V$; nói cách khác, mọi tập con của A là một tập mở trong tôpô V' cũng là một tập mở trong tôpô V (và do đó, tôpô càng mịn thì càng có nhiều tập mở).

#### Chú ý {#ens-iv-s2-n2-rem-1 .statement tag=03VT}

Ta vừa gặp một ví dụ (Ví dụ 2) trong đó hai cấu trúc so sánh được của cùng loài $\Sigma$ tất yếu là đồng nhất. Còn có nhiều ví dụ khác như vậy : các cấu trúc thứ tự tuyến tính, \* các tôpô compact, các cấu trúc không gian Fréchet (các cấu xạ là các ánh xạ tuyến tính liên tục), các tôpô được định nghĩa bởi một giá trị tuyệt đối (hay một định giá) trên một vành phép chia, v.v. \*

Đối với một loài cấu trúc như thế $\Sigma$, một cấu xạ $f$ từ E vào E' mà *song ánh* là một *đẳng cấu*; vì nếu ta chuyển lên E' cấu trúc $\mathscr{S}$ trên E nhờ $f$, thì ta thu được một cấu trúc thuộc loài $\Sigma$ mịn hơn cấu trúc $\mathscr{S}'$ trên E' và do đó trùng với $\mathscr{S}'$.

### 3. CẤU TRÚC BAN ĐẦU

Xét một họ $(A_\iota)_{\iota \in I}$ các tập hợp, mỗi tập hợp được trang bị một cấu trúc $\mathscr{S}_\iota$ thuộc loài $\Sigma$. Cho E là một tập hợp, và với mỗi $\iota \in I$ cho $f_\iota$ là một ánh xạ *từ* E *vào* $A_\iota$. Một cấu trúc $\mathscr{S}$ thuộc loài $\Sigma$ trên E được gọi là một *cấu trúc ban đầu đối với họ* $(A_\iota, \mathscr{S}_\iota, f_\iota)_{\iota \in I}$ nếu nó có tính chất sau :

(IN) Với mọi tập hợp E', mọi cấu trúc thuộc loài $\mathscr{S}'$ trên E', và mọi ánh xạ $g$ *từ* E' *vào* E, quan hệ

"$g$ là một cấu xạ từ E' vào E"

là *tương đương* với quan hệ

"với mỗi $\iota \in I, f_\iota \circ g$ là một cấu xạ từ E' vào $A_\iota$".

CST9. *Nếu tồn tại một cấu trúc ban đầu trên* E *đối với họ* $(\mathrm{A}_\iota,\ \mathscr{S}_\iota,\ f_\iota)_{\iota \in \mathrm{I}}$, *thì đó là cấu trúc thô nhất trong tất cả các cấu trúc thuộc loài* $\Sigma$ *trên* E *sao cho mỗi ánh xạ* $f_\iota$ *là một cấu xạ, và do đó là duy nhất.*

Cho $\mathscr{I}$ là một cấu trúc ban đầu trên E, và cho $\mathscr{S}$ là một cấu trúc thuộc loài $\Sigma$ trên E mà đối với nó mỗi $f_\iota$ là một cấu xạ. Nếu $i$ ký hiệu ánh xạ đồng nhất từ E, được trang bị $\mathscr{S}$, vào E, được trang bị $\mathscr{I}$, thì $f_\iota \circ i$ là một cấu xạ với mọi $\iota \in \mathrm{I}$, và điều kiện (IN) cho thấy rằng $i$ là một cấu xạ, điều đó có nghĩa (no. 2) là $\mathscr{S}$ *mịn hơn* $\mathscr{I}$. Mặt khác, áp dụng (IN) cho trường hợp trong đó $g$ là ánh xạ đồng nhất của E (được trang bị $\mathscr{I}$) lên chính nó, ta thấy (theo $(\mathrm{MO_{III}})$) rằng mỗi $f_\iota$ là một cấu xạ từ E vào $\mathrm{A}_\iota$, điều này hoàn tất chứng minh.

Có thể xảy ra trường hợp tồn tại một cấu trúc loài $\Sigma$ trên E thô nhất trong tất cả các cấu trúc loài $\Sigma$ mà đối với chúng các $f_\iota$ là cấu xạ, nhưng cấu trúc này lại không phải là cấu trúc ban đầu đối với $(\mathrm{A}_\iota, \mathscr{S}_\iota, f_\iota)$ (Bài tập 6).

Ta có *tiêu chuẩn tính bắc cầu* sau đây :

CST10. *Cho* E *là một tập hợp, cho* $(\mathrm{A}_\iota)_{\iota \in \mathrm{I}}$ *là một họ các tập hợp, và với mỗi* $\iota \in \mathrm{I}$ *cho* $\mathscr{S}_\iota$ *là một cấu trúc thuộc loài* $\Sigma$ *trên* $\mathrm{A}_\iota$. *Cho* $(\mathrm{J}_\lambda)_{\lambda \in \mathrm{L}}$ *là một phân hoạch của* I, *và cho* $(\mathrm{B}_\lambda)_{\lambda \in \mathrm{L}}$ *là một họ các tập hợp được đánh chỉ số bởi* L. *Với mỗi* $\lambda \in \mathrm{L}$ *cho* $h_\lambda$ *là một ánh xạ từ* E *vào* $\mathrm{B}_\lambda$, *và với mỗi* $\lambda \in \mathrm{L}$ *và mỗi* $\iota \in \mathrm{J}_\lambda$ *cho* $g_{\lambda\iota}$ *là một ánh xạ từ* $\mathrm{B}_\lambda$ *vào* $\mathrm{A}_\iota$, *và cho* $f_\iota = g_{\lambda\iota} \circ h_\lambda$. *Giả sử rằng, với mỗi* $\lambda \in \mathrm{L}$, *tồn tại một cấu trúc ban đầu* $\mathscr{S}'_\lambda$ *trên* $\mathrm{B}_\lambda$ *đối với họ* $(\mathrm{A}_\iota, \mathscr{S}_\iota, g_{\lambda\iota})_{\iota \in \mathrm{J}_\lambda}$. *Khi đó các mệnh đề sau là tương đương* :

(a) *tồn tại một cấu trúc ban đầu* $\mathscr{I}$ *trên* E *đối với họ* $(\mathrm{A}_\iota, \mathscr{S}_\iota, f_\iota)_{\iota \in \mathrm{I}}$;

(b) *tồn tại một cấu trúc ban đầu* $\mathscr{I}'$ *trên* E *đối với họ* $(\mathrm{B}_\lambda, \mathscr{S}'_\lambda, h_\lambda)_{\lambda \in \mathrm{L}}$.

*Hơn nữa, các mệnh đề này suy ra rằng* $\mathscr{I} = \mathscr{I}'$.

Cho F là một tập hợp được trang bị một cấu trúc thuộc loài $\Sigma$, và cho $u$ là một ánh xạ từ F vào E. Nhận thấy rằng theo định nghĩa quan hệ "$h_\lambda \circ u$ là một cấu xạ từ F vào $\mathrm{B}_\lambda$" là tương đương với quan hệ "với mọi $\iota \in \mathrm{J}_\lambda$, $g_{\lambda\iota} \circ h_\lambda \circ u = f_\iota \circ u$ là một cấu xạ từ F vào $\mathrm{A}_\iota$". Quan hệ

(1)     "với mọi $\lambda \in \mathrm{L}$, $h_\lambda \circ u$ là một cấu xạ từ F vào $\mathrm{B}_\lambda$"

do đó là tương đương với quan hệ

(2)     "với mọi $\iota \in \mathrm{I}$, $f_\iota \circ u$ là một cấu xạ từ F vào $\mathrm{A}_\iota$".

Bây giờ, nói rằng $\mathscr{I}'$ là cấu trúc ban đầu đối với họ $(\mathrm{B}_\lambda, \mathscr{S}'_\lambda, h_\lambda)_{\lambda \in \mathrm{L}}$ có nghĩa là quan hệ (1) tương đương với quan hệ "$u$ là một cấu xạ từ F vào E được trang bị $\mathscr{I}'$"; và nói rằng $\mathscr{I}$ là

cấu trúc ban đầu đối với họ $(\mathrm{A}_\iota, \mathscr{S}_\iota, f_\iota)_{\iota \in \mathrm{I}}$ có nghĩa là quan hệ (2) tương đương với quan hệ "$u$ là một cấu xạ từ F vào E được trang bị I". Do đó suy ra kết quả, theo tính chất về tính duy nhất của cấu trúc ban đầu.

### 4. CÁC VÍ DỤ VỀ CẤU TRÚC BAN ĐẦU

I. *Ảnh ngược của một cấu trúc*. Khi I là một tập hợp gồm một phần tử duy nhất, cấu trúc ban đầu đối với $(\mathrm{A}, \mathscr{S}, f)$ được gọi là *ảnh ngược theo $f$ của cấu trúc* $\mathscr{S}$ (khi nó tồn tại).

\* Một tôpô luôn có ảnh ngược theo mọi ánh xạ $f$; nhưng điều này không đúng đối với một cấu trúc thứ tự hoặc một cấu trúc đại số. \*

II. *Cấu trúc cảm sinh*. Cho A là một tập hợp được trang bị một cấu trúc $\mathscr{S}$ thuộc loài $\Sigma$, cho B là một tập con của A, và cho $j$ là đơn ánh chính tắc của B vào A. Khi đó ảnh ngược theo $j$ của cấu trúc B (nếu nó tồn tại) được gọi là *cấu trúc cảm sinh* bởi $\mathscr{S}$ trên B.

Một cấu trúc thứ tự cảm sinh một cấu trúc cùng loài trên mọi tập con của tập hợp mà trên đó nó được định nghĩa; nhưng điều này không đúng đối với cấu trúc của một tập có hướng. \* Một tôpô cảm sinh một tôpô trên mọi tập con của tập hợp mà trên đó nó được định nghĩa, nhưng nói chung một tôpô compắc không cảm sinh một tôpô compắc. Nói chung, một cấu trúc đại số trên một tập hợp A không cảm sinh một cấu trúc cùng loài trên một tập con tùy ý B; nếu cấu trúc đã cho trên A gồm những luật hợp thành được định nghĩa khắp nơi, thì điều kiện cần thiết là B phải ổn định đối với từng luật ấy, nhưng điều kiện cần thiết này không phải lúc nào cũng đủ. \*

Tiêu chuẩn tổng quát CST10 cho ta *tiêu chuẩn bắc cầu* sau đây đối với các cấu trúc cảm sinh :

CST11. *Cho* B *là một tập con của* A, *cho* C *là một tập con của* B, *và cho* $\mathscr{S}$ *là một cấu trúc thuộc loài* $\Sigma$ *trên* A *mà cảm sinh một cấu trúc* $\mathscr{S}'$ *cùng loài trên* B. *Khi đó* $\mathscr{S}$ *cảm sinh một cấu trúc thuộc loài* $\Sigma$ *trên* C *khi và chỉ khi* $\mathscr{S}'$ *cảm sinh một cấu trúc thuộc loài* $\Sigma$ *trên* C, *và khi đó các cấu trúc cảm sinh trên* C *bởi* $\mathscr{S}$ *và* $\mathscr{S}'$ *là đồng nhất.*

CST12. *Cho* A, A$'$ *là hai tập hợp được trang bị các cấu trúc* $\mathscr{S}$, $\mathscr{S}'$ *thuộc loài* $\Sigma$. *Cho* B *là một tập con của* A, *và* B$'$ *là một tập con của* A$'$. *Giả sử rằng* $\mathscr{S}$ (resp. $\mathscr{S}'$) *cảm sinh một cấu trúc thuộc loài* $\Sigma$ *trên* B (resp. B$'$). *Nếu* $f$ *là một cấu xạ từ* A *vào* A$'$ *sao cho* $f(\mathrm{B}) \subset \mathrm{B}'$, *thì ánh xạ* $g$ *từ* B *vào* B$'$ *trùng với* $f$ *trên* B *là một cấu xạ* (*đối với các cấu trúc do* $\mathscr{S}$ *và* $\mathscr{S}'$ *cảm sinh*).

Cho $j$ (tương ứng, $j'$) là đơn ánh chính tắc của B (tương ứng, B$'$) vào A (tương ứng, A$'$). Theo định nghĩa, ta có $f \circ j = j' \circ g$. Vì $f$ và $j$ là các cấu xạ,

nên $f \circ j$ cũng là một cấu xạ theo $(\mathrm{MO_{II}})$; nhưng khi đó, do $j' \circ g$ là một cấu xạ, ánh xạ $g$ là một cấu xạ theo định nghĩa của cấu trúc ban đầu.

III. *Cấu trúc tích.* Cho $(\mathrm{A}_\iota)_{\iota \in \mathrm{I}}$ là một họ các tập hợp, và trên mỗi tập hợp $\mathrm{A}_\iota$ cho $\mathscr{S}_\iota$ là một cấu trúc thuộc loài $\Sigma$. Gọi $\mathrm{E} = \prod_{\iota \in \mathrm{I}} \mathrm{A}_\iota$ là *tích* của họ $(\mathrm{A}_\iota)_{\iota \in \mathrm{I}}$ (Chương II, § 5), và ký hiệu $\mathrm{pr}_\iota$ là phép chiếu của $\mathrm{E}$ lên $\mathrm{A}_\iota$. Cấu trúc ban đầu (nếu tồn tại) đối với họ $(\mathrm{A}_\iota, \mathscr{S}_\iota, \mathrm{pr}_\iota)_{\iota \in \mathrm{I}}$ được gọi là *tích* của các cấu trúc $\mathscr{S}_\iota$.

Một họ các cấu trúc thứ tự luôn luôn thừa nhận một cấu trúc tích, nhưng điều đó không phải lúc nào cũng đúng đối với một họ các cấu trúc thứ tự toàn phần. \* Một họ các cấu trúc nhóm luôn luôn thừa nhận một cấu trúc tích, nhưng điều đó không nhất thiết đúng đối với một họ các cấu trúc vành chia. Một họ các tôpô luôn luôn thừa nhận một cấu trúc tích, nhưng điều này không phải lúc nào cũng đúng đối với một họ các cấu trúc không gian compact địa phương; trong trường hợp này, có một cấu trúc tích cùng loài nếu họ là *hữu hạn*, nhưng có thể không có nếu họ là *vô hạn* (xem *Topologie générale*, Chương I, § 9, no. 7, Mệnh đề 14). \*

Tiêu chuẩn CST10 dẫn đến *tiêu chuẩn tính kết hợp* sau đây đối với các cấu trúc tích :

CST13. *Cho $(\mathrm{A}_\iota)_{\iota \in \mathrm{I}}$ là một họ các tập hợp, và với mỗi chỉ số $\iota \in \mathrm{I}$, gọi $\mathscr{S}_\iota$ là một cấu trúc thuộc loài $\Sigma$ trên $\mathrm{A}_\iota$. Cho $(\mathrm{J}_\lambda)_{\lambda \in \mathrm{L}}$ là một phân hoạch của $\mathrm{I}$. Giả sử rằng trên mỗi tích bộ phận $\mathrm{B}_\lambda = \prod_{\iota \in \mathrm{J}_\lambda} \mathrm{A}_\iota$ họ $(\mathscr{S}_\iota)_{\iota \in \mathrm{J}_\lambda}$ thừa nhận một cấu trúc tích $\mathscr{S}'_\lambda$. Khi đó họ $(\mathscr{S}_\iota)_{\iota \in \mathrm{I}}$ thừa nhận một cấu trúc tích $\mathscr{S}$ khi và chỉ khi họ $(\mathscr{S}'_\lambda)_{\lambda \in \mathrm{L}}$ thừa nhận một cấu trúc tích $\mathscr{S}'$, và khi ấy ánh xạ chính tắc từ $\mathrm{E} = \prod_{\iota \in \mathrm{I}} \mathrm{A}_\iota$, được trang bị $\mathscr{S}$, lên $\mathrm{F} = \prod_{\lambda \in \mathrm{L}} \mathrm{B}_\lambda$, được trang bị $\mathscr{S}'$ (Chương II, § 5, no. 5), là một đẳng cấu.*

Một áp dụng khác của CST10 cho ta tiêu chuẩn sau đây liên quan đến các cấu trúc cảm sinh bởi một cấu trúc tích :

CST14. *Cho $(\mathrm{A}_\iota)_{\iota \in \mathrm{I}}$ là một họ các tập hợp, và với mỗi $\iota \in \mathrm{I}$, cho $\mathscr{S}_\iota$ là một cấu trúc thuộc loài $\Sigma$ trên $\mathrm{A}_\iota$. Với mỗi $\iota \in \mathrm{I}$, cho $\mathrm{B}_\iota$ là một tập con của $\mathrm{A}_\iota$. Giả sử rằng mỗi $\mathscr{S}_\iota$ cảm sinh một cấu trúc $\mathscr{S}'_\iota$ trên $\mathrm{B}_\iota$, và rằng trên tích $\mathrm{E} = \prod_{\iota \in \mathrm{I}} \mathrm{A}_\iota$ tồn tại một cấu trúc $\mathscr{S}_0$ là tích của họ $(\mathscr{S}_\iota)$. Khi đó các mệnh đề sau là tương đương :*

(a) *trên tập hợp $\mathrm{B} = \prod_{i \in \mathrm{I}} \mathrm{B}_\iota \subset \mathrm{E}$ tồn tại một cấu trúc $\mathscr{S}$ cảm sinh bởi $\mathscr{S}_0$;*

(b) *trên tập hợp $\mathrm{B}$ tồn tại một cấu trúc $\mathscr{S}'$ là tích của họ các cấu trúc $(\mathscr{S}'_\iota)$.*

*Hơn nữa, các mệnh đề này kéo theo rằng $\mathscr{S} = \mathscr{S}'$.*

Gọi $j_\iota$ là đơn ánh chính tắc của $\mathrm{B}_\iota$ vào $\mathrm{A}_\iota$, gọi $j$ là đơn ánh chính tắc của B vào E, gọi $p_\iota$ là phép chiếu của E lên $\mathrm{A}_\iota$, và gọi $p'_\iota$ là phép chiếu của B lên $\mathrm{B}_\iota$. Khi đó ta có $p_\iota \circ j = j_\iota \circ p'_\iota$ với mọi $\iota \in \mathrm{I}$. Theo CST10, $\mathscr{S}$ là cấu trúc ban đầu đối với họ $(\mathrm{A}_\iota, \mathscr{S}_\iota, p_\iota \circ j)_{\iota \in \mathrm{I}}$, và $\mathscr{S}'$ là cấu trúc ban đầu đối với họ $(\mathrm{A}_\iota, \mathscr{S}_\iota, j_\iota \circ p'_\iota)_{\iota \in \mathrm{I}}$. Suy ra kết quả.

¶ Các khái niệm ảnh ngược và tích liên quan với nhau theo tiêu chuẩn sau đây :

CST15. *Cho $(\mathrm{A}_\iota)_{\iota \in \mathrm{I}}$ là một họ tập hợp, và với mỗi $\iota \in \mathrm{I}$, cho $\mathscr{S}_\iota$ là một cấu trúc thuộc loài $\Sigma$ trên $\mathrm{A}_\iota$, và cho $f_\iota$ là một ánh xạ từ một tập hợp E vào $\mathrm{A}_\iota$. Giả sử rằng trên tập hợp tích $\mathrm{A} = \prod_{\iota \in \mathrm{J}} \mathrm{A}_\iota$ tồn tại một cấu trúc tích $\mathscr{S}$ của họ $(\mathscr{S}_\iota)_{\iota \in \mathrm{I}}$. Khi đó tồn tại một cấu trúc ban đầu đối với họ $(\mathrm{A}_\iota, \mathscr{S}_\iota, f_\iota)_{\iota \in \mathrm{I}}$ nếu và chỉ nếu cấu trúc $\mathscr{S}$ có một ảnh ngược qua ánh xạ $x \to f(x) = (f_\iota(x))$ từ E vào A, và khi đó hai cấu trúc này đồng nhất.*

Vì $f_\iota = \mathrm{pr}_\iota \circ f$, tiêu chuẩn này là một trường hợp riêng của CST10.

#### Nhận xét {#ens-iv-s2-n4-rem-1 .statement tag=03VU}

Cho $(\mathscr{S}_\lambda)_{\lambda \in \mathrm{L}}$ là một họ các cấu trúc thuộc loài $\Sigma$ trên *cùng một* tập hợp A; ký hiệu $\mathrm{A}_\lambda$ là tập hợp A được trang bị cấu trúc $\mathscr{S}_\lambda$, và ký hiệu $\mathrm{I}_\lambda$ là ánh xạ đồng nhất từ A vào $\mathrm{A}_\lambda$. Đặt B là tập hợp tích $\mathrm{A}^{\mathrm{L}} = \prod_{\lambda \in \mathrm{L}} \mathrm{A}_\lambda$, và $\Delta$ là đường chéo của tích này (Chương II, § 5, số 3). Gọi $h$ là ánh xạ đường chéo từ A lên $\Delta$, sao cho $h(x)$ là phần tử $(x_\lambda)_{\lambda \in \mathrm{L}}$ thỏa mãn $x_\lambda = x$ với mọi $\lambda \in \mathrm{L}$. Giả sử rằng trên B tồn tại một cấu trúc tích $\mathscr{S}'$ của họ $(\mathscr{S}_\lambda)$. Vì $h$ là đơn ánh, tiêu chuẩn CST 15 cho thấy rằng tồn tại một cấu trúc ban đầu $\mathscr{S}$ đối với họ $(\mathrm{A}_\lambda, \mathscr{S}_\lambda, \mathrm{I}_\lambda)_{\lambda \in \mathrm{L}}$ nếu và chỉ nếu tồn tại một cấu trúc $\mathscr{S}''$ trên $\Delta$ được cảm sinh bởi $\mathscr{S}'$; khi đó $\mathscr{S}''$ đồng nhất với cấu trúc thu được bằng cách chuyển $\mathscr{S}$ lên $\Delta$ nhờ $h$. Đặc biệt, khi mọi cấu trúc $\mathscr{S}_\lambda$ đều đồng nhất, $h$ là một *đẳng cấu* từ A (được trang bị cấu trúc này) lên $\Delta$.

Ta còn có tiêu chuẩn sau đây :

CST16. *Cho $(\mathrm{A}_\iota)_{\iota \in \mathrm{I}}$, $(\mathrm{B}_\iota)_{\iota \in \mathrm{I}}$ là hai họ tập hợp được đánh chỉ số bởi cùng một tập hợp. Với mỗi $\iota \in \mathrm{I}$, cho $\mathscr{S}_\iota$ là một cấu trúc thuộc loài $\Sigma$ trên $\mathrm{A}_\iota$ và cho $\mathscr{S}'_\iota$ là một cấu trúc thuộc loài $\Sigma$ trên $\mathrm{B}_\iota$. Giả sử tồn tại trên $\mathrm{A} = \prod_{\iota \in \mathrm{I}} \mathrm{A}_\iota \left( \text{tương ứng trên } \mathrm{B} = \prod_{\iota \in \mathrm{I}} \mathrm{B}_\iota \right)$ một cấu trúc tích $\mathscr{S}$ (tương ứng $\mathscr{S}'$) của họ $(\mathscr{S}_\iota)$ (tương ứng $(\mathscr{S}'_\iota)$). Với mỗi $\iota \in \mathrm{I}$, cho $f_\iota$ là một cấu xạ từ $\mathrm{A}_\iota$ vào $\mathrm{B}_\iota$. Khi đó ánh xạ $f = (f_\iota)_{\iota \in \mathrm{I}}$ là một cấu xạ từ A vào B.*

Gọi $p_\iota$ (tương ứng $q_\iota$) là phép chiếu của A lên $\mathrm{A}_\iota$ (tương ứng của B lên $\mathrm{B}_\iota$). Khi đó ta có $q_\iota \circ f = f_\iota \circ p_\iota$. Vì $f_\iota$ và $p_\iota$ là các cấu xạ (tiêu chuẩn

CST9), $f_\iota \circ p_\iota$ là một cấu xạ theo $(\mathrm{MO_{II}})$; do đó $f$ là một cấu xạ theo (IN).

#### Chú ý {#ens-iv-s2-n4-rem-2 .statement tag=03VV}

Đối với phần lớn các cấu trúc thông dụng, điều kiện nêu trong CST 16 không những là đủ mà còn là cần thiết để $f$ là một cấu xạ (xem Bài tập 7). Đặc biệt, điều này đúng trong các hoàn cảnh sau đây (chẳng hạn, nếu $\Sigma$ là loài các cấu trúc thứ tự, \* hoặc loài các cấu trúc nhóm, hoặc loài các cấu trúc tôpô $_*$, v.v.; xem Bài tập 8) :

¶ Tồn tại một họ $(a_\iota)_{\iota \in \mathrm{I}}$ sao cho $a_\iota \in \mathrm{A}_\iota$ với mọi $\iota \in \mathrm{I}$ và sao cho, nếu ta đặt $r_\iota(x_\iota) = (y_\varkappa)$, trong đó $y_\iota = x_\iota$ và $y_\varkappa = a_\varkappa$ mỗi khi $\varkappa \neq \iota$, thì mỗi ánh xạ $r_\iota$ là một *cấu xạ* từ $\mathrm{A}_\iota$ vào A. Thật vậy, nếu $f = (f_\iota)$ là một cấu xạ từ A vào B, ta có thể viết $f_\iota = q_\iota \circ f \circ r_\iota$ với mọi $\iota \in \mathrm{I}$, và chỉ cần áp dụng $(\mathrm{MO_{II}})$.

¶ Chú ý rằng $r_\iota$ là một cấu xạ nếu điều kiện sau đây được thỏa mãn :

(a) Với mọi tập hợp E được trang bị một cấu trúc thuộc loài $\Sigma$, ánh xạ hằng $z \to a_\iota$ là một cấu xạ từ E vào $\mathrm{A}_\iota$; thật vậy, với mỗi $\varkappa \in \mathrm{I}$, $p_\varkappa \circ r_\iota$ là một cấu xạ từ $\mathrm{A}_\iota$ vào $\mathrm{A}_\varkappa$, vì đó là ánh xạ đồng nhất khi $\varkappa = \iota$, và là một ánh xạ hằng $z \to a_\varkappa$ khi $\varkappa \neq \iota$; do định nghĩa của cấu trúc tích, vậy nên $r_\iota$ là một cấu xạ từ $\mathrm{A}_\iota$ vào A.

¶ Các ví dụ được liệt kê ở trên không những thỏa mãn (a), mà còn thỏa mãn điều kiện sau:

(b) Trên mỗi tập hợp $\mathrm{A}'_\iota = \mathrm{A}_\iota \times \prod_{\varkappa \neq \iota} \{a_\varkappa\}$, cấu trúc $\mathscr{S}$ cảm sinh một cấu trúc thuộc loài $\Sigma$.

¶ Ký hiệu $p'_\iota$ là hạn chế của $p_\iota$ trên $\mathrm{A}'_\iota$. Nếu cả hai điều kiện (a) và (b) đều được thỏa mãn, thì $p'_\iota$ là một *đẳng cấu* từ $\mathrm{A}'_\iota$ lên $\mathrm{A}_\iota$. Thật vậy, vì $p'_\iota = p_\iota \circ j_\iota$, trong đó $j_\iota$ là đơn ánh chính tắc của $\mathrm{A}'_\iota$ vào A, nên $p'_\iota$ là một cấu xạ theo $(\mathrm{MO_{II}})$. Mặt khác ta có $r_\iota = j_\iota \circ \overset{-1}{p'_\iota}$; do đó $\overset{-1}{p'_\iota}$ là một cấu xạ từ $\mathrm{A}_\iota$ vào $\mathrm{A}'_\iota$ theo định nghĩa của cấu trúc cảm sinh.

Sau cùng, ta có tiêu chuẩn sau đây, tiêu chuẩn này đặc trưng các cấu xạ trong nhiều trường hợp :

CST17. *Cho* A *và* B *là hai tập hợp, được trang bị các cấu trúc* $\mathscr{S}_\mathrm{A}$, $\mathscr{S}_\mathrm{B}$ *thuộc cùng một loài* $\Sigma$. *Giả sử rằng trên* $\mathrm{A} \times \mathrm{B}$ *tồn tại cấu trúc* $\mathscr{S}_{\mathrm{A} \times \mathrm{B}}$, *là tích của* $\mathscr{S}_\mathrm{A}$ *và* $\mathscr{S}_\mathrm{B}$. *Cho* $f$ *là một ánh xạ từ* A *vào* B, *cho* F *là đồ thị của nó, và cho* $\pi$ *là song ánh* $x \to (x, f(x))$ *từ* A *lên* F. *Khi đó, để* $f$ *là một cấu xạ từ* A *vào* B, *điều kiện cần và đủ là trên* F *tồn tại một cấu trúc thuộc loài* $\Sigma$ *được cảm sinh bởi* $\mathscr{S}_{\mathrm{A} \times \mathrm{B}}$ *và, khi* F *được trang bị cấu trúc này,* $\pi$ *là một đẳng cấu từ* A *lên* F.

Để chứng minh tính đủ, gọi $j$ là đơn ánh chính tắc của F vào $\mathrm{A} \times \mathrm{B}$. Ta có thể viết $f = \mathrm{pr}_2 \circ j \circ \pi$, và khi đó, theo giả thiết, $f$ là hợp thành của ba cấu xạ.

¶ Để chứng minh tính cần thiết, gọi $\mathscr{S}_{\mathbf{F}}$ là cấu trúc thuộc loài $\Sigma$ thu được bằng cách chuyển cấu trúc $\mathscr{S}_{\mathbf{A}}$ sang F nhờ song ánh $\pi$ (§ 1, no. 5). Khi đó ta phải chỉ ra rằng $\mathscr{S}_{\mathbf{F}}$ được cảm sinh bởi $\mathscr{S}_{\mathbf{A} \times \mathbf{B}}$ trên F. Trước hết ta chú ý rằng $j$ là một cấu xạ từ F vào $\mathbf{A} \times \mathbf{B}$; thật vậy, $j \circ \pi$ là ánh xạ $x \to (x, f(x))$ từ A vào $\mathbf{A} \times \mathbf{B}$, do đó là một cấu xạ theo giả thiết đặt lên $f$ và theo định nghĩa của cấu trúc tích; vì thế, theo định nghĩa của cấu trúc $\mathscr{S}_{\mathbf{F}}$, $j$ là một cấu xạ. Còn phải chỉ ra rằng nếu E là một tập hợp được trang bị một cấu trúc thuộc loài $\Sigma$, và nếu $g$ là một ánh xạ từ E vào F sao cho $j \circ g$ là một cấu xạ từ E vào $\mathbf{A} \times \mathbf{B}$, thì $g$ là một cấu xạ; hay, tương đương, rằng $g_1 = \overset{-1}{\pi} \circ g$ là một cấu xạ từ E vào A. Nhưng vì $g_1 = \mathrm{pr}_1 \circ (j \circ g)$, điều này suy ra từ giả thiết và định nghĩa của cấu trúc tích.

### 5. CÁC CẤU TRÚC CUỐI

Xét một họ các tập hợp $(\mathbf{A}_\iota)_{\iota \in \mathbf{I}}$, mỗi tập hợp được trang bị một cấu trúc $\mathscr{S}_\iota$ thuộc loài $\Sigma$. Cho E là một tập hợp, và với mỗi $\iota \in \mathbf{I}$ cho $g_\iota$ là một ánh xạ *từ* $\mathbf{A}_\iota$ *vào* E. Một cấu trúc $\mathscr{T}$ thuộc loài $\Sigma$ trên E được gọi là một *cấu trúc cuối đối với họ* $(\mathbf{A}_\iota, \mathscr{S}_\iota, g_\iota)_{\iota \in \mathbf{I}}$ nếu nó có tính chất sau :

(FI) Với mọi tập hợp E′, mọi cấu trúc $\mathscr{S}'$ thuộc loài $\Sigma$ trên E, và mọi ánh xạ $f$ *từ* E *vào* E′, quan hệ

$$\text{``}f \text{ là một cấu xạ từ E vào E'''}$$

là *tương đương* với quan hệ

$$\text{``với mọi } \iota \in \mathbf{I}, f \circ g_\iota \text{ là một cấu xạ từ } \mathbf{A}_\iota \text{ vào E'''}.$$

CST18. *Nếu tồn tại một cấu trúc cuối trên* E *đối với họ* $(\mathbf{A}_\iota, \mathscr{S}_\iota, g_\iota)_{\iota \in \mathbf{I}}$, *thì đó là cấu trúc mịn nhất thuộc loài* $\Sigma$ *trên* E *mà đối với nó mỗi ánh xạ* $g_\iota$ *đều là một cấu xạ, và do đó là duy nhất.*

Cho $\mathscr{T}$ là một cấu trúc cuối trên E, và cho $\mathscr{S}$ là một cấu trúc thuộc loài $\Sigma$ trên E sao cho mỗi $g_\iota$ là một cấu xạ. Nếu $i$ ký hiệu ánh xạ đồng nhất từ E, được trang bị $\mathscr{T}$, lên E, được trang bị $\mathscr{S}$, thì $i \circ g_\iota$ là một cấu xạ với mọi $\iota \in \mathbf{I}$. Khi đó điều kiện (FI) cho thấy rằng $i$ là một cấu xạ, điều đó có nghĩa (số 2) là $\mathscr{S}$ *thô hơn* $\mathscr{T}$. Áp dụng lại (FI) cho trường hợp trong đó $f$ là ánh xạ đồng nhất của E (được trang bị $\mathscr{T}$) lên chính nó, ta thấy (dùng $(\mathrm{MO_{III}})$) rằng mỗi $g_\iota$ là một cấu xạ từ $\mathbf{A}_\iota$ vào E. Điều này hoàn tất chứng minh.

Có thể xảy ra là tồn tại một cấu trúc thuộc loài $\Sigma$ trên E là cấu trúc mịn nhất trong tất cả các cấu trúc thuộc loài $\Sigma$ trên E mà đối với chúng các $g_\iota$ là các cấu xạ, nhưng cấu trúc này lại không phải là cấu trúc cuối cùng đối với họ $(\mathbf{A}_\iota, \mathscr{S}_\iota, g_\iota)$ (Bài tập 6).

Ta có *tiêu chuẩn tính bắc cầu* sau :

CST19. *Cho* E *là một tập hợp, cho* $(\mathrm{A}_\iota)_{\iota \in \mathrm{I}}$ *là một họ các tập hợp, và với mỗi* $\iota \in \mathrm{I}$ *cho* $\mathscr{S}_\iota$ *là một cấu trúc thuộc loài* $\Sigma$ *trên* $\mathrm{A}_\iota$. *Cho* $(\mathrm{J}_\lambda)_{\lambda \in \mathrm{L}}$ *là một phân hoạch của* I, *và cho* $(\mathrm{B}_\lambda)_{\lambda \in \mathrm{L}}$ *là một họ các tập hợp được đánh chỉ số bởi* L. *Với mỗi* $\lambda \in \mathrm{L}$, *cho* $h_\lambda$ *là một ánh xạ của* $\mathrm{B}_\lambda$ *vào* E; *với mỗi* $\lambda \in \mathrm{L}$ *và mỗi* $\iota \in \mathrm{J}_\lambda$, *cho* $g_{\iota\lambda}$ *là một ánh xạ của* $\mathrm{A}_\iota$ *vào* $\mathrm{B}_\lambda$, *và đặt* $f_\iota = h_\lambda \circ g_{\iota\lambda}$. *Giả sử rằng, với mỗi* $\lambda \in \mathrm{L}$, *tồn tại một cấu trúc cuối cùng* $\mathscr{S}'_\lambda$ *trên* $\mathrm{B}_\lambda$ *đối với họ* $(\mathrm{A}_\iota,\ \mathscr{S}_\iota,\ g_{\iota\lambda})_{\iota \in \mathrm{J}_\lambda}$. *Khi đó các mệnh đề sau là tương đương* :

(a) *Tồn tại một cấu trúc cuối* $\mathscr{S}$ *trên* E *đối với họ* $(\mathrm{A}_\iota, \mathscr{S}_\iota, f_\iota)_{\iota \in \mathrm{I}}$.

(b) *Tồn tại một cấu trúc cuối* $\mathscr{S}'$ *trên* E *đối với họ* $(\mathrm{B}_\lambda, \mathscr{S}'_\lambda, h_\lambda)_{\lambda \in \mathrm{L}}$.

*Hơn nữa các mệnh đề này kéo theo rằng* $\mathscr{S} = \mathscr{S}'$.

Cho F là một tập hợp được trang bị một cấu trúc thuộc loài $\Sigma$, và cho $u$ là một ánh xạ từ E vào F. Theo định nghĩa, quan hệ "$u \circ h_\lambda$ là một cấu xạ từ $\mathrm{B}_\lambda$ vào F" là tương đương với quan hệ

"với mọi $\iota \in \mathrm{J}_\lambda$, $u \circ h_\lambda \circ g_{\iota\lambda} = u \circ f_\iota$ là một cấu xạ từ $\mathrm{A}_\iota$ vào F".

Do đó quan hệ

(3)             "với mọi $\lambda \in \mathrm{L}$,   $u \circ h_\lambda$ là một cấu xạ từ $\mathrm{B}_\lambda$ vào F"

là tương đương với quan hệ

(4)             "với mọi $\iota \in \mathrm{I}$,   $u \circ f_i$ là một cấu xạ từ $\mathrm{A}_\iota$ vào F".

Nói rằng $\mathscr{S}'$ là cấu trúc cuối đối với họ $(\mathrm{B}_\lambda, \mathscr{S}'_\lambda, h_\lambda)_{\lambda \in \mathrm{L}}$ có nghĩa là quan hệ (3) tương đương với quan hệ "$u$ là một cấu xạ từ E (được trang bị $\mathscr{S}'$) vào F"; và nói rằng E là cấu trúc cuối đối với họ $(\mathrm{A}_\iota, \mathscr{S}_\iota, f_\iota)_{\iota \in \mathrm{I}}$ có nghĩa là quan hệ (4) tương đương với quan hệ "$u$ là một cấu xạ từ E (được trang bị $\mathscr{S}$) vào F"; do đó suy ra kết quả, xét đến tính chất về tính duy nhất của cấu trúc cuối.

### 6. CÁC VÍ DỤ VỀ CẤU TRÚC CUỐI

I. *Ảnh trực tiếp của một cấu trúc.*   Khi I là một tập hợp gồm một phần tử duy nhất, cấu trúc cuối đối với $(\mathrm{A}, \mathscr{S}, f)$ được gọi là *ảnh trực tiếp qua* $f$ *của cấu trúc* $\mathscr{S}$ (khi nó tồn tại).

II. *Cấu trúc thương.*   Cho A là một tập hợp được trang bị một cấu trúc $\mathscr{S}$ thuộc loài $\Sigma$, R là một quan hệ tương đương trên A, và $\varphi$ là ánh xạ

chính tắc từ A lên tập thương $\mathrm{E} = \mathrm{A}/\mathrm{R}$ (Chương II, § 6, no. 2). Ảnh trực tiếp của cấu trúc $\mathscr{S}$ qua ánh xạ $\varphi$ được gọi (khi nó tồn tại) là *thương* của cấu trúc $\mathscr{S}$ theo quan hệ R.

\* Nói chung, một cấu trúc thứ tự hoặc một cấu trúc đại số không thừa nhận cấu trúc thương đối với các quan hệ tương đương tùy ý (xem Chương III, § 1, Bài tập 2). Mặt khác, một tôpô luôn thừa nhận một cấu trúc thương đối với một quan hệ tương đương tùy ý, nhưng điều đó không tất yếu đúng đối với một tôpô Hausdorff. \*

Cho A, B là hai tập hợp tương ứng được trang bị các cấu trúc $\mathscr{S}$, $\mathscr{S}'$ thuộc loài $\Sigma$, và cho $f$ là một cấu xạ từ A vào B. Gọi R là quan hệ tương đương $f(x) = f(y)$, gọi $\varphi$ là ánh xạ chính tắc từ A lên $\mathrm{A}/\mathrm{R}$, và gọi $j$ là đơn ánh chính tắc từ $f(\mathrm{A})$ vào B. Giả sử rằng $\mathscr{S}$ thừa nhận một cấu trúc thương $\mathscr{S}_0$ đối với R, và rằng $\mathscr{S}'$ cảm sinh một cấu trúc $\mathscr{S}'_0$ trên $f(\mathrm{A})$. Khi đó, trong *phân tích chính tắc* $f = j \circ g \circ \varphi$ của $f$ (Chương II, § 6, số 5), song ánh $g$ từ $\mathrm{A}/\mathrm{R}$ lên $f(\mathrm{A})$ liên kết với $f$ là một *cấu xạ* (nhưng không nhất thiết là một đẳng cấu) khi $\mathrm{A}/\mathrm{R}$ được trang bị $\mathscr{S}_0$ và $f(\mathrm{A})$ được trang bị $\mathscr{S}'_0$. Thật vậy, $j \circ g$ là một cấu xạ từ $\mathrm{A}/\mathrm{R}$ vào B theo định nghĩa của cấu trúc thương, và do đó $g$ là một cấu xạ từ $\mathrm{A}/\mathrm{R}$ lên $f(\mathrm{A})$ theo định nghĩa của cấu trúc cảm sinh.

CST20. *Cho* A, A′ *là hai tập hợp được trang bị các cấu trúc* $\mathscr{S}$, $\mathscr{S}'$ *thuộc loài* $\Sigma$, *và cho* R (*tương ứng* R′) *là một quan hệ tương đương trên* A (*tương ứng* A′). *Giả sử tồn tại một cấu trúc thương* $\mathscr{S}_0$ (*tương ứng* $\mathscr{S}'_0$) *của* $\mathscr{S}$ *theo* R (*tương ứng của* $\mathscr{S}'$ *theo* R′). *Nếu* $f$ *là một cấu xạ từ* A *vào* A′ *tương thích với các quan hệ tương đương* R *và* R′, *và nếu* $g$ *là ánh xạ thu được từ* $f$ *bằng cách chuyển qua các thương, thì* $g$ *là một cấu xạ từ* $\mathrm{A}/\mathrm{R}$ *vào* $\mathrm{A}'/\mathrm{R}'$.

Gọi $\varphi$ (tương ứng, $\varphi'$) là ánh xạ chính tắc của A lên $\mathrm{A}/\mathrm{R}$ (tương ứng, của A′ lên $\mathrm{A}'/\mathrm{R}'$); khi đó ta có $g \circ \varphi = \varphi' \circ f$. Vì $\varphi'$ và $f$ là các cấu xạ, nên $\varphi' \circ f$ cũng là một cấu xạ theo ($\mathrm{MO_{II}}$). Nhưng khi đó, vì $g \circ \varphi$ là một cấu xạ, nên $g$ cũng là một cấu xạ theo định nghĩa của cấu trúc thương.

¶ Tiêu chuẩn tính bắc cầu CST19 đặc biệt dẫn đến tiêu chuẩn sau :

CST21. *Cho* A *là một tập hợp được trang bị một cấu trúc* $\mathscr{S}$ *thuộc loài* $\Sigma$, *và cho* R *là một quan hệ tương đương trên* A *sao cho tồn tại trên* $\mathrm{A}/\mathrm{R}$ *một cấu trúc thương* $\mathscr{S}'$ *của* $\mathscr{S}$ *theo* R. *Cho* S *là một quan hệ tương đương trên* A *thô hơn* R, *và cho* $\mathrm{S}/\mathrm{R}$ *ký hiệu quan hệ tương đương trên* $\mathrm{A}/\mathrm{R}$ *là quan hệ thương của* S *theo* R (Chương II, § 6, no. 7). *Khi đó tồn tại trên* $(\mathrm{A}/\mathrm{R})/(\mathrm{S}/\mathrm{R})$ *một cấu trúc thương* $\mathscr{S}''$ *của* $\mathscr{S}'$ *theo* $\mathrm{S}/\mathrm{R}$ *khi và chỉ khi tồn tại trên* $\mathrm{A}/\mathrm{S}$ *một cấu trúc thương* $\mathscr{S}_0$ *của* $\mathscr{S}$ *theo* S, *và ánh xạ chính tắc từ* $\mathrm{A}/\mathrm{S}$ (*được trang bị* $\mathscr{S}_0$) *lên* $(\mathrm{A}/\mathrm{R})/(\mathrm{S}/\mathrm{R})$ (*được trang bị* $\mathscr{S}''$) *là một đẳng cấu.*

Gọi $\varphi$ là ánh xạ chính tắc từ A lên $A/R$, và $\psi$ là ánh xạ chính tắc từ $A/R$ lên $(A/R)/(S/R)$. Theo CST19, $\mathscr{G}''$ là thương của $\mathscr{G}'$ theo $S/R$ khi và chỉ khi $\mathscr{G}''$ là cấu trúc cuối cùng đối với $(A,\mathscr{G},\psi\circ\varphi)$. Khi đó tiêu chuẩn suy ra từ việc quan hệ $\psi(\varphi(x))=\psi(\varphi(y))$ tương đương với S.

#### Nhận xét {#ens-iv-s2-n6-rem-1 .statement tag=03VW}

Cho A là một tập hợp được trang bị một cấu trúc $\mathscr{G}$ thuộc loài $\Sigma$, và cho R là một quan hệ tương đương trên A sao cho trên $E=A/R$ tồn tại một cấu trúc thương $\mathscr{G}'$ của $\mathscr{G}$ theo R. Gọi $\varphi$ là ánh xạ chính tắc từ A lên E. Nói chung, không tồn tại *tiết diện* $s$ nào của $\varphi$ (Chương II, § 3, no. 8) là một *cấu xạ* từ E vào A. Giả sử rằng có một tiết diện như vậy $s$, và hơn nữa rằng tồn tại một cấu trúc $\mathscr{G}''$ cảm sinh bởi $\mathscr{G}$ trên $s(E)$. Khi đó, nếu $j$ ký hiệu đơn ánh chính tắc từ $s(E)$ vào A và nếu $s=j\circ f$, thì song ánh $f$ là một *đẳng cấu* từ E lên $s(E)$. Thật vậy, $f$ là một cấu xạ theo định nghĩa của cấu trúc cảm sinh, và $g=\varphi\circ j$ là một cấu xạ từ $s(E)$ lên E do (MO$_{\mathrm{II}}$). Vì $g\circ f$ và $f\circ g$ lần lượt là các ánh xạ đồng nhất của E và của $s(E)$, nên mệnh đề là một hệ quả của CST8.

### Bài tập {#ens-iv-s2-exercises}

Xem [bài tập cho § 2](exercises/s2/).
