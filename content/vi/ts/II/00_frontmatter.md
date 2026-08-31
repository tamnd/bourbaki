---
book: ts
book_title: Théories spectrales
chapter: II
chapter_title: GROUPES LOCALEMENT COMPACTS COMMUTATIFS
section: 0
section_title: GROUPES LOCALEMENT COMPACTS COMMUTATIFS
kind: front
lang: vi
source: ts-i-ii-fr
book_pages: TS II.199-TS II.200
pdf_pages: 0211-0212
extraction: native
statements: 0
exercises: 0
content_sha256: ec71b15636c46ee40c7fe40c94be71588fbfd95ea029c314f6932e3dcf5bd702
translated_from: content/en-mt/ts/II/00_frontmatter.md
source_lang: en-mt
translation_method: machine
source_content_sha256: ac933dd2b350523831b4b93be737609a274c5a1c52ebe24ee0bd80640061df4f
translation_model: gpt-5.4
translation_run: translate-vi-494db22c
glossary_version: 34
glossary_terms_sha256: af70793382af3e327c40a3dd64c340de4bdfe7d839613e4456fc410bd8f744c4
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## CHƯƠNG II

# Các nhóm giao hoán địa phương compact

Trong suốt chương này, chữ G chỉ, trừ khi có nói khác, một nhóm giao hoán địa phương compact được trang bị một độ đo Haar thường được ký hiệu bởi $dx$; với $p\in [1,+\infty ]$, không gian $L^p(G, dx)$ sẽ được ký hiệu đơn giản là $L^p(G)$, và chuẩn của nó sẽ được ký hiệu bởi $f\mapsto  \|f\|_p$. Ta đồng nhất $L^1(G)$ với một không gian con của $\mathscr{M}^1(G)$ bằng ánh xạ chính tắc $f\mapsto f\cdot dx$. Nhắc lại rằng giá của độ đo Haar bằng G (INT, VII, §1, n$^o1$, nhận xét 3); đặc biệt (INT, III, §2, n$^o2$, mệnh đề 9), ánh xạ chính tắc từ không gian $\mathscr{K}(G)$ vào $L^p(G)$ là đơn ánh với $p\in [1,+\infty ]$. Với $p\not= +\infty$, ta sẽ đồng nhất $L^p(G)$ với một không gian con của không gian $\widetilde{\mathscr{F}}(G;\mathbf{C})$ gồm các lớp hàm nhận giá trị phức trên G, xác định và hữu hạn hầu khắp nơi (INT, IV, §3, n$^o5$, n$^o6$). Đặc biệt, ký hiệu $L^1(G)\cap L^2(G)$ chỉ giao của $L^1(G)$ và $L^2(G)$ trong không gian này. Ta ký hiệu bởi $f\mapsto \widetilde{f}$ phép đối hợp trên đại số có đối hợp $L^1(G)$ (ví dụ 4 của I, p. 99); ta có $\widetilde{f}(x) =\overline{f(x^{-1})}$ với mọi $x$ trong G.

Nhắc lại (INT, V, §5, n$^o3$, th. 1) rằng nếu $\mu$ là một độ đo phức trên một không gian tôpô địa phương compact X và nếu $f$ là một hàm khả tích địa phương đối với $\mu$ trên X, thì độ đo $\nu$ có mật độ $f$ đối với $\mu$ được ký hiệu là $f\cdot \mu$ hoặc cũng là $f \mu$. Một hàm $g$ từ X vào $\mathbf{C}$ là khả tích thiết yếu đối với độ đo $\nu$ khi và chỉ khi $gf$ là khả tích thiết yếu đối với $\mu$; khi đó ta có

$$
(f\cdot \mu)(g) =\int_Xgd(f\cdot \mu) =\int_Xgf d\mu=\mu(gf)
$$

Nếu G là một nhóm tôpô compact, độ đo Haar chuẩn hóa trên G được gọi là độ đo Haar duy nhất $\mu$ trên G sao cho $\mu(G) = 1$.

Nếu X là một không gian tôpô rời rạc, độ đo đếm trên X được gọi là độ đo rời rạc $\mu$ trên X sao cho $\mu(\{x\}) = 1$ với mọi $x\in X$. Nếu G là một nhóm tôpô rời rạc, độ đo đếm trên G là một độ đo Haar trên G.

Ta cũng sẽ dùng hai bổ đề sau.

**Bổ đề 1.** — Cho X là một không gian tôpô địa phương compact và $\mu$ là một độ đo dương trên X. Cho $x$ là một phần tử của giá của $\mu$. Cho U là một lân cận mở của $x$. Tồn tại một hàm $f\in \mathscr{K}_+(X)$ mà giá được chứa trong U sao cho $\int f d\mu= 1$.

Theo định nghĩa của giá của một độ đo (INT, III, §2, n$^o2$, def. 1), tồn tại một hàm $g\in \mathscr{K}(X)$ có giá chứa trong U sao cho $\mu(g)\not= 0$. Khi đó ta có $\mu(|g|)>0$ vì $\mu$ là dương, và hàm $f=\mu(|g|)^{-1}|g|$ có các tính chất cần tìm.

**Bổ đề 2.** — Cho G và H là các nhóm tôpô có các phần tử đơn vị $e_G$ và $e_H$; giả sử rằng nhóm tôpô G là tách. Cho $f$ là một đồng cấu các nhóm tôpô từ G vào H. Giả sử rằng với mọi lân cận U của $e_G$ trong G, tồn tại một lân cận W của $e_H$ trong H sao cho $\overset{-1}{f}(W)\subset U$. Khi đó đồng cấu $f$ là đơn ánh và ngặt (TG, III, p. 16, def. 1).

Các giả thiết kéo theo rằng Ker($f$) được chứa trong mọi lân cận của $e_G$ trong G, do đó Ker($f$) $=\{e_G\}$ vì G là tách. Khi đó đồng cấu từ G vào $f(G)$ suy ra từ $f$ bằng cách chuyển qua các không gian con là song ánh; ký hiệu bởi $g:f(G)\rightarrow G$ đồng cấu nghịch đảo. Khi đó các giả thiết kéo theo rằng $g$ liên tục tại $e_H$, do đó liên tục (TG, III, p. 15, prop. 23).
