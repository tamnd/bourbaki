---
book: ts
book_title: Théories spectrales
chapter: II
chapter_title: GROUPES LOCALEMENT COMPACTS COMMUTATIFS
section: 3
section_title: Sous-espaces invariants
lang: vi
source: ts-i-ii-fr
book_pages: TS II.250-TS II.261, TS II.308-TS II.318
pdf_pages: 0262-0273, 0320-0330
extraction: native
subsections:
    - "no": 1
      title: Le cas de l’espace hilbertien $L^2(G)$
      page: 251
      pdf_page: 263
    - "no": 2
      title: Idéaux fermés de $L^1(G)$
      page: 251
      pdf_page: 263
    - "no": 3
      title: Sous-espaces invariants faiblement fermés de $L^{\infty}(G)$
      page: 257
      pdf_page: 269
statements: 12
exercises: 19
content_sha256: 6ac75da9c6a361e3f9e3ed81faf6b23148403e91ea07f961976c573b5c8d7e6b
translated_from: content/en-mt/ts/II/03_s3_sous_espaces_invariants.md
source_lang: en-mt
translation_method: machine
source_content_sha256: e8711a1f911a52cd46969798526bf587664ce4bff24468093600ea5ec18b7674
translation_model: gpt-5.4
translation_run: translate-vi-61869897
glossary_version: 34
glossary_terms_sha256: 355ec574b9ba167218e84c0caa3fd192ab23a14edf50f4fd9c6f59cd290ed7e0
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 3. CÁC KHÔNG GIAN CON BẤT BIẾN

Mục đích của số này là nghiên cứu một số không gian con bất biến đối với phép tịnh tiến trong các không gian $L^1(G)$, $L^2(G)$ và $L^{\infty}(G)$.

### 1. Trường hợp của không gian Hilbert $L^2(G)$

Với mọi tập con đo được M của $\widehat{G}$, ta ký hiệu bởi $E_M$ tập hợp các $f\in$ $L^2(G)$ sao cho biến đổi Fourier $\mathscr{F}_G(f)$ bằng không hầu khắp nơi trên $\widehat{G}$. Gọi $\varphi_M$ là hàm đặc số của M. Không gian $E_M$ là hạt nhân của ánh xạ tuyến tính liên tục $f\mapsto \varphi_M\mathscr{F}_G(f)$ từ $L^2(G)$ vào $L^2(\widehat{G})$, và do đó là một không gian con đóng của $L^2(G)$.

#### Mệnh đề 1 {#ts-ii-s3-prop-1 .statement tag=02N3}

a) Cho M là một tập con đo được của $\widehat{G}$. Với mọi $x\in G$, không gian $E_M$ ổn định dưới ánh xạ $f\mapsto \varepsilon_x*f$;

b) Cho M và N là các tập con đo được của $\widehat{G}$. Ta có $E_M= E_N$ khi và chỉ khi M và N bằng nhau sai khác một tập địa phương không đáng kể;

c) Mọi không gian con của $L^2(G)$ ổn định dưới các ánh xạ $f\mapsto \varepsilon_x*f$ với mọi $x\in G$ đều có dạng $E_M$ đối với một tập con đo được nào đó M của $\widehat{G}$.

Kết quả này sẽ được chứng minh sau (xem V, sẽ xuất hiện).

### 2. Các iđêan đóng của $L^1(G)$

Đối biến đổi Fourier trên đại số Banach $L^1(G)$ được đồng nhất với biến đổi Gelfand của $L^1(G)$ (II, p. 209). Với sự đồng nhất này, nhắc lại rằng nếu I là một iđêan của $L^1(G)$, ta ký hiệu bởi V(I) tập đóng trong $\widehat{G}$ gồm các đặc trưng $\chi \in \widehat{G}$ sao cho, với mọi hàm $f\in I$, đối biến đổi Fourier của $f$ triệt tiêu tại $\chi ($xem I, p. 30). Với mọi tập con M của $\widehat{G}$, ta ký hiệu bởi Υ(M) iđêan đóng của các $f\in L^1(G)$ sao cho $\overline{\mathscr{F}}_G(f)$ triệt tiêu trên M (I, p. 30).

Theo mệnh đề 2 của II, p. 219, đại số Banach $L^1(G)$ là chính quy. Theo § 5 của I, p. 88, do đó ta suy ra các tính chất sau đây của biến đổi và đối biến đổi Fourier:

1) Nếu F là một tập con đóng của $\widehat{G}$ và K là một tập con compắc của $\widehat{G}$ sao cho $F\cap K =\emptyset$, thì tồn tại một hàm $f\in L^1(G)$ sao cho $\mathscr{F}_G(f)$ bằng 0 trên F và bằng 1 trên K (I, p. 88, mệnh đề 1; đối với sự kiện này và các sự kiện tiếp theo, người ta chuyển từ đối biến đổi Fourier sang biến đổi Fourier bằng công thức (8) của II, p. 207).

2) Cho M là một tập con đóng của $\widehat{G}$. Tập hợp các iđêan I của $L^1(G)$ sao cho V(I) = M có phần tử lớn nhất là Υ(M) và phần tử nhỏ nhất là tập các $f\in L^1(G)$ mà đối biến đổi Fourier có giá compắc rời khỏi M (I, p. 91, mệnh đề 4).

3) Cho I là một iđêan của $L^1(G)$, và cho $g:\widehat{G}\rightarrow \mathbf{C}$ là một hàm liên tục. Giả sử rằng, với mọi $\chi \in \widehat{G}$, tồn tại một hàm $f_{\chi}\in I$ sao cho $g$ bằng $\mathscr{F}_G(f_{\chi})$ trong một lân cận của $\chi$. Giả sử thêm rằng tồn tại một hàm $f_{\infty}\in I$ sao cho $g$ bằng $\mathscr{F}_G(f_{\infty})$ trong phần bù của một tập compact của $\widehat{G}$$, điều kiện sau này luôn được thỏa mãn nếu G là rời rạc. Khi đó tồn tại một hàm $f\in I$ sao cho $g=\mathscr{F}_G(f)$ (I, p. 91, hệ quả 2).

#### Bổ đề 1 {#ts-ii-s3-lem-1 .statement tag=02N4}

Không gian các hàm của $L^1(G)$ mà biến đổi Fourier có giá compact là trù mật trong $L^1(G)$.

Vì $\mathscr{K}(\widehat{G})$ trù mật trong $L^2(\widehat{G})$ và biến đổi Fourier của $L^2(G)$ là một đẳng cự lên $L^2(\widehat{G})$ (định lý 1 của II, p. 215), nên không gian con V của $L^2(G)$ gồm các $f\in L^2(G)$ sao cho $\mathscr{F}_G(f)\in \mathscr{K}(\widehat{G})$ là trù mật trong $L^2(G)$.

Cho $g\in L^1(G)$. Tồn tại $g_1, g_2\in L^2(G)$ sao cho $g=g_1g_2$ (chẳng hạn có thể lấy $g_1=|g|^{1/2}$, và $g_2(x) = 0$ nếu $g(x) = 0,g_2(x) =$ $g(x)/g_1(x)$ trong trường hợp ngược lại). Do đó, từ điều vừa nói trên suy ra rằng $g$ là giới hạn của một dãy các hàm có dạng $h_1h_2$, trong đó $h_1$ và $h_2$ thuộc V. Bây giờ $\mathscr{F}_G(h_1h_2) =\mathscr{F}_G(h_1)*\mathscr{F}_G(h_2)$ (II, p. 223, mệnh đề 14), và $\mathscr{F}_G(h_1)*$ $\mathscr{F}_G(h_2)$ thuộc $\mathscr{K}(G)$. Bổ đề được chứng minh.

#### Mệnh đề 2 {#ts-ii-s3-prop-2 .statement tag=02N5}

Cho I là một iđêan đóng của $L^1(G)$, và cho $f\in L^1(G)$. Nếu $\overline{\mathscr{F}}_G(f)$ triệt tiêu trên một lân cận của V(I), thì $f$ thuộc I.

Cho $\varepsilon  >0$. Tồn tại một hàm $g\in L^1(G)$ sao cho $\|f-f*g\|_1<$ $\varepsilon$ (mệnh đề 8 của II, p. 211 (iv)). Cho $h\in L^1(G)$ sao cho giá của $\overline{\mathscr{F}}_G(h)$ là compact và $\|f\|_1\|g-h\|_1< \varepsilon$ (bổ đề 1). Ta có

$$
\|f-f*h\|_1\leqslant \|f-f*g\|_1+\|f*(g-h)\|_1<2\varepsilon
$$

Theo giả thiết về $f$, hàm $\overline{\mathscr{F}}_G(f*h) =\overline{\mathscr{F}}_G(f)\overline{\mathscr{F}}_G(h)$ có giá compact rời nhau với V(I), điều này suy ra $f*h\in I$ (nhận xét 2 ở trên). Vì $\varepsilon$ nhỏ tùy ý, ta có $f\in$ I = I.

#### Định lý 1 {#ts-ii-s3-thm-1 .statement tag=02N6}

Cho I là một iđêan đóng của $L^1(G)$ phân biệt với $L^1(G)$. Tồn tại một đặc trưng $\widehat{x}\in \widehat{G}$ sao cho $\mathscr{F}_G(f)(\widehat{x}) = 0$ với mọi $f\in I$.

Vì đại số $L^1(G)$ là chính quy (mệnh đề 2 của II, p. 219) và không có căn (hệ quả của mệnh đề 22 của I, p. 126), và vì tập các hàm mà đối biến đổi Fourier có giá compact thì trù mật trong $L^1(G)$ (bổ đề 1), hệ quả 1 của I, p. 92 cho thấy iđêan I được chứa trong một iđêan cực đại chính quy của $L^1(G)$, nghĩa là trong hạt nhân của một đặc trưng $\widehat{y}$ của $L^1(G)$ (định lý 2 của I, p. 30); khi đó có thể lấy $\widehat{x}=\widehat{y}^{-1}($xem công thức (8) của II, p. 207).

Hệ quả 1 (Định lý Tauber của Wiener)

Cho $f\in L^1(G)$. Nếu biến đổi Fourier của $f$ không triệt tiêu, thì các hàm $f*\varepsilon_x:g\mapsto f(gx^{-1})$, trong đó $x$ chạy qua G, tạo thành một tập toàn phần trong $L^1(G)$ (EVT, I, p. 12, định nghĩa 1).

Cho V là không gian con vectơ đóng của $L^1(G)$ sinh bởi các $f*\varepsilon_x$. Theo INT, VIII, §4, hệ quả của mệnh đề 20, không gian V là một iđêan đóng của $L^1(G)$. Theo định lý 1, ta có $V = L^1(G)$.

#### Định nghĩa 1 {#ts-ii-s3-def-1 .statement tag=02N7}

Cho $g$ là một hàm phức trên G và cho Φ là một bộ lọc trên G. Ta nói rằng $g$ dao động chậm theo Φ nếu, với mọi $\varepsilon  >0$, tồn tại một tập $M\in \Phi$ và một lân cận V của $e$ trong G sao cho

$x\in M$ and $y\in V=\Rightarrow |g(xy)-g(x)|\leqslant \varepsilon$.

#### Hệ quả 2 {#ts-ii-s3-def-1-cor-2 .statement tag=02N8}

Cho Φ là một bộ lọc trên G bất biến dưới phép tịnh tiến. Cho $f\in L^1(G)$ sao cho biến đổi Fourier của $f$ không triệt tiêu và sao cho $\int_Gf(x)dx= 1$. Cho $g\in L^{\infty}(G)$. Giả sử rằng $f*g$ có giới hạn hữu hạn $\alpha$ theo Φ.

a) Với mọi hàm $h\in L^1(G)$ sao cho $\int_Gh(x)dx= 1$, giới hạn của $h*g$ theo Φ bằng $\alpha$;

b) Giả sử thêm rằng $g$ dao động chậm theo Φ. Khi đó $g$ tiến tới $\alpha$ theo Φ.

Thay $g$ bằng $g-\alpha$, ta rút gọn về trường hợp $\alpha = 0$. Cho I là tập các hàm $h\in L^1(G)$ sao cho $h*g$ tiến tới 0 theo Φ. Tập I là một không gian con vectơ của $L^1(G)$ bất biến dưới phép tịnh tiến. Nó là một không gian đóng. Thật vậy, cho $h\in \overline{I}$. Với mọi hàm $h_0\in L^1(G)$ và mọi $x\in G$, ta có

$$
|(h*g)(x)|\leqslant |((h-h_0)*g)(x)|+|(h_0*g)(x)|
$$

$$
\leqslant \|h-h_0\|_1\|g\|_{\infty}+|(h_0*g)(x)|
$$

Với mọi $\varepsilon  >0$, tồn tại $h_0\in I$ sao cho $\|h-h_0\|_1\|g\|_{\infty}< \varepsilon$. Cho $M\in$ Φ sao cho $|(h_0*g)(x)|< \varepsilon$ với mọi $x\in M$. Khi đó ta có $|(h*g)(x)|<2\varepsilon$ với mọi $x\in M$, do đó $h*g$ hội tụ về 0 theo Φ. Điều này cho thấy rằng $h\in I$.

Vì vậy không gian I là một iđêan đóng của $L^1(G)$. Theo giả thiết ta có $f\in I$, nên $I = L^1(G)$ theo định lý 1 vì biến đổi Fourier của $f$ không triệt tiêu. Điều này suy ra a).

Hãy đặt mình dưới các giả thiết của b). Cho $\varepsilon  >0$. Vì $g$ dao động chậm theo Φ, tồn tại $M\in \Phi$ và một lân cận compact V của $e$ sao cho

$x\in M$ and $y\in V =\Rightarrow  |g(y^{-1}x)-g(x)|\leqslant \varepsilon$.

Cho $\varphi$ là hàm đặc trưng của V và $\mu=\int\varphi (x)dx$. Với mọi $x\in G$, ta có

$$
\frac{1}{\mu}(\varphi *g)(x) =\frac{1}{\mu}\int_Vg(y^{-1}x)dy=g(x) +\frac{1}{\mu}\int_V(g(y^{-1}x)-g(x))dy
$$

Do đó với mọi $x\in M$, ta có

$$
|\frac{1}{\mu}(\varphi *g)(x)-g(x)|\leqslant \varepsilon
$$

Vì, theo a), giới hạn của $\varphi *g$ theo Φ bằng không, nên ta có lim sup$_{\Phi}|g|\leqslant \varepsilon$. Vì $\varepsilon$ tùy ý, ta kết luận rằng giới hạn của $g$ theo Φ bằng không, điều đó chứng minh b).

#### Bổ đề 2 {#ts-ii-s3-lem-2 .statement tag=02N9}

Cho K là một tập con compact của G. Với mọi $\eta  >0$, tồn tại một hàm $j\in L^1(G)$ sao cho:

$$
\surd
$$

a) $\|j\|_1\leqslant$ 2 ;

b) hàm $\mathscr{F}_G(j)$ bằng 1 trong một lân cận của phần tử đơn vị của $\widehat{G}$;

c) với mọi $x\in K$, ta có $\|j-j*\varepsilon_x\|_1\leqslant \eta$.

Tập hợp $U_1$ các phần tử $\widehat{x}\in \widehat{G}$ sao cho

$$
|\langle \widehat{x}, x\rangle  -1|\leqslant \frac{\eta}{4}
$$

với mọi $x\in$ K là một lân cận của $e$ trong $\widehat{G}$. Cho U $\subset U_1$ là một lân cận mở, đối xứng và khả tích đối với độ đo Haar $m=d\widehat{x}$ của $\widehat{G}$ đối ngẫu với độ đo $dx$. Cho $V\subset U$ là một lân cận compact đối xứng của $e$ sao cho $m(V)\geqslant \frac{1}{2}m(U)$. Ta ký hiệu bởi $\varphi_U$ (resp. $\varphi_V$) hàm đặc trưng của U (resp. của V). Vì $\varphi_U$ thuộc $L^2(G)$, tồn tại $u\in L^2(G)$ sao cho $\varphi_U=\mathscr{F}_G(u)$ (định lý 1 của II, p. 215). Tương tự, tồn tại một hàm $v\in L^2(G)$ sao cho $\varphi_V=\mathscr{F}_G(v)$. Bây giờ chứng minh rằng hàm $j=\frac{1}{m(V)}uv$ thỏa mãn các tính chất đã yêu cầu. Ta có $j\in L^1(G)$.

a) Theo định lý Plancherel và điều kiện $m(V)\geqslant \frac{1}{2}m(U)$, ta có

$$
\|j\|_1\leqslant \frac{\|u\|_2\|v\|_2}{m(V)}=\frac{\|\mathscr{F}_G(u)\|_2\|\mathscr{F}_G(v)\|_2}{m(V)}=\surd\overline{mm(U)(V)m(V)}\leqslant \surd \overline{2}
$$

b) Tồn tại một lân cận W của $e$ trong $\widehat{G}$ sao cho WV $\subset U$ (TG, II, p. 31, mệnh đề 4). Với mọi $\widehat{x}\in W$, ta có $\widehat{x}V\subset U$, và mệnh đề 14 của II, p. 223 suy ra

$$
\mathscr{F}_G(j)(\widehat{x}) =\frac{1}{m(V)}(\mathscr{F}_G(u)*\mathscr{F}_G(v))(\widehat{x})
$$

$$
=\frac{1}{m(V)}\int_{\widehat{G}}\varphi_U(\widehat{y})\varphi_V(\widehat{y}^{-1}\widehat{x})dm(\widehat{y})
$$

$$
=\frac{m(U \cap\widehat{x}V^{-1})}{m(V)}=\frac{m(\widehat{x}V)}{m(V)}= 1
$$

vì V đối xứng.

c) Nếu $x\in K$, ta có

$$
\|u-u*\varepsilon_x\|^2_2=\int_{\widehat{G}}|\mathscr{F}_G(u)(\widehat{x})(1- \langle x,\widehat{x}\rangle )||^2dm(\widehat{x})\leqslant m(U)(\frac{\eta}{4})^2
$$

vì $U\subset U_1$, và tương tự $\|v-v*\varepsilon_x\|^2_2\leqslant m(V)(\frac{\eta}{4})^2$. Do đó

$$
\|j-j*\varepsilon_x\|_1=\frac{1}{m(V)}\|u(v-v*\varepsilon_x) + (v*\varepsilon_x)(u-u*\varepsilon_x)\|_1
$$

$$
\leqslant \frac{\eta}{4m(V)}(\|u\|_2\surd m(V) +\|v\|_2\surd\overline{m(U)})
$$

$$
=\eta \surd\overline{m2m(U)(V)m(V)}< \eta
$$

#### Mệnh đề 3 {#ts-ii-s3-prop-3 .statement tag=02NA}

Đại số $L^1(G)$ thỏa mãn điều kiện Ditkin (I, p. 92, đn. 2).

Cho $\chi$ là một đặc trưng của $L^1(G)$. Phân biệt hai trường hợp tùy theo $\chi$ là không hay khác không. Nếu $\chi$ là không, cần kiểm tra rằng với mọi hàm $f\in L^1(G)$, tồn tại một dãy $(f_n)_{n\geqslant 1}$ trong $L^1(G)$ sao cho $\mathscr{F}(f_n)$ triệt tiêu ngoài một tập con compact của $\widehat{G}$ và sao cho $f_n*f$ tiến tới $f$ trong $L^1(G)$. Sự tồn tại của một dãy như vậy suy ra từ Bổ đề 1 ở trên và Mệnh đề 8 của II, p. 211.

Bây giờ giả sử rằng $\chi$ khác không, do đó $\chi \in \mathsf{X}(L^1(G)) =\widehat{G}$ (Mệnh đề 1 của II, p. 202). Cho $f\in L^1(G)$ sao cho $\mathscr{G}_{L^1(G)}(f)(\chi ) =$ $\overline{\mathscr{F}}(f)(\chi ) = 0$. Vấn đề là chứng minh sự tồn tại của một dãy $(f_n)_{n\geqslant 1}$ trong $L^1(G)$ sao cho $f*f_n$ hội tụ tới $f$ trong $L^1(G)$ và sao cho $\overline{\mathscr{F}}(f_n)$ triệt tiêu trong một lân cận của $\chi$. Ta có thể giả sử rằng $\|f\|_1= 1$. Bằng phép tịnh tiến trong $\widehat{G}$, ta rút gọn về trường hợp $\chi =e$.

Cho $K_n$ là một tập con compact của G sao cho

$$
\int_{G-K_n}|f(x)|dx\leqslant \frac{1}{n}
$$

Cho $u_n\in L^1(G)$ là một hàm $\geqslant 0$ sao cho $\|u_n\|_1= 1$ và

$$
\|f-f*u_n\|_1\leqslant \frac{1}{n}
$$

(x. Mệnh đề 8 của II, p. 211, (iii)). Theo Bổ đề$\surd$ 2, tồn tại một hàm $j_n$ trong $L^1(G)$ sao cho $\|j_n\|_1\leqslant \overline{2}$, đối biến đổi Fourier của nó bằng 1 trong một lân cận của $e$, và hơn nữa sao cho $\|j_n-j_n*\varepsilon_x\|_1\leqslant n^{-1}$ với mọi $x\in K_n$. Đặt

$$
f_n=u_n-j_n*u_n
$$

Ta sẽ chứng minh rằng dãy $(f_n)_{n\geqslant 1}$ có các tính chất cần có. Trước hết, ta có

$$
\mathscr{F}(f_n) =\mathscr{F}(u_n)-\mathscr{F}(j_n)\mathscr{F}(u_n) = (1-\mathscr{F}(j_n))\mathscr{F}(u_n)
$$

do đó biến đổi Fourier của $f_n$ triệt tiêu trong một lân cận của $\chi =e$. Mặt khác,

1

$$
\|f*f_n-f\|_1\leqslant \|f*u_n-f\|_1+\|f*j_n\|_1\|u_n\|_1\leqslant +\|f*j_n\|_1
$$

$$
n
$$

Bây giờ, với hầu khắp mọi $y\in G$, ta có

$$
(f*j_n)(y) =\int_Gf(x)j_n(x^{-1}y)dx=\int_Gf(x)(j_n(x^{-1}y)-j_n(y))dx
$$

vì, theo giả thiết, ta có $\mathscr{F}(f)(e) =\int_Gf(x)dx= 0$. Do đó

$$
\|f*j_n\|_1\leqslant \int_G|f(x)| \|j_n*\varepsilon_x-j_n\|_1dx
$$

$$
=\int|f(x)| \|j_n*\varepsilon_x-j_n\|_1dx
$$

$$
+\int^{K_n}|f(x)| \|j_n*\varepsilon_x-j_n\|_1dx
$$

$G-K_n$

$1\int\int$ 5 $\leqslant |f(x)|dx+ 4|f(x)|dx\leqslant$.

$n_{K_n}G-K_{_n}n$

Sau cùng, $\|f*f_n-f\|_1\leqslant 6n^{-1}$ và do đó $f*f_n$ hội tụ đến $f$ trong $L^1(G)$, như đã muốn.

Áp dụng mệnh đề 5, ta thu được kết quả sau:

#### Định lý 2 {#ts-ii-s3-thm-2 .statement tag=02NB}

Cho I là một iđêan đóng của $L^1(G)$ sao cho biên của V(I) không chứa tập hoàn hảo khác rỗng nào. Khi đó I là tập hợp các hàm $f\in L^1(G)$ sao cho $\mathscr{F}(f)$ triệt tiêu trên V(I).

Đối với một iđêan đóng tùy ý của $L^1(G)$, kết luận của định lý 2 nói chung là sai (xem bài tập 12 của II, p. 314). Chính xác hơn, bây giờ có thể chứng minh rằng, nếu G không compắc, thì tồn tại một iđêan đóng của $L^1(G)$ không tự liên hợp (xem chẳng hạn W. Rudin, Fourier analysis on groups, Interscience tracts in pure and applied mathematics, định lý 7.7.1.)

#### Hệ quả {#ts-ii-s3-n2-cor-1 .statement tag=02NC}

Nếu một iđêan đóng I của $L^1(G)$ được chứa trong một iđêan cực đại chính quy duy nhất, thì bản thân I là cực đại chính quy.

### 3. Các không gian con bất biến đóng yếu của $L^{\infty}(G)$

Trong số này, ta đồng nhất $L^{\infty}(G)$ với đối ngẫu của $L^1(G)$, và trang bị cho nó tôpô yếu $\sigma (L^{\infty}(G),L^1(G))$. Ta ký hiệu bởi $(f, g)\mapsto  \langle f, g\rangle$ ánh xạ song tuyến tính xác định tính đối ngẫu này đối với $f\in L^1(G)$ và $g\in L^{\infty}(G)$.

Ánh xạ $W\mapsto W^{\circ}$ là một song ánh từ tập hợp các không gian con vectơ đóng yếu của $L^{\infty}(G)$ lên tập hợp các không gian con vectơ đóng của $L^1(G)$ (EVT, II, p. 55, mệnh đề 10).

Mặt khác, nếu $f\in L^1(G)$ và $x\in G$, tự đồng cấu $g\mapsto f*g$ (tương ứng $g\mapsto \varepsilon_x*g$) của không gian Banach $L^1(G)$ có chuyển vị là tự đồng cấu $h\mapsto \check{f}*h$ (tương ứng $h\mapsto \varepsilon_{x^{-1}}*h$) của không gian Banach $L^{\infty}(G)$ (INT, VIII, §4, n$^o3$, ví dụ 6). Để một không gian con vectơ đóng của $L^1(G)$ là một iđêan của $L^1(G)$, điều kiện cần và đủ là nó bất biến dưới các phép tịnh tiến của G. Do đó, để một không gian con vectơ đóng yếu của $L^{\infty}(G)$ ổn định dưới phép chập với các phần tử của $L^1(G)$, điều kiện cần và đủ là nó bất biến dưới các phép tịnh tiến của G.

Cho W là một không gian con vectơ đóng yếu của $L^{\infty}(G)$. Giả sử rằng W (và do đó cả $W^{\circ}$) bất biến dưới các phép tịnh tiến của G. Cho $f\in$ $L^1(G)$. Với mọi $g\in L^{\infty}(G)$, ta có $(\check{f}*g)(x) =\langle \varepsilon_x*f, g\rangle =\langle f, \varepsilon_{x^{-1}}*g\rangle$. Do đó, để $f$ thuộc $W^{\circ}$, điều kiện cần và đủ là $\check{f}*g= 0$ với mọi $g\in W$.

Nếu W là một không gian con vectơ đóng yếu của $L^{\infty}(G)$ bất biến theo phép tịnh tiến, ta sẽ ký hiệu bởi A(W) tập hợp các đặc trưng $\chi \in \widehat{G}$ thuộc W. Đó là một tập con đóng của $\widehat{G}$. Nếu F là một tập con đóng của $\widehat{G}$, ta sẽ ký hiệu bởi Y(F) không gian con vectơ đóng yếu của $L^{\infty}(G)$ sinh bởi các phần tử của F; vì mọi phép tịnh tiến của G biến mỗi đặc trưng thành một hàm tỉ lệ với đặc trưng ấy, không gian Y(F) là bất biến theo phép tịnh tiến.

Cho W là một không gian con đóng yếu của $L^{\infty}(G)$ bất biến dưới các phép tịnh tiến của G. Theo định lý lưỡng cực (EVT, II, p. 48, định lý 1), một đặc trưng $\chi$ thuộc W khi và chỉ khi nó thuộc $(W^{\circ})^{\circ}$; không gian sau cùng này là tập hợp các hàm $g\in L^{\infty}(G)$ sao cho $\langle f, g\rangle = 0$ với $f\in W^{\circ}$. Ta có $\langle f, \chi \rangle =\overline{\mathscr{F}}(f)(\chi )$, và do đó

$$
A(W) = V(W^{\circ})
$$

Tương tự, một hàm $f\in L^1(G)$ thuộc $Y(F)^{\circ}$ khi và chỉ khi $\langle f, \chi \rangle = 0$ với mọi $\chi \in F$, điều này tương đương với $\overline{\mathscr{F}}(f)(\chi ) = 0$ với $\chi \in F$, tức là tương đương với $f\in \Upsilon (F)$. Do đó (sđd.) ta có

$$
Y(F) = \Upsilon (F)^{\circ}
$$

Các quan hệ V(Υ(F)) = F (I, p. 13 và I, p. 30) và $\Upsilon (V(I))\supset I$, kết hợp với định lý đối cực kép (TVS, II, p. 48, đl. 1), khi đó cho

$$
A(Y(F)) = F,Y(A(W))\subset W
$$

#### Mệnh đề 4 {#ts-ii-s3-prop-4 .statement tag=02ND}

Cho W là một không gian con vectơ đóng yếu của $L^{\infty}(G)$, bất biến đối với phép tịnh tiến và khác không. Khi đó W chứa ít nhất một đặc trưng của G.

Ta đã thấy rằng $A(W) = V(W^{\circ})$. Vì $W\not= 0$, ta có $W^{\circ}\not= L^1(G)$, và khi đó $V(W^{\circ})$ khác rỗng theo đl. 1 của II, p. 252.

#### Mệnh đề 5 {#ts-ii-s3-prop-5 .statement tag=02NE}

Cho W là một không gian con vectơ đóng yếu của $L^{\infty}(G)$ bất biến đối với phép tịnh tiến.

a) Với mọi lân cận U của A(W) trong $\widehat{G}$, mọi hàm của W là giới hạn yếu của các tổ hợp tuyến tính của các đặc trưng thuộc U;

b) Nếu biên của A(W) không chứa tập hoàn hảo khác rỗng nào, mọi hàm của W là giới hạn yếu của các tổ hợp tuyến tính của các đặc trưng thuộc W.

Để chứng minh a), theo định lý đối cực kép, chỉ cần chỉ ra rằng nếu $f$ là một hàm của $L^1(G)$ trực giao với các phần tử của U, thì $f$ trực giao với W. Khi đó đối biến đổi Fourier $\overline{\mathscr{F}}(f)$ triệt tiêu trên lân cận U của $A(W) = V(W^{\circ})$, nên mđ. 2 của II, p. 252 thực sự cho thấy rằng $f\in W^{\circ}$. Mệnh đề b) được thiết lập tương tự, dùng đl. 2 của II, p. 257 thay cho mđ. 2 của II, p. 252.

# Bài tập

Trong tất cả các bài tập của Chương II, đối ngẫu của $\mathbf{R}^n$ (resp. của $(\mathbf{R}/\mathbf{Z})^n$, của $\mathbf{Z}^n$) được đồng nhất với $\mathbf{R}^n$ (resp. với $\mathbf{Z}^n$, với $(\mathbf{R}/\mathbf{Z})^n$) theo hệ quả 3 của II, p. 236. Với $x$ và $y$ trong $\mathbf{R}^n$, ta viết $x\cdot y=\sum_ix_iy_i$. Ta viết $\mathbf{T}=\mathbf{R}/\mathbf{Z}$, và trang bị cho $\mathbf{T}$ cấu trúc nhóm Lie thực của nó (LIE, III, p. 105, mđ. 11). Biến đổi Fourier của một hàm $f$ thường sẽ được ký hiệu bởi $\widehat{f}$.

Với mọi số thực khác không $t$, ta viết s($t$) $=t/|t|$, và đặt s(0) = 0 (hàm dấu).

Nếu E là một không gian vectơ tôpô và $(x_h)_{h\in\mathbf{Z}}$ là một họ các phần tử của E, chuỗi có số hạng tổng quát $x_h$ được gọi là hội tụ đối xứng trong E tới $x\in E$ nếu dãy $(s_n)_{n\geqslant 1}$ xác định bởi

$$
s_n=\sum_{-n\leqslant h\leqslant n}x_h
$$

hội tụ tới $x$ trong E.

Một độ đo xác suất trên một không gian tôpô compact địa phương X là một độ đo dương có tổng khối lượng bằng 1. Tập hợp các độ đo xác suất trên X được ký hiệu bởi $\mathscr{P}(X)$.

Trừ khi có nói khác, G ký hiệu một nhóm tôpô compact địa phương giao hoán.

## BÀI TẬP {#ts-ii-s3-exercises}

Xem [các bài tập cho § 3](exercises/s3/).
