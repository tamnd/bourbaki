---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VIII
chapter_title: SPLIT SEMI-SIMPLE LIE ALGEBRAS
section: 12
section_title: Chevalley orders
lang: vi
source: lie-vii-ix
book_pages: 173-189
pdf_pages: 0181-0197
extraction: native
subsections:
    - "no": 1
      title: LATTICES AND ORDERS
      page: 173
      pdf_page: 181
    - "no": 2
      title: DIVIDED POWERS IN A BIGEBRA
      page: 173
      pdf_page: 181
    - "no": 3
      title: INTEGRAL VARIANT OF THE POINCARÉ-BIRKHOFF-WITT THEOREM
      page: 174
      pdf_page: 182
    - "no": 4
      title: 'EXAMPLE: POLYNOMIALS WITH INTEGER VALUES'
      page: 176
      pdf_page: 184
    - "no": 5
      title: SOME FORMULAS
      page: 178
      pdf_page: 186
    - "no": 6
      title: BIORDERS IN THE ENVELOPING ALGEBRA OF A SPLIT REDUCTIVE LIE ALGEBRA
      page: 180
      pdf_page: 188
    - "no": 7
      title: CHEVALLEY ORDERS
      page: 185
      pdf_page: 193
    - "no": 8
      title: ADMISSIBLE LATTICES
      page: 187
      pdf_page: 195
statements: 34
exercises: 0
content_sha256: 69c961f5fc9a723d6bf5458ccd70ecab8b7a92a22f58d6d0b5189c95e8d63c8a
translated_from: content/en/lie/VIII/12_s12_chevalley_orders.md
source_content_sha256: 50f43a34a9ae42cb38e10e1f32022dc1fddb5d2b07911570fec5baa09a40ebdf
translation_model: gpt-5.4-mini, gpt-5-mini, gpt-5-6-mini
translation_run: translate-vi-3648e84a
glossary_version: 34
glossary_terms_sha256: 799c17201fd8c713dae0cd294a415add243eccb9483bbc10218e5177c25a5e0b
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 12. THỨ TỰ CHEVALLEY

### 1. DÀN VÀ THỨ TỰ

Cho V là một $\mathbf{Q}$-không gian vectơ. Một dàn trong V là một $\mathbf{Z}$-môđun con tự do $\mathscr{V}$ của V sao cho ánh xạ $\mathbf{Q}$-tuyến tính $\alpha_{\mathscr{V},V}:\mathscr{V}\otimes_{\mathbf{Z}}\mathbf{Q}\rightarrow V$ cảm sinh bởi phép nhúng của $\mathscr{V}$ vào V là song ánh. Khi V hữu hạn chiều, điều này tương đương với việc nói rằng $\mathscr{V}$ là một $\mathbf{Z}$-môđun con hữu hạn sinh sinh ra $\mathbf{Q}$-không gian vectơ V (nhớ rằng một $\mathbf{Z}$-môđun không xoắn hữu hạn sinh là tự do theo Đại số, Chương VII, §4, no. 4, Hệ quả 2); hơn nữa, trong trường hợp này định nghĩa của chúng ta là một trường hợp riêng của định nghĩa trong Đại số giao hoán, Chương VII, §4, no. 1, Định nghĩa 1 (chỗ đã dẫn, Ví dụ 3). Nếu W là một không gian con vectơ của V, và $\mathscr{V}$ là một dàn trong V, thì $\mathscr{V}\cap W$ là một dàn trong W.

Nếu V là một $\mathbf{Q}$-đại số, một thứ tự trong V là một dàn $\mathscr{V}$ trong không gian vectơ nền mà là một $\mathbf{Z}$-đại số con của V; khi đó ánh xạ $\alpha_{\mathscr{V},V}$ là một đẳng cấu của $\mathbf{Q}$-đại số. Nếu V là một $\mathbf{Q}$-đại số có đơn vị, một thứ tự có đơn vị trong V là một thứ tự trong V chứa phần tử đơn vị.

Giả sử V là một $\mathbf{Q}$-bigebra, với đồng tích $c$ và đồng đơn vị $\gamma$. Nếu $\mathscr{V}$ là một dàn trong không gian vectơ V, thì ánh xạ chính tắc $i:\mathscr{V}\otimes_{\mathbf{Z}}\mathscr{V}\rightarrow V\otimes_{\mathbf{Q}}V$ là đơn ánh; một song thứ tự trong V là một thứ tự có đơn vị $\mathscr{V}$ trong đại số có đơn vị V sao cho $\gamma (\mathscr{V})\subset \mathbf{Z}$ và $c(\mathscr{V})\subset i(\mathscr{V}\otimes_{\mathbf{Z}}\mathscr{V})$; các ánh xạ

$\gamma_{\mathscr{V}}:\mathscr{V}\rightarrow \mathbf{Z}$ và $c_{\mathscr{V}}:\mathscr{V}\rightarrow \mathscr{V}\otimes_{\mathbf{Z}}\mathscr{V}$

cảm sinh bởi $\gamma$ và $c$ cho $\mathscr{V}$ cấu trúc của một $\mathbf{Z}$-bigebra, và khi đó ánh xạ $\alpha_{\mathscr{V},V}$ là một đẳng cấu của $\mathbf{Q}$-bigebra.

### 2. LŨY THỪA CHIA TRONG MỘT BIGEBRA

Cho A là một $k$-đại số có đơn vị, $x\in A,d\in k,n\in \mathbf{N}$. Đặt

$$
x(x-d). . .(x-d(n-1))^{n-1}
$$

$$
x^{(n,d)}==\prod(x-id)/(i+ 1) \tag{1}
$$

$n$!

$i=0$

Đặc biệt, $x^{(0,d)}= 1,x^{(1,d)}=x$. Quy ước rằng $x^{(n,d)}= 0$ nếu $n$ là một số nguyên $<0$. Đặt

$x^{(n)}=x^{(n,0)}=xn^n$! (2)

$(nx)=x^{(n,1)}=x(x-1). . .n($!$x-n+ 1)$. (3)

#### Mệnh đề 1 {#lie-viii-s12-prop-1 .statement tag=017V}

Cho A là một bigebra, với đồng tích $c$, và $x$ là một phần tử nguyên thủy (Chương II, §1, no. 2) của A. Khi đó

$$
c(x^{(n,d)}) =\sum x^{(p,d)}\otimes x^{(q,d)} \tag{4}
$$

$p\in \mathbf{N},q\in \mathbf{N},p+q=n$

Mệnh đề là hiển nhiên với $n\leq 0$. Ta chứng minh bằng quy nạp theo $n$. Nếu công thức (4) đúng với $n$, thì

$$
(n+ 1)c(x^{(n+1,d)}) =c(x-dn)c(x^{(n,d)})
$$

$$
= (x\otimes 1 + 1\otimes x-dn1\otimes 1)c(x^{(n,d)})
$$

$$
=\sum_{p+q=n}[xx^{(p,d)}\otimes x^{(q,d)}+x^{(p,d)}\otimes xx^{(q,d)}-(p+q)dx^{(p,d)}\otimes x^{(q,d)}]
$$

$$
=\sum_{p+q=n}(x-pd)x^{(p,d)}\otimes x^{(q,d)}+\sum_{p+q=n}x^{(p,d)}\otimes (x-qd)x^{(q,d)}
$$

$$
=\sum_{p+q=n}(p+ 1)x^{(p+1,d)}\otimes x^{(q,d)}+\sum_{p+q=n}(q+ 1)x^{(p,d)}\otimes x^{(q+1,d)}
$$

$$
=\sum_{r+s=n+1}rx^{(r,d)}\otimes x^{(s,d)}+\sum_{r+s=n+1}sx^{(r,d)}\otimes x^{(s,d)}
$$

$$
= (n+ 1)\sum_{r+s=n+1}x^{(r,d)}\otimes x^{(s,d)}
$$

suy ra công thức (4) cho $n+ 1$.

### 3. DẠNG NGUYÊN CỦA ĐỊNH LÝ POINCARÉ-BIRKHOFF-WITT

Cho $\mathfrak{g}$ là một đại số Lie $\mathbf{Q}$-hữu hạn chiều, $U(\mathfrak{g})$ là bigebra bao của nó. Nếu I là một tập sắp thứ tự toàn phần, $\mathbf{x}= (x_i)_{i\in I}$ là một họ các phần tử của $\mathfrak{g}$, và $\mathbf{n}=$ $(n_i)_{i\in I}\in \mathbf{N}^{(I)}$ là một đa chỉ số, đặt

$\mathbf{x}^{(\mathbf{n})}=\prod x\overset{ni}{n_{i}}$!$^{^i}$, (5)

$i\in I$

tích được tính trong $U(\mathfrak{g})$ phù hợp với tập có thứ tự I.

#### Định lý 1 {#lie-viii-s12-thm-1 .statement tag=017W}

Cho $\mathscr{U}$ là một song thứ tự trong bigebra $U(\mathfrak{g})$. Đặt $\mathscr{G}=\mathscr{U}\cap \mathfrak{g}$, đó là một cấp trong đại số Lie $\mathfrak{g}$. Cho $(x_i)_{i\in I}$ là một cơ sở của $\mathscr{G}$. Gán cho I một thứ tự toàn phần, và giả sử rằng ta đã cho, với mọi $\mathbf{n}\in \mathbf{N}^I$, một phần tử $[\mathbf{n}]$ của $\mathscr{U}$ sao cho $[\mathbf{n}]-\mathbf{x}^{(\mathbf{n})}$ có lọc $<|\mathbf{n}|$ trong $U(\mathfrak{g})$. Khi đó, họ các $[\mathbf{n}]$ với $\mathbf{n}\in \mathbf{N}^I$ là một cơ sở của môđun $\mathbf{Z}$ $\mathscr{U}$.

Với $p\in \mathbf{N}$, gọi $U_p(\mathfrak{g})$ là tập các phần tử của $U(\mathfrak{g})$ có lọc $\leq p$; khi đó các ảnh trong $U_p(\mathfrak{g})/U_{p-1}(\mathfrak{g})$ của các $\mathbf{x}^{(\mathbf{n})}$ sao cho $|\mathbf{n}|=p$ tạo thành một cơ sở của không gian vectơ $\mathbf{Q}$ này (Chap. I, §2, no. 7, Th. 1); do đó các $[\mathbf{n}]$ tạo thành một cơ sở của không gian vectơ $\mathbf{Q}$ $U(\mathfrak{g})$. Còn lại phải chứng minh mệnh đề sau (trong đó ta đặt $M =\mathbf{N}^I$)$:$

(*) nếu $u\in \mathscr{U}, (a_{\mathbf{n}})\in \mathbf{Z}^{(M)}$, và $d\in$ **N --**$\{0\}$ sao cho

$$
du=\sum_{\mathbf{n}\in M}a_{\mathbf{n}}[\mathbf{n}] \tag{6}
$$

thì $d$ chia hết mỗi $a_{\mathbf{n}}$.

Với mỗi số nguyên $r\geq 0$, đưa vào đồng tích lặp

$$
c_i:\mathscr{U}\rightarrow \mathbf{T}^r(\mathscr{U}) =\mathscr{U}\otimes \mathscr{U}\otimes  \cdots  \otimes \mathscr{U}
$$

theo định nghĩa, $c_0$ là đồng đơn vị của $\mathscr{U},c_1=$ Id$_{\mathscr{U}},c_2=c$ (đồng tích của $\mathscr{U}$), và, với $r\geq 2,c_{r+1}$ được định nghĩa là hợp thành $p\circ (c_r\otimes 1)\circ c:$

$$
\mathscr{U}\longrightarrow^c\mathscr{U}\otimes_{\mathbf{Z}}\mathscr{U}^c\longrightarrow^{^r\otimes 1}\mathbf{T}^r(\mathscr{U})\otimes_{\mathbf{Z}}\mathscr{U}\longrightarrow^p\mathbf{T}^{r+1}(\mathscr{U})
$$

nơi $p$ được xác định bằng cách sử dụng phép nhân trong đại số $\mathbf{T}(\mathscr{U})$. Hơn nữa, xét phép chiếu chính tắc $\pi$ của $\mathscr{U}$ lên $\mathscr{U}^+=$ Ker $c_0$, và ánh xạ hợp thành

$$
c^+_r=\mathbf{T}^r(\pi )\circ c_r:\mathscr{U}\rightarrow \mathbf{T}^r(\mathscr{U}^+)
$$

#### Bổ đề 1 {#lie-viii-s12-lem-1 .statement tag=017X}

Cho $\mathbf{n}\in \mathbf{N}^I$. Nếu $|\mathbf{n}|< r$, thì $c^+_r([\mathbf{n}]) = 0$. Nếu $|\mathbf{n}|=r$, thì

$$
c^+_r([\mathbf{n}]) =\sum_{\varphi}x_{\varphi(1)}\otimes x_{\varphi(2)}\otimes  \cdots  \otimes x_{\varphi(r)} \tag{7}
$$

trong đó $\varphi$ thuộc tập hợp các ánh xạ từ $\{1,2, . . . , r\}$ vào I nhận mỗi giá trị $i\in In_i$ lần.

Theo Mệnh đề 1,

$$
c_r(\mathbf{x}^{(\mathbf{n})}) =\sum\mathbf{x}^{(\mathbf{p}_1)}\otimes  \cdots  \otimes \mathbf{x}^{(\mathbf{p}_r)}
$$

trong đó phép lấy tổng mở rộng trên tập hợp các dãy $(\mathbf{p}_1, . . . ,\mathbf{p}_r)$ gồm $r$ phần tử của M sao cho $\mathbf{p}_1+\cdots +\mathbf{p}_r=\mathbf{n}$. Theo Chương II, §1, no. 3, Mệnh đề 6, ánh xạ $c^+_r$, được mở rộng bằng tính tuyến tính thành một ánh xạ từ $U(\mathfrak{g})$ vào $\mathbf{T}^r(U^+(\mathfrak{g}))$, triệt tiêu trên $U_{r-1}(\mathfrak{g})$. Suy ra rằng, với $r\geq  |\mathbf{n}|$,

$$
c^+_r([\mathbf{n}]) =c^+_r(\mathbf{x}^{(\mathbf{n})}) =\sum\pi (\mathbf{x}^{(\mathbf{p}_1)})\otimes  \cdots  \otimes \pi (\mathbf{x}^{(\mathbf{p}_r)}) \tag{8}
$$

Với $r >|\mathbf{n}|$, quan hệ $\mathbf{p}_1+\cdots +\mathbf{p}_r=\mathbf{n}$ kéo theo rằng ít nhất một trong các $\mathbf{p}_i$ là không, do đó $c^+_r([\mathbf{n}]) = 0$. Với $r=|\mathbf{n}|$, các số hạng khác không duy nhất của thành phần thứ ba của (8) là những số hạng sao cho $|\mathbf{p}_1|=\cdots =|\mathbf{p}_r|= 1$, do đó có (7).

Ta quay lại chứng minh Định lý 1. Ta giữ lại các ký hiệu của (*) và chứng minh, bằng quy nạp giảm dần theo $|\mathbf{n}|$, rằng $d$ chia hết cho $a_{\mathbf{n}}$, điều này là rõ ràng khi $|\mathbf{n}|$ đủ lớn. Nếu $d$ chia hết cho $a_{\mathbf{n}}$ với $|\mathbf{n}|> r$ thì, đặt

$$
u'=u-\sum_{|\mathbf{n}|>r}(a_{\mathbf{n}}/d)[\mathbf{n}]\in \mathscr{U}
$$

ta có

$$
du'=\sum_{|\mathbf{n}|\leq r}a_{\mathbf{n}}[\mathbf{n}] \tag{9}
$$

Với mọi ánh xạ $\varphi$ từ $\{1,2, . . . , r\}$ vào I, đặt

$$
e_{\varphi}=x_{\varphi(1)}\otimes  \cdots  \otimes x_{\varphi(r)}
$$

và $a_{\varphi}=a_{\mathbf{n}}$ trong đó $\mathbf{n}=$ (Card$\varphi^{-1}(i)$)$_{i\in I}$. Theo Bổ đề 1, (9) suy ra rằng

$$
dc^+_r(u') =\sum_{\varphi\in I^r}a_{\varphi}e_{\varphi} \tag{10}
$$

vì vậy $c^+_r(u')\in \mathbf{T}^r(\mathscr{U}^+)\cap \mathbf{Q}\mathbf{T}^r(\mathscr{G})$. Nhưng môđun con $\mathscr{G}$ của $\mathscr{U}^+$ là một nhân tử trực tiếp (Đại số, Chương VII, §4, no. 3, Hệ quả của Định lý 1), do đó môđun con $\mathbf{T}^r(\mathscr{G})$ là một nhân tử trực tiếp của $\mathbf{T}^r(\mathscr{U}^+)$, và suy ra $c^+_r(u')\in \mathbf{T}^r(\mathscr{G})$. Mặt khác, các $x_i$ lập thành một cơ sở của $\mathscr{G}$ theo giả thiết, nên các $e_{\varphi}$ lập thành một cơ sở của $\mathbf{T}^r(\mathscr{G})$. Khi đó (10) chứng minh rằng $d$ chia hết cho các $a_{\varphi}$, nghĩa là các $a_{\mathbf{n}}$ với $|\mathbf{n}|=r$. Điều này chứng minh (*).

### 4. VÍ DỤ: CÁC ĐA THỨC VỚI CÁC GIÁ TRỊ NGUYÊN

Cho V là một không gian vectơ $\mathbf{Q}$ hữu hạn chiều, $V^*$ là đối ngẫu của nó, $\mathscr{V}$ là một dàn trong V, $\mathscr{V}^*$ là môđun $\mathbf{Z}$ đối ngẫu của $\mathscr{V}$, có thể được đồng nhất một cách chính tắc với một dàn trong $V^*,\mathbf{S}(V)$ là đại số đối xứng của V, và

$$
\lambda :\mathbf{S}(V)\rightarrow A(V^*)
$$

là song ánh chính tắc từ $\mathbf{S}(V)$ đến đại số các hàm đa thức trên $V^*($Đại số, Chương IV, §5, no. 11, Nhận xét 1). Nếu ta đồng nhất $A(V^*\times V^*)$ với $A(V^*)\otimes_{\mathbf{Q}}A(V^*)$, thì $\lambda$ biến đổi đồng tích của $\mathbf{S}(V)$ thành ánh xạ $A(V^*)\rightarrow A(V^*\times V^*)$ gán cho hàm đa thức $\varphi$ trên $V^*$ hàm đa thức

$$
(x, y) \rightarrow \varphi (x+y)
$$

trên $V^*\times V^*($Đại số, Chương IV, §5, no. 11, Nhận xét 2).

Ký hiệu bởi $(^{\mathscr{V}}_{\mathbf{Z}})$ tập con của $\mathbf{S}(V)$ gồm các phần tử tương ứng với các ánh xạ đa thức từ $V^*$ vào $\mathbf{Q}$ nhận các giá trị nguyên trên $\mathscr{V}^*$.

#### Mệnh đề 2 {#lie-viii-s12-prop-2 .statement tag=017Y}

(i) $(^{\mathscr{V}}_{\mathbf{Z}})$ là một song thứ tự trong đại số song của $\mathbf{S}(V)$, và $(^{\mathscr{V}}_{\mathbf{Z}})\cap V =\mathscr{V}$.

(ii) Đại số $\mathbf{Z}$ $(^{\mathscr{V}}_{\mathbf{Z}})$ được sinh bởi các $(^h_n)$ với $h\in \mathscr{V}, n\in \mathbf{N}$.

(iii) Nếu $(h_1, . . . , h_r)$ là một cơ sở của $\mathscr{V}$, các phần tử

$$
(h)(h_1)(h_r)
$$

= $\cdots$,

$$
\mathbf{n}n_1n_r
$$

trong đó $\mathbf{n}= (n_1, . . . , n_r)$ thuộc $\mathbf{N}^r$, lập thành một cơ sở của môđun $\mathbf{Z}$ $(^{\mathscr{V}}_{\mathbf{Z}})$.

Với $m\in \mathbf{N}$, đặt $\mathbf{S}_m(V) =\sum_{i\leq m}\mathbf{S}^i$(V), $\mathbf{S}_m(\mathscr{V}) =\sum_{i\leq m}\mathbf{S}^i(\mathscr{V})$. Theo Đại số, Chương IV, §5, no. 9, Mệnh đề 15 và Nhận xét,

$\mathbf{S}_m(\mathscr{V})\subset \mathbf{S}_m(V)\cap (\mathscr{V}\mathbf{Z})\subset m1$!$\mathbf{S}_m(\mathscr{V})$

vì vậy $(^{\mathscr{V}}_{\mathbf{Z}})\cap V =\mathscr{V}$. Vì $\mathbf{S}_m(\mathscr{V})$ là một dàn trong $\mathbf{S}_m$(V), $\mathbf{S}_m(V)\cap (_{\mathbf{Z}}^{\mathscr{V}})$ cũng là một dàn trong $\mathbf{S}_m(V)$. Mặt khác, $\mathbf{S}_m(V)\cap (^{\mathscr{V}}_{\mathbf{Z}})$ là một nhân tử trực tiếp của $\mathbf{S}_{m+1}(V)\cap (_{\mathbf{Z}}^{\mathscr{V}})$ (vì môđun thương không xoắn), do đó nó thừa nhận một phần bù là một $\mathbf{Z}$-môđun tự do. Suy ra rằng $(^{\mathscr{V}}_{\mathbf{Z}})$ là một $\mathbf{Z}$-môđun tự do. Hiển nhiên đây là một cấp có đơn vị trong đại số $\mathbf{S}(V)$. Gọi $(u_n)_{n\in\mathbf{N}}$ là một cơ sở của $\mathbf{Z}$-môđun $(^{\mathscr{V}}_{\mathbf{Z}})$. Đây cũng là một cơ sở của $\mathbf{Q}$-môđun $\mathbf{S}(V)$ và, với mọi

$$
\varphi \in \mathbf{S}(V\times V) =\mathbf{S}(V)\otimes_{\mathbf{Q}}\mathbf{S}(V)
$$

tồn tại một dãy duy nhất $(v_n)$ gồm các phần tử của $\mathbf{S}(V)$ sao cho $\varphi =\sum u_n\otimes v_n$. Như trên, đồng nhất $\mathbf{S}(V)$ với $A(V^*)$ và $\mathbf{S}(V)\otimes \mathbf{S}(V)$ với $A(V^*\times V^*)$. Nếu $\varphi \in (^{\mathscr{V}\times\mathscr{V}}_{\mathbf{Z}})$, hàm đa thức $x \rightarrow \varphi (x, y)$ thuộc $(^{\mathscr{V}}_{\mathbf{Z}})$ với mọi $y\in \mathscr{V}^*$. Suy ra rằng $v_n(y)\in \mathbf{Z}$ với mọi $n$ và mọi $y\in \mathscr{V}^*$, nói cách khác $v_n\in (^{\mathscr{V}}_{\mathbf{Z}})$. Điều này chứng minh rằng đồng tích ánh xạ $(^{\mathscr{V}}_{\mathbf{Z}})$ vào $(_{\mathbf{Z}}^{\mathscr{V}})\otimes_{\mathbf{Z}}(_{\mathbf{Z}}^{\mathscr{V}})$. Nếu $h\in \mathscr{V}$ và $n\in \mathbf{N}$, thì $(_n^h)$ ánh xạ $u\in \mathscr{V}^*$ vào số nguyên $(^{u(h)}_n)$, do đó $(^h_n)\in (_{\mathbf{Z}}^{\mathscr{V}})$. Mệnh đề (iii) thu được bằng cách áp dụng Th. 1 cho đại số Lie giao hoán V, và (ii) suy ra.

#### Hệ quả {#lie-viii-s12-n4-cor-1 .statement tag=017Z}

Gọi X là một phần tử bất định. Các đa thức $(^X_n)$, với $n\in \mathbf{N}$, lập thành một cơ sở của $\mathbf{Z}$-môđun gồm các đa thức $P\in k[X]$ sao cho $P(\mathbf{Z})\subset \mathbf{Z}$.

Nếu $P(\mathbf{Z})\subset \mathbf{Z}$, công thức nội suy Lagrange (Đại số, Chap. IV, §2, no. 1, Mệnh đề 6) chỉ ra rằng các hệ số của P thuộc $\mathbf{Q}$; do đó, ta có thể giả sử rằng $k=\mathbf{Q}$ và áp dụng Mệnh đề 2 với $V =\mathbf{Q},\mathscr{V}=\mathbf{Z}$.

### 5. MỘT SỐ CÔNG THỨC

Trong số này, A ký hiệu một đại số kết hợp có đơn vị. Nếu $x\in A$, ta viết ad $x$ thay cho ad$_Ax$.

#### Bổ đề 2 {#lie-viii-s12-lem-2 .statement tag=0180}

Nếu $x, y\in A$ và $n\in \mathbf{N}$,

(ad$nx$! )$^ny=\sum(-1)^qxp^p$! $yxq^q$! = $\sum(-1)^qx^{(p)}yx^{(q)}$. (11)

$p+q=np+q=n$

Thật vậy, nếu ta ký hiệu bởi $L_x$ và $R_x$ các ánh xạ $z \rightarrow xz$ và $z \rightarrow zx$ từ A vào A, ta có, vì $L_x$ và $R_x$ giao hoán,

$n1$!(ad $x$)$^n=n1$!$(L_x-R_x)^n=\sum_{p+q=n}(-1)^qp1$! $L^p_xq1$! $R^q_x$.

#### Bổ đề 3 {#lie-viii-s12-lem-3 .statement tag=0181}

Cho $x, h\in A$ và $\lambda \in k$ sao cho (ad $h$)$x=\lambda x$. Với mọi $n\in \mathbf{N}$, và mọi $P\in k[X]$, ta có

$$
P(h)x^{(n)}=x^{(n)}P(h+n\lambda ) \tag{12}
$$

Vì ad $h$ là một đạo hàm của A và vì (ad $h$)$x$ giao hoán với $x$, ta có

(ad $h$)$x^n=nx^{n-1}$((ad $h$)$x$) $=n\lambda x^n$, (13) do đó

(ad $h$)$x^{(n)}=n\lambda x^{(n)}$.

Vì vậy, công thức (12) suy ra từ trường hợp đặc biệt

$$
P(h)x=xP(h+\lambda ) \tag{14}
$$

bằng cách thay thế $x$ bởi $x^{(n)}$ và $\lambda$ bởi $n\lambda$. Chỉ cần chứng minh (14) khi $P = X^m$, bằng quy nạp theo $m$. Điều này hiển nhiên khi $m= 0,1$. Nếu (14) đúng với $P = X^m$, thì

$$
h^{m+1}x=h.h^mx=hx(h+\lambda )^m=x(h+\lambda )^{m+1}
$$

điều này chứng minh (12).

#### Bổ đề 4 {#lie-viii-s12-lem-4 .statement tag=0182}

Cho $x, y, h\in A$ sao cho

$$
[y, x] =h,[h, x] = 2x,[h, y] =-2y \tag{15}
$$

(i) Với $m, n\in \mathbf{N}$, ta có

$$
_{(n)(m)}\sum_{(m-p)}(m+n-p-1-h)_{(n-p)}
$$

$xy$ = $yx$. (16)

$$
p
$$

$p\geq 0$

(ii) Cho $A'$ là đại số con $\mathbf{Z}$ của A được sinh bởi các $x^{(m)}$ và các $y^{(m)}$ với $m\in \mathbf{N}$. Khi đó $(^h_n)\in A'$ với mọi $n\in \mathbf{N}$.

Công thức (16) có thể được viết dưới dạng tương đương

$$
_{(n)(m)}\sum_{(m-p)}(m+n-p-1-h)_{(n-p)}
$$

(ad $x$)$y$ = $yx.(17_m)$

$$
p
$$

$p\geq 1$

Điều này là tầm thường với $m= 0$. Ta chứng minh bằng quy nạp theo $m$. Từ $(17_m)$, ta thu được

$(m+$ 1)(ad $x^{(n)}$)$y^{(m+1)}=$ (ad $x^{(n)}$)$y^{(m)}.y+y^{(m)}$.(ad $x^{(n)}$)$y$ (18)

$$
_{(m-p)}(m+n-p-1-h)_{(n-p)(m)}-
$$

$$
=\sum yxy+y(n-1-h)x^{(n1)}
$$

$$
p
$$

$p\geq 1$

(§1, no. 1, Bổ đề 1). Bây giờ, áp dụng bổ đề ấy, rồi đến Bổ đề 3,

ta có

$$
(m+n-p-1-h)_{(n-p)}
$$

$$
xy
$$

$$
p
$$

$$
(m+n-p+ 1-h)_{(n-p)}
$$

$$
=yx
$$

$$
p
$$

$$
(m+n-p-1-h)_{--}
$$

+ $(yx+ (n-p-1-h)x^{(np1)})$

$$
p
$$

$$
(m+n-p+ 1-h)_{(n-p)}
$$

$$
=yx
$$

$$
p
$$

$$
(m+n-p-1-h)_{--}
$$

+ $(n-p-1-h)x^{(np1)}$.

$$
p
$$

Thay điều này vào (18), ta được

$(m+$ 1)(ad $x^{(n)}$)$y^{(m+1)}$

$$
_-(m+n-p+ 1-h)_-
$$

$$
=\sum(m-p+ 1)y^{(mp+1)}x^{(np)}
$$

$$
p
$$

$p\geq 1$

$$
_-(m+n-p-1-h)_{--}
$$

$+\sum y^{(mp)}(n-p-1-h)x^{(np1)}$

$$
p
$$

$p\geq 1$

$$
+y^{(m)}(n-1-h)x^{(n-1)}
$$

$$
_-(m+n-p+ 1-h)_-
$$

$=\sum(m-p+ 1)y^{(mp+1)}x^{(np)}$

$$
p
$$

$p\geq 1$

$$
_{(m-p)}(m+n-p-1-h)_{--}
$$

$+\sum y(n-p-1-h)x^{(np1)}$.

$$
p
$$

$p\geq 0$ Đổi $p$ thành $p-1$ trong tổng thứ hai, và nhóm lại các hạng tử, ta được

$(m+$ 1)(ad $x^{(n)}$)$y^{(m+1)}=\sum_{p\geq 1}y^{(m-p+1)}A_px^{(n-p)}$ (19)

với

$$
(m+n-p+ 1-h)(m+n-p-h)
$$

$A_p= (m-p + 1)+ (n-p-h)$.

$$
pp-1
$$

Đặt $z=m+n-p-h$, điều này cũng có thể viết thành

$A_p=p1$!$(m-p + 1)(z+ 1)z(z-1). . .(z-p + 2)$

+ 1 $(z-m)z(z-1). . .(z-p + 2)$

$(p-$ 1)!

$=p1$! $z(z-1). . .(z-p+ 2)[(m-p+ 1)(z+ 1) +p(z-m)]$

$$
(z)((m+ 1) +n-p-1-h)
$$

$$
= (m+ 1)= (m+ 1)
$$

$$
pp
$$

Thay điều này vào (19), ta thu được $(17_{m+1})$, do đó (i).

Giả sử rằng $(^h_p)\in A'$ với $p < n$. Khi đó, với mọi $P\in \mathbf{Q}[T]$ có bậc $< n$ sao cho $P(\mathbf{Z})\subset \mathbf{Z}$, ta có $P(h)\in A'$ (no. 4, Hệ quả của Mệnh đề 2). Vì vậy, theo (16) với $m=n$,

$$
(h)(n-1-h)
$$

$(-1)^n$ =

$$
nn
$$

$$
^{n-1}_-(2n-p-1-h)_-'
$$

$=-x^{(n)}y^{(n)}+\sum y^{(np)}x^{(np)}\in A$ ;

$$
p
$$

$p=0$

do đó (ii) theo quy nạp trên $n$.

### 6. CÁC BIORDER TRONG ĐẠI SỐ BAO CỦA MỘT ĐẠI SỐ LIE REDUCTIVE TÁCH ĐƯỢC

Cho $\mathfrak{g}$ là một đại số Lie khả quy trên $\mathbf{Q},\mathfrak{h}$ là một đại số con Cartan tách của $\mathfrak{g}$, và $R = R(\mathfrak{g},\mathfrak{h}) ($§2, no. 1, Nhận xét 5).

#### Định nghĩa 1 {#lie-viii-s12-def-1 .statement tag=0183}

Một dàn $\mathscr{H}$ trong $\mathfrak{h}$ được gọi là chấp nhận được (đối với $\mathfrak{g}$) nếu, với mọi $\alpha \in R$, ta có $H_{\alpha}\in \mathscr{H}$ và $\alpha (\mathscr{H})\subset \mathbf{Z}$.

#### Nhận xét 1 {#lie-viii-s12-n6-rem-1 .statement tag=0184}

Cho B là một cơ sở của R. Một dàn $\mathscr{H}$ trong $\mathfrak{h}$ là chấp nhận được khi và chỉ khi $H_{\alpha}\in \mathscr{H}$ và $\alpha (\mathscr{H})\subset \mathbf{Z}$ với mọi $\alpha \in B$.

#### Nhận xét 2 {#lie-viii-s12-n6-rem-2 .statement tag=0185}

Cho $\mathfrak{c}$ là tâm của $\mathfrak{g}$. Khi đó, một dàn $\mathscr{H}$ trong $\mathfrak{h}$ là chấp nhận được khi và chỉ khi $Q(R^{\vee})\subset \mathscr{H}\subset P(R^{\vee})\oplus \mathfrak{c}$. Dàn $\mathscr{H}\cap \mathscr{D}\mathfrak{g}$ khi đó là chấp nhận được trong đại số con Cartan $\mathfrak{h}\cap \mathscr{D}\mathfrak{g}$ của $\mathscr{D}\mathfrak{g}$. Có thể tồn tại các dàn chấp nhận được $\mathscr{H}$ sao cho $\mathscr{H}\not= (\mathscr{H}\cap \mathscr{D}\mathfrak{g})\oplus (\mathscr{H}\cap \mathfrak{c})$ (xem §13, no. 1.IX).

#### Nhận xét 3 {#lie-viii-s12-n6-rem-3 .statement tag=0186}

Nếu $\mathfrak{g}$ là nửa đơn, các dàn chấp nhận được trong $\mathfrak{h}$ là các nhóm con $\mathscr{H}$ của $\mathfrak{h}$ sao cho $Q(R^{\vee})\subset \mathscr{H}\subset P(R^{\vee})$.

Trong phần còn lại của số này, ta giả sử cố định một đại số Lie reductive tách được $(\mathfrak{g},\mathfrak{h})$, một cơ sở B của $R = R(\mathfrak{g},\mathfrak{h})$ và, với mỗi $\alpha \in B$, một cặp $(x_{\alpha}, y_{\alpha})$ với

$$
y_{\alpha}\in \mathfrak{g}^{-\alpha},x_{\alpha}\in \mathfrak{g}^{\alpha},[y_{\alpha}, x_{\alpha}] =H_{\alpha} \tag{20}
$$

Nếu ta ký hiệu bởi $\mathfrak{n}_+$ (tương ứng $\mathfrak{n}_-$) đại số con của $\mathfrak{g}$ sinh bởi các $x_{\alpha}$ (tương ứng các $y_{\alpha}$), ta biết (§3, no. 3, Mệnh đề 9 (iii)) rằng

$$
\mathfrak{g}=\mathfrak{n}_-\oplus \mathfrak{h}\oplus \mathfrak{n}_+ \tag{21}
$$

$$
U(\mathfrak{g}) = U(\mathfrak{n}_-)\otimes_{\mathbf{Q}}U(\mathfrak{h})\otimes_{\mathbf{Q}}U(\mathfrak{n}_+) \tag{22}
$$

(trong đó $U(\mathfrak{g}), . .$. là các đại số bao của $\mathfrak{g}, . . .$).

Ký hiệu $\mathscr{U}_+$ là đại số con $\mathbf{Z}$ của $U(\mathfrak{n}_+)$ sinh bởi các $x^{(n)}_{\alpha}$ với $\alpha \in B$ và $n\in \mathbf{N}$. Gọi W là nhóm Weyl của $R, R_+$ là tập hợp các căn dương đối với B.

#### Bổ đề 5 {#lie-viii-s12-lem-5 .statement tag=0187}

(i) $\mathscr{U}_+$ là một dàn trong không gian vectơ $U(\mathfrak{n}_+)$.

(ii) Với mọi $\alpha \in B$, ta có $\mathscr{U}_+\cap U(\mathfrak{g}^{\alpha}) =\bigoplus_{n\in\mathbf{N}}\mathbf{Z}x^{(n)}_{\alpha}$.

Theo định nghĩa, $\mathscr{U}_+$ được sinh như một $\mathbf{Z}$-môđun bởi các phần tử

$x(\varphi \mathbf{n})$ = $1\leq \prod i\leq rx(\varphi n((ii)$))

trong đó $r\in \mathbf{N},\varphi = (\varphi (i))\in B^r$, và $\mathbf{n}= (n(i))\in \mathbf{N}^r$. Trang bị cho đại số $U(\mathfrak{n}_+)$ phép phân bậc kiểu Q(R) mà với nó mỗi $\mathfrak{g}^{\alpha}(\alpha \in R_+)$ là thuần nhất có bậc $\alpha$. Một đơn thức $x^{(\mathbf{n})}_{\varphi}$ thuộc kiểu nói trên là thuần nhất có bậc

$$
\sum_{1\leq i\leq r}n(i)\varphi (i)\in Q(R)
$$

Các đơn thức thuộc kiểu này có một bậc cho trước $q$ là hữu hạn về số lượng, và sinh trên $\mathbf{Q}$ thành phần thuần nhất của $U(\mathfrak{n}_+)$ có bậc $q$. Điều này chứng minh (i).

Nếu $\alpha \in B,\mathscr{U}_+\cap U(\mathfrak{g}^{\alpha})$ được chứa trong tổng của các thành phần thuần nhất có các bậc là bội của $\alpha$; do đó, theo điều trên, $\mathscr{U}_+\cap U(\mathfrak{g}^{\alpha})$ được sinh bởi các $x^{(\mathbf{n})}_{\varphi}$ sao cho $\sum n(i)\varphi (i)\in \mathbf{N}\alpha$, điều này buộc $\varphi (i) =\alpha$ với mọi $i$ (vì B là một cơ sở của R), do đó

$x^{(\mathbf{n})}_{\varphi}=x^{(n(1))}_{\alpha}. . . x^{(n(r))}_{\alpha}=(n(1) +n$(1)!$\cdots . . . n+(nr$)!$(r$))! $x^{(n(1)+\cdot \cdot \cdot+n(r))}_{\alpha}$.

Vì vậy, $\mathscr{U}_+\cap \mathscr{U}(\mathfrak{g}^{\alpha})\subset \bigoplus_n\mathbf{Z}x^{(n)}_{\alpha}$, suy ra (ii). Q.E.D.

Trong phần còn lại của đoạn này, nếu E và F là các môđun con $\mathbf{Z}$ của $U(\mathfrak{g})$, ta ký hiệu bởi $E.F$ môđun con $\mathbf{Z}$ của $U(\mathfrak{g})$ sinh bởi các tích $ab$, trong đó $a\in E, b\in F$.

#### Mệnh đề 3 {#lie-viii-s12-prop-3 .statement tag=0188}

Cho $\mathscr{H}$ là một dàn cho phép trong $\mathfrak{h}$. Cho $\mathscr{U}_+,\mathscr{U}_-,\mathscr{U}_0$ là các $\mathbf{Z}$-đại số con của $U(\mathfrak{g})$ được sinh lần lượt bởi các phần tử $x_{\alpha}^{(n)}$ $(\alpha \in B,n\in \mathbf{N}),y_{\alpha}^{(n)}(\alpha \in B, n\in \mathbf{N}),(^h_n)(h\in \mathscr{H}, n\in \mathbf{N})$. Cho $\mathscr{U}$ là $\mathbf{Z}$-đại số con của $U(\mathfrak{g})$ được sinh bởi $\mathscr{U}_+,\mathscr{U}_-,\mathscr{U}_0$.

(i) $\mathscr{U}$ là một song thứ tự trong song đại số $U(\mathfrak{g})$.

(ii) Ta có $\mathscr{U}=\mathscr{U}_-.\mathscr{U}_0.\mathscr{U}_+,\mathscr{U}\cap \mathfrak{h}=\mathscr{H}$ và, với mọi $\alpha \in B$,

$$
\mathscr{U}\cap \mathfrak{g}^{\alpha}=\mathbf{Z}x_{\alpha},V\cap \mathfrak{g}^{-\alpha}=\mathbf{Z}y_{\alpha}
$$

Theo Bổ đề 5 và Mệnh đề $2,\mathscr{U}_+,\mathscr{U}_-,\mathscr{U}_0$ là các trật tự trong các $\mathbf{Q}$-đại số $U(\mathfrak{n}_+),U(\mathfrak{n}_-),U(\mathfrak{h})$, tương ứng, và

$$
(\pm h+q)
$$

$\in \mathscr{U}_0$ với $h\in \mathscr{H}, q\in \mathbf{Z}, p\in \mathbf{N}$. (23)

$$
p
$$

Đặt $\mathscr{L}=\mathscr{U}_-.\mathscr{U}_0.\mathscr{U}_+\subset U(\mathfrak{g})$. Theo (22), $\mathscr{L}$ là một dàn trong $U(\mathfrak{g})$. Theo phép dựng,

$$
\mathscr{U}_-.\mathscr{L}\subset \mathscr{L} \tag{24}
$$

$$
\mathscr{L}.\mathscr{U}_+\subset \mathscr{L} \tag{25}
$$

trong khi Bổ đề 3 và (23) suy ra rằng

$$
\mathscr{U}_0.\mathscr{L}\subset \mathscr{L} \tag{26}
$$

$$
\mathscr{L}.\mathscr{U}_0\subset \mathscr{L} \tag{27}
$$

Cho $\alpha \in B, n\in \mathbf{N}, r\in \mathbf{N}, \varphi = (\varphi (i))\in B^r$, và

$$
(m(1), . . . , m(r))\in \mathbf{N}^r
$$

Ta chứng minh rằng

$$
x^{(n)}_{\alpha}y_{\varphi(1)}^{(m(1))}. . . y_{\varphi(r)}^{(m(r))}\in \mathscr{L} \tag{28}
$$

hoặc tương đương, xét theo (25), rằng

$$
[x^{(n)}_{\alpha}, y^{(m(1))}_{\varphi(1)}. . . y_{\varphi(r)}^{(m(r))}]\in \mathscr{L} \tag{29}
$$

Ta lập luận bằng quy nạp theo $r$. Biểu thức móc cần xét là tổng của các hạng

$(m(1))(m(k))(n)(m(k+1))(m(k+2))(m(r))$

$y_{\varphi(1)}. . . y_{\varphi(k)}[x_{\alpha}, y_{\varphi(k+1)}]y_{\varphi(k+2)}. . . y_{\varphi(r)}$. (30) Với $\alpha \not=\varphi (k+ 1),x_{\alpha}$ và $y_{\varphi(k+1)}$ giao hoán, nên $[x^{(n)}_{\alpha}, y^{(m(k+1))}_{\varphi(k+1)}] = 0$. Nếu $\alpha =\varphi (k+ 1)$, thì biểu thức (30), theo (17), là tổng của các biểu thức có dạng

$(m(1))(m(k))(m(k+1)-p)(q-h)(n-p)(m(k+2))(m(r))$

$$
y_{\varphi(1)}. . . y_{\varphi(k)}y_{\varphi(k+1)}x_{\alpha}y_{\varphi(k+2)}. . . y_{\varphi(r)} \tag{31}
$$

$$
p
$$

trong đó $q\in \mathbf{Z}, p\in$ **N --** $\{0\}, h\in \mathscr{H}$. Giả thiết quy nạp, cùng với (24) và (26), chứng tỏ rằng biểu thức (31) thuộc $\mathscr{L}$. Vậy ta đã chứng minh (28).

Theo (28), $x^{(n)}_{\alpha}\mathscr{U}_-\subset \mathscr{L}$; do đó, theo (25) và (27), $x^{(n)}_{\alpha}\mathscr{L}\subset \mathscr{L}$, nên $\mathscr{U}_+.\mathscr{L}\subset \mathscr{L}$ và

$$
\mathscr{L}.\mathscr{L}\subset \mathscr{U}_-.\mathscr{U}_0.\mathscr{L}\subset \mathscr{U}_-.\mathscr{L}\subset \mathscr{L}
$$

Vậy, $\mathscr{L}$ là một $\mathbf{Z}$-đại số con của $U(\mathfrak{g})$, do đó $\mathscr{U}=\mathscr{L}$. Nếu $c$ là đồng tích của $U(\mathfrak{g})$, thì $c(\mathscr{U})\subset \mathscr{U}\otimes_{\mathbf{Z}}\mathscr{U}$ (no. 2, Mệnh đề 1). Gọi $\gamma$ là đồng đơn vị của $U(\mathfrak{g})$. Vì $\gamma (x^{(n)}_{\alpha}) =\gamma (y^{(n)}_{\alpha}) =\gamma ((^h_n))= 0$ với $n >0$, ta có $\gamma (\mathscr{U})\subset \mathbf{Z}$. Điều này chứng minh (i). Mặt khác,

$$
\mathscr{U}\cap \mathfrak{h}=\mathscr{L}\cap \mathfrak{h}=\mathscr{U}_0\cap \mathfrak{h}=\mathscr{H}
$$

theo Mệnh đề 2 của no. 4; tương tự,

$$
\mathscr{U}\cap \mathfrak{g}^{\alpha}=\mathscr{U}_+\cap \mathfrak{g}^{\alpha}=\mathbf{Z}x_{\alpha}
$$

theo Bổ đề 5. Điều này chứng minh (ii).

#### Nhận xét 4 {#lie-viii-s12-n6-rem-4 .statement tag=0189}

Theo Mệnh đề 5 của §4, no. 4, tồn tại một tự đẳng cấu duy nhất $\theta$ của $\mathfrak{g}$ sao cho $\theta (x_{\alpha}) =y_{\alpha}$ và $\theta (y_{\alpha}) =x_{\alpha}$ với mọi $\alpha \in B$, và $\theta (h) =-h$ với mọi $h\in \mathfrak{h}$; ta có $\theta^2= 1$. Theo cách dựng $\mathscr{U}$, ta thấy rằng tự đẳng cấu của $U(\mathfrak{g})$ kéo dài $\theta$ giữ $\mathscr{U}$ ổn định.

#### Hệ quả 1 {#lie-viii-s12-prop-3-cor-1 .statement tag=018A}

Đặt $\mathscr{G}=\mathscr{U}\cap \mathfrak{g}$. Khi đó $\mathscr{G}$ là một thứ tự trong đại số Lie $\mathfrak{g}$, ổn định dưới $\theta$. Ta có $\mathscr{G}=\mathscr{H}+\sum_{\alpha\in R}(\mathscr{G}\cap \mathfrak{g}^{\alpha})$. Với mọi $\alpha \in B$ và mọi $n\in \mathbf{N}$, các ánh xạ (ad $x_{\alpha}$)$^n/n$!, (ad $y_{\alpha}$)$^n/n$! giữ $\mathscr{U}$ và $\mathscr{G}$ ổn định.

Khẳng định thứ nhất là hiển nhiên. Khẳng định thứ hai suy ra bằng cách xét phân cấp kiểu Q(R) trên $U(\mathfrak{g})$ và $\mathscr{U}$. Khẳng định thứ ba suy ra từ Bổ đề 2 của no. 5.

#### Hệ quả 2 {#lie-viii-s12-prop-3-cor-2 .statement tag=018B}

Cho $w\in W$. Tồn tại một tự đẳng cấu sơ cấp $\varphi$ của $\mathfrak{g}$ giao hoán với $\theta$, giữ $\mathscr{G}$ và $\mathscr{U}$ ổn định, và mở rộng $w$.

Chỉ cần xét trường hợp trong đó $w$ có dạng $s_{\alpha}(\alpha \in B)$. Trước hết, chú ý rằng ad $x_{\alpha}$ và ad $y_{\alpha}$ là lũy linh địa phương trên $U(\mathfrak{g})$, nói cách khác, với mọi $u\in U(\mathfrak{g})$ tồn tại một số nguyên $n$ sao cho (ad $x_{\alpha}$)$^nu=$ (ad $y_{\alpha}$)$^nu= 0$.

Điều này cho phép định nghĩa các tự đẳng cấu $e^{adx_{\alpha}}=\sum_{n=0}^{\infty}\frac{1}{n!}$(ad $x_{\alpha}$)$^n$ và $e^{ady_{\alpha}}$ của $U(\mathfrak{g})$; ta kiểm tra ngay lập tức rằng các tự đẳng cấu này của $U(\mathfrak{g})$ để $\mathscr{U}$ ổn định. Đặt $\varphi_1=e^{adx_{\alpha}}e^{ady_{\alpha}}e^{adx_{\alpha}},\varphi_2=e^{ady_{\alpha}}e^{adx_{\alpha}}e^{ady_{\alpha}}$. Ta có $\varphi_1|\mathfrak{g}=$ $\varphi_2|\mathfrak{g}($§2, no. 2, công thức (1)), nên $\varphi_1=\varphi_2$. Đặt $\varphi_1=\varphi_2=\varphi$. Ta có $\theta \varphi \theta^{-1}=\varphi$, nên $\theta$ và $\varphi$ giao hoán. Mặt khác, $\varphi |\mathfrak{h}=w$ theo §2, no. 2, Bổ đề 1.

#### Hệ quả 3 {#lie-viii-s12-prop-3-cor-3 .statement tag=018C}

Cho $\alpha \in R$. Nếu $x\in \mathscr{G}\cap \mathfrak{g}^{\alpha}$ và $n\in \mathbf{N}$, ta có $x^{(n)}\in \mathscr{U}$, và (ad $x$)$^n/n$! để $\mathscr{G}$ và $\mathscr{U}$ ổn định.

Điều này hiển nhiên nếu $\alpha \in B$, theo cách dựng của $\mathscr{U}$ và Hệ quả 1. Trong trường hợp tổng quát, tồn tại $w\in W$ sao cho $w(\alpha )\in B$ (Chương VI, §1, no. 5, Mệnh đề 15). Theo Hệ quả 2, tồn tại một tự đẳng cấu $\varphi$ của $\mathfrak{g}$ để $\mathscr{G}$ và $\mathscr{U}$ ổn định và đưa $\mathfrak{g}^{\alpha}$ đến $\mathfrak{g}^{w(\alpha)}$, do đó có hệ quả nhờ phép chuyển cấu trúc.

#### Hệ quả 4 {#lie-viii-s12-prop-3-cor-4 .statement tag=018D}

Tồn tại một hệ Chevalley $(X_{\alpha})_{\alpha\in R}$ trong $(\mathfrak{g},\mathfrak{h}) ($§2, no. 4, Định nghĩa 3) sao cho $X_{\alpha}=x_{\alpha}$ và $X_{-\alpha}=y_{\alpha}$ với $\alpha \in B$. Với mọi hệ Chevalley $(X'_{\alpha})_{\alpha\in R}$ có các tính chất này, và với mọi $\alpha \in R,X'_{\alpha}$ là một cơ sở của $\mathscr{G}\cap \mathfrak{g}^{\alpha}$.

Với $\alpha \in B$, đặt $X_{\alpha}=x_{\alpha}, X_{-\alpha}=y_{\alpha}$. Với $\alpha \in R_+$ **--** B, chọn một $w\in W$ sao cho $w(\alpha )\in B$ và một tự đẳng cấu $\varphi$ của $\mathfrak{g}$ sao cho $\theta \varphi =\varphi \theta ,\varphi (\mathscr{G}) =\mathscr{G}$ và $\varphi (h) =w^{-1}(h)$ với $h\in \mathfrak{h}$ (Hệ quả 2); đặt $X_{\alpha}=\varphi (x_{w(\alpha)}), X_{-\alpha}=\varphi (y_{w(\alpha)})$. Khi đó

$$
[X_{-\alpha}, X_{\alpha}] =\varphi ([y_{w(\alpha)}, x_{w(\alpha)}]) =\varphi (H_{w(\alpha)}) =w^{-1}(H_{w(\alpha)}) =H_{\alpha}
$$

$$
\theta (X_{\alpha}) =\theta \varphi (x_{w(\alpha)}) =\varphi \theta (x_{w(\alpha)}) =\varphi (y_{w(\alpha)}) =X_{-\alpha}
$$

nên $(X_{\alpha})_{\alpha\in R}$ là một hệ Chevalley. Hơn nữa,

$$
\mathscr{G}\cap \mathfrak{g}^{\alpha}=\varphi (\mathscr{G}\cap \mathfrak{g}^{w(\alpha)}) =\varphi (\mathbf{Z}x_{w(\alpha)}) =\mathbf{Z}X_{\alpha} \tag{32}
$$

$$
\mathscr{G}\cap \mathfrak{g}^{-\alpha}=\varphi (\mathscr{G}\cap \mathfrak{g}^{-w(\alpha)}) =\varphi (\mathbf{Z}y_{w(\alpha)}) =\mathbf{Z}X_{-\alpha} \tag{33}
$$

Cho $(X'_{\alpha})_{\alpha\in R}$ là một hệ Chevalley sao cho $X'_{\alpha}=x_{\alpha}, X'_{-\alpha}=y_{\alpha}$ với $\alpha \in B$. Gọi S là tập hợp các $\alpha \in R$ sao cho $X'_{\alpha}=\pm X_{\alpha}$. Theo §2, no. 4, Mệnh đề 7, S là một tập nghiệm đóng. Vì $S\supset B\cup (-B)$, ta có S = R (Chương VI, §1, no. 6, Mệnh đề 19). Do đó, theo (32) và (33), ta có $\mathscr{G}\cap \mathfrak{g}^{\alpha}=\mathbf{Z}X'_{\alpha}$ với mọi $\alpha \in R$.

#### Nhận xét 5 {#lie-viii-s12-n6-rem-5 .statement tag=018E}

Cho $(X_{\alpha})_{\alpha\in R}$ là hệ Chevalley được xây dựng ở trên. Nếu $\alpha , \beta , \alpha +\beta \in R$ và nếu ta đặt $[X_{\alpha}, X_{\beta}] = N_{\alpha ,\beta}X_{\alpha+\beta}$, ta có $[X_{\alpha}, X_{\beta}]\in$ $\mathscr{G}\cap \mathfrak{g}^{\alpha+\beta}$, và ta suy ra được rằng $N_{\alpha ,\beta}\in \mathbf{Z}$ (xem §2, no. 4, Mệnh đề 7).

#### Nhận xét 6 {#lie-viii-s12-n6-rem-6 .statement tag=018F}

Ta đã thu được nhân tiện một chứng minh mới về sự tồn tại của các hệ Chevalley (xem §4, no. 4, Hệ quả của Mệnh đề 5), độc lập với Bổ đề 4, §2.

### 7. CÁC TRẬT TỰ CHEVALLEY

Cho $(\mathfrak{g},\mathfrak{h})$ là một đại số Lie reductive tách được trên $\mathbf{Q}, R$ là hệ nghiệm của nó. Hãy chọn:

a) một dàn cho phép $\mathscr{H}$ trong $\mathfrak{h}$ (no. 6, Định nghĩa 1);

b) với mọi $\alpha \in R$, một dàn $\mathscr{G}^{\alpha}$ trong $\mathfrak{g}^{\alpha}$.

Đặt $\mathscr{G}=\mathscr{H}\oplus \sum_{\alpha\in R}\mathscr{G}^{\alpha}$. Đó là một dàn trong $\mathfrak{g}$. Ký hiệu $\mathscr{U}$ là $\mathbf{Z}$-đại số con của $U(\mathfrak{g})$ sinh bởi các $(^h_n)(h\in \mathscr{H}, n\in \mathbf{N})$ và các $x^{(n)}(x\in \mathscr{G}^{\alpha}, \alpha \in R$, $n\in \mathbf{N})$. Cuối cùng, với $\alpha \in R$ và $x\in \mathfrak{g}^{\alpha}$ **--** $\{0\}$, đặt

$w_{\alpha}(x) =$ (exp ad $x$)(exp ad $y$)(exp ad $x$),

trong đó $y$ là phần tử duy nhất của $\mathfrak{g}^{-\alpha}$ sao cho $[y, x] =H_{\alpha}$. Với các ký hiệu này:

#### Định lý 2 {#lie-viii-s12-thm-2 .statement tag=018G}

Các điều kiện sau là tương đương:

(i) Tồn tại một hệ Chevalley $(X_{\alpha})_{\alpha\in R}$ của $(\mathfrak{g},\mathfrak{h})$ sao cho $\mathscr{G}_{\alpha}=\mathbf{Z}X_{\alpha}$ với mọi $\alpha \in R$.

(ii) $\mathscr{U}\cap \mathfrak{g}=\mathscr{G}$ và $[\mathscr{G}^{\alpha},\mathscr{G}^{-\alpha}] =\mathbf{Z}H_{\alpha}$ với mọi $\alpha \in R$.

(iii) Với mọi $\alpha \in R, x\in \mathscr{G}^{\alpha}, n\in \mathbf{N}$, tự đồng cấu (ad $x$)$^n/n$! của $\mathfrak{g}$ biến $\mathscr{G}$ thành $\mathscr{G}$, và $[\mathscr{G}^{\alpha},\mathscr{G}^{-\alpha}] =\mathbf{Z}H_{\alpha}$.

Với mọi $\alpha \in R$ và mọi cơ sở $x$ của $\mathscr{G}^{\alpha},w_{\alpha}(x)$ ánh xạ $\mathscr{G}$ vào $\mathscr{G}$($\text{nghĩa là, }\!$ ánh xạ $\mathscr{G}^{\beta}$ vào $\mathscr{G}^{s_{\alpha}(\beta)}$ với mọi $\beta \in R)$.

(i) $=\Rightarrow$ (ii): cho $(X_{\alpha})_{\alpha\in R}$ là một hệ Chevalley trong $(\mathfrak{g},\mathfrak{h})$ sao cho $\mathscr{G}^{\alpha}=$ $\mathbf{Z}X_{\alpha}$ với mọi $\alpha \in R$, và cho B là một cơ sở của R. Với $\alpha \in B$, đặt $x_{\alpha}=X_{\alpha}, y_{\alpha}=$ $X_{-\alpha}$. Cho $\mathscr{U}'$ là song thứ tự liên kết theo Mệnh đề 3 của no. 6 với $\mathscr{H}$, các $x_{\alpha}$ và các $y_{\alpha}$. Rõ ràng là $\mathscr{U}'\subset \mathscr{U}$. Theo Hệ quả 3 và 4 của Mệnh đề $3,x^{(n)}\in \mathscr{U}'$ với mọi $\alpha \in R,x\in \mathscr{G}^{\alpha}$ và $n\in \mathbf{N}$. Vậy $\mathscr{U}=\mathscr{U}'$, điều đó chứng minh (ii).

(ii) $=\Rightarrow$ (iii): điều này rõ ràng theo Bổ đề 2 của no. 5.

(iii) $=\Rightarrow$ (iv): cho $\alpha \in R$ và cho $x$ là một cơ sở của $\mathscr{G}^{\alpha}$. Vì $[\mathscr{G}^{\alpha},\mathscr{G}^{-\alpha}] =\mathbf{Z}H_{\alpha}$, nên $y\in \mathfrak{g}^{-\alpha}$ duy nhất sao cho $[y, x] =H_{\alpha}$ thuộc $\mathscr{G}^{-\alpha}$. Vì exp ad $x$ và exp ad $y$ giữ $\mathscr{G}$ ổn định theo (iii), nên $w_{\alpha}(x)$ cũng vậy.

(iv) $=\Rightarrow$ (i): cho B là một cơ sở của R. Chọn một cơ sở $x_{\alpha}$ của $\mathscr{G}^{\alpha}$ với mọi $\alpha \in B$. Cho $y_{\alpha}\in \mathscr{G}^{-\alpha}$ sao cho $[y_{\alpha}, x_{\alpha}] =H_{\alpha}$. Theo §1, no. 5, các công thức (5), ta có $y_{\alpha}=w_{\alpha}(x_{\alpha}).x_{\alpha}$ nên $y_{\alpha}$ là một cơ sở của $\mathscr{G}^{-\alpha}$ theo (iv). Cho $\mathscr{G}'$ là cấp trong $\mathfrak{g}$ được xác định bởi $\mathscr{H}$, các $x_{\alpha}$ và các $y_{\alpha}$ (no. 6, Hệ quả 1 của Mệnh đề 3). Khi đó $\mathscr{G}'$ ổn định dưới các (ad $x_{\alpha}$)$^n/n$!, (ad $y_{\alpha}$)$^n/n$! (loc. cit.), và do đó dưới các $w_{\alpha}(x_{\alpha})$.

Cho $\beta \in R$. Tồn tại $\alpha_0, \alpha_1, . . . , \alpha_r\in B$ sao cho

$$
\beta =s_{\alpha_r}s_{\alpha_{r-1}}. . . s_{\alpha_1}(\alpha_0)
$$

(Chương VI, §1, mục 5, Mệnh đề 15). Khi đó $w_{\alpha_r}(x_{\alpha_r}).w_{\alpha_{r-1}}(x_{\alpha_{r-1}}). . . w_{\alpha_1}(x_{\alpha_1})$ ánh xạ $\mathscr{G}^{\alpha_0}$ vào $\mathscr{G}^{\beta}$ theo (iv), và ánh xạ $\mathscr{G}'\cap \mathfrak{g}^{\alpha_0}$ vào $\mathscr{G}'\cap \mathfrak{g}^{\beta}$ theo kết quả trước. Vì $\mathscr{G}'\cap \mathfrak{g}^{\alpha_0}=\mathscr{G}^{\alpha_0}$ (Mệnh đề 3 (ii)), ta có $\mathscr{G}'\cap \mathfrak{g}^{\beta}=\mathscr{G}^{\beta}$. Do đó

$$
\mathscr{G}'=\mathscr{H}\oplus \sum_{\beta\in R}(\mathscr{G}'\cap \mathfrak{g}^{\beta}) =\mathscr{H}\oplus \sum_{\beta\in R}\mathscr{G}^{\beta}=\mathscr{G}
$$

và Hệ quả 4 của Mệnh đề 3 kết thúc chứng minh.

#### Định nghĩa 2 {#lie-viii-s12-def-2 .statement tag=018H}

Khi các điều kiện (i) đến (iv) của Định lý 2 được thỏa mãn, $\mathscr{G}$ được gọi là một cấp Chevalley trong $(\mathfrak{g},\mathfrak{h})$.

#### Nhận xét {#lie-viii-s12-n7-rem-1 .statement tag=018I}

Các cấp Chevalley trong $(\mathfrak{g},\mathfrak{h})$ luôn tồn tại. Thật vậy, các cấp Chevalley là các tập hợp có dạng $\mathscr{H}\oplus \sum_{\alpha\in R}\mathbf{Z}X_{\alpha}$, trong đó $(X_{\alpha})_{\alpha\in R}$ là một hệ Chevalley trong $(\mathfrak{g},\mathfrak{h})$ và $\mathscr{H}$ là một dàn trong $\mathfrak{h}$ sao cho

$$
Q(R^{\vee})\subset \mathscr{H}\subset P(R^{\vee})\oplus \mathfrak{c}
$$

( $\mathfrak{c}$ là tâm của $\mathfrak{g}$).

#### Định lý 3 {#lie-viii-s12-thm-3 .statement tag=018J}

Ta giữ các ký hiệu ở đầu mục 7, và giả sử rằng $\mathscr{G}$ là một cấp Chevalley trong $(\mathfrak{g},\mathfrak{h})$.

(i) $\mathscr{U}$ là một song thứ tự trong $U(\mathfrak{g})$.

(ii) Cho B là một cơ sở của R, và $(X_{\alpha})_{\alpha\in B\cup(-B)}$ là một họ các phần tử của $\mathfrak{g}$ sao cho $\mathscr{G}^{\alpha}=\mathbf{Z}X_{\alpha}$ với $\alpha \in B\cup (-B)$. $\mathbf{Z}$-đại số $\mathscr{U}$ được sinh bởi các $(^h_n)$ và các $X_{\alpha}^{(n)}(h\in \mathscr{H}, \alpha \in B\cup (-B), n\in \mathbf{N})$. Nếu $\mathfrak{g}$ là nửa đơn và $\mathscr{H}= Q(R^{\vee})$, thì $\mathbf{Z}$-đại số $\mathscr{U}$ được sinh bởi các $X_{\alpha}^{(n)}(\alpha \in B\cup (-B), n\in \mathbf{N})$.

(iii) Cho B là một cơ sở của R, $R_+$ là tập hợp các nghiệm dương tương ứng, $R_-=-R_+,\mathfrak{n}_+=\sum_{\alpha\in R_+}\mathfrak{g}^{\alpha},\mathfrak{n}_-=\sum_{\alpha\in R_-}\mathfrak{g}^{\alpha}$. Khi đó,

$$
\mathscr{U}= (\mathscr{U}\cap U(\mathfrak{n}_-)).(\mathscr{U}\cap U(\mathfrak{h})).(\mathscr{U}\cap U(\mathfrak{n}_+))
$$

Cho $(h_i)_{i\in I}$ là một cơ sở của $\mathscr{H}$. Với mọi $\alpha \in R$, cho $X_{\alpha}$ là một cơ sở của $\mathscr{G}^{\alpha}$. Đặt cho tập $I\cup R$ một thứ tự toàn phần (ta giả sử rằng $I\cap R =\emptyset$ ). Với $\lambda \in I\cup R$ và $n\in \mathbf{N}$, đặt $e^{\langle n\rangle}_{\lambda}=(^{h_{\lambda}}_n)$ nếu $\lambda \in I,e^{\langle n\rangle}_{\lambda}=X_{\lambda}^{(n)}$ nếu $\lambda \in R$. Khi đó các tích $\prod_{\lambda\in I\cup R}e^{\langle n_{\lambda}\rangle}_{\lambda}$, trong đó $(n_{\lambda})$ thuộc $\mathbf{N}^{I\cup R}$, tạo thành một cơ sở của $\mathbf{Z}$-môđun $\mathscr{U}$. Các

Các tích $\prod_{\lambda\in I}(^{h_{\lambda}}_{n_{\lambda}})$, với $(n_{\lambda})$ thuộc $\mathbf{N}^I$, tạo thành một cơ sở của $\mathbf{Z}$-môđun $\mathscr{U}\cap U(\mathfrak{h})$. Các tích $\prod_{\lambda\in R_+}X_{\lambda}^{(n_{\lambda})}$, với $(n_{\lambda})$ thuộc $\mathbf{N}^{R_+}$, tạo thành một cơ sở của $\mathbf{Z}$-môđun $\mathscr{U}\cap U(\mathfrak{n}_+)$.

Cho B và $(X_{\alpha})_{\alpha\in B\cup(-B)}$ như trong (ii), và sao cho $[X_{-\alpha}, X_{\alpha}] =H_{\alpha}$. Gọi $\mathscr{U}'$ là $\mathbf{Z}$-đại số con của $U(\mathfrak{g})$ sinh bởi các $(_n^h)$ và các $X_{\alpha}^{(n)}$ $(h\in \mathscr{H}, \alpha \in B\cup (-B), n\in \mathbf{N})$. Ta đã thấy trong chứng minh Định lý 2, (i) $=\Rightarrow$ (ii), rằng $\mathscr{U}'$ bằng $\mathscr{U}$ và là một song thứ tự trong $U(\mathfrak{g})$. Điều đó chứng minh (i) và khẳng định đầu tiên của (ii); khẳng định thứ hai suy ra từ Bổ đề 4 (ii). Khẳng định (iii) suy ra từ Định lý 1 (no. 3) và Mệnh đề 3 (no. 6).

### 8. MẠNG CHẤP NHẬN ĐƯỢC

Khái quát hóa thuật ngữ đã dùng cho các không gian vectơ, một tự đồng cấu $u$ của một môđun M được gọi là chéo hóa được nếu tồn tại một cơ sở của M sao cho ma trận của $u$ theo cơ sở này là đường chéo.

#### Bổ đề 6 {#lie-viii-s12-lem-6 .statement tag=018K}

Cho M là một $\mathbf{Z}$-môđun tự do hữu hạn sinh, $u$ một tự đồng cấu của M, và $v$ là tự đồng cấu $u\otimes 1$ của $M\otimes_{\mathbf{Z}}\mathbf{Q}$. Giả sử rằng $(^v_n)(M)\subset M$ với mọi $n\in \mathbf{N}$. Khi đó $u$ chéo hóa được.

a) Với mọi đa thức $P\in \mathbf{Q}[T]$ sao cho $P(\mathbf{Z})\subset \mathbf{Z}$, ta có $P(v)(M)\subset M$ (no. 4, Hệ quả của Mệnh đề 2), nên det $P(v)\in \mathbf{Z}$.

b) Ký hiệu $\chi_v(t) =t^d+\alpha_1t^{d-1}+\cdots$ là đa thức đặc trưng của $v$. Cho $k\in \mathbf{Z}, n\in \mathbf{N}$. Áp dụng a) cho đa thức $(^{T-k}_n)$, ta thấy rằng số

$a_n=$ det $(v-k)=1_d$ det($v-k$) det($v-k-1$)$. .$ det($v-k-n+ 1$)

$n(n$!)

$$
=\frac{(-1)^n}{4}\chi_v(k)\chi_v(k+ 1). . . \chi_v(k+n-1)
$$

$(n$!)

là một số nguyên. Lấy $k-1<-\alpha_1/d$. Khi đó

$$
\chi_v(k+n-1) =n^d+ (\alpha_1+ (k-1)d)n^{d-1}+\cdots
$$

và

$$
|a_n|=\frac{|\chi_v(k + n- 1)|}{d}|a_{n-1}|
$$

$$
n
$$

suy ra, nếu $a_n\not= 0$ với mọi $n\in \mathbf{N}$, thì dãy các $|a_n|$ giảm nghiêm ngặt khi $n$ đủ lớn, điều này là vô lý. Suy ra $v$ có một trị riêng nguyên $\lambda$. Đặt $M'=$ Ker($u-\lambda .1$) và $M''= M/M'$. Khi đó $M'$ là giao với $M$ của một không gian con vectơ của $M\otimes_{\mathbf{Z}}\mathbf{Q}$, nên $\mathbf{Z}$-môđun $M''$ là không xoắn, kiểu hữu hạn, và do đó tự do có hạng $< d$. Lập luận bằng quy nạp theo $d$ và áp dụng giả thiết quy nạp cho tự đồng cấu của $M''$ cảm sinh bởi $u$, ta kết luận rằng mọi trị riêng của $v$ trong một mở rộng đóng đại số của $\mathbf{Q}$ đều là số nguyên.

c) Ta ցույց minh rằng $v$ chéo hóa được. Cho $\lambda$ là một trị riêng của $v$ và cho $x\in M\otimes_{\mathbf{Z}}\mathbf{Q}$ sao cho $(v-\lambda )^2x= 0$. Ta có $v(vx-\lambda x) =\lambda (vx-\lambda x)$, nên

$n1$!$(v-\lambda -n+ 1)(v-\lambda -n+ 2). . .(v-\lambda -1)(v-\lambda )x$

$$
=\frac{(-1)^{n-1}}{n}(vx-\lambda x)
$$

Theo a), điều này suy ra $vx-\lambda x\in nM$ với mọi $n\in \mathbf{N}$, nên $(v-\lambda )x= 0$.

d) Cho $\lambda$ là một trị riêng của $v$ và cho $\lambda -a, \lambda +b$ là một khoảng trong $\mathbf{Z}$ chứa mọi trị riêng của $v$. Xét đa thức

$$
(T-\lambda -1)(T-\lambda -2). . .(T-\lambda -b)
$$

$$
P(T) = (-1)^b
$$

$b$!

$$
(T-\lambda + 1)(T-\lambda + 2). . .(T-\lambda +a)
$$

$$
\times
$$

$a$!

Ta có $P(\mathbf{Z})\subset \mathbf{Z},P(\lambda ) = 1,P(\mu) = 0$ với $\mu\in \mathbf{Z}\cap (\lambda -a, \lambda +b)$ và $\mu\not=\lambda$. Theo $a), P(v)(M)\subset M$. Theo $c), P(v)$ là một phép chiếu của $M\otimes_{\mathbf{Z}}\mathbf{Q}$ lên không gian riêng tương ứng với $\lambda$. ĐPCM.

#### Nhận xét 1 {#lie-viii-s12-n8-rem-1 .statement tag=018L}

Nếu chỉ giả sử rằng $v$ chéo hóa được với các trị riêng nguyên, thì $u$ không nhất thiết chéo hóa được (ví dụ, lấy $M =\mathbf{Z}^2$ và $u(x, y) =$ $(y, x)$ với mọi $(x, y)\in M$).

Cho $\mathfrak{g},\mathfrak{h},R,\mathscr{H},\mathscr{G}^{\alpha},\mathscr{G},\mathscr{U}$ như ở no. 7, và giả sử rằng $\mathscr{G}$ là một thứ tự Chevalley trong $(\mathfrak{g},\mathfrak{h})$.

#### Định nghĩa 3 {#lie-viii-s12-def-3 .statement tag=018M}

Cho E là một $\mathfrak{g}$-môđun. Một dàn $\mathscr{E}$ trong E được gọi là chấp nhận được (đối với $\mathscr{G}$) nếu các điều kiện sau được thỏa mãn:

(i) $\mathscr{U}$ đưa $\mathscr{E}$ vào $\mathscr{E}$;

(ii) $\mathscr{E}$ ổn định dưới $(^h_n)$ và $x^{(n)}$ với mọi $\alpha \in R, x\in \mathscr{G}^{\alpha}, n\in \mathbf{N}, h\in \mathscr{H}$.

#### Nhận xét 2 {#lie-viii-s12-n8-rem-2 .statement tag=018N}

Cho $\rho$ là biểu diễn adjoint của $\mathfrak{g}$ trên $U(\mathfrak{g})$. Cho $\alpha , x, n, h$ như ở (ii) trên. Ta có $\rho (x^{(n)}).\mathscr{U}\subset \mathscr{U}$ theo Bổ đề 2. Mặt khác, nếu $p\in \mathbf{N}$,

$((h))_{(n)}($ ad $h)_{(n)}(n\alpha (h))_{(n)}$

$\rho x$ = $x$ = $x$

$$
ppp
$$

(no. 5, công thức (13)), nên $\rho ((^h_p)).\mathscr{U}\subset \mathscr{U}$. Điều này chứng tỏ rằng $\mathscr{U}$ là một dàn chấp nhận được trong $U(\mathfrak{g})$, và suy ra rằng $\mathscr{G}$ là một dàn chấp nhận được trong $\mathfrak{g}$ (đối với biểu diễn adjoint).

#### Nhận xét 3 {#lie-viii-s12-n8-rem-3 .statement tag=018O}

Cho E là một $\mathfrak{g}$-môđun hữu hạn chiều, $\mathscr{E}$ một dàn chấp nhận được trong E, $\mathfrak{c}$ là tâm của $\mathfrak{g}$. Theo Bổ đề 6, mọi phần tử của $\mathfrak{c}$ xác định một tự đồng cấu chéo hóa được của E. Do đó E là nửa đơn (Chương I, §6, no. 5, Định lý 4). Vì vậy, E là một tổng trực tiếp của các $\mathscr{D}\mathfrak{g}$-môđun đơn trên đó $\mathfrak{c}$ tác động bằng các phép nhân vô hướng. Theo Bổ đề $6,\mathscr{E}=\oplus (\mathscr{E}\cap E^{\lambda})$ và, với mọi trọng số $\lambda$ của E, ta có

$$
\lambda (\mathscr{H})\subset \mathbf{Z}
$$

#### Nhận xét 4 {#lie-viii-s12-n8-rem-4 .statement tag=018P}

Nếu $\mathfrak{g}$ là nửa đơn và $\mathscr{H}= Q(R^{\vee})$, các điều kiện (i) và (ii) của Định nghĩa 3, theo Định lý 3 (ii), tương đương với

(iii) $\mathscr{E}$ ổn định dưới $x^{(n)}$ với mọi $\alpha \in R, x\in \mathscr{G}^{\alpha}, n\in \mathbf{N}$.

#### Nhận xét 5 {#lie-viii-s12-n8-rem-5 .statement tag=018Q}

Cho B là một cơ sở của R; trong các điều kiện (i) và (ii) ở trên, “$\alpha \in$ R” có thể được thay bằng “$\alpha \in B\cup (-$B)” (loc. cit).

#### Định lý 4 {#lie-viii-s12-thm-4 .statement tag=018R}

Cho E là một $\mathfrak{g}$-môđun hữu hạn chiều. Các điều kiện sau là tương đương:

(i) E có một dàn chấp nhận được;

(ii) mọi phần tử của $\mathscr{H}$ xác định một tự đồng cấu chéo hóa được của E với các giá trị riêng nguyên.

(i) $=\Rightarrow$ (ii): điều này suy ra từ Nhận xét 3.

(ii) $=\Rightarrow$ (i): ta giả sử rằng điều kiện (ii) được thỏa mãn và chứng minh (i). Theo ĐL. 4 của Ch. I, §6, no. 5, ta có thể giả sử rằng các phần tử của $\mathfrak{c}$ xác định các phép vị tự của E, và rằng E là một $\mathscr{D}\mathfrak{g}$-môđun đơn. Cho B là một cơ sở của R, và $\mathfrak{g}=\mathfrak{n}_-\oplus \mathfrak{h}\oplus \mathfrak{n}_+$ là phân tích tương ứng của $\mathfrak{g}$. Cho $\lambda$ là trọng số cao nhất của $\mathscr{D}\mathfrak{g}$-môđun E, và cho $e\in E^{\lambda}$ **--** $\{0\}$. Đặt $\mathscr{E}=\mathscr{U}.e$. Hiển nhiên là $\mathscr{U}.\mathscr{E}\subset \mathscr{E}$. Vì E là đơn, $U(\mathfrak{g}).e= E$ và do đó $\mathscr{E}$ sinh ra E như một $\mathbf{Q}$-không gian vectơ. Với $h\in \mathscr{H}$ và $n\in \mathbf{N}$, ta có $(^h_n)e=(^{\lambda(h)}_n)e\in \mathbf{Z}e$, nên

$$
(\mathscr{U}\cap U(\mathfrak{h})).e=\mathbf{Z}e
$$

Vì $U(\mathfrak{n}_+).e= 0$, nên $\mathscr{E}= (\mathscr{U}\cap U(\mathfrak{n}_-)).e$ theo Mệnh đề 3. Suy ra từ ĐL. 3 (iii) rằng $\mathscr{E}$ là một $\mathbf{Z}$-môđun hữu hạn sinh.

#### Hệ quả {#lie-viii-s12-n8-cor-1 .statement tag=018S}

Nếu $\mathfrak{g}$ là nửa đơn và $\mathscr{H}= Q(R^{\vee})$, mọi $\mathfrak{g}$-môđun hữu hạn chiều đều có một dàn thích hợp.
