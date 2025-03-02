```js
function calculateAreaOfCircle(radius) {
    const pi = 3.14159; //  π
    let area = pi * radius * radius;  
    return area;
}

let radius = 10;
let area = calculateAreaOfCircle(radius);
console.log("The area of the circle with radius " + radius + " is: " + area.toFixed(2));  

```