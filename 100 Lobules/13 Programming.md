---
note_type: moc
tags:
  - programming
mn: "[[10 MM]]"
---
[[10 MM]]

# Table of content
```dataview 
TABLE WITHOUT ID link(file.name, short) AS "Note", question AS "Questions", overview
FROM "200 Neurons"
WHERE contains(file.name, "23") AND contains(note_type, "note")
FLATTEN substring(file.name, 3) AS short
SORT file.cday ASC
```


# Pending
```dataview 
TABLE file.ctime as "Created", checked AS "Status"
FROM "200 Neurons"
WHERE checked = "ongoing" AND contains(file.name, "23")
SORT file.ctime DESC
```

>[!quote] C sharp how to play
>The read a little, program a little model is far better at helping you learn fast.

