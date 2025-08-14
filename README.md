# demo12
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Login - Finance Tracker</title>
  <link rel="stylesheet" href="login.css">
  <script src="https://accounts.google.com/gsi/client" async defer></script> <!-- Google Sign-In -->
</head>
<body>
  <div class="login-container">
    <h1>Finance Tracker</h1>

    <form id="loginForm">
      <div class="input-group">
        <label for="email">Email Address</label>
        <input type="email" id="email" required placeholder="you@example.com">
      </div>
      <div class="input-group">
        <label for="password">Password</label>
        <input type="password" id="password" required placeholder="Enter your password">
      </div>
      <button type="submit" class="login-btn">Login</button>
    </form>

    <div class="divider">or</div>

    <!-- Google Sign-In Button -->
    <div id="g_id_onload"
      data-client_id="YOUR_GOOGLE_CLIENT_ID"
      data-login_uri="YOUR_BACKEND_LOGIN_HANDLER"
      data-auto_prompt="false">
    </div>
    <div class="g_id_signin"
      data-type="standard"
      data-size="large"
      data-theme="outline"
      data-text="sign_in_with"
      data-shape="rectangular"
      data-logo_alignment="left">
    </div>

    <p class="signup-link">Don't have an account? <a href="#">Sign up</a></p>
  </div>

  <script src="login.js"></script>
</body>
</html>
