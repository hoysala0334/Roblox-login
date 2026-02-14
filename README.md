<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Login - Roblox</title>
    <style>
        :root {
            --bg-color: #232527;
            --card-bg: #393b3d;
            --nav-bg: #191b1d;
            --input-bg: #4b4d4f;
            --button-blue: #0084ff;
            --button-hover: #0074e0;
            --text-main: #ffffff;
            --text-secondary: #bdbebf;
            --border-color: #111111;
        }

        * { box-sizing: border-box; margin: 0; padding: 0; }

        body {
            background-color: var(--bg-color);
            font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
            color: var(--text-main);
        }

        /* 1. TOP NAVIGATION BAR */
        nav {
            background-color: var(--nav-bg);
            height: 40px;
            display: flex;
            align-items: center;
            padding: 0 20px;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 100;
        }

        .nav-logo {
            height: 24px;
            cursor: pointer;
        }

        /* 2. MAIN CONTAINER */
        .page-content {
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            padding-top: 40px;
        }

        .login-card {
            background-color: var(--card-bg);
            padding: 30px;
            border-radius: 8px;
            width: 400px;
            box-shadow: 0 1px 4px rgba(0,0,0,0.5);
        }

        /* 3. SIGN IN / SIGN UP TABS */
        .tabs {
            display: flex;
            margin-bottom: 25px;
            border-bottom: 1px solid var(--input-bg);
        }

        .tab {
            flex: 1;
            text-align: center;
            padding-bottom: 10px;
            font-weight: bold;
            font-size: 16px;
            cursor: pointer;
            color: var(--text-secondary);
            text-decoration: none;
        }

        .tab.active {
            color: white;
            border-bottom: 3px solid white;
        }

        /* 4. FORM ELEMENTS */
        .form-title {
            font-size: 20px;
            font-weight: 500;
            margin-bottom: 20px;
            text-align: center;
        }

        .input-box {
            width: 100%;
            padding: 12px;
            background-color: var(--input-bg);
            border: 1px solid var(--border-color);
            border-radius: 4px;
            color: white;
            margin-bottom: 15px;
            font-size: 14px;
        }

        .login-btn {
            width: 100%;
            background-color: var(--button-blue);
            color: white;
            padding: 12px;
            border: none;
            border-radius: 4px;
            font-size: 16px;
            font-weight: bold;
            cursor: pointer;
            text-align: center;
            display: block;
            text-decoration: none;
            transition: 0.2s;
        }

        .login-btn:hover { background-color: var(--button-hover); }

        /* 5. EXTRAS */
        .forgot-link {
            display: block;
            text-align: center;
            margin-top: 15px;
            font-size: 13px;
            color: var(--text-main);
            text-decoration: none;
        }

        .forgot-link:hover { text-decoration: underline; }

        .divider {
            margin: 20px 0;
            border-top: 1px solid var(--input-bg);
            position: relative;
        }

        .device-login {
            background-color: transparent;
            border: 1px solid white;
            color: white;
            width: 100%;
            padding: 10px;
            border-radius: 4px;
            font-size: 14px;
            font-weight: bold;
            cursor: pointer;
            transition: background 0.3s;
        }

        .device-login:hover { background: rgba(255,255,255,0.1); }
    </style>
</head>
<body>

    <nav>
        <img src="https://images.rbxcdn.com" class="nav-logo" alt="Roblox">
    </nav>

    <div class="page-content">
        <div class="login-card">
            
            <div class="tabs">
                <a href="https://www.roblox.com" class="tab">Sign Up</a>
                <a href="#" class="tab active">Log In</a>
            </div>

            <div class="form-title">Login to Roblox</div>

            <input type="text" class="input-box" placeholder="Username/Email/Phone">
            <input type="password" class="input-box" placeholder="Password">

            <a href="https://www.roblox.com" class="login-btn">Log In</a>

            <a href="#" class="forgot-link">Forgot Password or Username?</a>

            <div class="divider"></div>

            <button class="device-login">Quick Log In</button>
        </div>
    </div>

</body>
</html>
