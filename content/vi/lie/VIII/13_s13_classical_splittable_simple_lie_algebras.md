---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VIII
chapter_title: SPLIT SEMI-SIMPLE LIE ALGEBRAS
section: 13
section_title: Classical splittable simple Lie algebras
lang: vi
source: lie-vii-ix
book_pages: 189-218, 266-271
pdf_pages: 0197-0226, 0274-0279
extraction: native+ocr
subsections:
    - "no": 1
      title: ALGEBRAS OF TYPE A$_{\boldsymbol{l}}$ ($\boldsymbol{l}\geq$ 1)
      page: 190
      pdf_page: 198
    - "no": 2
      title: ALGEBRAS OF TYPE B$_{\boldsymbol{l}}$ ($\boldsymbol{l}\geq$ 1)
      page: 195
      pdf_page: 203
    - "no": 3
      title: ALGEBRAS OF TYPE C$_{\boldsymbol{l}}$ ($\boldsymbol{l}\geq$ 1)
      page: 204
      pdf_page: 212
    - "no": 4
      title: ALGEBRAS OF TYPE $\boldsymbol{D}_{\boldsymbol{l}}$ ($\boldsymbol{l}\geq$ 2)
      page: 211
      pdf_page: 219
statements: 2
exercises: 19
content_sha256: d312db12e1d43397642271281fe7d5e8cf65e20ae609c003a10918873d0d0207
translated_from: content/en/lie/VIII/13_s13_classical_splittable_simple_lie_algebras.md
source_content_sha256: 6374fb400438df5a36d2c913925fb0624256c5324de93a908a0b9247182f92f3
translation_model: gpt-5-6-mini, gpt-5-6, gpt-5-mini, gpt-5.4-mini
translation_run: translate-vi-31a72259
glossary_version: 34
glossary_terms_sha256: 734d1eba915bc22fdb5c59df915f2bf445da792cda64fb36f7366e3620b367ff
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 13. CÁC ĐẠI SỐ LIE ĐƠN PHÂN RÃ ĐƯỢC CỔ ĐIỂN

Trong đoạn này, với mỗi kiểu của đại số Lie đơn phân rã được cổ điển, chúng tôi mô tả tường minh:

(I) một đại số thuộc kiểu này, chiều của nó và các đại số con Cartan tách của nó;

(II) các đối nghiệm của nó;

(III) các đại số con Borel và các đại số con parabolic của nó;

(IV) các biểu diễn đơn cơ bản của nó;

(V) những biểu diễn đơn cơ bản của nó là trực giao hoặc symplectic;

(VI) đại số các hàm đa thức bất biến;

(VII) một số tính chất của các nhóm Aut$\mathfrak{g}$, Aut$_0\mathfrak{g}$, Aut$_e\mathfrak{g}$;

(VIII) hạn chế của dạng Killing lên một đại số con Cartan;

(IX) các cấp Chevalley.

### 1. CÁC ĐẠI SỐ KIỂU A$_{\boldsymbol{l}}$ ($\boldsymbol{l}\geq$ 1)

(I) Cho V là một không gian vectơ có chiều $l+ 1$ trên $k$, và cho $\mathfrak{g}$ là đại số $\mathfrak{s}\mathfrak{l}(V)$ gồm các tự đồng cấu của V có vết bằng không. Cho $(e_i)_{1\leq i\leq l+1}$ là một cơ sở của V; ánh xạ gán cho một phần tử của $\mathfrak{g}$ ma trận của nó đối với cơ sở này là một phép đồng nhất $\mathfrak{g}$ với đại số $\mathfrak{s}\mathfrak{l}(l+ 1, k)$ gồm các ma trận có vết bằng không. Ta biết rằng $\mathfrak{g}$ là nửa đơn (Ch. I, §6, no. 7, Mđ. 8).

Nhắc lại (Đại số, Ch. II, §10, no. 3) rằng $E_{ij}$ ký hiệu ma trận $(\alpha_{mp})$ sao cho $\alpha_{ij}= 1$ và $\alpha_{mp}= 0$ với $(m, p)\not= (i, j)$. Các ma trận

$$
E_{ij}(1\leq i, j\leq l+ 1, i\not=j)
$$

$$
E_{i,i}-E_{i+1,i+1}(1\leq i\leq l)
$$

tạo thành một cơ sở của $\mathfrak{g}$. Do đó

dim$\mathfrak{g}=l(l+ 2)$.

Cho $\widehat{\mathfrak{h}}$ là tập hợp các phần tử đường chéo của $\mathfrak{g}\mathfrak{l}(l+ 1, k)$; dãy $(E_{ii})_{1\leq i\leq l+1}$ là một cơ sở của không gian vectơ $\widehat{\mathfrak{h}}$; cho $(\widehat{\varepsilon}_i)_{1\leq i\leq l+1}$ là cơ sở của $\widehat{\mathfrak{h}}^*$ đối ngẫu với $(E_{ii})_{1\leq i\leq l+1}$. Với mọi $h\in \widehat{\mathfrak{h}}$,

$$
[h, E_{ij}] = (\widehat{\varepsilon}_i(h)-\widehat{\varepsilon}_j(h))E_{ij} \tag{1}
$$

theo Ch. I, §1, no. 2, các công thức (5). Cho $\mathfrak{h}$ là tập hợp các phần tử của $\widehat{\mathfrak{h}}$ có vết bằng không, và đặt $\varepsilon_i= \widehat{\varepsilon}_i|\mathfrak{h}$. Khi đó $\mathfrak{h}$ là một đại số con Cartan của $\mathfrak{g}$ (Ch. VII, §2, no. 1, Ví dụ 4). Quan hệ (1) chứng minh rằng đại số con Cartan này là tách, và các nghiệm của $(\mathfrak{g},\mathfrak{h})$ là các $\varepsilon_i-\varepsilon_j(i\not=j)$. Cho $\widehat{\mathfrak{h}}^*_0$ là tập hợp các phần tử của $\widehat{\mathfrak{h}}^*$ mà tổng các tọa độ của chúng đối với $(\widehat{\varepsilon}_i)$ bằng không. Ánh xạ $\lambda  \rightarrow \lambda |\mathfrak{h}$ từ $\widehat{\mathfrak{h}}^*_0$ vào $\mathfrak{h}^*$ là song ánh. Do đó, hệ nghiệm R của $(\mathfrak{g},\mathfrak{h})$ có kiểu $A_l$ (Ch. VI, §4, no. 7). Do đó, $\mathfrak{g}$ là đơn (§3, no. 2, Hệ quả 1 của Mđ. 6). Vậy $\mathfrak{g}$ là một đại số Lie đơn phân rã được kiểu $A_l$.

Mọi đại số con Cartan tách $\mathfrak{h}'$ của $\mathfrak{g}$ đều là một biến đổi của $\mathfrak{h}$ dưới một tự đẳng cấu sơ cấp (§3, no. 3, Hệ quả của Mệnh đề 10). Vì Aut$_e\mathfrak{g}$ là tập hợp các tự đẳng cấu $x \rightarrow sxs^{-1}$ của $\mathfrak{g}$ với $s\in \mathbf{S}\mathbf{L}(V)$ (Chương VII, §3, no. 1, Nhận xét 2; xem thêm (VII)), tồn tại một cơ sở $\beta$ của V sao cho $\mathfrak{h}'$ là tập $\mathfrak{h}_{\beta}$ gồm các phần tử của $\mathfrak{g}$ có ma trận đối với cơ sở $\beta$ là đường chéo. Vì $\mathfrak{h}_{\beta}$ chứa một phần tử có các trị riêng phân biệt, các không gian con vectơ duy nhất của V ổn định dưới các phần tử của $\mathfrak{h}_{\beta}$ là những không gian được sinh bởi một tập con của $\beta$. Suy ra rằng ánh xạ $\beta  \rightarrow \mathfrak{h}_{\beta}$ cảm sinh bởi phép qua thương một song ánh từ tập hợp các phân tích của V thành tổng trực tiếp của $l+ 1$ không gian con có chiều 1 đến tập hợp các đại số con Cartan tách của $\mathfrak{g}$. (II) Cho $\alpha =\varepsilon_i-\varepsilon_j(i\not=j)$ là một nghiệm. Ta có $\mathfrak{g}^{\alpha}=kE_{ij}$. Vì

$$
[E_{ij}, E_{ji}] =E_{ii}-E_{jj}
$$

và vì $\alpha (E_{ii}-E_{jj}) = 2$, ta có (§2, no. 2, Định lý 1 (ii))

$$
H_{\alpha}=E_{ii}-E_{jj}
$$

(III) Đặt $\alpha_1=\varepsilon_1-\varepsilon_2, \alpha_2=\varepsilon_2-\varepsilon_3, . . . , \alpha_l=\varepsilon_l-\varepsilon_{l+1}$. Theo Chương VI, §4, no. $7.I, (\alpha_1, . . . , \alpha_l)$ là một cơ sở B của R; các nghiệm dương đối với B là các $\varepsilon_i-\varepsilon_j$ với $i < j$. Đại số con Borel tương ứng $\mathfrak{b}$ là tập hợp các ma trận tam giác trên có vết bằng không.

Một cờ trong V là một tập hợp các không gian con vectơ của V, khác với $\{0\}$ và V, được sắp thứ tự toàn phần bởi phép bao hàm. Sắp thứ tự tập hợp các cờ của V bởi phép bao hàm. Các cờ cực đại là các tập hợp $\{W_1, . . . ,W_l\}$, trong đó $W_i$ là một không gian con vectơ có chiều $i$ và

$$
W_1\subset  \cdots  \subset W_l
$$

Ví dụ, nếu $V_i$ chỉ không gian con của V được sinh bởi $e_1, . . . , e_i$, thì $\{V_1, . . . ,V_l\}$ là một cờ cực đại.

Ngay lập tức thấy rằng $\mathfrak{b}$ là tập hợp các phần tử của $\mathfrak{g}$ làm ổn định các phần tử của cờ cực đại $\{V_1, . . . ,V_l\}$. Ngược lại, vì $\mathfrak{b}$ chứa $\mathfrak{h}$ và các ma trận $E_{ij}$ với $i < j$, ta thấy rằng các $V_i$ là các không gian con vectơ không tầm thường duy nhất ổn định dưới $\mathfrak{b}$.

Bây giờ cho $\delta$ là một cờ cực đại trong V. Suy ra từ điều trên rằng tập hợp $\mathfrak{b}_{\delta}$ gồm các phần tử của $\mathfrak{g}$ làm ổn định tất cả các phần tử của $\delta$ là một đại số con Borel của $\mathfrak{g}$. Vì mọi đại số con Borel của $\mathfrak{g}$ đều là một biến đổi của $\mathfrak{b}$ dưới một tự đẳng cấu sơ cấp, ta thấy rằng ánh xạ $\delta  \rightarrow \mathfrak{b}_{\delta}$ là một song ánh từ tập hợp các cờ cực đại đến tập hợp các đại số con Borel của $\mathfrak{g}$.

Cho $\beta$ là một cơ sở của V. Theo (I) và phần trước, các đại số con Borel chứa $\mathfrak{h}_{\beta}$ là các đại số tương ứng với các cờ cực đại mà mỗi phần tử của chúng được sinh bởi một tập con của $\beta$. Các cờ này tương ứng song ánh với các cấp toàn phần trên $\beta$ theo cách sau: với một cấp toàn phần $\omega$ trên $\beta$ được liên kết cờ $\{W_1, . . . ,W_l\}$, trong đó $W_i$ là không gian con vectơ được sinh bởi $i$ phần tử đầu tiên của $\beta$ theo cấp $\omega$. Vì có $(l+$ 1)! cấp toàn phần trên $\beta$, ta thu được lại rằng tồn tại $(l+$ 1)! đại số con Borel của $(\mathfrak{s}\mathfrak{l}(V),\mathfrak{h}_{\beta}) ($§3, no. 3, Nhận xét).

Cho $\gamma$ là một cờ trong V. Vì $\gamma$ được chứa trong một cờ cực đại, tập hợp $\mathfrak{p}_{\gamma}$ gồm các phần tử của $\mathfrak{g}$ làm ổn định các phần tử của $\gamma$ là một đại số con parabol của $\mathfrak{g}$. Ta chứng minh rằng các không gian con vectơ không tầm thường duy nhất ổn định dưới $\mathfrak{p}_{\gamma}$ là các phần tử của $\gamma$. Để làm điều này, ta có thể giả sử rằng $\gamma =\{V_{i_1}, . . . ,V_{i_q}\}$ với $1\leq i_1<\cdots < i_q\leq l$. Đặt $i_0= 0, i_{q+1}=l+ 1$. Các khoảng không rỗng

$$
i_0+ 1, i_1, i_1+ 1, i_2, . . . , i_q+ 1, i_{q+1}
$$

tạo thành một phân hoạch của $\{1, . . . , l+ 1\}$, do đó mọi ma trận bình phương cấp $l+ 1$ có thể được viết thành một ma trận khối $(X_{ab})_{1\leq a,b\leq q+1}$. Đại số $\mathfrak{p}_{\gamma}$ khi đó là tập hợp $\mathfrak{p}_{i_1,...,i_q}$ gồm các phần tử $(X_{ab})_{1\leq a,b\leq q+1}$ của $\mathfrak{s}\mathfrak{l}(l+ 1, k)$ sao cho $X_{ab}= 0$ với $a > b$. Vì $\mathfrak{p}_{i_1,...,i_q}\supset \mathfrak{b}$, một không gian con vectơ không tầm thường ổn định dưới $\mathfrak{p}_{i_1,...,i_q}$ là một trong các $V_i$; nếu $i_k< i < i_{k+1}$, đại số $\mathfrak{p}_{i_1,...,i_q}$ chứa $E_{i_{k+1},i}$ và $V_i$ không ổn định, do đó ta có mệnh đề trên.

Do đó, $2^l$ cờ chứa trong cờ cực đại $\{V_1, . . . ,V_l\}$ sinh ra $2^l$ đại số con parabol phân biệt chứa $\mathfrak{b}$; vì có đúng $2^l$ đại số con parabol chứa $\mathfrak{b}($§3, no. 4, Nhận xét), suy ra rằng ánh xạ $\gamma  \rightarrow \mathfrak{p}_{\gamma}$ là một song ánh từ tập hợp các cờ của V vào tập hợp các đại số con parabol của $\mathfrak{g}$. Hơn nữa, $\mathfrak{p}_{\gamma}\supset \mathfrak{p}_{\gamma'}$ khi và chỉ khi $\gamma \subset \gamma '$.

Nhắc lại đại số con parabol $\mathfrak{p}=\mathfrak{p}_{i_1,...,i_q}(1\leq i_1<\cdots < i_q\leq l)$. Gọi $\mathfrak{s}$ (tương ứng $\mathfrak{n}$) là tập hợp các $(X_{ab})_{1\leq a,b\leq q+1}$ trong $\mathfrak{s}\mathfrak{l}(l+ 1, k)$ sao cho $X_{ab}= 0$ với $a\not=b$ (tương ứng $a\geq b$). Theo Mệnh đề 13 của §3, no. 4, ta có $\mathfrak{p}=\mathfrak{s}\oplus \mathfrak{n}$, đại số con $\mathfrak{s}$ là khả quy trong $\mathfrak{g}$ và $\mathfrak{n}$ vừa là iđêan lũy linh lớn nhất vừa là căn lũy linh của $\mathfrak{p}$.

(IV) Với $r= 1,2, . . . , l$, đặt $\varpi_r=\varepsilon_1+\cdots +\varepsilon_r$. Ta có $\varpi_i(H_{\alpha_j}) =\delta_{ij}$, do đó $\varpi_r$ là trọng số cơ bản tương ứng với $\alpha_r$.

Gọi $\sigma$ là biểu diễn đồng nhất của $\mathfrak{g}$ trên V. Lũy thừa ngoài $\bigwedge^r\sigma$ của $\sigma$ là một biểu diễn trên $E =\bigwedge^r(V)$. Gọi $(e_1, . . . , e_{l+1})$ là cơ sở đã chọn của V. Các $e_{i_1}\wedge  \cdots  \wedge e_{i_r}$, với $i_1<\cdots < i_r$, tạo thành một cơ sở của E. Nếu $h\in \mathfrak{h}$,

$$
(\bigwedge^r\sigma )(h).e_{i_1}\wedge  \cdots  \wedge e_{i_r}= (\varepsilon_{i_1}+\cdots +\varepsilon_{i_r})(h)e_{i_1}\wedge  \cdots  \wedge e_{i_r}
$$

Do đó, mọi trọng số đều có bội số $1,\varpi_r$ là một trọng số của $\bigwedge^r\sigma$, và mọi trọng số khác đều có dạng $\varpi_r-\mu$, trong đó $\mu$ là một trọng số căn dương. Do đó, $\varpi_r$ là trọng số cao nhất của $\bigwedge^r\sigma$, và $e_1\wedge \cdots \wedge e_r$ là một phần tử nguyên thủy. Theo Chương VI, §4, no. 7.IX, nhóm Weyl có thể được đồng nhất với nhóm đối xứng của

$$
\{\varepsilon_1, . . . , \varepsilon_{l+1}\}
$$

Quỹ đạo của $\varpi_r$ dưới tác động của nhóm Weyl do đó chứa tất cả các $\varepsilon_{i_1}+\cdots +\varepsilon_{i_r}$ với $i_1<\cdots < i_r$. Môđun con đơn sinh bởi phần tử nguyên thủy $e_1\wedge  \cdots  \wedge e_r$ do đó nhận tất cả các $\varepsilon_{i_1}+\cdots +\varepsilon_{i_r}$ làm các trọng số và do đó bằng E. Vậy $\bigwedge^r\sigma$ là bất khả quy với trọng số cao nhất $\varpi_r$.

Do đó, các biểu diễn $\bigwedge^r\sigma (1\leq r\leq l)$ là các biểu diễn cơ bản. Ta có dim($\bigwedge^r\sigma$ ) $=(^{l+1}_r)$.

(V) Ta có $w_0(\alpha_1) =-\alpha_l, w_0(\alpha_2) =-\alpha_{l-1}, . .$. (Chương VI, §4, no. 7, XI), do đó

$$
-w_0(\varpi_1) =\varpi_l,-w_0(\varpi_2) =\varpi_{l-1}, . . .
$$

Đặt

$$
\omega =n_1\varpi_1+\cdots +n_l\varpi_l(n_1, . . . , n_l\in \mathbf{N})
$$

là một trọng số trội. Khi đó, biểu diễn đơn với trọng số cao nhất $\omega$ là trực giao hoặc symplectic khi và chỉ khi

$$
n_1=n_l,n_2=n_{l-1}, . .
$$

(§7, no. 5, Mệnh đề 12). Đặc biệt, nếu $l$ là chẵn, không có biểu diễn cơ bản nào của $\mathfrak{s}\mathfrak{l}(l+ 1, k)$ là trực giao hoặc symplectic. Nếu $l$ là lẻ, biểu diễn $\bigwedge^i\sigma$ với $i\not= (l+ 1)/2$ không trực giao cũng không symplectic; theo Chương VI, §4, no. 7.VI, tổng các tọa độ của $\varpi_{(l+1)/2}$ đối với $(\alpha_1, . . . , \alpha_l)$ là

$$
\frac{1}{l + 1}[\frac{l + 1}{2}(1 + 2 +\cdots +\frac{l- 1}{2})+\frac{l + 1}{2}(1 + 2 +\cdots +\frac{l + 1}{2})]
$$

$$
= 1 + 2 +\cdots +\frac{l- 1}{2}+\frac{l + 1}{4}
$$

vì vậy $\bigwedge^{(l+1)/2}\sigma$ là trực giao nếu $l\equiv  -1$ (mod. 4) và symplectic nếu $l\equiv 1$ (mod. 4) (§7, no. 5, Mệnh đề 12). Kết quả cuối cùng này có thể được làm chính xác hơn như sau. Chọn một phần tử khác không $e$ trong $\bigwedge^{l+1}(V)$. Phép nhân trong đại số ngoài V xác định một ánh xạ song tuyến tính từ

$$
\bigwedge^{(l+1)/2}(V)\times \bigwedge^{(l+1)/2}(V)
$$

đến $\bigwedge^{l+1}$(V), có thể viết dưới dạng $(u, v) \rightarrow \Phi (u, v)e$, trong đó $\Phi$ là một dạng song tuyến tính trên $\bigwedge^{(l+1)/2}(V)$. Người ta kiểm tra ngay lập tức rằng $\Phi$ khác không, bất biến dưới $\mathfrak{g}$ (và do đó không suy biến), đối xứng nếu $(l+ 1)/2$ là chẵn, và phản xứng nếu $(l+ 1)/2$ là lẻ.

(VI) Với mọi $x\in \mathfrak{g}$, đa thức đặc trưng của $\sigma (x) =x$ có thể được viết

$$
T^{l+1}+f_2(x)T^{l-1}+f_3(x)T^{l-2}+\cdots +f_{l+1}(x)
$$

trong đó $f_2, . . . , f_{l+1}$ là các hàm đa thức bất biến dưới $\mathfrak{g}($§8, no. 3, Bổ đề 2).

Nếu $x=\xi_1E_{11}+\cdots +\xi_{l+1}E_{l+1l+1}\in \mathfrak{h}$, thì các $f_i(x)$, sai khác dấu, là các hàm đối xứng sơ cấp của $\xi_1, . . . , \xi_{l+1}$ có bậc $2, . . . , l+ 1$. Do đó, theo Chap. VI, §4, no. 7.IX, các $f_i|\mathfrak{h}$ sinh đại số của các phần tử của $\mathbf{S}(\mathfrak{h}^*)$ bất biến dưới nhóm Weyl, và độc lập đại số. Suy ra (§8, no. 3, Mệnh đề $3$) rằng $f_2, f_3, . . . , f_{l+1}$ sinh đại số của các hàm đa thức bất biến dưới $\mathfrak{g}$, và độc lập đại số.

(VII) Với mọi $g\in \mathbf{G}\mathbf{L}(l+ 1, k)$, đặt $\varphi_k(g) =\varphi (g)$ là tự đẳng cấu $x \rightarrow gxg^{-1}$ của $\mathfrak{g}$. Khi đó $\varphi$ là một đồng cấu từ $\mathbf{G}\mathbf{L}(l+ 1, k)$ đến Aut($\mathfrak{g}$). Ta có

$\varphi (\mathbf{S}\mathbf{L}(l+ 1, k)) =$ Aut$_e(\mathfrak{g})$

(Chap. VII, §3, no. 1, Nhận xét 2). Gọi $\overline{k}$ là một bao đóng đại số của $k$. Ta có

$$
\mathbf{G}\mathbf{L}(l+ 1,\overline{k}) = \overline{k}^*.\mathbf{S}\mathbf{L}(l+ 1,\overline{k})
$$

do đó $\varphi_{\overline{k}}(\mathbf{G}\mathbf{L}(l+ 1,\overline{k})) =\varphi_{\overline{k}}(\mathbf{S}\mathbf{L}(l+ 1,\overline{k})) =$ Aut$_e(\mathfrak{g}\otimes_k\overline{k})$; suy ra rằng $\varphi (\mathbf{G}\mathbf{L}(l+ 1, k))\subset$ Aut$_0(\mathfrak{g})$. Mặt khác, Aut$_0(\mathfrak{g})\subset \varphi (\mathbf{G}\mathbf{L}(l+ 1, k))$, theo Mệnh đề 2 của §7, no. 1, áp dụng cho biểu diễn đồng nhất của $\mathfrak{g}$. Vì vậy,

Aut$_0(\mathfrak{g}) =\varphi (\mathbf{G}\mathbf{L}(l+ 1, k))$.

Hạt nhân của $\varphi$ là tập hợp các phần tử của $\mathbf{G}\mathbf{L}(l+ 1, k)$ giao hoán với mọi ma trận cấp $l+1$, nghĩa là tập hợp $k^*$ các ma trận vô hướng khả nghịch. Do đó, Aut$_0(\mathfrak{g})$ có thể được đồng nhất với nhóm $\mathbf{G}\mathbf{L}(l+ 1, k)/k^*=\mathbf{P}\mathbf{G}\mathbf{L}(l+ 1, k)$. Hạt nhân của $\varphi '=\varphi |\mathbf{S}\mathbf{L}(l+ 1, k)$ là $\mu_{l+1}(k)$, trong đó $\mu_{l+1}(k)$ chỉ tập hợp các căn đơn vị bậc $(l+$ 1) trong $k$. Do đó, Aut$_e(\mathfrak{g})$ có thể được đồng nhất với nhóm $\mathbf{S}\mathbf{L}(l+ 1, k)/\mu_{l+1}(k) =\mathbf{P}\mathbf{S}\mathbf{L}(l+ 1, k)$. Mặt khác, ta có dãy khớp

1 $\longrightarrow \mathbf{S}\mathbf{L}(l+ 1, k)\longrightarrow \mathbf{G}\mathbf{L}(l+ 1, k)\longrightarrow^{det}k^*\longrightarrow$ 1

và ảnh của $k^*$ qua det là $k^{*l+1}$. Suy ra rằng có các đẳng cấu chính tắc

Aut$_0(\mathfrak{g})/$Aut$_e(\mathfrak{g})\longrightarrow \mathbf{P}\mathbf{G}\mathbf{L}(l+ 1, k)/\mathbf{P}\mathbf{S}\mathbf{L}(l+ 1, k)$

$$
\longrightarrow \mathbf{G}\mathbf{L}(l+ 1, k)/k^*.\mathbf{S}\mathbf{L}(l+ 1, k)\longrightarrow k^*/k^{*l+1}
$$

Nếu $k$ = $\mathbf{R}$, ta thấy rằng Aut$_0(\mathfrak{g}) =$ Aut$_e(\mathfrak{g})$ nếu $l+ 1$ là lẻ, và rằng Aut$_0(\mathfrak{g})/$Aut$_e(\mathfrak{g})$ là đẳng cấu với $\mathbf{Z}/2\mathbf{Z}$ nếu $l+ 1$ là chẵn.

Với các ký hiệu của §$5,f(T_{\mathbf{Q}})$ là tập hợp các tự đẳng cấu của $\mathfrak{g}$ cảm sinh đồng nhất trên $\mathfrak{h}$, và do đó bằng $\varphi$(D), trong đó D là tập hợp các phần tử đường chéo của $\mathbf{G}\mathbf{L}(l+ 1, k) ($§5, Mệnh đề 4). Gọi $D'$ là tập hợp các phần tử đường chéo của $\mathbf{S}\mathbf{L}(l+ 1, k)$. Theo Mệnh đề 3 của §5, và sự xác định của Aut$_e(\mathfrak{g})$, ta có $f(q(T_P))\subset \varphi (D')$. Ta chứng minh rằng $f(q(T_P)) =\varphi (D')$. Cho

$\lambda_1$ 0

$d=$ . ..

0 $\lambda_{l+1}$

là một phần tử của $D'$. Có một $\zeta \in$ Hom(Q(R)$, k^*$) $= T_Q$ sao cho $\zeta (\varepsilon_i-\varepsilon_j) =\lambda_i\lambda^{-1}_j$ với mọi $i$ và $j$. Dễ dàng kiểm tra rằng $f(\zeta ) =\varphi (d)$. Theo Chap. VI, §4, no. 7.VIII, P(R) được sinh bởi Q(R) và phần tử $\varepsilon =\varepsilon_1$, mà ảnh của nó trong $P(R)/Q(R)$ có cấp $l+ 1$; nhưng

$$
\zeta ((l+ 1)\varepsilon ) =\zeta ((\varepsilon_1-\varepsilon_2) + (\varepsilon_1-\varepsilon_3) +\cdots + (\varepsilon_1-\varepsilon_{l+1}))
$$

$$
=\lambda^l_1\lambda^{-1}_2\lambda^{-1}_3. . . \lambda^{-1}_{l+1}=\lambda^{l+1}_1
$$

nên $\zeta$ mở rộng thành một đồng cấu từ P(R) đến $k^*$. Điều này chứng minh rằng $\zeta \in q(T_P)$, do đó $\varphi (d)\in f(q(T_P))$.

Nhắc lại (§5, no. 3, Hệ quả 2 của Mệnh đề 5) rằng Aut($\mathfrak{g}$) $=$ Aut$_0(\mathfrak{g})$ với $l= 1$, và rằng Aut($\mathfrak{g}$)$/$Aut$_0(\mathfrak{g})$ là đẳng cấu với $\mathbf{Z}/2\mathbf{Z}$ với $l\geq 2$. Ánh xạ $\theta :x \rightarrow  -^tx$ là một tự đẳng cấu của $\mathfrak{s}\mathfrak{l}(l+ 1, k)$ và $a_0=\theta |\mathfrak{h}\notin W$ nếu $l\geq 2$ (Ch. VI, §4, no. 7.XI), do đó lớp của $a_0$ trong Aut($\mathfrak{g}$)$/$Aut$_0(\mathfrak{g})$ là phần tử không tầm thường của nhóm này (§5, no. 2, Mệnh đề 4).

(VIII) Hạn chế của dạng Killing trên $\mathfrak{h}$ là

$$
\Phi (\xi_1E_{11}+\cdots +\xi_{l+1}E_{l+1,l+1}, \xi '_1E_{11}+\cdots +\xi '_{l+1}E_{l+1,l+1})
$$

$$
=\sum_{i\not=j}(\xi_i-\xi_j)(\xi '_i-\xi '_j) =\sum_{i,j}(\xi_i-\xi_j)(\xi '_i-\xi '_j)
$$

$$
= (l+ 1)\sum_i\xi_i\xi '_i+ (l+ 1)\sum_j\xi_j\xi '_j-2(\sum_i\xi_i)(\sum_j\xi '_j
$$

$$
= 2(l+ 1)\sum_i\xi_i\xi '_i
$$

(IX) Với $1\leq i < j\leq l+ 1$, đặt

$$
X_{\varepsilon_i-\varepsilon_j}=E_{ij}X_{\varepsilon_j-\varepsilon_i}=-E_{ji}
$$

Khi đó, với mọi $\alpha \in R$, ta có $[X_{\alpha}, X_{-\alpha}] =-H_{\alpha}$ và $\theta (X_{\alpha}) =X_{-\alpha}$ (trong đó $\theta$ là tự đẳng cấu $x \rightarrow  -^tx$ được đưa vào trong (VII)). Do đó, $(X_{\alpha})_{\alpha\in R}$ là một hệ Chevalley trong $(\mathfrak{g},\mathfrak{h})$.

Lấy $k=\mathbf{Q}$. Các dàn cho phép trong $\mathfrak{h}($§12, no. 6, Định. 1) là những dàn nằm giữa $\mathbf{Z}$-môđun $Q(R^{\vee})$ được sinh bởi các $E_{ii}-E_{i+1,i+1}$, nghĩa là gồm các ma trận đường chéo thuộc $\mathfrak{s}\mathfrak{l}(l+ 1,\mathbf{Z})$, và $\mathbf{Z}$-môđun $P(R^{\vee})$ được sinh bởi $Q(R^{\vee})$ và $E_{11}-(l+ 1)^{-1}\sum E_{ii}$ (Ch. VI, §4, no. 7.VIII), nghĩa là gồm các ma trận đường chéo có vết bằng không dạng $x+ (l+ 1)^{-1}a.1$, trong đó $x$ có các phần tử nguyên và $a\in \mathbf{Z}$. Suy ra rằng $\mathfrak{s}\mathfrak{l}(l+1,\mathbf{Z})$ là cấp Chevalley trong $(\mathfrak{g},\mathfrak{h})$ liên kết với dàn cho phép $Q(R^{\vee})$ và hệ Chevalley $(X_{\alpha})$. Dễ dàng kiểm tra rằng $\bigwedge^r\mathbf{Z}^{l+1}$ là một dàn khả dụng trong $\bigwedge^r\mathbf{Q}^{l+1}$ đối với $\mathfrak{s}\mathfrak{l}(l+ 1,\mathbf{Z}) ($§12, no. 8, Định. 3).

Mặt khác, $\mathfrak{g}\mathfrak{l}(l+ 1,\mathbf{Z})$ là một dàn Chevalley trong đại số khả quy tách $\mathfrak{g}\mathfrak{l}(l+ 1,\mathbf{Q})$; phép chiếu của nó lên $\mathfrak{s}\mathfrak{l}(l+ 1,\mathbf{Q})$ song song với tâm $\mathbf{Q}.1$ của $\mathfrak{g}\mathfrak{l}(l+1,\mathbf{Q})$ là dàn Chevalley trong $(\mathfrak{g},\mathfrak{h})$ được xác định bởi dàn cho phép $P(R^{\vee})$ trong $\mathfrak{h}$ và hệ Chevalley $(X_{\alpha})$. Ta nhận xét rằng $\mathfrak{g}\mathfrak{l}(l+ 1,\mathbf{Z})$ không phải là tổng trực tiếp của các giao của nó với $\mathfrak{s}\mathfrak{l}(l+ 1,\mathbf{Q})$ và tâm của $\mathfrak{g}\mathfrak{l}(l+ 1,\mathbf{Q})$.

### 2. CÁC ĐẠI SỐ KIỂU B$_{\boldsymbol{l}}$ ($\boldsymbol{l}\geq$ 1)

(I) Cho V là một không gian vectơ hữu hạn chiều, và $\Psi$ là một dạng song tuyến tính đối xứng không suy biến trên V. Tập hợp các tự đồng cấu $x$ của V sao cho $\Psi (xv, v') +\Psi (v, xv') = 0$ với mọi $v, v'\in V$ là một đại số Lie con của $\mathfrak{s}\mathfrak{l}$(V), nửa đơn với dim $V\not= 2$ (Chương I, §6, no. 7, Mệnh đề 9). Ta ký hiệu nó bởi $\mathfrak{o}(\Psi )$ và gọi nó là đại số Lie trực giao liên kết với $\Psi$.

Giả sử rằng V có chiều lẻ $2l+ 1\geq 3$ và rằng $\Psi$ có chỉ số cực đại $l$. Ký hiệu bởi Q dạng toàn phương sao cho $\Psi$ liên kết với Q. Ta có $Q(x) =\frac{1}{2}\Psi (x, x)$ với $x\in V$. Theo Đại số, Chương IX, §4, no. 2, V có thể được viết thành tổng trực tiếp của hai không gian con hoàn toàn đẳng hướng cực đại F và $F'$ và phần bù trực giao G của $F + F'$, là không đẳng hướng và 1 chiều. Bằng cách nhân $\Psi$ với một hằng khác không, ta có thể giả sử rằng tồn tại $e_0\in G$ sao cho $\Psi (e_0, e_0) =-2$. Mặt khác, F và $F'$ đối ngẫu với nhau qua $\Psi$; gọi $(e_i)_{1\leq i\leq l}$ là một cơ sở của F và $(e_{-i})_{1\leq i\leq l}$ là cơ sở đối ngẫu của $F'$. Khi đó

$$
(e_1, . . . , e_l, e_0, e_{-l}, . . . , e_{-1})
$$

là một cơ sở của V; ta có

$$
Q(\sum x_ie_i)=-x^2_0+\sum_{i=1}^{i=l}x_ix_{-i}
$$

và ma trận của $\Psi$ đối với cơ sở này là ma trận vuông cấp $2l+ 1$

0 0 $\cdots$ 0 1

0 0 $s$ 0 0 $\cdots$ 1 0

$S=$ 0 $-2$ 0 $,s=$ ... ... . .. ... ...,

$s$ 0 0 0 1 $\cdots$ 0 0

1 0 $\cdots$ 0 0

trong đó $s$ là ma trận vuông cấp $l$ mà tất cả các phần tử của nó đều bằng không ngoại trừ các phần tử trên đường chéo thứ hai$^6$ bằng 1. Một cơ sở của V có các tính chất trước đó sẽ được gọi là một cơ sở Witt của V. Đại số $\mathfrak{g}=\mathfrak{o}(\Psi )$ khi đó có thể được đồng nhất với đại số $\mathfrak{o}_S(2l+ 1, k)$ của các ma trận vuông $a$ cấp $2l+ 1$ sao cho $a=-S^{-1}aS($Đại số, Chương IX, §1, no. 10, công thức (50)). Một tính toán đơn giản cho thấy rằng $\mathfrak{g}$ là tập hợp các ma trận có dạng

$$
A2s^txB
$$

$y$ 0 $x$ (2)

$$
C2s^tyD
$$

trong đó $x$ và $y$ là các ma trận có 1 hàng và $l$ cột và $A, B, C, D$ là các ma trận vuông cấp $l$ sao cho $B=-s^tBs, C=-s^tCs$, và $D=-s^tAs$. Vì ánh xạ $A \rightarrow s^tAs$ từ $\mathbf{M}_l(k)$ vào chính nó là phép đối xứng đối với đường chéo thứ hai, nên suy ra

dim$\mathfrak{g}= 2l+l^2+ 2\frac{l(l-1)}{2}=l(2l+ 1)$.

Gọi $\mathfrak{h}$ là tập hợp các phần tử đường chéo của $\mathfrak{g}$. Đây là một đại số con giao hoán của $\mathfrak{g}$, với cơ sở là các phần tử

$^6$ Đường chéo thứ hai của một ma trận vuông $(a_{ij})_{1\leq i,j\leq n}$ là họ các $a_{ij}$ sao cho

$$
i+j=n+ 1
$$

$$
H_i=E_{i,i}-E_{-i,-i}(1\leq i\leq l)
$$

Gọi $(\varepsilon_i)$ là cơ sở đối ngẫu của $\mathfrak{h}^*$ đối với $(H_i)$. Đặt

$$
X_{\varepsilon_i}= 2E_{i,0}+E_{0,-i}(1\leq i\leq l)
$$

$X_{-\varepsilon_i}$ = $-2E_{-i,0}-E_{0,i}(1\leq i\leq l)$

$X_{\varepsilon_i-\varepsilon_j}$ = $E_{i,j}-E_{-j,-i}(1\leq i < j\leq l)$

$X_{\varepsilon_j-\varepsilon_i}$ = $-E_{j,i}+E_{-i,-j}(1\leq i < j\leq l)$ (3)

$X_{\varepsilon_i+\varepsilon_j}$ = $E_{i,-j}-E_{j,-i}(1\leq i < j\leq l)$

$X_{-\varepsilon_i-\varepsilon_j}$ = $-E_{-j,i}+E_{-i,j}(1\leq i < j\leq l)$.

Dễ dàng kiểm tra rằng các phần tử này tạo thành một cơ sở của một phần bù của $\mathfrak{h}$ trong $\mathfrak{g}$ và rằng, với $h\in \mathfrak{h}$,

$$
[h, X_{\alpha}] =\alpha (h)X_{\alpha} \tag{4}
$$

với mọi $\alpha \in R$, trong đó R là tập hợp các $\pm \varepsilon_i$ và các $\pm \varepsilon_i\pm \varepsilon_j(1\leq i < j\leq l)$. Suy ra rằng $\mathfrak{h}$ bằng chuẩn hóa của nó trong $\mathfrak{g}$, và do đó là một đại số con Cartan của $\mathfrak{g}$, rằng $\mathfrak{h}$ tách, và rằng các nghiệm của $(\mathfrak{g},\mathfrak{h})$ là các phần tử của R. Hệ nghiệm R của $(\mathfrak{g},\mathfrak{h})$ có kiểu $B_l$ với $l\geq 2$, và có kiểu $A_1$ (cũng nói là có kiểu $B_1$) với $l= 1$ (Chương VI, §4, no. 5.I, mở rộng cho trường hợp $l= 1$). Do đó, $\mathfrak{g}$ là một đại số Lie đơn tách được kiểu $B_l$.

Mọi đại số con Cartan tách của $\mathfrak{o}(\Psi )$ là một biến đổi của $\mathfrak{h}$ bởi một tự đẳng cấu sơ cấp của $\mathfrak{o}(\Psi )$, và do đó bởi một phần tử của $\mathbf{O}(\Psi )$ (xem (VII)), và vì vậy là tập hợp $\mathfrak{h}_{\beta}$ gồm các phần tử của $\mathfrak{g}$ mà ma trận của chúng đối với một cơ sở Witt $\beta$ của V là đường chéo. Ta kiểm tra ngay lập tức rằng các không gian con vectơ duy nhất bất biến dưới $\mathfrak{h}_{\beta}$ là các không gian được sinh bởi một tập con của $\beta$.

Nếu $l= 1$, các đại số $\mathfrak{o}(\Psi )$ và $\mathfrak{s}\mathfrak{l}(2, k)$ có cùng các hệ nghiệm, và do đó đẳng cấu với nhau (xem thêm §1, Bài tập 16). Từ đây trở đi, ta giả sử rằng $l\geq 2$.

(II) Hệ nghiệm $R^{\vee}$ được xác định nhờ Chương VI, §4, no. 5.V, và ta thấy rằng

$$
H_{\varepsilon_i}= 2H_i, H_{\varepsilon_i-\varepsilon_j}=H_i-H_j, H_{\varepsilon_i+\varepsilon_j}=H_i+H_j
$$

(III) Đặt $\alpha_1=\varepsilon_1-\varepsilon_2, . . . , \alpha_{l-1}=\varepsilon_{l-1}-\varepsilon_l, \alpha_l=\varepsilon_l$. Theo Chương VI, §4, no. 5.II, $(\alpha_1, . . . , \alpha_l)$ là một cơ sở B của R; các nghiệm dương tương ứng với B là các $\varepsilon_i$ và các $\varepsilon_i\pm \varepsilon_j(i < j)$. Đại số con Borel tương ứng $\mathfrak{b}$ là tập hợp các ma trận tam giác trên trong $\mathfrak{g}$.

Ta kiểm tra ngay lập tức rằng các không gian con vectơ duy nhất của V khác $\{0\}$ và V và ổn định dưới $\mathfrak{b}$ là các phần tử của cờ cực đại tương ứng với cơ sở $(e_i)$, nghĩa là các không gian con toàn đẳng hướng $V_1, . . . ,V_l$, trong đó $V_i$ được sinh bởi $e_1, . . . , e_i$, cùng với các phần bù trực giao của chúng $V_{-1}, . . . ,V_{-i}:$ phần bù trực giao $V_{-i}$ của $V_i$ được sinh bởi $e_1, . . . , e_l, e_0, e_{-l}, . . . , e_{-i-1}$ và không toàn đẳng hướng. Mặt khác, nếu một phần tử của $\mathfrak{g}$ giữ ổn định một không gian con vectơ, thì nó giữ ổn định phần bù trực giao của không gian đó. Do đó, $\mathfrak{b}$ là tập hợp các phần tử của $\mathfrak{g}$ giữ ổn định các phần tử của cờ $\{V_1, . . . ,V_l\}$.

Một cờ được gọi là đẳng hướng nếu mỗi phần tử của nó là toàn đẳng hướng. Cờ $\{V_1, . . . ,V_l\}$ là một cờ đẳng hướng cực đại. Vì nhóm $\mathbf{O}(\Psi )$ tác động bắc cầu vừa trên các đại số con Borel của $\mathfrak{g}$ (xem (VII)) vừa trên các cờ đẳng hướng cực đại (Đại số, Chương IX, §4, no. 3, Định lý 1), ta thấy rằng, với mọi cờ đẳng hướng cực đại $\delta$ trong V, tập hợp $\mathfrak{b}_{\delta}$ gồm các phần tử của $\mathfrak{g}$ giữ ổn định các phần tử của $\delta$ là một đại số con Borel của $\mathfrak{g}$ và ánh xạ $\delta  \rightarrow \mathfrak{b}_{\delta}$ là một song ánh từ tập hợp các cờ đẳng hướng cực đại đến tập hợp các đại số con Borel của $\mathfrak{g}$.

Cho $\delta$ là một cờ đẳng hướng và cho $\mathfrak{p}_{\delta}$ là tập hợp các phần tử của $\mathfrak{g}$ làm ổn định các phần tử của $\delta$. Nếu $\delta \subset  \{V_1, . . . ,V_l\}$, thì $\mathfrak{p}_{\delta}$ là một đại số con parabolic của $\mathfrak{g}$ chứa $\mathfrak{b}$, và dễ dàng kiểm tra rằng các không gian con đẳng hướng toàn phần $\not=\{0\}$ duy nhất ổn định dưới $\mathfrak{p}_{\delta}$ là các phần tử của $\delta$. Điều này cho $2^l$ đại số con parabolic của $\mathfrak{g}$ chứa $\mathfrak{b}$. Ta thấy như trên rằng ánh xạ $\delta  \rightarrow \mathfrak{p}_{\delta}$ là một song ánh từ tập hợp các cờ đẳng hướng trong V đến tập hợp các đại số con parabolic của $\mathfrak{g}$. Hơn nữa, $\mathfrak{p}_{\delta}\subset \mathfrak{p}_{\delta'}$ khi và chỉ khi $\delta \supset \delta '$.

(IV) Các trọng số cơ bản tương ứng với $\alpha_1, . . . , \alpha_l$ là, theo Ch. VI, §4, no. 5.VI,

$$
\varpi_i=\varepsilon_1+\cdots +\varepsilon_i(1\leq i\leq l-1)
$$

$$
\varpi_l=\frac{1}{2}(\varepsilon_1+\cdots +\varepsilon_l)
$$

Cho $\sigma$ là biểu diễn đồng nhất của $\mathfrak{g}$ trên V. Lũy thừa ngoài $\bigwedge^r\sigma$ tác động trên $E =\bigwedge^rV$. Nếu $h\in \mathfrak{h}$,

$\sigma (h).e_i=\varepsilon_i(h)e_i$ for $1\leq i\leq l$

$$
\sigma (h).e_0= 0
$$

$\sigma (h).e_{-i}=-\varepsilon_i(h)e_{-i}$ for $1\leq i\leq l$.

Suy ra rằng, với $1\leq r\leq l,\varepsilon_1+\cdots +\varepsilon_r$ là trọng số cao nhất của $\bigwedge^r\sigma$, các phần tử có trọng số $\varepsilon_1+\cdots +\varepsilon_r$ là các phần tử tỉ lệ với $e_1\wedge  \cdots  \wedge$ $e_r$. Ta sẽ chứng minh rằng với $1\leq r\leq l-1$, biểu diễn $\bigwedge^r\sigma$ là một biểu diễn cơ bản của $\mathfrak{g}$ có trọng số cao nhất $\varpi_r$. Để làm điều này, chỉ cần chứng minh rằng $\bigwedge^r\sigma$ là bất khả quy với $0\leq r\leq 2l+ 1$. Nhưng dạng song tuyến tính $\Phi$ trên $\bigwedge^rV\times \bigwedge^{2l+1-r}V$ được xác định bởi

$$
x\wedge y=\Phi (x, y)e_1\wedge  \cdots  \wedge e_l\wedge e_0\wedge e_{-l}\wedge  \cdots  \wedge e_{-1}
$$

là bất biến dưới $\mathfrak{g}$ và đặt $\bigwedge^rV$ và $\bigwedge^{2l+1-r}V$ trong đối ngẫu. Do đó, biểu diễn $\bigwedge^{2l+1-r}\sigma$ là đối ngẫu của $\bigwedge^r\sigma$ và chỉ cần chứng minh tính bất khả quy của $\bigwedge^r\sigma$ với $0\leq r\leq l$, hay rằng không gian con nhỏ nhất $T_r$ của $\bigwedge^rV$ chứa $e_1\wedge  \cdots  \wedge e_r$ và ổn định dưới $\mathfrak{g}$ là toàn bộ $\bigwedge^rV$. Điều này là ngay lập tức đối với $r= 0$ và $r= 1$ (xem công thức (2)). Đối với $r= 2$ (và do đó $l\geq 2$), biểu diễn $\bigwedge^2\sigma$ và biểu diễn phụ hợp của $\mathfrak{g}$ (vốn là bất khả quy) có cùng chiều $l(2l+ 1)$ và cùng trọng số cao nhất $\varepsilon_1+\varepsilon_2$ (Chap. VI, §4, no. 5.IV). Ta kết luận rằng $\bigwedge^2\sigma$ tương đương với biểu diễn phụ hợp, và do đó là bất khả quy. Điều này chứng minh mệnh đề của ta đối với $l= 1$ và $l= 2$.

Bây giờ ta lập luận bằng quy nạp theo $l$, và giả sử rằng $l\geq r\geq 3$. Trước hết ta nhận xét rằng nếu W là một không gian con không đẳng hướng của V có chiều lẻ, với phần bù trực giao $W'$, thì hạn chế $\Psi_W$ của $\Psi$ lên W là không suy biến và $\mathfrak{o}(\Psi_W)$ có thể được đồng nhất với đại số con của $\mathfrak{g}$ gồm các phần tử triệt tiêu trên $W'$. Nếu dim $W<$ dim V, và nếu $\Psi_W$ có chỉ số cực đại, giả thiết quy nạp suy ra rằng nếu $T_r$ chứa một phần tử khác không có dạng $w'\wedge w$, với $w'\in \bigwedge^{r-k}W'$ và $w\in \bigwedge^kW (0\leq k\leq r)$, thì $T_r$ chứa $w'\wedge \bigwedge^kW:$ thật vậy, ta có $a.(w'\wedge w) =w'\wedge a.w$ với mọi $a\in \mathfrak{o}(\Psi_W)$. Ta chứng minh bằng quy nạp theo $p\in 0, r$ rằng $T_r$ chứa các phần tử

$$
x=e_{i_1}\wedge  \cdots  \wedge e_{i_{r-p}}\wedge e_{j_1}\wedge  \cdots  \wedge e_{j_p}
$$

với $1\leq i_1<\cdots < i_{r-p}\leq l$ và $-l\leq j_1<\cdots < j_p\leq 0$. Với $p= 0$, điều này suy ra từ tính bất khả quy của phép toán của $\mathfrak{g}\mathfrak{l}(F)$ trên $\bigwedge^rF$ (no. 1), vì

$\mathfrak{g}$ chứa các phần tử giữ cố định $F = V_l=\sum_{i=1}^lke_i$ và cảm sinh trên đó một tự đồng cấu bất kỳ (xem công thức (2)). Nếu $p= 1$, lấy $q\in (1, l)$ sao cho $q\not=-j_1$ và sao cho tồn tại $\lambda \in 1, r-p$ với $q=i_{\lambda}$; nếu $p\geq 2$, lấy $q\in 1, l$ sao cho $-q\in  \{j_1, . . . , j_p\}$. Sau khi hoán vị các $e_i$ nếu cần, ta có thể giả sử rằng $q= 1$. Bây giờ lấy W là phần bù trực giao của $W'=ke_1+ke_{-1}$. Nếu $p= 1$, ta có $x\in e_1\wedge \bigwedge^{r-1}W$; vì $T_r$ chứa $e_1\wedge  \cdots  \wedge e_r$, suy ra $T_r$ chứa $x$. Nếu $p\geq 2$, hoặc $x\in e_{-1}\wedge \bigwedge^{r-1}W$ hoặc $x\in e_1\wedge e_{-1}\wedge \bigwedge^{r-2}W$; vì theo giả thiết quy nạp, $T_r$ chứa $e_{-1}\wedge e_2\wedge  \cdots  \wedge e_{r-1}$ và $e_{-1}\wedge e_1\wedge e_2\wedge  \cdots  \wedge e_{r-2}$, suy ra $T_r$ chứa $x$, điều này hoàn tất chứng minh.

Để xem một chứng minh khác về tính bất khả quy của $\bigwedge^r\sigma$, xem Bài tập 6.

Bây giờ ta sẽ xác định biểu diễn cơ bản có trọng số cao nhất $\varpi_l$.

#### Bổ đề 1 {#lie-viii-s13-lem-1 .statement tag=018T}

Cho V là một không gian vectơ hữu hạn chiều, Q một dạng toàn phương không suy biến trên V$,\Psi$ dạng song tuyến tính đối xứng liên kết với Q, C(Q) đại số Clifford của V đối với Q$,f_0$ hợp của các ánh xạ chính tắc

$$
\mathfrak{o}(\Psi )\longrightarrow \mathfrak{g}\mathfrak{l}(V)\longrightarrow V\otimes V^*\longrightarrow V\otimes V\longrightarrow C^+(Q)
$$

(trong đó ánh xạ thứ 1 là đơn ánh chính tắc, ánh xạ thứ 3 được xác định bởi đẳng cấu chính tắc từ $V^*$ đến V tương ứng với $\Psi$, ánh xạ thứ 4 được xác định bởi phép nhân trong C(Q), xem Algebra, Chap. IX, § 9, no. 1). Đặt $f=\frac{1}{2}f_0$.

(i) Nếu $(e_r),(e'_r)$ là các cơ sở của V sao cho $\Psi (e_r, e'_s) =\delta_{rs}$, ta có $f_0(a) =$ $\sum_r(ae_r)e'_r$ với mọi $a\in \mathfrak{o}(\Psi )$.

(ii) Nếu $a, b\in \mathfrak{o}(\Psi )$, ta có $\sum_r(ae_r)(be'_r) =-\sum_r(abe_r)e'_r$.

(iii) Nếu $a\in \mathfrak{o}(\Psi )$ và $v\in V$, ta có $[f(a), v] =av$.

(iv) Nếu $a, b\in \mathfrak{o}(\Psi )$, ta có $[f(a), f(b)] =f([a, b])$.

(v) $f(\mathfrak{o}(\Psi ))$ sinh ra đại số kết hợp C^+(Q).

(vi) Cho N là một C^+(Q)-môđun trái và $\rho$ là đồng cấu tương ứng từ C^+(Q) vào End$_k(N)$. Khi đó $\rho \circ f$ là một biểu diễn của $\mathfrak{o}(\Psi )$ trên N. Nếu N là đơn, thì $\rho \circ f$ là bất khả quy.

Mệnh đề (i) là hiển nhiên. Nếu $a, b\in \mathfrak{o}(\Psi )$, ta có (đặt $\Psi (x, y) =\langle x, y\rangle$ )$:$

$$
\sum_r(ae_r)(be'_r) =\sum_{r,s,t}\langle ae_r, e'_s\rangle \langle be'_r, e_t\rangle e_se'_t=\sum_{r,s,t}\langle e_r, ae'_s\rangle \langle e'_r, be_t\rangle e_se'_t
$$

$$
=\sum_{s,t}\langle ae'_s, be_t\rangle e_se'_t=-\sum_{s,t}\langle e'_s, abe_t\rangle e_se'_t=-\sum_t(abe_t)e'_t
$$

điều này chứng minh (ii). Tiếp theo, với mọi $v\in V$, theo (i),

1 $''$

$$
[f(a), v] =\sum((ae_r)e_rv-v(ae_r)e_r)
$$

2

= $1\sum^r((ae_r)e'_rv+ (ae_r)ve'_r-(ae_r)ve'_r-v(ae_r)e'_r)$

2

$r$

1 $''$

= $\sum((ae_r)\langle e_r, v\rangle  - \langle ae_r, v\rangle e_r)$

2

= $1a(\sum^r\langle e'_r, v\rangle e_r)+1\sum\langle e_r, av\rangle e'_r=1av+1av=av$,

2 $_r$ 2 $_r$ 2 2

điều này chứng minh (iii). Khi đó

$[f(a), f(b)] =[f(a),\frac{1}{2}\sum(be_r)e'_r]$ theo (i)

$r$

$=\frac{1}{2}\sum([f(a), be_r]e'_r+ (be_r)[f(a), e'_r])$ $=\frac{1}{2}\sum^r((abe_r)e'_r+ (be_r)(ae'_r))$ theo (iii)

$r$

$=\frac{1}{2}\sum((abe_r)e'_r-(bae_r)e'_r)$ theo (ii)

$r$

$=f([a, b])$ theo (i)

điều này chứng minh (iv). Để chứng minh (v), ta có thể, bằng cách mở rộng vô hướng, giả sử rằng $k$ đóng đại số. Khi đó chọn một cơ sở $(e_r)$ của V sao cho $\Psi (e_r, e_s) =\delta_{rs}$, nên $e'_r=e_r$. Nếu $i\not=j$, thì $E_{ij}-E_{ji}\in \mathfrak{o}(\Psi )$ và

$$
f(E_{ij}-E_{ji}) =\frac{1}{2}(e_ie_j-e_je_i) =e_ie_j
$$

nhưng các $e_ie_j$ sinh $C^+(Q)$.

Mệnh đề (vi) suy ra từ (iv) và (v). Q.E.D.

Bây giờ nhắc lại các ký hiệu đã dùng ở đầu số này. Đặt $\widetilde{V} = F + F'$ và gọi $\widetilde{Q}$ (tương ứng $\widetilde{\Psi}$) là hạn chế của Q (tương ứng $\Psi$ ) trên $\widetilde{V}$. Khi đó $\widetilde{Q}$ là một dạng toàn phương không suy biến có chỉ số cực đại $l$ trên không gian $\widetilde{V}$ có chiều $2l$ và đại số Clifford $C( \widetilde{Q})$ là một đại số đơn tâm có chiều $2^{2l}($Algebra, Chap. IX, §9, no. 4, Định lý 2). Gọi N là đại số ngoài của không gian con đẳng hướng cực đại $F'$ sinh bởi $e_{-1}, . . . , e_{-l}$. Đồng nhất F với không gian đối ngẫu của $F'$ nhờ $\Psi$ và với $x\in F'$ (tương ứng $y\in F$) ký hiệu $\lambda (x)$ (tương ứng $\lambda (y)$) tích ngoài trái với $x$ (tương ứng phép co trái với $y$) trong N; nếu $a_1, . . . , a_k\in F'$, thì

$$
\lambda (x).(a_1\wedge  \cdots  \wedge a_k) =x\wedge a_1\wedge  \cdots  \wedge a_k
$$

$$
\lambda (y).(a_1\wedge  \cdots  \wedge a_k) =\sum_{i=1}^k(-1)^{i-1}\Psi (a_i, y)a_1\wedge  \cdots  \wedge a_{i-1}\wedge a_{i+1}\wedge  \cdots  \wedge a_k
$$

Dễ dàng kiểm tra rằng $\lambda (x)^2=\lambda (y)^2= 0$ và rằng

$$
\lambda (x)\lambda (y) +\lambda (y)\lambda (x) =\Psi (x, y).1
$$

Suy ra (Algebra, Chap. IX, §9, no. 1) rằng tồn tại một đồng cấu duy nhất (vẫn ký hiệu là $\lambda$ ) từ $C( \widetilde{Q})$ vào End(N) mở rộng ánh xạ $\lambda : F\cup F'\rightarrow$ End(N). Vì dim $N = 2^l$ và vì $C( \widetilde{Q})$ có một lớp duy nhất các môđun đơn, có chiều $2^l($Algebra, Chap. IX, §9, no. 4, Th. 2), biểu diễn của $C( \widetilde{Q})$ trên N xác định bởi $\lambda$ là bất khả quy và là một biểu diễn spinor của $C( \widetilde{Q}) ($loc. cit.).

Xét ánh xạ $\mu:v \rightarrow e_0v$ từ $\widetilde{V}$ vào $C^+(Q)$. Với $v\in \widetilde{V}$, ta có

$$
(e_0v)^2=-e^2_0v^2=-Q(e_0)Q(v) = Q(v) = \widetilde{Q}(v)
$$

và $\mu$ mở rộng duy nhất thành một đồng cấu, vẫn ký hiệu là $\mu$, từ $C( \widetilde{Q})$ vào $C^+(Q)$. Vì $C( \widetilde{Q})$ là đơn và vì

dim $C^+(Q) =$ dim $C( \widetilde{Q}) = 2^{2l}$,

ta thấy $\mu$ là một đẳng cấu. Do đó, $\lambda \circ \mu^{-1}$ xác định một cấu trúc môđun đơn của $C^+$(Q) trên N và $\rho =\lambda \circ \mu^{-1}\circ f$ là một biểu diễn bất khả quy của $\mathfrak{g}$ trên N (Bổ đề 1 (vi)).

Mặt khác, theo Bổ đề 1 (i), ta có

$$
f(H_i) =\frac{1}{2}(e_ie_{-i}-e_{-i}e_i)
$$

Vì $e_ie_{-i}=-e^2_0e_ie_{-i}=e_0e_ie_0e_{-i}$ và $e_ie_{-i}+e_{-i}e_i= 1$, ta có

$_{-1}$ 1 1

$$
\mu\circ f(H_i) =-e_{-i}e_i=-+e_ie_{-i}
$$

2 2 Ta suy ra rằng, với $1\leq i_1<\cdots < i_k\leq l:$

$\rho (H)(e\wedge  \cdots  \wedge e) =\{-\frac{1}{2}e_{-i_1}\wedge  \cdots  \wedge e_{-i_k}$ nếu $i\in  \{i_1, . . . , i_k\}$

$^{i-i_1}-_{i_k}\frac{1}{2}e_{-i_1}\wedge  \cdots  \wedge e_{-i_k}$ nếu $i \notin  \{i_1, . . . i_k\}$

và với $h\in \mathfrak{h}$

$$
\rho (h)(e_{-i_1}\wedge  \cdots  \wedge e_{-i_k}) \tag{5}
$$

$$
= (\frac{1}{2}(\varepsilon_1+\cdots +\varepsilon_l)-(\varepsilon_{i_1}+\cdots +\varepsilon_{i_k}))(h)(e_{-i_1}\wedge  \cdots  \wedge e_{-i_k})
$$

Điều này cho thấy rằng trọng số cao nhất của $\rho$ là $\varpi_l$. Ta gọi $\rho$ là biểu diễn spinor của $\mathfrak{g}$. Chú ý rằng các trọng số của nó đều đơn (hơn nữa, $\varpi_l$ là một trọng lượng minuscule).

(V) Ta có $w_0=-1$, do đó mọi biểu diễn đơn hữu hạn chiều của $\mathfrak{g}$ đều trực giao hoặc symplectic. Theo Chap. VI, §4, no. 5.VI, tổng các tọa độ của $\varpi_r$ đối với $(\alpha_1, . . . , \alpha_l)$ là nguyên với $1\leq r\leq l-1:$ do đó, biểu diễn $\bigwedge^r\sigma$ là trực giao. Hơn nữa, nó bất biến đối với mở rộng $\Psi_{(r)}$ của $\Psi$ lên $\bigwedge^rV$.

Đối với biểu diễn spinor, tổng các tọa độ của $\varpi_l$ đối với $(\alpha_1, . . . , \alpha_l)$ là $\frac{1}{2}(1 +\cdots +l) =\frac{l(l+1)}{4}($loc. cit.). Vì vậy, nó trực giao đối với $l\equiv 0$ hoặc $-1$ (mod. 4) và symplectic đối với $l\equiv 1$ hoặc 2 (mod. 4). Thực vậy, xét dạng song tuyến tính $\Phi$ trên $N =\bigwedge F'$ được xác định như sau: nếu $x\in \bigwedge^pF'$ và $y\in \bigwedge^qF'$, đặt $\Phi (x, y) = 0$ nếu $p+q\not=l$ và

$$
x\wedge y= (-1)^{^{p(p+1)}_2}\Phi (x, y)e_{-1}\wedge  \cdots  \wedge e_{-r}
$$

nếu $p+q=l$. Dễ dàng kiểm tra được rằng $\Phi$ là không suy biến và là trực giao đối với $l\equiv 0,-1$ (mod. 4) và phản xứng đối với $l\equiv 1,2$ (mod. 4). Mặt khác, theo Bổ đề 1 (i),

$$
f(X_{\varepsilon_i}) =e_0e_i,f(X_{-\varepsilon_i}) =-e_0e_{-i}
$$

với $1\leq i\leq l$ và

$$
f(X_{\varepsilon_i-\varepsilon_j}) =\frac{1}{2}(e_ie_{-j}-e_{-j}e_i) =e_ie_{-j}=e_0e_ie_0e_{-j}
$$

với $1\leq i < j\leq l$, và tương tự

$$
f(X_{\varepsilon_j-\varepsilon_i}) =-e_0e_je_0e_{-i}, f(X_{\varepsilon_i+\varepsilon_j}) =e_0e_ie_0e_j, f(X_{-\varepsilon_i-\varepsilon_j}) =e_0e_{-i}e_0e_{-j}
$$

do đó

$$
\mu^{-1}\circ f(X_{\varepsilon_i}) =e_i,\mu^{-1}f(X_{-\varepsilon_i}) =-e_{-i}
$$

và

$\mu^{-1}\circ f(X_{\pm\varepsilon_i\pm\varepsilon_j}) =ce_{\pm i}e_{\pm j}$ với $1\leq i, j\leq l, i\not=j$ và $c\in  \{1,-1\}$. Bây giờ việc kiểm tra rằng $\Phi$ thực sự là $\mathfrak{g}$-bất biến là không còn khó khăn (xem Bài tập 18).

(VI) Với $x\in \mathfrak{g}$, đa thức đặc trưng của $\sigma (x)$ có dạng

$$
T^{2l+1}+f_1(x)T^{2l}+f_2(x)T^{2l-1}+\cdots +f_{2l+1}(x)
$$

trong đó $f_1, . . . , f_{2l+1}$ là các hàm đa thức bất biến trên $\mathfrak{g}$.

Nếu $x=\xi_1H_1+\cdots +\xi_lH_l\in \mathfrak{h}$, thì các $f_i(x)$, sai khác một dấu, là các hàm đối xứng sơ cấp của $\xi_1, . . . , \xi_l,-\xi_1, . . . ,-\xi_l$; các hàm đối xứng này bằng không ở các bậc lẻ, và

$$
T^{2l+1}+f_2(x)T^{2l-1}+f_4(x)T^{2l-3}+\cdots +f_{2l}(x)T = T(T^2-\xi_1^2). . .(T^2-\xi^2_l)
$$

do đó $f_2, . . . , f_{2l}$, sai khác một dấu, là các hàm đối xứng sơ cấp của $\xi_1^2, . . . , \xi_l^2$, là các phần tử sinh độc lập đại số của $\mathbf{S}(\mathfrak{h}^*)^W$ (Chương VI, §4, no. 5.IX). Theo §8, no. 3, Định lý 1 (i), ta thấy rằng $f_1=f_3=f_5=\cdots = 0$ và $(f_2, f_4, . . . , f_{2l})$ là một họ tự do đại số sinh ra đại số các hàm đa thức bất biến trên $\mathfrak{g}$.

(VII) Vì tự đẳng cấu duy nhất của đồ thị Dynkin là đồng nhất, ta có Aut($\mathfrak{g}$) $=$ Aut$_0(\mathfrak{g})$.

Cho $\Sigma$ là nhóm các phép đồng dạng của V đối với $\Psi$. Với mọi $g\in \Sigma$, đặt $\varphi (g)$ là tự đẳng cấu $x \rightarrow gxg^{-1}$ của $\mathfrak{g}$. Khi đó $\varphi$ là một đồng cấu từ $\Sigma$ vào Aut($\mathfrak{g}$). Ta chứng minh rằng nó là toàn ánh. Cho $\alpha \in$ Aut($\mathfrak{g}$) $=$ Aut$_0(\mathfrak{g})$. Theo Mệnh đề 2 của §7, no. 1, tồn tại $s\in \mathbf{G}\mathbf{L}(V)$ sao cho $\alpha (x) =sxs^{-1}$ với mọi $x\in \mathfrak{g}$. Khi đó $s$ biến $\Psi$ thành một dạng song tuyến tính $\Psi '$ trên V bất biến đối với $\mathfrak{g}$, và do đó tỉ lệ với $\Psi ($§7, no. 5, Mệnh đề 12). Điều này chứng minh rằng $s\in \Sigma$.

Vì biểu diễn đồng nhất của $\mathfrak{g}$ là bất khả quy, hoán tập của nó thu gọn về các vô hướng (§6, no. 1, Mệnh đề 1), nên hạt nhân của $\varphi$ là $k^*$. Do đó nhóm Aut($\mathfrak{g}$) $=$ Aut$_0(\mathfrak{g})$ có thể được đồng nhất với $\Sigma /k^*$. Nhưng, từ Đại số, Chương IX, §6, no. 5 suy ra rằng nhóm $\Sigma$ là tích của các nhóm $k^*$ và $\mathbf{S}\mathbf{O}(\Psi )$; vì vậy Aut($\mathfrak{g}$) $=$ Aut$_0(\mathfrak{g})$ có thể được đồng nhất với $\mathbf{S}\mathbf{O}(\Psi )$.

Cho $\mathbf{O}^+_0(\Psi )$ là nhóm trực giao thu gọn của $\Psi ($Đại số, Chương IX, §9, no. 5). Vì $\mathbf{S}\mathbf{O}(\Psi )/\mathbf{O}^+_0(\Psi )$ là giao hoán (loc. cit.), nhóm Aut$_e(\mathfrak{g})$ được chứa trong $\mathbf{O}^+_0(\Psi ) ($§11, no. 2, Mệnh đề 3); thực ra, nó bằng nhóm đó (Bài tập 7).

(VIII) Dạng song tuyến tính chính tắc $\Phi_R$ trên $\mathfrak{h}^*$ được cho bởi

$\Phi_R(\xi_1\varepsilon_1+\cdots +\xi_l\varepsilon_l, \xi '\varepsilon_1+\cdots +\xi '\varepsilon_l) =$ 1 $(\xi_1\xi '+\cdots +\xi_l\xi ')$

$$
^1l\overline{4l- 2}^1l
$$

(Chương VI, §4, no. 5.V). Đẳng cấu từ $\mathfrak{h}$ đến $\mathfrak{h}^*$ được xác định bởi $\Phi_R$ biến $H_i$ thành $(4l-2).\varepsilon_i$. Vì vậy, dạng nghịch đảo của $\Phi_R$, nghĩa là hạn chế trên $\mathfrak{h}$ của dạng Killing, là

$$
\Phi (\xi_1H_1+\cdots +\xi_lH_l, \xi '_1H_1+\cdots +\xi '_lH_l) = (4l-2)(\xi_1\xi '_1+\cdots +\xi_l\xi '_l)
$$

(IX) Nhắc lại $X_{\alpha}(\alpha \in R)$ được xác định bởi các công thức (3). Dễ dàng kiểm tra rằng $[X_{\alpha}, X_{-\alpha}] =-H_{\alpha}$ với $\alpha \in R$. Mặt khác, cho M là ma trận $I+E_{0,0}$; vì $M=S^tM^{-1}S$, ánh xạ

$$
\theta :g \rightarrow  -M^{-1t}gM
$$

là một tự đẳng cấu của $\mathfrak{g}$ và $\theta (X_{\alpha}) =X_{-\alpha}$ với mọi $\alpha \in R$. Do đó, $(X_{\alpha})$ là một hệ Chevalley trong $(\mathfrak{g},\mathfrak{h})$.

Giả sử rằng $k=\mathbf{Q}$. Đại số con Cartan $\mathfrak{h}$ có hai dàn khả dĩ: dàn $Q(R^{\vee})$ sinh bởi các $H_{\alpha}$ và dàn $P(R^{\vee})$ được sinh bởi các $H_i$ và gồm các ma trận đường chéo trong $\mathfrak{h}$ có các phần tử là số nguyên. Suy ra rằng $\mathfrak{o}_S(2l+ 1,\mathbf{Z})$ (tập hợp các ma trận trong $\mathfrak{g}$ có các phần tử là số nguyên) là cấp Chevalley $P(R^{\vee}) +\sum\mathbf{Z}.X_{\alpha}$ trong $\mathfrak{g}$. Vì $(X_{\pm\varepsilon_i})^2= 2E_{\pm i,\mp i},(X_{\pm\varepsilon_i})^3= 0$ và $(X_{\pm\varepsilon_i\pm\varepsilon_j})^2= 0$, ta thấy rằng dàn $\mathscr{V}$ được sinh bởi cơ sở Witt $(e_i)_{-l\leq i\leq l}$ là một dàn khả dung cho $\mathfrak{o}_S(2l+ 1,\mathbf{Z})$ trong V. Điều tương tự cũng đúng đối với $\bigwedge^r\mathscr{V}$ trong $\bigwedge^rV$.

Bây giờ xét biểu diễn spinơ $\rho$ của $\mathfrak{g}$ trên $N =\bigwedge F'$. Vì các trọng của nó không biến $P(R^{\vee})$ thành $\mathbf{Z}$, nó không có dàn khả dung cho $\mathfrak{o}_S(2l+ 1,\mathbf{Z})$. Mặt khác, dàn $\mathscr{N}$ được sinh bởi cơ sở chính tắc $(e_{-i_1}\wedge  \cdots  \wedge e_{-i_k})$ của N (với $1\leq i_1<\cdots < i_k\leq l$) là một dàn khả dung cho cấp Chevalley $\mathscr{G}= Q(R^{\vee}) +\sum_{\alpha\in R}\mathbf{Z}.X_{\alpha}$. Thật vậy, ngay lập tức thấy rằng $\mathscr{N}$ ổn định dưới

phép tích ngoài với các $e_{-i}$ và phép tích trong với các $e_i$ (với $1\leq i\leq l$). Các công thức của (V) khi đó cho thấy rằng $\mathscr{N}$ ổn định dưới $\rho (\mathscr{G})$. Hơn nữa, vì $\rho (X_{\alpha})^2= 0$ với mọi $\alpha \in R$, suy ra rằng $\mathscr{N}$ là khả dung.

### 3. ĐẠI SỐ KIỂU C$_{\boldsymbol{l}}$ ($\boldsymbol{l}\geq$ 1)

(I) Cho $\Psi$ là một dạng song tuyến tính phản xứng không suy biến trên một không gian vectơ V có số chiều hữu hạn $2l\geq 2$; tập hợp các tự đồng cấu $x$ của V sao cho $\Psi (xv, v') +\Psi (v, xv') = 0$ với mọi $v, v'\in V$ là một đại số con Lie nửa đơn của $\mathfrak{s}\mathfrak{l}(V)$ (Ch. I, §6, no. 7, Prop. 9). Ta ký hiệu nó bởi $\mathfrak{s}\mathfrak{p}(\Psi )$ và gọi nó là đại số Lie symplectic liên kết với $\Psi$.

Theo Algebra, Cap. IX, §4, no. 2, V có thể được viết thành tổng trực tiếp của hai không gian con hoàn toàn đẳng hướng cực đại F và $F'$, chúng đối ngẫu với nhau đối với $\Psi$. Cho $(e_i)_{1\leq i\leq l}$ là một cơ sở của F, và $(e_{-i})_{1\leq i\leq l}$ là cơ sở đối ngẫu của $F'$. Khi đó

$$
(e_1, . . . , e_l, e_{-l}, . . . , e_{-1})
$$

là một cơ sở của V; ta nói rằng nó là một cơ sở Witt (hay cơ sở symplectic) của V. Ma trận của $\Psi$ đối với cơ sở này là ma trận bình phương cấp $2l$

$$
(0s)
$$

$J=-s$ 0

trong đó $s$ là ma trận vuông cấp $l$ mà mọi phần tử đều bằng không, ngoại trừ các phần tử trên đường chéo thứ hai đều bằng 1, xem no. 2.I.

Đại số $\mathfrak{g}=\mathfrak{s}\mathfrak{p}(\Psi )$ có thể được đồng nhất với đại số $\mathfrak{s}\mathfrak{p}(2l, k)$ gồm các ma trận vuông $a$ cấp $2l$ sao cho $a=-J^{-1t}aJ=J^taJ($Algebra, Chap. IX, §1, no. 10, formulas (50)), tức là có dạng

$$
(AB)
$$

$$
a=C-s^tAs
$$

trong đó $A, B, C$ là các ma trận vuông cấp $l$ sao cho $B=s^tBs$ và $C=$ $c^tCs$; nói cách khác, $B$ và $C$ đối xứng đối với đường chéo thứ hai. Do đó

dim$\mathfrak{g}=l^2+ 2\frac{l(l + 1)}{2}=l(2l+ 1)$.

Cho $\mathfrak{h}$ là tập hợp các ma trận đường chéo trong $\mathfrak{g}$. Đây là một đại số con giao hoán của $\mathfrak{g}$, với cơ sở gồm các phần tử $H_i=E_{i,i}-E_{-i,-i}$ với $1\leq i\leq l$. Gọi $(\varepsilon_i)_{1\leq i\leq l}$ là cơ sở đối ngẫu của $(H_i)$. Với $1\leq i < j\leq l$, đặt

$X_{2\varepsilon_i}$ = $E_{i,-i}$

$X_{-2\varepsilon_i}$ = $-E_{-i,i}$

$X_{\varepsilon_i-\varepsilon_j}$ = $E_{i,j}-E_{-j,-i}$

$X_{-\varepsilon_i+\varepsilon_j}$ = $-E_{j,i}+E_{-i,-j}$ (6)

$X_{\varepsilon_i+\varepsilon_j}$ = $E_{i,-j}+E_{j,-i}$

$X_{-\varepsilon_i-\varepsilon_j}$ = $-E_{-i,j}-E_{-j,i}$.

Dễ dàng kiểm tra rằng các phần tử này tạo thành một cơ sở của một phần bù của $\mathfrak{h}$ trong $\mathfrak{g}$ và rằng, với $h\in \mathfrak{h}$,

$$
[h, X_{\alpha}] =\alpha (h)X_{\alpha} \tag{7}
$$

với mọi $\alpha \in R$, trong đó R là tập hợp các $\pm 2\varepsilon_i$ và các $\pm \varepsilon_i\pm \varepsilon_j(i < j)$. Do đó $\mathfrak{h}$ bằng bộ chuẩn hóa của chính nó trong $\mathfrak{g}$, và vì thế là một đại số con Cartan của $\mathfrak{g}$, $\mathfrak{h}$ là tách, và các nghiệm của $(\mathfrak{g},\mathfrak{h})$ là các phần tử của R. Hệ nghiệm R của $(\mathfrak{g},\mathfrak{h})$ có kiểu $C_l$ với $l\geq 2$, và có kiểu $A_1$ (nói cách khác, kiểu $C_1$) với $l= 1$ (Chap. VI, §4, no. 6.I mở rộng cho trường hợp $l= 1$). Do đó, $\mathfrak{g}$ là một đại số Lie đơn tách được kiểu $C_l$.

Mọi đại số con Cartan tách của $\mathfrak{g}$ đều được biến đổi thành $\mathfrak{h}$ bởi một tự đẳng cấu sơ cấp, do đó bởi một phần tử của nhóm symplectic $\mathbf{S}\mathbf{p}(\Psi )$ (xem (VII)), và do đó là tập hợp $\mathfrak{h}_{\beta}$ gồm các phần tử của $\mathfrak{g}$ mà ma trận của chúng đối với một cơ sở Witt $\beta$ của $\mathfrak{g}$ là đường chéo. Ngay lập tức kiểm tra được rằng các không gian vectơ con duy nhất của V ổn định dưới $\mathfrak{h}_{\beta}$ là những không gian được sinh bởi một tập con của $\beta$.

Ta có $\mathfrak{s}\mathfrak{p}(2, k) =\mathfrak{s}\mathfrak{l}(2, k)$. Mặt khác, các đại số $\mathfrak{s}\mathfrak{p}(4, k)$ và $\mathfrak{o}_S(5, k)$ có cùng hệ nghiệm, và do đó đẳng cấu (xem Bài tập 3). Từ đây về sau, ta giả sử rằng $l\geq 2$.

(II) Hệ nghiệm $R^{\vee}$ được xác định theo Chương VI, §4, no. 6.I và 6.V; ta có

$$
H_{2\varepsilon_i}=H_i, H_{\varepsilon_i-\varepsilon_j}=H_i-H_j, H_{\varepsilon_i+\varepsilon_j}=H_i+H_j
$$

(III) Đặt $\alpha_1=\varepsilon_1-\varepsilon_2, . . . , \alpha_{l-1}=\varepsilon_{l-1}-\varepsilon_l, \alpha_l= 2\varepsilon_l$. Theo Chương VI, §4, no. 6.II, $\{\alpha_1, . . . , \alpha_l\}$ là một cơ sở B của R; các nghiệm dương đối với B là $2\varepsilon_i$ và $\varepsilon_i\pm \varepsilon_j(i < j)$. Đại số con Borel tương ứng $\mathfrak{b}$ là tập hợp các ma trận tam giác trên trong $\mathfrak{g}$.

Cho $\delta$ là một cờ đẳng hướng trong V (nghĩa là các phần tử của nó đều là các không gian con hoàn toàn đẳng hướng đối với $\Psi$), và cho $\mathfrak{p}_{\delta}$ là đại số con gồm các phần tử của $\mathfrak{g}$ làm cho các phần tử của $\delta$ ổn định. Ta chứng minh như trong no. 2.III rằng ánh xạ $\delta  \rightarrow \mathfrak{p}_{\delta}$ là một song ánh từ tập hợp các cờ đẳng hướng (resp. các cờ đẳng hướng cực đại) lên tập hợp các đại số con parabolic (resp. Borel) của $\mathfrak{g}$; ta có $\mathfrak{p}_{\delta}\supset \mathfrak{p}_{\delta'}$ khi và chỉ khi $\delta \subset \delta '$.

(IV) Các trọng số cơ bản tương ứng với $\alpha_1, . . . , \alpha_l$ là, theo Chương VI, §4, no. 6.VI, $\varpi_i=\varepsilon_1+\cdots +\varepsilon_i(1\leq i\leq l)$.

Ta sẽ chỉ ra cách biểu diễn cơ bản $\sigma_r$ có trọng số $\varpi_r$ có thể được thực hiện như một biểu diễn con của $\bigwedge^r\sigma$, trong đó $\sigma$ là biểu diễn đồng nhất của $\mathfrak{g}$ trên V, và để làm điều đó ta sẽ nghiên cứu phân tích của biểu diễn $\bigwedge\sigma$ của $\mathfrak{g}$ trên đại số ngoài $\bigwedge V$.

Gọi $(e^*_i)$ là cơ sở của $V^*$ đối ngẫu với $(e_i)$. Dạng song tuyến tính phản xứng $\Psi$ có thể được đồng nhất với một phần tử $\Gamma^*\in \bigwedge^2V^*($Algebra, Chap. III, §7, no. 4, Prop. 7 and §11, no. 10) và dễ dàng kiểm tra rằng

$$
\Gamma^*=-\sum_{i=1}^le^*_i\wedge e^*_{-i}
$$

Gọi $\Psi^*$ là dạng nghịch đảo của $\Psi$ (Algebra, Chương IX, §1, no. 7); ngay lập tức có

$$
\Psi^*(e^*_i, e^*_j) = 0
$$

với $i\not=-j$ và $\Psi^*(e^*_i, e^*_{-i}) =-1$ với $1\leq i\leq l$. Nếu ta đồng nhất $\Psi^*$ với một phần tử $\Gamma \in \bigwedge^2V$, thì

$$
\Gamma =\sum_{i=1}^le_i\wedge e_{-i}
$$

Ký hiệu $X_-$ là tự đồng cấu của $\bigwedge V$ cho bởi phép nhân ngoài trái với $\Gamma$ và $X_+$ là tự đồng cấu của $\bigwedge V$ cho bởi phép nhân trong trái với $-\Gamma^*:$

$$
X_-u=(\sum_{i=1}^le_i\wedge e_{-i})\wedge u
$$

$$
X_+u=(\sum_{i=1}^le^*_i\wedge e^*_{-i})\wedge u
$$

Để tính $X_+$ và $X_-$, đưa vào một cơ sở của $\bigwedge V$ theo cách sau: với mọi bộ ba $(A,B,C)$ được tạo bởi ba tập con rời nhau của $1, l$, đặt

$$
e_{A,B,C}=e_{a_1}\wedge  \cdots  \wedge e_{a_m}\wedge e_{-b_1}\wedge  \cdots  \wedge e_{-b_n}\wedge e_{c_1}\wedge e_{-c_1}\wedge  \cdots  \wedge e_{c_p}\wedge e_{-c_p}
$$

trong đó $(a_1, . . . , a_m)$ (tương ứng $(b_1, . . . , b_n),(c_1, . . . , c_p)$) là các phần tử của A (tương ứng $B,C$) được sắp xếp theo thứ tự tăng. Ta thu được theo cách này một cơ sở của $\bigwedge V$ và các phép tính đơn giản cho thấy rằng

$$
X_-.e_{A,B,C}=\sum e_{A,B,C\cup \{j\}} \tag{8}
$$

$j\in 1,l ,j \notin A\cup B\cup C$

$$
X_+.e_{A,B,C}=-\sum_{j\in C}e_{A,B,C-\{j\}} \tag{9}
$$

Gọi $H$ là tự đồng cấu của $\bigwedge V$ thu gọn thành phép nhân với $(l-r)$ trên $\bigwedge^rV (0\leq r\leq 2l)$. Không khó để kiểm tra (xem Bài tập 19) rằng

$$
[X_+, X_-] =-H
$$

$$
[H, X_+] = 2X_+
$$

$$
[H, X_-] =-2X_-
$$

Nói cách khác, không gian con vectơ $\mathfrak{s}$ sinh bởi $X_+, X_-$ và $H$ là một đại số Lie con của End($\bigwedge V$), đẳng cấu với $\mathfrak{s}\mathfrak{l}(2, k)$, và $\bigwedge^rV$ là không gian con của các phần tử có trọng số $l-r$. Ký hiệu $E_r$ là không gian con của $\bigwedge^rV$ gồm các phần tử nguyên thủy, nghĩa là, $E_r= (\bigwedge^rV)\cap$ Ker$X_+$. Suy ra từ §1 rằng, với $r < l$, hạn chế của $X_-$ trên $\bigwedge^rV$ là đơn ánh và rằng, với $r\leq l$, $\bigwedge^rV$ phân tích thành một tổng trực tiếp

$$
\bigwedge^rV = E_r\oplus X_-(E_{r-2})\oplus X_-^2(E_{r-4})\oplus  \cdots
$$

$$
= E_r\oplus X_-(\bigwedge^{r-2}V)
$$

Điều này đặc biệt cho thấy rằng dim $E_r=(^{2l}_r)-(_{r-2}^{2l})$ với $0\leq r\leq l$.

Mặt khác, chính định nghĩa của $\mathfrak{s}\mathfrak{p}(\Psi )$ cho thấy rằng $\Gamma^*$ bị triệt tiêu bởi lũy thừa ngoại thứ hai của đối ngẫu của $\sigma$. Tương tự, $\Gamma$ bị triệt tiêu bởi $\bigwedge^2\sigma$. Do đó, ngay lập tức suy ra rằng $X_+$ và $X_-$, và do đó cả $H$, giao hoán với các tự đồng cấu $\bigwedge\sigma (g)$ với $g\in \mathfrak{g}$. Do đó, các không gian con $E_r$ với $0\leq r\leq l$ ổn định dưới $\bigwedge^r\sigma$; ta sẽ chứng minh rằng hạn chế của $\bigwedge^r\sigma$ trên $E_r$ là một biểu diễn cơ bản $\sigma_r$ có trọng số $\varpi_r(1\leq r\leq l)$.

Trước hết, ta nhận xét rằng các trọng số của $\bigwedge^r\sigma$ đối với $\mathfrak{h}$ là

$$
\varepsilon_{i_1}+\cdots +\varepsilon_{i_k}-(\varepsilon_{j_1}+\cdots +\varepsilon_{j_{r-k}})
$$

trong đó $i_1, . . . , i_k$ (tương ứng $j_1, . . . , j_{r-k}$) là các phần tử phân biệt của $1, l$; do đó, trọng số cao nhất của $\bigwedge^r\sigma$ thực sự là

$$
\varpi_r=\varepsilon_1+\cdots +\varepsilon_r
$$

và các vectơ có trọng số $\overline{\varpi}_r$ là những vectơ tỉ lệ với $e_1\wedge\cdots\wedge e_r=e_{\{1,\ldots,r\},\varnothing,\varnothing}$. Công thức (9) cho thấy rằng $e_1\wedge\cdots\wedge e_r\in E_r$. Do đó, chỉ cần chứng minh rằng hạn chế của $\bigwedge^r\sigma$ trên $E_r$ là bất khả quy.

Nếu $s\in\mathbf{Sp}(\Psi)$, mở rộng của $s$ lên $\bigwedge V$ (tương ứng $\bigwedge V^*$) giữ cố định $\Gamma$ (tương ứng $\Gamma^*$), và do đó giao hoán với $X_+$ và $X_-$ và giữ $E_r$ ổn định. Do đó, $E_r$ chứa không gian vectơ con $F_r$ sinh bởi các ảnh của $e_1\wedge\cdots\wedge e_r$ qua $\mathbf{Sp}(\Psi)$. Định lý Witt cho thấy rằng đó là các $r$-vectơ phân tích được khác không sao cho không gian vectơ con tương ứng của $V$ là một không gian con hoàn toàn đẳng hướng, các $r$-vectơ mà ta sẽ gọi là đẳng hướng.

#### Bổ đề 2 {#lie-viii-s13-lem-2 .statement tag=01K8}

Với $1\leq r\leq\ell$, cho $F_r$ là không gian con của $\bigwedge^r V$ sinh bởi các $r$-vectơ đẳng hướng. Khi đó

$$
\bigwedge^r V=F_r+X_-\left(\bigwedge^{r-2}V\right)
=F_r+\left(\sum_{i=1}^{\ell}e_i\wedge e_{-i}\right)\wedge\bigwedge^{r-2}V.
$$

Trước hết ta chứng minh cách Bổ đề 2 suy ra mệnh đề của ta. Vì $F_r\subset E_r$ và $E_r\cap X_-\left(\bigwedge^{r-2}V\right)=\{0\}$, bổ đề suy ra rằng $F_r=E_r$. Mặt khác, cho $s\in\mathbf{Sp}(\Psi)$; tự đẳng cấu $a\mapsto sas^{-1}$ của $\operatorname{End}(V)$ bảo toàn $\mathfrak{g}$ và cảm sinh trên nó một phần tử của $\operatorname{Aut}_0(\mathfrak{g})$ (xem (§7, no. 1, Mệnh đề 2), và do đó biến mọi biểu diễn bất khả quy của $\mathfrak{g}$ thành một biểu diễn tương đương (§7, no. 1, Mệnh đề 2). Vì $e_1\wedge\cdots\wedge e_r$ thuộc một thành phần bất khả quy của $\bigwedge^r\sigma$, và vì $E_r=F_r$ được sinh bởi các ảnh của $e_1\wedge\cdots\wedge e_r$ qua $\mathbf{Sp}(\Psi)$, suy ra biểu diễn của $\mathfrak{g}$ trên $E_r$ là đẳng kiểu. Nhưng bội số của trọng số cao nhất của nó $\overline{\varpi}_r$ là $1$, do đó nó là bất khả quy.

Còn lại là chứng minh bổ đề. Điều này hiển nhiên đối với $r=1$. Ta lập luận bằng quy nạp, và giả sử rằng $r\geq 2$. Theo giả thiết quy nạp, ta quy về việc chứng minh rằng

$$
F_{r-1}\wedge V\subset F_r+\Gamma\wedge\bigwedge^{r-2}V,
$$

hay rằng, nếu $y$ là một $(r-1)$-vectơ phân tích được và $x\in V$, thì

$$
z=y\wedge x\in F_r+\Gamma\wedge\bigwedge^{r-2}V.
$$

Cho $(f_i)_{1\leq\pm i\leq\ell}$ là một cơ sở Witt của $V$ sao cho $y=f_1\wedge\cdots\wedge f_{r-1}$. Chỉ cần thực hiện chứng minh khi $x=f_i$. Nếu $i\notin[1-r,-1]$, $r$-vectơ $f_1\wedge\cdots\wedge f_{r-1}\wedge f_i$ là đẳng hướng. Ngược lại, ta có thể giả sử, bằng cách đánh lại số các $f_i$ nếu cần, rằng $i=1-r$. Khi đó $\Gamma=\displaystyle\sum_{j=1}^{\ell}f_j\wedge f_{-j}$, do đó

$$
f_{r-1}\wedge f_{1-r}
=
\frac{1}{\ell-r+2}
\left(
\Gamma-\sum_{i=1}^{r-2}f_i\wedge f_{-i}
+\sum_{j=r}^{\ell}(f_{r-1}\wedge f_{1-r}-f_j\wedge f_{-j})
\right),
$$

$$
z=
\frac{1}{\ell-r+2}\Gamma\wedge f_1\wedge\cdots\wedge f_{r-2}
+
\frac{1}{\ell-r+2}\sum_{j=r}^{\ell}
(f_1\wedge\cdots\wedge f_{r-2})\wedge
(f_{r-1}\wedge f_{1-r}-f_j\wedge f_{-j}).
$$

Nhưng

$$
f_{r-1}\wedge f_{1-r}-f_j\wedge f_{-j}= (f_{r-1}+f_j)\wedge (f_{1-r}-f_{-j})-f_j\wedge f_{1-r}+f_{r-1}\wedge f_{-j}
$$

và ta kiểm tra ngay lập tức rằng các $r$-vectơ

$$
f_1\wedge  \cdots  \wedge f_{r-2}\wedge (f_{r-1}+f_j)\wedge (f_{1-r}-f_{-j})
$$

$f_1\wedge  \cdots  \wedge f_{r-2}\wedge f_j\wedge f_{1-r}$ và $f_1\wedge  \cdots  \wedge f_{r-1}\wedge f_{-j}$

là đẳng hướng đối với $r\leq j\leq l$. Do đó, $z\in F_r+\Gamma \wedge \bigwedge^{r-2}V$, điều này hoàn tất chứng minh.

(V) Ta có $w_0=-1$, do đó mọi biểu diễn đơn hữu hạn chiều của $\mathfrak{g}$ đều là trực giao hoặc symplectic. Theo Chương VI, §4, no. 6.VI, tổng các tọa độ của $\varpi_r$ đối với $(\alpha_1, . . . , \alpha_l)$ là

$$
r
$$

$$
1 + 2 +\cdots + (r-1) +r+r+\cdots +r+
$$

2

do đó $\sigma_r$ là trực giao đối với $r$ chẵn và symplectic đối với $r$ lẻ.

Vì $e_1\wedge  \cdots  \wedge e_r$ và $e_{-1}\wedge  \cdots  \wedge e_{-r}$ thuộc $E_r$ và vì

$$
\Psi_{(r)}(e_1\wedge  \cdots  \wedge e_r, e_{-1}\wedge  \cdots  \wedge e_{-r}) = 1
$$

ta thấy rằng hạn chế của $\Psi_{(r)}$ trên $E_r$ là khác không: nó, sai khác một nhân tử hằng, chính là dạng song tuyến tính; nó đối xứng nếu $r$ chẵn, phản xứng nếu $r$ lẻ, và bất biến dưới $\sigma_r$.

(VI) Với mọi $x\in \mathfrak{g}$, đa thức đặc trưng của $\sigma (x)$ có dạng

$$
T^{2l}+f_1(x)T^{2l-1}+\cdots +f_{2l}(x)
$$

trong đó $f_1, . . . , f_{2l}$ là các hàm đa thức bất biến trên $\mathfrak{g}$.

Nếu $x=\xi_1H_1+\cdots +\xi_lH_l\in \mathfrak{h}$, thì $f_i(x)$, sai khác dấu, là các hàm đối xứng sơ cấp của $\xi_1, . . . , \xi_l,-\xi_1, . . . ,-\xi_l$; các hàm đối xứng này bằng không ở các bậc lẻ, và

$$
T^{2l}+f_2(x)T^{2l-2}+\cdots +f_{2l}(x) = (T^2-\xi_1^2). . .(T^2-\xi^2_l)
$$

Như trong no. 2.VI, suy ra rằng $f_1=f_3=f_5=\cdots = 0$, và

$$
(f_2, f_4, . . . , f_{2l})
$$

là một họ tự do đại số sinh đại số các hàm đa thức bất biến trên $\mathfrak{g}$.

(VII) Vì tự đẳng cấu duy nhất của đồ thị Dynkin là đồng nhất, ta có Aut($\mathfrak{g}$) $=$ Aut$_0(\mathfrak{g})$.

Gọi $\Sigma$ là nhóm các phép đồng dạng của V đối với $\Psi ($Đại số, Chap. IX, §6, end of no. 5). Ta chứng minh như trong no. 2.VII rằng các tự đẳng cấu của $\mathfrak{g}$ là các ánh xạ $x \rightarrow sxs^{-1}$ với $s\in \Sigma$, do đó Aut($\mathfrak{g}$) $=$ Aut$_0(\mathfrak{g})$ có thể được đồng nhất với $\Sigma /k^*$.

Với mọi $s\in \Sigma$, gọi $\mu(s)$ là nhân tử của $s$. Ánh xạ $s \rightarrow \mu(s)$ mod $k^{*2}$ từ $\Sigma$ vào $k^*/k^{*2}$ là một đồng cấu có hạt nhân chứa $k^*.1$, và do đó cho một đồng cấu $\lambda$ từ $\Sigma /k^*$ vào $k^*/k^{*2}$. Ta có $\mathbf{S}\mathbf{p}(\Psi )\cap k^*=\{1,-1\}$. Xét dãy các đồng cấu

1 $\longrightarrow \mathbf{S}\mathbf{p}(\Psi )/\{1,-1\}\longrightarrow^{\iota}\Sigma /k^*\longrightarrow^{\lambda}k^*/k^{*2}\longrightarrow 1$. (10) Ánh xạ $\iota$ là đơn ánh, và Im($\iota$ )$\subset$ Ker$\lambda$ vì nhân tử của một phần tử của $\mathbf{S}\mathbf{p}(\Psi )$ là 1. Nếu nhân tử của $s\in \Sigma$ là một phần tử của $k^{*2}$, tồn tại $\nu \in k^*$ sao cho $\nu s\in \mathbf{S}\mathbf{p}(\Psi )$; do đó, Im($\iota$ ) $=$ Ker($\lambda$ ). Tóm lại, dãy (10) là khớp. Ta đồng nhất $\mathbf{S}\mathbf{p}(\Psi )/\{1,-1\}$ với một nhóm con của $\Sigma /k^*$. Vì $k^*/k^{*2}$ là giao hoán, $\mathbf{S}\mathbf{p}(\Psi )/\{1,-1\}$ chứa nhóm dẫn xuất của $\Sigma /k^*$. Do đó, Aut$_e(\mathfrak{g})$ được chứa trong $\mathbf{S}\mathbf{p}(\Psi )/\{1,-1\}($§11, no. 2, Mệnh đề 3). Thực ra, nó bằng nhóm này, và Aut($\mathfrak{g}$)$/$Aut$_e(\mathfrak{g})$ được đồng nhất với $k^*/k^{*2}$ (Bài tập 9).

(VIII) Dạng song tuyến tính chính tắc $\Phi_R$ trên $\mathfrak{h}^*$ được cho bởi

$$
\Phi_R(\xi_1\varepsilon_1+\cdots +\xi_l\varepsilon_l, \xi '_1\varepsilon_1+\cdots +\xi '_l\varepsilon_l) =\frac{1}{4(l + 1)}(\xi_1\xi '_1+\cdots +\xi_l\xi '_l)
$$

(Chương VI, §4, no. 6.V). Do đó, dạng nghịch đảo của $\Phi_R$, tức là hạn chế của dạng Killing lên $\mathfrak{h}$, là

$$
\Phi (\xi_1H_1+\cdots +\xi_lH_l, \xi '_1H_1+\cdots +\xi '_lH_l) = 4(l+ 1)(\xi_1\xi '_1+\cdots +\xi_l\xi '_l)
$$

(IX) Nhắc lại các $X_{\alpha}$ được xác định bởi các công thức $(6) (\alpha \in R)$. Dễ dàng kiểm tra rằng $[X_{\alpha}, X_{-\alpha}] =-H_{\alpha}$ với $\alpha \in R$. Mặt khác, ánh xạ $\theta :a \rightarrow  -^ta$ là một tự đẳng cấu của $\mathfrak{g}$ và $\theta (X_{\alpha}) =X_{-\alpha}$ với mọi $\alpha \in R$. Do đó, $(X_{\alpha})_{\alpha\in R}$ là một hệ Chevalley trong $(\mathfrak{g},\mathfrak{h})$.

Giả sử rằng $k=\mathbf{Q}$. Đại số con Cartan $\mathfrak{h}$ có hai dàn khả dụng $Q(R^{\vee}) =\sum_{i=1}^l\mathbf{Z}.H_i$ và $P(R^{\vee}) = Q(R^{\vee}) +\frac{1}{2}\mathbf{Z}.\sum_{i=1}^lH_i$ (Chương VI, §4,

no. 5.VIII). Ta thấy rằng $Q(R^{\vee})$ là tập hợp các ma trận có các phần tử là số nguyên thuộc $\mathfrak{h}$. Suy ra cấp Chevalley $Q(R^{\vee}) +\sum_{\alpha\in R}\mathbf{Z}.X_{\alpha}$ là tập hợp $\mathfrak{s}\mathfrak{p}(2l,\mathbf{Z})$ gồm các ma trận trong $\mathfrak{g}$ có các phần tử là số nguyên.

Xét đại số Lie khả quy $\mathfrak{s}\mathfrak{p}(\Psi ) +\mathbf{Q}.1$. Dễ thấy rằng tập hợp các phần tử của nó có các phần tử là số nguyên là một cấp Chevalley, mà phép chiếu của nó lên $\mathfrak{s}\mathfrak{p}(\Psi )$ song song với $\mathbf{Q}.1$ là cấp Chevalley $P(R^{\vee}) +\sum\mathbf{Z}.X_{\alpha}$.

Cuối cùng, $X_{\alpha}^2= 0$ với mọi $\alpha \in R$. Suy ra rằng dàn $\mathscr{V}$ trong V sinh bởi các $e_i$ là khả dụng đối với cấp Chevalley $\mathfrak{s}\mathfrak{p}(2l,\mathbf{Z})$. Điều tương tự cũng đúng đối với dàn $E_r\cap \bigwedge^r\mathscr{V}$ trong $E_r$.

Cuối cùng, $E_r$ có một dàn khả chấp nhận được đối với cấp Chevalley

$$
P(R^{\vee}) +\sum\mathbf{Z}.X_{\alpha}
$$

chỉ khi $r$ chẵn; khi đó $E_r\cap \bigwedge^r\mathscr{V}$ là một dàn như vậy.

### 4. ĐẠI SỐ KIỂU $\boldsymbol{D}_{\boldsymbol{l}}$ ($\boldsymbol{l}\geq$ 2)

(I) Cho V là một không gian vectơ có chiều chẵn $2l\geq 4$ và $\Psi$ là một dạng song tuyến tính đối xứng không suy biến có chỉ số cực đại $l$ trên V. Theo Đại số, Chap. IX, §4, no. 2, V có thể viết thành tổng trực tiếp của hai không gian con hoàn toàn đẳng hướng cực đại F và $F'$. Gọi $(e_i)_{1\leq i\leq l}$ là một cơ sở của F và $(e_{-i})_{1\leq i\leq l}$ là cơ sở đối ngẫu của $F'$ (đối với song đối ngẫu giữa F và $F'$ xác định bởi $\Psi$ ). Khi đó $e_1, . . . , e_l, e_{-l}, . . . , e_{-1}$ là một cơ sở của V; ta sẽ gọi nó là một cơ sở Witt của V. Ma trận của $\Psi$ đối với cơ sở này là ma trận vuông S cấp $2l$, tất cả các phần tử của nó đều bằng không, ngoại trừ những phần tử nằm trên đường chéo thứ hai, bằng 1. Đại số $\mathfrak{g}=\mathfrak{o}(\Psi )$ có thể được đồng nhất với đại số $\mathfrak{o}_S(2l, k)$ gồm các ma trận vuông $g$ cấp $2l$ sao cho $g=-S^tgS$. Nó có chiều $l(2l-1)$. Một phép tính dễ dàng cho thấy $\mathfrak{g}$ là tập hợp các ma trận có dạng

$$
(AB)
$$

$$
CD
$$

trong đó $A, B, C, D$ là các ma trận vuông cấp $l$ sao cho $B=-s^tBs, C=$ $-s^tCs$ và $D=-s^tAs(s$ là ma trận cấp $l$ mà tất cả các phần tử đều bằng không, ngoại trừ những phần tử nằm trên đường chéo thứ hai, bằng 1).

Gọi $\mathfrak{h}$ là tập hợp các ma trận đường chéo thuộc $\mathfrak{g}$. Đây là một đại số con giao hoán của $\mathfrak{g}$, với cơ sở gồm các phần tử $H_i=E_{i,i}-E_{-i,-i}$ với $1\leq i\leq l$. Gọi $(\varepsilon_i)$ là cơ sở của $\mathfrak{h}^*$ đối ngẫu với $(H_i)$. Đặt, với $1\leq i < j\leq l$,

$X_{\varepsilon_i-\varepsilon_j}$ = $E_{i,j}-E_{-j,-i}$

$X_{-\varepsilon_i+\varepsilon_j}$ = $-E_{j,i}+E_{-i,-j}$

$X_{\varepsilon_i+\varepsilon_j}$ = $E_{i,-j}-E_{j,-i}$ (11)

$X_{-\varepsilon_i-\varepsilon_j}$ = $-E_{-j,i}+E_{-i,j}$.

Các phần tử này tạo thành một cơ sở của một phần bù của $\mathfrak{h}$ trong $\mathfrak{g}$. Với $h\in \mathfrak{h}$,

$$
[h, X_{\alpha}] =\alpha (h)X_{\alpha}
$$

với mọi $\alpha \in R$, trong đó R là tập hợp các $\pm \varepsilon_i\pm \varepsilon_j(i < j)$. Do đó, $\mathfrak{h}$ là một đại số con Cartan tách của $\mathfrak{g}$, và các nghiệm của $(\mathfrak{g},\mathfrak{h})$ là các phần tử của R. Hệ nghiệm R của $(\mathfrak{g},\mathfrak{h})$ do đó có kiểu $D_l$ với $l\geq 3$, có kiểu $A_1\times A_1$ (nói cách khác là kiểu $D_2$) với $l= 2$ (Chương VI, §4, no. 8.I mở rộng cho trường hợp $l= 2$). Do đó, $\mathfrak{g}$ là một đại số Lie đơn tách được kiểu $D_l$ nếu $l\geq 3$.

Mọi đại số con Cartan tách của $\mathfrak{g}$ đều được biến đổi thành $\mathfrak{h}$ bởi một tự đẳng cấu sơ cấp của $\mathfrak{g}$, và do đó bởi một phần tử của $\mathbf{O}(\Psi )$ (xem (VII)) và do đó là tập hợp $\mathfrak{h}_{\beta}$ của các phần tử của $\mathfrak{g}$ mà ma trận của chúng đối với một cơ sở Witt $\beta$ của V là đường chéo. Ta kiểm tra ngay lập tức rằng các không gian con duy nhất bất biến dưới $\mathfrak{h}_{\beta}$ là các không gian được sinh bởi một tập con của $\beta$.

Vì các đại số $\mathfrak{o}_S(4, k)$ và $\mathfrak{s}\mathfrak{l}(2, k)\times \mathfrak{s}\mathfrak{l}(2, k)$ có cùng các hệ nghiệm, nên chúng đẳng cấu. Tương tự, $\mathfrak{o}_S(6, k)$ và $\mathfrak{s}\mathfrak{l}(4, k)$ đẳng cấu (xem thêm Bài tập 3). Từ nay, ta giả sử rằng $l\geq 3$. (II) Ta xác định $R^{\vee}$ bằng cách dùng Chương VI, §4, no. 8.V. Ta tìm được rằng

$$
H_{\varepsilon_i-\varepsilon_j}=H_i-H_j,H_{\varepsilon_i+\varepsilon_j}=H_i+H_j
$$

(III) Đặt $\alpha_1=\varepsilon_1-\varepsilon_2, \alpha_2=\varepsilon_2-\varepsilon_3, . . . , \alpha_{l-1}=\varepsilon_{l-1}-\varepsilon_l, \alpha_l=\varepsilon_{l-1}+\varepsilon_l$. Theo Chương VI, §4, no. 8.II, $(\alpha_1, . . . , \alpha_l)$ là một cơ sở B của R; các nghiệm dương tương ứng với B là các $\varepsilon_i\pm \varepsilon_j(i < j)$. Đại số con Borel tương ứng $\mathfrak{b}$ là tập hợp các ma trận tam giác trên thuộc $\mathfrak{g}$.

Dễ dàng kiểm tra rằng các không gian con vectơ không tầm thường duy nhất bất biến dưới $\mathfrak{b}$ là các không gian con đẳng hướng hoàn toàn $V_1, . . . ,V_l,V'_l$, trong đó $V_i$ được sinh bởi $e_1, . . . , e_i$ và $V'_l$ bởi $e_1, . . . , e_{l-1}, e_{-l}$, và các không gian trực giao $V_{-1}, . . . ,V_{-l+1}$ của $V_1, . . . ,V_{l-1}$; không gian trực giao $V_{-i}$ của $V_i$ được sinh bởi $e_1, . . . , e_l, e_{-l}, . . . , e_{-(i+1)}$. Nhưng một tính toán ngay lập tức cho thấy rằng, nếu một phần tử $a\in \mathfrak{g}$ giữ ổn định $V_{l-1}$, ma trận của nó có dạng

$$
AxB
$$

$(\lambda$ 0 $)$

0 0 $-\lambda y$

0 0 $D$

trong đó $A, B, D$ là các ma trận vuông cấp $l-1,x$ (resp. $y$) là một ma trận có 2 cột và $l-1$ hàng (resp. 2 hàng và $l-1$ cột), và $\lambda \in k$. Suy ra rằng $a$ giữ ổn định $V_l$ và $V'_l$. Do đó, $\mathfrak{b}$ là tập hợp các $a\in \mathfrak{g}$ giữ ổn định mọi phần tử của cờ đẳng hướng $(V_1, . . . ,V_{l-1})$. Chú ý rằng điều vừa nêu và định lý Witt (Đại số, Chap. IX, §4, no. 3, Th. 1) suy ra rằng $V_l$ và $V'_l$ là các không gian con đẳng hướng toàn phần cực đại duy nhất chứa $V_{l-1}$.

Ta nói rằng một cờ đẳng hướng là gần cực đại nếu nó gồm $l-1$ không gian con đẳng hướng toàn phần có các chiều lần lượt là $1, . . . , l-1$. Khi đó, như trong no. 2, ta thấy rằng, với mọi cờ đẳng hướng gần cực đại $\delta$, tập hợp $\mathfrak{b}_{\delta}$ gồm các $a\in \mathfrak{g}$ giữ ổn định các phần tử của $\delta$ là một đại số con Borel của $\mathfrak{g}$ và ánh xạ $\delta  \rightarrow \mathfrak{b}_{\delta}$ là một song ánh từ tập hợp các cờ đẳng hướng gần cực đại lên tập hợp các đại số con Borel.

Ta nói rằng một cờ đẳng hướng là thực sự nếu nó không chứa đồng thời một không gian con có chiều $l$ và một không gian con có chiều $l-1$. Cho $\delta$ là một cờ đẳng hướng như vậy và gọi $\mathfrak{p}_{\delta}$ là tập hợp các $a\in \mathfrak{g}$ giữ ổn định các phần tử của $\delta$. Nếu $\delta \subset  \{V_1, . . . ,V_l,V'_l\}$, thì $\mathfrak{p}_{\delta}$ là một đại số con parabolic của $\mathfrak{g}$, chứa $\mathfrak{b}$, và dễ dàng kiểm tra rằng các không gian con đẳng hướng toàn phần $\not=\{0\}$ duy nhất ổn định dưới $\mathfrak{p}_{\delta}$ là các phần tử của $\delta$. Vì có $2^{l-2}$ cờ đẳng hướng thực sự chứa trong $\{V_1, . . . ,V_l,V'_l\}$ và chứa $V_{l-1}$ (resp. $V_l$, resp. $V'_l$, resp. chứa cả $V_{l-1}$, $V_l$, $V'_l$), nên điều này cho $2^l$ đại số con parabolic chứa $\mathfrak{b}$. Suy ra như trên rằng ánh xạ $\delta  \rightarrow \mathfrak{p}_{\delta}$ là một song ánh từ tập hợp các cờ đẳng hướng thực sự lên tập hợp các đại số con parabolic của $\mathfrak{g}$.

(IV) Các trọng số cơ bản tương ứng với $\alpha_1, . . . , \alpha_l$ là, theo Chap. VI, §4, no. 8.VI,

$$
\varpi_i=\varepsilon_1+\varepsilon_2+\cdots +\varepsilon_i(1\leq i\leq l-2)
$$

$$
\varpi_{l-1}=\frac{1}{2}(\varepsilon_1+\varepsilon_2+. . .+\varepsilon_{l-2}+\varepsilon_{l-1}-\varepsilon_l)
$$

$$
\varpi_l=\frac{1}{2}(\varepsilon_1+\varepsilon_2+. . .+\varepsilon_{l-2}+\varepsilon_{l-1}+\varepsilon_l)
$$

Cho $\sigma$ là biểu diễn đồng nhất của $\mathfrak{g}$ trên V. Lũy thừa ngoài $\bigwedge^r\sigma$ tác động trên $E =\bigwedge^r(V)$. Nếu $h\in \mathfrak{h}$, ta có

$$
\sigma (h)e_i=\varepsilon_i(h)e_i,\sigma (h)e_{-i}=-\varepsilon_i(h)e_{-i}
$$

for $1\leq i\leq l$. Do đó, với $1\leq r\leq l,\varepsilon_1+\cdots +\varepsilon_r$ là trọng số cao nhất của $\bigwedge^r\sigma$, các phần tử có trọng số $\varepsilon_1+\cdots +\varepsilon_r$ là những phần tử tỉ lệ với $e_1\wedge  \cdots  \wedge e_r$.

Ta sẽ chứng minh rằng, với $1\leq r\leq l-2$, biểu diễn $\bigwedge^r\sigma$ là một biểu diễn cơ bản có trọng số $\varpi_r$.

Để làm điều này, chỉ cần chứng minh rằng $\bigwedge^r\sigma$ là bất khả quy với $1\leq r\leq l-1$ (chú ý rằng biểu diễn $\bigwedge^l\sigma$ không bất khả quy, xem Bài tập 10), hay rằng không gian con nhỏ nhất $T_r$ của $\bigwedge^rV$ chứa $e_1\wedge  \cdots  \wedge e_r$ và ổn định dưới $\mathfrak{g}$ là toàn bộ $\bigwedge^rV$. Điều này ngay lập tức đúng với $r= 1$. Với $r= 2$, ta thấy như trong no. 2 rằng $\bigwedge^2\sigma$ tương đương với biểu diễn phụ hợp của $\mathfrak{g}$, biểu diễn này bất khả quy vì $\mathfrak{g}$ là đơn. Chứng minh được hoàn tất bằng cách quy nạp theo $l$, như trong no. 2, nhưng giả sử rằng $l-1\geq r\geq 3$.

Bây giờ ta sẽ xác định các biểu diễn cơ bản có trọng số cao nhất $\varpi_{l-1}$ và $\varpi_l$. Gọi Q là dạng toàn phương $x \rightarrow \frac{1}{2}\Psi (x, x)$. Trong no. 2.IV, ta đã định nghĩa biểu diễn spinor $\lambda$ của đại số Clifford C(Q) trên $N =\bigwedge F'$. Ta thấy ngay lập tức rằng không gian con $N_+$ (tương ứng $N_-$) của N cho bởi tổng của các $\bigwedge^pF'$ với $p$ chẵn (tương ứng lẻ) là ổn định dưới hạn chế của $\lambda$ lên $C^+(Q)$. Do đó, các biểu diễn $\lambda_+$ và $\lambda_-$ của $C^+(Q)$ trên $N_+$ và $N_-$ tương ứng là các biểu diễn bán-spinor của $C^+(Q) ($Đại số, Chap. IX, §9, no. 4); chúng bất khả quy, có chiều $2^{l-1}$ và không tương đương. Gọi $\rho_+=\lambda_+\circ f$ và $\rho_-=\lambda_-\circ f$ là các biểu diễn bất khả quy tương ứng của $\mathfrak{g}$ (no. 2, Bổ đề 1 (vi)). Theo Bổ đề 1 (i), ta có

$$
f(H_i) =\frac{1}{2}(e_ie_{-i}-e_{-i}e_i) =e_ie_{-i}-\frac{1}{2}=\frac{1}{2}-e_{-i}e_i
$$

và ta thấy, như trong no. 2.IV, rằng, với $h\in \mathfrak{h}$ và $1\leq i_1<\cdots < i_k\leq l$,

$$
\lambda \circ f(h)(e_{-i_1}\wedge  \cdots  \wedge e_{-i_k})
$$

$$
= (\frac{1}{2}(\varepsilon_1+\cdots +\varepsilon_l)-(\varepsilon_{i_1}+\cdots +\varepsilon_{i_k}))(h)(e_{-i_1}\wedge  \cdots  \wedge e_{-i_k})
$$

Do đó, trọng số cao nhất của $\rho_+$ (tương ứng $\rho_-$) là $\varpi_l$ (tương ứng $\varpi_{l-1}$).

Ta gọi $\rho_+$ và $\rho_-$ là các biểu diễn bán-spinor của $\mathfrak{g}$. Tất cả các trọng số của chúng đều đơn. Ta cũng gọi $\rho =\lambda \circ f=\rho_+\oplus \rho_-$ là biểu diễn spinor của $\mathfrak{g}$.

(V) Với $1\leq r\leq l-2$, biểu diễn cơ bản $\bigwedge^r\sigma$ là trực giao: nó bảo toàn dạng mở rộng của $\Psi$ trên $\bigwedge^rV$.

Xét bây giờ biểu diễn spinor $\rho$ của $\mathfrak{g}$. Ta chứng minh như trong no. 2 rằng, với $1\leq i, j\leq l, i\not=j$,

$$
f(X_{\varepsilon_i-\varepsilon_j}) =\pm e_ie_{-j}
$$

$$
f(X_{\varepsilon_i+\varepsilon_j}) =\pm e_ie_j
$$

$$
f(X_{-\varepsilon_i-\varepsilon_j}) =\pm e_{-i}e_{-j}
$$

Suy ra rằng dạng song tuyến tính không suy biến $\Phi$ được đưa vào trong no. 2.V là bất biến dưới $\rho (\mathfrak{g})$. Do đó, biểu diễn spinor $\rho$ bảo toàn một dạng không suy biến, đối xứng với $l\equiv 0,-1$ (mod. 4) và phản xứng với $l\equiv 1,2$ (mod. 4).

Nếu $l$ chẵn, các hạn chế của $\Phi$ lên $N_+$ và $N_-$ là không suy biến và các biểu diễn nửa spinor là trực giao với $l\equiv 0$ (mod. 4) và symplectic với $l\equiv 2$ (mod. 4). Hơn nữa, ta nhận xét rằng $w_0=-1$ (Chương VI, §4, no. 8.XI).

Mặt khác, nếu $l$ lẻ, $N_+$ và $N_-$ hoàn toàn đẳng hướng đối với $\Phi$. Hơn nữa, $-w_0(\alpha_i) =\alpha_i$ với $1\leq i\leq l-2,-w_0(\alpha_l) =\alpha_{l-1}$ và $-w_0(\alpha_{l-1}) =\alpha_l$ (Chương VI, §4, no. 8.XI), nên $-w_0(\varpi_l) =\varpi_{l-1}$ và các biểu diễn nửa spinor không trực giao cũng không symplectic; mỗi biểu diễn trong chúng đẳng cấu với đối ngẫu của biểu diễn kia.

(VI) Với mọi $x\in \mathfrak{g}$, đa thức đặc trưng của $\sigma (x)$ có dạng

$$
T^{2l}+f_1(x)T^{2l-1}+\cdots +f_{2l}(x)
$$

Ta thấy như trong no. 3 rằng $f_1=f_3=f_5=\cdots = 0$. Theo Chương VI, §4, no. 8.IX và §8, no. 3, Định lý 1, tồn tại một hàm đa thức $\widetilde{f}$ trên $\mathfrak{g}$ sao cho $f_2, f_4, . . . , f_{2l-2},\widetilde{f}$ sinh đại số $I(\mathfrak{g}^*)$ của các hàm đa thức bất biến trên $\mathfrak{g}$, độc lập đại số, và hơn nữa $\widetilde{f}^2= (-1)^lf_{2l}$.

Với mọi $x\in \mathfrak{g}$, ta có $^t(Sx) =^txS=-Sx$, nên ta có thể xét Pf($Sx$), là một hàm đa thức của $x$. Khi đó:

$f_{2l}(x) =$ det($x$) $= (-1)^l$ det($Sx$) $= (-1)^l$(Pf($Sx$))$^2$.

Do đó, ta có thể lấy $\widetilde{f}(x) =$ Pf($Sx$).

(VII) Nhắc lại (§5, no. 3, Hệ quả 1 của Mệnh đề 5) rằng Aut($\mathfrak{g}$)$/$Aut$_0(\mathfrak{g})$ có thể được đồng nhất với nhóm Aut(D) gồm các tự đẳng cấu của đồ thị Dynkin D của $(\mathfrak{g},\mathfrak{h})$. Khi $l\not= 4$, Aut(D) là nhóm cấp 2 gồm các hoán vị của $\alpha_1, . . . , \alpha_l$ giữ cố định $\alpha_1, . . . , \alpha_{l-2}$. Khi $l= 4$, Aut(D) gồm các hoán vị của $\alpha_1, . . . , \alpha_4$ giữ cố định $\alpha_2$; nó đẳng cấu với $\mathfrak{S}_3$ (cf. Chap. VI, §4, no. 8.XI). Trong mọi trường hợp, nhóm con của Aut(D) gồm các phần tử giữ cố định $\alpha_1$ có cấp 2. Ta ký hiệu Aut$'(\mathfrak{g})$ là nhóm con tương ứng của Aut($\mathfrak{g}$); ta có Aut$'(\mathfrak{g}) =$ Aut($\mathfrak{g}$) nếu $l\not= 4$ và (Aut($\mathfrak{g}$) $:$ Aut$'(\mathfrak{g})$) $= 3$ nếu $l= 4$; hơn nữa,

(Aut$'(\mathfrak{g}) :$ Aut$_0(\mathfrak{g})$) $= 2$.

Một phần tử $s\in$ Aut($\mathfrak{g}$) thuộc Aut$'(\mathfrak{g})$ khi và chỉ khi $\sigma \circ s$ tương đương với $\sigma$ (điều này suy ra từ sự kiện rằng $\varpi_1$ là trọng số cao nhất của $\sigma$ ). Ta kết luận như trong no. 2.VII rằng Aut$'(\mathfrak{g})$ có thể được đồng nhất với $\Sigma /k^*$, trong đó $\Sigma$ là nhóm các phép đồng dạng của V đối với $\Psi$.

Cho $s\in \Sigma$, và gọi $\lambda (s)$ là nhân tử của $s$. Ta có det($s$) $=\lambda (s)^l$ nếu $s$ là trực tiếp, và det($s$) $=-\lambda (s)^l$ nếu $s$ là nghịch đảo (Đại số, Chap. IX, §6, no. 5). Các phép đồng dạng trực tiếp tạo thành một nhóm con $\Sigma_0$ có chỉ số 2 trong $\Sigma$; ta có $\Sigma_0\supset k^*$. Nhóm $\Sigma_0/k^*$ bằng nhóm con Aut$_0(\mathfrak{g})$ của Aut$'(\mathfrak{g}) =\Sigma /k^*$. Thật vậy, chỉ cần kiểm tra điều này khi $k$ đóng đại số: trong trường hợp đó Aut$_0(\mathfrak{g}) =$ Aut$_e(\mathfrak{g})$ bằng nhóm dẫn xuất của nó (§11, no. 2, Mệnh đề 3), do đó được chứa trong $\Sigma_0/k^*$, và vì cả hai đều có chỉ số 2 trong $\Sigma /k^*$, nên chúng bằng nhau.

Mặt khác, như trong no. 3.VII có một dãy khớp

$$
1\longrightarrow \mathbf{S}\mathbf{O}(\Psi )/\{1,-1\} \longrightarrow \Sigma_0/k^*\longrightarrow k^*/k^{*2}\longrightarrow 1
$$

Đồng nhất $\mathbf{S}\mathbf{O}(\Psi )/\{1,-1\}$ với một nhóm con của $\Sigma_0/k^*=$ Aut$_0(\mathfrak{g})$. Vì $k^*/k^{*2}$ là giao hoán, ta có Aut$_e(\mathfrak{g})\subset \mathbf{S}\mathbf{O}(\Psi )/\{1,-1\}$. Thực ra, có thể chứng minh (Bài tập 11) rằng Aut$_e(\mathfrak{g})$ bằng ảnh trong $\mathbf{S}\mathbf{O}(\Psi )/\{1,-1\}$ của nhóm trực giao rút gọn $\mathbf{O}^+_0(\Psi )$ của $\Psi ($Đại số, Chương IX, §9, no. 5).

(VIII) Dạng song tuyến tính chính tắc $\Phi_R$ trên $\mathfrak{h}^*$ được cho bởi

$''$ 1 $''$

$$
\Phi_R(\xi_1\varepsilon_1+\cdots +\xi_l\varepsilon_l, \xi_1\varepsilon_1+\cdots +\xi_l\varepsilon_l) =(\xi_1\xi +\cdots +\xi_l\xi )
$$

$$
\overline{4(l- 1)}^1l
$$

(Chương VI, §4, no. 8.V). Do đó, hạn chế của dạng Killing trên $\mathfrak{h}$ là

$$
\Phi (\xi_1H_1+\cdots +\xi_lH_l, \xi '_1H_1+\cdots +\xi '_lH_l) = 4(l-1)(\xi_1\xi '_1+\cdots +\xi_l\xi '_l)
$$

(IX) Nhắc lại các $X_{\alpha}(\alpha \in R)$ được xác định bởi các công thức (11). Ta dễ dàng kiểm tra rằng $[X_{\alpha}, X_{-\alpha}] =-H_{\alpha}$ với $\alpha \in R$. Mặt khác, ánh xạ $\theta :a \rightarrow  -^ta$ là một tự đẳng cấu của $\mathfrak{g}$ và $\theta (X_{\alpha}) =X_{-\alpha}$ với mọi $\alpha \in R$. Do đó $(X_{\alpha})_{\alpha\in R}$ là một hệ Chevalley trong $(\mathfrak{g},\mathfrak{h})$.

Giả sử rằng $k=\mathbf{Q}$. Theo Chương VI, §4, no. 8.VIII, đại số con $\mathfrak{h}$ có ba dàn khả dĩ nếu $l$ lẻ và bốn dàn khả dĩ nếu $l$ chẵn. Đặc biệt, dàn $\mathscr{H}$ sinh bởi các $H_i$ là khả dĩ. Nhưng dàn này là tập hợp các ma trận đường chéo trong $\mathfrak{g}$ có các phần tử là số nguyên. Suy ra $\mathfrak{o}_S(2l,\mathbf{Z})$ là thứ tự Chevalley $\mathscr{H}+\sum\mathbf{Z}.X_{\alpha}$ trong $\mathfrak{g}$. Vì $X_{\alpha}^2= 0$ với mọi $\alpha \in R$, ta thấy rằng dàn $\mathscr{V}$ trong V sinh bởi cơ sở Witt $(e_i)$ là một dàn khả dụng trong V đối với $\mathfrak{o}_S(2l,\mathbf{Z})$. Điều tương tự đúng đối với $\bigwedge^r\mathscr{V}$ trong $\bigwedge^rV$.

Mặt khác, nếu ta lấy $P(R^{\vee}) =\mathbf{Z}.\frac{1}{2}\sum_{i=1}^lH_i+\mathscr{H}$ làm dàn khả dĩ và $\mathscr{G}= P(R^{\vee}) +\sum\mathbf{Z}.X_{\alpha}$ làm thứ tự Chevalley, ta thấy rằng $\bigwedge^rV$ có một dàn khả dụng chỉ khi $r$ chẵn; khi đó $\bigwedge^r\mathscr{V}$ là khả dụng.

Xét đại số Lie khả quy $\mathfrak{o}(\Psi ) +\mathbf{Q}.1$; ta thấy ngay lập tức rằng dàn $\widetilde{\mathscr{G}}= (\mathfrak{o}(\Psi ) +\mathbf{Q}.1)\cap \mathfrak{g}\mathfrak{l}(2l,\mathbf{Z})$ là một thứ tự Chevalley. Thứ tự Chevalley $\mathscr{G}$ là phép chiếu của $\widetilde{\mathscr{G}}$ lên $\mathfrak{o}(\Psi )$ song song với tâm $\mathbf{Q}.1$.

Cuối cùng, ta thấy như trong no. 2 rằng dàn $\mathscr{N}_+$ (tương ứng $\mathscr{N}_-$) sinh bởi các $e_{-i_1}\wedge  \cdots  \wedge e_{-i_{2k}}$ (tương ứng $e_{-i_1}\wedge  \cdots  \wedge e_{-i_{2k+1}}$) là khả chấp nhận được đối với biểu diễn nửa spinor của cấp Chevalley $Q(R^{\vee}) +\sum_{\alpha\in R}\mathbf{Z}.X_{\alpha}$. Mặt khác, $\mathscr{N}_+$ và $\mathscr{N}_-$ không có dàn khả chấp nhận được đối với $\mathfrak{o}_S(2l,\mathbf{Z})$.

BẢNG 1

Ta gán cho mỗi trọng số cơ bản số 1 (tương ứng $-1,0$) nếu biểu diễn đơn tương ứng là trực giao (tương ứng symplectic, tương ứng không trực giao cũng không symplectic). Về cơ bản, phép tính số này đã được trình bày trong §13 đối với các kiểu $A_l,B_l,C_l,D_l$. Các kết quả cũng được chỉ ra dưới đây đối với các kiểu $E_6,E_7,E_8,F_4,G_2$ (chỉ cần áp dụng §7, Mệnh đề 12, và Chương VI, §4, các số 9.VI, 9.XI, 10.VI, 10.XI, 11.VI, 11.XI, 12.VI, 12.XI, 13.VI, 13.XI).

$$
A_l(l\geq 1)B_l(l\geq 2)
$$

$\{0r\not=\frac{l+1}{2}\varpi_r$ 1 $r\not=l$

$$
\varpi_r
$$

$$
(-1)^rr=\frac{l+1}{2}\varpi_l(-1)^{l(l+1)/2}
$$

$$
C_l(l\geq 2)D_l(l\geq 2)
$$

$\varpi_r(-1)^r\varpi_r$ 1 $r\not=l-1, l$

$\{0$ nếu $l$ là lẻ

$\varpi_l$ và $\varpi_{l-1}(-1)^{l/2}$ nếu $l$ là chẵn

$$
E_6E_7E_8F_4G_2
$$

$\varpi_1$ 0 $\varpi_1$ 1 $\varpi_1$ 1 $\varpi_1$ 1 $\varpi_1$ 1

$\varpi_2$ 1 $\varpi_2-1\varpi_2$ 1 $\varpi_2$ 1 $\varpi_2$ 1

$\varpi_3$ 0 $\varpi_3$ 1 $\varpi_3$ 1 $\varpi_3$ 1

$\varpi_4$ 1 $\varpi_4$ 1 $\varpi_4$ 1 $\varpi_4$ 1

$\varpi_5$ 0 $\varpi_5-1\varpi_5$ 1

$\varpi_6$ 0 $\varpi_6$ 1 $\varpi_6$ 1

$\varpi_7-1\varpi_7$ 1

$\varpi_8$ 1

BẢNG 2

Ta gán cho mỗi trọng số cơ bản chiều của biểu diễn đơn tương ứng, được tính bằng Định lý 2 của §9.

$$
A_l(l\geq 1)B_l(l\geq 2)
$$

$$
(l+ 1)(2l+ 1)
$$

$$
\varpi_r(1\leq r\leq l)\varpi_r(1\leq r\leq l-1)
$$

$$
rr
$$

$$
\varpi_l2^l
$$

$$
C_l(l\geq 2)D_l(l\geq 2)
$$

$$
(2l)(2l)(2l)
$$

$$
\varpi_r(1\leq r\leq l)-\varpi_r(1\leq r\leq l-2)
$$

$$
rr-2r
$$

$$
\varpi_{l-1}2^{l-1}
$$

$$
\varpi_l2^{l-1}
$$

$$
E_6E_7
$$

$$
\varpi_127 = 3^3\varpi_1133 = 7.19
$$

$$
\varpi_278 = 2.3.13\varpi_2912 = 2^4.3.19
$$

$$
\varpi_3351 = 3^3.13\varpi_38645 = 5.7.13.19
$$

$$
\varpi_42925 = 3^2.5^2.13\varpi_4365750 = 2.5^3.7.11.19
$$

$$
\varpi_5351 = 3^3.13\varpi_527664 = 2^4.7.13.19
$$

$$
\varpi_627 = 3^3\varpi_61539 = 3^4.19
$$

$$
\varpi_756 = 2^3.7
$$

$$
E_8F_4
$$

$$
\varpi_13875 = 5^3.31\varpi_152 = 2^2.13
$$

$$
\varpi_2147250 = 2.5^3.19.31\varpi_21274 = 2.7^2.13
$$

$$
\varpi_36696000 = 2^6.3^3.5^3.31\varpi_3273 = 3.7.13
$$

$$
\varpi_46899079264 = 2^5.3.7^2.11^2.17.23.31\varpi_426 = 2.13
$$

$$
\varpi_5146325270 = 2.3.5.7^2.13^2.19.31
$$

$$
\varpi_62450240 = 2^6.5.13.19.31
$$

$$
\varpi_730380 = 2^2.5.7^2.31G_2
$$

$\varpi_8248 = 2^3.31\varpi_1$ 7

$$
\varpi_214 = 2.7
$$

### Bài tập {#lie-viii-s13-exercises}

Xem [các bài tập cho § 13](exercises/s13/).
