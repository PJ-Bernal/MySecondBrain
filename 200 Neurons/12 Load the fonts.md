---
note_type: note
tags:
  - web_development
mn: "[[12 Web Dev]]"
kt: theorical
checked: false
---
[[12 Web Dev]]

Having a public directory, create another called fonts. The fonts are plain .woff2 files. The example use space grotesk. 

Then, go to the main landing page and import the fonts. This is inside of the main html file. I have to create a font face at rule for every font the project will be using. 

![[Pasted image 20240917131022.png|center|450]]


After importing, test the bold. If it doesn't look good, I can indicate `font-weight: 100 900;` a range so the browser apply a better boldness. 

>[!important]
>I can import bold, light, black, etc. fonts of a same font. In this case, when extend that in tailwind, I will extend all of this imports.
>
>>[!multi-column]
>>
>>![[Pasted image 20240917133203.png|400]]
>>
>For example, the at rule is importing the bold and black trois mille fonts. Thus, when I extend in tailwind, I extend both. So, if I code `<strong class="font-trois font-black`, tailwind know it hae to pick the trois and black font.
>>![[Pasted image 20240917133617.png]]


## When importing bold fonts
I have to provide a specific font-weight value, not a range.

## Extend the font in tailwind
Inside of tailwind.config extend a font that won't be the main font. When a font is use in specific cases, extend it allow to tell tailwind I can call that font in its classes like `<strong class="font-trois">Test</strong>`. 

![[Pasted image 20240917132913.png|center|400]]

