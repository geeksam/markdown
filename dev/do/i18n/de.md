---
title: Verwende Übersetzungschlüssel, nicht Text
---

Fügen Sie keine Texte in Ihre Schnittmuster ein. Stattdessen fügen Sie bitte einen Schlüssel ein, der übersetzt werden kann.

For example, if you want to put *Finish with bias tape* on your pattern, don't be tempted to do this:

```js
path.seam.attr("data-text", "Finish with bias tape");
```

That (English) string is now hard-coded in your pattern. As freesewing supports translation out of the box, it would be a real shame not to make use of it.

Instead, insert a key to identify the string:

```js
path.seam.attr("data-text", "finishWithBiasTape");
```

This way, it can be translated.