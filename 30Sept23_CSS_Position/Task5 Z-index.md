The z-index property in CSS controls the stacking order of elements. When elements overlap each other, the z-index determines which one appears on top. It only works on elements that have a position value other than static (e.g., relative, absolute, fixed, or sticky).

Higher z-index values are stacked on top of lower values.
Elements with the same z-index are stacked in the order they appear in the HTML document.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>z-index Example</title>
    <style>
        *, *::after, *::before {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: Arial, sans-serif;
            background-color: #f0f0f0;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
        }

        .container {
            position: relative; 
            width: 300px;
            height: 300px;
            background-color: #fff;
            border: 1px solid #ccc;
        }

        .box {
            position: absolute; /
            width: 100px;
            height: 100px;
            transition: all 0.3s ease;
        }

        .box1 {
            background-color: red;
            top: 50px;
            left: 50px;
            z-index: 2; 
        }

        .box2 {
            background-color: blue;
            top: 100px;
            left: 100px;
            z-index: 1; /* Lower z-index: below .box1 */
        }

        .box3 {
            background-color: green;
            top: 150px;
            left: 150px;
            z-index: 3; 
        }

        .box:hover {
            transform: scale(1.1); 
        }
    </style>
</head>
<body>

    <div class="container">
        <div class="box box1"></div>
        <div class="box box2"></div>
        <div class="box box3"></div>
    </div>

</body>
</html>

```