---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 16
section_title: Other Descriptions of the Brauer Group
lang: vi
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.285-A VIII.333
pdf_pages: 0302-0350
extraction: native+ocr
subsections:
    - "no": 1
      title: $\tau$-Extensions of Groups
      page: 285
      pdf_page: 302
    - "no": 2
      title: Inverse Image of a $\tau$-Extension
      page: 287
      pdf_page: 304
    - "no": 3
      title: Direct Image of a $\tau$-Extension
      page: 289
      pdf_page: 306
    - "no": 4
      title: Group Law on the Classes of $\tau$-Extensions
      page: 293
      pdf_page: 310
    - "no": 5
      title: Cohomological Description
      page: 295
      pdf_page: 312
    - "no": 6
      title: Restriction and Corestriction
      page: 299
      pdf_page: 316
    - "no": 7
      title: Galois Algebras
      page: 304
      pdf_page: 321
    - "no": 8
      title: Actions on Galois Algebras
      page: 312
      pdf_page: 329
    - "no": 9
      title: Cross Products
      page: 314
      pdf_page: 331
    - "no": 10
      title: Application to the Brauer Group
      page: 317
      pdf_page: 334
    - "no": 11
      title: Index and Exponent
      page: 322
      pdf_page: 339
statements: 63
exercises: 17
content_sha256: a4b95f74d5227bf31f1e907ee23d76417bdb313ab9ae588722d3c4929a344a62
translated_from: content/en/alg/VIII/16_s16_other_descriptions_of_the_brauer_group.md
source_content_sha256: 3713d8d9181c73ddbea13d385e233b08d04e96e3e2863da632e02fba79c6640c
translation_model: gpt-5.4-mini, gpt-5-6-mini, gpt-5-6
translation_run: translate-vi-0cbae7af
glossary_version: 34
glossary_terms_sha256: f638b5e3cf3de93f99c562b837854fdb1c1394a57501fc95bea45c381dad6721
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 16. CÁC MÔ TẢ KHÁC VỀ NHÓM BRAUER

Trong tiết diện này, nếu F là một nhóm Abel và $g$ là một tự đẳng cấu của F, thì ta viết $g\cdot f$ cho $g(f)$.

### 1. $\tau$-Các mở rộng của nhóm

Trong tiểu mục này, ta cố định một nhóm G, một nhóm Abel F viết theo phép nhân, và một đồng cấu nhóm $\tau$ từ G đến nhóm tự đẳng cấu Aut(F) của F. Kí hiệu phần tử đơn vị của G bởi $e$ và phần tử đơn vị của F bởi 1.

Nhắc lại (I, §6, No. 1, p. 65) rằng một mở rộng $\mathscr{E}$ của G bởi F là một bộ ba $(\Gamma , \iota , \pi )$, trong đó Γ là một nhóm, $\pi : \Gamma \rightarrow G$ là một đồng cấu toàn ánh, và $\iota$ là một đơn cấu từ F đến Γ sao cho Im($\iota$ ) $=$ Ker($\pi$ ). Cho $\mathscr{E}= (\Gamma , \iota , \pi )$ là một mở rộng như vậy. Với mọi $\gamma \in \Gamma$, ánh xạ $\varphi_{\gamma}: F\rightarrow F$ được xác định bởi

$$
\iota (\varphi_{\gamma}(f)) =\gamma \iota (f)\gamma^{-1}
$$

với $f\in F$ là một tự đẳng cấu của F. Vì F giao hoán, với mọi $f\in F$, tự đẳng cấu được xác định bởi $\iota (f)$ là ánh xạ đồng nhất trên F. Chuyển qua thương, ta thu được một đồng cấu Int$_{\mathscr{E}}$ từ G đến Aut(F) được đặc trưng bởi

$\gamma \iota (f)\gamma^{-1}=\iota$(Int$_{\mathscr{E}}(\pi (\gamma ))\cdot f$)

với $\gamma \in \Gamma$ và $f\in F$.

Một $A\tau$-mở rộng của G bởi F là một mở rộng $\mathscr{E}= (\Gamma , \iota , \pi )$ sao cho Int$_{\mathscr{E}}$ bằng $\tau$, nói cách khác, thỏa mãn quan hệ

$$
\gamma \iota (f)\gamma^{-1}=\iota (\tau (\pi (\gamma ))\cdot f) \tag{1}
$$

với $\gamma \in \Gamma$ và $f\in F$. Nếu $\mathscr{E}= (\Gamma , \iota , \pi )$ và $\mathscr{E}'= (\Gamma ', \iota ', \pi ')$ là các mở rộng $\tau$, thì một cấu xạ của các mở rộng $\tau$ từ $\mathscr{E}$ đến $\mathscr{E}'$ là một cấu xạ của các mở rộng từ $\mathscr{E}$ đến $\mathscr{E}'$ (I, §6, No. 1, p. 65), tức là một đồng cấu nhóm $u: \Gamma \rightarrow \Gamma '$ sao cho $\pi '\circ u=\pi$ và $\iota '=u\circ \iota$. Lưu ý rằng các mở rộng $\tau$ tạo thành một loài cấu trúc mà mọi cấu xạ đều là một đẳng cấu (Lý thuyết tập hợp, IV, §1, No. 5, p. 264 và I, §6, No. 1, p. 66, Mệnh đề 1). Kí hiệu Iso$_{\tau}(\mathscr{E},\mathscr{F})$ cho quan hệ

“$\mathscr{E}$ và $\mathscr{F}$ là các mở rộng $\tau$ đẳng cấu.”

Đây là một quan hệ tương đương; lớp của mở rộng $\mathscr{E}$ là lớp các đối tượng tương đương với $\mathscr{E}$ đối với Iso$_{\tau}$(Lý thuyết tập hợp, II, §6, No. 6, p. 122).

#### Bổ đề 1 {#alg-viii-s16-lem-1 .statement tag=00I9}

Quan hệ

“$\alpha$ là lớp của một $\tau$-mở rộng đối với Iso$_{\tau}$”

là xác định tập trong $\alpha$.

Đặt $E_0= F\times G$, và xét các ánh xạ $\iota_0: F\rightarrow E_0$ và $\pi_0: E_0\rightarrow G$ được xác định bởi $\iota_0(f) = (f, e)$ với $f\in F$ và $\pi_0(f, g) =g$ với $(f, g)\in F\times G$. Cho $\mathscr{E}= (\Gamma , \iota , \pi )$ là một $\tau$-mở rộng của G bởi F. Ánh xạ $\pi$ là toàn ánh, nên có một tiết diện $\sigma : G\rightarrow \Gamma$ sao cho $\sigma (e) =e$. Ánh xạ $u: (f, g)\mapsto \iota (f)\sigma (g)$ từ $F\times G$ đến Γ là song ánh. Ta trang bị cho $F\times G$ luật nhóm thu được bằng cách chuyển cấu trúc. Khi đó bộ ba $(E_0, \iota_0, \pi_0)$ là một $\tau$-mở rộng đẳng cấu với $\mathscr{E}$. Bổ đề 1 bây giờ suy ra từ Lý thuyết tập hợp, II, §6, No. 6, p. 122.

Ta ký hiệu bởi Ex$_{\tau}(G,F)$ tập hợp các lớp của các $\tau$-mở rộng đối với quan hệ Iso$_{\tau}$.

#### Ví dụ 1 {#alg-viii-s16-n1-exa-1 .statement tag=00IA}

Tích nửa trực tiếp ngoài $(F\times_{\tau}G, i, p)$ (I, §6, No. 1, p. 66, Mệnh đề 3) là một $\tau$-mở rộng; ta ký hiệu nó bởi $\mathscr{I}_{\tau}$. Ta nói rằng một $\tau$-mở rộng là nửa tầm thường nếu nó đẳng cấu với $\tau$-mở rộng $\mathscr{I}_{\tau}$.

#### Ví dụ 2 {#alg-viii-s16-n1-exa-2 .statement tag=00IB}

Với $i\in  \{1,2\}$, lấy một nhóm $G_i$, một nhóm Abel $F_i$, và một đồng cấu nhóm $\tau_i$ từ $G_i$ đến nhóm tự đẳng cấu của $F_i$. Ta ký hiệu bởi $\tau_1\times \tau_2: G_1\times G_2\rightarrow$ Aut(F$_1\times F_2$) đồng cấu được xác định bởi

$$
(\tau_1\times \tau_2)(g_1, g_2)\cdot (f_1, f_2) = (\tau_1(g_1)\cdot f_1, \tau_2(g_2)\cdot f_2)
$$

với $g_1\in G_1,g_2\in G_2,f_1\in F_1$, và $f_2\in F_2$. Cho $\mathscr{E}_1= (\Gamma_1, \iota_1, \pi_1)$ là một $\tau_1$-mở rộng của $G_1$ bởi $F_1$ và $\mathscr{E}_2= (\Gamma_2, \iota_2, \pi_2)$ là một $\tau_2$-mở rộng của $G_2$ bởi $F_2$. Khi đó bộ ba $(\Gamma_1\times \Gamma_2, \iota_1\times \iota_2, \pi_1\times \pi_2)$ là một $\tau_1\times \tau_2$-mở rộng của $G_1\times G_2$ bởi $F_1\times F_2$; nó được gọi là tích ngoài của các mở rộng $\mathscr{E}_1$ và $\mathscr{E}_2$ và được ký hiệu bởi $\mathscr{E}_1\times \mathscr{E}_2$.

### 2. Ảnh ngược của một $\tau$-mở rộng

Cho G và $G'$ là các nhóm. Cho F là một nhóm Abel, và cho $\tau : G\rightarrow$ Aut(F) và $u: G'\rightarrow G$ là các đồng cấu nhóm. Xét đồng cấu nhóm $\tau '=\tau \circ u: G'\rightarrow$ Aut(F), và ký hiệu $\Gamma '$ là tích xơ $\Gamma \times_GG'$ đối với $\pi$ và $u$ (I, §4, No. 8, p. 46). Đó là nhóm con của $\Gamma \times G'$ gồm các cặp $(\gamma , g')$ sao cho $\pi (\gamma ) =u(g')$. Cho $\iota ': F\rightarrow \Gamma '$ là đồng cấu nhóm được cho bởi $\iota '(\alpha ) = (\iota (\alpha ), e)$ với $\alpha \in F$, và ký hiệu phép chiếu thứ hai là $\pi ': \Gamma '\rightarrow G'$. Khi đó cấu xạ $\iota '$ là đơn ánh, cấu xạ $\pi '$ là toàn ánh vì $\pi$ là như vậy, và ảnh của $\iota '$ trùng với hạt nhân của $\pi '$. Hơn nữa, với mọi $\alpha \in F$ và $\gamma '= (\gamma , g)\in \Gamma '$, ta có các hệ thức

$$
\gamma '\iota '(\alpha )\gamma^{'-1}= (\gamma , g)(\iota (\alpha ), e)(\gamma , g)^{-1}= (\iota (\tau (\pi (\gamma )).\alpha ), e) =\iota '(\tau '(\pi '(\gamma ')).\alpha )
$$

Do đó, $(\Gamma ', \iota ', \pi ')$ là một $\tau '$-mở rộng của $G'$ bởi F; ta gọi nó là ảnh ngược của $\mathscr{E}$ bởi $u$ và ký hiệu là $u^*(\mathscr{E})$. Phép chiếu thứ nhất là một đồng cấu nhóm $\varphi : \Gamma '\rightarrow \Gamma$ mà ta gọi là chính tắc.

#### Mệnh đề 1 {#alg-viii-s16-prop-1 .statement tag=00IC}

Biểu đồ sau giao hoán:

F $^{\iota'}$ // ${\Gamma'}^{\pi'}$ // $G'$

(2)

$\varphi u$

F $^{\iota}$ // Γ $^{\pi}$ // G.

Hơn nữa, nếu $\mathscr{E}_1'= (\Gamma '_1, \iota '_1, \pi '_1)$ là một $\tau '$-mở rộng và $\varphi_1: \Gamma '_1\rightarrow \Gamma$ là một đồng cấu nhóm sao cho biểu đồ

F $^{\iota'_1}$ // ${\Gamma'_1}^{\pi'_1}$ // $G'$

$\varphi_1u$

F $^{\iota}$ // Γ $^{\pi}$ // G

giao hoán, thì tồn tại một cấu xạ duy nhất $\psi$ của các $\tau '$-mở rộng từ $\mathscr{E}_1'$ đến $u^*(\mathscr{E})$ sao cho $\varphi_1=\varphi \circ \psi$.

Tính giao hoán của biểu đồ thứ nhất suy ra từ định nghĩa của $\varphi$. Sự tồn tại và tính duy nhất của $\psi$ suy ra từ Bổ đề 2 dưới đây.

#### Bổ đề 2 {#alg-viii-s16-lem-2 .statement tag=00ID}

Cho $F'_1$ là một nhóm Abel, và cho $w: F'_1\rightarrow$ F và $\tau_1: G'\rightarrow$ Aut(F$'_1$) là các đồng cấu nhóm sao cho

$$
w(\tau_1(g)(f)) =\tau (u(g))(w(f))
$$

với mọi $f\in F'_1$ và $g\in G'$. Cho $\mathscr{E}_1'= (\Gamma '_1, \iota '_1, \pi '_1)$ là một mở rộng $\tau_1$ của $G'$ bởi $F'_1$ và $\varphi_1: \Gamma '_1\rightarrow \Gamma$ là một đồng cấu nhóm sao cho biểu đồ sau giao hoán:

${F'_1}^{\iota'_1}$ // ${\Gamma'_1}^{\pi'_1}$ // $G'$

$w\varphi_1u$

F $^{\iota}$ // Γ $^{\pi}$ // G.

Khi đó tồn tại một đồng cấu nhóm duy nhất $\psi : \Gamma '_1\rightarrow \Gamma '$ sao cho biểu đồ

${F'_1}^{\iota'_1}$ // ${\Gamma'_1}^{\pi_1'}$ // $G'$

$w\psi$

F $^{\iota'}$ // ${\Gamma'}^{\pi'}$ // $G'$

giao hoán và $\varphi_1=\varphi \circ \psi$.

Nếu đồng cấu nhóm $\psi : \Gamma '_1\rightarrow \Gamma '$ có các tính chất đã yêu cầu, thì nó thỏa mãn các hệ thức

$$
\psi (\gamma ) = (\varphi \circ \psi (\gamma ), \pi '\circ \psi (\gamma )) = (\varphi_1(\gamma ), \pi '_1(\gamma ))
$$

với mọi $\gamma \in \Gamma '_1$. Ngược lại, đồng cấu nhóm từ $\Gamma '_1$ đến $\Gamma \times G'$ được xác định bởi $\gamma \mapsto (\varphi_1(\gamma ), \pi_1'(\gamma ))$ nhận giá trị trong tích thớ $\Gamma \times_GG'$ vì $\pi \circ \varphi_1(\gamma ) =u\circ \pi_1'(\gamma )$ với mọi $\gamma \in \Gamma '_1$.

#### Hệ quả 1 {#alg-viii-s16-lem-2-cor-1 .statement tag=00IE}

Cho $\mathscr{E}_1$ và $\mathscr{E}_2$ là các mở rộng $\tau$ của G bởi F, và cho $\psi$ là một cấu xạ của các mở rộng $\tau$ từ $\mathscr{E}_1$ đến $\mathscr{E}_2$. Ký hiệu bởi $\varphi_1($resp. $\varphi_2)$ đồng cấu chính tắc của $u^*(\mathscr{E}_1) ($resp. $u^*(\mathscr{E}_2))$. Khi đó tồn tại một cấu xạ duy nhất của các mở rộng $\tau '$ từ $u^*(\mathscr{E}_1)$ đến $u^*(\mathscr{E}_2)$, được ký hiệu bởi $u^*(\psi )$, sao cho $\varphi_2\circ u^*(\psi ) =\psi \circ \varphi_1$.

Chỉ cần áp dụng Mệnh đề 1 cho $\psi \circ \varphi_1$.

Do đó lớp của mở rộng $\tau '$ $u^*(\mathscr{E})$ chỉ phụ thuộc vào lớp của $\mathscr{E}$. Ta cũng ký hiệu bởi $u^*:$ Ex$_{\tau}(G,F)\rightarrow$ Ex$_{\tau'}(G',F)$ ánh xạ gửi lớp của một mở rộng $\tau$ $\mathscr{E}$ tới lớp của mở rộng $\tau '$ $u^*(\mathscr{E})$.

#### Hệ quả 2 {#alg-viii-s16-lem-2-cor-2 .statement tag=00IF}

Khi đó, ký hiệu $\varphi$ (tương ứng $\varphi ',\varphi ''$) là đồng cấu chính tắc liên kết với $\tau '$-mở rộng $u^*(\mathscr{E})$ (tương ứng $\tau ''$-mở rộng $u^{'*}(u^*(\mathscr{E}))$, $\tau ''$-mở rộng $(u\circ u')^*(\mathscr{E}))$. Khi đó tồn tại một cấu xạ duy nhất $\psi$ từ $\tau ''$-mở rộng $u^{'*}(u^*(\mathscr{E}))$ đến $\tau ''$-mở rộng $(u\circ u')^*(\mathscr{E})$ sao cho $\varphi ''\circ \psi =\varphi \circ \varphi '$.

#### Ví dụ {#alg-viii-s16-n2-exa-1 .statement tag=00RI}

Cho H là một nhóm con của G và $j: H\rightarrow G$ là đơn ánh chính tắc. Khi đó với mọi $\tau$-mở rộng $\mathscr{E}= (\Gamma , \iota , \pi )$, $\tau \circ j$-mở rộng $j^*(\mathscr{E})$ đẳng cấu với $(\overset{-1}{\pi}(H), \iota ', \pi ')$, trong đó $\iota ': F\rightarrow \overset{-1}{\pi}(H)$ (tương ứng $\pi ':\overset{-1}{\pi}(H)\rightarrow H$) là đồng cấu nhóm $f\mapsto \iota (f)$ (tương ứng $\gamma \mapsto \pi (\gamma )$). Nói chung hơn, nếu đồng cấu nhóm $u: G'\rightarrow G$ là đơn ánh, thì đồng cấu chính tắc $\varphi$ là đơn ánh với ảnh $\overset{-1}{\pi}(u(G'))$.

### 3. Ảnh trực tiếp của một $\tau$-mở rộng

Cho G là một nhóm, cho F và $F'$ là các nhóm Abel, cho $\tau$ (tương ứng $\tau '$) là một đồng cấu nhóm từ G vào nhóm tự đẳng cấu của F (tương ứng $F'$), và cho $v: F\rightarrow F'$ là một đồng cấu nhóm sao cho

$$
v(\tau (g)\cdot f) =\tau '(g)\cdot v(f) \tag{3}
$$

với mọi $g\in G$ và $f\in F$. Cho $\mathscr{E}= (\Gamma , \iota , \pi )$ là một $\tau$-mở rộng của G bởi F. Cho $\widetilde{\Gamma}$ là tích nửa trực tiếp ngoài $F'\times_{\tau'\circ\pi}\Gamma$. Ký hiệu $\widetilde{\imath}: F'\rightarrow \widetilde{\Gamma}$ là đồng cấu $f\mapsto (f, e)$ và $\widetilde{p}:\widetilde{\Gamma}\rightarrow \Gamma$ là phép chiếu thứ nhất. Ký hiệu $j: F\rightarrow \widetilde{\Gamma}$ là ánh xạ được định nghĩa bởi $f\mapsto (v(f), \iota (f)^{-1})$. Vì ảnh của $\iota$ được chứa trong hạt nhân của $\tau '\circ \pi$, nên ánh xạ $j$ là một đồng cấu nhóm; nó là đơn ánh vì $\iota$ là đơn ánh. Ta có các hệ thức

$$
(f', \gamma )j(f)(f', \gamma )^{-1}= (f', \gamma )(v(f), \iota (f)^{-1})(f', \gamma )^{-1}
$$

$$
= (\tau '(\pi (\gamma ))\cdot v(f), \iota (\tau (\pi (\gamma ))\cdot f)^{-1}) \tag{4}
$$

$$
=j(\tau (\pi (\gamma ))\cdot f)
$$

cho $f\in F,\gamma \in \Gamma$, và $f'\in F'$. Do đó, ảnh của $j$ là một nhóm con chuẩn của $\widetilde{\Gamma}$. Ta ký hiệu $\Gamma '$ là thương của $\widetilde{\Gamma}$ theo ảnh của $j$. Ta ký hiệu $\iota '$ là hợp thành của toàn cấu chính tắc từ $\widetilde{\Gamma}$ đến $\Gamma '$ và $\widetilde{\imath}$. Hạt nhân của đồng cấu $\pi \circ \widetilde{p}$ là tích $F'\times \iota$(F), trong đó chứa ảnh của $j$. Ta định nghĩa $\pi ': \Gamma '\rightarrow G$ là đồng cấu nhóm suy ra từ $\pi \circ \widetilde{p}$ bằng cách chuyển qua thương. Vì $\iota$ là đơn ánh, nên giao của $j(F)$ và $\widetilde{\imath}(F')$ chỉ còn lại phần tử đơn vị của $\widetilde{\Gamma}$; suy ra $\iota '$ là đơn ánh. Ánh xạ từ $F'\times F$ đến $F'\times \iota (F) =$ Ker($\pi \circ \widetilde{p}$) cho bởi

$$
(f', f)\longmapsto (f'v(f), \iota (f)^{-1})
$$

là một đẳng cấu nhóm. Vì thế ảnh của $\iota '$ trùng với hạt nhân của $\pi '$. Vì $\pi$ và $\widetilde{p}$ là toàn ánh, nên $\pi '$ cũng vậy. Điều này chứng tỏ rằng $\mathscr{E}'= (\Gamma ', \iota , \pi ')$ là một $\tau '$-mở rộng của G bởi $F'$; ta gọi nó là ảnh trực tiếp của $\mathscr{E}$ bởi $v$ và ký hiệu là $v_*(\mathscr{E})$. Hợp thành của toàn cấu chính tắc từ $\widetilde{\Gamma}$ đến $\Gamma '$ và đồng cấu nhóm từ Γ đến $\widetilde{\Gamma}$ cho bởi $\gamma \mapsto (1, \gamma )$ là một đồng cấu nhóm $\varphi : \Gamma \rightarrow \Gamma '$ mà ta gọi là chính tắc.

#### Mệnh đề 2 {#alg-viii-s16-prop-2 .statement tag=00IG}

Theo ký hiệu trên, biểu đồ sau giao hoán:

F $^{\iota}$ // Γ $^{\pi}$ // G

$$
v\varphi \tag{5}
$$

${F'}^{\iota'}$ // ${\Gamma'}^{\pi'}$ // G .

Cho $\mathscr{E}_1'= (\Gamma '_1, \iota '_1, \pi_1')$ là một $\tau '$-mở rộng của G bởi $F'$, và cho $\varphi_1: \Gamma \rightarrow \Gamma '_1$ là một đồng cấu nhóm sao cho biểu đồ sau giao hoán:

F $^{\iota}$ // Γ $^{\pi}$ // G

$v\varphi_1$

${F'}^{\iota'_1}$ // ${\Gamma'_1}^{\pi'_1}$ // G.

Khi đó tồn tại một cấu xạ duy nhất của các $\tau '$-mở rộng từ $v_*(\mathscr{E})$ đến $\mathscr{E}_1'$ sao cho $\varphi_1=\psi \circ \varphi$.

Tính giao hoán của biểu đồ thứ nhất suy ra từ phép dựng. Sự tồn tại và tính duy nhất của $\psi$ suy ra từ Bổ đề 3 dưới đây.

#### Bổ đề 3 {#alg-viii-s16-lem-3 .statement tag=00IH}

Cho $G'_1$ là một nhóm, và cho $w: G\rightarrow G'_1$ và $\tau_1: G'_1\rightarrow$ Aut(F$'$) là các đồng cấu nhóm sao cho $\tau '=\tau_1\circ w$. Cho $\mathscr{E}_1'= (\Gamma '_1, \iota '_1, \pi '_1)$ là một $\tau_1$-mở rộng của $G'_1$ bởi $F'$, và cho $\varphi_1: \Gamma \rightarrow \Gamma '_1$ là một đồng cấu nhóm sao cho biểu đồ sau giao hoán:

F $^{\iota}$ // Γ $^{\pi}$ // G

v\varphi_1w

${F'}^{\iota'_1}$ // ${\Gamma'_1}^{\pi'_1}$ // $G'_1$.

Khi đó tồn tại một đồng cấu nhóm duy nhất $\psi : \Gamma '\rightarrow \Gamma '_1$ sao cho biểu đồ

${F'}^{\iota'}$ // ${\Gamma'}^{\pi'}$ // G

$\psi w$

${F'}^{\iota'_1}$ // ${\Gamma'_1}^{\pi'_1}$ // $G'_1$ giao hoán và $\varphi_1=\psi \circ \varphi$.

Với mọi $(f, \gamma )\in F'\times \Gamma$, ký hiệu lớp của $(f, \gamma )$ trong $\Gamma '$ là $(f, \gamma )$. Nếu đồng cấu nhóm $\psi : \Gamma '\rightarrow \Gamma '_1$ có các tính chất mong muốn, thì nó thỏa mãn các hệ thức

$$
\psi (f', \gamma )=\psi (\iota '(f')\varphi (\gamma )) =\iota '_1(f')\varphi_1(\gamma )
$$

với mọi $f'\in F'$ và $\gamma \in \Gamma$. Ngược lại, ánh xạ $\widetilde{\psi}$ từ $F'\times_{\tau'\circ\pi}\Gamma$ đến $\Gamma '_1$ cho bởi $(f, \gamma )\mapsto \iota '_1(f)\varphi_1(\gamma )$ là một đồng cấu nhóm. Thật vậy, ta có các hệ thức

$$
\iota '_1(f)\varphi_1(\gamma )\iota '_1(f')\varphi_1(\gamma ') =\iota '_1(f \tau_1(\pi '_1(\varphi_1(\gamma )))\cdot f')\varphi_1(\gamma \gamma ')
$$

$$
=\iota '_1(f \tau '(\pi (\gamma ))\cdot f')\varphi_1(\gamma \gamma ')
$$

với $f, f'\in F'$ và $\gamma , \gamma '\in \Gamma$. Hạt nhân của $\widetilde{\psi}$ chứa ảnh của $j$ vì $\iota '_1(v(f)) =\varphi_1(\iota (f))$ với $f\in F$, và cấu xạ $\psi$ suy ra từ $\widetilde{\psi}$ bằng cách chuyển qua thương có các tính chất mong muốn.

#### Nhận xét {#alg-viii-s16-n3-rem-1 .statement tag=00II}

Ký hiệu Σ là loài cấu trúc của các $\tau '$-mở rộng, và định nghĩa các $\alpha$-ánh xạ là các ánh xạ từ Γ đến một nhóm $\Gamma '$ làm nền cho một $\tau '$-mở rộng mà là các đồng cấu nhóm và làm cho biểu đồ sau giao hoán:

F $^{\iota}$ // Γ $^{\pi}$ // G

$$
v\varphi \tag{6}
$$

${F'}^{\iota'}$ // ${\Gamma'}^{\pi'}$ // G .

Mệnh đề 2 phát biểu rằng $v_*(\mathscr{E})$ là một nghiệm của bài toán ánh xạ phổ quát tương ứng (Lý thuyết tập hợp, IV, §3, No. 1, p. 284).

#### Hệ quả 1 {#alg-viii-s16-lem-3-cor-1 .statement tag=00IJ}

Cho $\mathscr{E}_1$ và $\mathscr{E}_2$ là các $\tau$-mở rộng của $G$ bởi $F$, và cho $\psi$ là một cấu xạ của các $\tau$-mở rộng từ $\mathscr{E}_1$ đến $\mathscr{E}_2$. Ký hiệu bởi $\varphi_1($tương ứng. $\varphi_2)$ đồng cấu chính tắc cho $v_*(\mathscr{E}_1) ($tương ứng. $v_*(\mathscr{E}_2))$. Khi đó tồn tại một cấu xạ duy nhất của các $\tau '$-mở rộng từ $v_*(\mathscr{E}_1)$ đến $v_*(\mathscr{E}_2)$, ký hiệu là $v_*(\psi )$, sao cho $\varphi_2\circ \psi =v_*(\psi )\circ \varphi_1$.

Chỉ cần áp dụng Mệnh đề 2 cho $\varphi_2\circ \psi$.

Vì thế lớp của $\tau '$-mở rộng $v_*(\mathscr{E})$ chỉ phụ thuộc vào lớp của $\mathscr{E}$. Ta cũng ký hiệu bởi $v_*:$ Ex$_{\tau}(G,F)\rightarrow$ Ex$_{\tau'}(G,F')$ ánh xạ gửi lớp của một $\tau$-mở rộng $\mathscr{E}$ đến lớp của $\tau '$-mở rộng $v_*(\mathscr{E})$.

#### Hệ quả 2 {#alg-viii-s16-lem-3-cor-2 .statement tag=00RJ}

Ta giữ ký hiệu của mệnh đề. Cho $F''$ là một nhóm Abel, và cho $\tau '': G\rightarrow$ Aut(F$''$) và $v': F'\rightarrow F''$ là các đồng cấu nhóm sao cho

$$
\tau ''(g)\cdot v'(f) =v'(\tau '(g)\cdot f)
$$

với $g\in G$ và $f\in F'$. Cho $\mathscr{E}$ là một $\tau$-mở rộng của $G$ bởi $F$, và ký hiệu bởi $\varphi ($tương ứng. $\varphi ',\varphi '')$ đồng cấu chính tắc liên kết với $v_*(\mathscr{E}) ($tương ứng. $v'_*(v_*(\mathscr{E}))$, $(v'\circ v)_*(\mathscr{E}))$. Khi đó tồn tại một cấu xạ duy nhất $\psi$ từ $\tau ''$-mở rộng $v'_*(v_*(\mathscr{E}))$ của $G$ bởi $F''$ đến $\tau ''$-mở rộng $(v'\circ v)_*(\mathscr{E})$ sao cho $\varphi ''=\psi \circ \varphi '\circ \varphi$.

#### Ví dụ 1 {#alg-viii-s16-n3-exa-1 .statement tag=00IK}

Cho $j:\{1\} \rightarrow F$ là đơn ánh chính tắc. Mở rộng nửa tầm thường $\mathscr{I}_{\tau}$ đẳng cấu với $j_*((G, i$, Id$_G))$, trong đó $i:\{e\} \rightarrow G$ là đơn ánh chính tắc. Cho $c: F\rightarrow F$ là đồng cấu hằng $f\mapsto 1$, và cho $\mathscr{E}$ là một $\tau$-mở rộng. $\tau$-mở rộng $c_*(\mathscr{E})$ cũng đẳng cấu với $\mathscr{I}_{\tau}$.

#### Ví dụ 2 {#alg-viii-s16-n3-exa-2 .statement tag=00IL}

Cho E là một nhóm con của F ổn định dưới tác động của G. Kí hiệu $F'$ là thương của F theo E, $v: F\rightarrow F'$ là đồng cấu chính tắc, và $\tau ': G\rightarrow$ Aut(F$'$) là tác động của G lên $F'$ được xác định bởi

$$
\tau '(g)\cdot v(f) =v(\tau (g)\cdot f)
$$

với $g\in G$ và $f\in F$. Cho $\mathscr{E}= (\Gamma , \iota , \pi )$ là một $\tau$-mở rộng của G bởi F. Khi đó $\iota (E)$ là một nhóm con chuẩn tắc của Γ, và $\tau '$-mở rộng $v_*(\mathscr{E})$ của G bởi $F'$ là đẳng cấu với mở rộng $(\Gamma /\iota (E), \iota , \pi )$, trong đó $\overline{\iota}$ và $\overline{\pi}$ là các đồng cấu nhóm suy ra từ $\iota$ và $\pi$ bằng cách chuyển qua các thương. Theo đẳng cấu này, đồng cấu chính tắc $\varphi$ liên kết với $v_*(\mathscr{E})$ tương ứng với đồng cấu chính tắc từ Γ đến $\Gamma /\iota (E)$.

#### Mệnh đề 3 {#alg-viii-s16-prop-3 .statement tag=00IM}

Cho G và $G'$ là các nhóm, và cho F và $F'$ là các nhóm Abel. Cho $\tau : G\rightarrow$ Aut(F)$,\tau ': G\rightarrow$ Aut(F$'$)$,u: G'\rightarrow G$, và $v: F\rightarrow F'$ là các đồng cấu nhóm sao cho

$$
\tau '(g)\cdot v(f) =v(\tau (g)\cdot f)
$$

với $g\in G$ và $f\in F$. Ta viết $\tau ''=\tau '\circ u$. Cho $\mathscr{E}$ là một $\tau$-mở rộng của G bởi F. Kí hiệu $\varphi_u($resp. $\varphi_v,\varphi '_u,\varphi '_v)$ là đồng cấu chính tắc tương ứng với $\tau \circ u$-mở rộng $u^*(\mathscr{E}) ($resp. với $\tau '$-mở rộng $v_*(\mathscr{E})$, với các $\tau ''$-mở rộng $u^*(v_*(\mathscr{E}))$ và $v_*(u^*(\mathscr{E})))$. Khi đó tồn tại một cấu xạ duy nhất $\psi$ của các $\tau ''$-mở rộng từ $v_*(u^*(\mathscr{E}))$ đến $u^*(v_*(\mathscr{E}))$ sao cho $\varphi_v\circ \varphi_u=$ $\varphi '_u\circ \psi \circ \varphi '_v$.

Kí hiệu $\tau \circ u$-mở rộng $u^*(\mathscr{E})$ (resp. $\tau ''$-mở rộng $u^*(v_*(\mathscr{E}))$) bởi $(\Gamma_u, \iota_u, \pi_u)$ (resp. $(\Gamma '_u, \iota '_u, \pi '_u)$). Áp dụng Bổ đề 2 của VIII, p. 287 cho $\varphi_v\circ \varphi_u$, ta thấy rằng tồn tại một đồng cấu nhóm $\psi_1: \Gamma_u\rightarrow \Gamma '_u$ sao cho biểu đồ

F $^{\iota_u}$ // $\Gamma_u^{\pi_u}$ // $G'$

$v\psi_1$

${F'}^{\iota'_u}$ // ${\Gamma'_u}^{\pi'_u}$ // $G'$

giao hoán và $\varphi '_u\circ \psi_1=\varphi_v\circ \varphi_u$. Sự tồn tại của $\psi$ suy ra từ Mệnh đề 2 áp dụng cho $\psi_1$. Ngược lại, nếu $\psi '$ cũng có các tính chất mong muốn, thì ta có $\psi '\circ \varphi '_v=\psi_1$ theo Bổ đề 2, nên $\psi '=\psi$ (Mệnh đề 2).

### 4. Luật nhóm trên các lớp của các $\tau$-mở rộng

Cho G là một nhóm, F là một nhóm Abel, và $\tau : G\rightarrow$ Aut(F) là một đồng cấu nhóm. Kí hiệu $\delta : G\rightarrow G\times G$ là ánh xạ đường chéo $g\mapsto$ $(g, g)$ và $m: F\times F\rightarrow F$ là đồng cấu phép nhân $(f_1, f_2)\mapsto$ $f_1f_2$. Kí hiệu $s: F\rightarrow F$ là đồng cấu nhóm được cho bởi $f\mapsto f^{-1}$. Cho $\mathscr{E}_1= (\Gamma_1, \iota_1, \pi_1)$ và $\mathscr{E}_2= (\Gamma_2, \iota_2, \pi_2)$ là các mở rộng $\tau$ của G bởi F. Vì ta có quan hệ

$$
m(((\tau \times \tau )\circ \delta )(g)\cdot (f_1, f_2)) =\tau (g)\cdot m(f_1, f_2)
$$

với mọi $g\in G$ và mọi $f_1, f_2\in F$, mở rộng $m_*(\delta^*(\mathscr{E}_1\times \mathscr{E}_2))$ là một mở rộng $\tau$; ta gọi nó là tích của các mở rộng $\tau$ $\mathscr{E}_1$ và $\mathscr{E}_2$ và kí hiệu là $\mathscr{E}_1\mathscr{E}_2$. Lớp của mở rộng này chỉ phụ thuộc vào các lớp của các mở rộng $\mathscr{E}_1$ và $\mathscr{E}_2$ (VIII, p. 288, Hệ quả 1 và VIII, p. 291, Hệ quả 1). Vì vậy điều này cho một luật hợp thành trên Ex$_{\tau}(G,F)$.

#### Nhận xét {#alg-viii-s16-n4-rem-1 .statement tag=00IN}

Cho $\mathscr{E}_1= (\Gamma_1, \iota_1, \pi_1)$ và $\mathscr{E}_2= (\Gamma_2, \iota_2, \pi_2)$ là các mở rộng $\tau$ của G bởi F. Cho $\mathscr{E}_1\mathscr{E}_2= (\Gamma , \iota , \pi )$ là tích của các mở rộng này. Theo ví dụ của VIII, p. 289, phép dựng cho một đồng cấu nhóm toàn ánh từ tích sợi $\Gamma_1\times_G\Gamma_2$ đến Γ có hạt nhân là ảnh của đồng cấu nhóm $f\mapsto (\iota_1(f), \iota_2(f)^{-1})$ từ F đến $\Gamma_1\times_G\Gamma_2$.

#### Mệnh đề 4 {#alg-viii-s16-prop-4 .statement tag=00IO}

Phép nhân các mở rộng $\tau$ trang bị cho tập hợp Ex$_{\tau}(G,F)$ cấu trúc của một nhóm Abel. Phần tử đơn vị của nó là lớp của mở rộng nửa tầm thường $\mathscr{I}_{\tau}$. Phần tử nghịch đảo của lớp của một mở rộng $\tau$ $\mathscr{E}$ là lớp của $s_*(\mathscr{E})$.

Tính kết hợp của luật này suy ra từ tính giao hoán của các biểu đồ

$$
\begin{array}{ccc}
G & \xrightarrow{\delta} & G \times G \\
\downarrow \delta & & \downarrow \operatorname{Id} \times \delta \\
G \times G & \xrightarrow{\delta \times \operatorname{Id}} & G \times G \times G
\end{array}
$$
và
$$
\begin{array}{ccc}
F \times F \times F & \xrightarrow{m \times \operatorname{Id}} & F \times F \\
\downarrow \operatorname{Id} \times m & & \downarrow m \\
F \times F & \xrightarrow{m} & F
\end{array}
$$

và từ Hệ quả 2 của VIII, p. 288; Hệ quả 2 của VIII, p. 291; và Mệnh đề 3 của VIII, p. 292.

Cho $\Delta : F \to F \times F$ là ánh xạ đường chéo $f \mapsto (f, f)$. Cho $\mathcal{E} = (\Gamma, \iota, \pi)$ là một $\tau$-mở rộng. Cho $\tilde{\Delta} : \Gamma \to \Gamma \times_G \Gamma$ là đồng cấu nhóm được cho bởi $\gamma \mapsto (\gamma, \gamma)$. Biểu đồ sau giao hoán:

$$
\begin{array}{ccc}
F & \xrightarrow{\iota} & \Gamma & \xrightarrow{\pi} & G \\
\downarrow \Delta & & \downarrow \tilde{\Delta} & & \parallel \\
F \times F & \longrightarrow & \Gamma \times_G \Gamma & \longrightarrow & G.
\end{array}
$$

Theo Mệnh đề 2 của VIII, p. 290, suy ra mở rộng theo $(\tau \times \tau) \circ \delta$ $\delta^*(\mathcal{E} \times \mathcal{E})$ đẳng cấu với $\Delta_*(\mathcal{E})$.

Kí hiệu $c : F \to F$ là đồng cấu hằng $f \mapsto 1$. Theo Ví dụ 1 của VIII, p. 292, việc $\mathscr{I}_\tau$ là một phần tử đơn vị cho luật hợp thành này suy ra từ đẳng cấu từ $\delta^*(\mathcal{E} \times \mathcal{E})$ đến $\Delta_*(\mathcal{E})$ và biểu đồ giao hoán

$$
\begin{array}{ccc}
F & \xrightarrow{(\operatorname{Id}_F \times c) \circ \Delta} & F \times F \\
(c \times \operatorname{Id}_F) \circ \Delta & & \downarrow \operatorname{Id}_F \\
& & \downarrow m \\
F \times F & \xrightarrow{m} & F.
\end{array}
$$

Khẳng định cuối cùng suy ra từ biểu đồ giao hoán

$$
\begin{array}{ccc}
F & \xrightarrow{(\operatorname{Id}_F \times s) \circ \Delta} & F \times F \\
(s \times \operatorname{Id}_F) \circ \Delta & & \downarrow c \\
& & \downarrow m \\
F \times F & \xrightarrow{m} & F.
\end{array}
$$

Cho $\mathcal{E}_1 = (\Gamma_1, \iota_1, \pi_1)$ và $\mathcal{E}_2 = (\Gamma_2, \iota_2, \pi_2)$ là các $\tau$-mở rộng. Đẳng cấu nhóm $\Gamma_1 \times \Gamma_2 \to \Gamma_2 \times \Gamma_1$ cho bởi $(\gamma_1, \gamma_2) \mapsto (\gamma_2, \gamma_1)$ hạn chế thành một đẳng cấu nhóm $\sigma : \Gamma_1 \times_G \Gamma_2 \to \Gamma_2 \times_G \Gamma_1$. Do các quan hệ

$$
\sigma(\iota_1(f), \iota_2(f)^{-1}) = (\iota_2(f^{-1}), \iota_1(f^{-1})^{-1})
$$

với $f\in F$, đồng cấu nhóm $\sigma$ cảm sinh, khi chuyển qua các thương, một cấu xạ của các $\tau$-mở rộng từ $\mathscr{E}_1\mathscr{E}_2$ đến $\mathscr{E}_2\mathscr{E}_1$. Vậy luật hợp thành là giao hoán.

#### Mệnh đề 5 {#alg-viii-s16-prop-5 .statement tag=00IP}

a) Cho G và $G'$ là các nhóm, và cho F là một nhóm Abel. Cho $\tau : G\rightarrow$ Aut(F) và $u: G'\rightarrow G$ là các đồng cấu nhóm. Ánh xạ $u^*:$ Ex$_{\tau}(G,F)\rightarrow$ Ex$_{\tau\circ u}(G',F)$ là một đồng cấu nhóm.

b) Cho G là một nhóm, và cho F và $F'$ là các nhóm Abel. Cho $\tau : G\rightarrow$ Aut(F)$,\tau ': G\rightarrow$ Aut(F$'$), và $v: F\rightarrow F'$ là các đồng cấu nhóm sao cho

$$
\tau '(g)\cdot v(f) =v(\tau (g)\cdot f)
$$

với $g\in G$ và $f\in F$. Ánh xạ $v_*:$ Ex$_{\tau}(G,F)\rightarrow$ Ex$_{\tau'}(G,F')$ là một đồng cấu nhóm.

Điều này suy ra từ tính giao hoán của các biểu đồ

${G'}^{\delta}$ // $G'\times G'F\times F^m$ // F

$_uu_{\times u}$ và $v_{\times v}v$

G $^{\delta}$ // $G\times GF'\times {F'}^m$ // $F'$.

### 5. Mô tả đối đồng điều

Cho G là một nhóm, cho F là một nhóm Abel, và cho $\tau : G\rightarrow$ Aut(F) là một đồng cấu nhóm. Với mọi $g\in G$ và $f\in F$, ta cũng viết $^gf$ để chỉ $\tau (g)\cdot f$. Một 2-cocycle của G với giá trị trong F là một ánh xạ $c: G\times G\rightarrow F$ sao cho với mọi $(g_1, g_2, g_3)\in G\times G\times G$, ta có

$$
g_{_1}c(g_2, g_3)c(g_1, g_2g_3) =c(g_1, g_2)c(g_1g_2, g_3) \tag{7}
$$

Vì F giao hoán, tập hợp các 2-cocycle là một nhóm con của nhóm các ánh xạ từ $G\times G$ đến F; ta kí hiệu nó là $Z^2(G,F)$. Ta kí hiệu nhóm các ánh xạ từ G đến F là $C^1(G,F)$. Với mọi $h\in C^1(G,F)$ và $(g_1, g_2)\in G\times G$, đặt

$$
(\partial h)(g_1, g_2) =^{g_1}h(g_2)h(g_1g_2)^{-1}h(g_1) \tag{8}
$$

Một phép tính đơn giản cho thấy rằng ánh xạ $\partial h: G\times G\rightarrow F$ là một 2-cocycle. Ánh xạ $\partial : C^1(G,F)\rightarrow Z^2(G,F)$ là một đồng cấu nhóm. Với mọi $h\in C^1(G,F)$, 2-cocycle $\partial h$ được gọi là một 2-coboundary. Nhóm $Z^2(G,F)/\partial (C^1(G,F))$ được ký hiệu bởi $H^2(G,F)$ và được gọi là nhóm đối đồng điều thứ hai của G với hệ số trong F.

$*$The notation above agrees with that of X, §6, n$^o8$, p. 112 concerning group cohomology.$*$

Cho $\mathscr{E}= (\Gamma , \iota , \pi )$ là một $\tau$-mở rộng. Cho $\sigma$ là một tiết diện của ánh xạ toàn ánh $\pi ($Lý thuyết tập hợp, II, §3, No. 8, p. 86), nghĩa là một ánh xạ từ G đến Γ sao cho $\pi (\sigma (g)) =g$ với mọi $g$ trong G. Với mọi $g_1, g_2\in G$, $\sigma (g_1)\sigma (g_2)\sigma (g_1g_2)^{-1}$ thuộc Ker($\pi$ ), do đó tồn tại một ánh xạ duy nhất $c_{\sigma}: G\times G\rightarrow F$ sao cho

$$
\iota (c_{\sigma}(g_1, g_2)) =\sigma (g_1)\sigma (g_2)\sigma (g_1g_2)^{-1} \tag{9}
$$

với mọi $g_1, g_2\in G$. Ánh xạ $c_{\sigma}$ là hằng với giá trị 1 nếu và chỉ nếu $\sigma$ là một đồng cấu nhóm.

#### Mệnh đề 6 {#alg-viii-s16-prop-6 .statement tag=00IQ}

Ánh xạ $c_{\sigma}$ là một phần tử của nhóm $Z^2(G,F)$, và lớp của nó trong nhóm đối đồng điều $H^2(G,F)$ chỉ phụ thuộc vào lớp của $\tau$-mở rộng $\mathscr{E}$.

Ta nói rằng ánh xạ $c_{\sigma}$ là 2-cocycle liên kết với $\sigma$ và rằng lớp đối đồng điều của nó trong $H^2(G,F)$ là lớp đối đồng điều của $\tau$-mở rộng $\mathscr{E}$.

Trước hết ta kiểm tra rằng $c_{\sigma}$ thỏa mãn điều kiện cocycle. Cho $g_1,g_2$, và $g_3$ là các phần tử của G. Dùng công thức (1) của VIII, p. 285 và (9), ta thu được các đẳng thức

$$
\iota (^{g_1}c_{\sigma}(g_2, g_3)c_{\sigma}(g_1, g_2g_3))
$$

$$
=\sigma (g_1)\sigma (g_2)\sigma (g_3)\sigma (g_2g_3)^{-1}\sigma (g_1)^{-1}\sigma (g_1)\sigma (g_2g_3)\sigma (g_1g_2g_3)^{-1}
$$

$$
=\sigma (g_1)\sigma (g_2)\sigma (g_3)\sigma (g_1g_2g_3)^{-1}
$$

và

$$
\iota (c_{\sigma}(g_1, g_2)c_{\sigma}(g_1g_2, g_3))
$$

$$
=\sigma (g_1)\sigma (g_2)\sigma (g_1g_2)^{-1}\sigma (g_1g_2)\sigma (g_3)\sigma (g_1g_2g_3)^{-1}
$$

$$
=\sigma (g_1)\sigma (g_2)\sigma (g_3)\sigma (g_1g_2g_3)^{-1}
$$

Do đó ánh xạ $c_{\sigma}$ là một phần tử của $Z^2(G,F)$.

Bây giờ ta chứng minh rằng ảnh của $c_{\sigma}$ trong $H^2(G,F)$ không phụ thuộc vào tiết diện $\sigma$ đã chọn. Cho $\sigma$ và $\sigma '$ là những tiết diện như vậy. Với mọi phần tử $g$ của G, tồn tại một phần tử duy nhất $a_g$ của F sao cho $\sigma '(g) =\iota (a_g)\sigma (g)$. Cho $g_1$ và $g_2$ là các phần tử của G. Dùng định nghĩa (9), ta thu được các đẳng thức

$$
\iota (c_{\sigma'}(g_1, g_2)) =\sigma '(g_1)\sigma '(g_2)\sigma '(g_1g_2)^{-1}
$$

$$
=\iota (a_{g_1})\sigma (g_1)\iota (a_{g_2})\sigma (g_2)\sigma (g_1g_2)^{-1}\iota (a_{g_1g_2})^{-1} \tag{10}
$$

$$
=\iota (a_{g_1})\iota (^{g_1}a_{g_2})\iota (c_{\sigma}(g_1, g_2))\iota (a_{g_1g_2})^{-1}
$$

Vì nhóm F là giao hoán, ta có các đẳng thức

$$
c_{\sigma'}(g_1, g_2)c_{\sigma}(g_1, g_2)^{-1}= (^{g_1}a_{g_2})a^{-1}_{g_1g_2}a_{g_1}= (\partial a)(g_1, g_2) \tag{11}
$$

như suy ra từ (8). Điều đó chứng tỏ rằng các lớp của $c_{\sigma'}$ và $c_{\sigma}$ trong $H^2(G,F)$ trùng nhau.

Sau cùng, cho $\mathscr{E}= (\Gamma , \iota , \pi )$ và $\mathscr{E}'= (\Gamma ', \iota ', \pi ')$ là các $\tau$-mở rộng đẳng cấu, cho $u:\mathscr{E}\rightarrow \mathscr{E}'$ là một cấu xạ của các $\tau$-mở rộng, và cho $\sigma$ là một tiết diện của ánh xạ $\pi$. Ánh xạ $u\circ \sigma$ là một tiết diện của ánh xạ $\pi '$, và ta có $c_{\sigma}=c_{u\circ\sigma}$. Do đó lớp của $c_{\sigma}$ trong $H^2(G,F)$ chỉ phụ thuộc vào lớp của $\mathscr{E}$ trong Ex$_{\tau}(G,F)$.

Ta ký hiệu bởi $\Theta_{\tau}$ : Ex$_{\tau}(G,F)\rightarrow H^2(G,F)$, hay đơn giản hơn là Θ, ánh xạ gửi lớp của một $\tau$-mở rộng $(\Gamma , \iota , \pi )$ tới lớp của 2-cocycle $c_{\sigma}$, trong đó $\sigma$ là một tiết diện của đồng cấu toàn ánh $\pi$.

#### Định lý 1 {#alg-viii-s16-thm-1 .statement tag=00IR}

Ánh xạ Θ là một đẳng cấu nhóm từ Ex$_{\tau}(G,F)$ đến $H^2(G,F)$.

Trước hết ta chứng minh rằng Θ là một đồng cấu nhóm. Cho $\mathscr{E}= (\Gamma , \iota , \pi )$ và $\mathscr{E}'= (\Gamma ', \iota ', \pi ')$ là các $\tau$-mở rộng, và cho $\sigma$ (resp. $\sigma '$) là một tiết diện của ánh xạ $\pi$ (resp. $\pi '$). Ta ký hiệu $\mathscr{E} \mathscr{E}'= (\Gamma '', \iota '', \pi '')$ là tích của các $\tau$-mở rộng $\mathscr{E}$ và $\mathscr{E}'$. Ta ký hiệu bởi $[\gamma , \gamma ']$ ảnh trong $\Gamma ''$ của một phần tử $(\gamma , \gamma ')$ của $\Gamma \times_G\Gamma '$ qua đồng cấu toàn ánh trong nhận xét của VIII, p. 293. Ánh xạ từ G vào $\Gamma ''$ gửi một phần tử $g$ tới $[\sigma (g), \sigma '(g)]$ là một tiết diện $\sigma ''$ của ánh xạ $\pi ''$. Cho $g_1$ và $g_2$ là các phần tử của G. Ta có các hệ thức

$$
\iota ''(c_{\sigma''}(g_1, g_2)) =\sigma ''(g_1)\sigma ''(g_2)\sigma ''(g_1g_2)^{-1}
$$

$$
= [\iota (c_{\sigma}(g_1, g_2)), \iota '(c_{\sigma'}(g_1, g_2)]
$$

$$
=\iota ''(c_{\sigma}(g_1, g_2)c_{\sigma'}(g_1, g_2))
$$

Vì thế ta có $c_{\sigma''}(g_1, g_2) =c_{\sigma}(g_1, g_2)c_{\sigma'}(g_1, g_2)$.

Ta chứng minh rằng ánh xạ Θ là đơn ánh. Cho $\mathscr{E}= (\Gamma , \iota , \pi )$ là một $\tau$-mở rộng, và cho $\sigma$ là một tiết diện của ánh xạ $\pi$ sao cho ảnh của $c_{\sigma}$ trong $H^2(G,F)$ là tầm thường. Tồn tại một ánh xạ $a: G\rightarrow F$ sao cho

$$
c_{\sigma}(g_1, g_2) = (^{g_1}a(g_2))a(g_1g_2)^{-1}a(g_1)
$$

với mọi $g_1, g_2\in G$. Khi đó ta định nghĩa $\sigma ': G\rightarrow \Gamma$ bởi

$$
\sigma '(g) =\iota (a(g)^{-1})\sigma (g)
$$

với $g\in G$. Dùng (11), ta thu được rằng $c_{\sigma'}$ là hằng với giá trị 1; do đó, $\sigma '$ là một đồng cấu nhóm, điều đó chứng tỏ rằng $\tau$-mở rộng $\mathscr{E}$ là nửa tầm thường (I, §6, No. 1, p. 67, Mệnh đề 4).

Ta hãy chứng minh rằng ánh xạ Θ là toàn ánh. Cho $c$ là một phần tử của $Z^2(G,F)$. Ta trang bị cho tập hợp $\Gamma  = F\times G$ luật hợp thành sau: (12) $(f_1, g_1)(f_2, g_2) =(f_1(^{g_1}f_2)c(g_1, g_2), g_1g_2)$

với mọi $f_1, f_2\in F$ và $g_1, g_2\in G$. Ta có các hệ thức

$$
(f_1, g_1) ((f_2, g_2)(f_3, g_3)) = (f_1, g_1)(f_2(^{g_2}f_3)c(g_2, g_3), g_2g_3)
$$

$$
=(f_1(^{g_1}f_2)(^{g_1g_2}f_3)(^{g_1}c(g_2, g_3))c(g_1, g_2g_3), g_1g_2g_3)
$$

và

$$
((f_1, g_1)(f_2, g_2)) (f_3, g_3) =(f_1(^{g_1}f_2)c(g_1, g_2), g_1g_2)(f_3, g_3)
$$

$$
=(f_1(^{g_1}f_2)(^{g_1g_2}f_3)c(g_1, g_2)c(g_1g_2, g_3), g_1g_2g_3)
$$

với mọi $f_1, f_2, f_3\in F$ và $g_1,g_2, g_3\in G$. Suy ra luật này kết hợp vì $c$ là một 2-côxích. Với mọi $(f, g)\in \Gamma$, ta có

$$
(f, g)(c(e, e)^{-1}, e) = (f(^gc(e, e)^{-1})c(g, e), g)
$$

Bây giờ, từ định nghĩa của một 2-côxích suy ra rằng $c(g, e) =^gc(e, e)$, từ đó ta suy ra rằng $(f, g)(c(e, e)^{-1}, e) = (f, g)$. Ta cũng chứng minh tương tự rằng

$$
(c(e, e)^{-1}, e)(f, g) = (f c(e, e)^{-1}c(e, g), g) = (f, g)
$$

Luật hợp thành được xác định bởi (12) vì thế có phần tử đơn vị $(c(e, e)^{-1}, e)$, và mọi phần tử $(f, g)$ của Γ đều khả nghịch, với nghịch đảo

$$
(^{g^{-1}}(f^{-1}c(e, e)^{-1}c(g, g^{-1})^{-1}), g^{-1})
$$

Vì thế ta đã trang bị cho Γ một cấu trúc nhóm. Ký hiệu $\iota : F\rightarrow G$ là ánh xạ gửi $f$ đến $(c(e, e)^{-1}f, e)$, $\pi : \Gamma \rightarrow G$ là phép chiếu thứ hai, và $\sigma$ là ánh xạ $g\mapsto (1, g)$. Các ánh xạ $\iota$ và $\pi$ là các đồng cấu nhóm, nên bộ ba $\mathscr{E}= (\Gamma , \iota , \pi )$ là một $\tau$-mở rộng, $\sigma$ là một tiết diện của ánh xạ $\pi$, và côxích liên kết $c_{\sigma}$ bằng $c$ vì

$$
\sigma (g_1)\sigma (g_2)\sigma (g_1g_2)^{-1}= (1, g_1)(1, g_2)(1, g_1g_2)^{-1}= (c(g_1, g_2), g_1g_2)(1, g_1g_2)^{-1}
$$

$$
= (c(g_1, g_2)c(e, g_1g_2)^{-1}, e) = (c(e, e)^{-1}c(g_1, g_2), e)
$$

với $g_1, g_2\in G$.

#### Nhận xét {#alg-viii-s16-n5-rem-1 .statement tag=00RK}

Cho G là một nhóm, cho F và $F'$ là các nhóm Abel, cho $\tau$ (resp. $\tau '$) là một đồng cấu nhóm từ G đến nhóm tự đẳng cấu của F (resp. $F'$), và cho $v: F\rightarrow F'$ là một đồng cấu nhóm sao cho

$$
v(\tau (g)\cdot f) =\tau '(g)\cdot v(f) \tag{13}
$$

với $g\in G$ và $f\in F$. Cho $\alpha$ là một phần tử của Ex$_{\tau}(G,F)$. Nếu côxích $c$ biểu diễn $\Theta (\alpha )$, thì $v\circ c$ biểu diễn $\Theta (v_*(\alpha ))\in H^2(G,F')$.

### 6. Hạn chế và đồng hạn chế

Cho G và $G'$ là các nhóm, F là một nhóm Abel, và $\tau$ là một đồng cấu từ G vào nhóm tự đẳng cấu của F. Cho $u: G'\rightarrow G$ là một đồng cấu nhóm. Ta viết $\tau '=\tau \circ u$.

Nếu $\psi : G\times G\rightarrow F$ là một 2-cocycle của G với các giá trị trong F, thì ánh xạ $\psi \circ (u\times u)$ từ $G'\times G'$ đến F được cho bởi $(g_1, g_2)\mapsto \psi (u(g_1), u(g_2))$ là một 2-cocycle của $G'$ với các giá trị trong F, và ánh xạ $\psi \mapsto \psi \circ (u\times u)$ từ $Z^2(G,F)$ đến $Z^2(G',F)$ cảm sinh một đồng cấu nhóm $u^*: H^2(G,F)\rightarrow H^2(G',F)$. Với mọi $\lambda \in H^2(G,F)$, phần tử $u^*(\lambda )$ được gọi là ảnh ngược của $\lambda$ bởi $u$. Khi $G'$ là một nhóm con của G và $u: G'\rightarrow G$ là đơn ánh chính tắc, đồng cấu $u^*$ được gọi là đồng cấu hạn chế từ G đến $G'$; ta ký hiệu nó là Res$^G_{G'}$. Khi G là một thương của $G'$ và $u: G'\rightarrow G$ là toàn cấu chính tắc, đồng cấu $u^*$ được gọi là đồng cấu lạm phát từ G đến $G'$.

#### Mệnh đề 7 {#alg-viii-s16-prop-7 .statement tag=00IS}

Theo ký hiệu ở trên, biểu đồ sau giao hoán:

Ex$_{\tau}(G,F)^{u^*}$ // Ex$_{\tau}(G',F)$

$\Theta_{\tau}\Theta_{\tau'}$

$H_2(G,F)^{u^*}$ // $H_2(G',F)$.

Cho H là một nhóm con của G có chỉ số hữu hạn. Cho $s$ là một tiết diện của toàn cấu chính tắc từ G tới $H\backslash G$. Ta ký hiệu bởi $(g, x)\mapsto x\cdot g$ tác động phải của G trên $H\backslash G$ cảm sinh từ tác động phải của G lên chính nó bằng phép nhân. Chú ý rằng với mọi $x\in H\backslash G$ và $g\in G$, phần tử $s(x)gs(x\cdot g)^{-1}$ thuộc H. Với mọi ánh xạ $c: H\times H\rightarrow F$, vì thế ta có thể định nghĩa một ánh xạ $\widetilde{c}_s: G\times G\rightarrow F$ bởi quan hệ

$$
\widetilde{c}_s(g_1, g_2) =\prod_{x\in H\backslash G}^{s(x)^{-1}}c(s(x)g_1s(x\cdot g_1)^{-1}, s(x\cdot g_1)g_2s(x\cdot g_1g_2)^{-1})
$$

với $g_1,g_2\in G$. Ánh xạ $c\mapsto \widetilde{c}_s$ là một đồng cấu nhóm từ $F^{H\times H}$ đến $F^{G\times G}$.

#### Bổ đề 4 {#alg-viii-s16-lem-4 .statement tag=00IT}

Nếu $c: H\times H\rightarrow F$ là một 2-cocycle của H với các giá trị trong F, thì $\widetilde{c}_s$ là một 2-cocycle của G với các giá trị trong F.

Cho $g_1,g_2$, và $g_3$ là các phần tử của G. Với mọi $i\in  \{1,2,3\}$, ta định nghĩa một ánh xạ $h_i: H\backslash G\rightarrow H$ bởi quan hệ

$$
h_i(x) =s(x\cdot g_1\cdots g_{i-1})g_is(x\cdot g_1\cdots g_i)^{-1}
$$

với $x\in H\backslash G$. Chú ý rằng

$$
h_1(x)h_2(x) =s(x)g_1g_2s(x\cdot g_1g_2)^{-1}
$$

$$
h_2(x)h_3(x) =s(x\cdot g_1)g_2g_3s(x\cdot g_1g_2g_3)^{-1}
$$

với $x\in H\backslash G$. Khi đó ta có các quan hệ

$$
^{g_1}\widetilde{c}_s(g_2, g_3)\widetilde{c}_s(g_1g_2, g_3)^{-1}\widetilde{c}_s(g_1, g_2g_3)\widetilde{c}_s(g_1, g_2)^{-1}
$$

$$
=\prod_{x\in H\backslash G}^{g_1s(x)^{-1}}c(s(x)g_2s(x\cdot g_2)^{-1}, s(x\cdot g_2)g_3s(x\cdot g_2g_3)^{-1})
$$

$$
\times \prod_{x\in H\backslash G}^{s(x)^{-1}}(c(h_1(x)h_2(x), h_3(x))^{-1}
$$

$$
\times c(h_1(x), h_2(x)h_3(x))c(h_1(x), h_2(x))^{-1})
$$

trong đó đẳng thức thứ hai suy ra từ sự kiện rằng $c$ là một 2-đối chu trình.

#### Bổ đề 5 {#alg-viii-s16-lem-5 .statement tag=00IU}

Nếu $c$ là một 2-đối biên, thì $\widetilde{c}_s$ cũng là một 2-đối biên.

Cho $t: H\rightarrow F$ là một ánh xạ sao cho $c=\partial t$. Cho $\widetilde{t}_s: G\rightarrow F$ là ánh xạ được định nghĩa bởi

$$
\widetilde{t}_s(g) =\prod_{x\in H\backslash G}^{s(x)^{-1}}t(s(x)gs(x\cdot g)^{-1})
$$

với $g\in G$. Chỉ cần chứng minh rằng $\widetilde{c}_s=\partial \widetilde{t}_s$, điều này suy ra từ các quan hệ $\widetilde{c}_s(g_1, g_2) =\prod_{x\in H\backslash G}^{s(x)^{-1}s(x)g_1s(x\cdot g_1)^{-1}}t(s(x\cdot g_1)g_2s(x\cdot g_1g_2)^{-1})$

$$
\times \prod_{x\in H\backslash G}^{s(x)^{-1}}(t(s(x)g_1g_2s(x\cdot g_1g_2)^{-1})^{-1}t(s(x)g_1s(x\cdot g_1)^{-1}))
$$

$$
=\partial \widetilde{t}_s(g_1, g_2)
$$

với $g_1, g_2\in G$.

#### Bổ đề 6 {#alg-viii-s16-lem-6 .statement tag=00IV}

Cho $c$ là một 2-đối chu trình của H với giá trị trong F. Ảnh của $\widetilde{c}_s$ trong nhóm $H^2(G,F)$ không phụ thuộc vào lựa chọn của tiết diện $s$.

Cho $s'$ là một tiết diện của toàn cấu chính tắc từ G lên $H\backslash G$. Cho $h: H\backslash G\rightarrow H$ là ánh xạ được đặc trưng bởi quan hệ

$$
s'(x) =h(x)s(x)
$$

với $x\in H\backslash G$. Khi đó 2-đối chu trình $\widetilde{c}_{s'}$ được cho bởi các quan hệ

$$
\widetilde{c}_{s'}(g_1, g_2)
$$

$$
=\prod_{x\in H\backslash G}^{s(x)^{-1}h(x)^{-1}}c(h(x)s(x)g_1s'(x\cdot g_1)^{-1}, s'(x\cdot g_1)g_2s'(x\cdot g_1g_2)^{-1})
$$

$$
=\prod_{x\in H\backslash G}^{s(x)^{-1}}c(s(x)g_1s(x\cdot g_1)^{-1}h(x\cdot g_1)^{-1}, h(x\cdot g_1)s(x\cdot g_1)g_2s'(x\cdot g_1g_2)^{-1})
$$

$s(x)^{-1}(-1''-1-1$

$$
\times \prod_{x\in H\backslash G}c(h(x), s(x)g_1g_2s(x\cdot g_1g_2))
$$

$$
\times c(h(x)^{-1}, s'(x)g_1s'(x\cdot g_1)^{-1}))
$$

$=\prod_{x\in H\backslash G}^{g_1s(x\cdot g_1)^{-1}}c(h(x\cdot g_1)^{-1}, h(x\cdot g_1)s(x\cdot g_1)g_2s'(x\cdot g_1g_2)^{-1})$

$$
\times \prod_{x\in H\backslash G}^{s(x)^{-1}}c(s(x)g_1s(x\cdot g_1)^{-1}, s(x\cdot g_1)g_2s'(x\cdot g_1g_2)^{-1})
$$

$s(x)^{-1}-1-1-1$

$\times \prod_{x\in H\backslash G}c(s(x)g_1s(x\cdot g_1), h(x\cdot g_1))$

$$
\times \prod_{x\in H\backslash G}^{s(x)^{-1}}(c(h(x)^{-1}, s'(x)g_1g_2s'(x\cdot g_1g_2)^{-1})^{-1}
$$

$$
\times c(h(x)^{-1}, s'(x)g_1s'(x\cdot g_1)^{-1}))
$$

$=\prod_{x\in H\backslash G}^{s(x)^{-1}}c(s(x)g_1s(x\cdot g_1)^{-1}, s(x\cdot g_1)g_2s'(x\cdot g_1g_2)^{-1})$

$s(x)^{-1}-1-1-1$

$\times \prod_{x\in H\backslash G}c(s(x)g_1s(x\cdot g_1), h(x\cdot g_1))$ $\times \prod_{x\in H\backslash G}^{g_1s(x)^{-1}}c(h(x)^{-1}, h(x)s(x)g_2s'(x\cdot g_2)^{-1})$

$s(x)^{-1}(-1''-1-1$

$$
\times \prod_{x\in H\backslash G}c(h(x), s(x)g_1g_2s(x\cdot g_1g_2))
$$

$$
\times c(h(x)^{-1}, s'(x)g_1s'(x\cdot g_1)^{-1}))
$$

với mọi $g_1, g_2\in G$. Đẳng thức thứ nhất suy ra từ quan hệ đối chu trình (VIII, p. 295, công thức (7)) áp dụng cho các phần tử

$h(x)^{-1},h(x)s(x)g_1s'(x\cdot g_1)^{-1}$, và $s'(x\cdot g_1)g_2s'(x\cdot g_1g_2)^{-1}$;

đẳng thức thứ hai thu được bằng cách áp dụng quan hệ đối chu trình cho các phần tử

$s(x)g_1s(x\cdot g_1)^{-1},h(x\cdot g_1)^{-1}$, và $h(x\cdot g_1)s(x\cdot g_1)g_2s'(x\cdot g_1g_2)^{-1}$; và đẳng thức cuối chỉ dùng sự kiện rằng ánh xạ $x\mapsto x\cdot g_1$ là một phép hoán vị của $H\backslash G$.

Hai dòng cuối của biểu thức thu được tương ứng với một 2-đối biên. Ta thấy rằng $\widetilde{c}_{s'}$ có cùng lớp trong $H^2(G,F)$ với đối chu trình có giá trị tại $(g_1, g_2)\in G^2$ được cho bởi biểu thức

$$
\prod_{x\in H\backslash G}^{s(x)^{-1}}c(s(x)g_1s(x\cdot g_1)^{-1}, s(x\cdot g_1)g_2s(x\cdot g_1g_2)^{-1}h(x\cdot g_1g_2)^{-1})
$$

$s(x)^{-1}-1-1-1$

$$
\times \prod_{x\in H\backslash G}c(s(x)g_1s(x\cdot g_1), h(x\cdot g_1))
$$

$=\prod_{x\in H\backslash G}^{g_1s(x\cdot g_1)^{-1}}c(s(x\cdot g_1)g_2s(x\cdot g_1g_2)^{-1}, h(x\cdot g_1g_2)^{-1})^{-1}$

$$
\times \prod_{x\in H\backslash G}^{s(x)^{-1}}c(s(x)g_1s(x\cdot g_1)^{-1}, s(x\cdot g_1)g_2s(x\cdot g_1g_2)^{-1})
$$

$$
\times \prod_{x\in H\backslash G}^{s(x)^{-1}}(c(s(x)g_1g_2s(x\cdot g_1g_2)^{-1}, h(x\cdot g_1g_2)^{-1})
$$

$-1-1-1)$

$\times c(s(x)g_1s(x\cdot g_1), h(x\cdot g_1))$ $=\prod_{x\in H\backslash G}^{s(x)^{-1}}c(s(x)g_1s(x\cdot g_1)^{-1}, s(x\cdot g_1)g_2s(x\cdot g_1g_2)^{-1})$

$gs(x)^{-1}-1-1-1$

$$
\times \prod_{x\in H\backslash G^1}c(s(x)g_2s(x\cdot g_2), h(x\cdot g_2))
$$

$$
\times \prod_{x\in H\backslash G}^{s(x)^{-1}}(c(s(x)g_1g_2s(x\cdot g_1g_2)^{-1}, h(x\cdot g_1g_2)^{-1})
$$

$$
\times c(s(x)g_1s(x\cdot g_1)^{-1}, h(x\cdot g_1)^{-1})^{-1})
$$

trong đó đẳng thức thứ nhất suy ra từ quan hệ đối chu trình áp dụng cho các phần tử

$s(x)g_1s(x\cdot g_1)^{-1},s(x\cdot g_1)g_2s(x\cdot g_1g_2)^{-1}$, và $h(x\cdot g_1g_2)^{-1}$.

Hai dòng cuối của biểu thức thu được tương ứng với một đối biên bậc 2. Ta thấy rằng lớp của $\widetilde{c}_{s'}$ trùng với lớp của $\widetilde{c}_s$.

Ta đã xây dựng một đồng cấu từ nhóm $H^2(H,F)$ sang nhóm $H^2(G,F)$, mà ta gọi là đồng cấu đối hạn chế từ H đến G và ký hiệu bởi Cor$^G_H$.

#### Mệnh đề 8 {#alg-viii-s16-prop-8 .statement tag=00IW}

Cho H là một nhóm con của G có chỉ số hữu hạn. Tự đồng cấu Cor$^G_H\circ$ Res$^G_H$ của nhóm $H^2(G,F)$ trùng với phép nhân với chỉ số (G : H).

Cho $\alpha$ là một phần tử của $H^2(G,F)$, và cho $c$ là một phần tử của $Z^2(G,F)$ biểu diễn $\alpha$. Phần tử Cor$^G_H\circ$ Res$^G_H(\alpha )$ là lớp của đối chu trình có giá trị tại $(g_1, g_2)\in G^2$ được cho bởi biểu thức

$$
\prod_{x\in H\backslash G}^{s(x)^{-1}}c(s(x)g_1s(x\cdot g_1)^{-1}, s(x\cdot g_1)g_2s(x\cdot g_1g_2)^{-1})
$$

$$
=\prod_{x\in H\backslash G}c(g_1s(x\cdot g_1)^{-1}, s(x\cdot g_1)g_2s(x\cdot g_1g_2)^{-1})
$$

$$
\times \prod_{x\in H\backslash G}(c(s(x)^{-1}, s(x)g_1g_2s(x\cdot g_1g_2)^{-1})^{-1}c(s(x)^{-1}, s(x)g_1s(x\cdot g_1)^{-1}))
$$

$$
=\prod_{x\in H\backslash G}^{g_1}c(s(x\cdot g_1)^{-1}, s(x\cdot g_1)g_2s(x\cdot g_1g_2)^{-1})
$$

$$
\times \prod_{x\in H\backslash G}c(g_1, g_2s(x\cdot g_1g_2)^{-1})c(g_1, s(x\cdot g_1)^{-1})^{-1}
$$

$$
\times \prod_{x\in H\backslash G}(c(s(x)^{-1}, s(x)g_1g_2s(x\cdot g_1g_2)^{-1})^{-1}c(s(x)^{-1}, s(x)g_1s(x\cdot g_1)^{-1}))
$$

Đẳng thức thứ nhất đến từ quan hệ đối chu trình (VIII, p. 295, công thức (7)) áp dụng cho các phần tử

$s(x)^{-1},s(x)g_1s(x\cdot g_1)^{-1}$, và $s(x\cdot g_1)g_2s(x\cdot g_1g_2)^{-1}$;

đẳng thức thứ hai thu được bằng cách áp dụng quan hệ đối chu trình cho các phần tử

$g_1,s(x\cdot g_1)^{-1}$, và $s(x\cdot g_1)g_2s(x\cdot g_1g_2)^{-1}$.

Sau khi khử một đối biên, ta thu được rằng Cor$^G_H\circ$ Res$^G_H(\alpha )$ là lớp của đối chu trình có giá trị tại $(g_1, g_2)\in G^2$ được cho bởi biểu thức

$$
\prod_{x\in H\backslash G}c(g_1, g_2s(x\cdot g_1g_2)^{-1})c(g_1, s(x\cdot g_1)^{-1})^{-1}
$$

$$
=\prod_{x\in H\backslash G}^{g_1}c(g_2, s(x\cdot g_1g_2)^{-1})^{-1}c(g_1g_2, s(x\cdot g_1g_2)^{-1})c(g_1, g_2)
$$

$$
\times \prod_{x\in H\backslash G}c(g_1, s(x\cdot g_1)^{-1})^{-1}
$$

$$
=\prod_{x\in H\backslash G}^{g_1}c(g_2, s(x\cdot g_2)^{-1})^{-1}c(g_1g_2, s(x\cdot g_1g_2)^{-1})c(g_1, s(x\cdot g_1)^{-1})^{-1}
$$

$$
\times c(g_1, g_2)^{(G:H)}
$$

điều này chứng minh kết quả.

### 7. Đại số Galois

Cho K là một trường giao hoán. Nếu E là một đại số trên K, thì ta ký hiệu nhóm tự đẳng cấu của nó là Aut$_K(E)$. Nếu E là một mở rộng Galois của trường K, thì nhóm Aut$_K(E)$ chính là nhóm Galois Gal(E$/K$) (V, §10, No. 2, p. 58).

Cho G là một nhóm. Một $(K,G)$-đại số là một đại số trên K E được trang bị một đồng cấu nhóm $\lambda : G\rightarrow$ Aut$_K(E)$. Khi đó đồng cấu $\lambda$ trang bị cho E cấu trúc của một nhóm có toán tử trong G cũng như cấu trúc của một K[G]-môđun trái với phép toán ngoài cho bởi

$$
((\sum_{g\in G}\mu_gg)x=\sum_{g\in G}\mu_g\lambda (g).x \tag{14}
$$

với mọi $x\in L$ và mọi phần tử $(\mu_g)_{g\in G}$ của K[G]. Một cấu xạ của $(K,G)$-đại số là một cấu xạ của các đại số đồng thời cũng là một cấu xạ của các nhóm có toán tử.

#### Bổ đề 7 {#alg-viii-s16-lem-7 .statement tag=00IX}

a) Cho S là một tập con của G sao cho mọi phần tử của G đều viết duy nhất được dưới dạng $hs$ với $h\in H$ và $s\in S$. Khi đó ánh xạ gửi $f$ tới $(f(s))_{s\in S}$ là một đẳng cấu từ đại số trên K Coind$^G_H(E)$ đến đại số trên K $\mathscr{F}(S,E)$ của các ánh xạ từ S đến E.

b) Đại số Coind$^G_H(E)$ có bậc hữu hạn trên K khi và chỉ khi E có bậc hữu hạn trên K và chỉ số của H trong G là hữu hạn. Trong trường hợp này, ta có công thức

[Coind$^G_H(E) : K] = (G : H)[E : K]$.

c) Cho $E^H$ là đại số bất biến của nhóm H trong E và Coind$^G_H(E)^G$ là đại số bất biến của nhóm G trong Coind$^G_H(E)$. Ánh xạ $f\mapsto f(e)$ từ Coind$^G_H(E)$ đến E hạn chế thành một đẳng cấu đại số từ Coind$^G_H(E)^G$ đến $E^H$.

Mệnh đề a) suy ra từ các định nghĩa và kéo theo b). Theo (15), một ánh xạ từ G đến E là một phần tử của Coind$^G_H(E)$ bất biến dưới G khi và chỉ khi nó là hằng với giá trị là một phần tử của E bất biến dưới H.

#### Nhận xét 1 {#alg-viii-s16-n7-rem-1 .statement tag=00IY}

Cho G là một nhóm, H là một nhóm con của G, và N là một nhóm con của H. Cho E là một $(K$, N)-đại số. Cho $\alpha$ là một phần tử của $\mathscr{F}_H(G,\mathscr{F}_N(H,E))$. Ta có hệ thức

$$
\alpha (g)(nh) =n(\alpha (g)(h)) \tag{16}
$$

với mọi $g\in G,h\in H$, và $n\in N$ và các hệ thức

$$
\alpha (hg)(h') = (h\alpha (g))(h') =\alpha (g)(h'h) \tag{17}
$$

với mọi $h, h'\in H$ và với mọi $g\in G$. Do đó, $\alpha (ng)(e) =\alpha (g)(n) =$ $n(\alpha (g)(e))$ đối với mọi $g\in G$ và $n\in N$. Vì thế ta có thể xét ánh xạ

$$
\psi :\mathscr{F}_H(G,\mathscr{F}_N(H,E))\rightarrow \mathscr{F}_N(G,E)
$$

được xác định bởi quan hệ $\psi (\alpha )(g) =\alpha (g)(e)$ với $\alpha$ trong $\mathscr{F}_H(G,\mathscr{F}_N(H,E))$ và $g$ trong G. Ánh xạ $\psi$ là một đẳng cấu đại số từ Coind$^G_H$(Coind$^H_N(E)$) đến Coind$^G_N(E)$, nghịch đảo của nó gửi một phần tử $\beta$ của $\mathscr{F}_N(G,E)$ đến ánh xạ $\alpha$ được xác định bởi quan hệ $\alpha (g)(h) =\beta (hg)$ với $g\in G$ và $h\in H$.

Giả sử bây giờ cho một nhóm hữu hạn G và một đại số giao hoán trên K rút gọn (V, §6, No. 6, p. 32) có bậc hữu hạn, được trang bị một tác động của G cho bởi một đồng cấu $\lambda$ từ G đến Aut$_K(L)$. Với $x\in L$ và $g\in G$, ta ký hiệu $g\cdot x$ là biến đổi của $x$ dưới tự đẳng cấu $\lambda (g)$ của L. Gọi $\mathscr{S}$ là tập hợp các iđêan cực đại của L; ta ký hiệu $g\cdot \mathfrak{m}$ là biến đổi của một phần tử $\mathfrak{m}$ của $\mathscr{S}$ dưới tự đẳng cấu $\lambda (g)$ của L. Đó là một phần tử của $\mathscr{S}$. Với mọi $\mathfrak{m}$ trong $\mathscr{S}$, trường $L/\mathfrak{m}$ là một mở rộng hữu hạn của K. Ta viết $\pi_{\mathfrak{m}}: L\rightarrow L/\mathfrak{m}$ cho phép chiếu và ký hiệu $G_{\mathfrak{m}}$ là nhóm ổn định của $\mathfrak{m}$ trong G, tức là tập hợp các $g\in G$ sao cho $g\cdot \mathfrak{m}=\mathfrak{m}$. Đại số trên K $L/\mathfrak{m}$ được trang bị một tác động của $G_{\mathfrak{m}}$ thông qua đồng cấu $\lambda_{\mathfrak{m}}$ từ $G_{\mathfrak{m}}$ đến Aut$_K(L/\mathfrak{m})$ gửi một phần tử $h$ của $G_{\mathfrak{m}}$ đến tự đẳng cấu của $L/\mathfrak{m}$ suy ra từ $\lambda (h)$ khi chuyển qua các thương.

Cho $\mathscr{O}$ là tập hợp các quỹ đạo của G trong $\mathscr{S}$. Với một quỹ đạo $\sigma \in \mathscr{O}$, đặt $\mathfrak{a}_{\sigma}=\bigcap_{\mathfrak{m}\in\sigma}\mathfrak{m}$ và $L_{\sigma}= L/\mathfrak{a}_{\sigma}$. Vì $\mathfrak{a}_{\sigma}$ bất biến dưới G, nên khi chuyển qua các thương, tác động của G trên L xác định một đồng cấu $\lambda_{\sigma}$ từ G vào Aut$_K(L_{\sigma})$. Cuối cùng, ký hiệu $\pi_{\sigma}$ là ánh xạ chính tắc từ L đến $L_{\sigma}$.

#### Bổ đề 8 {#alg-viii-s16-lem-8 .statement tag=00RL}

a) Với mọi $g\in G,\sigma \in \mathscr{O}$, và $\mathfrak{m}\in \sigma$, ta có

$[L_{\sigma}: K] =$ Card($\sigma$ )$[L/\mathfrak{m}: K]$.

b) Ánh xạ $\pi :x\mapsto (\pi_{\sigma}(x))_{\sigma\in\mathscr{O}}$ là một đẳng cấu của các $(K,G)$-đại số từ L đến $\prod_{\sigma\in\mathscr{O}}L_{\sigma}$.

c) Ký hiệu $L^G($resp. $L^G_{\sigma})$ là đại số con của L (resp. $L_{\sigma}$) gồm các phần tử bất biến dưới tác động của G. Khi đó $\pi$ cảm sinh một đẳng cấu từ $L^G$ đến $\prod_{\sigma\in\mathscr{O}}L^G_{\sigma}$.

Vì đại số L là rút gọn và có bậc hữu hạn, giao của các ideal cực đại của L thu được 0 (VIII, p. 173, Hệ quả 2). Hơn nữa, nếu $\mathfrak{m}$ và $\mathfrak{m}'$ là hai ideal cực đại phân biệt của L, thì ta có $\mathfrak{m}+\mathfrak{m}'= L$. Theo Mệnh đề 10 của I, §8, No. 11, p. 110, ánh xạ chính tắc từ L đến $\prod_{\mathfrak{m}\in\mathscr{S}}L/\mathfrak{m}$ là một đẳng cấu, cũng như ánh xạ chính tắc từ $L/\mathfrak{a}_{\sigma}$ đến $\prod_{\mathfrak{m}\in\sigma}L/\mathfrak{m}$ với mọi $\sigma \in \mathscr{O}$. Mệnh đề a) suy ra. Vì $\mathscr{O}$ là một phân hoạch của $\mathscr{S}$, mệnh đề b) suy ra; mệnh đề c) là một hệ quả ngay lập tức của b).

Bây giờ hãy cố định một quỹ đạo $\sigma \in \mathscr{O}$ và một phần tử $\mathfrak{m}$ của $\sigma$. Đặt $F_{\mathfrak{m}}$ = Coind$^G_{G_{\mathfrak{m}}}(L/\mathfrak{m})$, và ký hiệu $\lambda_{F_{\mathfrak{m}}}$ là tác động của G trên $F_{\mathfrak{m}}$. Với mọi $x\in L$, ký hiệu $\overline{x}$ là ánh xạ từ G đến $L/\mathfrak{m}$, gửi $g$ tới $\pi_{\mathfrak{m}}(gx)$. Theo công thức (15) của VIII, p. 305 và định nghĩa của tác động của $G_{\mathfrak{m}}$ trên $L/\mathfrak{m}$, hiển nhiên là $\overline{x}$ thuộc $F_{\mathfrak{m}}$, và ánh xạ $u:x\mapsto \overline{x}$ từ L đến $F_{\mathfrak{m}}$ thỏa $\lambda_{F_{\mathfrak{m}}}(g)\circ u=u\circ \lambda (g)$ với $g\in G$. Nói cách khác, $u$ là một cấu xạ của các $(K$, G)-đại số.

#### Bổ đề 9 {#alg-viii-s16-lem-9 .statement tag=00IZ}

#### Bổ đề 10 {#alg-viii-s16-lem-10 .statement tag=00J0}

Cho $L$ là một $(K,G)$-đại số étale trên $K$. Ánh xạ $\psi$ từ $L_{(\Omega )}$ đến $\mathscr{F}(\mathscr{H},\Omega )$ được đặc trưng bởi quan hệ

$$
\psi (\xi \otimes x) = (\xi \chi (x))_{\chi\in\mathscr{H}}
$$

là một đẳng cấu của $(K,G)$-đại số.

Vì $L$ là étale, ánh xạ $\psi$ là một đẳng cấu của các đại số $\Omega$ (V, §6, No. 3, p. 30, Mệnh đề 2 và V, §6, No. 3, p. 29, Mệnh đề 1, c)). Ta có các quan hệ

$\psi$((Id $\otimes \lambda (g)$)$(\xi \otimes x)$) $= (\xi (\chi \circ \lambda (g))(x))_{\chi\in\mathscr{H}}$

với $\xi \in \Omega ,x\in L$, và $g\in G$. Do đó $\psi$ là một cấu xạ của $(\Omega$, G)-đại số.

#### Định lý 2 {#alg-viii-s16-thm-2 .statement tag=00J1}

Cho G là một nhóm hữu hạn, và cho L là một đại số giao hoán trên K có bậc hữu hạn, được trang bị một tác động của G do một đồng cấu đơn ánh $\lambda$ từ G đến Aut$_K(L)$. Các tính chất sau đây là tương đương:

(i) Tồn tại một nhóm con H của G, một mở rộng Galois E của K có bậc hữu hạn, một đẳng cấu từ H đến Gal(E$/K$), và một đẳng cấu của $(K,G)$-đại số từ L đến Coind$^G_H(E)$.

(ii) Đại số L là étale, và $\mathscr{H}$ là một G-tập chính thuần nhất (I, §5, No. 6, p. 60, Định nghĩa 7).

(iii)$\Rightarrow$(iv): Tồn tại một đẳng cấu của $(\Omega ,G)$-đại số $\psi : L_{(\Omega )}\rightarrow \mathscr{F}(G,\Omega )$; nói cách khác, với mọi $g\in G$, tự đẳng cấu $\psi \circ \lambda (g)_{(\Omega )}\circ \psi^{-1}$ của $\Omega^G$ bằng tự đẳng cấu

$$
(x_h)_{h\in G}\longmapsto (x_{hg})_{h\in G}
$$

(iv) Đại số L là reduced, và L là một $K[G]$-môđun tự do có hạng 1.

(v) Đại số L là reduced, ta có Card(G) = [L : K], và K là vành con của L gồm các phần tử bất biến dưới tác động của G.

(vi) Đại số L là reduced, nhóm G tác động bắc cầu lên tập hợp các iđêan cực đại của L, và, với mọi iđêan cực đại $\mathfrak{m}$ của L, nhóm ổn định $G_{\mathfrak{m}}$ của $\mathfrak{m}$ trong G tác động trung thành lên $L/\mathfrak{m}$ và nhận K làm trường con của các phần tử bất biến.

(i)$\Rightarrow$(ii): Cho E là một mở rộng Galois của K có bậc hữu hạn và $\tau$ là một đẳng cấu từ H đến Aut$_K(E)$. Gọi S là một hệ đại diện của các lớp ghép phải của G modulo H. Đại số trên K F = Coind$^G_H$(E) đẳng cấu với $\mathscr{F}(S,E)$ (Bổ đề 7, a)); do đó nó là étale. Kí hiệu $\lambda_F$ là tác động của G lên F. Hơn nữa, gọi $\psi$ là một đồng cấu đại số trên K từ E đến Ω, và gọi $\chi_0$ là đồng cấu $f\mapsto \psi (f(e))$ từ F đến Ω. Lấy $g\in G$ sao cho $\chi_0\circ \lambda_F(g) =\chi_0$; vì $\psi$ là đơn ánh, khi đó ta có $f(g) =f(e)$ với mọi $f\in F$. Theo Bổ đề 7, a), ta có $g\in H$, và theo công thức

$$
f(h) =\tau (h)\cdot f(e) \tag{18}
$$

đúng với mọi $h\in H$, điều này chỉ có thể xảy ra nếu $g=e$. Mặt khác, theo Bổ đề 7, b) và Định lý 3 của V, §10, No. 6, p. 66, ta có

[F : K] = (G : H)[E : K] = (G : H) Card(H) = Card(G).

Tập hợp $\mathscr{K}$ của các K-đồng cấu từ F đến Ω có lực lượng [F : K] vì F là étale (V, §6, No. 5, p. 32, Mệnh đề 4), do đó Card($\mathscr{K}$) $=$ Card(G). Vì nhóm ổn định của $\chi_0$ trong G bằng $\{e\}$ theo trên, nên $\mathscr{K}$ là một tập hợp G-chính thuần nhất.

(ii)$\Rightarrow$(iii): Giả sử rằng L là étale và $\mathscr{H}$ là một tập hợp G-chính thuần nhất. Theo Bổ đề 10, các $(\Omega$, G)-đại số $L_{(\Omega )}$ và $\mathscr{F}(\mathscr{H},\Omega )$ đẳng cấu. Vì $\mathscr{H}$ là một tập hợp G-chính thuần nhất, nên các $(\Omega$, G)-đại số $\mathscr{F}(\mathscr{H},\Omega )$ và $\mathscr{F}(G,\Omega )$ đẳng cấu.

(iii)$\Rightarrow$(iv): Giả sử rằng tính chất (iii) đúng. Khi đó $L_{(\Omega )}$ là một môđun tự do có hạng 1 trên đại số Ω[G]; đại số sau có thể được đồng nhất một cách chính tắc với $K[G]_{(\Omega )}$. Ta rồi áp dụng Định lý 3 của VIII, p. 37.

Hàm ý (iv)$\Rightarrow$(v) là ngay lập tức.

Chứng minh hàm ý (v)$\Rightarrow$(vi). Đại số L là reduced. Theo Bổ đề 8, c), nhóm G tác động bắc cầu lên tập hợp $\mathscr{S}$ các iđêan cực đại của L. Gọi $\mathfrak{m}$ là một phần tử của $\mathscr{S}$. Theo Bổ đề 9, vì $\bigcap_{\mathfrak{n}\in\mathscr{S}}\mathfrak{n}=\{0\}$, đại số L đẳng cấu với đại số Coind$^G_{G_{\mathfrak{m}}}(L/\mathfrak{m})$. Do đó đại số các phần tử bất biến của $G_{\mathfrak{m}}$ trong $L/\mathfrak{m}$ trùng với K theo Bổ đề 7, c). Suy ra đồng cấu $\lambda_{\mathfrak{m}}$ từ $G_{\mathfrak{m}}$ đến Gal((L$/\mathfrak{m}$)$/K$) là toàn ánh. Theo Bổ đề 7, ta còn có

Lực lượng của G $= [L : K] = (G : G_{\mathfrak{m}})[L/\mathfrak{m}: K]$. Do đó lực lượng của G$_{\mathfrak{m}}$ $= [L/\mathfrak{m}: K]$, và đồng cấu $\lambda_{\mathfrak{m}}$ là đơn ánh.

Còn lại chỉ cần chứng minh mệnh đề suy ra (vi)$\Rightarrow$(i). Cho $\mathfrak{m}$ là một iđêan cực đại của L. Theo Bổ đề 9, đại số L đẳng cấu với đại số Coind$^G_{G_{\mathfrak{m}}}(L/\mathfrak{m})$ như một $(K$, G)-đại số. Vì $G_{\mathfrak{m}}$ tác động trung thành trên $L/\mathfrak{m}$ và nhận K làm trường con bất biến, đồng cấu nhóm $\lambda_{\mathfrak{m}}$ xác định một đẳng cấu từ $G_{\mathfrak{m}}$ lên Gal((L$/\mathfrak{m}$)$/K$).

#### Nhận xét 2 {#alg-viii-s16-n7-rem-2 .statement tag=00J2}

Trong Định lý 2, ta có thể thay giả thiết rằng Ω là đóng đại số bằng giả thiết rằng Ω là đóng tách được. Thật vậy, nếu L là étale, thì ảnh của mọi đồng cấu K-đại số từ L đến Ω là một mở rộng tách được của K.

#### Nhận xét 3 {#alg-viii-s16-n7-rem-3 .statement tag=00J3}

Định lý cơ sở chuẩn (V, §10, No. 9, p. 73, Định lý 6) là một trường hợp riêng của mệnh đề suy ra (i)$\Rightarrow$(iv) trong Định lý 2.

#### Định nghĩa 1 {#alg-viii-s16-def-1 .statement tag=00J4}

Cho G là một nhóm hữu hạn, và cho L là một đại số giao hoán khác không bậc hữu hạn trên K được trang bị cấu trúc của một $(K,G)$-đại số, trong đó tác động của G được cho bởi một đồng cấu đơn ánh từ G vào nhóm Aut$_K$(L). Ta nói rằng L là một đại số Galois với nhóm G nếu nó có các tính chất tương đương (i) đến (vi) của Định lý 2.

#### Nhận xét 4 {#alg-viii-s16-n7-rem-4 .statement tag=00J5}

Giả sử L là một mở rộng của K được trang bị một tác động $\lambda$ của G. Khi đó L là một đại số Galois trên K khi và chỉ khi L là một mở rộng Galois của K và $\lambda$ là một đẳng cấu từ G lên nhóm Galois của L trên K.

#### Nhận xét 5 {#alg-viii-s16-n7-rem-5 .statement tag=00J6}

Giả sử nhóm G là Abel. Nếu G tác động trung thành và bắc cầu trên một tập hợp X, thì nhóm ổn định của mọi điểm của X chỉ còn phần tử đơn vị (vì các nhóm ổn định của các điểm của X đều bằng nhau và giao của chúng chỉ còn phần tử đơn vị của G). Do đó, các tính chất (i) đến (vi) của Định lý 2 cũng tương đương với điều sau:

(vii) Đại số L là étale, và G tác động trung thành và bắc cầu trên $\mathscr{H}$.

#### Nhận xét 6 {#alg-viii-s16-n7-rem-6 .statement tag=00J7}

Theo V, §10, No. 1, p. 75, Bổ đề 5; V, §10, No. 1, p. 76, Mệnh đề 12; và VIII, p. 137, Mệnh đề 3, một đại số Galois là giao hoán và nửa đơn.

#### Ví dụ 1 {#alg-viii-s16-n7-exa-1 .statement tag=00J8}

Cho $n$ là một số nguyên dương, nguyên tố cùng nhau với số mũ đặc số của K. Giả sử nhóm $\mu_n$ của các căn bậc $n$ của đơn vị trong K có cấp $n$. Khi đó với mọi ước $d$ của $n$, nhóm $\mu_d$ của các căn bậc $d$ của đơn vị có cấp $d$. Cho $a$ là một phần tử khác không của K, cho L là đại số $K[X]/(X^n-a)$, và cho $x$ là lớp của X trong L. Dãy $(1, x, . . . , x^{n-1})$ là một cơ sở của không gian vectơ L trên trường K, và ta có $x^n=a$. Hơn nữa, đa thức $X^n-a$ nguyên tố cùng nhau với đạo hàm của nó $nX^{n-1}$, nên đại số L là étale (V, §7, No. 2, p. 37, Mệnh đề 3). Với mọi $\zeta$ trong $\mu_n$, tự đẳng cấu $P(X)\mapsto P(\zeta X)$ của vành K[X] xác định, bằng cách chuyển qua các thương, một tự đồng cấu $\lambda (\zeta )$ của L vì ta có $(\zeta X)^n-a= X^n-a$; nó là một tự đẳng cấu. Ta có

$$
\lambda (\zeta )x^i=\zeta^ix^i \tag{19}
$$

với $0\leqslant i < n$. Ánh xạ $\lambda :\zeta \mapsto \lambda (\zeta )$ là một đồng cấu đơn ánh từ $\mu_n$ vào Aut$_K$(L), và vành bất biến của nhóm $\lambda (\mu_n)$ trong L bằng $K\cdot 1$. Vì lực lượng của $\mu_n$ bằng $n= [L : K]$, đại số L được trang bị tác động $\lambda$ là một đại số Galois (VIII, p. 308, Định lý 2, (v)).

Cho $r$ là số nguyên dương nhỏ nhất sao cho $a^r$ thuộc $K^{*n}$; nó chia $n$, và tồn tại một phần tử $b$ của $K^*$ sao cho $a=b^{n/r}$. Khi đó (V, §11, No. 8, p. 91, Nhận xét) đa thức $X^r-b$ là bất khả quy, và ta có $X^n-a=\prod_{\zeta\in\mu_{n/r}}(X^r-\zeta b)$. Cho E là trường $K[Y]/(Y^r-b)$, và cho $y$ là lớp của Y trong E. Tồn tại một đẳng cấu $\theta$ từ $\mu_{n/r}$ đến Gal(E$/K$), được đặc trưng bởi quan hệ $\theta (\xi )(y) =\xi y$ (V, §11, No. 8, p. 91, Ví dụ 3). Ta sẽ kiểm tra rằng đại số Galois L đẳng cấu với $(K, \mu_n$)-đại số Coind$^{\mu_n}_{\mu_{n/r}}(E)$.

#### Ví dụ 2 {#alg-viii-s16-n7-exa-2 .statement tag=00J9}

Bây giờ giả sử rằng trường K có đặc số $p\not= 0$. Cho $c$ là một phần tử của K. Đa thức $f= X^p-X-c$ nguyên tố cùng với đạo hàm của nó $f'=-1$, nên đại số $L = K[X]/(f)$ là étale (V, §7, No. 2, p. 37, Mệnh đề 3). Ký hiệu ảnh của X trong L là $x$; ta có quan hệ $x^p=x+c$. Dãy $(1, x, . . . , x^{p-1})$ là một cơ sở của L được xem như một không gian vectơ trên K.

Cho P là nhóm cộng của trường con nguyên tố của K; đó là một nhóm cyclic cấp $p$, được sinh bởi phần tử đơn vị 1 của K. Với mọi $j$ trong P, ta có $j^p=j$ (V, §1, No. 3, p. 4, công thức (4)) và do đó $f(X +j) =f(X)$. Vì thế tồn tại một tự đẳng cấu $\gamma (j)$ của đại số L được đặc trưng bởi quan hệ $\gamma (j)(x) =x+j$; hơn nữa, ánh xạ thu được $\gamma$ là một đơn cấu từ P vào Aut$_K(L)$.

Cho $\Omega$ là một mở rộng đóng đại số của K, và cho $\xi$ là một nghiệm của đa thức $f$ trong $\Omega$. Ta có $\xi^p=\xi +c$, do đó

$$
X^p-X-c= (X^p-\xi^p)-(X-\xi ) = (X-\xi )^p-(X-\xi ) =\prod_{j\in P}(X-\xi -j)
$$

theo V, §12, No. 1, p. 94, công thức (1). Với mọi $j$ trong P, tồn tại duy nhất một đồng cấu đại số $\chi_j: L\rightarrow \Omega$ gửi $x$ tới $\xi +j$; hơn nữa, mọi đồng cấu từ L đến $\Omega$ đều là một trong các $\chi_j$, và ta có quan hệ $\chi_j=\chi_0\circ \gamma (j)$. Đại số L được trang bị $\gamma$ có tính chất (ii) của Định lý 2 của VIII, p. 308 và do đó là một đại số Galois trên K.

Để mô tả cấu trúc của L, ta phải phân biệt hai trường hợp:

a) Ta có $\xi \notin K$. Khi đó đa thức $f(X)$ bất khả quy trong K[X] (V, §11, No. 9, p. 93, Ví dụ 3). Trong trường hợp này, L là một mở rộng cyclic của K có bậc $p$, và $\gamma$ là một đẳng cấu từ P tới Gal(L$/K$).

b) Ta có $\xi \in K$. Khi đó ánh xạ $\psi :y\mapsto (\chi_j(y))_{j\in P}$ là một đẳng cấu từ đại số L đến đại số tích $K^P$; hơn nữa, $\psi \circ \gamma (k)\circ \psi^{-1}$ là tự đẳng cấu $(x_j)_{j\in P}\mapsto (x_{j+k})_{j\in P}$ của $K^P$ với mọi $k\in P$.

### 8. Tác động lên các đại số Galois

#### Mệnh đề 9 {#alg-viii-s16-prop-9 .statement tag=00JA}

Cho G là một nhóm hữu hạn, H là một nhóm con của G, và E là một đại số Galois trên trường K với nhóm H. Khi đó $(K,G)$-đại số Coind$^G_H(E)$ thu được từ E bằng đồng quy nạp từ H đến G là một đại số Galois trên trường K với nhóm G.

Vì E là một đại số Galois trên K, theo tính chất (v) của Định lý 2 của VIII, p. 308, nó là reduced, ta có Card(H) = [E : K], và K là vành các bất biến của H trong E. Nhưng theo Bổ đề 7 của VIII, p. 305, đại số F = Coind$^G_H(E)$ là reduced, và ta có

[F : K] = (G : H)[E : K] = (G : H) Card(H) = Card(G),

và K là vành các bất biến của G trong F. Vậy F là một đại số Galois theo tiêu chuẩn cho trong Định lý 2, (v).

#### Mệnh đề 10 {#alg-viii-s16-prop-10 .statement tag=00JB}

Cho G là một nhóm hữu hạn. Cho L là một đại số Galois trên trường K với nhóm G, và cho $K'$ là một mở rộng của K. Khi đó $(K',G)$-đại số $L_{(K')}$ là một đại số Galois trên $K'$.

Ta dùng tính chất (v) trong Định lý 2 bằng cách nhận thấy rằng nếu K-đại số L là étale, thì $K'$-đại số $L_{(K')}$ cũng vậy (V, §6, No. 5, p. 32, Hệ quả 2), rằng ta có đẳng thức $[L_{(K')}: K'] = [L : K]$, và rằng vành các bất biến của G trong $L_{(K')}$ là $(L^G)_{(K')}$, trong đó $L^G$ là vành các bất biến của G trong L.

#### Mệnh đề 11 {#alg-viii-s16-prop-11 .statement tag=00JC}

Cho $G_1$ và $G_2$ là các nhóm. Cho $L_1$ và $L_2$ là các đại số Galois trên K với các tác động tương ứng $\lambda_1: G_1\rightarrow$ Aut$_K(L_1)$ và $\lambda_2: G_2\rightarrow$ Aut$_K(L_2)$. Đặt $L = L_1\otimes_KL_2,G = G_1\times G_2$, và $\lambda (g_1, g_2) =\lambda_1(g_1)\otimes \lambda_2(g_2)$ với $(g_1, g_2)\in G$. Khi đó K-đại số L được trang bị tác động $\lambda$ là một đại số Galois trên K.

Ta suy luận như trước, đồng thời xét rằng: Nếu $L_1$ và $L_2$ là étale, thì đại số $L = L_1\otimes_KL_2$ cũng vậy (V, §6, No. 5, p. 32, Hệ quả 1), và ta có các đẳng thức

$[L : K] = [L_1: K][L_2: K]$ và Card(G) = Card(G$_1$) Card(G$_2$).

Hơn nữa, nếu $L^{G_i}_i$ ký hiệu vành các bất biến của $G_i$ trong $L_i$, thì từ Bổ đề 11 dưới đây suy ra rằng $L^{G_1}_1\otimes_KL^{G_2}_2$ là vành các bất biến của $G_1\times G_2$ trong $L_1\otimes_KL_2$.

#### Bổ đề 11 {#alg-viii-s16-lem-11 .statement tag=00JD}

Cho $G_1$ và $G_2$ là các nhóm, và cho $W_1$ và $W_2$ là các K-không gian vectơ. Ta trang bị cho $W_1($resp. $W_2)$ một tác động của $G_1($resp. $G_2)$ được cho bởi một đồng cấu nhóm $\rho_1: G_1\rightarrow$ Aut$_K(W_1) ($resp. $\rho_2: G_2\rightarrow$ Aut$_K(W_2))$. Ta xét đồng cấu nhóm

$\rho_1\otimes \rho_2: G_1\times G_2\longrightarrow$ Aut$_K(W_1\otimes_KW_2)$

được xác định bởi quan hệ $(\rho_1\otimes \rho_2)(g_1, g_2)(w_1\otimes w_2) =\rho_1(g_1)(w_1)\otimes \rho_2(g_2)(w_2)$ với $g_1\in G_1,g_2\in G_2,w_1\in W_1$, và $w_2\in W_2$. Khi đó ánh xạ tuyến tính từ $W^{G_1}_1\otimes_KW^{G_2}_2$ đến $W_1\otimes_KW_2$ được cho bởi tích tenxơ của các đơn ánh chính tắc cảm sinh một đẳng cấu của các K-không gian vectơ từ $W_1^{G_1}\otimes_KW^{G_2}_2$ đến $(W_1\otimes_KW_2)^{G_1\times G_2}$.

Điều này suy ra từ Bổ đề 1 của VIII, p. 213 áp dụng cho các K[G]-môđun $M_1= M_2= K$ được trang bị tác động tầm thường của $G, N_1= W_1$, và $N_2= W_2$.

#### Nhận xét {#alg-viii-s16-n8-rem-1 .statement tag=00JE}

Cho $L$ là một mở rộng Galois của trường $K$ có bậc hữu hạn, và cho $G$ là nhóm Galois của nó; ta ký hiệu ánh xạ đồng nhất trên $G$ là $\lambda$. Khi đó $L$ được trang bị $\lambda$ là một đại số Galois trên $K$ với nhóm $G$. Cho $K'$ là một mở rộng của $K$. Theo Mệnh đề 10, đại số $L_{(K')}$ là Galois trên $K'$, nhưng nói chung nó không phải là một mở rộng của $K'$. Tương tự, theo Mệnh đề 11, tích tenxơ của các mở rộng Galois $E$ và $F$ của $K$ có bậc hữu hạn có thể được xem như một đại số Galois; nói chung, nó không phải là một mở rộng Galois của $K$. Tuy nhiên, nó là như vậy nếu $E$ và $F$ hơn nữa là các mở rộng con tách rời tuyến tính của một mở rộng của $K$ (V, §2, No. 5, p. 13 và V, §10, No. 1, p. 57, Mệnh đề 1).

### 9. Tích chéo

Cho $K$ là một trường, và cho $G$ là một nhóm có phần tử đơn vị mà ta ký hiệu là $e$. Cho $L$ là một đại số giao hoán trên $K$, và cho $\lambda$ là một đồng cấu từ $G$ vào nhóm tự đẳng cấu của đại số trên $K$ $L$. Với mọi $g$ trong $G$, cho $\tau (g)$ là tự đẳng cấu của nhóm nhân $L^*$ của $L$ cảm sinh bởi $\lambda (g)$.

Cho $\mathscr{E}= (\Gamma , \iota , \pi )$ là một $\tau$-mở rộng của nhóm $G$ bởi $L^*$. Định nghĩa một tác động phải của nhóm $L^*$ trên tập $L\times \Gamma$ bởi

$$
(\beta , \gamma ).\alpha = (\beta \alpha , \iota (\alpha )^{-1}\gamma ) \tag{20}
$$

với $\alpha \in L^*,\beta \in L$, và $\gamma \in \Gamma$. Ta ký hiệu $E$ là tập các quỹ đạo của $L^*$ trong $L\times \Gamma$ và $[\beta ;\gamma ]$ là quỹ đạo của cặp $(\beta , \gamma )$. Do đó, theo phép dựng, ta có quan hệ

$$
[\beta \alpha ;\gamma ] = [\beta ;\iota (\alpha )\gamma ] \tag{21}
$$

với $\alpha \in L^*,\beta \in L$, và $\gamma \in \Gamma$.

Cho $\beta$ trong $L$ và $\gamma$ trong Γ, ta ký hiệu $^{\gamma}\beta$ là biến đổi của $\beta$ dưới tự đẳng cấu $\lambda \circ \pi (\gamma )$ của $L$; ta có các hệ thức

(22) $^{\gamma}(^{\gamma'}\beta ) =^{\gamma \gamma'}\beta  ,^{\gamma}(\beta +\beta ') =^{\gamma}\beta +^{\gamma}\beta '$, và $^{\gamma}(\beta \beta ') =^{\gamma}\beta^{\gamma}\beta '$

với $\gamma , \gamma '$ trong Γ và $\beta , \beta '$ trong $L$. Tồn tại một luật hợp thành trên $E$ được đặc trưng bởi quan hệ

$$
[\beta ;\gamma ][\beta ';\gamma '] = [\beta^{\gamma}\beta ';\gamma \gamma '] \tag{23}
$$

Thật vậy, chỉ cần kiểm tra rằng vế phải không thay đổi nếu ta thay, tương ứng, $\beta ,\gamma ,\beta '$, và $\gamma '$ bằng $\beta \alpha ,\iota (\alpha )^{-1}\gamma ,\beta '\alpha '$, và $\iota (\alpha ')^{-1}\gamma '$ với mọi $\alpha ,\alpha '$ trong $L^*$. Điều này suy ra ngay lập tức bằng cách áp dụng cho $\mathscr{E}$ công thức (1) của VIII, p. 285, công thức này cũng có thể viết là $\gamma \iota (\alpha ) =\iota (^{\gamma}\alpha )\gamma$ với $\gamma \in \Gamma$ và $\alpha \in L^*$. Theo các công thức trong (22), tập $E$ được trang bị luật này là một monoid với phần tử đơn vị $[1;e]$.

Vì $\pi \circ \iota$ là hằng với giá trị $e$, tồn tại một ánh xạ $\widetilde{\pi}$ từ $E$ đến $G$ sao cho ta có

$$
\widetilde{\pi}([\beta ;\gamma ]) =\pi (\gamma ) \tag{24}
$$

với $\beta \in L$ và $\gamma \in \Gamma$.

Cho $g$ là một phần tử của G, và cho $E_g=\widetilde{\pi}^{-1}(g)$. Nếu $\gamma_0$ là một phần tử cố định của $\pi^{-1}(g)$, thì ánh xạ $\beta \mapsto [\beta ;\gamma_0]$ là một song ánh từ L đến $E_g$, nhờ đó ta sẽ chuyển sang $E_g$ cấu trúc không gian vectơ trên K của L. Vì $\pi^{-1}(g)$ gồm các phần tử có dạng $\iota (\alpha )\gamma_0$, trong đó $\alpha$ chạy qua $L^*$, và ta có

$$
[\beta ;\iota (\alpha )\gamma_0] = [\beta \alpha ;\gamma_0]
$$

nên cấu trúc không gian vectơ trên $E_g$ không phụ thuộc vào lựa chọn của $\gamma_0$.

Cho $g$ và $g'$ là các phần tử của G; theo các công thức (22) và (23), luật hợp thành trên E do hạn chế mà cảm sinh một ánh xạ K-song tuyến tính từ $E_g\times E_{g'}$ đến $E_{gg'}$. Do đó, không gian vectơ $P =\bigoplus_{g\in G}E_g$ được trang bị cấu trúc của một đại số kết hợp và có đơn vị, mà phép nhân của nó cảm sinh ánh xạ song tuyến tính trước đó từ $E_g\times E_{g'}$ đến $E_{gg'}$ với mọi $g$ và $g'$ trong G. Đại số P được gọi là tích có hướng của L và $\mathscr{E}$ và được ký hiệu bởi $\mathbf{A}[\mathscr{E}; L]$; phần tử đơn vị của nó là phần tử $[1;e]$ của $E_e$.

Đặt

$$
u(\beta ) = [\beta ;e] \tag{25}
$$

với $\beta$ trong L. Khi đó $u: L\rightarrow \mathbf{A}[\mathscr{E}; L]$ là một đơn cấu của K-đại số. Theo (23), với mọi $\gamma \in \Gamma$, phần tử $[1;\gamma ]$ là khả nghịch trong $\mathbf{A}[\mathscr{E},L]$, và ánh xạ $v: \Gamma \rightarrow \mathbf{A}[\mathscr{E},L]^*$ gửi $\gamma$ đến $[1;\gamma ]$ là một đơn cấu nhóm. Các đồng cấu $u$ và $v$ được gọi là chính tắc. Ta có các hệ thức

$$
u(\alpha ) =v(\iota (\alpha )) \tag{26}
$$

$$
u(^{\gamma}\beta ) =v(\gamma )u(\beta )v(\gamma )^{-1} \tag{27}
$$

$$
[\beta ;\gamma ] =u(\beta )v(\gamma ) \tag{28}
$$

với $\alpha \in L^*,\beta \in L$, và $\gamma \in \Gamma$.

Ngược lại, ta có tính chất phổ quát sau của đại số $\mathbf{A}[\mathscr{E}; L]$.

#### Mệnh đề 12 {#alg-viii-s16-prop-12 .statement tag=00JF}

Cho B là một K-đại số, $u': L\rightarrow B$ là một đồng cấu đại số trên K, và $v': \Gamma \rightarrow B^*$ là một đồng cấu nhóm. Ta giả sử các hệ thức sau được thỏa mãn

$$
u'(\alpha ) =v'(\iota (\alpha )) \tag{29}
$$

$$
u'(^{\gamma}\beta ) =v'(\gamma )u'(\beta )v'(\gamma )^{-1} \tag{30}
$$

với $\alpha \in L^*,\beta \in L$, và $\gamma \in \Gamma$. Khi đó tồn tại duy nhất một đồng cấu đại số $f$ từ $\mathbf{A}[\mathscr{E}; L]$ đến B sao cho ta có $u'=f\circ u$ và $v'=f\circ v$.

Để chứng minh tính duy nhất của $f$, xét rằng không gian vectơ $\mathbf{A}[\mathscr{E}; L]$ trên trường K được sinh bởi tập hợp các phần tử có dạng $[\beta ;\gamma ] =u(\beta )v(\gamma )$. Nếu đồng cấu $f':\mathbf{A}[\mathscr{E}; L]\rightarrow B$ thỏa $f'\circ u=u'$ và $f'\circ v=v'$, thì nó gửi $[\beta ;\gamma ]$ đến $u'(\beta )v'(\gamma )$ và do đó trùng với $f$.

Theo công thức (29), ta có

$$
u'(\beta \alpha )v'(\iota (\alpha )^{-1}\gamma ) =u'(\beta )v'(\gamma ) \tag{31}
$$

với $\alpha$ trong $L^*,\beta$ trong L, và $\gamma$ trong $\Gamma$. Theo định nghĩa của E, do đó tồn tại một ánh xạ $f_0: E\rightarrow B$ sao cho $f_0([\beta ;\gamma ]) =u'(\beta )v'(\gamma )$. Theo các công thức (23) và (30), ta có $f_0(xx') =f_0(x)f_0(x')$ với $x$ và $x'$ trong E. Hạn chế của $f_0$ lên $E_g$ là K-tuyến tính cho mọi phần tử $g$ của G; do đó, tồn tại một ánh xạ K-tuyến tính duy nhất $f$ từ $\mathbf{A}[\mathscr{E}; L]$ đến B trùng với $f_0$ trên E. Ánh xạ $f$ là một cấu xạ đại số thỏa $u'=f\circ u$ và $v'=f\circ v$.

#### Nhận xét {#alg-viii-s16-n9-rem-1 .statement tag=00JG}

Cho $\sigma : G\rightarrow \Gamma$ là một tiết diện của ánh xạ $\pi$. Đặt $\varepsilon_g=v(\sigma (g))$ với mọi $g$ trong G, và ký hiệu $c_{\sigma}$ là 2-cocycle liên kết với $\sigma$ (VIII, p. 296). Đặc biệt, ta có

$$
\varepsilon_g\varepsilon_{g'}=u(c_{\sigma}(g, g'))\varepsilon_{gg'} \tag{32}
$$

cho mọi $g, g'\in G$. Hơn nữa, hãy đồng nhất L với một đại số con của $\mathbf{A}[\mathscr{E}; L]$ thông qua đồng cấu u. Khi đó mọi phần tử của $\mathbf{A}[\mathscr{E}; L]$ có thể được viết duy nhất dưới dạng $\sum_{g\in G}a_g\varepsilon_g$, trong đó $(a_g)$ là một họ các phần tử của L có giá hữu hạn. Phép nhân trong $\mathbf{A}[\mathscr{E}; L]$ có thể được biểu diễn bởi công thức

$$
(\sum_ga_g\varepsilon_g)(\sum_gb_g\varepsilon_g)=\sum_gd_g\varepsilon_g \tag{33}
$$

với

$$
d_g=\sum_{hh'=g}a_h(\lambda (h)\cdot b_{h'})c_{\sigma}(h, h') \tag{34}
$$

Nếu mở rộng $\mathscr{E}$ là nửa tầm thường, thì ta có thể chọn một tiết diện $\sigma$ của $\pi$ là một cấu xạ nhóm từ G đến Γ; do đó, 2-cocycle $c_{\sigma}$ là hằng với giá trị 1, và công thức (34) rút gọn thành

$$
d_g=\sum_{hh'=g}a_h\lambda (h)\cdot b_{h'} \tag{35}
$$

Let $K'$ be an extension of the field K. Denote by $L'$ the $K'$-algebra $L_{(K')}$, and for any $g$ in G, denote by $\lambda '(g)$ the automorphism $\lambda (g)_{(K')}$ induced by $\lambda (g)$ on $L_{(K')}$. Moreover, let us denote by $\tau '(g)$ the automorphism of $L^{'*}$ induced by $\lambda '(g)$. Finally, let $h$ be the homomorphism from $L^*$ to $L^{'*}$ that sends $x$ to $x\otimes 1$. Let $\mathscr{E}'= (\Gamma ', \iota ', \pi ')$ be the direct image of the extension of $\mathscr{E}$ by $h$ (VIII, p. 289). Let $\mathbf{A}[\mathscr{E}',L']$ be the cross product $K'$-algebra of $\mathscr{E}'$ and $L'$, and let $u': L'\rightarrow \mathbf{A}[\mathscr{E}',L']$ and $v': \Gamma '\rightarrow \mathbf{A}[\mathscr{E}',L']^*$ be the canonical homomorphisms.

#### Mệnh đề 13 {#alg-viii-s16-prop-13 .statement tag=00JH}

Tồn tại duy nhất một đẳng cấu của $K'$-đại số $\varphi$ từ $\mathbf{A}[\mathscr{E}; L]_{(K')}$ đến $\mathbf{A}[\mathscr{E}'; L']$ thỏa mãn các hệ thức

$$
u'(h(\beta )) =\varphi (1\otimes u(\beta )) \tag{36}
$$

với $\beta \in L$ và

$$
v'(h(\gamma )) =\varphi (1\otimes v(\gamma )) \tag{37}
$$

với $\gamma \in \Gamma$.

Chứng minh suy ra ngay từ các phép xây dựng.

Đẳng cấu $\varphi$ được gọi là chính tắc.

### 10. Ứng dụng vào nhóm Brauer

Trong tiểu mục này, K là một trường, và L là một đại số Galois trên K với tác động $\lambda : G\rightarrow$ Aut$_K(L)$. Ta ký hiệu bậc của L trên K là $n$. Ta có $n=$ Card(G).

#### Định lý 3 {#alg-viii-s16-thm-3 .statement tag=00JI}

Cho $\mathscr{E}= (\Gamma , \iota , \pi )$ là một $\tau$-mở rộng của G bởi $L^*$. Đại số $\mathbf{A}[\mathscr{E}; L]$ là đơn tâm và có bậc $n^2$ trên K. Hơn nữa, đồng cấu chính tắc $u$ từ L đến $\mathbf{A}[\mathscr{E}; L]$ là một đẳng cấu từ L đến một đại số con giao hoán cực đại của $\mathbf{A}[\mathscr{E}; L]$.

#### Bổ đề 12 {#alg-viii-s16-lem-12 .statement tag=00JJ}

a) Không tồn tại bất kỳ iđêan nào của L, ngoài $\{0\}$ và L, là bất biến dưới G.

b) Cho $g$ là một phần tử của G khác với phần tử đơn vị, và cho $\mathfrak{a}_g$ là iđêan của L sinh bởi các phần tử có dạng $x-\lambda (g)x$, trong đó $x$ chạy qua L. Ta có $\mathfrak{a}_g= L$.

Cho $\mathscr{S}$ là tập các iđêan cực đại của L; với mọi tập con S của $\mathscr{S}$, đặt $\mathfrak{a}(S) =\bigcap_{\mathfrak{m}\in S}\mathfrak{m}$. Vì vành L là giao hoán và nửa đơn (VIII, p. 310, Nhận xét 6), ánh xạ $W\mapsto \mathfrak{a}(W)$ là một song ánh từ tập hợp các tập con của $\mathscr{S}$ đến tập hợp các iđêan của L (VIII, p. 142, Mệnh đề 9). Iđêan $\mathfrak{a}(S)$ là bất biến dưới G khi và chỉ khi S là như vậy. Vì G tác động bắc cầu trên $\mathscr{S}$ (VIII, p. 308, Định lý 2, vi)), các tập con duy nhất của $\mathscr{S}$ bất biến dưới G là $\emptyset$ và $\mathscr{S}$. Vì $\mathfrak{a}(\emptyset ) = L$ và $\mathfrak{a}(\mathscr{S}) =\{0\}$, ta đã chứng minh mệnh đề a).

Bây giờ chứng minh b) bằng phản chứng; giả sử rằng ta có $\mathfrak{a}_g\not= L$. Cho $\mathfrak{m}$ là một iđêan cực đại của L chứa $\mathfrak{a}_g$. Khi đó ta có $\lambda (g)x\equiv x$ mod $\mathfrak{m}$ với mọi $x$ trong L. Đặc biệt, $\mathfrak{m}$ là bất biến dưới $g$, và $\lambda (g)$ được cảm sinh bởi đồng nhất trên trường $L/\mathfrak{m}$. Theo tính chất (vi) trong Định lý 2 của VIII, p. 308, phần tử $g$ của $G_{\mathfrak{m}}$ là tầm thường, điều này mâu thuẫn với giả thiết của b).

Bây giờ chứng minh Định lý 3. Không gian vectơ $\mathbf{A}[\mathscr{E}; L]$ có số chiều hữu hạn Card(G)[L$: K] =n^2$ trên K, theo VIII, p. 316 và đẳng thức giả thiết Card(G) $= [L : K] =n$.

Cho $\mathfrak{a}$ là một iđêan hai phía khác không của đại số $\mathbf{A}[\mathscr{E}; L]$. Ta dùng ký hiệu của VIII, p. 316. Mỗi phần tử $a$ của $\mathbf{A}[\mathscr{E}; L]$ có thể viết duy nhất là $a=\sum_{g\in G}a_g\varepsilon_g$ với $a_g\in L$ với mọi $g\in G$; ta ký hiệu bởi $\Phi (a)$ tập hợp các phần tử $g$ của G sao cho $a_g\not= 0$. Theo công thức (32) của VIII, p. 316, ta có quan hệ

$$
\varepsilon_g\varepsilon_{g'}=c_{\sigma}(g, g')\varepsilon_{gg'} \tag{38}
$$

với mọi $g, g'\in G$ và do đó

$$
\Phi (a\varepsilon_g) = \Phi (a).g \tag{39}
$$

với mọi $g\in G$ và $a\in \mathbf{A}[\mathscr{E}; L]$.

Cho $a$ là một phần tử khác không của $\mathfrak{a}$ sao cho $\Phi (a)$ là cực tiểu theo bao hàm; theo công thức (39), nếu cần thay thế $a$ bởi một phần tử có dạng $a\varepsilon_{g^{-1}}$ với $g\in \Phi (a)$, ta có thể giả sử rằng $e\in \Phi (a)$. Cho $s$ là một phần tử của $\Phi (a)$ phân biệt với $e$. Theo Bổ đề 12, b), tồn tại một phần tử $x$ của L sao cho $a_s(x-\lambda (s)\cdot x)\not= 0$. Nhưng ta có quan hệ

$$
xa-ax=\sum_ga_g(x-\lambda (g)\cdot x)\varepsilon_g \tag{40}
$$

trong đó tổng được lấy trên các phần tử $g$ của $\Phi (a)$ phân biệt với $e$. Do tính tối tiểu của $\Phi (a)$, ta có $xa-ax= 0$, nhưng điều này mâu thuẫn với giả thiết về $x$. Do đó, bằng phản chứng, ta đã chứng minh rằng $\Phi (a)$ chỉ chứa phần tử đơn vị $e$ của G, nên $a\in L$.

Suy ra $L\cap \mathfrak{a}$ là một iđêan của L không giảm về $\{0\}$. Hơn nữa, với mọi $x$ trong L, ta có $\varepsilon_gx\varepsilon^{-1}_g=\lambda (g)\cdot x$, nên $L\cap \mathfrak{a}$ bất biến dưới G. Theo Bổ đề 12, do đó ta có $L\cap \mathfrak{a}= L$, tức là $L\subset \mathfrak{a}$. Vì L chứa phần tử đơn vị của $\mathbf{A}[\mathscr{E}; L]$, ta có $\mathfrak{a}=\mathbf{A}[\mathscr{E}; L]$.

Vì đại số $\mathbf{A}[\mathscr{E}; L]$ có chiều hữu hạn khác không trên K và các iđêan hai phía duy nhất của nó là $\{0\}$ và $\mathbf{A}[\mathscr{E}; L]$, nên nó là đơn.

Ta hãy chứng minh rằng mọi phần tử $a$ của $\mathbf{A}[\mathscr{E}; L]$ giao hoán với L đều thuộc L. Ta viết $a$ dưới dạng $\sum_{g\in G}a_g\varepsilon_g$ với các hệ số $a_g$ trong L. Với mọi $x$ trong L, ta có $xa-ax= 0$, và quan hệ (40) cho thấy rằng

$$
a_g(x-\lambda (g)\cdot x) = 0 \tag{41}
$$

với mọi $g\in G$ và $x\in L$. Theo Bổ đề 12, do đó ta có $a_g= 0$ với $g\not=e$; do đó, $a\in L$.

Cuối cùng, ta hãy xác định tâm của $\mathbf{A}[\mathscr{E}; L]$. Nếu $z$ thuộc tâm, thì nó giao hoán với L, nên thuộc L. Nhưng khi đó ta có

$$
0 =\varepsilon_gz-z\varepsilon_g= (\lambda (g)\cdot z-z)\varepsilon_g
$$

với mọi $g$ của G. Suy ra $z$ bất biến dưới nhóm tự đẳng cấu $\lambda (G)$ của L. Do đó, theo giả thiết, ta có $z\in K$.

#### Định lý 4 {#alg-viii-s16-thm-4 .statement tag=00JK}

Cho A là một đại số đơn tâm bậc hữu hạn trên K, và cho L là một đại số con giao hoán cực đại của A. Khi đó tồn tại một $\tau$-mở rộng $\mathscr{E}$ của G bởi $L^*$ sao cho A đẳng cấu với $\mathbf{A}[\mathscr{E}; L]$.

Không mất tính tổng quát, ta có thể giả sử rằng L là một đại số con giao hoán cực đại của A. Gọi Γ là nhóm nhân gồm các phần tử khả nghịch $\gamma$ của A sao cho tồn tại một $g$ trong G với

$$
\gamma x\gamma^{-1}=\lambda (g).x \tag{42}
$$

với mọi phần tử $x$ của L. Nếu $\gamma \in \Gamma$ được cho, thì phần tử $g$ thỏa mãn quan hệ này là duy nhất; ta ký hiệu nó là $\pi (\gamma )$. Hiển nhiên $\pi$ là một đồng cấu từ Γ vào G và hạt nhân của nó bằng $L^*$. Tính toàn ánh của $\pi$ suy ra từ định lý Skolem–Noether (VIII, p. 263, Hệ quả).

Nếu ta ký hiệu đơn ánh chính tắc của $L^*$ vào Γ bởi $\iota$, thì từ các xây dựng suy ra rằng $\mathscr{E}= (\Gamma , \iota , \pi )$ là một $\tau$-mở rộng của G bởi $L^*$. Gọi

$u: L\rightarrow \mathbf{A}[\mathscr{E}; L]$ và $v: \Gamma \rightarrow \mathbf{A}[\mathscr{E}; L]$

là các đồng cấu chính tắc. Theo tính chất phổ quát của $\mathbf{A}[\mathscr{E}; L]$ (VIII, p. 315, Mệnh đề 12), tồn tại duy nhất một đồng cấu đại số $f:\mathbf{A}[\mathscr{E}; L]\rightarrow A$ sao cho $f\circ u(x) =x$ và $f\circ v(\gamma ) =\gamma$ với $x\in L$ và $\gamma \in \Gamma$. Vì đại số $\mathbf{A}[\mathscr{E}; L]$ là đơn, nên đồng cấu $f$ là đơn ánh. Hơn nữa, đại số $\mathbf{A}[\mathscr{E}; L]$ có bậc $n^2$ trên K và A cũng có bậc ấy vì L là một đại số con giao hoán nửa đơn cực đại của A và ta có $n= [L : K]$ (VIII, p. 262, Mệnh đề 3, (ii)). Do đó $f$ là song ánh.

#### Định nghĩa 2 {#alg-viii-s16-def-2 .statement tag=00JL}

Cho $\mathscr{S}$ là tập hợp các ideal cực đại của L. Ta định nghĩa

Br(L$/K$) $=\bigcap_{\mathfrak{m}\in\mathscr{S}}$ Ker($r_{(L/\mathfrak{m})/K}$), trong đó $r_{(L/\mathfrak{m})/K}:$ Br(K) $\rightarrow$ Br(L$/\mathfrak{m}$) là đồng cấu mở rộng vô hướng (VIII, p. 281).

#### Định lý 5 {#alg-viii-s16-thm-5 .statement tag=00JM}

Tồn tại một đẳng cấu nhóm

Ψ : Ex$_{\tau}(G,L^*)\longrightarrow$ Br(L$/K$)

gửi lớp của một $\tau$-mở rộng $\mathscr{E}$ của G bởi $L^*$ tới lớp trong Br(L$/K$) của đại số $\mathbf{A}[\mathscr{E}; L]$.

Để định nghĩa Ψ và kiểm tra rằng nó là một song ánh, ta phải thiết lập các điểm sau:

a) Nếu $\mathscr{E}$ và $\mathscr{E}'$ là các $\tau$-mở rộng đẳng cấu của G bởi $L^*$, thì các đại số $\mathbf{A}[\mathscr{E}; L]$ và $\mathbf{A}[\mathscr{E}'; L]$ đẳng cấu.

b) Ngược lại, nếu các đại số $\mathbf{A}[\mathscr{E}; L]$ và $\mathbf{A}[\mathscr{E}'; L]$ đẳng cấu, thì các $\tau$-mở rộng $\mathscr{E}$ và $\mathscr{E}'$ của G bởi $L^*$ đẳng cấu.

c) Trong mỗi lớp của Br(L$/K$), có một đại số E chứa L như một đại số con giao hoán cực đại.

d) Nếu E là một đại số đơn tâm có bậc hữu hạn trên K chứa L như một đại số con giao hoán cực đại, thì tồn tại một $\tau$-mở rộng $\mathscr{E}$ của G bởi $L^*$ sao cho E đẳng cấu với $\mathbf{A}[\mathscr{E}; L]$.

Mệnh đề a) suy ra từ phép dựng của tích có hướng; b) suy ra từ VIII, p. 263, Hệ quả. Mệnh đề c) suy ra từ Mệnh đề 5 của VIII, p. 281, và d) đơn giản là Định lý 4 ở trên.

#### Nhận xét 1 {#alg-viii-s16-n10-rem-1 .statement tag=00JN}

Còn phải kiểm tra rằng Ψ là một đồng cấu nhóm; để làm điều này, chỉ cần chứng minh rằng nếu $\mathscr{E}_1= (\Gamma_1, \iota_1, \pi_1)$ và $\mathscr{E}_2= (\Gamma_2, \iota_2, \pi_2)$ là các $\tau$-mở rộng, thì đại số $\mathbf{A}[\mathscr{E}_1\mathscr{E}_2; L]$ tương đương với đại số $\mathbf{A}[\mathscr{E}_1; L]\otimes \mathbf{A}[\mathscr{E}_2; L]$. Ta kí hiệu mở rộng tích $\mathscr{E}_1\mathscr{E}_2$ bởi $\mathscr{E}= (\Gamma , \iota , \pi )$. Nhóm Γ đẳng cấu với đối hạt nhân của đồng cấu $\rho$ từ $L^*$ đến tích sợi $\Gamma_1\times_G\Gamma_2$ gửi $\mu$ vào $(\iota_1(\mu), \iota_2(\mu)^{-1})$. Với $i\in  \{1,2\}$, đặt $A_i=\mathbf{A}[\mathscr{E}_i; L]$. Cho $u_i: L\rightarrow A_i$ và $v_i: \Gamma_i\rightarrow A^*_i$ là các đồng cấu chính tắc. Đồng nhất L với các ảnh của nó qua các đồng cấu $u_i$, các đồng cấu này biến L thành các đại số con giao hoán cực đại của các $A_i$. Kí hiệu $V_i$ là không gian vectơ trên L được xác định bởi phép nhân trái trong $A_i$. Vành $L\otimes_KA^o_i$ tác động lên $V_i$. Vì nó là đơn và có chiều $n^2$ trên L, ta thu được một đẳng cấu từ $L\otimes_KA^o_i$ đến End$_L(V_i)$. Do đó vành $L\otimes_KA^o_1\otimes_KA^o_2$, mà ta có thể đồng nhất với $(L\otimes_KA^o_1)\otimes_L(L\otimes_KA^o_2)$, đẳng cấu với End$_L(V_1\otimes_LV_2)$. Đặt C = End$_{A^o_1\otimes_KA^o_2}(V_1\otimes_LV_2)$. Theo Bổ đề 3 của VIII, p. 282, vành C tương tự với $A_1\otimes_KA_2$, và $L\otimes 1\otimes 1$ là một đại số con giao hoán cực đại của C. Với mỗi cặp $(\gamma_1, \gamma_2)\in \Gamma_1\times \Gamma_2$ thỏa mãn $\pi_1(\gamma_1) =\pi_2(\gamma_2)$, ta kí hiệu $w(\gamma_1, \gamma_2)$ là $\lambda (\pi_1(\gamma_1$))-nửa tuyến tính (II, §1, No. 13, p. 223) tự đồng cấu duy nhất sao cho

$$
w(\gamma_1, \gamma_2)(x_1\otimes x_2) =v_1(\gamma_1)x_1\otimes v_2(\gamma_2)x_2
$$

với $x_1\in V_1$ và $x_2\in V_2$. Ta có $w(\gamma_1, \gamma_2)\in C^*$, và $w$ là một đồng cấu nhóm từ tích sợi $\Gamma_1\times_G\Gamma_2$ đến $C^*$. Đồng cấu này tầm thường trên ảnh của $\rho$ và cảm sinh một đồng cấu $v$ từ Γ đến $C^*$. Kí hiệu $u: L\rightarrow C$ là cấu xạ được cho bởi $u:\ell \mapsto \ell \otimes 1\otimes 1$. Ta có thể kiểm tra các quan hệ

$u(\alpha ) =v(\iota (\alpha ))$ và $u(^{\gamma}\beta ) =v(\gamma )u(\beta )v(\gamma )^{-1}$

với $\alpha \in L^*,\beta \in L$, và $\gamma \in \Gamma$. Mệnh đề 12 của VIII, p. 315 cho một đồng cấu $f$ từ đại số $\mathbf{A}[\mathscr{E}; L]$ đến C. Vì đại số $\mathbf{A}[\mathscr{E}; L]$ là đơn, đồng cấu $f$ là đơn ánh. Các đại số C và $\mathbf{A}[\mathscr{E}; L]$ có cùng chiều trên K, nên $f$ là một đẳng cấu.

#### Nhận xét 2 {#alg-viii-s16-n10-rem-2 .statement tag=00JO}

Ta có thể tính một 2-xiclo $c$ liên kết với một đại số A bị tách bởi một mở rộng Galois hữu hạn L với nhóm G như sau. Trước hết, tồn tại một K-đồng cấu $\varphi : A\rightarrow \mathbf{M}_m$(L), với $[A : K] =m^2$. Với $g\in G$, đặt $\varphi^g$ là đồng cấu từ A đến $\mathbf{M}_m(L)$ cho bởi $a\mapsto \varphi (g^{-1}ag)$. Theo định lý Skolem–Noether (VIII, p. 256, Định lý 3), với mọi $g\in G$, tồn tại một phần tử $u_g$ của $\mathbf{G}\mathbf{L}_m(L)$ sao cho

$$
\varphi^g(a) =u_g\varphi (a)u^{-1}_g
$$

với $a\in A$. Khi đó ta đặt

$$
c(g, g') =u_gu_{g'}u^{-1}_{gg'}
$$

Ta cũng có thể định nghĩa một mở rộng của G bởi $L^*$ bằng $\varphi :$ ta xét nhóm $\Gamma \subset \mathbf{G}\mathbf{L}_m(L)$ gồm các $\gamma$ sao cho tồn tại $g\in G$ với

$$
\varphi^g(a) =\gamma \varphi (a)\gamma^{-1}
$$

với mọi $a\in A$. Lớp của mở rộng này là ảnh ngược qua Ψ của lớp của A trong Br(L$/K$).

#### Hệ quả {#alg-viii-s16-n10-cor-1 .statement tag=00JP}

Ánh xạ $\Phi_{L/K}= \Theta \circ \Psi^{-1}$ định nghĩa một đẳng cấu nhóm từ Br(L$/K$) đến $H^2(G,L^*)$.

Cho K' là một mở rộng của K và $\varphi : K'\rightarrow L$ là một đồng cấu K-đại số. Tập H gồm các phần tử h của G sao cho $\lambda (h)\circ \varphi =\varphi$ là một nhóm con của G, và $K'$-đại số L được trang bị hạn chế của $\lambda$ lên H là một đại số Galois trên K'.

#### Mệnh đề 14 {#alg-viii-s16-prop-14 .statement tag=00JQ}

Biểu đồ sau giao hoán:

Br(L$/K$)$^{\Phi_{L/K}}/$/ $H_2(G,L_*)$

$r_{K'/K}$ Res$^G_H$

Br(L$/K'$)$^{\Phi_{L/K'}}/$/ $H_2(H,L_*)$ .

Điều này suy ra từ các Mệnh đề 7 của VIII, p. 299 và 13 của VIII, p. 317.

### 11. Chỉ số và số mũ

#### Định lý 6 {#alg-viii-s16-thm-6 .statement tag=00JR}

Cho K là một trường giao hoán, và cho A là một A-đại số đơn tâm bậc hữu hạn trên K. Cho L là một mở rộng tách được của K bậc hữu hạn là một trường phân rã của đại số A. Khi đó [L : K][A] bằng 0 trong Br(K).

Tồn tại một mở rộng M của L là một mở rộng Galois hữu hạn của K (V, §10, No. 1, p. 57, Mệnh đề 2). Lớp [A] của A trong nhóm Brauer của K thuộc nhóm con Br(M$/K$). Cho G là nhóm Galois của M trên K, và cho $\alpha$ là ảnh của [A] trong $H^2(G,M^*)$ (VIII, p. 321, Hệ quả). Cho H là nhóm Galois của M trên L. Khi đó H là một nhóm con chỉ số [L : K] trong G (V, §10, No. 7, p. 68, Hệ quả 5). Vì Res$^G_H(\alpha ) = \Phi_{M/L}(A_{(L)})$ (Mệnh đề 14), ta có Res$^G_H(\alpha ) = 0$. Theo Mệnh đề 8 của VIII, p. 303, suy ra $[L : K]\alpha = 0$, và do đó [L : K][A] = 0.

Cho K là một trường giao hoán, và cho A là một đại số đơn tâm bậc hữu hạn trên K. Khi đó A đẳng cấu với một đại số có dạng $\mathbf{M}_n$(D), trong đó D là một trường có tâm K, và [A] = [D] trong Br(K). Bậc rút gọn của D chỉ phụ thuộc vào A. Ta gọi bậc rút gọn này là chỉ số của A. Chỉ số của A chia hết bậc rút gọn của A. Số mũ của A là cấp của lớp của A trong nhóm Brauer của K.

#### Hệ quả 1 {#alg-viii-s16-thm-6-cor-1 .statement tag=00JS}

Số mũ của một đại số đơn tâm bậc hữu hạn trên một trường giao hoán chia hết chỉ số của nó.

Chỉ cần chứng minh điều này cho một trường D bậc hữu hạn trên tâm K của nó. Cho L là một trường con giao hoán cực đại của D là một mở rộng tách được của K; ta có $[D : K] = [L : K]^2$ (VIII, p. 265, Hệ quả 2, b) và c)). Khi đó mở rộng L của K là một trường phân rã của đại số D (VIII, p. 281, Mệnh đề 5), và [L : K] trùng với bậc rút gọn của D. Khi đó áp dụng Định lý 6.

#### Hệ quả 2 {#alg-viii-s16-thm-6-cor-2 .statement tag=00JT}

Cho K là một trường giao hoán, và cho A là một đại số đơn tâm bậc hữu hạn trên K. Cho $p$ là một số nguyên tố. Nếu $p$ chia hết chỉ số của A, thì nó chia hết số mũ của A.

Giả sử rằng số nguyên tố $p$ không chia hết số mũ của A và chứng minh rằng nó không chia hết chỉ số của A. Chỉ cần chứng minh kết quả này trong trường hợp A là một trường. Cho L là một mở rộng Galois hữu hạn của K làm tách A. Cho G là nhóm Galois của L trên K, và cho H là một $p$-nhóm Sylow của G (I, §6, No. 6, p. 78). Ký hiệu $L'= L^H$ là trường con của L gồm các bất biến của H. Số mũ của $A_{(L')}$ chia hết số mũ của A và do đó nguyên tố cùng nhau với $p$. Theo Định lý 6, ta có $[L : L'][A_{(L')}] = 0$ trong nhóm Brauer của $L'$. Suy ra $[A_{(L')}] = 0$ và trường $L'$ là trường phân rã của A. Khi đó áp dụng Hệ quả 2 của VIII, p. 283; suy ra chỉ số của A chia hết $[L': K]$ và do đó không chia hết cho $p$.

#### Hệ quả 3 {#alg-viii-s16-thm-6-cor-3 .statement tag=00JU}

Cho $p$ là một số nguyên tố và cho K là một trường hoàn hảo có đặc số $p$. Cho A là một đại số đơn tâm có bậc hữu hạn trên K. Khi đó $p$ không chia hết chỉ số của A.

Ta chứng minh rằng nhóm Brauer của K không chứa bất kỳ phần tử nào có cấp $p$. Mọi mở rộng Galois M của K có bậc hữu hạn đều là một trường hoàn hảo (V, §7, No. 1, p. 36, Mệnh đề 2). Do đó việc lấy lũy thừa bậc $p$ là một tự đẳng cấu của nhóm $M^*$. Suy ra phép nhân với $p$ là một tự đẳng cấu của nhóm $H^2$(Gal(M$/K$)$,M^*)$ đẳng cấu với Br(M$/K$).

Do đó, cấp của [A] nguyên tố cùng với $p$ và, theo Hệ quả 2, chỉ số của nó không chia hết cho $p$.

#### Nhận xét {#alg-viii-s16-n11-rem-1 .statement tag=00JV}

Bằng cách xét các tích tenxơ của các đại số quaternion, có thể xây dựng các trường có tâm K, số mũ 2, và chỉ số tùy ý lớn (cf. VIII, p. 371, Exercises 7 and 8).

$*$Ngược lại, nếu K là một mở rộng Galois hữu hạn của một trường $p$-adic hoặc một trường của chuỗi lũy thừa hình thức trên một trường hữu hạn, thì số mũ của một đại số đơn tâm có bậc hữu hạn trên K bằng chỉ số của nó (VIII, p. 332, Exercise 17, e)).$*$

### Bài tập {#alg-viii-s16-exercises}

Xem [bài tập cho § 16](exercises/s16/).
