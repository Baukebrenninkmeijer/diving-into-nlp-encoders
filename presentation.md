---
marp: true
theme: uncover
---

<!-- _class: invert lead -->

![bg](images/title-background.png)

# Text tokenizers for NLP

Bauke Brenninkmeijer

<!-- footer: DSFC 2022 -->

---

# Goal
Highlight the silent revolution of text tokenizers

<!-- footer: DSFC 2022 • **Text Tokenizers for NLP** • Bauke Brenninkmeijer-->

---

# whois: Bauke Brenninkmeijer

- Masters in CS and Data Science @Nijmegen
- @ABNAMRO since 2019

---

# Types of tokenizer

- character based
- word-based
- subword-based

---

# Character based tokenizer

- Character
- Vocabulary is only as large as the number of characters.
- For ASCII, 256. With unicode, this is 1.1M characters.
- Lose a lot of contextual information
- Models typically have `max input lengths`.

```python
>>> list('Cat')
['C', 'a', 't']
```

---

# Where it all started

![bg right](images/middle-ages.png)

- Word2Vec
- Glove

---
A note on this method, to use it with markdown you need to use code like this
<section class="hbox">	<div class="container"> <div class="flex-col" data-markdown> * Column 1 Content </div> <div class="flex-col" data-markdown> * Column 2 Content </div> </div> </section>

---
# Slide 2

- Footnote link only <sup>1<sup>.
- Footnote and superscript link <sup>[1][1]</sup>.

[1]: https://www.google.com