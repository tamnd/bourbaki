---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: ""
chapter_title: ""
section: 0
section_title: INTRODUCTION TO CHAPTERS IV, V AND VI
kind: introduction
lang: vi
source: lie-iv-vi
pdf_pages: 0006-0007
extraction: ocr
statements: 0
exercises: 0
content_sha256: 124dbe076a6f54d93ccb2a56f6da11680867dca18fb5b9b0e5c5ff75e7feddaf
translated_from: content/en/lie/00_introduction.md
source_content_sha256: 6039920d984a1193244721622035fbdcfccd3343c37bff11d7a710933b56f4fb
translation_model: gpt-5-mini, gpt-5-6-mini
translation_run: translate-vi-4a466f90
glossary_version: 34
glossary_terms_sha256: bba221ffcbb6144187f2e6a17bab40482e56c51d5c591269f4c8845a12b211a8
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## GIỚI THIỆU CÁC CHƯƠNG IV, V VÀ VI

Việc nghiên cứu các nhóm nửa đơn (giải tích hoặc đại số) và các đại số Lie của chúng dẫn đến việc xét các hệ nghiệm, các nhóm Coxeter và các hệ Tits. Các Chương IV, V và VI được dành cho các cấu trúc này.

Để định hướng cho độc giả, chúng tôi đưa ra dưới đây một vài ví dụ.

I. Cho $g$ là một đại số Lie nửa đơn phức và $h$ là một đại số con Cartan của $g^1$. Một nghiệm của $g$ đối với $h$ là một dạng tuyến tính không của $g$ khác không $\alpha$ trên $h$ sao cho tồn tại một phần tử khác không $x$ của $g$ với $[h, x] = \alpha(h)x$ với mọi $h \in h$. Các nghiệm này tạo thành một hệ căn rút gọn $R$ trong không gian vectơ $h^*$ đối ngẫu với $h$. Việc cho $R$ xác định $g$ sai khác một đẳng cấu và mọi hệ căn rút gọn đều đẳng cấu với một hệ nghiệm thu được theo cách này. Một tự đẳng cấu của $g$ giữ $h$ ổn định xác định một tự đẳng cấu của $h^*$ giữ $R$ bất biến, và mọi tự đẳng cấu của $R$ đều thu được theo cách này. Nhóm Weyl của $R$ gồm tất cả các tự đẳng cấu của $h^*$ được xác định bởi các tự đẳng cấu nội của $g$ giữ $h$ ổn định; đây là một nhóm Coxeter.

Cho $G$ là một nhóm Lie liên thông phức có đại số Lie là $g$, và cho $\Gamma$ là nhóm con của $G$ gồm các phần tử $h$ sao cho $\exp_G(2\pi i h) = 1$. Cho $R^-$ là hệ nghiệm trong $h$ nghịch đảo với $R$, cho $Q(R^-)$ là nhóm con của $h$ sinh bởi $R^-$ và cho $P(R^-)$ là nhóm con liên kết với nhóm con $Q(R)$ của $h^*$ sinh bởi $R$ (nghĩa là tập hợp các $h \in h$ sao cho $\lambda(h)$ là một số nguyên với mọi $\lambda \in Q(R)$). Khi đó $P(R^-) \supset \Gamma \supset Q(R^-)$. Hơn nữa, tâm của $G$ đẳng cấu một cách chính tắc với $P(R^-)/\Gamma$ và nhóm cơ bản của $G$ đẳng cấu với $\Gamma/Q(R^-)$. Đặc biệt, $\Gamma$ bằng $P(R^-)$ nếu $G$ là nhóm phụ hợp và $\Gamma$ bằng $Q(R^-)$ nếu $G$ là đơn liên. Cuối cùng, các trọng số của các biểu diễn tuyến tính hữu hạn chiều của $G$ là các phần tử của nhóm con của $h^*$ liên kết với $\Gamma$.

II. Cho $G$ là một nhóm Lie thực compact liên thông nửa đơn, và $g$ là đại số Lie của nó. Cho $T$ là một xuyến cực đại của $G$, với đại số Lie $t$, và cho $X$ là nhóm các ký tự của $T$. Cho $R$ là tập hợp các phần tử khác không $\alpha$ của $X$ sao cho tồn tại một phần tử khác không $x$ của $g$ với $(\mathrm{Ad}\, t).x = \alpha(t)x$ với mọi $t \in T$. Đồng nhất $X$ với một dàn trong không gian vectơ thực $V = X \otimes_{\mathbf{Z}} \mathbf{R}$; khi đó $R$ là một hệ căn rút gọn trong $V$. Cho $N$ là chuẩn hoá tử của $T$ trong $G$; tác động

1 Trong Lời giới thiệu này, chúng tôi sử dụng tự do thuật ngữ truyền thống cũng như các khái niệm được định nghĩa trong các Chương IV, V và VI.

của $N$ trên $T$ xác định một đẳng cấu từ nhóm $N/T$ vào nhóm Weyl của $R$. Ta có $P(R) ⊃ X ⊃ Q(R)$; hơn nữa, $X = P(R)$ nếu $G$ đơn liên và $X = Q(R)$ nếu tâm của $G$ thu gọn thành phần tử đơn vị.

Đại số Lie phức hoá $g_{(C)}$ của $g$ là nửa đơn và $t_{(C)}$ là một đại số con Cartan của nó. Tồn tại một đẳng cấu chính tắc từ $V_{(C)}$ vào đối ngẫu của $t_{(C)}$ biến $R$ thành hệ nghiệm của $g_{(C)}$ đối với $t_{(C)}$.

III. Cho G là một nhóm đại số nửa đơn liên thông trên một trường giao hoán $k$. Cho T là một phần tử cực đại của tập hợp các xuyến của G tách trên $k$ và cho X là nhóm các ký tự của T (các đồng cấu từ T vào nhóm nhân). Ta đồng nhất X với một dàn trong không gian vectơ thực $V = X \otimes_{\mathbf{Z}} \mathbf{R}$. Các nghiệm của G đối với T là các phần tử khác không $\alpha$ của X sao cho tồn tại một phần tử khác không $x$ của đại số Lie $g$ của G với $(\mathrm{Ad}\, t).x = \alpha(t)x$ với mọi $t \in T$. Điều này cho một hệ nghiệm R trong V, không nhất thiết phải rút gọn. Cho N là chuẩn hoá tử và Z là tâm hoá tử của T trong G và cho $N(k)$ và $Z(k)$ là các nhóm các điểm hữu tỉ của chúng trên $k$. Tác động của $N(k)$ trên T xác định một đẳng cấu từ $N(k)/Z(k)$ vào nhóm Weyl của R.

Cho U là một phần tử cực đại của tập hợp các nhóm con lũy linh của G, được xác định trên $k$ và được chuẩn hoá bởi Z. Đặt $P = Z.U$. Khi đó $P(k) = Z(k).U(k)$ và $P(k) \cap N(k) = Z(k)$. Hơn nữa, tồn tại một cơ sở $(\alpha_1, \ldots, \alpha_n)$ của R sao cho các trọng của T trong U là các nghiệm dương của R đối với cơ sở này; nếu S là tập hợp các phần tử của $N(k)/Z(k)$ tương ứng, qua đẳng cấu được xác định ở trên, với các phép đối xứng $s_{\alpha_i} \in W(R)$ liên kết với các nghiệm $\alpha_i$, thì bộ bốn $(G(k), P(k), N(k), S)$ là một hệ Tits.

IV. Trong lý thuyết các nhóm đại số nửa đơn trên một trường địa phương, ta gặp các hệ Tits mà nhóm Weyl của chúng là nhóm Weyl affine của một hệ nghiệm. Ví dụ, cho $G = \mathbf{SL}(n+1, \mathbf{Q}_p)$ (với $n \geq 1$). Cho B là nhóm các ma trận $(a_{ij}) \in \mathbf{SL}(n+1, \mathbf{Z}_p)$ sao cho $a_{ij} \in p\mathbf{Z}_p$ với $i < j$, và cho N là nhóm con của G gồm các ma trận chỉ có một phần tử khác không trong mỗi hàng và mỗi cột. Khi đó tồn tại một tập con S của $N/(B \cap N)$ sao cho bộ bốn $(G, B, N, S)$ là một hệ Tits. Nhóm $W = N/(B \cap N)$ là nhóm Weyl affine của một hệ nghiệm kiểu $A_n$; đây là một nhóm Coxeter vô hạn.

Nhiều cuộc trao đổi với J. Tits đã có sự trợ giúp vô giá đối với chúng tôi trong việc chuẩn bị các chương này. Chúng tôi chân thành cảm ơn ông.
