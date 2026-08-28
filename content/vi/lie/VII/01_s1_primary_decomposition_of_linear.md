---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VII
chapter_title: CARTAN SUBALGEBRAS AND REGULAR ELEMENTS
section: 1
section_title: Primary decomposition of linear representations
lang: vi
source: lie-vii-ix
book_pages: 1-12, 51-55
pdf_pages: 0011-0022, 0060-0064
extraction: native
subsections:
    - "no": 1
      title: DECOMPOSITION OF A FAMILY OF ENDOMORPHISMS
      page: 1
      pdf_page: 11
    - "no": 2
      title: THE CASE OF A LINEAR FAMILY OF ENDOMORPHISMS
      page: 6
      pdf_page: 16
    - "no": 3
      title: DECOMPOSITION OF REPRESENTATIONS OF A NILPOTENT LIE ALGEBRA
      page: 8
      pdf_page: 18
    - "no": 4
      title: DECOMPOSITION OF A LIE ALGEBRA RELATIVE TO AN AUTOMORPHISM
      page: 11
      pdf_page: 21
    - "no": 5
      title: INVARIANTS OF A SEMI-SIMPLE LIE ALGEBRA RELATIVE TO A SEMI-SIMPLE ACTION
      page: 11
      pdf_page: 21
statements: 25
exercises: 11
content_sha256: 15a77d0b314a0b2f47512590bd3e203e835e4f71404ae0e3e4a510bd5fa5fa2a
translated_from: content/en/lie/VII/01_s1_primary_decomposition_of_linear.md
source_content_sha256: 6b3a7f44b594659cd25df9f6c944977706304b56c54522de1260ddcaf18891f2
translation_model: gpt-5-6-mini, gpt-5.4-mini
translation_run: translate-vi-6af4f374
glossary_version: 34
glossary_terms_sha256: 0b72c17aa52c5c5ea3f034d2b67374064b56558c9298b7ca09dfc31a9e4eec17
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 1. PHÂN TÍCH NGUYÊN SƠ CỦA CÁC BIỂU DIỄN TUYẾN TÍNH

### 1. PHÂN TÍCH MỘT HỌ CÁC TOÁN TỬ KẾT THÚC

Cho V là một không gian vectơ, S là một tập hợp, và $r$ là một ánh xạ từ S vào End(V). Ký hiệu P là tập hợp các ánh xạ từ S vào $k$. Nếu $\lambda \in P$, ký hiệu $V_{\lambda}(S)$ (tương ứng $V^{\lambda}(S)$) là tập hợp các $v\in V$ sao cho, với mọi $s\in S,r(s)v=\lambda (s)v$ (tương ứng $(r(s)-\lambda (s))^nv= 0$ với $n$ đủ lớn). Các tập hợp $V_{\lambda}(S)$ và $V^{\lambda}(S)$ là các không gian vectơ con của V, và $V_{\lambda}(S)\subset V^{\lambda}(S)$. Ta nói rằng $V_{\lambda}(S)$ là không gian riêng của V tương ứng với $\lambda$ (và với $r$), rằng $V^{\lambda}(S)$ là không gian con nguyên sơ của V tương ứng với $\lambda$ (và với $r$), và rằng $V^0(S)$ là không gian lũy linh của V (tương ứng với $r$). Ta nói rằng $\lambda$ là một trọng số của S trong V nếu $V^{\lambda}(S)\not= 0$.

Đặc biệt, nếu S thu gọn thành một phần tử duy nhất $s, P$ có thể được đồng nhất với $k$; ta dùng các ký hiệu $V_{\lambda(s)}(s)$ và $V^{\lambda(s)}(s)$, hoặc $V_{\lambda(s)}(r(s))$ và $V^{\lambda(s)}(r(s))$, thay cho $V_{\lambda}(\{s\}), V^{\lambda}(\{s\})$; ta nói đến các không gian riêng, các không gian con nguyên sơ và không gian lũy linh của $r(s)$; một phần tử $v$ của $V_{\lambda(s)}(s)$ được gọi là một vectơ riêng của $r(s)$, và, nếu $v\not= 0,\lambda (s)$ được gọi là trị riêng tương ứng (xem Đại số, Chương VII, §5).

Với mọi $\lambda \in P$, các hệ thức sau là ngay lập tức:

$$
V^{\lambda}(S) =\bigcap_{s\in S}V^{\lambda(s)}(s) \tag{1}
$$

$$
V_{\lambda}(S) =\bigcap_{s\in S}V_{\lambda(s)}(s) \tag{2}
$$

Cho $k'$ là một mở rộng của $k$. Ánh xạ chính tắc từ End(V) vào End($V\otimes_kk'$) cho, bằng hợp thành với $r$, một ánh xạ $r': S\rightarrow$ End($V\otimes_kk'$). Tương tự, mỗi ánh xạ $\lambda$ từ S vào $k$ xác định một cách chính tắc một ánh xạ, cũng ký hiệu là $\lambda$, từ S vào $k'$. Với các ký hiệu này, ta có mệnh đề sau:

#### Mệnh đề 1 {#lie-vii-s1-prop-1 .statement tag=00SJ}

Với mọi $\lambda \in P$,

$(V\otimes_kk')^{\lambda}(S) = V^{\lambda}(S)\otimes_kk'$ và $(V\otimes_kk')_{\lambda}(S) = V_{\lambda}(S)\otimes_kk'$.

Cho $(a_i)$ là một cơ sở của không gian vectơ $k$-vectơ $k'$. Nếu $v\in V\otimes_kk',v$ có thể được biểu diễn duy nhất dưới dạng $\sum v_i\otimes a_i$ trong đó $(v_i)$ là một họ hữu hạn phần tử của V có giá hữu hạn. Với mọi $s\in S$,

$$
(r'(s)-\lambda (s))^n(v) =\sum(r(s)-\lambda (s))^nv_i\otimes a_i
$$

Suy ra rằng

$v\in (V\otimes_kk')^{\lambda}(S)\Leftarrow \Rightarrow v_i\in V^{\lambda}(S)$ với mọi $i$,

$v\in (V\otimes_kk')_{\lambda}(S)\Leftarrow \Rightarrow v_i\in V_{\lambda}(S)$ với mọi $i$,

suy ra mệnh đề.

#### Mệnh đề 2 {#lie-vii-s1-prop-2 .statement tag=00SK}

Cho $V,V',W$ là các không gian vectơ. Cho $r$ : S $\rightarrow$ End(V), $r': S\rightarrow$ End(V$'$) và $q: S\rightarrow$ End(W) là các ánh xạ.

(i) Cho $f: V\rightarrow W$ là một ánh xạ tuyến tính sao cho $q(s)f(v) =f(r(s)v)$ với $s\in S$ và $v\in V$. Khi đó, với mọi $\lambda \in P,f$ biến $V^{\lambda}(S)$ (tương ứng $V_{\lambda}(S)$) vào $W^{\lambda}(S)$ (tương ứng $W_{\lambda}(S)$).

(ii) Cho $B : V\times V'\rightarrow W$ là một ánh xạ song tuyến tính sao cho

$$
q(s)B(v, v') = B(r(s)v, v') + B(v, r'(s)v')
$$

với $s\in S,v\in V,v'\in V'$. Khi đó, với mọi $\lambda , \mu\in P$, B biến $V^{\lambda}(S)\times {V'}^\mu(S)$ (tương ứng $V_{\lambda}(S)\times V'_\mu(S)$) vào $W^{\lambda+\mu}(S)$ (tương ứng $W_{\lambda+\mu}(S)$).

(iii) Cho $B : V\times V'\rightarrow W$ là một ánh xạ song tuyến tính sao cho

$$
q(s)B(v, v') = B(r(s)v, r'(s)v')
$$

với $s\in S,v\in V,v'\in V'$. Khi đó, với mọi $\lambda , \mu\in P$, B biến $V^{\lambda}(S)\times {V'}^\mu(S)$ (tương ứng $V_{\lambda}(S)\times V'_\mu(S)$) vào $W^{\lambda \mu}(S)$ (tương ứng $W_{\lambda \mu}(S)$).

Trong trường hợp (i), $(q(s)-\lambda (s))^nf(v) =f((r(s)-\lambda (s))^nv)$ với $s\in S$ và $v\in V$, do đó có kết luận. Trong trường hợp (ii),

$$
(q(s)-\lambda (s)-\mu(s))B(v, v') = B((r(s)-\lambda (s))v, v') + B(v,(r'(s)-\mu(s))v')
$$

với $s\in S,v\in V,v'\in V'$, do đó bằng quy nạp theo $n$

$$
'(n)''
$$

$(q(s)-\lambda (s)-\mu(s))^nB(v, v) =\sum B((r(s)-\lambda (s))^iv,(r(s)-\mu(s))^jv)$.

$$
i
$$

$i+j=n$

Các mệnh đề trong (ii) suy ra ngay lập tức. Trong trường hợp (iii), $(q(s)-\lambda (s)\mu(s))B(v, v') = B((r(s)-\lambda (s))v, r'(s)v')+B(\lambda (s)v,(r'(s)-\mu(s))v')$ với $s\in S,v\in V,v'\in V'$, do đó bằng quy nạp theo $n$

$$
(q(s)-\lambda (s)\mu(s))^nB(v, v')
$$

= $\sum(n)B(\lambda (s)^j(r(s)-\lambda (s))^iv, r'(s)^i(r'(s)-\mu(s))^jv')$.

$$
i
$$

$i+j=n$

Các mệnh đề trong (iii) suy ra ngay lập tức.

#### Mệnh đề 3 {#lie-vii-s1-prop-3 .statement tag=00SL}

Tổng $\sum_{\lambda\in P}V^{\lambda}(S)$ là trực tiếp. Tổng $\sum_{\lambda\in P}V_{\lambda}(S)$ là trực tiếp.

Mệnh đề thứ hai là hệ quả của mệnh đề thứ nhất; do đó chỉ cần chứng minh điều đó. Ta phân biệt một số trường hợp.

$a) S$ là rỗng. Mệnh đề là tầm thường.

$b) S$ được thu gọn còn một phần tử duy nhất $s$. Cho $\lambda_0, \lambda_1, . . . , \lambda_n$ là các phần tử phân biệt của $k$. Với $i= 0,1, . . . , n$, cho $v_i\in V^{\lambda_i}(s)$ và giả sử rằng $v_0=v_1+\cdots +v_n$. Chỉ cần chứng minh rằng $v_0$ = 0. Với $i= 0, . . . , n$, tồn tại một số nguyên $q_i>$ 0 sao cho $(r(s)-\lambda_i)^{q_i}v_i$ = 0. Xét các đa thức $P(X) =\prod_{i\geq 1}(X-\lambda_i)^{q_i}$ và $Q(X) = (X-\lambda_0)^{q_0}$. Ta có $Q(r(s))v_0= 0$, và

$P(r(s))v_0=\sum_{i=1}^nP(r(s))v_i= 0$. Vì P và Q nguyên tố cùng nhau, đẳng thức Bezout chứng minh rằng $v_0= 0$.

$c) S$ là hữu hạn và không rỗng. Ta chứng minh bằng quy nạp theo lực lượng của S. Cho $s\in S$ và $S'= S$**--** $\{s\}$. Cho $(v_{\lambda})_{\lambda\in P}$ là một họ có giá đỡ hữu hạn của các phần tử của V sao cho $\sum_{\lambda\in P}v_{\lambda}= 0$ và $v_{\lambda}\in V^{\lambda}(S)$. Cho $\lambda_0\in P$. Cho $P'$ là tập các $\lambda \in P$ sao cho $\lambda |S'=\lambda_0|S'$. Theo giả thiết quy nạp áp dụng cho $S'$, ta có $\sum_{\lambda\in P'}v_{\lambda}= 0$. Nếu $\lambda , \mu$ là các phần tử phân biệt của $P'$, thì $\lambda (s)\not=\mu(s)$.

Vì tổng $\sum_{\alpha\in k}V^{\alpha}(s)$ là trực tiếp theo $b)$, và vì $v_{\lambda}\in V^{\lambda(s)}(s)$, suy ra $v_{\lambda}= 0$ với mọi $\lambda \in P'$, và đặc biệt $v_{\lambda_0}= 0$, điều phải chứng minh.

$d)$ Trường hợp tổng quát. Cho $(v_{\lambda})_{\lambda\in P}$ là một họ có giá đỡ hữu hạn của các phần tử của V sao cho $\sum_{\lambda\in P}v_{\lambda}= 0$ và $v_{\lambda}\in V^{\lambda}(S)$. Cho $P'$ là tập hữu hạn các $\lambda \in P$ sao cho $v_{\lambda}\not= 0$, và cho $S'$ là một tập con hữu hạn của S sao cho các điều kiện $\lambda \in P'$, $\mu\in P',\lambda |S'=\mu|S'$ suy ra rằng $\lambda =\mu$. Ta có $v_{\lambda}\in V^{\lambda|S'}(S')$; áp dụng $c)$, ta thấy rằng $v_{\lambda}= 0$ với $\lambda \in P'$, điều đó hoàn tất chứng minh.

Nhắc lại rằng, nếu $x\in$ End(V), ta ký hiệu ad $x$ là ánh xạ $y \rightarrow xy-yx= [x, y]$ từ End(V) vào chính nó.

#### Bổ đề 1 {#lie-vii-s1-lem-1 .statement tag=00SM}

Cho $x, y\in$ End(V).

(i) Giả sử rằng V hữu hạn chiều. Khi đó $x$ tam giác hóa được khi và chỉ khi $V =\sum_{a\in k}V^a(x)$.

(ii) Nếu tồn tại một số nguyên $n$ sao cho (ad $x$)$^ny= 0$, thì mỗi $V^a(x)$ đều ổn định dưới $y$.

(iii) Giả sử V hữu hạn chiều. Nếu $V =\sum_{a\in k}V^a(x)$ và nếu mỗi

$V^a(x)$ đều ổn định dưới $y$, thì tồn tại một số nguyên $n$ sao cho (ad $x$)$^ny= 0$.

Phần (i) suy ra từ Algebra, Chương VII, §5, no. 2, Mệnh đề 3.

Đặt E = End(V). Gọi B là ánh xạ song tuyến tính $(u, v) \rightarrow u(v)$ từ $E\times V$ đến V. Theo định nghĩa của ad $x$,

$x(B(u, v)) =B(u, x(v)) +$ B((ad $x$)$(u), v$)

với $x\in E,u\in E,v\in V$. Cho $x$ tác động lên E qua ad $x$. Theo Mệnh đề 2 (ii), $B(E^0(x),V^a(x))\subset V^a(x)$ với mọi $a\in k$. Nếu (ad $x$)$^ny= 0$, thì $y\in E^0(x)$, do đó $y(V^a(x))\subset V^a(x)$, điều này chứng minh (ii).

Để chứng minh (iii), ta có thể thay V bởi $V^a(x)$ và thay $x$ (tương ứng $y$) bởi hạn chế của nó trên $V^a(x)$. Thay $x$ bởi $x-a$, ta có thể giả sử rằng $x$ là lũy linh. Khi đó, (ad $x$)$^{2 dim V-1}= 0$ (Chương I, §4, no. 2), điều này chứng minh (iii).

#### Nhận xét {#lie-vii-s1-n1-rem-1 .statement tag=00SN}

Lập luận chứng minh rằng, nếu V hữu hạn chiều và nếu tồn tại một số nguyên $n$ sao cho (ad $x$)$^ny= 0$, thì (ad $x$)$^{2 dim V-1}y= 0$.

Sau đây, ta sẽ nói rằng ánh xạ $r: S\rightarrow$ End(V) thỏa mãn điều kiện (AC) (“gần giao hoán”) nếu:

(AC) Với mọi cặp $(s, s')$ của các phần tử của S, tồn tại một số nguyên $n$ sao cho

(ad $r(s)$)$^nr(s') = 0$.

#### Định lý 1 {#lie-vii-s1-thm-1 .statement tag=00SO}

Giả sử V hữu hạn chiều. Các điều kiện sau là tương đương:

(i) Điều kiện (AC) được thỏa mãn và, với mọi $s\in S,r(s)$ là khả tam giác hóa.

(ii) Với mọi $\lambda \in P$, $V^{\lambda}(S)$ ổn định dưới $r(S)$, và $V =\sum_{\lambda\in P}V^{\lambda}(S)$.

Nếu $V =\sum_{\lambda\in P}V^{\lambda}$(S), thì $V =\sum_{a\in k}V^a(s)$ với mọi $s\in S$, và suy ra từ Bổ đề 1 rằng (ii) kéo theo (i). Giả sử điều kiện (i) được thỏa mãn. Bổ đề 1 và công thức (1) suy ra rằng mỗi $V^{\lambda}(S)$ đều ổn định dưới $r(S)$. Còn phải chứng minh rằng $V =\sum_{\lambda\in P}V^{\lambda}(S)$. Ta chứng minh bằng quy nạp theo dim V. Ta phân biệt hai trường hợp.

$a)$ Với mọi $s\in S,r(s)$ có một trị riêng duy nhất $\lambda (s)$. Khi đó $V = V^{\lambda}(S)$.

$b)$ Tồn tại $s\in S$ sao cho $r(s)$ có ít nhất hai giá trị riêng phân biệt. Khi đó V là tổng trực tiếp của các $V^a(s)$ với $a\in k$, và dim $V^a(s)<$ dim V với mọi $a$. Mỗi $V^a(s)$ đều ổn định dưới $r$(S), và chỉ cần áp dụng giả thiết quy nạp.

#### Hệ quả 1 {#lie-vii-s1-thm-1-cor-1 .statement tag=00SP}

Giả sử rằng V hữu hạn chiều và điều kiện (AC) được thỏa mãn. Cho $k'$ là một mở rộng của $k$. Giả sử rằng, với mọi $s\in S$, tự đồng cấu $r(s)\otimes 1$ của $V\otimes_kk'$ là khả tam giác hóa. Cho $P'$ là tập hợp các ánh xạ từ S đến $k'$. Khi đó $V\otimes_kk'=\sum_{\lambda'\in P'}(V\otimes_kk')^{\lambda'}(S)$.

Cho $r': S\rightarrow$ End(V$\otimes_kk'$) là ánh xạ được xác định bởi $r$. Nếu $s_1, s_2\in S$, tồn tại một số nguyên $n$ sao cho (ad $r(s_1)$)$^nr(s_2) = 0$, do đó (ad $r'(s_1)$)$^nr'(s_2) = 0$. Bây giờ chỉ cần áp dụng Định lý 1.

#### Hệ quả 2 {#lie-vii-s1-thm-1-cor-2 .statement tag=00SQ}

Giả sử rằng V hữu hạn chiều và điều kiện (AC) được thỏa mãn. Ký hiệu $V^+(S)$ là không gian con vectơ $\sum_{s\in S}((\bigcap_{i\geq 1}r(s)^iV)$. Khi đó:

(i) $V^0(S)$ và $V^+(S)$ đều ổn định dưới $r(S)$;

(ii) $V = V^0(S)\oplus V^+(S)$;

(iii) mọi không gian con vectơ W của V, ổn định dưới $r(S)$ và thỏa $W^0(S) = 0$, đều được chứa trong $V^+(S)$;

(iv) $\sum_{s\in S}r(s)V^+(S) = V^+(S)$.

Hơn nữa, $V^+(S)$ là không gian con vectơ duy nhất của V có các tính chất (i) và (ii). Với mọi mở rộng $k'$ của $k,(V\otimes_kk')^+(S) = V^+(S)\otimes_kk'$.

Khẳng định cuối cùng là hiển nhiên. Do đó, xét đến Mệnh đề 1, khi chứng minh các mệnh đề còn lại ta có thể giả sử rằng $k$ đóng đại số. Theo Định lý 1, V = $\sum_{\lambda\in P}V^{\lambda}$(S), và các $V^{\lambda}(S)$ đều ổn định dưới $r(S)$. Nếu $s\in S$, đa thức

đặc trưng của $r(s)|V^{\lambda}(S)$ là $(X-\lambda (s))^{dim V^{\lambda}(S)}$; suy ra rằng $\bigcap_{i\geq 1}r(s)^iV^{\lambda}(s)$

là không nếu $\lambda (s) = 0$ và bằng $V^{\lambda}(S)$ nếu $\lambda (s)\not= 0$; do đó,

$$
V^+(S) =\sum_{\lambda\in P,\lambda\not=0}V^{\lambda}(S) \tag{3}
$$

điều này chứng minh (i), (ii) và (iv). Nếu W là một không gian con vectơ của V ổn định dưới $r$(S), thì $W =\sum_{\lambda\in P}W^{\lambda}(S)$ và $W^{\lambda}(S) = W\cap V^{\lambda}(S)$. Nếu $W^0(S) = 0$, ta thấy rằng $W\subset V^+$(S), điều này chứng minh (iii).

Cho $V'$ là một không gian con của V ổn định dưới $r(S)$ và sao cho $V'\cap V^0(S) = 0$. Khi đó ${V'}^0(S) = 0$, nên $V'\subset V^+(S)$ theo (iii). Nếu, thêm nữa, $V = V^0(S) + V'$, ta thấy rằng $V'= V^+(S)$. Q.E.D.

Đôi khi ta gọi $(V^0(S),V^+(S))$ là phân rã Fitting của V, hay của ánh xạ $r: S\rightarrow$ End(V). Nếu S chỉ còn một phần tử $s$, ta viết $V^+(s)$ hoặc $V^+(r(s))$ thay cho $V^+(\{s\})$. Ta có $V = V^0(s)\oplus V^+(s), V^0(s)$ và $V^+(s)$ ổn định dưới $r(s),r(s)|V^0(s)$ là lũy linh và $r(s)|V^+(s)$ là song ánh.

#### Hệ quả 3 {#lie-vii-s1-thm-1-cor-3 .statement tag=00SR}

Cho V và $V'$ là các không gian vectơ hữu hạn chiều, và cho $r: S\rightarrow$ End(V) và $r': S\rightarrow$ End(V$'$) là các ánh xạ thỏa mãn điều kiện (AC). Cho $f: V\rightarrow V'$ là một ánh xạ tuyến tính toàn ánh sao cho $f(r(s)v) =r'(s)f(v)$ với $s\in S$ và $v\in V$. Khi đó $f(V^{\lambda}{(S)) = V'}^{\lambda}(S)$ với mọi $\lambda \in P$.

Theo Mệnh đề 1, ta quy về trường hợp $k$ là đóng đại số. Ta có $V =\bigoplus_{\lambda\in P}V^{\lambda}$(S), $V'=\bigoplus_{\lambda\in P}{V'}^{\lambda}(S)$ theo Định lý 1, và $V'=f(V) =$ $\sum_{\lambda\in P}f(V^{\lambda}(S))$. Cuối cùng, $f(V^{\lambda}(S))\subset {V'}^{\lambda}(S)$ theo Mệnh đề 2 (i), suy ra hệ quả.

#### Mệnh đề 4 {#lie-vii-s1-prop-4 .statement tag=00SS}

Giả sử rằng $k$ là hoàn hảo. Cho V là một không gian vectơ hữu hạn chiều, $u$ là một phần tử của End(V)$,u_s, u_n$ là các thành phần nửa đơn và lũy linh của $u($Đại số, Chương VII, §5, no. 8).

(i) Với mọi $\lambda \in k,V^{\lambda}(u) = V^{\lambda}(u_s) = V_{\lambda}(u_s)$.

(ii) Nếu V có cấu trúc đại số và nếu $u$ là một đạo hàm của V$,u_s$ và $u_n$ là các đạo hàm của V.

(iii) Nếu V có cấu trúc đại số và nếu $u$ là một tự đẳng cấu của V, thì $u_s$ và $1 +u^{-1}_su_n$ là các tự đẳng cấu của V.

Theo Mệnh đề 1, ta có thể giả sử rằng $k$ là đóng đại số, nên

$$
V =\sum_{\lambda\in k}V^{\lambda}(u)
$$

Thành phần nửa đơn của $u|V^{\lambda}(u)$ là phép vị tự với tỉ số $\lambda$ trên $V^{\lambda}(u)$. Điều đó chứng minh (i).

Từ đây giả sử rằng V có cấu trúc đại số. Cho $x\in V^{\lambda}(u)$, $y\in V^\mu(u)$.

Nếu $u$ là một đạo hàm của V, thì $xy\in V^{\lambda+\mu}(u)$ (Mệnh đề 2 (ii)), nên

$$
u_s(xy) = (\lambda +\mu)(xy) = (\lambda x)y+x(\mu y) = (u_sx)y+x(u_sy)
$$

Điều đó chứng minh rằng $u_s$ là một đạo hàm của V. Khi đó $u_n=u-u_s$ là một đạo hàm của V.

Nếu $u$ là một tự đẳng cấu của V, Ker($u_s$) $= V^0(u) = 0$, nên $u_s$ là song ánh. Mặt khác, $xy\in V^{\lambda \mu}(u)$ (Mệnh đề 2 (iii)), nên

$$
u_s(xy) = (\lambda \mu)(xy) = (\lambda x)(\mu y) =u_s(x).u_s(y)
$$

Điều này chứng tỏ rằng $u_s$ là một tự đẳng cấu của V; nhưng khi đó thì

$$
1 +u^{-1}_su_n=u^{-1}_su
$$

### 2. TRƯỜNG HỢP CỦA MỘT HỌ TUYẾN TÍNH CÁC TỰ ĐỒNG CẤU

Giả sử bây giờ rằng S có cấu trúc không gian vectơ, rằng ánh xạ $r: S\rightarrow$ End(V) là tuyến tính, và rằng V và S là hữu hạn chiều.

#### Mệnh đề 5 {#lie-vii-s1-prop-5 .statement tag=00ST}

Giả sử điều kiện (AC) được thỏa mãn, và cho $\lambda : S\rightarrow k$ sao cho $V^{\lambda}(S)\not= 0$. Nếu $k$ có đặc số 0, ánh xạ $\lambda$ là tuyến tính. Nếu $k$ có đặc số $p\not= 0$, tồn tại một lũy thừa $q$ của $p$ chia hết chiều của $V^{\lambda}(S)$, và một hàm đa thức thuần nhất $P : S\rightarrow k$ bậc $q$, sao cho $\lambda (s)^q= P(s)$ với mọi $s\in S$.

Vì $V^{\lambda}(S)$ ổn định dưới $r(S)$ (Bổ đề 1 và công thức (1) của no. 1), ta có thể giả sử rằng $V = V^{\lambda}(S)$. Cho $n=$ chiều của V. Do đó, với $s\in S$,

det(X $-r(s)$) $= (X-\lambda (s))^n$.

Mặt khác, khai triển của định thức cho thấy rằng

det(X $-r(s)$) $= X^n+a_1(s)X^{n-1}+\cdots +a_i(s)X^{n-i}+\cdots$

trong đó $a_i: S\rightarrow k$ là một hàm đa thức thuần nhất bậc $i$. Viết $n=qm$ trong đó $q$ là một lũy thừa của số mũ đặc số của $k$ và $(q, m) = 1$. Khi đó $(X-\lambda (s))^n= (X^q-\lambda (s)^q)^m$; suy ra $-m\lambda (s)^q=a_q(s)$, điều này chứng tỏ kết quả.

#### Mệnh đề 6 {#lie-vii-s1-prop-6 .statement tag=00SU}

Giả sử rằng $k$ là vô hạn và điều kiện (AC) được thỏa mãn. Cho $k'$ là một mở rộng của $k$. Đặt $V'= V\otimes_kk',S'= S\otimes_kk'$. Cho $r': S'\rightarrow$ End(V$'$) là ánh xạ thu được từ $r$ bằng mở rộng vô hướng. Khi đó

$$
V^0(S)\otimes_kk'{= V'}^0{(S) = V'}^0(S')
$$

Đẳng thức thứ nhất suy ra từ Mệnh đề 1. Để chứng minh đẳng thức thứ hai, ta có thể giả sử rằng $V = V^0(S)$ và do đó $V'{= V'}^0(S)$. Cho $(s_1, . . . , s_m)$ là một cơ sở của S và $(e_1, . . . , e_n)$ là một cơ sở của V. Tồn tại các đa thức $P_{ij}(X_1, . . . ,X_m)$ sao cho

$$
r'(a_1s_1+\cdots +a_ms_m)^ne_j=\sum_{i=1}^nP_{ij}(a_1, . . . , a_m)e_i
$$

với $1\leq j\leq n$ và $a_1, . . . , a_m\in k'$. Theo giả thiết, $r'(s)^n= 0$ với mọi $s\in S$, nói cách khác $P_{ij}(a_1, . . . , a_m) = 0$ với $1\leq i, j\leq n$ và $a_1, . . . , a_m\in k$. Vì $k$ là vô hạn, $P_{ij}= 0$. Do đó, mọi phần tử của $r'(S')$ đều lũy linh và $V'{= V'}^0(S')$.

#### Mệnh đề 7 {#lie-vii-s1-prop-7 .statement tag=00SV}

Giả sử rằng $k$ là vô hạn và điều kiện (AC) được thỏa mãn. Gọi $\widetilde{S}$ là tập hợp các $s\in S$ sao cho $V^0(s) = V^0(S)$. Nếu $s\in S$, gọi $P(s)$ là định thức của tự đồng cấu của $V/V^0(S)$ do $r(s)$ xác định (no. 1, Hệ quả 2 (i) của Định lý 1).

(i) Hàm $s \rightarrow P(s)$ là đa thức trên S. Ta có $\widetilde{S} =\{s\in S|P(s)\not= 0\}$; đây là một tập con mở của S trong tôpô Zariski (App. 1).

(ii) $\widetilde{S}$ không rỗng, và $V^+(s) = V^+(S)$ với mọi $s\in \widetilde{S}$.

Việc $s \rightarrow P(s)$ là đa thức suy ra từ tính tuyến tính của $r$. Nếu $s\in S, V^0(s)\supset V^0$(S), với đẳng thức khi và chỉ khi $r(s)$ xác định một tự đẳng cấu của $V/V^0$(S), suy ra (i).

Bây giờ cho $k'$ là một bao đóng đại số của $k$, và giới thiệu $V',S', r'$ như trong Mệnh đề 6. Chúng ta nhận xét rằng $S'$ thỏa mãn điều kiện (AC) nhờ tiếp tục đẳng thức đa thức (ad $r(s_1)$)$^{2 dim V-1}r(s_2) = 0$ đúng với $s_1, s_2\in S$ (no. 1, Nhận xét ). Áp dụng Định lý 1, ta suy ra một phân tích

$$
V'{= V'}^0(S')\oplus \sum_{i=1}^m{V'}^{\lambda_i}(S')
$$

với $\lambda_i\not= 0$ cho $1\leq i\leq m$. Với $1\leq i\leq m$, tồn tại một hàm đa thức $P_i$ không bằng 0 trên $S'$ và một số nguyên $q_i$ sao cho $\lambda^{q_i}_i= P_i$ (Mệnh đề 5). Vì $k$ là vô hạn, tồn tại $s\in S$ sao cho $(P_1. . .P_m)(s)\not= 0$, xem Đại số, Chương IV, §2, no. 3, Hệ quả 2 của Mệnh đề 9. Khi đó $\lambda_i(s)\not= 0$ với mọi $i$, nên ${V'}^0(S'{) = V'}^0(s)$ và do đó $V^0(S) = V^0(s)$ (Mệnh đề 6), điều này cho thấy rằng $\widetilde{S}\not=\emptyset$. Nếu $s\in \widetilde{S}$, việc $V^+(S)$ ổn định dưới $r(s)$ và là một phần bù của $V^0(s)$ trong V suy ra rằng $V^+(S) = V^+(s)$ (Hệ quả 2 của Định lý 1).

### 3. PHÂN TÍCH CÁC BIỂU DIỄN CỦA MỘT ĐẠI SỐ LIE LŨY LINH

Cho $\mathfrak{h}$ là một đại số Lie và M là một $\mathfrak{h}$-môđun. Với mọi ánh xạ $\lambda$ từ $\mathfrak{h}$ đến $k$, ta đã định nghĩa ở no. 1 các không gian con vectơ $M^{\lambda}(\mathfrak{h})$ và $M_{\lambda}(\mathfrak{h})$ của M. Đặc biệt, nếu $\mathfrak{g}$ là một đại số Lie chứa $\mathfrak{h}$ như một đại số con, và nếu $x\in \mathfrak{g}$, ta thường dùng các ký hiệu $\mathfrak{g}^{\lambda}(\mathfrak{h})$ và $\mathfrak{g}_{\lambda}(\mathfrak{h})$; khi đó hiểu rằng $\mathfrak{h}$ tác động lên $\mathfrak{g}$ qua biểu diễn kề ad$_{\mathfrak{g}}$.

#### Mệnh đề 8 {#lie-vii-s1-prop-8 .statement tag=00SW}

Cho $\mathfrak{h}$ là một đại số Lie, và $L,M,N\mathfrak{h}$-môđun. Kí hiệu P là tập hợp các ánh xạ từ $\mathfrak{h}$ đến $k$.

(i) Tổng $\sum_{\lambda\in P}L^{\lambda}(P)$ là trực tiếp.

(ii) Nếu $f: L\rightarrow M$ là một đồng cấu của $\mathfrak{h}$-môđun, thì $f(L^{\lambda}(\mathfrak{h}))\subset M^{\lambda}(\mathfrak{h})$ với mọi $\lambda \in P$.

(iii) Nếu $f: L\times M\rightarrow N$ là một ánh xạ song tuyến tính bất biến theo $\mathfrak{h}$,

$$
f(L^{\lambda}(\mathfrak{h})\times M^\mu(\mathfrak{h}))\subset N^{\lambda+\mu}(\mathfrak{h})
$$

với mọi $\lambda , \mu\in P$.

Điều này suy ra từ các Mệnh đề 2 và 3.

#### Mệnh đề 9 {#lie-vii-s1-prop-9 .statement tag=00SX}

Cho $\mathfrak{h}$ là một đại số Lie lũy linh và M là một $\mathfrak{h}$-môđun hữu hạn chiều. Kí hiệu P là tập hợp các ánh xạ từ $\mathfrak{h}$ đến $k$.

(i) Mỗi $M^{\lambda}(\mathfrak{h})$ là một $\mathfrak{h}$-môđun con của M. Nếu $x_M$ là tam giác hóa được với mọi $x\in \mathfrak{h}$, thì $M =\sum_{\lambda\in P}M^{\lambda}(\mathfrak{h})$.

(ii) Nếu $k$ là vô hạn, tồn tại $x\in \mathfrak{h}$ sao cho $M^0(x) = M^0(\mathfrak{h})$.

(iii) Nếu $k$ có đặc số 0, và nếu $\lambda \in P$ sao cho $M^{\lambda}(\mathfrak{h})\not= 0$, thì $\lambda$ là một dạng tuyến tính trên $\mathfrak{h}$ triệt tiêu trên $[\mathfrak{h},\mathfrak{h}]$, và $M_{\lambda}(\mathfrak{h})\not= 0$.

(iv) Nếu $f: M\rightarrow N$ là một đồng cấu toàn ánh của các $\mathfrak{h}$-môđun hữu hạn chiều, thì $f(M^{\lambda}(\mathfrak{h})) = N^{\lambda}(\mathfrak{h})$ với mọi $\lambda \in P$.

(v) Nếu N là một $\mathfrak{h}$-môđun hữu hạn chiều, và B là một dạng song tuyến tính trên $M\times N$ bất biến dưới $\mathfrak{h}$, thì $M^{\lambda}(\mathfrak{h})$ và $N^\mu(\mathfrak{h})$ trực giao đối với B nếu $\lambda +\mu\not= 0$. Hơn nữa, nếu B không suy biến thì phép hạn chế của nó trên $M^{\lambda}(\mathfrak{h})\times N^{-\lambda}(\mathfrak{h})$ cũng không suy biến với mọi $\lambda \in P$.

Phần (i) suy ra từ no. 1, Bổ đề 1 và Định lý 1. Phần (ii) suy ra từ no. 2, Mệnh đề 7. Phần (iv) suy ra từ no. 1, Hệ quả 3 của Định lý 1. Ta chứng minh (iii). Ta có thể giả sử rằng $M = M^{\lambda}(\mathfrak{h})$. Khi đó, với mọi $x\in \mathfrak{h},\lambda (x) =$ (dim $M$)$^{-1}$Tr($x_M$); điều này chứng tỏ rằng $\lambda$ là tuyến tính (điều này cũng suy ra từ Mệnh đề 5) và rằng $\lambda$ triệt tiêu trên $[\mathfrak{h},\mathfrak{h}]$. Xét ánh xạ $\rho :\mathfrak{h}\rightarrow$ End$_k(M)$ được xác định bởi

$$
\rho (x) =x_M-\lambda (x)1_M
$$

theo trên, đây là một biểu diễn của $\mathfrak{h}$ trên M, và $\rho (x)$ là lũy linh với mọi $x\in \mathfrak{h}$. Theo định lý Engel (Chương I, §4, no. 2, Định lý 1), tồn tại $m\not= 0$ trong M sao cho $\rho (x)m= 0$ với mọi $x\in \mathfrak{h}$, nên $m\in M_{\lambda}(\mathfrak{h})$.

Mệnh đề đầu tiên của (v) suy ra từ no. 1, Mệnh đề 2 (ii). Để chứng minh mệnh đề thứ hai, ta có thể giả sử rằng $k$ là đóng đại số theo Mệnh đề 1 của no. 1; khi đó suy ra từ mệnh đề thứ nhất và तथ्य rằng $M =\sum_{\lambda}M^{\lambda}(\mathfrak{h}), N =\sum_{\lambda}N^{\lambda}(\mathfrak{h})$, xem (i).

#### Nhận xét {#lie-vii-s1-n3-rem-1 .statement tag=00SY}

Giả sử rằng $k$ là hoàn hảo và có đặc số 2. Cho $\mathfrak{h}=\mathfrak{s}\mathfrak{l}(2, k)$, và

$$
_2(ab)
$$

cho M là $\mathfrak{h}$-môđun $k$ (với ánh xạ đồng nhất của $\mathfrak{h}$). Nếu $x=$ là một

$$
ca
$$

phần tử tùy ý của $\mathfrak{h}$, ký hiệu $\lambda (x)$ là $\lambda \in k$ duy nhất sao cho $\lambda^2=a^2+bc$. Một phép tính cho thấy ngay lập tức rằng $M = M^{\lambda}(\mathfrak{h})$; mặt khác, $M_{\lambda}(\mathfrak{h}) = 0$ và $\lambda$ không tuyến tính cũng không bằng không trên $[\mathfrak{h},\mathfrak{h}]$, mặc dù $\mathfrak{h}$ là lũy linh.

#### Hệ quả {#lie-vii-s1-n3-cor-1 .statement tag=00SZ}

Cho $\mathfrak{h}$ là một đại số Lie lũy linh, và M là một $\mathfrak{h}$-môđun hữu hạn chiều sao cho $M^0(\mathfrak{h}) = 0$. Cho $f:\mathfrak{h}\rightarrow M$ là một ánh xạ tuyến tính sao cho

$f([x, y]) =x.f(y)-y.f(x)$ for $x, y\in \mathfrak{h}$.

Tồn tại $a\in M$ sao cho $f(x) =x.a$ với mọi $x\in \mathfrak{h}$.

Đặt $N = M\times k$. Cho $\mathfrak{h}$ tác động lên N theo công thức

$$
x.(m, \lambda ) = (x.m-\lambda f(x),0)
$$

Đồng nhất thức mà $f$ thỏa mãn suy ra rằng N là một $\mathfrak{h}$-môđun (Chương I, §1, no. 8, Ví dụ 2). Ánh xạ $(m, \lambda ) \rightarrow \lambda$ từ N đến $k$ là một đồng cấu từ N vào môđun tầm thường $\mathfrak{h}$-môđun $k$. Theo Mệnh đề 9 (iv), suy ra $N^0(\mathfrak{h})$ chứa một phần tử có dạng $(a,1)$ với $a\in M$. Xét theo giả thiết trên M,

$$
(M\times 0)\cap N^0(\mathfrak{h}) = 0
$$

nên $N^0(\mathfrak{h})$ có chiều 1 và do đó bị triệt tiêu bởi $\mathfrak{h}$. Vì vậy, $x.a-f(x) = 0$ với mọi $x\in \mathfrak{h}$, điều đó chứng minh hệ quả.

#### Mệnh đề 10 {#lie-vii-s1-prop-10 .statement tag=00T0}

Cho $\mathfrak{g}$ là một đại số Lie, $\mathfrak{h}$ là một đại số con lũy linh của $\mathfrak{g}$. Ký hiệu P là tập hợp các ánh xạ từ $\mathfrak{h}$ đến $k$.

(i) Với $\lambda , \mu\in P$, $[\mathfrak{g}^{\lambda}(\mathfrak{h}),\mathfrak{g}^\mu(\mathfrak{h})]\subset \mathfrak{g}^{\lambda+\mu}(\mathfrak{h})$; nói riêng, $\mathfrak{g}^0(\mathfrak{h})$ là một đại số con Lie của $\mathfrak{g}$ chứa $\mathfrak{h}$, và các $\mathfrak{g}^{\lambda}(\mathfrak{h})$ ổn định dưới ad $\mathfrak{g}^0(\mathfrak{h})$. Hơn nữa, $\mathfrak{g}^0(\mathfrak{h})$ là bộ chuẩn hóa của chính nó trong $\mathfrak{g}$.

(ii) Nếu M là một $\mathfrak{g}$-môđun, thì $\mathfrak{g}^{\lambda}(\mathfrak{h})M^\mu(\mathfrak{h})\subset M^{\lambda+\mu}(\mathfrak{h})$ với $\lambda , \mu\in P$; nói riêng, mỗi $M^{\lambda}(\mathfrak{h})$ là một $\mathfrak{g}^0(\mathfrak{h})$-môđun.

(iii) Nếu B là một dạng song tuyến tính trên $\mathfrak{g}$ bất biến dưới $\mathfrak{h}$, thì $\mathfrak{g}^{\lambda}(\mathfrak{h})$ và $\mathfrak{g}^\mu(\mathfrak{h})$ trực giao đối với B khi $\lambda +\mu\not= 0$. Giả sử B không suy biến. Khi đó, với mọi $\lambda \in P$, phép hạn chế của B lên $\mathfrak{g}^{\lambda}(\mathfrak{h})\times \mathfrak{g}^{-\lambda}(\mathfrak{h})$ là không suy biến; nói riêng, phép hạn chế của B lên $\mathfrak{g}^0(\mathfrak{h})\times \mathfrak{g}^0(\mathfrak{h})$ là không suy biến.

(iv) Giả sử rằng $k$ có đặc số 0. Khi đó, nếu $x\in \mathfrak{g}^{\lambda}(\mathfrak{h})$ với $\lambda \not= 0$, ad $x$ là lũy linh.

Ánh xạ $(x, y) \rightarrow [x, y]$ từ $\mathfrak{g}\times \mathfrak{g}$ đến $\mathfrak{g}$ là bất biến theo $\mathfrak{g}$ theo đồng nhất thức Jacobi, do đó bất biến theo $\mathfrak{h}$. Phần đầu của (i) vì thế suy ra từ Mệnh đề 2 (ii). Phần (ii) được chứng minh tương tự.

Nếu $x$ thuộc bộ chuẩn hóa của $\mathfrak{g}^0(\mathfrak{h})$ trong $\mathfrak{g}$, (ad $y$)$.x=-[x, y]\in \mathfrak{g}^0(\mathfrak{h})$ với mọi $y\in \mathfrak{h}$, nên (ad $y$)$^n.x= 0$ với $n$ đủ lớn. Điều này chứng tỏ rằng $x\in \mathfrak{g}^0(\mathfrak{h})$. Mệnh đề (i) nay đã được chứng minh hoàn toàn.

Mệnh đề (iii) suy ra từ Mệnh đề 9 (v).

Để chứng minh (iv), ta có thể giả sử rằng $k$ đóng đại số. Cho $x\in \mathfrak{g}^{\lambda}(\mathfrak{h})$, với $\lambda \not= 0$. Với mọi $\mu\in P$ và mọi số nguyên $n\geq 0$, (ad $x$)$^n\mathfrak{g}^\mu(\mathfrak{h})\subset \mathfrak{g}^{\mu+n\lambda}(\mathfrak{h})$; cho $P_1$ là tập hữu hạn các $\mu\in P$ sao cho $\mathfrak{g}^\mu(\mathfrak{h})\not= 0$; nếu $k$ có đặc số 0 và $\lambda \not= 0$, thì $(P_1+n\lambda )\cap P_1=\emptyset$ với $n$ đủ lớn, nên (ad $x$)$^n= 0$.

#### Bổ đề 2 {#lie-vii-s1-lem-2 .statement tag=00T1}

Giả sử rằng $k$ có đặc số 0. Cho $\mathfrak{g}$ là một đại số Lie nửa đơn trên $k$, B là dạng Killing của $\mathfrak{g}$, $\mathfrak{m}$ là một đại số con của $\mathfrak{g}$. Giả sử rằng các điều kiện sau được thỏa mãn:

1) hạn chế của B lên $\mathfrak{m}$ là không suy biến;

2) nếu $x\in \mathfrak{m}$, thì các thành phần nửa đơn và lũy linh$^1$ của $x$ trong $\mathfrak{g}$ thuộc $\mathfrak{m}$.

Khi đó $\mathfrak{m}$ là khả quy trong $\mathfrak{g}$ (Chương I, § 6, no. 6).

Theo Chương I, §6, no. 4, Mệnh đề $5d),\mathfrak{m}$ là khả quy. Cho $\mathfrak{c}$ là tâm của $\mathfrak{m}$. Nếu $x\in \mathfrak{c}$ là lũy linh, thì $x= 0$; quả vậy, với mọi $y\in \mathfrak{m}$, ad $x$ và ad $y$ giao hoán, hợp thành ad $x\circ$ ad $y$ là lũy linh, và $B(x, y) = 0$, nên $x= 0$. Giờ cho $x$ là một phần tử tùy ý của $\mathfrak{c}$; gọi $s$ và $n$ là các thành phần nửa đơn và lũy linh của nó. Ta có $n\in \mathfrak{m}$. Vì ad $n$ có dạng P(ad $x$), trong đó P là một đa thức không có số hạng hằng, (ad $n$)$.\mathfrak{m}= 0$ nên $n\in \mathfrak{c}$, và rồi $n= 0$ như trên. Do đó ad $x$ là nửa đơn. Suy ra, hạn chế lên $\mathfrak{m}$ của biểu diễn phụ hợp của $\mathfrak{g}$ là nửa đơn (Chương I, §6, no. 5, Định lý $4b$)$)$.

#### Mệnh đề 11 {#lie-vii-s1-prop-11 .statement tag=00T2}

Giả sử $k$ có đặc số không. Cho $\mathfrak{g}$ là một đại số Lie nửa đơn, $\mathfrak{h}$ là một đại số con lũy linh của $\mathfrak{g}$. Đại số $\mathfrak{g}^0(\mathfrak{h})$ thỏa mãn các điều kiện (1) và (2) của Bổ đề 2; nó là khả quy trong $\mathfrak{g}$.

$^1$ Theo Chương I, §6, no. 3, Định lý 3, mọi $x\in \mathfrak{g}$ đều có thể viết duy nhất thành tổng của một phần tử nửa đơn $s$ và một phần tử lũy linh $n$ giao hoán với nhau; phần tử $s$ (resp. $n$) được gọi là thành phần nửa đơn (resp. lũy linh) của $x$.

Cho $x, x'\in \mathfrak{g},s$ và $s'$ là các thành phần nửa đơn của chúng, $n$ và $n'$ là các thành phần lũy linh của chúng. Ta có

$x'\in \mathfrak{g}^0(x)\Leftarrow \Rightarrow$ (ad $s$)$(x') = 0$ (Prop$.4$)

$\Leftarrow \Rightarrow$ (ad $x'$)$(s) = 0$

$=\Rightarrow$ (ad $s'$)$(s) = 0$

$\Leftarrow \Rightarrow$ (ad $s$)$(s') = 0$

$\Leftarrow \Rightarrow s'\in \mathfrak{g}^0(x)$ (Prop$.4$)

suy ra $x'\in \mathfrak{g}^0(x)\Rightarrow n'\in \mathfrak{g}^0(x)$ và (2) được chứng minh. Dạng Killing của $\mathfrak{g}$ là không suy biến, nên hạn chế của nó lên $\mathfrak{g}^0(\mathfrak{h})$ là không suy biến (Prop. 10 (iii)). Do đó, việc $\mathfrak{g}^0(\mathfrak{h})$ là khả quy trong $\mathfrak{g}$ suy ra từ Bổ đề 2.

### 4. PHÂN TÍCH CỦA MỘT ĐẠI SỐ LIE TƯƠNG ĐỐI VỚI MỘT TỰ ĐẲNG CẤU

#### Mệnh đề 12 {#lie-vii-s1-prop-12 .statement tag=00T3}

Cho $\mathfrak{g}$ là một đại số Lie, $a$ là một tự đẳng cấu của $\mathfrak{g}$.

(i) Với $\lambda , \mu\in k,[\mathfrak{g}^{\lambda}(a),\mathfrak{g}^\mu(a)]\subset \mathfrak{g}^{\lambda \mu}(a)$; nói riêng, $\mathfrak{g}^1(a)$ là một đại số con của $\mathfrak{g}$.

(ii) Nếu B là một dạng song tuyến tính đối xứng trên $\mathfrak{g}$ bất biến dưới $a,\mathfrak{g}^{\lambda}(a)$ và $\mathfrak{g}^\mu(a)$ trực giao đối với B khi $\lambda \mu\not= 1$. Giả sử B không suy biến. Khi đó, nếu $\lambda \not= 0$, hạn chế của B lên $\mathfrak{g}^{\lambda}(a)\times \mathfrak{g}^{1/\lambda}(a)$ là không suy biến.

Khẳng định (i) và nửa đầu của (ii) suy ra từ Prop. 2 (iii) áp dụng cho luật hợp thành $\mathfrak{g}\times \mathfrak{g}\rightarrow \mathfrak{g}$ và dạng song tuyến tính B. Để chứng minh nửa sau của (ii), ta có thể giả sử rằng $k$ là đóng đại số. Khi đó $\mathfrak{g}=\bigoplus_{\nu\in k}\mathfrak{g}^{\nu}(a)$. Theo nhận xét trên, $\mathfrak{g}^{\lambda}(a)$ trực giao với $\mathfrak{g}^{\nu}(a)$ nếu $\lambda \nu \not= 1$; vì B không suy biến, suy ra rằng hạn chế của nó lên $\mathfrak{g}^{\lambda}(a)\times \mathfrak{g}^{1/\lambda}(a)$ cũng không suy biến.

#### Hệ quả {#lie-vii-s1-n4-cor-1 .statement tag=00T4}

Giả sử rằng $k$ có đặc số không và rằng $\mathfrak{g}$ là nửa đơn. Khi đó đại số con $\mathfrak{g}^1(a)$ thỏa mãn các điều kiện (1) và (2) của Bổ đề 2; nó là khả quy trong $\mathfrak{g}$.

Điều kiện (1) suy ra từ phần (ii) của Prop. 12; điều kiện (2) suy ra từ Prop. 4 của no. 1.

### 5. CÁC BẤT BIẾN CỦA MỘT ĐẠI SỐ LIE NỬA ĐƠN TƯƠNG ĐỐI VỚI MỘT TÁC ĐỘNG NỬA ĐƠN

Trong mục này, $k$ được giả thiết có đặc số không.

#### Mệnh đề 13 {#lie-vii-s1-prop-13 .statement tag=00T5}

Cho $\mathfrak{g}$ là một đại số Lie nửa đơn, $\mathfrak{a}$ là một đại số con của $\mathfrak{g}$ khả quy trong $\mathfrak{g}$, và $\mathfrak{m}$ là hoán tập của $\mathfrak{a}$ trong $\mathfrak{g}$. Đại số con $\mathfrak{m}$ thỏa mãn các điều kiện (1) và (2) của Bổ đề 2 của no. 3; nó khả quy trong $\mathfrak{g}$.

Theo Mệnh đề 6 của Chương I, §3, no. 5, áp dụng cho $\mathfrak{a}$-môđun $\mathfrak{g}$, ta có $\mathfrak{g}=\mathfrak{m}\oplus [\mathfrak{a},\mathfrak{g}]$. Gọi B là dạng Killing của $\mathfrak{g}$, và cho $x\in \mathfrak{a}, y\in \mathfrak{m}, z\in \mathfrak{g}$. Khi đó,

$B([z, x], y) = B(z,[x, y]) = 0$ since $[x, y] = 0$,

điều này cho thấy rằng $\mathfrak{m}$ trực giao với $[\mathfrak{a},\mathfrak{g}]$ đối với B. Vì B là không suy biến, và vì $\mathfrak{g}=\mathfrak{m}\oplus [\mathfrak{a},\mathfrak{g}]$, suy ra sự hạn chế của B lên $\mathfrak{m}$ là không suy biến; do đó điều kiện (1) của Bổ đề 2 được thỏa mãn.

Bây giờ cho $x\in \mathfrak{m}$ và cho $s$ và $n$ là các thành phần nửa đơn và lũy linh của nó. Thành phần nửa đơn của ad $x$ là ad $s$, xem Chương I, §6, no. 3. Vì ad $x$ bằng không trên $\mathfrak{a}$, nên ad $s$ cũng vậy, theo Mệnh đề 4 (i). Do đó $s\in \mathfrak{m}$, nên $n=x-s\in \mathfrak{m}$, và điều kiện (2) của Bổ đề 2 được thỏa mãn.

#### Nhận xét {#lie-vii-s1-n5-rem-1 .statement tag=00T6}

Hoán tập của $\mathfrak{m}$ trong $\mathfrak{g}$ không nhất thiết rút gọn về $\mathfrak{a}$, xem Bài tập 4.

#### Mệnh đề 14 {#lie-vii-s1-prop-14 .statement tag=00T7}

Cho $\mathfrak{g}$ là một đại số Lie nửa đơn, A là một nhóm và $r$ là một đồng cấu từ A vào Aut($\mathfrak{g}$). Cho $\mathfrak{m}$ là đại số con của $\mathfrak{g}$ gồm các phần tử bất biến dưới $r(A)$. Giả sử biểu diễn tuyến tính $r$ là nửa đơn. Khi đó $\mathfrak{m}$ thỏa mãn các điều kiện (1) và (2) của Bổ đề 2 của no. 3; nó khả quy trong $\mathfrak{g}$.

Chứng minh tương tự như của mệnh đề trước:

Cho $\mathfrak{g}^+$ là không gian con vectơ của $\mathfrak{g}$ được sinh bởi các $r(a)x-x,a\in A, x\in \mathfrak{g}$. Không gian vectơ $\mathfrak{g}'=\mathfrak{m}+\mathfrak{g}^+$ ổn định dưới $r(A)$. Cho $\mathfrak{n}$ là một phần bù của $\mathfrak{g}'$ trong $\mathfrak{g}$ ổn định dưới $r(A)$. Nếu $x\in \mathfrak{n}, a\in A,r(a)x-x\in \mathfrak{n}\cap \mathfrak{g}^+= 0$, thì $x\in \mathfrak{m}$ và khi đó $x= 0$ vì $\mathfrak{m}\cap \mathfrak{n}= 0$. Vậy, $\mathfrak{g}=\mathfrak{g}'=\mathfrak{m}+\mathfrak{g}^+$. Gọi B là dạng Killing của $\mathfrak{g}$ và cho $y\in \mathfrak{m}, a\in A, x\in \mathfrak{g}$. Khi đó

$$
B(y, r(a)x-x) = B(y, r(a)x)-B(y, x)
$$

$$
= B(r(a^{-1})y, x)-B(y, x)
$$

$$
= B(y, x)-B(y, x) = 0
$$

Vì vậy $\mathfrak{m}$ và $\mathfrak{g}^+$ trực giao đối với B. Suy ra rằng hạn chế của B lên $\mathfrak{m}$ là không suy biến; do đó điều kiện (1) của Bổ đề 2. Điều kiện (2) là ngay lập tức bằng phép chuyển cấu trúc.

### Bài tập {#lie-vii-s1-exercises}

Mọi đại số Lie và các môđun trên chúng đều được giả thiết là hữu hạn chiều trên $k$; từ §3 trở đi, $k$ được giả thiết có đặc số không.

Xem [các bài tập cho § 1](exercises/s1/).
