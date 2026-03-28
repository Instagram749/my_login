<!DOCTYPE html>
<html lang="ja">
<head>
  <meta charset="UTF-8">
  <title>Login</title>

  <style>
    body {
      font-family: Arial;
      background-color: #fafafa;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
    }

    .box {
      background: white;
      padding: 40px;
      border: 1px solid #ddd;
      width: 300px;
      text-align: center;
    }

    input {
      width: 100%;
      padding: 10px;
      margin: 5px 0;
      border: 1px solid #ddd;
      background: #fafafa;
    }

    button {
      width: 100%;
      padding: 10px;
      background: #0095f6;
      color: white;
      border: none;
      margin-top: 10px;
    }

    .message {
      margin-top: 10px;
      color: red;
    }
  </style>
</head>

<body>

<div class="box">
  <h1>Instagram</h1>

  <input type="text" id="username" placeholder="ユーザーネーム">
  <input type="password" id="password" placeholder="パスワード">

  <button onclick="login()">ログイン</button>

  <div class="message" id="msg"></div>
</div>

<script>
function login() {
  const user = document.getElementById("username").value;
  const pass = document.getElementById("password").value;

  if(user === "test" && pass === "1234") {
    document.getElementById("msg").style.color = "green";
    document.getElementById("msg").innerText = "ログイン成功！";
  } else {
    document.getElementById("msg").innerText = "失敗";
  }
}
</script>

</body>
</html>
