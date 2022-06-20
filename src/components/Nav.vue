<template>
  <nav>
    <div class="nav-inner">
      <div class="nav-content">
        <RouterLink to="/">
          <div class="logo">
            <h2>SHIIRO</h2>
          </div>
        </RouterLink>

        <div class="links-container">
          <ul class="nav-links">
            <li class="link link_drop">
              CLOTHING
              <ul class="drop-down">
                <RouterLink to="/store/shirts">
                  <li class="link">SHIRTS</li>
                </RouterLink>
                <RouterLink to="/store/trouser">
                  <li class="link">TROUSER</li>
                </RouterLink>
                <RouterLink to="/store/vest">
                  <li class="link">VEST</li>
                </RouterLink>
                <RouterLink to="/store/jacket">
                  <li class="link">JACKET</li>
                </RouterLink>
                <RouterLink to="/store/hoodie">
                  <li class="link">HOODIE</li>
                </RouterLink>
              </ul>
            </li>
            <li class="link link_drop">
              ACCESSORIES
              <ul class="drop-down">
                <RouterLink to="/store/accessories">
                  <li class="link">ALL</li>
                </RouterLink>
                <RouterLink to="/store/belt">
                  <li class="link">BELT</li>
                </RouterLink>
                <RouterLink to="/store/mask">
                  <li class="link">MASK</li>
                </RouterLink>
                <RouterLink to="/store/gloves">
                  <li class="link">GLOVES</li>
                </RouterLink>
              </ul>
            </li>
            <RouterLink to="/store/footwear">
              <li class="link">FOOTWEAR</li>
            </RouterLink>
            <li class="link link_drop">
              HEADWEAR
              <ul class="drop-down">
                <RouterLink to="/store/headwear">
                  
                <li class="link">ALL</li>
                </RouterLink>
                <RouterLink to="/store/caps">
                  
                <li class="link">CAPS</li>
                </RouterLink>
                <RouterLink to="/store/beanies">
                  
                <li class="link">BEANIES</li>
                </RouterLink>
                <RouterLink to="/store/hats">
                  
                <li class="link">HATS</li>
                </RouterLink>
              </ul>
            </li>
          </ul>
        </div>
        <div class="nav-icons">
          <span class="search-icon icon-container">
            <svg class="icon search" viewBox="0 0 48 48">
              <path
                d="M 21 3 C 11.601563 3 4 10.601563 4 20 C 4 29.398438 11.601563 37 21 37 C 24.355469 37 27.460938 36.015625 30.09375 34.34375 L 42.375 46.625 L 46.625 42.375 L 34.5 30.28125 C 36.679688 27.421875 38 23.878906 38 20 C 38 10.601563 30.398438 3 21 3 Z M 21 7 C 28.199219 7 34 12.800781 34 20 C 34 27.199219 28.199219 33 21 33 C 13.800781 33 8 27.199219 8 20 C 8 12.800781 13.800781 7 21 7 Z"
              ></path>
            </svg>
          </span>
          <RouterLink to="/account/login">
            <span class="profile-icon icon-container">
              <svg class="icon profile" viewBox="0 0 50 50">
                <path
                  d="M 25.875 3.40625 C 22.195313 3.472656 19.507813 4.570313 17.875 6.71875 C 15.941406 9.265625 15.589844 13.144531 16.8125 18.21875 C 16.363281 18.769531 16.023438 19.605469 16.15625 20.71875 C 16.417969 22.914063 17.296875 23.824219 18 24.1875 C 18.339844 25.921875 19.296875 27.863281 20.21875 28.78125 L 20.21875 29.25 C 20.222656 29.910156 20.210938 30.535156 20.1875 31.1875 C 20.710938 32.28125 22.371094 34 26 34 C 29.65625 34 31.359375 32.246094 31.84375 31.03125 C 31.824219 30.429688 31.839844 29.859375 31.84375 29.25 L 31.84375 28.78125 C 32.738281 27.867188 33.660156 25.921875 34 24.1875 C 34.722656 23.828125 35.578125 22.921875 35.84375 20.71875 C 35.976563 19.628906 35.65625 18.800781 35.21875 18.25 C 35.800781 16.269531 36.988281 11.113281 34.9375 7.8125 C 34.078125 6.429688 32.777344 5.558594 31.0625 5.21875 C 30.117188 4.027344 28.304688 3.40625 25.875 3.40625 Z M 32.75 33.34375 C 31.488281 34.800781 29.257813 36 26 36 C 22.683594 36 20.515625 34.78125 19.28125 33.375 C 18.328125 34.175781 16.804688 34.777344 15.125 35.4375 C 11.21875 36.972656 6.363281 38.871094 6 44.9375 L 5.9375 46 L 46.0625 46 L 46 44.9375 C 45.636719 38.871094 40.800781 36.972656 36.90625 35.4375 C 35.21875 34.769531 33.699219 34.15625 32.75 33.34375 Z"
                ></path>
              </svg>
            </span>
          </RouterLink>
        </div>
      </div>
    </div>
  </nav>
</template>

<script>
export default {};
</script>

<style scoped>
nav {
  background: var(--color-dark);
  padding: 20px 0;
  color: var(--color-light);
}
ul {
  list-style: none;
}
.nav-inner {
  max-width: 1450px;
  padding: 0 45px;
}
.nav-content {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.logo {
  font-family: "Cabin Sketch", sans-serif;
  font-size: 26px;
  color: var(--color-light);
}
.logo h2 {
  font-size: 26px;
  font-weight: 700;
}
.nav-links {
  display: flex;
  align-items: center;
}
.link {
  padding: 8px 15px;
  font-weight: 700;
  cursor: pointer;
  transition: all 0.3s ease;
  color: var(--color-light);
}
.link:hover {
  background: rgba(121, 120, 120, 0.889);
}
.link_drop {
  position: relative;
}
.link_drop:hover .drop-down {
  transform: translateZ(0);
  visibility: visible;
}
.drop-down {
  background: rgba(255, 255, 255, 0.929);
  text-align: left !important;
  display: block;
  min-width: 100%;
  margin: 0;
  padding: 10px 0 5px;
  position: absolute;
  left: 0;
  z-index: 5;
  transform: translateY(-12px);
  visibility: hidden;
  /* transition: all 0.12s cubic-bezier(0.2, 0.06, 0.05, 0.95); */
  transition: all 0.1s ease-in-out;
}
.drop-down .link {
  display: block;
  margin: 0;
  text-align: left;
  padding: 8px 15px;
  color: var(--text-color);
}

/* left icons */
.icon-container {
  padding: 7.5px;
}
.nav-icons .icon {
  color: var(--color-light);
  display: inline-block;
  width: 28px;
  height: 28px;
  vertical-align: middle;
  fill: currentColor;
  padding: 3px 3px 2px;
  cursor: pointer;
}


/* Media Query */
</style>
