---
book: ac
book_title: Commutative Algebra
chapter: VII
chapter_title: DIVISORS
section: 4
section_title: Modules over integrally closed Noetherian domains
lang: vi
source: ac-i-vii
book_pages: 512-544, 571-578
pdf_pages: 0530-0562, 0589-0596
extraction: ocr
subsections:
    - "no": 1
      title: LATTICES
      page: 512
      pdf_page: 530
    - "no": 2
      title: DUALITY; REFLEXIVE MODULES
      page: 517
      pdf_page: 535
    - "no": 3
      title: LOCAL CONSTRUCTION OF REFLEXIVE MODULES
      page: 521
      pdf_page: 539
    - "no": 4
      title: PSEUDO-ISOMORPHISMS
      page: 523
      pdf_page: 541
    - "no": 5
      title: DIVISORS ATTACHED TO TORSION MODULES
      page: 527
      pdf_page: 545
    - "no": 6
      title: RELATIVE INVARIANT OF TWO LATTICES
      page: 529
      pdf_page: 547
    - "no": 7
      title: DIVISOR CLASSES ATTACHED TO FINITELY GENERATED MODULES
      page: 531
      pdf_page: 549
    - "no": 8
      title: PROPERTIES RELATIVE TO FINITE EXTENSIONS OF THE RING OF SCALARS
      page: 535
      pdf_page: 553
    - "no": 9
      title: A REDUCTION THEOREM
      page: 540
      pdf_page: 558
    - "no": 10
      title: MODULES OVER DEDEKIND DOMAINS
      page: 543
      pdf_page: 561
statements: 56
exercises: 26
content_sha256: c7a5110def2d2b4ac1b8f44a8124e28b58061244c2f290ef565f0077196c192f
translated_from: content/en/ac/VII/04_s4_modules_over_integrally_closed.md
source_content_sha256: 2b0e46004ec0336ef8389dfa0cd64f75eed1d16406a473ee4d387f8c0fa0eaa6
translation_model: gpt-5-6-mini, gpt-5.4
translation_run: translate-vi-2cf0ee81
glossary_version: 34
glossary_terms_sha256: bd9486e0a98026941ed4840602d338535a6148f1f94addc99907d430eea07a92
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 4. CÁC MÔĐUN TRÊN CÁC MIỀN NOETHER ĐÓNG NGUYÊN

Trong suốt đoạn này, $\mathbf{A}$ sẽ là một *miền nguyên giao hoán* với trường phân thức $K$. Bắt đầu từ no. 2, $\mathbf{A}$ sẽ còn được giả thiết là *Noether và đóng nguyên* (và do đó là một miền Krull ($\S$ 1, no. 3, Hệ quả của Định lý 2)); khi đó $P(\mathbf{A})$, $D(\mathbf{A})$ và $C(\mathbf{A})$ lần lượt sẽ chỉ tập hợp các iđêan nguyên tố của $\mathbf{A}$ có chiều cao 1 ($\S$ 1, no. 6), nhóm ước của $\mathbf{A}$ ($\S$ 1, no. 3) và nhóm lớp ước của $\mathbf{A}$ ($\S$ 1, no. 10), các nhóm sau này được viết *cộng tính*.

Phương pháp tổng quát để nghiên cứu các môđun sinh hữu hạn trên một miền Noether đóng nguyên $\mathbf{A}$ bao gồm việc "địa phương hóa" các môđun đối với tất cả các iđêan nguyên tố $p \in P(\mathbf{A})$ có *chiều cao* 1 trong $\mathbf{A}$; vì khi đó $\mathbf{A}$ là một *vành định giá rời rạc* ($\S$ 1, no. 6, Định lý 4), cấu trúc của các $\mathbf{A}_p$-môđun sinh hữu hạn đã được biết rõ (*Đại số*, Chương VII, $\S$ 4) và do đó cho thông tin về cấu trúc của các $\mathbf{A}$-môđun sinh hữu hạn. Trong trường hợp riêng khi $\mathbf{A}$ là một miền Dedekind, ta có thể đạt được một lý thuyết đầy đủ như khi $\mathbf{A}$ là một miền iđêan chính (no. 10).

### 1. CÁC DÀN

#### Định nghĩa 1 {#ac-vii-s4-def-1 .statement}

*Cho $V$ là một không gian vectơ hữu hạn chiều trên trường $K$. Một dàn của $V$ đối với $\mathbf{A}$ (hay đơn giản là một dàn của $V$) được định nghĩa là bất kỳ môđun con-$\mathbf{A}$ $M$ nào của $V$ thỏa mãn điều kiện sau:*

Tồn tại hai môđun con-$\mathbf{A}$ tự do $L_1,\ L_2$ của $V$ sao cho $L_1 \subset M \subset L_2$ và $\mathrm{rg}_{\mathbf{A}}(L_1) = \mathrm{rg}_K(V)$.

Ví dụ
(1) Nếu lấy $V = K$, các dàn của $K$ chính là *các iđêan phân thức* $\neq (0)$ của $K$ ($\S$ 1, no. 1, Định nghĩa 1).

(2) Nếu $\mathrm{rg}_K(V) = n$, mọi môđun con-A *tự do* L của V có một cơ sở chứa nhiều nhất n phần tử, mọi tập con của V tự do trên A cũng tự do trên K; để L là một dàn của V, điều kiện cần và đủ là L có một cơ sở gồm n phần tử (nói cách khác, $\mathrm{rg}_A(L) = n$).

(3) Nếu A là *một miền iđêan chính*, mọi dàn M của V là một A-môđun sinh hữu hạn (vì A là Noether) không xoắn và do đó là một A-môđun *tự do* (*Đại số*, Chương VII, § 4, no. 3, Hệ quả 2 của Định lý 2).

#### Mệnh đề 1 {#ac-vii-s4-prop-1 .statement}

*Đối với một môđun con-A M của V là một dàn của V, điều kiện cần và đủ là KM = V và M được chứa trong một môđun con-A sinh hữu hạn của V.*

Các điều kiện rõ ràng là cần thiết, vì một môđun con-A tự do của V có cùng hạng với V sinh ra V. Ngược lại, nếu KM = V, M chứa một cơ sở $(a_i)_{1 \leq i \leq n}$ của V trên K và do đó nó chứa môđun con-A tự do L, sinh bởi các $a_i$; mặt khác, nếu $M \subset M_1$, trong đó M, là một môđun con-A của V được sinh bởi một số hữu hạn phần tử b, và $(e_i)_{1 \leq i \leq n}$ là một cơ sở của V trên K, tồn tại một phần tử s $\neq 0$ của A sao cho mỗi b, là một tổ hợp tuyến tính của các $s^{-1}e_i$ với các hệ số *trong* A; nếu L, là các môđun con-A tự do của V được sinh bởi các $s^{-1}e_i$, thì $M \subset L_2$.

#### Hệ quả {#ac-vii-s4-n1-cor-1 .statement}

*Giả sử rằng A là Noether; đối với một môđun con-A M của V là một dàn của V, điều kiện cần và đủ là KM = V và M sinh hữu hạn.*

*Nhận xét* (1). Nhắc lại rằng với mọi môđun con-A M của V, ánh xạ chính tắc $M \otimes_A K \to V$ là đơn ánh và có ảnh KM (*Đại số*, Chương II, § 7, no. 10, Mệnh đề 26); nói rằng KM = V có nghĩa là do đó ánh xạ này là *song ánh*.

#### Mệnh đề 2 {#ac-vii-s4-prop-2 .statement}

*Cho M là một dàn của V và M, một môđun con-A của V. Nếu tồn tại hai phần tử x, y của $K^*$ sao cho $xM \subset M_1 \subset yM$, $M_1$ là một dàn của V; ngược lại, nếu $M_1$ là một dàn của V, tồn tại hai phần tử khác không a, b của A sao cho $aM \subset M, \subset b^{-1}M$.*

Nếu $L_1, L_2$ là hai dàn tự do của V sao cho $L, \subset M \subset L,$, các quan hệ $xM \subset M_1 \subset yM$ kéo theo $xL_1 \subset M, \subset yL_2$ và $xL_1$ và $yL_2$ là các dàn tự do; ngược lại, nếu M, là một dàn và $(e_i)_{1 \leq i \leq n}$ là một cơ sở của L, trên A, thì quan hệ KM, = V kéo theo sự tồn tại của $x = a/s \in K^*$ (trong đó a và s là các phần tử khác không của A) sao cho $xe_i \in M,$ với mọi $i$, do đó $xM \subset xL_2 \subset M_1$ và *a fortiori* $aM \subset M,$; khi đổi vai trò của M và M, cũng có thể chứng minh tương tự rằng tồn tại $b \neq 0$ trong A sao cho $bM_1 \subset M$.

#### Mệnh đề 3 {#ac-vii-s4-prop-3 .statement}

(i) *Nếu $M_1$ và $M_2$ là các dàn của V, thì $M_1 \cap M,$ và $M_1 + M_2$ cũng vậy.

(ii) *Nếu W là một không gian con vectơ của V và M là một dàn của V, thì $M \cap W$ là một dàn của W.*

(iii) Cho $V, V_1, \ldots, V_k$ là các không gian vectơ hạng hữu hạn trên $K$ và cho
$$
f : V_1 \times \cdots \times V_k \to V
$$
là một ánh xạ đa tuyến tính mà ảnh sinh ra $V$. *Nếu $M_i$ là một dàn của $V_i$ với $1 \leq i \leq k$, thì A-môđun con của $V$ sinh bởi $f$ ($(M, x \ldots x M_k)$) là một dàn của $V$.*

(iv) Cho $V$ và $W$ là hai không gian vectơ hạng hữu hạn trên $K$, $M$ là một dàn của $V$ và $N$ là một dàn của $W$. *A-môđun con $N$: $M$ của $\mathrm{Hom}_K(V, W)$, gồm các ánh xạ K-tuyến tính $f$ sao cho $f(M) \subset N$, là một dàn của $\mathrm{Hom}_K(V, W)$.*

(i) Chiếu theo Mệnh đề 2, tồn tại các phần tử khác không $a$ và $b$ trong $A$ sao cho $aM_1 \subset M_2 \subset b^{-1}M_1$; ta kết luận rằng $M, \cap M,$ và $M, + M_2$ nằm giữa $aM_1$ và $b^{-1}M_1$ và do đó là các dàn, chiếu theo Mệnh đề 2.

(ii) Cho $S$ là một phần bù của $W$ trong $V$, $L_w$ là một dàn tự do của $W$ và $L_s$ là một dàn tự do của $S$, sao cho $L = L_w \oplus L_s$ là một dàn tự do của $V$. Khi đó tồn tại $x, y$ trong $K^*$ sao cho $xL \subset M \subset yL$. Suy ra $xL_w \subset M \cap W \subset yL_w$, điều này chứng tỏ rằng $M \cap W$ là một dàn của $W$ (Mệnh đề 2).

(iii) Vì $KM, = V,$ nên rõ ràng theo tính tuyến tính $f$ ($M, x \ldots x M,$)  sinh không gian vectơ trên K $V$; mặt khác, với mọi $i$, tồn tại một A-môđun con sinh hữu hạn $N_i$ của $V$, sao cho $M, \subset N_i;$ A-môđun con $N$ của $V$ được sinh bởi $f(N, x \ldots x N,)$ là sinh hữu hạn và chứa $M$ và do đó $M$ là một dàn của $V$ (Mệnh đề 1).

(iv) Cho $P$ (ứng với $Q$) là một dàn tự do của $V$ (ứng với $W$) chứa $M$ (ứng với được chứa trong $N$); hiển nhiên $N : M \supset Q : P$. Khi đó ngay lập tức suy ra $Q : P$ đẳng cấu với $\mathrm{Hom}_A(P, Q)$, do đó là một A-môđun tự do hạng $(\mathrm{rg}_A P)(\mathrm{rg}_A Q)$ (*Algebra*, Chương II, § 1, no. 6, Hệ quả 1 của Mệnh đề 6) và vì thế là một dàn của $\mathrm{Hom}_K(V, W)$. Tương tự, nếu $P'$ (ứng với $Q'$) là một dàn tự do của $V$ (ứng với $W$) được chứa trong $M$ (ứng với chứa $N$), thì $Q' : P' \supset N : M$ và $Q' : P'$ là một dàn của $\mathrm{Hom}_K(V, W)$; do đó có kết luận.

*Nhận xét*
(2) Mệnh đề 3 (i) cho thấy rằng tập hợp $R(V)$ các dàn của $V$ là *có thứ tự bởi dàn* đối với quan hệ bao hàm; hơn nữa, nếu $M$ là một dàn cố định của $V$, thì các $xM$, với $x$ chạy qua $K^*$, tạo thành một tập con của $R(V)$ vừa *coinitial* vừa *cofinal* (*Set Theory*, Chương III, § 1, no. 7).

(3) Với các ký hiệu của Mệnh đề 3 (iv), ánh xạ chính tắc
$$
N : M \to \mathrm{Hom}_A(M, N),
$$
ánh xạ mỗi ánh xạ K-tuyến tính $f \in N : M$ tới ánh xạ A-tuyến tính từ $M$ vào $N$ có cùng đồ thị như $f|_M$, là *song ánh*, vì mọi ánh xạ A-tuyến tính $g : M \to N$ đều có thể được nhúng vào một ánh xạ K-tuyến tính
$$
g \otimes 1 : M \otimes_A K \to N \otimes_A K
$$

và ta đã thấy rằng $M \otimes_A K$ và $N \otimes_A K$ được đồng nhất tương ứng với $V$ và $W$.

Đặc biệt, nếu ta lấy $W = K$, $N = A$, thì $\operatorname{Hom}_K(V, W)$ chính là *không gian vectơ K đối ngẫu* $V^*$ của $V$ và $A$: $M$ được đồng nhất với *A-môđun đối ngẫu* $M^*$ của $M$; từ nay về sau ta sẽ thực hiện sự đồng nhất này và ta sẽ nói rằng $M^*$ là *dàn đối ngẫu* của $M$: do đó nó là *tập hợp các* $x^* \in V^*$ *sao cho* $\langle x, x^* \rangle \in A$ *với mọi* $x \in M$.

#### Hệ quả {#ac-vii-s4-n1-cor-2 .statement}

*Cho U, V, W là ba không gian vectơ hạng hữu hạn trên K và f: U × V → W là một ánh xạ K-song tuyến tính không suy biến trái* (Đại số, Chương IX, § 1, no. 1, Định nghĩa 3). *Nếu M là một dàn của V và N là một dàn của W, thì tập hợp N: ,M các x ∈ U sao chof (x, y) ∈ N với mọiy ∈ M là một dàn của U*.

Gọi $s_f: U \to \operatorname{Hom}_K(V, W)$ là ánh xạ K-tuyến tính liên kết trái với $f$ (Đại số, Chương IX, *loc. cit.*) sao cho $s_f(x)$ là ánh xạ tuyến tính $y \mapsto f(x, y)$; nhắc lại rằng nói $f$ là không suy biến trái có nghĩa là $s_f$ là *đơn ánh*. Theo Mệnh đề 3 (iv), $N: M$ là một dàn của $\operatorname{Hom}_K(V, W)$; vì $N: fM = s_f^{-1}(N: M)$ và $s_f$ là đơn ánh, hệ quả suy ra từ Mệnh đề 3 (ii).

*Ví dụ*

(4) Cho $S$ là một đại số trên K (không nhất thiết kết hợp) hạng hữu hạn có một phần tử đơn vị; khi đó ánh xạ song tuyến tính $(x, y) \mapsto xy$ từ $S \times S$ đến $S$ là không suy biến (trái và phải). Nếu $M$ và $N$ là các dàn của $S$ đối với $A$, thì $M.N$ (Mệnh đề 3 (iii)) và tập hợp các $x \in S$ sao cho $xM \subset N$ (Hệ quả của Mệnh đề 3) cũng vậy. Chú ý rằng tồn tại một *đại số con trên A* của $S$ chứa phần tử đơn vị của $S$ và là một *dàn* của $S$; thật vậy, xét một cơ sở $(e_i)_{1 \leq i \leq n}$ của $S$ sao cho $e_1$ là phần tử đơn vị của $S$ và đặt $e_i e_j = \sum_k c_{ijk} e_k$ là bảng phép nhân của $S$ ($1 \leq i \leq n, 1 \leq j \leq n$), *sao cho* $c_{1jk} = \delta_{jk}, c_{i1k} = \delta_{ik}$ (các ký hiệu Kronecker). Cho $s \in A$ là khác không và sao cho $c'_{ijk} = s \cdot c_{ijk} \in A$ với mọi bộ ba chỉ số $(i, j, k)$; nếu ta viết $e'_i = s^{-1} e_i$ với $i \geq 2$, thì

$$
e'_i e'_j = s c'_{ij1} e'_1 + \sum_{k \geq 2} c'_{ijk} e'_k
$$

với $i \geq 2$ và $j \geq 2$; dàn của $S$ có cơ sở là $e_1$ và các $e'_i$ ($2 \leq i \leq n$) là một đại số con trên A của $S$ có phần tử đơn vị $e_1$.

(5) Cho $V$ là một không gian vectơ hữu hạn chiều trên $K$ và $f$ là một dạng song tuyến tính không suy biến trên $V$. Nếu $M$ là một dàn của $V$, thì từ Hệ quả của Mệnh đề 3 suy ra rằng tập $M^*_f$ các $x \in V$ sao cho $f(x, y) \in A$ với mọi y $\in M$ cũng là một dàn của $V$; nếu $s_f: V \to V^*$ là ánh xạ tuyến tính trái liên kết với $f$ (là song ánh), thì $s_f(M^*_f)$ chính là dàn đối ngẫu $M^*$ của $M$.

#### Mệnh đề 4 {#ac-vii-s4-prop-4 .statement}

*Cho B là một miền nguyên, A là một vành con của B và K và L là các trường & trường phân thức tương ứng của A và B. Cho V là một không gian vectơ hữu hạn chiều trên K.*

(i) Với mọi dàn $M$ của $V$ đối với $A$, ảnh $BM$ của $M_{(B)} = M \otimes_A B$ trong $V_{(L)} = V \otimes_K L$ là một dàn của $V_{(L)}$ đối với $B$.

(ii) Giả sử thêm rằng $B$ là một $A$-môđun phẳng. Khi đó ánh xạ chính tắc $M_{(B)} \to BM$ là song ánh. Nếu hơn nữa $B$ là phẳng trung thành, ánh xạ biến mỗi dàn $M$ của $V$ đối với $A$ thành dàn $BM$ của $V_{(L)}$ đối với $B$ là đơn ánh.

(i) Vì $KM = V$, rõ ràng $L . (BM) = V_{(L)}$; mặt khác $M$ được chứa trong một môđun con hữu hạn sinh $M_1$ của $V$ trên $A$ và do đó $BM$ được chứa trong $BM_1$ là một $B$-môđun sinh hữu hạn; do đó mệnh đề (i) (Mệnh đề 1).

(ii) $V_{(L)} = V \otimes_K L = V \otimes_A L$ (Chương II, § 2, no. 7, Mệnh đề 18) và, vì $L$ là một $B$-môđun phẳng, nó cũng là một $A$-môđun phẳng (Chương I, § 2, no. 7, Hệ quả 3 của Mệnh đề 8). Vì $B$ là một $A$-môđun phẳng, ánh xạ chính tắc $M \otimes_A B \to V \otimes_A B$ là đơn ánh; mặt khác, vì $V$ là một $K$-môđun tự do và $K$ là một $A$-môđun phẳng, $V$ là một $A$-môđun phẳng (Chương I, § 2, no. 7, Hệ quả 3 của Mệnh đề 8) và do đó ánh xạ chính tắc $V \otimes_A B \to V \otimes_A L$ là đơn ánh, điều này chứng minh mệnh đề thứ nhất. Để cũng thấy rằng quan hệ $BM_1 = BM_2$ kéo theo $M_1 = M_2$ đối với hai dàn $M_1, M_2$ của $V$ đối với $A$ khi $B$ là một $A$-môđun phẳng trung thành, trước hết chú ý rằng $BM_1 \cap BM_2 = B(M_1 \cap M_2)$ (Chương I, § 2, no. 6, Mệnh đề 6); do đó ta có thể chỉ xét trường hợp $M_1 \subset M$, và khi ấy mệnh đề của ta suy ra từ Chương I, § 3, no. 1, Mệnh đề 3 áp dụng cho đơn ánh chính tắc $M_1 \to M_2$.

#### Hệ quả {#ac-vii-s4-n1-cor-3 .statement}

Giả sử rằng $A$ là một vành định giá rời rạc. Gọi $\hat{A}$ là vành hoàn thành của nó và $\hat{K}$ là trường phân thức của $\hat{A}$ (Chương VI, § 5, no. 3). Ánh xạ $\phi$, biến mỗi dàn $M$ của $V$ thành dàn $\hat{A}M$ của $\hat{V} = V \otimes_K \hat{K}$ đối với $\hat{A}$, là song ánh và ánh xạ nghịch đảo của nó biến mỗi dàn $M'$ của $\hat{V}$ đối với $\hat{A}$ thành giao của nó với $V$, tức $M' \cap V$ ($V$ được đồng nhất một cách chính tắc với một không gian con-vectơ trên $K$ của $\hat{V}$).

Nếu $L$ là một dàn tự do của $V$, thì các dàn $aL$ (với $a \in A, a \neq 0$) tạo thành một hệ cơ bản các lân cận của 0 đối với một tôpô $\mathcal{T}$ trên $V$ (tương thích với cấu trúc $A$-môđun của nó), tôpô này (khi chọn một cơ sở của $L$ trên $A$) được đồng nhất với tôpô tích trên $K^n$); nhờ Mệnh đề 2, một hệ cơ bản các lân cận của 0 đối với $\mathcal{T}$ cũng gồm tất cả các dàn của $V$ đối với $A$; rõ ràng $\hat{V}$ là bổ sung của $V$ đối với $\mathcal{T}$. Hơn nữa, nếu $m$ là iđêan cực đại của $A$, thì tôpô $\mathcal{T}$ cảm sinh trên mọi dàn $M$ của $V$ đối với $A$ tôpô $m$-adic vì $M$ là một $A$-môđun sinh hữu hạn (Chương III, § 3, no. 2, Định lý 2) và $\hat{A}M$ là bổ sung của $M$ đối với tôpô này (Chương III, § 2, no. 12, Mệnh đề 16); hơn nữa, vì $M$ là mở (và do đó đóng) trong $V$, nên $\hat{A}M \cap V = M$, điều này lại chứng minh rằng $\dagger$ là đơn ánh (điều này suy ra trực tiếp từ Mệnh đề 4, (ii), vì $A$ là một $A$-môđun phẳng trung thành). Cuối cùng, nếu $M'$ là một dàn của $\hat{V}$ đối với $\hat{A}$, thì $M = M' \cap V$ là một dàn của $V$ đối với $A$, vì mọi phần tử của $\hat{A}$ là tích của một phần tử của $A$ và một phần tử khả nghịch của $\hat{A}$, và do đó từ Mệnh đề 2 suy ra rằng tồn tại $a, b$ trong $A - \{0\}$ sao cho $a \hat{A}L \subset M' \subset b \hat{A}L$, nên $aL \subset M' \cap V \subset bL$. Hơn nữa $M'$ là mở trong $V$ và, vì $V$ là trù mật trong $\hat{V}$, $M'$ là bổ sung của $M' \cap V = M$; điều này chứng minh rằng $\phi$ là toàn ánh, do đó có hệ quả.

Ví dụ (6) Cho $S$ là một tập con nhân tính của $A$ không chứa 0; ta áp dụng Mệnh đề 4 cho $B = S^{-1}A$; khi đó $L = K$, $BM = S^{-1}M$; do đó $S^{-1}M$ là một dàn của $V$ đối với $S^{-1}A$. Hơn nữa:

#### Mệnh đề 5 {#ac-vii-s4-prop-5 .statement}

*Cho $V, W$ là các không gian vectơ hạng hữu hạn trên $K$, $M$ là một dàn của $V$ và $N$ là một dàn của $W$. Nếu $M$ sinh hữu hạn, thì (theo ký hiệu của Mệnh đề 3):*

(1)
$$
S^{-1}(N : M) = S^{-1}N : S^{-1}M
$$
*trong* $\operatorname{Hom}_K(V, W)$.

Rõ ràng vế trái của (1) được chứa trong vế phải. Ngược lại, cho $f \in S^{-1}N : S^{-1}M$ và cho $(x_i)_{1 \leq i \leq n}$ là một hệ sinh của $M$. Tồn tại $s \in S$ sao cho $f(x_i) \in s^{-1}N$ với mọi $i$ và do đó $sf \in N : M$, điều đó chứng minh mệnh đề.

### 2. ĐỐI NGẪU; MÔĐUN PHẢN XẠ

Nhắc lại rằng từ bây giờ miền $A$ được giả thiết là *Noether và đóng nguyên* và $P(A)$ (hoặc đơn giản là $P$) ký hiệu tập hợp các iđêan nguyên tố của $A$ *có chiều cao* 1. Mọi dàn đối với $A$ đều là *một* $A$-môđun *sinh hữu hạn* (no. 1, Hệ quả của Mệnh đề 1).

Cho $V$ là một không gian vectơ hạng hữu hạn trên $K$, $V^*$ là đối ngẫu của nó và $V^{**}$ là đối ngẫu kép của nó; ta sẽ đồng nhất $V$ và $V^{**}$ bằng ánh xạ chính tắc $c_V$ (*Algebra*, Chương II, § 7, no. 5, Định lý 6). Cho $M$ là một dàn của $V$; nhắc lại rằng $A$-môđun đối ngẫu $M^*$ của $M$ được đồng nhất một cách chính tắc với *dàn đối ngẫu* của $M$, tức là tập hợp các $x^* \in V^*$ sao cho $\langle x, x^* \rangle \in A$ với mọi $x \in M$; do đó $A$-môđun *đối ngẫu kép* $M^{**}$ của $M$ là một *dàn* của $V$ chứa $M$. Hơn nữa $M^{***} = M^*$, vì quan hệ $M \subset M^{**}$ kéo theo $(M^{**})^* \subset M^*$ và mặt khác $M^* \subset (M^*)^{**}$ theo điều trên (xem *Set Theory*, Chương III, § 1, no. 5, Mệnh đề 2).

Nếu $p$ là một iđêan nguyên tố, thì Mệnh đề 5 áp dụng với $N = A$ cho quan hệ $(M^*)_p = (M_p)^*$, điều này biện minh cho ký hiệu $M_p^*$ cho cả hai vế.

#### Định lý 1 {#ac-vii-s4-thm-1 .statement}

*Nếu $M$ là một dàn của $V$, thì* $M^* = \bigcap_{p \in P} M_p^*$.

Rõ ràng $M^*$ được chứa trong mỗi $M_p^*$. Ngược lại, giả sử $x^* \in \bigcap M_p^*$; nếu $x \in M$, thì $\langle x, x^* \rangle \in \bigcap_{p \in P} A_p$ và, vì $A = \bigcap_{p \in P} A_p$ (\S 1, no. 6, Định lý 4), nên $x^* \in M^*$.

Áp dụng Định lý 1 cho $M^*$ cho thấy rằng $M^{**} = \bigcap_{p \in P} M_p^{**}$. Nhưng vì $A$, là một miền iđêan chính ($\S 1$, no. **6**, Định lý **4**), $M$, là một $A$-môđun tự do sinh hữu hạn và do đó $M_p^{**}$ được đồng nhất một cách chính tắc với $M$, (*Algebra*, Chương II, $\S 2$, no. **7**, Mệnh đề **14**), do đó suy ra hệ quả.

Với mọi dàn $M$ đối với $A$, ánh xạ chính tắc $c_M : M \to M^{**}$ (*Algebra*, Chapter 11, $\S 2$, no. **7**) đồng nhất một phần tử $x \in M$ với chính nó, vì $x$ là phần tử duy nhất $y$ của $V = V^{**}$ sao cho $\langle x, x^* \rangle = \langle y, x^* \rangle$ với mọi $x^* \in M^*$, do $M^*$ sinh ra $V^*$. Ta sẽ nói rằng $M$ là *phản xạ* nếu $M^{**} = M$ (*loc. cit.*). Vì ở trên ta có $M^* = (M^*)^{**}$, nên thấy rằng *đối ngẫu* của mọi dàn $M$ luôn luôn là *phản xạ*.

*Nhận xét* (1) Cho $M$ là một $A$-môđun sinh hữu hạn; ngay lập tức thấy rằng đối ngẫu $M^*$ của $M$, được đồng nhất với một môđun con-$A$ của $\operatorname{Hom}_A(M, K)$, là một *dàn* của không gian vectơ $K$ $\operatorname{Hom}_A(M, K)$; đặc biệt, mọi $A$-môđun *phản xạ* sinh hữu hạn đều đẳng cấu với một dàn của một không gian vectơ $K$ thích hợp.

#### Định lý 2 {#ac-vii-s4-thm-2 .statement}

*Nếu $M$ là một dàn của* $V$, *thì các điều kiện sau là tương đương*:
(a) $M$ *là phản xạ*.
(b) $M = \bigcap_{p \in P} M_p$.
(c) $\operatorname{Ass}(V/M) \subset P$.

Sự tương đương của (a) và (b) suy ra từ Hệ quả của Định lý 1. Nếu (b) đúng, $V/M$ được đồng nhất một cách chính tắc với một môđun con-$A$ của tích $\prod_{p \in P} (V/M_p)$; nhưng thực ra nó được chứa trong *tổng trực tiếp* $\bigoplus_{p \in P} (V/M_p)$: thật vậy, nếu $L \subset M$ là một dàn tự do và $(e_i)_{1 \leq i \leq n}$ là một cơ sở của $L$, thì mỗi tọa độ $x_i$ của một điểm $x \in V$ đối với $(e_i)$ đều thuộc $A$, trừ ra đối với một số hữu hạn giá trị của $p \in P$. Khi đó quan hệ $V/M \subset \bigoplus_{p \in P} (V/M_p)$ kéo theo:

$$
\operatorname{Ass}(V/M) \subset \bigcap_{p \in P} \operatorname{Ass}(V/M_p).
$$

Vì $V/M_p$ là một $A_p$-môđun, một phần tử của $A - p$ không thể triệt tiêu một phần tử $\neq 0$ của $V/M_p$, vì các phần tử của $A - p$ là khả nghịch trong $A$; do đó các phần tử của $\operatorname{Ass}(V/M_p)$ được chứa trong $p$ và khác $0$, vì $V/M_p$ là một $A$-môđun xoắn; vì $p$ có chiều cao **1**, tất yếu $\operatorname{Ass}(V/M_p) = \{ p \}$ nếu $V/M_p \neq (0)$ và $\operatorname{Ass}(V/M_p) = \varnothing$ nếu $V/M_p = (0)$; suy ra $\operatorname{Ass}(V/M) \subset P$.

Cuối cùng, nếu điều kiện (c) đúng, thì

$$
\operatorname{Ass}(M^{**}/M) \subset \operatorname{Ass}(V/M) \subset P.
$$

Mặt khác, nếu $p \in P$, thì trong chứng minh của Hệ quả của Định lý 1 ta đã thấy rằng $M_p^{**} = M_p$, do đó $p \notin \operatorname{Ass}(M^{**}/M)$ (Chương IV, $\S 1$, no. 3, Hệ quả 1 của Mệnh đề 7). Ta kết luận rằng Ass(M**/M) = ∅, do đó M** = M (Chương IV, § 1, no. 1, Hệ quả 1 của Mệnh đề 2).

#### Hệ quả {#ac-vii-s4-n2-cor-1 .statement}

Cho M, N là hai dàn của V đối với A sao cho N phản xạ. Để có M ⊂ N, điều kiện cần và đủ là, với mọi p ∈ P, M_p ⊂ N_p.

Điều kiện ấy hiển nhiên là cần và, nếu nó được thỏa mãn, thì

$$
\bigcap_{p \in P} M_p \subset \bigcap_{p \in P} N_p = N.
$$

Vì M ⊂ M** = \bigcap_p M_p, chắc chắn M ⊂ N.

Ví dụ
(1) Mọi dàn tự do đều phản xạ.
(2) Lấy V = K. Để một iđêan phân số a của K là một dàn phản xạ, điều kiện cần và đủ là nó là một iđêan divisorial, theo tiêu chuẩn (b) của Định lý 2 và § 1, no. 4, các Mệnh đề 5 và 7.
(3) Cho M là một dàn đối với A; nếu S là một tập con nhân tính của A không chứa 0, Mệnh đề 5 của no. 1 cho thấy rằng S^{-1}(M*) = (S^{-1}M)*; do đó, nếu M phản xạ, thì S^{-1}M là một dàn phản xạ đối với S^{-1}A.

#### Mệnh đề 6 {#ac-vii-s4-prop-6 .statement}

(i) Nếu M_1 và M là các dàn phản xạ của V, thì M, n M cũng vậy.
(ii) Nếu W là một không gian con vectơ của V và M là một dàn phản xạ của V, thì M n W là một dàn phản xạ của W.
(iii) Cho V, W là hai không gian vectơ hạng hữu hạn trên K và M (tương ứng N) là một dàn của V (tương ứng W). Nếu N phản xạ, thì dàn N: M của Hom_K(V, W) (no. 1, Mệnh đề 3) là phản xạ.

(i) (M, n M_2)_p = (M_1)_p n (M_2)_p với mọi p ∈ P (Chương II, § 2, no. 4, Định lý 1). Nếu M_1 = \bigcap_{p \in P} (M_1)_p và M_2 = \bigcap_{p \in P} (M_2)_p, thì

$$
M, n M_2 = \bigcap_{p \in P} (M, n M_2)_p
$$

do đó kết luận suy ra theo Định lý 2.
(ii) Tương tự, (M n W)_p = M_p n W_p = M_p n W, do đó

$$
M \cap W = \bigcap_{p \in P} (M \cap W)_p,
$$

điều này chứng minh (ii).
(iii) Vì M sinh hữu hạn, từ no. 1, Mệnh đề 5 suy ra rằng (N: M)_p = N_p M_p; hơn nữa, quan hệ N = \bigcap_{p \in P} N_p kéo theo:

$$
N: M = \bigcap_{p \in P} (N_p : M_p).
$$

Thật vậy, nếu $f \in \bigcap_{p \in P} (N_p : M_p)$ và $x \in M$, thì $f(x) \in \bigcap_{p \in P} N_p = N$, do đó $f \in N : M$; điều này cho thấy rằng $N : M$ là phản xạ.

Nhận xét
(2) Nếu $M_1$ và $M_2$ là các dàn phản xạ của $V$, thì dàn $M_1 + M_2$ không nhất thiết là phản xạ (xem § 1, Bài tập 2).
(3) Nếu $M$ là một $A$-môđun sinh hữu hạn và $T$ là môđun con xoắn của nó, thì đối ngẫu $M^*$ của $M$ cũng chính là đối ngẫu của $M/T$, vì với mọi dạng tuyến tính $f$ trên $M$, ảnh $f(T)$ là một môđun con xoắn của $A$ và do đó bằng không. Vì $M/T$ đẳng cấu với một dàn của một không gian vectơ trên $K$, ta thấy rằng đối ngẫu của mọi $A$-môđun sinh hữu hạn đều là phản xạ.

#### Mệnh đề 7 {#ac-vii-s4-prop-7 .statement}

Cho $0 \to M \to N \to Q \to 0$ là một dãy khớp các $A$-môđun. Giả sử rằng $N$ sinh hữu hạn và không xoắn.
(i) Nếu $M$ phản xạ, thì $\operatorname{Ass}(Q) \subset P \cup \{\{0\}\}$ (nói cách khác, mọi iđêan liên kết với $Q$ hoặc là $(0)$, hoặc có chiều cao bằng 1).
(ii) Ngược lại, nếu $N$ phản xạ và $\operatorname{Ass}(Q) \subset P \cup \{\{0\}\}$, thì $M$ phản xạ.

Vì $A$ là Noether, $M$ cũng sinh hữu hạn; nếu ta viết $V = M_{(K)}$, $W = N_{(K)}$, thì $M$ (tương ứng $N$) được đồng nhất một cách chính tắc với một dàn của $V$ (tương ứng của $W$) (no. 1, Mệnh đề 1). Xét hai dãy khớp:
$$
0 \to V/M \to W/M \to W/V \to 0 \\
0 \to Q \to W/M \to W/N \to 0.
$$
(i) Ta suy ra (Chương IV, § 1, no. 1, Mệnh đề 3) rằng:
$$
\operatorname{Ass}(Q) \subset \operatorname{ASS}(W/M) \subset \operatorname{ASS}(V/M) \cup \operatorname{ASS}(W/V).
$$
Nếu $M$ phản xạ, thì $\operatorname{Ass}(V/M) \subset P$ (Định lý 2); mặt khác, rõ ràng $\operatorname{Ass}(W/V)$ hoặc rỗng, hoặc thu về $\{0\}$; do đó có (i).
(ii) Tương tự:
$$
\operatorname{Ass}(V/M) \subset \operatorname{Ass}(W/M) \subset \operatorname{Ass}(Q) \cup \operatorname{Ass}(W/N).
$$
Do đó các giả thiết kéo theo $\operatorname{Ass}(V/M) \subset P \cup \{\{0\}\}$. Nhưng $V/M$ là một $A$-môđun xoắn và vì thế $\{0\} \notin \operatorname{Ass}(V/M)$; khi đó Định lý 2 cho thấy rằng $M$ phản xạ.

#### Mệnh đề 8 {#ac-vii-s4-prop-8 .statement}

Cho $R$ và $S$ là hai vành giao hoán, $p : R \to S$ là một đồng cấu vành và $M$ là một $R$-môđun sinh hữu hạn. Giả sử rằng $R$ là Noether và $S$ là một $R$-môđun phẳng. Khi đó, nếu $M$ phản xạ, thì $S$-môđun $M_{(S)} = M \otimes_R S$ cũng phản xạ.
Ta biết (Chương I, § 2, no. 10, Mệnh đề 11) rằng tồn tại một đẳng cấu chính tắc $\omega_M : (M^*)_{(S)} \to (M_{(S)})^*$, sao cho
$$
\langle x \otimes 1, \omega_M(x^* \otimes 1) \rangle = \rho(\langle x, x^* \rangle)
$$

Với x \in M, x^* \in M^*. Vì M là một thương của một R-môđun tự do sinh hữu hạn L, M* đẳng cấu với một môđun con trên R của đối ngẫu L* và L* là tự do và sinh hữu hạn; vì $\mathbf{R}$ là Noether, do đó M* cũng là một R-môđun sinh hữu hạn, suy ra một đẳng cấu $\omega_{M^*}: (M^{**})_{(S)} \to ((M^*)_{(S)})^*$ sao cho

$$
\langle x^* \otimes 1, \omega_{M^*}(x^{**} \otimes 1) \rangle = \rho(\langle x^*, x^{**} \rangle)
$$

với $x^* \in M$ và $x^{**} \in M^{**}$. Mặt khác, có một đẳng cấu $^t\omega_M: (M_{(S)})^{**} \to ((M^*)_{(S)})^*$, suy ra bằng hợp thành một đẳng cấu chính tắc:

$$
\phi = (t\omega_M^{-1}) \circ (\omega_{M^*}): (M^{**})_{(S)} \to (M_{(S)})^{**}
$$

sao cho, theo ký hiệu ở trên:

(1)

$$
\langle \omega_M(x^* \otimes 1), \phi(x^{**} \otimes 1) \rangle = \rho(\langle x^*, x^{**} \rangle).
$$

Bây giờ ta xét đồng cấu chính tắc $c_M: M \to M^{**}$ và chỉ ra rằng đồng cấu hợp thành:

(2)

$$
\psi: M_{(S)} \xrightarrow{c_M \otimes 1} (M^{**})_{(S)} \longrightarrow (M_{(S)})^{**}
$$

chính là đồng cấu chính tắc $c_{M_{(S)}}$. Điều này theo ngay lập tức từ (1), cho các hệ thức:

$$
\langle \omega_M(x^* \otimes 1), \psi(x \otimes 1) \rangle = \rho(\langle x^*, c_M(x) \rangle)
$$
$$
= \rho(\langle x, x^* \rangle) = \langle x \otimes 1, \omega_M(x^* \otimes 1) \rangle
$$

và từ việc các phần tử $\omega_M(x^* \otimes 1)$ sinh ra $(M_{(S)})^*$. Như vậy, giả thiết rằng M là phản xạ có nghĩa là $c_M$ là song ánh, do đó $c_M \otimes 1$ cũng vậy và vì thế $\psi = c_{M_{(S)}}$ là song ánh, điều này chứng minh mệnh đề.

### 3. PHÉP DỰNG ĐỊA PHƯƠNG CỦA CÁC MÔĐUN PHẢN XẠ

Ta giữ ký hiệu và các giả thiết của no. 2. Ta sẽ nói rằng một tính chất đúng *với hầu hết* $p \in P$ nếu tập hợp các $p \in P$ mà đối với chúng tính chất đó không đúng *là hữu hạn*.

#### Định lý 3 {#ac-vii-s4-thm-3 .statement}

*Cho V là một không gian vectơ hạng hữu hạn trên K và M là một dàn của V đối với A.*

(i) *Cho N là một dàn của V đối với A; khi đó, với mọi iđêan nguyên tố p của A, $N_p$ là một dàn của V đối với A, và, với hầu hết* $p \in P, N_p = M_p$.

(ii) *Ngược lại, giả sử đã cho với mọi* $p \in P$ *một dàn* $N(p)$ *của V đối với A, sao cho* $N(p) = M_p$ *với hầu hết* $p \in P$. *Khi đó* $N = \bigcap N(p)$ *là một dàn phản xạ của A đối với A và đó là dàn phản xạ duy nhất* $N'$ *của V đối với A sao cho* $N'_p = N(p)$ *với mọi* $p \in P$.

(i) Khẳng định thứ nhất suy ra từ no. 1, Mệnh đề 4. Hơn nữa, tồn tại $x, y$ trong $\mathbf{K}^*$ sao cho $xN \subset M \subset yN$ (no. 1, Mệnh đề 2); ta biết rằng, với hầu hết $p \in P, v_p(x) = v_p(y) = 0$ ($\S 1$, no. 6, Định lý 4), điều này cho thấy $x$ và $y$ là khả nghịch trong A, và do đó $M_p = N_p$.

(ii) Ta có thể thay thế $M$ bằng $x^{-1}M$ với $x \neq 0$ trong $A$ và giả sử rằng $N(p) \subset M$, với mọi $p \in P$. Gọi $p_1, \ldots, p_h$ là các phần tử của $P$ sao cho $N(p) = M$, với $p$ phân biệt với các $p_i$ ($1 \leq i \leq h$); ta viết:

$$
Q = M \cap N(p_1) \cap \cdots \cap N(p_h).
$$

Vì mỗi $N(p_i)$ đều chứa một dàn tự do đối với $A_{p_i}$, nên nó chứa *a fortiori* một dàn của $V$ đối với $A$, do đó $Q$ chứa một dàn của $V$ đối với $A$ (no. 1, Mệnh đề 3) và, vì $Q$ được chứa trong $M$, $Q$ là một dàn đối với $A$. Để chứng minh rằng $Q_p = N(p)$ với mọi $p \in P$, ta sẽ dùng bổ đề sau:

#### Bổ đề 1 {#ac-vii-s4-lem-1 .statement}

*Cho $p$ và $p'$ là hai iđêan nguyên tố của $A$ sao cho (0) là iđêan nguyên tố duy nhất của $A$ được chứa trong $p \cap p'$. Khi đó, với mọi môđun con-A $E$ của $V$, $(E_p)_{p'} = K.E.$*

Đặt $S$ là tập con nhân $(A - p)(A - p')$ của $A$; theo Chương II, $\S 2$, no. 3, Mệnh đề 7, $(E_p)_{p'} = S^{-1}E$. Hơn nữa, $A \subset S^{-1}A \subset K$; các iđêan nguyên tố của $S^{-1}A$ tương ứng với các iđêan nguyên tố $q$ của $A$ sao cho $q \cap S = \varnothing$ (Chương II, $\S 2$, no. 5, Mệnh đề 11) và theo giả thiết thì (0) là iđêan nguyên tố duy nhất của $A$ không cắt $S$; do đó $S^{-1}A = K$ và $S^{-1}E = K.E.$

Bây giờ ta trở lại chứng minh của (ii). Nếu $p \in P$ phân biệt với các $p_i$ ($1 \leq i \leq h$), thì Bổ đề 1 áp dụng cho $N(p_i)$ cho $((N(p_i))_{p_i})_p = (K.N(p_i))_p = V$, vì $p_i$ và $p$ có chiều cao 1. Khi đó

$$
Q_p = M_p \cap (N(p_1))_p \cap \cdots \cap (N(p_h))_p = M_p = N(p)
$$

(Chương II, $\S 2$, no. 4). Mặt khác, nếu $p$ bằng $p_i$ ($1 \leq i \leq h$), thì $(N(p_i))_{p_j} = V$ với $i \neq j$ theo lập luận trên và $(N(p_i))_{p_i} = N(p_i)$, do đó

$$
Q_{p_i} = M_{p_i} \cap N(p_i) = N(p_i).
$$

Vậy ta đã chứng minh được rằng $Q_p = N(p)$ với mọi $p \in P$. Khi đó

$$
N = Q^{**} = \bigcap_{p \in P} Q_p
$$

là phản xạ và thỏa mãn các hệ thức $N_p = Q_p = N(p)$ với mọi $p \in P$; tính duy nhất suy ra ngay lập tức từ Định lý 2 của no. 2.

#### Nhận xét {#ac-vii-s4-n3-rem-1 .statement}

Cho $L$ là một dàn tự do của $V$ đối với $A$. Vì $A$, là một miền iđêan chính đối với $p \in P$, $N(p)$ là một A-môđun tự do có cùng hạng với $L$ và tồn tại $u(p) \in \mathbf{GL}(V)$ sao cho $u(p)(L,) = N;$; hơn nữa điều kiện này xác định $u(p)$ sai khác bởi phép nhân bên phải với một phần tử của $\mathbf{GL}(L_p)$. Điều kiện $N(p) = L$, với hầu hết $p \in P$ có nghĩa là tất yếu $u(p) \in \mathbf{GL}(L_p)$ với hầu hết $p \in P$. Các họ $(u(p))_{p \in P}$ thỏa mãn tính chất sau tạo thành một nhóm nhân $\mathbf{GL}_a(V)$ chứa như một nhóm con tích $\prod_{p \in P} \mathbf{GL}(L_p)$. Khi đó Định lý 3 cho thấy rằng *tập hợp các dàn phản xạ của V tương ứng song ánh chính tắc với không gian thuần nhất* $\mathbf{GL}_a(V)/\prod_{p \in P} \mathbf{GL}(L_p)$. Nếu chọn một cơ sở $(e_i)_{1 \leq i \leq n}$ của L trên A, $\mathbf{GL}(V)$ (tương ứng $\mathbf{GL}(L_p)$) được đồng nhất với nhóm các ma trận khả nghịch $\mathbf{GL}(n, K)$ (tương ứng $\mathbf{GL}(n, A, )$) và nhóm $\mathbf{GL}_a(V)$ với nhóm các hệ ma trận cấp $n$, $(U(p))_{p \in P}$, sao cho $U(p) \in \mathbf{GL}(n, K)$ với mọi $p \in P$ và $U(p) \in \mathbf{GL}(n, A_p)$ với hầu hết $p \in P$. Nếu A là một miền Dedekind, nhóm $\mathbf{GL}_a(V)$ cũng được đồng nhất với nhóm $\mathbf{GL}(n, A)$, trong đó A là vành các adèle hạn chế ($\S 2$, no. 4).

### 4. GIẢ ĐẲNG CẤU

Ta giữ các ký hiệu và giả thiết của các số 2 và 3.

#### Mệnh đề 9 {#ac-vii-s4-prop-9 .statement}

*Cho M là một A-môđun hữu hạn sinh. Các điều kiện sau là tương đương*:

(a) $M_p = 0$ với *mọi iđêan nguyên tố* $p$ có chiều cao $\leq 1$.
(b) *Linh hóa tử* $a \triangleleft M$ *là một iđêan* $\neq (0)$ *và* $A : a = A$ (*A*: $a$ ký hiệu, như trong $\S 1$, no. 1, *tập hợp các* $x \in K$ *sao cho* $xa \in A$).

Ta biết (Chương II, $\S 2$, no. 2, Hệ quả 2 của Mệnh đề 4) rằng điều kiện $M_p = 0$ tương đương với $a + p$ và do đó tương đương với $aA_p = A$, (Chương II, $\S 2$, no. 5, *Nhận xét*); mặt khác, với mọi iđêan nguyên $b \neq 0$ của A, quan hệ "*$bA_p = A$, với mọi $p \in P$*" tương đương với $\operatorname{div} b = \operatorname{div} A = 0$ trong $D(A)$ ($\S 1$, no. 4, Mệnh đề 7), hoặc cũng tương đương với $\operatorname{div}(A : b) = 0$ và, vì $A : b$ là divisorial ($\S 1$, no. 1, Mệnh đề 1), quan hệ này cũng tương đương với $A : b = A$. Khi đó mệnh đề suy ra bằng cách ghi nhận rằng nói $a \notin p$ với $p = (0)$ có nghĩa là $a \neq (0)$.

*Nhận xét* (1) Các điều kiện tương đương của Mệnh đề 9 cũng có nghĩa là $\operatorname{Ass}(M)$ không chứa iđêan nguyên tố nào có chiều cao $\leq 1$. *Chúng cũng có thể được diễn giải bằng cách nói rằng* $\operatorname{Supp}(M)$ *có đối chiều* $\geq 2$ *trong* $\operatorname{Spec}(A)$. \*

#### Định nghĩa 2 {#ac-vii-s4-def-2 .statement}

*Một A-môđun M được gọi là giả-không nếu nó sinh hữu hạn và thỏa mãn các điều kiện tương đương của Mệnh đề 9.*

Định nghĩa này và Mệnh đề 9 cho thấy rằng một A-môđun giả-không là một *A-môđun xoắn*; đảo lại là sai.

*Ví dụ*
(1) Nếu A là một miền Dedekind, mọi iđêan nguyên tố của A đều có chiều cao $\leq 1$; khi đó nói rằng M là giả-không có nghĩa là $\operatorname{Supp}(M) = \varnothing$ và do đó $M = 0$ (Chương 11, $\S 4$, no. 4).

(2) Cho $k$ là trường và $A = k[X, Y]$ là vành đa thức trên $k$ theo hai ẩn số; nếu $m$ là iđêan cực đại $AX + AY$ của $A$, thì A-môđun $A/m$ là giả-không; thật vậy linh hóa tử của nó là $m$ không có chiều cao $\leq 1$ vì nó chứa các iđêan nguyên tố chính $AX$ và $AY$ và phân biệt với chúng; do đó $A : m = A$ (\S 1, no. 6, Hệ quả 1 của Định lý 3).

#### Định nghĩa 3 {#ac-vii-s4-def-3 .statement}

*Cho $M$ và $N$ là hai $A$-môđun và $f : M \to N$ một đồng cấu. Ta gọi $f$ là giả-đơn ánh (resp. giả-toàn ánh giả-không) nếu $\mathrm{Ker}(f)$ (resp. $\mathrm{Coker}(f)$, $\mathrm{Im}(f)$) là giả-không; ta gọi $f$ là giả-song ánh nếu nó vừa giả-đơn ánh vừa giả-toàn ánh.*

Một đồng cấu giả-song ánh cũng được gọi là một *giả-đẳng cấu*.

Giả sử rằng $M$ và $N$ sinh hữu hạn; khi đó, để $f : M \to N$ là giả-đơn ánh (resp. giả-toàn ánh, giả-không), điều kiện cần và đủ là, với mọi $p \in P \cup \{\{0\}\}$, $f_p : M_p \to N_p$, là đơn ánh (resp. toàn ánh, không); điều này suy ra từ tính phẳng của A-môđun $A$, (xem Chương I, \S 2, no. 3, *Nhận xét 2*).

*Ví dụ (3)* Cho $M$ là một A-môđun không xoắn sinh hữu hạn; khi đó ánh xạ chính tắc $c_M : M \to M^{**}$ từ $M$ vào đối ngẫu kép của nó là một *giả đẳng cấu*. Thật vậy, $M$ được đồng nhất với một dàn của $V = M \otimes_A K$ (no. 1, Mệnh đề 1); ta đã thấy rằng $M_p = M_p^{**}$ với mọi $p \in P$ (no. 2, Ví dụ 2) và, với $p = 0$, $M_p$ và $M_p^{**}$ đều bằng $V$.

#### Định lý 4 {#ac-vii-s4-thm-4 .statement}

*Cho $E$ là một A-môđun sinh hữu hạn, $T$ là môđun con xoắn của $E$ và $M = E/T$. Tồn tại một giả đẳng cấu*

$$
f : E \to T \times M.
$$

Trước hết ta sẽ chứng minh hai bổ đề.

#### Bổ đề 2 {#ac-vii-s4-lem-2 .statement}

*Cho $(p_i)_{1 \leq i \leq k}$ là một họ hữu hạn khác rỗng các iđêan nguyên tố của $A$ có chiều cao 1 và đặt $S = \bigcap_i (A - p_i)$; khi đó vành $S^{-1}A$ là một miền iđêan chính.*

$S^{-1}A$ là một vành nửa địa phương mà các iđêan cực đại là các $m_i = p_i S^{-1}A$ với $1 \leq i \leq k$, vành địa phương $(S^{-1}A)_{m_i}$ đẳng cấu với $A$, (Chương 11, \S 3, no. 5, Mệnh đề 17) và do đó là một vành định giá rời rạc. Vậy vành $S^{-1}A$ là một miền Dedekind (\S 2, no. 2, Định lý 1 (f)) và, vì nó là nửa địa phương, nó là một miền iđêan chính (\S 2, no. 2, Mệnh đề 1).

#### Bổ đề 3 {#ac-vii-s4-lem-3 .statement}

*Tồn tại một đồng cấu $g : E \to T$ mà hạn chế của nó trên $T$ vừa là một phép vị tự vừa là một giả đẳng cấu.*

Gọi $a$ là linh hóa tử của $T$; vì $T$ là một A-môđun xoắn sinh hữu hạn, nên $a \neq 0$. Gọi $p_i$ ($1 \leq i \leq k$) là các iđêan nguyên tố chiều cao 1 chứa $a$ (chúng có số lượng hữu hạn ($§\ 1$, no. 6, Định lý 4)); nếu số lượng này bằng 0 thì T là giả-không (Mệnh đề 9(a)) và ta có thể lấy $g = 0$. Nếu không, đặt $S = \bigcap_i (A - p_i)$; theo Bổ đề 2, $S^{-1}A$ là một miền iđêan chính và do đó $S^{-1}M$, là một $S^{-1}A$-môđun không xoắn sinh hữu hạn, là *tự do* (*Đại số*, Chương VII, §4, no. 3, Hệ quả 2 của Định lý 2) và, vì $S^{-1}M = (S^{-1}E)/(S^{-1}T)$, nên $S^{-1}T$ là một nhân tử trực tiếp của $S^{-1}E$ (*Đại số*, Chương II, §1, no. 11, Mệnh đề 21). Bây giờ,

$$
\operatorname{Hom}_{S^{-1}A}(S^{-1}E, S^{-1}T) = S^{-1} \operatorname{Hom}_A(E, T)
$$

(Chương II, §2, no. 7, Mệnh đề 19); do đó tồn tại $s_0 \in S$ và $g_0 \in \operatorname{Hom}_A(E, T)$ sao cho $s_0^{-1}g_0$ là một phép chiếu từ $S^{-1}E$ lên $S^{-1}T$. Nếu $h_0 \in \operatorname{Hom}_A(T, T)$ ký hiệu hạn chế của $g_0$ trên $T$, thì do đó tồn tại $s_1 \in S$ sao cho $s_1 h_0(x) = s_1 s_0 x$ với mọi $x \in T$; đặt $s = s_1 s_0$, $g = s_1 g_0$, $h = s_1 h_0$, khi đó $h$ là phép vị tự tỉ số $s$ trên $T$ và là hạn chế của $g$ trên $T$. Còn phải kiểm tra rằng $h$ là một giả đẳng cấu. Bây giờ, nếu $p = 0$ hoặc nếu $p \in P$ phân biệt với các $p_i$ ($1 \leq i \leq k$), thì $T_p = 0$ (Chương II, §4, no. 4, Mệnh đề 17) và $h,\ : T_p \to T_p$ là một đẳng cấu; trái lại, nếu $p$ bằng một trong các $p_i$ ($1 \leq i \leq k$), thì $s$ khả nghịch trong $A$, và $h_{,,}$, là phép vị tự tỉ số $s$ trên $T_{p_i}$, cũng là một đẳng cấu, điều này hoàn tất chứng minh của Bổ đề 3.

Bây giờ chúng ta chứng minh Định lý 4. Cho $g : E \to T$ là một đồng cấu thỏa mãn các tính chất của Bổ đề 3; gọi $h$ là hạn chế của $g$ trên $T$ và gọi $x$ là phép chiếu chính tắc của $E$ lên $M$. Ta chứng tỏ rằng đồng cấu $f = (g, x) : E \to T \times M$ giải bài toán. Ta có biểu đồ giao hoán:

$$
\begin{array}{ccccccccc}
0 & \longrightarrow & T & \longrightarrow & E & \longrightarrow & M & \longrightarrow & 0 \\
& & \downarrow h & & \downarrow f & & \downarrow I_M & & \\
0 & \longrightarrow & T & \longrightarrow & T \times M & \longrightarrow & M & \longrightarrow & 0
\end{array}
$$

trong đó các hàng là khớp. Biểu đồ con rắn (Chương I, §1, no. 4, Mệnh đề 2) cho dãy khớp:

$$
0 \to \operatorname{Ker}(h) \to \operatorname{Ker}(f) \to 0 \to \operatorname{Coker}(h) \to \operatorname{Coker}(f) \to 0
$$

và do đó $\operatorname{Ker}(f)$ đẳng cấu với $\operatorname{Ker}(h)$ và $\operatorname{Coker}(f)$ đẳng cấu với $\operatorname{Coker}(h)$. Vì $h$ là một giả đẳng cấu, nên $f$ cũng vậy.

Có thể nói rằng "xét đến giả đẳng cấu" thì Định lý 4 quy việc nghiên cứu các $A$-môđun sinh hữu hạn về một phía là việc nghiên cứu các môđun không xoắn và về phía kia là việc nghiên cứu các môđun xoắn. Hơn nữa, ta đã thấy ở trên (*Ví dụ 3*) rằng một môđun không xoắn là giả đẳng cấu với song đối ngẫu của nó và do đó với một môđun *phản xạ*. Còn đối với các môđun xoắn, có kết quả sau đây, xác định chúng xét đến giả đẳng cấu:

#### Định lý 5 {#ac-vii-s4-thm-5 .statement}

Cho T là một A-môđun xoắn sinh hữu hạn. Tồn tại hai họ hữu hạn $(n_i)_{i \in I}$ và $(p_i)_{j \in I}$, trong đó các $n_i$ là những số nguyên $\geq 1$ và các $p_i$ là những iđêan nguyên tố của $A$ có chiều cao 1 sao cho, nếu viết $T' = \bigoplus_{i \in I} A/p_i^{n_i}$, thì tồn tại một giả đẳng cấu từ $T$ đến $T'$. Hơn nữa, các họ $(n_i)_{i \in I}$ và $(p_i)_{i \in I}$ có tính chất này là duy nhất, sai khác nhiều nhất bởi một song ánh của tập chỉ số, và các $p_i$ chứa linh hóa tử của $T$.

Tính duy nhất: Thật vậy, giả sử $T \to T'$ là một giả đẳng cấu và $p \in P, f_p : T, \to T'_p$ là một đẳng cấu. Khi đó, $T'_p$ là tổng trực tiếp của các $A_p/p^{n_i}A_p$, tổng lấy theo các chỉ số $i$ sao cho $p_i = p$; do đó các $p^{n_i}A_p$ là các *ước số sơ cấp* của A-môđun xoắn $T$, (*Algebra*, Chương VII, § 4, no. 7); tính duy nhất của chúng đã được chứng minh trong *Algebra*, Chương VII, § 4, no. 7, Mệnh đề 7.

Sự tồn tại: Ta có thể chỉ xét trường hợp $T \neq 0$. Gọi $a$ là linh hóa tử (khác không và phân biệt với $A$) của $T$, gọi $p_i$ ($1 \leq i \leq k$) là các iđêan nguyên tố của $A$ có chiều cao 1 chứa $a$ (chúng chỉ có hữu hạn về số lượng ($§ 1$, no. 6, Định lý 4)) và đặt $S = \bigcap_i (A - p_i)$. Vành nửa địa phương $A' = S^{-1}A$ là một miền iđêan chính (Bổ đề 2) và có các iđêan cực đại là $m_i = p_iA'$; vì $S^{-1}T$ là một $A$-môđun xoắn sinh hữu hạn, nó đẳng cấu với một tổng trực tiếp hữu hạn $\bigoplus_{j \in I} A'/m_{\phi(j)}^{n_j}$, trong đó $\phi$ là một ánh xạ từ một tập hợp hữu hạn $I$ vào $[1, k]$ (*Algebra*, Chương VII, § 4, no. 7, Mệnh đề 7); vì $A'/m_{\phi(j)}^{n_j}$ đẳng cấu với $S^{-1}(A/p_{\phi(j)}^{n_j})$ (Chương II, § 2, no. 4), ta đã thu được một $A$-môđun xoắn $T'$ thuộc kiểu mong muốn và một đẳng cấu $f_0$ từ $S^{-1}T$ lên $S^{-1}T'$. Vì $\operatorname{Hom}_{S^{-1}A}(S^{-1}T, S^{-1}T')$ bằng $S^{-1} \operatorname{Hom}_A(T, T')$ (Chương 11, § 2, no. 7, Mệnh đề 19), tồn tại $s \in S$ và một đồng cấu $f : T \to T'$ sao cho $f_0 = s^{-1}f$. Còn phải chứng minh rằng $f$ là một giả đẳng cấu: thật vậy, nếu $p = 0$ hoặc nếu $p \in P$ phân biệt với các $p_i$, thì $T_p = T'_p = 0$ (Chương II, § 4, no. 4, Mệnh đề 17); ngược lại, nếu $p$ là một trong các $p_i$ ($1 \leq i \leq k$), thì $s$ khả nghịch trong $A_p$, và, vì $f_{p_i} = s(f_0)_{p_i}$ và $(f_0)_{p_i}$ là một đẳng cấu từ $T_{p_i} = (S^{-1}T)_{m_i}$ lên $T'_{p_i} = (S^{-1}T')_{m_i}$, nên $f_{p_i}$ cũng vậy.

Nhận xét (2) Trong mệnh đề của Định lý 5, các môđun $A/p_i^{n_i}$ có thể được thay bởi $A/p_i^{(n_i)}$ ($§ 1$, no. 4, Mệnh đề 8). Với mọi $p \in P$, ánh xạ chính tắc $g : A/p^n \to A/p^{(n)} = A/(A \cap p^nA_p)$ là một giả đẳng cấu, vì, với mọi $q \in P$ phân biệt với $p$, $A_q/p^nA_q = A_q/p^{(n)}A_q = 0$ và $A_p/p^nA_p = A_p/p^{(n)}A_p$.

\* Cho một dãy khớp các $A$-môđun, $E \to F \to G$, nếu $E$ và $G$ là giả-không thì $F$ cũng vậy, như suy ra từ Định nghĩa 2 và Chương II, §2, no. 4, Định lý 1. Theo ngôn ngữ của các phạm trù, khi đó ta có thể nói rằng, trong phạm trù $\mathcal{C}$ các $A$-môđun, phạm trù con $\mathcal{C}'$ của các môđun giả-không là *đầy đủ* và khi đó ta có thể định nghĩa phạm trù *thương* $\mathcal{C}/\mathcal{C}'$: các đối tượng trong phạm trù này cũng là các $A$-môđun nhưng tập các cấu xạ từ $E$ đến $F$ (với $E, F$ trong $\mathcal{C}/\mathcal{C}'$) là giới hạn trực tiếp của tập các nhóm giao hoán $\mathrm{Hom}_A(E', F')$, trong đó $E'$ (tương ứng $F'$) chạy qua tập các môđun con của $E$ (tương ứng tập các môđun thương $F/F''$ của $F$) sao cho $E/E'$ (tương ứng $F''$) là giả-không. Dĩ nhiên, với mọi cặp có thứ tự các $A$-môđun $E, F$, có một đồng cấu chính tắc $\mathrm{Hom}_{\mathcal{E}}(E, F) \to \mathrm{Hom}_{\mathcal{E}/\mathcal{E}'}(E, F)$. Nói rằng một đồng cấu $u \in \mathrm{Hom}_A(E, F)$ là giả-không (tương ứng giả-đơn ánh, giả-toàn ánh, giả-song ánh) có nghĩa là ảnh chính tắc của nó trong $\mathrm{Hom}_{\mathcal{E}/\mathcal{E}'}(E, F)$ là không (tương ứng một đơn cấu, một toàn cấu, một đẳng cấu). \*

### 5. CÁC ƯỚC GẮN VỚI CÁC MÔĐUN XOẮN

Ta giữ cùng các ký hiệu và giả thiết như trong các số 2, 3 và 4. Nhắc lại rằng $D(A)$ (hay đơn giản là $D$) ký hiệu *nhóm ước* của $A$, viết theo lối cộng: ta biết (\S 1, no. 3, Định lý 2) rằng $D$ là $\mathbf{Z}$-môđun tự do sinh bởi các phần tử của $P$.

Cho $T$ là một $A$-môđun xoắn sinh hữu hạn. Với mọi $p \in P$, $T_p$ là một $A_p$-môđun xoắn sinh hữu hạn và do đó là một môđun có *độ dài hữu hạn* (Chương IV, \S 2, no. 5, Hệ quả 2 của Mệnh đề 7); ta sẽ ký hiệu độ dài này bởi $l_p(T)$. Mặt khác $T_p = 0$ với mọi $p$ không chứa linh hóa tử của $T$ và do đó với hầu hết mọi $p$ (\S 1, no. 6, Định lý 4), điều này biện minh cho định nghĩa sau:

#### Định nghĩa 4 {#ac-vii-s4-def-4 .statement}

*Nếu $T$ là một $A$-môđun xoắn sinh hữu hạn, thì ước:*

$$
\chi(T) = \sum_{p \in P} l_p(T) \cdot p.
$$

*được gọi là nội dung của $T$*.

#### Mệnh đề 10 {#ac-vii-s4-prop-10 .statement}

(i) *Cho $0 \to T_1 \to T_2 \to T_3 \to 0$ là một dãy khớp các $A$-môđun xoắn sinh hữu hạn. Khi đó*

$$
\chi(T_2) = \chi(T_1) + \chi(T_3).
$$

(ii) *Nếu tồn tại một giả-đẳng cấu $f : T_1 \to T_2$, thì $\chi(T_1) = \chi(T_2)$.*

(iii) *Để có $\chi(T) = 0$, điều kiện cần và đủ là $T$ giả-không.*

Xét theo Định nghĩa 4, chỉ cần xét với mỗi $p \in P$ các giá trị của $l_p$ đối với các môđun xoắn đang xét. Khi đó tính chất (i) suy ra từ Chương II, \S 2, no. 4, Định lý 1 và tính cộng được của các độ dài trong một dãy khớp (*Đại số* Chương 11, \S 1, no. 10, Mệnh đề 16) và các tính chất (ii) và (iii) suy ra ngay lập tức từ các định nghĩa trong no. 4.

#### Hệ quả {#ac-vii-s4-n5-cor-1 .statement}

*Cho $0 \to T_n \to T_{n-1} \to \ldots \to T_0 \to 0$ là một dãy khớp các $A$-môđun xoắn sinh hữu hạn. Khi đó* $\sum_{i=0}^n (-1)^i \chi(T_i) = 0$.

Xét theo Chương II, \S 2, no. 4, Định lý 1, điều này lại suy ra từ tính chất tương tự của các $l_p$ (*Đại số*, Chương II, \S 1, no. 10, Hệ quả 3 của Mệnh đề 16).

Nhắc lại (Chương II, § 5, no. 4) rằng ta có thể nói về *tập hợp* $F(A)$ các *lớp của các A-môđun hữu hạn sinh* đối với quan hệ đẳng cấu; với mọi A-môđun hữu hạn sinh M, ký hiệu $\mathrm{cl}(M)$ là phần tử tương ứng của $F(A)$; ta sẽ ký hiệu bởi $T(A)$ tập con của $F(A)$ gồm các lớp của các A-môđun xoắn hữu hạn sinh. Rõ ràng $\chi$ xác định một ánh xạ từ $T(A)$ vào $D(A)$, cũng được ký hiệu bởi $\chi$, sao cho $\chi(\mathrm{cl}(T)) = \chi(T)$.

#### Mệnh đề 11 {#ac-vii-s4-prop-11 .statement}

*Cho G là một nhóm giao hoán viết theo phép cộng và $\phi : T(A) \to G$ là một ánh xạ; với mọi A-môđun xoắn hữu hạn sinh T, ta cũng viết, do lạm dụng ngôn ngữ, $\phi(T) = \phi(\mathrm{cl}(T))$. Giả sử rằng các điều kiện sau được thỏa mãn:
(1) *Nếu* $0 \to T_1 \to T_2 \to T_3 \to 0$ *là một dãy khớp của các A-môđun xoắn hữu hạn sinh, thì* $\phi(T_2) = \phi(T_1) + \phi(T_3)$.
(2) *Nếu* T *là giả-không, thì* $\phi(T) = 0$.
*Khi đó tồn tại một đồng cấu duy nhất* $\theta : D(A) \to G$ *sao cho* $\phi = \theta \circ \chi$.*

Vì $\chi(A/p) = p$ với mọi p, tất yếu $\theta(p) = \phi(A/p)$ với mọi $p \in P$, điều này chứng minh tính duy nhất của $\theta$, vì các phần tử của P tạo thành một cơ sở của $D(A)$. Ngược lại, cho $\theta$ là đồng cấu từ $D(A)$ vào G sao cho $\theta(p) = \phi(A/p)$ với mọi $p \in P$ và hãy chỉ ra rằng nó giải quyết bài toán. Vì điều này, ta viết

$$
\psi(T) = \phi(T) - \theta(\chi(T))
$$

với mọi A-môđun xoắn hữu hạn sinh T; rõ ràng các điều kiện (1) và (2) cũng được thỏa mãn nếu thay $\phi$ bởi $\psi$. Mặt khác, $\psi(A/p) = 0$ nếu $p \in P$; nếu p là một iđêan nguyên tố $\neq 0$ và không thuộc P, thì linh hóa tử của $A/p$ không được chứa trong bất kỳ iđêan nào của P, do đó (no. 4, Định lý 5) $A/p$ là giả-không và vì thế $\psi(A/p) = 0$. Như vậy, mọi A-môđun xoắn hữu hạn sinh T đều thừa nhận một chuỗi phân tích mà các thương số của nó đẳng cấu với các A-môđun dạng $A/p$, trong đó $p \in \mathrm{Supp}(T)$ (Chương IV, § 1, no. 4, Định lý 1 và 2), và do đó $p \neq 0$ vì T là một môđun xoắn. Bằng quy nạp theo độ dài của chuỗi phân tích này, ta suy ra (xét đến tính chất (1) đối với $\psi$) rằng $\psi(T) = 0$.

\* Ta có thể, như trong no. 4, xét phạm trù thương $\mathcal{T}/\mathcal{T}'$ của phạm trù $\mathcal{T}$ các A-môđun xoắn hữu hạn sinh theo phạm trù con đầy đủ $\mathcal{T}'$ gồm các A-môđun xoắn hữu hạn sinh giả-không. Theo ngôn ngữ các phạm trù Abel, Mệnh đề 11 khi đó biểu thị sự kiện rằng *nhóm Grothendieck* của phạm trù Abel $\mathcal{T}/\mathcal{T}'$ đẳng cấu chính tắc với $D(A)$. \*

#### Mệnh đề 12 {#ac-vii-s4-prop-12 .statement}

*Nếu a là một iđêan $\neq 0$ của A,

$$
\chi(A/a) = \chi((A : a)/A) = \mathrm{div}\, a.
$$

Cho $p \in P$. Khi đó $aA_p = p^{n_p}A_p$ trong đó $n_p \geq 0$, vì $A_p$ là một vành định giá rời rạc. *Vì* $(A/a)_p = A_p/aA_p,\ l_p(A/a) = n_p$, do đó $\chi(A/a) = \sum_{p \in P} n_p p = \mathrm{div}\, a$ (§ 1, no. 4, Mệnh đề 7).

Mặt khác, $(A : a) = A ; aA_p = p^{-n_p}A_p$, do đó $l_p((A : a)/A) = n_p$ và ta kết luận theo cùng một cách.

### 6. BẤT BIẾN TƯƠNG ĐỐI CỦA HAI MẠNG LƯỚI

Ta giữ ký hiệu và các giả thiết của các no. 2 đến 5. Cho V là một không gian vectơ hạng hữu hạn $n$ trên $K$ và M là một dàn của V đối với A. Cho W là lũy thừa ngoài $\bigwedge^n V$, là một không gian vectơ *hạng 1* trên $K$, và ký hiệu $M_w$ là dàn của W sinh bởi ảnh của $M^n$ dưới ánh xạ chính tắc $V^n \to \bigwedge^n V$ (no. 1, Mệnh đề 3 (iii); chú ý rằng $M_w$ không nhất thiết đẳng cấu với $\bigwedge^n M$ (*Algebra*, Chương III, § 5, Bài tập 9)). Nếu $e$ là một cơ sở của W trên K, ta có thể viết $M = a.e$, trong đó a là một iđêan phân thức $\neq 0$ của A.

Cho $M'$ là một dàn khác của V và viết $M'_w = a'.e$, trong đó $a'$ là một iđêan phân thức $\neq 0$ của A; ước $\operatorname{div}(a) - \operatorname{div}(a')$ *không phụ thuộc vào lựa chọn cơ sở* $e$ của W, vì a và $a'$ bị nhân với cùng một phần tử của $K^*$ khi thay đổi cơ sở; ta sẽ viết $\chi(M, M') = \operatorname{div}(a) - \operatorname{div}(a')$ và nói rằng ước này là *bất biến tương đối* của $M'$ *đối với* M. Rõ ràng, nếu M, $M', M''$ là ba dàn của V, thì:

(3)
$$
\chi(M, M') + \chi(M', M'') + \chi(M'', M) = 0
$$
(4)
$$
\chi(M, M') + \chi(M', M) = 0.
$$

Với mọi $p \in P$, theo các định nghĩa suy ra ngay lập tức rằng $(M_w)_p = (M_p)_w$; hơn nữa, vì M, khi đó là một A,-môđun *tự do* do A, là một miền iđêan chính, một cơ sở của M, trên A, là một cơ sở của V trên K, do đó $(M_p)_w = \bigwedge^n (M_p)$ (Chương II, § 2, no. 8) và iđêan phân thức $a_p = aA_p$ là một miền iđêan chính. Nếu ta đặt $a_p = p^{n_p}A_p$, $a' = p^{n'_p}A_p$, thì:
$$
\chi(M, M') = \sum_{p \in P} (n_p - n'_p).p,
$$
cũng có thể viết là:
(5)
$$
\chi(M, M') = \sum_{p \in P} \chi(M_p, M'_p)
$$
khi đồng nhất $D(A_p)$ với môđun con-Z của $D(A)$ sinh bởi $p$.

#### Mệnh đề 13 {#ac-vii-s4-prop-13 .statement}

*Cho M là một dàn của V và u là một tự đẳng cấu K của V. Khi đó* :
(6)
$$
-\chi(M, u(M)) = \operatorname{div}(\det(u)).
$$
Với mọi $p \in P$, khi đó $\bigwedge^n (u(M)_p) = \bigwedge^n (u(M_p))$; nếu $(e_i)_{1 \leq i \leq n}$ là một cơ sở của $M_p$, thì
$$
\bigwedge^n (M_p) = A_p \cdot e_1 \text{ } A \text{ } e_2 \text{ } A \ldots A \text{ } e_n,
$$

và $\bigwedge^n (u(M_p)) = A_p \cdot \det(u) e_1 \wedge e_2 \mathbf{A} \ldots \mathbf{A} e_n$, do đó có mệnh đề theo công thức (5).

#### Mệnh đề 14 {#ac-vii-s4-prop-14 .statement}

*Nếu M, M' là hai dàn của V sao cho M' \subset M, M/M' là một A-môđun xoắn sinh hữu hạn và:*

$$
\chi(M, M') = -\chi(M/M').
$$

Rõ ràng M/M' \subset V/M' là một môđun xoắn sinh hữu hạn; mặt khác, với mọi $p \in P$, ta biết (*Algebra*, Chương VII, § 4, số 2, Định lý 1) rằng tồn tại các cơ sở $(e_i)_{1 \leq i \leq n}$ của M, và $(e'_i)_{1 \leq i \leq n}$ của $M'_p$ sao cho $e'_i = \pi^{v_i} e_i$ với $1 \leq i \leq n$ và các số nguyên $v_i \geq 0$, trong đó $\pi$ là một phần tử chuẩn hoá của $A_p$. Do đó (theo ký hiệu đã đưa vào ở trên) $n'_p - n_p = \sum_{i=1}^n v_i$; và mặt khác,

$$(M/M')_p = M_p/M'_p$$ đẳng cấu với A,-môđun xoắn $\bigoplus_{i=1}^n A_p/p^{v_i} A_p$ và do đó độ dài của nó là $\sum_{i=1}^n v_i$, điều này chứng minh mệnh đề, theo (5) và Định nghĩa 4 của no. 5.

#### Hệ quả {#ac-vii-s4-n6-cor-1 .statement}

*Cho L,, L_2 là hai A-môđun tự do cùng hạng n và cho f: L_1 \to L_2 là một đồng cấu. Cho U là ma trận của f đối với các cơ sở của L, và L_2. Để Coker(f) là một A-môđun xoắn, điều kiện cần và đủ là \det(U) \neq 0, và khi đó:*

$$
\chi(\operatorname{Coker}(f)) = \operatorname{div}(\det(U)).
$$

Có thể coi $L_1$ và $L_2$ lần lượt là các mạng trong $V_1 = L_1 \otimes_A K$ và $V_2 = L_2 \otimes_A K$, còn $f$ được mở rộng thành một K-đồng cấu $f_{(K)}: V_1 \to V_2$. Khi đó

$$(\operatorname{Coker}(f))_{(K)} = \operatorname{Coker}(f_{(K)})$$

và nói rằng $\operatorname{Coker}(f)$ là một A-môđun xoắn có nghĩa là $\operatorname{Coker}(f_{(K)}) = 0$; mà điều đó tương đương với việc nói rằng $f_{(K)}$ là toàn ánh hoặc $\det(U) \neq 0$, do đó có mệnh đề thứ nhất. Mặt khác, ta có thể viết $f(L,) = u(L_2)$, trong đó $u$ là một tự đồng cấu của L, có định thức $\det(U)$; vì

$$\operatorname{Coker}(f) = L_2/u(L_2),$$

công thức (8) suy ra từ (7) và (6).

#### Ví dụ {#ac-vii-s4-n6-exa-1 .statement}

Nếu $A = \mathbf{Z}$, nhóm ước của $A$ được đồng nhất với nhóm nhân $\mathbf{Q}_+^*$ của các số hữu tỉ > 0. Với mọi nhóm giao hoán hữu hạn T, $\chi(T)$ là *cấp* của T; hệ quả trên cho thấy cấp của nhóm $\operatorname{Coker}(f)$ bằng *giá trị tuyệt đối* của $\det(U)$ (xem *Algebra*, Chương VII, § 4, no. 7, Hệ quả 3 của Định lý 3).

### 7. CÁC LỚP ƯỚC GẮN VỚI CÁC MÔĐUN SINH HỮU HẠN

Ta giữ ký hiệu và các giả thiết của các số 2 đến 6. Nhắc lại rằng C(A) (hoặc đơn giản là C) ký hiệu nhóm lớp ước của $A$, là thương của $D(A)$ bởi nhóm con các ước chính. Với mọi ước $d \in D$, ta sẽ ký hiệu bởi $c(d)$ lớp của nó trong C.

#### Mệnh đề 15 {#ac-vii-s4-prop-15 .statement}

*Cho M là một A-môđun hữu hạn sinh. Tồn tại một môđun con tự do L của M sao cho M/L là một môđun xoắn và phần tử $c(\chi(M/L))$ của C không phụ thuộc vào môđun con tự do L được chọn.*

Ta viết $S = A - \{0\}$ và đặt $V = S^{-1}M = M \otimes_A K$; nếu $n$ là hạng của V trên K, thì tồn tại $n$ phần tử $e_i$ ($1 \leq i \leq n$) của M sao cho các ảnh chính tắc của chúng trong V tạo thành một cơ sở của V; các phần tử ấy hiển nhiên độc lập tuyến tính trong M và do đó sinh ra một môđun con tự do L của M sao cho $S^{-1}(M/L) = S^{-1}M/S^{-1}L = 0$, vì thế M/L là một môđun xoắn.

Bây giờ giả sử L, là một môđun con tự do khác của M có hạng $n$. Vì $S^{-1}L = S^{-1}L_1$, tồn tại $s \in S$ sao cho $sL_1 \subset L$; do đó ta có thể chỉ cần chứng minh rằng, nếu $L_1 \subset L_2$ là hai môđun con tự do của M có hạng $n$, thì

$$
c(\chi(M/L_1)) = c(\chi(M/L_2)).
$$

Mà $\chi(M/L_1) = \chi(M/L_2) + \chi(L_2/L_1)$ và suy ra từ no. 6, Hệ quả của Mệnh đề 14 rằng $\chi(L_2/L_1)$ là một ước chính và do đó

$$
c(\chi(L_2/L_1)) = 0.
$$

Phần tử $c(\chi(M/L))$ trong phần sau sẽ được ký hiệu là $-c(M)$; ta sẽ nói rằng $c(M)$ là lớp ước gắn với M.

#### Mệnh đề 16 {#ac-vii-s4-prop-16 .statement}

(i) *Cho $0 \to M_1 \xrightarrow{\alpha} M_2 \xrightarrow{g} M_3 \to 0$ là một dãy khớp của các A-môđun hữu hạn sinh. Khi đó*

$$
c(M_2) = c(M_1) + c(M_3).
$$

(ii) *Nếu tồn tại một giả đẳng cấu từ M, tới M,, thì $c(M_1) = c(M_2)$.

(iii) *Nếu T là một môđun xoắn, thì $c(T) = -c(\chi(T))$.

(iv) *Nếu $a \neq 0$ là một iđêan phân thức của K, thì*

$$
c(a) = c(\operatorname{div}(a)).
$$

(v) *Nếu L là một A-môđun tự do, thì $c(L) = 0$.

Để chứng minh (i), xét một môđun con tự do $L_1$ (tương ứng $L_3$) của M, (tương ứng $M_3$) sao cho $M_1/L_1$ (tương ứng $M_3/L_3$) là một môđun xoắn. Vì $L_3$ là tự do và $g$ là toàn ánh, tồn tại trong $g^{-1}(L_3)$ một phần bù tự do $L_{23}$ của $\operatorname{Ker}(g)$ đẳng cấu với $L_3$ (*Đại số*, Chương II, § 1, no. 11, Mệnh đề 21); nhưng $\operatorname{Ker}(g) = f(M_1)$ chứa $f(L_1) = L_{12}$, là môđun tự do vì $f$ là đơn ánh. Tổng $L_2 = L_{12} + L_{23}$ là trực tiếp và do đó $L_2$ là một môđun con *tự do* của $M$. Hơn nữa có biểu đồ giao hoán:

$$
\begin{array}{ccccccccc}
0 & \longrightarrow & L_1 & \longrightarrow & L_2 & \longrightarrow & L_3 & \longrightarrow & 0 \\
0 & \longrightarrow & M_1 & \xrightarrow{f} & M_2 & \xrightarrow{g} & M_3 & \longrightarrow & 0
\end{array}
$$

trong đó các hàng là khớp và các mũi tên thẳng đứng là các đơn ánh. Do đó từ biểu đồ rắn (Chương I, § 1, no. 4, Mệnh đề 2) ta thu được dãy khớp:

$$
0 \to M_1/L_1 \to M_2/L_2 \to M_3/L_3 \to 0.
$$

Vì $M_1/L_1$ và $M_3/L_3$ là các môđun xoắn, dãy khớp này trước hết cho thấy $M_2/L_2$ cũng vậy, rồi tiếp theo, theo Mệnh đề 10 của no. 5, rằng:

$$
\chi(M_2/L_2) = \chi(M_1/L_1) + \chi(M_3/L_3)
$$

điều này chứng minh (i).

Các khẳng định (iii) và (v) là hiển nhiên từ định nghĩa. Ta chứng minh (ii). Vậy cho $f : M_1 \to M_2$ là một giả đẳng cấu và cho $L_1$ là một môđun con tự do của $M_1$ sao cho $M_1/L_1$ là một môđun xoắn. Đặt $L_2 = f(L_1)$; vì $\mathrm{Ker}(f)$ là giả-không, nó là một môđun xoắn, do đó $\mathrm{Ker}(f) \cap L_1 = 0$ và vì vậy $L_2$ là tự do. Gọi $\tilde{f} : M_1/L_1 \to M_2/L_2$ là đồng cấu dẫn xuất từ $f$ bằng cách lấy thương; $\mathrm{Ker}(\tilde{f})$ đẳng cấu với $\mathrm{Ker}(f)$ và $\mathrm{Coker}(\tilde{f})$ đẳng cấu với $\mathrm{Coker}(f)$ và do đó $\tilde{f}$ là một giả đẳng cấu; hơn nữa

$$
\mathrm{Coker}(\tilde{f}) = M_2/f(M_1)
$$

là một môđun xoắn và $f(M_1)/L_2 = \tilde{f}(M_1/L_1)$ cũng vậy, nên $M_2/L_2$ là một môđun xoắn và từ no. 5, Mệnh đề 10 (ii) suy ra rằng

$$
\chi(M_1/L_1) = \chi(M_2/L_2).
$$

Cuối cùng còn phải chứng minh (iv). Cho $x \in K^*$ sao cho $a \subset xA$. Bằng cách xét dãy khớp $0 \to a \to xA \to xA/a \to 0$, ta được

$$
c(a) = c(xA) - c(xA/a) = -c(xA/a)
$$

theo (i) và (v). Nhưng $xA/a$ đẳng cấu với $A/x^{-1}a$, do đó, theo (iii),

$$
c(xA/a) = -c(\chi(A/x^{-1}a)) = -c(\mathrm{div}(x^{-1}a)) = -c(\mathrm{div}(a))
$$

(no. 5, Mệnh đề 12). Điều này hoàn tất chứng minh.

Khi $M$ là một *dàn* của $V$ đối với $A$, $\chi(M/L) = -\chi(M, L)$ (no. 6, Mệnh đề 14); cho $(e_i)_{1 \leq i \leq n}$ là một cơ sở của $L$, $e = e_1 \wedge e_2 \wedge \ldots \wedge e_n$, và

$M_w = a \cdot e$ (ký hiệu của no. 6); khi đó $\chi(M, L) = \operatorname{div}(a)$, do đó $c(M) = c(\operatorname{div}(a))$, điều này tổng quát hóa Mệnh đề 16 (v).

#### Hệ quả 1 {#ac-vii-s4-prop-16-cor-1 .statement}

*Cho* $0 \to M, \xrightarrow{u} M_{n-1} \to \cdots \to M_0 \to 0$ *là một dãy khớp các A-môđun sinh hữu hạn.* Khi đó

$$
\sum_{i=0}^n (-1)^i c(M_i) = 0.
$$

Ta lập luận bằng quy nạp theo $n$, trường hợp $n = 2$ là Mệnh đề 16 (i). Nếu $M'_{n-1} = \operatorname{Coker}(u)$, ta có hai dãy khớp:

$$
\begin{align*}
0 &\to M, \to M_{n-1} \to M'_{n-1} \to 0 \\
0 &\to M'_{n-1} \to M_{n-2} \to \cdots \to M_0 \to 0.
\end{align*}
$$

Dãy thứ nhất cho thấy $M'_{n-1}$ là sinh hữu hạn và giả thiết quy nạp cho

$$
(-1)^{n-1} c(M'_{n-1}) + \sum_{t=0}^{n-a} (-1)^t c(M_t) = 0
$$

và

$$
c(M'_{n-1}) = c(M_{n-1}) - c(M_n),
$$

do đó có hệ quả.

Một dãy khớp

$$
0 \to L_n \to L_{n-1} \to \cdots \to L_0 \to E \to 0
$$

trong đó các $L_i$ ($0 \leq i \leq n$) là các A-môđun *tự do sinh hữu hạn*, được gọi là một *phân giải tự do hữu hạn* của A-môđun E.

#### Hệ quả 2 {#ac-vii-s4-prop-16-cor-2 .statement}

*Nếu một iđêan phân thức ước tính* $a \neq 0$ *của* $\mathbf{A}$ *có một phân giải tự do hữu hạn, thì nó là chính.*

Thật vậy, ta áp dụng Hệ quả 1 cho một phân giải tự do hữu hạn của $a$:

$$
0 \to L_n \to L_{n-1} \to \cdots \to L_0 \to a \to 0.
$$

Theo Mệnh đề 16 (v), $c(a) = 0$ và vì thế, theo Mệnh đề 16 (iv), $\operatorname{div}(a)$ là chính; vì $a$ được giả thiết là ước tính, nó là chính (\S 1, no. 1).

#### Hệ quả 3 {#ac-vii-s4-prop-16-cor-3 .statement}

*Nếu mọi iđêan ước tính* $\neq 0$ *của* $\mathbf{A}$ *đều có một phân giải tự do hữu hạn,* $\mathbf{A}$ *là giai thừa.*

Đây là một hệ quả ngay lập tức của Hệ quả 2 và § 3, no. 1, Định nghĩa 1.

\* Ta sẽ thấy về sau rằng một vành địa phương chính quy thỏa mãn giả thiết của Hệ quả 3 và do đó là *giai thừa.* \*

Nếu M là một A-môđun hữu hạn sinh, ta sẽ ký hiệu *hạng* của nó bởi $r(M)$ (nhớ rằng đó là hạng trên K của $M_{(K)} = M \otimes_A K$); nếu $0 \to M_1 \to M_2 \to M_3 \to 0$ là một dãy khớp các A-môđun hữu hạn sinh, thì dãy

$$
0 \to (M_1)_{(K)} \to (M_2)_{(K)} \to (M_3)_{(K)} \to 0
$$

cũng khớp và do đó $r(M_2) = r(M_1) + r(M_3)$. Ta viết

$$
\gamma(M) = (r(M), c(M)) \in \mathbf{Z} \times C(A);
$$

vì vậy $\gamma$ thỏa mãn tính chất (i) của Mệnh đề 16 và, nếu M là giả-không, thì $\gamma(M) = 0$ (vì M là một môđun xoắn). Tồn tại một ánh xạ duy nhất từ $F(A)$ vào $\mathbf{Z} \times C(A)$, cũng được ký hiệu bởi y, sao cho $\gamma(M) = \gamma(\mathrm{cl}(M))$ với mọi A-môđun hữu hạn sinh M. Ta sẽ thấy rằng các tính chất trên về cơ bản xác định y:

#### Mệnh đề 17 {#ac-vii-s4-prop-17 .statement}

Cho G là một nhóm giao hoán được viết *theo phép cộng* và $\phi$ là một *ánh xạ* từ tập hợp $F(A)$ các lớp của các A-môđun sinh hữu hạn vào G; đối với *mọi* A-môđun sinh hữu hạn M ta cũng viết, do một sự lạm dụng ngôn ngữ, $\phi(M) = \phi(\mathrm{cl}(M))$. *Giả sử* các điều kiện sau được *thỏa mãn*:
  (1) *Nếu* $0 \to M_1 \to M_2 \to M_3 \to 0$ là một dãy khớp *các* A-môđun sinh hữu hạn, thì $\phi(M_2) = \phi(M_1) + \phi(M_3)$.
  (2) *Nếu* T là giả-không, thì $\phi(T) = 0$.
*Khi đó* tồn tại một đồng cấu duy nhất $\theta : Z \times C \to G$ sao cho $\phi = 8 \circ y$.

Theo Mệnh đề 16 (iv), mọi phần tử của $Z \times C$ đều có dạng $(r(M), c(M))$ với một A-môđun sinh hữu hạn M thích hợp nào đó; do đó có tính duy nhất của $\theta$. Ta áp dụng Mệnh đề 11 của no. 5 cho hạn chế của $-\phi$ lên $T(A)$: khi đó tồn tại một đồng cấu $\theta_0 : D \to G$ sao cho

$$
-\phi(T) = \theta_0(\chi(T))
$$

đối với mọi A-môđun xoắn sinh hữu hạn T. Cho x là một phần tử khác không của A; áp dụng tính chất (1) cho dãy khớp:

$$
0 \longrightarrow A \xrightarrow{h_x} A \longrightarrow A/xA \longrightarrow 0
$$

trong đó $h_x$ là phép nhân bởi x, ta được $\phi(A/xA) = 0$, do đó $\theta_0(\mathrm{div}(x)) = 0$. Lấy thương, vì thế $\theta_0$ xác định một đồng cấu $\theta_1 : C \to G$ và $\phi(T) = \theta_1(c(T))$ với mọi A-môđun xoắn T. Bây giờ ta chứng minh rằng đồng cấu $\theta$ được định nghĩa bởi $\theta(n, z) = n.\phi(A) + \theta_1(z)$ giải quyết bài toán. Vì mục đích đó, ta viết $\phi'(M) = \phi(M) - \theta(\gamma(M))$ với mọi A-môđun hữu hạn sinh M; rõ ràng điều kiện (1) vẫn được thỏa mãn nếu thay $\phi$ bằng $\phi'$. Hơn nữa, $\phi'(M) = 0$ khi M là một môđun xoắn hoặc một môđun tự do; nhưng vì với mọi A-môđun hữu hạn sinh M, tồn tại một môđun con tự do L của M sao cho M/L là một môđun xoắn (Mệnh đề 15), tính chất (1) cho thấy rằng $\phi'(M) = 0$ với mọi A-môđun hữu hạn sinh M.

\* Theo ngôn ngữ của các phạm trù Abel, Mệnh đề 17 cho thấy rằng $\mathbf{Z} \times C(A)$ đẳng cấu chính tắc với nhóm Grothendieck của phạm trù thương $\mathcal{F}/\mathcal{F}'$, trong đó $\mathcal{F}$ là phạm trù các A-môđun hữu hạn sinh và $\mathcal{F}'$ là phạm trù con đầy đủ của $\mathcal{F}$ gồm các môđun giả-không. \*

### 8. CÁC TÍNH CHẤT ĐỐI VỚI CÁC MỞ RỘNG HỮU HẠN CỦA VÀNH VÔ HƯỚNG

Trong số này, A và B chỉ hai miền nguyên đóng nguyên Noether sao cho $A \subset B$ và B là một A-môđun hữu hạn sinh, còn K và L lần lượt là các trường phân thức của A và B. Ta sẽ viết div$_A$, $\chi_A$, $c_A$, $\gamma_A$, $r_A$ thay cho div, $\chi$, c, y, r tương ứng khi xét các A-môđun, và dùng các ký hiệu tương tự cho các B-môđun.

Ta biết (\S 1, no. 10) rằng để một iđêan nguyên tố $\mathfrak{p}$ của B có chiều cao 1 thì điều kiện cần và đủ là $\mathfrak{p} = \mathfrak{P} \cap A$ có chiều cao 1; hơn nữa (loc. cit., Mệnh đề 14), với $\mathfrak{p} \in P(A)$, chỉ có hữu hạn iđêan nguyên tố $\mathfrak{P} \in P(B)$ nằm trên $\mathfrak{p}$. Để viết gọn, ta sẽ ký hiệu bởi $\mathfrak{P}|_{\mathfrak{p}}$ quan hệ "“$\mathfrak{P}$ nằm trên $\mathfrak{p}$" (nghĩa là $\mathfrak{p} = \mathfrak{P} \cap A$); khi đó ta sẽ ký hiệu bởi $e_{\mathfrak{P}/\mathfrak{p}}$ hoặc $e(\mathfrak{P}/\mathfrak{p})$ chỉ số phân nhánh $e(v_{\mathfrak{P}}/v_{\mathfrak{p}})$ của định giá $v_{\mathfrak{P}}$ trên định giá $v_{\mathfrak{p}}$ (Chương VI, \S 8, no. 1) và bởi $f_{\mathfrak{P}/\mathfrak{p}}$ hoặc $f(\mathfrak{P}/\mathfrak{p})$ bậc thặng dư $f(v_{\mathfrak{P}}/v_{\mathfrak{p}})$ (loc. cit.); nhắc lại rằng các định giá rời rạc $v_{\mathfrak{p}}$ và $v_{\mathfrak{P}}$ đều được chuẩn hóa và $f_{\mathfrak{P}/\mathfrak{p}}$ là bậc của trường phân thức của $B/\mathfrak{P}$ trên trường phân thức của $A/\mathfrak{p}$. Đặt $n = r_A(B)$, trong đó B được coi như một A-môđun; do đó theo định nghĩa $n = [L:K]$ và, với mọi $\mathfrak{p} \in P(A)$, $n$ cũng là hạng của A,-môđun tự do B với mọi $\mathfrak{P}|_{\mathfrak{p}}$. Khi đó suy ra từ Chương VI, \S 8, no. 5, Định lý 2 rằng với mọi $\mathfrak{p} \in P(A)$:

$$
\sum_{\mathfrak{P}|_{\mathfrak{p}}} e_{\mathfrak{P}/\mathfrak{p}} f_{\mathfrak{P}/\mathfrak{p}} = n.
$$

Như vậy, vì $D(A)$ và $D(B)$ là các $\mathbf{Z}$-môđun tự do, ta định nghĩa một đồng cấu tăng của các nhóm có thứ tự $N : D(B) \to D(A)$ (cũng ký hiệu là $N_{B/A}$), bởi điều kiện:

$$
N(\mathfrak{P}) = f_{\mathfrak{P}/\mathfrak{p}} \cdot \mathfrak{p} \quad \text{với} \quad \mathfrak{P} \in P(B), \quad \text{trong đó} \quad \mathfrak{p} = \mathfrak{P} \cap A.
$$

Mặt khác (\S 1, no. 10, Mệnh đề 14), ta đã định nghĩa một đồng cấu tăng của các nhóm có thứ tự $i : D(A) \to D(B)$ (cũng ký hiệu là $i_{B/A}$), bởi điều kiện:

$$
i(p) = \sum_{\mathfrak{P}|_p} e_{\mathfrak{P}/\mathfrak{p}} \cdot \mathfrak{P} \quad \text{với} \quad p \in P(A).
$$

Rõ ràng với mọi họ $(d_i)$ (tương ứng $(d'_i)$) các ước của A (tương ứng của B):

$$
N(\sup(d'_i)) = \sup(N(d'_i)), \qquad N(\inf(d'_i)) = \inf(N(d'_i))
$$
$$
i(\sup(d_i)) = \sup(i(d_i)), \qquad i(\inf(d_i)) = \inf(i(d_i)).
$$

Công thức (9) cho thấy rằng:

(14) $$ N \circ i = n . 1_{D(A)} $$

Với mọi $a \in A$ (\S 1, no. 10, Mệnh đề 14):

(15) $$ i(\operatorname{div}_A(a)) = \operatorname{div}_B(a). $$

Ta suy ra (nhờ (13)) rằng, với mọi iđêan phân thức $a$ của $A$, cũng có:

(16) $$ i(\operatorname{div}_A(a)) = \operatorname{div}_B(aB). $$

Với mọi phần tử $b \in B$, ta biết (Chương V, \S 1, no. 3, Hệ quả của Mệnh đề 11) rằng $N_{L/K}(b) \in A$; hơn nữa (Chương VI, \S 8, no. 5, công thức (9)):

(17) $$ v_p(N_{L/K}(b)) = \sum_{\mathfrak{p}/p} f_{\mathfrak{p}/p} v_{\mathfrak{p}}(b) $$

do đó:

(18) $$ N(\operatorname{div}_B(b)) = \operatorname{div}_A(N_{L/K}(b)). $$

Các công thức (15) và (18) cho thấy rằng, bằng cách lấy thương, các đồng cấu $N$ và $i$ xác định các đồng cấu mà, do lạm dụng ngôn ngữ, cũng sẽ được ký hiệu là:

$$ N : C(B) \to C(A), \quad i : C(A) \to C(B). $$

Chú ý rằng đồng cấu $i : C(A) \to C(B)$ nói chung không đơn ánh (\S 3, Bài tập 7).

Nhắc lại rằng với mọi $B$-môđun $R$, $R_{[A]}$ ký hiệu $A$-môđun thu được từ $R$ bằng cách thu hẹp các vô hướng xuống $A$ (Đại số, Chương 11, \S 1, no. 13).

#### Mệnh đề 18 {#ac-vii-s4-prop-18 .statement}

(i) *Để $R$ là một $B$-môđun giả-không, điều kiện cần và đủ là $A$-môđun $R_{[A]}$ là giả-không.*

(ii) *Để $R$ là một $B$-môđun xoắn sinh hữu hạn, điều kiện cần và đủ là $R_{[A]}$ là một $A$-môđun xoắn sinh hữu hạn và khi đó:*

(19) $$ \chi_A(R_{[A]}) = N(\chi_B(R)). $$

(iii) *Để $R$ là một $B$-môđun sinh hữu hạn, điều kiện cần và đủ là $R_{[A]}$ là một $A$-môđun sinh hữu hạn và khi đó:*

(20) $$ c_A(R_{[A]}) = N(c_B(R)) + r_B(R)c_A(B) $$
(21) $$ r_A(R_{[A]}) = n . r_B(R) \quad \text{(nhắc lại rằng } n = r_A(B)). $$

Vì $B$ là một $A$-môđun sinh hữu hạn, để $R$ là một $B$-môđun sinh hữu hạn, điều kiện cần và đủ là $R_{[A]}$ là một $A$-môđun sinh hữu hạn. Hơn nữa, nếu $b$ là linh hóa tử của $R$, thì $b \cap A = a$ là linh hóa tử của $R_{[A]}$; vì $B$ nguyên trên $A$, không có iđêan nào khác 0 nằm trên iđêan 0 của $A$ (Chương V, § 2, no. 1, Hệ quả 1 của Mệnh đề 1), và do đó nói $a \neq 0$ hay $b \neq 0$ thì cũng là một điều.

(i) Theo nhận xét cuối cùng này, ta có thể chỉ giới hạn sự chú ý vào trường hợp $R$ là một $B$-môđun xoắn. Nếu $b$ được chứa trong một iđêan nguyên tố $\mathfrak{p} \in P(B)$, thì $a$ được chứa trong $\mathfrak{p} \cap A = p$, iđêan này có chiều cao bằng 1. Ngược lại, nếu $a$ được chứa trong một iđêan nguyên tố $p \in P(A)$, thì tồn tại một iđêan nguyên tố $\mathfrak{p}$ của $B$ chứa $b$ và nằm trên $p$ (Chương V, § 2, no. 1, Hệ quả 2 của Định lý 1). Mệnh đề (i) suy ra từ các nhận xét này và no. 4, Định nghĩa 2.

(ii) Với mọi $B$-môđun xoắn sinh hữu hạn $R$, ta viết

$$
\phi(R) = \chi_A(R_{[A]});
$$

rõ ràng (đối với các $B$-môđun xoắn sinh hữu hạn) $\phi$ thỏa mãn các điều kiện (1) và (2) của Mệnh đề II ở no. 5 (có tính đến (i)). Do đó tồn tại một đồng cấu $\theta : D(B) \to D(A)$ sao cho $\phi(R) = \theta(\chi_B(R))$ với mọi $B$-môđun xoắn sinh hữu hạn $R$. Đồng cấu $\theta$ được xác định bởi giá trị của nó trên mọi $B$-môđun có dạng $B/\mathfrak{p}$ với $\mathfrak{p} \in P(B)$, vì $\chi_B(B/\mathfrak{p}) = \mathfrak{p}$. Bây giờ, với mọi iđêan nguyên tố $q \neq p = \mathfrak{p} \cap A$ trong $P(A)$, ta có $p \notin q$ và do đó $(B/\mathfrak{p})_q = 0$. Mặt khác, nếu đặt $S = A - p$, thì $\mathfrak{p}.S^{-1}B$ là một iđêan cực đại của $S^{-1}B$ và $(B/\mathfrak{p})_p = S^{-1}B/\mathfrak{p}$. $S^{-1}B$ đẳng cấu với trường phân thức của $B/\mathfrak{p}$ (Chương II, § 2, no. 5, Mệnh đề 11), tức là với trường thặng dư của $v_{\mathfrak{p}}$; do đó độ dài của nó như một $A$-môđun là $f_{\mathfrak{p}/p}$; điều này chứng minh rằng $\theta = N$ (no. 5, Định nghĩa 4).

(iii) Nếu $T$ là môđun con xoắn của $R$, thì $T_{[A]}$ là môđun con xoắn của $R_{[A]}$ và $(R/T)_{[A]} = R_{[A]}/T_{[A]}$; do đó để chứng minh (21) ta có thể chỉ cần xét trường hợp $R$ không xoắn. Khi đó $R$ được đồng nhất với một môđun con-$B$ của $R_{(L)}$ và chứa một cơ sở $(e_i)_1 < < m$ của $R_{(L)}$ trên $L$. Nếu $(b_j)_1 s < n$ là một cơ sở của $L$ trên $K$ gồm các phần tử của $B$, thì các $b_j e_i$ lập thành một cơ sở của $R_{(L)}$ trên $K$ gồm các phần tử của $R$, do đó suy ra (21). Mặt khác, cho $M$ là một môđun con-$B$ tự do của $R$ sao cho $R/M$ là một $B$-môđun xoắn; vì $M_{[A]}$ là tổng trực tiếp của $r_B(R)$ $A$-môđun đẳng cấu với $B$, theo Mệnh đề 16 (i)

$$
c_A(M_{[A]}) = r_B(R).c_A(B).
$$

Hơn nữa, $c_A((R/M)_{[A]}) = -c_A(N(\chi_B(R/M)))$ theo (19); nhưng theo định nghĩa của đồng cấu $N : C(B) \to C(A)$, ta có $c_A(N(d)) = N(c_B(d))$ với mọi $d \in D(B)$ và, vì $c_B(\chi(R/M)) = -c_B(R)$ theo định nghĩa, cuối cùng

$$
c_A((R/M)_{[A]}) = N(c_B(R));
$$

khi đó chỉ cần áp dụng Mệnh đề 16 (i) để thu được (20).

#### Mệnh đề 19 {#ac-vii-s4-prop-19 .statement}

Cho $R$ là *một môđun* $B$ sinh *hữu hạn*. Điều kiện cần *và đủ* để $R$ *phản xạ* là $R_{[A]}$ là *một môđun* $A$ *phản xạ*.

Ta đã nhận xét trong chứng minh của Mệnh đề 18 rằng điều kiện cần và đủ để R là một B-môđun không xoắn là $R_{[A]}$ là một A-môđun không xoắn. Do đó ta có thể giả thiết rằng R là một dàn của $W = R \otimes_B L$ đối với B. Ta sẽ dùng bổ đề sau:

#### Bổ đề 4 {#ac-vii-s4-lem-4 .statement}

*Cho W là một không gian vectơ hạng hữu hạn trên L và cho R là một dàn của W đối với B. Khi đó, với mọi $p \in P(A)$, $(R_{[A]})_p = \bigcap_{\mathfrak{p}/p} R_{\mathfrak{p}}$.*

Nếu $S = A - p$, các iđêan nguyên tố của vành $S^{-1}B$ được sinh bởi các iđêan nguyên tố của B không gặp S, nói cách khác là các iđêan $\mathfrak{P}_i$ ($1 \leq i \leq m$) nằm trên p và iđêan (0); điều này cho thấy rằng $S^{-1}B$ là một vành nửa địa phương mà các iđêan cực đại của nó là các m, $= \mathfrak{P}_i(S^{-1}B)$ với $1 \leq i \leq m$; hơn nữa, vành địa phương $(S^{-1}B)_{\mathfrak{P}_i}$ đẳng cấu với $B_{\mathfrak{p}_i}$ (Chương 11, § 2, no. 5, Mệnh đề 11) và do đó là một vành định giá rời rạc. Vậy vành $S^{-1}B$ là một miền Dedekind (§ 2, no. 2, Định lý 1 (f)) và, vì nó là nửa địa phương, nó là một miền iđêan chính (§ 2, no. 2, Mệnh đề 1). Như vậy, $(R_{[A]})_p$ bằng $S^{-1}R$ được xét như một A,-môđun; theo trên, $S^{-1}R$ là một dàn tự do của W đối với $S^{-1}B$ và do đó có thể áp dụng cho nó Định lý 2 của no. 2, suy ra $S^{-1}R = \bigcap_i (S^{-1}R)_{m_i}$: nhưng $(S^{-1}R)_{m_i} = R_{\mathfrak{p}_i}$, điều này chứng minh bổ đề.

Quay trở lại chứng minh của Mệnh đề 19, theo Bổ đề 4,

$$
\bigcap_{\mathfrak{p} \in P(B)} R_{\mathfrak{p}} = \bigcap_{p \in P(A)} (R_{[A]})_p
$$

và kết luận suy ra từ no. 2, Định lý 2.

#### Hệ quả {#ac-vii-s4-n8-cor-1 .statement}

*Vành B là một A-môđun phản xạ.*

#### Mệnh đề 20 {#ac-vii-s4-prop-20 .statement}

(i) *Điều kiện cần và đủ để một A-môđun hữu hạn sinh M là giả-không là $M \otimes_A B$ là một B-môđun giả-không.*
(ii) *Nếu M là một A-môđun xoắn hữu hạn sinh, thì $M \otimes_A B$ là một B-môđun hữu hạn sinh và:*
(22)
$$
\chi_B(M \otimes_A B) = i(\chi_A(M)).
$$
(iii) *Nếu M là một A-môđun hữu hạn sinh, thì $M \otimes_A B$ là một B-môđun hữu hạn sinh và:*
(23)
$$
c_B(M \otimes_A B) = i(c_A(M))
$$
(24)
$$
r_B(M \otimes_A B) = r_A(M).
$$

(i) Cho $\mathfrak{p}$ là một iđêan nguyên tố của $B$, $\mathfrak{p} = \mathfrak{P} \cap A$; khi đó $(M \otimes_A B)_{\mathfrak{p}} = M \otimes_A B_{\mathfrak{p}}$ (Chương 11, § 2, no. 7, Mệnh đề 18) và mặt khác
$$
M \otimes_A B_{\mathfrak{p}} = (M \otimes_A A_p) \otimes_{A_p} B_{\mathfrak{p}} = M_p \otimes_{A_p} B_{\mathfrak{p}};
$$
vì thế quan hệ $M_p = 0$ là tương đương với $(M \otimes_A B)_{\mathfrak{p}} = 0$ (Chương II, § 4, no. 4, Bổ đề 4). Chỉ cần áp dụng nhận xét này cho iđêan $\mathfrak{P} = (0)$ và các iđêan $\mathfrak{p} \in P(B)$ để chứng minh (i), có tính đến no. 4, Định nghĩa 2.

Để chứng minh (ii), chúng ta sẽ dùng bổ đề sau:

#### Bổ đề 5 {#ac-vii-s4-lem-5 .statement}

*Cho $M_1, M$, là hai $A$-môđun hữu hạn sinh, và $f : M_1 \to M_2$ là một đồng cấu đơn cấu. Khi đó hạt nhân của $f \otimes 1 ; M_1 \otimes_A B \to M_2 \otimes_A B$ là giả-không.*

Cho $\mathfrak{p}$ là một iđêan nguyên tố của $A$ có chiều cao $\leq 1$. Khi đó $(M_i \otimes_A B)_\mathfrak{p} = (M_i)_\mathfrak{p} \otimes_{A_\mathfrak{p}} B_\mathfrak{p}$ ($i = 1, 2$) (Chương 11, § 2, no. 7, Mệnh đề 18) và $(f \otimes 1_B)_\mathfrak{p} = f_\mathfrak{p} \otimes 1_{B_\mathfrak{p}}$; giả thiết rằng $f$ là đơn cấu kéo theo rằng $f$, cũng vậy (Chương II, § 2, no. 4, Định lý 1); mặt khác, do lựa chọn của $\mathfrak{p}$, $A_\mathfrak{p}$ là một miền iđêan chính và $B_\mathfrak{p}$ là một $A_\mathfrak{p}$-môđun xoắn-không hữu hạn sinh và do đó là *tự do*; chúng ta kết luận rằng $f_\mathfrak{p} \otimes 1_{B_\mathfrak{p}}$ bản thân nó cũng là đơn cấu. Nếu $I = \mathrm{Ker}(f \otimes 1)$, thì $I_\mathfrak{p} = \mathrm{Ker}((f \otimes 1)_\mathfrak{p})$ (Chương 11, § 2, no. 4, Định lý 1); do đó $I_\mathfrak{p} = 0$, do đó *a fortiori* $I_\mathfrak{p} = (I_\mathfrak{p})_\mathfrak{p} = 0$ với $\mathfrak{p}|p$, điều này chứng minh bổ đề (no. 4, Định nghĩa 2).

Bây giờ ta trở lại chứng minh của (ii). Với mọi $A$-môđun xoắn sinh hữu hạn $M$, đặt $\phi(M) = \chi_B(M \otimes_A B)$; từ (i) suy ra rằng, nếu $M$ là giả-không, thì $\phi(M) = 0$. Mặt khác, xét một dãy khớp các $A$-môđun xoắn sinh hữu hạn:
$$
0 \to M_1 \to M_2 \to M_3 \to 0.
$$
Từ Bổ đề 4 suy ra có một dãy khớp các $B$-môđun:
$$
0 \to I \to M_1 \otimes_A B \to M_2 \otimes_A B \to M_3 \otimes_A B \to 0
$$
trong đó $I$ là giả-không. Do đó, dùng no. 5, Hệ quả của Mệnh đề 10, ta được $\phi(M_2) = \phi(M_1) + \phi(M_3)$. Vậy từ Mệnh đề 11 của no. 5 ta kết luận rằng tồn tại một đồng cấu $\theta : D(A) \to D(B)$ sao cho $\phi(M) = \theta(\chi_A(M))$ với mọi $A$-môđun xoắn sinh hữu hạn $M$. Để chứng minh $\theta = i$, chỉ cần chỉ ra rằng $\phi(A/p) = i(p)$ với mọi $p \in P(A)$; mà $(A/p) \otimes_A B = B/pB$ và, với mọi $\mathfrak{p} \in P(B)$, $(B/pB)_{\mathfrak{p}} = B_{\mathfrak{p}}/pB_{\mathfrak{p}}$; môđun sau cùng bằng 0 nếu $\mathfrak{p}$ không nằm trên $p$; trái lại, nếu $\mathfrak{p}|p$, thì $B_{\mathfrak{p}}/pB_{\mathfrak{p}}$ là một $B_{\mathfrak{p}}$-môđun có độ dài $e(\mathfrak{p}/p)$ theo định nghĩa của chỉ số phân nhánh (Chương VI, § 8, no. 1); do đó $\chi_B(B/pB) = \sum_{\mathfrak{p}|p} e_{\mathfrak{p}/p} . 13 = i(p)$, điều này hoàn tất chứng minh của (ii).

Công thức (24) là ngay lập tức, vì
$$
(M \otimes_A B) \otimes_B L = M \otimes_A L = (M \otimes_A K) \otimes_K L
$$

và hạng của $(M \otimes_A K) \otimes_K L$ trên $L$ bằng hạng của $M \otimes_A K$ trên $K$. Để chỉ ra (23), xét một môđun con tự do $H$ của $M$ sao cho $Q = M/H$ là một $A$-môđun xoắn. Áp dụng Bổ đề 4 như trên, ta thu được một dãy khớp các $B$-môđun:

$$
0 \to I \to H \otimes_A B \to M \otimes_A B \to Q \otimes_A B \to 0
$$

trong đó $I$ là giả-không. Do đó từ no. 7, Mệnh đề 16(ii) và (v) và Hệ quả 1 của Mệnh đề 16 suy ra rằng

$$
c_B(M \otimes_A B) = c_B(Q \otimes_A B) = -c_B(\chi_B(Q \otimes_A B)) = -c_B(i(\chi_A(Q)))
$$

theo (ii); nhưng theo định nghĩa của đồng cấu $i : C(A) \to C(B)$,
$c_B(i(\chi_A(Q))) = i(c_A(\chi_A(Q))) = -i(c_A(M))$, điều này hoàn tất chứng minh của (23).

**Nhận xét**
(1) Nếu $M$ là một $A$-môđun phản xạ, thì $M \otimes_A B$ không nhất thiết phản xạ (bài tập 6). Tuy nhiên điều đó đúng khi $B$ là một $A$-môđun phẳng (no. 2, Mệnh đề 8).
(2) Cho $C$ là một miền Noether đóng nguyên thứ ba sao cho $B \subset C$ và $C$ là một $B$-môđun sinh hữu hạn (và do đó cũng là một $A$-môđun sinh hữu hạn). Khi đó ta có các công thức bắc cầu:

(25)
$$
N_{C/A} = N_{B/A} \circ N_{C/B},
$$
(26)
$$
i_{C/A} = i_{C/B} \circ i_{B/A}
$$

chúng suy ra ngay lập tức từ các công thức bắc cầu đối với các chỉ số phân nhánh và các bậc thặng dư (Chương VI, § 8, no. 1, Bổ đề 1).

### 9. MỘT ĐỊNH LÝ RÚT GỌN

Ta giữ nguyên ký hiệu và các giả thiết của các số 2 đến 7.

#### Bổ đề 6 {#ac-vii-s4-lem-6 .statement}

*Cho $R$ là một vành giao hoán và $p_i$ ($1 \leq i \leq n$) là các iđêan nguyên tố phân biệt của $R$.*

(i) *Với $1 \leq i \leq n$, gọi $H_i$ là một tập con của $R/p_i$ thỏa mãn điều kiện sau: không tồn tại phần tử nào $\alpha_i \in R/p_i$ sao cho $\alpha_i + H_i$ chứa một iđêan $\neq 0$ của $R/p_i$. Khi đó tồn tại $a \in R$ sao cho, với $1 \leq i \leq n$, ảnh chính tắc của $a$ trong $R/p_i$ không thuộc $H_i$.*

(ii) *Nếu $\operatorname{Card}(H_i) < \operatorname{Card}(R/p_i)$, thì các $H_i$ thỏa mãn điều kiện ở (i).*

(i) Ta lập luận bằng quy nạp theo $n$, trường hợp $n = 0$ là tầm thường. Vậy giả sử $n \geq 1$. Ta có thể thực hiện một phép hoán vị trên các chỉ số $i$ và có thể giả sử rằng $p_1$ là cực tiểu trong các $p_i$ và do đó, với $2 \leq i \leq n$, tồn tại $c_i \in p_i$ sao cho $c_i \notin p_1$. Theo giả thiết quy nạp, tồn tại $b \in R$ sao cho ảnh chính tắc của $b$ trong $R/p_i$ không thuộc $H_i$ với $2 \leq i \leq n$. Với mọi $x \in R$ ta đặt $a_i = b + x c_2 c_3 \ldots c_n$; vì $c_i \in p_i$, hiển nhiên $a_i \equiv b \pmod{p_i}$ với $2 \leq i \leq n$. Do đó chỉ cần chứng minh rằng tồn tại $x \in \mathbf{R}$ sao cho ảnh chính tắc của $a_i$ trong $\mathbf{R}/p_1$ không thuộc $H_1$. Bây giờ, tập hợp các ảnh chính tắc của các $a_i$ trong $\mathbf{R}/p_1$, khi $x$ chạy qua $\mathbf{R}$, chính là $\beta + c$, trong đó $\beta$ là ảnh chính tắc của $b$ và $c$ là iđêan của $\mathbf{R}/p_1$ sinh bởi ảnh chính tắc của $c_2 c_3 \ldots c_n$; nhờ cách lựa chọn các $c_i$, ta có $c \neq 0$ vì $\mathbf{R}/p_1$ là một miền nguyên và giả thiết về $H_1$ suy ra sự tồn tại của một $x$ giải được bài toán.

(ii) Vì $\mathbf{R}/p_i$ là một miền nguyên, mọi iđêan $\neq 0$ của $\mathbf{R}/p_i$ đều có lực lượng bằng lực lượng của $\mathbf{R}/p_i$ và điều tương tự cũng đúng với mọi phép tịnh tiến của một iđêan bởi một phần tử của $\mathbf{R}/p_i$, do đó suy ra kết luận.

#### Định lý 6 {#ac-vii-s4-thm-6 .statement}

*Cho M là một A-môđun không xoắn hữu hạn sinh. Tồn tại một môđun con tự do L của M sao cho M/L đẳng cấu với một iđêan của A.*

Ta sẽ ký hiệu bởi $n$ *hạng* của $M$ (hạng của $V = M \otimes_A K$ trên $K$) và xem $M$ như một dàn của $V$ đối với $A$. Khi đó, với mọi $p \in P(A)$, $M_p$ là một dàn của $V$ đối với $A_p$ (no. 1, *Ví dụ 6*) và, vì $A_p$ là một miền iđêan chính, $M_p$ là một A-môđun *tự do* hạng $n$. Ta sẽ viết:

$$
M(p) = M_p/pM_p.
$$

Ta sẽ ký hiệu bởi $k(p)$ trường phân thức của $A/p$ (đẳng cấu với trường thặng dư của $A_p$); do đó $M(p) = M \otimes_A k(p)$ là một không gian vectơ hạng $n$ trên $k(p)$. Với mọi $x \in M$, ta sẽ ký hiệu bởi $x(p)$ ảnh chính tắc của $x$ trong $M(p)$.

#### Bổ đề 7 {#ac-vii-s4-lem-7 .statement}

*Cho $x_i$ ($1 \leq i \leq m$) là các phần tử độc lập tuyến tính của $M$ (trên $A$ hoặc $K$, điều này là như nhau) và cho $L$ là môđun con-A của $M$ sinh bởi các $x_i$. Khi đó, với hầu hết mọi $p \in P$, các $x_i(p) \in M(p)$ là độc lập tuyến tính trên $k(p)$; để chúng độc lập tuyến tính trên $k(p)$ với mọi $p \in P$, điều kiện cần và đủ là $M/L$ không xoắn.*

Cho $x_1, \ldots, x_n$ là các phần tử của $M$ mà cùng với $x_1, \ldots, x_n$ chúng lập thành một cơ sở của $V$, và cho $N$ là môđun con-A tự do của $M$ sinh bởi các $x_i$ ($1 \leq i \leq n$). Từ no. 3, Định lý 3 suy ra rằng $N_p = M_p$, với hầu hết mọi $p \in P$; vì $x_1(p), \ldots, x_n(p)$ lập thành một cơ sở của $N(p)$ trên $k(p)$, điều này chứng minh mệnh đề thứ nhất.

Nếu $M/L$ không xoắn, thì $(M/L)_p = M_p/L_p$ cũng không xoắn với mọi $p \in P$ (no. 1, *Ví dụ 6*) và, vì $A_p$ là một miền iđêan chính, $M_p/L_p$ là tự do. Do đó $M$, là tổng trực tiếp của $L$, và của một $A$-môđun tự do $E$ hạng $n - m$; suy ra $M(p)$ là tổng trực tiếp của $L(p)$ và của không gian vectơ $k(p)$ $E/pE$ hạng $n - m$; bởi vậy $L(p)$ có hạng $m$ và, vì nó được sinh bởi các $x_i(p)$ ($1 \leq i \leq m$), các phần tử sau là độc lập tuyến tính.

Ngược lại, giả sử rằng các $x_i(p)$ ($1 \leq i \leq m$) là độc lập tuyến tính trên $k(p)$ với mọi $p \in P$. Khi đó $L$, là một nhân tử trực tiếp của $M$, với mọi $p$ (Chương II, § 3, no. 2, Hệ quả 1 của Mệnh đề 5) và do đó $M_p/L_p = (M/L)_p$ không xoắn với mọi $p \in P$. Ta kết luận rằng $P \cap \operatorname{Ass}(M/L) = \varnothing$ theo Chương IV, § 1, no. 2, Hệ quả của Mệnh đề 5. Nhưng vì L là phản xạ, suy ra từ no. 2, Mệnh đề 7 (i) rằng iđêan nguyên tố duy nhất có thể thuộc $\operatorname{Ass}(M/L)$ là iđêan (0); do đó $M/L$ không xoắn.

#### Bổ đề 8 {#ac-vii-s4-lem-8 .statement}

*Giả sử rằng hạng $n$ của $M$ là $\geqslant 2$; khi đó tồn tại một phần tử $x \neq 0$ của $M$ sao cho $M/Ax$ không xoắn.*

Cho $y \neq 0$ là một phần tử của $M$. Theo Bổ đề 7, tập hợp $Y$ các $p \in P$ sao cho $y(p) = 0$ là hữu hạn. Nếu $Y = \varnothing$, thì theo Bổ đề 7, áp dụng cho dãy $(x,)$ gồm phần tử duy nhất $y$, suy ra $M/Ay$ là không xoắn. Vậy giả sử rằng $Y \# @$ và đặt $S = \bigcap_{p \in Y} (A - p)$; ta biết (no. 4, Bổ đề 2) rằng $S^{-1}A$ là một miền iđêan chính nửa địa phương mà các iđêan cực đại là các $pS^{-1}A$, với $p \in Y$, các vành địa phương tương ứng là các $A_p$. Do đó
$$
S^{-1}A/pS^{-1}A = k(p),
$$
suy ra
$$
S^{-1}M/pS^{-1}M = (M/pM) \otimes_A S^{-1}A = M \otimes_A ((A/p) \otimes_A S^{-1}A) = M \otimes_A k(p) = M(p)
$$
với mọi $p \in Y$. Theo Chương II, § 1, no. 2, Mệnh đề 6, tồn tại một phần tử $z/s \in S^{-1}M$ ($z \in M, s \in S$) mà các ảnh chính tắc của nó trong các $M(p)$ với $p \in Y$ đều $\neq 0$. Vậy theo định nghĩa của $S$ ta có $z(p) \neq 0$ với mọi $p \in Y$. Hơn nữa, ta có thể giả sử rằng $y$ và $z$ *độc lập tuyến tính* trên $K$. Thật vậy, trong trường hợp đối, hãy xét một phần tử $t \in M$ độc lập tuyến tính với $y$ (phần tử như vậy tồn tại vì $n \geqslant 2$); mặt khác lấy một phần tử $a \neq 0$ thuộc $\bigcap_{p \in Y} p$ (giao này không thu về 0 vì $A$ là một miền nguyên) và đặt $z' = z + at$: rõ ràng $y$ và $z'$ độc lập tuyến tính trên $K$ và $z'(p) = z(p) \neq 0$ với mọi $p \in Y$.

Vậy giả sử rằng $y$ và $z$ độc lập tuyến tính trên $K$, đặt $Z$ là tập hợp các $p \in P - Y$ sao cho $y(p)$ và $z(p)$ độc lập tuyến tính trên $k(p)$; theo Bổ đề 7, tập hợp này là *hữu hạn*. Do đó, với mọi $p \in Z$, ta có thể viết $z(p) = \lambda(p)y(p)$ với $\lambda(p) \in k(p)$. Mặt khác, $\operatorname{Card}(A/p) > 2$ với mọi $p \in P$; bởi vậy theo Bổ đề 6, tồn tại $b \in A$ sao cho, với mọi $p \in Z$, ảnh chính tắc của $b$ trong $A/p$ khác với $\lambda(p)$. Bây giờ ta sẽ chỉ ra rằng phần tử $x = z - by$ giải được bài toán; chỉ cần (chiếu theo Bổ đề 7 áp dụng với $m = 1$) kiểm tra rằng $x(p) \neq 0$ với *mọi* $p \in P$. Thật vậy:

— nếu $p \in Y$, thì $x(p) \neq 0$ theo phép dựng;
— nếu $p \in Z$, thì $x(p) = \mu_p y(p)$ với $\mu_p \neq 0$ do cách chọn $b$ và do đó $x(p) \neq 0$ vì $y(p) \# 0$;
— nếu $p \in P - (Y \cup Z)$, thì $y(p)$ và $z(p)$ độc lập tuyến tính và do đó $x(p) \neq 0$.

Sau khi đã thiết lập các bổ đề này, ta chuyển sang chứng minh Định lý 6. Ta lập luận bằng quy nạp theo $n$, trường hợp $n \leq 1$ là tầm thường vì khi đó chính $M$ đẳng cấu với một iđêan của $A$. Vậy giả sử rằng $n \geq 2$; theo Bổ đề 8, tồn tại một môđun con tự do $L_0$ của $M$ có hạng 1 sao cho $M/L_0$ không xoắn; do đó $M/L_0$ có hạng $n - 1$. Theo giả thiết quy nạp, tồn tại một môđun con tự do $L$, của $M/L_0$ sao cho $(M/L_0)/L_1$ đẳng cấu với một iđêan của $A$. Gọi $L$ là ảnh ngược của $L_1$ trong $M$; $L/L_0$ đẳng cấu với $L_1$ và, vì $L_1$ là tự do, $L$ đẳng cấu với $L_0 \oplus L_1$ (Algebra, Chapter II, § 1, no. 11, Proposition 21) và do đó là tự do; vì $M/L$ đẳng cấu với $(M/L_0)/L_1$, định lý được chứng minh.

#### Nhận xét {#ac-vii-s4-n9-rem-1 .statement}

Nếu $M$ là phản xạ, thì điều tương tự không nhất thiết còn đúng đối với $M/L$ (Bài tập 9).

### 10. MÔĐUN TRÊN CÁC MIỀN DEDEKIND

Bây giờ ta giả sử rằng $A$ là một miền Dedekind; khi đó ta biết rằng các iđêan $p \in P$ là cực đại và chúng là các iđêan nguyên tố duy nhất $\neq 0$ của $A$ ($\S 2$, no. 1 ); nhóm $D(A)$ được đồng nhất với nhóm $I(A)$ các iđêan phân thức $\neq 0$ của $A$.

#### Mệnh đề 21 {#ac-vii-s4-prop-21 .statement}

Cho $A$ là một miền Dedekind. Mọi A-môđun giả-không đều là môđun không. Mọi đồng cấu A-môđun giả-đơn ánh (resp. giả-toàn ánh, giả-song ánh, giả-không) đều là đơn ánh (resp. toàn ánh, song ánh, không).

Mệnh đề thứ nhất đã được chỉ ra rồi (no. 4, Ví dụ 1); các mệnh đề kia suy ra từ đó ngay lập tức.

#### Mệnh đề 22 {#ac-vii-s4-prop-22 .statement}

Cho $A$ là một miền Dedekind và $M$ là một A-môđun sinh hữu hạn. Các tính chất sau là tương đương:
(a) $M$ không xoắn.
(b) $M$ phản xạ.
(c) $M$ xạ ảnh.

Ta đã biết rồi (không có giả thiết nào trên miền nguyên $A$) rằng (b) kéo theo (a) (no. 2, Nhận xét 1) và rằng (c) kéo theo (b) (Algebra, Chương II, § 2, no. 7, Hệ quả 4 của Mệnh đề 14). Nếu $M$ không xoắn, nó được đồng nhất với một dàn của $V = M \otimes_A K$ đối với $A$; do đó $M$, là một $A_p$-môđun tự do với mọi iđêan cực đại $p \in P$, vì $A$, là một miền iđêan chính. Kết luận khi đó suy ra từ Chương II, § 5, no. 2, Định lý 1 (b).

#### Hệ quả {#ac-vii-s4-n10-cor-1 .statement}

Cho $M$ là một A-môđun sinh hữu hạn và $T$ là môđun con xoắn của nó. Khi đó $T$ là một hạng tử trực tiếp của $M$.

Vì $M/T$ không xoắn và sinh hữu hạn, nó là xạ ảnh theo Mệnh đề 22, và do đó hệ quả suy ra từ Algebra, Chương II, § 2, no. 2, Mệnh đề 4.

#### Mệnh đề 23 {#ac-vii-s4-prop-23 .statement}

Cho $A$ là một miền Dedekind và $T$ là một A-môđun xoắn sinh hữu hạn. Tồn tại hai họ hữu hạn $(n_i)_{i \in I}$ và $(\mathfrak{p}_i)_{i \in I}$, trong đó các $n_i$ là các số nguyên $\geq 1$ và các $\mathfrak{p}_i$ là các phần tử của $P$, sao cho $T$ đẳng cấu với tổng trực tiếp $\bigoplus_{i \in I} (A/\mathfrak{p}_i^{n_i})$. Hơn nữa, các họ $(n_i)_{i \in I}$ và $(\mathfrak{p}_i)_{i \in I}$ là duy nhất sai khác một song ánh của tập hợp chỉ số.

Điều này suy ra từ no. 4, Định lý 5, có lưu ý đến việc ở đây một giả-đẳng cấu là một đẳng cấu.

#### Mệnh đề 24 {#ac-vii-s4-prop-24 .statement}

Cho $A$ là một miền Dedekind và $M$ là một A-môđun không xoắn sinh hữu hạn & hạng $n \geq 1$. Khi đó tồn tại một iđêan $b \neq 0$ của $A$ sao cho $M$ đẳng cấu với tổng trực tiếp của các môđun $A^{n-1}$ và $b$. Hơn nữa, lớp của iđêan $b$ được xác định duy nhất bởi điều kiện này.

Định lý 6 của no. 9 cho thấy rằng tồn tại một môđun con tự do $L$ của $M$ sao cho $M/L$ đẳng cấu với một iđêan $a$ của $A$. Nếu $a = 0$, ta lấy $b = A$. Nếu không, $a$ có hạng 1, do đó $L = A^{n-1}$ và $a$ là một môđun *xạ ảnh* (Mệnh đề 22); vì thế $M$ đẳng cấu với tổng trực tiếp của $L$ và $a$ (*Đại số*, Chương II, § 2, no. 2, Mệnh đề 4), điều này chứng minh phần thứ nhất của mệnh đề. Hơn nữa, từ no. 7, Mệnh đề 16 (i), (iv) và (v) suy ra rằng $c(M) = c(b)$ do đó có tính duy nhất của lớp của $b$.

Nhận xét
(1) Các Mệnh đề 23 và 24 và Hệ quả của Mệnh đề 22 xác định hoàn toàn cấu trúc của các $A$-môđun sinh hữu hạn. Mệnh đề 24 cho thấy rằng một $A$-môđun sinh hữu hạn không xoắn được xác định đến đẳng cấu bởi *hạng* của nó và lớp *ước* gắn với nó.
(2) Có thể chỉ ra rằng trên một miền Dedekind, một môđun xạ ảnh không sinh hữu hạn thì tất yếu là *tự do* (Bài tập 21), và mọi môđun con của một môđun xạ ảnh đều là xạ ảnh (Bài tập 20).

### Bài tập {#ac-vii-s4-exercises}

Xem [các bài tập của § 4](exercises/s4/).
