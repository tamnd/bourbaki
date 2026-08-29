---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VIII
chapter_title: SPLIT SEMI-SIMPLE LIE ALGEBRAS
section: 10
section_title: Maximal subalgebras of semi-simple Lie algebras
lang: vi
source: lie-vii-ix
book_pages: 159-163, 260-261
pdf_pages: 0167-0171, 0268-0269
extraction: native
statements: 8
exercises: 7
content_sha256: 53f5bd3688dc700f1fb348ef1cabcf8f1e553bb2c3a712e12a6cca103ed5904c
translated_from: content/en/lie/VIII/10_s10_maximal_subalgebras_of_semi_simple_lie.md
source_content_sha256: 345f66620b2c4fae05d0eb5d76aa4f165ea7875de6e8bd6a97f18302eec6a845
translation_model: gpt-5.4
translation_run: translate-vi-f189c613
glossary_version: 34
glossary_terms_sha256: cb5ba6ece684844df359b42733ad4d37a73d0df2148cf8f985f2fa1776273db1
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 10. CÁC ĐẠI SỐ CON CỰC ĐẠI CỦA CÁC ĐẠI SỐ LIE NỬA ĐƠN

#### Định lý 1 {#lie-viii-s10-thm-1 .statement tag=016L}

Cho V là một không gian vectơ hữu hạn chiều, $\mathfrak{g}$ một đại số con Lie khả quy của $\mathfrak{g}\mathfrak{l}(V),\mathfrak{q}$ một đại số con Lie của $\mathfrak{g}$ và $\Phi$ dạng song tuyến tính $(x, y) \rightarrow$ Tr($xy$) trên $\mathfrak{g}\times \mathfrak{g}$. Giả sử phần bù trực giao $\mathfrak{n}$ của $\mathfrak{q}$ đối với $\Phi$ là một đại số con Lie của $\mathfrak{g}$ gồm các nội đồng cấu lũy linh của V. Khi đó $\mathfrak{q}$ là một đại số con parabolic của $\mathfrak{g}$.

$a)\mathfrak{q}$ là chuẩn hóa tử của $\mathfrak{n}$ trong $\mathfrak{g}:$ đặt $\mathfrak{p}$ là chuẩn hóa tử này. Cho $x\in \mathfrak{q}$ và $y\in \mathfrak{n}$; với mọi $z\in \mathfrak{q}$, ta có $[z, x]\in \mathfrak{q}$, nên

$$
\Phi ([x, y], z) =\Phi (y,[z, x]) = 0
$$

nói cách khác, $[x, y]\in \mathfrak{n}$. Do đó $\mathfrak{q}\subset \mathfrak{p}$. Vì $\mathfrak{n}$ là một iđêan của $\mathfrak{p}$ gồm các nội tự đồng cấu lũy linh của V, nên P trực giao với $\mathfrak{n}$ đối với $\Phi$ (Chap. I, no. 3, Prop. $4d$)$)$. Vì $\Phi$ không suy biến$^4,\mathfrak{p}\subset \mathfrak{q}$, do đó mệnh đề của chúng ta.

b) Tồn tại một đại số con Lie khả quy $\mathfrak{m}$ trong $\mathfrak{g}\mathfrak{l}(V)$ sao cho $\mathfrak{q}$ là tích nửa trực tiếp của $\mathfrak{m}$ và $\mathfrak{n}:$ gọi $\mathfrak{n}_V(\mathfrak{q})$ là iđêan lớn nhất của $\mathfrak{q}$ gồm các nội tự đồng cấu lũy linh của V. Khi đó $\mathfrak{n}_V(\mathfrak{q})$ chứa $\mathfrak{n}$, và nó trực giao với $\mathfrak{q}($loc. cit.); do đó $\mathfrak{n}=\mathfrak{n}_V(\mathfrak{q})$. Hơn nữa, $\mathfrak{g}$ khả quy trong $\mathfrak{g}\mathfrak{l}(V)$ theo giả thiết, vì thế phân tích được (Chương VII, §5, no. 1, Mệnh đề 2); vì $\mathfrak{q}$ là giao của $\mathfrak{g}$ với bộ chuẩn hóa của $\mathfrak{n}$ trong $\mathfrak{g}\mathfrak{l}$(V), nên nó là một đại số Lie phân tích được (loc. cit., Hệ quả 1 của Mệnh đề 3). Do đó, mệnh đề của chúng ta suy ra từ Mệnh đề 7 của Chương VII, §5, no. 3.

Chọn một đại số con Cartan $\mathfrak{h}$ của $\mathfrak{m}$; ký hiệu $\mathfrak{g}_1$ là hoán tập của $\mathfrak{h}$ trong $\mathfrak{g}$, và đặt $\mathfrak{q}_1=\mathfrak{q}\cap \mathfrak{g}_1,\mathfrak{n}_1=\mathfrak{n}\cap \mathfrak{g}_1$.

c) Các đại số Lie $\mathfrak{g}_1,\mathfrak{q}_1$ và $\mathfrak{n}_1$ thỏa mãn các giả thiết giống như $\mathfrak{g},\mathfrak{q}$ và $\mathfrak{n}:$ vì $\mathfrak{m}$ là khả quy trong $\mathfrak{g}\mathfrak{l}$(V), $\mathfrak{h}$ giao hoán và được hợp thành bởi các nội cấu nửa đơn của V (Chương VII, §2, no. 4, Hệ quả 3 của Định lý 2). Do đó $\mathfrak{g}_1=\mathfrak{g}^0(\mathfrak{h})$ là khả quy trong $\mathfrak{g}$ (Chương VII, §1, no. 3, Mệnh đề 11), vì thế cũng khả quy trong $\mathfrak{g}\mathfrak{l}(V)$ (Chương I, §6, no. 6, Hệ quả 2 của Mệnh đề 7). Hiển nhiên là $\mathfrak{n}_1$ được hợp thành

$^4$ Gọi $\mathfrak{z}$ là phần bù trực giao của $\mathfrak{g}$ đối với $\Phi$; đây là một iđêan của $\mathfrak{g}$ được chứa trong $\mathfrak{n}$, nên mọi phần tử của $\mathfrak{z}$ đều lũy linh. Biểu diễn đồng nhất của $\mathfrak{g}$ là nửa đơn (Chương I, §6, Hệ quả 1 của Mệnh đề 7). Do đó $\mathfrak{z}= 0$ (Chương I, §4, no. 3, Bổ đề 2). của các nội cấu lũy linh của V. Vì $\mathfrak{h}$ là một đại số con của $\mathfrak{q}$, khả quy trong $\mathfrak{g}\mathfrak{l}$(V), nên biểu diễn phụ hợp của $\mathfrak{h}$ trên $\mathfrak{q}$ là nửa đơn; theo phép dựng, $\mathfrak{q}_1$ là tập hợp các bất biến của ad$_{\mathfrak{q}}(\mathfrak{h})$, nên $\mathfrak{q}=\mathfrak{q}_1+ [\mathfrak{h},\mathfrak{q}]$ (Chương I, §3, no. 5, Mệnh đề 6). Vì

$$
\Phi (\mathfrak{g}_1,[\mathfrak{h},\mathfrak{q}]) =\Phi ([\mathfrak{h},\mathfrak{g}_1],\mathfrak{q}) = 0
$$

một phần tử của $\mathfrak{g}_1$ trực giao với $\mathfrak{q}_1$ khi và chỉ khi nó trực giao với $\mathfrak{q}$; do đó, $\mathfrak{n}_1=\mathfrak{g}_1\cap \mathfrak{n}$ là phần bù trực giao của $\mathfrak{q}_1$ trong $\mathfrak{g}_1$.

d) Đại số con Cartan $\mathfrak{h}$ của $\mathfrak{m}$ là một đại số con Cartan của $\mathfrak{g}:$ Ta có $\mathfrak{q}=\mathfrak{m}\oplus \mathfrak{n}$ và $\mathfrak{h}=\mathfrak{m}\cap \mathfrak{g}_1$, nên ngay lập tức có $\mathfrak{q}_1=\mathfrak{h}\oplus \mathfrak{n}_1$. Hơn nữa, $[\mathfrak{h},\mathfrak{n}_1] = 0,\mathfrak{h}$ giao hoán và $\mathfrak{n}_1$ lũy linh, nên đại số Lie $\mathfrak{q}_1$ lũy linh. Theo a) và $c),\mathfrak{q}_1$ là chuẩn hóa tử của $\mathfrak{n}_1$ trong $\mathfrak{g}_1$; a fortiori$,\mathfrak{q}_1$ bằng chuẩn hóa tử của chính nó trong $\mathfrak{g}_1$, do đó là một đại số con Cartan của $\mathfrak{g}_1$. Vì $\mathfrak{g}_1$ khả quy trong $\mathfrak{g}\mathfrak{l}$(V), suy ra từ Hệ quả 3 của Định lý 2 của Chương VII, §2, no. 4, rằng $\mathfrak{q}_1$ gồm các nội tự đồng cấu nửa đơn của V; do đó, vì $\mathfrak{n}_1$ gồm các nội tự đồng cấu lũy linh của V, ta có $\mathfrak{n}_1= 0$. Do đó, $\mathfrak{h}=\mathfrak{q}_1$ là một đại số con Cartan của $\mathfrak{g}_1$, và vì $\mathfrak{g}_1$ chuẩn hóa $\mathfrak{h}$, ta có $\mathfrak{h}=\mathfrak{g}_1$. Vậy, ta đã chứng minh rằng mọi phần tử của $\mathfrak{h}$ là một phần tử nửa đơn của $\mathfrak{g}$, và rằng hoán tập của $\mathfrak{h}$ trong $\mathfrak{g}$ bằng $\mathfrak{h}$; suy ra $\mathfrak{h}=\mathfrak{g}^0(\mathfrak{h})$, nên $\mathfrak{h}$ là một đại số con Cartan của $\mathfrak{g}$.

$e)\mathfrak{q}$ là một đại số con parabolic của $\mathfrak{g}:$ theo điều vừa nói trước đó, $\mathfrak{h}$ là một đại số con Cartan của $\mathfrak{g},\mathfrak{n}$ gồm các phần tử lũy linh của $\mathfrak{g}$, và $[\mathfrak{h},\mathfrak{n}]\subset \mathfrak{n}$. Cho $\overline{k}$ là một bao đóng đại số của $k$; theo định nghĩa, $\mathfrak{q}$ là parabolic trong $\mathfrak{g}$ khi và chỉ khi $\overline{k}\otimes_k\mathfrak{q}$ là một đại số con parabolic của $\overline{k}\otimes_k\mathfrak{g}$. Vì các tính chất đã nêu ở trên được bảo toàn qua mở rộng vô hướng, nên để chứng minh ta có thể tự giới hạn vào trường hợp $\mathfrak{h}$ là tách. Gọi R là hệ nghiệm của $(\mathfrak{g},\mathfrak{h})$; theo Mệnh đề 2 (v) của §3, no. 1, tồn tại một tập con P của R sao cho $P\cap (-P) =\emptyset$ và $\mathfrak{n}=\sum_{\alpha\in P}\mathfrak{g}^{\alpha}$.

Cho $P'$ là tập hợp các nghiệm $\alpha$ sao cho $-\alpha  \notin P$; ta có $P'\cup (-P') = R$, và phần bù trực giao $\mathfrak{q}$ của $\mathfrak{n}$ trong $\mathfrak{g}$ bằng $\mathfrak{h}+\sum_{\alpha\in P'}\mathfrak{g}^{\alpha}$. Ta có

đã chứng minh rằng $\mathfrak{q}$ là parabolic. Q.E.D.

#### Bổ đề 1 {#lie-viii-s10-lem-1 .statement tag=016M}

Cho $\mathfrak{g}$ là một đại số Lie nửa đơn, V là một không gian vectơ hữu hạn chiều, $\rho$ là một biểu diễn tuyến tính của $\mathfrak{g}$ trên V, D là một không gian con vectơ của V$,\mathfrak{h}$ là một đại số con Cartan của $\mathfrak{g},\mathfrak{s}$ là (resp. $\mathfrak{s}'$) tập hợp các $x\in \mathfrak{h}$ sao cho $\rho (x)D\subset D$ (resp. $\rho (x)D = 0$), và $\Phi$ là dạng song tuyến tính trên $\mathfrak{g}$ liên kết $^5$ với $\rho$.

(i) Nếu $\mathfrak{h}$ là tách, thì các không gian con vectơ $\mathfrak{s}$ và $\mathfrak{s}'$ của $\mathfrak{h}$ là hữu tỉ trên $\mathbf{Q}$.

(ii) Nếu $\rho$ là đơn ánh, thì hạn chế của $\Phi$ lên $\mathfrak{s}$ (tương ứng lên $\mathfrak{s}'$) là không suy biến.

Giả sử rằng đại số con Cartan $\mathfrak{h}$ là tách. Gọi $d$ là chiều của D; đặt $W =\bigwedge^d(V)$ và $\sigma =\bigwedge^d(\rho )$; cũng ký hiệu bởi $(e_1, . . . , e_d)$ một cơ sở của D và $e=e_1\wedge  \cdots  \wedge e_d$ là một $d$-vectơ phân tích được liên kết với D. Gọi P là tập hợp các trọng số của $\sigma$ đối với $\mathfrak{h}$; ký hiệu bởi $W^\mu$ không gian con của

$^5$ Nói cách khác, $\Phi (x, y) =$ Tr($\rho (x)\rho (y)$) với $x, y\in \mathfrak{g}$. W liên kết với trọng số $\mu$, và đặt $e=\sum_{\mu\in P}e^\mu$ (với $e^\mu\in W^\mu$ với mọi

$\mu\in P)$; sau cùng, gọi $P'$ là tập hợp các trọng số $\mu$ sao cho $e^\mu\not= 0$ và gọi $P''$ là tập hợp các hiệu của các phần tử của $P'$. Cho $x$ thuộc $\mathfrak{h}$; khi đó $x$ thuộc $\mathfrak{s}$ khi và chỉ khi tồn tại $c$ trong $k$ sao cho $\rho (x).e=c.e$ (Chương VII, §5, no. 4, Bổ đề 2 (i)). Vì $\rho (x).e^\mu=\mu(x).e^\mu$, ta thấy rằng $x\in \mathfrak{s}$ tương đương với quan hệ “$\mu(x) = 0$ for all $\mu\in P''$ ”. Bây giờ, cấu trúc $\mathbf{Q}$ của $\mathfrak{h}$ là không gian con vectơ trên $\mathbf{Q}$ $\mathfrak{h}_{\mathbf{Q}}$ của $\mathfrak{h}$ được sinh bởi các đối căn $H_{\alpha}$ và mọi $\mu$ trong $P''$ đều nhận các giá trị hữu tỉ trên $\mathfrak{h}_{\mathbf{Q}}$; suy ra (Đại số, Chương II, §8, no. 4, Mệnh đề 5) rằng $\mathfrak{s}$ là một không gian con của $\mathfrak{h}$ hữu tỉ trên $\mathbf{Q}$.

Với mọi trọng số $\mu\in P$, gọi $p_\mu$ là phép chiếu lên $V^\mu$ liên kết với phân tích $V =\bigoplus_{\mu\in P}V^\mu$; ký hiệu bởi $P_1$ tập hợp các $\mu\in P$ sao cho

$p_\mu(D)\not= 0$. Hiển nhiên $\mathfrak{s}'$ là giao của các hạt nhân (trong $\mathfrak{h}$) của các phần tử của $P_1$; do đó, theo cùng một cách như đối với $\mathfrak{s}$, $\mathfrak{s}'$ là một không gian con của $\mathfrak{h}$ hữu tỉ trên $\mathbf{Q}$. Điều này chứng minh (i).

Bằng phép mở rộng vô hướng, chỉ cần chứng minh (ii) khi $k$ đóng đại số, do đó khi $\mathfrak{h}$ tách. Cho $\mathfrak{m}$ là một không gian con vectơ của $\mathfrak{h}$ hữu tỉ trên $\mathbf{Q}$; với mọi $x$ khác không trong $\mathfrak{m}_{\mathbf{Q}}=\mathfrak{m}\cap \mathfrak{h}_{\mathbf{Q}}$, ta có $\Phi (x, x)>0$ theo Hệ quả của Mệnh đề 1 của §7, no. 1. Hạn chế của $\Phi$ lên $\mathfrak{m}_{\mathbf{Q}}$ là không suy biến, và do đó hạn chế của $\Phi$ lên $\mathfrak{m}$ cũng vậy vì $\mathfrak{m}$ đẳng cấu chính tắc với $k\otimes_{\mathbf{Q}}\mathfrak{m}_{\mathbf{Q}}$.

#### Định nghĩa 1 {#lie-viii-s10-def-1 .statement tag=016N}

Cho $\mathfrak{q}$ là một đại số con Lie của đại số Lie nửa đơn $\mathfrak{g}$. Khi đó người ta nói $\mathfrak{q}$ là phân tích được trong $\mathfrak{g}$ nếu, với mọi $x\in \mathfrak{q}$, các thành phần nửa đơn và lũy linh của $x$ trong $\mathfrak{g}$ thuộc $\mathfrak{q}$. Ký hiệu $\mathfrak{n}_{\mathfrak{g}}(\mathfrak{q})$ là tập hợp các phần tử $x$ của căn của $\mathfrak{q}$ sao cho ad$_{\mathfrak{g}}x$ là lũy linh.

Cho $\rho$ là một biểu diễn đơn ánh của $\mathfrak{g}$ trên một không gian vectơ V hữu hạn chiều. Ta biết (Chap. I, §6, no. 3, Định lý 3) rằng một phần tử $x$ của $\mathfrak{g}$ là nửa đơn (resp. lũy linh) nếu và chỉ nếu tự đồng cấu $\rho (x)$ của V là nửa đơn (resp. lũy linh). Suy ra ngay lập tức rằng đại số $\mathfrak{q}$ là phân tích được trong $\mathfrak{g}$ nếu và chỉ nếu $\rho (\mathfrak{q})$ là một đại số con phân tích được của $\mathfrak{g}\mathfrak{l}(V)$ theo nghĩa của Định nghĩa 1 của Chap. VII, §5, no. 1. Với các ký hiệu của Chap. VII, §5, no. 3, ta cũng có

$$
\rho (\mathfrak{n}_{\mathfrak{g}}(\mathfrak{q})) =\mathfrak{n}_V(\rho (\mathfrak{q}))
$$

#### Định lý 2 {#lie-viii-s10-thm-2 .statement tag=016O}

Cho $\mathfrak{g}$ là một đại số Lie nửa đơn, $\mathfrak{n}$ là một đại số con của $\mathfrak{g}$ gồm các phần tử lũy linh, $\mathfrak{q}$ là bộ chuẩn hoá của $\mathfrak{n}$ trong $\mathfrak{g}$. Giả sử rằng $\mathfrak{n}$ là tập hợp các phần tử lũy linh của căn của $\mathfrak{q}$. Khi đó $\mathfrak{q}$ là parabolic.

Trước hết, chú ý rằng $\mathfrak{q}$ là phân tích được (Ch. VII, §5, no. 1, Hệ quả 1 của Mệnh đề 3). Theo Định lý 1, chỉ cần chứng minh rằng $\mathfrak{q}$ là phần bù trực giao $\mathfrak{n}^0$ của $\mathfrak{n}$ đối với dạng Killing $\Phi$ của $\mathfrak{g}$. Ta biết rằng $\mathfrak{q}\subset \mathfrak{n}^0$ (Ch. I, §4, no. 3, Mệnh đề $4d$)$)$. Theo Ch. VII, §5, no. 3, Mệnh đề 7, tồn tại một đại số con $\mathfrak{m}$ của $\mathfrak{q}$, khả quy trong $\mathfrak{g}$, sao cho $\mathfrak{q}$ là tích nửa trực tiếp của $\mathfrak{m}$ và $\mathfrak{n}$. Ta sẽ chỉ ra rằng hạn chế của $\Phi$ trên $\mathfrak{m}$ là không suy biến. Gọi $\mathfrak{c}$ là tâm của $\mathfrak{m}$. Ta có $\Phi ([\mathfrak{m},\mathfrak{m}],\mathfrak{c}) = 0$ theo Ch. I, §5, no. 5, Mệnh đề 5, và hạn chế của $\Phi$ trên $[\mathfrak{m},\mathfrak{m}]$ là không suy biến theo Ch. I, §6, no. 1, Mệnh đề 1. Còn lại phải xét rằng hạn chế của $\Phi$ trên $\mathfrak{c}$ là không suy biến. Gọi $\mathfrak{k}$ là một đại số con Cartan của $[\mathfrak{m},\mathfrak{m}]$; khi đó $\mathfrak{k}\oplus \mathfrak{c}$ là giao hoán và khả quy trong $\mathfrak{g}$. Gọi $\mathfrak{h}$ là một đại số con Cartan của $\mathfrak{g}$ chứa $\mathfrak{k}\oplus \mathfrak{c}$ (Ch. VII, §2, no. 3, Mệnh đề 10). Khi đó $\mathfrak{h}\cap \mathfrak{q}$ là một đại số con giao hoán của $\mathfrak{q}$ chứa $\mathfrak{k}\oplus \mathfrak{c}$, và ad$_{\mathfrak{q}}x$ là nửa đơn với mọi $x\in \mathfrak{h}\cap \mathfrak{q}$; do đó $\mathfrak{h}\cap \mathfrak{q}$ được chứa trong một đại số con Cartan $\mathfrak{h}'$ của $\mathfrak{q}$ (Ch. VII, §2, no. 3, Mệnh đề 10); gọi $f$ là phép chiếu của $\mathfrak{q}$ lên $\mathfrak{m}$ với hạt nhân $\mathfrak{n}$; khi đó $f(\mathfrak{h}')$ là một đại số con Cartan của $\mathfrak{m}$ (Ch. VII, §2, no. 1, Hệ quả 2 của Mệnh đề 4) chứa $\mathfrak{k}\oplus \mathfrak{c}$, và do đó bằng $\mathfrak{k}\oplus \mathfrak{c}$; điều này chứng minh rằng $f(\mathfrak{h}\cap \mathfrak{q}) =\mathfrak{k}\oplus \mathfrak{c}$, và vì mọi phần tử của $\mathfrak{h}$ đều là nửa đơn trong $\mathfrak{g}$, ta có $\mathfrak{h}\cap \mathfrak{q}=\mathfrak{k}\oplus \mathfrak{c}$. Vậy,

$\mathfrak{c}=\{x\in \mathfrak{h}|[x,\mathfrak{n}]\subset \mathfrak{n}$ và $[x,[\mathfrak{m},\mathfrak{m}]] = 0\}$.

Theo Bổ đề 1, hạn chế của $\Phi$ trên $\mathfrak{c}$ là không suy biến.

Gọi $\mathfrak{q}^0$ là trực giao bù của $\mathfrak{q}$ trong $\mathfrak{g}$ đối với $\Phi$. Điều đi trước chứng minh rằng $\mathfrak{q}\cap \mathfrak{q}^0=\mathfrak{n}$. Giả sử $\mathfrak{q}\not=\mathfrak{q}^0$, khi đó $\mathfrak{q}^0\not=\mathfrak{n}$ (và $\mathfrak{q}^0\supset \mathfrak{n}$). Vì ad$_{\mathfrak{g}}\mathfrak{n}$ để $\mathfrak{q}$ ổn định, ad$_{\mathfrak{g}}\mathfrak{n}$ để $\mathfrak{q}^0$ ổn định; định lý Engel chứng minh rằng tồn tại $x\in \mathfrak{q}^0$ sao cho $x \notin \mathfrak{n}$ và $[x,\mathfrak{n}]\subset \mathfrak{n}$. Nhưng khi đó $x\in \mathfrak{q}^0\cap \mathfrak{q}=\mathfrak{n}$, mâu thuẫn. Vậy $\mathfrak{q}=\mathfrak{n}^0$.

#### Hệ quả 1 {#lie-viii-s10-thm-2-cor-1 .statement tag=016P}

Cho $\mathfrak{q}$ là một phần tử cực đại của tập hợp các đại số con của $\mathfrak{g}$ phân biệt với $\mathfrak{g}$. Khi đó $\mathfrak{q}$ hoặc là parabolic hoặc là khả quy trong $\mathfrak{g}$.

Ta có thể giả sử rằng $\mathfrak{g}$ là một đại số Lie con của $\mathfrak{g}\mathfrak{l}(V)$ đối với một không gian vectơ hữu hạn chiều nào đó V. Gọi $\mathfrak{e}(\mathfrak{q})\subset \mathfrak{g}$ là bao phân tích được của $\mathfrak{q}$. Nếu $\mathfrak{e}(\mathfrak{q}) =\mathfrak{g},\mathfrak{q}$ là một iđêan của $\mathfrak{g}$ (Chương VII, §5, no. 2, Mệnh đề 4), do đó là nửa đơn, và vì thế $\mathfrak{q}$ là khả quy trong $\mathfrak{g}$. Giả sử rằng $\mathfrak{e}(\mathfrak{q})\not=\mathfrak{g}$. Khi đó $\mathfrak{e}(\mathfrak{q}) =\mathfrak{q}$, nên $\mathfrak{q}$ là phân tích được. Giả sử rằng $\mathfrak{q}$ không khả quy trong $\mathfrak{g}$. Gọi $\mathfrak{n}$ là tập hợp các phần tử lũy linh của căn của $\mathfrak{q}$. Khi đó $\mathfrak{n}\not= 0$ (Chương VII, §5, no. 3, Mệnh đề 7 (i)). Gọi $\mathfrak{p}$ là bộ chuẩn hóa của $\mathfrak{n}$ trong $\mathfrak{g}$. Khi đó $\mathfrak{p}\supset \mathfrak{q}$, và $\mathfrak{p}\not=\mathfrak{g}$ vì $\mathfrak{g}$ là nửa đơn. Vậy $\mathfrak{p}=\mathfrak{q}$. Do đó $\mathfrak{q}$ là parabolic (Định lý 1).

#### Hệ quả 2 {#lie-viii-s10-thm-2-cor-2 .statement tag=016Q}

Cho $\mathfrak{n}$ là một đại số con của $\mathfrak{g}$ gồm các phần tử lũy linh. Tồn tại một đại số con parabolic $\mathfrak{q}$ của $\mathfrak{g}$ có các tính chất sau:

(i) $\mathfrak{n}\subset \mathfrak{n}_{\mathfrak{g}}(\mathfrak{q})$;

(ii) chuẩn hóa tử của $\mathfrak{n}$ trong $\mathfrak{g}$ được chứa trong $\mathfrak{q}$;

(iii) mọi tự đẳng cấu của $\mathfrak{g}$ giữ $\mathfrak{n}$ bất biến đều giữ $\mathfrak{q}$ bất biến.

Nếu $\mathfrak{g}$ là phân rã được, thì $\mathfrak{n}$ được chứa trong một đại số con Borel của $\mathfrak{g}$.

Cho $\mathfrak{q}_1$ là bộ chuẩn hóa của $\mathfrak{n}$ trong $\mathfrak{g}$. Đây là một đại số con phân tích được của $\mathfrak{g}$. Đặt $\mathfrak{n}_1=\mathfrak{n}_{\mathfrak{g}}(\mathfrak{q}_1)$. Định nghĩa quy nạp $\mathfrak{q}_i$ là bộ chuẩn hóa của $\mathfrak{n}_{i-1}$ trong $\mathfrak{g}$, và $\mathfrak{n}_i$ bằng $\mathfrak{n}_{\mathfrak{g}}(\mathfrak{q}_i)$. Các dãy $(\mathfrak{n},\mathfrak{n}_1,\mathfrak{n}_2, . . .)$ và $(\mathfrak{q}_1,\mathfrak{q}_2, . . .)$ là tăng. Tồn tại $j$ sao cho $\mathfrak{q}_j=\mathfrak{q}_{j+1}$, nói cách khác $\mathfrak{q}_j$ là bộ chuẩn hóa của $\mathfrak{n}_{\mathfrak{g}}(\mathfrak{q}_j)$ trong $\mathfrak{g}$. Do đó $\mathfrak{q}_j$ là parabolic (Định lý 1). Ta có $\mathfrak{n}\subset \mathfrak{n}_j=$ $\mathfrak{n}_{\mathfrak{g}}(\mathfrak{q}_j)$, và $\mathfrak{q}_1\subset \mathfrak{q}_j$; mọi tự đẳng cấu của $\mathfrak{g}$ để $\mathfrak{n}$ bất biến hiển nhiên cũng để $\mathfrak{n}_1,\mathfrak{n}_2, . .$. và $\mathfrak{q}_1,\mathfrak{q}_2, . .$. bất biến. Nếu $\mathfrak{g}$ phân rã được, $\mathfrak{q}_j$ chứa một đại số con Borel $\mathfrak{b}$, và do đó (§3, no. 4, Mệnh đề 13), ta có $\mathfrak{b}\supset \mathfrak{n}_{\mathfrak{g}}(\mathfrak{q}_j)\supset \mathfrak{n}$.

#### Định lý 3 {#lie-viii-s10-thm-3 .statement tag=016R}

Giả sử rằng $k$ đóng đại số. Cho $\mathfrak{g}$ là một đại số Lie nửa đơn. Cho $\mathfrak{a}$ là một đại số con giải được của $\mathfrak{g}$. Tồn tại một đại số con Borel của $\mathfrak{g}$ chứa $\mathfrak{a}$.

Theo Chương VII, §5, no. 2, Hệ quả 1 (ii) của Mệnh đề 4, ta có thể giả sử rằng $\mathfrak{a}$ phân tích được. Tồn tại một đại số con giao hoán $\mathfrak{t}$ của $\mathfrak{g}$, gồm các phần tử nửa đơn, sao cho $\mathfrak{a}$ là tích nửa trực tiếp của $\mathfrak{t}$ và $\mathfrak{n}_{\mathfrak{g}}(\mathfrak{a})$ (Chương VII, §5, no. 3, Hệ quả 2 của Mệnh đề 6). Tồn tại (Hệ quả 2 của Định lý 2) một đại số con parabolic $\mathfrak{q}$ của $\mathfrak{g}$ sao cho $\mathfrak{n}_{\mathfrak{g}}(\mathfrak{a})\subset \mathfrak{n}_{\mathfrak{g}}(\mathfrak{q})$, và sao cho chuẩn hóa tử của $\mathfrak{n}_{\mathfrak{g}}(\mathfrak{a})$ trong $\mathfrak{g}$ được chứa trong $\mathfrak{q}$; a fortiori$,\mathfrak{a}\subset \mathfrak{q}$. Gọi $\mathfrak{b}$ là một đại số con Borel của $\mathfrak{g}$ được chứa trong $\mathfrak{q}$ và $\mathfrak{h}$ là một đại số con Cartan của $\mathfrak{g}$ được chứa trong $\mathfrak{b}$. Khi đó $\mathfrak{h}$ là một đại số con Cartan của $\mathfrak{q}$, nên tồn tại $s\in$ Aut$_e(\mathfrak{q})$ sao cho $s(\mathfrak{t})\subset \mathfrak{h}$ (Chương VII, §2, no. 3, Mệnh đề 10 và Chương VII, §3, no. 2, Định lý 1). Ta có $s(\mathfrak{n}_{\mathfrak{g}}(\mathfrak{q})) =\mathfrak{n}_{\mathfrak{g}}(\mathfrak{q})$ (Chương VII, §3, no. 1, Nhận xét 1), nên

$$
s(\mathfrak{a}) =s(\mathfrak{t}) +s(\mathfrak{n}_{\mathfrak{g}}(\mathfrak{a}))\subset \mathfrak{h}+s(\mathfrak{n}_{\mathfrak{g}}(\mathfrak{q})) =\mathfrak{h}+\mathfrak{n}_{\mathfrak{g}}(\mathfrak{q})\subset \mathfrak{b}
$$

#### Hệ quả {#lie-viii-s10-n0-cor-1 .statement tag=016S}

Nếu $k$ đóng đại số, mọi đại số con giải được cực đại của $\mathfrak{g}$ đều là một đại số con Borel.

### Bài tập {#lie-viii-s10-exercises}

Xem [các bài tập cho § 10](exercises/s10/).
