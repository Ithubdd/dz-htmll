<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Машинка</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #e0f7fa;
            margin: 0;
        }

        .car {
            width: 200px;
            height: 100px;
            background-color: #ff5722;
            border-radius: 10px;
            position: relative;
        }

        .car::before {
            content: '';
            width: 80px;
            height: 50px;
            background-color: #ff5722;
            border-radius: 10px;
            position: absolute;
            top: -25px;
            left: 60px;
        }

        .wheel {
            width: 40px;
            height: 40px;
            background-color: #000;
            border-radius: 50%;
            position: absolute;
            bottom: -20px;
        }

        .wheel.left {
            left: 20px;
        }

        .wheel.right {
            right: 20px;
        }
    </style>
</head>
<body>
    <div class="car">
        <div class="wheel left"></div>
        <div class="wheel right"></div>
    </div>
</body>
</html>
