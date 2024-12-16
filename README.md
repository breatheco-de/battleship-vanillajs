<!--hide-->
# Acorazado en Vanilla.js
<!--endhide-->

Write a battleship game using Vanilla.js

![Demonstration of Battleship](https://github.com/breatheco-de/exercise-battleship-vanillajs/blob/master/preview.gif?raw=true)

<onlyfor saas="false" withBanner="false">
    
## 🌱  How to start this project

Do not clone this repository because we are going to be using a different template.

We recommend opening the `vanillajs-hello` template, using a provisioning tool like [Codespaces](https://4geeks.com/lesson/what-is-github-codespaces) (recommended) or [Gitpod](https://4geeks.com/lesson/how-to-use-gitpod). Alternatively, you can [clone the GitHub repository](https://4geeks.com/how-to/github-clone-repository) on your local computer using the `git clone` command.

This is the repository you need to open or clone:

```
https://github.com/4GeeksAcademy/vanillajs-hello
```

💡 Important: Remember to create a new repository, update the remote (`git remote set-url origin <your new url>`), and upload the code to your new repository using `add`, `commit` and `push`.

</onlyfor>

## 📝 Instructions

1. Create your HTML/CSS. First, we recomend using a parent div with `display:flex` and `flex-wrap: wrap` (to allow multiple rows), the container must have 100 divs inside.
2. After your HTML/CSS looks good, start thinking on how to make it dynamic using JS.
3. To represent the gameBoard you can use a JS matrix like this:

```js
// 0 = empty
// 1 = part of a ship
// 2 = a sunken part of a ship
// 3 = a missed shot
let gameBoard = [
    [1,1,1,1,1,0,0,0,0,1],
    [0,0,0,0,0,0,0,0,0,1],
    [0,0,0,0,0,0,0,0,0,1],
    [0,0,0,0,0,0,0,0,0,1],
    [0,0,0,0,0,0,0,0,0,0],
    [1,0,0,1,1,0,0,0,0,0],
    [1,0,0,0,0,0,0,0,0,0],
    [1,0,0,0,0,0,0,0,0,0],
    [0,0,0,0,0,0,0,0,0,0],
    [1,1,1,1,0,0,0,0,0,0]
];
```
4. Add one onClick to every `<div>` and call the `fireTorpedo` function with the coordinates of the div.
5. Replace the value on the gameBoard and render the board again.

## 😎 Feeling confident?

+ Try implementing a "showShips" function that shows the ship positions when clicked.
