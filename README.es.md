<!--hide-->
# Battleship In Vanilla.js
<!--endhide-->

Crea una batalla naval usando Vanilla.js

![Demonstration of Battleship](https://github.com/breatheco-de/exercise-battleship-vanillajs/blob/master/preview.gif?raw=true)

<onlyfor saas="false" withBanner="false">
 
## 🌱  Cómo iniciar este proyecto

No clones este repositorio porque usaremos una plantilla diferente.  

Recomendamos abrir la plantilla `vanillajs-hello`, utilizando una herramienta de aprovisionamiento como [Codespaces](https://4geeks.com/lesson/what-is-github-codespaces) (recomendado) o [Gitpod](https://4geeks.com/lesson/how-to-use-gitpod). Alternativamente, puedes [clonar el repositorio de GitHub](https://4geeks.com/how-to/github-clone-repository) en tu computadora local utilizando el comando `git clone`.  

Este es el repositorio que necesitas abrir o clonar:  

```
https://github.com/4GeeksAcademy/vanillajs-hello  
```  

💡 Importante: Recuerda crear un nuevo repositorio, actualizar el remoto (`git remote set-url origin <tu nueva url>`), y subir el código a tu nuevo repositorio utilizando `add`, `commit` y `push`.  

</onlyfor>

## 📝 Instrucciones

1. Crea tu HTML / CSS. Primero, te recomendamos usar un div padre con `display: flex` y` flex-wrap: wrap` (para permitir múltiples filas), el contenedor debe tener 100 divs adentro.
2. Una vez que tu HTML / CSS se vea bien, comienza a pensar en cómo hacerlo dinámico usando JS.
3. Para representar el tablero de juego, puedes usar una array o arreglo JS como este:

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

4. Agrega un onClick a cada `<div>` y llama a la función `fireTorpedo` con las coordenadas del div.
5. Reemplaza el valor en el tablero y muestra (render) el tablero nuevamente.

## 😎 ¿Te sientes seguro?

+ Intenta implementar una función "showShips" que muestre las posiciones del barco cuando se hace clic.
