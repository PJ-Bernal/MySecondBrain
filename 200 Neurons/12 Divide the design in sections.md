---
note_type: note
tags:
  - web_development
mn: "[[12 Web Dev]]"
kt: theorical
checked: false
---
[[12 Web Dev]]

Divide each webpage in sections, for example, the following is the division of the index webpage: hero image, info, projects, personal, contact, footer, etc.
>[!blank-container|float-left]
>![[Pasted image 20240917125159.png|center|200]]


![[Pasted image 20240917125236.png]]

This image is from Astro, but the logic is the same, I create sections. 

Each webpage should have an file within a directory called pages. 

>[!blank-container|float-right]
![[Pasted image 20240917125832.png|200]]

Thus I can import each component (each section) into that specific webpage. In this case, I already have the sections in components, so I have to import them inside of index.astro.


![[Pasted image 20240917130002.png]]

## Folder structure
Within the public directory I can create a videos  directory, fonts directory. 

Then, inside src directory:
- components: my sections can have components, for example a header is not a section but a component, for example, with a logo, so I can have the logo and the component. And inside of the logo is only the svg, and inside of header is all the header component.

![[Pasted image 20240917135108.png|center|450]]

And then, inside of the component I need to import the assets, in this case, the logo.

![[Pasted image 20240917135329.png|center|400]]
