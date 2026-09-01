---
book: ac
book_title: Commutative Algebra
chapter: I
chapter_title: FLAT MODULES
section: 4
section_title: Flat modules and "Tor" functors
lang: vi
source: ac-i-vii
book_pages: 37-38, 50
pdf_pages: 0057-0058, 0070-0070
extraction: ocr
statements: 3
exercises: 1
content_sha256: b879d4d60fcaaa8f1d12b4ae4a138533fbf9f9b0b3dfc42441a6c52daa949938
translated_from: content/en/ac/I/04_s4_flat_modules_and_tor_functors.md
source_content_sha256: 9fd11944f9ccd26af40fbfd7087174fd30283103e635ee58c967ecaf0bfa5f58
translation_model: gpt-5.4
translation_run: translate-vi-9b653a8f
glossary_version: 34
glossary_terms_sha256: 7ced34067a1896236338e2bd92b3ecd0b4a5fb6a4fb674c30828d5fe4a46d8fc
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 4. MÔĐUN PHẲNG VÀ CÁC HÀM TỬ "TOR"

Để thuận tiện cho những độc giả đã quen thuộc với Đại số đồng điều (*), chúng tôi sẽ chỉ ra vắn tắt lý thuyết môđun phẳng liên quan như thế nào với lý thuyết các hàm tử Tor.

#### Mệnh đề 1 {#ac-i-s4-prop-1 .statement}

Cho E là một A-môđun phải. Bốn tính chất sau là tương đương:

(a) E là phẳng.
(b) Với mọi A-môđun trái F và mọi số nguyên n $\geq 1$, $\mathrm{Tor}_n^A(E, F) = 0$.
(c) Với mọi A-môđun trái F, $\mathrm{Tor}_1^A(E, F) = 0$.
(d) Với mọi iđêan trái sinh hữu hạn $a$ của A,
$$
\mathrm{Tor}_1^A(E, A_s/a) = 0.
$$

Ta chứng minh rằng (a) kéo theo (b). Cho
$$
\cdots \to L_n \to L_{n-1} \to \cdots \to L_0 \to F \to 0
$$
là một phân giải tự do của F. Vì E là phẳng, dãy
$$
(1) \quad \cdots \to E \otimes L_n \to E \otimes L_{n-1} \to \cdots \to E \otimes L_0 \to E \otimes F \to 0
$$
là khớp. Vì các $\mathrm{Tor}_n^A(E, F)$ đẳng cấu với các nhóm đồng điều của phức (1), nên chúng bằng không với $n \geq 1$. Hiển nhiên là (b) kéo theo (c) và (c) kéo theo (d). Sau cùng ta chứng minh rằng (d) kéo theo (a). Dãy khớp
$$
0 \to a \to A, \to A_s/a \to 0
$$
suy ra dãy khớp
$$
\mathrm{Tor}_1^A(E, A_s/a) \to E \otimes_A a \to E \otimes_A A.
$$
Vì (d) được thỏa mãn, đồng cấu chính tắc
$$
E \otimes_A a \to E \otimes_A A = E
$$
là đơn ánh, điều đó có nghĩa là E là phẳng (§ 2, no. 3, Mệnh đề 1).

Mệnh đề 1 cung cấp một đặc trưng hóa của các môđun phẳng, điều thường hữu ích trong các ứng dụng. Như một ví dụ, chúng tôi sẽ chỉ giới hạn ở việc cho một

(*) Xem phần của bộ Chuyên luận này dành cho các phạm trù và đặc biệt là các phạm trù Abel (đang được chuẩn bị). Trong khi chờ phần đó được xuất bản, độc giả có thể tham khảo H. CARTAN-S. EILENBERG, Homological Algebra, Princeton, 1956, hoặc R. GODEMENT, Théorie des Faisceaux, Paris (Hermann), 1958.

$$
\operatorname{Tor}_1^A(E', F) \to \operatorname{Tor}_1^A(E, F) \to \operatorname{Tor}_1^A(E'', F)
$$

cho thấy rằng $\operatorname{Tor}_1^A(E, F) = 0$ với mọi A-môđun trái F, do đó E là phẳng. Nếu E và E'' là phẳng, dãy khớp

$$
\operatorname{Tor}_2^A(E'', F) \to \operatorname{Tor}_1^A(E', F) \to \operatorname{Tor}_1^A(E, F)
$$

cho thấy rằng $\operatorname{Tor}_1^A(E', F) = 0$, do đó E' là phẳng.

#### Mệnh đề 2 {#ac-i-s4-prop-2 .statement}

*Cho R, S là hai vành, $\rho : \mathbf{R} \to \mathbf{S}$ là một đồng cấu và F là một R-môđun trái. Hai tính chất sau là tương đương:*
(a) $\operatorname{Tor}_1^R(\rho_*(E), F) = 0$ với mọi S-môđun phải E.
(b) *S-môđun trái $\varphi^*(F) = F_{(S)} = S \otimes_R F$ là phẳng và $\operatorname{Tor}_1^R(\rho_*(S_d), F) = 0$.*

Giả sử rằng (a) được thỏa mãn. Lấy $E = S_d$, ta thấy rằng $\operatorname{Tor}_1^R(\rho_*(S_d), F) = 0$. Ta cũng chứng minh rằng $F_{(S)}$ là một S-môđun phẳng. Thật vậy, ta lưu ý rằng, nếu E là một S-môđun phải, nhóm cộng $E \otimes_S F_{,,}$ được đồng nhất với $\rho_*(E) \otimes_R F$. Khi đó nếu có một dãy khớp các S-môđun phải

$$
0 \to E' \to E \to E'' \to 0
$$

thì, dùng (a), ta thu được một dãy khớp

$$
0 \to \rho_*(E') \otimes_R F \to \rho_*(E) \otimes_R F \to \rho_*(E'') \otimes_R F \to 0
$$

hay cũng là

$$
0 \to E' \otimes_S F_{(S)} \to E \otimes_S F_{(S)} \to E'' \otimes_S F_{(S)} \to 0
$$

điều đó chứng minh rằng $F_{(S)}$ là phẳng.

Ngược lại, nếu (b) được thỏa mãn, trước hết ta có, với mọi S-môđun phải *tự do* $L = S_d^{(I)}$, $\operatorname{Tor}_1^R(\rho_*(L), F) = (\operatorname{Tor}_1^R(\rho_*(S_d), F))^{(I)} = 0$. Mọi S-môđun phải E đều có thể viết dưới dạng $E = L/H$ với một S-môđun tự do thích hợp L; khi đó ta có dãy khớp

(2) $0 = \operatorname{Tor}_1^R(\rho_*(L), F) \to \operatorname{Tor}_1^R(\rho_*(E), F) \to \rho_*(H) \otimes_R F \to \rho_*(L) \otimes_R F.$

Nhưng vì $F_{,,}$ là phẳng, đồng cấu $H \otimes_S F_{(S)} \to L \otimes_S F_{(S)}$ là đơn ánh và được đồng nhất với đồng cấu

$$
\rho_*(H) \otimes_R F \to \rho_*(L) \otimes_R F.
$$

Từ đó suy ra từ (2) rằng $\operatorname{Tor}_1^R(\rho_*(E), F) = 0$.

#### Nhận xét {#ac-i-s4-n0-rem-1 .statement}

Mệnh đề 2 cũng suy ra từ sự tồn tại của dãy khớp

$$
E \otimes_S \operatorname{Tor}_1^R(\rho_*(S_d), F) \to \operatorname{Tor}_1^R(\rho_*(E), F) \to \operatorname{Tor}_1^S(E, S_d \otimes_R F) \to 0
$$

phát sinh từ dãy phổ của "tính kết hợp" của các hàm tử Tor.

### Bài tập {#ac-i-s4-exercises}

Xem [bài tập của § 4](exercises/s4/).
