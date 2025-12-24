<!DOCTYPE html>
<html lang="uk">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Jur1us</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        html, body {
            height: 100%;
            width: 100%;
            overflow: hidden;
            background-color: #000;
        }
        
        .fullscreen-gif {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            object-fit: cover;
            z-index: 1;
        }
        
        .content-overlay {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: 2;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            background-color: rgba(0, 0, 0, 0.3);
        }
        
        .links {
            display: flex;
            gap: 30px;
            margin-top: 20px;
        }
        
        .link {
            color: white;
            text-decoration: none;
            font-family: Arial, sans-serif;
            font-size: 18px;
            padding: 10px 20px;
            background-color: rgba(0, 0, 0, 0.5);
            border-radius: 5px;
            transition: all 0.3s ease;
        }
        
        .link:hover {
            background-color: rgba(255, 255, 255, 0.2);
            transform: translateY(-2px);
        }
        
        .separator {
            color: white;
            font-size: 20px;
            margin: 0 5px;
        }
        
        /* Адаптивність для мобільних */
        @media (max-width: 768px) {
            .links {
                flex-direction: column;
                gap: 15px;
                align-items: center;
            }
            
            .separator {
                display: none;
            }
            
            .link {
                font-size: 16px;
                padding: 8px 16px;
            }
        }
    </style>
</head>
<body>
    <!-- Гіфка на всю площу -->
    <img src="https://raw.githubusercontent.com/glepnir/glepnir/master/1.gif" 
         alt="Background GIF" 
         class="fullscreen-gif">
    
    <!-- Контент поверх гіфки -->
    <div class="content-overlay">
        <!-- Посилання -->
        <div class="links">
            <a href="https://www.instagram.com/jur1us/?__d=1%2F%2F" 
               class="link" 
               target="_blank">Instagram</a>
            
            <span class="separator">•</span>
            
            <a href="mailto:romanworkoutvlg@gmail.com" 
               class="link">Email me</a>
        </div>
    </div>
</body>
</html>
