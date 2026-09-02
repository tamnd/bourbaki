---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: III
chapter_title: LIE GROUPS
section: 10
section_title: The automorphism group of a Lie group
lang: vi
source: lie-i-iii
pdf_pages: 0377-0386, 0427-0481
extraction: ocr
subsections:
    - "no": 1
      title: INFINITESIMAL AUTOMORPHISMS
      page: 0
      pdf_page: 377
    - "no": 2
      title: THE AUTOMORPHISM GROUP OF A LIE GROUP (REAL OR COMPLEX CASE)
      page: 0
      pdf_page: 380
    - "no": 3
      title: THE AUTOMORPHISM GROUP OF A LIE GROUP (ULTRAMETRIC CASE)
      page: 0
      pdf_page: 385
statements: 13
exercises: 3
content_sha256: 989bdc385ba0ef057f8c59e3d24092ac73e934d7b04addca9b9bad4a484351ae
translated_from: content/en/lie/III/10_s10_the_automorphism_group_of_a_lie_group.md
source_content_sha256: 9324e1961b118ac5c4f73e3fb335e08c0b72a588687b17147d05e2b458b10af4
translation_model: gpt-5-6-mini
translation_run: translate-vi-89dd5412
glossary_version: 34
glossary_terms_sha256: 5dfb677a175003c57b8d055bf7023500888ceab438110a44051f3a5d08a332bf
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 10. NHÓM TỰ ĐẲNG CẤU CỦA MỘT NHÓM LIE

Trong đoạn này, K được giả sử là có đặc số không.

### 1. CÁC TỰ ĐẲNG CẤU VÔ CÙNG BÉ

#### Bổ đề 1 {#lie-iii-s10-lem-1 .statement}

Cho G là một nhóm Lie và $\alpha$ là một trường vectơ trên G. Với mọi $g \in G$, đặt
$$
\beta(g) = \alpha(g)g^{-1} \in L(G).
$$
Các điều kiện sau là tương đương:
(i) $\alpha$ là một đồng cấu của nhóm G vào nhóm T(G);
(ii) với mọi $g, g'$ trong G, $\alpha(gg') = \alpha(g)g' + g\alpha(g')$;
(iii) với mọi $g, g'$ trong G, $\beta(gg_1) = \beta(g) + (\mathrm{Ad}\,g)\beta(g')$.

Điều kiện (i) có nghĩa là, với mọi $g, g'$ trong G, ta có trong nhóm T(G):
$$
\beta(g)g\beta(g')g' = \beta(gg')gg'
$$
hoặc
$$
\beta(g)((\mathrm{Ad}\,g)\beta(g'))gg' = \beta(gg')gg'.
$$
Nhưng tích của $\beta(g)$ và $(\mathrm{Ad}\,g)\beta(g')$ trong T(G) chính là tổng của $\beta(g)$ và $(\mathrm{Ad}\,g)\beta(g')$ trong $L(G)$ (§ 2, no. 1, Mệnh đề 2). Do đó (i) $\Leftrightarrow$ (iii). Mặt khác, điều kiện (ii) có thể được viết $\beta(gg')gg' = \beta(g)gg' + g\beta(g')g'$, hoặc
$$
\beta(gg') = \beta(g) + (\mathrm{Ad}\,g)\beta(g')
$$
và do đó (ii) $\Leftrightarrow$ (iii).

#### Định nghĩa 1 {#lie-iii-s10-def-1 .statement}

Cho G là một nhóm Lie. Một tự đẳng cấu vô cùng bé của G là bất kỳ trường vectơ giải tích nào trên G thỏa mãn các điều kiện của Bổ đề 1.

#### Bổ đề 2 {#lie-iii-s10-lem-2 .statement}

Cho $K'$ là một trường con đóng không rời rạc của K, A là một $K'$-đa tạp, B và C là các $K$-đa tạp và $f$ là một ánh xạ giải tích $K'$ từ $A \times B$ vào C. Giả sử rằng, với mọi

LIE GROUPS

$a \in A$, *ánh xạ* $b \mapsto f(a, b)$ *của* B *vào* C *là* K-*giải tích*. *Khi đó, với mọi* $t \in TA$, *ánh xạ* $u \mapsto (Tf)(t, u)$ *của* TB *vào* TC *là* K-*giải tích*.

Ta cố định $t \in TA$ và viết $g(u) = (Tf)(t, u)$. Rõ ràng $g$ là K'-giải tích. Theo *Differentiable and Analytic Manifolds*, R, 5.14.6, chỉ cần chứng minh rằng các ánh xạ tiếp xúc của $g$ là K-tuyến tính. Có thể giả sử rằng A, B, C là các lân cận mở của 0 trong các không gian chuẩn hóa đầy đủ E, F, G trên K', K, K và rằng $t$ là tiếp xúc với A tại 0. Ta đồng nhất TA, TB, TC, với $A \times E, B \times F, C \times G$ và $t$ với một phần tử của E. Khi đó với mọi $(x, y) \in TB = B \times F$.

$$
g(x, y) = (f(0, x), (D_1f)(0, x)(t) + (D_2f)(0, x)(y)).
$$

Ta đồng nhất $T(B \times F)$ với $(B \times F) \times (F \times F)$ và $T(C \times G)$ với $(C \times G) \times (G \times G)$. Khi đó, với mọi

$$
((x, y), (h, k)) \in T(B \times F) = (B \times F) \times (F \times F),
$$

$(Tg)((x, y), (h, k)) = ((a, b), (c, d))$, trong đó

$$
\begin{align*}
a &= f(0, x), \\
b &= (D_1f)(0, x)(t) + (D_2f)(0, x)(y), \quad c = (D_2f)(0, x)(h), \\
d &= (D_2D_1f)(0, x)(t, h) + (D_2D_2f)(0, x)(y, h) + (D_2f)(0, x)(k).
\end{align*}
$$

Bây giờ ta cố định $(x, y) \in B \times F$. Ta cần chứng minh rằng ánh xạ $(h, k) \mapsto (c, d)$ từ $F \times F$ vào $G \times G$ là K-tuyến tính. Vì ánh xạ $x \mapsto f(0, x)$ từ B vào C là K-giải tích, các ánh xạ

$$
(h, k) \mapsto (D_2f)(0, x)(h), \quad (h, k) \mapsto (D_2D_2f)(0, x)(y, h),
$$
$$(h, k) \mapsto (D_2f)(0, x)(k)$$

là K-tuyến tính. Mặt khác

$$
(D_2D_1f)(0, x)(t, h) = \lim_{\lambda \in K', \lambda \to 0} \lambda^{-1}((D_2f)(\lambda t, x)(h) - (D_2f)(0, x)(h))
$$

và, với $\lambda$ cố định, ánh xạ $x \mapsto f(\lambda t, x)$ là K-giải tích, do đó ánh xạ $h \mapsto (D_2f)(\lambda t, x)(h)$ là K-tuyến tính.

#### Mệnh đề 1 {#lie-iii-s10-prop-1 .statement}

*Cho* K' *là một trường con đóng rời rạc của* K, G *là một nhóm Lie trên* K, V *là một đa tạp trên* K' *và* $(v, g) \mapsto vg$ *là một ánh xạ* K'-*giải tích từ* V $\times$ G *vào* G. *Giả sử rằng, với mọi* $v \in V$, *ánh xạ* $g \mapsto vg$ *của* G *vào* G *là một tự đẳng cấu của* G. *Cho* $\varepsilon$ *là một phần tử của* V *sao cho* $\varepsilon g = g$ *với mọi* $g \in G$ *và* $a \in T_\varepsilon(V)$. *Khi đó trường vectơ* $g \mapsto ag$ *trên* G *là một tự đẳng cấu vô cùng bé của* G.

Với $v \in V,\ g_1 \in G,\ g_2 \in G,\ v(g_1g_2) = (vg_1)(vg_2)$. Do đó, với $u_1 \in TG,\ u_2 \in TG,\ a(u_1u_2) = (au_1)(au_2)$ (§ 2, no. 1, Mệnh đề 3). Đặc biệt, ánh xạ $g \mapsto ag$ của G vào TG là một đồng cấu nhóm. Mặt khác, ánh xạ này là giải tích theo Bổ đề 2.

#### Mệnh đề 2 {#lie-iii-s10-prop-2 .statement}

*Cho* G *là một nhóm Lie thực hoặc phức và* $\alpha$ *là một tự đẳng cấu vô cùng bé của G. Tồn tại một luật phép toán giải tích $(\lambda, g) \mapsto \phi_\lambda(g)$ của K trên G với các tính chất sau:
(1) nếu D là luật liên kết của phép toán vô cùng bé, thì $D(1) = \alpha$;
(2) với mọi $\lambda \in K$, $\phi_\lambda \in \mathrm{Aut}\, G$.
(a) Với mọi $\mu > 0$, cho $K_\mu$ là quả cầu mở tâm 0 bán kính $\mu$ trong K. Với mọi $g \in G$, cho $\mathcal{F}_g$ là tập hợp các đường cong nguyên giải tích $f$ của $\alpha$ được xác định trong một quả cầu $K_\mu$ và sao cho $f(0) = g$. Theo Differentiable and Analytic Manifolds, R, 9.1.3 và 9.1.5, $\mathcal{F}_g$ không rỗng và hai phần tử của $\mathcal{F}_g$ trùng nhau trên giao của các miền xác định của chúng; gọi $\mu(g)$ là cận trên nhỏ nhất của các số $\mu$ sao cho tồn tại một phần tử của $\mathcal{F}_g$ được xác định trong $K_\mu$; tồn tại một phần tử duy nhất của $\mathcal{F}_g$ được xác định trong $K_{\mu(g)}$; ta ký hiệu nó là $f_g$.
(b) Cho $g_1, g_2$ thuộc G, $f_1 \in \mathcal{F}_{g_1}, f_2 \in \mathcal{F}_{g_2}$ với $f_1$ và $f_2$ được xác định trên cùng một quả cầu $K_\mu$. Khi đó $f_1 f_2 : K_\mu \to G$ là giải tích và $(f_1 f_2)(0) = g_1 g_2$. Mặt khác, với mọi $\lambda \in K_\mu$,

$$
(T_\lambda(f_1 f_2))1 = (T_\lambda f_1)1 \cdot f_2(\lambda) + f_1(\lambda) \cdot (T_\lambda f_2)1 \quad (\S\ 2,\ \text{Mệnh đề 7})
$$
$$
= \alpha(f_1(\lambda)) f_2(\lambda) + f_1(\lambda) \alpha(f_2(\lambda))
$$
$$
= \alpha((f_1 f_2)(\lambda)) \tag{\text{Bổ đề 1}}
$$

và do đó $f_1 f_2 \in \mathcal{F}_{g_1 g_2}$. Điều này chứng minh rằng $\mu(g_1 g_2) \geq \inf_{g \in V} (\mu(g_1), \mu(g_2))$.
(c) Theo Differentiable and Analytic Manifolds, R, 9.1.4 và 9.1.5, tồn tại một lân cận V của e trong G sao cho $\sigma = \inf_{g \in V} \mu(g) > 0$. Cho $h \in G$ và C là thành phần liên thông của nó. Với mọi $h' \in C$, theo (b), $\mu(h') \geq \inf(\sigma, \mu(h)) > 0$. Mặt khác, các hàm $f_{h'}$, với $h' \in C$, nhận giá trị trong C. Theo Differentiable and Analytic Manifolds, R, 9.1.4 và 9.1.5, $\mu = +\infty$ trong C và cuối cùng $\mu = +\infty$ trong G. Khi đó đặt $f_g(\lambda) = \phi_\lambda(g)$ với mọi $g \in G$ và mọi $\lambda \in K$. Theo Differentiable and Analytic Manifolds, R, 9.1.4 và 9.1.5, ánh xạ $(\lambda, g) \mapsto \phi_\lambda(g)$ là một luật của phép toán giải tích của K trên G. Rõ ràng, nếu D là luật liên kết của phép toán vi phân, $D(1) = \alpha$. Theo (b),

$$
\phi_\lambda(g_1 g_2) = \phi_\lambda(g_1) \phi_\lambda(g_2)
$$

với mọi $\lambda \in K, g_1 \in G, g_1 \in G$.

#### Mệnh đề 3 {#lie-iii-s10-prop-3 .statement}

Giả sử K là ultrametric. Cho G là một nhóm Lie compact và $\alpha$ là một tự đẳng cấu vi phân của G. Tồn tại một nhóm con mở I của K và một luật của phép toán giải tích $(\lambda, g) \mapsto \phi_\lambda(g)$ của I trên G có các tính chất sau:
(1) nếu D là luật liên kết của phép toán vi phân, thì $D(1) = \alpha$;
(2) với mọi $\lambda \in I, \phi_\lambda \in \mathrm{Aut}\, G$.
Vì G compact, tồn tại một nhóm con mở I' của K và một luật của phép toán giải tích $(\lambda, g) \mapsto \phi_\lambda(g)$ của I' trên G có tính chất (1) của mệnh đề (§ 4, no. 7, Hệ quả 2 của Định lý 6). Ta viết $\phi_\lambda(g) = f_g(\lambda)$ với $\lambda \in I'$ và $g \in G$. Khi đó, với $g_1, g_2$ trong G và $\lambda \in I'$,

$$
(T_\lambda(f_{g_1}f_{g_2}))1 = (T_\lambda f_{g_1})1 \cdot f_{g_2}(\lambda) + f_{g_1}(\lambda) \cdot (T_\lambda f_{g_2})1 \\
= \alpha(f_{g_1}(\lambda)) f_{g_2}(\lambda) + f_{g_1}(\lambda) \alpha(f_{g_2}(\lambda)) \\
= \alpha(f_{g_1}(\lambda) f_{g_2}(\lambda))
$$

và $(f_{g_1}f_{g_2})(0) = g_1 g_2 = f_{g_1g_2}(0)$. Do đó $f_{g_1'g_2'}(\lambda) = f_{g_1'}(\lambda) f_{g_2'}(\lambda)$ đối với $(g_1', g_2', \lambda)$

trong một lân cận của $(g_1, g_2, 0)$ (Differentiable and Analytic Manifolds, R, 9.1.8). Vì G compact, tồn tại một nhóm con mở I của I' sao cho $f_{g_1g_2}(\lambda) = f_{g_1}(\lambda) f_{g_2}(\lambda)$ với mọi $g_1 \in G, g_2 \in G, \lambda \in I$. Nói cách khác, $\phi_\lambda \in \mathrm{Aut}\, G$ với $\lambda \in I$.

#### Bổ đề 3 {#lie-iii-s10-lem-3 .statement}

Cho $G$ và $G'$ là các nhóm Lie và $\phi$ là một đồng cấu từ $G$ vào $\mathrm{Aut}(G')$. Đặt $f(g, g') = (\phi(g))(g')$ với $g \in G, g' \in G'$. Xét các điều kiện sau:
(i) $f$ giải tích;
(ii) $f$ giải tích trong một lân cận của $(e_G, e_{G'})$;
(iii) với mọi $g' \in G'$, ánh xạ $g \mapsto f(g, g')$ là giải tích.
Khi đó (i) $\Leftrightarrow$ ((ii) và (iii)). Nếu G liên thông, (i) $\Leftrightarrow$ (ii).
Rõ ràng (i) suy ra (ii) và (iii). Cho $g_0 \in G, g_0' \in G'$. Với mọi $g \in G, g' \in G'$,

$$
f(gg_0, g'g_0') = (\phi(g)\phi(g_0))(g'g_0') = \phi(g)(\phi(g_0)g').\phi(g)(\phi(g_0)g_0').
$$

Điều này chứng minh hàm ý ((ii) và (iii)) $\Rightarrow$ (i). Cuối cùng, nếu $G'$ liên thông, $G'$ được sinh bởi mọi lân cận của $e_{G'}$ và do đó (ii) $\Rightarrow$ (iii).

### 2. NHÓM TỰ ĐẲNG CẤU CỦA MỘT NHÓM LIE (TRƯỜNG HỢP THỰC HOẶC PHỨC)

Trong số này, ta giả sử rằng $K = \mathbf{R}$ hoặc $\mathbf{C}$.

#### Bổ đề 4 {#lie-iii-s10-lem-4 .statement}

Cho $H$ là một nhóm Lie đơn liên hữu hạn chiều.
(i) Với mọi $u \in \mathrm{Aut}\, L(H)$, gọi $\theta(u)$ là tự đẳng cấu duy nhất của $H$ sao cho $L(\theta(u)) = u$. Khi đó ánh xạ $(u, g) \mapsto \theta(u)g$ từ $(\mathrm{Aut}\, L(H)) \times H$ vào $H$ là giải tích.
(ii) Cho $N$ là một nhóm con Lie của $H$ và $\mathrm{Aut}(H, N)$ là tập hợp các $v \in \mathrm{Aut}\, H$ sao cho $v(N) = N$. Khi đó $0^{-1}(\mathrm{Aut}(H, N))$ là một nhóm con Lie của $\mathrm{Aut}\, L(H)$.
(iii) Giả sử rằng $N$ là rời rạc và chuẩn, sao cho đại số Lie của $G = H/N$ được đồng nhất với $L(H)$. Với mọi $w \in \mathrm{Aut}\, G$, gọi $\eta(w)$ là tự đẳng cấu duy nhất của $H$ sao cho $L(\eta(w)) = L(w)$. Khi đó ánh xạ $\eta$ là một đẳng cấu của nhóm $\mathrm{Aut}\, G$ lên nhóm $\mathrm{Aut}(H, N)$.
Để chứng minh (i), theo Bổ đề 3 của no. 1, chỉ cần kiểm tra rằng ánh xạ $(u, g) \mapsto \theta(u)g$ là giải tích trong một lân cận của $(\mathrm{Id}_{L(H)}, e)$. Tồn tại một lân cận mở B của 0 trong $L(H)$ sao cho $\psi = \exp_H|B$ là một đẳng cấu giải tích của B lên một lân cận mở của e trong H. Tồn tại một lân cận mở U của $\mathrm{Id}_{L(H)}$ trong Aut $L(H)$ và một lân cận mở $B'$ của 0 trong $L(H)$ sao cho $U(B') \subset B$. Khi đó ánh xạ $(u, g) \mapsto \theta(u)g$ từ $U \times \psi(B')$ vào H được hợp thành bởi các ánh xạ sau:

ánh xạ $(u, g) \mapsto (u, \psi^{-1}(g))$ từ $U \times \psi(B')$ vào $U \times B'$;
ánh xạ $(u, x) \mapsto u(x)$ từ $U \times B'$ vào $B$;
ánh xạ $y \mapsto \psi(y)$ từ $B$ vào $G$.

Do đó ánh xạ này là giải tích.

Gọi $p$ là ánh xạ chính tắc của H vào không gian thuần nhất $H/N$. Khi đó $\theta^{-1}(\mathrm{Aut}(H, N))$ là tập hợp các $u \in \mathrm{Aut}\ L(H)$ sao cho
$$
p(\theta(u)g) = p(e), \quad p(\theta(u^{-1})g) = p(e)
$$
với mọi $g \in N$. Theo § 8, no. 2, Định lý 2 và Hệ quả 2 của Định lý 2, điều này chứng minh (ii).

Giả sử rằng N là rời rạc và chuẩn tắc. Cho $w \in \mathrm{Aut}\ G$. Khi đó
$$
L(p \circ \eta(w)) = L(\eta(w)) = L(w) = L(w \circ p)
$$
suy ra $p \circ \eta(w) = w \circ p$ và do đó $\eta(w) \in \mathrm{Aut}(H, N)$. Rõ ràng ánh xạ $\eta$ từ $\mathrm{Aut}\ G$ vào $\mathrm{Aut}(H, N)$ là một đơn cấu. Đồng cấu này là toàn ánh vì $p : H \to G$ là một toàn ánh địa phương.

Cho G là một nhóm compact địa phương và $\Gamma$ là nhóm tự đẳng cấu của G. Nhắc lại rằng một tôpô $\mathcal{T}_\beta$ đã được xác định trên $\Gamma$ (Tôpô đại cương, Chương X, § 3, no. 5). Đây là tôpô thô nhất sao cho các ánh xạ $v \mapsto v$ và $v \mapsto v^{-1}$ từ $\Gamma$ vào $C_c(G; G)$ (không gian các ánh xạ liên tục từ G vào G với tôpô hội tụ compact) là liên tục. Tôpô $\mathcal{T}_\beta$ tương thích với cấu trúc nhóm trên $\Gamma$ (loc. cit.). Với mọi tập con compact L của G và mọi lân cận U của $e_G$ trong G, gọi $N(L, U)$ là tập hợp các $\phi \in \Gamma$ sao cho $\phi(g) \in gU$ và $\phi^{-1}(g) \in gU$ với mọi $g \in L$; khi đó các $N(L, U)$ tạo thành một hệ cơ bản các lân cận của $e_\Gamma$. Nếu G được sinh bởi một tập con compact C, tôpô $\mathcal{T}_\beta$ cũng là tôpô thô nhất sao cho các ánh xạ $v \mapsto v|C$ và $v \mapsto v^{-1}|C$ từ $\Gamma$ vào $C_u(C; G)$ là liên tục (vì mọi tập con compact của G đều được chứa trong $(C \cup C^{-1})^n$ với n đủ lớn). Nếu K là compact địa phương và V là một không gian vectơ hữu hạn chiều trên K, tôpô $\mathcal{T}_\beta$ trên $\mathbf{GL}(V)$ chính là tôpô thông thường.

#### Định lý 1 {#lie-iii-s10-thm-1 .statement}

Cho G là một nhóm Lie hữu hạn chiều và $G_0$ là thành phần đơn vị của nó. Giả sử rằng G được sinh bởi $G_0$ và một số hữu hạn phần tử.

(i) Tồn tại duy nhất một cấu trúc đa tạp giải tích trên $\mathrm{Aut}\ G$ thỏa mãn điều kiện sau:
(AUT) với mọi đa tạp giải tích M và mọi ánh xạ f từ M vào $\mathrm{Aut}\ G$, f là giải tích khi và chỉ khi ánh xạ $(m, g) \mapsto f(m)g$ từ $M \times G$ vào G là giải tích.

Giả sử trong phần còn lại của mệnh đề rằng Aut G có cấu trúc này.
(ii) Aut G là một nhóm Lie hữu hạn chiều.
(iii) Cấu xạ $\phi : u \mapsto L(u)$ của Aut G vào Aut L(G) là giải tích.
(iv) Nếu G liên thông, $\phi$ là một đẳng cấu của nhóm Lie Aut G lên một nhóm Lie con của Aut L(G); nhóm Lie con này bằng Aut L(G) nếu G liên thông đơn.
(v) Cho $a$ là tập hợp các tự đẳng cấu vi phân của G. Khi đó $a$ là một đại số Lie của các trường vectơ và luật phép toán vi phân liên kết với ánh xạ $(u, g) \mapsto u(g)$ của (Aut G) $\times$ G vào G là một đẳng cấu của L(Aut G) lên $a$.
(vi) Tôpô của nhóm Lie Aut G là tôpô $\mathcal{T}_\beta$.
(a) Tính duy nhất của cấu trúc giải tích được xét trong (i) là hiển nhiên.
(b) Giả sử G liên thông. Cho H là không gian phủ phổ quát của G, $p$ là cấu xạ chính tắc của H lên G và N = Ker $p$. Ta đưa vào các ký hiệu $\theta$, $\eta$ và Aut(H, N) của Bổ đề 4. Ta chuyển cấu trúc nhóm Lie của Aut L(G) sang Aut H bằng $\theta$. Khi đó Aut H trở thành một nhóm Lie hữu hạn chiều và Aut(H, N) trở thành một nhóm Lie con của Aut H (Bổ đề 4 (ii)). Ta chuyển cấu trúc nhóm Lie của Aut(H, N) sang Aut G bằng $\eta^{-1}$. Khi đó Aut G trở thành một nhóm Lie hữu hạn chiều. Các tính chất (ii), (iii) và (iv) của định lý được thỏa mãn và ánh xạ $(u, g) \mapsto u(g)$ của (Aut G) $\times$ G vào G là giải tích (Bổ đề 4 (i)). Cho M là một đa tạp giải tích, $f$ là một ánh xạ của M vào Aut G và $\phi$ là ánh xạ $(m, g) \mapsto f(m)g$ của M $\times$ G vào G. Rõ ràng, nếu $f$ là giải tích thì $\phi$ là giải tích. Giả sử rằng $\phi$ là giải tích. Khi đó T$\phi$: TM $\times$ TG $\to$ TG là giải tích; hạn chế của nó lên M $\times$ L(G), tức là ánh xạ $(m, x) \mapsto L(f(m))x$ của M $\times$ L(G) vào L(G), do đó là giải tích; vì L(G) hữu hạn chiều, suy ra ánh xạ $m \mapsto L(f(m))$ của M vào Aut L(G) là giải tích và do đó $f$ là giải tích. Như vậy (i) được thỏa mãn.

Cho L(G) một chuẩn. Với mọi $\lambda > 0$, cho B_\lambda là quả cầu mở có tâm 0 và bán kính $\lambda$ trong L(G). Ta chọn $\lambda > 0$ đủ nhỏ để $\psi = \exp_G|_{B_\lambda}$ là một đẳng cấu của đa tạp giải tích B_\lambda lên đa tạp con mở $\psi(B_\lambda)$ của G. Cho $\Phi$ là một bộ lọc trên Aut G. Để $\Phi$ hội tụ tới $\mathrm{Id}_G$ trong Aut G, điều kiện cần và đủ là $L(\Phi)$ hội tụ tới $\mathrm{Id}_{L(G)}$ trong Aut L(G) và do đó $L(\Phi)|_{B_{\lambda/2}}$ và $L(\Phi)^{-1}|_{B_{\lambda/2}}$ hội tụ đều tới $\mathrm{Id}_{B_{\lambda/2}}$. Điều kiện này kéo theo $\Phi|\psi(B_{\lambda/2})$ và $\Phi^{-1}|\psi(B_{\lambda/2})$ hội tụ đều tới $\mathrm{Id}_{\psi(B_{\lambda/2})}$. Ngược lại, giả sử rằng $\Phi|\psi(B_{\lambda/2})$ hội tụ đều tới $\mathrm{Id}_{\psi(B_{\lambda/2})}$. Tồn tại M $\in \Phi$ sao cho, nếu $u \in M$, thì $u(\psi(B_{\lambda/2})) \subset \psi(B_{2\lambda/3})$; khi đó L(u)(B_{\lambda/2}) là một tập con liên thông của L(G) mà ảnh qua $\exp_G$ được chứa trong $\psi(B_{2\lambda/3})$, do đó L(u)(B_{\lambda/2}) không giao với $B_\lambda - B_{2\lambda/3}$ và vì vậy L(u)(B_{\lambda/2}) $\subset$ B_\lambda; khi đó giả thiết rằng $\Phi|\psi(B_{\lambda/2})$ hội tụ đều tới $\mathrm{Id}_{\psi(B_{\lambda/2})}$ kéo theo $L(\Phi)|_{B_{\lambda/2}}$ hội tụ đều tới $\mathrm{Id}_{B_{\lambda/2}}$. Suy ra rằng:

$$
(\Phi \text{ hội tụ tới } \mathrm{Id}_G \text{ trong Aut } G) \iff (\Phi \text{ hội tụ tới } \mathrm{Id}_G \text{ theo } \mathcal{T}_\beta).
$$

Điều này chứng minh (vi).

Cho D là luật của phép toán vi phân liên kết với luật của phép toán trái của Aut(G) trên G. Theo các Mệnh đề 1 và 2 của no. 1, $D(L(\text{Aut } G)) = a$. Do đó a là một đại số Lie của các trường vectơ và D là một cấu xạ từ $L(\text{Aut } G)$ lên a. Cho $x_1$ và $x_2$ là các phần tử của $L(\text{Aut } G)$ sao cho $D(x_1) = D(x_2)$. Khi đó các luật của phép toán $(\lambda, g) \mapsto (\exp \lambda x_1)g$ và $(\lambda, g) \mapsto (\exp \lambda x_2)g$ của K trên G có cùng luật của phép toán vi phân liên kết; do đó, với $|\lambda|$ đủ nhỏ, $\exp \lambda x_1$ và $\exp \lambda x_2$ trùng nhau trên một lân cận của e ($§ 4$, no. 7, Định lý 6), do đó $\exp \lambda x_1 = \exp \lambda x_2$. Suy ra $x_1 = x_2$ và do đó D là một đẳng cấu từ $L(\text{Aut } G)$ lên a.

Định lý đã được chứng minh hoàn toàn đối với G liên thông.

(c) Ta chuyển sang trường hợp tổng quát. Theo giả thiết, G được sinh bởi $G_0$ và một số hữu hạn các phần tử $x_1, x_2, \ldots, x_n$. Mọi $u \in \text{Aut } G$ đều để $G_0$ ổn định. Gọi $\text{Aut}_1 G$ là tập hợp các $u \in \text{Aut } G$ mà khi chuyển qua thương, cho tự đẳng cấu đồng nhất của $G/G_0$. Đây là một nhóm con chuẩn tắc của $\text{Aut } G$. Theo phần (b) của chứng minh, $\text{Aut } G_0$ có một cấu trúc nhóm Lie chính tắc và ánh xạ $(g_1, g_2, \ldots, g_n, u) \mapsto (ug_1, ug_2, \ldots, ug_n)$ từ $G_0^n \times \text{Aut } G_0$ vào $G_0^n$ là giải tích. Gọi P là tích nửa trực tiếp tương ứng của $\text{Aut } G_0$ bởi $G_0^n$; nó là một nhóm Lie hữu hạn chiều ($§ 1$, no. 4, Mệnh đề 7).

Nếu $w \in \text{Aut}_1 G$, ta viết
$$
w_0 = w|G_0 \in \text{Aut } G_0 \\
w_i = x_i^{-1}w(x_i) \in G_0 \quad (1 \leq i \leq n) \\
\zeta(w) = ((w_1, \ldots, w_n), w_0) \in P.
$$
Với mọi $w, w'$ trong $\text{Aut}_1 G$,
$$
\begin{align*}
\zeta(w)\zeta(w') &= ((w_1, \ldots, w_n)(w_0(w'_1), \ldots, w_0(w'_n)), w_0w'_0) \\
&= ((w_1w_0(w'_1), \ldots, w_nw_0(w'_n)), w_0w'_0) \\
&= ((x^{-1}w(x_1)w(x_1^{-1}w'(x_1)), \ldots, x_n^{-1}w(x_n)w(x_n^{-1}w'(x_n))), w_0w'_0) \\
&= (((ww')_1, \ldots, (ww')_n), (ww')_0) \\
&= \zeta(ww')
\end{align*}
$$
và do đó $\zeta$ là một đồng cấu từ $\text{Aut}_1 G$ vào P. Đồng cấu này hiển nhiên đơn ánh.

Ta chứng minh rằng $\zeta(\text{Aut}_1 G)$ là đóng trong P. Cho $\Phi$ là một lọc trên $\text{Aut}_1 G$ sao cho $\zeta(\Phi)$ hội tụ đến một điểm $((w_1, \ldots, w_n), w_0)$ của P. Khi đó $\Phi$ hội tụ điểm-điểm đến một ánh xạ v từ G vào G. Rõ ràng v là một tự đồng cấu của nhóm G. Hơn nữa, v để mỗi lớp kề modulo $G_0$ ổn định và $v|G_0 = w_0$. Suy ra $v \in \text{Aut}_1 G$. Vì $\zeta(v) = ((w_1, \ldots, w_n), w_0)$, ta đã chứng minh rằng $\zeta(\text{Aut}_1 G)$ là đóng trong P.

(d) Trong phần (d) của chứng minh, ta giả thiết rằng $K = \mathbf{R}$. Theo $§ 8$, no. 2, Định lý 2, $\zeta(\text{Aut}_1 G)$ là một nhóm con Lie của P. Ta chuyển cấu trúc nhóm Lie thực trên $\zeta(\text{Aut}_1 G)$ sang $\text{Aut}_1 G$ bằng $\zeta^{-1}$. Do đó $\text{Aut}_1 G$ trở thành một nhóm Lie hữu hạn chiều.

Cho M là một đa tạp giải tích, f một ánh xạ từ M vào Aut_1G và φ là ánh xạ (m, g) ↦ f(m)g từ M × G vào G. Ta có các tương đương sau:

f giải tích
⇔ các ánh xạ m: ↦ (f(m))_i, với 0 ≤ i ≤ n, là giải tích
⇔ {các ánh xạ m ↦ f(m)x_i từ M vào G, với 1 ≤ i ≤ n, là giải tích
và
ánh xạ (m, g) ↦ f(m)g từ M × G_0 vào G là giải tích
⇔ φ là giải tích.

Với w ∈ Aut_1G, L(w) = L(w_0) và do đó cấu xạ w ↦ L(w) từ Aut_1G vào Aut L(G) là giải tích. Ta thấy như trong (b) rằng luật của phép toán vi phân liên kết với luật của phép toán của Aut_1G trên G là một đẳng cấu từ L(Aut_1G) lên a.

Cho C là một tập con compact của G_0 sinh G_0. Để một lọc Φ hội tụ đến $\mathrm{Id}_G$ trên Aut_1G, điều kiện cần và đủ là Φ|(C ∪ {x_1} ∪ ... ∪ {x_n}) và Φ^{-1}|(C ∪ {x_1} ∪ ... ∪ {x_n}) hội tụ đều đến

Id_a|(C ∪ {x_1} ∪ ... ∪ {x_n}).

Do đó tôpô của Aut_1G là tôpô $\mathcal{T}_\beta$.

Hiển nhiên Aut_1G là mở trong Aut G với tôpô $\mathcal{T}_\beta$. Trên Aut G tồn tại một cấu trúc nhóm Lie tương thích với tôpô này và cảm sinh trên Aut_1G cấu trúc đã xây dựng ở trên ($§ 8$, no. 1, Hệ quả 2 của Định lý 1). Việc nhóm Lie Aut G có các tính chất của định lý suy ra từ các tính chất tương ứng của Aut_1G.

(e) Trong phần (e) của chứng minh, ta giả thiết rằng $K = C$. Theo (c) và Định lý 2 của $§ 8$, no. 2, trên Aut_1G tồn tại một cấu trúc nhóm Lie thực sao cho ζ là một đẳng cấu từ Aut_1G lên một nhóm con Lie thực của P.

Luật của phép toán (w, g) ↦ wg của (Aut_1G) × G trên G là giải tích thực. Gọi D là luật của phép toán vi phân liên kết. Theo các Mệnh đề 1 và 2 của no. 1, D(L(Aut_1G)) = a.

Với mọi α ∈ a, gọi α_0 là hạn chế của α trên G_0; nó là một tự đẳng cấu vi phân của G_0 mà ta đồng nhất, do phần (b) của chứng minh, với một phần tử của L(Aut G_0). Với 1 ≤ i ≤ n, ta viết

$$ \alpha_i = x_i^{-1} \alpha(x_i) \in L(G) = L(G_0). $$

Cuối cùng, ta viết $f(\alpha) = ((\alpha_1, ..., \alpha_n), \alpha_0) \in L(P)$. Khi đó f là một ánh xạ tuyến tính C từ a vào L(P).

Mặt khác, rõ ràng $L(\zeta) = f \circ D$. Do đó $L(\zeta)(L(Aut_1G)) = f(a)$ là một không gian con vectơ phức của L(P). Theo Mệnh đề 2 của § 4, no. 2, $\zeta(Aut_1G)$ là một nhóm con Lie phức của P và ta có thể tiến hành đúng như trong (d): ta thực hiện phép chuyển cấu trúc nhóm Lie phức trên $\zeta(Aut_1G)$ sang Aut_1G bằng $\zeta^{-1}$ và thấy, như trong (d), rằng Aut_1G có các tính chất tương tự các tính chất (i), (ii), (iii), (v) và (vi) của định lý.

Rõ ràng Aut₁G là mở trong Aut G với tôpô $\mathcal{T}_\beta$. Cho $w \in \mathrm{Aut}\ G$. Gọi $\sigma$ là tự đẳng cấu $v \mapsto wvw^{-1}$ của Aut₁G. Nó giải tích thực ($§ 8$, no. 1, Định lý 1), $L(\sigma)$ là một tự đẳng cấu $\mathbf{R}$-tuyến tính của $L(\mathrm{Aut}_1 G)$ và

$$
D \circ L(\mathrm{Aut}_1 G) \circ D^{-1}
$$

là một tự đẳng cấu $\mathbf{R}$-tuyến tính của $a$. Tự đẳng cấu này cũng là tự đẳng cấu của $a$ dẫn xuất từ $w$ bằng phép chuyển cấu trúc; vì $w$ là K-giải tích, ta thấy rằng $L(\sigma)$ là K-tuyến tính. Do đó $\sigma$ là K-giải tích ($§ 3$, no. 8, Mệnh đề 32). Theo $§ 1$, no. 9, Mệnh đề 18, trên Aut G tồn tại duy nhất một cấu trúc nhóm Lie K sao cho $\mathrm{Aut}_1 G$ là một nhóm con Lie mở của Aut G. Việc cấu trúc này có các tính chất của định lý suy ra từ các tính chất tương ứng của $\mathrm{Aut}_1 G$.

#### Hệ quả 1 {#lie-iii-s10-thm-1-cor-1 .statement}

*Một nhóm Lie thực hữu hạn chiều G và $G_0$ là thành phần đơn vị của nó. Giả sử rằng G được sinh bởi $G_0$ và một số hữu hạn phần tử. Khi đó Aut G có tôpô $\mathcal{T}_\beta$ và là một nhóm Lie thực hữu hạn chiều.*

#### Hệ quả 2 {#lie-iii-s10-thm-1-cor-2 .statement}

*Nếu G là một nhóm Lie thực hoặc phức liên thông nửa đơn. Nhóm Int G là thành phần đơn vị của Aut G.*

Ánh xạ $u \mapsto L(u)$ là một đẳng cấu của Aut G lên một nhóm con Lie của Aut $L(G)$ (Định lý 1). Ảnh của Int G qua đẳng cấu này là Ad G. Nhưng Ad G là thành phần đơn vị của Aut $L(G)$ ($§ 9$, no. 8, Mệnh đề 30 (ii)).

### 3. NHÓM TỰ ĐẲNG CẤU CỦA MỘT NHÓM LIE (TRƯỜNG HỢP SIÊU METRIC)

#### Định lý 2 {#lie-iii-s10-thm-2 .statement}

*Khi K là siêu metric và compact địa phương và G là một nhóm Lie compact, các mệnh đề (i), (ii), (iii), (v) và (vi) của Định lý 1 là đúng.*
(a) Tính duy nhất của cấu trúc giải tích được xét trong (i) là hiển nhiên.
(b) Giả sử G là nhóm Lie được định nghĩa bởi đại số Lie khả chuẩn L. Khi đó G là một quả cầu vừa mở vừa đóng trong L. Cho $w \in \mathrm{Aut}\ G$. Khi đó $L(w)$ trùng với $w$ trong một lân cận của 0. Cho $x \in G$. Gọi $p$ là đặc số của trường thặng dư. Khi đó $p^n x$ tiến tới 0 khi $n$ tiến tới $+\infty$. Do đó tồn tại $n$ sao cho $w(p^n x) = L(w)(p^n x)$. Vì vậy

$$
p^n w(x) = w(x)^{p^n} = w(x^{p^n}) = w(p^n x)
= L(w)(p^n x) = p^n L(w)(x)
$$

do đó $w(x) = L(w)(x)$. Vậy, $w = L(w)|G$.

Gọi $\Gamma$ là tập hợp các $\gamma \in \mathrm{Aut}\ L(G)$ sao cho $\gamma(G) = G$. Vì G mở và compact trong $L(G)$, $\Gamma$ là một nhóm con mở của $\mathrm{Aut}\ L(G)$. Theo trên, Aut G được đồng nhất với $\Gamma$, do đó có một cấu trúc nhóm Lie trên Aut G, với cấu trúc đó các tính chất (i), (ii), (iii) và (vi) của Định lý 1 là hiển nhiên. Tính chất (v) suy ra từ các Mệnh đề 1 và 3 của no. 1.

(c) Ta chuyển sang trường hợp tổng quát. Theo § 7, no. 1, Mệnh đề 1, tồn tại một nhóm con compact mở G_0 của G thuộc kiểu được xét trong (b). Khi đó G được sinh bởi G_0 và một số hữu hạn phần tử x_1, x_2, ..., x_n. Gọi Aut_1G là tập hợp các u ∈ Aut G sao cho u(G_0) = G_0 và u(x_iG_0) = x_iG_0 với 1 ≤ i ≤ n. Như trong chứng minh Định lý 1, phần (c), ta định nghĩa một tích nửa trực tiếp P của Aut G_0 bởi G_0^n và một đơn cấu ζ từ Aut_1G vào P, mà ảnh của nó là đóng trong P.

(d), (e): lập luận hoàn toàn giống như trong các phần (d), (e) của chứng minh Định lý 1, với R được thay bằng Q_p và sử dụng Mệnh đề 3 thay cho Mệnh đề 2.

#### Nhận xét {#lie-iii-s10-n3-rem-1 .statement}

Nếu K = Q_p và nhóm Lie G được sinh bởi một tập con compact (xem Bài tập 2), các mệnh đề (i), (ii), (iii) và (vi) của Định lý 1 vẫn đúng, nhưng (v) thì không (Bài tập 3).

### Bài tập {#lie-iii-s10-exercises}

Xem [các bài tập cho § 10](exercises/s10/).
