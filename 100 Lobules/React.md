## Use vite to build up application
Vite is builder used for different frameworks, this one incorporates typescript with react.  
Execute this command: `npm create vite@latest`
Then put a project name
after that run `npm install`
Then open the application folder

To execute the application execute: `npm run dev`

## How to create components and include in index
Components should be created within the folder src, under a directory call 'components'

At the end of every component file I have to export it with `export default <component name>;`

Exporting components make them available in the main app of tsx

The 'index' file of my project is App.tsx 

To add a component to the index website use its name as a tag in the App.tsx

![[Pasted image 20240603191448.png]]

## How to style components
I have to execute `npm install styled-components`

At the top of the component `import styled from "styled-components"` this has to be done for every component file. 

Then, I have to create a variable, that will be a component itself, that can be used anywhere. 
Now, within the '' is where the styling goes with classic CSS.

```typescript
import styled from 'styled-components'
const Button = styled.button` 
background: transparent;
  border-radius: 3px;
  border: 2px solid #BF4F74;
  color: #BF4F74;
  margin: 0 1em;
  padding: 0.25em 1em;
  `;
```

>The name of the style component should match the name of the tags used in the return statement of the component body.

```tsx
function MyButton() {
    return (
      <StyledButton>I'm a button</StyledButton>
    );
  }
```

To add 'states' to a component I have to import `{css}` and then interpolate a function ('embed' a function into the template literal). In this example, when the $primary property is set we want to add some more css to our component, in this case change the background and color. And to set properties I can add them as 'attributes' in the index of the application.

>Detail the question mark after the variable primary, this makes this argument optional. 

>Also detail the props here is an arrow function. When I need to write multiple properties is recommended this formatting; if not, use the one below as an inline. 

```typescript
import styled, { css } from 'styled-components'


const StyledButton = styled.button<{ $primary?: boolean; }>`
  background: transparent;
  border-radius: 3px;
  border: 2px solid #BF4F74;
  color: '#BF4F74';
  margin: 0 1em;
  padding: 0.25em 1em;


  ${props =>
    props.$primary &&
    css`
      background: '#BF4F74';
      color: white;
    `};
`

function MyButton() {
    return (
      <StyledButton>I'm a button</StyledButton>
    );
  }
// - - - - - - - - - - - - - - - - - - - - - - - 

// In the index page
<MyButton>Normal Button</MyButton>
<MyButton $primary>Primary Button</MyButton>
```

![[Pasted image 20240603172709.png|center]]

### Another way to style components
To control 'manually' the components I can set ternary operators to all css properties of my interest and then, set the state of the component within the return statement. In this case, the disabled parameter is not optional, this I have to included in the return statement. But this is not a good practice. (This is how kevin does it)

![[Pasted image 20240603172924.png]]
![[Pasted image 20240603182856.png]]Because the state is set to disable, the button looks like this. 
So here is showing this property as optional, thus, I don't have to include disabled=true in the return. 

![[Pasted image 20240603215021.png]]

## How to import
To import components to the app.tsx I have to import every component from a file 8so I can have multiple components in one file) to the main script. For example if my component file is called `MyButton.tsx` and the component is called Button, the import will be `import Button from './components/MyButton'` and the tag will be `<Button></Button>`
# Storybook

Run `npx storybook@latest init`