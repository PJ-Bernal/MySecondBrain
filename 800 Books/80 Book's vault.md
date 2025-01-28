---
note_type: moc
tags:
  - books
mn: "[[10 MM]]"
total_page: 10
---
[[10 MM]]

# Programming
```dataview 
Table author as Author, ("![|100](" + coverUrl + ")") as Cover, total_page AS "Pages", status AS "Status", start_date, end_date
From "800 Books"
WHERE contains(note_type, "book_note") AND contains(topic, "programming")
```

# Psychology
```dataview 
Table author as Author, ("![|100](" + coverUrl + ")") as Cover, total_page AS "pages", status
From "800 Books"
WHERE contains(note_type, "book_note") AND contains(topic, "psychology")
```

```tracker
searchType: dvField
folder: 300 Journal
searchTarget: linux, js, top
datasetName: How linux works, JS, TOP
line:
	title: Book tracker
	yMax: 10
	yMin: 0
	lineColor: white, gray, yellow
	showLegend: true
	fillGap: true
```
```tracker
searchType: dvField
folder: 300 Journal
searchTarget: linux, js, top
datasetName: How linux works, JS, TOP
summary:
	template: "Streaks\nLongest Streak: {{maxStreak()}} day(s)\tLongest Breaks: {{maxBreaks()}} day(s)\tLast streak: {{currentStreak()}} day(s)"
```

```tracker
searchType: dvField
folder: 300 Journal
searchTarget: linux, js, top
datasetName: How linux works, JS, TOP
summary:
	template: "AVERAGES\nlinux: {{average(dataset(0))}}\tjs: {{average(dataset(1))}}\ttop:{{average(dataset(2))}}\n"
```

