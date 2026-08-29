---
book: ens
book_title: Theory of Sets
chapter: ""
chapter_title: ""
section: 0
section_title: TO THE READER
kind: reader
lang: vi
source: ens-i-iv
source_edition: 2004, Springer
pdf_pages: 0005-0007
extraction: ocr
statements: 0
exercises: 0
content_sha256: 2092be9cb831076644a0690b8d557342c0e22e4192143e32930e90806b8e2dcd
translated_from: content/en/ens/00_to_the_reader.md
source_content_sha256: 47ab664cac8f5f795d2044796b3391ca190ab6598f4137432142ea2c6871cd7e
translation_model: gpt-5-mini, gpt-5-6-mini
translation_run: translate-vi-ab3b66f0
glossary_version: 34
glossary_terms_sha256: 76186de53f36d631ddd164476e894ef54a04b981c4aca55c33b07f20a27ad312
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## ĐẾN NGƯỜI ĐỌC

1. This series of volumes, a list of which is given on pages vii and viii, takes up mathematics at the beginning, and gives complete proofs. In principle, it requires no particular knowledge of mathematics on the reader’s part, but only a certain familiarity with mathematical reasoning and a certain capacity for abstract thought. Nevertheless, it is directed especially to those who have a good knowledge of at least the content of the first year or two of a university mathematics course.

2. The method of exposition we have chosen is axiomatic and abstract, and normally proceeds from the general to the particular. This choice has been dictated by the main purpose of the treatise, which is to provide a solid foundation for the whole body of modern mathematics. For this it is indispensable to become familiar with a rather large number of very general ideas and principles. Moreover, the demands of proof impose a rigorously fixed order on the subject matter. It follows that the utility of certain considerations will not be immediately apparent to the reader unless he has already a fairly extended knowledge of mathematics; otherwise he must have the patience to suspend judgment until the occasion arises.

3. In order to mitigate this disadvantage we have frequently inserted examples in the text which refer to facts the reader may already know but which have not yet been discussed in the series. Such examples are always placed between two asterisks: \* ... \*. Most readers will undoubtedly find that these examples will help them to understand the text, and will prefer not to leave them out, even at a first reading. Their omission would of course have no disadvantage, from a purely logical point of view.

4. This series is divided into volumes (here called “Books”). The first six Books are numbered and, in general, every statement in the text

v giả thiết là đã biết chỉ những kết quả đã được thảo luận trong các quyển trước. Quy tắc này vẫn đúng trong phạm vi mỗi Quyển, nhưng để thuận tiện cho việc trình bày, các Quyển này không còn được sắp xếp theo một thứ tự liên tiếp nữa. Ở đầu mỗi Quyển này (hoặc mỗi chương này), người đọc sẽ tìm thấy một chỉ dẫn chính xác về mối quan hệ lôgic của nó với các Quyển khác và do đó sẽ có thể tự thỏa mãn rằng không có vòng luẩn quẩn nào.

5. The logical framework of each chapter consists of the *definitions*, the *axioms*, and the *theorems* of the chapter. These are the parts that have mainly to be borne in mind for subsequent use. Less important results and those which can easily be deduced from the theorems are labelled as “propositions”, “lemmas”, “corollaries”, “remarks”, etc. Those which may be omitted at a first reading are printed in small type. A commentary on a particularly important theorem appears occasionally under the name of “scholium”.

Để tránh những sự lặp lại tẻ nhạt, đôi khi thuận tiện khi đưa vào các ký hiệu hoặc các chữ viết tắt chỉ có hiệu lực trong một chương nhất định hoặc một tiết diện nhất định của một chương (chẳng hạn, trong một chương chỉ liên quan đến các vành giao hoán, từ “vành” sẽ luôn có nghĩa là “vành giao hoán”). Những quy ước như vậy luôn được nêu rõ một cách tường minh, nói chung là ở đầu chương mà chúng xuất hiện.

6. Some passages in the text are designed to forewarn the reader against serious errors. These passages are signposted in the margin with the sign

☡

(“khúc quanh nguy hiểm”).

7. The Exercises are designed both to enable the reader to satisfy himself that he has digested the text and to bring to his notice results which have no place in the text but which are nonetheless of interest. The most difficult exercises bear the sign ¶.

8. In general, we have adhered to the commonly accepted terminology, except where there appeared to be good reasons for deviating from it.

9. We have made a particular effort always to use rigorously correct language, without sacrificing simplicity. As far as possible we have drawn attention in the text to *abuses of language*, without which any mathematical text runs the risk of pedantry, not to say unreadability.

10. Since in principle the text consists of the dogmatic exposition of a theory, it contains in general no references to the literature. Bibliographical references are gathered together in *Historical Notes*, usually at the end of each chapter. These notes also contain indications, where appropriate, of the unsolved problems of the theory.

VI

Thư mục đi sau mỗi ghi chú lịch sử nói chung chỉ chứa những sách và hồi ký nguyên bản có tầm quan trọng lớn nhất trong sự phát triển của lý thuyết đang được bàn đến. Nó không hề có tham vọng đầy đủ; đặc biệt, những tài liệu tham khảo chỉ nhằm xác định các vấn đề về quyền ưu tiên hầu như luôn được bỏ qua.
Đối với các bài tập, nói chung chúng tôi không thấy đáng để chỉ ra nguồn gốc của chúng, vì chúng được lấy từ nhiều nguồn khác nhau (các bài báo gốc, các giáo trình, các tuyển tập bài tập).

11. References to a part of this series are given as follows :
a) If reference is made to theorems, axioms, or definitions presented *in the same section*, they are quoted by their number.
b) If they occur *in another section of the same chapter*, this section is also quoted in the reference.
c) If they occur *in another chapter in the same Book*, the chapter and section are quoted.
d) If they occur *in another Book*, this Book is first quoted by its title.

Các *Tóm tắt các kết quả* được trích dẫn bằng chữ cái R : như vậy *Lý thuyết tập hợp*, R có nghĩa là “*Tóm tắt các kết quả của lý thuyết tập hợp*”.

# MỤC LỤC
# CỦA
# BỘ SÁCH CÁC CƠ SỞ CỦA TOÁN HỌC

## I. LÝ THUYẾT TẬP HỢP

1. Description of formal mathematics.  2. Theory of sets.  3. Ordered sets; cardinals; natural numbers.  4. Structures.

## II. ĐẠI SỐ

1. Algebraic structures.  2. Linear algebra.  3. Tensor algebras, exterior algebras, symmetric algebras.  4. Polynomials and rational fractions.
5. Fields.  6. Ordered groups and fields.  7. Modules over principal ideal rings.  8. Semi-simple modules and rings.  9. Sesquilinear and quadratic forms.

VII
