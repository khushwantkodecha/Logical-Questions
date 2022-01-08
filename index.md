## 1. String palindrome check

```
    let str = "nitin";
    let str2 = "";
    for (let i = str.length - 1; i >= 0; i--) {
    str2 = str2 + str[i];
    }
    if (str == str2) {
    console.log("palindrome");
    } else {
    console.log("not palidrome!");
    }
```

## 2. Number palindrome check

```
    function Palindrome(num) {
    var rem,
        temp,
        final = 0;
    var number = Number(num);

    temp = number;
    while (number > 0) {
        rem = number % 10;
        number = parseInt(number / 10);
        final = final * 10 + rem;
    }
    if (final == temp) {
        console.log("The inputed number is Palindrome");
    } else {
        console.log("The inputted number is not palindrome");
    }
    }

    Palindrome(123321);
```
