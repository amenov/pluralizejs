# pluralizejs
  
###### JavaScript пакет для склонения существительных по числам    
  
  
### Пример использования  
  
Представим, что вам необходимо отображать правильное склонение существительных не в зависимости от переданного числа:  
  
1 яблоко  
2 яблока  
3 яблок  
24 яблок  
... т.д.  
  
```javascript
const pluralize = require('pluralizejs')

let words = ['яблоко', 'яблока', 'яблок'] // здесь может быть любое существительное в трех видах (машина, машины, машин) и т.д
let number = 3; // Представим, что это число приходит нам с API
let concat = true // Конкатенирует переданное число со словом

let result = pluralize(number, words, concat)

console.log(result) // 3 яблок

concat = false

console.log(pluralize(number, word, concat)) // яблок

```
