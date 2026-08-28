---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VIII
chapter_title: SPLIT SEMI-SIMPLE LIE ALGEBRAS
section: 1
section_title: The Lie algebra sl(2, k) and its representations
lang: vi
source: lie-vii-ix
book_pages: 69-77, 219-226
pdf_pages: 0077-0085, 0227-0234
extraction: native+ocr
subsections:
    - "no": 1
      title: CANONICAL BASIS OF $\mathfrak{s}\mathfrak{l}$(2$\boldsymbol{, k}$)
      page: 69
      pdf_page: 77
    - "no": 2
      title: PRIMITIVE ELEMENTS OF $\mathfrak{s}\mathfrak{l}$(2$\boldsymbol{, k}$)-MODULES
      page: 70
      pdf_page: 78
    - "no": 3
      title: THE SIMPLE MODULES V($\boldsymbol{m}$)
      page: 72
      pdf_page: 80
    - "no": 4
      title: LINEAR REPRESENTATIONS OF THE GROUP SL(2$\boldsymbol{, k}$)
      page: 74
      pdf_page: 82
    - "no": 5
      title: SOME ELEMENTS OF SL(2$\boldsymbol{, k}$)
      page: 76
      pdf_page: 84
statements: 23
exercises: 18
content_sha256: ffc5ee382a861ae32aeab4a38a0a8c4fe87d649973da062411662d43313169ca
translated_from: content/en/lie/VIII/01_s1_the_lie_algebra_sl_2_k_and_its.md
source_content_sha256: d56ad334c8b961365f3d72d7c521802edd95553bc6c867158ffa18290345692f
translation_model: gpt-5.4
translation_run: translate-vi-d50e07ef
glossary_version: 34
glossary_terms_sha256: ec9c62c2ef7c555a3c2d342ee12c5ec4769a652e9a0199c9f9373b01fc6044f1
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 1. ĐẠI SỐ LIE $\mathfrak{s}\mathfrak{l}$(2$\boldsymbol{, k}$) VÀ CÁC BIỂU DIỄN CỦA NÓ

### 1. CƠ SỞ CHÍNH TẮC CỦA $\mathfrak{s}\mathfrak{l}$(2$\boldsymbol{, k}$)

#### Bổ đề 1 {#lie-viii-s1-lem-1 .statement tag=00XS}

Cho A là một đại số kết hợp trên $k,H$ và $X$ là các phần tử của A sao cho $[H, X] = 2X$.

(i) $[H, X^n] = 2nX^n$ với mọi số nguyên $n\geq 0$.

(ii) Nếu $Z$ là một phần tử của A sao cho $[Z, X] =H$, thì, với mọi số nguyên $n >0$,

$$
[Z, X^n] =nX^{n-1}(H+n-1) =n(H-n+ 1)X^{n-1}
$$

Ánh xạ $T \rightarrow [H, T]$ từ A vào A là một đạo hàm, điều đó suy ra (i). Với các giả thiết trong (ii),

$$
[Z, X^n] =\sum_{i+j=n-1}X^iHX^j
$$

$$
=\sum_{i+j=n-1}(X^iX^jH+X^i2jX^j)
$$

$$
=nX^{n-1}H+ 2X^{n-1}\frac{n(n- 1)}{2}
$$

$$
=nX^{n-1}(H+n-1)
$$

Mặt khác, $X^{n-1}(H+n-1) = (H-n+ 1)X^{n-1}$ theo (i). Q.E.D.

Nhớ rằng ta ký hiệu bởi $\mathfrak{s}\mathfrak{l}(2, k)$ đại số Lie gồm các ma trận vuông cấp 2, vết không, và với các phần tử trong $k$. Đại số Lie này là đơn, chiều 3 (Chap. I, §6, no. 7, Ví dụ). Cơ sở chính tắc của $\mathfrak{s}\mathfrak{l}(2, k)$ là cơ sở $(X_+, X_-, H)$, trong đó

$(01)($ 0 $0)(1$ 0 $)$

$X_+=$ 0 0 $X_-=-1$ 0 $H=$ 0 $-1$.

Ta có

$$
[H, X_+] = 2X_+[H, X_-] =-2X_-[X_+, X_-] =-H \tag{1}
$$

Vì biểu diễn đồng nhất của $\mathfrak{s}\mathfrak{l}(2, k)$ là đơn ánh, $H$ là một phần tử nửa đơn của $\mathfrak{s}\mathfrak{l}(2, k)$ và $X_+, X_-$ là những phần tử lũy linh của $\mathfrak{s}\mathfrak{l}(2, k)$ (Chap. I, §6, no. 3, Định lý 3). Theo Chap. VII, §2, no. 1, Ví dụ $4,kH$ là một đại số con Cartan của $\mathfrak{s}\mathfrak{l}(2, k)$. Ánh xạ $U \rightarrow  -^tU$ là một tự đẳng cấu đối hợp của đại số Lie $\mathfrak{s}\mathfrak{l}(2, k)$, được gọi là đối hợp chính tắc của $\mathfrak{s}\mathfrak{l}(2, k)$; nó biến $(X_+, X_-, H)$ thành $(X_-, X_+,-H)$.

#### Bổ đề 2 {#lie-viii-s1-lem-2 .statement tag=00XT}

Trong đại số bao của $\mathfrak{s}\mathfrak{l}(2, k)$,

$$
[H, X_+^n] = 2nX_+^n[H, X_-^n] =-2nX_-^n
$$

với mọi số nguyên $n\geq 0$, và

$$
[X_-, X_+^n] =nX_+^{n-1}(H+n-1) =n(H-n+ 1)X_+^{n-1}
$$

$$
[X_+, X_-^n] =nX_-^{n-1}(-H+n-1) =n(-H-n+ 1)X_-^{n-1}
$$

nếu $n >0$.

Các hệ thức thứ nhất và thứ ba suy ra từ Bổ đề 1. Các hệ thức khác có thể được suy ra từ chúng bằng cách dùng phép đối hợp chính tắc của $\mathfrak{s}\mathfrak{l}(2, k)$.

### 2. CÁC PHẦN TỬ NGUYÊN THỦY CỦA CÁC $\mathfrak{s}\mathfrak{l}$(2$\boldsymbol{, k}$)-MÔĐUN

Cho E là một $\mathfrak{s}\mathfrak{l}(2, k$)-môđun. Nếu $A\in \mathfrak{s}\mathfrak{l}(2, k)$ và $x\in E$, ta sẽ thường viết $Ax$ thay cho $A_Ex$. Cho $\lambda \in k$. Nếu $Hx=\lambda x$ thì ta nói, theo lối nói lạm dụng, rằng $x$ là một phần tử của E có trọng số $\lambda$, hoặc rằng $\lambda$ là trọng số của $x$. Nếu E hữu hạn chiều, thì $H_E$ là nửa đơn, do đó tập hợp các phần tử có trọng số $\lambda$ là không gian con nguyên sơ của E ứng với $H_E$ và $\lambda$ (x. Chương VII, §1, no. 1).

#### Bổ đề 3 {#lie-viii-s1-lem-3 .statement tag=00XU}

Nếu $x$ là một phần tử có trọng số $\lambda$, thì $X_+x$ là một phần tử có trọng số $\lambda + 2$ và $X_-x$ là một phần tử có trọng số $\lambda -2$.

Thật vậy, $HX_+x= [H, X_+]x+X_+Hx= 2X_+x+X_+\lambda x= (\lambda + 2)X_+x$, và tương tự $HX_-x= (\lambda -2)X_-x$ (xem thêm cả Chap. VII, §1, no. 3, Mệnh đề 10 (ii)).

#### Định nghĩa 1 {#lie-viii-s1-def-1 .statement tag=00XV}

Cho E là một $\mathfrak{s}\mathfrak{l}(2, k)$-môđun. Một phần tử của E được gọi là nguyên thủy nếu nó là một vectơ riêng khác không của $H_E$ và thuộc hạt nhân của $X_{+E}$.

Một phần tử khác không $e$ của E là nguyên thủy khi và chỉ khi $ke$ ổn định dưới phép toán của $kH+kX_+$; điều này chẳng hạn suy ra từ Bổ đề 3.

Ví dụ Phần tử $X_+$ là nguyên thủy có trọng số 2 đối với biểu diễn liên hợp của $\mathfrak{s}\mathfrak{l}(2, k)$. Phần tử $(1,0)$ của $k^2$ là nguyên thủy có trọng số 1 đối với biểu diễn đồng nhất của $\mathfrak{s}\mathfrak{l}(2, k)$ trên $k^2$.

#### Bổ đề 4 {#lie-viii-s1-lem-4 .statement tag=00XW}

Cho E là một $\mathfrak{s}\mathfrak{l}(2, k)$-môđun hữu hạn chiều khác không. Khi đó E có các phần tử nguyên thủy.

Vì $X_+$ là một phần tử lũy linh của $\mathfrak{s}\mathfrak{l}(2, k),X_{+E}$ là lũy linh. Giả sử rằng $X_{+E}^{m-1}\not= 0$ và $X_{+E}^m$ = 0. Theo Bổ đề 2,

$$
m(H_E-m+ 1)X_{+E}^{m-1}= [X_{-E}, X_{+E}^m] = 0
$$

và do đó các phần tử của $X_+^{m-1}(E)$**--** $\{0\}$ là nguyên thủy.

#### Mệnh đề 1 {#lie-viii-s1-prop-1 .statement tag=00XX}

Cho E là một $\mathfrak{s}\mathfrak{l}(2, k)$-môđun, và $e$ là một phần tử nguyên thủy của E có trọng số $\lambda$. Đặt $e_n=\frac{(-1)^n}{n}X_-^ne$ với $n\geq 0$, và $e_{-1}= 0$. Khi đó

$$
He_n= (\lambda -2n)e_n
$$

$$
X_-e_n=-(n+ 1)e_{n+1} \tag{2}
$$

$$
X_+e_n= (\lambda -n+ 1)e_{n-1}
$$

Công thức thứ nhất suy ra từ Bổ đề 3, và công thức thứ hai suy ra từ định nghĩa của các $e_n$. Ta chứng minh công thức thứ ba bằng quy nạp theo $n$. Nó được thỏa mãn với $n= 0$ vì $e_{-1}= 0$. Nếu $n >0$,

$$
nX_+e_n=-X_+X_-e_{n-1}=-[X_+, X_-]e_{n-1}-X_-X_+e_{n-1}
$$

$$
=He_{n-1}-X_-(\lambda -n+ 2)e_{n-2}
$$

$$
= (\lambda -2n+ 2 + (n-1)(\lambda -n+ 2))e_{n-1}
$$

$$
=n(\lambda -n+ 1)e_{n-1}
$$

#### Hệ quả {#lie-viii-s1-n2-cor-1 .statement tag=00XY}

Môđun con của E sinh bởi $e$ là không gian vectơ con sinh bởi các $e_n$.

Điều này suy ra từ các công thức (2).

Các số nguyên $n\geq 0$ sao cho $e_n\not= 0$ tạo thành một khoảng trong $\mathbf{N}$, và các phần tử tương ứng $e_n$ lập thành một cơ sở trên $k$ của môđun con sinh bởi $e$ (thật vậy, chúng độc lập tuyến tính vì chúng là các phần tử khác không có các trọng số phân biệt). Cơ sở này sẽ được gọi là liên kết với phần tử nguyên thủy $e$.

#### Mệnh đề 2 {#lie-viii-s1-prop-2 .statement tag=00XZ}

Nếu môđun con V của E sinh bởi phần tử nguyên thủy $e$ là hữu hạn chiều, thì:

(i) trọng số $\lambda$ của $e$ là nguyên và bằng dim $V-1$;

(ii) $(e_0, e_1, . . . , e_{\lambda})$ là một cơ sở của V, và $e_n= 0$ với $n > \lambda$;

(iii) các giá trị riêng của $H_V$ là $\lambda , \lambda -2, \lambda -4, . . . ,-\lambda$; tất cả đều có bội số 1;

(iv) mọi phần tử nguyên thủy của V đều tỉ lệ với $e$;

(v) hoán tập của môđun V thu về các vô hướng; đặc biệt, V là đơn tuyệt đối.

Gọi $m$ là số nguyên lớn nhất sao cho $e_m\not= 0$. Khi đó $0 =X_+e_{m+1}=$ $(\lambda -m)e_m$, nên $\lambda =m$; vì $(e_0, e_1, . . . , e_m)$ là một cơ sở của V, điều này chứng minh (i) và (ii). Mệnh đề (iii) suy ra từ đẳng thức $He_n= (\lambda -2n)e_n$. Ta có $X_+e_n\not= 0$ với $1\leq n\leq m$, do đó có (iv). Gọi $c$ là một phần tử của hoán tập của môđun V. Khi đó $Hc(e) =cH(e) =\lambda c(e)$, nên tồn tại $\mu\in k$ sao cho $c(e) =\mu e$; khi đó

$$
cX_-^qe=X_-^qce=\mu X_-^qe
$$

với mọi $q\geq 0$, nên $c=\mu.1$, điều đó chứng minh (v).

#### Hệ quả {#lie-viii-s1-n2-cor-2 .statement tag=00Y0}

Cho E là một $\mathfrak{s}\mathfrak{l}(2, k)$-môđun hữu hạn chiều.

(i) Tự đồng cấu $H_E$ chéo hóa được và các giá trị riêng của nó là các số nguyên.

(ii) Với mọi $p\in \mathbf{Z}$, gọi $E_p$ là không gian riêng của $H_E$ tương ứng với trị riêng $p$. Cho $i$ là một số nguyên $\geq 0$. Ánh xạ $X_{-E}^i|E_p: E_p\rightarrow E_{p-2i}$ là đơn ánh với $i\leq p$, song ánh với $i=p$, và toàn ánh với $i\geq p$. Ánh xạ $X_{+E}^i|E_{-p}: E_{-p}\rightarrow E_{-p+2i}$ là đơn ánh với $i\leq p$, song ánh với $i=p$, và toàn ánh với $i\geq p$.

(iii) Độ dài của E bằng chiều của Ker$X_{+E}$ và chiều của Ker$X_{-E}$.

(iv) Gọi $E'$ (tương ứng, $E''$) là tổng của các $E_p$ với $p$ chẵn (tương ứng, lẻ). Khi đó $E'$ (tương ứng, $E''$) là tổng của các môđun con đơn của E có chiều lẻ (tương ứng, chẵn); và $E = E'\oplus E''$. Độ dài của $E'$ là chiều của $E_0$, và độ dài của $E''$ là chiều của $E_1$.

(v) Ker$X_{+E}\cap$ Im$X_{+E}\subset \sum_{p>0}E_p$ và Ker$X_{-E}\cap$ Im$X_{-E}\subset \sum_{p<0}E_p$.

Nếu E đơn, thì E được sinh bởi một phần tử nguyên thủy (Bổ đề 4), và chỉ cần áp dụng các Mệnh đề 1 và 2. Trường hợp tổng quát suy ra vì mọi $\mathfrak{s}\mathfrak{l}(2, k$)-môđun hữu hạn chiều đều là nửa đơn.

### 3. CÁC MÔĐUN ĐƠN V($\boldsymbol{m}$)

Gọi $(u, v)$ là cơ sở chính tắc của $k^2$. Đối với biểu diễn đồng nhất của $\mathfrak{s}\mathfrak{l}(2, k)$,

$$
X_+u= 0Hu=uX_-u=-v
$$

$$
X_+v=uHv=-vX_-v= 0
$$

Xét đại số đối xứng $\mathbf{S}(k^2)$ của $k^2($Đại số, Chương III, §6, no. 1, Định nghĩa 1). Các phần tử của $\mathfrak{s}\mathfrak{l}(2, k)$ mở rộng duy nhất thành các phép đạo hàm của $\mathbf{S}(k^2)$, làm cho $\mathbf{S}(k^2)$ có cấu trúc của một $\mathfrak{s}\mathfrak{l}(2, k$)-môđun (Chương I, §3, no. 2). Gọi $V(m)$ là tập hợp các phần tử thuần nhất của $\mathbf{S}(k^2)$ có bậc $m$. Khi đó $V(m)$ là một môđun con $\mathfrak{s}\mathfrak{l}(2, k$) của $\mathbf{S}(k^2)$ có chiều $m+ 1$, lũy thừa đối xứng bậc $m$ của $V(1) =k^2$ (Chương III, phụ lục). Nếu $m, n$ là các số nguyên sao cho $0\leq n\leq m$, đặt

$$
e^{(m)}_n=(m)u^{m-n}v^n\in V(m)
$$

$$
n
$$

#### Mệnh đề 3 {#lie-viii-s1-prop-3 .statement tag=00Y1}

Với mọi số nguyên $m\geq 0$, $V(m)$ là một $\mathfrak{s}\mathfrak{l}(2, k)$-môđun đơn tuyệt đối. Trong môđun này, $e^{(m)}_0=u^m$ là nguyên thủy có trọng số $m$.

Ta có $X_+u^m= 0$ và $Hu^m=mu^m$, nên $u^m$ là nguyên thủy có trọng số $m$. Môđun con của $V(m)$ sinh bởi $u^m$ có số chiều hữu hạn $m+ 1$ (Mệnh đề 2 (i)) và do đó bằng $V(m)$. Theo Mệnh đề 2 (v), $V(m)$ là đơn tuyệt đối.

#### Định lý 1 {#lie-viii-s1-thm-1 .statement tag=00Y2}

Mọi $\mathfrak{s}\mathfrak{l}(2, k)$-môđun đơn hữu hạn chiều $n$ đều đẳng cấu với $V(n-1)$. Mọi $\mathfrak{s}\mathfrak{l}(2, k)$-môđun hữu hạn chiều đều là một tổng trực tiếp của các môđun con đẳng cấu với các môđun $V(m)$.

Điều này suy ra từ Bổ đề 4 và các Mệnh đề 1, 2 và 3.

#### Nhận xét 1 {#lie-viii-s1-n3-rem-1 .statement tag=00Y3}

Biểu diễn kề của $\mathfrak{s}\mathfrak{l}(2, k)$ xác định trên $\mathfrak{s}\mathfrak{l}(2, k)$ cấu trúc của một $\mathfrak{s}\mathfrak{l}(2, k$)-môđun đơn. Môđun này đẳng cấu với V(2) bởi một đẳng cấu biến $u^2$ thành $X_+, 2uv$ thành $-H$, và $v^2$ thành $X_-$.

#### Nhận xét 2 {#lie-viii-s1-n3-rem-2 .statement tag=00Y4}

Với $n\geq 0$ và $m > n$,

$$
X_-e^{(m)}_n=-(m-n)(m)u^{m-n-1}v^{n+1}=-(n+ 1)e^{(m)}_{n+1}
$$

$$
n
$$

Do đó, $(e_0^{(m)}, e_1^{(m)}, . . . , e_m^{(m)})$ là cơ sở của $V(m)$ liên kết với phần tử nguyên thủy $e_0^{(m)}$.

#### Nhận xét 3 {#lie-viii-s1-n3-rem-3 .statement tag=00Y5}

Cho $\Phi$ là dạng song tuyến tính trên $V(m)$ sao cho

$\Phi (e^{(m)}_n, e^{(m)}_{n'}) = 0$ nếu $n+n'\not=m$

$$
\Phi (e^{(m)}_n, e^{(m)}_{m-n}) = (-1)^n(m)
$$

$$
n
$$

Nếu $x=au+bv$ và $y=cu+dv$, thì $\Phi (x^m, y^m) = (ad-bc)^m$. Giờ đây dễ kiểm tra rằng $\Phi$ là bất biến, và rằng $\Phi$ là đối xứng khi $m$ chẵn, và phản xứng khi $m$ lẻ.

#### Mệnh đề 4 {#lie-viii-s1-prop-4 .statement tag=00Y6}

Cho E là một $\mathfrak{s}\mathfrak{l}(2, k)$-môđun hữu hạn chiều, $m$ là một số nguyên $\geq 0$, $P_m$ là tập hợp các phần tử nguyên thủy có trọng số $m$. Gọi L là không gian vectơ các đồng cấu từ $\mathfrak{s}\mathfrak{l}(2, k)$-môđun $V(m)$ vào $\mathfrak{s}\mathfrak{l}(2, k)$-môđun E. Ánh xạ $f \rightarrow f(u^m)$ từ L vào E là tuyến tính, đơn ánh, và ảnh của nó là $P_m\cup  \{0\}$.

Ánh xạ này rõ ràng là tuyến tính, và nó là đơn ánh vì $u^m$ sinh ra $\mathfrak{s}\mathfrak{l}(2, k$)-môđun $V(m)$. Nếu $f\in L$,

$$
X_+(f(u^m)) =f(X_+u^m) = 0,H(f(u^m)) =f(Hu^m) =mf(u^m)
$$

do đó $f(u^m)\in P_m\cup  \{0\}$. Cho $e\in P_m$, và V là môđun con của E sinh bởi $e$. Theo Mệnh đề 1, tồn tại một đẳng cấu từ môđun $V(m)$ lên môđun V biến $u^m$ thành $e$. Khi đó $L(u^m) = P_m\cup  \{0\}$.

#### Hệ quả {#lie-viii-s1-n3-cor-1 .statement tag=00Y7}

Thành phần đẳng kiểu của E kiểu $V(m)$ có độ dài

dim(P$_m\cup  \{0\}$.

### 4. BIỂU DIỄN TUYẾN TÍNH CỦA NHÓM SL(2$\boldsymbol{, k}$)

Nhắc lại (Đại số, Chương III, §8, no. 9) rằng ta ký hiệu bởi $\mathbf{S}\mathbf{L}(2, k)$ nhóm các ma trận vuông cấp 2 với các hệ số trong $k$ có định thức bằng 1. Nếu $x\in \mathfrak{s}\mathfrak{l}(2, k)$ là lũy linh, thì $x^2= 0 ($Đại số, Chương VII, §5, Hệ quả 3 của Mệnh đề 5) và $e^x= 1 +x\in \mathbf{S}\mathbf{L}(2, k)$. Nếu E là một không gian vectơ hữu hạn chiều và $\rho$ là một biểu diễn tuyến tính của $\mathfrak{s}\mathfrak{l}(2, k)$ trên E, thì $\rho (x)$ là lũy linh và do đó $e^{\rho(x)}$ được xác định (Chương I, §6, no. 3).

#### Định nghĩa 2 {#lie-viii-s1-def-2 .statement tag=00Y8}

Cho E là một không gian vectơ hữu hạn chiều, và $\rho$ (resp. $\pi$ ) là một biểu diễn tuyến tính của $\mathfrak{s}\mathfrak{l}(2, k)$ (resp. $\mathbf{S}\mathbf{L}(2, k)$) trên E. Khi đó $\rho$ và $\pi$ được gọi là tương thích nếu, với mọi phần tử lũy linh $x$ của $\mathfrak{s}\mathfrak{l}(2, k),\pi (e^x) =e^{\rho(x)}$.

Nói cách khác, $\rho$ và $\pi$ là tương thích nếu, với mọi phần tử lũy linh $x$ của $\mathfrak{s}\mathfrak{l}(2, k)$, hạn chế của $\rho$ lên $kx$ tương thích với hạn chế của $\pi$ lên nhóm $1 +kx$ (Chap. VII, §3, no. 1).

Nếu $\rho$ và $\pi$ tương thích, thì các biểu diễn đối ngẫu, các lũy thừa tenxơ bậc $m$, và các lũy thừa đối xứng bậc $m$ của $\rho$ và $\pi$, tương ứng, cũng tương thích (Chap. VII, §5, no. 4, Bổ đề 1 (i) và (ii)). Tương tự đối với các biểu diễn cảm sinh bởi $\rho$ và $\pi$ trên một không gian con vectơ ổn định dưới $\rho$ và $\pi ($loc. cit.).

Đặc biệt, biểu diễn $\rho_m$ của $\mathfrak{s}\mathfrak{l}(2, k)$ trên $V(m)$ (no. 3) là tương thích với lũy thừa đối xứng thứ $m$ $\pi_m$ của biểu diễn đồng nhất $\pi_1$ của $\mathbf{S}\mathbf{L}(2, k)$. Đặt $e^{(m)}_n=(^m_n)u^{m-n}v^n$ như trên, ta có

$(m)(m)m-nn$

$\pi_m(s)e_n$ = $(su)(sv)$ (3)

$$
n
$$

với $s\in \mathbf{S}\mathbf{L}(2, k)$ và $0\leq n\leq m$.

#### Định lý 2 {#lie-viii-s1-thm-2 .statement tag=00Y9}

Cho $\rho$ là một biểu diễn tuyến tính của $\mathfrak{s}\mathfrak{l}(2, k)$ trên một không gian vectơ hữu hạn chiều E.

(i) Tồn tại một biểu diễn tuyến tính duy nhất $\pi$ của $\mathbf{S}\mathbf{L}(2, k)$ trên E tương thích với $\rho$.

(ii) Một không gian con vectơ F của E là ổn định dưới $\pi$ khi và chỉ khi nó ổn định dưới $\rho$.

(iii) Cho $x\in E$. Khi đó $\pi (s)x=x$ với mọi $s\in \mathbf{S}\mathbf{L}(2, k)$ khi và chỉ khi $x$ là bất biến dưới $\rho ($nghĩa là, $\rho (a)x= 0$ với mọi $a\in \mathfrak{s}\mathfrak{l}(2, k))$.

Sự tồn tại của $\pi$ suy ra từ điều trước và Đl. 1. Mặt khác, ta biết rằng nhóm $\mathbf{S}\mathbf{L}(2, k)$ được sinh bởi các phần tử có dạng

$$
_{tX}(1t)_{-tX_-}(10)
$$

$e^+=e$ =

0 1 $t$ 1

trong đó $t\in k($đại số, Chương III, §8, no. 9, Mệnh đề 17). Điều này chứng minh tính duy nhất của $\pi$.

Các khẳng định (ii) và (iii) suy ra từ những điều ta đã nói, cùng với Chương VII, §3, no. 1, Bổ đề 1 (i). C.Q.F.D.

Vì vậy, mọi $\mathfrak{s}\mathfrak{l}(2, k$)-môđun hữu hạn chiều đều có một cấu trúc môđun $\mathbf{S}\mathbf{L}(2, k)$ duy nhất, được gọi là liên kết với cấu trúc môđun $\mathfrak{s}\mathfrak{l}(2, k$) của nó.

#### Nhận xét {#lie-viii-s1-n4-rem-1 .statement tag=00YA}

Khi $k$ là $\mathbf{R}$ hoặc $\mathbf{C}$ hoặc một trường ultrametric đầy đủ không rời rạc, $\mathfrak{s}\mathfrak{l}(2, k)$ là đại số Lie của $\mathbf{S}\mathbf{L}(2, k)$. Cho $\rho$ và $\pi$ như trong Định lý 2. Đồng cấu $\pi$ là một đồng cấu các nhóm Lie từ $\mathbf{S}\mathbf{L}(2, k)$ đến $\mathbf{G}\mathbf{L}(E):$ điều này hiển nhiên khi $E = V(m)$, và trường hợp tổng quát suy ra theo Định lý 1. Theo Chương VII, §3, số $1,\rho (X_+) = L(\pi )(X_+),\rho (X_-) = L(\pi )(X_-)$. Do đó $\rho = L(\pi )$ (về đảo lại, xem Bài tập 18).

#### Mệnh đề 5 {#lie-viii-s1-prop-5 .statement tag=00YB}

Cho E, F là các $\mathfrak{s}\mathfrak{l}(2, k)$-môđun hữu hạn chiều, và cho $f\in$ Hom$_k(E,F)$. Các điều kiện sau là tương đương:

(i) $f$ là một đồng cấu của các $\mathfrak{s}\mathfrak{l}(2, k)$-môđun;

(ii) $f$ là một đồng cấu của các $\mathbf{S}\mathbf{L}(2, k)$-môđun.

Điều kiện (i) có nghĩa là $f$ là một phần tử bất biến của $\mathfrak{s}\mathfrak{l}(2, k$)-môđun Hom$_k(E,F)$, và điều kiện (ii) có nghĩa là $f$ là một phần tử bất biến của $\mathbf{S}\mathbf{L}(2, k$)-môđun Hom$_k(E,F)$. Vì các cấu trúc môđun này được liên kết bởi Chương VII, §5, no. 4, Bổ đề 1 (iii), mệnh đề suy ra từ Định lý 2 (iii).

#### Định nghĩa 3 {#lie-viii-s1-def-3 .statement tag=00YC}

Biểu diễn liên hợp của nhóm $\mathbf{S}\mathbf{L}(2, k)$ là biểu diễn tuyến tính Ad của $\mathbf{S}\mathbf{L}(2, k)$ trên $\mathfrak{s}\mathfrak{l}(2, k)$ được xác định bởi

Ad($s$)$.a=sas^{-1}$

với mọi $a\in \mathfrak{s}\mathfrak{l}(2, k)$ và mọi $s\in \mathbf{S}\mathbf{L}(2, k)$. Khi $k$ là $\mathbf{R}$ hoặc $\mathbf{C}$ hoặc một trường ultrametric đầy đủ không rời rạc, ta thu lại Định nghĩa 7 của Chương III, §3, no. 12 (xem loc. cit., Mệnh đề 49).

Theo Chương VII, §5, no. 4, Bổ đề 1 (i) và (ii), các biểu diễn liên hợp của $\mathfrak{s}\mathfrak{l}(2, k)$ và $\mathbf{S}\mathbf{L}(2, k)$ là tương thích. Theo Chương VII, §3, no. 1, Nhận xét 2, Ad($\mathbf{S}\mathbf{L}(2, k)$) $=$ Aut$_e(\mathfrak{s}\mathfrak{l}(2, k))$.

### 5. MỘT SỐ PHẦN TỬ CỦA SL(2$\boldsymbol{, k}$)

Với mọi $t\in k^*$, đặt

$$
\theta (t) =e^{tX_+}e^{t^{-1}X_-}e^{tX_+}
$$

$(1t)(($ 1 $0)((1t)$

= 0 1 $-t^{-1}$ 1 0 1

$($ 0 t)

= $-t^{-1}$ 0

$$
=e^{t^{-1}X_-}e^{tX_+}e^{t^{-1}X_-}
$$

Với các ký hiệu của no. 3,

$$
\theta (t)u=-t^{-1}v\theta (t)v=tu
$$

nên

$$
\theta (t)e^{(m)}_n= (-1)^{m-n}t^{2n-m}e^{(m)}_{m-n} \tag{4}
$$

Do đó, phần tử $\theta (t)^2=(-1$ 0 $)$ tác động bởi $(-1)^m$ trên $V(m)$. Nếu

0 $-1$

E là một $\mathfrak{s}\mathfrak{l}(2, k$)-môđun đơn có chiều lẻ, thì $\theta (t)_E$ do đó là một tự đẳng cấu đối hợp của không gian vectơ E. Đặc biệt, lấy E là biểu diễn liên hợp:

$$
\theta (t)_EX_+=t^{-2}X_-\theta (t)_EX_-=t^2X_+\theta (t)_EH=-H \tag{5}
$$

suy ra $\theta (1)_E=\theta (-1)_E$ là phép đối hợp chính tắc của $\mathfrak{s}\mathfrak{l}(2, k)$.

Với mọi $t\in k^*$, đặt

$$
h(t) =(0tt^-0_1)=\theta (t)\theta (-1)
$$

Khi đó $h(t)u=tu,h(t)v=t^{-1}v$, nên

$$
h(t)e^{(m)}_n=t^{m-2n}e^{(m)}_n \tag{6}
$$

#### Mệnh đề 6 {#lie-viii-s1-prop-6 .statement tag=01L4}

Cho E là một $\mathfrak{s}\mathfrak{l}(2, k)$-môđun hữu hạn chiều, và $t\in k^*$. Gọi $E_p$ là tập hợp các phần tử của E có trọng số $p$.

(i) $\theta (t)_E|E_p$ là một song ánh từ $E_p$ lên $E_{-p}$.

(ii) $h(t)_E|E_p$ là phép vị tự có tỷ số $t^p$ trên $E_p$.

Nếu $E = V(n)$, mệnh đề suy ra từ các công thức (4) và (6). Trường hợp tổng quát suy ra từ Định lý 1.

#### Hệ quả {#lie-viii-s1-n5-cor-1 .statement tag=00YD}

Cho $E = E'\oplus E''$ là phân tích của E được xác định trong Hệ quả của Mệnh đề 2. Phần tử $(-10)$ của $\mathbf{S}\mathbf{L}(2, k)$ tác động như +1 trên $E'$

0 $-1$

và bởi $-1$ trên $E''$.

Điều này suy ra từ (ii), áp dụng cho $t=-1$.

### Bài tập {#lie-viii-s1-exercises}

Trường cơ sở $k$ được giả thiết có đặc số không.

Trừ khi có phát biểu tường minh ngược lại, các đại số Lie được giả thiết là hữu hạn chiều.

Ta ký hiệu bởi $\mathfrak{s}$ đại số Lie $\mathfrak{s}\mathfrak{l}(2, k)$.

Xem [các bài tập của § 1](exercises/s1/).
