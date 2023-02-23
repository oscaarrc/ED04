# **ED04 - *botón submit con animación***


## **Descripción**

>**Este código consiste en crear una animación para un botón (en este caso es un botón submit) con CSS y javascript. Tan solo es una demostración de la animación, para su correcta implementación en una página web, el código debe ser modificado.**


## **Highlights**

### HTML
```htmlembedded
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ed04</title>
    <link rel="stylesheet" href="index.css">
    <link rel="stylesheet" href="index.js">
</head>
<body>

    <div class="container">
    <div class="bottom"></div>
    <div class="cover cut"></div>
    <div class="text-container">
        <div class="text text-dark">SUBMIT</div>
    </div>
    <div class="text-container cut">
        <div class="text">SUBMIT</div>
    </div>
    <div class="overlay"></div>
    </div>

</body>
</html>
```

### CSS

```css
@import url("https://fonts.googleapis.com/css2?family=Questrial&display=swap");
body {
  align-items: center;
  display: flex;
  font-family: "Questrial";
  font-weight: 800;
  justify-content: center;
  height: 100vh;
  background-color: black;
}

.container {
  align-items: center;
  border-radius: 26px;
  box-shadow: 0 1px 1px rgba(0, 0, 0, 0.11), 0 2px 2px rgba(0, 0, 0, 0.11),
    0 4px 4px rgba(0, 0, 0, 0.11), 0 6px 8px rgba(0, 0, 0, 0.11),
    0 8px 16px rgba(0, 0, 0, 0.11);
  cursor: pointer;
  display: flex;
  justify-content: center;
  position: relative;
  height: 52px;
  width: 190px;
}

.bottom {
  border-radius: 26px;
  background: #fff01a;
  height: 100%;
  overflow: hidden;
  position: absolute;
  width: 100%;
}

.cover {
  background-color: #c845f0;
  border-radius: 26px;
  height: 100%;
  position: absolute;
  width: 100%;
}
.cut {
  clip-path: polygon(
    100% 0%,
    99.73714% -0.13875%,
    98.96737% -0.53964%,
    97.71887% -1.17957%,
    96.01985% -2.03547%,
    93.89849% -3.08428%,
    91.38299% -4.30291%,
    88.50154% -5.66829%,
    85.28234% -7.15734%,
    81.75358% -8.74699%,
    77.94346% -10.41416%,
    73.88016% -12.13578%,
    69.59189% -13.88876%,
    65.10683% -15.65005%,
    60.45319% -17.39655%,
    55.65915% -19.10519%,
    50.75291% -20.75291%,
    45.76266% -22.31661%,
    40.7166% -23.77324%,
    35.64292% -25.09971%,
    30.56981% -26.27294%,
    25.52548% -27.26986%,
    20.5381% -28.0674%,
    15.63589% -28.64248%,
    10.84702% -28.97202%,
    6.1997% -29.03295%,
    1.72212% -28.8022%,
    -2.55753% -28.25668%,
    -6.61106% -27.37332%,
    -10.41026% -26.12905%,
    -13.92694% -24.50079%,
    -17.13292% -22.46546%,
    -20% -20%,
    -22.46546% -17.13292%,
    -24.50079% -13.92694%,
    -26.12905% -10.41026%,
    -27.37332% -6.61106%,
    -28.25668% -2.55753%,
    -28.8022% 1.72212%,
    -29.03295% 6.1997%,
    -28.97202% 10.84702%,
    -28.64248% 15.63589%,
    -28.0674% 20.5381%,
    -27.26986% 25.52548%,
    -26.27294% 30.56981%,
    -25.09971% 35.64292%,
    -23.77324% 40.7166%,
    -22.31661% 45.76266%,
    -20.75291% 50.75291%,
    -19.10519% 55.65915%,
    -17.39655% 60.45319%,
    -15.65005% 65.10683%,
    -13.88876% 69.59189%,
    -12.13578% 73.88016%,
    -10.41416% 77.94346%,
    -8.74699% 81.75358%,
    -7.15734% 85.28234%,
    -5.66829% 88.50154%,
    -4.30291% 91.38299%,
    -3.08428% 93.89849%,
    -2.03547% 96.01985%,
    -1.17957% 97.71887%,
    -0.53964% 98.96737%,
    -0.13875% 99.73714%,
    0% 100%,
    100% 100%
  );
  transition: clip-path 500ms;
}
.container:hover .cut {
  clip-path: polygon(
    100% 0%,
    100.00018% 0.14326%,
    99.99754% 0.56399%,
    99.98732% 1.24864%,
    99.96476% 2.18368%,
    99.92511% 3.35553%,
    99.8636% 4.75066%,
    99.77547% 6.35551%,
    99.65597% 8.15653%,
    99.50033% 10.14017%,
    99.3038% 12.29288%,
    99.06161% 14.60111%,
    98.76901% 17.0513%,
    98.42123% 19.62992%,
    98.01352% 22.3234%,
    97.54112% 25.11819%,
    96.99926% 28.00074%,
    96.38318% 30.95751%,
    95.68814% 33.97494%,
    94.90936% 37.03949%,
    94.0421% 40.13759%,
    93.08158% 43.2557%,
    92.02305% 46.38027%,
    90.86174% 49.49775%,
    89.59291% 52.59459%,
    88.21179% 55.65723%,
    86.71362% 58.67212%,
    85.09364% 61.62572%,
    83.34709% 64.50448%,
    81.46921% 67.29483%,
    79.45524% 69.98324%,
    77.30042% 72.55614%,
    75% 75%,
    72.55614% 77.30042%,
    69.98324% 79.45524%,
    67.29483% 81.46921%,
    64.50448% 83.34709%,
    61.62572% 85.09364%,
    58.67212% 86.71362%,
    55.65723% 88.21179%,
    52.59459% 89.59291%,
    49.49775% 90.86174%,
    46.38027% 92.02305%,
    43.2557% 93.08158%,
    40.13759% 94.0421%,
    37.03949% 94.90936%,
    33.97494% 95.68814%,
    30.95751% 96.38318%,
    28.00074% 96.99926%,
    25.11819% 97.54112%,
    22.3234% 98.01352%,
    19.62992% 98.42123%,
    17.0513% 98.76901%,
    14.60111% 99.06161%,
    12.29288% 99.3038%,
    10.14017% 99.50033%,
    8.15653% 99.65597%,
    6.35551% 99.77547%,
    4.75066% 99.8636%,
    3.35553% 99.92511%,
    2.18368% 99.96476%,
    1.24864% 99.98732%,
    0.56399% 99.99754%,
    0.14326% 100.00018%,
    0% 100%,
    100% 100%
  );
}
.container:active .cut {
  clip-path: polygon(
    127.29527% 25.2734%,
    127.29545% 25.41665%,
    127.2928% 25.83738%,
    127.28259% 26.52204%,
    127.26003% 27.45707%,
    127.22038% 28.62893%,
    127.15887% 30.02405%,
    127.07074% 31.6289%,
    126.95124% 33.42992%,
    126.7956% 35.41357%,
    126.59907% 37.56628%,
    126.35688% 39.8745%,
    126.06428% 42.3247%,
    125.7165% 44.90331%,
    125.30879% 47.59679%,
    124.83638% 50.39158%,
    124.29452% 53.27414%,
    123.67845% 56.23091%,
    122.98341% 59.24834%,
    122.20463% 62.31288%,
    121.33736% 65.41099%,
    120.37685% 68.5291%,
    119.31831% 71.65367%,
    118.15701% 74.77115%,
    116.88818% 77.86798%,
    115.50706% 80.93062%,
    114.00889% 83.94552%,
    112.3889% 86.89912%,
    110.64235% 89.77787%,
    108.76447% 92.56823%,
    106.75051% 95.25663%,
    104.59569% 97.82954%,
    102.29527% 100.2734%,
    99.85141% 102.57382%,
    97.2785% 104.72864%,
    94.5901% 106.7426%,
    91.79974% 108.62048%,
    88.92099% 110.36703%,
    85.96739% 111.98702%,
    82.9525% 113.48519%,
    79.88985% 114.86631%,
    76.79302% 116.13514%,
    73.67554% 117.29644%,
    70.55097% 118.35497%,
    67.43286% 119.31549%,
    64.33476% 120.18276%,
    61.27021% 120.96154%,
    58.25278% 121.65658%,
    55.29601% 122.27265%,
    52.41345% 122.81451%,
    49.61866% 123.28692%,
    46.92518% 123.69463%,
    44.34657% 124.0424%,
    41.89638% 124.33501%,
    39.58815% 124.5772%,
    37.43544% 124.77373%,
    35.4518% 124.92937%,
    33.65078% 125.04887%,
    32.04593% 125.137%,
    30.6508% 125.19851%,
    29.47894% 125.23816%,
    28.54391% 125.26071%,
    27.85926% 125.27093%,
    27.43852% 125.27358%,
    27.29527% 125.2734%,
    127.29527% 125.2734%
  );
}
.dot {
  position: absolute;
  /*draw particles as circles:*/
  border-radius: 50%;
  background-color: #eaf828;
}
.text-container {
  align-items: center;
  display: flex;
  height: 100%;
  justify-content: center;
  position: absolute;
  width: 100%;
}
.text {
  color: #fcff56;
  font-size: 22px;
  position: absolute;
}
.text-dark {
  color: #b500ec;
}
.overlay {
  height: 100%;
  position: absolute;
  width: 100%;
}
```

### JS

```javascript
const bottom = document.querySelector(".bottom");
const overlay = document.querySelector(".overlay");
const count = 110;
const size = 50;
for (let i = 0; i <= count; i += 1) {
  const dot = document.createElement("div");
  dot.classList.add("dot");
  bottom.appendChild(dot);
}
const dots = Array.from(document.querySelectorAll(".dot"));

const updateText = (text) => {
  Array.from(document.querySelectorAll(".text")).forEach(
    (e) => (e.innerHTML = text)
  );
};

const reset = () => {
  dots.forEach((dot, i) => {
    const x = (i / count) * (190 + size) - size / 2;
    const y = Math.random(1) * 52 - size / 2;
    dot.style.width = `${size}px`;
    dot.style.height = `${size}px`;
    dot.style.left = `${x}px`;
    dot.style.top = `${y}px`;
    dot.style.opacity = 1;
    dot.style.transform = "scale(1)";
  });
};
reset();

overlay.addEventListener("click", () => {
  anime({
    easing: "linear",
    targets: document.querySelectorAll(".dot"),
    opacity: [{ value: 0, duration: 600, delay: anime.stagger(10) }],
    translateX: {
      value: function () {
        return anime.random(-30, 30);
      },
      duration: 400,
      delay: anime.stagger(10)
    },
    translateY: {
      value: function () {
        return anime.random(-30, 30);
      },
      duration: 400,
      delay: anime.stagger(10)
    },
    scale: {
      value: function () {
        return 0;
      },
      duration: 400,
      delay: anime.stagger(10)
    }
  });
  anime({
    easing: "linear",
    delay: 4000,
    complete: () => {
      updateText("Submitted");
      setTimeout(() => {
        updateText("Submit");
        reset();
      }, 3000);
    }
  });
});
```
## **Support**
>**En caso de cualquier problema, puedes contactar con el creador, [Mikael Ainalem](https://twitter.com/mikaelainalem) en twitter, pues no hay otro método para contactarlo.**
