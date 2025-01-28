---
note_type: moc
tags:
  - web_development
mn: "[[10 MM]]"
---
[[10 MM]]

There is a muscle memory aspect to computer programming that can often be overlooked. This is not something that requires a lot of effort per se. It is something that happens naturally through repetition. You can learn with your fingers.

# How to create a project
```dataview 
TABLE WITHOUT ID link(file.name, short) AS "Note",  dateformat(file.ctime,"yyyy-MM-dd") AS "Creation date", question AS "Questions"
FROM "200 Neurons"
WHERE contains(file.name, "12") and contains(tags, "web_development")
FLATTEN substring(file.name, 2) AS short
SORT file.ctime ASC
```
# Resources


| Name - Link                                                                                                                                            | Description                                                                                                                                           | To-do |
| ------------------------------------------------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------- | ----- |
| [Why Learning to Code is So Damn Hard](https://web.archive.org/web/20230630111131/https://www.thinkful.com/blog/why-learning-to-code-is-so-damn-hard/) | Describe the four phases of the autonomous learning path in web development.                                                                          |       |
| [What makes a good developer?](https://jaredthenerd.com/2013/05/What-Makes-A-Good-Developer/)                                                          | Detail what is required to be a good junior, middle and senior web developer.                                                                         |       |
| [50 projects in 50 days to practices HTML, CSS, JS](https://github.com/bradtraversy/50projects50days)                                                  | 50 Projects in 50 Days - HTML/CSS and JavaScript                                                                                                      | X     |
| [Excerism](https://exercism.org)                                                                                                                       | Exercises and tutorials in multiple programming languages.                                                                                            |       |
| [100 days of css](https://100dayscss.com/about/)                                                                                                       | 100 mini projects to master css.                                                                                                                      |       |
| [Dev Docs](https://devdocs.io/)                                                                                                                        | Massive API documentation collection that even works offline of HTML, CSS, JS.                                                                        |       |
| [Learn HTML and more](https://web.dev/learn/html)                                                                                                      | Learn about HTMl and more                                                                                                                             |       |
| [Unlighthouse](https://unlighthouse.dev/)                                                                                                              | Unlighthouse is a tool to scan your entire site with Google Lighthouse in 2 minutes (on average). Open source, fully configurable with minimal setup. |       |
| [squoosh](https://squoosh.app/)                                                                                                                        | Optimize and provide tools for image optimization. Optimize one image at a time                                                                       |       |
| [imgto.xyz](https://imgto.xyz/)                                                                                                                        | Optimize several images at a time. It doesn't provide tools .                                                                                         |       |
| [pdfslicker](https://pdfslick.dev/)                                                                                                                    | To render pdf in a website.                                                                                                                           |       |
| [Guia entrevista programacion](https://github.com/DevCaress/guia-entrevistas-de-programacion?tab=readme-ov-file#buenas-practicas)                      |                                                                                                                                                       |       |
| [Web dev tools](https://www.hubdev.tools/)                                                                                                             | A collection of web dev tools of all sorts.                                                                                                           |       |
| [CrUX Vis](https://cruxvis.withgoogle.com/)                                                                                                            | See the  metric of any page based in real users                                                                                                       |       |

## Improving image loading with sprites
Instead of making multiple request for all images, create one sprite with all images, make a single request, and then use the back ground position css property to select the image. Visit: https://www.mcmaster.com/

![[Pasted image 20241217131256.png]]

# To do
- Lear about Vite and learn farm (https://www.farmfe.org/) that is even faster. This is to create projects. Both are applications packager, but farm is extrmely fast.  Learn aswell makojs. One of the major advantages of Farm is the retrocompatibility with vite, so all vite plugins work in farm. 
- Add girgraph extension to vscode.


- [This page](https://visualgo.net/en) shows algorithms visually. 
