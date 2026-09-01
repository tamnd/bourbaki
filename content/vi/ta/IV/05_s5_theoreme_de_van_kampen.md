---
book: ta
book_title: Topologie algébrique
chapter: IV
chapter_title: ESPACES DÉLAÇABLES
section: 5
section_title: Théorème de van Kampen
lang: vi
source: ta-i-iv-fr
book_pages: TA IV.405-TA IV.436, TA IV.463-TA IV.477
pdf_pages: 0421-0452, 0479-0493
extraction: native
subsections:
    - "no": 1
      title: Coégalisateur des projections d’un carré fibré
      page: 405
      pdf_page: 421
    - "no": 2
      title: Recouvrements
      page: 409
      pdf_page: 425
    - "no": 3
      title: Cas particulier d’un recouvrement formé de deux parties
      page: 421
      pdf_page: 437
    - "no": 4
      title: Espaces quotients
      page: 424
      pdf_page: 440
    - "no": 5
      title: Cônes ; contraction d’un sous-espace
      page: 425
      pdf_page: 441
    - "no": 6
      title: Éclatement et recollement
      page: 429
      pdf_page: 445
statements: 31
exercises: 34
content_sha256: f4165a881d61f32d7cd534e8ab43c49f896ec1224a1b31bb10e2a908df886e3a
translated_from: content/en-mt/ta/IV/05_s5_theoreme_de_van_kampen.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 84e9569f0eddb7fac79bf16826926ee8cb4b772f7dd4d387346d3742ab8abf2a
translation_model: gpt-5.4
translation_run: translate-vi-a4d71d9d
glossary_version: 34
glossary_terms_sha256: 0df5bdb409fd11c82def6f49ce2fa1bc195b81ea0de02607f91d0ec76aa7636c
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 5. ĐỊNH LÝ VAN KAMPEN

### 1. Đối đồng chuẩn của các phép chiếu của một hình vuông sợi

Cho X và Y là các không gian tôpô và cho $f$ là một ánh xạ liên tục từ X vào Y. Ký hiệu bởi Z hình vuông sợi $X\times_YX$ và bởi $p_1,p_2$ hai phép chiếu từ Z vào X. Ký hiệu bởi W tích sợi $X\times_YX\times_YX$; với mọi cặp $(s, t)$ số nguyên bằng 1, 2 hoặc 3, ký hiệu bởi $q_{st}: W\rightarrow Z$ ánh xạ xác định bởi $q_{st}(x_1, x_2, x_3) = (x_s, x_t)$.

Ký hiệu bởi Coeg($f$) groupoid Coeg($\varpi (p_1), \varpi (p_2)$), đối đồng chuẩn của hai cấu xạ $\varpi (p_1),\varpi (p_2)$ của groupoid Poincaré $\varpi (Z)$ vào groupoid Poincaré $\varpi (X)$. Ký hiệu bởi $\gamma :\varpi (X)\rightarrow$ Coeg($f$) cấu xạ chính tắc của các groupoid. Vì $f\circ p_1$ = $f\circ p_2$, các cấu xạ groupoid $\varpi (f)\circ \varpi (p_1)$ và $\varpi (f)\circ \varpi (p_2)$ từ $\varpi (Z)$ vào $\varpi (Y)$ là bằng nhau; do đó tồn tại một cấu xạ groupoid duy nhất $\varpi '(f):$ Coeg($f$)$\rightarrow \varpi (Y)$ sao cho $\varpi '(f)\circ \gamma =\varpi (f)$.

#### Định nghĩa 1 {#ta-iv-s5-def-1 .statement tag=0230}

Ta nói rằng ánh xạ $f$ thỏa mãn tính chất (VK) nếu nó là ngặt, toàn ánh và nếu cấu xạ $\varpi '(f)$ là một đẳng cấu.

#### Ví dụ 1 {#ta-iv-s5-n1-exa-1 .statement tag=0231}

Tính chất này được thỏa mãn dưới một trong các giả thiết sau:

(i) Các không gian X và Y là co được, không gian $X\times_YX$ là liên thông địa phương bằng cung, ánh xạ $f$ là toàn ánh, thực sự, tách biệt, với các thớ liên thông địa phương;

(ii) Các không gian X và Y là co được, ánh xạ $f$ là toàn ánh, thực sự, tách biệt, với các thớ hữu hạn, đường chéo $\Delta_X$ của $X\times_YX$ là mở và phần bù của nó là liên thông địa phương;

(iii) Các không gian X và Y là co được, ánh xạ $f$ là toàn ánh, mở và có tính chất nâng đường đi;

(iv) Mọi điểm của Y đều có một lân cận mà trên đó tồn tại một tiết diện liên tục của ánh xạ $f$.

Thật vậy, dưới mỗi giả thiết này, ánh xạ $f$ là toàn ánh; nó cũng là ngặt theo I, p. 18, ví dụ 2. Sau cùng, cấu xạ $\varpi '(f)$ là một đẳng cấu, dưới các giả thiết (i), (ii) hoặc (iii) theo IV, p. 398, định lý 1, và dưới giả thiết (iv) ( IV, p. 400, định lý 2).

Mệnh đề 5 của II, p. 208 mô tả các nhóm đẳng hướng của groupoid Coeg($f$). Mục đích của no$^o$ này là làm tường minh, khi $f$ thỏa mãn tính chất (VK), mô tả các nhóm Poincaré của Y được suy ra từ đó bởi hợp thành với đẳng cấu groupoid $\varpi '(f)$. Các nos$^{os}$ sau sẽ được dành cho những trường hợp riêng quan trọng.

Giả sử rằng ánh xạ $f$ thỏa mãn tính chất (VK).

Đặt $\mathsf{I}=\pi_0(X),\mathsf{J}=\pi_0(Z),\mathsf{K}=\pi_0(W)$; với $j\in \mathsf{J}$ và $s\in  \{1,2\}$, đặt $i_s(j) =\pi_0(p_s)(j)$ ; với $k\in \mathsf{K}$ và $s,t\in  \{1,2,3\}$, đặt $j_{st}(k) =\pi_0(q_{st})(k)$. Ký hiệu bởi $\mathsf{\Gamma}$ bộ xương của cặp $(\varpi (p_1), \varpi (p_2))$ các cấu xạ groupoid từ $\varpi (Z)$ vào $\varpi (X)$ (II, p. 185, định nghĩa 3). Nó là quiver $(\mathsf{I},\mathsf{J}, \pi_0(p_1), \pi_0(p_2))$, vì các quỹ đạo của groupoid Poincaré của một không gian tôpô là các thành phần liên thông bằng cung của không gian này.

Giả sử thêm rằng Y liên thông bằng cung và khác rỗng. Theo II, p. 200, nhận xét 2, $\pi_0(\mathsf{\Gamma})$ khi đó song ánh với tập hợp các quỹ đạo của groupoid Coeg($f$); vì ánh xạ $f$ thỏa mãn tính chất (VK), groupoid Coeg($f$) đẳng cấu với groupoid $\varpi (Y)$. Do đó đồ thị $\mathsf{\Gamma}$ là liên thông và khác rỗng.

Gọi dữ kiện van Kampen của $f$ là dữ kiện của các phần tử sau:

(i) với mọi $i\in \mathsf{I}$, một điểm $\mathsf{a}(i)$ của thành phần liên thông bởi đường đi $i$ của X ;

(ii) với mọi $j\in \mathsf{J}$, một điểm $\mathsf{b}(j) = (\mathsf{b}_1(j),\mathsf{b}_2(j))$ của thành phần liên thông bởi đường đi $j$ của Z ;

(iii) với mọi $k\in \mathsf{K}$, một điểm $\mathsf{c}(k) = (\mathsf{c}_1(k),\mathsf{c}_2(k),\mathsf{c}_3(k))$ của thành phần liên thông bởi đường đi $k$ của W;

(iv) với mọi $j\in \mathsf{J}$, lớp $\beta_1(j)$ của một đường đi trong X nối $\mathsf{b}_1(j)$ với $\mathsf{a}(i_1(j))$ và lớp $\beta_2(j)$ của một đường đi trong X nối $\mathsf{b}_2(j)$ với $\mathsf{a}(i_2(j))$;

(v) với mọi $k\in \mathsf{K}$ và với mọi cặp $(s, t)$ bằng $(1,2)$, $(2,3)$ hoặc $(1,3)$, lớp $\gamma_{st}(k)$ của một đường đi trong Z nối $(\mathsf{c}_s(k),\mathsf{c}_t(k))$ với $\mathsf{b}(j_{st}(k))$;

(vi) một dưới-quiver $\mathsf{T}$ của $\mathsf{\Gamma}$ mà đồ thị liên kết là một cây cực đại của đồ thị $\widetilde{\mathsf{\Gamma }}$;

(vii) một phần tử $i_0$ của $\mathsf{I}$.

Hãy chọn một dữ liệu van Kampen của $f$. Khi đó, $(\mathsf{a},\mathsf{b}, \beta_1, \beta_2,\mathsf{T}, i_0)$ là một trang bị cơ bản của cặp $(\varpi (p_1), \varpi (p_2))$ các cấu xạ groupoid từ $\varpi (Z)$ vào $\varpi (X)$ (II, p. 192, déf. 4). Hơn nữa, các bộ ba

$$
\mathsf{z}= ((q_{12}(\mathsf{c}(k)),1),(q_{23}(\mathsf{c}(k)),1),(q_{13}(\mathsf{c}(k)),-1))
$$

và các lớp đường đi $(\gamma_{1,2}(k), \gamma_{2,3}(k), \gamma_{1,3}(k))$, trong đó $k$ chạy qua $\mathsf{K}$, xác định một trang bị bù của cặp $(\varpi (p_1), \varpi (p_2))$ (II, p. 208, déf. 3 ; II, p. 205, exemple ; II, p. 205, remarque). Ta sẽ nói rằng trang bị đầy đủ của đối cân bằng tử Coeg($f$) được xác định như vậy được suy ra từ dữ liệu van Kampen của $f$ mà ta đã chọn.

Với mọi $j\in \mathsf{J}$, gọi $\varphi_j:\pi_1(Z,\mathsf{b}(j))\rightarrow \pi_1(X,\mathsf{a}(i_1(j)))$ và $\psi_j:\pi_1(Z,\mathsf{b}(j))\rightarrow \pi_1(X,\mathsf{a}(i_2(j)))$ là các đồng cấu nhóm được định nghĩa bởi

$\varphi_j=$ Int($\beta_1(j)$)$^{-1}\circ (p_1)_*,v\mapsto \beta_1(j)^{-1}((p_1)_*(v))\beta_1(j)$

(1)

$\psi_j=$ Int($\beta_2(j)$)$^{-1}\circ (p_2)_*,v\mapsto \beta_2(j)^{-1}((p_2)_*(v))\beta_2(j)$,

với $v\in \pi_1(Z,\mathsf{b}(j))$. Với mọi $k\in \mathsf{K}$ và mọi $s\in  \{1,2,3\}$, gọi $\lambda_s(k)$ là lớp của một vòng tại điểm $\mathsf{a}(i_s(k))$ trong X được định nghĩa bởi

(2)

$$
\lambda_1(k) =\beta_1(j_{13}(k))^{-1}\cdot ((p_1)_*(\gamma_{13}(k)))^{-1}\cdot ((p_1)_*(\gamma_{12}(k)))\cdot \beta_1(j_{12}(k))
$$

$\lambda_2(k) =\beta_2(j_{12}(k))^{-1}\cdot ((p_2)_*(\gamma_{12}(k)))^{-1}\cdot ((p_1)_*(\gamma_{23}(k)))\cdot \beta_1(j_{23}(k))$,

$$
\lambda_3(k) =\beta_2(j_{23}(k))^{-1}\cdot ((p_2)_*(\gamma_{23}(k)))^{-1}\cdot ((p_2)_*(\gamma_{13}(k)))\cdot \beta_2(j_{13}(k))
$$

Cho $\tau$ là cấu xạ groupoid duy nhất từ Grp($\mathsf{\Gamma}$) vào $\varpi (Y)$ sao cho ánh xạ Som($\tau$ ) ánh xạ $i\in \mathsf{I}$ lên $f(\mathsf{a}(i))$ và Fl($\tau$ ) ánh xạ $j\in \mathsf{J}$ lên lớp các đường đi $f_*(\beta_1(j))^{-1}f_*(\beta_2(j))$ nối $f(\mathsf{a}(i_1(j)))$

$$
\mathsf{a}(i_1(k))
$$

$$
\lambda_1(k)
$$

$$
\mathsf{b}_1(j_{12}(k))\mathsf{b}_1(j_{13}(k))
$$

$$
\mathsf{b}_2(j_{12}(k))\mathsf{b}_2(j_{13}(k))
$$

$$
\mathsf{c}_1(k)
$$

$$
\mathsf{c}_2(k)\mathsf{c}_3(k)
$$

$$
\lambda_2(k)\lambda_3(k)
$$

$$
\mathsf{a}(i_2(k))\mathsf{b}_1(j_{23}(k))\mathsf{b}_2(j_{23}(k))\mathsf{a}(i_3(k))
$$

với $f(\mathsf{a}(i_2(j)))$ trong Y. Với $i\in \mathsf{I}$, gọi $d_i\in$ Grp($\mathsf{\Gamma}$) là lớp của đường đi duy nhất không quay lui nối $i_0$ với $i$ trong cây $\widetilde{\mathsf{T}}$ và đặt $\delta_i=$ $\tau (d_i)$.

Nếu S là một tập hợp, nhắc lại rằng F(S) ký hiệu nhóm tự do trên S; ảnh trong F(S) của một phần tử $s\in S$ bởi ánh xạ chính tắc được ký hiệu bởi $[s]$, hoặc bởi $s$ nếu không có khả năng gây nhầm lẫn.

#### Định lý 1 {#ta-iv-s5-thm-1 .statement tag=0232}

Giả sử Y liên thông bằng đường và $f$ thỏa mãn tính chất (VK). Với các ký hiệu trước đó, tồn tại một đồng cấu nhóm duy nhất

$$
\mathsf{L}:(_i*_{\in\mathsf{I}}\pi_1(X,\mathsf{a}(i)))*F(\mathsf{J})\rightarrow \pi_1(Y, f(\mathsf{a}(i_0)))
$$

sao cho

$\mathsf{L}(v) =\delta_if_*(v)\delta^{-1}_i$ với $i\in \mathsf{I}$ và $v\in \pi_1(X,\mathsf{a}(i))$,

$\mathsf{L}(j) =\delta_{i_1(j)}\tau (j)\delta^{-1}_{i_2(j)}$ với $j\in \mathsf{J}$.

Hơn nữa, đồng cấu $\mathsf{L}$ là toàn ánh và hạt nhân của nó là nhóm con chuẩn tắc nhỏ nhất chứa các phần tử sau:

($R_1$)$\mathsf{r}_1(j) =j$ với $j$ thuộc Fl($\mathsf{T}$) ;

($R_2$)$\mathsf{r}_2(j, v) =\varphi_j(v)j\psi_j(v)^{-1}j^{-1}$ với $j\in \mathsf{J}$ và $v\in \pi_1(Z,\mathsf{b}(j))$;

($R_3$)$\mathsf{r}_3(k) =\lambda_1(k)j_{12}(k)\lambda_2(k)j_{23}(k)\lambda_3(k)j_{13}(k)^{-1}$, với $k\in \mathsf{K}$.

Sự tồn tại và tính duy nhất của đồng cấu $\mathsf{L}$ suy ra từ tính chất phổ quát của các tích tự do và các nhóm tự do. Hơn nữa, đồng cấu này là hợp thành của đồng cấu $\varpi '(f)_{\gamma(\mathsf{a}(i_0))}$ suy ra từ $\varpi '(f)$ bằng cách chuyển qua các nhóm đẳng hướng, và của đồng cấu nhóm $\lambda$ được xác định bởi Mệnh đề 5 của II, p. 208, có tính đến sự kiện rằng dữ liệu van Kampen đã chọn xác định một trang bị đầy đủ của cặp $(\varpi (p_1), \varpi (p_2))$ các cấu xạ nhóm vị từ $\varpi (Z)$ vào $\varpi (X)$. Theo mệnh đề đó, ảnh của đồng cấu $\lambda$ là nhóm Coeg($f$)$_{\gamma(\mathsf{a}(i_0))}$ và hạt nhân của nó là nhóm con chuẩn tắc nhỏ nhất chứa các phần tử được xác định bởi các quan hệ ($R_1$)$, (R_2)$ và ($R_3$). Mặt khác, cấu xạ nhóm vị $\varpi '(f):$ Coeg($f$)$\rightarrow \varpi (Y)$ là một đẳng cấu, theo định nghĩa của tính chất (VK). Vậy định lý được chứng minh.

### 2. Phủ

Cho Y là một không gian tôpô khác rỗng liên thông bằng cung, và cho $(A_i)_{i\in I}$ là một phủ của Y bởi các tập con khác rỗng liên thông bằng cung, được đánh chỉ số bởi một tập sắp thứ tự toàn phần I. Cho $X =\bigsqcup_{i\in I}A_i$ là không gian tổng của họ $(A_i)$ và cho $f: X\rightarrow Y$ là ánh xạ suy ra từ họ các đơn ánh chính tắc của mỗi $A_i$ vào Y. Giả sử rằng ánh xạ $f$ thỏa mãn tính chất (VK). Điều này đặc biệt xảy ra trong hai trường hợp sau:

(i) các phần trong của các tập hợp $A_i$, với $i\in I$, phủ Y (xem IV, p. 402, Ví dụ 2);

(ii) không gian Y co được, cũng như các không gian $A_i$, với $i\in I$, họ $(A_i)_{i\in I}$ là hữu hạn địa phương, các $A_i$ đóng trong Y và các giao từng đôi một của chúng là liên thông bằng cung địa phương (xem IV, p. 399, Ví dụ 1).

Cho $J'$ là tập hợp các bộ ba $(i, i',V)$, trong đó $i$ và $i'$ là các phần tử của I và V là một thành phần liên thông bằng cung của $A_i\cap A_{i'}$. Nếu $j= (i, i',V)\in J'$, đặt $i_1(j) =i,i_2(j) =i'$ và $\overline{j}= (i', i,V)$. Cho J là tập con của $J'$ gồm các bộ ba sao cho $i < i'$. *Khung* của phủ là đồ thị có hướng Γ mà tập các đỉnh là I, tập các mũi tên là J, và các ánh xạ gốc và đích của nó lần lượt là các ánh xạ $j\mapsto i_1(j)$ và $j\mapsto i_2(j)$. Ta đồng nhất đồ thị liên kết với Γ với đồ thị $\widetilde{\Gamma}$ mà tập các đỉnh là I, tập các mũi tên là $J\cup \overline{J}$, các ánh xạ gốc và đích là các ánh xạ $j\mapsto i_1(j)$ và $j\mapsto i_2(j)$, và phép đối hợp là ánh xạ $j\mapsto \overline{j}$.

Cho $p_1$ và $p_2$ ký hiệu các phép chiếu của tích thớ $X\times_YX$ lên X; cho $\mathsf{\Gamma}$ là khung của cặp $(\varpi (p_1), \varpi (p_2))$ các cấu xạ nhóm vị từ $\varpi (X\times_YX)$ vào $\varpi (X)$.

#### Bổ đề 1 {#ta-iv-s5-lem-1 .statement tag=0233}

Đồ thị có hướng Γ đồng nhất với một đồ thị có hướng con của $\mathsf{\Gamma}$; các đồ thị có hướng Γ và $\mathsf{\Gamma}$ là liên thông.

Các thành phần cung-liên thông của X là các $A_i$, với $i\in I$. Các thành phần cung-liên thông của $X\times_YX$ là các $(V\times  \{i\})\times_Y$ $(V\times  \{i'\})$, với $(i, i',V)\in J'$. Do đó, khung $\mathsf{\Gamma}$ của cặp $(\varpi (p_1), \varpi (p_2))$ đẳng cấu với quiver có tập đỉnh là I, có tập mũi tên là $J'$, các ánh xạ gốc và ngọn lần lượt là các ánh xạ $j\mapsto i_1(j)$ và $j\mapsto i_2(j)$. Quiver $\mathsf{\Gamma}$ là liên thông (IV, p. 406). Hơn nữa, mô tả này đồng nhất Γ với một quiver con của $\mathsf{\Gamma}$. Ta cũng nhận thấy rằng với mọi mũi tên $j$ của $\mathsf{\Gamma}$, hoặc $j\in$ Fl($\widetilde{\Gamma}$), hoặc tồn tại $i\in I$ sao cho $j= (i, i,A_i)$. Suy ra ánh xạ $\pi_0(\Gamma )\rightarrow \pi_0(\mathsf{\Gamma})$ suy ra từ đơn ánh của Γ vào $\mathsf{\Gamma}$ là song ánh, nên Γ là liên thông.

Với mọi phần tử $i$ của I, chọn một điểm $a(i)$ của $A_i$.

Với mọi phần tử $j= (i, i',V)$ của J, chọn một điểm $b(j)$ trong V, một đường đi $B_1(j)$ nối $b(j)$ với $a(i)$ trong $A_i$ và một đường đi $B_2(j)$

nối$\overline{j}= (i', i,b(jV)$) tớibelongs to$a(i')$ trong A$J^{i'}$. Choand và đặt$j= (i, ib(',\overline{j}V)$) =một phần tử của$b(j)$, $B_1(j) = B\overline{J}_2$; khi đó$(\overline{j})$ và $B_2(j) = B_1(\overline{j})$. Với $j\in J'\cup \overline{J'}$, các đường đi $\overline{B_1(j)}$ và $B_2(j)$ trong Y ghép được. Đặt

$$
B(j) = B_1(j)*B_2(j) \tag{3}
$$

Đó là một đường đi nối $a(i_1(j))$ với $a(i_2(j))$ trong Y; ta có quan hệ $B(\overline{j}) = B(j)$.

Với mọi $j= (i, i',V)\in J'$, ký hiệu $p_{j,1}: V\rightarrow A_i$ và $p_{j,2}: V\rightarrow A_{i'}$ là các đơn ánh chính tắc; cũng ký hiệu $\varphi_j:\pi_1(V, b(j))\rightarrow \pi_1(A_i, a(i))$ và $\psi_j:\pi_1(V, b(j))\rightarrow \pi_1(A_{i'}, a(i'))$ là các đồng cấu nhóm được xác định bởi

$$
\varphi_j(v) = [B_1(j)]^{-1}(p_{j,1})_*(v)[B_1(j)]
$$

và

$$
\psi_j(v) = [B_2(j)]^{-1}(p_{j,2})_*(v)[B_2(j)]
$$

với $v\in \pi_1(V, b(j))$ (xem IV, p. 407).

Cố định một phần tử $i_0$ của I, cũng như một quiver con T trong quiver Γ mà đồ thị liên kết $\widetilde{T}$ của nó là một cây cực đại của đồ thị $\widetilde{\Gamma}$.

Với $i\in I$, xét $(i_0, j_1, i_1, . . . , j_n, i)$ là đường đi duy nhất không quay lui nối $i_0$ với $i$ trong cây $\widetilde{T}$, và đặt

$$
\delta (i) = [B(j_1)][B(j_2)]. . .[B(j_n)]
$$

đây là lớp của một đường đi nối $a(i_0)$ với $a(i)$ trong Y. Ký hiệu $\alpha_i$ là đồng cấu từ $\pi_1(A_i, a(i))$ vào $\pi_1(Y, a(i))$ suy ra từ đơn ánh chính tắc, và ký hiệu $\mu_i:\pi_1(A_i, a(i))\rightarrow \pi_1(Y, a(i_0))$ là đồng cấu nhóm được xác định bởi

$$
\mu_i(v) =\delta (i)\alpha_i(v)\delta (i)^{-1}
$$

Sau hết, ký hiệu $\mu: F(J)\rightarrow \pi_1(Y, a(i_0))$ là đồng cấu nhóm duy nhất sao cho ta có

$$
\mu(j) =\delta (i_1(j))[B(j)]\delta (i_2(j))^{-1}
$$

với mọi $j\in J$. Tồn tại một đồng cấu nhóm duy nhất

$$
\mathsf{M}:(_i*_{\in I}\pi_1(A_i, a(i)))*F(J)\rightarrow \pi_1(Y, a(i_0))
$$

trùng với $\mu_i$ trên $\pi_1(A_i, a(i))$, với mọi $i\in$ I, và với $\mu$ trên F(J).

Gọi $K'$ là tập hợp các bộ bốn $(i_1, i_2, i_3,U)$, trong đó $i_1, i_2, i_3$ là các phần tử của I và U là một thành phần liên thông bằng đường của $A_{i_1}\cap A_{i_2}\cap A_{i_3}$. Với mọi phần tử $k= (i_1, i_2, i_3,U)$ của $K'$ và mọi cặp $(s, t)$ các phần tử của $\{1,2,3\}$, đặt $j_{st}(k) = (i_s, i_t,V)$, trong đó V là thành phần liên thông bằng đường của $A_{i_s}\cap A_{i_t}$ chứa U; đây là một phần tử của $J'$.

Gọi K là tập con của $K'$ tạo thành bởi các bộ bốn $(i_1, i_2, i_3,U)$ sao cho $i_1< i_2< i_3$. Với mọi phần tử $k= (i_1, i_2, i_3,U)$ của K, chọn một điểm $c(k)$ của U, cùng với các đường đi $C_{12}(k)$, $C_{23}(k)$ và $C_{13}(k)$, sao cho $C_{st}(k)$ nối $c(k)$ với $b(j_{st}(k))$ trong $A_{i_s}\cap A_{i_t}$ với $s, t\in  \{1,2,3\}$ và $s < t$.

Khi đó đặt, với $k\in K$,

$$
L_1(k) = B_1(j_{13}(k))*\overline{C_{13}(k)}*C_{12}(k)*B_1(j_{12}(k))
$$

(4) L$L^2_3((kk) = B) = B^2_2((jj^{12}_{23}((kk))))**\overline{CC^{1223}((kk))}**CC^{23}_{13}((kk))**BB^1_2((jj^{23}_{13}((kk))))$,.

Với $s\in  \{1,2,3\}$, ký hiệu $\lambda_s(k)$ là lớp trong $\pi_1(A_{i_s}, a(i_s))$ của vòng $L_s(k)$.

#### Mệnh đề 1 {#ta-iv-s5-prop-1 .statement tag=0234}

Cho Y là một không gian tôpô liên thông bằng đường và cho $(A_i)_{i\in I}$ là một phủ của Y bởi các tập con không rỗng, liên thông bằng đường, được đánh chỉ số bởi một tập sắp thứ tự toàn phần I. Giả sử rằng ánh xạ chính tắc của không gian tổng của họ $(A_i)_{i\in I}$ vào Y thỏa mãn tính chất (VK). Khi đó đồng cấu $\mathsf{M}$ được đưa vào ở trên là toàn ánh, và hạt nhân của nó là nhóm con chuẩn tắc nhỏ nhất chứa các phần tử sau:

($R_1$)$r_1(j) =j$ for $j$ in Fl(T);

($R_2$)$r_2(j, v) =\varphi_j(v)j\psi_j(v)^{-1}j^{-1}$

với $j= (i, i',V)\in J$ và $v\in \pi_1(V, b(j))$;

($R_3$)$r_3(k) =\lambda_1(k)j_{12}(k)\lambda_2(k)j_{23}(k)\lambda_3(k)j_{13}(k)^{-1}$

với $k\in K$.

Cho X là tổng tôpô của họ $(A_i)_{i\in I}$ và gọi $f: X\rightarrow Y$ là ánh xạ cảm sinh bởi họ các đơn ánh chính tắc của mỗi $A_i$ vào Y. Theo giả thiết, ánh xạ $f$ thỏa mãn tính chất (VK); do đó ta sẽ áp dụng Định lý 1 của No$^o1$ cho nó. Vì vậy, ta lấy lại ký hiệu của No$^o$ này và bắt đầu bằng việc xác định một dữ liệu van Kampen cho ánh xạ $f$.

Các thành phần liên thông bằng cung của X là các tập hợp $X_i=$ $A_i\times  \{i\}$ với $i\in I$. Do đó $\pi_0(X)$ được đồng nhất với tập hợp I. Với mỗi $i\in I$, gọi $\mathsf{a}(i)$ là điểm $(a(i), i)$ của $X_i$.

Đặt $Z = X\times_YX$. Các thành phần liên thông bằng cung của Z là các tập hợp $Z_j= (V\times \{i\})\times_Y(V\times \{i'\})$, trong đó $j= (i, i',V)$ chạy qua $J'$. Do đó $\pi_0(Z)$ được đồng nhất với tập hợp $J'$. Gọi $J_0$ là tập hợp các phần tử của J có dạng $(i, i,A_i)$, sao cho họ $(J_0,J,J)$ là một phân hoạch của $J'$. Với $i\in I$ và $j= (i, i,A_i)\in J_0$, đặt $\mathsf{b}(j) = (\mathsf{a}(i),\mathsf{a}(i))$ và lấy cho $\beta_1(j)$ và $\beta_2(j)$ lớp của đường đi hằng tại $\mathsf{a}(i)$. Với $j= (i, i',V)\in J\cup \overline{J}$, gọi $\mathsf{b}(j)$ là điểm $((b(j), i),(b(j), i'))$ của $Z_j$ và gọi $\beta_1(j)$ và $\beta_2(j)$ là các lớp của những đường đi $t\mapsto (B_1(j)(t), i)$ và $t\mapsto (B_2(j)(t), i')$ trong X.

Đặt $W = X\times_YX\times_YX$. Các thành phần liên thông bằng cung của W là các tập hợp $W_k= (U\times  \{i_1\})\times_Y(U\times  \{i_2\})\times_Y(U\times  \{i_3\})$, trong đó $k= (i_1, i_2, i_3,U)$ chạy qua $K'$. Do đó $\pi_0(W)$ được đồng nhất với tập hợp $K'$.

Gọi $K_0$ là tập hợp các phần tử của $K'$ có dạng $k= (i, i, i,A_i)$, với $i\in I$. Với một phần tử như vậy $k\in K_0$, đặt $\mathsf{c}(k) = (\mathsf{a}(i),\mathsf{a}(i),\mathsf{a}(i))$ và chọn cho $\gamma_{st}(k)$ lớp của đường đi hằng tại $(\mathsf{a}(i),\mathsf{a}(i))$.

Gọi $K_1$ là tập hợp các phần tử của $K'$ có dạng $k$ = $(i_1, i_2, i_3,V)$ mà tập hợp $\{i_1, i_2, i_3\}$ có hai phần tử. Gọi $k$ là một phần tử của $K'$ có dạng $(i, i, i',V)$, sao cho $j= (i, i',V)$ thuộc $J\cup \overline{J}$. Khi đó ta đặt

$$
\mathsf{c}(k) = ((b(j), i),(b(j), i),(b(j), i')),\gamma_{12}(k) = (\beta_1(j), \beta_1(j))
$$

và lấy cho $\gamma_{13}(k)$ và $\gamma_{23}(k)$ lớp của đường đi hằng tại $\mathsf{b}(j)$. Người ta định nghĩa tương tự $c(k),\gamma_{12}(k),\gamma_{13}(k),\gamma_{23}(k)$ cho mọi phần tử $k$ của $K'$.

Với mọi phần tử $k= (i_1, i_2, i_3,U)$ của K, đặt

$$
\mathsf{c}(k) = ((c(k), i_1),(c(k), i_2),(c(k), i_3))
$$

với mọi cặp $(s, t)$ gồm các phần tử phân biệt của $\{1,2,3\}$, lấy cho $\gamma_{st}(k)$ ảnh qua ánh xạ $x\mapsto ((x, s),(x, t))$ của lớp của đường đi $C_{st}(k)$ trong $A_{i_s(k)}\cap A_{i_t(k)}$.

Với mọi điểm $x= (x_1, x_2, x_3)$ của $X\times_YX\times_YX$ và mọi phép hoán vị $\sigma \in \mathfrak{S}_3$, đặt $\sigma (x) = (x_{\sigma^{-1}(1)}, x_{\sigma^{-1}(2)}, x_{\sigma^{-1}(3)})$. Như vậy xác định được một phép toán của nhóm $\mathfrak{S}_3$ trên W. Với mọi $k= (i_1, i_2, i_3,U)\in K'$ và mọi phép hoán vị $\sigma \in \mathfrak{S}_3$, đặt tương tự $\sigma (k) = (i_{\sigma^{-1}(1)}, i_{\sigma^{-1}(2)}, i_{\sigma^{-1}(3)},U)$; ta có

$$
\sigma (W_k) = (U\times  \{i_{\sigma^{-1}(1)}\})\times_Y(U\times  \{i_{\sigma^{-1}(2)}\})\times_Y(U\times  \{i_{\sigma^{-1}(3)}\}) = W_{\sigma(k)}
$$

Gọi $k= (i_1, i_2, i_3,U)$ là một phần tử của $K'$ sao cho $i_1, i_2, i_3$ từng đôi một phân biệt. Tồn tại một phép hoán vị duy nhất $\sigma \in$ $\mathfrak{S}_3$ sao cho $i_{\sigma^{-1}(1)}< i_{\sigma^{-1}(2)}< i_{\sigma^{-1}(3)}$, để $\sigma (k) =$ $(i_{\sigma^{-1}(1)}, i_{\sigma^{-1}(2)}, i_{\sigma^{-1}(3)},U)$ thuộc K. Với $s\in  \{1,2,3\}$, khi đó ta đặt $c_s(k) =c_{\sigma(s)}(\sigma (k))$ và $c(k) = (c_1(k), c_2(k), c_3(k))$, sao cho $c(k) =\sigma^{-1}(c(\sigma (k)))$. Với $(s, t)\in  \{(1,2),(1,3),(2,3)\}$, người ta định nghĩa $C_{st}(k) = C_{\sigma^{-1}(s)\sigma^{-1}(t)}(\sigma (k))$; đó là một đường đi nối $c(k)$ với $b(j_{\sigma(s)\sigma(t)}(\sigma (k))) =b(j_{st}(k))$.

Kí hiệu $g$ là cấu xạ của các quiver từ Γ vào $\mathsf{\Gamma}$ gắn với một đỉnh $i\in I$ của Γ đỉnh $X_i= A_i\times  \{i\}$ của $\mathsf{\Gamma}$ và với một mũi tên $j= (i, i',V)\in J'$ của Γ mũi tên $Z_j= (V\times \{i\})\times_Y(V\times \{i'\})$ của $\mathsf{\Gamma}$. Ánh xạ Som($g$) là song ánh; ánh xạ Fl($g$) là đơn ánh và đồ thị Γ là liên thông (IV, p. 410, bổ đề 1), và ảnh của quiver con T dưới $g$ là một quiver con $\mathsf{T}$ của $\mathsf{\Gamma}$ mà đồ thị liên kết của nó là một cây cực đại của đồ thị $\widetilde{\mathsf{\Gamma }}$.

Các điểm $\mathsf{a}(i)$, với $i\in I$, các điểm $\mathsf{b}(j)$, với $j\in J'$, các điểm $\mathsf{c}(k)$, với $k\in K'$, các lớp đường đi $\beta_1(j)$ và $\beta_2(j)$, với $j\in J'$, các lớp đường đi $\gamma_{st}(k)$, với $k\in K'$, quiver con $g(T)$ của $\mathsf{\Gamma}$ và phần tử $i_0$ của I xác định một dữ liệu van Kampen cho $f$.

Kí hiệu $\rho$ là đồng cấu nhóm duy nhất

$$
\rho :(_i*_{\in I}\pi_1(X,\mathsf{a}(i)))*F(J')\rightarrow (_i*_{\in I}\pi_1(A_i, a(i)))*F(J)
$$

cảm sinh đẳng cấu từ $\pi_1(X,\mathsf{a}(i))$ lên $\pi_1(A_i, a(i))$ suy ra từ sự đồng nhất $A_i\times  \{i\}$ với $A_i$, với mọi $i\in I$, và sao cho ta có

$\rho (j) = 1$ với $j\in J_0$

$\rho (j) =j,\rho (\overline{j}) =j^{-1}$ với $j\in J$.

Kí hiệu $\mathsf{L}$ là đồng cấu nhóm được định nghĩa trong Định lý 1 của IV, p. 408. Với $j= (i, i,A_i)\in J_0$, ta có $\mathsf{L}(j) = 1 =\mathsf{M}\circ \rho (j)$. Cho $j= (i, i',V)$ là một phần tử của J; ta có $\mathsf{L}(j) = (\mathsf{M}\circ \rho )(j)$ theo định nghĩa. Sau cùng, nếu $j=$ $(i, i',V)$ là một phần tử của $\overline{J},\overline{j}\in J$ thì ta kiểm tra được rằng

$$
\mathsf{L}(j) =\mathsf{L}(\overline{j})^{-1}=\mathsf{M}(\rho (\overline{j}))^{-1}=\mathsf{M}(\rho (j))
$$

Do đó, ta có $\mathsf{M}\circ \rho =\mathsf{L}$.

Đồng cấu $\mathsf{L}$ là toàn ánh (nơi đã dẫn), do đó đồng cấu $\mathsf{M}$ cũng vậy. Vì đồng cấu $\rho$ là toàn ánh, hạt nhân của $\mathsf{M}$ là nhóm con chuẩn tắc nhỏ nhất của $(_i*_{\in I}\pi_1(A_i, a(i)))*F(J_1)$ chứa các ảnh qua $\rho$ của những phần tử được xác định bởi các quan hệ ($R_1$), ($R_2$)$, (R_3)$ của định lý 1 (IV, p. 408). Chứng minh sẽ đầy đủ một khi ta đã kiểm tra rằng các ảnh này, ngoài các phần tử được xác định bởi các quan hệ ($R_1$)$, (R_2), (R_3)$ của Mệnh đề 1, còn là những phần tử liên hợp với chúng, hoặc liên hợp với các nghịch đảo của chúng, cùng với phần tử đơn vị.

Các phần tử $R_1$. — Một mũi tên của cây có hướng $\mathsf{T}$ có dạng $Z_j$, với $j= (i, i',V)\in J$; ảnh của nó là phần tử $j$ của F(J).

Các phần tử $R_2$. — Cho $j= (i, i',V)\in J'$. Nếu $i=i'$, ta có $\rho (\mathsf{r}_2(j, v)) = 1$ với mọi $v\in \pi_1(A_i,\mathsf{a}(i))$. Nếu $j\in J$, ảnh của $\mathsf{r}_2(j, v)$ là phần tử $r_2(j, v) =\varphi_j(v)j\psi_j(v)^{-1}j^{-1}$, với mọi $v\in \pi_1(Z,\mathsf{b}(j))$. Trong trường hợp còn lại, ta có $\overline{j}\in J$ và đẳng thức

$$
\rho (\mathsf{r}_2(j, v)) =\rho (\varphi_j(v)j\psi_j(v)^{-1}j^{-1})
$$

$$
= [B_1(j)]^{-1}v[B_1(j)]\rho (j)[B_2(j)]^{-1}v^{-1}[B_2(j)]\rho (j)^{-1}
$$

$$
= [B_2(\overline{j})]^{-1}v[B_2(\overline{j})]\overline{j}^{-1}[B_1(\overline{j})]^{-1}v^{-1}[B_1(\overline{j})]\overline{j}
$$

cho thấy rằng $\rho (\mathsf{r}_2(j, v))$ liên hợp với $\rho (\mathsf{r}_2(j, v^{-1}))$.

Các phần tử $R_3$. — Cho $k= (i_1, i_2, i_3,U)$ là một phần tử của $K'$.

Nếu $k\in K_0,i_1$ = $i_2$ = $i_3,\lambda_s(k)$ là lớp của đường đi tầm thường với mọi $s\in  \{1,2,3\},j_{st}(k)\in J_0$ với mọi cặp $(s, t)\in$ $\{(1,2),(1,3),(2,3)\}$. Khi đó $\rho (\mathsf{r}_3(k))$ là phần tử đơn vị.

Giả sử $k\in K_1$. Nếu $i_1=i_2$, thì $j= (i_1, i_3,U)\in J\cup \overline{J}$ và ta có

$$
\mathsf{r}_3(k) =\beta_1(j)^{-1}j_{12}\beta_1(j)j_{23}\beta_2(j)^{-1}\beta_2(j)j_{13}^{-1}
$$

mà ảnh của nó qua $\rho$ là phần tử đơn vị. Các trường hợp khác được xử lý tương tự.

Giả sử rằng $i_1, i_2, i_3$ phân biệt từng đôi một. Nếu $i_1< i_2< i_3$, $k\in K$ và ảnh của $\rho (\mathsf{r}_3(k))$ là phần tử $r_3(k)$.

Cho $\sigma \in \mathfrak{S}_3$ là phép hoán vị biến 1 thành 2 và 2 thành 3. Ta có

$$
\lambda_1(\sigma (k)) =\beta_1(j_{13}(\sigma (k)))^{-1}\cdot p_{1,*}(\gamma_{13}(\sigma (k)))^{-1}\cdot
$$

$$
\cdot p_{1,*}(\gamma_{12}(\sigma (k)))\cdot \beta_1(j_{12}(\sigma (k)))
$$

$$
=\beta_1(j_{32}(k))^{-1}\cdot p_{1,*}(\gamma_{32}(k))^{-1}\cdot p_{1,*}(\gamma_{31}(k))\cdot \beta_1(j_{31}(k))
$$

$$
=\beta_2(j_{23}(k))^{-1}\cdot p_{2,*}(\gamma_{2,3}(k))^{-1}\cdot p_{2,*}(\gamma_{13}(k))\cdot \beta_2(j_{13}(k))
$$

$$
=\lambda_3(k)
$$

Ta kiểm tra tương tự rằng $\lambda_2(\sigma (k)) =\lambda_1(k)$ và $\lambda_3(\sigma (k)) =\lambda_2(k)$. Do đó,

$$
\rho (\mathsf{r}_3(\sigma (k))) =\lambda_1(\sigma (k))\rho (j_{12}(\sigma (k)))\lambda_2(\sigma (k))\cdot
$$

$$
\cdot \rho (j_{23}(\sigma (k)))\lambda_3(\sigma (k))\rho (j_{13}(\sigma (k)))^{-1}
$$

$$
=\lambda_3(k)\rho (j_{31}(k))\lambda_1(k)\rho (j_{12}(k))\lambda_2(k)\rho (j_{32}(k))^{-1}
$$

$$
=\lambda_3(k)j_{13}(k)^{-1}\lambda_1(k)j_{12}(k)\lambda_2(k)j_{23}(k)
$$

điều này chứng minh rằng $\rho (\mathsf{r}_3(\sigma (k)))$ liên hợp với

$$
\lambda_1(k)j_{12}(k)\lambda_2(k)j_{23}(k)\lambda_3(k)j_{13}(k)^{-1}=\rho (\mathsf{r}_3(k))
$$

Cho $\tau \in \mathfrak{S}_3$ là phép hoán vị đổi chỗ có giá đỡ $\{1,2\}$. Ta có

$\lambda_1(\tau (k)) =\lambda_2(k)^{-1},\lambda_2(\tau (k)) =\lambda_1(k)^{-1}$ và $\lambda_3(\tau (k)) =\lambda_3(k)^{-1}$. Các đẳng thức

$$
\rho (\mathsf{r}_3(\tau (k))) =\lambda_2(k)^{-1}\rho (j_{21}(k))\lambda_1(k)^{-1}\rho (j_{13}(k))\lambda_3(k)^{-1}\rho (j_{23}(k))^{-1}
$$

$$
=(\rho (j_{23}(k))\lambda_3(k)\rho (j_{13}(k))^{-1}\lambda_1(k)\rho (j_{12}(k))\lambda_2(k))^{-1}
$$

cho thấy rằng $\rho (\mathsf{r}_3(\tau (k)))$ liên hợp với nghịch đảo của

$$
\lambda_1(k)\rho (j_{12}(k))^{-1}\lambda_2(k)\rho (j_{23}(k))\lambda_3(k)\rho (j_{13}(k))^{-1}=\rho (\mathsf{r}_3(k))
$$

Vì nhóm $\mathfrak{S}_3$ được sinh bởi các hoán vị $\tau$ và $\sigma$, suy ra rằng, với mọi $k\in K$ và mọi $\sigma \in \mathfrak{S}_3,\rho (\mathsf{r}_3(\sigma (k)))$ liên hợp với $\rho (\mathsf{r}_3(k))$ hoặc với nghịch đảo của nó.

Vậy mệnh đề 1 được chứng minh.

#### Hệ quả 1 {#ta-iv-s5-prop-1-cor-1 .statement tag=0235}

Dưới các giả thiết của mệnh đề 1, giả sử thêm rằng, với mọi $i\in$ I, ảnh của đồng cấu từ $\pi_1(A_i, a(i))$ vào $\pi_1(Y, a(i))$, cảm sinh bởi đơn ánh chính tắc từ $A_i$ vào Y, là tầm thường. Khi đó đồng cấu $\mathsf{M}': F(J)\rightarrow \pi_1(Y, a(i_0))$ cảm sinh bởi $\mathsf{M}$ bằng phép hạn chế là toàn ánh, và hạt nhân của nó là nhóm con phân biệt nhỏ nhất chứa các phần tử $j\in$ Fl(T) và các phần tử $j_{12}(k)j_{23}(k)j_{13}(k)^{-1}$ với $k\in K$.

Cho $\pi : (_i*_{\in I}\pi_1(A_i, a(i)))*F(J)\rightarrow F(J)$ là đồng cấu duy nhất cảm sinh đồng cấu tầm thường trên mỗi $\pi_1(A_i, a(i))$ và đồng nhất trên F(J); nó là toàn ánh. Cho $i\in I$. Định nghĩa của $\mathsf{M}$ và giả thiết rằng ảnh của đồng cấu từ $\pi_1(A_i, a(i))$ vào $\pi_1(Y, a(i))$ cảm sinh bởi đơn ánh chính tắc là tầm thường kéo theo rằng, với mọi $v\in \pi_1(A_i, a(i)),\mathsf{M}(v)$ là phần tử đơn vị của $\pi_1(Y, a(i_0))$. Do đó $\mathsf{M}=\mathsf{M}'\circ \pi$. Suy ra đồng cấu $\mathsf{M}'$ là toàn ánh, và hạt nhân của nó là nhóm con phân biệt nhỏ nhất chứa các ảnh qua $\pi$ của các phần tử $r_1(j),r_2(j, v)$ và $r_3(k)$ được định nghĩa trong Mệnh đề 1. Với $j\in$ Fl(T), ta có $\pi (r_1(j)) =j$. Với mọi $j\in$ J và mọi $v\in \pi_1(V, b(j))$, ta có $\pi (r_2(j, v)) =e$. Cuối cùng, với mọi $k= (i_1, i_2, i_3,U)\in K$ và mọi $s\in$ $\{1,2,3\},\lambda_s(k)$ là lớp của một đường vòng trong $A_{i_s}$; do đó $\pi (\lambda_s(k)) =e$, nên $\pi (r_3(k)) =j_{12}(k)j_{23}(k)j_{13}(k)^{-1}$. Hệ quả được suy ra.

#### Hệ quả 2 {#ta-iv-s5-prop-1-cor-2 .statement tag=0236}

Dưới các giả thiết của mệnh đề 1, giả sử thêm rằng với mọi $i\in I$, nhóm $\pi_1(A_i, a(i))$ thu về phần tử đơn vị và rằng, với mọi bộ ba $(i_1, i_2, i_3)$ gồm các phần tử của I phân biệt từng đôi một, tập hợp $A_{i_1}\cap A_{i_2}\cap A_{i_3}$ là rỗng. Khi đó đồng cấu $\mathsf{M}'':$ F(J-Fl(T)) $\rightarrow \pi_1(Y, a(i_0))$ cảm sinh bởi $\mathsf{M}$ bằng phép hạn chế là một đẳng cấu.

Cho $\pi ': F(J)\rightarrow$ F(J - Fl(T)) là đồng cấu ánh xạ $[j]$ lên $[j]$ nếu $j\in$ J-Fl(T) và ánh xạ $[j]$ lên phần tử đơn vị nếu $j\in$ Fl(T); nó là toàn ánh và ta có $\mathsf{M}''\circ \pi '=\mathsf{M}'$, trong đó $\mathsf{M}'$ là đồng cấu toàn ánh được định nghĩa trong hệ quả 1. Suy ra $\mathsf{M}''$ là toàn ánh và hạt nhân của nó là nhóm con phân biệt nhỏ nhất của F(J-Fl(T)) chứa các ảnh qua $\pi '$ của các phần tử được mô tả trong loc. cit. Nhưng, theo phép dựng, $\pi '(j) =e$ nếu $j\in$ Fl(T) và tập hợp K là rỗng, theo giả thiết. Vậy đồng cấu $\mathsf{M}''$ là một đẳng cấu.

#### Ví dụ 1 {#ta-iv-s5-n2-exa-1 .statement tag=0237}

Đối với trường hợp một phủ gồm hai tập hợp, xem No. 3.

#### Ví dụ 2 {#ta-iv-s5-n2-exa-2 .statement tag=0238}

Cho G là một đồ thị (II, p. 155, định nghĩa 1); gọi S là tập hợp các đỉnh của G, A là tập hợp các cạnh định hướng của nó, $o$ và $t$ là các ánh xạ gốc và ngọn từ A vào S; với mỗi cạnh định hướng $a\in A$, gọi $\overline{a}$ là cạnh định hướng đối. Trang bị cho các tập hợp S và A tôpô rời rạc; gọi X là không gian tổng của không gian S và của không gian $\mathbf{I}\times A$, và gọi $\sim$ là quan hệ tương đương mịn nhất trên X sao cho $(u, a)\sim (1-u, a)$, $(0, a)\sim o(a)$ và $(1, a)\sim t(a)$ với mọi $u\in \mathbf{I}$ và mọi cạnh định hướng $a\in A$. Không gian thương $|G|= X/\sim$ được gọi là thực hiện hình học của đồ thị G. Gọi $p$ là phép chiếu chính tắc từ X lên $|G|$.

Ta hãy chứng minh rằng $|G|$ co được địa phương. Cho $s\in S$. Gọi $X_s$ là hợp của $\{s\}$ và của các tập hợp $[0,1[\times  \{a\}$ với $a\in \overset{-1}{o}(s)$ và của các

tập hợp $]0,1]\times \{a\}$ với $a\in \overset{-1}{t}(s)$. Gọi $U_s$ là ảnh của $X_s$ trong $|G|$; đó là một lân cận mở của $p(s)$ trong $|G|$ vì $X_s$ là một lân cận mở bão hòa của $s$ trong X. Gọi $f$ là ánh xạ từ $X_s\times \mathbf{I}$ vào $X_s$ được xác định, với $u, v\in \mathbf{I}$ và $a\in A$, bởi các quan hệ

$$
f(s, v) =s
$$

$((1-v)u, a)$ nếu $0\leqslant u <1$ và $o(a) =s$,

$$
f((u, a), v) =
$$

$(1-(1-v)(1-u), a)$ nếu $0< u\leqslant 1$ và $t(a) =s$.

Nó liên tục và tương thích với quan hệ tương đương $\sim$. Do đó, bằng cách chuyển qua thương, nó xác định một ánh xạ $\varphi_s: U_s\times \mathbf{I}\rightarrow U_s$ liên tục, vì $\mathbf{I}$ là compact địa phương (I, p. 19, Prop. 10). Đó là một phép co mạnh của $U_s$ lên $p(s)$ (III, p. 237, Def. 6).

Giả sử thêm rằng $x= (\tau , a)\in ]0,1[\times A$. Ta ký hiệu bởi $X_x= ]0,1[\times  \{a, a\}$ và gọi $U_x$ là ảnh của nó trong $|G|$ bởi $p$; đó là một lân cận của $p(x)$ trong $|G|$, đồng phôi với $]0,1[$. Ánh xạ từ $X_x\times \mathbf{I}$ vào $X_x$ cho bởi $((u, a), v)\mapsto ((1-v)u+v\tau , a)$ và $((u, a), t)\mapsto ((1-v)u+v(1-\tau ), a)$ là liên tục. Bằng cách chuyển qua thương, nó xác định một ánh xạ $\varphi_x: U_x\times$ $\mathbf{I}\rightarrow U_x$ liên tục (loc. cit.) và là một phép co mạnh tại $x$.

Mọi điểm của $|G|$ là ảnh của một điểm $s\in S$ hoặc của một điểm của $\mathbf{I}\times A$ có dạng $(\tau , a)$ với $0< \tau  <1$. Suy ra mọi điểm của $|G|$ đều có một lân cận co được tại điểm đó. Nói cách khác, $|G|$ co được địa phương và, đặc biệt, tháo xoắn được (IV, p. 346, Prop. 5).

Ta chọn một thứ tự toàn phần trên S và xét phủ mở $(U_s)_{s\in S}$ của $|G|$. Cho $s$ và $s'$ là hai phần tử phân biệt của S. Giao $U_s\cap U_{s'}$ là hợp của các $p(]0,1[, a)$ khi $a$ chạy qua tập hợp các cạnh có hướng của G mà các đầu mút là $s$ và $s'$. Do đó, cốt của phủ $(U_s)_{s\in S}$ được đồng nhất với quiver G. Hơn nữa, với mọi $s\in S$, $U_s$ co được tại $s$, nên $\pi_1(U_s, p(s))$ thu về phần tử đơn vị. Khi đó suy ra từ Hệ quả 2 của IV, p. 416 rằng với mọi $s\in S,\pi_1(|G|, p(s))$ là một nhóm tự do (định lý Nielsen-Schreier).

#### Hệ quả 3 {#ta-iv-s5-prop-1-cor-3 .statement tag=0239}

Dưới các giả thiết của Mệnh đề 1, giả sử thêm rằng cốt của phủ $(A_i)_{i\in I}$ là một cây có hướng. Khi đó đồng cấu $\mathsf{N}:_i*_{\in I}\pi_1(A_i, a(i))\rightarrow \pi_1(Y, a(i_0))$ suy ra từ $\mathsf{M}$ bằng cách hạn chế là toàn ánh; hạt nhân của nó là nhóm con chuẩn tắc nhỏ nhất của $_i*_{\in I}\pi_1(A_i, a(i))$ chứa các phần tử $\varphi_j(v)\psi_j(v)^{-1}$, với

mọi $j= (i_1, i_2,V)\in J$ và mọi $v\in \pi_1(V, b(j))$.

Nếu thêm nữa các thành phần liên thông theo cung của các giao $A_i\cap A_{i'}$, với $i=\not i'$, là đơn liên, thì đồng cấu $\mathsf{N}$ là một đẳng cấu.

Dưới các giả thiết của hệ quả, đồ thị liên kết với quiver Γ là một cây, do đó T = Γ. Suy ra ảnh của nhóm F(J) bởi đồng cấu $\mathsf{M}$ thu về phần tử đơn vị.

Cho

$$
\rho :(_i*_{\in I}\pi_1(A_i, a(i)))*F(J)\rightarrow_i*_{\in I}\pi_1(A_i, a(i))
$$

là đồng cấu nhóm duy nhất cảm sinh đồng cấu đồng nhất trên $\pi_1(A_i, a(i))$ và có hạt nhân chứa F(J). Ta có $\mathsf{M}=\mathsf{N}\circ \rho$. Do đó, đồng cấu $\mathsf{N}$ là toàn ánh và hạt nhân của nó là nhóm con chuẩn tắc nhỏ nhất của $_i*_{\in I}\pi_1(A_i, a(i))$ mà nó

chứa các ảnh qua $\rho$ của các phần tử được xác định bởi các quan hệ ($R_1$), ($R_2$) và ($R_3$) của Mệnh đề 1. Ta có $\rho (j) = 1$ với mọi $j\in$ Fl(Γ). Vì khung của phủ $(A_i)_{i\in I}$ là một cây, nên ta có $A_{i_1}\cap A_{i_2}\cap A_{i_3}=\emptyset$ với mọi bộ ba $(i_1, i_2, i_3)$ gồm các phần tử phân biệt của I. Suy ra hạt nhân của $\mathsf{N}$ là nhóm con chuẩn tắc nhỏ nhất chứa các phần tử $\varphi_j(v)\psi_j(v)^{-1}$ với mọi $j= (i_1, i_2,V)\in J$ và mọi $v\in \pi_1(V, b(j))$.

#### Ví dụ 3 (Mặt phẳng bỏ đi $n$ điểm) {#ta-iv-s5-n2-exa-3 .statement tag=023A}

Nhóm cơ bản của $\mathbf{R}^2$ $\{0\}$ đẳng cấu với $\mathbf{Z}$, và lớp của đường đi $t\mapsto e^{2\pi it}$ là một phần tử sinh của nó (IV, p. 347, hệ quả). Nói chung hơn, cho $n$ là một số tự nhiên và cho $A =\{z_1, . . . , z_n\}$ là một tập hợp gồm $n$ điểm của $\mathbf{R}^2$. Gọi Y là không gian $\mathbf{R}^2-$ A; ta sẽ chứng minh rằng nhóm cơ bản của Y đẳng cấu với nhóm tự do $F_n$ trên $n$ phần tử sinh. Với mọi $i$, đặt $z_i= (u_i, v_i)$. Nếu cần, thay thế $z_i$ bởi $f(z_i)$, trong đó $f:\mathbf{R}^2\rightarrow \mathbf{R}^2$ là một đồng phôi có dạng $(u, v)\mapsto (u+\alpha v, v)$, ta có thể giả sử rằng các hoành độ của các $z_i$ phân biệt từng đôi một. Tương tự, cũng không mất tính tổng quát khi giả sử rằng ta có $u_1<\cdots < u_n$.

Đặt $V_1= ]-\infty , u_2[\times \mathbf{R},V_i= ]u_{i-1}, u_{i+1}[\times \mathbf{R}$ với $2\leqslant i\leqslant n-1$, $V_n= ]u_{n-1},+\infty [\times \mathbf{R}$. Với $1\leqslant i\leqslant n$, tập hợp $U_i= V_i-\{z_i\}$ là mở trong mặt phẳng và đồng phôi với $\mathbf{R}^2-\{0\}$. Họ $(U_i)_{1\leqslant i\leqslant n}$ là một phủ mở của không gian $Y =\mathbf{R}^2-$ A. Giao $U_i\cap U_j$ là rỗng khi $|i-j|\geqslant 2$, đồng phôi với $\mathbf{R}^2$ khi $|i-j|= 1$. Theo Hệ quả 3, nhóm cơ bản của Y đẳng cấu với nhóm tự do $F_n$.

Cho $a$ là một điểm của Y. Với mọi số nguyên $i\in  \{1, . . . , n\}$, cho $r_i$ là một số thực dương ngặt và nhỏ hơn một cách ngặt khoảng cách từ $z_i$ đến các điểm $z_j$, với $j=\not i$. Ký hiệu $v_i$ là lớp của vòng lặp $t\mapsto$ $z_i+r_ie^{2\pi it}$ tại điểm $z_i+r_i$ của Y. Ký hiệu $\theta_i$ là lớp của một đường đi $\gamma_i$ nối điểm $a$ với điểm $z_i+r_i$ trong Y. Nếu các đường đi $\gamma_i$ là đơn ánh và nếu các ảnh của chúng chỉ gặp nhau tại $a$, thì có thể chứng minh rằng đồng cấu duy nhất của nhóm tự do $F(t_1, . . . , t_n)$ vào $\pi_1(Y, a)$ sao cho $\varphi (t_i) =\theta_iv_i\theta^{-1}_i$ với mọi $i\in  \{1, . . . , n\}$ là một đẳng cấu nhóm.

Một lập luận tương tự cho phép chứng minh rằng với mọi tập con đóng rời rạc A của mặt phẳng, nhóm cơ bản của $\mathbf{R}^2-$ A đẳng cấu với F(A) (IV, p. 463, Bài tập 1).

#### Hệ quả 4 {#ta-iv-s5-prop-1-cor-4 .statement tag=023B}

Dưới các giả thiết của Mệnh đề 1, giả sử tồn tại một tập con A của Y, liên thông bởi các cung và khác rỗng, sao cho giao $A_i\cap A_{i'}$ bằng A với mọi cặp $(i, i')$ gồm các phần tử phân biệt của I. Cho $a$ là một điểm của A. Tồn tại một đồng cấu duy nhất $\varphi$ từ tổng của họ các nhóm $(\pi_1(A_i, a))_{i\in I}$ ghép theo $\pi_1(A, a)$ vào $\pi_1(Y, a)$, trùng với đồng cấu cảm sinh bởi đơn ánh chính tắc từ $A_i$ vào Y, với mọi $i\in I$. Đồng cấu $\varphi$ là một đẳng cấu.

Đặc biệt, nếu nhóm $\pi_1(A, a)$ thu về phần tử đơn vị, thì đồng cấu chính tắc từ tích tự do của họ các nhóm $(\pi_1(A_i, a))_{i\in I}$ vào $\pi_1(Y, a)$ là một đẳng cấu.

Với $i\in$ I, ký hiệu $g_i:\pi_1(A, a)\rightarrow \pi_1(A_i, a)$ và $f_i:\pi_1(A_i, a)\rightarrow$ $\pi_1(Y, a)$ là các đồng cấu chính tắc cảm sinh bởi các bao hàm của A vào $A_i$ và của $A_i$ vào Y. Ký hiệu $*\pi_1(A_i, a)$ là tổng của các nhóm $\pi_1(A_i, a)$ ghép theo $\pi_1(A, a)$. Lại nữa, gọi$^Ap$ là đồng cấu duy nhất của $_i*_{\in I}\pi_1(A_i, a)$ vào $*_A\pi_1(A_i, a)$ cảm sinh đồng nhất trên $\pi_1(A_i, a)$ (A, I, p. 80, prop. 4). Đồng cấu $p$ là toàn ánh và từ định nghĩa của monoide $*\pi_1(A_i, a)$ suy ra rằng hạt nhân của nó là nhóm con chuẩn tắc nhỏ nhất của$^A_i*_{\in I}\pi_1(A_i, a)$ chứa các

phần tử $g_i(v)g_{i'}(v)^{-1}$, với $i, i'\in I$ và $v\in \pi_1(A, a)$.

Các đồng cấu $f_i\circ g_i:\pi_1(A, a)\rightarrow \pi_1(Y, a)$, với $i\in I$, bằng nhau. Do đó suy ra từ tính chất phổ quát của các tổng hợp nhất của monoit (A, I, p. 80, Prop. 4) rằng tồn tại một đồng cấu nhóm duy nhất $\varphi$ (resp. $f$) từ $*_A\pi_1(A_i, a)$ (resp. from $_i*_{\in I}\pi_1(A_i, a)$) vào $\pi_1(Y, a)$ cảm sinh đồng cấu $f_i$ trên $\pi_1(A_i, a)$. Ta có $f=$ $\varphi \circ p$.

Với $i\in$ I, gọi $u_i$ là đơn ánh chính tắc của A vào $A_i$ và $v_i$ là đơn ánh chính tắc của $A_i$ vào Y. Cũng gọi $w$ là đơn ánh chính tắc của A vào Y. Với mọi $i\in$ I, ta có $v_i\circ u_i$ = $w$, nên $\pi_1(v_i, a)\circ \pi_1(u_i, a) =\pi_1(w, a)$. Khi đó suy ra từ tính chất phổ quát của các tổng hợp nhất của monoit (A, I, p. 80, Prop. 4) rằng tồn tại một đồng cấu nhóm duy nhất $\varphi$ từ $*_i\pi_1(A_i, a)$ vào $\pi_1(Y, a)$ cảm sinh đồng cấu $\pi_1(v_i, a)$ trên $\pi_1(A_i, a)$. Còn lại phải chứng minh rằng $\varphi$ là một đẳng cấu.

Tập hợp J được đồng nhất với tập hợp các cặp $(i, i')$ các phần tử của I sao cho $i < i'$. Tập hợp K được đồng nhất với tập hợp các bộ ba $(i_1, i_2, i_3)$ các phần tử của I sao cho $i_1< i_2< i_3$. Hãy chọn tất cả các điểm cơ sở $a(i),b(j)$ và $c(k)$ đều bằng $a$ và tất cả các đường $B(j)$, $C_{st}(k)$ đều bằng đường hằng có ảnh là $a$. Ta cũng cố định một điểm $i_0\in I$.

Với mọi cặp $(i, i')$ các điểm phân biệt của I, khung Γ của phủ $(A_i)$ có đúng một mũi tên với hai đầu mút là $i$ và $i'$. Các mũi tên của Γ mà một trong hai đầu mút bằng $i_0$ là các mũi tên của một cây cực đại có hướng T.

Với mọi phần tử $k\in K$, ta có $r_3(k) =j_{12}(k)j_{23}(k)j_{13}(k)^{-1}$; gọi R là nhóm con chuẩn tắc của F(J) sinh bởi các phần tử $j\in$ Fl(T) và các phần tử $r_3(k),k\in$ K. Hãy chứng minh rằng R = F(J). Chỉ cần chỉ ra rằng mọi phần tử $j= (i_1, i_2)$ của J đều thuộc R. Điều này đúng, theo giả thiết, nếu $i_1=i_0$ hoặc $i_2=i_0$. Giả sử $i_0< i_1$ và đặt $k= (i_0, i_1, i_2)$. Đây là một phần tử của K sao cho $j=j_{23}(k) =j$. Hơn nữa, $j_{12}(k)$ và $j_{13}(k)$ thuộc Fl(T). Suy ra $j$ thuộc R. Các trường hợp $i_1< i_0< i_2$ hoặc $i_2< i_0$ được xử lý một cách tương tự.

Suy ra từ Mệnh đề 1 (IV, p. 412) rằng đồng cấu $f$ là toàn ánh và hạt nhân của nó là nhóm con chuẩn tắc nhỏ nhất chứa các quan hệ $r_2(j, v) =g_i(v)g_{i'}(v)^{-1}$, với $j= (i, i',A)\in J$ và $v\in \pi_1(A, a)$. Nói cách khác, Ker($f$) $=$ Ker($p$). Suy ra $\varphi$ là một đẳng cấu, đúng như phải chứng minh.

Nếu $\pi_1(A, a)$ thu về phần tử đơn vị, thì $p$ là một đẳng cấu, do đó có mệnh đề thứ hai.

#### Ví dụ 4 {#ta-iv-s5-n2-exa-4 .statement tag=023C}

Cho $((X_i, x_i))_{i\in I}$ là một họ các không gian tôpô có điểm gốc. Bó của họ $((X_i, x_i))_{i\in I}$ theo định nghĩa, và được ký hiệu bởi $\bigvee_{i\in I}(X_i, x_i)$, là không gian tôpô thương của không gian tổng của họ $(X_i)_{i\in I}$ theo quan hệ tương đương đồng nhất hóa tất cả các điểm $(x_i, i)$ với nhau, với $i\in I$. Gọi X là không gian tôpô này và $x$ là ảnh chung của các $x_i$. Giả sử rằng, với mọi $i\in$ I, điểm $x_i$ là đóng trong $X_i$ và các không gian $X_i$ là đơn liên. Nếu I là hữu hạn, Hệ quả 4 suy ra rằng đồng cấu chính tắc $_i*_{\in I}\pi_1(X_i, x_i)\rightarrow \pi_1(X, x)$ là một đẳng cấu.

Nhận xét 1 của IV, p. 429 và Bài tập 3, IV, p. 463 cho những điều kiện ít chặt hơn để đồng cấu này là một đẳng cấu. Tuy vậy, xem Bài tập 4, IV, p. 464.

### 3. Trường hợp riêng của một phủ gồm hai phần

Cho X là một không gian tôpô liên thông bằng đường, và cho B và C là các tập con không rỗng liên thông bằng đường của X. Giả sử thêm một trong hai giả thuyết sau đây:

(i) Các phần trong của các tập hợp B và C phủ X;

(ii) Các tập hợp B và C đóng trong X, hợp của chúng bằng X, các không gian X, B, C là đơn liên, và không gian $B\cap C$ là địa phương liên thông bằng đường.

Dưới các giả thuyết này, ánh xạ chính tắc từ không gian tổng của họ $(B,C)$ lên không gian X thỏa mãn tính chất (VK) (x. IV, p. 409).

Đặt $A = B\cap C$. Vì không gian X liên thông, tập hợp A là không rỗng. Cho $a$ là một điểm của A; gọi $j_0$ là thành phần liên thông bằng đường của $a$ trong A. Với mỗi thành phần liên thông bằng đường $j$ của A khác $j_0$, chọn một điểm $a_j$ của $j$, lớp $\beta_j$ của một đường trong B và lớp $\gamma_j$ của một đường trong C, cả hai đều nối $a_j$ với $a$; gọi $\varphi_j:\pi_1(A, a_j)\rightarrow \pi_1(B, a)$ và $\psi_j:\pi_1(A, a_j)\rightarrow \pi_1(C, a)$ là các đồng cấu nhóm được xác định bởi

$\varphi_j(v) =\beta_j^{-1}v\beta_j$ và $\psi_j(v) =\gamma_j^{-1}v\gamma_j$

với $v\in \pi_1(A, a_j)$. Gọi $\varphi_0$ và $\psi_0$ cũng là các đồng cấu từ $\pi_1(A, a)$ vào $\pi_1(B, a)$ và $\pi_1(C, a)$ tương ứng, cảm sinh bởi các phép chèn chính tắc. Gọi $\iota_B$ và $\iota_C$ là các đồng cấu từ $\pi_1(B, a)$ và $\pi_1(C, a)$ tương ứng vào $\pi_1(X, a)$, cảm sinh bởi các phép chèn chính tắc. Sau cùng, gọi $\mu$ là đồng cấu duy nhất từ nhóm tự do $F(\pi_0(A)-\{j_0\})$ vào $\pi_1(X, a)$ sao cho $\mu(j) =\beta_j^{-1}\gamma_j$ với mọi $j\in \pi_0(A)-\{j_0\}$.

#### Mệnh đề 2 {#ta-iv-s5-prop-2 .statement tag=023D}

Tồn tại một đồng cấu nhóm duy nhất

$$
\mathsf{M}:\pi_1(B, a)*\pi_1(C, a)*F(\pi_0(A)-\{j_0\})\rightarrow \pi_1(X, a)
$$

trùng với $\iota_B$ trong $\pi_1(B, a)$, với $\iota_C$ trong $\pi_1(C, a)$ và với $\mu$ trong $F(\pi_0(A)$ $\{j_0\})$. Đồng cấu này là toàn ánh và hạt nhân của nó là nhóm con chuẩn tắc nhỏ nhất chứa các phần tử

$$
\varphi_j(v)j\psi_j(v)^{-1}j^{-1}
$$

với $j\in \pi_0(A)-\{j_0\}$ và $v\in \pi_1(A, a_j)$, và các phần tử

$$
\varphi_0(v)\psi_0(v)^{-1}
$$

với $v\in \pi_1(A, a)$.

Khung Γ của phủ của X xác định bởi họ $(B,C)$ có hai đỉnh $b$ và $c$ tương ứng với hai tập hợp B và C. Tập hợp các mũi tên của nó bằng $\pi_0(A)$; chúng nối điểm $b$ với điểm $c$. Đồ thị liên kết với đồ thị có hướng con của Γ mà mũi tên duy nhất là $j_0$ là một cây cực đại của $\widetilde{\Gamma}$. Khi đó mệnh đề suy ra từ IV, p. 412, mệnh đề 1.

#### Ví dụ {#ta-iv-s5-n3-exa-1 .statement tag=023E}

Với $n\geqslant 1$, mặt cầu $\mathbf{S}_n$ là hợp của hai bán cầu đóng, đồng phôi với quả cầu đóng $\mathbf{B}_{n-1}$ (TG, VI, p. 12), và có giao được đồng nhất với mặt cầu $\mathbf{S}_{n-1}$. Với $n\geqslant 2$, mặt cầu $\mathbf{S}_{n-1}$ liên thông từng cung; suy ra nhóm Poincaré của $\mathbf{S}_n$ là tầm thường (xem I, p. 127, ví dụ 3).

Mặt cầu $\mathbf{S}_0$ có hai thành phần liên thông từng cung; do đó ta thu lại được rằng nhóm Poincaré của đường tròn $\mathbf{S}_1$ đẳng cấu với một nhóm tự do trên một phần tử sinh. Chính xác hơn, gọi B và C là các giao của $\mathbf{S}_1$ với các nửa mặt phẳng có phương trình $y\geqslant 0$ và $y\leqslant 0$ trong mặt phẳng $\mathbf{R}^2$. Đặt $a= (1,0),a'= (-1,0)$; ta có $B\cap C =\{a, a'\}$; các thành phần liên thông của nó là $j_0=\{a\}$ và $j=\{a'\}$. Gọi $\beta$ là lớp của đường đi $t\mapsto e^{\pi it}$ trong $\mathbf{C}$; nếu đồng nhất $\mathbf{C}$ với $\mathbf{R}^2$, nó nối $a$ với $a'$ trong B. Tương tự, gọi $\gamma$ là lớp của đường đi $t\mapsto e^{-\pi it}$ nối $a$ với $a'$ trong C. Đường đi $\beta \gamma^{-1}$ là một vòng tại $a$, cho bởi $t\mapsto e^{2\pi it}$. Theo mệnh đề 2, lớp của nó sinh ra nhóm $\pi_1(\mathbf{S}_1, a)$.

#### Hệ quả 1 {#ta-iv-s5-prop-2-cor-1 .statement tag=023F}

Đồng cấu $\mu$ là đơn ánh. Chính xác hơn, tồn tại một phép co rút liên kết với $\mu$ là một đồng cấu nhóm.

Cho $\rho$ là đồng cấu duy nhất từ $\pi_1(B, a)*\pi_1(C, a)*F(\pi_0(A)$ $\{j_0\})$ vào $F(\pi_0(A)$ - $\{j_0\})$ cảm sinh đồng cấu tầm thường trên $\pi_1(B, a)$ và $\pi_1(C, a)$ và đồng nhất trên $F(\pi_0(A)-\{j_0\})$. Gọi N là hạt nhân của đồng cấu $\mathsf{M}$. Theo mệnh đề $2,\rho (N)$ thu về phần tử đơn vị. Do đó tồn tại một đồng cấu duy nhất $\mathsf{r}$ từ $\pi_1(X, a)$ vào $F(\pi_0(A)-\{j_0\})$ sao cho $\rho =\mathsf{r}\circ \mathsf{M}$. Với mọi $v\in F(\pi_0(A)-\{j_0\})$, ta có $\mathsf{M}(v) =\mu(v)$, nên $\mathsf{r}\circ \mu$ là đồng cấu đồng nhất. Hệ quả được suy ra.

#### Hệ quả 2 {#ta-iv-s5-prop-2-cor-2 .statement tag=023G}

Nếu nhóm $\pi_1(X, a)$ là tầm thường, tập hợp A = $B\cap C$ liên thông bằng cung; nếu nó giao hoán, tập hợp A có nhiều nhất hai thành phần liên thông bằng cung.

Thật vậy, nếu S là một tập hợp, nhóm tự do F(S) chỉ tầm thường khi S rỗng và chỉ giao hoán khi Card $S\leqslant 1$.

#### Hệ quả 3 {#ta-iv-s5-prop-2-cor-3 .statement tag=023H}

Nếu các nhóm $\pi_1(X, a)$ và $\pi_1(A, a)$ là tầm thường, thì điều tương tự cũng đúng với các nhóm $\pi_1(B, a)$ và $\pi_1(C, a)$.

Theo hệ quả 2, tập hợp A liên thông bằng cung. Do đó nhóm $\pi_1(X, a)$ đẳng cấu với tích tự do của các nhóm $\pi_1(B, a)$ và $\pi_1(C, a)$. Đặc biệt nó chứa các nhóm con đẳng cấu với các nhóm $\pi_1(B, a)$ và $\pi_1(C, a)$ (A, I, p. 83). Vậy hai nhóm này là tầm thường nếu $\pi_1(X, a)$ là tầm thường.

### 4. Không gian thương

Cho X là một không gian tôpô liên thông bằng cung được trang bị một phép toán (phải) thực sự của một nhóm rời rạc G. Đặt $Y = X/G$ và ký hiệu bởi $f: X\rightarrow Y$ ánh xạ chính tắc. Nếu $g\in G$ và $c:\mathbf{I}\rightarrow X$ là một đường trong X, gọi $g^*c$ là đường $t\mapsto c(t)\cdot g$ và $g^*[c]$ là lớp đồng luân ngặt của nó.

Gọi $o$ là một điểm của X. Với mỗi $g\in G$, gọi $\beta_g$ là lớp của một đường nối $o\cdot g$ với $o$ trong X. Với mỗi $g\in G$, gọi $X^g$ là tập hợp các điểm $x\in X$ sao cho $x\cdot g=x$; với mỗi thành phần liên thông bằng cung $j$ của $X^g$, gọi $a_j$ là một điểm của $j$ và gọi $\gamma_j$ là lớp của một đường trong X nối $a_j$ với $o$. Gọi $\nu : F(G)\rightarrow \pi_1(Y, f(o))$ là đồng cấu nhóm duy nhất sao cho $\nu (g) =f_*(\beta_g)$ với $g\in G$. Gọi $\mathsf{N}:\pi_1(X, o)*F(G)\rightarrow \pi_1(Y, f(o))$ là đồng cấu nhóm duy nhất trùng với $\pi_1(f, o)$ trên $\pi_1(X, o)$ và với $\nu$ trên F(G).

#### Mệnh đề 3 {#ta-iv-s5-prop-3 .statement tag=023I}

Giả sử rằng X là tháo được. Khi đó đồng cấu $\mathsf{N}$ là toàn ánh, và hạt nhân của nó là nhóm con bất biến nhỏ nhất của $\pi_1(X, o)*F(G)$ chứa các phần tử

($R_2$)$r_2(k, v) = [k]^{-1}v[k](\beta_k^{-1}k^*(v)^{-1}\beta_k)$

với $k\in G$ và $v\in \pi_1(X, o)$;

($R'_3$)$r'_3(k, j) = [k](\beta_k^{-1}k^*(\gamma_j)^{-1}\gamma_j)$

với $k\in G$ và $j\in \pi_0(X^k)$;

($R''_3$)$r''_3(k, h) = [kh]^{-1}[k][h](\beta_h^{-1}h^*(\beta_k^{-1})\beta_{kh})$

với $k$ và $h\in G$.

Cấu xạ groupoid $\varpi (f)$ cảm sinh một cấu xạ

$$
\varpi ''(f):\varpi (X)/G\rightarrow \varpi (Y)
$$

là một đẳng cấu theo Định lý 3 (IV, p. 403), vì không gian X được giả sử là tháo được. Khi đó mệnh đề suy ra từ II, p. 211, mệnh đề 6.

Ba hệ quả dưới đây suy ra từ các hệ quả tương ứng ngay lập tức của mệnh đề 6 ở II, p. 211.

#### Hệ quả 1 {#ta-iv-s5-prop-3-cor-1 .statement tag=023J}

Giả sử rằng X là tháo được và nhóm G được sinh bởi các nhóm ổn định của các điểm của X. Khi đó cấu xạ chính tắc $\pi_1(f, o):\pi_1(X, o)\rightarrow \pi_1(Y, f(o))$ là toàn ánh. Đặc biệt, nếu X đơn liên thông bằng cung, thì Y cũng vậy.

#### Nhận xét {#ta-iv-s5-n4-rem-1 .statement tag=023K}

Nếu X là tháo được, thì Y cũng vậy (IV, p. 349, mệnh đề 8). Vì một không gian liên thông tháo được là đơn liên thông bằng cung khi và chỉ khi nó đơn liên thông (IV, p. 344, hệ quả 1 của Định lý 1), do đó ta thu lại được mệnh đề 11 của I, p. 137.

#### Ví dụ 1 {#ta-iv-s5-n4-exa-1 .statement tag=023L}

Cho X là một không gian tôpô tách biệt, liên thông bằng cung, tháo được, và cho $a$ là một điểm của X. Cho $n$ là một số nguyên $\geqslant 2$ và cho Y là thương của không gian $X^n$ theo tác động của nhóm $\mathfrak{S}_n$ tác động bằng phép hoán vị các thừa số; ký hiệu $f: X^n\rightarrow Y$ là ánh xạ chính tắc; ký hiệu $g: X\rightarrow Y$ là ánh xạ $x\mapsto f(x, a, . . . , a)$. Từ mệnh đề suy ra rằng, với mọi $i$, đồng cấu $\pi_1(g, a)$ từ $\pi_1(X, a)$ vào $\pi_1(Y, g(a))$ là toàn ánh và hạt nhân của nó là nhóm dẫn xuất của $\pi_1(X, a)$. Đặc biệt, nhóm $\pi_1(Y, g(a))$ là Abel.

#### Hệ quả 2 {#ta-iv-s5-prop-3-cor-2 .statement tag=023M}

Giả sử rằng X là tháo được và nhóm G tác động tự do trên X. Tồn tại một đồng cấu nhóm duy nhất $p:\pi_1(Y, f(o))\rightarrow G$ mà hạt nhân của nó chứa ảnh của $\pi_1(X, o)$ và sao cho $p(\mathsf{N}(g)) =g$ với mọi $g\in G$. Hơn nữa, $\pi_1(X, o)\rightarrow \pi_1(Y, f(o))-\overset{p}{\rightarrow}G$ là một mở rộng của G bởi $\pi_1(X, o)$.

#### Hệ quả 3 {#ta-iv-s5-prop-3-cor-3 .statement tag=023N}

Giả sử rằng X đơn liên thông bằng cung. Ánh xạ từ G vào $\pi_1(Y, f(o))$ gán cho $g\in$ G lớp đường đi $f_*(\beta_g)$ là một đồng cấu nhóm toàn ánh; hạt nhân của nó là nhóm con của G được sinh bởi các nhóm ổn định của các điểm của X.

### 5. Các nón; sự co rút của một không gian con

Cho X và Y là các không gian tôpô không rỗng, và cho $f: X\rightarrow Y$ là một ánh xạ liên tục. Gọi Cone$(f)$ là nón của ánh xạ $f$, và gọi $s$ là đỉnh của nó. Ký hiệu $\alpha '_f: X\times \mathbf{I}\rightarrow$ Cone$(f)$ và $\beta '_f: Y\rightarrow$ Cone$(f)$ là các ánh xạ chính tắc. Hạn chế của $\alpha '_f$ lên không gian con $X\times  \{0\}$ của $X\times \mathbf{I}$ là ánh xạ hằng có ảnh là $\{s\}$. Ánh xạ $\beta '_f$ cảm sinh một đồng phôi của Y lên cơ sở của nón Cone$(f)$, nhờ đó ta sẽ đồng nhất hai không gian này. Cũng ký hiệu bởi

$\sigma '_f: ($Cone$(f)-\{s\})\times \mathbf{I}\rightarrow$ Cone$(f)-\{s\}$

sự co rút chính tắc, và bởi $\rho '_f:$ Cone$(f)-\{s\} \rightarrow Y$ phép co rút chính tắc của nón bị tước mất đỉnh của nó lên cơ sở của nó.

Đặt $J =\pi_0(X)$; với mỗi phần tử $j$ của J, ký hiệu $X_j$ là thành phần $j$ của X, ký hiệu $b_j$ là một điểm của $X_j$, và ký hiệu $\gamma_j$ là lớp của đường đi $t\mapsto \alpha '_f(b_j, t)$ trong Côn$(f)$ nối $s$ với $f(b_j)$.

Gọi I là ảnh của ánh xạ $\pi_0(f)$; đó là tập hợp các thành phần liên thông từng cung của Y cắt $f(X)$; ký hiệu $\varphi : J\rightarrow I$ là ánh xạ suy ra từ $f$ bằng cách chuyển qua các thành phần liên thông từng cung. Với mỗi phần tử $i\in I$, ký hiệu $Y_i$ là thành phần $i$ của Y và chọn một điểm $a_i$ trong $Y_i$.

Với mỗi phần tử $j$ của J, chọn một đường đi $B_j$ nối điểm $f(b_j)$ với điểm $a_{\varphi(j)}$ trong $Y_{\varphi(j)}$, và ký hiệu $\beta_j$ là lớp của nó. Ký hiệu $\psi_j$ là đồng cấu từ $\pi_1(X, b_j)$ vào $\pi_1(Y, a_{\varphi(j)})$ được xác định bởi

$$
\psi_j(v) =\beta_j^{-1}f_*(v)\beta_j
$$

với $v\in \pi_1(X, a_j)$.

Gọi $\sigma : I\rightarrow J$ là một tiết diện của ánh xạ $\varphi$. Đặt $T =\sigma (I)$ và $\tau =\sigma \circ \varphi$; nhận thấy rằng $\varphi \circ \tau =\varphi$.

#### Mệnh đề 4 {#ta-iv-s5-prop-4 .statement tag=023O}

Giả sử rằng các thành phần liên thông từng cung của Y là mở. Với mỗi $i\in$ I, gọi $G_i$ là thương của nhóm $\pi_1(Y_i, b_i)$ theo nhóm con chuẩn tắc nhỏ nhất chứa ảnh của các đồng cấu $\psi_j$, với $j\in \overset{-1}{\varphi}(i)$ ; ký hiệu $p_i$ là toàn cấu chính tắc của $\pi_1(Y_i, b_i)$ lên $G_i$.

Tồn tại một đồng cấu nhóm duy nhất

$\mathsf{P}:_i*_{\in I}G_i*F(J-T)\rightarrow \pi_1($Côn$(f), s)$

sao cho

$\mathsf{P}(p_i(v)) =$ Int($\gamma_{\sigma(i)}\beta_{\sigma(i)}$)$(v)$ với $i\in I$ và $v\in \pi_1(Y_i, b_i)$,

$\mathsf{P}(j) =\gamma_j\beta_j\beta_{\tau(j)}^{-1}\gamma_{\tau(j)}^{-1}$ với $j\in J-T$.

Đồng cấu $\mathsf{P}$ là một đẳng cấu.

Gọi $Y'$ là hợp của các thành phần liên thông bằng cung của Y cắt $f(X)$, và gọi $f': X\rightarrow Y'$ là ánh xạ cho bởi $x\mapsto f(x)$. Tập hợp $Y'$ là một tập con mở của Y; các thành phần liên thông bằng cung của nó là mở. Cone$(f')$ được đồng nhất với thành phần liên thông bằng cung của $s$ trong Cone$(f)$. Điều này cho phép giả sử rằng $Y = Y'$, nói cách khác rằng ánh xạ $\pi_0(f)$ là toàn ánh và $I =\pi_0(Y)$.

Với mỗi $j\in J$, đặt $V_j=\alpha '_f(X_j\times ]0,1[)$. Khi chuyển qua các không gian con, ánh xạ $\alpha '_f$ cảm sinh một đồng phôi từ $X\times ]0,1[$ lên phần bù của $Y\cup  \{s\}$ trong Cone$(f)$. Do đó các tập hợp $V_j$ là các thành phần liên thông bằng cung của Cone$(f)-(Y\cup  \{s\})$.

Với mỗi $i\in I$, đặt $U_i= (\rho '_f)^{-1}(Y_i)$; đây là một tập con mở của Cone$(f)$, vì $Y_i$ mở trong Y theo giả thiết. Với mỗi $j\in \overset{-1}{\varphi}(i)$, ta có $f(X_j)\subset Y_i$ và

$$
V_j\cup Y_i=\alpha '_f(X_j\times ]0,1])\cup Y_i
$$

nên $V_j\cup Y_i$ là một tập con liên thông bằng cung của Cone$(f)$ chứa $Y_i$. Vì $U_i$ là hợp của $Y_i$ và của các tập hợp $V_j$, với $j\in \overset{-1}{\varphi}(i)$, suy ra $U_i$ là liên thông bằng cung.

Sau cùng, tập hợp $C'(X) =$ Cone$(f)$ - Y là một tập con mở của Cone$(f)$; nó co rút được về $s$, do đó liên thông bằng cung.

Tập hợp $C'(X)$ và các tập hợp $U_i$, với $i\in I$, lập thành một phủ mở liên thông bằng cung của Cone$(f)$, mà ta sẽ áp dụng mệnh đề 1 của IV, p. 412. Gọi $I'$ là tập hợp thu được bằng cách thêm $s$ vào I; trang bị cho nó một thứ tự toàn phần sao cho $s$ là phần tử nhỏ nhất của nó.

Với các phần tử phân biệt $i, i'$ của I, ta có $U_i\cap U_{i'}=\emptyset$. Với $i\in I$, $C'(X)\cap U_i$ là hợp của các tập hợp $V_j$, với $j\in \overset{-1}{\varphi}(i)$; chúng liên thông và rời nhau từng đôi một. Giao của ba tập hợp phân biệt bất kỳ nào của phủ này là rỗng.

Khung Γ của phủ đang xét có tập hợp $I'$ làm tập đỉnh. Các cạnh của nó là các bộ ba $(s, i,V_j)$, với $j\in J$ và $i=\varphi (j)$; do đó tập hợp các cạnh của Γ sẽ được đồng nhất với tập hợp J.

Với $i\in I$, ta chọn làm điểm cơ sở $\mathsf{a}(i) =a_i\in U_i$; đồng thời cũng đặt $\mathsf{a}(s) =s\in C'(X)$.

Với $j\in$ J, đặt $\mathsf{b}(j) =\alpha '_f(b_j,\frac{1}{2})$. Gọi $B_1(j)$ là đường đi trong $C'(X)$ có gốc $\mathsf{b}(j)$ và điểm cuối $\mathsf{a}(s)$ cho bởi $t\mapsto \alpha '_f(b_j,(1-t)/2)$. Gọi $B_2(j)$ là đường đi trong $U_{\varphi(j)}$ có gốc $\mathsf{b}(j)$ và điểm cuối $\mathsf{a}(\varphi (j)) =a_{\varphi(j)}$, thu được bằng cách ghép nối đường đi $t\mapsto \alpha '_f(b_j,(1 +t)/2)$ và đường đi $B_j$. Khi đó lớp của đường đi $B(j) =\overline{B}_1(j)*B_2(j)$ bằng $\gamma_j\beta_j$.

Ta chọn $i_0=s$.

Ta lấy làm cây có hướng cực đại T cây có hướng duy nhất của Γ mà tập các mũi tên là $\sigma (I)$. Ta có $\delta (s) =e$, còn với $i\in I,\delta (i) = [B(\sigma (i))] =\gamma_{\sigma(i)}\beta_{\sigma(i)}$.

Cho $j\in J$ và đặt $i=\varphi (j)$.

Đồng cấu $\varphi_j$ từ $\pi_1(V_j,\mathsf{b}(j))$ vào $\pi_1(C'(X), s)$ là đồng cấu tầm thường, vì $C'(X)$ co rút được về $s$.

Ánh xạ $\alpha '_f$ cảm sinh một đồng phôi từ $X_j\times ]0,1[$ lên $V_j$; đồng phôi này cảm sinh một đẳng cấu từ nhóm $\pi_1(V_j,\mathsf{b}(j))$ lên nhóm $\pi_1(X_j, b_j) =\pi_1(X, b_j)$. Bằng cách chuyển qua các không gian con, ánh xạ $\sigma '_f$ cảm sinh một phép co mạnh của $U_i$ lên $Y_i$, phép co này cảm sinh một đẳng cấu từ nhóm $\pi_1(U_i,\mathsf{a}(i))$ lên nhóm $\pi_1(Y, a_i)$. Nhờ các đẳng cấu này, đồng cấu

$$
\psi_j:\pi_1(V_j,\mathsf{b}(j))\rightarrow \pi_1(U_{\varphi(j)},\mathsf{a}(\varphi (j)))
$$

được đồng nhất với đồng cấu Int($\beta_{\varphi(j)}^{-1}$)$\circ f_*$ từ $\pi_1(X, b_j)$ vào $\pi_1(Y, a_i)$.

Vì $C'(X)$ co rút được về $s$, đồng cấu $\mu_s$ là đồng cấu tầm thường.

Cho $i\in I$. Đồng cấu $\mu_i$ từ $\pi_1(U_i,\mathsf{a}(i))$ vào $\pi_1($Côn$(f), s)$ được đồng nhất với đồng cấu từ $\pi_1(Y, a_i)$ vào $\pi_1($Côn$(f), s)$ thu được bằng cách hợp thành đồng cấu Int($\delta (i)$) và đồng cấu từ $\pi_1(U_i, s)$ vào $\pi_1($Côn$(f), s)$ suy ra từ đơn ánh chính tắc của $U_i$ vào Côn$(f)$.

Sau cùng, đồng cấu $\mu: F(J)\rightarrow \pi_1($Côn$(f), s)$ được cho bởi

$$
\mu(j) =\gamma_j\beta_j\beta_{\tau(j)}^{-1}\gamma_{\tau(j)}^{-1}
$$

Cho $\mathsf{P}'$ là đồng cấu nhóm duy nhất

$\mathsf{P}':_i*_{\in I}\pi_1(Y_i, a_i)*F(J)\rightarrow \pi_1($Cone$(f), s)$

trùng với đồng cấu Int($\delta (i)^{-1}$) trên $\pi_1(Y_i, a_i)$ và với đồng cấu $\mu$ trên F(J). Theo Mệnh đề 1 của IV, p. 412, đồng cấu $\mathsf{P}'$ là toàn ánh và hạt nhân của nó là nhóm con chuẩn tắc nhỏ nhất của $*_i\pi_1(Y_i, a_i)*F(J)$ chứa các phần tử $\mathsf{r}_1(j)$, với $j\in T$, và các phần tử $\mathsf{r}_2(j, v)$, với $j\in J$ và $v\in \pi_1(V_j,\mathsf{b}(j))$. (Không có các phần tử $\mathsf{r}_3(k)$, vì tập hợp K là rỗng.)

Với $j\in T$, ta có $r_1(j) =j$. Cho $j\in J$ và $v\in \pi_1(V_j,\mathsf{b}(j))$. Theo sự đồng nhất $\pi_1(V_j,\mathsf{b}(j))$ với $\pi_1(X, b_j)$, ta có $\mathsf{r}_2(j, v) =j\psi_j(v)j^{-1}$. Ký hiệu $p$ là đồng cấu toàn ánh chính tắc từ $*\pi_1(Y_i, a_i)*F(J)$ lên $*G_i*F(J$ - T). Với $j\in T$, ta có $p(\mathsf{r}_1(j)) =^ie$; với $j\in J$ và $v\in \pi_1(X^i, b_j)$, ta có $p(\psi_j(v)) =e$. Do đó tồn tại một đồng cấu nhóm duy nhất $\mathsf{P}$ từ $*G_i*F(J-T)$ vào $\pi_1($Cone$(f), s)$ sao cho $\mathsf{P}'\circ p=\mathsf{P}$; nó là một đẳng cấu.$^i$

#### Hệ quả 1 {#ta-iv-s5-prop-4-cor-1 .statement tag=023P}

Giả sử thêm rằng các không gian X và Y liên thông theo cung và cho $a$ là một điểm của X. Ánh xạ chính tắc từ $\pi_1(Y, f(a))$ vào $\pi_1($Cone$(f), f(a))$ là toàn ánh, và hạt nhân của nó là nhóm con chuẩn tắc nhỏ nhất chứa ảnh của đồng cấu $\pi_1(f, a)$.

#### Hệ quả 2 {#ta-iv-s5-prop-4-cor-2 .statement tag=023Q}

Giả sử thêm rằng các thành phần liên thông theo cung của Y là đơn liên thông theo cung. Khi đó đồng cấu $\mu: F(J-T)\rightarrow \pi_1($Cone$(f), s)$ là một đẳng cấu.

#### Nhận xét 1 {#ta-iv-s5-n5-rem-1 .statement tag=023R}

Cho X là một không gian tôpô mà các thành phần liên thông theo cung của nó là mở. Cho A là một không gian con đóng của X; ký hiệu $\iota : A\rightarrow$ X là đơn ánh chính tắc, ký hiệu $X/A$ là không gian suy ra từ X bằng cách co A thành một điểm $o$, và ký hiệu $p: X\rightarrow X/A$ là ánh xạ chính tắc. Giả sử thêm rằng cặp $(X,A)$ có tính chất mở rộng đồng luân. Khi đó ánh xạ chính tắc $\overline{\rho}:$ Cone$(\iota )\rightarrow X/A$ là một tương đương đồng luân (III, p. 255, Nhận xét 1), và từ Mệnh đề 4 suy ra cách tính nhóm Poincaré của $X/A$ tại điểm gốc $o$ của nó. Đặc biệt, nếu các thành phần liên thông theo cung của X là đơn liên thông theo cung, thì nhóm $\pi_1(X/A, o)$ là một nhóm tự do.

### 6. Thổi phồng và dán lại với nhau

Cho C là một không gian tôpô và cho $(B_{\ell})_{\ell\in L}$ là một họ hữu hạn các tập con đóng của C, rời nhau từng đôi một. Cho B là một không gian tôpô và, với mỗi $\ell \in L$, cho $h_{\ell}$ là một đồng phôi của B lên $B_{\ell}$. Ta ký hiệu bởi $B_L$ hợp của họ $(B_{\ell})_{\ell\in L}$. Ta sẽ giả sử rằng B và L đều không rỗng. Cho R là quan hệ tương đương trên C được định nghĩa như sau. Lớp của một phần tử $x$ của $C-B_L$ là tập hợp $\{x\}$; nếu $x$ là một phần tử của $B_{\ell}$, với $\ell \in L$, thì lớp của $x$ là

tập hợp các phần tử $h_k(\overset{-1}{h_{\ell}}(x))$, trong đó $k$ chạy qua L. Cho A là không gian tôpô thương $C/R$ và $f: C\rightarrow A$ là toàn cấu chính tắc. Người ta nói rằng không gian A thu được từ không gian C bằng cách đồng nhất các tập hợp $B_{\ell}$ nhờ các đồng phôi $h_{\ell}$.

Ánh xạ $f\circ h_{\ell}$ của B vào A là độc lập với phần tử $\ell$ của L; nó là đóng và đơn ánh; do đó nó cảm sinh một đồng phôi của B lên một tập con đóng của A. Vì thế ta đồng nhất B với $f\circ h_{\ell}(B)$ nhờ đồng phôi $f\circ h_{\ell}$; ánh xạ $f$ cảm sinh một đồng phôi của $C-B_L$ lên A-B.

Giả sử thêm rằng tồn tại một họ $(N_{\ell})_{\ell\in L}$ các tập con mở của C, rời nhau từng đôi một, sao cho $N_{\ell}$ chứa $B_{\ell}$ với mỗi $\ell \in L$. Hợp U của họ $(f(N_{\ell}))_{\ell\in L}$ là mở trong A và chứa B. Tập hợp U-B là hợp của các tập hợp mở rời nhau từng đôi một $f(N_{\ell}-B_{\ell})$, với $\ell \in L$.

#### Bổ đề 2 {#ta-iv-s5-lem-2 .statement tag=023S}

Ánh xạ $f: C\rightarrow A$ là riêng và tách biệt; các thớ của nó là hữu hạn.

Ta hãy chứng minh rằng $f$ là đóng. Cho X là một tập con đóng của C. Ta hãy chứng minh rằng ảnh của nó là đóng trong A. Với mỗi $\ell \in L$, $X\cap B_{\ell}$ là đóng trong $B_{\ell}$, do đó không gian $Y =\bigcup_{\ell\in L}h^{-1}_{\ell}(X\cap B_{\ell})$ là đóng trong B vì L là hữu hạn. Bão hòa $X^*$ của X đối với quan hệ tương đương R khi đó bằng $X\cup \bigcup_{\ell\in L}h_k(Y)$, do đó là đóng trong C. Do đó, $f(X) =f(X^*)$ là đóng trong A, điều phải chứng minh.

Các thớ của $f$ là các lớp tương đương của quan hệ R; chúng là hữu hạn. Do đó, ánh xạ $f$ là riêng (TG, I, p. 75, Định lý 1).

Sau cùng, ta hãy chỉ ra rằng $f$ là tách biệt. Cho $x$ và $y$ là các điểm phân biệt của C có cùng ảnh dưới $f$. Do đó tồn tại một điểm $b\in B$ và các phần tử phân biệt $\ell$ và $m\in L$ sao cho $x=h_{\ell}(b)$ và $y=h_m(b)$. Do đó, $N_{\ell}$ và $N_m$ là các lân cận rời nhau của $x$ và $y$ trong C, do đó có mệnh đề cần chứng minh theo Mệnh đề 1 của I, p. 25.

Giả sử thêm các giả thiết sau đây:

– không gian A là đơn liên và liên thông;

– không gian C là đơn liên;

– không gian B là liên thông và địa phương liên thông từng cung.

Đặt $I =\pi_0(C)$; nếu $i$ là một phần tử của I, ký hiệu $C_i$ là thành phần liên thông $i$ của C. Ký hiệu $\eta : L\rightarrow I$ là ánh xạ gán cho một phần tử $\ell \in L$ thành phần liên thông của C chứa $B_{\ell}$. Ánh xạ $\eta$ là toàn ánh. Thật vậy, lập luận phản chứng, xét một thành phần liên thông X của C không gặp tập nào $B_{\ell}$. Đó là một tập con vừa mở vừa đóng của C, bão hòa đối với quan hệ tương đương R. Do đó ảnh của nó $f(X)$ là một tập con vừa mở vừa đóng của A, rời nhau với B. Vì A được giả thiết là liên thông và B khác rỗng, $f(X)$ là rỗng, do đó dẫn đến mâu thuẫn.

Lấy $\sigma : I\rightarrow L$ là một tiết diện của ánh xạ $\eta$; đặt $\tau =\sigma \circ \eta$ và $T =\sigma (I)$.

Chọn một điểm $b$ của B. Với mọi $\ell \in L$, đặt $b_{\ell}=h_{\ell}(b)$ và chọn lớp $\beta_{\ell}$ của một đường đi nối $b_{\ell}$ với $b_{\tau(\ell)}$ trong C; nếu $\ell =\tau (\ell )$, lấy $\beta_{\ell}$ là lớp của đường đi hằng có ảnh là $b_{\ell}$. Với mọi $\ell \in L$, ký hiệu $\vartheta_{\ell}$ là đồng cấu từ $\pi_1(B, b)$ vào $\pi_1(C, b_{\tau(\ell)})$ được xác định bởi

$\vartheta_{\ell}(v) =$ Int($\beta_{\ell}$)$^{-1}((h_{\ell})_*(v)) =\beta_{\ell}^{-1}(h_{\ell})_*(v)\beta_{\ell}$,

với mọi $v\in \pi_1(B, b)$. Sau cùng, cố định một phần tử $\ell_0$ của L sao cho $\ell_0=$ $\tau (\ell_0)$.

Gọi $\mathsf{Q}$ là đồng cấu nhóm duy nhất

$$
\mathsf{Q}:(_i*_{\in I}\pi_1(C_i, b_{\sigma(i)}))*F(L-T)\rightarrow \pi_1(A, b)
$$

sao cho $\mathsf{Q}(\ell ) =f_*(\beta_{\ell})$ với mọi $\ell \in$ L - T và trùng với $\pi_1(f, b_{\sigma(i)})$ trên $\pi_1(C_i, b_{\sigma(i)})$ với mọi $i\in I$.

#### Mệnh đề 5 (Van Kampen) {#ta-iv-s5-prop-5 .statement tag=023T}

Đồng cấu $\mathsf{Q}$ là toàn ánh; hạt nhân của nó là nhóm con chuẩn tắc nhỏ nhất chứa các phần tử

$\vartheta_{\ell_0}(v)\vartheta_{\ell}(v)^{-1}$ với $v\in \pi_1(B, b)$ và $\ell \in T$,

$\vartheta_{\ell_0}(v)\ell \vartheta_{\ell}(v)^{-1}\ell^{-1}$ với $v\in \pi_1(B, b)$ và $\ell \in L-T$.

Ánh xạ $f: C\rightarrow$ A là thực sự, tách biệt, có các thớ hữu hạn (IV, p. 430, bổ đề 2); các không gian A và C là tháo được. Hơn nữa, $C\times_AC$ là hợp của đường chéo $\Delta_C$ và của các tập con rời nhau $B_{\ell}\times_AB_k=$ $(h_{\ell}, h_k)(B)$, với $(\ell , k)\in L^2$ sao cho $\ell =\not k$. Với một cặp như vậy $(\ell , k)$, ta có $B_{\ell}\times_AB_k= N_{\ell}\times_AN_k$; do đó tập con này vừa mở vừa đóng trong $C\times_AC$. Vì thế đường chéo $\Delta_C$ là mở, và phần bù của nó trong $C\times_AC$, là một hợp hữu hạn của các tập con rời nhau đồng phôi với B, thì liên thông địa phương. Điều này chứng minh rằng ánh xạ $f$ thỏa mãn tính chất (VK) (trường hợp (ii) của IV, p. 405). Để áp dụng định lý 1 của IV, p. 408, chúng ta sẽ định nghĩa các dữ kiện van Kampen cho $f$.

Với mỗi $i\in I$, hãy chọn làm điểm cơ sở trong $C_i$ điểm $\mathsf{a}(i) =$ $b_{\sigma(i)}$.

Gọi J là tập hợp các thành phần liên thông bằng đường đi của $C\times_AC$. Các tập $\Delta_{C_i}$, với $i\in I$, là các thành phần liên thông của đường chéo $\Delta_C$, vốn vừa mở vừa đóng trong $C\times_AC$, do đó các tập này thuộc J. Tương tự, các tập $[\ell_1, \ell_2] = B_{\ell_1}\times_A$ $B_{\ell_2}$ với $\ell_1$ và $\ell_2$ trong L sao cho $\ell_1=\not\ell_2$, thuộc J. Vì các tập này tạo thành một phân hoạch của $C\times_AC$, chúng mô tả tập hợp J.

Cho $j$ là một phần tử của J có dạng $\Delta_{C_i}$, với $i\in I$. Hãy chọn làm điểm cơ sở $\mathsf{b}(j)$ điểm $(\mathsf{a}(i),\mathsf{a}(i)) = (b_{\sigma(i)}, b_{\sigma(i)})$ và lấy cho các lớp đường đi $\beta_1(j)$ và $\beta_2(j)$ lớp của đường đi hằng tại $b_{\sigma(i)}$. Cho $j$ là một phần tử của J có dạng $[\ell_1, \ell_2]$, trong đó $\ell_1$ và $\ell_2$ là các phần tử phân biệt của L. Khi đó đặt $\mathsf{b}([\ell_1, \ell_2]) = (b_{\ell_1}, b_{\ell_2}),\beta_1([\ell_1, \ell_2]) =\beta_{\ell_1}$ và $\beta_2([\ell_1, \ell_2]) =\beta_{\ell_2}$.

Gọi $K =\pi_0(C\times_AC\times_AC)$.

Ký hiệu $\Delta '_C$ là đường chéo của không gian $C\times_AC\times_AC$; đây là một tập con đóng của $C\times_AC\times_AC$, vì $f$ là tách được, và nó đồng phôi với C. Với mọi $i\in$ I, cũng ký hiệu $\Delta '_{C_i}$ là ảnh của $C_i$ dưới ánh xạ đường chéo của C vào $C\times_AC\times_AC$; đó là các tập con vừa mở vừa đóng của $\Delta '_C$. Với mọi bộ ba $(\ell_1, \ell_2, \ell_3)$ gồm các phần tử của L, cũng đặt $[\ell_1, \ell_2, \ell_3] = B_{\ell_1}\times_AB_{\ell_2}\times_AB_{\ell_3}$; đó là các tập con đóng của $C\times_A$ $C\times_AC$, đồng phôi với B. Nếu tập hợp $\{\ell_1, \ell_2, \ell_3\}$ có ít nhất hai phần tử, ta có $[\ell_1, \ell_2, \ell_3] = N_{\ell_1}\times_AN_{\ell_2}\times_AN_{\ell_3}$, điều này suy ra $[\ell_1, \ell_2, \ell_3]$ cũng mở trong $C\times_AC\times_AC$. Hơn nữa, $C\times_AC\times_AC$ là hợp của các tập con rời nhau từng đôi một $\Delta '_C$ và $[\ell_1, \ell_2, \ell_3]$, trong đó $(\ell_1, \ell_2, \ell_3)$ chạy qua tập hợp các bộ ba phần tử của L không đồng thời bằng cùng một phần tử. Do đó, $\Delta_{C'}$, rồi các $\Delta '_{C_i}$, với $i\in I$, đều vừa mở vừa đóng trong $C\times_AC\times_AC$. Điều này kéo theo tập hợp K các thành phần liên thông của không gian này là hợp của hai tập hợp rời nhau sau đây $K_0$ và $K_1$.

Tập hợp $K_0$ là tập hợp các thành phần có dạng $\Delta '_{C_i}$. Cho $i\in I$ và đặt $k= \Delta '_{C_i}$. Đặt $\mathsf{c}(k) = (b_{\sigma(i)}, b_{\sigma(i)}, b_{\sigma(i)})$. Với $(s, t)\in  \{(1,2),(2,3),(1,3)\}$, chọn cho $\gamma_{st}(k)$ lớp của đường đi hằng tại $(b_{\sigma(i)}, b_{\sigma(i)})$.

Tập hợp $K_1$ gồm các thành phần có dạng $k$ = $[\ell_1, \ell_2, \ell_3]$, trong đó $\ell_1, \ell_2, \ell_3$ là ba phần tử của B sao cho tập hợp $\{\ell_1, \ell_2, \ell_3\}$ có lực lượng $\geqslant 2$. Đặt $\mathsf{c}(k) = (b_{\ell_1}, b_{\ell_2}, b_{\ell_3})$. Cho $(s, t)\in  \{(1,2),(1,3),(2,3)\}$. Nếu $\ell_s=\ell_t$, lấy cho $\gamma_{st}(k)$ lớp $(\beta_{\ell_s}, \beta_{\ell_t})$; nếu $\ell_s=\not\ell_t$, lấy cho $\gamma_{st}(k)$ lớp của đường đi hằng tại $(b_{\ell_s}, b_{\ell_t})$.

Khi đó người ta kiểm tra được rằng, với mọi $k\in K$ và với mọi $s\in  \{1,2,3\}$, lớp các vòng $\lambda_s(k)$ được xác định bởi quan hệ (2) của IV, p. 407, là tầm thường.

Khung $\mathsf{\Gamma}$ của cặp cấu xạ groupoid $(\varpi (p_1), \varpi (p_2))$ từ $\varpi (C\times_AC)$ vào $\varpi (C)$ có tập đỉnh là I và tập cạnh có hướng là J. Nếu $i\in I$, mũi tên $j= \Delta_{C_i}$ có gốc và ngọn là $i$; nếu $(\ell_1, \ell_2)$ là một cặp phần tử phân biệt của L, mũi tên $j= [\ell_1, \ell_2]$ có gốc là $\eta (\ell_1)$ và ngọn là $\eta (\ell_2)$.

Gọi $\mathsf{T}$ là tiểu quiver của $\mathsf{\Gamma}$ mà tập đỉnh là I và các mũi tên là những mũi tên dạng $[\ell_0, \ell ]$, với $\ell \in T-\{\ell_0\}$. Đồ thị liên kết với $\mathsf{T}$ là một cây cực đại của $\widetilde{\mathsf{\Gamma }}$.

Đặt $i_0=\eta (\ell_0)$.

Nếu $i\in I-\{i_0\}$, đường đi duy nhất trong $\mathsf{T}$ nối $i_0$ với $i$ là $(i_0,[\ell_0, \sigma (i)], i)$. Cấu xạ groupoid từ Grp($\mathsf{\Gamma}$) vào $\varpi (Y)$ được định nghĩa ở p. 407 (và được ký hiệu bởi $\tau$ loc. cit.) gửi $j$ lên phần tử đơn vị nếu $j= \Delta_{C_i}$, với $i\in I$, và gửi $j= [\ell_1, \ell_2]$ lên $f_*(\beta_{\ell_1})^{-1}f_*(\beta_{\ell_2})$, nếu $\ell_1$ và $\ell_2$ là các phần tử phân biệt của L. Với mọi $i\in I$, lớp đường đi $\delta_i$ được định nghĩa loc. cit. và nối $b=f(b_{\sigma(i_0)})$ với $b=f(b_{\sigma(i)})$ được cho bởi

$$
\delta_i=f_*(\beta_{\ell_0})^{-1}f_*(\beta_{\sigma(i)}) =e
$$

vì $\beta_{\ell}=e$ nếu $\ell \in T$.

Như vậy một dữ liệu van Kampen của ánh xạ $f$ đã được xác định. Khi đó xét đồng cấu nhóm duy nhất

$$
\mathsf{Q}':(_i*_{\in I}\pi_1(C_i, b_{\sigma(i)}))*F(J)\rightarrow \pi_1(A, b)
$$

trùng với $\pi_1(f, b_{\sigma(i)})$ trên $\pi_1(C, b_{\sigma(i)})$ và sao cho

$$
\mathsf{Q}'(j) =f_*(\beta_1(j))^{-1}f_*(\beta_2(j))
$$

với $j\in J$. Theo IV, p. 408, Định lý 1, đồng cấu này là toàn ánh và hạt nhân của nó là nhóm con chuẩn nhỏ nhất chứa các hệ thức $\mathsf{r}_1(j)$ (với $j\in$ Fl($\mathsf{T}$)), $\mathsf{r}_2(j, v)$ (với $j\in$ J và $v\in$ $\pi_1(C\times_AC,\mathsf{b}(j))$) và $\mathsf{r}_3(k)$ (với $k\in K$) được định nghĩa, loc. cit., bởi các phương trình ($R_1$)$, (R_2)$ và ($R_3$).

Gọi $q'$ là đồng cấu duy nhất của F(L) vào F(L - T) sao cho $q'(\ell ) =\ell$ nếu $\ell \in L-T$ và $q'(\ell ) =e$ nếu không. Gọi

$$
q:(_i*_{\in I}\pi_1(C_i, b_{\sigma(i)}))*F(J)\rightarrow (_i*_{\in I}\pi_1(C_i, b_{\sigma(i)}))*F(L-T)
$$

là đồng cấu nhóm duy nhất trùng với đồng nhất trên $\pi_1(C_i, b_{\sigma(i)})$, với $i\in$ I và sao cho ta có $q(j) =e$ nếu $j= \Delta_{C_i}$, $q([\ell , \ell ']) =q'(\ell )^{-1}q'(\ell ')$ nếu $\ell$ và $\ell '$ là những phần tử phân biệt của L. Đồng cấu $q$ là toàn ánh.

Nếu $i\in I$ và $j= \Delta_{C_i}$, ta có $\mathsf{Q}'(j) =e_b=\mathsf{Q}'(q(j))$. Nếu $j= [\ell , \ell ']$, với $\ell$ và $\ell '$ thuộc L, phân biệt, ta có

$$
\mathsf{Q}'(j) =f_*(\beta_{\ell})^{-1}f_*(\beta_{\ell'}) =\mathsf{Q}(q'(\ell ))^{-1}\mathsf{Q}(q'(\ell '))
$$

$$
=\mathsf{Q}(q'(\ell )^{-1}q'(\ell ')) =\mathsf{Q}\circ q([\ell , \ell '])
$$

Vì vậy, $\mathsf{Q}'$ = $\mathsf{Q}\circ q$. Suy ra đồng cấu $\mathsf{Q}$ là toàn ánh và hạt nhân của nó là nhóm con chuẩn nhỏ nhất của $(_i*_{\in I}\pi_1(C_i, b_{\sigma(i)}))*F(L-T)$ chứa các ảnh dưới $q$ của các relator $\mathsf{r}_1(j)$ (với $j\in$ Fl($\mathsf{T}$))$,\mathsf{r}_2(j, v)$ (với $j\in J$ và $v\in \pi_1(C\times_AC,\mathsf{b}(j))$) và $\mathsf{r}_3(k)$ (với $k\in K$).

Nếu $\ell \in T-\{\ell_0\}$ và $j= [\ell_0, \ell ]$, ta có $\mathsf{r}_1(j) =j$ và $q(\mathsf{r}_1(j)) =e$.

Gọi $k\in K$. Ta có $\mathsf{r}_3(k) =j_{12}(k)j_{23}(k)j_{13}(k)^{-1}$. Nếu $k= \Delta '_{C_i}$, với $i\in I$, đặt $j= \Delta_{C_i}$; khi đó ta có

$$
q(\mathsf{r}_3(k)) =q(jjj^{-1}) =q(j) =e
$$

Gọi $\ell$ và $\ell '$ là những phần tử phân biệt của L. Nếu $k= [\ell , \ell , \ell ']$, do đó ta có

$$
q(\mathsf{r}_3(k)) =q(\Delta_{C_{\eta(\ell)}}[\ell , \ell '][\ell , \ell ']^{-1}) =q(\Delta_{C_{\eta(\ell)}}) =e
$$

Nếu $k= [\ell , \ell ', \ell ]$, ta được

$$
q(\mathsf{r}_3(k)) =q([\ell , \ell '][\ell ', \ell ]\Delta^{-1_{(\ell)}}_{C_{\eta}})
$$

$$
=q'(\ell )^{-1}q'(\ell ')q'(\ell ')^{-1}q'(\ell )q(\Delta_{C_{\eta}(\ell)})^{-1}=e
$$

Hơn nữa, nếu $k= [\ell ', \ell , \ell ]$, ta có

$$
q(\mathsf{r}_3(k)) =q([\ell ', \ell ]\Delta_{C_{\eta(\ell)}}[\ell ', \ell ]^{-1})
$$

$$
=q(\ell ')^{-1}q(\ell )q(\Delta_{C_{\eta(\ell)}})q(\ell )^{-1}q(\ell ') =e
$$

Cuối cùng, nếu $k= [\ell_1, \ell_2, \ell_3]$, trong đó $\ell_1, \ell_2, \ell_3$ là những phần tử của L phân biệt từng đôi một, ta có

$$
q(\mathsf{r}_3(k)) =q([\ell_1, \ell_2])q([\ell_2, \ell_3])q([\ell_1, \ell_3])^{-1}=e
$$

Cho $i\in I$ và đặt $j= \Delta_{C_i}$. Các đồng cấu nhóm $\varphi_j$ và $\psi_j$, từ $\pi_1(C\times_AC,\mathsf{b}(j)) =\pi_1(C_i,\mathsf{a}(i))$ vào $\pi_1(C,\mathsf{a}(i))$ được xác định bởi các hệ thức (1) của IV, p. 407, lần lượt bằng $(p_1)_*$ và $(p_2)_*$. Khi đó, với $v\in \pi_1(C_i,\mathsf{a}(i)),\mathsf{r}_2(j, v) =vjv^{-1}j^{-1}$, do đó $q(\mathsf{r}_2(j, v)) =e$.

Cuối cùng, đặt $j= [\ell , \ell ']$, trong đó $\ell$ và $\ell '$ là các phần tử phân biệt của L. Đồng cấu nhóm $\varphi_j:\pi_1(B_{\ell}\times_AB_{\ell'},\mathsf{b}(j))\rightarrow \pi_1(C_{\eta(\ell)}, b_{\tau(\ell)})$ được xác định ở chỗ đã dẫn là đồng cấu $\vartheta_{\ell}$, và đồng cấu $\psi_j$ là đồng cấu $\vartheta_{\ell'}$. Khi đó, với $v\in \pi_1(B_{\ell}\times_AB_{\ell'},\mathsf{b}(j))$

$$
q(\mathsf{r}_2(j, v)) =\vartheta_{\ell}(v)q'(\ell )^{-1}q'(\ell ')\vartheta_{\ell'}(v)^{-1}q'(\ell ')^{-1}q'(\ell )
$$

Hãy phân biệt bốn trường hợp. Nếu $\ell$ và $\ell '$ đều thuộc T, ta có

$$
q(\mathsf{r}_2(j, v)) =(\vartheta_{\ell_0}(v)\vartheta_{\ell}(v)^{-1})^{-1}(\vartheta_{\ell_0}(v)\vartheta_{\ell'}(v)^{-1})
$$

Khi $\ell '=\ell_0$, ta được nghịch đảo của phần tử $\vartheta_{\ell_0}(v)\vartheta_{\ell}(v)^{-1}$. Nếu $\ell \in T$ nhưng $\ell '\notin T$, ta có

$$
q(\mathsf{r}_2(j, v)) =\vartheta_{\ell}(v)\ell '\vartheta_{\ell'}(v)^{-1}(\ell ')^{-1}
$$

$$
=(\vartheta_{\ell_0}(v)\vartheta_{\ell}(v)^{-1})^{-1}\vartheta_{\ell_0}(v)\ell '\vartheta_{\ell'}(v)^{-1}(\ell ')^{-1}
$$

Tương tự, nếu $\ell \notin T$ và $\ell '\in T$, ta có

$$
q(\mathsf{r}_2(j, v)) =\vartheta_{\ell}(v)\ell^{-1}\vartheta_{\ell'}(v)^{-1}\ell
$$

$$
=\ell^{-1}(\vartheta_{\ell_0}(v)\ell \vartheta_{\ell}(v)^{-1}\ell^{-1})^{-1}(\vartheta_{\ell_0}(v)\vartheta_{\ell'}(v)^{-1})\ell
$$

Lấy $\ell '=\ell_0$, ta được một phần tử liên hợp với nghịch đảo của $\vartheta_{\ell_0}(v)\ell \vartheta_{\ell}(v)^{-1}\ell^{-1}$. Cuối cùng, nếu cả $\ell$ lẫn $\ell '$ đều không thuộc T, ta có

$$
q(\mathsf{r}_2(j, v)) =(\vartheta_{\ell}(v)\ell^{-1}\vartheta_{\ell_0}(v)^{-1}\ell )\ell^{-1}(\vartheta_{\ell_0}(v)\ell '\vartheta_{\ell'}(v)^{-1}(\ell ')^{-1})\ell
$$

Các hệ thức này chứng minh, một mặt, rằng các phần tử được nêu trong mệnh đề thuộc hạt nhân của đồng cấu $\mathsf{Q}$, và, mặt khác, rằng tất cả các phần tử $q(\mathsf{r}_2(j, v))$ này đều thuộc nhóm con chuẩn nhỏ nhất chứa các phần tử được nêu trong mệnh đề. Mệnh đề được chứng minh.

#### Nhận xét {#ta-iv-s5-n6-rem-1 .statement tag=023U}

Cho A là một không gian tôpô, B là một tập con đóng của A, và U là một lân cận mở của B trong A. Giả sử tập hợp U-B là hợp của một họ hữu hạn $(M_{\ell})_{\ell\in L}$ các tập mở rời nhau từng đôi một. Với mỗi $\ell \in L$, đặt $N'_{\ell}= M_{\ell}\cup B$. Ký hiệu $C'$ là tổng tôpô của các không gian A-B và $N'_{\ell}$, với $\ell \in L$; ký hiệu thêm $\varphi : A-B\rightarrow C'$ và $\varphi_{\ell}: N'_{\ell}\rightarrow C'$, với $\ell \in L$, là các ánh xạ chính tắc. Gọi C là không gian tôpô thương của $C'$ theo quan hệ tương đương mịn nhất S mà đối với nó các điểm $\varphi (x)$ và $\varphi_{\ell}(x)$ là tương đương, với mỗi $\ell \in L$ và mỗi $x\in M_{\ell}$; gọi $\rho : C'\rightarrow C$ là ánh xạ chính tắc.

Hãy chứng minh rằng không gian A được phục hồi từ không gian C bằng cách đồng nhất các tập $B_{\ell}$ nhờ các đồng phôi $\rho \circ$ $(\varphi_{\ell}|B): B\rightarrow B_{\ell}$.

Với mọi $\ell \in L$, tập hợp $M_{\ell}$ là mở trong A-B và trong $N'_{\ell}$. Các ánh xạ $\rho \circ \varphi$ và $\rho \circ \varphi_{\ell}$ là các đồng phôi của các không gian A-B và $N'_{\ell}$, với $\ell \in L$, lên các tập con mở của C (TG, I, p. 17, Prop. 9). Với mọi $\ell \in L$, tập hợp $\varphi_{\ell}(B)$ là đóng trong $C'$ và bão hòa đối với quan hệ tương đương S. Do đó tập hợp $B_{\ell}=\rho (\varphi_{\ell}(B))$ là đóng trong C và ánh xạ $\rho \circ \varphi_{\ell}$ suy ra một đồng phôi từ B lên $B_{\ell}($loc. cit.). Tương tự, với mọi $\ell \in L$, tập hợp $N_{\ell}=\rho (\varphi_{\ell}(N'_{\ell}))$ là một lân cận mở của $B_{\ell}$; các tập hợp $N_{\ell}$ đôi một rời nhau.

Bằng cách chuyển qua thương, ánh xạ $f': C'\rightarrow A$ suy ra từ các đơn ánh chính tắc vào A của các không gian A-B và $N_{\ell}$, với $\ell \in L$, suy ra một

ánh xạ liên tục $f: C\rightarrow A$. Nếu $x$ là một điểm của B, thớ $\overset{-1}{f}(x)$ là tập hợp các điểm $\rho (\varphi_{\ell}(x))$, với $\ell \in L$. Quan hệ tương đương trên C liên kết với ánh xạ $f$ là quan hệ R được xác định ở đầu số này. Ký hiệu $B_L$ là hợp của họ $(B_{\ell})_{\ell\in L}$. Theo phép dựng, ánh xạ $f$ suy ra một đồng phôi từ $C-B_L$ lên A-B và, với $\ell \in L$, một đồng phôi từ $N'_{\ell}$ lên $N_{\ell}$. Ta sẽ chứng minh rằng ánh xạ $f$ là đóng; khi đó tôpô của A sẽ là tôpô thương của C theo quan hệ tương đương R (I, p. 18, Ví dụ 2). Để làm điều đó, hãy chứng minh rằng nếu F là một tập con của A sao cho $F\cap (A-B)$ là đóng trong A-B và sao cho $F\cap N'_{\ell}$ là đóng trong $N'_{\ell}$, với $\ell \in L$, thì tập hợp F là đóng trong A. Tập hợp U, là hợp của họ $(N'_{\ell})_{\ell\in L}$, là mở trong A và các tập hợp $N'_{\ell}$, với $\ell \in L$, lập thành một phủ đóng hữu hạn của nó. Do đó tập hợp $F\cap U$ là đóng trong U (TG, I, p. 18, Prop. 3). Các tập hợp U và A-B tạo thành một phủ mở của A, vì vậy tập hợp F là đóng trong A (loc. cit.).

## BÀI TẬP {#ta-iv-s5-exercises}

Xem các [bài tập của § 5](exercises/s5/).
