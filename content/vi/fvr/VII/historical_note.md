---
book: fvr
book_title: Functions of a Real Variable
chapter: VII
chapter_title: THE GAMMA FUNCTION
section: 0
section_title: Historical Note
kind: historical
lang: vi
source: fvr-i-vii
pdf_pages: 0344-0353
extraction: ocr
statements: 0
exercises: 0
content_sha256: e5b995bfcbdfa783a08291eabce47a1122a017177fec88975427eb0b65644834
translated_from: content/en/fvr/VII/historical_note.md
source_content_sha256: 1041088601c93e87563d0f075a725ecae387676a67a10cbf4e0c2ebe1dc7757d
translation_model: gpt-5.4
translation_run: translate-vi-289adf01
glossary_version: 34
glossary_terms_sha256: d1863aa8bc0d32befd1f35cfd0a459f3d6501068fae8d4a266085d43415f7472
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

# GHI CHÚ LỊCH SỬ

(Xin lưu ý: các chữ số La Mã chỉ thư mục tài liệu tham khảo ở cuối ghi chú này.)

Ý tưởng “nội suy” một dãy $(u_n)$ bằng các giá trị của một tích phân phụ thuộc vào một tham số thực $\lambda$ và bằng $u_n$ khi $\lambda = n$, có từ Wallis (III, p. 55). Chính ý tưởng này là điều chủ yếu đã dẫn dắt Euler khi, vào năm 1730 ((I), v. XIV, p. 1-24), ông bắt tay vào việc nội suy dãy các giai thừa. Trước hết ông nhận xét rằng $n!$ bằng tích vô hạn
$$
\prod_{k=1}^{\infty} \left( \frac{k+1}{k} \right)^n \frac{k}{k+n},
$$
mà tích này được xác định với mọi giá trị của $n$ (là số nguyên hay không), và đặc biệt, với giá trị $n = \frac{1}{2}$ thì nó nhận giá trị $\frac{1}{2} \sqrt{\pi}$ theo công thức của Wallis. Sự tương tự giữa kết quả này và kết quả của Wallis đã dẫn ông đến chỗ xét lại tích phân
$$
\int_0^1 x^e (1-x)^n dx
$$
$(n$ nguyên, $e$ tùy ý) mà Wallis đã xét trước đó. Euler tính được giá trị
$$
\frac{n!}{(e+1)(e+2)\ldots(e+n+1)}
$$
của nó, bằng cách dùng khai triển nhị thức; khi đó một phép thay đổi biến cho ông thấy rằng $n!$ là giới hạn, khi $z$ tiến tới 0, của tích phân
$$
\int_0^1 \left( \frac{1-x^z}{z} \right)^n dx,
$$
do đó có “tích phân Euler thứ hai”
$$
n! = \int_0^1 \left( \log \frac{1}{x} \right)^n dx;
$$
bằng cùng phương pháp đó, và dùng công thức của Wallis, ông thu được công thức
$$
\int_0^1 \sqrt{\log 1/x} dx = \frac{1}{2} \sqrt{\pi}.
$$
Trong các công trình về sau của mình Euler thường quay trở lại các tích phân này; như vậy ông đã phát hiện quan hệ về các phần bù ((I), t. XV, p 82 and t. XVII, p. 342), công thức $\mathbf{B}(p, q) = \Gamma(p)\Gamma(q)/\Gamma(p+q)$ ((I), t. XVII, p. 355), và trường hợp riêng của công thức Legendre-Gauss tương ứng với $x = 1$ ((I), t. XIX, p. 483); tất cả những điều đó dĩ nhiên là không bận tâm đến các vấn đề hội tụ.

Gauss đã theo đuổi việc nghiên cứu hàm $\Gamma$ gắn với nghiên cứu của ông về hàm siêu bội, mà hàm $\Gamma$ là một trường hợp giới hạn (II); chính trong quá trình nghiên cứu này ông đã thu được công thức phép nhân tổng quát (đã được Legendre lưu ý sớm hơn một chút cho $p = 2$). Các công trình về sau về $\Gamma$ chủ yếu nhằm mở rộng hàm này sang miền phức. Chỉ gần đây người ta mới nhận ra rằng tính chất lồi lôgarit đặc trưng cho $\Gamma(x)$ (trong miền thực), sai khác bởi một thừa số hằng, giữa các nghiệm của phương trình hàm $f(x + 1) = x\, f(x)$ (III); và Artin đã chỉ ra (IV) cách có thể liên kết mọi kết quả cổ điển về $\Gamma(x)$ một cách đơn giản với tính chất này. Chúng tôi đã theo sát khá chặt chẽ cách trình bày của ông.

(I) L. Euler, Opera omnia, Leipzig-Berlin (Teubner): t. XIV (1924), t. XV (1927), t. XVII (1915) và t. XIX (1932).
(II) C.F. Gauss, Werke, t. III, Göttingen, 1866.
(III) H. Bohr und J. Mollerup, Laerebog i matematisk Analyse, t. III, Kopenhagen, 1922, p. 149-164.
(IV) E. Artin, Einführung in die Theorie der Gammafunktion, Leipzig (Teubner), 1931.

Df(x_0): 5
f'(x_0): 5
f'_d(x_0): 6
f'_g(x_0): 6
Df: 7
df/dx: 7
f'_d: 7
f'_g: 7
D^n f: 23
f^{(n)}: 23
\int_{x_0}^x f: 61
\int_{x_0}^x f(t)\,dt: 61
\int_{x_0}^x f: 61
\int_{x_0}^x f(t)dt: 61
h(t)|_{x_0}^x: 62
\int_a^{(n)} f: 66
\int_1^a f(t)\,dt: 69
e: 97
\exp x: 97
\log x\ (x\ \text{thực}\ > 0): 97
\pi: 99
\operatorname{Arc}\cos x: 100
\operatorname{Arc}\sin x: 100
\operatorname{Arc}\tan x: 100
\cos x: 100
\cot x: 100
\csc x: 100
\sec x: 100
\sin x: 100
\tan x: 100
e^z: 103
\exp z: 103
\cos z: 107 cot z: 107
log z: 105
sin z: 107
tan z: 107
cosh x: 108
sinh x: 108
tanh x: 108
Arg cosh x: 109
Arg sinh x: 109
Arg tanh: 110
$$
\binom{m}{n}
$$: 114
$e^A$: 198
exp A: 198
$\mathcal{H}(\mathfrak{F}, V)$: 221
R_\infty: 221
$\mathcal{H}_\infty(\mathfrak{F}, V)$: 222
f_1 \preceq f_2: 223
f_2 \succeq f_1: 223
f \preceq g: 223
g \succeq f: 223
f + g: 223
fg: 223
f\lambda: 223
\|f\|: 223
f \asymp g: 224
f_1 \ll f_2: 225
f_2 \gg f_1: 225
f \ll g: 225
g \gg f: 225
f \sim g: 226
O(f), O_k(f), o(f), o_k(f): 230
l_0(x), l_n(x): 240
\mathcal{K}(y) (\mathcal{K} một trường Hardy): 261
e_0(x), e_n(x): 265
$$
\sum_{k=0}^\infty \alpha_k D^k
$$: 285
B_n(X): 288
b_n: 288
U_\lambda^\xi(f(\xi)): 290
\Gamma(n), \Gamma(x): 317
\mathbf{B}(x, y): 324
\Gamma(z): 327

Mục tra cứu

Kề thêm một nghiệm của một đa thức, của một nguyên hàm, của một hàm mũ của một nguyên hàm, vào một trường vi phân, 121
Liên hợp (phương trình) của một phương trình vi phân tuyến tính, 186
Các đa thức Appell, 272
Nghiệm gần đúng đến sai số $\varepsilon$ của một phương trình vi phân, 166
Khai triển tiệm cận
– chính xác hơn một khai triển khác, 222
– của một hàm đối với một thang so sánh, 222
– của một hàm với độ chính xác $g_\alpha$, 222
– độ chính xác của, 222
Các khai triển tiệm cận, 220
– với các hệ số biến thiên, 226

Các số Bernouilli, 276
Các đa thức Bernouilli, 275
Công thức nhị thức, 108
Chuỗi nhị thức, 109

Bất đẳng thức của Carleman, 117
Bất đẳng thức của Carlson, 116
Tiêu chuẩn của Cauchy đối với các tích phân, 65
Công thức đổi biến số, 60
Đặc trưng
– địa phương, 211
Các hệ số
– nhị thức, 21
Các thang so sánh, 220
Quan hệ bù, 316
Toán tử hợp thành, 270
– hàm chỉ thị, 278
– cấp của, 272
– chính quy, 279
Hàm cosec, 95
Hàm cosin
– hyperbolic, 102
Cosin của một số phức, 102
Hàm cotang, 95
Các tiêu chuẩn
– hội tụ
– – loại thứ hai, 244
– tích phân
– – lôgarit, 229
Tiêu chuẩn
– tiêu chuẩn của Cauchy đối với các tích phân, 65
– Cauchy-Maclaurin, 237
– của Ermakoff, 86

d’Alembert
– tiêu chuẩn hội tụ, 245
Dãy định nghĩa của một hàm (H), 252
Đạo hàm
– bậc nhất, 3
– vô hạn, 10
– lôgarit, 94
– $n^{th}$, 20
– bậc hai, 20
– đối xứng, 39
Đạo hàm của một hàm, 3
– trái, 4
– phải, 4
Định thức của $n$ tích phân của một hệ $n$ phương trình vi phân tuyến tính, 184
Phương trình vi phân
– liên hợp, 187
– tích phân, 163
– tuyến tính, 177
– tuyến tính thuần nhất, 178
– tuyến tính cấp $n$, 192
– Lipschitz, 171
– Lipschitz địa phương, 171
– cấp nhất, 164
– cấp $n$, 164
– biến thực, 163
– vô hướng, 164
– nghiệm, 163

– nghiệm ngặt, 164
Các phương trình vi phân
– hệ, 164
các định lý du Bois-Reymond, 265

các tích phân Euler, 310
hằng Euler, 242
các công thức Euler, 99
công thức tổng Euler-Maclaurin, 282
khai triển Euler của cot $z$, 286
khai triển Euler của sin $z$, 287
Khai triển
– của log $\Gamma(z)$
– Stirling, 322
Hàm mũ
– phức, 97
Các hàm mũ
– lặp, 253
Mở rộng
– sơ cấp của một trường vi phân, 121
– của một trường Hardy, 248

Trường
– vi phân, 121
Công thức
– đổi biến, 60
– tổng Euler-Maclaurin, 282
– Gauss, 307
– tích phân từng phần, 60
– tích phân từng phần cấp $n$, 60
– phép nhân Legendre-Gauss, 318
– Leibniz, 20
– Stirling, 243
– Taylor, 21
– Wallis, 123
– Weierstrass, 308
Các công thức
– Euler, 99
Hàm
– khả vi $n$ lần
– tại một điểm, 20
– trên một khoảng, 20
– (H), 252
– lõm, 26
– lồi, 26
– dẫn xuất, 4
– khả vi
– tại một điểm, 3
– vô hạn lần, 20
– trên một khoảng, 4
– sự trội của một hàm này đối với một hàm khác, 212
– sơ cấp, 122
– tăng về phía phải, 37
– khả vi trái
– tại một điểm, 4
– trên một khoảng, 4
– Lipschitz, 168, 171
– Lipschitz địa phương, 171
– bị chặn lôgarit, 214
– lồi lôgarit, 310
– giá trị trung bình của, 58
– không đáng kể đối với một hàm khác, 214
– có biến phân bị chặn, 79
– có dấu không đổi, 217
– trội hơn một hàm khác, 214
– lồi chính quy, 260
– bị điều chỉnh, 54
– từng phần, 63
– khả vi phải
– tại một điểm, 4
– trên một khoảng, 4
– bậc thang, 53
– lõm ngặt, 26
– lồi ngặt, 25
– siêu cộng tính, 48
Các hàm
– so sánh được
– mạnh, 217
– tới cấp $k$, 232
– yếu, 214
– tương đương, 216
– hyperbolic, 102
– tương tự, 214

công thức Gauss, 307
tích phân Gauss, 314
khai triển Taylor suy rộng của một hàm, 278
khai triển Taylor suy rộng của một đa thức, 274
chuỗi sinh của các đa thức Appell gắn với một toán tử hợp thành, 275

bất đẳng thức Hadamard, 118
trường Hardy, 247
bất đẳng thức Hardy, 117
bất đẳng thức Hardy-Littlewood, 89
định lý tauber Hardy-Littlewood, 45
các đa thức Hermite, 282
bất đẳng thức Hlawka, 90
các hàm hyperbolic, 102
bất đẳng thức Hölder, 115

Đồng nhất thức
– Redheffer, 88

Hàm khả vi vô hạn lần, 20
Biểu đồ chỉ của một toán tử hợp thành, 278
Bất đẳng thức
– Carleman, 117
– Carlson, 116
– Cauchy-Buniakowski-Schwarz, 115
– Cauchy-Schwarz, 88
– Hadamard, 118
– Hardy, 117
– Hardy-Littlewood, 89
– Hlawka, 90
– Hölder, 115
– Opial, 90
– Weyl, 90
Tích phân
– hội tụ tuyệt đối, 67
– hội tụ, 63
– Euler, 310
– Gauss, 314
– hội tụ chuẩn tắc, 71, 73
– của một hàm bị điều chỉnh từng phần, 63
– của một hàm bị điều chỉnh trên một khoảng không compắc, 63
– của phương trình vi phân, 163
– Raabe, 318
– hội tụ đều, 71
Công thức tích phân từng phần, 60
Công thức tích phân từng phần cấp $n$, 60
Các hàm mũ lặp, 253
Lôgarit lặp, 229

các đồng dư thức của Kummer, 295

công thức Leibniz, 20
Đường thẳng
– ở địa phương phía trên một đồ thị, 31
– ở địa phương phía dưới một đồ thị, 31
– ở địa phương trên một đồ thị, 31
định lý Liouville, 122
điều kiện Lipschitz, 168
phương trình vi phân Lipschitz, 171
hàm Lipschitz, 171
đặc trưng địa phương, 211
Lôgarit
– lặp, 229
– Naper, 92
– tự nhiên, 92
– của số phức, 100
– giá trị chính, 100
Đạo hàm lôgarit, 94
Hàm bị chặn lôgarit, 214
Hàm lồi lôgarit, 310

Cực đại
– tương đối, 11
– ngặt, 11
Trung bình
– số học, 93
– có trọng, 93
– hình học, 93
– có trọng, 93
Giá trị trung bình của một hàm, 58
Định lý giá trị trung bình, 14
Phương pháp biến thiên các tham số, 182
Cực tiểu
– tương đối, 11
– ngặt, 11
lôgarit Naper, 92
lôgarit tự nhiên, 92
đa giác Newton, 259
tích phân hội tụ chuẩn tắc, 71

Toán tử
– hợp thành, 270
– tịnh tiến, 270
bất đẳng thức Opial, 90
Cấp của một hàm đối với một hàm khác, 218
định lý Peano, 167
Hàm bị điều chỉnh từng phần, 63
Đa giác
– Newton, 259
Các đa thức
– Appell, 272
– Bernouilli, 275
– Hermite, 282
Trội
– một hàm đối với một hàm khác, 214
Số nguyên tố
– không chính quy, 295
– chính quy, 295
Nguyên hàm
– của một hàm trên một khoảng của $\mathbf{R}$, 51
– cấp $n$, 62
– bậc hai, 62
– ngặt, 51
Phần chính
– của một hàm đối với một thang so sánh, 221
– của một hàm đối với một thang so sánh và một miền hệ số, 227
Nguyên lý so sánh các tích phân, 66

tích phân Raabe, 318
tiêu chuẩn Raabe, 244
đồng nhất thức Redheffer, 88
Rút gọn tới độ chính xác $g_\alpha$
– khai triển tiệm cận của một hàm, 222
Toán tử hợp thành chính quy, 279
Hàm bị điều chỉnh, 54
Số dư
– trong khai triển tiệm cận, 222
– trong công thức Euler-Maclaurin, 283
– trong công thức Taylor, 22
Toán tử giải của một phương trình vi phân tuyến tính, 180
định lý Rolle, 12
Các nghiệm
– đặc trưng, của một phương trình vi phân tuyến tính với các hệ số hằng, 190

Thang so sánh, 220
Cát tuyến, 95
Định lý giá trị trung bình thứ hai, 82
Các hàm tương tự, 214
Sin
– hyperbolic, 102
Sin của một số phức, 102
Nghiệm sai số đến $\varepsilon$ của một phương trình vi phân, 166
Công thức Stirling, 243
Nguyên thủy ngặt, 51
Nghiệm ngặt của một phương trình vi phân, 164
Ngặt
– phía trên một đồ thị, 23
– phía dưới một đồ thị, 23
Hàm lõm ngặt, 26
Hàm lồi ngặt, 25
Đường tựa của đồ thị của một hàm lồi, 29
Hệ các phương trình vi phân, 164
Các hệ
– các hệ cơ bản các nguyên của một hệ tuyến tính các phương trình vi phân vô hướng, 183

Tiếp tuyến
– nửa
– – trái, 11
– – phải, 11
– hyperbolic, 102
– với một đồ thị, 11
Khai triển Taylor, 22
Công thức Taylor, 21
– cấp $n$, 22
Kiểm tra
– của d’Alembert, 245
– của Raabe, 244
Định lý
– định lý tồn tại của Cauchy, 171
– Clausen-von Staudt, 294
– tauber Hardy-Littlewood, 45
– Liouville, 122
– giá trị trung bình, 14
– Peano, 167
– Rolle, 12
Các định lý
– du Bois-Reymond, 265
Toán tử tịnh tiến, 270

Nguyên hội tụ đều, 71

Giá trị
– giá trị trung bình của một hàm, 58
Biến thiên hằng số
– phương pháp, 182

Công thức Wallis, 123
Công thức Weierstrass, 308
Bất đẳng thức Weyl, 90
Wronski của $n$ nguyên của một phương trình vi phân tuyến tính cấp $n$, 193
