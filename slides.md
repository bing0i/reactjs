
# <uil-react class="text-blue-400" /> ReactJS
A summarized version of new React Docs\
by Tuyen Phan

<!-- Feel free to interrupt me. This presentation is mostly about how React works in new React docs... -->

---
layout: two-cols
---

<uil-html5 class="text-red-400" /> index.html

```html
<!DOCTYPE html>
<html>
 <head>
  <link rel="stylesheet" href="style.css">
 </head>
 <body>
    <button id="hwButton" onclick="changeButtonColor()">
      Hello World
    </button>
    <script src="script.js"></script>
 </body>
</html>
```

<uil-css3-simple class="text-blue-400" /> style.css

```css
button {
  background-color: blue;
}
```

<uil-java-script class="text-yellow-400" /> script.js

```js
const changeButtonColor = () => {
  const hwButton = document.getElementById("hwButton");
  hwButton.style.background = 'red';
}
```

::right::
<div class="ml-6">

  <uil-react class="text-blue-400" /> HelloWorld.jsx
  ```jsx
  import React, { useState } from 'react';

  const HelloWorld = () => {
    const [color, setColor] = useState('blue');
    const changeButtonColor = () => {
      setColor('red');
    };

    return (
      <button 
        style={{backgroundColor: color}}
        onClick={changeButtonColor}>
        Hello World
      </button>
    );
  };

  export default HelloWorld;
  ```

</div>

<!--
<script> tag can be placed in <head> or <body> tags, or in both. Mention that it is recommended to place it in the <body> tag, as it will then be executed after the page has been loaded. Mention async and defer attributes. Why <script> tag is placed at <head> or <body>?

Of course, ReactJS also has some default files such as index.html, index.js or even App.jsx which I will shortly show you in later slides. But we rarely touch those files after the initial setup. Usually, we only need to create new components such as this HelloWorld.jsx and import them into the suitable component.

We are not here to compare the length but I want to emphasize the logic is tightly coupled with the user interface.
-->

---
layout: two-cols
---

# Installation with CRA
- Install [Node.js](https://nodejs.org/en/)
- Use [Create React App](https://create-react-app.dev/)
```bash
npx create-react-app my-app 
```

- Run the app
```bash
cd my-app
npm start
```

::right::
<div class="ml-6">

# Other Toolchains
- Vite
- Parcel
# Frameworks
- Next.js
- Gatsby
- Remix
- Razzle
</div>

<!-- We can use React instantly by ... -->

---

# React Templates

---

# Ideal of React
