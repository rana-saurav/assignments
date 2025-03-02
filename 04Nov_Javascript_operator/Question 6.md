```js
function calculateBMI(weight, height) {
    let bmi = weight / (height * height);
    return bmi;
}


let bmi = calculateBMI(70, 1.75);
console.log("Your BMI is: " + bmi.toFixed(2));  //22.86
