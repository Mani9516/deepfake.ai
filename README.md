
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Login and Signup Page</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background:linear-gradient(271deg, #5e2275, #070b0f);
    }
  
    .container {
      max-width: 400px;
      margin: 100px auto;
      padding: 20px;
      background-color: #00000017;
      border-radius: 5px;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    }
  
    h2 {
      text-align: center;
    }
  
    input[type="text"],
    input[type="password"],
    input[type="submit"] {
      width: 100%;
      padding: 10px;
      margin: 8px 0;
      display: inline-block;
      border: 1px solid #ccc;
      border-radius: 20px;
      background-color: #2e2e2e00;
      box-sizing: border-box;
  }
    
  input[type="submit"] {
      background-color: #5f5f5f3b;
      color: white;
      border: none;
      width: 70px;
      margin-left: 170px;
      cursor: pointer;
  }
  
    input[type="submit"]:hover {
      background-color: #7c7c7c00;
    }
  
    .login-form,
    .signup-form {
      display: none;
    }
  
    .switch-btn {
      text-align: center;
      margin-top: 20px;
    }
  
    .switch-btn a {
      text-decoration: none;
      color: #000000;
      cursor: pointer;
    } 
     .button{
      background-color: #4ea9e2;
    color: white;
    padding: 14px 25px;
    text-align: center;
    text-decoration: none;
    display: inline-block;
  }
  
  a:hover, a:active {
    background-color: rgb(255, 255, 255);
  }
  
a.button {
  display: block;
  width: 100%;
  padding: 10px 15px;
  margin-top: 20px;
  text-align: center;
  font-size: 16px;
  font-weight: bold;
  color: #ffffff;
  background-color: #007bff;
  border: none;
  border-radius: 5px;
  cursor: pointer;
  text-decoration: none; /* Remove underline from the link */
  transition: background-color 0.3s ease;
}

a.button:hover {
  background-color: #0056b3;
}
  
  </style>
  </head>
  <body>
  
  <div class="container">
    <h2>Welcome</h2>
    <form id="login-form" class="login-form" action="login_process.php" method="POST">
      <input type="text" placeholder="Username" name="username" required="">
      <input type="password" placeholder="Password" name="password" required="">
      <a href="deep.html">Login</a>
    </form>
    <form id="signup-form" class="signup-form" style="display: none;">
      <input type="text" placeholder="Username" required="">
      <input type="password" placeholder="Password" required="">
      <input type="password" placeholder="Confirm Password" required="">
      <input type="submit" value="Sign Up">
      
    </form>
    
    <div class="switch-btn">
      <a href="#" onclick="toggleForm('login')">Login</a> | <a href="#" onclick="toggleForm('signup')">Sign Up</a>
    </div>
  </div>
  
  <script>
    function toggleForm(form) {
      var loginForm = document.getElementById('login-form');
      var signupForm = document.getElementById('signup-form');
      function signInWithGoogle() {
      }
      if (form === 'login') {
        loginForm.style.display = 'block';
        signupForm.style.display = 'none';
      } else {
        loginForm.style.display = 'none';
        signupForm.style.display = 'block';
      }
    }
  </script>
  <script>
    function toggleForm(form) {
      var loginForm = document.getElementById('login-form');
      var signupForm = document.getElementById('signup-form');
      function signInWithGoogle() {
      }
      if (form === 'login') {
        loginForm.style.display = 'block';
        signupForm.style.display = 'none';
      } else {
        loginForm.style.display = 'none';
        signupForm.style.display = 'block';
      }
    }
  </script>  
  </body>
</html>
