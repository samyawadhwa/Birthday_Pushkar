<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Happy Birthday Pushkar</title>
    <style>
        * {
            box-sizing: border-box;
        }

        body, html {
            margin: 0;
            padding: 0;
            width: 100%;
            height: 100%;
            background-color: #000;
            overflow: hidden; /* Prevents scrolling */
            display: flex;
            justify-content: center;
            align-items: center;
        }

        /* This creates the full-page floral frame */
        .floral-frame {
            position: fixed;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            pointer-events: none; /* Allows clicking through the border */
            border: 25px solid transparent;
            border-image: url("data:image/svg+xml,%3Csvg width='100' height='100' viewBox='0 0 100 100' xmlns='http://www.w3.org/2000/svg'%3E%3Ctext y='50' font-size='40'%3E🌸%3C/text%3E%3Ctext x='50' y='90' font-size='40'%3E🌺%3C/text%3E%3C/svg%3E") 30 round;
            z-index: 10;
        }

        .content {
            text-align: center;
            z-index: 5;
            padding: 20px;
        }

        .line-1 {
            color: #ffffff;
            font-family: 'Segoe UI', Roboto, sans-serif;
            font-size: 1.8rem;
            font-weight: 300;
            margin-bottom: 10px;
            opacity: 0;
            transform: translateY(30px);
            animation: appear 1.2s ease-out forwards;
        }

        .line-2 {
            color: #ff4081;
            font-family: 'Arial Black', sans-serif;
            font-size: 4rem;
            text-transform: uppercase;
            letter-spacing: 4px;
            margin: 0;
            opacity: 0;
            transform: translateY(30px);
            animation: appear 1.2s ease-out forwards;
            animation-delay: 0.6s;
            text-shadow: 0 0 20px rgba(255, 64, 129, 0.4);
        }

        @keyframes appear {
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        /* Subtle glow in the center */
        .bg-glow {
            position: absolute;
            width: 100%;
            height: 100%;
            background: radial-gradient(circle, rgba(255, 64, 129, 0.15) 0%, rgba(0,0,0,0) 70%);
            z-index: 1;
        }
    </style>
</head>
<body>

    <div class="floral-frame"></div>
    <div class="bg-glow"></div>

    <div class="content">
        <div class="line-1">Happiest Birthday</div>
        <h1 class="line-2">Pushkar</h1>
    </div>

</body>
</html>
