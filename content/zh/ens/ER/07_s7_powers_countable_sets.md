---
book: ens
book_title: Theory of Sets
chapter: ER
chapter_title: SUMMARY OF RESULTS
section: 7
section_title: Powers. Countable sets
lang: zh
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 380-382
pdf_pages: 0385-0387
extraction: ocr
statements: 0
exercises: 0
content_sha256: 5f166744bf5d13415b032c547da97a870eafb1208bb927c0e3fddbeeb258e98c
translated_from: content/en/ens/ER/07_s7_powers_countable_sets.md
translation_method: google
source_content_sha256: 86ddec08acce4507f77a4f26c22ecf7fe435bb7014433e7736350957d8534e86
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: d6a60f7c627fe9edcdb2a88ae9b785041bf55079525e855f385f74565b63affd
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## 7. 幂。 可数集

1. 如果两个集合 E、F 可以一对一地放在对应中，则称它们“等价”。
两个集合，每个等价于第三个，它们本身也是等价的。
如果 E 和 F 等价，则 $\mathfrak{P}(E)$ 和 $\mathfrak{P}(F)$ 等价。
如果E和F、E'和F'、E"和F"分别等价，则$E\times E'\times E''$和$F\times F'\times F''$等价。 集合中任意数的命题扩展至乘积。

2. 令X和Y为集合E的两个泛型子集。关系“X和Y等价”是$\mathfrak{P}(E)$上的*等价关系*。 等价类（相对于这个关系），X属于被称为X的*幂*[^1]，以及这些类的集合（即商 $\mathfrak{P}(E)$被上面的关系)称为E的子集的幂**集合。
如果E和F是两个不同的集合，关系，E的子集X和F的子集Y之间“X和Y等价”可以用说表示，X的幂和Y的幂是*等效*。这样我们就在E的子集幂集合子集和F的子集幂集合子集之间有了一一对应的对应。

3. 令 E、F 为任意两个集合，它们可能不同，也可能不同，并令 $\mathfrak{a}$（分别为 $\mathfrak{b}$）为 E（分别为 F）的子集的幂集合的元素。 然后，如果存在子集 $X\subset E$ 与幂 $\mathfrak{a}$ 到子集的一对一映射，则称$\mathfrak{a}$ *小于* $\mathfrak{b}$，或 $\mathfrak{b}$ *大于* $\mathfrak{a}$ $Y\subset F$ 与幂 $\mathfrak{b}$。 如果$\mathfrak{a}$和$\mathfrak{b}$也不等于幂，则$\mathfrak{a}$被称为*严格小于*$\mathfrak{b}$，或$\mathfrak{b}$*严格大于*$\mathfrak{a}$。

如果 $\mathfrak{a}$ 和 $\mathfrak{b}$ 相等，则 $\mathfrak{a}$ 既大于又小于 $\mathfrak{b}$。

相反，定理*如果$\mathfrak{a}$既大于又小于$\mathfrak{b}$，则$\mathfrak{a}$和$\mathfrak{b}$等价。*特别是，集合E的子集、幂的集合*排序*为关系“$\mathfrak{a}$小于$\mathfrak{b}$”；每当我们将这个集合称为有序的集合时，我们所指的始终是这个关系定义的顺序。

此外，使用 Zorn 的引理（以及选择公理），可以证明集合 of 幂 of 子集 of 集合 E 是良序的。*

4. 集合 E 的幂 *严格小于* 集合 $\mathfrak{P}(E)$。

如果$f$是集合E的映射到集合F，那么E的任何子集X的像$f(X)$的幂*小于*X的幂。

5. 令$(X_i)_{i\in I}$是集合E的子集族，使得每当$i\ne k$时就有$X_i\cap X_k=\varnothing$。 令 $(Y_i)_{i\in I}$ 为集合 F 的子集族，由同一集合 I 索引，并且对于所有 $i\in I$，$Y_i$ 的幂*小于*$X_i$ 的幂。 那么对于 I 的所有子集 J，并集 $\bigcup_{i\in J}Y_i$ 的幂*小于*$\bigcup_{i\in J}X_i$ 的幂。

如果只要 $i\ne k$ 也有 $Y_i\cap Y_k=\varnothing$，并且如果 $X_i$ 和 $Y_i$ 对于所有 $i\in I$ 都是“等价”，那么 $\bigcup_{i\in J}X_i$ 与 $\bigcup_{i\in J}Y_i$ 都是“等价”。

特别是，如果 F 和 E 是同一集合，我们会看到 E 的一组“成对不相交”子集的并集的幂仅取决于这些子集的幂；它被称为这些幂的*和*（因此，仅当存在 E 的成对不相交子集的族 $(X_i)$ 且使得 $X_i$ 对于每个索引 $i$ 具有幂 $\mathfrak{a}_i$ 时，才为幂集的元素族 $(\mathfrak{a}_i)$ 定义此函数）。

如果$(X_i)_{i\in I}$和$(Y_i)_{i\in I}$分别是E和F的子集族，由相同的集合I索引，使得$X_i$和$Y_i$对于所有$i$“等价”，则乘积$\prod_i X_i$和$\prod_i Y_i$ *等价*。

6. 自然整数的集合 $\mathbf{N}$ 可以被视为*无限* 集合的*有限* 子集的幂的集合。 $\mathbf{N}$上的序关系“$x\leq y$”就是关系点幂的这个集合，两个自然整数的*和*函数与两个幂的和相同，如上面定义的。

7. 如果集合等于集合$\mathbf{N}$或自然整数的子集，则称集合是“可数”。 *因此，每个有限的集合* 都是可数的；如果它有 $n$ 元素，则相当于集合 $\mathbf{N}$ 的区间 $[0,n-1]$。每个

## 结果总结

*可数无穷* 集合等价于 $\mathbf{N}$；特别是，$\mathbf{N}$的每个无限子集都具有与$\mathbf{N}$相同的幂。

如果$E$是*无限*集合，则在*可数无限*集合中存在$E$的*划分*；特别是，每个无限集合都有幂*大于*$\mathbf{N}$。

如果$E$是*无限*集合，集合$E \times E$和$E \times \mathbf{N}$都*等价于$E$，并且$E$的*有限子集*的集合*等价于* $E$。特别是，$\mathbf{N} \times \mathbf{N}$是一个*可数无穷*集合。

8. 集合 $E$ 的元素* 的 *序列由定义 $E$ 的元素组成，索引为集合 $\mathbf{N}$ 或子集 $\mathbf{N}$。因此，序列的指标集合是$\mathbf{N}$，因此写为$(x_n)_{n\in\mathbf{N}}$，或更简单地写为$(x_n)$，以免混淆。如果$n$表示泛型整数，则$x_n$被称为序列的*泛型项*，或*n个项*。当 $n$ 被特定的整数替换时，也会使用后者术语。 序列元素集合是可数的。

序列被称为“无限”或“有限”，因为指标集合是$\mathbf{N}$ 的无限或有限子集。 有限序列元素集合是有限的。

序列的每个子族又是序列，称为给定序列的*子序列*。 有限序列的每个子序列都是有限序列。

元素的族，其指标集合为$\mathbf{N} \times \mathbf{N}$，或子集为$\mathbf{N} \times \mathbf{N}$，称为*双序列*。由 $\mathbf{N} \times \mathbf{N}$ 索引的双序列写作 $(x_{m,n})$，或更简单地写为 $(x_{mn})$（如果不存在混淆的风险）。对于具有两个以上指标的序列也是如此。

如果存在指标集合的置换 $f$，则两个序列 $(x_n)$、$(y_n)$ *仅在其项的序上有所不同*，使得所有$y_n=x_{f(n)}$ 都存在$n$。

对于任何元素$(x_\iota)_{\iota\in I}$族，其指标集合$I$可数无穷，我们可以关联一个无限序列，如下：存在$\mathbf{N}$的双射$n\to f(n)$到$I$；将$y_n=x_{f(n)}$，序列$(y_n)$据说是通过*将家庭*$(x_\iota)$放入$f$定义的*序中获得的。因此，序列相应的到$\mathbf{N}$的两个不同的双射到$I$的不同之处仅在于它们的项的序。

当$I$是*有限*时以同样的方式操作，我们得到与族$(x_\iota)$相关联的*有限序列*。

9. 如果$I$是*可数*集合，则集合$E$的子集族$(X_\iota)_{\iota\in I}$的并、交和乘积被称为*可数*，如果$I$是有限的，则称*有限*。

如果$I$是*可数的*，并且如果$X_\iota$的幂*小于*所有$\iota\in I$的给定无限幂$\alpha$，则并$\bigcup_\iota X_\iota$的幂*小于*$\alpha$。如果$X_\iota$中至少有一个具有幂$\alpha$，则$\bigcup_\iota X_\iota$具有幂$\alpha$。特别地，幂$\alpha$的集合的每个可数并还有幂$\alpha$； 可数集中的每个可数并都是可数集合。

[^1]: 在形式化的集合理论（cf.章III, § 3）中，我们将集合的*基数*的定义概念，我们也将其称为（滥用语言）集合的*幂*。 然而，这种语言滥用不会造成任何混乱，因为集合中的两个子集具有相同的幂（在上面定义的意义上）当且仅当它们具有相同的基数；同样，集合 E 的子集 A 的幂小于集合 F (no. 3) 的子集 B 幂，当且仅当 A 的基数小于 B 的基数；最后，如果A的幂是E的子集的$(A_\iota)$的幂的和（no. 5），则A的基数是$A_\iota$的基数的和。
