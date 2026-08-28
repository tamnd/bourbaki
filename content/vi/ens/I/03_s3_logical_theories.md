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
content_sha256: 6a2d7dda8f5f4d337b8766c66ff66bde0b47a745cf53db11a57921368f70c7e7
translated_from: content/en/ens/I/03_s3_logical_theories.md
source_content_sha256: 37ec32a3c0cdf2c61a57848be909293d325cc40d690c0e328f7cb619bf02c9e1
translation_model: gpt-5.4-mini
translation_run: translate-vi-5cba219d
glossary_version: 34
glossary_terms_sha256: 6ee8e697f06aaa331f7a039a31ad0254f072aeeaf957fad290a416d86217b7bd
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 3. CÁC LÝ THUYẾT LÔGIC

### 1. CÁC TIÊN ĐỀ

Một *lý thuyết lôgic* là bất kỳ lý thuyết $\mathscr{T}$ nào trong đó các sơ đồ S1 đến S4 dưới đây cung cấp các tiên đề ẩn.

S1. *Nếu $A$ là một quan hệ trong $\mathscr{T}$, thì quan hệ $(A$ or $A) \Rightarrow A$ là một tiên đề của $\mathscr{T}$* [^1].

S2. *Nếu $A$ và $B$ là các quan hệ trong $\mathscr{T}$, thì quan hệ $A \Rightarrow (A$ or B) là một tiên đề của $\mathscr{T}$.*

S3. *Nếu $A$ và $B$ là các quan hệ trong $\mathscr{T}$, thì quan hệ $(A$ hoặc $B) \Rightarrow (B$ hoặc A) là một tiên đề của $\mathscr{T}$.*

S4. *Nếu $A$, $B$, và $C$ là các quan hệ trong $\mathscr{T}$, thì quan hệ*

$$(A \Rightarrow B) \Rightarrow ((C \text{ hoặc } A) \Rightarrow (C \text{ hoặc } B))$$

*là một tiên đề của $\mathscr{T}$.*

Những quy tắc này thực ra là các sơ đồ; hãy kiểm tra điều này, chẳng hạn đối với S2. Cho $R$ là một quan hệ thu được bằng cách áp dụng S2; khi đó tồn tại các quan hệ $A$ và $B$ trong $\mathscr{T}$ sao cho $R$ là quan hệ $A \Rightarrow (A$ hoặc B). Cho $T$ là một số hạng trong $\mathscr{T}$, cho $x$ là một chữ cái, và cho $A'$ và $B'$ là các quan hệ $(T|x)A$ và $(T|x)B$; khi đó $(T|x)R$ chính là $A' \Rightarrow (A'$ hoặc $B')$, và do đó có thể thu được bằng cách áp dụng S2.

Một cách trực giác, các quy tắc S1 đến S4 chỉ đơn thuần biểu thị ý nghĩa gắn với các từ "hoặc" và "kéo theo" trong ngôn ngữ thông thường của toán học [^2].

Nếu một lý thuyết lôgic $\mathscr{T}$ là mâu thuẫn, *mọi quan hệ trong $\mathscr{T}$ đều là một định lý trong $\mathscr{T}$.* Vì hãy cho $A$ là một quan hệ trong $\mathscr{T}$ sao cho $A$ và "không phải $A$" là các định lý trong $\mathscr{T}$, và cho $B$ là bất kỳ quan hệ nào trong $\mathscr{T}$. Theo S2, (không phải $A$) $\Rightarrow$ ((không phải $A$) hoặc $B$) là một định lý trong $\mathscr{T}$; do đó, theo C1 (§ 2, no. 2), "(không phải $A$) hoặc $B$", tức là $A \Rightarrow B$, là một định lý trong $\mathscr{T}$. Một áp dụng thứ hai của C1 cho thấy rằng $B$ là một định lý trong $\mathscr{T}$.

¶ *Từ nay $\mathscr{T}$ sẽ ký hiệu một lý thuyết lôgic.*

### 2. CÁC HỆ QUẢ ĐẦU TIÊN

C6. *Cho $A$, $B$, $C$ là các quan hệ trong $\mathscr{T}$. Nếu $A \Rightarrow B$ và $B \Rightarrow C$ là các định lý trong $\mathscr{T}$, thì $A \Rightarrow C$ là một định lý trong $\mathscr{T}$.*

Đối với $(B \Rightarrow C) \Rightarrow ((A \Rightarrow B) \Rightarrow (A \Rightarrow C))$ là một tiên đề của $\mathscr{T}$, bằng cách thay thế $A$ bởi $B$, $B$ bởi $C$, và $C$ bởi "không phải $A$" trong S4. Theo C1 (§ 2, no. 2), $(A \Rightarrow B) \Rightarrow (A \Rightarrow C)$ là một định lý trong $\mathscr{T}$. Một lần áp dụng C1 nữa hoàn tất chứng minh.

C7. *Nếu $A$ và $B$ là các quan hệ trong $\mathscr{T}$, thì $B \Rightarrow (A$ hoặc B) là một định lý trong $\mathscr{T}$. \*

Vì $B \Rightarrow (B$ hoặc A) và $(B$ hoặc $A) \Rightarrow (A$ hoặc B) là các tiên đề của $\mathscr{T}$ do S2 và S3. Bây giờ dùng C6.

C8. *Nếu $A$ là một quan hệ trong $\mathscr{T}$, $A \Rightarrow A$ là một định lý trong $\mathscr{T}$.*

Vì $A \Rightarrow (A$ hoặc A) và $(A$ hoặc $A) \Rightarrow A$ là các tiên đề, theo S2 và S1. Bây giờ dùng C6.

C9. *Nếu $A$ là một quan hệ và $B$ là một định lý trong $\mathscr{T}$, thì $A \Rightarrow B$ là một định lý trong $\mathscr{T}$.*

Vì $B \Rightarrow ((\text{không phải } A)$ or B) là một định lý theo C7, và do đó "(không phải $A$) or $B$", tức là $A \Rightarrow B$, là một định lý theo C1.

C10. *Nếu $A$ là một quan hệ trong $\mathscr{T}$, thì "$A$ or (không phải $A$)" là một định lý trong $\mathscr{T}$.*

Vì "(không phải $A$) or $A$" là một định lý theo C8; bây giờ dùng S3 và C1.

C11. *Nếu $A$ là một quan hệ trong $\mathscr{T}$, "$A \Rightarrow$ (không phải không $A$)" là một định lý trong $\mathscr{T}$.*

Vì quan hệ này là "(không phải $A$) hoặc (không phải không $A$)", và kết quả suy ra từ C10.

C12. *Cho $A$ và $B$ là hai quan hệ trong $\mathscr{T}$. Khi đó quan hệ*

$$(A \Rightarrow B) \Rightarrow ((\text{không } B) \Rightarrow (\text{không } A))$$

*là một định lý trong $\mathscr{T}$.*

Vì

$$((\text{không } A) \text{ hoặc } B) \Rightarrow ((\text{không } A) \text{ hoặc } (\text{không không } B))$$

là một định lý, theo C11, S4 và C1. Mặt khác,

$$((\text{không } A) \text{ hoặc } (\text{không không } B)) \Rightarrow ((\text{không không } B) \text{ hoặc } (\text{không } A))$$

là một tiên đề, theo S3. Do đó

$$((\text{không } A) \text{ hoặc } B) \Rightarrow ((\text{không không } B) \text{ hoặc } (\text{không } A))$$

là một định lý theo C6. Vậy kết quả.

C13. *Cho $A$, $B$, $C$ là các quan hệ trong $\mathscr{T}$. Nếu $A \Rightarrow B$ là một định lý trong $\mathscr{T}$, thì $(B \Rightarrow C) \Rightarrow (A \Rightarrow C)$ là một định lý trong $\mathscr{T}$.*

Vì $(\text{không } B) \Rightarrow (\text{không } A)$ là một định lý, theo C12 và C1. Do đó $(C \text{ hoặc } (\text{không } B)) \Rightarrow (C \text{ hoặc } (\text{không } A))$ là một định lý, theo S4 và C1. Bằng hai lần áp dụng S3 và C6, suy ra rằng

$$((\text{không } B) \text{ hoặc } C) \Rightarrow ((\text{không } A) \text{ hoặc } C)$$

là một định lý; nhưng đây chính là quan hệ đã cho.

¶ *Từ nay về sau, chúng ta nói chung sẽ dùng* C1 *và* C6 *mà không viện dẫn chúng tường minh.*

### 3. CÁC PHƯƠNG PHÁP CHỨNG MINH

I. *Phương pháp giả thiết phụ.* Phương pháp này dựa trên quy tắc sau :

C14 (*Tiêu chuẩn suy diễn*). *Cho $A$ là một quan hệ trong $\mathscr{T}$, và cho $\mathscr{T}'$ là lý thuyết thu được bằng cách thêm $A$ vào các tiên đề của $\mathscr{T}$. Nếu $B$ là một định lý trong $\mathscr{T}'$, thì $A \Rightarrow B$ là một định lý trong $\mathscr{T}$.*

Cho $B_1$, $B_2$, ..., $B_n$ là một chứng minh trong $\mathscr{T}'$ trong đó có $B$ xuất hiện. Ta sẽ chứng minh, từng bước một, rằng các mệnh đề $A \Rightarrow B_k$ là các định lý trong $\mathscr{T}$. Giả sử điều này đã được thiết lập cho các mệnh đề đi trước $B_i$, và ta sẽ chứng minh rằng $A \Rightarrow B_i$ là một định lý trong $\mathscr{T}$. Nếu $B_i$ là một tiên đề của $\mathscr{T}'$, thì $B_i$ hoặc là một tiên đề của $\mathscr{T}$ hoặc là $A$. Trong cả hai trường hợp, $A \Rightarrow B_i$ là một định lý trong $\mathscr{T}$ nhờ áp dụng C9 hoặc C8. Nếu $B_i$ được đi trước bởi các mệnh đề $B_j$ và $B_j \Rightarrow B_i$, ta biết rằng $A \Rightarrow B_j$ và $A \Rightarrow (B_j \Rightarrow B_i)$ là các định lý trong $\mathscr{T}$. Suy ra $(B_j \Rightarrow B_i) \Rightarrow (A \Rightarrow B_i)$ là một định lý trong $\mathscr{T}$ nhờ C13. Suy ra, theo C6, $A \Rightarrow (A \Rightarrow B_i)$, tức là "$(\text{không phải } A)$ hoặc $(A \Rightarrow B_i)$", là một định lý trong $\mathscr{T}$, và do đó "$(A \Rightarrow B_i)$ hoặc $(\text{không phải } A)$" cũng là nhờ S3. Bây giờ, $(\text{không phải } A) \Rightarrow ((\text{không phải } A) \text{ hoặc } B_i)$, tức là $(\text{không phải } A) \Rightarrow (A \Rightarrow B_i)$, là một định lý trong $\mathscr{T}$, nhờ S2. Áp dụng S4, ta thấy rằng

$$((A \Rightarrow B_i) \text{ hoặc } (\text{không } A)) \Rightarrow ((A \Rightarrow B_i) \text{ hoặc } (A \Rightarrow B_i))$$

là một định lý trong $\mathscr{T}$, và do đó rằng "$(A \Rightarrow B_i)$ hoặc $(A \Rightarrow B_i)$" là một định lý trong $\mathscr{T}$. Theo S1 ta kết luận rằng $A \Rightarrow B_i$ là một định lý trong $\mathscr{T}$.

Trong thực hành, ta chỉ ra rằng mình sẽ dùng tiêu chuẩn này bằng một cụm từ như "giả sử rằng $A$ là đúng". Cụm từ này có nghĩa là trong lúc đó lập luận sẽ được tiến hành trong lý thuyết $\mathscr{T}'$, cho đến khi quan hệ $B$ đã được chứng minh. Khi điều này đã đạt được thì đã xác lập rằng $A \Rightarrow B$ là một định lý trong $\mathscr{T}$, và từ đó về sau người ta tiếp tục lập luận trong $\mathscr{T}$ mà nói chung không chỉ ra rằng mình đã rời bỏ lý thuyết $\mathscr{T}'$. Quan hệ $A$ được đưa vào như một tiên đề mới được gọi là *giả thiết phụ*. \* Chẳng hạn, khi ta nói "hãy cho $x$ là một số thực", ta đang xây dựng một lý thuyết trong đó quan hệ "$x$ là một số thực" là một giả thiết phụ. \*

II. *Phương pháp chứng minh phản chứng.* Phương pháp này dựa trên quy tắc sau:

C15. *Cho $A$ là một quan hệ trong $\mathscr{T}$, và cho $\mathscr{T}'$ là lý thuyết thu được bằng cách thêm tiên đề* "không $A$" *vào các tiên đề của $\mathscr{T}$. Nếu $\mathscr{T}'$ là mâu thuẫn, thì $A$ là một định lý trong $\mathscr{T}$.*

Vì $A$ là một định lý trong $\mathscr{T}'$; do đó (phương pháp của giả thiết phụ) "(không $A$) $\Rightarrow A$" là một định lý trong $\mathscr{T}$. Theo S4,

$$(A \text{ hoặc } (\text{không } A)) \Rightarrow (A \text{ hoặc } A)$$

là một định lý trong $\mathscr{T}$; theo C10, "$A$ or $A$" là một định lý trong $\mathscr{T}$. Bây giờ dùng S1.

Trong thực tế, ta chỉ ra rằng mình sẽ dùng tiêu chuẩn này bằng một cụm từ như "giả sử rằng $A$ là sai". Cụm từ này có nghĩa là trong lúc này lập luận sẽ được thực hiện trong lý thuyết $\mathscr{T}'$, cho đến khi hai định lý có dạng $B$ và "không $B$" đã được chứng minh. Khi điều này đã đạt được thì suy ra rằng $A$ là một định lý trong $\mathscr{T}$, điều này thường được chỉ ra bằng một cụm từ như "Bây giờ điều này (tức là, theo ký hiệu ở trên, $B$ và "không $B$") là vô lý; do đó $A$ là đúng". Khi đó ta tiếp tục trong lý thuyết gốc $\mathscr{T}$.

¶ Là những áp dụng đầu tiên của các phương pháp này, hãy thiết lập các tiêu chuẩn sau :

C16. *Nếu $A$ là một quan hệ trong $\mathscr{T}$, thì* (không không $A$) $\Rightarrow A$ *là một định lý trong $\mathscr{T}$.*

Vì giả sử rằng "không không $A$" là đúng; khi đó ta phải chứng minh $A$. Giả sử $A$ là sai. Trong lý thuyết được định nghĩa như vậy, "không không $A$" và "không $A$" đều là các định lý, điều đó vô lý; do đó $A$ là đúng.

C17. *Nếu $A$ và $B$ là các quan hệ trong $\mathscr{T}$, thì*

$$((\text{không } B) \Rightarrow (\text{không } A)) \Rightarrow (A \Rightarrow B)$$

*là một định lý trong $\mathscr{T}$.*

Vì giả sử rằng $(\text{không }B) \Rightarrow (\text{không }A)$ là đúng. Ta phải chứng minh rằng $A \Rightarrow B$ là đúng. Giả sử rằng $A$ là đúng, và ta hãy chứng minh rằng $B$ là đúng. Giả sử “không $B$” là đúng. Khi đó “không $A$” là đúng, điều đó là vô lý.

III. *Phương pháp phân ly các trường hợp.* Điều này dựa trên quy tắc sau :

C18. *Cho $A$, $B$, $C$ là các quan hệ trong $\mathscr{T}$. Nếu “$A$ hoặc $B$” $A \Rightarrow C$, $B \Rightarrow C$ là các định lý trong $\mathscr{T}$, thì $C$ là một định lý trong $\mathscr{T}$.*

Vì, theo S4, “$(A\text{ hoặc }B) \Rightarrow (A\text{ hoặc }C)$” và “$(C\text{ hoặc }A) \Rightarrow (C\text{ hoặc }C)$” là các định lý trong $\mathscr{T}$. Theo S3 và S1, suy ra $(A\text{ hoặc }B) \Rightarrow C$ là một định lý trong $\mathscr{T}$; do đó kết quả.

Để chứng minh $C$ thì do đó chỉ cần, khi ta có sẵn một định lý “$A$ or $B$”, trước hết chứng minh $C$ bằng cách thêm $A$ vào các tiên đề của $\mathscr{T}$, rồi sau đó chứng minh $C$ bằng cách thêm $B$ vào các tiên đề của $\mathscr{T}$. Điểm thú vị của phương pháp này nằm ở chỗ nếu “$A$ or $B$” là đúng, thì nói chung ta không thể khẳng định rằng $A$ là đúng hay rằng $B$ là đúng.

Đặc biệt, theo C10, nếu “$A \Rightarrow C$” và “$(\text{không }A) \Rightarrow C$” đều là các định lý trong $\mathscr{T}$, thì $C$ là một định lý trong $\mathscr{T}$.

IV. *Phương pháp của hằng số phụ.* Điều này dựa trên quy tắc sau :

C19. *Cho $x$ là một chữ cái và cho $A$ và $B$ là các quan hệ trong $\mathscr{T}$ sao cho :*

(1) *chữ cái $x$ không là một hằng của $\mathscr{T}$ và không xuất hiện trong $B$;*
(2) *có một số hạng $T$ trong $\mathscr{T}$ sao cho $(T|x)A$ là một định lý trong $\mathscr{T}$.*

*Cho $\mathscr{T}'$ là lý thuyết thu được bằng cách thêm $A$ vào các tiên đề của $\mathscr{T}$. Nếu $B$ là một định lý trong $\mathscr{T}'$, thì $B$ là một định lý trong $\mathscr{T}$.*

Thật vậy, $A \Rightarrow B$ là một định lý trong $\mathscr{T}$ (tiêu chuẩn suy diễn). Vì $x$ không phải là một hằng của $\mathscr{T}$, $(T|x)(A \Rightarrow B)$ là một định lý trong $\mathscr{T}$ theo C3. Vì $x$ không xuất hiện trong $B$, $(T|x)(A \Rightarrow B)$ đồng nhất với $((T|x)A) \Rightarrow B$, theo CS5 (§ 1, no. 2). Cuối cùng, $(T|x)A$ là một định lý trong $\mathscr{T}$, và do đó $B$ cũng vậy.

Về trực giác, phương pháp này cốt ở việc dùng, để chứng minh $B$, một đối tượng tùy ý $x$ (the *hằng phụ*) mà được giả thiết là được trang bị những tính chất nào đó, ký hiệu bởi $A$. \* Chẳng hạn, trong một chứng minh hình học có liên quan, trong số những điều khác, đến một đường thẳng $D$, ta có thể “lấy” một điểm $x$ trên đường thẳng này; khi đó quan hệ $A$ là $x \in D$. \* Để có thể dùng một đối tượng được trang bị những tính chất nào đó trong quá trình chứng minh, rõ ràng cần phải có sự tồn tại của những đối tượng như thế. Định lý $(T|x)A$, gọi là *định lý hợp thức hóa*, bảo đảm sự tồn tại này.

Trong thực hành, ta chỉ ra rằng ta sắp dùng phương pháp này bằng một cụm như “cho $x$ là một đối tượng sao cho $A$”. Trái với phương pháp của giả thiết phụ, kết luận của lập luận không liên quan đến $x$.

### 4. PHÉP HỘI

Cho $A$, $B$ là các dãy ký hiệu. Dãy ký hiệu

$$
\text{không } ((\text{không } A) \text{ hoặc } (\text{không } B))
$$

được ký hiệu là “$A$ và $B$”.

CS6.  Cho $A$, $B$, $T$ là các dãy ký hiệu và $x$ là một chữ cái.  Khi đó dãy ký hiệu

$$
(T|x)(A\text{ và }B)
$$

trùng với “$(T|x)A$ và $(T|x)B$”.

Đây là hệ quả ngay lập tức của CS5 (§ 1, no. 2).

CF9.  Nếu $A$, $B$ là các quan hệ trong $\mathscr{T}$, thì “$A$ và $B$” là một quan hệ trong $\mathscr{T}$ (gọi là phép hội của $A$ và $B$).

Điều này suy ra ngay lập tức từ CF1 và CF2 (§ 1, no. 4).

C20.  Nếu $A$, $B$ là các định lý trong $\mathscr{T}$, thì “$A$ và $B$” là một định lý trong $\mathscr{T}$.

Giả sử “$A$ và $B$” là sai, tức là,

$$
\text{không không } ((\text{không } A) \text{ hoặc } (\text{không } B))
$$

là đúng. Theo C16, “$(\text{không } A)$ hoặc $(\text{không } B)$”, tức là, $A \Longrightarrow (\text{không } B)$ là đúng, suy ra “không $B$” là đúng; nhưng điều này vô lý. Vậy nên “$A$ và $B$” là đúng.

C21. Nếu $A$, $B$ là các quan hệ trong $\mathscr{T}$, thì

$$
(A\text{ và }B) \Longrightarrow A,\qquad (A\text{ và }B) \Longrightarrow B
$$

là các định lý trong $\mathscr{T}$.

Các quan hệ $(\text{không } A) \Longrightarrow ((\text{không } A) \text{ hoặc } (\text{không } B))$, $(\text{không } B) \Longrightarrow ((\text{không } A) \text{ hoặc } (\text{không } B))$ là các định lý trong $\mathscr{T}$, theo S2 (no. 1) và C7 (no. 2).  Bây giờ $((\text{không } A) \text{ hoặc } (\text{không } B)) \Longrightarrow (\text{không } (A\text{ và }B))$ là một định lý trong $\mathscr{T}$ theo C11.  Do đó $(\text{không } A) \Longrightarrow (\text{không } (A\text{ và }B))$, $(\text{không } B) \Longrightarrow (\text{không } (A\text{ và }B))$ là các định lý trong $\mathscr{T}$.  Kết quả suy ra bằng cách áp dụng C17.

¶ Ta sẽ ký hiệu bằng "$A$ và $B$ và $C$" (tương ứng "$A$ hoặc $B$ hoặc $C$") quan hệ "$A$ và ($B$ và $C$)" (tương ứng "$A$ hoặc ($B$ hoặc $C$)"). Nói chung hơn, nếu

$$A_1, \quad A_2, \quad \ldots, \quad A_n$$

Là các quan hệ, ta ký hiệu bằng "$A_1$ và $A_2$, và ... và $A_p$" một quan hệ được xây dựng từng bước theo quy ước rằng "$A_1$ và $A_2$ và ... và $A_h$" ký hiệu cùng một quan hệ như "$A_1$ và ($A_2$ và ... và $A_h$)". Quan hệ "$A_1$ hoặc $A_2$ hoặc ... hoặc $A_h$" được định nghĩa tương tự. Quan hệ "$A_1$ và $A_2$ và ... và $A_h$" là một định lý trong $\mathscr{T}$ khi và chỉ khi mỗi quan hệ $A_1$, $A_2$, ..., $A_h$ là một định lý trong $\mathscr{T}$.

Suy ra rằng mọi lý thuyết lôgic $\mathscr{T}$ đều tương đương với một lý thuyết lôgic $\mathscr{T}'$ có nhiều nhất một tiên đề tường minh. Điều này là hiển nhiên nếu $\mathscr{T}$ không có tiên đề tường minh nào. Nếu $\mathscr{T}$ có các tiên đề tường minh $A_1$, $A_2$, ..., $A_h$, hãy đặt $\mathscr{T}'$ là lý thuyết có cùng các ký hiệu và lược đồ như $\mathscr{T}$, và tiên đề tường minh "$A_1$ và $A_2$ và ... và $A_h$". Ta thấy ngay rằng mỗi tiên đề của $\mathscr{T}$ (resp. $\mathscr{T}'$) là một định lý của $\mathscr{T}'$ (resp. $\mathscr{T}$).

Cho $\mathscr{T}_0$ là lý thuyết không có các tiên đề tường minh nào, có cùng các ký hiệu với $\mathscr{T}$ và S1, S2, S3, S4 là các lược đồ duy nhất của nó. Khi đó việc nghiên cứu $\mathscr{T}$, về nguyên tắc, quy về việc nghiên cứu $\mathscr{T}_0$ : để quan hệ $A$ là một định lý trong $\mathscr{T}$ thì cần và đủ rằng tồn tại các tiên đề $A_1$, $A_2$, ..., $A_h$ của $\mathscr{T}$ sao cho $(A_1$ và $A_2$ và ... và $A_h) \Rightarrow A$ là một định lý trong $\mathscr{T}_0$. Điều kiện này hiển nhiên là đủ. Ngược lại, giả sử rằng $A$ là một định lý trong $\mathscr{T}$, và cho $A_1$, $A_2$, ..., $A_h$ là các tiên đề của $\mathscr{T}$ xuất hiện trong một chứng minh trong $\mathscr{T}$ chứa $A$. Cho $\mathscr{T}'$ (tương ứng $\mathscr{T}''$) là lý thuyết được xây dựng từ $\mathscr{T}_0$ bằng cách thêm vào các tiên đề $A_1$, $A_2$, ..., $A_h$ (tương ứng tiên đề "$A_1$ và $A_2$ và ... và $A_h$"). Chứng minh của $A$ trong $\mathscr{T}$ là một chứng minh của $A$ trong $\mathscr{T}'$, do đó $A$ là một định lý trong $\mathscr{T}'$ và do đó trong $\mathscr{T}''$, vì (như ta đã nhận xét ở trên) $\mathscr{T}'$ và $\mathscr{T}''$ là tương đương. Theo tiêu chuẩn suy diễn, $(A_1$ và $A_2$ và ... và $A_h) \Rightarrow A$ là một định lý trong $\mathscr{T}_0$.

Nếu $\mathscr{T}$ là mâu thuẫn, thì suy ra từ những gì đã nói rằng tồn tại một phép hội $A$ của các tiên đề của $\mathscr{T}$ và một quan hệ $R$ trong $\mathscr{T}$ sao cho $A \Rightarrow (R$ và (không $R$)) là một định lý trong $\mathscr{T}_0$. Do đó

$$((\text{không } R) \text{ hoặc } (\text{không không } R)) \Rightarrow (\text{không } A)$$

là một định lý trong $\mathscr{T}_0$, và vì "(không $R$) hoặc (không không $R$)" là một định lý trong $\mathscr{T}_0$, "không $A$" là một định lý trong $\mathscr{T}_0$. Ngược lại, nếu tồn tại một phép hội $A$ của các tiên đề của $\mathscr{T}$ sao cho "không $A$" là một định lý trong $\mathscr{T}_0$, thì $A$ và "không $A$" là các định lý trong $\mathscr{T}$, do đó $\mathscr{T}$ là mâu thuẫn.

### 5. TƯƠNG ĐƯƠNG

Cho $A$ và $B$ là các dãy ký hiệu. Dãy ký hiệu

$$(A \Rightarrow B) \text{ và } (B \Rightarrow A)$$

sẽ được ký hiệu bởi $A \Leftrightarrow B$.

CS7. *Cho $A$, $B$, $T$ là các dãy ký hiệu, và cho $x$ là một chữ cái. Khi đó dãy ký hiệu $(T|x)(A \Leftrightarrow B)$ trùng với $(T|x)A \Leftrightarrow (T|x)B$.*

Điều này suy ra ngay lập tức từ CS5 (§ 1, no. 2) và CS6 (no. 4).

CF10. *Nếu $A$ và $B$ là các quan hệ trong $\mathscr{T}$, thì $A \Leftrightarrow B$ là một quan hệ trong* **T**.

Điều này suy ra ngay lập tức từ CF5 (§ 1, no. 4) và CF9 (no. 4).

¶ Nếu $A \Leftrightarrow B$ là một định lý trong $\mathscr{T}$, ta sẽ nói rằng $A$ và $B$ là *tương đương* trong $\mathscr{T}$; nếu $x$ là một chữ cái không phải là một hằng của $\mathscr{T}$, và nếu $A$ và $B$ được xét như các quan hệ theo $x$, thì mọi số hạng trong $\mathscr{T}$ thỏa một cái cũng thỏa cái kia.

¶ Suy ra từ các tiêu chuẩn C20, C21 (no. 4) rằng để chứng minh một định lý trong $\mathscr{T}$ có dạng $A \Leftrightarrow B$, thì cần và đủ phải có thể chứng minh $A \Rightarrow B$ và $B \Rightarrow A$ trong $\mathscr{T}$. Điều này thường được thực hiện bằng cách chứng minh $B$ trong lý thuyết suy ra từ $\mathscr{T}$ bằng cách thêm tiên đề $A$, và sau đó bằng cách chứng minh $A$ trong lý thuyết suy ra từ $\mathscr{T}$ bằng cách thêm tiên đề $B$. Những nhận xét này dẫn ngay lập tức đến các tiêu chuẩn sau, mà chúng tôi để lại phần chứng minh cho người đọc :

C22. *Cho $A$, $B$, $C$ là các quan hệ trong $\mathscr{T}$. Nếu $A \Leftrightarrow B$ là một định lý trong $\mathscr{T}$, thì $B \Leftrightarrow A$ là một định lý trong $\mathscr{T}$. Nếu $A \Leftrightarrow B$ và $B \Leftrightarrow C$ là các định lý trong $\mathscr{T}$, thì $A \Leftrightarrow C$ là một định lý trong $\mathscr{T}$.*

C23. *Cho $A$, $B$ là các quan hệ tương đương trong $\mathscr{T}$, và cho $C$ là một quan hệ trong $\mathscr{T}$. Khi đó các điều sau là các định lý trong $\mathscr{T}$ :*

$$(\text{không phải } A) \Leftrightarrow (\text{không phải } B); \qquad (A \Rightarrow C) \Leftrightarrow (B \Rightarrow C);$$
$$(C \Rightarrow A) \Leftrightarrow (C \Rightarrow B);$$
$$(A \text{ và } C) \Leftrightarrow (B \text{ và } C); \qquad (A \text{ hoặc } C) \Leftrightarrow (B \text{ hoặc } C).$$

C24. *Cho $A$, $B$, $C$ là các quan hệ trong $\mathscr{T}$. Khi đó các điều sau là các định lý trong $\mathscr{T}$ :*

$$(\text{không phải không phải } A) \Leftrightarrow A; \qquad (A \Rightarrow B) \Leftrightarrow ((\text{không phải } B) \Rightarrow (\text{không phải } A));$$
$$(A \text{ và } A) \Leftrightarrow A; \qquad (A \text{ và } B) \Leftrightarrow (B \text{ và } A);$$
$$(A \text{ và } (B \text{ và } C)) \Leftrightarrow ((A \text{ và } B) \text{ và } C);$$
$$(A \text{ hoặc } B) \Leftrightarrow \text{không phải } ((\text{không phải } A) \text{ và } (\text{không phải } B));$$
$$(A \text{ hoặc } A) \Leftrightarrow A; \qquad (A \text{ hoặc } B) \Leftrightarrow (B \text{ hoặc } A);$$
$$(A \text{ hoặc } (B \text{ hoặc } C)) \Leftrightarrow ((A \text{ hoặc } B) \text{ hoặc } C);$$
$$(A \text{ và } (B \text{ hoặc } C)) \Leftrightarrow ((A \text{ và } B) \text{ hoặc } (A \text{ và } C));$$
$$(A \text{ hoặc } (B \text{ và } C)) \Leftrightarrow ((A \text{ hoặc } B) \text{ và } (A \text{ hoặc } C));$$
$$(A \text{ và } (\text{không phải } B)) \Leftrightarrow \text{không phải } (A \Rightarrow B);$$
$$(A \text{ hoặc } B) \Leftrightarrow ((\text{không phải } A) \Rightarrow B).$$

C25. *Nếu $A$ là một định lý trong $\mathscr{T}$ và $B$ là một quan hệ trong $\mathscr{T}$, thì*

$$(A \text{ và } B) \Leftrightarrow B$$

¶ *là một định lý trong $\mathscr{T}$. Nếu "không phải $A$" là một định lý trong $\mathscr{T}$, thì $(A$ hoặc $B) \Rightarrow B$ là một định lý trong $\mathscr{T}$.*

¶ *Về nguyên tắc, từ nay trở đi trong suốt phần còn lại của chuỗi này, các tiêu chuẩn* C1 *đến* C25 *sẽ được dùng mà không cần viện dẫn.*

### Bài tập {#ens-i-s3-exercises}

Xem [các bài tập cho § 3](exercises/s3/).

[^1]: Sơ đồ này có thể được diễn đạt mà không dùng chữ cái $A$ hay ký hiệu viết tắt $\Rightarrow$ như sau : *hễ ta có một quan hệ, ta thu được một định lý bằng cách viết, từ trái sang phải,* $\vee$, $\neg$, $\vee$, *rồi quan hệ đã cho ba lần*. Bạn đọc có thể, như một bài tập, dịch theo cách tương tự các biểu thức của những sơ đồ khác.
[^2]: Trong lời nói hằng ngày, từ "hoặc" có hai nghĩa khác nhau, tùy theo ngữ cảnh : khi nối hai mệnh đề bằng từ "hoặc" ta có thể muốn khẳng định ít nhất một trong hai (và có thể cả hai cùng lúc), hoặc ta có thể muốn khẳng định một cái để loại trừ cái kia.
