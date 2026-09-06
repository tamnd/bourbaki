---
book: top
book_title: General Topology
chapter: IX
chapter_title: UTILISATION DES NOMBRES RÉELS EN TOPOLOGIE GÉNÉRALE
section: 1
section_title: Espaces de Lindelöf
appendix: true
lang: vi
source: top-v-x-fr
pdf_pages: 0195-0197
extraction: ocr
statements: 8
exercises: 0
content_sha256: b872381b94e865d9b288374e307f08584da8de6cb1bfb32fee005e990397d274
translated_from: content/en-mt/top/IX/A1_a1_espaces_de_lindelof.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 5aac80a9b98ddbb1cf5a95c04cc8ed38c807091d7166c22e6a9660e70b077fde
translation_model: gpt-5-6
translation_run: translate-vi-0af31321
glossary_version: 34
glossary_terms_sha256: 47ef48c3424138c158396502ef870447dccdd7d8fa0f05822d916e764d32a36b
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## PHỤ LỤC 1

# CÁC KHÔNG GIAN LINDELÖF

#### Định nghĩa 1 {#top-ix-a1-def-1 .statement}

Người ta nói rằng một không gian tôpô $X$ (không nhất thiết tách được) là một không gian Lindelöf nếu, từ mọi phủ mở của $X$, có thể trích ra một phủ đếm được của $X$.

#### Mệnh đề 1 {#top-ix-a1-prop-1 .statement}

Cho $X$ là một không gian tôpô.

(i) Nếu tôpô của $X$ có một cơ sở đếm được, thì $X$ là một không gian Lindelöf.

(ii) Cho $f : X \to Y$ là một ánh xạ liên tục từ $X$ vào một không gian tôpô $Y$ (không nhất thiết tách được). Nếu $X$ là một không gian Lindelöf, thì điều tương tự cũng đúng với không gian con $f(X)$ của $Y$.

(i) Cho $\mathcal{R}$ là một phủ mở của $X$, $\mathcal{B}$ là một cơ sở đếm được của tôpô của $X$, $\mathcal{B}'$ là tập hợp các phần tử $A \in \mathcal{B}$ sao cho tồn tại một phần tử của $\mathcal{R}$ chứa $A$; $\mathcal{B}'$ là một phủ đếm được của $X$, vì mọi $x \in X$ đều được chứa trong một tập hợp $U \in \mathcal{R}$, và khi đó tồn tại $A \in \mathcal{B}$ sao cho $x \in A \subset U$. Khi đó tồn tại một ánh xạ $\Phi$ từ $\mathcal{B}'$ vào $\mathcal{R}$ sao cho $A \subset \Phi(A)$ với mọi $A \in \mathcal{B}'$; hiển nhiên rằng $\Phi(\mathcal{B}')$ là một phủ mở đếm được của $X$ được chứa trong $\mathcal{R}$.

(ii) Cho $(V_\lambda)_{\lambda \in L}$ là một họ các tập mở trong $Y$ tạo thành một phủ của $f(X)$. Khi đó các tập $f^{-1}(V_\lambda)$ tạo thành một phủ mở của $X$, và do đó tồn tại một tập con đếm được $J$ của $L$ sao cho các tập mở $f^{-1}(V_\lambda)$ với $\lambda \in J$ tạo thành một phủ của $X$. Nhưng khi đó các tập $V_\lambda$ với $\lambda \in J$ tạo thành một phủ của $f(X)$, điều này chứng minh rằng $f(X)$ là một không gian Lindelöf.

#### Hệ quả {#top-ix-a1-n0-cor-1 .statement}

*Mọi không gian Lindelöf con, và đặc biệt mọi không gian Polish hoặc Lusin, đều là một không gian Lindelöf.*

Điều này suy ra ngay lập tức từ mệnh đề trước đó 1 và từ định nghĩa của các không gian Lindelöf con (IX, p. 59, định nghĩa 2), vì một không gian Polish có một cơ sở đếm được.

#### Mệnh đề 2 {#top-ix-a1-prop-2 .statement}

*Mọi không gian Lindelöf chính quy đều là paracompact.*

Cho $X$ là một không gian Lindelöf chính quy, và $\mathcal{R}$ là một phủ mở của $X$. Với mọi $x \in X$, lấy $U_x \in \mathcal{R}$ chứa $X$, và lấy $V_x$ là một lân cận mở của $x$ sao cho $V_x \subset U_x$. Vì $X$ là một không gian Lindelöf, tồn tại một dãy $(x_n)_{n \geq 0}$ các điểm của $X$ sao cho các $V_{x_n}$ tạo thành một phủ của $X$. Khi đó, với mọi số nguyên $n \geq 0$, đặt $W_n = U_{x_n} \cap \complement \left( \bigcup_{k < n} V_{x_k} \right)$. Các tập hợp $W_n$ là mở và tạo thành một phủ của $X$ mịn hơn $\mathcal{R}$. Mặt khác, phủ này là hữu hạn địa phương, vì mọi $x \in X$ thuộc một $V_{x_i}$ nào đó với ít nhất một $i$; khi đó $V_{x_i}$ là một lân cận của $x$, không gặp tập hợp $W_n$ nào với $n > i$.

#### Hệ quả {#top-ix-a1-n0-cor-2 .statement}

*Mọi không gian sublinian chính quy đều là paracompact* (và đặc biệt là *chuẩn tắc* (IX, p. 49, mệnh đề 4) và *a fortiori hoàn toàn chính quy*).

#### Mệnh đề 3 {#top-ix-a1-prop-3 .statement}

*Một không gian tôpô $X$ (không nhất thiết tách được). Các tính chất sau là tương đương*:
a) *Mọi không gian con mở của $X$ là một không gian Lindelöf*.
b) *Mọi tập hợp các hàm nửa liên tục dưới (tương ứng nửa liên tục trên) trong $X$ chứa một tập con đếm được có cùng bao trên (tương ứng bao dưới)*.

Trước hết hãy chứng minh rằng b) suy ra a). Cho $U$ là một không gian con mở của $X$, và $(U_\lambda)_{\lambda \in L}$ là một họ các tập hợp mở trong $U$ (do đó trong $X$) phủ $U$. Vì các hàm $\varphi_{U_\lambda}$ là nửa liên tục dưới trong $X$, tồn tại một tập con đếm được $J$ của $L$ sao cho họ $(\varphi_{U_\lambda})_{\lambda \in J}$ có cùng bao trên $\varphi_U$ với họ $(\varphi_{U_\lambda})_{\lambda \in L}$. Do đó, $U = \bigcup_{\lambda \in J} U_\lambda$, và $U$ là một không gian Lindelöf.

Bây giờ hãy chứng minh rằng a) suy ra b). Cho $\mathcal{F}$ là một tập hợp các hàm nửa liên tục dưới trong $X$, và cho $s$ là bao trên của $\mathcal{F}$. Cho $D$ là một tập con trù mật đếm được của $\overline{\mathbf{R}}$. Với mọi hàm $f \in \mathcal{F}$ và mọi số $d \in D$, gọi $U_{f,d}$ là tập hợp mở của các $x \in X$ sao cho $f(x) > d$ (IV, p. 29). Theo giả thiết, tồn tại một tập con đếm được $\mathcal{F}_d'$ của $\mathcal{F}$ sao cho

$$
\bigcup_{f \in \mathcal{F}} U_{f,d} = \bigcup_{f \in \mathcal{F}_d'} U_{f,d}.
$$

Cho $\mathcal{F}' = \bigcup_{d \in D} \mathcal{F}'_d$, và ký hiệu $s'$ là bao trên của $\mathcal{F}'$. Hiển nhiên ta có $s \geqslant s'$; mặt khác, cho $x$ là một điểm của $X$, và cho $d$ là một phần tử của $D$ sao cho $s(x) > d$; tồn tại một hàm $f \in \mathcal{F}$ sao cho $f(x) > d$; do đó $x \in U_{f,d}$, và tồn tại một hàm $f' \in \mathcal{F}'_d$ sao cho $x \in U_{f',d}$. Do đó, ta cũng có $s'(x) > d$, từ đó có bất đẳng thức $s' \geqslant s$, và cuối cùng $s' = s$. Vì $\mathcal{F}'$ là đếm được, mệnh đề được thiết lập cho các hàm nửa liên tục dưới; trường hợp các hàm nửa liên tục trên được quy về trường hợp này bằng cách đổi dấu.

#### Hệ quả 1 {#top-ix-a1-prop-3-cor-1 .statement}

*Cho $X$ là một không gian souslin chính quy, $H$ là một tập hợp các hàm số liên tục trên $X$, tách các điểm của $X$* (IX, p. 9, định nghĩa 5). *Khi đó tồn tại một tập con đếm được $H'$ của $H$ tách các điểm của $X$*.

Thật vậy, $X \times X$ là một không gian souslin (IX, p. 60, mệnh đề 7); điều tương tự cũng đúng với mọi không gian con mở của $X \times X$ (IX, p. 59, mệnh đề 5), do đó nó là một không gian Lindelöf (IX, p. 76, hệ quả). Với mỗi hàm $h \in H$, gán cho tập đóng $F_h$ gồm các cặp $(x, y) \in X \times X$ sao cho $h(x) = h(y)$. Theo mệnh đề 3, tồn tại một tập con đếm được $H'$ của $H$ sao cho ta có $\bigcap_{h \in H'} F_h = \bigcap_{h \in H} F_h$. Nhưng theo giả thiết, vế thứ hai là đường chéo của $X \times X$; do đó điều tương tự cũng đúng với vế thứ nhất, và vì vậy $H'$ tách các điểm của $X$.

#### Hệ quả 2 {#top-ix-a1-prop-3-cor-2 .statement}

*Mọi không gian souslin compact đều mêtric hóa được*.

Cho $X$ là một không gian souslin compact, $I$ là khoảng $[0, 1]$ của $\mathbf{R}$, $H$ là tập hợp các ánh xạ liên tục từ $X$ vào $I$. Vì $X$ là chính quy hoàn toàn, $H$ tách các điểm của $X$, và hệ quả 1 suy ra sự tồn tại của một dãy $(f_n)$ các phần tử của $H$ tách các điểm của $X$. Nhưng khi đó ánh xạ $x \mapsto (f_n(x))_{n \in \mathbf{N}}$ từ $X$ vào $I^\mathbf{N}$, liên tục và đơn ánh, là một phép đồng phôi của không gian compact $X$ lên một không gian con của $I^\mathbf{N}$; điều này chứng minh rằng $X$ mêtric hóa được.
