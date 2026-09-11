---
book: ens
book_title: Theory of Sets
chapter: ER
chapter_title: SUMMARY OF RESULTS
section: 4
section_title: Union, intersection, product of a family of sets
lang: vi
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 363-370
pdf_pages: 0368-0375
extraction: ocr
statements: 0
exercises: 0
content_sha256: 87ba2ccd7d84125d2ec363b2d4009197b50afe4d29db0d8d0e8dfa6bf9f31a8d
translated_from: content/en/ens/ER/04_s4_union_intersection_product_of_a_family.md
source_content_sha256: f9b5a61bff54537ebfed0e8bade3350c49d974cf5c55ab2cbce40ab5f4be65d9
translation_model: gpt-5-6
translation_run: translate-vi-7841d112
glossary_version: 34
glossary_terms_sha256: 544918c35e4612ce0b577bd73ac00f86ed8682cc9d3388179ff4b9c16ee5a47c
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 4. HỢP, GIAO, TÍCH CỦA MỘT HỌ TẬP HỢP

1. Trong tiết diện này, ta xét một họ $(X_i)_{i\in I}$ các tập con của một tập hợp $E$, trong đó tập chỉ số $I$ là tùy ý; tập hợp các tập con của $E$ thuộc họ được ký hiệu là $\mathfrak{X}$ (do đó là một tập con của $\mathfrak{P}(E)$).

Nếu $I$ là hữu hạn, việc xét họ $(X_i)$ quy về việc xét một số tập con của $E$, có thể phân biệt hoặc không phân biệt, và số lượng bằng số phần tử của $I$. Ví dụ, ba tập con bất kỳ $X_1,X_2,X_3$ của $E$ lập thành một họ các tập con của $E$, tập chỉ số ở đây gồm các số 1, 2, 3.

2. Cho $J$ là một tập con tùy ý của $I$, và xét tập hợp tất cả các phần tử $x$ có tính chất “tồn tại $i\in J$ sao cho $x\in X_i$”. Tập hợp này được gọi là hợp của họ các tập hợp $(X_i)_{i\in J}$, và được ký hiệu là $\displaystyle\bigcup_{i\in J}X_i$.

Ta cũng có thể phát biểu định nghĩa này như sau: tương ứng với ánh xạ $i\mapsto X_i$ của $I$ vào $\mathfrak{P}(E)$ là một tập con $C$ xác định rõ của $I\times E$ sao cho $X_i=C(i)$ (§ 3, no. 7), và ta có $\displaystyle\bigcup_{i\in J}X_i=C(J)$.

Đặc biệt,

$$
\bigcup_{i\in\varnothing}X_i=C(\varnothing)=\varnothing .
$$

Khi $J=I$, ta thường viết $\displaystyle\bigcup X_i$, hoặc đơn giản là $\displaystyle\bigcup X_i$, thay cho $\displaystyle\bigcup_{i\in I}X_i$.

Hợp $\displaystyle\bigcup_{i\in I}X_i$ chỉ phụ thuộc vào tập hợp $\mathfrak{X}$; nói cách khác, nó giống nhau đối với hai họ tương ứng với cùng một tập con $\mathfrak{X}$ của $\mathfrak{P}(E)$. Đặc biệt, nó bằng hợp của họ được xác định bởi ánh xạ chính tắc của $\mathfrak{X}$ vào $\mathfrak{P}(E)$, và do đó ta có thể viết $\displaystyle\bigcup_{X\in\mathfrak{X}}X$, cũng được gọi là hợp của các tập hợp thuộc $\mathfrak{X}$.

Khi $I$ là một tập hợp mà các phần tử của nó được chỉ rõ tường minh, chẳng hạn các số 1, 2, 3, ta có

$$
\bigcup_{i\in I}X_i=X_1\cup X_2\cup X_3,
$$

điều này giải thích tên gọi “hợp” được đặt trong trường hợp tổng quát cho tập hợp $\displaystyle\bigcup_{i\in I}X_i$.

# TÓM TẮT CÁC KẾT QUẢ

3. Với mọi $J\subset I$ ta có

$$
\bigcup_{\iota\in J}X_{\iota}\subset\bigcup_{\iota\in I}X_{\iota}.
$$

Đặc biệt, với mọi $\iota\in I$, ta có

$$
X_{\iota}\subset\bigcup_{\iota\in I}X_{\iota}.
$$

Ngược lại, nếu $Y$ là một tập con của $E$ sao cho $X_{\iota}\subset Y$ với mọi $\iota\in I$, thì

$$
\bigcup_{\iota}X_{\iota}\subset Y.
$$

Tổng quát hơn, nếu $(Y_{\iota})$ là một họ khác các tập con của $E$, được đánh chỉ số bởi cùng tập hợp $I$, và nếu $X_{\iota}\subset Y_{\iota}$ với mọi $\iota\in I$, thì

$$
\bigcup_{\iota}X_{\iota}\subset\bigcup_{\iota}Y_{\iota}.
$$

Cho $F$ là một tập hợp khác, và cho $X\to K(X)$ là ánh xạ từ $\mathfrak{P}(E)$ vào $\mathfrak{P}(F)$ được xác định bởi một tập con $K$ của $E\times F$. Khi đó ta có

(34)

$$
K\left(\bigcup_{\iota\in J}X_{\iota}\right)=\bigcup_{\iota\in J}K(X_{\iota}).
$$

Bây giờ cho $L$ là một tập hợp chỉ số khác, và $(J_{\lambda})_{\lambda\in L}$ là một họ các tập con của $I$. Khi đó

(35)

$$
\bigcup_{\iota\in\bigcup_{\lambda\in L}J_{\lambda}}X_{\iota}
=
\bigcup_{\lambda\in L}\left(\bigcup_{\iota\in J_{\lambda}}X_{\iota}\right).
$$

Đây là công thức *tính kết hợp* tổng quát đối với các phép hợp. Khi $I$ và $L$ là các tập hợp mà các phần tử của chúng được chỉ định tường minh, các quan hệ thu được đã được nêu (xem § 1, no. 14). Nếu chỉ $L$ thỏa mãn điều kiện này và gồm, chẳng hạn, các số 1, 2, thì ta có

(36)

$$
\bigcup_{\iota\in J_1\cup J_2}X_{\iota}
=
\left(\bigcup_{\iota\in J_1}X_{\iota}\right)\cup
\left(\bigcup_{\iota\in J_2}X_{\iota}\right).
$$

Cho $(X_{\iota})_{\iota\in I}$ và $(Y_{\chi})_{\chi\in K}$ là hai họ bất kỳ các tập con của $E$. Khi đó ta có

(37)

$$
\left(\bigcup_{\iota\in I}X_{\iota}\right)\cap
\left(\bigcup_{\chi\in K}Y_{\chi}\right)
=
\bigcup_{(\iota,\chi)\in I\times K}(X_{\iota}\cap Y_{\chi}).
$$

công thức *tính phân phối*, bao hàm công thức thứ hai của (10) như một trường hợp riêng.

Nếu $(X_i)_{i\in I}$ là một họ các tập con của E, và nếu $(Y_x)_{x\in K}$ là một họ các tập con của F, thì

(38)

$$
\left(\bigcup_{i\in I}X_i\right)\times\left(\bigcup_{x\in K}Y_x\right)=\bigcup_{(i,x)\in I\times K}(X_i\times Y_x).
$$

4. Một họ $(X_i)_{i\in I}$ các tập con của E là một *phủ* của một tập con A của E, hay phủ A, nếu

$$
A\subset\bigcup_{i\in I}X_i.
$$

Đặc biệt, nếu $(X_i)$ là một *phủ* của E, ta có

$$
\bigcup_{i\in I}X_i=E.
$$

Một *phân hoạch* của E là một *phủ* $(X_i)$ của E sao cho

(a) $X_i\neq\varnothing$ với mọi $i\in I$;

(b) $X_i\cap X_j=\varnothing$ với mỗi cặp chỉ số *khác nhau* $i,\ j$ trong I. (Điều kiện thứ hai này có thể được diễn đạt bằng cách nói rằng các $X_i$ *rời nhau từng đôi một*.)

Các điều kiện này suy ra rằng $i\mapsto X_i$ là một *song ánh* từ I lên tập hợp $\mathfrak{P}$ gồm các tập con của phân hoạch. Do đó, nếu $\mathfrak{P}$ được cho, thì họ được xác định sai khác bởi một sự tương ứng một-một giữa các tập hợp chỉ số. Đặc biệt, một phân hoạch có thể được xem không phân biệt như một tập hợp các tập con hoặc như một *họ* các tập con.

5. Cho $(X_i)_{i\in I}$ là một họ bất kỳ các tập con khác rỗng của một tập hợp E. Trong tích $I\times E$, ký hiệu $X'_i$ là tập con $\{i\}\times X_i$ với mỗi $i\in I$. Tập hợp

$$
S=\bigcup_{i\in I}X'_i
$$

được gọi là *tổng* của họ $(X_i)_{i\in I}$. Rõ ràng họ $(X'_i)_{i\in I}$ là một phân hoạch của S và với mỗi $i\in I$ ánh xạ $x_i\mapsto(i,x_i)$ là một song ánh từ $X_i$ lên $X'_i$. Do lạm dụng ngôn ngữ, bất kỳ tập hợp nào có sự tương ứng một-một với S thường được gọi là tổng của họ $(X_i)_{i\in I}$, và các $X_i$ thường được đồng nhất với các tập con của tập hợp này mà chúng tương ứng.

Tổng của hai tập hợp khác rỗng E và F thường được nói là thu được bằng cách *ghép thêm* tập hợp F vào E.

6. Với ký hiệu của no. 2, tập hợp các phần tử $x$ của E có tính chất “với mọi $i\in J$, $x\in X_i$” được gọi là *giao của họ các tập hợp*

$(X_\iota)_{\iota\in J}$, và được ký hiệu bởi $\displaystyle\bigcap_{\iota\in J}X_\iota$; khi $J=I$, ta thường viết $\displaystyle\bigcap_\iota X_\iota$, hoặc đơn giản $\displaystyle\cap X_\iota$, thay cho $\displaystyle\bigcap_{\iota\in I}X_\iota$.

Ta có

(39)
$$
\mathrm{C}\left(\bigcup_{\iota\in J}X_\iota\right)=\bigcap_{\iota\in J}(\mathrm{C}X_\iota).
$$

Đặc biệt, nếu $J=\varnothing$,

(40)
$$
\bigcap_{\iota\in\varnothing}X_\iota=E.
$$

Giao $\displaystyle\bigcap_\iota X_\iota$ chỉ phụ thuộc vào tập hợp $\mathfrak{F}$, và có thể được viết là $\displaystyle\bigcap_{X\in\mathfrak{F}}X$. Ví dụ, nếu $I$ gồm các số $1$, $2$, $3$, thì ta có

$$
\bigcap_\iota X_\iota=X_1\cap X_2\cap X_3.
$$

7. Công thức (39) cho phép ta tổng quát hóa *quy tắc đối ngẫu*. Nếu một tập con A của E được thu được từ các tập con khác X, Y, Z và các họ $(X_\iota)$, $(Y_\iota)$, $(Z_\lambda)$ của các tập con của E bằng cách áp dụng (theo thứ tự bất kỳ) *chỉ* các phép toán $\mathrm{C}$, $\cup$, $\cap$, $\displaystyle\bigcup$, $\displaystyle\bigcap$, thì ta sẽ thu được phần bù $\mathrm{C}A$ bằng cách thay thế các tập con X, Y, Z, $X_\iota$, $Y_\iota$, $Z_\lambda$ bằng các phần bù của chúng, và các phép toán $\cup$, $\cap$, $\displaystyle\bigcup$, $\displaystyle\bigcap$ lần lượt bằng $\cap$, $\cup$, $\displaystyle\bigcap$, $\displaystyle\bigcup$, trong khi vẫn giữ nguyên thứ tự của các phép toán; dĩ nhiên, các phép toán giao và hợp không được thay đổi khi chúng áp dụng vào các tập hợp *chỉ số* được viết dưới các dấu $\displaystyle\bigcup$ và $\displaystyle\bigcap$.

Như trong § 1, no. 15, ta định nghĩa *đối ngẫu* của một quan hệ A = B hoặc A $\subset$ B trong đó A và B là các tập con của E có dạng trên.

8. Với mọi $J\subset I$ ta có

$$
\bigcap_{\iota\in I}X_\iota\subset\bigcap_{\iota\in J}X_\iota.
$$

Đặc biệt, với mọi $x\in I$ ta có

$$
\bigcap_\iota X_\iota\subset X_x.
$$

Ngược lại, nếu $Y\subset X_\iota$ với mọi $\iota\in I$, thì

$$
Y\subset\bigcap_\iota X_\iota.
$$

Nói chung, nếu $(Y_i)$ là một họ khác của các tập con của E, được đánh chỉ số bởi cùng một tập hợp I, và nếu $X_i\subset Y_i$ với mọi $i\in I$, thì

$$\bigcap_{i}X_i\subset\bigcap_iY_i.$$

Hợp của các tập hợp $X_i$ là giao của tất cả các tập hợp $Y$ sao cho $X_i\subset Y$ với mọi $i\in I$. Giao của các $X_i$ là hợp của tất cả các $Z$ sao cho $Z\subset X_i$ với mọi $i\in I$.

Các công thức sau là các đối ngẫu của (35) và (37), tương ứng:

(41)

$$\bigcap_{i\in\bigcup_{\lambda\in L}J_\lambda}X_i=\bigcap_{\lambda\in L}\left(\bigcap_{i\in J_\lambda}X_i\right)\qquad\text{(tính kết hợp)};$$

(42)

$$\left(\bigcap_{i\in I}X_i\right)\cup\left(\bigcap_{x\in K}Y_x\right)=\bigcap_{(i,x)\in I\times K}(X_i\cup Y_x)\qquad\text{(tính phân phối)}.$$

Nếu $(X_i)_{i\in I}$ là một họ các tập con của E, và $(Y_x)_{x\in K}$ là một họ các tập con của F, thì

(43)

$$\left(\bigcap_{i\in I}X_i\right)\times\left(\bigcap_{x\in K}Y_x\right)=\bigcap_{(i,x)\in I\times K}(X_i\times Y_x).$$

Hơn nữa, nếu $(X_i)$ và $(Y_i)$ lần lượt là các họ các tập con của E và F, được đánh chỉ số bởi cùng một tập hợp I, thì

(44)

$$\left(\bigcap_{i\in I}X_i\right)\times\left(\bigcap_{i\in I}Y_i\right)=\bigcap_{i\in I}(X_i\times Y_i).$$

Công thức (34) không có đối ngẫu; nói chung, tất cả những gì ta có thể nói là

(45)

$$K\left(\bigcap_{i\in J}X_i\right)\subset\bigcap_{i\in J}K(X_i).$$

Ta có đẳng thức (45) với mọi họ $(X_i)$ khi và chỉ khi $X\mapsto K(X)$ là mở rộng nghịch đảo của một ánh xạ từ một tập con của F vào E. Do đó, nếu $f$ là một ánh xạ từ F vào E, ta có (tổng quát hóa (14))

(46)

$$\overline{f}^{\, -1}\left(\bigcap_{i\in J}X_i\right)=\bigcap_{i\in J}\overline{f}^{\, -1}(X_i).$$

9. Cho E là một tập hợp bất kỳ và I là một tập hợp chỉ số bất kỳ. Tập hợp tất cả các họ $(x_i)_{i\in I}$ gồm các phần tử của E, được đánh chỉ số bởi I, được ký hiệu là $E^I$, và phép toán chuyển từ E sang $E^I$ được gọi là phép lũy thừa. Do đó, $E^I$ tương ứng một-một với tập hợp tất cả các ánh xạ từ I vào E (vì lý do này, bằng cách lạm dụng ngôn ngữ, thường cũng được ký hiệu là $E^I$), cũng như với một tập con của $\mathfrak{P}(I \times E)$, bằng cách xét các đồ thị của các ánh xạ này. Do đó, các tập hợp $E^J$ tương ứng với các tập con $J$ của tập hợp I có thể được coi tất cả là các tập con của cùng một tập hợp, tập hợp này tương ứng một-một với một tập con của $\mathfrak{P}(I \times E)$.

Bây giờ cho $(X_\ell)_{\ell\in I}$ là một *họ các tập con* của E, được đánh chỉ số bởi cùng tập hợp I, và cho J là một tập con bất kỳ của I. Tính chất “với mọi $\ell\in J$, $x_\ell\in X_\ell$,” của họ $(x_\ell)_{\ell\in J}$ xác định một tập con của $E^J$, được gọi là *tích của họ các tập hợp* $(X_\ell)_{\ell\in J}$, và được ký hiệu là $\displaystyle\prod_{\ell\in J} X_\ell$ (hoặc đơn giản là $\displaystyle\prod_\ell X_\ell$ khi $J=I$). Các $X_\ell$ được gọi là *các thừa số* của tích. Chú ý rằng $\displaystyle\prod_{\ell\in\varnothing} X_\ell$ là một tập hợp gồm một phần tử (tương ứng với tập con rỗng của $I\times E$). Nếu $X_\ell=E$ với mọi $\ell\in J$, thì ta có

$$
\prod_{\ell\in J} X_\ell=E^J.
$$

Chẳng hạn, nếu I gồm ba số 1, 2, 3, thì $\displaystyle\prod_{\ell\in J} X_\ell$ tương ứng một-một với tập hợp $X_1\times X_2\times X_3$.

10. Nếu $R\{x,y\}$ là một quan hệ giữa một phần tử tùy ý $x$ của một tập hợp E và một phần tử tùy ý $y$ của một tập hợp F, thì các mệnh đề sau là *tương đương*:

“với mỗi $x$ tồn tại $y$ sao cho $R\{x,y\}$”

và

“tồn tại một ánh xạ $f$ từ E vào F sao cho $R\{x,f(x)\}$ với mọi $x$”.

Mệnh đề về tương đương này được gọi là *tiên đề lựa chọn* (hay *tiên đề Zermelo*). Đôi khi chúng ta sẽ chỉ rõ liệu chứng minh của một định lý có phụ thuộc vào tiên đề này hay không.

Tiên đề lựa chọn *tương đương* với mệnh đề sau: “nếu với mỗi $\ell\in I$, ta có $X_\ell\ne\varnothing$, thì $\displaystyle\prod_{\ell\in I}X_\ell\ne\varnothing$”.

11. Trong tiểu mục này và tiểu mục tiếp theo, ta sẽ xét một tích khác rỗng $\displaystyle\prod_{\ell\in I}A_\ell$, trong đó $(A_\ell)$ là một *họ* bất kỳ gồm các tập con (khác rỗng) của E.

Cho J là một tập con của I. Ánh xạ $(x_\ell)_{\ell\in I}\to(x_\ell)_{\ell\in J}$ từ $\displaystyle\prod_{\ell\in I}A_\ell$ lên $\displaystyle\prod_{\ell\in J}A_\ell$ được gọi là *phép chiếu* của $\displaystyle\prod_{\ell\in I}A_\ell$ lên $\displaystyle\prod_{\ell\in J}A_\ell$, và được ký hiệu bởi $\operatorname{pr}_J$.

Đặc biệt, ánh xạ $(x_\ell)_{\ell\in I}\to x_\kappa$ từ $\displaystyle\prod_{\ell\in I}A_\ell$ lên $A_\kappa$ được gọi là *hàm tọa độ* (hay *phép chiếu*) có *chỉ số* $\kappa$, và được ký hiệu bởi $\operatorname{pr}_\kappa$.

Nếu $z$ là một phần tử của $\displaystyle\prod_{\ell\in I}A_\ell$, thì ta có $z=(\operatorname{pr}_\ell z)_{\ell\in I}$.

Cho $J_1, J_2$ là hai tập hợp lập thành một phân hoạch của $I$. Khi đó $z\mapsto(\operatorname{pr}_{J_1}z,\operatorname{pr}_{J_2}z)$ là một ánh xạ một-một từ $\prod_{i\in I}A_i$ lên $\prod_{i\in J_1}A_i\times\prod_{i\in J_2}A_i$.

Nói chung, nếu $(J_\lambda)_{\lambda\in L}$ là một phân hoạch bất kỳ của tập hợp $I$, thì ánh xạ $z\mapsto(\operatorname{pr}_{J_\lambda}z)_{\lambda\in L}$ là một song ánh (gọi là chính tắc) từ $\prod_{i\in I}A_i$ lên tích $\prod_{\lambda\in L}(\prod_{i\in J_\lambda}A_i)$. Điều này cũng có thể được diễn đạt bằng cách nói rằng tích của một họ tập hợp là kết hợp.

12. Các mệnh đề sau đây khái quát những mệnh đề ở §3, no. 3; $(X_i)$, $(Y_i)$ ký hiệu các họ tập con của $E$ sao cho $X_i\subset A_i$, và $Y_i\subset A_i$, với mọi $i\in I$; $Z$ ký hiệu một tập con bất kỳ của $\prod A_i$.

(a) Nếu $\prod_iX_i\neq\varnothing$, quan hệ “$\prod_iX_i\subset\prod_iY_i$” tương đương với “với mọi $i\in I$, $X_i\subset Y_i$”.

(b) Ta có $\operatorname{pr}_x^{-1}(X_x)=\prod_iY_i$, trong đó $Y_x=X_x$ và $Y_i=A_i$ mỗi khi $i\neq x$. Do đó

$$
\prod_{i\in I}X_i=\bigcap_{i\in I}\operatorname{pr}_i^{-1}(X_i).
$$

(c) Nếu $\prod_iX_i\neq\varnothing$, thì

$$
\operatorname{pr}_x\left(\prod_iX_i\right)=X_x.
$$

(d) Với mọi $Z$, ta có

$$
Z\subset\prod_i\operatorname{pr}_i(Z).
$$

(e) Cho $(J_1,J_2)$ là một phân hoạch của $I$ thành hai tập hợp, cho $(a_i)_{i\in J_1}$ là một họ các phần tử của $E$, và cho $(X_i)_{i\in J_2}$ là một họ các tập con của $E$, sao cho $a_i\in A_i$ với mọi $i\in J_1$, và $X_i\subset A_i$ với mọi $i\in J_2$. Khi đó tích $\prod_iY_i$, trong đó $Y_i=\{a_i\}$ khi $i\in J_1$, và $Y_i=X_i$ khi $i\in J_2$, có thể đặt trong một sự tương ứng một-một với $\prod_{i\in J_2}X_i$ bằng cách chiếu lên tập hợp sau.

13. Cho $(A_i)_{i\in I}$ là một họ các tập con của một tập hợp $F$, và cho $f$ là một ánh xạ từ một tập hợp $E$ vào tích $\prod_iA_i$. Nếu đặt $f_i(x)=\operatorname{pr}_i(f(x))$, thì $f_i$ là một ánh xạ từ $E$ vào $A_i$, và $f$ là ánh xạ $x\mapsto(f_i(x))$. Ngược lại, nếu với mỗi chỉ số $i\in I$, $f_i$ là một ánh xạ từ $E$ vào $A_i$, thì

$$
x\mapsto(f_i(x))
$$

là một ánh xạ từ E vào $\prod_{i\in I} A_i$, được ký hiệu bởi $(f_i)$ (lạm dụng ngôn ngữ, vì ký hiệu này đã chỉ họ các ánh xạ $f_i$). Do đó ta định nghĩa một song ánh (gọi là chính tắc) từ tập hợp $(\prod_{i\in I} A_i)^E$ lên tập hợp $\prod_{i\in I}(A_i^E)$.

14. Cho E, F, G là ba tập hợp. Với mỗi ánh xạ $f$ từ $F \times G$ vào $E$ và với mỗi $y\in G$, ký hiệu $f_y$ là ánh xạ bộ phận $x\mapsto f(x,y)$ từ $F$ vào $E$. Khi đó $y\mapsto f_y$ là một ánh xạ từ $G$ vào $E^F$. Ngược lại, với mỗi ánh xạ $g$ từ $G$ vào $E^F$ tồn tại một ánh xạ duy nhất $f$ từ $F\times G$ vào $E$ sao cho $f_y=g(y)$ với mọi $y\in G$. Do đó ta định nghĩa một song ánh (gọi là chính tắc) từ tập hợp $E^{F\times G}$ lên tập hợp $(E^F)^G$.

15. Cho $(A_i)_{i\in I}$ là một họ các tập con khác rỗng của một tập hợp E. Với mỗi $i\in I$, cho $f_i$ là một ánh xạ từ $A_i$ vào một tập hợp F sao cho, với mỗi cặp chỉ số $(i,x)$, $f_i$ và $f_x$ trùng nhau trên $A_i\cap A_x$. Khi đó, nếu

$$
A=\bigcup_{i\in I}A_i,
$$

tồn tại một ánh xạ duy nhất $f$ từ A vào F sao cho hạn chế của $f$ trên mỗi $A_i$ bằng $f_i$. Đặc biệt, nếu $A_i\cap A_x=\varnothing$ mỗi khi $i\ne x$, ta thấy rằng các tập hợp $F^A$ và $\prod_{i\in I}F^{A_i}$ có sự tương ứng một-một (gọi là chính tắc).
