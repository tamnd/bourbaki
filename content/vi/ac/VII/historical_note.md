---
book: ac
book_title: Commutative Algebra
chapter: VII
chapter_title: DIVISORS
section: 0
section_title: Historical Note
kind: historical
lang: vi
source: ac-i-vii
book_pages: 579-625
pdf_pages: 0597-0642
extraction: ocr
statements: 0
exercises: 0
content_sha256: c26bd9d8cff95f7e80315ab5d9225fb9db6c59f04eb3cdbe00fc29692a3a1b26
translated_from: content/en/ac/VII/historical_note.md
source_content_sha256: 310b51f7681f87389ad268cda064f6af31cea24a76ec2275974603d2dfff3682
translation_model: gpt-5-6-mini, gpt-5-6, gpt-5-mini, copied
translation_run: translate-vi-580ac2ef
glossary_version: 34
glossary_terms_sha256: 2cc4573acf7ed1aa986fe8475431773d9db4bc6521c4ef0badf04aaa394e31a7
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

# GHI CHÚ LỊCH SỬ

(Các số trong ngoặc vuông chỉ đến thư mục tài liệu ở cuối Ghi chú này.)

Đại số giao hoán "trừu tượng" là một sáng tạo gần đây nhưng sự phát triển của nó chỉ có thể được hiểu như một hàm của sự phát triển của lý thuyết số đại số và hình học đại số, những thứ đã sinh ra nó.

Người ta đã phỏng đoán, không phải không có lý do, rằng "chứng minh" nổi tiếng mà Fermat tuyên bố sở hữu về tính không thể có của phương trình $x^p + y^p = z^p$ với $p$ là một số nguyên tố lẻ và $x, y, z$ là các số nguyên $\neq 0$ phụ thuộc vào sự phân tích

$$
(x + y)(x + \zeta y) \ldots (x + \zeta^{p-1} y) = z^p
$$

trong vành $\mathbf{Z}[\zeta]$ (trong đó $\zeta \neq 1$ là một nghiệm bậc $p$ của đơn vị) và vào một lập luận về tính chia hết trong vành này, giả sử nó là một miền iđêan chính. Trong mọi trường hợp, một lập luận tương tự được Lagrange phác thảo ([2], vol. II, p. 531); chính bằng các lập luận kiểu này, với một số biến đổi nhất định (đặc biệt là các phép đổi biến nhằm hạ bậc của phương trình), Euler ([1], vol. I, p. 488) (*) và Gauss ([3], vol. II, p. 387) chứng minh Định lý Fermat với $p = 3$, Gauss (loc. cit.) và Dirichlet ([4], vol. I, p. 42) với $p = 5$ và Dirichlet chứng minh tính không thể có của phương trình $x^{14} + y^{14} = z^{14}$ ([4], vol. I, p. 190). Cuối cùng, trong nghiên cứu đầu tiên của ông về lý thuyết số, Kummer tin rằng ông đã thu được bằng cách này một chứng minh tổng quát và chắc chắn chính sai lầm này (mà Dirichlet đã chỉ ra cho ông) đã dẫn ông đến nghiên cứu số học của các trường cyclotomic, từ đó cuối cùng ông đã thành công trong việc suy ra một phiên bản đúng của chứng minh của mình cho các số nguyên tố $p < 100$ [7d].

Mặt khác, hồi ký nổi tiếng của Gauss năm 1831 về

(*) Trong chứng minh, Euler lập luận như thể $\mathbf{Z}[\sqrt{-3}]$ là một miền iđêan chính, điều này không đúng; tuy nhiên, lập luận của ông có thể được làm cho đúng bằng cách xét vành dẫn của $\mathbf{Z}[\rho]$ ($\rho$ là một nghiệm bậc ba của đơn vị) trên $\mathbf{Z}[\sqrt{-3}]$ (cf. Sommer, Introduction à la théorie des nombres algébriques (trans. A. Lévy), Paris (Hermann), 1911, p. 190).

các thặng dư song bình phương, với các kết quả được suy ra từ một nghiên cứu chi tiết về tính chia hết trong vành $\mathbf{Z}[i]$ của "các số nguyên Gaussian" ([3], vol. II, p. 109), đã chỉ ra rõ ràng sự quan tâm mà việc mở rộng tính chia hết sang các số đại số có thể mang lại cho các bài toán cổ điển của lý thuyết số (*); vì vậy không có gì đáng ngạc nhiên rằng giữa năm 1830 và 1850 lý thuyết này là đối tượng của nhiều công trình của các nhà toán học Đức, trước hết là Jacobi, Dirichlet và Eisenstein, rồi sau đó một ít là Kummer và học trò cũng như bạn của ông là Kronecker. Ở đây chúng ta sẽ không nói về lý thuyết các đơn vị, một nhánh quá chuyên biệt của lý thuyết số, nơi sự tiến bộ diễn ra rất nhanh, Eisenstein thu được cấu trúc của nhóm các đơn vị cho các trường bậc ba và Kronecker cho các trường cyclotomic, ngay trước khi Dirichlet năm 1846 ([4], vol. I, p. 640) chứng minh định lý tổng quát mà Hermite đã gần đạt tới một cách độc lập ([8], vol. I, p. 159). Câu hỏi (trung tâm của toàn bộ lý thuyết) về sự phân tích thành các thừa số nguyên tố dường như khó khăn hơn nhiều. Vì Lagrange đã đưa ra các ví dụ về các số có dạng $x^2 + D y^2$ (x, y, D là các số nguyên) với các ước không có dạng $m^2 + D n^2$ ([2], vol. II, p. 465), nên người ta thực sự đã biết rằng nói chung không thể mong đợi vành $\mathbf{Z}[\sqrt{-D}]$ là một miền iđêan chính và sự táo bạo của Euler đã được tiếp nối bởi sự thận trọng đáng kể; khi Dirichlet, chẳng hạn, chứng minh rằng quan hệ $p^2 - 5 q^2 = r^5$ ($p, q, r$ là các số nguyên) tương đương với

$$
p + q \sqrt{5} = (x + y \sqrt{5})^5
$$

với các số nguyên x, y, ông chỉ hạn chế ở việc chỉ ra rằng "có những định lý tương tự cho nhiều số nguyên tố khác [ngoài 5]" ([4], vol. I, p. 31). Trong hồi ký của Gauss năm 1831 và công trình của Eisenstein về các thặng dư bậc ba [6a], đúng là có những nghiên cứu nâng cao về số học trong các miền iđêan chính $\mathbf{Z}[i]$ và $\mathbf{Z}[\rho]$ ($\rho = (-1 + i \sqrt{3})/2$, một nghiệm bậc ba của đơn vị) hoàn toàn tương tự với lý thuyết các số nguyên hữu tỉ và trong các ví dụ này ít nhất mối liên hệ chặt chẽ giữa số học trong các trường bậc hai và lý thuyết các dạng toàn phương nhị phân được Gauss phát triển là rất rõ ràng; nhưng trường hợp tổng quát thiếu một "từ điển" cho phép xử lý các trường bậc hai bằng một phép dịch đơn giản từ lý thuyết của Gauss (†).

Thực tế, không phải đối với các trường bậc hai mà đối với các trường cyclotomic (và vì những lý do chỉ xuất hiện rõ ràng rất lâu sau đó (cf. p. 585)) mà bài toán được

(*) Nghiên cứu của Gauss về phép chia trên đường lemniscate và các hàm elliptic liên quan đến đường cong này, không được công bố trong thời gian ông còn sống, nhưng có niên đại khoảng năm 1800, hẳn đã dẫn ông từ thời điểm này đến việc xét các tính chất số học của vành $\mathbf{Z}[i]$, phép chia bởi các số trong vành này đóng một vai trò quan trọng trong lý thuyết; xem Jacobi nói gì về chủ đề này ([5], vol. VI, p. 275) và cũng các tính toán liên quan đến những câu hỏi này được tìm thấy trong các bài viết của Gauss ([3], vol. II, p. 411; xem thêm [3], vol. X_2, p. 33 et seq.).

† Người đọc sẽ tìm thấy một mô tả khớp về sự tương ứng này giữa các dạng toàn phương và các trường bậc hai trong Sommer, loc. cit., pp. 205–229.

giải quyết đầu tiên. Từ năm 1837 trở đi, Kummer, vốn ban đầu là một nhà giải tích, chuyển sang số học của các trường cyclotomic, lĩnh vực sẽ chiếm gần như toàn bộ thời gian của ông trong 25 năm. Giống như những người đi trước, ông nghiên cứu tính chia hết trong vành $\mathbf{Z}[\zeta]$, trong đó $\zeta$ là một nghiệm bậc $p$ của đơn vị $\neq 1$ ($p$ là một số nguyên tố lẻ); ông nhanh chóng thấy rằng ở đây cũng gặp phải những vành không phải là các miền iđêan chính, cản trở mọi tiến bộ trong việc mở rộng các định luật số học [7a] và chỉ đến năm 1845, sau 8 năm nỗ lực, ánh sáng mới xuất hiện, nhờ định nghĩa của ông về "các số iđêan" ([7c] và [7d]).

Điều mà Kummer thực hiện, xét trong ngôn ngữ hiện đại, chính là định nghĩa các định giá trên trường $\mathbf{Q}(\zeta)$: chúng tương ứng một-một với các "số nguyên tố iđêan" của ông, "số mũ" mà một nhân tử như vậy xuất hiện trong sự "phân tích" của một số $x \in \mathbf{Z}[\zeta]$ chính là giá trị tại $x$ của định giá tương ứng. Vì các liên hợp của $x$ cũng thuộc $\mathbf{Z}[\zeta]$ và tích của chúng $N(x)$ (chuẩn của $x (*)$) là một số nguyên hữu tỉ, nên các "nhân tử nguyên tố iđêan" cần được định nghĩa cũng phải là các "nhân tử" của các số nguyên tố hữu tỉ và để định nghĩa chúng chỉ cần nói các "ước nguyên tố iđêan" của một số nguyên tố $q \in \mathbf{Z}$ là gì. Với $q = p$ Kummer đã thực sự chứng minh [7a] rằng iđêan chính $(1 - \zeta)$ là nguyên tố và lũy thừa thứ $(p - 1)$ của nó là iđêan chính $(p)$; do đó trường hợp này không đặt ra bài toán mới nào. Với $q \neq p$ ý tưởng dường như đã dẫn dắt Kummer là thay thế phương trình cyclotomic $\Phi_p(z) = 0$ bằng đồng dư thức $\Phi_p(u) \equiv 0 \pmod{q}$, nói cách khác là phân tích đa thức cyclotomic $\Phi_p(X)$ trên trường $\mathbf{F}_q$ và gắn với mỗi nhân tử bất khả quy của đa thức này một "nhân tử nguyên tố iđêan". Một trường hợp đơn giản (được nêu tường minh trong Chú ý [7b], nơi Kummer công bố các kết quả của mình mà không có chứng minh) là trường hợp $q \equiv 1 \pmod{p}$; nếu $q = mp + 1$ và $y \in \mathbf{F}_q$ là một nghiệm nguyên thủy bậc $(q - 1)$ của 1, thì, trong $\mathbf{F}_q[X]$,
$$
\Phi_p(X) = \prod_{k=1}^{q-1} (X - \gamma^{km})
$$

(*) Khái niệm chuẩn của một số đại số bắt nguồn từ Lagrange: nếu $\alpha_i$ ($1 \leq i \leq n$) là các nghiệm của một đa thức bậc $n$, ông thậm chí còn xét "dạng chuẩn" $N(x_0, x_1, \ldots, x_{n-1}) = \prod_{i=1}^n (x_0 + \alpha_i x_1 + \cdots + \alpha_i^{n-1} x_{n-1})$ theo các biến $x_i$

điều này không nghi ngờ gì đã được gợi ý cho ông bởi nghiên cứu của ông về nghiệm của các phương trình và "các giải thức Lagrange" ([2], tập VII, p. 170). Cần chú ý rằng chính tính chất nhân của chuẩn đã dẫn Lagrange đến đồng nhất thức của ông về các dạng toàn phương nhị phân, do đó Gauss đã có thể thu được sự "hợp thành" của các dạng này ([2], tập II, p. 522). Mặt khác, khi lý thuyết các số đại số ra đời vào khoảng năm 1830, nó rất thường xuất hiện dưới dạng nghiệm của các phương trình $N(x_0, \ldots, x_{n-1}) = \lambda$ (đặc biệt với $\lambda = 1$ trong nghiên cứu về các đơn vị) hoặc sự nghiên cứu các "dạng chuẩn" (còn gọi là "dạng phân tích được") mà các bài toán được trình bày; và ngay cả trong các công trình gần đây, các tính chất của những phương trình Diophant riêng biệt này được sử dụng một cách có hiệu quả, đáng chú ý trong lý thuyết các số p-adic (Skolem, Chabauty).

vì $\gamma^{pm} = 1$. Khi đó, gắn với mỗi nhân tử $X - \gamma^{km}$ một "nhân tử nguyên tố iđêan" $q_k$ của $q$, Kummer nói rằng một phần tử $x \in \mathbf{Z}[\zeta]$, mà P là đa thức tối tiểu trên $\mathbf{Q}$ của nó, chia hết cho $q_k$ nếu trong $\mathbf{F}_q$, $P(\gamma^{km}) = 0$; tóm lại, trong ngôn ngữ hiện đại, ông viết vành thương $\mathbf{Z}[\zeta]/q\mathbf{Z}[\zeta]$ như một hợp thành trực tiếp của các trường đẳng cấu với $\mathbf{F}_r$. Với $q \not\equiv 1 \pmod{p}$, các nhân tử bất khả quy của $\Phi_p(X)$ trong $\mathbf{F}_q[X]$ không còn là bậc nhất nữa và do đó cần phải thay thế X trong $P(X)$ bằng các nghiệm "ảo Galois" của các nhân tử của $\Phi_p$ trong $\mathbf{F}_q[X]$. Kummer tránh khó khăn này bằng cách chuyển qua, như ngày nay ta sẽ nói, đến trường phân tích của $q$; nếu f là số nguyên cực tiểu sao cho $q^f \equiv 1 \pmod{p}$ và $p - 1 = ef$, K chính là trường con của $\mathbf{Q}(\zeta)$ gồm các phần tử bất biến của nhóm con cấp f của nhóm Galois (xyclic cấp $p - 1$) của $\mathbf{Q}(\zeta)$ trên $\mathbf{Q}$; nói cách khác nó là trường con duy nhất của $\mathbf{Q}(\zeta)$ có bậc e trên $\mathbf{Q}$; nó đã được biết rõ từ Disquisitiones của Gauss, vì được sinh bởi các "chu kỳ"

$$
\eta_k = \zeta_k + \zeta_{k+f} + \zeta_{k+2f} + \cdots + \zeta_{k+(e-1)f}
$$

$(0 \leq k \leq e-1, \zeta_v = \zeta^{g^v}$ trong đó g là một nghiệm nguyên thủy của đồng dư $z^{p-1} \equiv 1 \pmod{p}$), tạo thành một cơ sở chuẩn đối với nó. Nếu $R(X)$ là đa thức tối tiểu (monic và có các hệ số nguyên hữu tỉ) của bất kỳ "chu kỳ" nào trong số các chu kỳ này $\eta$, Kummer, bắt đầu từ các công thức của Gauss, chứng minh rằng, trên trường $\mathbf{F}_r$, $R(X)$ cũng phân tích thành các nhân tử phân biệt bậc nhất $X - u_j$ ($1 \leq j \leq e$) và chính với mỗi $u_j$ mà ông gán một "nhân tử nguyên tố iđêan" $q_j$. Để định nghĩa "tính chia hết cho $q_j$", Kummer viết mọi $x \in \mathbf{Z}[\zeta]$ dưới dạng $x = \sum_{k=0}^{f-1} \gamma^k y_k$, trong đó mỗi $y_k \in K$ lại có thể được viết duy nhất như một đa thức bậc $\leq e - 1$ theo $\eta$ với các hệ số nguyên hữu tỉ; ông nói rằng $x$ chia hết cho $q_j$ khi và chỉ khi, khi thay $u_j$ cho $\eta$ trong mỗi $y_k$, các phần tử của F thu được đều bằng không. Nhưng cũng cần phải định nghĩa "số mũ" của $q_j$ trong $x$. Vì điều này, Kummer đưa vào cái mà ngày nay ta gọi là một phần tử chuẩn hóa đối với $q_j$, tức là một phần tử $\rho_j \in K$ sao cho $N(\rho_j) \equiv 0 \pmod{q}$, $N(\rho_j) \not\equiv 0 \pmod{q^2}$ và cuối cùng sao cho $\rho_j$ chia hết cho $q_j$ (theo nghĩa đã định nghĩa ở trên) nhưng không chia hết cho bất kỳ nhân tố iđêan nào khác $\neq q$, của $q$. Sự tồn tại của một $\rho_j$ như vậy thực sự đã được Kronecker chứng minh trong luận án của ông vào năm trước đó ([9a], p. 23); sau đó viết $\rho = N(\rho_j)/\rho_j$, Kummer nói rằng số mũ của $q_j$ trong $x$ bằng h nếu $x\rho_j^h \equiv 0 \pmod{q^h}$ nhưng $x\rho_j^{h+1} \not\equiv 0 \pmod{q^{h+1}}$; dĩ nhiên ông bắt đầu bằng việc chứng minh rằng quan hệ $x\rho_j' \equiv 0 \pmod{q}$ tương đương với việc $x$ chia hết cho $q_j$ (theo nghĩa trên). Một khi các định nghĩa này được thiết lập, việc mở rộng sang $\mathbf{Z}[\zeta]$ các quy luật chia hết thông thường đối với "các số iđêan" không còn gây ra khó khăn nghiêm trọng nữa; và ngay từ hồi ký đầu tiên của mình [7c] Kummer thậm chí có thể, sử dụng "phương pháp hộp" của Dirichlet, chỉ ra rằng "các lớp" và "các nhân tố iđêan" là hữu hạn về số lượng (*).

(*) Ông không làm gì hơn ngoài việc tái hiện một lập luận của Kronecker trong luận án-

Chúng ta sẽ không theo đuổi lịch sử các công trình sau này của Kummer về các trường cyclotomic, liên quan đến việc xác định số lớp và việc áp dụng vào chứng minh định lý Fermat trong một số trường hợp. Chúng ta chỉ nhắc đến cách thức mà, vào năm 1859, ông mở rộng phương pháp của mình để thu được (ít nhất là một phần) các “số nguyên tố iđêan” trong một “trường Kummer” $\mathbf{Q}(\zeta, \mu)$, trong đó $\mu$ là một nghiệm của đa thức bất khả quy $P(X) = X^p - \alpha$, trong đó $\alpha \in \mathbf{Z}[\zeta]$ [7e]. Điều thú vị là Kummer xem xét bài toán chính xác bằng cách coi $\mathbf{Q}(<+)$ như một mở rộng cyclic của trường $\mathbf{Q}(\zeta)$ được lấy làm “trường cơ sở” (†): ông bắt đầu với một “số nguyên tố iđêan” $q$ của $\mathbf{Z}[\zeta]$ mà ông giả sử không chia hết cho $p$ cũng không chia hết cho $\alpha$ và lần này ông khảo sát (theo thuật ngữ hiện đại) đa thức $\overline{P}(X) = X^p - \bar{\alpha}$ trong trường thặng dư $k$ của định giá trên $\mathbf{Q}(\zeta)$ tương ứng với $q$ ($\bar{\alpha}$ là ảnh chính tắc của $a$ trong $k$). Vì $\mathbf{Q}(\zeta)$ là trường của các nghiệm bậc $p$ của đơn vị, $\overline{P}$ hoặc là bất khả quy trên $k$, hoặc là tích của các nhân tử bậc nhất. Trong trường hợp thứ nhất, Kummer nói rằng $q$ vẫn là nguyên tố trong $\mathbf{Z}[\zeta, \mu]$; trong trường hợp thứ hai, ông đưa vào các phần tử $w_i$ ($1 \leq i \leq p$) của $\mathbf{Z}[\zeta]$ mà ảnh của chúng trong $k$ là các nghiệm của $\overline{P}$ và ông liên kết với mỗi chỉ số $i$ một nhân tử nguyên tố iđêan $r_i$ của $q$; rồi viết $W_i(X) = \prod_{j \neq i} (X - w_j)$, ông nói rằng, đối với một đa thức $f$ với các hệ số trong $\mathbf{Z}[\zeta], f(\mu)$ chứa nhân tử $r_i$ $m$ lần nếu
$$
f(w_i) W_i^m(w_i) \equiv 0 \pmod{q^m}
$$
nhưng
$$
f(w_i) W_i^{m+1}(w_i) \not\equiv 0 \pmod{q^{m+1}}.
$$
Tóm lại, bằng cách này ông thu được các định giá trên $\mathbf{Q}(\zeta, \mu)$ không phân nhánh trên $\mathbf{Q}$, đủ cho các áp dụng mà ông hướng tới.

\*   \*   \*

Kummer đã có dịp gặp phải, trong khi nghiên cứu các trường riêng biệt mà nghiên cứu của ông về Định lý Fermat ban đầu đã dẫn tới, một số hoàn cảnh ngẫu nhiên khiến việc nghiên cứu chúng trở nên dễ tiếp cận hơn nhiều. Sự mở rộng đến tation, liên quan đến các lớp nghiệm của các phương trình có dạng
$$
N(x_0, x_1, \ldots, x_{n-1}) = a
$$
([9a], p. 25). Mặt khác, Kummer đưa ra nhiều ám chỉ đến các kết quả thu được bởi Dirichlet về các phương trình loại này (đối với mọi trường số đại số); nhưng các kết quả này chưa từng được công bố cũng như không được tìm thấy trong các giấy tờ của Dirichlet.

(†) Trong hồi ký của mình về các dạng bậc hai với các hệ số trong vành các số nguyên Gauss ([4], vol. I, pp. 533–618), Dirichlet ở nhiều chỗ đã được dẫn dắt đến việc xét chuẩn tương đối của trường $\mathbf{Q}(\sqrt{D}, i)$ trên trường con bậc hai của nó $\mathbf{Q}(\sqrt{D})$. Tương tự, Eisenstein, khi nghiên cứu các nghiệm bậc 8 của đơn vị, xét trường do chúng sinh ra như một mở rộng bậc hai của $\mathbf{Q}(i)$ và sử dụng chuẩn tương đối với trường con này ([&], p. 253). Nhưng công trình của Kummer là ví dụ đầu tiên về một nghiên cứu số học sâu sắc của một “trường tương đối”.

Trường hợp tổng quát của các kết quả của Kummer đã đặt ra những khó khăn đáng kể và cần nhiều năm nỗ lực để giải quyết.

Với Kronecker và Dedekind, những người giữ vai trò chính ở đây, lịch sử của lý thuyết các số đại số, trong 40 năm sau phát hiện của Kummer, không khác mấy (nhưng may mắn là không có cùng sự cay đắng) với lịch sử sự cạnh tranh giữa Newton và Leibniz 180 năm trước đó về việc phát minh ra phép tính vô cùng bé. Là học trò và sau này là đồng nghiệp của Kummer ở Berlin, Kronecker (người mà luận án, như chúng ta đã thấy, đã đóng vai trò một điểm cốt yếu trong lý thuyết của Kummer) rất quan tâm đến các “số iđêan” nhằm áp dụng chúng vào các nghiên cứu riêng của mình; và chúng ta khâm phục sự thấu suốt đáng kinh ngạc của ông khi thấy ông, ngay từ năm 1853 ([9b], p. 10), công bố định lý tổng quát về cấu trúc của các mở rộng Abel của $\mathbf{Q}$ và, điều có lẽ còn đáng chú ý hơn nữa, tạo ra trong những năm tiếp theo lý thuyết nhân phức và phát hiện mầm đầu tiên của lý thuyết trường lớp ([9c] và [9d]). Một lá thư của Kronecker gửi Dirichlet năm 1857 ([9], vol. 5, pp. 418–421) cho thấy rằng vào thời điểm đó ông đã sở hữu một phép tổng quát hóa lý thuyết của Kummer, điều mà hơn nữa chính Kummer xác nhận trong một trong các công trình của mình ([7e], p. 57) và Kronecker sẽ nhiều lần ám chỉ đến lý thuyết này trong các hồi ký của ông từ năm 1860 đến 1880 (*).

Nhưng mặc dù vào thời điểm đó không một nhà toán học nào của trường phái Đức về Lý thuyết Số không biết đến sự tồn tại của các công trình này của Kronecker, dường như ông chỉ truyền đạt các nguyên lý của các phương pháp của mình cho một nhóm hạn chế các bạn bè và học trò, và khi cuối cùng ông quyết định công bố chúng trong hồi ký năm 1881 của mình về biệt thức [9e] và trên hết trong “Festschrift” lớn năm 1882 [9f], Dedekind không thể không bày tỏ sự ngạc nhiên của mình ([10], vol. III, p. 427), vì đã tưởng tượng rằng các quá trình hoàn toàn khác, từ những tiếng vọng mà ông đã nghe thấy ([10], vol. III, p. 287). Hơn nữa, Kronecker còn lâu mới sở hữu ở cùng mức độ những tài năng trình bày và sự sáng sủa đáng chú ý của Dedekind, và do đó không có gì đáng ngạc nhiên khi chính các phương pháp của người sau, đã được công bố từ năm 1871, đã tạo thành khuôn khổ của lý thuyết các số đại số; dù thú vị đến đâu, phương pháp “phép nối các bất định” của Kronecker, xét về Lý thuyết Số, trong mắt chúng ta hầu như không hơn một biến thể của phương pháp của Dedekind (xem Chương VII, § 1, Bài tập 31), và chính chủ yếu theo một hướng khác, hướng về Hình học Đại số, mà các ý tưởng của Kronecker đạt được toàn bộ tầm quan trọng của chúng đối với lịch sử của Đại số giao hoán, như chúng ta sẽ thấy sau này.

Vì những lý do chỉ có thể được nhìn nhận rõ ràng hơn nhiều về sau, bước chuẩn bị đầu tiên dĩ nhiên đối với mọi nỗ lực xây dựng một lý thuyết tổng quát là làm sáng tỏ khái niệm số nguyên đại số. Điều này đạt được vào khoảng 1845–50, mặc dù rất khó

(*) Về sự tiến triển các ý tưởng của ông về chủ đề này, xem phần mở đầu rất thú vị cho hồi ký của ông năm 1881 về biệt thức ([9e], p. 195).

để xác định chính xác thời điểm nó xuất hiện; có vẻ có khả năng rằng chính ý tưởng về một hệ ổn định đối với phép cộng và phép nhân (hay, chính xác hơn, cái mà ngày nay ta gọi là một Z-đại số có hạng hữu hạn) đã, một cách ít nhiều có ý thức, dẫn đến định nghĩa tổng quát về các số nguyên đại số: thực vậy định nghĩa này tất yếu xuất hiện khi một Z-đại số có dạng $\mathbf{Z}[\theta]$ được hạn chế là có hạng hữu hạn, bằng phép loại suy với vành $\mathbf{Z}[\zeta]$ sinh bởi một nghiệm đơn vị, vốn luôn ở trung tâm các mối quan tâm của các nhà số học vào thời điểm này. Dù sao đi nữa, khi, một cách độc lập, Dirichlet ([4], vol. I, p. 640), Hermite ([8], vol. I, pp. 115 and 146) và Eisenstein ([6c], p. 236) đưa vào khái niệm số nguyên đại số, họ dường như không xem rằng mình đang xử lý một khái niệm mới cũng như không đánh giá rằng việc nghiên cứu chi tiết nó sẽ hữu ích; chỉ có Eisenstein chứng minh một cách thực sự (*loc. cit.*) rằng tổng và tích của hai số nguyên đại số là các số nguyên đại số, hơn nữa không khẳng định rằng kết quả này là nguyên bản.

Một điểm tinh tế hơn nhiều là việc xác định các vành trong đó có thể chờ đợi một phép tổng quát hóa lý thuyết của Kummer. Người sau, trong chú ý đầu tiên của mình [7b], không ngần ngại khẳng định rằng ông có thể thu được lại bằng phương pháp của mình lý thuyết của Gauss về các dạng toàn phương nhị phân bằng cách xét các vành $\mathbf{Z}[\sqrt{D}]$ (D là một số nguyên); ông không bao giờ phát triển ý tưởng này, nhưng chắc chắn có vẻ như cả ông lẫn bất kỳ ai khác trước Dedekind đều không nhận thấy rằng phép hợp thành duy nhất thành các nhân tử nguyên tố “iđêan” là không thể trong vành $\mathbf{Z}[\sqrt{D}]$ khi $D \equiv 1 \pmod{4}$ (mặc dù ví dụ về các nghiệm bậc ba của đơn vị cho thấy rằng vành $\mathbf{Z}[\rho]$ được xét từ thời Gauss là phân biệt với $\mathbf{Z}[\sqrt{-3}]$) (*). Trước Dedekind và Kronecker, các vành duy nhất được nghiên cứu luôn có kiểu $\mathbf{Z}[\theta]$ hoặc đôi khi là một số vành riêng biệt có kiểu $\mathbf{Z}[\theta, \theta']$ (†). Đối với Kronecker, có thể ý tưởng xét *tất cả* các số nguyên của một mở rộng đại số lần đầu tiên được gợi ý cho ông bởi việc nghiên cứu trường các hàm đại số, nơi vành này xuất hiện một cách tự nhiên như tập hợp các hàm “hữu hạn tại vô cực”; trong mọi trường hợp ông nhấn mạnh trong hồi ký của mình năm 1881 về biệt thức (được viết và công bố tại Viện Hàn lâm Berlin ngay từ năm 1862) đặc trưng hóa này của các “số nguyên” trong các trường đó [9e]. Dedekind không đưa ra chỉ dẫn nào về nguồn gốc các ý tưởng riêng của ông về điểm này, nhưng trong công bố đầu tiên của ông về các trường số năm 1871, vành của tất cả các số nguyên của một trường như vậy đóng một vai trò then chốt trong lý thuyết của ông; cũng chính Dedekind làm sáng tỏ quan hệ giữa một vành như vậy và các vành con của nó có cùng trường phân thức, bằng việc đưa vào khái niệm *vật dẫn* [10c].

(*) Mặc dù Kronecker hẳn đã được dẫn dắt đến việc nghiên cứu số học của các vành $\mathbf{Z}[\sqrt{-D}]$ ($D > 0$) bởi công trình của ông về phép nhân phức, ông không công bố gì về chủ đề này và đặc trưng hóa các số nguyên của bất kỳ trường bậc hai nào $\mathbf{Q}(\sqrt{D})$ lần đầu tiên được đưa ra tường minh bởi Dedekind năm 1871 ([10c], pp. 105–106).

(†) Trước đây chúng ta đã thấy ví dụ về vành $\mathbf{Z}[\zeta, \mu]$ được đưa vào bởi Kummer [7e]. Trước đó, Eisenstein đã được dẫn dắt đến việc xét một vành con được sinh bởi hai phần tử của vành các số nguyên trong trường của các nghiệm bậc 21 của đơn vị [6b].

Nhưng đây không phải là khó khăn duy nhất. Để tổng quát hóa các ý tưởng của Kummer, trước hết cần phải loại bỏ việc chuyển qua trường phân tích, vốn dĩ tự nhiên không thể có tương tự trong trường hợp một trường không Abel. Sự đi đường vòng này hơn nữa thoạt nhìn có vẻ rất đáng ngạc nhiên và nhân tạo, vì, bắt đầu với đa thức bất khả quy $\Phi_p(X)$ của $\mathbf{Z}[X]$, người ta có thể tự hỏi tại sao Kummer không đẩy các ý tưởng của mình đến kết luận lôgic của chúng và điều gì ngăn cản ông sử dụng lý thuyết về các số "Galois tưởng tượng" vốn đã được biết rõ vào thời đó. Trở ngại này hiện ra rõ hơn trong một cố gắng tổng quát hóa không may được thực hiện ngay từ năm 1865 bởi Selling, một học trò của Dedekind: cho một đa thức bất khả quy $P \in \mathbf{Z}[X]$, Selling phân tích đa thức tương ứng $\overline{P}(X)$ thành các nhân tử bất khả quy trong $\mathbf{F}_q[X]$; các nghiệm của đa thức này do đó thuộc về một mở rộng hữu hạn $F$, của $\mathbf{F}_q$; nhưng Selling, để định nghĩa theo cách của Kummer số mũ của một "nhân tử nguyên tố iđêan" của $q$ trong một số nguyên của trường phân rã của $P(X)$, không ngần ngại nói, *trong trường* $\mathbf{F}_r$, về các đồng dư thức modulo một *lũy thừa của* $q$ ([11], p. 26); và một chút sau đó khi ông cố gắng tiếp cận vấn đề phân nhánh, ông "thêm" vào $\mathbf{F}_r$ các "nghiệm tưởng tượng" của một phương trình dạng $x^h = q$ ([11], p. 34). Rõ ràng những bước đi táo bạo này (vốn sẽ được biện minh nếu trường hữu hạn $\mathbf{F}_q$ được thay bằng trường $q$-adic) vào thời đó chỉ có thể dẫn đến điều vô nghĩa. May mắn thay, Dedekind năm 1857 [10a], dưới tên gọi "lý thuyết về các đồng dư thức cấp cao", đã nghiên cứu lại dưới một dạng khác lý thuyết về các trường hữu hạn (*): ông giải thích các phần tử của trường sau như là các "thặng dư" của các đa thức của $\mathbf{Z}[X]$ đối với một "môđun kép" gồm các tổ hợp tuyến tính với các hệ số trong $\mathbf{Z}[X]$ của một số nguyên tố $p$ và một đa thức đơn khởi bất khả quy $P \in \mathbf{Z}[X]$ (điều này chắc chắn đối với ông, cũng như đối với Kronecker, là nguồn gốc của ý tưởng tổng quát về *môđun* mà họ sẽ đi tới một cách độc lập một chút sau đó). Theo lời chứng của chính ông ([10d], p. 218), dường như Dedekind đã bắt đầu bằng cách tấn công bài toán về các "nhân tử iđêan" của $p$ trong một trường $\mathbf{Q}(\xi)$, nơi $P \in \mathbf{Z}[X]$ là đa thức tối tiểu của $\xi$, như sau (chắc chắn ít nhất trong trường hợp "không phân nhánh", nghĩa là khi đa thức $p$ trong $\mathbf{F}_p[X]$ tương ứng với $P$ không có nghiệm bội): ông viết, trong $\mathbf{Z}[X]$,

$$
P = P_1 P_2 \ldots P_h + p \cdot G
$$

trong đó các $\overline{P}_i$ là bất khả quy và phân biệt trong $\mathbf{F}_p[X]$; có thể giả sử rằng $G$ không chia hết (trong $\mathbf{Z}[X]$) cho bất kỳ $P_i$ nào và với mọi $i$ ông viết $W_i = \prod_{j \neq i} P_j$; khi đó, nếu $f \in \mathbf{Z}[X]$, người ta sẽ nói rằng $f(\xi)$ chứa "nhân tử iđêan" $p_i$ của $p$

(*) Người ta biết rằng một số kết quả của lý thuyết này, được công bố lần đầu bởi Galois, đã được Gauss thu được (dưới ngôn ngữ của các đồng dư thức) vào khoảng năm 1800; sau cái chết của Gauss, Dedekind được giao việc công bố một phần các công trình của ông và đã phát hiện lại đặc biệt trong các tài liệu Gauss để lại bản hồi ký về các trường hữu hạn ([3], tập II, tr. 212–240).

tương ứng với $P_i$ $k$ lần nếu

$$
f W_i^k \equiv 0 \pmod{p^k, P}
$$

và

$$
f W_i^{k+1} \not\equiv 0 \pmod{p^{k+1}, P}.
$$

Mối liên hệ với phương pháp được Kummer sử dụng cho các "trường Kummer" ở đây là hiển nhiên và định nghĩa ban đầu của Kummer cho các trường cyclotomic có thể, bằng cách này, dễ dàng được khôi phục (xem chẳng hạn công trình của Zolotareff [14], người ban đầu độc lập với Dedekind, đã phát triển các ý tưởng này một chút sau đó).

Tuy nhiên, cả Dedekind lẫn Kronecker, người dường như cũng đã thực hiện các cố gắng tương tự, đều không thể tiến xa hơn theo hướng này, cả hai đều bị chặn lại bởi những khó khăn do sự phân nhánh gây ra ([10d], p. 218 và [9f], p. 325) (*). Nếu vành các số nguyên $\mathbf{A}$ của trường số $K$ đang xét thừa nhận một cơ sở (trên $\mathbf{Z}$) gồm các lũy thừa của cùng một số nguyên $\theta$, thì không khó để tổng quát hóa phương pháp trên cho các số nguyên tố phân nhánh trong $\mathbf{Z}[\theta]$ (như Zolotareff chỉ ra *loc. cit.*)). Nhưng có những trường $K$ trong đó không tồn tại cơ sở kiểu này trong vành $\mathbf{A}$; và Dedekind cuối cùng còn phát hiện rằng có những trường hợp trong đó một số số nguyên tố $p$ (các "nhân tử bất thường của biệt thức" của trường $K$) là sao cho, *đối với mọi* $0 \in \mathbf{A}$, áp dụng phương pháp trên cho đa thức tối tiểu của $0$ trên $\mathbf{Q}$ dẫn đến việc gán các nhân tử iđêan bội cao nhất trong khi thực tế $p$ không phân nhánh trong $\mathbf{A}$ ($\dagger$); ông thừa nhận rằng mình đã bị cản trở trong một thời gian dài bởi khó khăn không lường trước này, trước khi vượt qua được nó bằng việc tạo ra từ đầu lý thuyết về các môđun và iđêan, trong một sự trình bày bậc thầy (và đã hoàn toàn theo phong cách hiện đại, trái ngược với phong cách dài dòng của những người cùng thời với ông) trong tác phẩm chắc chắn là kiệt tác của ông, "phần bù thứ 11" nổi tiếng cho cuốn sách Lý thuyết về Số của Dirichlet [10f]. Công trình này trải qua ba phiên bản liên tiếp, nhưng ngay từ phiên bản đầu tiên (được xuất bản như "phần bù thứ 10" cho lần xuất bản thứ hai của cuốn sách của Dirichlet năm 1871 [4 bis]) những điều cốt yếu của phương pháp đã có mặt và gần như chỉ trong một bước lý thuyết về các số đại số chuyển từ những phác thảo và những dò dẫm trước đó sang một ngành khoa học hoàn toàn trưởng thành đã sở hữu các công cụ cốt yếu của nó: ngay từ đầu, vành của tất cả các số nguyên của một trường số được đặt ở trung tâm của lý thuyết; Dedekind chứng minh sự tồn tại của một cơ sở của vành này trên $\mathbf{Z}$ và

(*) Zolotareff vượt qua khó khăn bằng một sự tinh chỉnh phương pháp của mình, điều này dường như chỉ có giá trị không đáng kể ngoài phương diện giai thoại [14].

($\dagger$) Kronecker tuyên bố đã bắt gặp cùng hiện tượng đó trong một trường con của trường các căn bậc 13 của đơn vị mà ông không mô tả chính xác hơn ([9f], p. 384). Ví dụ về một nhân tử bất thường của định thức được Dedekind đưa ra được trình bày chi tiết trong Hasse, Zahlentheorie (Berlin, Akad. Verlag, 1949), p. 333; ít lâu sau, Hasse đưa ra một ví dụ về một trường $K$ trong đó không có nhân tử bất thường của định thức, nhưng không tồn tại $\theta \in \mathbf{A}$ sao cho $\mathbf{A} = \mathbf{Z}[\theta]$ (*loc. cit.*, p. 335).

từ đó suy ra định nghĩa định thức của trường là bình phương của định thức tạo bởi các phần tử của một cơ sở của vành các số nguyên và các phần tử liên hợp của chúng; tuy nhiên, trong phần bổ sung thứ 11, ông chỉ đưa ra đặc trưng hóa các số nguyên tố phân nhánh (như các nhân tử nguyên tố của định thức) đối với các trường bậc hai ([10f], p. 202), trong khi từ năm 1871 trở đi ông đã nắm được định lý tổng quát (*). Kết quả trung tâm của công trình là định lý tồn tại và duy nhất về phân tích các iđêan thành các nhân tử nguyên tố, mà để có được nó Dedekind bắt đầu bằng cách xây dựng một lý thuyết sơ cấp về “môđun”; thực ra, trong phần bổ sung thứ 11, ông dành tên gọi này cho các môđun con của một trường số, nhưng quan niệm mà ông hình thành về chúng và các kết quả ông chứng minh đã được trình bày theo một cách có thể áp dụng ngay lập tức cho các môđun tổng quát (†); trong số những điều khác, cần ghi nhận, ngay từ năm 1871, việc đưa vào khái niệm “transporter”, đóng vai trò quan trọng (cũng như “điều kiện dãy tăng”) trong chứng minh đầu tiên của định lý phân tích nhân tử duy nhất. Trong hai lần xuất bản tiếp theo, Dedekind cũng đưa ra hai chứng minh khác của định lý này mà ông có lý khi coi là nền tảng của lý thuyết mình. Cần lưu ý ở đây rằng chính trong chứng minh thứ ba, các iđêan phân số được sử dụng (đã được Kummer đưa vào từ năm 1859 đối với các trường cyclotomic) và tính chất chúng tạo thành một nhóm được thiết lập; sau này chúng ta sẽ trở lại với chứng minh thứ hai (p. 594).

Tất cả các kết quả này (ngoại trừ thuật ngữ) hẳn đã được Kronecker biết đến từ khoảng năm 1860 dưới dạng các trường hợp riêng của những quan niệm tổng quát hơn của ông mà chúng ta sẽ nói đến sau (trong khi Dedekind thừa nhận rằng ông chỉ vượt qua được những khó khăn cuối cùng của lý thuyết của mình vào năm 1869–70 ([10e], p. 351)) (‡); đối với các trường số, đặc biệt cần nhấn mạnh rằng, ngay từ thời điểm này, Kronecker đã biết toàn bộ lý thuyết có thể áp dụng mà không cần thay đổi cốt yếu, bắt đầu từ một “trường cơ sở” k vốn tự nó là một trường số (khác $\mathbf{Q}$), một quan điểm mà lý thuyết về phép nhân phức dẫn đến một cách tự nhiên; do đó ông đã nhận ra, đối với một số trường k, sự tồn tại của các mở rộng đại số $K \neq k$ không phân nhánh trên k ([9f], p. 269), một sự kiện không thể xảy ra với $k = \mathbf{Q}$ (như suy ra từ các đánh giá dưới của Hermite và Minkowski đối với định thức). Dedekind không bao giờ phát triển quan điểm cuối cùng này (mặc dù ông chỉ ra khả năng của nó trong hồi ký năm 1882 về biệt thức) và công trình trình bày có hệ thống đầu tiên về lý thuyết “trường tương đối” là của Hilbert [16d].

(*) Ông chỉ đưa ra chứng minh của định lý này trong hồi ký năm 1882 về biệt thức [10e].
(†) Trong hồi ký năm 1882 về các đường cong đại số (cùng với H. Weber) [10 bis], ông sử dụng lý thuyết các môđun trên vành $\mathbf{C}[X]$ theo cùng một cách.
(‡) Tuy nhiên, Kronecker đã không thành công trong việc dùng các phương pháp của mình để đạt được đặc trưng hóa đầy đủ các iđêan phân nhánh trong trường hợp các trường số. Mặt khác, ông có được đặc trưng hóa này đối với các trường các hàm đại số của một biến và hơn nữa chứng minh rằng trong trường hợp này không có “nhân tử bất thường” của định thức [9e].

Cuối cùng, vào năm 1882 [10e], Dedekind hoàn thiện lý thuyết bằng cách đưa vào biệt thức, qua đó ông có một định nghĩa mới về định thức và cho phép ông xác định chính xác các số mũ của các nhân tử iđêan nguyên tố trong phân tích của nó. Cũng vào khoảng thời gian này, ông bắt đầu quan tâm đến những đặc điểm riêng biệt của các mở rộng Galois, đưa vào các khái niệm nhóm phân tích và nhóm quán tính (trong hồi ký [10g] của ông, chỉ được xuất bản năm 1894) và thậm chí (trong các công trình không được xuất bản khi ông còn sống ([10], vol. 11, pp. 410–411)) một phác thảo về các nhóm phân nhánh, mà Hilbert (độc lập với Dedekind) sẽ phát triển ít lâu sau ([16c] và [16d]).

Như vậy, vào khoảng năm 1895, lý thuyết các số đại số đã hoàn thành giai đoạn đầu tiên của quá trình phát triển; những công cụ được rèn giũa trong thời kỳ hình thành này sẽ cho phép nó gần như ngay lập tức bước vào giai đoạn tiếp theo, lý thuyết trường lớp tổng quát (hay, điều tương đương, lý thuyết các mở rộng Abel của các trường số), tiếp tục cho đến thời đại chúng ta và chúng ta sẽ không trình bày ở đây. Từ quan điểm của Đại số giao hoán, có thể nói rằng đồng thời lịch sử của các miền Dedekind về cơ bản đã hoàn tất, nếu không xét đặc trưng hóa tiên đề của chúng, cũng như cấu trúc của các môđun sinh hữu hạn trên các miền này (mà trong trường hợp các trường số, chỉ được Steinitz làm sáng tỏ đáng kể vào năm 1912 [20b]) (*).

\*   \*   \*

Những tiến triển sau này của Đại số giao hoán chủ yếu nảy sinh từ những vấn đề hoàn toàn khác, xuất phát từ Hình học đại số (môn này hơn nữa sẽ ảnh hưởng trực tiếp đến Lý thuyết số ngay cả trước những phát triển “trừu tượng” của thời kỳ hiện tại).

Chúng ta sẽ không xét ở đây lịch sử chi tiết của Hình học Đại số, lĩnh vực mà cho đến cái chết của Riemann hầu như không chạm đến chủ đề của chúng ta. Chỉ cần nhắc lại rằng nó chủ yếu quan tâm đến việc nghiên cứu các đường cong đại số trong mặt phẳng xạ ảnh phức, thường được tiếp cận bằng các phương pháp hình học xạ ảnh (có hoặc không sử dụng tọa độ). Có một sự phát triển song song, với Abel, Jacobi, Weierstrass và Riemann, của lý thuyết về các "hàm đại số" của một biến phức và các tích phân của chúng; các nhà toán học hiển nhiên ý thức được mối liên hệ giữa lý thuyết này và hình học của các đường cong đại số phẳng, và thậm chí đôi khi còn được biết đến là đã "áp dụng Giải tích vào Hình học"; nhưng các phương pháp được dùng để nghiên cứu các hàm đại số chủ yếu có bản chất "siêu việt", ngay cả trước Riemann (†); đặc trưng này còn được nhấn mạnh hơn nữa trong công trình của ông sau này,

(*) Việc nghiên cứu môđun trên một vành của các số đại số đã được Dedekind bắt đầu trước đó [10h].

(†) Tuy nhiên cần lưu ý rằng Weierstrass, trong nghiên cứu của ông về các hàm Abel (bắt đầu từ năm 1857 nhưng chỉ được trình bày trong các bài giảng của ông khoảng năm 1865 và chỉ được xuất bản trong Toàn tập của ông ([17], tập IV)), đưa ra, trái với việc đưa vào các "mặt Riemann" và các hàm giải tích tùy ý được định nghĩa trên một mặt như vậy. Ngay lập tức sau cái chết của Riemann, Roch và trên hết là Clebsch đã nhận ra khả năng thu được từ những kết quả sâu sắc đạt được bằng các phương pháp siêu việt của Riemann nhiều ứng dụng đáng chú ý vào hình học xạ ảnh của các đường cong, điều dĩ nhiên đã thúc đẩy các nhà hình học đương thời đưa ra các chứng minh thuần túy "hình học" cho các kết quả này; chương trình này, được Clebsch và Gordan thực hiện chưa đầy đủ, đã được Brill và M. Noether hoàn thành vài năm sau đó [13], nhờ việc nghiên cứu các hệ điểm biến thiên trên một đường cong đã cho và các đường cong phụ trợ ("đường cong phụ") đi qua các hệ điểm như vậy. Nhưng ngay cả đối với những người cùng thời với ông, các phương pháp siêu việt của Riemann (và đặc biệt là việc ông sử dụng các khái niệm tôpô và "nguyên lý Dirichlet") dường như dựa trên những nền tảng không chắc chắn; và mặc dù Brill và Noether cẩn thận hơn khá nhiều so với phần lớn các nhà hình học "tổng hợp" đương thời (xem dưới đây p. 593), các phương pháp hình học-giải tích của họ không tránh khỏi mọi sự chỉ trích. Chính yếu là nhằm đặt cho lý thuyết các đường cong đại số phẳng một cơ sở vững chắc mà Dedekind và Weber đã công bố vào năm 1882 hồi ký lớn của họ về chủ đề này [10 bis]: "Nghiên cứu được công bố dưới đây", họ nói, "nhằm đặt nền tảng cho lý thuyết về các hàm đại số của một biến, một trong những sáng tạo chính của Riemann, theo một cách đồng thời đơn giản, chặt chẽ và hoàn toàn tổng quát. Trong các nghiên cứu trước đây về chủ đề này, nói chung các giả thiết hạn chế đã được đặt ra về các điểm kỳ dị của các hàm được xét và các trường hợp được cho là ngoại lệ thì hoặc được đề cập thoáng qua như các trường hợp giới hạn, hoặc hoàn toàn bị bỏ qua. Tương tự, một số định lý cơ bản về tính liên tục hoặc tính giải tích được chấp nhận, mà "tính hiển nhiên" của chúng phụ thuộc vào các trực giác hình học có bản chất đa dạng" ([10 bis], p. 181) (*).

đối với Riemann, một định nghĩa thuần túy đại số về giống của một đường cong, như là số nguyên nhỏ nhất $p$ sao cho có các hàm hữu tỉ trên đường cong với các cực tại $p + 1$ điểm tùy ý đã cho. Điều thú vị là cần chỉ ra rằng, khi tìm cách thu được các phần tử đóng vai trò là các hàm chỉ có một cực trên đường cong, Weierstrass, trước khi cuối cùng sử dụng các hàm siêu việt cho mục đích này, đã, theo Kronecker ([9e], p. 197), thúc giục người sau mở rộng cho các hàm đại số của một biến những kết quả mà khi đó ông vừa thu được cho các trường số ("các nhân tử nguyên tố của iđêan" thực sự đóng vai trò mà Weierstrass mong muốn).

(*) Người ta biết rõ rằng, bất chấp những nỗ lực của Dedekind, Weber và Kronecker, sự lỏng lẻo trong quan niệm về điều tạo nên một chứng minh đúng đắn, vốn đã thấy rõ trong trường phái Hình học Đại số Đức trong những năm 1870–1880, chỉ càng ngày càng trầm trọng hơn trong công trình của các nhà hình học Pháp và trên hết là Ý của hai thế hệ tiếp theo, những người, theo các nhà hình học Đức và phát triển các phương pháp của họ, đã tấn công lý thuyết các mặt đại số: một "vụ bê bối" thường bị các nhà đại số lên án (chủ yếu từ năm 1920), nhưng ở một mức độ nào đó được biện minh bởi những thành công rực rỡ đạt được nhờ các phương pháp "không chặt chẽ" này, trái ngược với thực tế là, cho đến khoảng năm 1940, những người kế tục chính thống của Dedekind đã tỏ ra không có khả năng xây dựng với đủ tính linh hoạt và sức mạnh các khái niệm đại số cho phép đưa ra các chứng minh đúng đắn về những kết quả này.

Ý tưởng cốt yếu trong công trình của họ là mô hình hóa lý thuyết các hàm đại số của một biến theo lý thuyết các số đại số như Dedekind vừa mới phát triển; để làm điều này, trước hết họ phải xem xét nó từ một quan điểm “afin” (trái với những người cùng thời với họ, những người luôn luôn xem các đường cong đại số như được nhúng trong không gian xạ ảnh phức): do đó họ bắt đầu với một mở rộng đại số hữu hạn K của trường $\mathbf{C}(X)$ các hàm hữu tỉ và vành A của các “hàm đại số nguyên” trong K, tức là các phần tử của trường này nguyên trên vành đa thức $\mathbf{C}[X]$; kết quả cơ bản của họ, mà họ thu được mà không dùng bất kỳ xem xét tôpô nào (*), là A là một miền Dedekind, mà vào đó có thể áp dụng mutatis mutandis (và thậm chí, như Dedekind và Weber nhận xét, mà chưa nhìn thấy rõ lý do ([10], tập I, p. 268), theo một cách đơn giản hơn) tất cả các kết quả của “phần bù thứ 11”. Sau khi làm điều này, họ chứng minh rằng các định lý của họ thực sự là bất biến song hữu tỉ (nói cách khác, chỉ phụ thuộc vào trường K) và đặc biệt không phụ thuộc vào sự lựa chọn của “đường thẳng ở vô cực” được thực hiện lúc đầu. Điều chắc chắn còn thú vị hơn đối với chúng ta là, để định nghĩa các điểm của “mặt Riemann” tương ứng với K (và đặc biệt là các “điểm ở vô cực”, vốn không thể tương ứng với các iđêan của A), họ được dẫn đến việc đưa vào khái niệm nơi của trường K: Họ thấy mình ở cùng tình huống mà Gelfand sẽ gặp vào năm 1940 khi xây dựng lý thuyết các đại số chuẩn, biết một tập hợp K gồm các phần tử vốn ngay từ đầu không được cho như các hàm nhưng người ta vẫn muốn xem như vậy; và, để thu được tập hợp xác định của các hàm giả định, lần đầu tiên họ có ý tưởng (mà Gelfand đã theo và đã trở thành thông dụng vì được sử dụng ở mọi nơi trong toán học hiện đại) là gắn với một điểm x một tập hợp E và với một tập hợp $\mathcal{F}$ các ánh xạ từ E vào một tập hợp G ánh xạ $f \mapsto f(x)$ của $\mathcal{F}$ vào G, nói cách khác là xem xét, trong biểu thức $f(x)$, $f$ như biến và $x$ như cố định, trái với truyền thống cổ điển. Cuối cùng, bắt đầu từ khái niệm nơi, họ không gặp khó khăn nào trong việc định nghĩa các “ước dương” (“Polygon” theo thuật ngữ của họ), bao gồm các iđêan của A như những trường hợp riêng và tương ứng với các “hệ điểm” của Brill và Noether; nhưng, mặc dù họ viết các ước chính và các ước của vi phân như các “thương” của các ước dương, họ không đưa ra định nghĩa tổng quát về ước và chỉ đến năm 1902 Hensel và Landsberg mới đưa vào, bằng phép tương tự với các iđêan phân thức, khái niệm này, khái niệm sẽ luôn gây khó khăn cho những người ủng hộ các phương pháp “hình học” thuần túy (bị buộc dù không muốn phải định nghĩa chúng với tên “các hệ ảo”, nhưng không thoải mái vì không thể cho chúng một cách giải thích “cụ thể”).

Cùng năm 1882 cũng chứng kiến sự xuất hiện hồi ký lớn của Kronecker được chờ đợi hơn 20 năm [9f]. Tham vọng hơn nhiều so với công trình của Dedekind-

(*) Họ nhấn mạnh rằng, nhờ sự kiện này, tất cả các kết quả của họ vẫn đúng nếu trường $\mathbf{C}$ được thay thế bởi trường gồm tất cả các số đại số ([10], tập I, p. 240).

Weber, công trình này cũng không may là mơ hồ và tối nghĩa hơn nhiều. Chủ đề trung tâm của nó là (theo ngôn ngữ hiện đại) việc nghiên cứu các iđêan của một đại số nguyên hữu hạn trên một trong các vành đa thức $\mathbf{C}[X_1, \ldots, X_n]$ hoặc $\mathbf{Z}[X_1, \ldots, X_n]$; Kronecker tự giới hạn $a\ priori$ vào các iđêan đó là sinh hữu hạn (sự kiện rằng tất cả chúng đều như vậy chỉ được chứng minh (đối với các iđêan của $\mathbf{C}[X_1, \ldots, X_n]$)) vài năm sau bởi Hilbert trong quá trình công trình của ông về các bất biến [16a]). Đối với $\mathbf{C}[X_1, \ldots, X_n]$ hoặc $\mathbf{Z}[X_1, \ldots, X_n]$, điều này tự nhiên dẫn đến việc gắn với mỗi iđêan của một trong các vành này “đa tạp đại số” gồm các nghiệm chung của tất cả các phần tử của iđêan; và việc nghiên cứu hình học trong 2 và 3 chiều trong thế kỷ 19 đã dẫn đến một cách trực giác ý tưởng rằng mọi đa tạp là hợp của một số hữu hạn các đa tạp “bất khả quy” mà các “chiều” của chúng không nhất thiết đều giống nhau. Có vẻ như chứng minh của sự kiện này là mục tiêu mà Kronecker đặt ra cho mình, mặc dù ông không nói điều đó ở bất kỳ đâu một cách tường minh và không thể tìm thấy trong hồi ký của ông một định nghĩa nào về “đa tạp bất khả quy”, cũng như về “chiều”. Thực tế, ông chỉ giới hạn ở việc chỉ ra một cách tóm tắt rằng một phương pháp khử tổng quát (*) cho, bắt đầu với một hệ các phần tử sinh của iđêan được xét, một số hữu hạn các đa tạp đại số, mà đối với mỗi đa tạp trong số đó, trong một hệ tọa độ thích hợp, một số tọa độ nhất định là tùy ý còn các tọa độ khác là các “hàm đại số” của chúng (†). Nhưng nếu quả thực sự phân tích thành các đa tạp bất khả quy là điều mà Kronecker hướng tới, thì phải thừa nhận rằng ông chỉ đạt được điều đó trong trường hợp sơ cấp của một iđêan chính, nơi ông chứng minh một cách hiệu quả, mở rộng một bổ đề cổ điển của Gauss về $\mathbf{Z}[X]$ ([3], tập I, p. 34), rằng các miền $\mathbf{C}[X_1, \ldots, X_n]$ và $\mathbf{Z}[X_1, \ldots, X_n]$ là các vành nhân tử; còn trong trường hợp tổng quát, có thể nghi ngờ liệu Kronecker có nắm được khái niệm iđêan nguyên tố hay không (cái mà ông gọi là “Primmodulsystem” là một iđêan không phân tích được thành tích của hai iđêan khác ([9f], p. 336); điều này càng đáng ngạc nhiên hơn vì định nghĩa đã được Dedekind đưa ra vào năm 1871 là hoàn toàn tổng quát).

Tuy nhiên, phải nói rằng phương pháp khử của Kronecker, khi được áp dụng thích hợp, chắc chắn dẫn đến sự phân tích một đa tạp đại số thành các thành phần bất khả quy của nó: điều này được E. Lasker thiết lập rõ ràng ở đầu hồi ký lớn của ông năm 1905 về các iđêan đa thức [19]; ông định nghĩa đúng đắn các

(*) Bằng một phép thay đổi tọa độ tuyến tính, có thể giả sử rằng các phần tử sinh $F_i$ ($1 \leq i \leq r$) của iđêan là các đa thức mà số hạng có bậc cao nhất theo $X_1$ có dạng $c_i X_1^{m_i}$, trong đó $c_i$ là một hằng $\neq 0$. Cũng có thể giả sử rằng các $F_i$ không có nhân tử chung. Khi đó xét đối với $2r$ bất định $u_i, v_i$ ($1 \leq i \leq r$) các đa thức $\sum_{i=1}^r u_i F_i$ và $\sum_{i=1}^r v_i F_i$ như các đa thức theo $X_1$; lập định thức Sylvester của chúng, đó là một đa thức theo các $u_i$ và $v_i$ với các hệ số thuộc $\mathbf{C}[X_2, \ldots, X_n]$ (tương ứng $\mathbf{Z}[X_2, \ldots, X_n]$); bằng cách triệt tiêu các hệ số này, thu được một hệ phương trình mà các nghiệm $(x_2, \ldots, x_n)$ chính xác là các hình chiếu của các nghiệm $(x_1, \ldots, x_n)$ của hệ phương trình $F_i(x_1, x_2, \ldots, x_r) = 0$ ($1 \leq i \leq r$). Khi đó có thể tiếp tục áp dụng phương pháp bằng quy nạp theo $n$.

(†) Chính số các tọa độ tùy ý này mà ông gọi là *chiều* ("Stufe").

khái niệm đa tạp bất khả quy (trong $\mathbf{C}^n$) như một đa tạp đại số V sao cho tích của hai đa thức chỉ có thể bằng không trên toàn bộ đa tạp V nếu một trong hai đa thức đó bằng không trên toàn bộ đa tạp, và ông cũng đưa ra một định nghĩa độc lập với lựa chọn các trục. Trong những xem xét lịch sử thú vị mà ông đưa vào công trình này, Lasker cho thấy rằng ông quan tâm không chỉ đến các khuynh hướng đại số thuần túy của Kronecker và Dedekind, mà còn đến các bài toán do các phương pháp hình học của trường phái Clebsch và M. Noether đặt ra, và đặc biệt đến định lý nổi tiếng được người sau chứng minh năm 1873 [12]. Về bản chất, ông quan tâm, như cách chúng ta nói ngày nay, đến việc xác định iđêan $\mathfrak{a}$ của các đa thức thuộc $\mathbf{C}[X_1, \ldots, X_n]$ triệt tiêu tại các điểm của một tập hợp M cho trước của $\mathbf{C}^n$; thông thường M là "đa tạp đại số" của các không điểm chung của các đa thứcf, hữu hạn về số lượng, và trong một thời gian dài dường như người ta đã chấp nhận (tất nhiên không có chứng minh) rằng, ít nhất đối với $n = 2$ hoặc $n = 3$, iđêan $\mathfrak{a}$ đơn giản chỉ được sinh bởi các f, (*). M. Noether đã chỉ ra rằng ngay cả đối với $n = 2$ và đối với hai đa thức $f_1, f_2$ điều này nói chung là sai, và ông đã đưa ra các điều kiện đủ để $\mathfrak{a}$ được sinh bởi $f_1$ và $f_2$. Mười năm sau, Netto chứng minh rằng, không có giả thiết nào về $f_1$ và $f_2$, một lũy thừa của $\mathfrak{a}$ luôn được chứa trong iđêan sinh bởi $f_1$ và $f_2$ [15], một định lý mà Hilbert đã tổng quát hóa năm 1893 trong Nullstellensatz nổi tiếng của ông [16b]. Không nghi ngờ gì được gợi ý bởi kết quả này, Lasker, trong hồi ký của mình, đưa vào khái niệm tổng quát về iđêan nguyên sơ (†) trong các vành $\mathbf{C}[X_1, \ldots, X_n]$ và $\mathbf{Z}[X_1, \ldots, X_n]$ (sau khi đã đưa ra cho các vành này định nghĩa về iđêan nguyên tố, bằng cách chép lại định nghĩa của Dedekind) và chứng minh (*) sự tồn tại của một phân tích nguyên sơ

(*) Xem các nhận xét của M. Noether ở phần đầu hồi ký của ông [13]. Thật thú vị khi lưu ý về vấn đề này rằng, theo Lasker, Cayley, vào khoảng năm 1860, đã phỏng đoán rằng đối với mỗi đường cong đại số xoắn trong $\mathbf{C}^3$ tồn tại một số hữu hạn các đa thức sinh ra iđêan của các đa thức thuộc $\mathbf{C}[X, Y, Z]$ triệt tiêu trên đường cong (nói cách khác, một trường hợp riêng của định lý hữu hạn của Hilbert [16a]).

(†) Các ví dụ về những iđêan nguyên sơ không phải là lũy thừa của các iđêan nguyên tố đã được Dedekind gặp trong các "thứ tự", tức là các vành của các số đại số với một trường số cho trước làm trường phân thức ([10], tập III, p. 306). Kronecker cũng đưa ra làm ví dụ về một iđêan "không phân tích được" như là tích của hai iđêan không tầm thường khác, iđêan của $\mathbf{Z}[X]$ sinh bởi $p^2$ và $X^2 + p$, trong đó $p$ là một số nguyên tố (một iđêan là nguyên sơ đối với iđêan nguyên tố sinh bởi $X$ và $p$ ([9f], p. 341)).

(‡) Lasker tiến hành bằng quy nạp theo chiều cực đại $h$ của các thành phần bất khả quy của đa tạp V các không điểm của iđêan $\mathfrak{a}$ đang được xét. Theo thuật ngữ hiện đại, trước hết ông xét các iđêan nguyên tố $\mathfrak{p}_i$ ($1 \leq i \leq r$) chứa $\mathfrak{a}$, tương ứng với các thành phần bất khả quy có chiều cực đại $h$ của V. Với mỗi $\mathfrak{p}_i$, ông liên kết phần bão hòa $q_i$ của $\mathfrak{a}$ đối với $\mathfrak{p}_i$ (xem Chương IV, § 2, no. 3, Mệnh đề 5); sau đó ông xét toán tử chuyển $b_i = \mathfrak{a} : q_i$ của $q_i$ trong $\mathfrak{a}$, lấy trong $\sum b_i$ một phần tử c thuộc không một $\mathfrak{p}_i$ nào và chỉ ra một mặt rằng $\mathfrak{a}$ là giao của các $q_i$ và $\mathfrak{a} + (c) = \mathfrak{a}'$ và mặt khác rằng đa tạp V' của với mọi iđêan trong các vành này (*). Ông dường như không quan tâm đến các vấn đề về tính duy nhất trong phân tích này; chính Macaulay là người, ít lâu sau [21], đưa ra sự phân biệt giữa các iđêan nguyên sơ "nhúng" và "không nhúng" và chỉ ra rằng các iđêan sau được xác định duy nhất, nhưng không phải các iđêan trước. Cuối cùng cần lưu ý rằng Lasker cũng mở rộng các kết quả của mình đến vành các chuỗi lũy thừa hội tụ trong một lân cận của một điểm, bằng cách sử dụng "định lý chuẩn bị" của Weierstrass. Phần này trong hồi ký của ông chắc chắn là nơi đầu tiên vành này được xét từ một quan điểm đại số thuần túy và các phương pháp mà Lasker phát triển trong dịp này đã ảnh hưởng mạnh đến Krull khi vào năm 1938 ông tạo ra lý thuyết tổng quát về các vành địa phương (xem [29d], p. 204 và các chỗ khác).

\*   \*   \*

Trào lưu các ý tưởng sẽ khai sinh Đại số giao hoán hiện đại bắt đầu hình thành vào khoảng năm 1910. Nếu khái niệm tổng quát về trường đã đạt được vào đầu thế kỷ 20, thì trái lại công trình đầu tiên trong đó khái niệm tổng quát về vành được định nghĩa có lẽ là công trình của Fraenkel năm 1914 [23]. Vào thời điểm này, đã có làm ví dụ về các vành, không chỉ các miền nguyên của Lý thuyết Số và Hình học Đại số, mà còn các vành chuỗi lũy thừa (hình thức và hội tụ) và cuối cùng là các đại số (giao hoán hoặc không) trên một trường cơ sở. Tuy nhiên, đối với lý thuyết về các trường cũng như lý thuyết về các vành, vai trò xúc tác dường như đã được đảm nhận bởi lý thuyết về các số $p$-adic của Hensel, mà Fraenkel và cả Steinitz [20a] đều đặc biệt nhắc đến như điểm khởi đầu của nghiên cứu của họ.

Công bố đầu tiên của Hensel về chủ đề này có từ năm 1897; tại đó ông xuất phát từ sự tương tự được Dedekind và Weber chỉ ra giữa các điểm của một mặt Riemann của một trường hàm đại số K và các iđêan nguyên tố của một trường số $k$; ông đề xuất chuyển sang Lý thuyết Số các "khai triển Puiseux" (cổ điển từ giữa thế kỷ 19), các khai triển này trong một lân cận của bất kỳ điểm nào của mặt Riemann của K cho phép mọi phần tử $x \in \mathbf{K}$ được biểu diễn dưới dạng một chuỗi hội tụ các lũy thừa của "phần tử chuẩn hóa" tại điểm được xét (một chuỗi chỉ có một số hữu hạn số hạng

các không điểm của $a'$ chỉ có các thành phần bất khả quy có chiều $\leq h - 1$, điều này cho phép ông kết luận bằng quy nạp.

(*) Điều thú vị cần lưu ý là chứng minh thứ hai của Dedekind về định lý phân tích duy nhất tiến hành bằng cách trước hết thiết lập sự tồn tại của một phân tích nguyên sơ rút gọn duy nhất; và trong một đoạn không được công bố trong phần bổ sung thứ 11, Dedekind nhận xét một cách tường minh rằng phần này của chứng minh không chỉ đúng cho vành A của tất cả các số nguyên của một trường số K, mà còn cho mọi "vành thứ tự" của K ([10], tập III, p. 303). Chỉ sau đó, sau khi chỉ ra một cách tường minh rằng A là "đóng nguyên hoàn toàn" (theo thuật ngữ tương ứng) ông mới chứng minh, sử dụng sự kiện này, rằng các iđêan nguyên sơ của phân tích trên thực ra là các lũy thừa của các iđêan nguyên tố ([10], tập III, p. 307).

với số mũ âm). Hensel cũng chỉ ra tương tự rằng, nếu $\mathfrak{p}$ là một iđêan nguyên tố của $k$ nằm trên một số nguyên tố $p$, thì một "chuỗi $p$-adic" có thể được liên kết với mọi $x \in k$, có dạng $\sum_i \alpha_i p^i$ (hoặc $\sum_i \alpha_i p^{i/e}$ khi $\mathfrak{p}$ phân nhánh trên $p$), các $\alpha_i$ được lấy trong một hệ đại diện đã cho của trường thặng dư của iđêan $\mathfrak{p}$; nhưng tính độc đáo lớn của ông nằm ở việc đã có ý tưởng xét các "khai triển" như vậy ngay cả khi chúng tương ứng với *không phần tử nào* của $k$, theo sự tương tự với các khai triển thành chuỗi nguyên của các hàm siêu việt trên một mặt Riemann [18a].

Trong suốt phần còn lại của sự nghiệp, Hensel dành hết tâm trí để trau chuốt và hoàn thiện dần từng chút một phép tính mới của mình; và nếu cách trình bày của ông đối với chúng ta có vẻ do dự hoặc nặng nề, thì không được quên rằng ít nhất vào lúc ban đầu ông không có trong tay bất kỳ công cụ tôpô hay đại số nào của toán học hiện đại vốn có thể làm cho công việc của ông dễ dàng hơn. Trong các công bố đầu tiên của mình, ông hơn nữa hầu như không nói đến các khái niệm tôpô và nói chung đối với ông vành của $p$-adic nguyên ($\mathfrak{p}$ là một iđêan nguyên tố trong vành các số nguyên $\mathbf{A}$ của một trường số $k$) theo thuật ngữ hiện đại là giới hạn ngược của các vành $\mathbf{A}/\mathfrak{p}^n$ với $n$ tăng vô hạn, theo một nghĩa hoàn toàn đại số; và để thiết lập các tính chất của vành này và trường các phân thức của nó, cần phải ở mỗi bước sử dụng những lập luận *ad hoc* ít nhiều khó nhọc (chẳng hạn để chứng minh rằng các số nguyên $p$-adic tạo thành một miền nguyên). Ý tưởng đưa các khái niệm tôpô vào một trường $p$-adic không xuất hiện trong các công trình của Hensel trước năm 1905 [18d]; và chỉ đến năm 1907, sau khi đã xuất bản cuốn sách trong đó ông trình bày lại lý thuyết về các số đại số theo những ý tưởng của mình [18f]), ông mới đi đến định nghĩa và các tính chất cốt yếu của các giá trị tuyệt đối $p$-adic [18e], bắt đầu từ đó ông có thể phát triển, mô phỏng theo lý thuyết của Cauchy, một “giải tích $p$-adic” mới mà ông có thể áp dụng một cách hiệu quả vào Lý thuyết Số (đặc biệt bằng cách sử dụng hàm mũ và lôgarit $p$-adic) và tầm quan trọng của nó kể từ đó ngày càng tăng.

Hensel đã thấy rõ, ngay từ đầu, những sự đơn giản hóa mà lý thuyết của ông mang lại cho các cách trình bày cổ điển, bằng cách cho phép các vấn đề được “địa phương hóa” và công việc được tiến hành trong một trường mà ở đó không chỉ các tính chất chia hết là tầm thường, mà còn, nhờ bổ đề cơ bản mà ông đã phát hiện ngay từ năm 1902 [18c], việc nghiên cứu các đa thức mà các đa thức “thu gọn” của chúng mod $p$ không có nghiệm bội được quy về việc nghiên cứu các đa thức trên một trường hữu hạn. Ngay từ năm 1897 [18b], ông đã đưa ra những ví dụ đáng chú ý về các sự đơn giản hóa này, đặc biệt về các câu hỏi liên quan đến biệt thức (đặc biệt là một chứng minh ngắn gọn cho tiêu chuẩn mà ông đã đưa ra vài năm trước về sự tồn tại của các “ước ngoại thường”). Nhưng trong một thời gian dài dường như các số $p$-adic đã gây ra sự không tin tưởng đáng kể ở các nhà toán học đương thời; một thái độ hiện thời chắc chắn đối với những ý tưởng “quá trừu tượng”, nhưng cũng được biện minh một phần bởi sự nhiệt tình hơi quá mức của tác giả của chúng (điều rất thường thấy trong toán học ở những người nhiệt thành với các lý thuyết mới). Không chỉ bằng lòng với việc áp dụng lý thuyết của mình một cách hiệu quả vào các số đại số, Hensel, bị ấn tượng như tất cả những người cùng thời với ông bởi các chứng minh về tính siêu việt của $e$ và $\pi$ và có lẽ bị đánh lạc hướng bởi tính từ "siêu việt" được áp dụng đồng thời cho các số và các hàm, đã đi đến chỗ nghĩ rằng tồn tại một mối liên hệ giữa các số p-adic của ông và các số thực siêu việt và ông đã từng nghĩ trong một thời gian ngắn rằng mình đã thu được một chứng minh đơn giản về tính siêu việt của $e$ và thậm chí của $e^e$ ([18d], p. 556) (*).

Ngay sau năm 1910, tình hình thay đổi, với sự trỗi dậy của thế hệ tiếp theo, chịu ảnh hưởng bởi các ý tưởng của Frtchet và F. Riesz về tôpô và bởi các ý tưởng của Steinitz về đại số, và ngay từ đầu đã dành cho “sự trừu tượng”; thế hệ này sẽ biết cách đồng hóa và đặt các công trình của Hensel vào đúng vị trí của chúng. Ngay từ năm 1913, Kürschak [22] đưa ra một định nghĩa tổng quát về khái niệm giá trị tuyệt đối, nhận ra tầm quan trọng của các giá trị tuyệt đối siêu mêtric (mà giá trị tuyệt đối p-adic là một ví dụ), chứng minh (bằng cách mô phỏng chứng minh theo trường hợp các số thực) sự tồn tại của phép hoàn thiện của một trường đối với một giá trị tuyệt đối và trên hết chỉ ra một cách tổng quát khả năng mở rộng một giá trị tuyệt đối đến bất kỳ mở rộng đại số nào của trường đã cho. Nhưng ông đã không thấy rằng đặc trưng siêu mêtric của một giá trị tuyệt đối đã được bộc lộ ngay trong trường nguyên tố; điểm này được Ostrowski thiết lập, người cũng là người xác định tất cả các giá trị tuyệt đối trên trường $\mathbf{Q}$ và định lý cơ bản đặc trưng các trường có một giá trị tuyệt đối không siêu mêtric như các trường con của $\mathbf{C}$ [24]. Trong những năm từ 1920 đến 1935, lý thuyết sẽ được hoàn thiện bằng một nghiên cứu chi tiết hơn về các giá trị tuyệt đối không nhất thiết rời rạc, bao gồm trong số đó việc khảo sát nhiều hoàn cảnh khác nhau nảy sinh khi chuyển qua một mở rộng đại số hoặc siêu việt (Ostrowski, Deuring, F. K. Schmidt); mặt khác, năm 1931, Krull đưa vào và nghiên cứu khái niệm tổng quát về định giá [29b], khái niệm này sẽ được Zariski và trường phái của ông trong Hình học Đại số sử dụng rất nhiều trong những năm tiếp theo (†). Cũng cần phải nhắc đến ở đây, mặc dù nằm ngoài phạm vi của chúng ta, những nghiên cứu sâu sắc hơn về cấu trúc của các trường đầy đủ có định giá và các vành địa phương đầy đủ, có cùng niên đại với giai đoạn này (Hasse-Schmidt, Witt, Teichmuller, I. Cohen).

\*   \*   \*

Công trình của Fraenkel được nhắc đến ở trên (p. 594) chỉ xét một trường hợp rất đặc biệt

(*) Việc nghiên cứu bằng mọi giá một sự song song chặt chẽ giữa các chuỗi p-adic và các chuỗi Taylor này cũng khiến Hensel tự đặt ra cho mình những vấn đề kỳ lạ: chẳng hạn ông chứng minh rằng mọi số nguyên p-adic có thể được viết dưới dạng một chuỗi $\sum_{k=0}^{\infty} a_k p^k$ trong đó các $a_k$ là các số hữu tỉ được chọn sao cho chuỗi hội tụ không chỉ trong $\mathbf{Q}_p$, mà còn trong $\mathbf{R}$ (có lẽ do sự tương tự với các chuỗi Taylor hội tụ đồng thời tại nhiều nơi?) ([16e] và [16f]).

(†) Một ví dụ về một định giá có chiều cao 2 đã được H. Jung đưa vào một cách tình cờ từ năm 1925 [27].

kiểu vành (Artin với chỉ một iđêan nguyên tố duy nhất, hơn nữa được giả sử là chính). Ngoại trừ công trình của Steinitz về các trường [20a], những công trình quan trọng đầu tiên về việc nghiên cứu các vành giao hoán tổng quát là hai hồi ký lớn của E. Noether về lý thuyết iđêan: hồi ký năm 1921 [25a], dành cho phân tích nguyên sơ, trong đó nhắc lại một cách hoàn toàn tổng quát và hoàn thiện trên nhiều điểm các kết quả của Lasker và Macaulay; và hồi ký năm 1927 đặc trưng các miền Dedekind một cách tiên đề [25b]. Cũng như Steinitz đã chỉ ra đối với các trường, trong các hồi ký này người ta thấy rằng một số nhỏ các ý tưởng trừu tượng, như khái niệm iđêan bất khả quy, các điều kiện dây chuyền và ý tưởng về miền đóng nguyên (hai ý tưởng sau, như ta đã thấy, đã được Dedekind làm sáng tỏ từ trước), tự chúng có thể dẫn đến các kết quả tổng quát mà dường như gắn bó không thể tách rời với các kết quả của tính toán thuần túy trong những trường hợp trước đây chúng đã được biết.

Cùng với các hồi ký này của E. Noether, kết hợp với các công trình hơi muộn hơn của Artin-van der Waerden về các iđêan chia [31] và của Krull liên hệ các iđêan này với các định giá cốt yếu [29b], việc nghiên cứu lâu dài về phân tích các iđêan bắt đầu từ một thế kỷ trước (*) nay hoàn tất, đồng thời với việc Đại số giao hoán hiện đại được khai sinh.

Các công trình nghiên cứu vô số về Đại số giao hoán sau này được nhóm lại dễ dàng nhất theo một số hướng phát triển quan trọng:

(A) Các vành địa phương và các tôpô

Mặc dù mầm đã được chứa trong tất cả các công trình trước đây về Lý thuyết Số và Hình học Đại số, ý tưởng tổng quát về địa phương hóa xuất hiện rất chậm. Khái niệm tổng quát về vành phân thức chỉ được định nghĩa vào năm 1926 bởi H. Grell, một học trò của E. Noether, và chỉ đối với các miền nguyên [28]; mở rộng của nó đến các vành tổng quát hơn chỉ được đưa ra vào năm 1944 bởi C. Chevalley cho các vành Noether và vào năm 1948 bởi Uzkov trong trường hợp tổng quát. Cho đến khoảng năm 1940, Krull và trường phái của ông gần như một mình sử dụng trong các lập luận tổng quát việc xét các vành địa phương A, của một miền nguyên A; các vành này chỉ bắt đầu xuất hiện tường minh trong Hình học Đại số với các công trình của Chevalley và Zariski bắt đầu từ năm 1940 (†).

Việc nghiên cứu tổng quát bản thân các vành địa phương chỉ bắt đầu vào năm 1938 với hồi ký lớn [29d] của Krull. Các kết quả quan trọng nhất của công trình này liên quan đến lý thuyết chiều và các vành chính quy, mà ta sẽ không nói đến ở đây; nhưng tại đây lần đầu tiên xuất hiện phép đầy đủ hóa của mọi vành địa phương Noether tùy ý và cũng xuất hiện một dạng còn chưa hoàn thiện của vành phân bậc liên kết với một vành địa phương (*); dạng sau chỉ được định nghĩa vào khoảng năm 1948 bởi P. Samuel [36] và một cách độc lập trong các nghiên cứu về Tôpô Đại số bởi Leray và H. Cartan. Krull, trong công trình nói trên, hầu như không sử dụng ngôn ngữ tôpô; nhưng ngay từ năm 1928[29a], ông đã chứng minh rằng, trong một vành Noether $\mathbf{A}$, giao của các lũy thừa của một iđêan $\mathbf{a}$ là tập hợp các $x \in \mathbf{A}$ sao cho $x(1 - a) = 0$ với một $a \in \mathbf{a}$ nào đó; từ đó dễ dàng suy ra rằng, đối với mọi iđêan $m$ của $\mathbf{A}$, tôpô $m$-adic trên $\mathbf{A}$ cảm sinh trên một iđêan $\mathbf{a}$ tôpô $m$-adic trên $\mathbf{a}$; trong hồi ký năm 1938 của mình, Krull hoàn thiện kết quả này bằng cách chứng minh rằng trong một vành địa phương Noether mọi iđêan đều đóng. Các định lý này ngay sau đó được Chevalley mở rộng cho các vành nửa địa phương Noether và rồi được Zariski mở rộng cho các vành mang tên ông [33b]; việc đưa vào "tính compact tuyến tính" trong các vành tôpô, cũng như việc xác định cấu trúc của các vành nửa địa phương đầy đủ [32b], cũng bắt nguồn từ Chevalley.

(B) Chuyển từ địa phương sang toàn cục

Kể từ Weierstrass, một hàm giải tích của một biến (và đặc biệt là một hàm đại số) thường được liên kết với tập hợp các "khai triển" của nó tại tất cả các điểm của mặt Riemann nơi nó được xác định. Trong phần mở đầu cuốn sách của ông về Lý thuyết Số ([18f], p. V), Hensel cũng tương tự liên kết với mỗi phần tử của một trường số đại số $k$ tập hợp các phần tử tương ứng với nó trong các phép đầy đủ hóa của $k$ đối với tất cả các giá trị tuyệt đối trên $k$ ($\dagger$). Có thể nói rằng chính quan điểm này, trong Đại số giao hoán hiện đại, đã thay thế công thức phân tích một iđêan thành tích của các iđêan nguyên tố (mở rộng theo một nghĩa nào đó quan điểm ban đầu của Kummer). Nhận xét của Hensel ngầm tương đương với việc nhúng $k$ vào tích của tất cả các phép đầy đủ hóa của nó; đây là điều mà Chevalley thực hiện một cách tường minh vào năm 1936 với lý thuyết của ông về

(*) Nếu $m$ là iđêan cực đại của vành địa phương Noether $\mathbf{A}$ đang xét và $(\alpha_i)_{1 \leq i \leq r}$, một hệ sinh cực tiểu của $m$, Krull định nghĩa với $x \neq 0$ trong $\mathbf{A}$ các "dạng ban đầu" của $x$ như sau: nếu $j$ là số nguyên lớn nhất sao cho $x \in m^j$, các dạng ban đầu của $x$ là tất cả các đa thức thuần nhất bậc $j$, $P(X_1, \ldots, X_r)$ với các hệ số trong trường thặng dư $k = \mathbf{A}/m$, sao cho $x \equiv P(\alpha_1, \ldots, a,) \pmod{m^{j+1}}$. Với mỗi iđêan $\mathbf{a}$ của $\mathbf{A}$ ông liên kết iđêan phân bậc của $k[X_1, \ldots, X_r]$ sinh bởi các dạng ban đầu của tất cả các phần tử của $\mathbf{a}$ ("Leitideal"); hai khái niệm này đối với ông thay thế cho vành phân bậc liên kết.

($\dagger$) Hensel lấy, như các giá trị tuyệt đối không siêu chuẩn trên một trường $K$ có bậc $n$ trên $\mathbf{Q}$, các hàm $x \mapsto |x^{(i)}|$ (trong đó các $x^{(i)}$ với $1 \leq i \leq n$ là các phần tử liên hợp của $x$) hiện đang được sử dụng kể từ Dirichlet; Ostrowski sau đó ít lâu đã chứng minh rằng các hàm này về cơ bản là các giá trị tuyệt đối không siêu chuẩn duy nhất trên $K$.

"idèles" [32a], hoàn thiện các ý tưởng tương tự trước đó của Priifer và von Neumann (người sau chỉ giới hạn ở việc nhúng $k$ vào tích của các hoàn thành $p$-adic của nó)(*). Mặc dù điều này hơi nằm ngoài phạm vi của chúng ta, điều quan trọng là phải nhắc đến ở đây rằng, nhờ một tôpô thích hợp trên nhóm idèles, tất cả các kỹ thuật của các nhóm compact địa phương (bao gồm độ đo Haar) do đó có thể được áp dụng rất hiệu quả vào Lý thuyết Số.

Trong một bối cảnh tổng quát hơn, định lý của Krull [29b] đặc trưng một miền nguyên đóng dưới nguyên như một giao của các vành định giá (điều này cũng tương đương với việc nhúng miền đang xét vào một tích của các vành định giá) thường tạo thuận lợi cho việc nghiên cứu các vành này, mặc dù phương pháp này chỉ thực sự khả thi đối với các định giá cốt yếu của các miền Krull. Hơn nữa Krull thường trình bày [29e] các ví dụ (khá sơ cấp) về phương pháp "chuyển từ địa phương sang toàn cục", gồm việc chứng minh một tính chất của một miền nguyên $A$ bằng cách kiểm tra nó đối với các vành "địa phương hóa" $A_i$, của $A$ tại tất cả các iđêan nguyên tố của nó ($\dagger$); gần đây hơn, Serre nhận thấy rằng phương pháp này đúng cho các vành giao hoán tùy ý $A$, rằng nó cũng áp dụng được cho các $A$-môđun và rằng thậm chí thường chỉ cần "địa phương hóa" tại các iđêan cực đại của $A$ (Chương II, §3, Định lý 1): một quan điểm liên hệ chặt chẽ với các ý tưởng về "phổ" và các bó được định nghĩa trên các phổ này (xem dưới đây, p. 602).

(C) Số nguyên và bao đóng nguyên
Chúng ta đã thấy rằng khái niệm số nguyên đại số, ban đầu được đưa vào cho các trường số, đã được Kronecker và Dedekind mở rộng cho các trường hàm đại số, mặc dù trong trường hợp này nó có thể xuất hiện khá nhân tạo (không tương ứng với một khái niệm xạ ảnh). Hồi ký của E. Noether năm 1927, tiếp theo là công trình của Krull bắt đầu từ năm 1931, đã chỉ ra sự quan tâm mà các khái niệm này mang lại cho các vành tổng quát hơn ($\ddagger$). Đặc biệt Krull chịu trách nhiệm về

(*) Do nhận xét này của Hensel, các giá trị tuyệt đối không siêu chuẩn trên một trường số $K$ theo thói quen đã được gọi (do lạm dụng ngôn ngữ) là các "điểm ở vô tận" của $K$, tương tự với quá trình mà Dedekind và Weber định nghĩa các "điểm ở vô tận" của mặt Riemann của một đường cong afin (xem p. 591).

($\dagger$) Khi nói về "chuyển từ địa phương sang toàn cục", thường có sự ám chỉ đến những câu hỏi khó hơn nhiều, liên quan đến lý thuyết trường lớp, và các ví dụ được biết đến nhiều nhất là những ví dụ được xử lý trong các hồi ký của Hasse ([26a] và [26b]) về các dạng toàn phương trên một trường số đại số $k$; ở đó ông chỉ ra, trong số những điều khác, rằng để một phương trình $f(x_1, \ldots, x_n) = a$ có một nghiệm trong $k^n$ ($f$ là một dạng toàn phương, $a \in k$), điều kiện cần và đủ là nó có một nghiệm trong mỗi hoàn thành của $k$. Theo Hasse, ý tưởng về kiểu định lý này đã được thầy của ông là Hensel gợi ý cho ông [26c]. Sự mở rộng "nguyên lý Hasse" này sang các nhóm khác ngoài nhóm trực giao là một trong những mục tiêu của lý thuyết hiện đại về "adelization" của các nhóm đại số.

($\ddagger$) Krull và E. Noether chỉ giới hạn trong các miền nguyên, nhưng việc mở rộng các phương pháp của họ sang trường hợp tổng quát không khó; các định lý hồi ký thú vị nhất về việc nâng các iđêan nguyên tố lên các đại số nguyên [29c], cũng như về việc mở rộng lý thuyết các nhóm phân tích và quán tính của Dedekind-Hilbert [29b]. Còn đối với E. Noether, chúng ta mắc nợ bà về dạng phát biểu tổng quát của bổ đề chuẩn hóa (*) (từ đó suy ra, trong số những điều khác, Định lý không điểm của Hilbert) cũng như tiêu chuẩn tổng quát đầu tiên (chuyển thể các lập luận cổ điển của Kronecker và Dedekind) để bao đóng nguyên của một miền nguyên là hữu hạn trên miền đó.

Cuối cùng, cần chỉ ra ở đây rằng một trong những lý do cho tầm quan trọng hiện nay của khái niệm miền đóng dưới nguyên là do các nghiên cứu của Zariski về các đa tạp đại số; ông đã phát hiện rằng các đa tạp "chuẩn" (nghĩa là những đa tạp mà các vành địa phương của chúng là các miền nguyên đóng dưới nguyên) được phân biệt bởi các tính chất đặc biệt thuận lợi, đáng chú ý là việc chúng không có "điểm kỳ dị đối chiều 1"; và sau đó người ta đã thấy rằng các hiện tượng tương tự cũng đúng đối với các "không gian giải tích". Vì vậy "chuẩn hóa" (nghĩa là phép toán mà đối với các vành địa phương của một đa tạp, gồm việc lấy các bao đóng nguyên của chúng) đã trở thành một vũ khí mạnh trong kho vũ khí của Hình học Đại số hiện đại.

(D) Việc nghiên cứu các môđun và ảnh hưởng của Đại số đồng điều

Một trong những đặc điểm nổi bật của công trình của E. Noether và W. Krull trong Đại số là xu hướng “tuyến tính hóa”, mở rộng sự phát triển tương tự đã được Dedekind và Steinitz đưa ra trong lý thuyết trường; nói cách khác, các iđêan trước hết được xem như các môđun và do đó mọi kiến tạo của Đại số tuyến tính (thương, tích và gần đây hơn là tích tenxơ và sự tạo thành các môđun đồng cấu) đều được áp dụng cho chúng, tạo ra nói chung các môđun không còn là các iđêan nữa. Vì vậy người ta nhanh chóng thấy rằng trong nhiều câu hỏi (đối với các vành giao hoán hoặc không giao hoán), sự quan tâm không nên chỉ giới hạn vào việc nghiên cứu các iđêan của một vành A, mà trái lại các định lý phải được phát biểu một cách tổng quát cho các A-môđun (đôi khi chịu một số điều kiện hữu hạn nào đó).

Sự can thiệp của Đại số đồng điều đã củng cố mạnh mẽ xu hướng trên, vì nhánh này của Đại số về bản chất liên quan đến các câu hỏi có tính chất tuyến tính. Ở đây chúng ta sẽ không nhắc lại lịch sử của nó; nhưng điều đáng chỉ ra là một số khái niệm cơ bản của Đại số đồng điều (chẳng hạn khái niệm môđun xạ ảnh và khái niệm hàm tử Tor) đã ra đời nhân dịp một sự nghiên cứu chi tiết về ứng xử của các môđun trên một miền Dedekind đối với tích tenxơ, một nghiên cứu do H. Cartan tiến hành năm 1948.

về chủ đề này là trường hợp trong đó I. Cohen và Seidenberg mở rộng các định lý nâng của Krull, chỉ ra chính xác các giới hạn về tính đúng của chúng [35]. Cần nhắc rằng E. Noether đã tường minh đề cập đến khả năng của những sự tổng quát hóa như vậy trong hồi ký của bà năm 1927 ([25b], p. 30).

(*) Một trường hợp đặc biệt đã được Hilbert khẳng định từ năm 1893 ([16b], p. 316).

Ngược lại, người ta có thể thấy trước rằng các lớp môđun mới được Đại số đồng điều đưa vào một cách tự nhiên như là các “phần tử triệt tiêu phổ quát” của các hàm tử Ext (các môđun xạ ảnh và các môđun đơn ánh) và các hàm tử Tor (các môđun phẳng) sẽ đem lại ánh sáng mới cho Đại số giao hoán. Thực tế là chủ yếu các môđun xạ ảnh và còn hơn thế nữa các môđun phẳng đã tỏ ra hữu ích: tầm quan trọng của các môđun sau này trước hết xuất phát từ nhận xét, được Serre đưa ra đầu tiên [38b], rằng địa phương hóa và hoàn thiện đưa vào một cách tự nhiên các môđun phẳng, do đó “giải thích” theo một cách thỏa đáng hơn nhiều các tính chất của những phép toán này vốn đã được biết và làm cho chúng dễ sử dụng hơn nhiều. Cũng cần phải nhắc rằng (như chúng ta sẽ thấy trong các chương sau) các ứng dụng của Đại số đồng điều còn lâu mới chỉ giới hạn ở điều này và nó đang đóng một vai trò ngày càng quan trọng trong Hình học đại số.

(E) Khái niệm phổ
Khái niệm mới nhất về ngày tháng trong số các khái niệm mới của Đại số giao hoán có một lịch sử phức tạp. Định lý phổ của Hilbert đã đưa vào các tập hợp có thứ tự của các phép chiếu trực giao của một không gian Hilbert, tạo thành một “đại số Boolean” (hay đúng hơn là một dàn Boolean) (*), tương ứng một-một với một dàn Boolean của các lớp tập con đo được (đối với một độ đo thích hợp) của $\mathbf{R}$. Chắc chắn công trình trước đó của ông về các toán tử trên các không gian Hilbert, vào khoảng năm 1935, đã dẫn M. H. Stone đến việc nghiên cứu các dàn Boolean nói chung và đặc biệt tìm kiếm các “biểu diễn” của chúng bằng các tập con của một tập hợp (hoặc các lớp tập con đối với một quan hệ tương đương nào đó). Ông nhận thấy rằng một dàn Boolean trở thành một vành *giao hoán* (hơn nữa thuộc một kiểu rất đặc biệt), nếu phép nhân được định nghĩa trên nó bởi $xy = \inf(x, y)$ và phép cộng bởi $x + y = \sup(\inf(x, y'), \inf(x', y))$. Trong trường hợp riêng khi dàn Boolean đang xét là tập hợp $\mathfrak{P}(X)$ gồm mọi tập con của một tập hữu hạn $X$, người ta thấy ngay lập tức rằng các phần tử của $X$ tương ứng một-một một cách tự nhiên với các iđêan cực đại của vành “Boolean” tương ứng; và Stone thu được chính xác định lý biểu diễn tổng quát của ông cho một dàn Boolean bằng cách xét tương tự tập hợp các iđêan cực đại của vành tương ứng và gắn với mỗi phần tử của dàn Boolean tập hợp các iđêan cực đại chứa nó [30a].

Mặt khác, tập hợp các tập con vừa mở vừa đóng của một không gian tôpô là một ví dụ cổ điển quen thuộc của một dàn Boolean. Trong một bài báo thứ hai [30b], Stone đã chỉ ra rằng thực tế mọi dàn Boolean cũng đẳng cấu với một dàn Boolean có bản chất này. Để làm điều đó dĩ nhiên cần phải định nghĩa một *tôpô* trên tập hợp các iđêan cực đại của một vành “Boolean”; điều này được thực hiện rất

(*) Một *dàn Boolean* là một tập hợp có thứ tự dàn $E$, với một phần tử nhỏ nhất $a$ và một phần tử lớn nhất $\omega$, trong đó mỗi luật sup và inf là *phân phối* đối với luật kia và, với mọi $a \in E$, tồn tại một $a' \in E$ duy nhất sao cho $\inf(a, a') = a$ và $\sup(a, a') = w$ (xem *Lý thuyết tập hợp*, Chương III, § 1, Bài tập 17).

đơn giản bằng cách lấy làm các tập đóng đối với mỗi iđêan $a$ tập hợp các iđêan cực đại chứa $a$.

Chúng ta sẽ không bàn ở đây về ảnh hưởng của các ý tưởng này đối với Giải tích hàm, nơi chúng đã đóng một vai trò quan trọng trong sự ra đời của lý thuyết các đại số chuẩn được phát triển bởi I. Gelfand và trường phái của ông. Nhưng vào năm 1945, Jacobson nhận xét [34] rằng quá trình định nghĩa một tôpô, được phát minh bởi Stone, thực ra có thể được áp dụng cho mọi vành $A$ (giao hoán hoặc không) với điều kiện tập hợp các iđêan được lấy không phải là tập hợp các iđêan cực đại mà là tập hợp các iđêan "nguyên thủy" hai phía (nghĩa là các iđêan hai phía $b$ sao cho $A/b$ là một vành nguyên thủy); đối với một vành giao hoán, dĩ nhiên các iđêan này hóa ra là các iđêan cực đại. Về phần mình, Zariski, vào năm 1944 [33a], sử dụng một phương pháp tương tự để định nghĩa một tôpô trên tập hợp các *vị trí* của một trường hàm đại số. Tuy nhiên, đối với phần lớn các nhà đại số học, các tôpô này vẫn chỉ là những sự tò mò, bởi vì chúng thường không Hausdorff và người ta cảm thấy một sự ác cảm hoàn toàn dễ hiểu đối với việc làm việc trên những đối tượng khác thường như vậy. Sự ngờ vực này chỉ được vượt qua khi A. Weil chỉ ra, vào năm 1952, rằng mọi đa tạp đại số đều có thể được trang bị một tôpô tự nhiên thuộc kiểu trên và rằng tôpô này cho phép định nghĩa, hoàn toàn tương tự với trường hợp các đa tạp khả vi hoặc giải tích, khái niệm *bó sợi* [37]; ngay sau đó, Serre đã có ý tưởng mở rộng lý thuyết *bó kết hợp* cho các đa tạp này đã được trang bị tôpô, nhờ đó tôpô đem lại trong trường hợp các đa tạp "trừu tượng" những dịch vụ tương tự như tôpô thông thường khi trường cơ sở là $\mathbf{C}$, đặc biệt liên quan đến việc áp dụng các phương pháp của Tôpô đại số ([38a] và [38b]).

Từ đó trở đi, việc sử dụng ngôn ngữ hình học này trong toàn bộ Đại số giao hoán trở nên tự nhiên. Người ta nhanh chóng nhận thấy rằng việc xét các iđêan cực đại thường là không đủ để thu được các khẳng định hữu ích (*) và rằng khái niệm thích hợp là tập hợp các iđêan *nguyên tố* của vành được trang bị tôpô theo cùng một cách. Với sự đưa vào của khái niệm phổ, hiện nay tồn tại một từ điển cho phép biểu diễn mọi định lý của Đại số giao hoán bằng một ngôn ngữ hình học rất gần với ngôn ngữ của Hình học đại số trong thời kỳ Weil-Zariski; điều này hơn nữa đã ngay lập tức đem lại một sự mở rộng đáng kể phạm vi của lý thuyết sau, đến mức Đại số giao hoán hầu như không còn gì khác hơn là phần sơ cấp nhất của nó [39].

(*) Sự bất tiện của việc chỉ giới hạn sự chú ý vào "phổ cực đại" xuất phát từ thực tế rằng, nếu $\phi : A \to B$ là một đồng cấu và $n$ là một iđêan cực đại của $B$, $\phi^{-1}(n)$ không nhất thiết là một iđêan cực đại của $A$, trong khi đối với mọi iđêan nguyên tố $p$ của $B$, $\phi^{-1}(p)$ là một iđêan nguyên tố của $A$. Do đó, nói chung một ánh xạ từ tập hợp các iđêan cực đại của $B$ vào tập hợp các iđêan cực đại của $A$ không thể được liên kết một cách tự nhiên với $\phi$.

1. L. Euler, Vollständige Anleitung zur Algebra (=Opera Omnia (1), vol. I, Leipzig-Berlin (Teubner), 1911).
2. J. L. Lagrange, Oeuvres, 14 volumes, Paris (Gauthier-Villars), 1867–1892.
3. C. F. Gauss, Werke, 12 volumes, Gottingen, 1870-1927.
4. P. G. Lejeune-Dirichlet, Werke, 2 volumes, Berlin (Reimer), 1889–1897.
4 (bis). P. G. Lejeune-Dirichlet, Vorlesungen über Zahlentheorie, 2te Aufl., Braunschweig (Vieweg), 1871.
5. C. G. J. Jacobi, Gesammelte Werke, 7 volumes, Berlin (Reimer), 1881–1891.
6. G. Eisenstein: (a) Beweis der Reciprocitatsgesetzefur die cubischen Reste in der Theorie der aus dritten Wurzeln der Einheit zusammengesetzen Zahlen, Crelle’s Journal, 27 (1844), pp. 289–310; (b) Zur Theorie der quadratischen Zerfallung der Primzahlen 8n + 3, 7n + 2 und 7n + 4, Crelle’s Journal, 37 (1848), pp. 97–126; (c) Über einige allgemeine Eigenschaften der Gleichung von welcher die Teilung der ganzen Lemniscate abhangt, nebst Anwendungen derselben auf die Zahlentheorie, Crelle’s Journal, 39 (1850), pp. 160–179 and 224–287.
7. E. Kummer: (a) Sur les nombres complexes qui sont formés avec les nombres entiers réels et les racines de l’unité, J. de Math., (1), 12 (1847), pp. 185–212; (b) Zur Theorie der complexen Zahlen, Crelle’s Journal, 35 (1847), pp. 319–326; (c) Ueber die Zerlegung der aus Wurzeln der Einheit gebildeten complexen Zahlen in Primfactoren, Crelle’s Journal, 35 (1847), pp. 327–367; (d) Mémoire sur les nombres complexes composés de racines de l’unité et des nombres entiers, J. de Math., (1), 16 (1851), pp. 377–498; (e) Über die allgemeinen Reciprocitatsgesetze unter den Resten und Nichtresten der Potenzen deren Grad eine Primzahl ist (Abh. der Kon. Akad. der Wiss. zu Berlin (1859), Math. Abhandl., pp. 19–159).
8. C. Hermite, Oeuvres, 4 Volumes, Paris (Gauthier-Villars), 1905–1917.
9. L. Kronecker, Werke, 5 volumes, Leipzig (Teubner), 1895–1930: (a) De unitatibus complexis, vol. I, pp. 5–71 (= Inaug. Diss., Berolini, 1845); (b) Über die algebraisch auflosbaren Gleichungen I, vol. IV, pp. 1–11 (= Monatsber. der Kon. Preuss. Akad. der Wiss., 1853, pp. 365–374); (c) Über die elliptischen Functionen fur welche complexe Multiplication stattfindet vol. IV, pp. 177–183 (= Monatsber. der Kon. Preuss. Akad. der Wiss., 1857, pp. 455–460); (d) Uber die complexe Multiplication der elliptischen Functionen, vol. IV, pp. 207–217 (= Monatsber. der Kön. Preuss. Akad. der Wiss., 1862, pp. 363–372); (e) Über die Discriminante algebraischer Functionen einer Variabeln, vol. II, pp. 193–236 (= Crelle’s Journal, 91 (1881), pp. 301–334); (f) Grundzuge einer arithmetischen Theorie der algebraischen Grössen, vol. II, pp. 237–387 (=Crelle’s Journal, 92 (1882), pp. 1–122).

10. R. Dedekind, Gesammelte mathematische Werke, 3 volumes, Braunschweig (Vieweg), 1932: (a) Abriss einer Theorie der höheren Kongruenzen in bezug auf einen reellen Primzahl-Modulus, vol. I, pp. 40–66 (=Crelle’s Journal, 54 (1857), pp. 1–26; (b) Sur la Théorie des Nombres entiers algébriques, vol. III, pp. 262–296 (=Bull. Sci. Math., (1), 11 (1876), pp. 278–288 and (2), 1 (1877), pp. 17–41, 69–92, 144–164, 207–248); (c) Uber die Anzahl der Ideal-Klassen in den verschiedenen Ordnungen eines endlichen Korpers, vol. I, pp. 105–157 (=Festschrift der Technischen Hochschule in Braunschweig zur Säkularfeier des Geburtstages von C. F. Gauss, Braunschweig, 1877, pp. 1–55); (d) Über den Zusammenhang zwischen der Theorie der Ideals und der Theorie der höheren Kongruenzen, vol. I, pp. 202–230 (=Abh. Kön. Ges. Wiss. zu Gottingen, 23 (1878), pp. 1–23); (e) Uber die Discriminantend endlicher Korper, vol. I, pp. 351–396 (=Abh. Kön. Ges. Wiss. zu Gdttingen, 29 (1882), pp. 1–56); (f) Uber die Theorie der ganzen algebraischen Zahlen, vol. III, pp. 1–222 (=Supplement XI von Dirichlets Vorlesungen über Zahlentheorie, 4 Aufl. (1894), pp. 434–657); (g) Zur Theorie der Ideale, vol. 11, pp. 43–48 (=Nachr. Gottingen, 1894, pp. 272–277); (h) Uber eine Erweiterung des Symbols (a, b) in der Theorie der Moduln, vol. II, pp. 59–85 (=Nachr. Göttingen, 1895, pp. 183–208).

10(bis). R. Dedekind-H. Weber, Theorie der algebraischen Funktionen einer Veränderlichen, Crelle’s Journal, 92 (1882), pp. 181–290 (=R. Dedekind, Ges. Math. Werke, vol. I, pp. 238–349).

11. E. Selling, Ueber die idealen Primfactoren der complexen Zahlen, welche aus den Wurzeln einer beliebigen irreductiblen Gleichung rational gebildet sind, Zeitschr.fur Math. und Phys., 10 (1865), pp. 17–47.

12. M. Noether, Uber einen Satz aus der Theorie der algebraischen Funktionen, Math. Ann., 6 (1873), pp. 351–359.

13. A. Brill-M. Noether, Ueber algebraischen Funktionen, Math. Ann., 7 (1874), pp. 269–310.

14. G. Zolotareff, Sur la théorie des nombres complexes, J. de Math. (3), 6 (1880), pp. 51–84 and 129–166.

15. E. Netto, Zur Theorie der Elimination, Acta Math., 7 (1885), pp. 101–104.

16. D. Hilbert: (a) Uber die Theorie der algebraischen Formen, Math. Ann., 36 (1890), pp. 473–534; (b) Uber die vollen Invariantensysteme, Math. Ann., 42 (1893), pp. 313–373; (c) Grundzuge einer Theorie des Galoischen Zahlkorpers, Gött. Nachr., (1894), pp. 224–236; (d) Zahlbericht, Jahresber. der D. M. V., 4 (1897), pp. 175–546 (translated into French by A. Lévy and Th. Got under the title “Théorie des corps de nombres algébriques”, Paris (Hermann), 1913).

17. K. Weierstrass, Mathematische Werke, 7 volumes, Berlin (Mayer und Muller), 1894–1927.

18. K. HENSEL: (a) Über eine neue Begriindung der Theorie der algebraischen Zahlen, Jahresber. der D. M. V., 6 (1899), pp. 83–88; (b) Ueber die Fundamentalgleichung und die ausserwesentlichen Diskriminantentheiler eines algebraischen Korpers, Gött. Nachr., (1897), pp. 254–260; (c) Neue Grundlagen der Arithmetik, Crelle’s Journal, 127 (1902), pp. 51–84; (d) Über die arithmetische Eigenschaften der algebraischen und transcendenten Zahlen, Jahresber. der D. M. V., 14 (1905), pp. 545–558; (e) Ueber die arithmetischen Eigenschaften der Zahlen, Jahresber. der D. M. V., 16 (1907), pp. 299–319, 388–393, 474–496; (f) Theorie der algebraischen Zahlen, Leipzig (Teubner), 1908.

19. E. LASKER, Zur Theorie der Moduln und Ideale, Math. Ann., 60 (1905), pp. 20–116.

20. E. STEINITZ: (a) Algebraische Theorie der Korper, Crelle’s Journal, 137 (1910), pp. 167–308; (b) Rechteckige Systeme und Moduln in algebraischen Zahlkörpern, Math. Ann. 71 (1912), pp. 328–354 and 72 (1912), pp. 297–345.

21. F. S. MACAULAY, Về sự phân giải của một hệ môđun đã cho thành các hệ nguyên sơ, bao gồm một số tính chất của các số Hilbert, Math. Ann., 74 (1913), tr. 66–121.

22. J. KÜRSCHAK, Über Limesbildung und allgemeine Körpertheorie, Crelle’s Journal, 142 (1913), pp. 211–253.

23. A. FRAENKEL, Uber die Teiler der Null und die Zerlegung von Ringen, Crelle’s Journal, 145 (1914), p p 139–176.

24. A. OSTROWSKI, Über einige Lösungen der Funktionalgleichung $\phi(x)\phi(y) = \phi(x.y)$, Acta Math., 41 (1917), pp. 271–284.

25. E. NOETHER: (a) Idealtheorie in Ringbereichen, Math. Ann., 83 (1921), pp. 24–66; (b) Abstrakter Aufbau der Idealtheorie in algebraischen Zahl- und Funktionenkörpern, Math. Ann., 96 (1927), pp. 26–61.

26. H. HASSE: (a) Ueber die Darstellbarkeit von Zahlen durch quadratischen Formen im Korper der rationalen Zahlen, Crelle’s Journal, 152 (1923), pp. 129–148; (b) Ueber die Äquivalenz quadratischer Formen im Korper der rationalen Zahlen, Crelle’s Journal, 152 (1923), pp. 205–224; (c) Kurt Hensels entscheidender Anstoss zur Entdeckung des Lokal-Global-Prinzips, Crelle’s Journal, 209 (1960), pp. 3–4.

27. H. JUNG, Algebraischen Flachen, Hannover (Helwing), 1925.

28. H. GRELL, Beziehung zwischen den Idealen verschiedener Ringe, Math. Ann., 97 (1927), pp. 490–523.

29. W. KRULL: (a) Primidealketten in allgemeine Ringbereichen, Sitz. Ber. Heidelberg Akad. Wiss., 1928; (b) Allgemeine Bewertungstheorie, Crelle’s Journal, 167 (1931), pp. 160–196; (c) Beiträge zur Arithmetik kommutativer Integritatsbereiche, III, Math. Zeitschr., 42 (1937), pp. 745–766; (d) Dimensionstheorie in Stellenringen, Crelle’s Journal, 179 (1938), pp. 204–226; (e) Idealtheorie, Berlin (Springer), 1935.

30. M. H. Stone: (a) The theory of representations for Boolean algebras, Trans. Amer. Math. Soc., 40 (1936), pp. 37–111; (b) Applications of the theory of Boolean rings to general topology, Trans. Amer. Math. Soc., 41 (1937), pp. 375–481.
31. B. L. van der Waerden, Moderne Algebra, vol. II, Berlin (Springer), 1931.
32. C. Chevalley: (a) Généralisation de la théorie du corps de classes pour les extensions infinies, J. de Math., (9), 15 (1936), pp. 359–371; (b) On the theory of local rings, Ann. of Math., 44 (1943), pp. 690–708.
33. O. Zariski: (a) The compactness of the Riemann manifold of an abstract field of algebraic functions, Bull. Amer. Math. Soc., 50 (1944), pp. 683–691 ; (b) Generalized semi-local rings, Summa Bras. Math., 1 (1946), pp. 169–195.
34. N. Jacobson, A topology for the set of primitive ideals in an arbitrary ring, Proc. Nat. Acad. Sci. U.S.A., 31 (1945), pp. 333–338.
35. I. Cohen-A. Seidenberg, Prime ideals and integral independence, Bull. Amer. Math. Soc., 52 (1946), pp. 252–261.
36. P. Samuel, La notion de multiplicité en Algèbre et en Gtomtrie algébrique, J. de Math., (9), 30 (1951), pp. 159–274.
37. A. Weil, Fibre-spaces in Algebraic Geometry (Notes by A. Wallace), Chicago Univ., 1952.
38. J. P. Serre: (a) Faisceaux algébriques cohérents, Ann. of Math., 61 (1955), pp. 197–278; (b) Géométrie algébrique et géométrie analytique, Ann. Inst. Fourier, 6 (1956), pp. 1–42.
39. A. Grothendieck, Éléments de géométrie algébrique, Publ. math. Inst. Htes Et. Scient., 1960.

Các số tham chiếu chỉ chương, tiết diện và tiểu tiết diện (hoặc bài tập) theo thứ tự đó.

1, (E một tập hợp), U . V, UV (U, V các nhóm con cộng tính), $a^0$ (a một iđêan): Các quy ước sơ bộ của Chương I
E : F : 1.2.10
$A[S^{-1}], a/s$ (A một vành, S một tập con của A, $a \in A$, s một tích của các phần tử của S): 11.2.1 $i_A^S$: 11.2.1
$S^{-1}A, A_p$ (S một tập con nhân, p một iđêan nguyên tố): 11.2.1
$M[S^{-1}], m/s, i_M^S$ (M một A-môđun, S một tập con của A, $m \in M$, s một tích của các phần tử của S): 11.2.2
$S^{-1}M, M_p$ (M một A-môđun, S một tập con nhân của A, p một iđêan nguyên tố của A): 11.2.2
$S^{-1}u, u_p$ (u một đồng cấu môđun A): 11.2.2
$r(a)$ (a một iđêan): 11.2.6
$V(M), V(f)$ (M một tập con của vành A, $f \in A$): 11.4.3
$\operatorname{Spec}(A)$: 11.4.3
$X_f$ ($f \in A, X = \operatorname{Spec}(A)$): II.4.3
$\mathfrak{g}(Y)$ (Y một tập con của $\operatorname{Spec}(A)$): 11.4.3
$ah$ (h một đồng cấu vành): 11.4.3
$\operatorname{Supp}(M)$ (M một A-môđun): 11.4.4
$A, M_f, u_f$ (A một vành, M một A-môđun, u một đồng cấu A, $f \in A$): II.5.1
$\operatorname{rg}_p(P)$ (P một môđun xạ ảnh): 11.5.3
$\operatorname{rg}(P)$ (P một môđun xạ ảnh): 11.5.3
$P(A), \operatorname{cl}(M)$ (A một vành, M một A-môđun xạ ảnh hạng 1): 11.5.4
$\mathfrak{C}, \mathfrak{C}(A)$: 11.5.7
$\det(u), \chi_u$ (u một tự đồng cấu của một môđun xạ ảnh hạng n): 11.5. Ex. 9
$A^{(d)}, M^{(d,k)}, M^{(d)}$ (A một vành phân bậc, M một A-môđun phân bậc): III.1.3
$A_{(p)}, M_{(p)}$ (A một vành phân bậc, p một iđêan nguyên tố phân bậc của A, M một A-môđun phân bậc): 111.1.4 gr_n(G), gr(G) (G một nhóm lọc): 111.2.3
gr(h) (h một đồng cấu tương thích với các phép lọc): 111.2.4
\mathbf{Z}_n (n một số nguyên > 1): 111.2.12
\hat{\mathbf{Z}}: 111.2.13
A\{X_1, \ldots, X_p\} (A một vành có tôpô tuyến tính): 111.4.2
f(b_1, \ldots, b_p) (f một chuỗi lũy thừa hình thức hạn chế): 111.4.2
f \circ g, M_f, M_f(\mathbf{X}), J_f, J_f(\mathbf{X}), \mathbf{X}, \mathbf{1}, (\mathbf{f}, \mathbf{g} các hệ chuỗi lũy thừa hình thức, \mathbf{g} không có số hạng hằng): 111.4.4
f(x) (f một hệ chuỗi lũy thừa hình thức, x một hệ các phần tử lũy linh tôpô): 111.4.5
m \times n (m một iđêan): 111.4.5
Ass_A(M), Ass(M) (M một A-môđun): IV. 1.1
Ass_f(M): IV.1. Ex. 17
A^G (A một đại số, G một nhóm tác động trên A): V.1.9
G^Z(p'), G^Z, A^Z(p'), A^Z (G một nhóm tác động trên một vành A', p' một iđêan nguyên tố của A'): V.2.2
G^T(p'), G^T, A^T(p'), A^T (A nhóm tác động trên một vành A', p' một iđêan nguyên tố của A): v.2.2
K^Z(p'), K^Z, K^T(p'), K^T (K trường các phân thức của một miền nguyên đóng toàn phần, p' một iđêan nguyên tố của bao đóng nguyên của A trong một mở rộng Galois gần của K): V.2.3
Y^p (trong đó p = (p_1, \ldots, p_m), các p_i là các số nguyên \geqslant 0): V.3.1
m(A), \kappa(A), U(A) (A một vành địa phương): VI
R, a: VI.2.1
+\infty: VI.3.1
\Gamma_A, v_A: VI.3.2
a(M) (M một tập hợp lớn): VI.3.5
h(G) (G một nhóm được sắp thứ tự toàn phần): VI.4.4
\mathcal{T}_v (v một định giá): VI.5.2
e(v'/v), e(A'/A), e(L/K): VI.8.1
f(v'/v), f(A'/A), f(L/K): VI.8.1
\varepsilon(G, H) (G một nhóm được sắp thứ tự toàn phần, H một nhóm con của G có chỉ số hữu hạn): VI.8.4
\varepsilon(v'/v) (v một định giá, v' một mở rộng của v): VI.8.4
\operatorname{mod}(x), \operatorname{mod}_K(x) (K một trường địa phương compact không rời rạc, x \in K): VI.9.1
r(G) (hạng hữu tỉ của một nhóm giao hoán): VI.10.2
d(K'/K), s(v'/v), r(v'/v) (v một định giá trên K, v' một mở rộng của v tới một mở rộng siêu việt K' của K): VI.10.3
I(A), D(A) (A một miền nguyên): VIII.1.1
a \prec b, \operatorname{div}(a), \operatorname{div}(x) (a, b các iđêan phân thức, x một phần tử của trường các phân thức): VII.1.1
\tilde{a} (a một iđêan phân thức): VII.1.1
d_1 \leq d_2 (d_1, d_2 các ước): VII.1.1 $b : a$ (a, $b$ các iđêan phân thức): VII.1.1
$J(A)$ (A một miền nguyên): VII.1.2
$P(A)$ (A một miền Krull): VII.I.3
$p^{(n)}$ ($p$ một iđêan nguyên tố chia được): VII.1.4
$v_p$ ($p$ một iđêan nguyên tố chiều cao 1 trong một miền Krull): VII.1.10
$F(A), C(A)$ (A một miền Krull): VII.1.10
$e(\mathfrak{P}/p)$ ($p \in P(A), \mathfrak{P} \in P(B), A \subset B, \mathfrak{P} \cap A = p$) VII.1.10
$i$ (đồng cấu từ $D(A)$ đến $D(B)$, hoặc từ $C(A)$ đến $C(B)$): VII.1.10
$\bar{i}$ (đồng cấu từ $C(A)$ đến $C(B)$): VII.1.10
$A, A,, \Delta(K)$ (các vành adèle hạn chế): VII.2.4
$\mathfrak{P}^*, \mathfrak{P}^*(A)$ (A một miền nguyên): VII.3.2
$M^*$ (dàn đối ngẫu của một dàn $M$): VII.4.2
$l_p(T), \chi(T)$ (T một A-môđun xoắn, $p$ một iđêan nguyên tố có chiều cao 1): VII.4.5
$F(A), T(A), cl(M)$: VII.4.5
$\chi(M, M')$ (M, $M'$ các dàn): VII.4.6
$c(d)$ (da divisor): VII.4.7
$c(M), r(M), \gamma(M)$ (M một dàn): VII.4.7
$\mathfrak{P}|p, e_{\mathfrak{P}/p}, f_{\mathfrak{P}/p}, f(\mathfrak{P}/p)$ (A $\subset$ B các miền Krull sao cho B là một A-đại số hữu hạn $P \in P(A), \mathfrak{P} \in P(B), \mathfrak{P} \cap A = p$): VII.4.8
$N_{B/A}, N, i_{B/A}$: VII.4.8

Số tham chiếu chỉ chương, tiết và tiểu tiết (hoặc bài tập) theo thứ tự đó.

Adèle, hạn chế, chính hạn chế adtle : VII.2.4
lọc m-adic: 111.2.1
— tôpô: 111.2.5
số nguyên n-adic: 111.2.12
Đại số, Azumaya: II.1.7
— sinh hữu hạn : 111.1.1
— nguyên, hữu hạn, trên một vành: V. 1.1
Bao đóng đại số của một trường trong một đại số : V. 1.2
Trường đóng đại số trong một đại số: V. 1.2
— phụ thuộc, độc lập, các phần tử: 111.1.1
— tự do, liên kết, họ: 111.1.1
Hầu hết mọi $p \in P(A)$ (tính chất đúng với) : VII.4.3
— tự đồng cấu lũy linh: IV. 1.4
Định lý xấp xỉ cho các giá trị tuyệt đối : VI.7.3
— định lý cho các định giá: VI.7.2
Bổ đề Artin-Rees: 111.3.1
Liên kết (môđun lọc) với một môđun phân bậc: 111.2.1
— (vành lọc) với một vành phân bậc: 111.2.1
— (lọc) với một phép phân bậc: III.2.1
— (đồng cấu phân bậc) với một đồng cấu tương thích với các lọc: 111.2.4
— (môđun phân bậc) với một môđun lọc: 111.2.3
— (vành phân bậc) với một vành lọc: 111.2.3
— (ánh xạ) với một đồng cấu vành: 11.4.3
— (iđêan nguyên tố) với một môđun: IV. 1.1
— vành, điểm, định giá: VI.3.3

Phân tích chính tắc của một điểm : VI.2.3
— phân tích thành nhân tử chính tắc của một định giá: VI.3.2
— đồng cấu chính tắc của nhóm phân rã của một iđêan nguyên tố $\mathfrak{p}'$ của $\mathbf{A}'$ vào nhóm tự đẳng cấu của $\mathbf{A}'/\mathfrak{p}'$: V.2.2
Lớp, ước, gắn với một môđun hữu hạn sinh : VII.4.7
Các lớp, ước (đơn vị giao hoán của): VII.1.2
Bao đóng, đại số, của một trường trong một đại số : V.1.2
— nguyên, của một miền nguyên : V.1.2
— nguyên, của một vành trong một đại số: V.1.2
Biểu đồ giao hoán: I.1.2
Tương thích (lọc) với một cấu trúc vành, cấu trúc môđun: 111.2.1
— (đồng cấu) với các lọc: 111.2.4
Hệ đầy đủ các mở rộng của một định giá: VI.8.2
Miền đóng nguyên hoàn toàn : V.1.4
Thành phần, bất khả quy (của một không gian tôpô) : 11.4.1
Các điều kiện của Hensel: 111.4.5
Nhạc trưởng của một môđun con : V.1.5
Nội dung của một đa thức trên một miền giả-Bézout: VII.1.Ex.23
— của một môđun xoắn: VII.4.5
Tiêu chuẩn bất khả quy Eisenstein: VII.3.Ex.20

Phân tích, chính tắc, của một điểm : VI.2.3
— đầy đủ, của một iđêan nguyên tố: V.2.2
— trường của một iđêan nguyên tố: V.2.2
— nhóm, vành, của một iđêan nguyên tố: V.2.2
— của một iđêan trong một miền Dedekind thành các nhân tử nguyên tố: VII.2.3
— nguyên sơ: IV.2.2 và Ex.20
— nguyên sơ rút gọn: IV.2.3 và Ex.20
Lọc giảm: 111.2.1
Miền Dedekind: VII.2.1
Được xác định (tôpô) bởi một lọc: 111.2.5
Iđêan xác định: III.3.2
Bậc, lớp thặng dư, của một định giá trên một định giá khác: VI.8.1
Phụ thuộc, nguyên (phương trình của) : V.1.1
Dẫn xuất (lọc môđun) từ một lọc vành: 111.2.1
Biểu đồ, giao hoán: I.1.2
— rắn : I.1.4
Lọc rời rạc: 111.2.1
— định giá rời rạc: VI.3.6
Đa thức đặc biệt : VII.3.8
Ước, ước chính: VII.1.1
— định thức: VII.4.Ex.11
— hữu hạn sinh: VII.1.Ex.11

Iđêan phân thức chia hết : VII. 1.1
Các ước, tương đương: VII. 1.2
Miền Bézout (hoặc Bézout) : VII.1.Ex.20
— đóng nguyên hoàn toàn : V. 1.4
— Dedekind: VII.2.1
— phân tích nhân tử: VII.3.1
— đóng nguyên : V. 1.2
— đóng nguyên, có đặc trưng hữu hạn: VII.1.Ex.25, 26 và 28
— Noether nguyên: V.3.Ex.6
— Krull: VII.1.3
— nguyên địa phương, chiều 1 : VI.4.Ex.7
— Prüfer (hoặc Prüfer): VII.2.Ex.12
— giả-Bézout: VII. 1.Ex.21
— giả-chính: VII. 1.Ex.21
— giả-Prüfer: VII.2.Ex.19
— đóng nguyên chính quy: VII. 1.Ex.30
Trội (vành địa phương) một vành địa phương: VI. 1.1
Đối ngẫu, xuyến đại số, của một môđun: VI.5.Ex.9
— dàn: VII.4.2
— xuyến tôpô: VI.5.Ex.10

Phần tử, lũy linh tôpô: 111.4.3
Các phần tử, phụ thuộc đại số, độc lập: III.1.]
— nguyên tố cùng nhau mạnh: 111.4.1
Tự đồng cấu, gần lũy linh: IV. 1.4
Các ước tương đương: VII. 1.2
— các định giá tương đương: VI.3.2
Iđêan phân bậc cốt yếu: III.1.4
— các định giá cốt yếu: VII.1.4
Trường có thứ tự Euclid: VI.2.Ex.4
Lọc đầy đủ: III.2.1
Mở rộng gần Galois: V.2.2

Nhân tử, bất biến: VII.4.Ex. 11 và 14
Miền phân tích nhân tử: VII.3.1
Phân tích thành nhân tử, chính tắc, của một định giá : VI.3.2
Môđun phẳng trung thành: 1.3.1
Họ, tự do đại số, liên kết : 111.1.1
— tự do hình thức: 111.2.9
Trường, đóng đại số trong một đại số : V. 1.2
— phân rã: V.2.3
— xạ ảnh: VI.2.1
— thặng dư, của một vành địa phương: II.3.1

Trường, thặng dư, của một điểm: VI.2.3
— thặng dư, của một định giá: VI.3.2
— giá trị, của một điểm: VI.2.2
Nhóm, vành, môđun lọc: 111.2.1
Lọc, m-adic: 111.2.1
— liên kết với một phép phân bậc: 111.2.1
— tương thích với một cấu trúc vành, cấu trúc môđun: 111.2.1
— rời rạc: 111.2.5
— m-tốt: 111.3.1
— tăng, giảm, tách, đầy đủ: 111.2.1
— cảm sinh, tích, thương: III.2.1
— môđun, dẫn xuất từ một lọc vành: III.2.1
— tầm thường: 111.2
Đại số hữu hạn trên một vành : V. 1.1
— (điểm) tại một phần tử: VI.2.2
Đại số hữu hạn sinh: 111.1.1
Hữu hạn trình bày: 1.2.8
Phẳng đối với M, M-phẳng (môđun): 1.2.2
— môđun: 1.2.3
Họ tự do hình thức: 111.2.9
Iđêan phân thức: VII.1.1
Hàm, cấp: 111.2.2

Số nguyên Gaussian: V. 1.1
Bổ đề Gauss: VII.3.5
Định lý Gelfand-Mazur: V1.6.4.
Sinh bởi một tập con (tập con nhân): 11.2.1
Các phần tử sinh, hệ hình thức của: 111.2.9
Lọc m-tốt: 111.3.1
Nhóm, phân rã: V.2.2
— lọc: 111.2.1
— quán tính: V.2.2
— của các lớp môđun khả nghịch: 11.5.7
— của các toán tử, hữu hạn địa phương : V. 1.9
— tác động trên một vành: V. 1.9
— cấp, của một định giá: VI.3.2
— có thứ tự, cấp $n$, cấp $+\infty$: VI.4.4

Cao độ $\leq 1$ (của iđêan nguyên tố) : VII.1.6
— của một nhóm có thứ tự, của một định giá : VI.4.4
Vành Hensel : III.4.Ex.3
Các điều kiện của Hensel: 111.4.5
— Định lý: 111.4.3

Đồng cấu, chính tắc, của nhóm phân tích của iđêan nguyên tố $p'$
— từ $A'$ đến nhóm tự đẳng cấu của $A'/p'$: V.2.2
— tương thích với các phép lọc: III.2.4
— phân bậc, liên kết với một đồng cấu tương thích với các phép lọc: 111.2.4
— địa phương: 11.3.1
— giả đơn ánh, giả toàn ánh, giả không, giả song ánh: VII.4.4

Iđêan, định thức: VII.4.Ex.10 và 14
— phân bậc cốt yếu: III.1.4
— nguyên tố đắm: IV.2.3
— nguyên, iđêan phân thức: VII.1.1
— phân thức khả nghịch: 11.5.7
— nằm trên một iđêan: V.2.1
— nguyên tố cực tiểu: 11.2.6
— của một nơi: VI.2.3
— của một định giá: VI.3.2
— nguyên tố: II.1.1
— nguyên tố, liên kết với một môđun: IV.1.1
— nguyên tố, phân tích hoàn toàn: V.2.2
— nguyên tố, có chiều cao $\leq 1$: VII.1.6
— nguyên sơ, p-nguyên sơ: IV.2.1 và Ex.20
— không phân nhánh: V.2.Ex.18 và 19
Môđun Hausdorff theo iđêan: 111.5.1
Các iđêan, nguyên tố cùng nhau: 11.1.2
Đồng nhất thức Cauchy: VII.3.Ex.18
Iđêan nguyên tố đắm: IV.2.3
Định giá không đúng: VI.3.1
Phép lọc tăng: III.2.1
Các vành định giá độc lập: VI.7.2
— các định giá: VI.7.2
Chỉ số ban đầu của một nhóm con của một nhóm có thứ tự, chỉ số phân nhánh ban đầu của một định giá: VI.8.4
— phân nhánh: VI.8.1
Phép lọc cảm sinh: 111.2.1
Quy nạp Noether (nguyên lý của): II.4.2
Trường quán tính: V.2.3
— vành, nhóm: V.2.2
Chỉ số phân nhánh ban đầu: VI.8.4
Số nguyên, đại số: V.1.1
— Gaussian: V.1.1
— trên một vành: V.1.1

Iđêan phân thức khả nghịch: 11.5.7
— môđun con khả nghịch: 11.5.6
Thành phần bất khả quy: 11.4.1
— tập hợp bất khả quy: 11.4.1
— không gian bất khả quy: 11.4.1
Nhóm con cô lập: VI.4.2

Vành Jacobson: V.3.4

Môđun phân bậc, liên kết với một môđun được lọc: 111.2.3
— Hausdorff theo iđêan: 111.5.1
— phân thức được xác định bởi một tập con của một vành: 11.2.2
— xạ ảnh, có hạng $n$: 11.5.3
— giả liên hợp: I.2.Ex.11
— giả không: VII.4.4
Nửa nhóm, lớp ước: VII.1.2
Cấu xạ đối với các luật hợp thành không được xác định khắp nơi: VI.2.1
Tập con nhân: 11.2.1

Căn nil của một vành: 11.2.6
Không gian Noether: 11.4.2
Môđun con không suy biến: 11.5.5
Bổ đề chuẩn hóa: V.3.1
Định giá rời rạc có chuẩn: VI.3.6
Nullstellensatz: V.3.3

Nhóm cấp của một định giá: VI.3.2
— của một phần tử đối với một định giá: VI.3.2
— rút gọn, của một chuỗi lũy thừa hình thức: VII.3.8
Cặp có thứ tự của các vành với tính chất mở rộng tuyến tính: 1.3.7
Định lý Ostrowski: VI.6.4

Nơi, hữu hạn tại $x$: VI.2.2
— của một trường: VI.2.2
— tầm thường: VI.2.2
Điểm tổng quát của một không gian bất khả quy: II.4.Ex.2
Đa giác Newton: VI.4.Ex.11
Đa thức, đặc biệt: VII.3.8
— cực tiểu: V.1.3
Định lý chuẩn bị: VII.3.8
Biểu diễn của một môđun, — hữu hạn: 1.2.8
n-biểu diễn: I.2.Ex.6
Được biểu diễn, hữu hạn (môđun): 1.2.8
Phân tích nguyên sơ: IV.2.2 và Ex.20
— p-nguyên sơ, iđêan, môđun con: IV.2.1 và Ex.20
Iđêan nguyên tố: II.1.1
— phổ nguyên tố: 11.4.3
Ước chính: VII.1.1
— adèle hạn chế: VII.2.4
Nguyên lý quy nạp Noether: 11.4.2
Phép lọc tích: III.2.1
Trường xạ ảnh: VI.2.1

Giả đơn ánh, giả toàn ánh, giả không, giả song ánh (đồng cấu): VII.4.4
Giả đẳng cấu: VII.4.4
Môđun giả không: VII.4.4

Mở rộng giả Galois: V.2.2
Phép lọc thương: III.2.1

Căn của một iđêan: 11.2.6
Hạng tại p của một môđun xạ ảnh: 11.5.3
— của một môđun xạ ảnh: 11.5.3
— hữu tỉ, của một nhóm giao hoán: VI.10.2
— thặng dư: VI.8.5
Hạng hữu tỉ của một nhóm giao hoán: VI.10.2
Cấp rút gọn: VII.3.8
— phân tích nguyên sơ rút gọn: IV.2.3
— vành rút gọn: 11.2.6
— chuỗi rút gọn: VII.3.8
Dàn phản xạ: VII.4.2
Các vành địa phương liên quan: VI.1.Ex.1
Các iđêan nguyên tố cùng nhau: II.1.2
Hệ đại diện của các phần tử cực biên: VII.3.3
Bậc lớp thặng dư của một định giá: VI.8.1
— trường thặng dư: 11.3.1
— hạng thặng dư của một định giá: VI.8.5
Phân giải, tự do hữu hạn, của một môđun: VII.4.7
Adèle hạn chế: VIII.2.4
— chuỗi lũy thừa hình thức hạn chế: 111.4.2
Vành, phẳng tuyệt đối: I.2.Ex.17
— liên hợp (trái, phải): I.2.Ex.17
— phân tích: V.2.2
— được lọc: 111.2.1
— được lọc, liên kết với một vành phân bậc: 111.2.1
— phân bậc, liên kết với một vành được lọc: 111.2.3
— quán tính: V.2.2
— đóng nguyên trong một đại số: V.1.2
— Jacobson: V.3.4
— có tôpô tuyến tính: 111.4.2
— địa phương: 11.3.1
— địa phương, trội một vành địa phương: VI.1.1
— địa phương của A tại p, của p (p là một iđêan nguyên tố): 11.3.1
— của một nơi: VI.2.3
— của một định giá: VI.3.2

Vành phân thức được xác định bởi một tập con của một vành: 11.2.1
— rút gọn: 11.2.6
— nửa địa phương: 11.3.5
— toàn bộ, của phân thức: 11.2.1
— không phân nhánh: V.2.Ex.19
— định giá, vành định giá của một trường: VI. 1.1
— Zariski: 111.3.3
Các vành, định giá độc lập: VI.7.2

Bão hòa của một môđun con đối với một tập con nhân (đối với một iđêan nguyên tố): 11.2.4
Vành nửa địa phương: 11.3.5
Chuỗi, rút gọn: VII.3.8
— chuỗi lũy thừa hình thức hạn chế: 111.4.2
Tập hợp, bất khả quy: 11.4.1
— lớn, trong một nhóm được sắp thứ tự toàn phần: VI.3.5
Không gian, bất khả quy: 11.4.1
— Noether: 11.4.2
Tôpô đặc biệt: 11.4.3
Phổ, nguyên tố, của một vành: 11.4.3
Môđun Laskerian mạnh: IV.2.Ex.28
— môđun con nguyên sơ: IV.2.Ex.27
— các phần tử nguyên tố cùng nhau: 111.4.1
Nhóm con, cô lập, của một nhóm có thứ tự: VI.4.2
Môđun con, khả nghịch: II.5.6
— không suy biến: 11.5.5
— nguyên sơ, p-nguyên sơ: IV.2.1
Tập con, nhân, của một vành: 11.2.1
— nhân, sinh bởi một tập con: 11.2.1
— nhân bão hòa: II.2.Ex.1
Giá đỡ của một môđun: 11.4.4
Hệ, đầy đủ, của các mở rộng của một định giá: VI.8.2
— hình thức, của các phần tử sinh: 111.2.9
— đại diện, của các phần tử cực biên: VII.3.3

Định lý, xấp xỉ, đối với các giá trị tuyệt đối: VI.7.3
— xấp xỉ, đối với các định giá: VI.7.2
— Gelfand-Mazur: VI.6.4
— Hensel: III.4.3
— các không điểm của Hilbert (Nullstellensatz): V.3.3
— của Krull: 111.3.1
— Krull-Akizuki: VII.3.5
— của Ostrowski: VI.6.3

Định lý, chuẩn bị: VII.3.8
— của Stickelberger: VI.8.Ex.18
— Chính của Zariski: V.3.Ex.7
Phần tử lũy linh tôpô: 111.4.3
Tôpô xác định bởi một lọc: 111.2.5
— phổ: 11.4.3
— Zariski: 11.4.3
Bộ chuyển: 1.2.10
Lọc tầm thường: 111.2.1
— địa điểm: VI.2.2

Giá trị tuyệt đối ultramêtric: VI.6.1
Phần tử đồng nhất hóa của một định giá rời rạc: VI.3.6
Định giá không phân nhánh: VI.8.1

Định giá, định giá của một phần tử $x$: VI.3.1 và 2
— rời rạc, định giá rời rạc chuẩn hóa: VI.3.6
— cốt yếu: VII.1.4 và Ex.26
— không đúng: VI.3.1
— vành: VI.1.1
— không phân nhánh: VI.8.1
Các định giá, tương đương: VI.3.2
— độc lập: VI.7.2
Trường giá trị của một địa điểm: VI.2.2
— giá trị tuyệt đối ultramêtric: VI.6.1

Liên kết yếu (iđêan nguyên tố) với một môđun: IV.1.Ex.17

Zariski, vành: 111.3.3
— tôpô: 11.4.3 vành nửa địa phương
    ↑
vành địa phương
    ↑
---------------------------
miền nguyên đóng nguyên ↔ vành định giá
    ↑
miền nguyên đóng nguyên hoàn toàn ↔ vành định giá chiều cao 1
    ↑
miền Krull
    ↑
nguyên
vành Noether

Trong trường hợp các vành Noether bảng này rút gọn thành bảng sau:

miền nguyên đóng nguyên        vành nửa địa phương
    ↑                        ↑
miền Dedekind   miền phân tích thành nhân tử   vành địa phương
    ↑                        ↑
miền iđêan chính ↔ vành định giá rời rạc

Trong bảng này và các bảng sau, mỗi hàng tương ứng với một tính chất mà một vành có thể có và mỗi cột với một vành dẫn xuất từ vành $\mathbf{A}$ ($p$ ký hiệu một iđêan nguyên tố của $\mathbf{A}$, $S$ một tập con nhân của $\mathbf{A}$ không chứa 0 và $\mathbf{A}'$ là bao đóng nguyên của $\mathbf{A}$ trong một mở rộng đại số hữu hạn $L$ của trường phân thức $K$ của $\mathbf{A}$). Giả sử vành $\mathbf{A}$ có tính chất được chỉ ra trong hàng; từ "yes" (tương ứng "no", "?") ở giao điểm của hàng này và một cột có nghĩa là đúng (tương ứng sai, vẫn chưa biết) rằng mọi vành được xây dựng từ $\mathbf{A}$ bằng quá trình được chỉ ra bởi cột có tính chất được chỉ ra trong hàng.

Các tham chiếu chỉ nơi trong Quyển này hoặc Quyển Đại số mà kết quả đang xét được chứng minh, và tương tự đối với hai công trình sau đây khi liên quan đến các kết quả không được nêu trong văn bản hoặc trong các bài tập:

(1) A. Grothendieck, Éléments de géométrie algébrique, Chương IV (Publ. Inst. Htes etudes Scient., nos. 20 và 24, 1964).
(2) M. Nagata, Local rings, Interscience (New York), 1962.

<table>
  <tr>
    <th></th>
    <th>A/p</th>
    <th>S^{-1}\mathbf{A}</th>
    <th>\mathbf{A}[X]</th>
    <th>\mathbf{A}[[X]]</th>
    <th>\mathbf{A}'</th>
  </tr>
  <tr>
    <td>A là một miền iđêan chính</td>
    <td>CÓ</td>
    <td>CÓ</td>
    <td>KHÔNG<br><i>Alg. VII,</i><br>§ 1, Ex. 1</td>
    <td>KHÔNG</td>
    <td>KHÔNG<br><i>Alg. VII,</i><br>1, Ex. 12</td>
  </tr>
  <tr>
    <td>A là một miền Dedekind</td>
    <td>CÓ</td>
    <td>CÓ</td>
    <td>KHÔNG<br><i>Alg. VII,</i><br>§ 1, Ex. 1</td>
    <td>KHÔNG<br>VII, § 1,<br>Ex. 9</td>
    <td>CÓ<br>VII, § 2,<br>Hệ quả 2 của Mệnh đề 9)</td>
  </tr>
</table> <table>
  <tr>
    <th></th>
    <th>A/p</th>
    <th>S^{-1}A</th>
    <th>A[X]</th>
    <th>A[[X]]</th>
    <th>A'</th>
  </tr>
  <tr>
    <td>A là một miền phân tích thành nhân tử</td>
    <td>KHÔNG<br>'§ 1, Ex. !</td>
    <td><b>CÓ</b><br>VII, § 3, Mệnh đề 3</td>
    <td><b>CÓ</b><br>VII, § 3, Định lý 2</td>
    <td>KHÔNG<br>VII, § 3, Ex. 9</td>
    <td><b>KHÔNG</b><br><i>Alg.</i> VII, § 1, Ex. 12</td>
  </tr>
  <tr>
    <td>A là một miền nguyên đóng nguyên Noether</td>
    <td>KHÔNG<br>'§ 1, Ex. !</td>
    <td><b>CÓ</b><br>'§ 1, Hệ quả của Mệnh đề 16</td>
    <td><b>CÓ</b><br>'§ 1, Hệ quả 1 của Mệnh đề 13</td>
    <td><b>CÓ</b><br>V, § 1, Mệnh đề 14</td>
    <td>?</td>
  </tr>
  <tr>
    <td>A là một trường hoặc một vành định giá rời rạc</td>
    <td><b>CÓ</b><br>VI, § 3, no. 6</td>
    <td><b>CÓ</b><br>VI, § 3, no. 6</td>
    <td><b>KHÔNG</b><br><i>Alg.</i> VII, § 1, Ex. 1</td>
    <td>KHÔNG<br>VII, § 1, Ex. 9</td>
    <td><b>KHÔNG</b><br>V, § 2, Ex. 6</td>
  </tr>
  <tr>
    <td>A là một trường hoặc một vành định giá chiều cao 1</td>
    <td><b>CÓ</b><br>VI, § 4</td>
    <td><b>CÓ</b><br>VI, § 4, Mệnh đề 1</td>
    <td><b>KHÔNG</b><br><i>Alg.</i> VII, § 1, Ex. 1</td>
    <td>KHÔNG<br>VII, § 1, Ex. 9</td>
    <td><b>KHÔNG</b><br>V, § 2, Ex. 6</td>
  </tr>
  <tr>
    <td>A là một vành định giá</td>
    <td><b>CÓ</b><br>VI, § 1, Định lý 1</td>
    <td><b>CÓ</b><br>VI, § 1, Định lý 1</td>
    <td><b>KHÔNG</b><br><i>Alg.</i> VII, § 1, Ex. 1</td>
    <td>KHÔNG<br>VII, § 1, Ex. 9</td>
    <td><b>KHÔNG</b><br>V, § 2, Ex. 6</td>
  </tr>
  <tr>
    <td>A là một vành định giá đầy đủ</td>
    <td><b>CÓ</b><br>VI, § 5, Mệnh đề 1</td>
    <td><b>CÓ</b><br>VI, § 7, Mệnh đề 3</td>
    <td><b>KHÔNG</b><br><i>Alg.</i> VII, § 1, Ex. 1</td>
    <td>KHÔNG<br>VII, § 1, Ex. 9</td>
    <td><b>KHÔNG</b><br>V, § 2, Ex. 6</td>
  </tr>
  <tr>
    <td>A là một miền Krull</td>
    <td>KHÔNG<br>V, § 1, Ex. 9</td>
    <td><b>CÓ</b><br>VII, § 1, Mệnh đề 6</td>
    <td><b>CÓ</b><br>VII, § 1, Mệnh đề 13</td>
    <td><b>CÓ</b><br>VII, § 1, Ex. 9</td>
    <td><b>CÓ</b><br>VII, § 1, Mệnh đề 12</td>
  </tr>
</table>

Trong bảng này $a$ ký hiệu một iđêan của $\mathbf{A}$ khác với $\mathbf{A}$, $S$ một tập con nhân của $\mathbf{A}$ và $\mathbf{A}'$ là bao đóng nguyên của $\mathbf{A}$ được giả sử là một miền nguyên.

<table>
  <tr>
    <th></th>
    <th>A/a</th>
    <th>S^{-1}A</th>
    <th>A[X]</th>
    <th>A[[X]]</th>
    <th>A'</th>
  </tr>
  <tr>
    <td>A địa phương</td>
    <td>CÓ</td>
    <td>KHÔNG<br>II, §2, Mệnh đề 11</td>
    <td>KHÔNG</td>
    <td>CÓ<br>Alg. IV, §5, Mệnh đề 4</td>
    <td>KHÔNG<br>V, 42, Bài tập 20</td>
  </tr>
  <tr>
    <td>A địa phương và đầy đủ</td>
    <td>?<br>CÓ nếu $\Lambda$ là Noether (III, §3, Mệnh đề 6)</td>
    <td>KHÔNG<br>II, §2, Mệnh đề 11</td>
    <td>KHÔNG</td>
    <td>CÓ<br>III, §2, Mệnh đề 6</td>
    <td>?<br>CÓ nếu $\Lambda$ là Noether (1)</td>
  </tr>
  <tr>
    <td>A nửa địa phương</td>
    <td>CÓ</td>
    <td>KHÔNG<br>IV, §2, Bài tập 23(c)</td>
    <td>KHÔNG</td>
    <td>CÓ<br>Alg. IV, §5, Mệnh đề 4</td>
    <td>CÓ nếu $\mathbf{A}$ là Noether<br>V, §2, Bài tập 7</td>
  </tr>
  <tr>
    <td>A nửa địa phương và đầy đủ</td>
    <td>?<br>CÓ nếu $\mathbf{A}$ là Noether (III, §3, Mệnh đề 6)</td>
    <td>KHÔNG<br>IV, 42, Bài tập 23(c)</td>
    <td>KHÔNG</td>
    <td>CÓ<br>III, §2, Mệnh đề 6</td>
    <td>—</td>
  </tr>
  <tr>
    <td>A Noether</td>
    <td>CÓ<br>Alg. VIII, §2, Mệnh đề 6</td>
    <td>CÓ<br>II, §2, Hệ quả cho Mệnh đề 10</td>
    <td>CÓ<br>III, §2, Hệ quả 1 cho Định lý 2</td>
    <td>CÓ<br>III, §2, Hệ quả 6 cho Định lý 2</td>
    <td>KHÔNG<br>V, §1, Bài tập 21<br>CÓ nếu $\mathbf{A}$ là đầy đủ địa phương (1)<br>$\mathbf{A}'$ luôn là miền Krull (2)</td>
  </tr>
</table> (a) Cho $\mathbf{A}$ là một vành và $m$ là một iđêan của $\mathbf{A}$ phân biệt với $\mathbf{A}$. Trang bị cho $\mathbf{A}$ tôpô $m$-adic và ký hiệu $\hat{\mathbf{A}}$ là phần bù Hausdorff của nó.

$$
\begin{array}{ll}
\mathbf{A} \text{ Hausdorff} & \text{CÓ} \\
\mathbf{A} \text{ Noether} & \text{CÓ (III, § 3, Mệnh đề 8)} \\
\mathbf{A} \text{ địa phương} & \text{CÓ (III, § 2, Mệnh đề 19)} \\
\mathbf{A} \text{ nửa địa phương} & \text{CÓ (III, § 2, Hệ quả cho Mệnh đề 19)} \\
\mathbf{A} \text{ một vành Zariski} & \text{CÓ (III, § 3, Mệnh đề 8)}
\end{array}
$$

(b) Bây giờ giả sử rằng $\mathbf{A}$ là địa phương và Noether và $m$ là iđêan cực đại của nó.

$$
\begin{array}{ll}
\mathbf{A} \text{ một miền nguyên} & \text{KHÔNG (III, § 3, Bài tập 15 (b))} \\
\mathbf{A} \text{ một miền đóng nguyên} & \text{KHÔNG (2)} \\
& \text{CÓ đối với các vành xuất sắc (1)} \\
\mathbf{A} \text{ một vành định giá rời rạc} & \text{CÓ (VI, § 5, Mệnh đề 5)} \\
\mathbf{A} \text{ giảm} & \text{KHÔNG (2)} \\
& \text{CÓ đối với các vành xuất sắc (1)}
\end{array}
$$
