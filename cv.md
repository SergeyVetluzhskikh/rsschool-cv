 # Sergey Vetluzhskikh
 ![my photo](./assets/img/photo.jpeg)
---
| My contacts
---
#[Telegram](https://t.me/Lord_Hemingway)
#[Github](https://github.com/SergeyVetluzhskikh)
# Discord rs-school > 🐾(@SergeyVetluzhskikh)
---
| About me
---
 ### I am actively studying html css and javascript, my goal is to learn how to work with technologies and frameworks related to frontend development.
 ---
 | Skills 
 ---
 * HTML
 * CSS
 * JAVASCRIPT
 ---
 | Code examples
 ---
 #### Gamebot
 ```
 "use strict";
let getRandomNumber = (min, max) => {
  min = Math.ceil(min);
  max = Math.floor(max);
  return Math.floor(Math.random() * (max - min + 1)) + min;
};

let attempts = 10;
let botNumber = getRandomNumber(1, 20);
console.log(botNumber);

const gameBot = () => {
  let userNumber = prompt("Угадай число от 1 до 20");
  
  const decision = () => {
    attempts--;
    if (userNumber == botNumber) {
      alert("Поздравляю, Вы угадали!!!");
      if (confirm("Хотели бы сыграть еще?")) {
        attempts = 10;
        botNumber = getRandomNumber(1, 20);
        gameBot();
      }
    } else if (attempts === 0) {
      alert("Попытки закончились");
      if (confirm("Xотите попробовать снова?")) {
        attempts = 10;
        botNumber = getRandomNumber(1, 20);
        gameBot();
      }
    } else if (userNumber < botNumber && userNumber > 0 && userNumber < 21) {
      alert(`Загаданное число больше, осталось попыток ${attempts}`);
      gameBot();
    } else if (userNumber > botNumber && userNumber > 0 && userNumber < 21) {
      alert(`Загаданное число меньше, осталось попыток ${attempts}`);
      gameBot();
    } else if (isNaN(userNumber)) {
      alert("Введи число!");
      gameBot();
    } else if (userNumber == null) {
      alert("Игра окончена");
    }
    return;
  };
  decision();
};
gameBot();
```
---
| English language
---
### A1
