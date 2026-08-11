---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 3
section_title: Hilbert’s Nullstellensatz
appendix: true
lang: vi
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.461-A VIII.462
pdf_pages: 0478-0479
extraction: native
statements: 3
exercises: 0
content_sha256: 7c4fd824eb0e3e20ccefcc64916d5999a91e528d0a689475af9f52d3464111ea
translated_from: content/en/alg/VIII/A3_a3_hilbert_s_nullstellensatz.md
source_content_sha256: ed79b6c8c8435d95bb1c4ac0037daf25f70b49402c1cdbcf88620ae44264cfbb
translation_model: gpt-5-6
translation_run: translate-vi-ab0abfcc
glossary_version: 5
prompt_sha256: 7816e1600c72058e14ecd8b330e9a16e059e370f96fa366ad5fc8f147bcd8dd9
---

## PHỤ LỤC 3 NULLSTELLENSATZ CỦA HILBERT

#### Định lý 1 {#alg-viii-a3-thm-1 .statement tag=00QM}

Cho A là một miền nguyên, K là trường phân thức của nó, và L là một đại số giao hoán K. Giả sử rằng đại số trên A L được sinh bởi hữu hạn phần tử và L là một trường.

a) Bậc của L trên K là hữu hạn.

b) Tồn tại một phần tử khác không $a$ của A sao cho K bằng $A[a^{-1}]$.

Cho S là một tập con sinh của đại số trên A L. Ta dùng quy nạp theo lực lượng của S.

Trước hết, giả sử các phần tử của S đều đại số trên K. Khi đó bậc của L trên K là hữu hạn (V, §3, No. 2, p. 18, Định lý 2). Gọi $(e_i)_{i\in I}$ là một cơ sở của L trên K. Tồn tại một phần tử khác không $a$ của A sao cho các tọa độ theo cơ sở này của các phần tử của S, của phần tử 1, và của các phần tử $e_ie_j$ với $i,j$ thuộc I đều thuộc $A[a^{-1}]$. Tập các tổ hợp tuyến tính $\sum_{i\in I}a_ie_i$ với $a_i\in A[a^{-1}]$ với mọi $i$ khi đó là một vành con của L. Theo phép dựng, nó chứa A và S, do đó bằng L. Đặc biệt, nó chứa $Ke_1$, nên K bằng $A[a^{-1}]$.

Giả sử một phần tử $s$ của S là siêu việt trên K. Ký hiệu E là trường các phân thức của vành $A[s]$. Đại số $A[s$]-L được sinh bởi S $\{s\}$. Theo giả thiết quy nạp, tồn tại một đa thức $P\in A[X]$ khác không sao cho E bằng $A[s][P(s)^{-1}]$. Cho K là một bao đóng đại số của K (V, §4, No. 3, p. 23, Định lý 2). Vì trường K là vô hạn (V, §4, No. 1, p. 20, Mệnh đề 3), tồn tại một phần tử $x$ của K sao cho $P(x)\not= 0$. Gọi $\varphi : E\rightarrow K$ là đồng cấu duy nhất từ đại số K $E = A[s][P(s)^{-1}]$ vào đại số K K biến $s$ thành $x$. Điều này là vô lý vì E là một mở rộng siêu việt của K và K là một mở rộng đại số của K. Điều này hoàn tất chứng minh định lý.

#### Hệ quả 1 {#alg-viii-a3-thm-1-cor-1 .statement tag=00RV}

Cho K là một trường giao hoán, A là một đại số giao hoán K được sinh bởi hữu hạn phần tử, và $\mathfrak{m}$ là một iđêan cực đại của A.

a) Bậc của $A/\mathfrak{m}$ trên K là hữu hạn.

b) Cho Ω là một mở rộng đóng đại số của K. Tồn tại một đồng cấu đại số K từ A vào Ω có hạt nhân $\mathfrak{m}$.

Đại số $A/\mathfrak{m}$ được sinh bởi hữu hạn phần tử, và $A/\mathfrak{m}$ là một trường. Theo Định lý 1, bậc của $A/\mathfrak{m}$ là hữu hạn; mệnh đề a) được suy ra. Mọi mở rộng K có bậc hữu hạn đều đẳng cấu với một mở rộng con của Ω (V, §4, No. 1, p. 20, Định lý 1); điều này cho b).

#### Hệ quả 2 {#alg-viii-a3-thm-1-cor-2 .statement tag=00QN}

Cho K là một trường giao hoán, $n$ là một số tự nhiên, $(P_i)_{i\in I}$ là một họ các phần tử của $K[X_1, . . . ,X_n]$, và Ω là một mở rộng đóng đại số của K. Các điều kiện sau là tương đương:

(i) Các đa thức $P_i$ không có không điểm chung nào trong $\Omega^n$.

(ii) Tồn tại một họ $(Q_i)_{i\in I}$, có giá hữu hạn, gồm các phần tử của $K[X_1, . . . ,X_n]$ sao cho $\sum_{i\in I}P_iQ_i= 1$.

Gọi A là vành $K[X_1, . . . ,X_n]$ và $\mathfrak{a}$ là iđêan sinh bởi đa thức $P_i$. Điều kiện (i) có nghĩa là không có đồng cấu đại số K nào từ $A/\mathfrak{a}$ vào Ω. Nếu điều kiện này được thỏa mãn thì theo Hệ quả 1, vành $A/\mathfrak{a}$ không có iđêan cực đại nào và do đó là không, và 1 thuộc $\mathfrak{a}$. Điều này chứng minh rằng (i) suy ra (ii). Hàm ý (ii) $\Rightarrow$ (i) là hiển nhiên.
