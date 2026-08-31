---
book: ts
book_title: Théories spectrales
chapter: III
chapter_title: APPLICATIONS LINÉAIRES COMPACTES ET PERTURBATIONS
section: 0
section_title: APPLICATIONS LINÉAIRES COMPACTES ET PERTURBATIONS
kind: front
lang: vi
source: ts-iii-v-fr
book_pages: TS III.1-TS III.2
pdf_pages: 0015-0016
extraction: native
statements: 0
exercises: 0
content_sha256: 6156fdaab70880a84a771b465ad5ba07eea8b3f64c3c2e7e32202c9072e3bb87
translated_from: content/en-mt/ts/III/00_frontmatter.md
source_lang: en-mt
translation_method: machine
source_content_sha256: cf641e4cbb31fe3db85b127e2ad05f309c8c542af9c2da074b4581d2bd1d69cb
translation_model: gpt-5.4
translation_run: translate-vi-95b72767
glossary_version: 34
glossary_terms_sha256: 02102fcf90e2b64a0f1816a85c4fbb798ca616cc9d40052ac369556d86493a92
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## CHƯƠNG III

# Ánh xạ tuyến tính compact và nhiễu loạn

Trong chương này, tất cả các không gian vectơ được xét đều là các không gian vectơ trên một trường K bằng $\mathbf{R}$ hoặc $\mathbf{C}$. Các dẫn chiếu đến EVT, II trong sách này nói chung liên quan đến trường hợp $K =\mathbf{R}$; đối với trường hợp $K =\mathbf{C}$, xem EVT, II, p. 64 đến 68.

Một không gian nửa định chuẩn là một không gian vectơ E được trang bị một nửa chuẩn $p$ và tôpô xác định bởi $p($xem EVT, II, p. 2). Quả cầu đơn vị của E, hay của $p$, được gọi là tập hợp các phần tử $x$ của E sao cho $p(x)\leqslant 1$.

Với mọi không gian vectơ E, $1_E$ ký hiệu ánh xạ đồng nhất của E. Nếu E, F và G là các không gian vectơ và $u: E\rightarrow F,v: F\rightarrow G$ là các ánh xạ tuyến tính, đôi khi người ta ký hiệu bởi $vu$ ánh xạ tuyến tính $v\circ u$ từ E vào G.

Cho E và F là các không gian vectơ tôpô. Một ánh xạ tuyến tính liên tục từ E vào F cũng sẽ được gọi là một cấu xạ, và là một tự đồng cấu khi F = E. Một ánh xạ tuyến tính song ánh từ E vào F, liên tục và có nghịch đảo cũng liên tục, sẽ được gọi là một đẳng cấu, và khi F = E, là một tự đẳng cấu. Khi E và F là các không gian nửa định chuẩn, các khái niệm tự đồng cấu, đẳng cấu và tự đẳng cấu liên quan đến cấu trúc không gian vectơ tôpô nền.

Với các không gian vectơ tôpô E và F, $\mathscr{L}^f(E; F)$ ký hiệu không gian vectơ các ánh xạ tuyến tính liên tục hạng hữu hạn từ E vào F. Người ta cũng ký hiệu bởi $\mathscr{L}^f(E)$ không gian vectơ $\mathscr{L}^f(E; E)$.

Nhắc lại rằng một ánh xạ tuyến tính liên tục $u$ từ E vào F là ngặt nếu nó cảm sinh, bằng cách chuyển qua thương, một đẳng cấu của $E/$ Ker($u$) lên $u(E)$ (TG, III, p. 16, déf. 1); điều đó tương đương với nói rằng ảnh của mọi lân cận của 0 trong E là một lân cận của 0 trong $u(E)$ (TG, III, p. 16, prop. 24).
