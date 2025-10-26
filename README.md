<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Login Page</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #f0f2f5;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
    }
    .login-container {
      background: white;
      padding: 2rem;
      border-radius: 10px;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
      width: 300px;
    }
    h2 {
      text-align: center;
      margin-bottom: 1.5rem;
    }
    input {
      width: 100%;
      padding: 10px;
      margin: 0.5rem 0;
      border: 1px solid #ccc;
      border-radius: 5px;
    }
    button {
      width: 100%;
      padding: 10px;
      background: #007bff;
      border: none;
      color: white;
      border-radius: 5px;
      cursor: pointer;
    }
    button:hover {
      background: #0056b3;
    }
    .error {
      color: red;
      font-size: 0.9rem;
      text-align: center;
    }
  </style>
</head>
<body>
  <div class="login-container">
    <h2>Login</h2>
    <div class="error" id="error"></div>
    <input type="text" id="username" placeholder="Username" required />
    <input type="password" id="password" placeholder="Password" required />
    <button onclick="login()">Login</button>
  </div>

  <script>
    function login() {
      const username = document.getElementById('username').value.trim();
      const password = document.getElementById('password').value.trim();
      const error = document.getElementById('error');

      // Example: Hardcoded credentials
      const validUser = "admin";
      const validPass = "1234";

      if (username === validUser && password === validPass) {
        // Redirect to dashboard
        window.location.href = "dashboard.html";
      } else {
        error.textContent = "Invalid username or password!";
      }
    }
  </script>
</body>
</html>