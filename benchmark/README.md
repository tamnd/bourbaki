# benchmark

Answers that a person has already ruled on, put in front of the judges to find out what a verdict in this corpus is worth.

The pipeline decides for itself whether a solution is right, so every `verified` under `content/solutions` is the judges marking their own work. The only way to put a number on that is to hand them answers whose worth was settled beforehand, some right and some wrong on purpose, and count how often they agree. That is what `bourbaki solve eval` does, and this directory is the answers it reads.

One directory to the language, one file to the case, named `<label>.<variant>.md`. The variant `as-solved` is what the pipeline wrote and a person then read. The other variants are written by hand, and the ones that are wrong say in their name what is wrong with them: `one-direction-only` proves one implication and declares the equivalence, `substitution-dropped` loses a substitution and then claims a theorem of one theory as a theorem of another, and so on. Each of those carries a single deliberate fault in an argument that is otherwise complete, because a stub is not a test of anything.

This sits beside `content/` rather than inside it for a plain reason. `content/` is Bourbaki, the audit walks it, and the tags and the translations follow it. An answer that is wrong on purpose has no business being read as part of the book.

The verdicts themselves, the labels and one line of reasoning each, live with the code in `tamnd/bourbaki-solver` under `benchmark/set.json`. Nothing of Bourbaki is in that file. The text is here, where text belongs.
