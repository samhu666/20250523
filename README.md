<!DOCTYPE html>
<html lang="zh">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>登入頁面</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f9;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }
        .login-form {
            background: white;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            width: 300px;
        }
        .form-group {
            margin-bottom: 15px;
        }
        label {
            display: block;
            margin-bottom: 5px;
            font-weight: bold;
        }
        input[type="email"], input[type="password"] {
            width: 100%;
            padding: 8px;
            border: 1px solid #ccc;
            border-radius: 4px;
        }
        .checkbox-group {
            display: flex;
            align-items: center;
            margin-bottom: 15px;
        }
        button {
            background-color: #007BFF;
            color: white;
            border: none;
            padding: 10px 15px;
            border-radius: 4px;
            cursor: pointer;
            width: 100%;
        }
        button:hover {
            background-color: #0056b3;
        }
        .links {
            margin-top: 10px;
            text-align: center;
        }
        .links a {
            color: #007BFF;
            text-decoration: none;
        }
    </style>
</head>
<body>
    <div class="login-form">
        <h2>登入</h2>
        <form action="/login" method="POST">
            <div class="form-group">
                <label for="email">電子郵件</label>
                <input type="email" id="email" name="email" placeholder="輸入您的電子郵件" required>
            </div>
            <div class="form-group">
                <label for="password">密碼</label>
                <input type="password" id="password" name="password" placeholder="輸入您的密碼" required>
            </div>
            <div class="checkbox-group">
                <input type="checkbox" id="remember" name="remember">
                <label for="remember">記住我</label>
            </div>
            <button type="submit">立即登入</button>
            <div class="links">
                <a href="/forgot-password">忘記密碼？</a>
                <span> | </span>
                <a href="/signup">註冊帳號</a>
            </div>
        </form>
    </div>
</body>
</html>
