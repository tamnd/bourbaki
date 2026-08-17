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
content_sha256: 4b716ccc24a6c8dd244f03c7a779ff0af9df1bf507cfc6541f6346a0ed55832f
translated_from: content/en/ens/I/02_s2_theorems.md
source_content_sha256: c8b7ac12f220f9f720128bb004ee9ac705cf905ac08dfbc648d08a0ff3975ca7
translation_model: hy3-free, gpt-5-6, laguna-s-2.1-free, gpt-5-6-mini
translation_run: translate-vi-66ad11cf
glossary_version: 27
glossary_terms_sha256: 428b3ca241c6c75dddf942f4ccb81e1f43311d46e51df6fb6e41a4897d25309b
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 2. CÁC ĐỊNH LÝ

*Từ nay về sau, nếu $A$ là một quan hệ, chúng ta sẽ viết không($A$) thay cho $\neg A$. Nếu $A$ và $B$ là các quan hệ, chúng ta sẽ viết “($A$) hoặc ($B$)” thay cho $\vee AB$, và ($A$) $\Rightarrow$ ($B$) thay cho $\Rightarrow AB$. Đôi khi chúng ta sẽ bỏ qua các dấu ngoặc. Trong mỗi trường hợp, độc giả sẽ có thể xác định mà không gặp khó khăn sự lắp ghép đang xét.*

### 1. CÁC TIÊN ĐỀ

Chúng ta đã thấy rằng các dấu đặc hiệu xác định các thuật ngữ và các quan hệ trong một lý thuyết $\mathscr{T}$. Để xây dựng $\mathscr{T}$, chúng ta tiến hành như sau :

(1) Trước hết, ta viết ra một số quan hệ trong $\mathscr{T}$; chúng được gọi là các *tiên đề tường minh* của $\mathscr{T}$. Các chữ cái xuất hiện trong các tiên đề tường minh được gọi là các *hằng* của $\mathscr{T}$.

(2) Ta đặt ra một hoặc nhiều quy tắc [^1], được gọi là các *lược đồ* của $\mathscr{T}$, và chúng phải có các tính chất sau đây : (a) áp dụng một quy tắc như vậy $\mathscr{R}$ cho ta một quan hệ trong $\mathscr{T}$; (b) nếu $T$ là một số hạng trong $\mathscr{T}$, nếu $x$ là một chữ cái, và nếu $R$ là một quan hệ trong $\mathscr{T}$ được xây dựng bằng cách áp dụng lược đồ $\mathscr{R}$, thì quan hệ $(T|x)R$ cũng có thể được xây dựng bằng cách áp dụng $\mathscr{R}$.

Trong tất cả các trường hợp mà ta xét, việc kiểm tra các điều kiện này luôn dễ dàng.

Mọi quan hệ được kiến tạo bằng cách áp dụng một lược đồ của $\mathscr{T}$ được gọi là một *tiên đề ngầm* của $\mathscr{T}$.

Một cách trực quan, các tiên đề đại diện cho hoặc là những khẳng định hiển nhiên, hoặc là những giả thiết mà từ đó người ta muốn rút ra các hệ quả. Các hằng số đại diện cho các đối tượng được định nghĩa rõ mà các tính chất được biểu diễn bởi các tiên đề tường minh được giả định là đúng. Mặt khác, nếu chữ cái $x$ không phải là một hằng số, thì nó đại diện cho một đối tượng hoàn toàn không xác định; nếu một tính chất của đối tượng $x$ được giả sử là đúng thông qua một tiên đề, thì tiên đề này tất yếu là ngầm, do đó tính chất vẫn đúng với bất kỳ đối tượng $T$ nào.

### 2. CHỨNG MINH

Một *văn bản chứng minh* trong một lý thuyết $\mathscr{T}$ gồm :

(1) Một phép dựng kiến tạo phụ của các quan hệ và thuật ngữ trong $\mathscr{T}$.

(2) Một *chứng minh trong* $\mathscr{T}$, nói cách khác là một dãy các quan hệ trong $\mathscr{T}$ xuất hiện trong phép dựng kiến tạo phụ, sao cho với mọi quan hệ $\mathbf{R}$ trong dãy đó ít nhất một trong các điều kiện sau được thỏa mãn :

(a$_1$) $\mathbf{R}$ là một tiên đề tường minh của $\mathscr{T}$.

(a$_2$) $\mathbf{R}$ có được từ việc áp dụng một lược đồ của $\mathscr{T}$ cho các thuật hạng hoặc các quan hệ xuất hiện trong phép dựng kiến tạo phụ.

(b) có hai quan hệ $\mathbf{S}$, $\mathbf{T}$ trong dãy đi trước $\mathbf{R}$, sao cho $\mathbf{T}$ là $\mathbf{S} \Rightarrow \mathbf{R}$.

¶ A *định lý* trong $\mathscr{T}$ là một quan hệ *xuất hiện trong một chứng minh trong* $\mathscr{T}$.

Khái niệm này do đó về bản chất phụ thuộc vào trạng thái của lý thuyết đang được xem xét tại thời điểm mô tả nó. Một quan hệ trong một lý thuyết $\mathscr{T}$ *trở thành* một định lý trong $\mathscr{T}$ khi thành công trong việc chèn nó vào một chứng minh trong $\mathscr{T}$. Để nói rằng một quan hệ trong $\mathscr{T}$ "không phải là một định lý trong $\mathscr{T}$" không thể có bất kỳ ý nghĩa nào nếu không có tham chiếu đến giai đoạn phát triển của lý thuyết $\mathscr{T}$.

Một định lý trong $\mathscr{T}$ còn được gọi là một quan hệ "*đúng* trong $\mathscr{T}$" (hoặc "mệnh đề", "bổ đề", "hệ quả", v.v.). Cho $\mathbf{R}$ là một quan hệ trong $\mathscr{T}$, $\mathbf{x}$ là một chữ và $\mathbf{T}$ là một số hạng trong $\mathscr{T}$; nếu $(\mathbf{T}|\mathbf{x})\mathbf{R}$ là một định lý trong $\mathscr{T}$, thì $\mathbf{T}$ được nói là *thỏa mãn quan hệ* $\mathbf{R}$ trong $\mathscr{T}$ (hoặc là một *nghiệm của* $\mathbf{R}$), khi $\mathbf{R}$ được xét như một quan hệ trong $\mathbf{x}$.

¶ Một quan hệ được gọi là *sai* trong $\mathscr{T}$ nếu phủ định của nó là một định lý trong $\mathscr{T}$. Một lý thuyết $\mathscr{T}$ được gọi là *mâu thuẫn* khi người ta đã viết một quan hệ vừa đúng vừa sai trong $\mathscr{T}$.

Ở đây cũng vậy, ta đang xét một khái niệm phụ thuộc vào trạng thái phát triển cụ thể của một lý thuyết. Người đọc cần cảnh giác với sự nhầm lẫn (đáng tiếc là do ý nghĩa trực giác của từ "sai" gợi ra), tức là tin rằng, một khi đã chứng minh một quan hệ $\mathbf{R}$ là sai trong $\mathscr{T}$, thì qua đó đã xác lập rằng $\mathbf{R}$ "không đúng" trong $\mathscr{T}$ (nói một cách chặt chẽ, cụm từ này không có ý nghĩa chính xác *trong toán học*, như đã nhận xét ở trên).

¶ Trong phần tiếp theo, chúng ta sẽ đưa ra các tiêu chuẩn siêu toán học, gọi là *các tiêu chuẩn suy diễn*, cho phép rút ngắn các chứng minh. Các tiêu chuẩn này sẽ được ký hiệu bằng chữ C theo sau bởi một số.

C1 (*Tam đoạn luận*). *Cho $\mathbf{A}$ và $\mathbf{B}$ là các quan hệ trong một lý thuyết $\mathscr{T}$. Nếu $\mathbf{A}$ và $\mathbf{A} \Rightarrow \mathbf{B}$ là các định lý trong $\mathscr{T}$, thì $\mathbf{B}$ là một định lý trong $\mathscr{T}$.*

Cho $R_1$, $R_2$, ..., $R_n$ là một chứng minh trong $\mathscr{T}$ trong đó $A$ xuất hiện, và cho $S_1$, $S_2$, ..., $S_p$ là một chứng minh trong $\mathscr{T}$ trong đó $A \Rightarrow B$ xuất hiện. Rõ ràng $R_1$, $R_2$, ..., $R_n$, $S_1$, $S_2$, ..., $S_p$ là một chứng minh trong $\mathscr{T}$ trong đó cả $A$ và $A \Rightarrow B$ xuất hiện. Do đó

$$R_1, \; R_2, \; \ldots, \; R_n, \; S_1, \; S_2, \; \ldots, \; S_p, \; B$$

là một chứng minh trong $\mathscr{T}$, và do đó $B$ là một định lý trong $\mathscr{T}$.

### 3. PHÉP THẾ TRONG MỘT LÝ THUYẾT

Cho $\mathscr{T}$ là một lý thuyết, $A_1$, $A_2$, ..., $A_n$ là các tiên đề rõ ràng của nó, $x$ là một ký tự và $T$ là một số hạng của $\mathscr{T}$. Gọi $(T|x)\mathscr{T}$ là lý thuyết mà các ký hiệu và lược đồ của nó giống như các ký hiệu và lược đồ của $\mathscr{T}$, và các tiên đề rõ ràng của nó là $(T|x)A_1$, $(T|x)A_2$, ..., $(T|x)A_n$.

C2. *Cho $A$ là một định lý trong một lý thuyết $\mathscr{T}$, cho $T$ là một số hạng của $\mathscr{T}$, và cho $x$ là một chữ cái. Khi đó $(T|x)A$ là một định lý trong lý thuyết $(T|x)\mathscr{T}$.*

Cho $R_1$, $R_2$, ..., $R_n$ là một chứng minh trong $\mathscr{T}$ trong đó $A$ xuất hiện. Xét dãy $(T|x)R_1$, $(T|x)R_2$, ..., $(T|x)R_n$, là một dãy các quan hệ trong $\mathscr{T}$ bởi lý do của CF8 (§ 1, no. 4). Chúng ta sẽ chứng minh rằng dãy này là một chứng minh trong lý thuyết $(T|x)\mathscr{T}$; điều này sẽ thiết lập tiêu chí. Nếu $R_k$ là một tiên đề ngầm của $\mathscr{T}$, thì $(T|x)R_k$ cũng là một tiên đề ngầm của $\mathscr{T}$ (no. 1) và do đó của $(T/x)\mathscr{T}$. Nếu $R_k$ là một tiên đề tường minh của $\mathscr{T}$, thì $(T|x)R_k$ là một tiên đề tường minh của $(T|x)\mathscr{T}$. Cuối cùng, nếu $R_k$ được đi trước bởi các quan hệ $R_i$ và $R_j$, trong đó $R_j$ là $R_i \Rightarrow R_k$, thì $(T|x)R_k$ được đi trước bởi $(T|x)R_i$ và $(T|x)R_j$, và phần sau này là giống với $(T|x)R_i \Rightarrow (T|x)R_k$ (tiêu chí CS5).

C3. *Cho $A$ là một **định lý** của một **lý thuyết** $\mathscr{T}$, cho $T$ là một **số hạng** của $\mathscr{T}$, và cho $x$ là một **chữ cái** mà không phải là **hằng số** của $\mathscr{T}$. Khi đó $(T|x)A$ là một **định lý** của $\mathscr{T}$.

Đây là hệ quả ngay lập tức từ C2, vì $x$ không xuất hiện trong các tiên đề tường mội của $\mathscr{T}$. Cụ thể hơn, nếu $\mathscr{T}$ không chứa tiên đề tường mội nào, hoặc nếu các tiên đề tường mội không chứa bất kỳ chữ cái nào, thì điều kiện C3 áp dụng mà không có sự hạn chế nào đối với chữ cái $x$.

### 4. SO SÁNH CÁC LÝ THUYẾT

Một lý thuyết $\mathscr{T}'$ được gọi là *mạnh hơn* một lý thuyết $\mathscr{T}$ nếu mọi ký hiệu của $\mathscr{T}$ đều là ký hiệu của $\mathscr{T}'$, mọi tiên đề tường minh của $\mathscr{T}$ đều là định lý trong $\mathscr{T}'$, và các lược đồ của $\mathscr{T}$ đều là các lược đồ của $\mathscr{T}'$.

C4. *Nếu một lý thuyết $\mathscr{T}'$ mạnh hơn một lý thuyết $\mathscr{T}$, thì mọi định lý của $\mathscr{T}$ đều là định lý của $\mathscr{T}'$.*

Cho $R_1$, $R_2$, ..., $R_n$ là một chứng minh trong $\mathscr{T}$. Ta sẽ chứng minh, từng bước một, rằng mỗi $R_i$ là một định lý trong $\mathscr{T}'$. Giả sử điều này đúng đối với các quan hệ đứng trước $R_k$. Nếu $R_k$ là một tiên đề của $\mathscr{T}$, thì nó là một định lý trong $\mathscr{T}'$ theo giả thiết. Nếu $R_k$ đứng sau các quan hệ $R_i$ và $R_i \Rightarrow R_k$, ta đã biết rằng $R_i$ và $R_i \Rightarrow R_k$ là các định lý trong $\mathscr{T}'$, và do đó $R_k$ là một định lý trong $\mathscr{T}'$ theo C1. Vì vậy, trong mọi trường hợp, $R_k$ là một định lý trong $\mathscr{T}'$, và chứng minh là đầy đủ.

Nếu mỗi một trong hai lý thuyết $\mathscr{T}$ và $\mathscr{T}'$ mạnh hơn lý thuyết kia, thì $\mathscr{T}$ và $\mathscr{T}'$ được gọi là *tương đương*. Khi đó mọi định lý của $\mathscr{T}$ đều là một định lý của $\mathscr{T}'$, và ngược lại.

C5. *Cho $\mathscr{T}$ là một lý thuyết, cho $A_1$, $A_2$, ..., $A_n$ là các tiên đề tường minh của nó, $a_1$, $a_2$, ..., $a_h$ là các hằng số của nó, và cho $T_1$, $T_2$, ..., $T_h$ là các số hạng trong $\mathscr{T}$. Giả sử rằng*

$$(T_1|a_1) \, (T_2|a_2) \, \ldots \, (T_h|a_h)A_i \qquad (\text{đối với} \quad i = 1, 2, \ldots, n)$$

*là các định lý trong một lý thuyết $\mathscr{T}'$, rằng các ký hiệu của $\mathscr{T}$ là ký hiệu của $\mathscr{T}'$, và rằng các lược đồ của $\mathscr{T}$ là lược đồ của $\mathscr{T}'$. Khi đó, nếu $A$ là một định lý trong $\mathscr{T}$,*

$$(T_1|a_1) \, \ldots \, (T_h|a_h)A$$

*là một định lý trong $\mathscr{T}'$.*

Bởi vì $\mathscr{T}'$ mạnh hơn lý thuyết $(T_1|a_1) \ldots (T_n|a_n) \mathscr{T}$, và ta có thể áp dụng C2 và C4.

Khi dùng thủ tục này để suy ra một định lý trong $\mathscr{T}'$ từ một định lý trong $\mathscr{T}$, ta nói rằng *ta áp dụng trong $\mathscr{T}'$ các kết quả của $\mathscr{T}$. Về trực giác, các tiên đề của $\mathscr{T}$ biểu thị các tính chất của $a_1, a_2, ..., a_h$, và $A$ biểu thị một tính chất là hệ quả của các tiên đề này. Nếu các đối tượng $T_1, T_2, ..., T_h$ trong $\mathscr{T}'$ có các tính chất được biểu thị bởi các tiên đề của $\mathscr{T}$, thì chúng cũng có tính chất $A$.

\*Ví dụ, trong lý thuyết nhóm $\mathscr{T}$, các tiên đề tường minh chứa hai hằng G và $\mu$ (nhóm và luật hợp thành). Trong lý thuyết tập hợp $\mathscr{T}'$, ta định nghĩa hai thuật ngữ: dòng thực và phép cộng các số thực. Nếu thay lần lượt các thuật ngữ này cho G và $\mu$ trong các tiên đề tường minh của $\mathscr{T}$, ta thu được các định lý trong $\mathscr{T}'$. Hơn nữa, các sơ đồ và dấu hiệu của $\mathscr{T}$ và $\mathscr{T}'$ là như nhau. Do đó ta có thể "áp dụng các kết quả của lý thuyết nhóm cho nhóm cộng các số thực". Ta nói rằng ta đã xây dựng một *mô hình* của lý thuyết nhóm trong lý thuyết tập hợp. (Lưu ý rằng vì lý thuyết nhóm mạnh hơn lý thuyết tập hợp, ta cũng có thể áp dụng các kết quả của lý thuyết tập hợp cho lý thuyết nhóm.)\*

#### Nhận xét {#ens-i-s2-n4-rem-1 .statement tag=03G7}

Dưới các giả thiết của C5, nếu lý thuyết $\mathscr{T}$ hóa ra là mâu thuẫn, thì điều tương tự sẽ đúng với $\mathscr{T}'$. Bởi vì nếu $A$ và "không $A$" là các định lý trong $\mathscr{T}$, thì $(T_1|a_1) \ldots (T_h|a_h)A$ và $\mathrm{not}(T_1|a_1) \ldots (T_h|a_h)A$ là các định lý trong $\mathscr{T}'$. \* Ví dụ, nếu lý thuyết nhóm mâu thuẫn, thì lý thuyết tập hợp cũng sẽ mâu thuẫn. \*

### Bài tập {#ens-i-s2-exercises}

Xem các [bài tập cho § 2](exercises/s2/).

[^1]: Để ngắn gọn, các quy tắc này được diễn đạt bằng cách sử dụng các ký hiệu được nhắc đến trong § 1, no. 1 (và đặc biệt là các chữ in nghiêng đậm); nhưng sẽ dễ dàng tránh hoàn toàn việc sử dụng các ký hiệu này trong việc hình thành các quy tắc (xem § 3, no. 1, chú ý (*) trên p. 28).
