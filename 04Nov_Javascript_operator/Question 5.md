```js
function calculateSimpleInterest(principal, rate, time) {
    let simpleInterest = (principal * rate * time) / 100;
    return simpleInterest;
}


let interest = calculateSimpleInterest(1000, 5, 3);
console.log("The Simple Interest is: " + interest); //150

```