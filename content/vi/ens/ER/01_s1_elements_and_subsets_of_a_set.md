---
book: ens
book_title: Theory of Sets
chapter: ER
chapter_title: SUMMARY OF RESULTS
section: 1
section_title: Elements and subsets of a set
lang: vi
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 347-351
pdf_pages: 0352-0356
extraction: ocr
statements: 0
exercises: 0
content_sha256: c4ba72edd9791e05505ccb6f7a4cbeeb581dce579f157c1bbd5135499c0c3282
translated_from: content/en/ens/ER/01_s1_elements_and_subsets_of_a_set.md
source_content_sha256: 0e243e5f12383731f0a5a2c71334e71b3cefa638eb23c7b52b81096a04bed198
translation_model: gpt-5-6
translation_run: translate-vi-dc47367a
glossary_version: 34
glossary_terms_sha256: cdd573de76cd7908c689b91d97414b2e6e5606b27023a00f4365d72aa5d0f751
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 1. PHẦN TỬ VÀ TẬP CON CỦA MỘT TẬP HỢP

1. Một *tập hợp* gồm các *phần tử* có khả năng có những *tính chất* nhất định và có những *quan hệ* nhất định với nhau hoặc với các phần tử của những tập hợp khác.

2. Các tập hợp và các phần tử được biểu diễn trong các lập luận toán học bằng những ký hiệu hình thức, nói chung là các chữ cái (thuộc các bảng chữ cái khác nhau) hoặc các tổ hợp chữ cái và các dấu hiệu khác. Các quan hệ giữa các phần tử của một hoặc nhiều tập hợp được biểu diễn bằng cách đưa các ký hiệu biểu diễn các phần tử ấy vào một lược đồ đặc trưng cho quan hệ đang xét [^1]; và tương tự đối với các tính chất.

Một chữ cái có thể biểu diễn hoặc một phần tử *cố định* hoặc một phần tử *tùy ý* (còn gọi là phần tử *biến*, *đối số*, hoặc *tổng quát*) của một tập hợp. Khi một phần tử tùy ý được thay bằng một phần tử cố định trong một quan hệ (hoặc tính chất), ta nói phần tử tùy ý được cho giá trị là phần tử cố định này.

Để chỉ ra các phần tử xuất hiện trong một quan hệ không được viết tường minh, ta biểu diễn quan hệ đó bằng một ký hiệu như $\mathrm{R}\{x, y, z\}$ (nếu $x, y, z$ là các phần tử đang xét).

3. Một quan hệ hoặc một tính chất trong đó có các phần tử tùy ý [^2] được gọi là một *đẳng nhất thức* nếu nó trở thành một mệnh đề đúng với bất kỳ giá trị nào ta cho các phần tử tùy ý ấy. Nếu R và S biểu diễn hai quan hệ (hoặc tính chất), ta nói R *suy ra* S nếu S đúng bất cứ khi nào các phần tử tùy ý xuất hiện trong các quan hệ này được cố định sao cho R đúng. Các quan hệ (hoặc tính chất) R và S được gọi là *tương đương* nếu mỗi quan hệ suy ra quan hệ kia.

4. Cho $\mathrm{R}\{x,\ y,\ z\}$ là một quan hệ giữa các biến $x$, $y$, $z$. Cụm từ "với mọi $x$, $\mathrm{R}\{x,\ y,\ z\}$" là một quan hệ *giữa $y$ và $z$*, được xem là đúng đối với một hệ các giá trị đã cho của các biến sau nếu R đúng với các giá trị ấy của $y$ và $z$ và *mọi* giá trị của $x$. Cụm từ "tồn tại $x$ sao cho $\mathrm{R}\{x,\ y,\ z\}$" (hoặc "với một $x$, $\mathrm{R}\{x,\ y,\ z\}$") lại là một quan hệ giữa $y$ và $z$, được xem là đúng đối với một hệ các giá trị đã cho của $y$ và $z$ nếu, khi các biến này đã được cố định như vậy, có *ít nhất một* giá trị của $x$ sao cho R đúng. Tương tự đối với một quan hệ giữa một số tùy ý các biến.

Nếu $\overline{\mathrm{R}}$ biểu diễn *phủ định* của R, thì phủ định của "với mọi $x$, R" là "tồn tại $x$ sao cho $\overline{\mathrm{R}}$"; phủ định của "tồn tại $x$ sao cho R" là "với mọi $x$, $\overline{\mathrm{R}}$".

5. Nếu R, S biểu diễn hai quan hệ, ta xem "R và S" như một *quan hệ duy nhất*, được coi là đúng khi *cả* R *và* S đều đúng. Tương tự, "R hoặc S" là một quan hệ được coi là đúng khi *ít nhất một* trong các quan hệ R, S đúng (và, đặc biệt, khi cả hai đều đúng. Từ "hoặc" ở đây vì thế không mang nghĩa tuyển định mà đôi khi nó có trong ngôn ngữ thông thường). Gọi $\overline{\mathrm{R}}$, $\overline{\mathrm{S}}$ lần lượt là các phủ định của R, S. Khi đó phủ định của "R và S" là "$\overline{\mathrm{R}}$ hoặc $\overline{\mathrm{S}}$", và phủ định của "R hoặc S" là "$\overline{\mathrm{R}}$ và $\overline{\mathrm{S}}$".

6. Bằng cách viết hai ký hiệu, mỗi ký hiệu ở một phía của dấu "$=$" (đọc là "bằng"), ta có một quan hệ gọi là quan hệ *đẳng thức*, có nghĩa là hai ký hiệu biểu diễn *cùng một* phần tử. Phủ định của quan hệ này được thu được bằng cách viết cùng các ký hiệu ấy ở hai phía của dấu "$\neq$" (đọc là "không bằng" hoặc "khác").

7. Cho một tập hợp E và một *tính chất* của một phần tử tổng quát của E, những phần tử của E có tính chất này tạo thành một tập hợp mới, gọi là một *tập con* của E. Do đó, hai tính chất *tương đương* định nghĩa *cùng một* tập con của E, và ngược lại.

Cho A là một tập con của E. Khi $x$ là một phần tử tổng quát của E, tính chất "$x$ thuộc A" (tức là "$x$ là một phần tử của A") được viết là "$x \in A$"; tập hợp các phần tử có tính chất này rõ ràng chính là A.

Phủ định của tính chất này được viết là "$x \notin A$" (đọc là "$x$ không thuộc A"); tập hợp các phần tử của E có tính chất này được gọi là *phần bù* của A và được viết là $\complement A$ hoặc $E - A$.

8. Một số tính chất, chẳng hạn $x = x$, đúng với *mọi* phần tử của E. Hai tính chất bất kỳ như vậy là tương đương, và tập con do chúng định nghĩa chính là tập hợp E.

Mặt khác, một số tính chất, chẳng hạn $x \neq x$, không đúng với *bất kỳ* phần tử nào của E. Một lần nữa, hai tính chất bất kỳ như vậy là tương đương, và tập con do chúng định nghĩa được gọi là *tập con rỗng*, được ký hiệu bởi $\emptyset$.

Chú ý rằng E và $\emptyset$ là *phần bù* của nhau.

9. Cho $a$ là một phần tử xác định của E. Một số tính chất, chẳng hạn $x = a$, chỉ đúng với *duy nhất* phần tử $a$. Hai tính chất bất kỳ như vậy là tương đương; tập con do chúng định nghĩa được ký hiệu là $\{a\}$, và được gọi là tập con *gồm riêng a*.

10. Tập hợp mà các phần tử của nó là tất cả các *tập con* của một tập hợp E được gọi là *tập hợp các tập con* của E, và được ký hiệu bởi $\mathfrak{P}(E)$. Ta có $\emptyset \in \mathfrak{P}(E)$, $E \in \mathfrak{P}(E)$, và $\{x\} \in \mathfrak{P}(E)$ với mọi $x \in E$. Nếu $x$ ký hiệu một phần tử bất kỳ của E, và X một phần tử bất kỳ của $\mathfrak{P}(E)$, thì quan hệ "$x \in X$" giữa $x$ và X được gọi là *quan hệ thuộc*.

11. Cho $x$ và $y$ là hai phần tử của E và X là một phần tử bất kỳ của $\mathfrak{P}(E)$. Khi đó quan hệ đẳng thức "$x = y$" *tương đương* với quan hệ "với mọi X sao cho $x \in X$, ta có $y \in X$".

12. Cho X, Y là hai tập con của một tập hợp E. Nếu tính chất $x \in X$ kéo theo tính chất $x \in Y$, nói cách khác nếu mọi phần tử của X đều thuộc Y, thì ta nói X *được chứa trong* Y, hoặc Y *chứa* X, hoặc X *là một tập con của* Y. Quan hệ này giữa X và Y được gọi là quan hệ *bao hàm* (của X trong Y), và được ký hiệu bởi "$X \subset Y$" hoặc "$Y \supset X$". Phủ định của nó được ký hiệu bởi "$X \not\subset Y$" hoặc "$Y \not\supset X$".

Với mọi tập con X của E, ta có $\emptyset \subset X$ và $X \subset E$. Quan hệ thuộc "$x \in X$" tương đương với "$\{x\} \subset X$".

Quan hệ "$X \subset Y$ and $Y \subset Z$" kéo theo "$X \subset Z$".

Quan hệ "$X \subset Y$" không loại trừ khả năng "$X = Y$". Quan hệ "$X \subset Y$ and $Y \subset X$" tương đương với "$X = Y$".

13. Cho X và Y là hai tập con bất kỳ của E. Tập hợp tất cả các phần tử có tính chất "$x \in X$ or $x \in Y$" được ký hiệu bởi $X \cup Y$ và được gọi là *hợp* của X và Y. Tập hợp tất cả các phần tử có tính chất "$x \in X$ and $x \in Y$" được ký hiệu bởi $X \cap Y$ và được gọi là *giao* của X và Y.

Hợp và giao của nhiều tập con của E được định nghĩa theo cùng một cách.

Nếu $x$, $y$, $z$ là ba phần tử của E, hợp $\{x\} \cup \{y\} \cup \{z\}$ được ký hiệu bởi $\{x, y, z\}$. Tương tự đối với một số bất kỳ các phần tử (được đặt tên riêng).

Cho X và Y là hai tập con của E. Tùy theo $X \cap Y \neq \emptyset$ hay $X \cap Y = \emptyset$, ta nói X và Y *giao nhau* hoặc *rời nhau*.

14. Trong các phát biểu của các mệnh đề sau đây, X, Y, Z ký hiệu các tập con bất kỳ của cùng một tập hợp E.

(a) Ta có $\emptyset = \complement E$, $\quad E = \complement \emptyset$.

(b) Với mọi X, ta có

(1)
$$\complement(\complement X) = X;$$

(2)
$$X \cup X = X, \qquad X \cap X = X;$$

(3)
$$X \cup (\complement X) = E, \qquad X \cap (\complement X) = \emptyset;$$

(4)
$$X \cup \emptyset = X, \qquad X \cap E = X;$$

(5)
$$X \cup E = E, \qquad X \cap \emptyset = \emptyset.$$

(c) Với mọi X, Y, ta có

(6)
$$X \cup Y = Y \cup X, \qquad X \cap Y = Y \cap X \quad \text{(tính giao hoán)};$$

(7)
$$X \subset X \cup Y, \qquad X \cap Y \subset X;$$

(8)
$$\complement(X \cup Y) = (\complement X) \cap (\complement Y), \qquad \complement(X \cap Y) = (\complement X) \cup (\complement Y).$$

(d) Các quan hệ $X \subset Y$, $\complement X \supset \complement Y$, $X \cup Y = Y$, $X \cap Y = X$ là *tương đương*.

(e) Các quan hệ $X \cap Y = \emptyset$, $X \subset \complement Y$, $Y \subset \complement X$ là *tương đương*.

(f) Các quan hệ $X \cup Y = E$, $\complement X \subset Y$, $\complement Y \subset X$ là *tương đương*.

(g) Với mọi X, Y, Z ta có

(9)
$$\left.\begin{array}{l} X \cup (Y \cup Z) = (X \cup Y) \cup Z = X \cup Y \cup Z \\ X \cap (Y \cap Z) = (X \cap Y) \cap Z = X \cap Y \cap Z \end{array}\right\} \quad \text{(tính kết hợp)};$$

(10)
$$\left.\begin{array}{l} X \cup (Y \cap Z) = (X \cup Y) \cap (X \cup Z) \\ X \cap (Y \cup Z) = (X \cap Y) \cup (X \cap Z) \end{array}\right\} \quad \text{(tính phân phối)}.$$

(h) Quan hệ "$X \subset Y$" kéo theo các quan hệ "$X \cup Z \subset Y \cup Z$" và "$X \cap Z \subset Y \cap Z$".

(i) Quan hệ "$Z \subset X$ và $Z \subset Y$" tương đương với "$Z \subset X \cap Y$". Quan hệ "$X \subset Z$ và $Y \subset Z$" tương đương với "$X \cup Y \subset Z$".

15. Từ các đẳng thức (8) ta kết luận rằng nếu một tập con A của E được tạo thành từ các tập con X, Y, Z khác của E bằng cách áp dụng *chỉ* các phép toán $\complement$, $\cup$, $\cap$ (theo một thứ tự tùy ý), thì phần bù $\complement A$ có thể được thu được bằng cách thay thế các tập con X, Y, Z bởi các phần bù tương ứng của chúng, và các phép toán $\cup$, $\cap$ lần lượt bởi $\cap$, $\cup$, trong khi vẫn giữ nguyên thứ tự của các phép toán. Đây là *quy tắc đối ngẫu*. Cho một đẳng thức $A = B$ giữa các tập con có dạng nói trên, xét đẳng thức tương đương $\complement A = \complement B$. Nếu ta thay thế $\complement A$ và $\complement B$ bởi các biểu thức thu được bằng cách áp dụng quy tắc đối ngẫu, rồi nếu ta thay thế $\complement X$, $\complement Y$, $\complement Z$ lần lượt bởi X, Y, Z, và ngược lại, ta thu được một đẳng thức được gọi là *đối ngẫu* của $A = B$. Ta có thể làm tương tự đối với một quan hệ bao hàm $A \subset B$, nhưng khi đó phải chú ý thay dấu " $\subset$ " bởi " $\supset$ ".

Các đẳng thức ở trên mang cùng một số là các đối ngẫu của nhau.

16. Trong một số câu hỏi, ta phải xét một tập con cố định A của một tập hợp E. Nếu X là một tập con tùy ý của E, tập hợp $A \cap X$ được gọi là *vết* của X trên A, và đôi khi được ký hiệu bởi $X_A$; trong trường hợp này, nó được coi là một tập con của A. Với mọi tập con X, Y của E, ta có

$$(X \cup Y)_A = X_A \cup Y_A, \qquad (X \cap Y)_A = X_A \cap Y_A,$$

và
$$\complement_A X_A = (\complement_E X)_A,$$

trong đó $\complement_E X$ ký hiệu phần bù của X trong E và $\complement_A X_A$ ký hiệu phần bù của $X_A$ trong A.

Nếu $\mathfrak{S}$ ký hiệu một tập hợp các tập con của E, thì tập hợp $\mathfrak{S}_A$ gồm các vết trên A của các tập hợp thuộc $\mathfrak{S}$ được gọi là *vết* của $\mathfrak{S}$ trên A.

[^1]: Khi ký hiệu biểu thị một phần tử là một tổ hợp gồm nhiều dấu và cần được đưa vào một quan hệ ở vị trí của một chữ cái duy nhất, người ta thường đặt nó trong ngoặc để tránh mọi sự nhầm lẫn có thể xảy ra.

[^2]: Cần nhấn mạnh rằng, khi ta nói về một *tính chất của một* phần tử *tổng quát* của một tập hợp E, điều này hoàn toàn không hàm ý rằng tính chất đó đúng đối với *mọi* phần tử của E, mà chỉ đơn giản có nghĩa là nó *có ý nghĩa* đối với *mọi* phần tử của E; nó có thể đúng đối với một số phần tử trong số đó và sai đối với những phần tử khác. Điều tương tự cũng đúng đối với các quan hệ.
