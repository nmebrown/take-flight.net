<template>
  <header class="header">
    <div class="top-bar">
      <nav class="nav container">
        <a href="/" class="home-link">
          <img src="@/assets/images/logo.png" class="logo" />
        </a>

        <ul class="main-menu">
          <li><RouterLink to="/">Home</RouterLink></li>
          <li><RouterLink to="/about">About</RouterLink></li>
          <li><RouterLink to="/work">Work</RouterLink></li>
          <li><RouterLink to="/contact">Contact</RouterLink></li>
        </ul>
      </nav>
    </div>

    <div class="container intro">
      My name is Cole Brown<br />and I <span>design & code</span> websites!
    </div>
  </header>
</template>

<style>
@import '@/assets/base.css';

header {
  background: var(--brand-blue) url('@/assets/images/background.jpg') 50% 10% no-repeat;
  background-size: cover;
  padding: 0 0 3em;
}

.top-bar {
  background: rgba(255, 255, 255, 0.6);
  margin: 0 0 3em;
  padding: 1em;
  width: 100%;
}

.nav {
  display: flex;
  justify-content: center;
  margin: 0 auto;
}

.logo {
  box-shadow: 0 3px 5px rgba(0, 0, 0, 0.3);
  border-radius: 50%;
  display: block;
  margin: -1em 0 -4em;
  height: auto;
  width: 100px;
}

.main-menu {
  display: flex;
  grid-gap: 20px;
  list-style: none;
  margin: 0;
  margin-left: auto;
  padding: 0;
}

.main-menu a {
  color: var(--brand-blue);
  font-weight: 600;
  text-decoration: none;
  text-transform: uppercase;

  background: rgba(255, 255, 255, 0.5);
  border: 0;
  display: block;
  margin: 0;
  padding: 0.5em 1em;
  transition: all ease 0.2s;
}

.main-menu a:hover {
  background: #fff;
  border: 0;
}

.main-menu a.router-link-exact-active {
  color: var(--color-text);
}

.intro {
  border: 0;
  color: var(--brand-dkblue);
  font-family: var(--brand-header-font);
  font-size: 30px;
  line-height: 1.2;
  margin: 0;
  text-align: center;
  text-shadow: 0 1px 1px rgba(255, 255, 255, 0.6);
}

@media (min-width: 1024px) {
  header {
    padding: 0 0 4em;
  }

  .top-bar {
    margin: 0 0 4em;
  }

  .intro {
    font-size: 42px;
  }
}
</style>
