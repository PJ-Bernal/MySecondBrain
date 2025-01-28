---
note_type: note
tags:
  - web_development
mn: "[[12 Web Dev]]"
kt: theorical
checked: false
---
[[12 Web Dev]]

To avoid having relative imports (using . and ..), modify the confi file like this, thus, each `@` import will be mapped to a specific path.

![[Pasted image 20240917130436.png|center|500]]

Thus, in the index of each webpage the imports will look like this:

![[Pasted image 20240917130517.png|center|400]]

This is useful when having deep routing, I donot have to do ./../. etc..
