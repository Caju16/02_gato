# Learn JavaScript. Interactive tutorial.

Realiza los retos de [learnjavascript.online](https://learnjavascript.online/), una forma de aprender y practicar JavaScript moderno. 
Aprende en un entorno interactivo, con lecciones breves y resolviendo  desafíos directamente en el navegador.
Pega aquí los enunciados y tus soluciones.

Refactoriza el código de manera que sea REALMENTE JavaScript moderno:
- Evita el uso de bucles `for`/`while`
- No uses `var`
- Usa arrow functions. Simplifícalas lo más posible.
- Haz uso de médodos iterativos de arrays `map`, `filter`, `reduce`, `slice`...
- Usa operador ternario
- Usa template literal
- Usa las asignaciones simplificadas `++`, `+=`...

## 1. Basic Functions
### Basic sum
```javascript
/**
 * Realiza la suma de dos números 
 * 
 * @param {number} a sumando 1
 * @param {number} b sumando 2
 * 
 */
function sum(a, b) {
    return a+b;
}

// sample usage - do not modifyç

console.log(sum(1, 3));
console.log(sum(2, 5));
```

### Basic multiplication
```javascript
/**
 * @param {number} a
 * @param {number} b
 */
function multiply(a, b) {
    return a*b
}

// sample usage - do not modify
console.log(multiply(2, 4));
console.log(multiply(3, 2));
```

## 2. Strings I
### Strings

#### String length
 

```javascript
/**
 * @param {string} str
 */
function getCharCount(str) {
    return str.length
}

// Sample usage - do not modify
console.log(getCharCount("Sam")); // 3
console.log(getCharCount("Alex 123")); // 8
console.log(getCharCount("Charley is here")); // 15
```

#### Shout my name

```javascript
/**
 * @param {string} name
 */
function shoutMyName(name) {
    return name.toUpperCase()
}

// Sample usage - do not modify
console.log(shoutMyName("Sam")); // "SAM"
console.log(shoutMyName("Charley")); // "CHARLEY"
console.log(shoutMyName("alex")); // "ALEX"
```
 
#### Lower case string
 

```javascript
/**
 * @param {string} name
 */
function lowerName(name) {
    return name.toLocaleLowerCase()
}

// Sample usage - do not modify
console.log(lowerName("Sam")); // "sam"
console.log(lowerName("ALEX")); // "alex"
```
### Character access

#### Get first character

 ```javascript
/**
 * @param {string} name
 */
function getFirstCharacter(name) {
    return name.at(0)
}

// Sample usage - do not modify
console.log(getFirstCharacter("Amsterdam")); // "A"
console.log(getFirstCharacter("Japan")); // "J"
```


 
#### Get last character
 
 ```javascript
/**
 * @param {string} name
 */
function getLastCharacter(name) {
    return name.at(-1)
}

// Sample usage - do not modify
console.log(getLastCharacter("Sam")); // "m"
console.log(getLastCharacter("Alex")); // "x"
console.log(getLastCharacter("Charley")); // "y"
```

### Substrings

#### Skip first character
 ```javascript
/**
 * @param {string} text
 */
function skipFirstCharacter(text) {
    return text.slice(1)
}

// Sample usage - do not modify
console.log(skipFirstCharacter("Xcode")); // "code"
console.log(skipFirstCharacter("Hello")); // "ello"
```
 
#### Text ellipsis Project I

```javascript
/**
 * @param {string} text
 */
export function getDescription(text) {
    return text.slice(0,10)
}
```
 
### Plus operator

#### String concatenation

```javascript
/**
 * @param {string} firstNameInitial
 * @param {string} lastNameInitial
 */
function concatInitials(firstNameInitial, lastNameInitial) {
    return firstNameInitial+lastNameInitial
}

// Sample usage - do not modify
console.log(concatInitials("J", "D")); // "JD"
console.log(concatInitials("S", "B")); // "SB"
```
 
#### Text ellipsis Project II




```javascript
/**
 * @param {string} text
 */
export function getDescription(text) {
    console.log(text); // write something in the BROWSER and see it in the console
    return text.slice(0, 10)+"..."
}
```

### Template strings

#### String interpolation

```javascript
/**
 * @param {string} name
 */
function sayHello(name) {
    return `Hello ${name}` 
}

// Sample usage - do not modify
console.log(sayHello("Alex")); // "Hello Alex"
console.log(sayHello("Sam")); // "Hello Sam"
```

#### String interpolation advanced


```javascript
/**
 * @param {string} firstName
 * @param {string} lastName
 */
function getFullName(firstName, lastName) {
    return `${firstName} ${lastName}`
}

// Sample usage - do not modify
console.log(getFullName("Sam", "Doe")); // "Sam Doe"
console.log(getFullName("Alex", "Blue")); // "Alex Blue"
```
#### Multiline string

```javascript
function getMultilineString() {
return `I am learning JavaScript  
    and I found it to be  
    quite fun!`
}

// Sample usage - do not modify
console.log(getMultilineString());
```
#### Nutrition table I

```javascript
/**
 * @param {string} label
 * @param {string} value
 */
export function renderTableRow(label, value) {
return `
<tr>
    <td>${label}</td>
    <td>${value}</td>
</tr>`
}
```
#### Capitalize word

```javascript
/**
 * @param {string} word
 */
function capitalize(word) {
    return word.slice(0, 1).toLocaleUpperCase()+word.slice(1).toLowerCase()
}

// Sample usage - do not modify
console.log(capitalize("sam")); // "Sam"
console.log(capitalize("ALEX")); // "Alex"
console.log(capitalize("chARLie")); // "Charlie"
```
#### Name variations Project

```javascript
/** @param {string} name */
export function getNumberOfChars(name) {
    // number of characters in: name
    return name.length
}

/** @param {string} name */
export function getFirstChar(name) {
    // first character of: name
    return name[0]
}

/** @param {string} name */
export function getLastChar(name) {
    // last character of: name
    return name.at(-1)
}

/** @param {string} name */
export function getLower(name) {
    // name all in lower case (example: "ABC" becomes "abc")
    return name.toLocaleLowerCase()
}

/** @param {string} name */
export function getUpper(name) {
    // name all in upper case (example: "abc" becomes "ABC")
    return name.toLocaleUpperCase()
}

/** @param {string} name */
export function getCapitalized(name) {
    // capitalized version of name (example: "alEX" becomes "Alex")
    return name.slice(0, 1).toLocaleUpperCase()+name.slice(1).toLocaleLowerCase()
}
```


## 3. Numbers

### Numbers

#### Number to string conversion
```javascript
/**
 * @param {number} number
 */
function convertNumberToString(number) {
    return number + ""
}

// Sample usage - do not modify
console.log(convertNumberToString(42)); // "42"
console.log(convertNumberToString(97)); // "97"
console.log(convertNumberToString(11)); // "11"
```

### Convert string to number

#### Get next age I
```javascript
/**
 * @param {string} age
 */
export function getNextAge(age) {
    return ++age
}
```

#### Get box width
```javascript
/**
 * @param {string} value
 */
export function getBoxWidth(value) {
    return Number.parseInt(value)
}
```

### Operations

#### Get division remainder by 2
```javascript
/**
 * @param {number} number
 */
export function getDivisionRemainderBy2(number) {
    return number%2
}
```

## 4. Variables
### Variables
#### Define a variable
```javascript
//define a variable "count" with value 0
let count=0
//then increment it
count++
```
#### Age limit
```javascript
//define a variable "ageLimit" with value 18 that cannot be re-assigned
const ageLimit=18
```
 
## 5. Conditions
### Conditions
#### Can you vote?
```javascript
/**
 * @param {number} age
 */
function canVote(age) {
    return age>=18
}

// Sample usage - do not modify
console.log(canVote(25)); // true
console.log(canVote(18)); // true
console.log(canVote(10)); // false
```
### Advanced if
#### Get next age II
```javascript
/**
 * @param {string} age
 */
export function getNextAge(age) {
    return age?++age:0
}
```
#### Text ellipsis Project III
```javascript
/**
 * @param {string} text
 */
export function getDescription(text) {
    return text.slice(0, 10)+(text.length>10?"...":"");
}
```
### Returning booleans
#### Can you vote (improved)
```javascript
/**
 * @param {number} age
 */
function canVote(age) {
    return age>=18
}

// Sample usage - do not modify
console.log(canVote(25)); // true
console.log(canVote(18)); // true
console.log(canVote(17)); // false
```
### Even & Odd
#### Get division remainder by 2
```javascript
/**
 * @param {number} number
 */
export function evenOrOdd(number) {
    return number%2?"odd":"even"
}
```
 
## 6. Arrays I

### Arrays

#### Empty array
```javascript
function getEmptyArray() {
    return []
}

// Sample usage - do not modify
console.log(getEmptyArray());
```

#### Number of elements
```javascript
/**
 * @param {array} elements
 */
function getNumberOfElements(elements) {
    return elements.length
}

// Sample usage - do not modify
console.log(getNumberOfElements(['a', 'b', 'c'])); // 3
console.log(getNumberOfElements([])); // 0
```

#### Add calculator to apps
```javascript
/**
 * @param {array} elements
 */
function getNumberOfElements(elements) {
    return elements.length
}

// Sample usage - do not modify
console.log(getNumberOfElements(['a', 'b', 'c'])); // 3
console.log(getNumberOfElements([])); // 0
```

#### Use any app
```javascript
/**
 * @param {array} apps
 * @param {string} app
 */
function useApp(apps, app) {
    apps.push(app)
    return apps
}

// Sample usage - do not modify
console.log(useApp(["Clock", "Twitter"], "Firefox")); // ["Clock", "Twitter", "Firefox"]
console.log(useApp([], "Safari")); // ["Safari"]
```

#### Get first app
```javascript
/**
 * @param {array} apps
 */
function getFirstApp(apps) {
    return apps[0]
}

// Sample usage - do not modify
console.log(getFirstApp(["Chrome", "Clock", "Twitter"])); // "Chrome"
console.log(getFirstApp(["Clock", "Contacts"])); // "Clock"
```

#### Get last app
```javascript
/**
 * @param {array} apps
 */
function getLastApp(apps) {
    return apps.at(-1)
}

// Sample usage - do not modify
console.log(getLastApp(["Chrome", "Clock", "Twitter"])); // "Twitter"
console.log(getLastApp(["Safari", "Contacts"])); // "Contacts"
```

### Array forEach


#### Loop through array elements
```javascript
/**
 * @param {array} elements
 */
function loopThroughElements(elements) {
    elements.forEach( e => console.log(e));
}

// Sample usage - do not modify
loopThroughElements(["Sam", "Charlie", "Alex"]); // should log every name to the console
```

#### Log user ids
```javascript
/**
 * @param {number[]} userIds
 */
function logUserIds(userIds) {
    userIds.forEach( u => console.log(u))
}

// Sample usage - do not modify
logUserIds([10, 15, 14]); // should log every userId to the console
```

#### Return confusion

#### Sum grades
```javascript
/**
 * @param {number[]} grades
 */
function sumGrades(grades) {
    return grades.reduce((a, b) => a+b)
}

// Sample usage - do not modify
console.log(sumGrades([15, 5, 10])); // 30
console.log(sumGrades([12, 10, 13, 19])); // 54
```

#### Sum positive numbers
```javascript
/**
 * @param {number[]} numbers
 */
function sumPositiveNumbers(numbers) {
    return numbers
        .filter(x=>x>0)
        .reduce((a, b)=>a+b, 0)
}

// Sample usage - do not modify
console.log(sumPositiveNumbers([15, -5, 10])); // 25
console.log(sumPositiveNumbers([-3, 4, -2, 1])); // 5
```

#### Sum odd numbers
```javascript
/**
 * @param {number[]} numbers
 */
function sumOddNumbers(numbers) {
    return numbers
        .filter( n => n%2)
        .reduce((a, b) => a+b)
}

// Sample usage - do not modify
console.log(sumOddNumbers([15, 5, 10])); // 20
console.log(sumOddNumbers([2, 3, 4, 5, 6])); // 8
console.log(sumOddNumbers([-2, -3, 4, 5, 6])); // 2
```

#### Countries dropdown I
```javascript
/**
 * @param {string[]} countries
 */
export function getDropdown(countries) {
    let options =`<option value="">Please select</option>`;
    countries.forEach(c => options += `<option value="${c.toLocaleLowerCase()}">${c}</option>`);
    return options;
}
```

#### Nutrition table II
```javascript
/**
 * @param {array[][]} rows
 */
export function renderTableRows(rows) {
    let table = "";
    rows.forEach(r => table += `
    <tr>
        <td>${r[0]}</td>
        <td>${r[1]}</td>
    </tr>`);
    return table;
    }
```

## 7. Arrays II & callbacks

### Array filter

#### Positive temperatures
```javascript
/**
 * @param {number[]} temperatures
 */
function getPositiveTemperatures(temperatures) {
    return temperatures.filter(t=>t>0)
}

// Sample usage - do not modify
console.log(getPositiveTemperatures([-5, 12, 3])); // [12, 3]
console.log(getPositiveTemperatures([1, -3, -2, 4, 10])); // [1, 4, 10]
```
#### Freezing temperatures
```javascript
/**
 * @param {number[]} temperatures
 */
function getFreezingTemperatures(temperatures) {
    return temperatures.filter(t=>t<0)
}

// Sample usage - do not modify
console.log(getFreezingTemperatures([-5, 12, 3])); // [-5]
console.log(getFreezingTemperatures([1, -3, -2, 4, 10])); // [-3, -2]
```

#### Array find


#### Get year
```javascript
/**
 * @param {number[]} years
 * @param {number} searchYear
 */
function getYear(years, searchYear) {
    return years.find(y=>y==searchYear)
}

// Sample usage - do not modify
console.log(getYear([2019, 2020, 2021], 2020)); // 2020
console.log(getYear([2019, 2020, 2021], 1990)); // undefined
```

#### Odd Years
```javascript
/**
 * @param {number[]} years
 */
function getOddYears(years) {
    return years.filter(y=>y%2)
}

// Sample usage - do not modify
console.log(getOddYears([2019, 2020, 2021])); // [2019, 2021]
console.log(getOddYears([2000, 2015, 2018, 2020])); // [2015]
```

### More array methods

#### Is app used?
```javascript
/**
 * @param {string[]} apps
 * @param {string} app
 */
function isAppUsed(apps, app) {
    return apps.includes(app)
}

// Sample usage - do not modify
console.log(isAppUsed(["Twitter", "Calculator"], "Calculator")); // true
console.log(isAppUsed(["Clock", "Calculator"], "Safari")); // false
```

#### String sizes
```javascript
/**
 * @param {string[]} strings
 */
function getStringSizes(strings) {
    return strings.map(s=>s.length)
}

// Sample usage - do not modify
console.log(getStringSizes(["a", "abc"])); // [1, 3]
console.log(getStringSizes(["Sam", "Alex", "Charlie"])); // [3, 4, 7]
console.log(getStringSizes(["Hello", "Blue"])); // [5, 4]
```

#### Classroom Project I
```javascript
/** @param {number[]} grades */
export function getNumberOfGrades(grades) {
    return grades.length
}

/** @param {number[]} grades */
export function getSumGrades(grades) {
    return  grades.reduce((a, b) => a+b, 0)
}

/** @param {number[]} grades */
export function getAverageValue(grades) {
    return  grades.reduce((a, b) => a+b, 0)/grades.length
}

/** @param {number[]} grades */
export function getPassingGrades(grades) {
    return grades.filter(g => g>=10)
}

/** @param {number[]} grades */
export function getFailingGrades(grades) {
    // TODO: return all failing grades (9 and below)
    return grades.filter(g => g<10)
}

/** @param {number[]} grades */
export function getRaisedGrades(grades) {
    // TODO: return all the grades raised by 1 (no grade should exceed 20)
    return grades.map(g => ++g>20?20:g);
    //return grades.map(g => Math.min(++g, 20));
}
```

#### Voters stats API
```javascript
/**
 * @param {number[]} ages
 */
export function getVotersCount(ages) {
    return ages.filter(a => a>=18).length
}
```