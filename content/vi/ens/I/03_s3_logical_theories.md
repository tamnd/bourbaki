---
book: ens
book_title: Theory of Sets
chapter: I
chapter_title: DESCRIPTION OF FORMAL MATHEMATICS
section: 3
section_title: Logical theories
lang: vi
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 28-36, 57-58
pdf_pages: 0035-0043, 0064-0065
extraction: ocr
subsections:
    - "no": 1
      title: THE AXIOMS
      page: 28
      pdf_page: 35
    - "no": 2
      title: FIRST CONSEQUENCES
      page: 29
      pdf_page: 36
    - "no": 3
      title: METHODS OF PROOF
      page: 30
      pdf_page: 37
    - "no": 4
      title: CONJUNCTION
      page: 33
      pdf_page: 40
    - "no": 5
      title: EQUIVALENCE
      page: 34
      pdf_page: 41
statements: 0
exercises: 5
content_sha256: 898a330261649cb8d4f4b7e8b9e78a59ef708baf1ebaf978d5bbaa703df57e1a
translated_from: content/en/ens/I/03_s3_logical_theories.md
source_content_sha256: b429aa448e801f5e6c98174f23720386650518026195c14d31873c2ba51f7dd2
translation_model: gpt-5.4
translation_run: translate-vi-7032b096
glossary_version: 29
glossary_terms_sha256: b6629014b0a25ad61d0aa69b0db5f7f32f3a39e7a06633719ad49f44fcde8175
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 3. CÁC LÝ THUYẾT LOGIC

### 1. CÁC TIÊN ĐỀ

Một *lý thuyết lôgic* là một lý thuyết bất kỳ $\mathscr{T}$ trong đó các lược đồ S1 đến S4 dưới đây cho các tiên đề ẩn.

S1. *Nếu $A$ là một quan hệ trong $\mathscr{T}$, thì quan hệ $(A$ hoặc $A) \Rightarrow A$ là một tiên đề của $\mathscr{T}$* (\*)[^1].

S2. *Nếu $A$ và $B$ là các quan hệ trong $\mathscr{T}$, thì quan hệ $A \Rightarrow (A$ hoặc $B)$ là một tiên đề của $\mathscr{T}$.*

S3. *Nếu $A$ và $B$ là các quan hệ trong $\mathscr{T}$, thì quan hệ $(A$ hoặc $B) \Rightarrow (B$ hoặc $A)$ là một tiên đề của $\mathscr{T}$.*

S4. *Nếu $A$, $B$ và $C$ là các quan hệ trong $\mathscr{T}$, thì quan hệ*

$$(A \Rightarrow B) \Rightarrow ((C \text{ hoặc } A) \Rightarrow (C \text{ hoặc } B))$$

*là một tiên đề của $\mathscr{T}$.*

Thực vậy, những quy tắc này là các lược đồ; chẳng hạn, hãy kiểm tra điều đó đối với S2. Cho $R$ là một quan hệ thu được bằng cách áp dụng S2; khi đó tồn tại các quan hệ $A$ và $B$ trong $\mathscr{T}$ sao cho $R$ là quan hệ $A \Rightarrow (A$ hoặc $B)$. Cho $T$ là một số hạng trong $\mathscr{T}$, cho $x$ là một chữ cái, và cho $A'$ và $B'$ là các quan hệ $(T|x)A$ và $(T|x)B$; khi đó $(T|x)R$ cũng chính là $A' \Rightarrow (A'$ hoặc $B')$, và vì thế có thể thu được bằng cách áp dụng S2.

Về mặt trực giác, các quy tắc S1 đến S4 chỉ đơn thuần diễn đạt ý nghĩa được gắn cho các từ "hoặc" và "suy ra" trong ngôn ngữ toán học thông thường (†)[^2].

Nếu một lý thuyết lôgic $\mathscr{T}$ là mâu thuẫn, *mọi quan hệ trong $\mathscr{T}$ đều là định lý trong $\mathscr{T}$.* Thật vậy, cho $A$ là một quan hệ của $\mathscr{T}$ sao cho $A$ và "không $A$" là các định lý trong $\mathscr{T}$, và cho $B$ là một quan hệ bất kỳ của $\mathscr{T}$. Theo S2, (không $A$) $\Rightarrow$ ((không $A$) hoặc $B$) là một định lý của $\mathscr{T}$; do đó, theo C1 (§ 2, no. 2), "(không $A$) hoặc $B$", tức là $A \Rightarrow B$, là một định lý của $\mathscr{T}$. Áp dụng C1 lần thứ hai cho thấy $B$ là một định lý của $\mathscr{T}$.

¶ *Từ nay về sau $\mathscr{T}$ sẽ ký hiệu một lý thuyết lôgic.*

### 2. CÁC HỆ QUẢ ĐẦU TIÊN

C6. *Cho $A$, $B$, $C$ là các quan hệ trong $\mathscr{T}$. Nếu $A \Rightarrow B$ và $B \Rightarrow C$ là các định lý trong $\mathscr{T}$, thì $A \Rightarrow C$ là một định lý trong $\mathscr{T}$.*

Vì $(B \Rightarrow C) \Rightarrow ((A \Rightarrow B) \Rightarrow (A \Rightarrow C))$ là một tiên đề của $\mathscr{T}$, theo S4 khi thay thế $A$ bởi $B$, $B$ bởi $C$, và $C$ bởi "không $A$". Theo C1 (§ 2, no. 2), $(A \Rightarrow B) \Rightarrow (A \Rightarrow C)$ là một định lý trong $\mathscr{T}$. Một lần áp dụng nữa của C1 hoàn tất chứng minh.

C7. *Nếu $A$ và $B$ là các quan hệ trong $\mathscr{T}$, thì $B \Rightarrow (A$ hoặc $B)$ là một định lý trong $\mathscr{T}$.*

Vì $B \Rightarrow (B$ hoặc $A)$ và $(B$ hoặc $A) \Rightarrow (A$ hoặc $B)$ là các tiên đề của $\mathscr{T}$ theo S2 và S3. Bây giờ dùng C6.

C8. *Nếu $A$ là một quan hệ trong $\mathscr{T}$, thì $A \Rightarrow A$ là một định lý trong $\mathscr{T}$.*

Vì $A \Rightarrow (A$ hoặc $A)$ và $(A$ hoặc $A) \Rightarrow A$ là các tiên đề, theo S2 và S1. Bây giờ dùng C6.

C9. *Nếu $A$ là một quan hệ và $B$ là một định lý trong $\mathscr{T}$, thì $A \Rightarrow B$ là một định lý trong $\mathscr{T}$.*

Vì $B \Rightarrow ((\text{không } A)$ hoặc $B)$ là một định lý theo C7, và do đó "(không $A$) hoặc $B$", tức là $A \Rightarrow B$, là một định lý theo C1.

C10. *Nếu $A$ là một quan hệ trong $\mathscr{T}$, thì "$A$ hoặc (không $A$)" là một định lý trong $\mathscr{T}$.*

Vì "(không $A$) hoặc $A$" là một định lý theo C8; bây giờ dùng S3 và C1.

C11. *Nếu $A$ là một quan hệ trong $\mathscr{T}$, thì "$A \Rightarrow$ (không không $A$)" là một định lý trong $\mathscr{T}$.*

Thật vậy, quan hệ này là "(không $A$) hoặc (không không $A$)", và kết quả suy ra từ C10.

C12. *Cho $A$ và $B$ là hai quan hệ trong $\mathscr{T}$. Khi đó quan hệ*

$$(A \Rightarrow B) \Rightarrow ((\text{không } B) \Rightarrow (\text{không } A))$$

*là một định lý trong $\mathscr{T}$.*

Thật vậy,

$$((\text{không } A) \text{ hoặc } B) \Rightarrow ((\text{không } A) \text{ hoặc } (\text{không không } B))$$

là một định lý, theo C11, S4 và C1. Mặt khác,

$$((\text{không } A) \text{ hoặc } (\text{không không } B)) \Rightarrow ((\text{không không } B) \text{ hoặc } (\text{không } A))$$

là một tiên đề, theo S3. Do đó

$$((\text{không } A) \text{ hoặc } B) \Rightarrow ((\text{không không } B) \text{ hoặc } (\text{không } A))$$

là một định lý theo C6. Suy ra kết quả.

C13. *Cho $A$, $B$, $C$ là các quan hệ trong $\mathscr{T}$. Nếu $A \Rightarrow B$ là một định lý trong $\mathscr{T}$, thì $(B \Rightarrow C) \Rightarrow (A \Rightarrow C)$ là một định lý trong $\mathscr{T}$.*

Vì $(\text{không } B) \Rightarrow (\text{không } A)$ là một định lý, theo C12 và C1. Do đó $(C \text{ hoặc } (\text{không } B)) \Rightarrow (C \text{ hoặc } (\text{không } A))$ là một định lý, theo S4 và C1. Bằng cách áp dụng kép S3 và C6, ta suy ra rằng

$$((\text{không } B) \text{ hoặc } C) \Rightarrow ((\text{không } A) \text{ hoặc } C)$$

là một định lý; nhưng đó là quan hệ đã cho.

¶ *Từ nay về sau, nói chung chúng tôi sẽ dùng* C1 *và* C6 *mà không dẫn chúng một cách tường minh.*

### 3. CÁC PHƯƠNG PHÁP CHỨNG MINH

I. *Phương pháp giả thiết phụ.* Phương pháp này dựa trên quy tắc sau :

C14 (*Tiêu chuẩn suy diễn*). *Cho $A$ là một quan hệ trong $\mathscr{T}$, và gọi $\mathscr{T}'$ là lý thuyết thu được bằng cách thêm $A$ vào các tiên đề của $\mathscr{T}$. Nếu $B$ là một định lý trong $\mathscr{T}'$, thì $A \Rightarrow B$ là một định lý trong $\mathscr{T}$.*

Cho $B_1$, $B_2$, ..., $B_n$ là một chứng minh trong $\mathscr{T}'$ trong đó $B$ xuất hiện. Ta sẽ chỉ ra, từng bước một, rằng các hệ thức $A \Rightarrow B_k$ là các định lý trong $\mathscr{T}$. Giả sử điều đó đã được thiết lập đối với các hệ thức đứng trước $B_i$, và hãy chỉ ra rằng $A \Rightarrow B_i$ là một định lý trong $\mathscr{T}$. Nếu $B_i$ là một tiên đề của $\mathscr{T}'$, thì $B_i$ hoặc là một tiên đề của $\mathscr{T}$ hoặc là $A$. Trong cả hai trường hợp, $A \Rightarrow B_i$ là một định lý trong $\mathscr{T}$ do áp dụng C9 hoặc C8. Nếu trước $B_i$ có các hệ thức $B_j$ và $B_j \Rightarrow B_i$, ta biết rằng $A \Rightarrow B_j$ và $A \Rightarrow (B_j \Rightarrow B_i)$ là các định lý trong $\mathscr{T}$. Do đó $(B_j \Rightarrow B_i) \Rightarrow (A \Rightarrow B_i)$ là một định lý trong $\mathscr{T}$ theo C13. Suy ra, theo C6, $A \Rightarrow (A \Rightarrow B_i)$, nghĩa là "$(\text{không } A)$ hoặc $(A \Rightarrow B_i)$", là một định lý trong $\mathscr{T}$, và do đó "$(A \Rightarrow B_i)$ hoặc $(\text{không } A)$" cũng là một định lý theo S3. Bây giờ, $(\text{không } A) \Rightarrow ((\text{không } A) \text{ hoặc } B_i)$, nghĩa là $(\text{không } A) \Rightarrow (A \Rightarrow B_i)$, là một định lý trong $\mathscr{T}$ theo S2. Do áp dụng S4 ta thấy khi đó rằng

$$((A \Rightarrow B_i) \text{ hoặc } (\text{không } A)) \Rightarrow ((A \Rightarrow B_i) \text{ hoặc } (A \Rightarrow B_i))$$

là một định lý trong $\mathscr{T}$, và do đó "$(A \Rightarrow B_i)$ hoặc $(A \Rightarrow B_i)$" là một định lý trong $\mathscr{T}$. Theo S1 ta kết luận rằng $A \Rightarrow B_i$ là một định lý trong $\mathscr{T}$.

Trong thực hành, ta chỉ ra rằng mình sẽ dùng tiêu chuẩn này bằng một câu như "giả sử $A$ là đúng". Câu này có nghĩa là tạm thời lập luận sẽ được tiến hành trong lý thuyết $\mathscr{T}'$, cho đến khi quan hệ $B$ đã được chứng minh. Khi điều này đã đạt được thì đã xác lập rằng $A \Rightarrow B$ là một định lý trong $\mathscr{T}$, và sau đó ta tiếp tục lập luận trong $\mathscr{T}$ mà nói chung không cần chỉ ra rằng mình đã rời bỏ lý thuyết $\mathscr{T}'$. Quan hệ $A$ được đưa vào như một tiên đề mới được gọi là *giả thiết phụ trợ*. \* Chẳng hạn, khi ta nói "cho $x$ là một số thực", ta đang xây dựng một lý thuyết trong đó quan hệ "$x$ là một số thực" là một giả thiết phụ trợ. \*

II. *Phương pháp phản chứng.* Phương pháp này dựa trên quy tắc sau :

C15. *Hãy cho $A$ là một quan hệ trong $\mathscr{T}$, và gọi $\mathscr{T}'$ là lý thuyết thu được bằng cách thêm tiên đề* "không $A$" *vào các tiên đề của $\mathscr{T}$. Nếu $\mathscr{T}'$ là mâu thuẫn, hãy chứng minh rằng $A$ là một định lý trong $\mathscr{T}$.*

Vì $A$ là một định lý trong $\mathscr{T}'$; do đó (phương pháp giả thiết phụ) "(không $A$) $\Rightarrow A$" là một định lý trong $\mathscr{T}$. Theo S4,

$$(A \text{ hoặc } (\text{không } A)) \Rightarrow (A \text{ hoặc } A)$$

là một định lý trong $\mathscr{T}$; theo C10, "$A$ hoặc $A$" là một định lý trong $\mathscr{T}$. Bây giờ áp dụng S1.

Trong thực hành, ta chỉ ra rằng mình sẽ dùng tiêu chuẩn này bằng một cụm từ như "giả sử $A$ là sai". Cụm từ này có nghĩa là tạm thời lập luận sẽ được tiến hành trong lý thuyết $\mathscr{T}'$, cho đến khi đã chứng minh được hai định lý dạng $B$ và "không $B$". Khi đã làm được điều đó thì suy ra rằng $A$ là một định lý trong $\mathscr{T}$, điều này nói chung được chỉ ra bằng một cụm từ như "Bây giờ điều này (tức là, theo ký hiệu ở trên, $B$ và "không $B$") là phi lý; do đó $A$ là đúng". Khi đó ta tiếp tục trong lý thuyết ban đầu $\mathscr{T}$.

¶ Như những áp dụng đầu tiên của các phương pháp này, hãy thiết lập các tiêu chuẩn sau :

C16. *Nếu $A$ là một quan hệ trong $\mathscr{T}$, thì* (không không $A$) $\Rightarrow A$ *là một định lý trong $\mathscr{T}$.*

Thật vậy, giả sử rằng "không không $A$" là đúng; khi đó ta phải chứng minh $A$. Giả sử $A$ là sai. Trong lý thuyết được định nghĩa như vậy, "không không $A$" và "không $A$" là các định lý, điều này là phi lý; do đó $A$ là đúng.

C17. *Nếu $A$ và $B$ là các quan hệ trong $\mathscr{T}$, thì*

$$((\text{không } B) \Rightarrow (\text{không } A)) \Rightarrow (A \Rightarrow B)$$

*là một định lý trong $\mathscr{T}$.*

Thật vậy, giả sử rằng $(\text{không phải }B) \Rightarrow (\text{không phải }A)$ là đúng. Ta phải chứng minh rằng $A \Rightarrow B$ là đúng. Giả sử $A$ là đúng, và ta hãy chứng minh rằng $B$ là đúng. Giả sử “không phải $B$” là đúng. Khi đó “không phải $A$” là đúng, điều này vô lý.

III. *Phương pháp phân biệt các trường hợp.* Phương pháp này dựa trên quy tắc sau :

C18. *Cho $A$, $B$, $C$ là các quan hệ trong $\mathscr{T}$. Nếu “$A$ hoặc $B$”, $A \Rightarrow C$, $B \Rightarrow C$ là các định lý trong $\mathscr{T}$, thì $C$ là một định lý trong $\mathscr{T}$.*

Thật vậy, theo S4, “$(A\text{ hoặc }B) \Rightarrow (A\text{ hoặc }C)$” và “$(C\text{ hoặc }A) \Rightarrow (C\text{ hoặc }C)$” là các định lý trong $\mathscr{T}$. Theo S3 và S1, suy ra rằng $(A\text{ hoặc }B) \Rightarrow C$ là một định lý trong $\mathscr{T}$; do đó có kết quả phải chứng minh.

Vì vậy, để chứng minh $C$ thì chỉ cần, khi ta có trong tay một định lý “$A$ or $B$”, trước hết chứng minh $C$ bằng cách thêm $A$ vào các tiên đề của $\mathscr{T}$, rồi chứng minh $C$ bằng cách thêm $B$ vào các tiên đề của $\mathscr{T}$. Đặc điểm đáng chú ý của phương pháp này nằm ở chỗ nếu “$A$ or $B$” là đúng thì nói chung ta không thể khẳng định rằng $A$ đúng hay $B$ đúng.

Đặc biệt, theo C10, nếu “$A \Rightarrow C$” và “$(\text{không }A) \Rightarrow C$” đều là các định lý trong $\mathscr{T}$, thì $C$ là một định lý trong $\mathscr{T}$.

IV. *Phương pháp hằng số phụ.* Phương pháp này dựa trên quy tắc sau :

C19. *Cho $x$ là một chữ và $A$ và $B$ là các quan hệ trong $\mathscr{T}$ sao cho :*

(1) *chữ cái $x$ không phải là một hằng số của $\mathscr{T}$ và không xuất hiện trong $B$;*
(2) *có một số hạng $T$ trong $\mathscr{T}$ sao cho $(T|x)A$ là một định lý trong $\mathscr{T}$.*

*Gọi $\mathscr{T}'$ là lý thuyết thu được bằng cách thêm $A$ vào các tiên đề của $\mathscr{T}$. Nếu $B$ là một định lý trong $\mathscr{T}'$, thì $B$ là một định lý trong $\mathscr{T}$.*

Quả thật, $A \Rightarrow B$ là một định lý trong $\mathscr{T}$ (tiêu chuẩn suy diễn). Vì $x$ không phải là một hằng số của $\mathscr{T}$, $(T|x)(A \Rightarrow B)$ là một định lý trong $\mathscr{T}$ theo C3. Vì $x$ không xuất hiện trong $B$, $(T|x)(A \Rightarrow B)$ đồng nhất với $((T|x)A) \Rightarrow B$, theo CS5 (§ 1, no. 2). Sau cùng, $(T|x)A$ là một định lý trong $\mathscr{T}$, và do đó $B$ cũng vậy.

Một cách trực giác, phương pháp này hệ tại việc dùng, để chứng minh $B$, một đối tượng tùy ý $x$ ( *hằng số phụ* ) được giả sử là được trang bị những tính chất nào đó, được ký hiệu bởi $A$. * Ví dụ, trong một chứng minh hình học có liên quan, cùng với những thứ khác, đến một đường thẳng $D$, ta có thể “lấy” một điểm $x$ trên đường thẳng này; khi đó quan hệ $A$ là $x \in D$. * Để có thể dùng một đối tượng được trang bị những tính chất nào đó trong quá trình một chứng minh, rõ ràng điều cần thiết là những đối tượng như vậy phải tồn tại. Định lý $(T|x)A$, được gọi là *định lý hợp thức hóa*, bảo đảm sự tồn tại này.

Trong thực hành, ta chỉ ra rằng ta sắp dùng phương pháp này bằng một câu như “cho $x$ là một đối tượng sao cho $A$”. Trái với phương pháp của giả thiết phụ, kết luận của lập luận không chứa $x$.

### 4. PHÉP HỘI

Cho $A$, $B$ là các dãy ký hiệu. Dãy ký hiệu

$$
\text{không } ((\text{không } A) \text{ hoặc } (\text{không } B))
$$

sẽ được ký hiệu bởi “$A$ và $B$”.

CS6.  Cho $A$, $B$, $T$ là các dãy ký hiệu và $x$ là một chữ cái.  Khi đó dãy ký hiệu

$$
(T|x)(A\text{ và }B)
$$

đồng nhất với “$(T|x)A$ và $(T|x)B$”.

Đây là một hệ quả ngay lập tức của CS5 (§ 1, no. 2).

CF9.  Nếu $A$, $B$ là các quan hệ trong $\mathscr{T}$, thì “$A$ và $B$” là một quan hệ trong $\mathscr{T}$ (được gọi là phép hội của $A$ và $B$).

Điều này suy ra ngay lập tức từ CF1 và CF2 (§ 1, no. 4).

C20.  Nếu $A$, $B$ là các định lý trong $\mathscr{T}$, thì “$A$ và $B$” là một định lý trong $\mathscr{T}$.

Giả sử rằng “$A$ và $B$” là sai, nghĩa là,

$$
\text{không phải không } ((\text{không } A) \text{ hoặc } (\text{không } B))
$$

là đúng. Theo C16, “$(\text{không } A)$ hoặc $(\text{không } B)$”, nghĩa là, $A \Longrightarrow (\text{không } B)$ là đúng, do đó “không $B$” là đúng; nhưng điều này là phi lý. Vậy “$A$ và $B$” là đúng.

C21. Nếu $A$, $B$ là các quan hệ trong $\mathscr{T}$, thì

$$
(A\text{ và }B) \Longrightarrow A,\qquad (A\text{ và }B) \Longrightarrow B
$$

là các định lý trong $\mathscr{T}$.

Các hệ thức $(\text{không } A) \Longrightarrow ((\text{không } A) \text{ hoặc } (\text{không } B))$, $(\text{không } B) \Longrightarrow ((\text{không } A) \text{ hoặc } (\text{không } B))$ là các định lý trong $\mathscr{T}$, theo S2 (no. 1) và C7 (no. 2).  Bây giờ $((\text{không } A) \text{ hoặc } (\text{không } B)) \Longrightarrow (\text{không } (A\text{ và }B))$ là một định lý trong $\mathscr{T}$ theo C11.  Do đó $(\text{không } A) \Longrightarrow (\text{không } (A\text{ và }B))$, $(\text{không } B) \Longrightarrow (\text{không } (A\text{ và }B))$ là các định lý trong $\mathscr{T}$.  Kết quả suy ra bằng cách áp dụng C17.

¶ Ta sẽ ký hiệu quan hệ "$A$ và $B$ và $C$" (tương ứng "$A$ hoặc $B$ hoặc $C$") để chỉ quan hệ "$A$ và ($B$ và $C$)" (tương ứng "$A$ hoặc ($B$ hoặc $C$)"). Nói chung hơn, nếu

$$A_1, \quad A_2, \quad \ldots, \quad A_n$$

là các quan hệ, ta ký hiệu bởi "$A_1$ và $A_2$, và ... và $A_p$" một quan hệ được xây dựng từng bước nhờ quy ước rằng "$A_1$ và $A_2$ và ... và $A_h$" biểu thị cùng một quan hệ như "$A_1$ và ($A_2$ và ... và $A_h$)". Quan hệ "$A_1$ hoặc $A_2$ hoặc ... hoặc $A_h$" được định nghĩa tương tự. Quan hệ "$A_1$ và $A_2$ và ... và $A_h$" là một định lý trong $\mathscr{T}$ khi và chỉ khi mỗi quan hệ $A_1$, $A_2$, ..., $A_h$ là một định lý trong $\mathscr{T}$.

Suy ra mọi lý thuyết lôgic $\mathscr{T}$ đều tương đương với một lý thuyết lôgic $\mathscr{T}'$ có nhiều nhất một tiên đề tường minh. Điều này là hiển nhiên nếu $\mathscr{T}$ không có tiên đề tường minh nào. Nếu $\mathscr{T}$ có các tiên đề tường minh $A_1$, $A_2$, ..., $A_h$, thì gọi $\mathscr{T}'$ là lý thuyết có cùng các ký hiệu và các lược đồ như $\mathscr{T}$, và có tiên đề tường minh "$A_1$ và $A_2$ và ... và $A_h$". Ngay lập tức thấy rằng mọi tiên đề của $\mathscr{T}$ (resp. $\mathscr{T}'$) đều là định lý của $\mathscr{T}'$ (resp. $\mathscr{T}$).

Cho $\mathscr{T}_0$ là lý thuyết không có tiên đề tường minh nào, có cùng các ký hiệu với $\mathscr{T}$ và chỉ có các lược đồ S1, S2, S3, S4. Khi đó việc nghiên cứu $\mathscr{T}$, về nguyên lý, quy về việc nghiên cứu $\mathscr{T}_0$ : để quan hệ $A$ là một định lý trong $\mathscr{T}$ thì điều kiện cần thiết và đủ là tồn tại các tiên đề $A_1$, $A_2$, ..., $A_h$ của $\mathscr{T}$ sao cho $(A_1$ and $A_2$ and ... and $A_h) \Rightarrow A$ là một định lý trong $\mathscr{T}_0$. Điều kiện này hiển nhiên là đủ. Trái lại, giả sử $A$ là một định lý trong $\mathscr{T}$, và gọi $A_1$, $A_2$, ..., $A_h$ là các tiên đề của $\mathscr{T}$ xuất hiện trong một chứng minh trong $\mathscr{T}$ có chứa $A$. Gọi $\mathscr{T}'$ (tương ứng $\mathscr{T}''$) là lý thuyết được xây dựng từ $\mathscr{T}_0$ bằng cách thêm vào các tiên đề $A_1$, $A_2$, ..., $A_h$ (tương ứng tiên đề "$A_1$ and $A_2$ and ... and $A_h$"). Chứng minh của $A$ trong $\mathscr{T}$ là một chứng minh của $A$ trong $\mathscr{T}'$, do đó $A$ là một định lý trong $\mathscr{T}'$ và do đó trong $\mathscr{T}''$, vì (như đã nhận thấy ở trên) $\mathscr{T}'$ và $\mathscr{T}''$ là tương đương. Theo tiêu chuẩn suy diễn, $(A_1$ and $A_2$ and ... and $A_h) \Rightarrow A$ là một định lý trong $\mathscr{T}_0$.

Nếu $\mathscr{T}$ là mâu thuẫn, thì từ những điều đã nói suy ra rằng tồn tại một phép hội $A$ của các tiên đề của $\mathscr{T}$ và một quan hệ $R$ trong $\mathscr{T}$ sao cho $A \Rightarrow (R$ và (không $R$)) là một định lý trong $\mathscr{T}_0$. Do đó

$$((\text{không } R) \text{ hoặc } (\text{không không } R)) \Rightarrow (\text{không } A)$$

là một định lý trong $\mathscr{T}_0$, và vì "(không $R$) hoặc (không không $R$)" là một định lý trong $\mathscr{T}_0$, nên "không $A$" là một định lý trong $\mathscr{T}_0$. Ngược lại, nếu tồn tại một phép hội $A$ của các tiên đề của $\mathscr{T}$ sao cho "không $A$" là một định lý trong $\mathscr{T}_0$, thì $A$ và "không $A$" là các định lý trong $\mathscr{T}$, do đó $\mathscr{T}$ là mâu thuẫn.

### 5. TƯƠNG ĐƯƠNG

Cho $A$ và $B$ là các dãy ký hiệu. Dãy ký hiệu

$$(A \Rightarrow B) \text{ và } (B \Rightarrow A)$$

sẽ được ký hiệu bởi $A \Leftrightarrow B$.

CS7. *Cho $A$, $B$, $T$ là các dãy ký hiệu, và cho $x$ là một chữ cái. Khi đó dãy ký hiệu $(T|x)(A \Leftrightarrow B)$ đồng nhất với $(T|x)A \Leftrightarrow (T|x)B$.*

Điều này suy ra ngay lập tức từ CS5 (§ 1, no. 2) và CS6 (no. 4).

CF10. *Nếu $A$ và $B$ là các quan hệ trong $\mathscr{T}$, thì $A \Leftrightarrow B$ là một quan hệ trong* **T**.

Điều này suy ra ngay lập tức từ CF5 (§ 1, no. 4) và CF9 (no. 4).

¶ Nếu $A \Leftrightarrow B$ là một định lý trong $\mathscr{T}$, ta sẽ nói rằng $A$ và $B$ là *tương đương* trong $\mathscr{T}$; nếu $x$ là một chữ cái không phải là một hằng số của $\mathscr{T}$, và nếu $A$ và $B$ được xét như những quan hệ theo $x$, thì mọi số hạng trong $\mathscr{T}$ thỏa mãn một trong hai quan hệ ấy cũng thỏa mãn quan hệ kia.

¶ Suy ra từ các tiêu chuẩn C20, C21 (no. 4) rằng để chứng minh một định lý trong $\mathscr{T}$ có dạng $A \Leftrightarrow B$, điều cần thiết và đủ là có thể chứng minh $A \Rightarrow B$ và $B \Rightarrow A$ trong $\mathscr{T}$. Điều này thường được thực hiện bằng cách chứng minh $B$ trong lý thuyết suy ra từ $\mathscr{T}$ bằng cách thêm tiên đề $A$, rồi chứng minh $A$ trong lý thuyết suy ra từ $\mathscr{T}$ bằng cách thêm tiên đề $B$. Các nhận xét này dẫn ngay lập tức đến các tiêu chuẩn sau đây, mà chúng tôi để bạn đọc tự chứng minh :

C22. *Cho $A$, $B$, $C$ là các quan hệ trong $\mathscr{T}$. Nếu $A \Leftrightarrow B$ là một định lý trong $\mathscr{T}$, thì $B \Leftrightarrow A$ là một định lý trong $\mathscr{T}$. Nếu $A \Leftrightarrow B$ và $B \Leftrightarrow C$ là các định lý trong $\mathscr{T}$, thì $A \Leftrightarrow C$ là một định lý trong $\mathscr{T}$.*

C23. *Cho $A$, $B$ là các quan hệ tương đương nhau trong $\mathscr{T}$, và cho $C$ là một quan hệ trong $\mathscr{T}$. Khi đó các mệnh đề sau là các định lý trong $\mathscr{T}$ :*

$$(\text{không } A) \Leftrightarrow (\text{không } B); \qquad (A \Rightarrow C) \Leftrightarrow (B \Rightarrow C);$$
$$(C \Rightarrow A) \Leftrightarrow (C \Rightarrow B);$$
$$(A \text{ và } C) \Leftrightarrow (B \text{ và } C); \qquad (A \text{ hoặc } C) \Leftrightarrow (B \text{ hoặc } C).$$

C24. *Cho $A$, $B$, $C$ là các quan hệ trong $\mathscr{T}$. Khi đó các mệnh đề sau là các định lý trong $\mathscr{T}$ :*

$$(\text{không không } A) \Leftrightarrow A; \qquad (A \Rightarrow B) \Leftrightarrow ((\text{không } B) \Rightarrow (\text{không } A));$$
$$(A \text{ và } A) \Leftrightarrow A; \qquad (A \text{ và } B) \Leftrightarrow (B \text{ và } A);$$
$$(A \text{ và } (B \text{ và } C)) \Leftrightarrow ((A \text{ và } B) \text{ và } C);$$
$$(A \text{ hoặc } B) \Leftrightarrow \text{không } ((\text{không } A) \text{ và } (\text{không } B));$$
$$(A \text{ hoặc } A) \Leftrightarrow A; \qquad (A \text{ hoặc } B) \Leftrightarrow (B \text{ hoặc } A);$$
$$(A \text{ hoặc } (B \text{ hoặc } C)) \Leftrightarrow ((A \text{ hoặc } B) \text{ hoặc } C);$$
$$(A \text{ và } (B \text{ hoặc } C)) \Leftrightarrow ((A \text{ và } B) \text{ hoặc } (A \text{ và } C));$$
$$(A \text{ hoặc } (B \text{ và } C)) \Leftrightarrow ((A \text{ hoặc } B) \text{ và } (A \text{ hoặc } C));$$
$$(A \text{ và } (\text{không } B)) \Leftrightarrow \text{không } (A \Rightarrow B);$$
$$(A \text{ hoặc } B) \Leftrightarrow ((\text{không } A) \Rightarrow B).$$

C25. *Nếu $A$ là một định lý trong $\mathscr{T}$ và $B$ là một quan hệ trong $\mathscr{T}$, thì*

$$(A \text{ và } B) \Leftrightarrow B$$

*là một định lý trong $\mathscr{T}$. Nếu "không $A$" là một định lý trong $\mathscr{T}$, thì $(A$ hoặc $B) \Rightarrow B$ là một định lý trong $\mathscr{T}$.*

¶ *Về nguyên lý, từ nay trong toàn bộ phần còn lại của chuỗi này, các tiêu chuẩn* C1 *đến* C25 *sẽ được dùng mà không cần viện dẫn.*

### Bài tập {#ens-i-s3-exercises}

Xem [bài tập của § 3](exercises/s3/).

[^1]: (\*) Lược đồ này có thể được diễn đạt mà không dùng chữ cái $A$ hoặc ký hiệu viết tắt $\Rightarrow$ như sau : *mỗi khi ta có một quan hệ, ta thu được một định lý bằng cách viết, từ trái sang phải,* $\vee$, $\neg$, $\vee$, *rồi sau đó quan hệ đã cho ba lần*. Người đọc có thể, như một bài tập, dịch theo một cách đồng dạng các cách diễn đạt của những lược đồ khác.
[^2]: (†) Trong lời nói hằng ngày, từ "hoặc" có hai nghĩa khác nhau, tùy theo ngữ cảnh : khi ta nối hai mệnh đề bằng từ "hoặc", ta có thể muốn khẳng định rằng ít nhất một trong hai mệnh đề là đúng (và có thể cả hai cùng đúng), hoặc ta có thể muốn khẳng định một mệnh đề mà loại trừ mệnh đề kia.
