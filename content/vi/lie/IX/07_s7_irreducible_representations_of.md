---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IX
chapter_title: COMPACT REAL LIE GROUPS
section: 7
section_title: Irreducible representations of connected compact Lie groups
lang: vi
source: lie-vii-ix
book_pages: 347-359, 414-417
pdf_pages: 0354-0366, 0421-0424
extraction: native
subsections:
    - "no": 1
      title: DOMINANT CHARACTERS
      page: 347
      pdf_page: 354
    - "no": 2
      title: HIGHEST WEIGHT OF AN IRREDUCIBLE REPRESENTATION
      page: 348
      pdf_page: 355
    - "no": 3
      title: THE RING R(G)
      page: 351
      pdf_page: 358
    - "no": 4
      title: CHARACTER FORMULA
      page: 353
      pdf_page: 360
    - "no": 5
      title: DEGREE OF IRREDUCIBLE REPRESENTATIONS
      page: 356
      pdf_page: 363
    - "no": 6
      title: CASIMIR ELEMENTS
      page: 358
      pdf_page: 365
statements: 28
exercises: 8
content_sha256: bf745ad7d616247079dc8d4ff8eaccea9b34909364c76fac74cb387b10f8c61d
translated_from: content/en/lie/IX/07_s7_irreducible_representations_of.md
source_content_sha256: e5d4512731c2c4775f6967a56df8bfea9f2c9f836e9424ff340a85f1fc7ae72d
translation_model: gpt-5-6, gpt-5-6-mini, gpt-5.4-mini, gpt-5-mini
translation_run: translate-vi-82beb20c
glossary_version: 34
glossary_terms_sha256: 8e77e50d32d3d2704c2c78cf99adeb7c884c88128d5b132c5e773df1ab9a209b
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 7. CÁC BIỂU DIỄN BẤT KHẢ QUY CỦA CÁC NHÓM LIE COMPACT LIÊN THÔNG

Ta giữ lại các ký hiệu của §6. Một biểu diễn của G là một đồng cấu liên tục (do đó giải tích) từ G vào một nhóm $\mathbf{G}\mathbf{L}(V)$, trong đó V là một không gian vectơ phức hữu hạn chiều. Mọi biểu diễn của G đều nửa đơn (§1, no. 1).

Chọn một phòng C của $\mathfrak{t}($§5, no. 2), và đặt $\Gamma (T)_{++}=\overline{C}\cap \Gamma (T)$.

### 1. CÁC ĐẶC TRƯNG TRỘI

Ký hiệu $X_+$ là tập hợp các phần tử $\lambda$ của X(T) sao cho $\langle \lambda , x\rangle  \geq 0$ với mọi $x\in \Gamma (T)_{++}$, nghĩa là, sao cho dạng tuyến tính $\delta (\lambda ) :\mathfrak{t}_{\mathbf{C}}\rightarrow \mathbf{C}$ biến phòng C của $\mathfrak{t}$ thành $i\mathbf{R}_+$.

Trang bị cho X(T) cấu trúc nhóm có thứ tự mà các phần tử dương là các phần tử của $X_+$; đặt $R_+= R(G,T)\cap X_+$ và $R_-=-R_+$. Các phần tử của $R_+$ được gọi là các nghiệm dương, các phần tử của $R_-$ được gọi là các nghiệm âm; mỗi nghiệm hoặc là dương hoặc là âm (Chap. VI, §1, no. 6, Định lý 3). Một nghiệm dương không phải là tổng của hai nghiệm dương được gọi là đơn; mọi nghiệm dương là tổng của các nghiệm đơn (loc. cit.); các nghiệm đơn tạo thành một cơ sở của nhóm con của X(T) sinh bởi các nghiệm, một nhóm con có thể được đồng nhất với $X(T/C(G))$ (§4, no. 4); các phép phản xạ đối với các nghiệm đơn sinh ra nhóm Weyl $W = W_G(T)$ (Chap. VI, §1, no. 5, Định lý 2).

#### Bổ đề 1 {#lie-ix-s7-lem-1 .statement tag=01FZ}

Cho $\lambda$ là một phần tử của X(T). Các điều kiện sau là tương đương:

(i) $\lambda -w(\lambda )\geq 0$ (resp. $>0$) với mọi $w\in W$ sao cho $w\not= 1$;

(ii) với mọi $w\in W$ sao cho $w\not= 1,\lambda -w(\lambda )$ là một tổ hợp tuyến tính với các hệ số dương (resp. các hệ số dương không phải tất cả đều bằng không) của các nghiệm đơn;

(iii) $\langle \lambda , K_{\alpha}\rangle  \geq 0$ (resp. $>0$) với mọi nghiệm dương $\alpha$;

(iv) $\langle \lambda , K_{\alpha}\rangle  \geq 0$ (resp. $>0$) với mọi nghiệm đơn $\alpha$.

Sự tương đương của (iii) và (iv) là ngay lập tức. Vì tập hợp các $K_{\alpha}$ có thể được đồng nhất với hệ nghiệm nghịch đảo của $R(G,T) ($§4, no. 5), sự tương đương của (i) và (iii) suy ra từ Chap. VI, §1, no. 6, Mệnh đề 18 và Hệ quả. Hàm ý (ii) $\Rightarrow$ (i) là tầm thường, và hàm ý đối suy ra từ loc. cit.

Ký hiệu $X_{++}$ là tập hợp các phần tử của X(T) sao cho $\langle \lambda , K_{\alpha}\rangle  \geq 0$ với mọi nghiệm dương $\alpha$. Các phần tử của $X_{++}$ được gọi là trội. Chúng tạo thành một miền cơ bản cho phép toán của W trên X(T) (Chap. VI, §1, no. 10). Ta có $X_{++}\subset X_+$.

Nếu G đơn liên, với mỗi nghiệm đơn $\alpha$ tồn tại một phần tử $\varpi_{\alpha}$ của X(T) sao cho $\langle \varpi_{\beta}, K_{\alpha}\rangle =\delta_{\alpha \beta}$ với mỗi nghiệm đơn $\beta$, nghĩa là, $s_{\alpha}(\varpi_{\alpha}) =$ $\varpi_{\alpha}-\alpha ,s_{\beta}(\varpi_{\alpha}) =\varpi_{\alpha}$ với mỗi nghiệm đơn $\beta \not=\alpha$; các $\varpi_{\alpha}$ được gọi là các trọng số trội cơ bản; chúng tạo thành một cơ sở của nhóm giao hoán X(T) và của nửa nhóm giao hoán $X_{++}$; chính xác hơn, mỗi phần tử $\lambda$ của X(T) có thể được viết dưới dạng $\lambda =\sum_{\alpha}\langle \lambda , K_{\alpha}\rangle \varpi_{\alpha}$.

Ký hiệu $\rho$ là phần tử của $X(T)\otimes \mathbf{Q}$ sao cho

$$
2\rho =\sum_{\alpha\in R_+}\alpha
$$

Ta có $\langle \rho , K_{\alpha}\rangle = 1$ với mọi nghiệm đơn $\alpha$ (Chap. VI, §1, no. 10, Mệnh đề 29). Nếu G đơn liên, $\rho$ là tổng của các trọng số trội cơ bản.

### 2. TRỌNG SỐ CAO NHẤT CỦA MỘT BIỂU DIỄN BẤT KHẢ QUY

Gắn với mọi biểu diễn $\tau : G\rightarrow \mathbf{G}\mathbf{L}(V)$ đồng cấu $L(\tau )_{(\mathbf{C})}$ từ đại số Lie $\mathbf{C}$-Lie $\mathfrak{g}_{\mathbf{C}}$ vào End(V) mở rộng biểu diễn tuyến tính $L(\tau )$ của $\mathfrak{g}$ trên không gian vectơ thực nền của V (Chap. III, §3, no. 11). Theo Mệnh đề 7 của §4, no. 3, ánh xạ $\delta$ từ X(T) vào Hom$_{\mathbf{C}}(\mathfrak{t}_{\mathbf{C}},\mathbf{C}) =\mathfrak{t}^*_{\mathbf{C}}$ cảm sinh một song ánh từ tập hợp các trọng số của $\tau$ tương đối với T vào tập hợp các trọng số của $L(\tau )_{(\mathbf{C})}$ tương đối với đại số con Cartan $\mathfrak{t}_{\mathbf{C}}$ của $\mathfrak{g}_{\mathbf{C}}$.

#### Bổ đề 2 {#lie-ix-s7-lem-2 .statement tag=01G0}

Cho $\varphi$ là một biểu diễn tuyến tính của đại số Lie phức $\mathfrak{g}_{\mathbf{C}}$ trên một không gian vectơ phức hữu hạn chiều V. Tồn tại một biểu diễn $\tau$ của G trên V sao cho $L(\tau )_{(\mathbf{C})}=\varphi$ khi và chỉ khi $\varphi$ là nửa đơn và các trọng số của $\mathfrak{t}_{\mathbf{C}}$ trên V thuộc $\delta (X(T))$.

Nếu tồn tại một biểu diễn $\tau$ của G sao cho $L(\tau )_{(\mathbf{C})}=\varphi$, thì $\varphi$ là nửa đơn vì G liên thông và $\tau$ là nửa đơn (Chap. III, §6, no. 5, Hệ quả 2 của Mệnh đề 13), và các trọng số của $\mathfrak{t}_{\mathbf{C}}$ trên V thuộc ảnh của $\delta$. Do đó, điều kiện là cần thiết; ta sẽ chứng minh rằng nó là đủ. Nếu $\varphi$ là nửa đơn, V là tổng trực tiếp của các $V_\mu(\mathfrak{t}_{\mathbf{C}})$, trong đó $\mu$ thuộc tập hợp các trọng số của $\mathfrak{t}_{\mathbf{C}}$ trên V (Chap. VII, §2, no. 4, Hệ quả 3 của Định lý 2); nếu tất cả các trọng số thuộc ảnh của $\delta$, thì tồn tại một biểu diễn $\tau_T$ của T trên V sao cho $L(\tau_T)_{(\mathbf{C})}=\varphi |\mathfrak{t}_{\mathbf{C}}:$ thực vậy, chỉ cần đặt $\tau_T(t)v=t^{\lambda}v$ với $t\in T$ và $v\in V_{\delta(\lambda)}(\mathfrak{t}_{\mathbf{C}})$. Bổ đề được suy ra từ Mệnh đề 8 của §2, no. 6.

#### Định lý 1 {#lie-ix-s7-thm-1 .statement tag=01G1}

a) Cho $\tau : G\rightarrow \mathbf{G}\mathbf{L}(V)$ là một biểu diễn bất khả quy của G. Khi đó tập hợp các trọng số của $\tau$ (tương đối với T) có một phần tử lớn nhất $\lambda$, là trội, và không gian $V_{\lambda}(T)$ có chiều 1.

b) Hai biểu diễn bất khả quy của G là tương đương khi và chỉ khi các trọng số cao nhất của chúng bằng nhau.

c) Với mọi phần tử trội $\lambda$ của X(T), tồn tại một biểu diễn bất khả quy của G có trọng số cao nhất $\lambda$.

Theo Bổ đề 2, các lớp tương đương của các biểu diễn bất khả quy của G tương ứng song ánh với các lớp của các biểu diễn bất khả quy hữu hạn chiều của $\mathfrak{g}$ có các trọng số thuộc $\delta (X(T))$.

Ký hiệu $\mathscr{C}\mathfrak{g}_{\mathbf{C}}$ là tâm và $\mathscr{D}\mathfrak{g}_{\mathbf{C}}$ là đại số Lie dẫn xuất của $\mathfrak{g}_{\mathbf{C}}$, sao cho $\mathfrak{g}_{\mathbf{C}}=\mathscr{C}\mathfrak{g}_{\mathbf{C}}\oplus \mathscr{D}\mathfrak{g}_{\mathbf{C}}$. Với mọi dạng song tuyến tính $\mu$ trên $\mathfrak{t}_{\mathbf{C}}\cap \mathscr{D}\mathfrak{g}_{\mathbf{C}}$, ký hiệu $E(\mu)$ là môđun $\mathscr{D}\mathfrak{g}_{\mathbf{C}}$ đơn được đưa vào trong Chap. VIII, §6, no. 3; với mọi dạng tuyến tính $\nu$ trên $\mathscr{C}\mathfrak{g}_{\mathbf{C}}$, ký hiệu $\mathbf{C}(\nu )$ là môđun $\mathscr{C}\mathfrak{g}_{\mathbf{C}}$ chiều 1 trên $\mathbf{C}$ liên kết với nó. Khi đó các môđun $\mathfrak{g}_{\mathbf{C}}$ $\mathbf{C}(\nu )\otimes E(\mu)$ là đơn, và theo Chap. VIII, §7, no. 2, Hệ quả 2 của Định lý 1 và Algebra, Chap. VIII, §11, no. 1, Định lý 1, mọi môđun $\mathfrak{g}_{\mathbf{C}}$ đơn hữu hạn chiều đều đẳng cấu với một trong các môđun $\mathbf{C}(\nu )\otimes E(\mu)$; hơn nữa (loc. cit.)$\mathbf{C}(\nu )\otimes E(\mu)$ là hữu hạn chiều khi và chỉ khi $\mu(H_{\alpha})$ là một số nguyên dương với mọi nghiệm đơn $\alpha$. Nếu ta ký hiệu $\nu +\mu$ là dạng tuyến tính trên $\mathfrak{t}_{\mathbf{C}}$ cảm sinh $\nu$ trên $\mathscr{C}\mathfrak{g}_{\mathbf{C}}$ và $\mu$ trên $\mathfrak{t}_{\mathbf{C}}\cap \mathscr{D}\mathfrak{g}_{\mathbf{C}}$, thì $(\nu +\mu)(H_{\alpha}) =\mu(H_{\alpha})$; hơn nữa, các trọng số của $\mathbf{C}(\nu )\otimes E(\mu)$ là các $\nu +\lambda$, trong đó $\lambda$ là một trọng số bất kỳ của $E(\mu)$, và do đó có dạng $\nu +\mu-\theta$, với $\theta \in \delta (X_+)$ (Chap. VIII, §6, no. 2, Bổ đề 2).

Ta kết luận rằng môđun $\mathfrak{g}$-môđun $\mathbf{C}(\nu )\otimes E(\mu)$ là hữu hạn chiều khi và chỉ khi $(\nu +\mu)(H_{\alpha})$ là một số nguyên dương với mọi nghiệm đơn $\alpha$, và các trọng số của nó thuộc $\delta (X(T))$ khi và chỉ khi $\nu +\mu$ thuộc $\delta (X(T))$. Phép hội của hai điều kiện này có nghĩa là $\nu +\mu$ thuộc $\delta (X_{++})$; trong trường hợp đó, $\nu +\mu$ là trọng số cao nhất của $\mathbf{C}(\nu )\otimes E(\mu)$. Như vậy, ta đã xây dựng với mỗi trọng số trội $\lambda$ của X(T) một biểu diễn bất khả quy của G có trọng số cao nhất $\lambda$, và do đó đã thu được, sai khác một tương đương, tất cả các biểu diễn bất khả quy của G. Vì các vectơ có trọng số $\nu +\mu$ trong $\mathbf{C}(\nu )\otimes E(\mu)$ tạo thành một không gian con có chiều 1, nên chứng minh đầy đủ.

#### Hệ quả {#lie-ix-s7-n2-cor-1 .statement tag=01G2}

Nhóm G có một biểu diễn tuyến tính trung thành (hữu hạn chiều).

Trước hết hãy nhận xét rằng mọi phần tử của X(T) đều bằng hiệu của hai trọng số trội: chính xác hơn, hãy lấy $\varpi$ là một phần tử của $X_{++}$ sao cho $\langle \varpi , K_{\alpha}\rangle >0$ với mọi nghiệm đơn $\alpha$; với mọi $\lambda \in X(T)$ tồn tại một số nguyên dương $n$ sao cho $\langle \lambda +n\varpi , K_{\alpha}\rangle  \geq 0$ với mọi nghiệm đơn $\alpha$, nghĩa là (no. 1, Bổ đề $1$)$\lambda +n\varpi \in X_{++}$.

Do đó, tồn tại một họ hữu hạn $(\lambda_i)_{i\in I}$ các phần tử của $X_{++}$ sinh môđun $\mathbf{Z}$-môđun X(T). Với $i\in I$, cho $\tau_i$ là một biểu diễn bất khả quy của G có trọng số cao nhất $\lambda_i$ (Định lý 1); gọi biểu diễn $\tau$ là tổng trực tiếp của các $\tau_i$. Theo phép dựng, tập hợp $P(\tau ,T)$ các trọng số của $\tau$ (đối với T) sinh môđun $\mathbf{Z}$-môđun X(T). Bây giờ, từ Mệnh đề 6 của §4, no. 3 suy ra rằng đồng cấu $\tau$ là đơn ánh, do đó là hệ quả.

#### Nhận xét 1 {#lie-ix-s7-n2-rem-1 .statement tag=01G3}

Cho $\mathfrak{n}_+$ là đại số con của $\mathfrak{g}_{\mathbf{C}}$ là tổng của các $\mathfrak{g}^{\alpha}$ với $\alpha  >0$. Cho $\tau : G\rightarrow \mathbf{G}\mathbf{L}(V)$ là một biểu diễn bất khả quy, $\lambda \in X_{++}$ là trọng số cao nhất của nó và $\tau ':\mathfrak{g}_{\mathbf{C}}\rightarrow \mathfrak{g}\mathfrak{l}(V)$ là biểu diễn cảm sinh bởi $\tau$. Khi đó $V_{\lambda}(T)$ là không gian con gồm các vectơ $v$ trong V sao cho $\tau '(x)v= 0$ với mọi $x\in \mathfrak{n}_+$.

Thật vậy, điều này suy ra từ mệnh đề tương ứng đối với các $\mathfrak{g}_{\mathbf{C}}$-môđun $\mathbf{C}(\nu )\otimes E(\mu)$ (Chương VIII, §6, no. 2, Mệnh đề 3).

#### Nhận xét 2 {#lie-ix-s7-n2-rem-2 .statement tag=01G4}

Cho $\Theta (G)$ là đại số các hàm đại diện liên tục trên G với các giá trị trong $\mathbf{C}($Đại số, Chương VIII). Cho G tác động trên $\Theta (G)$ bằng các phép tịnh tiến trái và phải. Với mỗi $\lambda \in X_{++}$, cho $(V_{\lambda}, \tau_{\lambda})$ là một biểu diễn bất khả quy của G có trọng số cao nhất $\lambda$ (Định lý 1), và $(V^*_{\lambda},\check{\tau}_{\lambda})$ là biểu diễn đối ngẫu (Chương III, §3, no. 11); theo Các lý thuyết phổ, biểu diễn của $G\times G$ trên $\Theta (G)$ là đẳng cấu với tổng trực tiếp của các biểu diễn $(V_{\lambda}\otimes V^*_{\lambda}, \tau_{\lambda}\otimes \check{\tau}_{\lambda})$ với mọi $\lambda$ trong $X_{++}$. Nhận xét 1 bây giờ kéo theo mệnh đề sau: Cho $\lambda \in X_{++}$, và cho $E_{\lambda}$ là không gian con vectơ của $\Theta (G)$ gồm các hàm đại diện liên tục $f$ trên G sao cho $f(gt) =\lambda (t)^{-1}f(g)$ với mọi $g\in G$ và mọi $t\in T$, và sao cho $f*x= 0$ với mọi $x\in \mathfrak{n}_-=\bigoplus_{\alpha <0}\mathfrak{g}^{\alpha}$.

Khi đó $E_{\lambda}$ ổn định đối với các phép tịnh tiến trái, và biểu diễn của G trên $E_{\lambda}$ bởi các phép tịnh tiến trái là bất khả quy có trọng số cao nhất $\lambda$.

#### Nhận xét 3 {#lie-ix-s7-n2-rem-3 .statement tag=01G5}

Cho $\tau : G\rightarrow \mathbf{G}\mathbf{L}(V)$ là một biểu diễn bất khả quy. Tồn tại một phần tử $\nu$ của X(C(G)) sao cho $\tau (s)v=\nu (s)v$ với mọi $s\in C(G), v\in V:$ thật vậy, $\tau (C(G))$ được chứa trong hoán tập của $\tau$(G), là $\mathbf{C}^*.1_V($Algebra, Chap. VIII, §3, no. 2, Th. 1). Với mọi trọng số $\lambda$ của $\tau$, hạn chế của $\lambda$ trên C(G) bằng $\nu$.

#### Nhận xét 4 {#lie-ix-s7-n2-rem-4 .statement tag=01G6}

Các định nghĩa và các mệnh đề của Chap. VIII, §7, nos. 2 đến 5 có thể được tổng quát hóa không khó khăn cho tình huống hiện tại; ta để các chi tiết cho người đọc.

#### Mệnh đề 1 {#lie-ix-s7-prop-1 .statement tag=01G7}

Cho $\tau : G\rightarrow \mathbf{G}\mathbf{L}(V)$ là một biểu diễn bất khả quy của G có trọng số cao nhất $\lambda \in X_{++}$. Gọi $m$ là số nguyên $\sum_{\alpha\in R_+}\langle \lambda , K_{\alpha}\rangle$, và gọi $w_0$

là phần tử của nhóm Weyl sao cho $w_0(R_+) = R_-$ (Chap. VI, § 6, Hệ quả 3 của Mệnh đề 17). Có ba trường hợp có thể xảy ra:

a$)w_0(\lambda ) =-\lambda$ và $m$ là chẵn. Khi đó tồn tại một dạng song tuyến tính đối xứng tách được bất biến bởi G trên V; biểu diễn $\tau$ có kiểu thực (Phụ lục II).

b$)w_0(\lambda )\not=-\lambda$. Mọi dạng song tuyến tính bất biến bởi G trên V đều bằng không; biểu diễn $\tau$ có kiểu phức (loc. cit.).

c$)w_0(\lambda ) =-\lambda$ và $m$ là lẻ. Khi đó tồn tại một dạng song tuyến tính phản xứng tách được bất biến bởi G trên V; biểu diễn $\tau$ có kiểu quaternion (loc. cit.).

Nếu hạn chế của $\tau$ trên $C(G)_0$ không tầm thường, ta ở trường hợp b).

Một dạng song tuyến tính B trên V là bất biến dưới G khi và chỉ khi nó bất biến dưới $\mathfrak{g}_{\mathbf{C}}$ (Chap. III, §6, no. 5, Hệ quả 3). Vì vậy, nếu G là nửa đơn, mệnh đề suy ra từ Chap. VIII, §7, no. 5, Mệnh đề 12 và Mệnh đề 3 của Phụ lục II.

Trong trường hợp tổng quát, đặt $C(G)_0= S$, và đồng nhất $X(T/S)$ với một nhóm con của X(T) (ổn định dưới W). Nếu $\tau (S) =\{1_V\},\tau$ cảm sinh qua phép đi qua thương một biểu diễn $\tau ': G/S\rightarrow \mathbf{G}\mathbf{L}(V)$ có trọng số cao nhất $\lambda$; trong trường hợp này mệnh đề suy ra từ điều trước, áp dụng cho $G/S$.

Giả sử rằng $\tau (S)\not=\{1_V\}$. Tồn tại một phần tử khác không $\nu$ của X(S) sao cho $\tau (s) =\nu (s)_V$ với mọi $s\in S$ (Nhận xét 3). Khi đó $\nu$ là ảnh của $\lambda$ qua đồng cấu hạn chế $X(T)\rightarrow X(S)$; vì W tác động tầm thường trên X(S), đẳng thức $w_0(\lambda ) =-\lambda$ kéo theo rằng $\nu =-\nu$, điều này là không thể: do đó $w_0(\lambda )\not=-\lambda$. Mặt khác, nếu B là một dạng song tuyến tính bất biến bởi G trên V, ta có, với mọi $x, y$ trong V và $s$ trong S,

$$
B(\nu (s)x, \nu (s)y) = B(x, y) =\nu (s)^2B(x, y)
$$

điều này suy ra rằng B = 0, do đó mệnh đề được chứng minh.

Gọi $\mathfrak{S}_{\mathbf{R}}(G)$ là tập hợp các lớp của các biểu diễn liên tục bất khả quy của G trên các không gian vectơ thực hữu hạn chiều. Mệnh đề 1 và các kết quả của Phụ lục II cho một song ánh $\Phi : X_{++}/\Sigma \rightarrow \mathfrak{S}_{\mathbf{R}}$(G), trong đó $\Sigma$ ký hiệu nhóm con $\{1,-w_0\}$ của Aut(X(T)). Chính xác hơn, cho $\lambda \in X_{++}$, và gọi $E_{\lambda}$ là một biểu diễn của G có trọng số cao nhất $\lambda$; khi đó

$\Phi (\{\lambda ,-w_0(\lambda )\}) = E_{\lambda[\mathbf{R}]}$ nếu $\lambda \not=-w_0(\lambda )$ hoặc nếu $\sum_{\alpha\in R_+}\langle \lambda , K_{\alpha}\rangle \notin2\mathbf{Z}$

$\Phi (\{\lambda ,-w_0(\lambda )\}) = E'_{\lambda}$ nếu $\lambda =-w_0(\lambda )$ và $\sum_{\alpha\in R_+}\langle \lambda , K_{\alpha}\rangle  \in 2\mathbf{Z}$

trong đó $E'_{\lambda}$ là một $\mathbf{R}$-cấu trúc trên $E_{\lambda}$ bất biến dưới tác động của G.

### 3. VÀNH R(G)

Cho R(G) là vành các biểu diễn (liên tục, trên các không gian vectơ phức hữu hạn chiều) của G (Đại số, Chương VIII, §10, no. 6). Nếu $\tau$ là một biểu diễn của G, ký hiệu $[\tau ]$ là lớp của nó trong R(G); nếu $\tau$ và $\tau '$ là hai biểu diễn của G, theo định nghĩa ta có,

$$
[\tau ] + [\tau '] = [\tau \oplus \tau ']
$$

$$
[\tau ][\tau '] = [\tau \otimes \tau ']
$$

Vì mọi biểu diễn của G đều nửa đơn, môđun $\mathbf{Z}$ R(G) là tự do và nhận tập các lớp của các biểu diễn bất khả quy của G làm cơ sở, một tập có thể đồng nhất với $X_{++}$ theo Định lý 1. Ánh xạ $\tau  \rightarrow L(\tau )_{(\mathbf{C})}$ cảm sinh một đồng cấu $l$ từ vành R(G) đến vành $\mathscr{R}(\mathfrak{g}_{\mathbf{C}})$ các biểu diễn của $\mathfrak{g}_{\mathbf{C}}$ (Chương VIII, §7, no. 6).

Cho $\tau : G\rightarrow \mathbf{G}\mathbf{L}(V)$ là một biểu diễn của G; ta xét sự phân bậc $(V_{\lambda}(T))_{\lambda\in X(T)}$ của không gian vectơ trên $\mathbf{C}$ V. Ký hiệu Ch(V), hoặc Ch($\tau$ ), là đặc trưng của không gian vectơ phân bậc V (Chương VIII, §7, no. 7); nếu $(e^{\lambda})_{\lambda\in X(T)}$ ký hiệu cơ sở chính tắc của đại số $\mathbf{Z}[X(T)] =\mathbf{Z}^{(X(T))}$, ta có, theo định nghĩa,

Ch($\tau$ ) $=\sum_{\lambda\in X(T)}$(dim $V_{\lambda}(T)$)$e^{\lambda}$.

Theo cách tương tự (loc. cit.) ta định nghĩa một đồng cấu vành, cũng ký hiệu Ch, từ R(G) đến $\mathbf{Z}[X(T)]$. Nếu G nửa đơn, ta có một biểu đồ giao hoán

R(G) $\longrightarrow^{Ch}\mathbf{Z}[X(T)]$

$$
_{l\widetilde{\delta}} \tag{1}
$$

$$
\mathscr{R}(\mathfrak{g}_{\mathbf{C}})\longrightarrow^{ch}\mathbf{Z}[P]
$$

trong đó P ký hiệu nhóm các trọng số của $R(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}})$ và $\widetilde{\delta}$ là đồng cấu cảm sinh bởi $\delta$.

Nhóm Weyl W tác động bằng các tự đẳng cấu lên nhóm X(T), và do đó lên vành $\mathbf{Z}[X(T)]$. Theo Mệnh đề 5 của §4, no. 3, ảnh của Ch chứa trong vành con $\mathbf{Z}[X(T)]^W$ gồm các phần tử bất biến dưới W.

#### Mệnh đề 2 {#lie-ix-s7-prop-2 .statement tag=01G8}

Đồng cấu Ch cảm sinh một đẳng cấu từ R(G) đến $Z[X(T)]^W$.

Với $\lambda \in X_{++}$, ký hiệu $[\lambda ]$ là lớp trong R(G) của biểu diễn bất khả quy có trọng số cao nhất $\lambda$. Vì họ $([\lambda ])_{\lambda\in X_{++}}$ là một cơ sở của môđun $\mathbf{Z}$ R(G), chỉ cần chứng minh mệnh đề sau:

Họ (Ch[$\lambda ]$)$_{\lambda\in X_{++}}$ là một cơ sở của môđun $\mathbf{Z}[X(T)]^W$.

Với mỗi phần tử $u=\sum_{\lambda}a_{\lambda}e^{\lambda}$ của $\mathbf{Z}[X(T)]$, một số hạng $a_{\lambda}e^{\lambda}$ trong $u$ được gọi là cực đại nếu $\lambda$ là một phần tử cực đại của tập các $\mu\in X(T)$ sao cho $a_\mu\not= 0$. Định lý 1 suy ra rằng Ch[$\lambda ]$ có một số hạng cực đại duy nhất, cụ thể là $e^{\lambda}$. Do đó, mệnh đề suy ra từ bổ đề sau.

#### Bổ đề 3 {#lie-ix-s7-lem-3 .statement tag=01G9}

Với mỗi $\lambda \in X_{++}$, cho $C_{\lambda}$ là một phần tử của $\mathbf{Z}[X(T)]^W$ có số hạng cực đại duy nhất $e^{\lambda}$. Khi đó họ $(C_{\lambda})_{\lambda\in X_{++}}$ là một cơ sở của $\mathbf{Z}[X(T)]^W$.

Chứng minh này giống hệt chứng minh của Mệnh đề 3 của Chương VI, §3, no. 4, bằng cách thay A bởi $\mathbf{Z}, P$ bởi X(T) và $P\cap \overline{C}$ bởi $X_{++}$.

Gọi $\Theta (G)$ (tương ứng $\Theta (T)$) là đại số $\mathbf{C}$ của các hàm đại diện liên tục trên G (tương ứng T), và gọi $Z\Theta (G)$ (tương ứng $\Theta (T)^W$) là đại số con gồm các hàm trung tâm (tương ứng W-bất biến). Ánh xạ hạn chế $\Theta (G)\rightarrow \Theta (T)$ cảm sinh một đồng cấu của các vành $r: Z\Theta (G)\rightarrow \Theta (T)^W$. Mặt khác, ánh xạ gán cho một biểu diễn $\tau$ đặc trưng của nó (nghĩa là, hàm $g \rightarrow$ Tr $\tau (g)$) mở rộng thành một đồng cấu của các đại số $\mathbf{C}$ Tr$:\mathbf{C}\otimes_{\mathbf{Z}}R(G)\rightarrow Z\Theta (G)$ mà, theo Spectral Theories, là một đẳng cấu. Tương tự, đơn ánh chính tắc $X(T)\rightarrow \Theta (T)$ cảm sinh một đẳng cấu của các đại số $\mathbf{C}$ $\iota :\mathbf{C}[X(T)]\rightarrow \Theta$(T), đẳng cấu này cảm sinh một đẳng cấu $\iota :\mathbf{C}[X(T)]^W\rightarrow \Theta (T)^W$. Biểu đồ

$$
\mathbf{C}\otimes_{\mathbf{Z}}R(G)\overset{1\otimes Ch}{\longrightarrow}\mathbf{C}[X(T)]^W
$$

$$
_{Tr}^{\iota} \tag{2}
$$

$$
Z\Theta (G)\longrightarrow^r\Theta (T)^W
$$

là giao hoán: thật vậy, với mọi biểu diễn $\tau : G\rightarrow \mathbf{G}\mathbf{L}(V)$ và mọi $t\in T$,

Tr $\tau (t) =\sum_{\lambda\in X(T)}$(dim $V_{\lambda}(T)$)$\lambda (t) =\iota$(Ch$\tau$ )$(t)$,

nghĩa là, $(r\circ$ Tr)[$\tau ] = (\iota \circ$ Ch)[$\tau ]$.

Bây giờ ta có thể suy ra từ mệnh đề kết quả sau.

#### Hệ quả {#lie-ix-s7-n3-cor-1 .statement tag=01GA}

Ánh xạ hạn chế $r: Z\Theta (G)\rightarrow \Theta (T)^W$ là song ánh.

### 4. CÔNG THỨC ĐẶC TRƯNG

Trong số này, ta viết nhóm X(T) theo phép nhân, và xem các phần tử của nó như các hàm nhận giá trị phức trên T. Ta giả sử rằng phần tử $\rho$ của $X(T)\otimes \mathbf{Q}$ thuộc về X(T).

Ký hiệu $L^2(T)$ là không gian Hilbert của các lớp các hàm phức khả tích bình phương trên T, và $\Theta (T)$ là không gian con gồm các hàm đại diện liên tục. Theo Spectral Theories, X(T) là một cơ sở trực chuẩn của $L^2(T)$ và là một cơ sở đại số của $\Theta (T)$.

Với $f\in L^2(T)$ và $w\in W$, ký hiệu $^wf$ là phần tử của $L^2(T)$ được xác định bởi $^wf(t) =f(w^{-1}(t))$; do đó, với $\lambda \in X(T)$ ta có $^w\lambda =w(\lambda )$. Ký hiệu $\varepsilon : W\rightarrow  \{1,-1\}$ là dấu (đồng cấu duy nhất sao cho $\varepsilon (s) =$ $-1$ với mọi phản xạ $s$); với $f\in L^2$(T), đặt

$$
J(f) =\sum_{w\in W}\varepsilon (w)^wf
$$

Nếu $\lambda \in X_{++}$, các đặc trưng $^w(\lambda \rho )$ là phân biệt; thật vậy, chỉ cần chứng minh rằng $^w(\lambda \rho )\not=\lambda \rho$ với mọi $w\not= 1$; nhưng điều này suy ra từ Bổ đề 1 (no. 1) và sự kiện rằng $\langle \lambda \rho , K_{\alpha}\rangle =\langle \lambda , K_{\alpha}\rangle + 1>0$ với mọi nghiệm dương $\alpha$. Do đó,

$\|J(\lambda \rho )\|^2=$ Card(W) $=w(G)$.

Một phần tử $f\in L^2(T)$ được gọi là phản bất biến nếu $^wf=\varepsilon (w)f$ với mọi $w\in W$ (nghĩa là, nếu $^sf=-f$ với mọi phép phản xạ $s$). Ta sẽ chứng minh rằng $\frac{1}{w(G)}J$ là phép chiếu trực giao của $L^2(T)$ lên không gian con gồm các phần tử phản bất biến. Thật vậy, cho $f, f'$ thuộc $L^2$(T), với $f'$ phản bất biến; khi đó $J(f)$ là phản bất biến và

$$
\langle f',J(f)\rangle =\sum_{w\in W}\varepsilon (w)\langle f',^wf\rangle =\sum_{w\in W}\langle^wf',^wf\rangle
$$

$$
=\sum_{w\in W}\langle f', f\rangle =w(G)\langle f', f\rangle
$$

#### Mệnh đề 3 {#lie-ix-s7-prop-3 .statement tag=01GB}

Các phần tử $J(\lambda \rho )/\surd\overline{w(G)}$, với $\lambda \in X_{++}$, lập thành một cơ sở trực chuẩn của không gian con các phần tử phản bất biến của $L^2(T)$, và một cơ sở đại số của không gian con các phần tử phản bất biến của $\Theta (T)$.

Chứng minh giống hệt chứng minh của Chương VI, §3, no. 3, Mệnh đề 1.

Theo Chương VI, loc. cit., Mệnh đề 2,

$$
J(\rho ) =\rho \prod_{\alpha >0}(1-\alpha^{-1}) =\rho^{-1}\prod_{\alpha >0}(\alpha -1) \tag{3}
$$

nên

$$
J(\rho )J(\rho ) =\prod_{\alpha}(\alpha -1) \tag{4}
$$

Theo Hệ quả 2 của Định lý 1 (§6, no. 2), ta suy ra:

#### Bổ đề 4 {#lie-ix-s7-lem-4 .statement tag=01GC}

Nếu $\varphi$ và $\psi$ là hai hàm trung tâm liên tục trên G,

$$
\int_G\overline{\varphi(g)}\psi (g)dg=\frac{1}{w(G)}\int_T\overline{(\varphi(t)J(\rho)(t))}.(\psi (t)J(\rho )(t))dt
$$

Với mọi $\lambda \in X_{++}$, ký hiệu $\chi_{\lambda}$ là đặc trưng của một biểu diễn bất khả quy của G có trọng số cao nhất $\lambda$.

#### Định lý 2 (H. Weyl) {#lie-ix-s7-thm-2 .statement tag=01GD}

Với mọi $\lambda \in X_{++}$, ta có $J(\rho ).\chi_{\lambda}|T = J(\lambda \rho )$.

Hàm $J(\rho ).\chi_{\lambda}|T$ là phản bất biến dưới W, và là một tổ hợp tuyến tính với các hệ số nguyên của các phần tử của X(T). Vì vậy, theo Chương VI, §3, no. 3, Mệnh đề 1, nó có thể được viết thành $\sum_\mu a_\mu J(\mu\rho )$, trong đó $\mu$ thuộc $X_{++}$, và các $a_\mu$ là các số nguyên, tất cả trừ hữu hạn số trong đó là không; vì $\int_G|\chi_{\lambda}(g)|^2dg= 1$

(Các lý thuyết phổ), suy ra từ Mệnh đề 3 và Bổ đề 4 rằng $\sum_\mu(a_\mu)^2= 1$; do đó, các $a_\mu$ đều bằng không, trừ một số phải bằng 1 hoặc $-1$. Nhưng hệ số của $\lambda$ trong $\chi_{\alpha}|T$ bằng 1 (Định lý 1), vậy hệ số của $\lambda \rho$ trong $J(\rho ).\chi_{\lambda}|T$ bằng 1 (Chương VI, §3, no. 3, Nhận xét 2), điều này kéo theo rằng $a_{\lambda \rho}= 1$, do đó định lý được chứng minh.

#### Hệ quả 1 {#lie-ix-s7-thm-2-cor-1 .statement tag=01GE}

Với các ký hiệu của no. 3, ta có trong $\mathbf{Z}[X(T)]$,

$(\sum_{w\in W}\varepsilon (w)e^{w\rho})$ Ch[$\lambda ] =\sum_{w\in W}\varepsilon (w)e^{w\lambda}e^{w\rho}$ với mọi $\lambda \in X_{++}$.

Điều này suy ra từ định lý và biểu đồ giao hoán (2) (no. 3).

#### Hệ quả 2 {#lie-ix-s7-thm-2-cor-2 .statement tag=01GF}

Với mọi $\lambda \in X_{++}$ và mọi phần tử chính quy $t$ của T,

$$
\chi_{\lambda}(t) =\sum\sum^w\varepsilon_w(w\varepsilon )(\lambda w()wt\rho ()wt\rho ()wt) \tag{5}
$$

trong đó hai tổng được lấy theo các phần tử $w$ của W.

Thật vậy, $J(\rho )(t)$ khác không, vì $t$ là chính quy (công thức (4)).

Nếu $\varphi$ là một hàm trung tâm trên G, hạn chế của $\varphi$ lên T là bất biến dưới W, nên $J(\rho ).\varphi |T$ là phản bất biến dưới W. Hơn nữa, theo Các lý thuyết phổ và Định lý 1, họ $(\chi_{\lambda})_{\lambda\in X_{++}}$ là một cơ sở đại số của không gian các hàm đại diện trung tâm trên G và một cơ sở trực chuẩn của không gian ZL$^2(G)$ gồm các hàm trung tâm khả tích bình phương trên G.

Vậy, từ Mệnh đề 3 và Định lý 2 ta suy ra:

#### Hệ quả 3 {#lie-ix-s7-thm-2-cor-3 .statement tag=01GG}

Ánh xạ gán cho mỗi hàm trung tâm liên tục $\varphi$ trên G hàm $w(G)^{-1/2}J(\rho )(\varphi |T)$ gây ra một đẳng cấu từ không gian các hàm đại diện trung tâm trên G đến không gian các phần tử phản bất biến của $\Theta (T)$; nó mở rộng bởi tính liên tục thành một đẳng cấu của các không gian Hilbert từ ZL$^2(G)$ đến không gian con các phần tử phản bất biến của $L^2(T)$.

#### Hệ quả 4 {#lie-ix-s7-thm-2-cor-4 .statement tag=01GH}

Cho $\varphi$ là một hàm trung tâm liên tục trên G. Khi đó,

$$
\int_G\overline{\chi_{\lambda}(g)}\varphi (g)dg=\int_T\overline{\lambda(t)}\prod_{\alpha >0}(1-\alpha (t)^{-1})\varphi (t)dt=\int_T\overline{\lambda \rho(t)}.\varphi (t)J(\rho )(t)dt
$$

Thật vậy, theo Bổ đề 4 và Định lý 2,

$$
\int_G\overline{\chi_{\lambda}(g)}\varphi (g)dg=\frac{1}{w(G)}\int_T\chi_{\lambda}(t)J(\rho )(t)(\varphi (t)J(\rho )(t))dt
$$

$$
=\frac{1}{w(G)}\int_T\overline{J(\lambda \rho)(t)}\varphi (t)J(\rho )(t)dt
$$

Nhưng hàm $t \rightarrow \varphi (t)J(\rho )(t)$ là phản bất biến và $\frac{1}{w(G)}J(\lambda \rho )$ là phép chiếu trực giao của $\lambda \rho$ lên không gian con các phần tử phản bất biến của $L^2$(T), do đó

$$
\frac{1}{w(G)}\int_T\overline{J(\lambda \rho)(t)}\varphi (t)J(\rho )(t)dt=\int_T\overline{\lambda \rho(t)}\varphi (t)J(\rho )(t)dt
$$

cuối cùng, theo công thức (3), ta có $\rho (t)J(\rho )(t) =\prod_{\alpha >0}(1-\alpha (t)^{-1})$, do đó có hệ quả.

#### Nhận xét 1 {#lie-ix-s7-n4-rem-1 .statement tag=01GI}

Với mọi $w\in W$, đặt $\rho_w=^w\rho /\rho$; khi đó

$$
\sum_w\varepsilon (w)\rho_w=\prod_{\alpha >0}(1-\alpha^{-1}) =\rho^{-2}\prod_{\alpha >0}(\alpha -1) \tag{6}
$$

Nếu $t$ là một phần tử chính quy của T, ta suy ra từ (5) rằng

$$
\chi_{\lambda}(t) =\sum\sum^w\varepsilon_w(w\varepsilon )(\overset{w}{w}\lambda )\rho (t_w)(\rho t^w)(t)=\sum\prod^w_{\alpha >}\varepsilon (_0w(1)\overset{w}{-}\lambda \alpha (t()t\rho )^{w-}(_1t)) \tag{7}
$$

Chú ý rằng $\rho_w$ là một tổ hợp tuyến tính của các nghiệm với các hệ số nguyên, và do đó thuộc X(T) ngay cả khi ta không giả thiết rằng $\rho \in X(T)$. Suy ra rằng công thức (7) đúng mà không cần giả thiết rằng $\rho \in X(T):$ thật vậy, để chứng minh điều này ta thay thế G bằng một phủ liên thông thích hợp, và khi đó được rút gọn về Hệ quả 2.

#### Nhận xét 2 {#lie-ix-s7-n4-rem-2 .statement tag=01GJ}

Tương tự, đẳng thức thứ nhất của Hệ quả 4 vẫn đúng mà không cần giả thiết rằng $\rho \in X(T)$.

#### Nhận xét 3 {#lie-ix-s7-n4-rem-3 .statement tag=01GK}

Ta có thể suy ra Định lý 2 từ mệnh đề vi phân tương tự (Chương VIII, §9, no. 1, Định lý 1); điều tương tự cũng đúng đối với Định lý 3 của số tiếp theo (là tương tự của Định lý 2 của loc. cit., no. 2).

### 5. BẬC CỦA CÁC BIỂU DIỄN BẤT KHẢ QUY

Bây giờ ta quay lại ký hiệu cộng tính cho nhóm X(T) và ta không còn giả thiết rằng $\rho$ thuộc X(T).

#### Định lý 3 {#lie-ix-s7-thm-3 .statement tag=01GL}

Chiều của không gian của một biểu diễn bất khả quy của G có trọng số cao nhất $\lambda$ được cho bởi

$$
\chi_{\lambda}(e) =\prod_{\alpha\in R_+}\frac{\langle\lambda + \rho , K_{\alpha}\rangle}{\langle\rho , K_{\alpha}\rangle}
$$

Đặt $\gamma =\frac{1}{2}\sum_{\alpha >0}K_{\alpha}$, sao cho $\delta (\alpha )(\gamma ) = 2\pi i$ với mọi nghiệm đơn $\alpha$ (Chương VI, §1, no. 10, Mệnh đề 29). Đường thẳng $\mathbf{R}\gamma$ không được chứa trong bất kỳ siêu phẳng nào Ker $\delta (\alpha )$, nên exp($z\gamma$ ) là một phần tử chính quy của G với mọi $z\in \mathbf{R}^*$ đủ nhỏ; với mọi $\mu\in X(T)$ và mọi $z\in \mathbf{R}$, ta có

$J(\mu$)(exp($z\gamma$ )) $=\sum_{w\in W}\varepsilon (w)e^{z\delta(\mu)(w^{-1}\gamma)}$.

Ta tạm thời chấp nhận bổ đề sau:

#### Bổ đề 5 {#lie-ix-s7-lem-5 .statement tag=01GM}

Ta có

$J(\mu$)(exp($z\gamma$ )) $=e^{z\delta(\mu)(\gamma)}\prod_{\alpha >0}(1-e^{-z\delta(\mu)(K_{\alpha})})$.

Do đó, hàm $J(\mu$)(exp($z\gamma$ )) là tích của một hàm tiến tới 1 khi $z$ tiến tới 0 và của

$$
z^N\prod_{\alpha >0}\delta (\mu)(K_{\alpha}) = (2\pi iz)^N\prod_{\alpha >0}\langle \mu, K_{\alpha}\rangle
$$

trong đó N = Card $R_+$.

Trước hết giả sử rằng $\rho \in X(T)$; áp dụng Hệ quả 2 của Định lý 2 ta thấy rằng, khi $z$ tiến tới $0,\chi_{\lambda}(z\gamma )$ tiến tới

$$
\prod_{\alpha >0}\langle \lambda +\rho , K_{\alpha}\rangle /\prod_{\alpha >0}\langle \rho , K_{\alpha}\rangle
$$

do đó định lý đúng trong trường hợp này.

Trong trường hợp tổng quát, chỉ cần chú ý rằng, khi chứng minh Định lý 3, ta luôn có thể thay thế G bằng một phủ liên thông thích hợp và do đó rút gọn về trường hợp trước.

Bây giờ ta chứng minh Bổ đề 5. Cho $z\in \mathbf{C}$; ký hiệu $\varphi_z$ là ánh xạ từ $\mathfrak{t}$ đến đại số $\mathbf{C}$-Map(X(T)$,\mathbf{C}$) của các ánh xạ từ X(T) đến $\mathbf{C}$, gán cho $H\in \mathfrak{t}$ ánh xạ

$\varphi_z(H) :\mu \rightarrow \mu$(exp $zH$) $=e^{z\delta(\mu)(H)}$.

Ta có $\varphi_z(H+H') =\varphi_z(H)\varphi_z(H')$, nên tồn tại một đồng cấu vành

$\psi_z:\mathbf{Z}[\mathfrak{t}]\rightarrow$ Map(X(T)$,\mathbf{C}$)

sao cho $\psi_z(e^H)(\mu) =e^{z\delta(\mu)(H)}$. Mặt khác, theo Chap. VI, §3, no. 3, Mệnh đề 2, ta có quan hệ sau trong $\mathbf{Z}[\mathfrak{t}]:$

$$
\sum_{w\in W}\varepsilon (w)e^{w\gamma}=e^{\gamma}\prod_{\alpha >0}(1-e^{-K_{\alpha}})
$$

Áp dụng đồng cấu $\psi_z$, và dùng đẳng thức

$$
\psi_z(e^{w\gamma})(\mu) =e^{z\delta(\mu)(w\gamma)}=e^{z\delta(w^{-1}\mu)(\gamma)}
$$

ta suy ra công thức đã nêu.

#### Hệ quả 1 {#lie-ix-s7-lem-5-cor-1 .statement tag=01GN}

Cho $\| \|$ là một chuẩn trên $X(T)\otimes \mathbf{R}$. Với mọi $\lambda \in X_{++}$, cho $d(\lambda )$ là chiều của không gian của một biểu diễn bất khả quy của G có trọng số cao nhất $\lambda$.

a) sup$_{\lambda\in X_{++}}d(\lambda )/\|\lambda +\rho \|^N<\infty$, trong đó $N = 1/$2(dim $G-$ dim T).

b) Nếu G là nửa đơn, inf$_{\lambda\in X_{++}}d(\lambda )/\|\lambda +\rho \|>0$.

$a)$ Với mọi $\alpha \in R_+$, tồn tại $A_{\alpha}>0$ sao cho $|\langle \lambda +\rho , K_{\alpha}\rangle | \leq A_{\alpha}\|\lambda +\rho \|$, do đó $d(\lambda )/\|\lambda +\rho \|^N\leq \prod_{\alpha >0}A_{\alpha}/\langle \rho , K_{\alpha}\rangle$.

$b)$ Giả sử G là nửa đơn, ký hiệu $\beta_1, . . . , \beta_r$ là các rễ đơn và đặt $N_i=K_{\beta_i}$. Khi đó

$$
d(\lambda )\geq \prod_{i=1}^r\frac{\langle\lambda + \rho , N_i\rangle}{\langle\rho , N_i\rangle}=\prod_{i=1}^r\langle \lambda +\rho , N_i\rangle
$$

vì $\langle \lambda +\rho , N_i\rangle  \geq  \langle \rho , N_i\rangle = 1$, điều này suy ra rằng

$d(\lambda )\geq$ sup$_i|\langle \lambda +\rho , N_i\rangle |$.

Nếu G là nửa đơn, $x \rightarrow$ sup$|\langle x, N_i\rangle |$ là một chuẩn trên $X(T)\otimes \mathbf{R}$, tất yếu tương đương với chuẩn đã cho, nên b).

#### Hệ quả 2 {#lie-ix-s7-lem-5-cor-2 .statement tag=01GO}

Giả sử G là nửa đơn; cho $d$ là một số nguyên. Tập hợp các lớp biểu diễn của G có chiều $\leq d$ là hữu hạn.

Hệ quả 1b) suy ra rằng tập hợp $X_d$ của các phần tử $\lambda$ của $X_{++}$ sao cho $d(\lambda )\leq d$ là hữu hạn. Với mọi $\lambda$ trong $X_d$, cho $V_{\lambda}$ là một biểu diễn bất khả quy có trọng số cao nhất $\lambda$; mọi biểu diễn có chiều $\leq d$ đều đẳng cấu với một tổng trực tiếp $\bigoplus_{\lambda\in X_d}V^{n_{\lambda}}_{\lambda}$, với $n_{\lambda}\leq d$, suy ra hệ quả.

### 6. CÁC PHẦN TỬ CASIMIR

Theo Mệnh đề 3 của §1, no. 3, tồn tại các dạng song tuyến tính đối xứng âm trên $\mathfrak{g}$, phân biệt và bất biến dưới Ad(G) (nếu G là nửa đơn, chẳng hạn, ta có thể lấy dạng Killing của $\mathfrak{g}$). Cho F là một dạng như vậy. Nhắc lại (Chap. I, §3, no. 7) rằng phần tử Casimir liên kết với F là phần tử $\Gamma$ của tâm của đại số bao $U(\mathfrak{g})$ sao cho, với bất kỳ cơ sở $(e_i)$ của $\mathfrak{g}$ thỏa mãn $F(e_i, e_j) =-\delta_{ij}$, ta có $\Gamma =-\sum e^2_i$.

Trong phần còn lại của chương này, ta sẽ gọi các phần tử Casimir của G là các phần tử của $U(\mathfrak{g})$ thu được theo cách này từ các dạng song tuyến tính đối xứng bất biến, phân biệt và âm trên $\mathfrak{g}$. Nếu $\Gamma$ là một phần tử Casimir của G và nếu $\tau : G\rightarrow \mathbf{G}\mathbf{L}(V)$ là một biểu diễn bất khả quy của G, thì tự đồng cấu $\Gamma_V$ của V là một phép vị tự (Algebra, Chap. VIII, §3, no. 2, Th. 1), mà tỉ số của nó sẽ được ký hiệu là $\widetilde{\Gamma}(\tau )$.

#### Mệnh đề 4 {#lie-ix-s7-prop-4 .statement tag=01GP}

Cho $\Gamma$ là một phần tử Casimir của G.

a) Nếu $\tau$ là một biểu diễn bất khả quy của G, thì $\widetilde{\Gamma}(\tau )$ là thực và dương. Nếu $\tau$ không phải là biểu diễn tầm thường, thì $\widetilde{\Gamma}(\tau )>0$.

b) Tồn tại một và chỉ một dạng toàn phương $Q_{\Gamma}$ trên $X(T)\otimes \mathbf{R}$ sao cho, với mọi biểu diễn bất khả quy $\tau$ của G,

$$
\widetilde{\Gamma}(\tau ) = Q_{\Gamma}(\lambda +\rho )-Q_{\Gamma}(\rho )
$$

trong đó $\lambda$ là trọng số cao nhất của $\tau$. Dạng $Q_{\Gamma}$ là dương, phân biệt và bất biến dưới W.

Cho F là một dạng song tuyến tính đối xứng âm phân biệt trên $\mathfrak{g}$ xác định $\Gamma$. Cho $\tau : G\rightarrow \mathbf{G}\mathbf{L}(V)$ là một biểu diễn bất khả quy của G; cho $\langle ,\rangle$ là một tích vô hướng Hilbert trên V bất biến dưới G (§1, no. 1), và $(e_i)$ là một cơ sở của $\mathfrak{g}$ sao cho $F(e_i, e_j) =-\delta_{ij}$. Khi đó, với mọi phần tử $v$ của V không bất biến dưới G, ta có

$$
\widetilde{\Gamma}(\tau )\langle v, v\rangle =\langle v, \Gamma_V(v)\rangle =-\sum_i\langle v,(e_i)^2_Vv\rangle =\sum_i\langle v,(e_i)^*_V(e_i)_Vv\rangle
$$

$$
=\sum_i\langle (e_i)_Vv,(e_i)_Vv\rangle >0
$$

suy ra a).

Cho B là dạng nghịch đảo trên $\mathfrak{t}^*_{\mathbf{C}}$ của phần hạn chế lên $\mathfrak{t}_{\mathbf{C}}$ của dạng song tuyến tính trên $\mathfrak{g}_{\mathbf{C}}$ cảm sinh bởi F nhờ mở rộng vô hướng. Theo Hệ quả của Mệnh đề 7 của Chap. VIII, §6, no. 4, ta có$^5\widetilde{\Gamma}(\tau ) = B(\delta (\lambda ), \delta (\lambda +2\rho ))$. Mở rộng $\delta : X(T)\rightarrow$ $\mathfrak{t}^*_{\mathbf{C}}$ thành một ánh xạ $\mathbf{R}$-tuyến tính từ $X(T)\otimes \mathbf{R}$ vào $\mathfrak{t}^*_{\mathbf{C}}$ và cho $Q_{\Gamma}$ là dạng toàn phương $x \rightarrow B(\delta (x), \delta (x))$ trên $X(T)\otimes \mathbf{R}$; nó là phân biệt và bất biến dưới W, và

$$
\widetilde{\Gamma}(\tau ) = B(\delta (\lambda +\rho ), \delta (\lambda +\rho ))-B(\delta (\rho ), \delta (\rho )) = Q_{\Gamma}(\lambda +\rho )-Q_{\Gamma}(\rho )
$$

Ta chứng minh rằng dạng $Q_{\Gamma}$ là dương. Thật vậy, nếu $x\in X(T)\otimes \mathbf{Q}$, thì phần tử $\delta (x)$ của $\mathfrak{t}^*_{\mathbf{C}}$ nhận các giá trị thuần ảo trên $\mathfrak{t}$, do đó nhận giá trị thực trên $i\mathfrak{t}$; ta kết luận bằng cách nhận xét rằng, với $y\in i\mathfrak{t}$, ta có $F(y, y)\geq 0$.

Còn phải chứng minh mệnh đề duy nhất trong b). Cho Q là một dạng toàn phương trên $X(T)\otimes \mathbf{R}$ thỏa mãn điều kiện yêu cầu, và cho $\Phi$ (resp. $\Phi_{\Gamma}$) là dạng song tuyến tính liên kết với Q (resp. $Q_{\Gamma}$). Với $\lambda , \mu\in X_{++}$, ta có

$$
\Phi (\lambda , \mu) = (Q(\lambda +\mu+\rho )-Q(\rho ))-(Q(\lambda +\rho )-Q(\rho ))-(Q(\mu+\rho )-Q(\rho ))
$$

$$
=\Phi_{\Gamma}(\lambda , \mu)
$$

Vì $X(T)_{++}$ sinh ra không gian vectơ $\mathbf{R}$-vector space $X(T)\otimes \mathbf{R}$, ta có $\Phi =\Phi_{\Gamma}$, do đó $Q = Q_{\Gamma}$.

#### Nhận xét {#lie-ix-s7-n6-rem-1 .statement tag=01GQ}

Cho $x\in \mathfrak{g}$. Tồn tại một số thực dương ngặt A sao cho, với mọi biểu diễn bất khả quy $\tau : G\rightarrow \mathbf{G}\mathbf{L}(V)$ và mọi cấu trúc Hilbert trên V bất biến dưới G,

$$
\|L(\tau )(x)\|^2\leq A.\widetilde{\Gamma}(\tau )
$$

Thật vậy, với các ký hiệu trong chứng minh trước, ta có thể chọn cơ sở $(e_i)$ của $\mathfrak{g}$ sao cho $x=ae_1,a\in \mathbf{R}$. Khi đó, với $v\in V$, ta có

$$
\langle x_Vv, x_Vv\rangle =|a|^2\langle e_1v, e_1v\rangle  \leq  |a|^2\widetilde{\Gamma}(\tau )\langle v, v\rangle
$$

### Bài tập {#lie-ix-s7-exercises}

Xem [các bài tập cho § 7](exercises/s7/).
