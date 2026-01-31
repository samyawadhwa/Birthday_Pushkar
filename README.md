# Birthday_Pushkar
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy Birthday Pushkar</title>
    <style>
        body {
            margin: 0;
            height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            background-color: #000; /* Modern Black */
            font-family: 'Inter', -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif;
            overflow: hidden;
            /* Medium Sized Floral Border */
            border: 25px solid transparent;
            border-image: url("data:image/svg+xml,%3Csvg width='100' height='100' viewBox='0 0 100 100' xmlns='http://www.w3.org/2000/svg'%3E%3Ctext y='50' font-size='40'%3E🌸%3C/text%3E%3Ctext x='50' y='90' font-size='40'%3E🌺%3C/text%3E%3C/svg%3E") 30 round;
            box-sizing: border-box;
        }

        .container {
            text-align: center;
            padding: 20px;
        }

        h1 {
            color: #ffffff;
            font-weight: 700;
            line-height: 1.2;
            margin: 0;
        }

        .line-1 {
            font-size: 2.5rem;
            color: #fce4ec;
            opacity: 0;
            transform: translateY(20px);
            animation: appear 1s ease-out forwards;
        }

        .line-2 {
            font-size: 5rem;
            color: #ff4081; /* Vibrant Pink */
            text-transform: uppercase;
            letter-spacing: 5px;
            opacity: 0;
            transform: translateY(20px);
            animation: appear 1s ease-out forwards;
            animation-delay: 0.8s; /* Appears after first line */
        }

        /* Modern Fade-In Appear Animation */
        @keyframes appear {
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .glow {
            position: absolute;
            width: 300px;
            height: 300px;
            background: radial-gradient(circle, rgba(255, 64, 129, 0.2) 0%, rgba(0,0,0,0) 70%);
            z-index: -1;
        }
    </style>
</head>
<body>

    <div class="glow"></div>
    <div class="container">
        <div class="line-1">Happiest Birthday</div>
        <h1 class="line-2">Pushkar</h1>
    </div>

</body>
</html>
