<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Dashboard</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #eef2f7;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      height: 100vh;
    }
    .dashboard {
      background: white;
      padding: 2rem;
      border-radius: 10px;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
      text-align: center;
    }
    h1 {
      color: #333;
    }
    button {
      margin-top: 1rem;
      padding: 10px 20px;
      border: none;
      background: #007bff;
      color: white;
      border-radius: 5px;
      cursor: pointer;
    }
    button:hover {
      background: #0056b3;
    }
  </style>
</head>
<body>
  <div class="dashboard">
    <h1>Welcome to your Dashboard!</h1>
    <p>You have successfully logged in.</p>
    <button onclick="logout()">Logout</button>
  </div>

  <script>
    function logout() {
      window.location.href = "login.html";
    }
  </script>
</body>
</html>
