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
Showcase the silent revolution of text tokenizers

<!-- footer: DSFC 2022 • **Text Tokenizers for NLP** • Bauke Brenninkmeijer-->

---

## whois:`Bauke Brenninkmeijer`

- MSc in CS and Data Science @Nijmegen
- Data Scientist @ABNAMRO since 2019
    - 1.5 years in Data Management
    - ~1 years in Global Markets
- Co-founder of DSFC

- [![](/images/GitHub-Mark-32px.png)](https://github.com/Baukebrenninkmeijer) [@baukebrenninkmeijer](https://github.com/Baukebrenninkmeijer)


---

# Tokenization [1/2]
- Required for using text in any NLP techniques.
- Chops a text into smaller units called **`tokens`**.
- Tokens can represent many different things, such as
    - words
    - parts of words
    - characters.

---

# Tokenization [2/2]

- Form the building blocks of any NLP model
- Tokens are mapped to an ID
- Models ingest these IDs, since they can only use numeric values.


---

# Definitions

- **Corpus**: Dataset in NLP
- **Token**: Part of a text, used to segment a corpus
- **ID**: an index (i.e. a unique integer) that maps to a token.

---

# Types of tokenizer

- word-based
`'tokenizer'`
- character based
`'t', 'o', 'k', 'e', 'n', 'i', 'z', 'e', 'r'`
- subword-based
`'token', 'izer'`

---

# Character based tokenizer

- `Small vocabulary`. For ASCII, 256. With unicode, this is 1.1M characters.
- No out of vocabulary (OOV) words/characters.
- Lose a lot of meaninful information
- Models typically have `max input lengths`

```python
>>> list('Cat')
['C', 'a', 't']
```

---

# Character tokenizer in eastern languages
*Disclaimer: I don't speak chinese*

- Characters change meaning depending on surrounding characters
- Names can contain multiple characters

進口 means import, but word by word means “get into the mouth”

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