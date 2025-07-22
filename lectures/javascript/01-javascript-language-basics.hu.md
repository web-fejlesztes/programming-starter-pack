# JavaScript alapok - 1. lecke

- Szintaxis (syntax)
  > A "szintaxis" egy programozási nyelv
  vagy bármilyen formális nyelv szabályainak és struktúráinak összessége,
  amely meghatározza, hogyan kell használni a nyelvet, hova kell írni a pontosvesszőket, blokkokat, utasításokat, stb.
- Változók (variables)
- Adat típusok (data types)
- Kiiratás (console)
- Operátorok (operators)
- Vezérlési szerkezetek (control flow)
  - Feltételek (conditions)
  - Ciklusok (loops)

## Megnézendő ingyenes anyagok - videók

Videó nézése közben érdemes jegyzetelni, felírni a kérdéseidet,
amiket fel tudsz később tenni akár egy mentornak, akár a ChatGPT-nek, így is segítve,
hogy mégjobban megértsd a témát.

Ha a videó megnézése után marad időd, akkor érdemes megpróbálni megoldani a feladatokat,
hogy még több kérdésed legyen, hogy szembesülj azzal, hogyha valamit mégse értesz egészen. 

### Magyar nyelvű anyagok

| Forrás                                                                                              | hossz |
|-----------------------------------------------------------------------------------------------------|-------|
| [#1 Tanulj JavaScript-et!](https://youtu.be/IV8aGwttIv0)                                            | 06:34 |
| [#2 Hello Világ, felkészülünk a fejlesztésre](https://youtu.be/aStmt8T0h5U)                         | 05:14 |
| [#3 Literálok, Kifejezések, Utasítások, Változók](https://youtu.be/RBiQOlM8HpQ)                     | 13:10 |
| [#4 Konstansok, speciális értékek, még több operátor, típuskonverzió](https://youtu.be/GABLMi7Bki4) | 09:28 |
| [#5 Feltételek, Elágazások](https://youtu.be/Br7ekaB9hZI)                                           | 10:34 |
| [#6 Ciklusok: while és for](https://youtu.be/n4vq0I_hd9o)                                           | 06:56 |

### Angol nyelvű anyagok (Opcionális)

| Source                                                                                                                | Duration |
|-----------------------------------------------------------------------------------------------------------------------|----------|
| [JavaScript Tutorial For Beginners 01 - Introduction](https://www.youtube.com/watch?v=qoSksQ4s_hg)                    | 3:40     |
| [JavaScript for Beginners 02 - What is JavaScript?](https://www.youtube.com/watch?v=VB7y0yxZjro)                      | 4:03     |
| [JavaScript Tutorial For Beginners 03 - Hello World! in JavaScript](https://www.youtube.com/watch?v=ranSYb-EhrU)      | 3:17     |
| [JavaScript Tutorial For Beginners #4 - Where to put your JS](https://www.youtube.com/watch?v=czlwRUeTCgw)            | 5:13     |
| [JavaScript Tutorial For Beginners #5 - Google Chrome Developer Tools](https://www.youtube.com/watch?v=JzZFccCEgGA)   | 4:51     |
| [JavaScript Tutorial For Beginners #6 - Basic JavaScript Syntax & Rules](https://www.youtube.com/watch?v=QLatPwsbDrQ) | 7:49     |
| [JavaScript Tutorial For Beginners #7 - JavaScript Variables](https://www.youtube.com/watch?v=u0Mq3FzpsmI)            | 8:59     |
| [let vs var - Topics of JavaScript/ES6](https://www.youtube.com/watch?v=q8SHaDQdul0)                                  | 12:19    |
| [const - Topics of JavaScript/ES6](https://www.youtube.com/watch?v=2iLVFyYwyRA)                                       | 7:41     |
| [JavaScript Tutorial For Beginners #8 - Basic Mathematical Operators](https://www.youtube.com/watch?v=_MC0Gw07w8M)    | 6:16     |
| [JavaScript Tutorial For Beginners #9 - Math Operator Short-hand](https://www.youtube.com/watch?v=Z1eV0RBRam0)        | 4:55     |
| [JavaScript Tutorial For Beginners #10 - Logging to the Console](https://www.youtube.com/watch?v=tH-q9QFNUdA)         | 3:38     |
| [JavaScript Tutorial For Beginners #11 - Booleans in JavaScript](https://www.youtube.com/watch?v=B4ZCFdrBmbE)         | 6:13     |
| [JavaScript Tutorial For Beginners #12 - If Statements](https://www.youtube.com/watch?v=Lp-Du2fKoug)                  | 8:45     |
| [JavaScript Tutorial For Beginners #13 - Else If Statements](https://www.youtube.com/watch?v=1v1Bk3Q02Sc)             | 4:03     |
| [JavaScript Tutorial For Beginners #14 - Comparison Operators](https://www.youtube.com/watch?v=LjGaaWX_NbE)           | 5:25     |
| [JavaScript Tutorial For Beginners #15 - Logical Operators](https://www.youtube.com/watch?v=mbT7sSmVUS8)              | 6:01     |
| [JavaScript Tutorial For Beginners #16 - While Loops](https://www.youtube.com/watch?v=PpbFyLTtpWI)                    | 4:09     |
| [JavaScript Tutorial For Beginners #17 - For Loops](https://www.youtube.com/watch?v=U87UmD-5h4o)                      | 7:49     |
| [JavaScript Tutorial For Beginners #18 - Break & Continue](https://www.youtube.com/watch?v=QSuTH0C_3_Y)               | 4:13     |
| [JavaScript Tutorial For Beginners #19 - Practical Example using Loops](https://www.youtube.com/watch?v=eZBTLsv2ktM)  | 4:02     |
| [JavaScript Tutorial For Beginners #22 - Numbers](https://www.youtube.com/watch?v=TD3Pfuxgnuc)                        | 6:09     |
| [JavaScript Tutorial For Beginners - NaN (Not a Number)](https://www.youtube.com/watch?v=0ZiltZDg9Gg)                 | 6:34     |
| [JavaScript Tutorial For Beginners #24 - Strings](https://www.youtube.com/watch?v=k8MIbEVXhE0)                        | 9:37     |

## Téma áttekintése

- Saját kérdéseid amik felmerültek a videók nézése közben?

- Mire használjuk a JavaScriptet?
- Hogyan tudunk JavaScript kódot futtatni?
- Mi a Node.js?
- Kommentek (Comments)
- Szintaxis (Syntax)
- Mire szolgálnak a változók? Mihez hasonlíthatóak?
- Változók deklarálás (Declaring a variable)
  - `var` - Már ritkán használjuk
  - `let`
  - `const`
- Változók elnevezése
  - camelCase
  - angol nyelvű változónevek
  - Mikor használunk mégis anyanyelvi változóneveket?
- Változó inicializálása (Initializing a variable)
- Utasítások futtatási sorrendje (Execution order)
- `console`
- értékadás (assignment: `=`)
  - let
  - const
- Adat típusok
  - `string`
  - `number` - integer, float
  - `boolean`
  - `null`
  - `undefined`
- `typeof` - típusvizsgálat
- `'use strict'` használata
- Operátorok (Operators)
  - string összefűzés (concatenation: `+`)
  - aritmetikai (arithmetic: `+`, `-`, `/`, `*`, `%`, `**`, `++`, `--`)
    - 0-val való osztás
    - 0-t 0-al osztani
  - logikai (logical: `&&`, `||`, `!`)
  - összehasonlítás (comparison: `==`, `!=`, `===`, `!==`, `<`, `<=`, `>`, `>=`)
- Irányítási szerkezetek (Control structures)
  - `if` (ha)
  - `for` (ciklus)
- Típus konverzió (Type conversion)

## Előkövetelmények a feladatok elkezdéséhez

- CLI (Command Line Interface) ismeretek
- Git ismerete, legyen telepítve a gépen, ismerd a git parancsokat

### Node.js telepítése

- Mi a NodeJS?
  - A NodeJS egy JavaScript futtatási környezet, amely lehetővé teszi a JavaScript kód futtatását a számítógépen.
- [Node.js](https://nodejs.org/en/) - A NodeJS a JavaScript futtatásához szükséges program.
  - Az LTS (Long Term Support) verziót ajánlott telepíteni
- Ellenőrizd, hogy telepítve van-e a Node.js a gépeden:
  - Nyisd meg a terminált (Git Bash vagy CMD vagy PowerShell vagy Terminal vagy stb.)
  - Írd be a következő parancsot: `node -v`
  - Ha a parancs visszaad egy verziószámot, akkor telepítve van a Node.js
  - Ha nem ad vissza semmit, akkor nincs telepítve a Node.js

### Visual Studio Code telepítése

- Letöltés és majd telepítés innen: https://code.visualstudio.com/

## Feladatok

A feladatokat egy saját repositorydban oldd meg.

### Hello Firstname!

```js
// Modify this program to greet you instead of the World!
console.log('Hello, World!');
```

### Hello Mates!

```js
// Greet 3 of your classmates with this program in three separate lines
// like:
//
// Hello, May!
// Hello, Robert!
// Hello, Joe!
```

### My personal data

```js
// Write a program that prints a few details to the console about you
// It should print each detail to a new line:
//  - Your name
//  - Your age
//  - Your height in meters (as a decimal fraction)
//
//  Example output:
//  Nicolas Cage
//  42
//  1.78
```

### Basic arithmetics

```js
// Create a program that prints a few operations on two numbers: 22 and 13
// Solve it programmatically! Do not just write the result, but use variables.
// Print the result of 13 added to 22
// Print the result of 13 substracted from 22
// Print the result of 22 multiplied by 13
// Print the result of 22 divided by 13 (as a decimal fraction)
// Print the remainder of 22 divided by 13
```

### Calculate learning hours for a month

```js
// Solve it programmatically! Do not just write the result, but use variables.
// You are a student who wants to know how much time you spent with learning in a month
// If you spend 6 hours with learning from Monday to Friday it means that you spent 30 hours in a week with learning
// If you spend 4 hours with learning on Saturday and Sunday it means that you spent 8 hours in a weekend with learning
// How many hours did you spend with learning in a month of 4 weeks? Console out the result!
```

### Swap values

```js
// Swap the values of these variables
let longOfTheBridge = 123;
let longOfTheBoat = 526;
```

### Time left from the day

```js
// Write a program that prints the remaining seconds (as an integer) from a
// day if these variables represent the current time
let currentHours = 14;
let currentMinutes = 34;
let currentSeconds = 42;
```

### Even numbers

```js
// Print the even numbers till 20
```

### Multiplication table

```js
// Create a program that prints the multiplication table with number
let number = 15;

//
// Example:
// The number 15 should print:
//
// 1 * 15 = 15
// 2 * 15 = 30
// 3 * 15 = 45
// 4 * 15 = 60
// 5 * 15 = 75
// 6 * 15 = 90
// 7 * 15 = 105
// 8 * 15 = 120
// 9 * 15 = 135
// 10 * 15 = 150
```

### Count from to

```js
// Create a program that prints all the number from a beginning number to an end number
// For example the program should print all the numbers between 0 and 6
let from = 0;
let to = 6;
```

### FizzBuzz

```js
// Write a program that prints the numbers from 1 to 100.
// But for multiples of three print “Fizz” instead of the number
// and for the multiples of five print “Buzz”.
// For numbers which are multiples of both three and five print “FizzBuzz”.
```
