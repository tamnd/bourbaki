---
book: evt
book_title: Topological Vector Spaces
chapter: III
chapter_title: SPACES OF CONTINUOUS LINEAR MAPPINGS
section: 2
section_title: Bornological spaces
lang: vi
source: evt-i-v
book_pages: TVS III.11-TVS III.13, TVS III.40-TVS III.41
pdf_pages: 0143-0145, 0172-0173
extraction: ocr
statements: 6
exercises: 4
content_sha256: 0317c818260ffbfa4a3030d900f6cf053698ff49e1c9bb49cb386da2c1e35549
translated_from: content/en/evt/III/02_s2_bornological_spaces.md
source_content_sha256: bb1d36cab9df89b385af8d7360027293742cb8fa7a2b0d897e890f98dbb2fbda
translation_model: gpt-5.4
translation_run: translate-vi-b564a2fb
glossary_version: 34
glossary_terms_sha256: 475f4555179c9c6829a34dad93f09fec44432b57a0b53b3ece5107968bba3600
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 2. KHÔNG GIAN BÔNÔLÔGIC

Trong đoạn này, E ký hiệu một không gian lồi địa phương, và $ \mathcal{B} $ là bônôlôgi chính tắc của nó (III, p. 3, đn. 5).

#### Bổ đề 1 {#evt-iii-s2-lem-1 .statement}

— *Cho G là một không gian nửa định chuẩn, p là nửa chuẩn của nó, và u là một ánh xạ tuyến tính từ G vào E. Các điều kiện sau là tương đương* :

(i) *u liên tục* ;
(ii) *ảnh của quả cầu đơn vị của G qua u bị chặn trong E* ;
(iii) *với mọi dãy $ (x_n) $ các điểm của G hội tụ đến 0, dãy $ (u(x_n)) $ bị chặn trong E*.

Điều hiển nhiên là (i) suy ra (ii) (III, p. 4, hệ quả 1) và (ii) suy ra (iii). Cho V là một lân cận của 0 trong E ; nếu $ u^{-1}(V) $ không là một lân cận của 0 trong G, thì tồn tại một dãy $ (y_n) $ các điểm của $ G - u^{-1}(V) $ sao cho $ p(y_n) \leq \frac{1}{n^2} $. Do đó dãy $ x_n = n y_n $ hội tụ đến 0 trong G và $ u(x_n) \notin nV $, điều này suy ra rằng dãy $ (u(x_n)) $ không bị chặn. Vậy (iii) suy ra (i).

*Mệnh đề 1.* — *Các điều kiện sau là tương đương* :
(i) *Mọi nửa chuẩn trên E bị chặn trên các tập con bị chặn của E đều liên tục*.
(i') *Mọi tập con lồi cân bằng của E hấp thụ các tập con bị chặn của E* (I, p. 7, def. 4) *đều là một lân cận của 0 trong E*.
(ii) *E là giới hạn quy nạp của các không gian nửa chuẩn $ E_A $, trong đó A chạy qua tập có hướng tăng các tập con đóng, lồi, cân bằng và bị chặn của E*.
(ii') *Tồn tại một họ $ (E_i)_{i \in I} $ các không gian nửa chuẩn, và với mọi $ i \in I $, một ánh xạ tuyến tính $ u_i : E_i \to E $ sao cho tôpô của E là tôpô lồi địa phương mịn nhất mà đối với nó các $ u_i $ là liên tục*.
(iii) *Với một không gian lồi địa phương tùy ý F, một ánh xạ tuyến tính $ u : E \to F $ là liên tục khi và chỉ khi với mọi dãy $ (x_n) $ các điểm trong E tiến tới 0, dãy $ (u(x_n)) $ bị chặn trong F*.

(iii') *Với một không gian nửa chuẩn tùy ý F, một ánh xạ tuyến tính u : E → F là liên tục khi và chỉ khi u(X) bị chặn trong F với mọi tập bị chặn X trong E.*

Ngay lập tức thấy rằng (i) và (i') là tương đương, xét đến sự tương ứng giữa các nửa chuẩn và các tập con lồi, cân bằng, hấp thụ (II, p. 20). Nếu p là một nửa chuẩn trên E, liên tục trên mỗi E_A, thì p bị chặn trên các tập con bị chặn của E; do đó (i) suy ra (ii) (II, p. 27, prop. 5). Hiển nhiên rằng (ii) suy ra (ii').

Bây giờ giả sử (E_i, u_i)_{i \in I} như trong (ii') và u là một ánh xạ tuyến tính từ E vào một không gian lồi địa phương F, sao cho (u(x_n)) bị chặn trong F với mọi dãy (x_n) các điểm của E tiến tới 0. Từ bổ đề 1 của III, p. 11 suy ra rằng ánh xạ tuyến tính u \circ u_i : E_i \to F là liên tục với mọi i \in I. Vì thế, nếu tôpô của E là tôpô lồi địa phương mịn nhất mà đối với nó các u_i là liên tục, thì u là liên tục (II, p. 27, prop. 5). Điều này chứng tỏ rằng (ii') suy ra (iii).

Ngay lập tức thấy rằng (iii) suy ra (iii') (III, p. 3, hệ quả.) Cuối cùng, nếu p là một nửa chuẩn trên E, bị chặn trên các tập con bị chặn của E, thì điều kiện (iii') khẳng định rằng ánh xạ đồng nhất là liên tục từ E vào không gian nửa chuẩn (E, p); nói cách khác, p là liên tục. Điều này chứng tỏ rằng (iii') suy ra (i).

#### Định nghĩa 1 {#evt-iii-s2-def-1 .statement}

*Một không gian lồi địa phương được gọi là sinh chặn nếu nó thỏa mãn các điều kiện tương đương của mệnh đề 1.*

#### Ví dụ {#evt-iii-s2-n0-exa-1 .statement}

— 1) Mọi không gian nửa chuẩn đều là sinh chặn.
2) Đặc biệt, mọi không gian lồi địa phương hữu hạn chiều đều là sinh chặn.
3) Do tính bắc cầu của các tôpô lồi địa phương cuối cùng (II, p. 28, hệ quả 2), ta suy ra ngay từ điều kiện (ii') rằng nếu (E_i)_{i \in I} là một họ các không gian lồi địa phương sinh chặn và nếu E được trang bị tôpô lồi địa phương mịn nhất mà đối với nó các ánh xạ tuyến tính u_i : E_i \to E (với i \in I) là liên tục, thì E là sinh chặn. Đặc biệt, *một giới hạn quy nạp, một tổng trực tiếp, một không gian thương của các không gian sinh chặn đều là các không gian sinh chặn*.

Mặt khác, một không gian con đóng của một không gian sinh chặn không nhất thiết là sinh chặn (IV, p. 63, exerc. 8).

#### Hệ quả {#evt-iii-s2-n0-cor-1 .statement}

*Mọi không gian sinh chặn Hausdorff và bán đầy đủ đều là một giới hạn quy nạp của các không gian Banach.*

Thật vậy, các không gian E_A, trong đó A đóng và bị chặn, là các không gian Banach (III, p. 8, hệ quả).

#### Mệnh đề 2 {#evt-iii-s2-prop-2 .statement}

*Một không gian lồi địa phương mêtric hóa được là sinh chặn.*

Giả sử E là mêtric hóa được, và p là một nửa chuẩn trên E bị chặn trên các tập con bị chặn của E, nhưng không liên tục. Gọi A là tập hợp mọi x \in E sao cho p(x) < 1. Gọi (V_n)_{n \geq 1} là một dãy giảm tạo thành một hệ cơ bản các lân cận của 0 trong E. Vì p không liên tục, A không phải là một lân cận của 0; do đó với mọi n > 0, ta có A \not\supseteq n^{-1} V_n và tồn tại một điểm x_n trong V_n sao cho n^{-1} x_n \notin A, nghĩa là, p(x_n) \geq n. Dãy (x_n) tiến tới 0, nên bị chặn (III, p. 3, hệ quả); điều này mâu thuẫn với giả thiết về p.

#### Hệ quả {#evt-iii-s2-n0-cor-2 .statement}

— *Mọi không gian Fréchet* (II, p. 24) *đều là giới hạn quy nạp của các không gian Banach*.

### Bài tập {#evt-iii-s2-exercises}

Xem [bài tập của § 2](exercises/s2/).
