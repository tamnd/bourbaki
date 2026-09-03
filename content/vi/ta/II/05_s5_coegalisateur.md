---
book: ta
book_title: Topologie algébrique
chapter: II
chapter_title: GROUPOÏDES
section: 5
section_title: Coégalisateur
lang: vi
source: ta-i-iv-fr
book_pages: TA II.196-TA II.214, TA II.227-TA II.228
pdf_pages: 0212-0230, 0243-0244
extraction: native
subsections:
    - "no": 1
      title: Contraction des flèches d’une homotopie
      page: 196
      pdf_page: 212
    - "no": 2
      title: Définition du coégalisateur
      page: 199
      pdf_page: 215
    - "no": 3
      title: Comparaison des groupes d’isotropie du cohomotopeur et du coégalisateur
      page: 201
      pdf_page: 217
    - "no": 4
      title: Groupe d’isotropie d’un coégalisateur
      page: 206
      pdf_page: 222
    - "no": 5
      title: Quotient d’un groupoïde par l’action d’un groupe
      page: 210
      pdf_page: 226
statements: 22
exercises: 3
content_sha256: 4cc7a0d01672bd0cb00ea29e03e781387f1ffbf388127165a3ba2c27e77968f9
translated_from: content/en-mt/ta/II/05_s5_coegalisateur.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 711dd705966b5505898a3e12ce8803f21dfe784179862e01ca5ae334296e89f9
translation_model: gpt-5.4
translation_run: translate-vi-09985b18
glossary_version: 34
glossary_terms_sha256: 94c33ea4bbddcd7e9d09755bf5c19a086ac01ef963506e0a661d16aafbbe7f92
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 5. ĐỐI ĐỒNG ĐẲNG TỬ

### 1. Sự co rút các mũi tên của một đồng luân

Cho H là một đồ thị có hướng, G là một vị nhóm, $\varphi$ và $\psi$ là các cấu xạ đồ thị có hướng từ H vào G, và $h:$ Som(H) $\rightarrow$ Fl(G) là một đồng luân nối $\varphi$ với $\psi$. Gọi $G'$ là vị nhóm suy ra từ G bằng sự co rút các mũi tên của ảnh của $h($II, p. 175, No.$^o11$) và $\beta : G\rightarrow G'$ là cấu xạ chính tắc.

Ta ký hiệu bởi Γ đồ thị có hướng (Som(G), Som(H), Som($\varphi$ ), Som($\psi$ )). Theo định nghĩa của một đồng luân, cặp (Id$_{Som(G)}, h$) là một cấu xạ đồ thị có hướng từ Γ vào G; nó mở rộng thành một cấu xạ vị nhóm duy nhất $\eta :$ Grp(Γ) $\rightarrow$ G. Theo phép dựng, tập các đỉnh của $G'$ là tập các thành phần liên thông của đồ thị có hướng Γ.

Trong tất cả những gì tiếp theo trong No.$^o$ này, ta sẽ giả thiết rằng vị nhóm G là bắc cầu. Theo nhận xét 1 của II, p. 170, điều này tương đương với việc giả thiết rằng vị nhóm $G'$ cũng vậy. Ta cũng cố định một đỉnh $a_0$ của G.

Ta ký hiệu bởi $\widetilde{\Gamma}$ đồ thị liên kết với đồ thị có hướng Γ (xem II, p. 156). Tập các chu trình độ dài $\geqslant 1$ trong $\widetilde{\Gamma}$ được đồng nhất với tập $\Omega (\widetilde{\Gamma})$ các dãy hữu hạn $(z_1, . . . , z_n)$, trong đó $n$ là một số nguyên sao cho $n\geqslant 1$ và $z_1, . . . , z_n$ là các phần tử của Fl($\widetilde{\Gamma}$) sao cho $t(z_i) =o(z_{i+1})$ với mọi số nguyên $i$ sao cho $1\leqslant i < n$ và $t(z_n) =o(z_1)$.

Cho $\mathbf{z}= ((b_1, \varepsilon_1), . . . ,(b_n, \varepsilon_n))$ là một phần tử của $\Omega (\widetilde{\Gamma})$. Lớp liên hợp của phần tử

Int($g$)$(\eta (\mathbf{z})) =gh(b_1)^{\varepsilon_1}. . . h(b_n)^{\varepsilon_n}g^{-1}$

trong $G_{a_0}$ không phụ thuộc vào lựa chọn mũi tên $g$ của G nối đỉnh $a_0$ với gốc của $(b_1, \varepsilon )$. Ta ký hiệu lớp liên hợp này bởi $c(\mathbf{z})$.

#### Mệnh đề 1 {#ta-ii-s5-prop-1 .statement tag=01UI}

Cấu xạ nhóm $\beta_{a_0}: G_{a_0}\rightarrow G'_{\beta(a_0)}$ là toàn ánh, và hạt nhân của nó là nhóm con nhỏ nhất của $G_{a_0}$ chứa các lớp liên hợp $c(\mathbf{z})$ với $\mathbf{z}\in \Omega (\widetilde{\Gamma})$.

Gọi K là vị nhóm con phân biệt nhỏ nhất của G mà tập các mũi tên chứa ảnh của $h$. Cấu xạ $G_{a_0}\rightarrow G'_{\beta(a_0)}$ là toàn ánh và hạt nhân của nó bằng $K_{a_0}($II, p. 170, prop. 2). Khi đó mệnh đề suy ra từ mệnh đề 8 của II, p. 176.

#### Định nghĩa 1 {#ta-ii-s5-def-1 .statement tag=01UJ}

Một tập con Z của $\Omega (\widetilde{\Gamma})$ được gọi là phân biệt (đối với cặp $(\varphi , \psi )$) nếu nó thỏa mãn các tính chất sau:

(i) Với mọi mũi tên $z$ của $\widetilde{\Gamma}$, ta có $(z, z)\in Z$ ;

(ii) Với mọi $(z_1, . . . , z_n)\in$ Z, ta có $(\overline{z}_n, . . . ,\overline{z}_2,\overline{z}_1)\in$ Z và $(z_n, z_1, . . . , z_{n-1})\in Z$ ;

(iii) Cho $\mathbf{z}= (z_1, . . . , z_n)$ và $\mathbf{z}'= (z'_1, . . . , z'_m)$ là các phần tử của Z sao cho $t(z_n) =o(z'_1)$. Đặt $\mathbf{z}\mathbf{z}'= (z_1, . . . , z_n, z'_1, . . . , z'_m)$. Nếu hai phần tử trong số $\mathbf{z},\mathbf{z}',\mathbf{z}\mathbf{z}'$ thuộc Z, thì phần tử thứ ba cũng vậy;

(iv) Với mọi mũi tên $f$ của H, đặt $\widetilde{\varphi}(f,1) =\widetilde{\psi}(f,-1) =$ $\varphi (f)$ và $\widetilde{\varphi}(f,-1) =\widetilde{\psi}(f,1) =\psi (f)$. Cho $n$ là một số nguyên $\geqslant$ 1 và $(f_1, \varepsilon_1), . . . ,(f_n, \varepsilon_n)$ là một dãy các phần tử của Fl(H) $\times  \{-1,1\}$ sao cho $\widetilde{\psi}(f_i, \varepsilon_i) =\widetilde{\varphi}(f_{i+1}, \varepsilon_{i+1})$ với $1\leqslant i < n$ và $\widetilde{\psi}(f_n, \varepsilon_n) =\widetilde{\varphi}(f_1, \varepsilon_1)$; ký hiệu $a_i$ là gốc của $f_i$ và $b_i$ là đích của nó. Để $((a_1, \varepsilon_1), . . . ,(a_n, \varepsilon_n))$ thuộc Z, điều kiện cần và đủ là $((b_1, \varepsilon_1), . . . ,(b_n, \varepsilon_n))$ thuộc Z.

Giao trong $\Omega (\widetilde{\Gamma})$ của mọi họ các tập con phân biệt (đối với $(\varphi , \psi )$) lại là phân biệt. Đặc biệt, tồn tại một tập con phân biệt nhỏ nhất chứa một tập con Z đã cho của $\Omega (\widetilde{\Gamma})$.

#### Mệnh đề 2 {#ta-ii-s5-prop-2 .statement tag=01UK}

Nếu N là một nhóm con phân biệt của $G_a$, tập các phần tử $\mathbf{z}\in \Omega (\widetilde{\Gamma})$ sao cho $c(\mathbf{z})$ được chứa trong N là một tập con phân biệt của $\Omega (\widetilde{\Gamma})$.

Cho Z ký hiệu tập các phần tử $\mathbf{z}\in \Omega (\widetilde{\Gamma})$ sao cho $c(\mathbf{z})\subset N$.

Cho $z\in$ Fl($\widetilde{\Gamma}$). Ta có $c(z, z) =\{e_a\}$ theo định nghĩa, do đó $(z, z)\in Z$.

Cho $(z_1, . . . , z_n)\in Z$. Theo định nghĩa của $c$, lớp liên hợp $c(z_1, . . . , z_n)$ bằng $c(z_n, z_1, . . . , z_{n-1})$ và được tạo thành bởi các phần tử nghịch đảo của các phần tử của $c(\overline{z}_n, . . . ,\overline{z}_1)$. Điều này cho thấy Z thỏa mãn điều kiện (ii).

Với ký hiệu của điều kiện (iii), ta có thể chọn các phần tử $u\in c(\mathbf{z}),v\in c(\mathbf{z}')$ và $w\in c(\mathbf{z}\mathbf{z}')$ sao cho $uv=w$. Nếu hai trong ba phần tử $u,v$ và $w$ thuộc N, thì phần tử thứ ba cũng vậy, do đó N thỏa mãn (iii).

Ký hiệu là ký hiệu của (iv), ta có, với mọi số nguyên $i$ sao cho $1\leqslant i\leqslant n$, quan hệ

$$
\varphi (f_i)h(b_i) =h(a_i)\psi (f_i)
$$

vì $h$ là một đồng luân nối $\varphi$ với $\psi$. Đẳng thức này cũng có thể viết thành

$$
\widetilde{\varphi}(f_i, \varepsilon_i)h(b_i)^{\varepsilon_i}=h(a_i)^{\varepsilon_i}\widetilde{\psi}(f_i, \varepsilon_i)
$$

Tính đến các quan hệ $\widetilde{\psi}(f_i, \varepsilon_i) =\widetilde{\varphi}(f_{i+1}, \varepsilon_{i+1})$ với $1\leqslant i < n$ và $\widetilde{\psi}(f_n, \varepsilon_n) =\widetilde{\varphi}(f_1, \varepsilon_1)$, ta suy ra

$$
\widetilde{\varphi}(f_1, \varepsilon_1)h(b_1)^{\varepsilon_1}. . . h(b_n)^{\varepsilon_n}=h(a_1)^{\varepsilon_1}. . . h(a_n)^{\varepsilon_n}\widetilde{\varphi}(f_1, \varepsilon_1)
$$

nên các lớp liên hợp $c((a_1, \varepsilon_1), . . . ,(a_n, \varepsilon_n))$ và $c((b_1, \varepsilon_1), . . . ,(b_n, \varepsilon_n))$ bằng nhau. Điều này cho thấy Z thỏa mãn điều kiện (iv) và hoàn tất chứng minh của mệnh đề.

#### Hệ quả {#ta-ii-s5-n1-cor-1 .statement tag=01UL}

Cho Z là một tập con của $\Omega (\widetilde{\Gamma})$; để các lớp liên hợp $c(\mathbf{z})$, với $\mathbf{z}\in$ Z, sinh hạt nhân của đồng cấu chính tắc $\beta_{a_0}: G_{a_0}\rightarrow G'_{\beta(a_0)}$, chỉ cần tập con phân biệt nhỏ nhất của $\Omega (\widetilde{\Gamma})$ chứa Z bằng $\Omega (\widetilde{\Gamma})$.

Cho N là nhóm con nhỏ nhất của $G_{a_0}$ chứa $c(\mathbf{z})$ với mọi $\mathbf{z}\in Z$; nó là phân biệt. Cho $Z'$ là tập hợp các phần tử $\mathbf{z}$ của $\Omega (\widetilde{\Gamma})$ sao cho $c(\mathbf{z})\in N$. Theo mệnh đề 2, $Z'$ là một tập con phân biệt của $\Omega (\widetilde{\Gamma})$. Nó chứa Z. Vậy theo giả thiết, nó bằng $\Omega (\widetilde{\Gamma})$. Khi đó suy ra từ mệnh đề 1 (II, p. 197) rằng N là hạt nhân của đồng cấu $\beta_a$.

### 2. Định nghĩa của đối đồng đẳng tử

Cho H là một quiver, G là một groupoid và $\varphi ,\psi$ là các cấu xạ quiver từ H vào G. Ký hiệu Coh($\varphi , \psi$ ) là đồng điều tử của cặp $(\varphi , \psi )$ (II, p. 185, def. 3)$,\alpha : G\rightarrow$ Coh($\varphi , \psi$ ) là cấu xạ groupoid chính tắc và $h$ là đồng luân chính tắc nối $\alpha \circ \varphi$ với $\alpha \circ \psi$.

Cho Coeg($\varphi , \psi$ ) là groupoid thu được từ Coh($\varphi , \psi$ ) bằng phép co các mũi tên thuộc ảnh của $h$ (II, p. 196, n$^o$ 1), ký hiệu $\beta :$ Coh($\varphi , \psi$ )$\rightarrow$ Coeg($\varphi , \psi$ ) là cấu xạ chính tắc và đặt $\gamma =\beta \circ \alpha$.

#### Định nghĩa 2 {#ta-ii-s5-def-2 .statement tag=01UM}

Groupoid Coeg($\varphi , \psi$ ) được gọi là đối đồng đẳng tử của cặp $(\varphi , \psi )$; cấu xạ groupoid $\gamma$ được gọi là cấu xạ chính tắc từ G vào Coeg($\varphi , \psi$ ).

#### Mệnh đề 3 {#ta-ii-s5-prop-3 .statement tag=01UN}

Cặp (Coeg($\varphi , \psi$ )$, \gamma$ ) có tính chất phổ quát sau đây:

a) Ta có $\gamma \circ \varphi =\gamma \circ \psi$.

b) Cho $G'$ là một groupoid và $\theta : G\rightarrow G'$ là một cấu xạ groupoid sao cho $\theta \circ \varphi =\theta \circ \psi$. Tồn tại duy nhất một cấu xạ groupoid $\overline{\theta}:$ Coeg($\varphi , \psi$ )$\rightarrow G'$ sao cho $\overline{\theta}\circ \gamma =\theta$.

Cho $a$ là một đỉnh của H. Mũi tên $h(a)$ của Coh($\varphi , \psi$ ) nối $\alpha (\varphi (a))$ với $\alpha (\psi (a))$. Theo định nghĩa của groupoid Coeg($\varphi , \psi$ ), gốc và đích của mũi tên $\beta (h(a))$ bằng nhau; do đó ta có $\gamma (\varphi (a)) =\gamma (\psi (a))$.

Cho $f$ là một mũi tên của H; nếu $a$ ký hiệu gốc của nó và $b$ ký hiệu đích của nó, thì ta có

$$
\alpha (\varphi (f))\cdot h(b) =h(a)\cdot \alpha (\psi (b))
$$

Lấy ảnh bởi $\beta$ của hai vế của đẳng thức này, ta thu được quan hệ $\gamma (\varphi (f)) =\gamma (\psi (f))$. Điều này chứng minh mệnh đề a).

Hãy chứng minh b). Ánh xạ $\eta :$ Som(H) $\rightarrow$ Fl(G$'$) gắn với mỗi đỉnh $a$ của H mũi tên $e_{\theta(\varphi(a))}$ của $G'$ là một đồng luân nối $\theta \circ \varphi$ với $\theta \circ \psi$. Theo tính chất phổ quát của các cohomotopizer (II, p. 185, prop. 3), tồn tại một cấu xạ groupoid duy nhất $\theta_1:$ Coh($\varphi , \psi$ )$\rightarrow G'$ sao cho $\theta_1\circ \alpha =\theta$ và $\theta_1(h(a)) =e_{\theta(\varphi(a))}$ với mọi đỉnh $a$ của H. Theo prop. 7 của II, p. 176, tính chất sau này suy ra sự tồn tại của một cấu xạ groupoid duy nhất $\overline{\theta}:$ Coeg($\varphi , \psi$ )$\rightarrow G'$ sao cho $\overline{\theta}\circ \beta =\theta_1$. Khi đó ta có $\overline{\theta}\circ \gamma =\theta_1\circ \alpha =\theta$.

Ngược lại, nếu $\overline{\theta}':$ Coeg($\varphi , \psi$ )$\rightarrow G'$ là một cấu xạ groupoid sao cho $\overline{\theta}'\circ \gamma =\theta$, thì ta có $(\overline{\theta}'\circ \beta )\circ \alpha = (\overline{\theta}\circ \beta )\circ \alpha$, do đó $\overline{\theta}'\circ \beta =\overline{\theta}\circ \beta$ theo II, p. 185, prop. 3, do đó $\overline{\theta}'=\overline{\theta}$ theo prop. 7 của II, p. 176. Điều này chứng minh tính duy nhất của $\overline{\theta}$, vì thế mệnh đề b).

#### Hệ quả {#ta-ii-s5-n2-cor-1 .statement tag=01UO}

Groupoid Coeg($\varphi , \psi$ ) được sinh bởi ảnh của cấu xạ $\gamma$.

Gọi C là subgroupoid của Coeg($\varphi , \psi$ ) được sinh bởi ảnh của G; gọi $i$ là cấu xạ chính tắc từ C vào Coeg($\varphi , \psi$ ) và $\theta : G\rightarrow C$ là cấu xạ sao cho $i\circ \theta =\gamma$. Theo proposition 2, tồn tại một cấu xạ groupoid duy nhất $\overline{\theta}:$ Coeg($\varphi , \psi$ )$\rightarrow C$ sao cho $\overline{\theta}\circ \gamma =\theta$. Khi đó $\gamma =i\circ \overline{\theta}\circ \gamma$, do đó $i\circ \overline{\theta}$ là cấu xạ đồng nhất của Coeg($\varphi , \psi$ ) (loc. cit.). Đặc biệt, các ánh xạ Som($i$) và Fl($i$) là toàn ánh, vì vậy C = Coeg($\varphi , \psi$ ).

#### Nhận xét 1 {#ta-ii-s5-n2-rem-1 .statement tag=01UP}

Tập hợp các đỉnh của Coeg($\varphi , \psi$ ) là tập hợp các thành phần liên thông của quiver

Γ = (Som(G), Som(H), Som($\varphi$ ), Som($\psi$ ))

(II, p. 197). Nói cách khác, đó là tập thương của Som(G) theo quan hệ tương đương tinh nhất sao cho $\varphi (a)$ tương đương với $\psi (a)$ với mọi $a\in$ Som(G).

#### Nhận xét 2 {#ta-ii-s5-n2-rem-2 .statement tag=01UQ}

Ánh xạ Orb($\gamma$ ), suy ra từ $\gamma$ bằng cách chuyển qua các quỹ đạo, xác định bằng chuyển sang thương một song ánh từ tập hợp các thành phần liên thông của khung của cặp $(\varphi , \psi )$ lên tập hợp các quỹ đạo của đối đồng bằng hóa tử. Điều này suy ra từ II, p. 185, prop. 4 và từ sự kiện rằng ánh xạ suy ra từ $\beta$ bằng cách chuyển qua các quỹ đạo là song ánh ( II, p. 170, remark 1).

Do đó, ánh xạ của Som(G) vào Orb(Coeg($\varphi , \psi$ )) suy ra từ $\gamma$ đồng nhất tập hợp các quỹ đạo của Coeg($\varphi , \psi$ ) với tập thương của Som(G) theo quan hệ tương đương sinh bởi các cặp $(\varphi (x), \psi (x))$ với $x\in$ Som(H) và các cặp $(o(f), t(f))$ với $f\in$ Fl(G).

#### Nhận xét 3 {#ta-ii-s5-n2-rem-3 .statement tag=01UR}

Ánh xạ Fl($\gamma$ ) của Fl(G) vào Fl(Coeg($\varphi , \psi$ )) nói chung không toàn ánh.

### 3. So sánh các nhóm đẳng hướng của bộ đối đồng luân hóa và đối cân bằng tử

Cho H là một quiver, G là một groupoid, và $\varphi$ và $\psi$ là các cấu xạ quiver từ H vào G. Ta ký hiệu bởi $\alpha : G\rightarrow$ Coh($\varphi , \psi$ ), $\beta :$ Coh($\varphi , \psi$ )$\rightarrow$ Coeg($\varphi , \psi$ ) và $\gamma : G\rightarrow$ Coeg($\varphi , \psi$ ) các cấu xạ chính tắc của các groupoid, và bởi $h$ phép đồng luân chính tắc nối $\alpha \circ \varphi$ với $\alpha \circ \psi$. Các ký hiệu này được tóm tắt bởi biểu đồ sau

$\gamma$

H $^{\varphi}_{\psi}$ G $^{\alpha}$ Coh($\varphi , \psi$ )$^{\beta}$ Coeg($\varphi , \psi$ ) .

Trong toàn bộ phần còn lại của n$^o$ này, ta giả sử rằng khung của cặp $(\varphi , \psi )$ là một quiver liên thông và ta cố định một đỉnh $a_0$ của G. Do đó, các groupoid Coh($\varphi , \psi$ ) và Coeg($\varphi , \psi$ ) là bắc cầu.

Ký hiệu Γ là quiver (Som(G), Som(H), Som($\varphi$ ), Som($\psi$ )), $\widetilde{\Gamma}$ là đồ thị liên kết với Γ, và gọi $\Omega (\widetilde{\Gamma})$ là tập hợp các dãy hữu hạn $(z_1, . . . , z_n)$ các mũi của $\widetilde{\Gamma}$, với $n\geqslant 1$, sao cho đích của $z_i$ là gốc của $z_{i+1}$ nếu $1\leqslant i < n$ và đích của $z_n$ là gốc của $z_1$. Trong No. 1 đã xây dựng một ánh xạ $\mathbf{z}\mapsto c(\mathbf{z})$ từ tập hợp $\Omega (\widetilde{\Gamma})$ vào tập hợp các lớp liên hợp của nhóm Coh($\varphi , \psi$ )$_{a_0}$.

Ký hiệu $H\times_GH$ là bộ cân bằng trong $H\times H$ của các cấu xạ đồ thị mũi tên $\psi \circ$pr$_1$ và $\varphi \circ$pr$_2$. Tập hợp các đỉnh của nó là tập hợp các cặp $(a, b)$ đỉnh của H sao cho $\psi (a) =\varphi (b)$; tập hợp các mũi tên của nó là tập hợp các cặp $(f, g)$ mũi tên của H sao cho $\psi (f) =\varphi (g)$; gốc của một mũi tên $(f, g)$ là đỉnh $(o(f), o(g))$ và số hạng của nó là đỉnh $(t(f), t(g))$ (xem II, p. 153).

Cuối cùng, ký hiệu Ker($\varphi , \psi$ ) là bộ cân bằng của $\varphi$ và $\psi$; nhắc lại (II, p. 165, ví dụ 2) rằng đó là đồ thị con của H mà các đỉnh $a$ là những đỉnh thỏa $\varphi (a) =\psi (a)$ và các mũi tên là các $f\in$ Fl(H) sao cho $\varphi (f) =\psi (f)$.

#### Mệnh đề 4 {#ta-ii-s5-prop-4 .statement tag=01US}

Cho $\mu: H\times_GH\rightarrow H$ là một cấu xạ đồ thị mũi tên sao cho $\varphi \circ \mu=\varphi \circ$ pr$_1$ và $\psi \circ \mu=\psi \circ$ pr$_2$. Giả sử rằng, với mọi cặp $(a, b)$ đỉnh của H sao cho $\varphi (a) =\varphi (b)$, tồn tại một đỉnh $c$ của H sao cho $\varphi (c) =\psi (b)$ và $a=\mu(b, c)$.

Cho $A_1$ là một tập hợp các đỉnh của Ker($\varphi , \psi$ ) cắt mỗi thành phần liên thông của nó và cho $Z_1$ là tập hợp các phần tử của $\Omega (\widetilde{\Gamma})$ có dạng $((a,1))$, trong đó $a\in A_1$. Cũng vậy, cho $A_2$ là một tập hợp các đỉnh của $H\times_GH$ cắt mỗi thành phần liên thông của $H\times_GH$ và cho $Z_2$ là tập hợp các bộ ba có dạng $((a,1),(b,1),(\mu(a, b),-1))$, khi $(a, b)$ chạy qua $A_2$.

Khi đó $\Omega (\widetilde{\Gamma})$ là tập con phân biệt nhỏ nhất của $\Omega (\widetilde{\Gamma})$ chứa $Z_1\cup Z_2$. Đặc biệt, các lớp liên hợp $c(\mathbf{z})$ trong Coh($\varphi , \psi$ )$_{a_0}$, trong đó $\mathbf{z}$ chạy qua $Z_1\cup Z_2$, sinh hạt nhân của đồng cấu chính tắc $\beta_a$ từ Coh($\varphi , \psi$ )$_{a_0}$ vào Coeg($\varphi , \psi$ )$_{\beta(a_0)}$.

Ký hiệu $Z'_1,Z'_2$ và $Z'$ lần lượt là các tập con phân biệt nhỏ nhất của $\Omega (\widetilde{\Gamma})$ chứa $Z_1,Z_2$ và $Z_1\cup Z_2($II, p. 197, định nghĩa 1). Cần chứng minh rằng $Z'$ bằng $\Omega (\widetilde{\Gamma})$; theo II, p. 199, Hệ quả 1 của Mệnh đề 1 ở II, p. 197, khẳng định cuối cùng của mệnh đề sẽ suy ra.

#### Bổ đề 1 {#ta-ii-s5-lem-1 .statement tag=01UT}

a) Với mọi đỉnh $a$ của Ker($\varphi , \psi$ ), $((a,1))$ thuộc $Z'_1$.

b) Với mọi đỉnh $(a, b)$ của $H\times_GH$, $((a,1),(b,1),(\mu(a, b),-1))$ thuộc $Z'_2$.

a) Gọi $A'_1$ là tập hợp các đỉnh $a$ của Ker($\varphi , \psi$ ) sao cho $((a,1))$ thuộc $Z'_1$. Theo định nghĩa của $Z'_1$, ta có $A_1\subset A'_1$. Gọi $f$ là một mũi tên của Ker($\varphi , \psi$ ), gọi $a$ là gốc của nó và $b$ là đích của nó. Từ tính chất (iv) trong định nghĩa của một tập con phân biệt (II, p. 197, định nghĩa 1) áp dụng cho dãy $((f,1))$ suy ra rằng $a\in A'_1$ tương đương với $b\in A'_1$. Vì $A_1$ cắt mọi thành phần liên thông của Ker($\varphi , \psi$ ), ta có $A'_1=$ Som(Ker($\varphi , \psi$ )), điều phải chứng minh.

b) Gọi $A'_2$ là tập hợp các đỉnh $(a, b)$ của $H\times_GH$ sao cho bộ ba $((a,1),(b,1),(\mu(a, b),-1))$ thuộc $Z'_2$. Theo giả thiết, ta có $A_2\subset A'_2$. Vì $A_2$ cắt mỗi thành phần liên thông của $H\times_GH$, chỉ cần thiết lập rằng, nếu tồn tại một mũi tên $(f, f')$ nối một đỉnh $(a', b')$ với một đỉnh $(a, b)$, thì $(a, b)$ thuộc $A'_2$ khi và chỉ khi tương tự đối với $(a', b')$.

Đặt $f''=\mu(f, f')$; đây là một mũi tên nối $\mu(a', b')$ với $\mu(a, b)$, và ta có $\varphi (f'') =\varphi (f)$ và $\psi (f'') =\psi (f')$. Theo điều kiện (iv) trong định nghĩa của một tập con phân biệt của $\Omega (\widetilde{\Gamma})$ (nơi đã dẫn) áp dụng cho dãy $((f,1),(f',1),(f'',-1))$, hai điều kiện

(i) bộ ba $((a,1),(b,1),(\mu(a, b),-1))$ thuộc $Z'$;

(ii) bộ ba $((a',1),(b',1),(\mu(a', b'),-1))$ thuộc $Z'$;

là tương đương. Điều này cho thấy $(a, b)$ thuộc $A'_2$ khi và chỉ khi $(a', b')$ thuộc $A'_2$ và hoàn tất chứng minh của bổ đề.

Bây giờ ta hãy chứng minh bằng quy nạp theo số nguyên $n\geqslant 1$ rằng mọi phần tử $((a_1, \varepsilon_1),(a_2, \varepsilon_2), . . . ,(a_n, \varepsilon_n))$ của $\Omega (\widetilde{\Gamma})$ đều thuộc $Z'$.

A) Trường hợp trong đó $n= 1$.

Cho $((a, \varepsilon ))$ là một phần tử của $\Omega (\widetilde{\Gamma})$ có độ dài 1. Ta có $\varphi (a) =\psi (a)$, do đó $((a,1))\in Z'$ theo bổ đề 1. Điều kiện (ii) trong định nghĩa của một tập con phân biệt khi đó suy ra rằng $((a,-1))$ thuộc $Z'$.

B) Trường hợp trong đó $n\geqslant 2$.

Do điều kiện (ii) đối với một tập con phân biệt, chỉ cần xét trường hợp $\varepsilon_2= 1$. Giả sử $\varepsilon_1= 1$; khi đó $(a_1, a_2)$ là một đỉnh của $H\times_GH$; đặt $a=\mu(a_1, a_2)$; theo bổ đề 1, bộ ba $((a_1,1),(a_2,1),(a,-1))$ do đó thuộc $Z'$. Trong trường hợp $\varepsilon_1=-1$, ta có $\varphi (a_1) =\varphi (a_2)$; do đó ta có thể chọn một đỉnh $a$ của H sao cho $\mu(a_2, a) =a_1$ và bộ ba $((a_2,1),(a,1),(a_1,-1))$ thuộc $Z'$, nên bộ ba $((a_1,-1),(a_2,1),(a,1))$ cũng vậy, do điều kiện (ii) trong định nghĩa của một tập con phân biệt.

Khi đó $((a, \varepsilon_1),(a_3, \varepsilon_3), . . . ,(a_n, \varepsilon_n))$ thuộc $\Omega (\widetilde{\Gamma})$ và có độ dài $n-1$. Theo giả thiết quy nạp, nó là một phần tử của $Z'$. Do các điều kiện (i), (ii) và (iii) trong định nghĩa của một tập con phân biệt, ta suy ra liên tiếp rằng các phần tử

$$
((a_1, \varepsilon_1),(a_2,1),(a,-\varepsilon_1),(a, \varepsilon_1),(a_3, \varepsilon_3), . . . ,(a_n, \varepsilon_n))
$$

$$
((a,-\varepsilon_1),(a, \varepsilon_1),(a_3, \varepsilon_3), . . . ,(a_n, \varepsilon_n),(a_1, \varepsilon_1),(a_2,1))
$$

$$
((a_3, \varepsilon_3), . . . ,(a_n, \varepsilon_n),(a_1, \varepsilon_1),(a_2,1))
$$

$$
((a_1, \varepsilon_1),(a_2,1),(a_3, \varepsilon_3), . . . ,(a_n, \varepsilon_n))
$$

đều thuộc $Z'$. Điều này hoàn tất chứng minh của mệnh đề.

#### Hệ quả {#ta-ii-s5-n3-cor-1 .statement tag=01UU}

a) Với ký hiệu của mệnh đề 4, giả sử thêm rằng ánh xạ (Som($\varphi$ ), Som($\psi$ )) từ Som(H) vào Som(G) $\times$ Som(G) là đơn ánh và ảnh của nó là đồ thị của một quan hệ tương đương trong Som(G). Khi đó, với mọi đỉnh $(a, b)$ của $H\times_GH$, tồn tại một đỉnh duy nhất $c_{a,b}$ của H sao cho $\varphi (c_{a,b}) =\varphi (a)$ và $\psi (c_{a,b}) =\psi (b)$.

b) Giả sử thêm nữa rằng với mọi mũi tên $(f, f')$ của $H\times_GH$, tồn tại một mũi tên $f''$ của H sao cho $\varphi (f'') =\varphi (f)$ và $\psi (f'') =\psi (f')$.

Cho A là một tập hợp các đỉnh của $H\times_GH$ gặp mỗi thành phần liên thông của nó. Khi đó, hạt nhân của cấu xạ $\beta_{a_0}$ là nhóm con phân biệt nhỏ nhất của Coh($\varphi , \psi$ )$_{a_0}$ chứa các lớp liên hợp $c((a,1),(b,1),(c_{a,b},-1))$, với $(a, b)\in A$.

Cho R là quan hệ tương đương trong Som(G) mà đồ thị của nó là ảnh của ánh xạ (Som($\varphi$ ), Som($\psi$ )). Cho $(a, b)$ là một đỉnh của $H\times_GH$. Khi đó ta có $R\{\varphi (a), \psi (a)\}$ và $R\{\varphi (b), \psi (b)\}$, do đó $R\{\varphi (a), \psi (b)\}$ vì $\psi (a) =\varphi (b)$. Do đó, tồn tại một đỉnh duy nhất $c$ của H sao cho $\varphi (c) =\varphi (a)$ và $\psi (c) =\psi (b)$; ta ký hiệu nó là $\mu(a, b)$.

Với mọi mũi tên $(f, f')$ của $H\times_GH$, chọn một mũi tên $f''$ của H sao cho $\varphi (f'') =\varphi (f)$ và $\psi (f'') =\psi (f)$ và ký hiệu nó là $\mu(f, f')$.

Như vậy đã xác định được một cấu xạ quiver $\mu: H\times_GH\rightarrow H$ sao cho $\varphi \circ \mu=\varphi \circ$ pr$_1$ và $\psi \circ \mu=\psi \circ$ pr$_2$.

Cho $(a, b)$ là một cặp đỉnh của H sao cho $\varphi (a) =\varphi (b)$. Ta có $R\{\varphi (a), \psi (a)\}$ và $R\{\varphi (b), \psi (b)\}$, do đó $R\{\psi (b), \psi (a)\}$. Do đó tồn tại một đỉnh duy nhất $c$ của H sao cho $\varphi (c) =\psi (b)$ và $\psi (c) =\psi (a)$. Đỉnh $\mu(b, c)$ thỏa $\varphi (\mu(b, c)) =\varphi (b) =\varphi (a)$ và $\psi (\mu(b, c)) =$ $\psi (c) =\psi (a)$. Vậy $\mu(b, c) =a$ vì ánh xạ (Som($\varphi$ ), Som($\psi$ )) từ Som(H) vào Som(G) $\times$ Som(G) là đơn ánh.

Cho $A_1$ là tập hợp các đỉnh của Ker($\varphi , \psi$ ) và cho $Z_1$ là tập hợp các phần tử của $\Omega (\widetilde{\Gamma})$ có dạng $((a,1))$, với $a\in A_1$. Đặt $A_2= A$ và cho $Z_2$ là tập hợp các phần tử $((a,1),(b,1),(\mu(a, b),-1))$ của $\Omega (\widetilde{\Gamma})$, với $(a, b)\in A_2$. Gọi $\widetilde{Z}$ (tương ứng $\widetilde{Z}_1$, tương ứng $\widetilde{Z}_2$) là tập con phân biệt nhỏ nhất của $\Omega (\widetilde{\Gamma})$ chứa $Z_1\cup Z_2$ (tương ứng $Z_1$, tương ứng $Z_2$).

Cho $a\in A_1$; ta có $\varphi (a) =\psi (a)$ ; đặt $x=\varphi (a)$. Đỉnh $a$ là đỉnh duy nhất của H sao cho $\varphi (a) =\psi (a) =x$; đặc biệt, ta có $\mu(a, a) =a$. Do đó bộ ba $((a,1),(a,1),(a,-1))$ thuộc $Z_2$. Khi ấy từ các điều kiện (i) và (iii) trong định nghĩa của một tập con phân biệt suy ra rằng $((a,1))$ thuộc $\widetilde{Z}_2$. Do đó, ta có $Z_1\subset \widetilde{Z}_2$, do đó $\widetilde{Z} =\widetilde{Z}_2$.

Theo Mệnh đề 4, $\Omega (\widetilde{\Gamma})$ là tập con phân biệt nhỏ nhất của $\Omega (\widetilde{\Gamma})$ chứa $Z_2$ và hạt nhân của $\beta_{a_0}$ là nhóm con phân biệt nhỏ nhất của Coh($\varphi , \psi$ )$_{a_0}$ chứa các lớp liên hợp $c(\mathbf{z})$, với $\mathbf{z}\in Z_2$, do đó có hệ quả.

#### Ví dụ {#ta-ii-s5-n3-exa-1 .statement tag=01UV}

Cho X và R là các không gian tôpô, cho $o$ và $t$ là các ánh xạ liên tục từ R vào X, cho C là tập hợp các cặp $(f, g)\in R^2$ sao cho $t(f) =o(g)$ trong R, và cho $m$ là một ánh xạ liên tục từ C vào R biến mũi tên đồ $(X,R, o, t)$ thành một groupoid; giả sử thêm rằng ánh xạ $f\mapsto f^{-1}$ từ R vào R là liên tục. Khi đó các giả thiết của mệnh đề được thỏa mãn nếu đặt $H =\varpi (R)$, $G =\varpi (X),\varphi =\varpi (o),\psi =\varpi (t)$ và $\mu=\varpi (m)$.

Giả sử thêm rằng R là đồ thị của một quan hệ tương đương trong X, các ánh xạ $o$ và $t$ được suy ra từ các phép chiếu của $X\times X$ lên X bằng cách chuyển qua các không gian con. Khi đó các giả thiết của hệ quả được thỏa mãn.

#### Nhận xét {#ta-ii-s5-n3-rem-1 .statement tag=01UW}

*Nói chung hơn, các giả thiết của mệnh đề được thỏa mãn khi $(G,H, \varphi , \psi , \mu)$ là một "groupoid của các groupoid". Điều này có nghĩa là G và H là các groupoid, $\varphi$ và $\psi$ là các cấu xạ groupoid từ H vào G, biến bộ bốn $(G,H, \varphi , \psi )$ thành một "mũi tên đồ trong các groupoid"; sau cùng, $\mu$ là một luật hợp thành trong "mũi tên đồ" này được cho bởi một cấu xạ groupoid $H\times_GH\rightarrow H$, thỏa mãn một số tính chất biểu thị tính kết hợp của luật và sự kiện là mọi "mũi tên" đều khả nghịch. Bạn đọc cũng sẽ nhận xét rằng các ánh xạ tới groupoid cơ bản được nghiên cứu trong công trình này đều thuộc trường hợp này.*

### 4. Nhóm đẳng hướng của một đối đồng hóa tử

Cho G và H là các groupoid; cho $\varphi$ và $\psi$ là các cấu xạ groupoid từ H vào G. Mục đích của số này là tóm tắt phép tính các nhóm đẳng hướng của cohomotopizer (II, p. 193, mệnh đề 6) và sự so sánh các nhóm đẳng hướng của cohomotopizer và của đối đồng hóa tử đã được thực hiện trong số trước, để từ đó suy ra phép tính các nhóm đẳng hướng của đối đồng hóa tử Coeg($\varphi , \psi$ ).

Ký hiệu bởi $\alpha : G\rightarrow$ Coh($\varphi , \psi$ )$,\beta :$ Coh($\varphi , \psi$ )$\rightarrow$ Coeg($\varphi , \psi$ ) và $\gamma =\beta \circ$ $\alpha : G\rightarrow$ Coeg($\varphi , \psi$ ) các cấu xạ groupoid chính tắc. Ký hiệu bởi $h:$ Som(H) $\rightarrow$ Fl(Coh($\varphi , \psi$ )) phép đồng luân chính tắc; xin nhắc lại rằng tập hợp các đỉnh của Coh($\varphi , \psi$ ) bằng Som(G).

Ký hiệu $\Gamma$ là đồ thị có hướng (Som(G), Som(H), Som($\varphi$ ), Som($\psi$ )); khi đó ký hiệu $\varphi_0$ và $\psi_0$ là các ánh xạ suy ra từ $\varphi$ và $\psi$ bằng cách chuyển qua các quỹ đạo và $\Gamma_0$ là khung (Orb(G), Orb(H)$, \varphi_0, \psi_0$) của cặp $(\varphi , \psi )$. Ta sẽ giả sử rằng đồ thị có hướng $\Gamma_0$ là liên thông và tập hợp các đỉnh của nó không rỗng, điều này tương đương với việc giả sử rằng các nhóm vị Coh($\varphi , \psi$ ) và Coeg($\varphi , \psi$ ) là bắc cầu.

Nhắc lại (x. II, p. 192, định nghĩa 4) rằng một trang bị cơ bản bao gồm dữ liệu của một họ $(a, b, c_1, c_2,T, i_0)$ trong đó: với mọi $i\in$ Orb(G)$,a(i)$ là một đỉnh trong quỹ đạo $i$ của G; với mọi $j\in$ Orb(H)$,b(j)$ là một đỉnh trong quỹ đạo $j$ của H$,c_1(j)$ và $c_2(j)$ là các mũi tên của G nối tương ứng $\varphi (b(j))$ với $a(\varphi_0(j))$ và $\psi (b(j))$ với $a(\psi_0(j))$; T là một đồ thị con có hướng của $\Gamma_0$ mà cây liên kết với nó là một cây cực đại của đồ thị $\widetilde{\Gamma}_0$; sau cùng, $i_0$ là một quỹ đạo của G và ta đặt $a_0=a(i_0)$.

Khi đó ta định nghĩa một cấu xạ của các đồ thị có hướng $\tau_0$ từ $\Gamma_0$ vào Coh($\varphi , \psi$ ) sao cho $\tau_0(i) =\beta (a(i))$ và $\tau_0(j) =\alpha (c_1(j))^{-1}h(b(j))\alpha (c_2(j))$ với $i\in$ Orb(G) và $j\in$ Orb(H). Nếu $i$ thuộc Orb(G), ký hiệu $d_i$ là lớp đường đi duy nhất trong đồ thị $\widetilde{T}$ nối $i_0$ với $i$, và ký hiệu $\delta_i$ là ảnh của nó trong Coh($\varphi , \psi$ ) dưới cấu xạ nhóm vị $\tau_0$.

Từ các dữ liệu này, Mệnh đề 6 (II, p. 193) cho một đồng cấu toàn ánh

$\Lambda :(_{i\in\pi}*_{_0(G)}G_{a(i)})*$ F(Orb(H)) $\rightarrow$ Coh($\varphi , \psi$ )$_{a(i_0)}$

và mô tả các phần sinh của hạt nhân của nó, do đó cung cấp một biểu diễn của nhóm Coh($\varphi , \psi$ )$_{a_0}$.

Tập hợp các vòng độ dài $\geqslant 1$ trong đồ thị $\widetilde{\Gamma}$ liên kết với Γ được đồng nhất với tập $\Omega (\widetilde{\Gamma})$ các dãy $(z_1, . . . , z_n)$ các mũi tên của $\widetilde{\Gamma}$, được đánh chỉ số bởi $\mathbf{Z}/n\mathbf{Z}$, trong đó $n$ chạy qua tập hợp các số nguyên $\geqslant 1$, sao cho với mọi $k\in \mathbf{Z}/n\mathbf{Z}$, điểm cuối của $z_k$ là điểm đầu của $z_{k+1}$. Gọi Z là một tập con của $\Omega (\widetilde{\Gamma})$ sao cho các lớp liên hợp $c(z)$, với $z\in Z$, sinh hạt nhân của đồng cấu toàn ánh $\beta_{a_0}$. Đồng cấu $\beta_{a_0}\circ \Lambda$ là toàn ánh; để suy ra hạt nhân của nó, tức là một biểu diễn của nhóm Coeg($\varphi , \psi$ )$_{\beta(a_0)}$, còn phải chọn, với mỗi $z\in Z$, một phần tử $C(z)$ trong nhóm $(*G_{a(i)})*F(\pi_0(H))$

$i\in$Orb(G)

sao cho $\Lambda (C(z))$ thuộc lớp liên hợp $c(z)$.

Vậy cho $z= (z_1, . . . , z_n)$ là một phần tử của $\Omega (\widetilde{\Gamma})$; đặt $z_k= (y_k, \varepsilon_k)$, trong đó $y_k\in$ Fl(Γ) = Som(H) và $\varepsilon_k\in  \{\pm 1\}$. Theo định nghĩa, $c(z)$ là lớp liên hợp của phần tử

$$
gh(y_1)^{\varepsilon_1}. . . h(y_n)^{\varepsilon_n}g^{-1}
$$

của groupoid Coh($\varphi , \psi$ )$_{a_0}$, trong đó $g$ là một mũi tên tùy ý của Coh($\varphi , \psi$ ) nối $a_0$ với điểm đầu của $z_1$. Với $k\in \mathbf{Z}/n\mathbf{Z}$, gọi $j_k$ là quỹ đạo của $y_k$ trong H và chọn một mũi tên $f_k$ của H nối $y_k$ với đỉnh $b(j_k)$. Theo định nghĩa của một đồng luân, khi đó ta có quan hệ

$$
h(y_k)(\alpha \circ \psi )(f_k) = (\alpha \circ \varphi )(f_k)h(b(j_k))
$$

trong groupoid Coh($\varphi , \psi$ ). Do đó, dùng định nghĩa của cấu xạ quiver $\tau_0$, ta có

$$
h(y_k) = (\alpha \circ \varphi )(f_k)\cdot h(b(j_k))\cdot (\alpha \circ \psi )(f_k)^{-1}
$$

$$
= (\alpha \circ \varphi )(f_k)\cdot (\alpha \circ c_1)(j_k)\cdot \tau_0(j_k)\cdot (\alpha \circ c_2)(j_k)^{-1}\cdot (\alpha \circ \psi )(f_k)^{-1}
$$

$$
= (\alpha \circ \varphi )(f_k)\cdot (\alpha \circ c_1)(j_k)\cdot \delta_{\varphi_0(j_k)}^{-1}\cdot
$$

$$
\cdot \delta_{\varphi_0(j_k)}\cdot \tau_0(j_k)\cdot \delta_{\psi_0(j_k)}^{-1}\cdot
$$

$$
\cdot \delta_{\psi_0(j_k)}\cdot (\alpha \circ c_2)(j_k)^{-1}\cdot (\alpha \circ \psi )(f_k)^{-1}
$$

$$
=u_k\Lambda (j_k)v_k
$$

trong đó ta đã đặt

$u_k=\alpha (\varphi (f_k)c_1(j_k))\cdot \delta_{\varphi_0(j_k)}^{-1}$ và $v_k=\delta_{\psi_0(j_k)}\cdot \alpha (\psi (f_k)c_2(j_k))^{-1}$. Với mọi phần tử $k\in \mathbf{Z}/n\mathbf{Z}$, định nghĩa các mũi tên $\widetilde{u}_k,\widetilde{v}_k$ trong G bởi

$$
h(y_k)^{\varepsilon_k}=\widetilde{u}_k\Lambda (j_k)^{\varepsilon_k}\widetilde{v}_k
$$

sao cho

$(u_k, v_k)$ nếu $\varepsilon_k= 1$ ;

$$
(\widetilde{u}_k,\widetilde{v}_k) =_{--}
$$

$(v_k^1, u_k^1)$ nếu $\varepsilon_k=-1$.

Kí hiệu $x_k$ là gốc của mũi tên $h(y_k)^{\varepsilon_k}$; khi đó đích của nó là $x_{k+1}$; gọi $i_k$ là quỹ đạo của $x_k$. Khi đó ta định nghĩa một vòng $\lambda_k(z)$ tại $a(i_k)$ trong vị nhóm G bởi công thức

(1)

$c_2(j_{k-1})^{-1}\psi (f_{k-1})^{-1}\varphi (f_k)c_1(j_k)$ nếu $(\varepsilon_{k-1}, \varepsilon_k) = (1,1)$;

$c_2(j_{k-1})^{-1}\psi (f_{k-1})^{-1}\psi (f_k)c_2(j_k)$ nếu $(\varepsilon_{k-1}, \varepsilon_k) = (1,-1)$; $\lambda_k(z) =$

$c_1(j_{k-1})^{-1}\varphi (f_{k-1})^{-1}\varphi (f_k)c_1(j_k)$ nếu $(\varepsilon_{k-1}, \varepsilon_k) = (-1,1)$;

$c_1(j_{k-1})^{-1}\varphi (f_{k-1})^{-1}\psi (f_k)c_2(j_k)$ nếu $(\varepsilon_{k-1}, \varepsilon_k) = (-1,-1)$. Theo phép dựng, ta có

$$
\Lambda (\lambda_k(z)) =\widetilde{v}_{k-1}\widetilde{u}_k
$$

nên ảnh qua đồng cấu Λ của phần tử

$$
C(z) =\lambda_1(z)(j_1)^{\varepsilon_1}\lambda_2(z)(j_2)^{\varepsilon_2}. . . \lambda_n(z)(j_n)^{\varepsilon_n} \tag{2}
$$

thuộc lớp liên hợp $c(z)$.

#### Định nghĩa 3 {#ta-ii-s5-def-3 .statement tag=01UX}

Cho G và H là các vị nhóm; cho $\varphi$ và $\psi$ là các cấu xạ vị nhóm từ H vào G. Giả sử vị nhóm Coeg($\varphi , \psi$ ) là bắc cầu. Cho $(a, b, c_1, c_2,T, i_0)$ là một trang bị cơ bản của cặp $(\varphi , \psi )$.

Một trang bị bổ sung là dữ liệu của một tập con Z của $\Omega (\widetilde{\Gamma})$ sao cho các lớp liên hợp $c(\mathbf{z})$ với $\mathbf{z}\in$ Z sinh hạt nhân của đồng cấu $\beta_{a(i_0)}$ và, với mỗi phần tử $\mathbf{z}= ((y_1, \varepsilon_1), . . . ,(y_n, \varepsilon_n))$ của Z, của một dãy $f(\mathbf{z}) = (f_1, . . . , f_n)$ các mũi tên trong H sao cho $f_k$ nối $y_k$ với đỉnh $b(j_k)$, trong đó $j_k$ là quỹ đạo của $y_k$ trong H.

Một trang bị đầy đủ của cặp $(\varphi , \psi )$ là dữ liệu của một trang bị cơ bản và của một trang bị bổ sung.

#### Mệnh đề 5 {#ta-ii-s5-prop-5 .statement tag=01UY}

Cho G và H là các vị nhóm; cho $\varphi$ và $\psi$ là các cấu xạ vị nhóm từ H vào G. Giả sử vị nhóm Coeg($\varphi , \psi$ ) là bắc cầu. Gọi $\gamma : G\rightarrow$ Coeg($\varphi , \psi$ ) là cấu xạ chính tắc của các vị nhóm.

Ta trang bị cho cặp $(\varphi , \psi )$ một trang bị đầy đủ

$$
(a, b, c_1, c_2,T, i_0,Z,(f(\mathbf{z}))_{\mathbf{z}\in Z})
$$

Với $j\in$ Orb(H), gọi $\varphi_j: H_{b(j)}\rightarrow G_{a(\varphi_0(j))}$ và $\psi_j: H_{b(j)}\rightarrow G_{a(\psi_0(j))}$ lần lượt là các đồng cấu nhóm Int($c_1(j)$)$^{-1}\circ \varphi_{b(j)}$ và Int($c_2(j)$)$^{-1}\circ \psi_{b(j)}$, trong đó $\varphi_0$ và $\psi_0$ ký hiệu các ánh xạ chính tắc suy ra từ $\varphi$ và $\psi$ bằng cách chuyển qua các quỹ đạo. Gọi $\tau$ là cấu xạ của khung $\Gamma_0$ của cặp $(\varphi , \psi )$ vào Coeg($\varphi , \psi$ ) được xác định bởi Som($\tau$ )$(i) =\gamma (a(i))$ nếu $i\in$ Orb(G) và sao cho Fl($\tau$ )$(j)$ là đường $\gamma (c_1(j))^{-1}\gamma (c_2(j))$ trong Coeg($\varphi , \psi$ ). Nếu $i$ là một quỹ đạo của G, gọi $c_i$ là lớp duy nhất các đường trong $\widetilde{T}$ nối $i_0$ với $i$ và đặt $\delta_i=\widetilde{\tau}(c_i)$, trong đó $\widetilde{\tau}:$ Grp(G) $\rightarrow$ Coeg($\varphi , \psi$ ) là cấu xạ groupoid chính tắc suy ra từ $\tau$.

Khi đó tồn tại một đồng cấu nhóm duy nhất

$\lambda :(*G_{a(i)})*$ F(Orb(H)) $\rightarrow$ Coeg($\varphi , \psi$ )$_{\gamma(a(i_0))}$

$i\in$Orb(G)

sao cho

$\lambda (f) =\delta_i\gamma_{a(i)}(f)\delta_i^{-1}$ cho $i\in$ Orb(G) và $f\in G_{a(i)}$,

$\lambda (j) =\delta_{\varphi_0(j)}\tau (j)\delta_{\psi_0(j)}^{-1}$ for $j\in$ Orb(H).

Đồng cấu $\lambda$ là toàn ánh; hạt nhân của nó là nhóm con chuẩn tắc nhỏ nhất chứa các phần tử sau:

($R_1$)$r_1(j) =j$ for $j$ in Fl(T) ;

($R_2$)$r_2(j, f) =\varphi_j(f)j\psi_j(f)^{-1}j^{-1}$

cho $j\in$ Orb(H) và $f\in H_{b(j)}$;

($R_3$)$r_3(z) =\lambda_1(z)j_1^{\varepsilon_1}\lambda_2(z)j_2^{\varepsilon_2}. . . \lambda_n(z)j_n^{\varepsilon_n}$

for $z= ((y_1, \varepsilon_1), . . . ,(y_n, \varepsilon_n))\in Z$,

trong đó các vòng $\lambda_i(z)$ được xác định bởi công thức (1), p. 208.

Sự tồn tại và tính duy nhất của một cấu xạ như vậy suy ra từ tính chất phổ quát của tích tự do của một họ nhóm (A, I, p. 85, mệnh đề 8). Ta ký hiệu bởi $\alpha : G\rightarrow$ Coh($\varphi , \psi$ ) và $\beta :$ Coh($\varphi , \psi$ )$\rightarrow$ Coeg($\varphi , \psi$ ) các cấu xạ chính tắc, sao cho $\gamma$ = $\beta \circ \alpha$. Lấy thêm $h:$ Som(H) $\rightarrow$ Fl(Coh($\varphi , \psi$ )) là phép đồng luân chính tắc nối $\alpha \circ \varphi$ với $\alpha \circ \psi$. Vì $\beta$ là cấu xạ groupoid thu được bằng cách co các mũi tên nằm trong ảnh của $h$, ta có

Fl($\tau$ )$(j) =\gamma (c_1(j))^{-1}\gamma (c_2(j)) =\gamma (c_1(j)^{-1})\beta (h(j))\gamma (c_2(j)) =\beta (\tau_0(j))$ trong Coeg($\varphi , \psi$ ), trong đó $\tau_0: \Gamma_0\rightarrow$ Coh($\varphi , \psi$ ) ký hiệu cấu xạ quiver suy ra từ trang bị cơ sở $(a, b, c_1, c_2,T, i_0)$. Do đó, đồng cấu $\lambda$ là hợp thành của đồng cấu Λ được định nghĩa trong mệnh đề 6 (II, p. 193) và đồng cấu toàn ánh $\beta_{a(i_0)}$. Đặc biệt, nó là toàn ánh.

Cho $z\in Z$; theo phép dựng, $\Lambda (r_3(z))$ thuộc lớp liên hợp $c(z)$. Theo định nghĩa của một trang bị bù, hạt nhân của đồng cấu $\beta_{a(i_0)}$ vì thế là nhóm con bất biến nhỏ nhất của Coh($\varphi , \psi$ )$_{a(i_0)}$ chứa các phần tử $\Lambda (r_3(z))$ với $z\in Z$. Vì đồng cấu Λ là toàn ánh, hạt nhân của đồng cấu $\lambda =\beta_{a(i_0)}\circ \Lambda$ vì thế là nhóm con bất biến nhỏ nhất của nhóm $(*G_{a(i)})*F(\pi_0(H))$ chứa các phần tử sinh của hạt nhân

$i\in$Orb(G)

của Λ cho bởi các công thức ($R_1$)$, (R_2)$, cùng với các phần tử được xác định bởi các công thức ($R_3$). Mệnh đề do đó được chứng minh.

### 5. Thương của một groupoid theo tác động của một nhóm

Cho G là một groupoid bắc cầu, K là một nhóm, và $\theta : K\rightarrow$ Aut(G)$^{\circ}$ là một đồng cấu nhóm từ K vào nhóm đối của nhóm tự đẳng cấu của groupoid G. Ta sẽ nói rằng nhóm K tác động phải trên G. Nếu $k\in K$, đôi khi ta sẽ ký hiệu bởi $k^*x$ (resp. $k^*f$) ảnh của một đỉnh $x$ (resp. của một mũi tên $f$) của G dưới tự đẳng cấu groupoid $\theta (k)$.

Cho $|K|$ là groupoid mà tập hợp các đỉnh là K và tập hợp các mũi tên nối hai đỉnh là rỗng nếu các đỉnh này phân biệt, và ngược lại thì chỉ gồm một phần tử. Cho H là groupoid tích $G\times  |K|$; một đỉnh của H là một cặp $(a, k)$, trong đó $a$ là một đỉnh của G và $k$ là một phần tử của K; nếu $f$ là một mũi tên của G nối một đỉnh $a$ với một đỉnh $b$, ta sẽ ký hiệu bởi $(f, k)$ mũi tên duy nhất của H nối $(a, k)$ với $(b, k)$. Cho $\varphi : H\rightarrow G$ là cấu xạ groupoid xác định bởi phép chiếu thứ nhất và cho $\psi : H\rightarrow G$ là cấu xạ groupoid sao cho Som($\psi$ )$((a, k)) =k^*a$ và Fl($\psi$ )$((f, k)) =k^*f$ nếu $k\in K,a\in$ Som(G) và $f\in$ Fl(G).

Ký hiệu bởi $G/K$ đối cân bằng tử Coeg($\varphi , \psi$ ) và ký hiệu bởi $\gamma : G\rightarrow G/K$ cấu xạ groupoid chính tắc.

Cho $o$ là một đỉnh của G. Với $k\in K$, chọn một mũi tên $c_k$ nối $k^*o$ với $o$ trong G; tồn tại một mũi tên như vậy vì G là bắc cầu. Với $k\in K$, ký hiệu bởi Fix($k$) groupoid con của G mà các đỉnh (tương ứng, các mũi tên) là các phần tử của Som(G) (tương ứng, của Fl(G)) được cố định bởi $k$; chọn một tập hợp $A_k$ các đỉnh của Fix($k$) cắt mọi quỹ đạo của groupoid này. Với $k\in K$ và $a\in A_k$, cũng chọn một mũi tên $f_{(a,k)}$ trong G nối đỉnh $a$ với đỉnh $o$.

#### Mệnh đề 6 {#ta-ii-s5-prop-6 .statement tag=01UZ}

Đồng cấu nhóm duy nhất

$$
\lambda : G_o*F(K)\rightarrow (G/K)_{\gamma(o)}
$$

sao cho $\lambda (f) =\gamma_o(f)$ với $f\in G_o$ và $\lambda ([k]) =\gamma (c_k)$ với $k\in K$ là toàn ánh. Hạt nhân của nó là nhóm con chuẩn nhỏ nhất của $G_o*F(K)$ chứa các phần tử sau:

($R_2$)$r_2(k, f) = [k]^{-1}f[k](c^{-1}_kk^*(f)^{-1}c_k)$

với $k\in K$ và $f\in G_o$;

($R'_3$)$r'_3(k, a) = [k](c^{-1}_kk^*(f_{(a,k)})^{-1}f_{(a,k)}))$

với $k\in K-\{e\}$ và $a\in A_k$

($R''_3$)$r''_3(k, h) = [kh]^{-1}[k][h](c^{-1}_hh^*(c^{-1}_k)c_{kh})$

với $k$ và $h\in K$.

Vì G là bắc cầu, ánh xạ liên kết với một phần tử $k\in K$ quỹ đạo của $(o, k)$ là một song ánh từ K lên tập hợp các quỹ đạo của H. Do đó Orb(G) được đồng nhất với $\{o\}$ và Orb(H) với K. Khi đó khung $\Gamma_0$ của cặp $(\varphi , \psi )$ được đồng nhất với quiver có một đỉnh duy nhất $o$ và có tập hợp các mũi tên là K. Gọi T là quiver con của $\Gamma_0$ có tập hợp các đỉnh là $\{o\}$ và có tập hợp các mũi tên là rỗng; đồ thị liên kết là cây cực đại duy nhất của đồ thị $\widetilde{\Gamma}_0$.

Họ $(o,(o, k)_{k\in K},(e_o)_{k\in K},(c_k)_{k\in K},T, o)$ là một trang bị cơ bản của cặp $(\varphi , \psi )$.

Ánh xạ $f\mapsto (f, k)$ xác định một đẳng cấu từ nhóm đẳng hướng $G_o$ lên nhóm đẳng hướng $H_{(o,k)}$; nhờ đẳng cấu này, các đồng cấu $\varphi_k$ và $\psi_k$ từ $H_{(o,k)}$ vào $G_o$ được xác định bởi Mệnh đề 5 của II, p. 208 được cho bởi

(3) $\varphi_k(f, k) =f$ và $\psi_k(f, k) =c^{-1}_kk^*(f)c_k$,

với $k\in K$ và $f\in G_o$.

Quiver $H\times_GH$ là bộ cân bằng trong $H\times H$ của các cấu xạ quiver $\psi \circ$ pr$_1$ và $\varphi \circ$ pr$_2$. Các đỉnh của nó là các cặp $((a, k),(b, h))$ trong đó $a$ và $b$ là các đỉnh của G và $k$ và $h$ là các phần tử của K sao cho $b=k^*a$, và các mũi tên của nó là các cặp $((f, k),(g, h))$ trong đó $f$ và $g$ là các mũi tên của G, và $k$ và $h$ là các phần tử của K sao cho $g=k^*f$; gốc của mũi tên $((f, k),(g, h))$ bằng $((o(f), k),(o(g), h))$; ngọn của nó bằng $((t(f), k),(t(g), h))$.

Khi đó ta xác định một cấu xạ quiver $\mu$ từ $H\times_GH$ vào H bằng cách đặt $\mu((a, k),(b, h)) = (a, kh)$ và $\mu((f, k),(g, h)) = (f, kh)$. Ta có $\varphi \circ \mu=\varphi \circ$ pr$_1$ và $\psi \circ \mu=\psi \circ$ pr$_2$.

Cho $x$ và $y$ là các đỉnh của H sao cho $\varphi (x) =\varphi (y)$. Khi đó tồn tại một đỉnh $a$ của G và các phần tử $k$ và $h$ của K sao cho $x= (a, k)$ và $y= (a, h)$. Đặt $z= (h^*a, h^{-1}k)$; khi đó $\mu(y, z) =x$. Điều này cho thấy cặp $(\varphi , \psi )$ thỏa mãn các giả thiết của Mệnh đề 4 (II, p. 202).

Một đỉnh $(a, k)$ của H thuộc groupoid Ker($\varphi , \psi$ ), bộ cân bằng của $\varphi$ và $\psi$, khi và chỉ khi $k^*a=a$, nghĩa là, khi $k$ thuộc nhóm ổn định của đỉnh $a$ trong nhóm K. Gọi $A_1$ là tập hợp các cặp $(a, k)$, với $k\in K$ và $a\in A_k$; nó cắt tất cả các quỹ đạo của subgroupoid Ker($\varphi , \psi$ ) của H. Gọi $Z_1$ là tập con của $\Omega (\widetilde{\Gamma})$ gồm các dãy có dạng $(((a, k),1))$, với $(a, k)\in A_1$. Với $\mathbf{z}= ((a, k),1)\in Z_1,(f_{(a,k)}, k)$ là một mũi tên của H nối $(a, k)$ với $(o, k)$. Đặt $f(\mathbf{z}) = ((f_{(a,k)}, k))$.

Tập hợp $A_2$ các đỉnh của $H\times_GH$ có dạng $((o, k),(k^*o, h))$, với $(k, h)\in K^2$, cắt tất cả các quỹ đạo của $H\times_GH$. Cũng nhận thấy rằng ta có $\mu((o, k),(k^*o, h)) = (o, kh)$. Các mũi tên $(e_o, k)$, $(c_k, h)$, $(e_o, kh)$ trong H lần lượt nối $(o, k)$, $(k^*o, h)$, $(o, kh)$ với $(o, k)$, $(o, h)$ và $(o, kh)$. Gọi $Z_2$ là tập hợp các dãy có dạng $(((o, k),1),((k^*o, h),1),((o, kh),-1))$ trong $\Omega (\widetilde{\Gamma})$; với một phần tử như thế $\mathbf{z}$ của $Z_2$, đặt $f(\mathbf{z}) = ((e_o, k),(c_k, h),(e_o, kh))$.

Theo Mệnh đề 4 của II, p. 202, tập hợp $Z = Z_1\cup Z_2$ và họ $(f(\mathbf{z}))_{z\in Z}$ là một trang bị bù.

Cho $k\in K$ và cho $a\in A_k$. Phần tử $C((a, k),1)$ của nhóm $G_o*F(K)$ được xác định bởi công thức (2) của II, p. 208 bằng

$$
c^{-1}_k\psi ((f_{(a,k)}, k))^{-1}\varphi (f_{(a,k)})e_o[k] =(c^{-1}_kk^*(f_{(a,k)})^{-1}f_{(a,k)})[k] \tag{4}
$$

Cho $k$ và $h\in K$ đã cho. Ta kiểm tra được rằng phần tử

$$
C(((o, k),1),((k^*o, h),1),((o, kh),-1))
$$

của nhóm $G_o*F(K)$ được định nghĩa bởi công thức (2) của II, p. 208 bằng

$$
[k][h](c^{-1}_hh^*(c^{-1}_k)c_{kh})[kh]^{-1} \tag{5}
$$

Các phần tử $r'_3(e, a)$ được cho bởi các quan hệ ($R'_3$) đối với $k=e$ đều bằng $[e]c^{-1}_e$, một phần tử của nhóm $G_o*F(K)$ mà ta thu được bằng cách áp dụng quan hệ ($R''_3$) cho $k=h=e$. Do đó, có kể đến các quan hệ (3), (4), và (5), mệnh đề suy ra từ II, p. 208, Prop. 5.

#### Hệ quả 1 {#ta-ii-s5-prop-6-cor-1 .statement tag=01V0}

Giả sử rằng nhóm K được sinh bởi các bộ ổn định của các đỉnh của G. Khi đó đồng cấu nhóm $\gamma_o: G_o\rightarrow (G/K)_{\gamma(o)}$ là toàn ánh. Hơn nữa, nếu groupoid G là đơn bắc cầu, thì điều tương tự cũng đúng đối với groupoid $G/K$.

Quan hệ ($R''_3$) kéo theo $\lambda ([e]) =\lambda (c_e) =\gamma_o(c_e)$. Khi đó các quan hệ ($R''_3$) kéo theo rằng tập hợp các $k\in K$ sao cho $\lambda ([k])$ thuộc ảnh của $\gamma_o$ là một nhóm con của K. Cuối cùng, các quan hệ ($R'_3$) cho thấy rằng, với mọi phần tử $k\in K$ mà bộ ổn định của nó không rỗng, $\lambda ([k])$ thuộc ảnh của $\gamma_o$. Hệ quả được suy ra.

#### Nhận xét 1 {#ta-ii-s5-n5-rem-1 .statement tag=01V1}

Người ta có thể đưa ra một mô tả khác, đôi khi tiện lợi hơn, của nhóm $(G/K)_{\gamma(o)}$. Để làm điều này, đặt $M = K\times G_o$ và định nghĩa một luật hợp thành trên M bằng công thức

$$
(k, a)\cdot (h, b) = (kh, c^{-1}_{kh}h^*(c_ka)c_hb)
$$

với $k,h\in K$ và $a,b\in G_o$. Ta kiểm tra được rằng luật hợp thành này là kết hợp, rằng $(e, c^{-1}_e)$ là một phần tử đơn vị, và rằng phần tử $(k^{-1}, c^{-1_1}_{k^-}(k^{-1})^*(c_ka)^{-1}c_e)$ là nghịch đảo của $(k, a)$. Do đó nó trang bị cho M một cấu trúc nhóm. Hơn nữa, ánh xạ $\lambda ': M\rightarrow (G/K)_{\gamma(o)}$ được định nghĩa bởi $(k, a)\mapsto \lambda ([k]a)$ là một đồng cấu nhóm. Gọi $\alpha '$ là cấu xạ nhóm duy nhất từ $G_o*F(K)$ vào M sao cho $\alpha '(f) =$ $(e, f)$ nếu $f\in G_o$ và $\alpha '([k]) = (k, e_o)$ nếu $k\in K$; ta có $\lambda '\circ \alpha '=\lambda$.

Các quan hệ ($R_2$) và ($R''_3$) cho thấy rằng mọi phần tử của $(G/K)_{\gamma(o)}$ là ảnh qua đồng cấu $\lambda$ của một phần tử của $G_o*F(K)$ có dạng $[k]f$, với $f\in G_o$ và $k\in K$. Do đó đồng cấu $\lambda '$ là toàn ánh. Hơn nữa ta cũng kiểm tra được rằng ảnh qua $\alpha '$ của một phần tử của $G_o*$ F(K) có dạng $(R_2)$ hoặc $(R''_3)$ bằng phần tử đơn vị. Do đó, hạt nhân của đồng cấu $\lambda '$ là nhóm con chuẩn tắc nhỏ nhất của M chứa các ảnh qua $\alpha '$ của các phần tử của $G_o*F(K)$ có dạng ($R'_3$).

#### Hệ quả 2 {#ta-ii-s5-prop-6-cor-2 .statement tag=01V2}

Giả sử rằng nhóm K tác động tự do trên Som(G). Khi đó tồn tại một đồng cấu nhóm duy nhất $\pi : (G/K)_{\gamma(o)}\rightarrow$ K mà hạt nhân chứa ảnh của $\gamma_o$ và sao cho $\pi (\lambda ([k])) =k$ với mọi $k\in K$. Hơn nữa, $G_o\longrightarrow^{\gamma_o}(G/K)_{\gamma(o)}-\rightarrow^{\pi}$ K là một mở rộng của K bởi $G_o$.

Nếu tồn tại một đồng cấu nhóm như vậy $\pi$, thì đồng cấu nhóm $\pi \circ \lambda$ tất yếu bằng đồng cấu nhóm duy nhất $p$ từ $G_o*F(K)$ vào K sao cho $p(f) =e$ với $f\in G_o$ và $p([k]) =k$. Ngay lập tức kiểm tra được rằng các phần tử của $G_o*F(K)$ được xác định bởi các công thức ($R_2$) và ($R''_3$) thuộc hạt nhân của $p$. Theo giả thiết, không có phần tử nào kiểu ($R'_3$). Do đó, hạt nhân của cấu xạ $\lambda$ chứa hạt nhân của $p$. Hệ quả là, tồn tại một đồng cấu nhóm duy nhất $\pi : (G/K)_{\gamma(o)}\rightarrow K$ sao cho $\pi \circ \lambda =p$.

Hiển nhiên là đồng cấu $\pi$ là toàn ánh. Để chứng minh rằng đồng cấu $\gamma_o$ là đơn ánh và ảnh của nó chính xác là hạt nhân của $\pi$, ta nhận xét rằng đồng cấu $\lambda ': M\rightarrow (G/K)_{\gamma(o)}$ (II, p. 213, nhận xét 1) là một đẳng cấu, vì đã giả sử rằng K tác động tự do trên Som(G). Đồng cấu hợp thành $(\lambda ')^{-1}\circ \gamma_o$ từ $G_o$ vào M được cho bởi $f\mapsto (e, f)$, trong khi đồng cấu $\pi \circ \lambda ': M\rightarrow K$ biến $(k, f)$ thành $k$. Hệ quả được suy ra.

#### Hệ quả 3 {#ta-ii-s5-prop-6-cor-3 .statement tag=01V3}

Giả sử rằng groupoid G là đơn bắc cầu. Gọi $K_0$ là nhóm con của K sinh bởi các nhóm ổn định của các đỉnh của G. Ánh xạ từ K vào $(G/K)_{\gamma(o)}$ gán cho $k\in K$ phần tử $\gamma (c_k)$ là một đồng cấu nhóm toàn ánh, có hạt nhân là $K_0$.

Nếu một phần tử $k\in K$ cố định một đỉnh $a$ của G, thì phần tử $g^{-1}kg$ cố định đỉnh $g^*a$; điều này kéo theo rằng $K_0$ là một nhóm con chuẩn tắc của K.

Theo mệnh đề 5, đồng cấu duy nhất $\lambda : F(K)\rightarrow$ $(G/K)_{\gamma(o)}$ sao cho $\lambda ([k]) =\gamma (c_k)$ là toàn ánh, và hạt nhân của nó là nhóm con chuẩn tắc nhỏ nhất của F(K) chứa các phần tử $[k]$, trong đó $k$ là một phần tử của K cố định một đỉnh của G, và các phần tử $[kh]^{-1}[k][h]$, trong đó $(k, h)\in K^2$. Đặc biệt, ánh xạ $\lambda ': K\rightarrow (G/K)_{\gamma(o)}$, xác định bởi $\lambda '(k) =\gamma (c_k) =\lambda ([k])$ với $k\in K$, là một đồng cấu nhóm. Ta có $\lambda =\lambda '\circ p$, trong đó $p: F(K)\rightarrow K$ ký hiệu đồng cấu nhóm duy nhất chính tắc. Do đó, đồng cấu $\lambda '$ là toàn ánh và hạt nhân của nó là nhóm con chuẩn tắc nhỏ nhất của K chứa các phần tử $k$, với $k$ cố định một đỉnh của G, nghĩa là $K_0$. Điều này chứng minh mệnh đề.

## BÀI TẬP {#ta-ii-s5-exercises}

Xem [các bài tập của § 5](exercises/s5/).
