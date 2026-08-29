---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IX
chapter_title: COMPACT REAL LIE GROUPS
section: 1
section_title: Structure of compact groups
appendix: true
lang: vi
source: lie-vii-ix
book_pages: 381-385, 424-425
pdf_pages: 0388-0392, 0431-0432
extraction: native
subsections:
    - "no": 1
      title: EMBEDDING A COMPACT GROUP IN A PRODUCT OF LIE GROUPS
      page: 381
      pdf_page: 388
    - "no": 2
      title: PROJECTIVE LIMITS OF LIE GROUPS
      page: 382
      pdf_page: 389
    - "no": 3
      title: STRUCTURE OF CONNECTED COMPACT GROUPS
      page: 384
      pdf_page: 391
statements: 9
exercises: 1
content_sha256: 9f831e4ee0b6d9c2e4ca25f32ff6d6376b3be352906f1d21a84e77b43daa41c3
translated_from: content/en/lie/IX/A1_a1_structure_of_compact_groups.md
source_content_sha256: 5e7319fca99d12df0397567af8fdb7c23d7ffbc97775400d0463c84a608eb608
translation_model: gpt-5-6, gpt-5.4
translation_run: translate-vi-f121e56d
glossary_version: 34
glossary_terms_sha256: 31e827be535e44be3cb0779680adf0e5f0eba72f577b8f67d1e01326faad715a
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## PHỤ LỤC I

# CẤU TRÚC CỦA CÁC NHÓM COMPACT

### 1. NHÚNG MỘT NHÓM COMPACT VÀO MỘT TÍCH CÁC NHÓM LIE

#### Mệnh đề 1 {#lie-ix-a1-prop-1 .statement tag=01II}

Mọi nhóm tôpô compact G đều đẳng cấu với một nhóm con đóng của một tích các nhóm Lie compact.

Ký hiệu $\widehat{G}$ là tập hợp các lớp của các biểu diễn unita liên tục bất khả quy của G trên các không gian Hilbert phức hữu hạn chiều (Lý thuyết Phổ, đang chuẩn bị). Với mọi $u\in \widehat{G}$, gọi $Hu$ là không gian của $u$ và $\rho_u: G\rightarrow \mathbf{U}(H_u)$ là đồng cấu liên kết với $u$. Theo định lý Peter-Weyl (Lý thuyết Phổ, đang chuẩn bị), đồng cấu liên tục $\rho = (\rho_u)_{u\in\widehat{G}}$ từ G vào $\prod_{u\in\widehat{G}}\mathbf{U}(H_u)$ là đơn ánh; vì G compact, $\rho$ cảm sinh một đẳng cấu

từ G lên một nhóm con đóng của nhóm $\prod_{u\in\widehat{G}}\mathbf{U}(H_u)$.

#### Hệ quả 1 {#lie-ix-a1-prop-1-cor-1 .statement tag=01IJ}

Cho V là một lân cận của phần tử đơn vị của G. Khi đó V chứa một nhóm con chuẩn tắc đóng H của G sao cho thương $G/H$ là một nhóm Lie.

Cho $(K_{\lambda})_{\lambda\in L}$ là một họ các nhóm Lie compact sao cho G có thể được đồng nhất với một nhóm con đóng của $\prod_{\lambda\in L}K_{\lambda}$; với mỗi $\lambda \in L$, ký hiệu bởi $p_{\lambda}: G\rightarrow K_{\lambda}$ hạn chế lên G của phép chiếu chính tắc. Tồn tại một tập con hữu hạn $J\subset L$, và với mỗi $\lambda \in J$ một lân cận $V_{\lambda}$ của gốc trong $K_{\lambda}$, sao cho V chứa $\bigcap_{\lambda\in J}p^{-1}_{\lambda}(V_{\lambda})$. Khi đó chỉ cần đặt $H =\bigcap_{\lambda\in J}$ Ker($p_{\lambda}$).

Ký hiệu bởi $(H_{\alpha})_{\alpha\in I}$ họ lọc giảm các nhóm con chuẩn tắc đóng của G, sao cho thương $G/H_{\alpha}$ là một nhóm Lie. Xét hệ xạ ảnh các nhóm Lie compact $G/H_{\alpha}$ (x. Tôpô đại cương, Chương III, §7, no. 2, Mệnh đề 2).

#### Hệ quả 2 {#lie-ix-a1-prop-1-cor-2 .statement tag=01IK}

Ánh xạ chính tắc $G\rightarrow$ lim$_{_{\leftarrow -}}G/H_{\alpha}$ là một đẳng cấu của các nhóm tôpô. $\alpha$

Thật vậy, Hệ quả 1 kéo theo rằng điều kiện (PA) của Topologie Générale, Chương III, §7, no. 2, được thỏa mãn; khi đó mệnh đề suy ra từ Mệnh đề 2 của tài liệu đã dẫn.

#### Hệ quả 3 {#lie-ix-a1-prop-1-cor-3 .statement tag=01IL}

G là một nhóm Lie khi và chỉ khi tồn tại một lân cận của phần tử đơn vị $e$ của G không chứa nhóm con chuẩn tắc nào khác $\{e\}$.

Sự cần thiết của điều kiện này đã được chứng minh (Chương III, §4, no. 2, Hệ quả 1 của Định lý 2), và tính đủ là một hệ quả ngay lập tức của Hệ quả 1.

### 2. GIỚI HẠN XẠ ẢNH CỦA CÁC NHÓM LIE

#### Bổ đề 1 {#lie-ix-a1-lem-1 .statement tag=01IM}

Cho $(G_{\alpha}, f_{\alpha \beta})$ là một hệ xạ ảnh các nhóm tôpô đối với một tập hợp chỉ số lọc I, và G là giới hạn của nó. Giả sử rằng các ánh xạ chính tắc $f_{\alpha}: G\rightarrow G_{\alpha}$ là toàn ánh.

a) Các nhóm con $D(G_{\alpha})$ (tương ứng $C(G_{\alpha})$, tương ứng $C(G_{\alpha})_0$) tạo thành một hệ xạ ảnh các tập hợp con của $G_{\alpha}$.

b) Ta có D(G) = lim$_{_{\leftarrow -}\alpha}\overline{D(G_{\alpha})}$ và C(G) = lim$_{_{\leftarrow -}\alpha}C(G_{\alpha})$.

c) Nếu $G_{\alpha}$ là compact với mọi $\alpha \in I$, thì $C(G)_0=$ lim$_{_{\leftarrow -}\alpha}C(G_{\alpha})_0$.

Cho $\alpha , \beta$ là hai phần tử của I, với $\alpha \leq \beta$. Khi đó $f_{\alpha \beta}(D(G_{\beta}))\subset D(G_{\alpha})$, và $f_{\alpha \beta}(C(G_{\beta}))\subset C(G_{\alpha})$ vì $f_{\alpha \beta}$ là toàn ánh; do $f_{\alpha \beta}$ liên tục, suy ra $f_{\alpha \beta}(\overline{D(G_{\beta})})\subset \overline{D(G_{\alpha})}$ và $f_{\alpha \beta}(C(G_{\beta})_0)\subset C(G_{\alpha})_0$, do đó a). Vì $f_{\alpha}$ là toàn ánh, $f_{\alpha}(D(G)) = D(G_{\alpha})$ (Đại số, Chương I, §6, no. 2, Mệnh đề 6), nên $\overline{D(G)}=$ lim$_{\leftarrow -}\overline{D(G_{\alpha})}$ (Tôpô đại cương, Chương I, §4, no. 4, Hệ quả của Mệnh đề 9). Tính toàn ánh của $f_{\alpha}$ cũng suy ra bao hàm $f_{\alpha}(C(G))\subset$ $C(G_{\alpha})$ và do đó $C(G)\subset$ lim$_{\leftarrow -}C(G_{\alpha})$; bao hàm đối là ngay lập tức. Sau cùng, mệnh đề c) suy ra từ b) và Tôpô đại cương, Chương III, §7, no. 2, Mệnh đề 4).

#### Bổ đề 2 {#lie-ix-a1-lem-2 .statement tag=01IN}

Cho $(S_a)_{a\in A},(T_b)_{b\in B}$ là hai họ hữu hạn các nhóm Lie gần đơn, đơn liên thông (Ch. III, § 9, no. 8, Định nghĩa 3)$,u:\prod_{a\in A}S_a\rightarrow \prod_{b\in B}T_b$ là một cấu xạ toàn ánh. Khi đó tồn tại một ánh xạ đơn ánh $l: B\rightarrow A$ và các đẳng cấu $u_b: S_{l(b)}\rightarrow T_b(b\in B)$ sao cho $u((s_a)_{a\in A}) = (u_b(s_{l(b)}))_{b\in B}$ với mọi phần tử $(s_a)_{a\in A}$ của $\prod_{a\in A}S_a$.

Ký hiệu $\mathfrak{s}_a$ (resp. $\mathfrak{t}_b$) là đại số Lie của $S_a$ (resp. $T_b$) với $a\in A$ (resp. $b\in B$), và xét đồng cấu $L(u) :\prod_{a\in A}\mathfrak{s}_a\rightarrow \prod_{b\in B}\mathfrak{t}_b$. Hạt nhân của nó

là một iđêan của đại số Lie nửa đơn $\prod_{a\in A}\mathfrak{s}_a$, và do đó có dạng $\prod_{a\in A''}\mathfrak{s}_a$, với $A''\subset A$ (Chương I, §6, no. 2, Hệ quả 1). Đặt $A'= A$**--** $A''$. Theo

hạn chế, $L(u)$ cảm sinh một đẳng cấu $f:\prod_{a\in A'}\mathfrak{s}_a\rightarrow \prod_{b\in B}\mathfrak{t}_b$. Theo loc. cit., với mọi $a\in A'$ iđêan $f(\mathfrak{s}_a)$ bằng một trong các $\mathfrak{t}_b$; do đó, tồn tại một song ánh $l: B\rightarrow A'$ sao cho $f(\mathfrak{s}_{l(b)}) =\mathfrak{t}_b$ với $b\in B$, và $f$ cảm sinh một đẳng cấu $f_b:\mathfrak{s}_{l(b)}\rightarrow \mathfrak{t}_b$. Vì các nhóm $S_a$ và $T_b$ là đơn liên thông, nên tồn tại các đẳng cấu $u_b: S_{l(b)}\rightarrow T_b$ sao cho $L(u_b) =f_b$ với $b\in B$ (Chap. III, §6, no. 3, Định lý 3).

Ký hiệu bởi $\widetilde{u}:\prod_{a\in A}S_a\rightarrow \prod_{b\in B}T_b$ cấu xạ được xác định bởi $\widetilde{u}((s_a)_{a\in A}) =$

$(u_b(s_{l(b)}))_{b\in B}$. Theo phép dựng, $L(\widetilde{u}) =f= L(u)$, nên $\widetilde{u}=u$, điều này chứng minh bổ đề.

#### Bổ đề 3 {#lie-ix-a1-lem-3 .statement tag=01IO}

Dưới các giả thiết của Bổ đề 1, giả sử rằng các $G_{\alpha}$ là các nhóm Lie compact đơn liên. Khi đó nhóm tôpô G đẳng cấu với tích của một họ các nhóm Lie compact gần đơn, đơn liên.

Với mọi $\alpha \in I$, nhóm $G_{\alpha}$ là tích trực tiếp của một họ hữu hạn các nhóm con gần đơn, đơn liên thông $(S^{\lambda}_{\alpha})_{\lambda\in L_{\alpha}}$ (Chương III, §9, no. 8, Mệnh đề 28). Cho $\beta \in I,\beta \geq \alpha$. Theo Bổ đề 2, tồn tại một ánh xạ $l_{\beta \alpha}: L_{\alpha}\rightarrow L_{\beta}$ sao cho $f_{\alpha \beta}(S^{l_{\beta \alpha}(\lambda)}_{\beta}) = S^{\lambda}_{\alpha}$ với $\lambda \in L_{\alpha}$. Ta có $l_{\gamma \beta}\circ l_{\beta \alpha}=l_{\gamma \alpha}$ với $\alpha \leq \beta \leq \gamma$, do đó $(L_{\alpha}, l_{\beta \alpha})$ là một hệ quy nạp các tập hợp đối với I. Gọi L là giới hạn của nó; do các ánh xạ $l_{\beta \alpha}$ là đơn ánh, $L_{\alpha}$ có thể được đồng nhất với một tập con của L, sao cho $L =\bigcup_{\alpha\in I}L_{\alpha}$.

Cho $\lambda \in L$. Đặt $S^{\lambda}_{\alpha}=\{1\}$ khi $\lambda  \notin L_{\alpha}$, và ký hiệu bởi $\varphi^{\lambda}_{\alpha \beta}: S^{\lambda}_{\beta}\rightarrow S^{\lambda}_{\alpha}$ cấu xạ cảm sinh bởi $f_{\alpha \beta}$; điều đó cho một hệ xạ ảnh các nhóm tôpô $(S^{\lambda}_{\alpha}, \varphi^{\lambda}_{\alpha \beta})$, mà giới hạn của nó đẳng cấu với $S_{\lambda}$. Đồng cấu chính tắc của các nhóm tôpô

lim$_{_{\leftarrow -\alpha\in I}}((\prod_{\lambda\in L}S^{\lambda}_{\alpha})\rightarrow \prod_{\lambda\in L}($lim$_{_{\alpha\leftarrow -\in I}}S^{\lambda}_{\alpha})$

là song ánh (Lý thuyết tập hợp, Chương III, §7, no. 3, Hệ quả 2); do đó nó là một đẳng cấu vì các nhóm đang xét là compact. Nhưng nhóm thứ nhất trong các nhóm ấy có thể được đồng nhất với G và nhóm thứ hai với tích của các $S_{\lambda}$, suy ra bổ đề.

### 3. CẤU TRÚC CỦA CÁC NHÓM COMPACT LIÊN THÔNG

Cho G là một nhóm compact giao hoán. Nhắc lại rằng (Lý thuyết phổ, Chương II, §1, no. 9, Mệnh đề 11) khi đó G đẳng cấu với nhóm tôpô đối ngẫu của một nhóm giao hoán rời rạc $\widehat{G}$. Nhóm G là liên thông khi và chỉ khi $\widehat{G}$ không xoắn (Lý thuyết phổ, Chương II, §2, no. 2, Hệ quả 1 của Mệnh đề 4).

Các tính chất sau là tương đương (Lý thuyết phổ, Chương II, §2, no. 2, Hệ quả 2 của Mệnh đề 4 và §1, no. 9, Hệ quả 2 của Mệnh đề 11):

(i) G là hoàn toàn gián đoạn;

(ii) $\widehat{G}$ là một nhóm xoắn;

(iii) nhóm tôpô G đẳng cấu với giới hạn của một hệ xạ ảnh các nhóm (giao hoán) hữu hạn, mỗi nhóm được trang bị tôpô rời rạc.

Mệnh đề dưới đây tổng quát hóa Hệ quả 1 của Mệnh đề 4 của §1, no. 4.

#### Mệnh đề 2 {#lie-ix-a1-prop-2 .statement tag=01IP}

Cho G là một nhóm compact liên thông.

a$) C(G)_0$ là một nhóm compact liên thông giao hoán; D(G) là một nhóm compact liên thông, bằng với nhóm dẫn xuất của nó.

b) Đồng cấu liên tục $(x, y) \rightarrow xy$ từ $C(G)_0\times D(G)$ đến G là toàn ánh và hạt nhân của nó là một nhóm con trung tâm của $C(G)_0\times D(G)$, nhóm con này compact và hoàn toàn không liên thông.

c) Tồn tại một họ $(S_{\lambda})_{\lambda\in L}$ các nhóm Lie compact gần đơn và một đồng cấu liên tục toàn ánh $\prod_{\lambda\in L}S_{\lambda}\rightarrow D(G)$, mà hạt nhân là một

nhóm con trung tâm compact, hoàn toàn không liên thông.

Cho $(G_{\alpha}, f_{\alpha \beta})$ là một hệ xạ ảnh các nhóm Lie compact, đối với một tập hợp lọc I, sao cho G đẳng cấu với lim$_{\leftarrow -}G_{\alpha}$ và sao cho các ánh xạ chính tắc $f_{\alpha}: G\rightarrow G_{\alpha}$ là toàn ánh (Hệ quả 2 của Mệnh đề 1). Với $\alpha \in I$, gọi $\pi_{\alpha}: \widetilde{D}(G_{\alpha})\rightarrow D(G_{\alpha})$ là một phủ phổ quát của nhóm $D(G_{\alpha})$. Các $f_{\alpha \beta}$ cảm sinh các cấu xạ $\widetilde{f}_{\alpha \beta}: \widetilde{D}(G_{\beta})\rightarrow \widetilde{D}(G_{\alpha})$, và $( \widetilde{D}(G_{\alpha}),\widetilde{f}_{\alpha \beta})$ là một hệ xạ ảnh các nhóm tôpô thỏa mãn các giả thiết của Bổ đề 3.

Từ bổ đề này suy ra rằng nhóm tôpô lim$_{\leftarrow -}\widetilde{D}(G_{\alpha})$ đẳng cấu với tích của một họ $(S_{\lambda})_{\lambda\in L}$ các nhóm Lie compact hầu đơn. Theo Bổ đề 1, giới hạn của hệ xạ ảnh các đồng cấu $(\pi_{\alpha})$ có thể được đồng nhất với một đồng cấu liên tục $\pi :\prod_{\lambda\in L}S_{\lambda}\rightarrow D(G)$,

đồng cấu này là toàn ánh (Topologie générale, Ch. I, §9, no. 6, Hệ quả 2 của Mệnh đề 8).

Bây giờ hãy nhận thấy rằng nhóm $\prod_{\lambda\in L}S_{\lambda}$ bằng nhóm dẫn xuất của nó: điều này

suy ra từ §4, no. 5, Hệ quả của Mệnh đề 10. Điều tương tự cũng đúng với D(G), vì $\pi$ là toàn ánh. Do đó, $D(G)\supset D(D(G)) = D(G)$. Vậy nhóm D(G) là compact và bằng nhóm dẫn xuất của nó; điều này chứng minh a), vì các khẳng định liên quan đến $C(G)_0$ là tầm thường.

Mặt khác, hạt nhân của $\pi :\prod_{\lambda\in L}S_{\lambda}\rightarrow D(G)$ có thể được đồng nhất

với lim$_{\leftarrow -}$ Ker($\pi_{\alpha}$) $($Algèbre, Ch. II, §6, no. 1, Nhận xét 1), và do đó với một

nhóm con compact, hoàn toàn không liên thông, trung tâm, vậy nên có c).

Ta chứng minh b). Với mọi $\alpha$ trong I, cấu xạ $s_{\alpha}: C(G_{\alpha})_0\times D(G_{\alpha})\rightarrow G_{\alpha}$ sao cho $s_{\alpha}(x, y) =xy$ với $x\in C(G_{\alpha})_0, y\in D(G_{\alpha})$, là toàn ánh và hạt nhân của nó là một nhóm con trung tâm hữu hạn (§1, no. 4, Hệ quả 1 của Mệnh đề 4). Các $s_{\alpha}$ tạo thành một hệ xạ ảnh các ánh xạ mà giới hạn, theo điều trước, có thể được đồng nhất với đồng cấu $(x, y) \rightarrow xy$ từ $C(G)_0\times D(G)$ vào G. Bây giờ ta thấy như trước rằng ánh xạ này là toàn ánh và hạt nhân của nó là trung tâm và hoàn toàn gián đoạn, do đó suy ra b).

#### Hệ quả {#lie-ix-a1-n3-cor-1 .statement tag=01IQ}

Mọi nhóm compact liên thông giải được đều giao hoán.

Thật vậy, nhóm dẫn xuất khi đó là giải được và bằng với nhóm dẫn xuất của nó (Mệnh đề $2a$)$)$, do đó thu về phần tử đơn vị.

### Bài tập {#lie-ix-a1-exercises}

Xem [các bài tập cho Phụ lục 1](exercises/a1/).
