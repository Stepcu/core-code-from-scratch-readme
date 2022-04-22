# Interpreted and Compiled Programming Languages
1. Compiled Languagues are converted directly into machine code, they tend to be faster and more efficient than the Interpreted Language. It requires an aditional step before executing since it needs to convert our code to machine language. Some compiled languages are: C++, C, GO. 
2. The Interpreted Language goes through the instructions and interprets them one by one, every time the program is executed. They are a little bit slower than the compiled languages but with the development of just-in-time-compilation this is decreasing. Some Interpreted languages are: JavaScript, PHP, Python.
3. The JAVA programming language can be considered as a Hybrid because it can be either an Interpreted Language or a Compiled Language. It is first compiled into bytecode and then interpreted.
# Pseudocode currency converter
1. START
2. B <-- GET FROM('https://coinmarketcap.com/es/currencies/bitcoin/')
3. Q <-- GET
4. R <-- Q * B
5. PRINT R
6. END
# Date of birth in binary
date of birth: 1998
* 1998/2 = 999 R 0
* 999/2 = 499 R 1
* 499/2 = 249 R 1
* 249/2 = 124 R 1
* 124/2 = 62 R 0
* 62/2 = 31 R 0
* 31/2 = 15 R 1
* 15/2 = 7 R 1
* 7/2 = 3 R 1
* 3/2 = 1 R 1
* 1/2 = 0 R 1

Decimal : 1998   Binary : 11111001110
# program that adds any two given numbers provided by the user
``
.data<br>
	      number1: .asciiz "\nAdd a first number: "<br>
	      number2: .asciiz "\nAdd a second number: "<br>
  .text<br>
	      main:<br>
              li $v0, 4<br>
              la $a0, number1<br>
              syscall<br>
              li $v0, 5<br>
              syscall<br>
              move $t0, $v0<br>
              li $v0, 4<br>
              la $a0, number2<br>
              syscall<br>
              li $v0, 5<br>
              syscall<br>
              move $t1, $v0<br>
              li $v0, 1<br>
              move $a0, $t0<br>
              syscall<br>``
# Program that displays my name
``
.data
<br>
         message: .asciiz "\nStefhany Castro\n"<br>
  .text<br>
        main:<br>
              li $v0, 4<br>
              la $a0, message<br>
              syscall<br>
	      ``
# Print special numbers
``
for(let i=0; i<=100; i=i+2){
console.log(i);
}
``
# Bad code
``
var cond = false;
if (cond == true) {
  console.log('The cond variable is true');
} else {
  console.log('The cond variable is false');
}``
The code was using an assignment instead of a comparision expression.
# Bad code 2
``var n = 100;
if (n == 100) {
  console.log('This is a special number!');
} else if (n < 1000 && n % 10 == 0) {
  console.log('This number is almost special');
} else {
  console.log('Just a regular number');
}``
# Multiply
``function multiply(a, b){
  return a * b
}``
# ASCII Total
``function uniTotal(string) {
  let total = 0;
  for (i = 0; i < string.length; i++) {
    total += string[i].charCodeAt();
  }
  return total;
}``
# Char From ASCII Value
``function getChar(c){
  return String.fromCharCode(c);
}``
# Binary Addition
``function addBinary(a,b) {
  return (a + b).toString(2);
}``
# Student's Final Grade
``function finalGrade (exam, projects) {
  if(exam > 90 || projects > 10){
    return 100;
  } else if(exam > 75 && projects >= 5){
    return 90;
  } else if(exam > 50 && projects >= 2){
    return 75;
  }
    return 0;  
}``
# Holiday VIII - Duty Free
``function dutyFree(normPrice, discount, hol){
let discountAmount = normPrice * discount / 100;
return Math.floor(hol / discountAmount);
}``
# Twice As Old
``function twiceAsOld(dadYearsOld, sonYearsOld) {
  let twice = sonYearsOld * 2;
  return Math.abs(dadYearsOld - twice);
}``
# Valid Spacing
``function validSpacing(s) {
  return s.trim() == s && !s.includes("  ");
}``
# Fake Binary
``function fakeBin(x){
  let final = '';
  for(let i = 0; i < x.length; i++){
    if(parseInt(x[i]) < 5){
      final = final + '0'; 
    } else {
      final = final + '1';
    }
  }
  return final;
}``
# Remove All Exclamation Marks From The End Of Sentence
``function remove (string) { 
  return string.replace(/!+$/, '');
}``
# Vowel Remover
``function shortcut (string) {
  return string.replace(/[aeiou]/gi, '');
}``
# Rock Paper Scissors!
``const rps = (p1, p2) => {
  if((p1 == 'scissors' && p2 == 'paper') || (p1 == 'rock' && p2 == 'scissors') || (p1 == 'paper' && p2 == 'rock')){
    return 'Player 1 won!'
  } else if((p2 == 'scissors' && p1 == 'paper') || (p2 == 'rock' && p1 == 'scissors') || (p2 == 'paper' && p1 == 'rock')){
    return 'Player 2 won!'
  }
  return 'Draw!'
};``
# Persistent Bugger
``function persistence(num) {
   var times = 0;
    num = num.toString();
    while (num.length > 1) {
        times++;
        num = num.split('').map(Number).reduce((a, b) => a * b).toString();
    }
    return times;
}``
