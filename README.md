<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Método Moreira 50</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: "Poppins", sans-serif;
    }

    body {
      background: linear-gradient(135deg, #001f3f, #003366);
      color: white;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      min-height: 100vh;
      text-align: center;
    }

    .login-box {
      background: rgba(255, 255, 255, 0.08);
      padding: 30px;
      border-radius: 20px;
      backdrop-filter: blur(10px);
      box-shadow: 0 0 20px rgba(0, 0, 0, 0.4);
      width: 90%;
      max-width: 400px;
    }

    h1 {
      color: #00bfff;
      margin-bottom: 15px;
    }

    input {
      width: 100%;
      padding: 12px;
      border: none;
      outline: none;
      border-radius: 8px;
      margin-top: 10px;
      font-size: 1rem;
    }

    button {
      margin-top: 15px;
      width: 100%;
      padding: 12px;
      border: none;
      border-radius: 8px;
      background: #00bfff;
      color: white;
      font-weight: 600;
      font-size: 1rem;
      cursor: pointer;
      transition: 0.3s;
    }

    button:hover {
      background: #0094cc;
      transform: scale(1.03);
    }

    #errorMsg {
      color: red;
      margin-top: 10px;
      display: none;
    }
  </style>
</head>
<body>
  <div class="login-box" id="loginBox">
    <h1>Método Moreira 50</h1>
    <p>Digite o login e a senha para acessar:</p>
    <input type="text" id="loginInput" placeholder="Login">
    <input type="password" id="passwordInput" placeholder="Senha">
    <button onclick="checkLogin()">Entrar</button>
    <p id="errorMsg">Login ou senha incorretos.</p>
  </div>

  <script>
    function checkLogin() {
      const login = document.getElementById('loginInput').value;
      const senha = document.getElementById('passwordInput').value;
      const loginCorreto = "Moreira";
      const senhaCorreta = "155";
      const errorMsg = document.getElementById('errorMsg');

      if (login === loginCorreto && senha === senhaCorreta) {
        // Redireciona para o link do Roblox
        window.location.href = "https://www.roblox.com/share?code=d0ba0ef251580e48a41fa820625296d3&type=Server";
      } else {
        errorMsg.style.display = 'block';
      }
    }
  </script>
</body>
</html>
