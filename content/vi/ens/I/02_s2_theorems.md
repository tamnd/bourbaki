---
book: ens
book_title: Theory of Sets
chapter: I
chapter_title: DESCRIPTION OF FORMAL MATHEMATICS
section: 2
section_title: Theorems
lang: vi
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 24-28, 56-57
pdf_pages: 0031-0035, 0063-0064
extraction: ocr
subsections:
    - "no": 1
      title: AXIOMS
      page: 24
      pdf_page: 31
    - "no": 2
      title: PROOFS
      page: 25
      pdf_page: 32
    - "no": 3
      title: SUBSTITUTIONS IN A THEORY
      page: 26
      pdf_page: 33
    - "no": 4
      title: COMPARISON OF THEORIES
      page: 26
      pdf_page: 33
statements: 1
exercises: 1
content_sha256: ca2ec1dd2433c47c4a52ac5e076a33047c5e082b1734212cf017c54adb277922
translated_from: content/en/ens/I/02_s2_theorems.md
source_content_sha256: c8b7ac12f220f9f720128bb004ee9ac705cf905ac08dfbc648d08a0ff3975ca7
translation_model: gpt-5.4-mini
translation_run: translate-vi-5cba219d
glossary_version: 34
glossary_terms_sha256: 63d4f24f6f0e16375df75bc3837477076a3192cb730e53023cc9f862a70cde9d
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 2. CÁC ĐỊNH LÝ

*Từ nay về sau, nếu $A$ là một quan hệ, ta sẽ viết not($A$) thay cho $\neg A$. Nếu $A$ và $B$ là các quan hệ, ta sẽ viết “($A$) or ($B$)” thay cho $\vee AB$, và ($A$) $\Rightarrow$ ($B$) thay cho $\Rightarrow AB$. Đôi khi ta sẽ bỏ các ngoặc. Trong mỗi trường hợp, người đọc sẽ có thể dễ dàng xác định cách ghép đang xét.*

### 1. CÁC TIÊN ĐỀ

Ta đã thấy rằng các ký hiệu đặc thù xác định các thuật ngữ và các quan hệ trong một lý thuyết $\mathscr{T}$. Để xây dựng $\mathscr{T}$, ta tiến hành như sau :

(1) Trước hết ta viết ra một số quan hệ trong $\mathscr{T}$; chúng được gọi là các *tiên đề tường minh* của $\mathscr{T}$. Các chữ cái xuất hiện trong các tiên đề tường minh được gọi là các *hằng số* của $\mathscr{T}$.

(2) Ta đặt ra một hay nhiều quy tắc [^1], gọi là các *lược đồ* của $\mathscr{T}$, và chúng phải có các tính chất sau: (a) việc áp dụng một quy tắc như vậy $\mathscr{R}$ cho ta một quan hệ trong $\mathscr{T}$; (b) nếu $T$ là một số hạng trong $\mathscr{T}$, nếu $x$ là một chữ cái, và nếu $R$ là một quan hệ trong $\mathscr{T}$ được xây dựng bằng cách áp dụng lược đồ $\mathscr{R}$, thì quan hệ $(T|x)R$ cũng có thể được xây dựng bằng cách áp dụng $\mathscr{R}$.

Trong mọi trường hợp mà ta xét đến, việc kiểm tra các điều kiện này luôn luôn dễ dàng.

Mỗi quan hệ được dựng bằng cách áp dụng một lược đồ của $\mathscr{T}$ được gọi là một *tiên đề ẩn* của $\mathscr{T}$.

Về mặt trực giác, các tiên đề hoặc biểu thị những mệnh đề hiển nhiên, hoặc là những giả thiết từ đó người ta muốn rút ra các hệ quả. Các hằng biểu thị những đối tượng được xác định rõ ràng mà các tính chất được diễn tả bởi các tiên đề tường minh được giả thiết là đúng. Mặt khác, nếu chữ $x$ không phải là một hằng, thì nó biểu thị một đối tượng hoàn toàn chưa xác định; nếu một tính chất của đối tượng $x$ được giả sử là đúng bằng một tiên đề, thì tiên đề đó tất yếu là ẩn, sao cho tính chất ấy vẫn đúng đối với mọi đối tượng $T$.

### 2. CHỨNG MINH

Một *văn bản chứng minh* trong một lý thuyết $\mathscr{T}$ gồm :

(1) Một phép dựng phụ trợ kiến tạo các quan hệ và các hạng trong $\mathscr{T}$.

(2) Một *chứng minh trong* $\mathscr{T}$, tức là một dãy các quan hệ trong $\mathscr{T}$ xuất hiện trong phép dựng kiến tạo phụ trợ, sao cho với mỗi quan hệ $\mathbf{R}$ trong dãy, ít nhất một trong các điều kiện sau được thỏa mãn :

(a$_1$) $\mathbf{R}$ là một tiên đề tường minh của $\mathscr{T}$.

(a$_2$) $\mathbf{R}$ được thu được từ việc áp dụng một lược đồ của $\mathscr{T}$ lên các hạng hoặc quan hệ xuất hiện trong phép dựng kiến tạo phụ trợ.

(b) có hai quan hệ $\mathbf{S}$, $\mathbf{T}$ trong dãy đứng trước $\mathbf{R}$, sao cho $\mathbf{T}$ là $\mathbf{S} \Rightarrow \mathbf{R}$.

¶ Một *định lý* trong $\mathscr{T}$ là một quan hệ *xuất hiện trong một chứng minh trong* $\mathscr{T}$.

Khái niệm này vì thế về thực chất phụ thuộc vào trạng thái của lý thuyết đang xét, vào thời điểm nó được mô tả. Một quan hệ trong một lý thuyết $\mathscr{T}$ *trở thành* một định lý trong $\mathscr{T}$ khi người ta thành công trong việc đưa nó vào một chứng minh trong $\mathscr{T}$. Nói rằng một quan hệ trong $\mathscr{T}$ "không phải là một định lý trong $\mathscr{T}$" không thể có bất kỳ ý nghĩa nào nếu không quy chiếu đến giai đoạn phát triển của lý thuyết $\mathscr{T}$.

Một định lý trong $\mathscr{T}$ cũng được gọi là một "*quan hệ đúng* trong $\mathscr{T}$" (hoặc "mệnh đề", "bổ đề", "hệ quả", v.v.). Cho $\mathbf{R}$ là một quan hệ trong $\mathscr{T}$, cho $\mathbf{x}$ là một chữ và $\mathbf{T}$ là một số hạng trong $\mathscr{T}$; nếu $(\mathbf{T}|\mathbf{x})\mathbf{R}$ là một định lý trong $\mathscr{T}$, thì $\mathbf{T}$ được gọi là *thỏa mãn quan hệ* $\mathbf{R}$ trong $\mathscr{T}$ (hay là một *nghiệm của* $\mathbf{R}$), khi $\mathbf{R}$ được xét như một quan hệ theo $\mathbf{x}$.

¶ Một quan hệ được nói là *sai* trong $\mathscr{T}$ nếu phủ định của nó là một định lý trong $\mathscr{T}$. Một lý thuyết $\mathscr{T}$ được nói là *mâu thuẫn* khi người ta đã viết ra một quan hệ vừa đúng vừa sai trong $\mathscr{T}$.

Ở đây một lần nữa, ta đang xét một khái niệm phụ thuộc vào trạng thái phát triển cụ thể của một lý thuyết. Người đọc nên đề phòng sự lẫn lộn (đáng tiếc là được gợi ra bởi nghĩa trực giác của từ "sai"), tức là tin rằng, một khi đã chứng minh một quan hệ $\mathbf{R}$ là sai trong $\mathscr{T}$, thì như thế đã xác lập rằng $\mathbf{R}$ "không đúng" trong $\mathscr{T}$ (nói chính xác, cụm từ này không có nghĩa chính xác *trong toán học*, như ta đã nhận xét ở trên).

¶ Trong phần tiếp theo, chúng ta sẽ nêu các tiêu chuẩn siêu toán học, gọi là *các tiêu chuẩn suy diễn*, cho phép rút gọn các chứng minh. Các tiêu chuẩn này sẽ được ký hiệu bởi chữ C theo sau bởi một số.

C1 (*Tam đoạn luận*). *Cho $\mathbf{A}$ và $\mathbf{B}$ là các quan hệ trong một lý thuyết $\mathscr{T}$. Nếu $\mathbf{A}$ và $\mathbf{A} \Rightarrow \mathbf{B}$ là các định lý trong $\mathscr{T}$, thì $\mathbf{B}$ là một định lý trong $\mathscr{T}$.*

Cho $R_1$, $R_2$, ..., $R_n$ là một chứng minh trong $\mathscr{T}$, trong đó $A$ xuất hiện, và cho $S_1$, $S_2$, ..., $S_p$ là một chứng minh trong $\mathscr{T}$, trong đó $A \Rightarrow B$ xuất hiện. Rõ ràng $R_1$, $R_2$, ..., $R_n$, $S_1$, $S_2$, ..., $S_p$ là một chứng minh trong $\mathscr{T}$, trong đó cả $A$ và $A \Rightarrow B$ đều xuất hiện. Suy ra

$$R_1, \; R_2, \; \ldots, \; R_n, \; S_1, \; S_2, \; \ldots, \; S_p, \; B$$

là một chứng minh trong $\mathscr{T}$, và do đó $B$ là một định lý trong $\mathscr{T}$.

### 3. CÁC PHÉP THAY THẾ TRONG MỘT LÝ THUYẾT

Cho $\mathscr{T}$ là một lý thuyết, cho $A_1$, $A_2$, ..., $A_n$ là các tiên đề tường minh của nó, cho $x$ là một chữ cái và $T$ là một số hạng của $\mathscr{T}$. Cho $(T|x)\mathscr{T}$ là lý thuyết có các ký hiệu và các sơ đồ giống như của $\mathscr{T}$, và có các tiên đề tường minh là $(T|x)A_1$, $(T|x)A_2$, ..., $(T|x)A_n$.

C2. *Cho $A$ là một định lý trong một lý thuyết $\mathscr{T}$, cho $T$ là một số hạng của $\mathscr{T}$, và cho $x$ là một chữ cái. Khi đó $(T|x)A$ là một định lý trong lý thuyết $(T|x)\mathscr{T}$.

Cho $R_1$, $R_2$, ..., $R_n$ là một chứng minh trong $\mathscr{T}$ trong đó $A$ xuất hiện. Xét dãy $(T|x)R_1$, $(T|x)R_2$, ..., $(T|x)R_n$, là một dãy các quan hệ trong $\mathscr{T}$ theo CF8 (§ 1, no. 4). Ta sẽ chứng minh rằng dãy này là một chứng minh trong lý thuyết $(T|x)\mathscr{T}$; điều này sẽ xác lập tiêu chuẩn. Nếu $R_k$ là một tiên đề ẩn của $\mathscr{T}$, thì $(T|x)R_k$ lại là một tiên đề ẩn của $\mathscr{T}$ (no. 1) và do đó của $(T/x)\mathscr{T}$. Nếu $R_k$ là một tiên đề tường minh của $\mathscr{T}$, thì $(T|x)R_k$ là một tiên đề tường minh của $(T|x)\mathscr{T}$. Cuối cùng, nếu $R_k$ được đặt sau các quan hệ $R_i$ và $R_j$, trong đó $R_j$ là $R_i \Rightarrow R_k$, thì $(T|x)R_k$ được đặt sau $(T|x)R_i$ và $(T|x)R_j$, và quan hệ sau đồng nhất với $(T|x)R_i \Rightarrow (T|x)R_k$ (criterion CS5).

C3. *Cho $A$ là một định lý của một lý thuyết $\mathscr{T}$, cho $T$ là một số hạng của $\mathscr{T}$, và cho $x$ là một chữ cái không phải là một hằng của $\mathscr{T}$. Khi đó $(T|x)A$ là một định lý của $\mathscr{T}$.*

Điều này suy ra ngay lập tức từ C2, vì $x$ không xuất hiện trong các tiên đề tường minh của $\mathscr{T}$. Cụ thể hơn, nếu $\mathscr{T}$ không chứa tiên đề tường minh nào, hoặc nếu các tiên đề tường minh không chứa chữ cái nào, thì tiêu chuẩn C3 áp dụng mà không có hạn chế đối với chữ cái $x$.

### 4. SO SÁNH CÁC LÝ THUYẾT

A lý thuyết $\mathscr{T}'$ được gọi là *mạnh hơn* một lý thuyết $\mathscr{T}$ nếu mọi ký hiệu của $\mathscr{T}$ đều là ký hiệu của $\mathscr{T}'$, mọi tiên đề tường minh của $\mathscr{T}$ đều là định lý trong $\mathscr{T}'$, và các lược đồ của $\mathscr{T}$ là các lược đồ của $\mathscr{T}'$.

C4. *Nếu một lý thuyết $\mathscr{T}'$ mạnh hơn một lý thuyết $\mathscr{T}$, thì mọi định lý của $\mathscr{T}$ đều là định lý của $\mathscr{T}'$.*

Cho $R_1$, $R_2$, ..., $R_n$ là một chứng minh trong $\mathscr{T}$. Ta sẽ chỉ ra, từng bước, rằng mỗi $R_i$ là một định lý trong $\mathscr{T}'$. Giả sử điều này đúng với các quan hệ đứng trước $R_k$. Nếu $R_k$ là một tiên đề của $\mathscr{T}$, thì nó là một định lý trong $\mathscr{T}'$ theo giả thiết. Nếu $R_k$ được đặt sau các quan hệ $R_i$ và $R_i \Rightarrow R_k$, ta đã biết rằng $R_i$ và $R_i \Rightarrow R_k$ là các định lý trong $\mathscr{T}'$, và do đó $R_k$ là một định lý trong $\mathscr{T}'$ nhờ C1. Vì thế, trong mọi trường hợp, $R_k$ là một định lý trong $\mathscr{T}'$, và chứng minh là đầy đủ.

Nếu mỗi một trong hai lý thuyết $\mathscr{T}$ và $\mathscr{T}'$ đều mạnh hơn lý thuyết kia, thì $\mathscr{T}$ và $\mathscr{T}'$ được gọi là *tương đương*. Khi đó mọi định lý của $\mathscr{T}$ đều là định lý của $\mathscr{T}'$, và ngược lại.

C5. *Cho $\mathscr{T}$ là một lý thuyết, cho $A_1$, $A_2$, ..., $A_n$ là các tiên đề tường minh của nó, $a_1$, $a_2$, ..., $a_h$ là các hằng của nó, và cho $T_1$, $T_2$, ..., $T_h$ là các hạng trong $\mathscr{T}$. Giả sử rằng*

$$(T_1|a_1) \, (T_2|a_2) \, \ldots \, (T_h|a_h)A_i \qquad (\text{cho} \quad i = 1, 2, \ldots, n)$$

*là các định lý trong một lý thuyết $\mathscr{T}'$, rằng các ký hiệu của $\mathscr{T}$ là các ký hiệu của $\mathscr{T}'$, và rằng các lược đồ của $\mathscr{T}$ là các lược đồ của $\mathscr{T}'$. Khi đó, nếu $A$ là một định lý trong $\mathscr{T}$,*

$$(T_1|a_1) \, \ldots \, (T_h|a_h)A$$

*là một định lý trong $\mathscr{T}'$.*

Vì $\mathscr{T}'$ mạnh hơn lý thuyết $(T_1|a_1) \ldots (T_n|a_n) \mathscr{T}$, và ta có thể áp dụng C2 và C4.

Khi ta dùng thủ tục này để suy ra một định lý trong $\mathscr{T}'$ từ một định lý trong $\mathscr{T}$, ta nói rằng *ta đang áp dụng trong $\mathscr{T}'$ các kết quả của $\mathscr{T}$*. Về trực giác, các tiên đề của $\mathscr{T}$ biểu thị các tính chất của $a_1, a_2, ..., a_h$, và $A$ biểu thị một tính chất là một hệ quả của các tiên đề này. Nếu các đối tượng $T_1, T_2, ..., T_h$ trong $\mathscr{T}'$ có các tính chất được biểu thị bởi các tiên đề của $\mathscr{T}$, thì chúng cũng có tính chất $A$.

*Ví dụ, trong lý thuyết nhóm $\mathscr{T}$, các tiên đề tường minh chứa hai hằng số G và $\mu$ (nhóm và luật hợp thành). Trong lý thuyết tập hợp $\mathscr{T}'$, ta định nghĩa hai thuật ngữ: đường thẳng thực và phép cộng các số thực. Nếu ta thay các thuật ngữ này cho G và $\mu$ tương ứng trong các tiên đề tường minh của $\mathscr{T}$, ta thu được các định lý trong $\mathscr{T}'$. Hơn nữa, các sơ đồ và ký hiệu của $\mathscr{T}$ và $\mathscr{T}'$ là như nhau. Vì thế ta có thể "áp dụng các kết quả của lý thuyết nhóm cho nhóm cộng của các số thực". Ta nói rằng ta đã xây dựng một *mô hình* cho lý thuyết nhóm trong lý thuyết tập hợp. (Lưu ý rằng vì lý thuyết nhóm mạnh hơn lý thuyết tập hợp, ta cũng có thể áp dụng các kết quả của lý thuyết tập hợp cho lý thuyết nhóm.)*

#### Nhận xét {#ens-i-s2-n4-rem-1 .statement tag=03G7}

Dưới các giả thiết của C5, nếu lý thuyết $\mathscr{T}$ hóa ra là mâu thuẫn, thì điều đó cũng sẽ đúng với $\mathscr{T}'$. Vì nếu $A$ và "không phải $A$" là các định lý trong $\mathscr{T}$, thì $(T_1|a_1) \ldots (T_h|a_h)A$ và $\mathrm{not}(T_1|a_1) \ldots (T_h|a_h)A$ là các định lý trong $\mathscr{T}'$. \* Chẳng hạn, nếu lý thuyết các nhóm là mâu thuẫn, thì lý thuyết tập hợp cũng sẽ là mâu thuẫn. \*

### Bài tập {#ens-i-s2-exercises}

Xem [các bài tập cho § 2](exercises/s2/).

[^1]: Để cho ngắn gọn, các quy tắc này được biểu đạt bằng cách dùng các ký hiệu đã nhắc đến ở § 1, no. 1 (và đặc biệt là các chữ in nghiêng đậm); nhưng thật dễ tránh hoàn toàn việc dùng các ký hiệu này trong việc phát biểu các quy tắc (xem § 3, no. 1, chú ý (*) ở p. 28).
