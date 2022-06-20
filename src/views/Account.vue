<template>
  <main>
    <div class="forms">
      <!-- Login-page -->
      <div class="login-form" v-if="$route.params.route == 'login'">
        <header>
          <h1>Login</h1>
        </header>
        <div class="form-container">
          <form @submit.prevent="login">
            <div class="email">
              <label for="">Email</label>
              <input type="email" placeholder="Email address" />
            </div>
            <div class="password">
              <label for="">Password</label>
              <input type="password" placeholder="Password" />
            </div>
            <input class="login-btn blue-btn" type="submit" value="Log In" />
          </form>
          <div class="create-account">
            <RouterLink to="/account/register">
              <p>Create Account</p>
            </RouterLink>
          </div>
        </div>
      </div>
      <!-- Sign-up Page -->
      <div class="signup-form" v-if="$route.params.route == 'register'">
        <header>
          <h1>CREATE ACCOUNT</h1>
        </header>
        <div class="form-container">
          <form @submit.prevent="register">
            <div class="first-name">
              <label for="">FIRST NAME</label>
              <input type="text" />
            </div>
            <div class="last-name">
              <label for="">LAST NAME</label>
              <input type="text" />
            </div>
            <div class="email">
              <label for="">Email</label>
              <input type="email" />
            </div>
            <div class="password">
              <label for="">Password</label>
              <input type="password" />
            </div>
            <input class="signup-btn" type="submit" value="CREATE" />
          </form>
          <div class="create-account">
            <RouterLink to="/account/login">
              <p>Login</p>
            </RouterLink>
          </div>
        </div>
      </div>
    </div>
    <!-- Profile Page -->
    <div class="profile" v-if="$route.params.route == 'profile'">
      <h2>WelcomeUser to profile page</h2>
    </div>
  </main>
</template>

<script>
export default {};
</script>

<style>
.forms {
    margin-top: 50px;
}
.login-form,
.signup-form {
  max-width: 350px;
  margin: 0 auto;
}
header {
  text-align: center;
}
header h1 {
  font-size: 22px;
  font-weight: 700;
}
form label {
  display: block;
  font-size: 20px;
  margin-bottom: 10px;
}
form input {
  display: block;
  width: 100%;
  padding: 8px 10px;
  margin-bottom: 20px;
  font-size: 18px;
}
.login-btn {
  background: #111111;
  border: 1px solid #111111;
  cursor: pointer;
  color: #fff;
}
.create-account {
  text-align: center;
}
.create-account p {
  color: var(--text-color);
}
.signup-btn {
  background: #fff;
  border: 1px solid #111111;
  cursor: pointer;
  color: var(--text-color);
  margin: 25px 0 !important;
}
.signup-form input {
  margin-bottom: 6px;
}
</style>
