<template>
  <header class="header">
    <nav class="nav">
      <a href="/">
        <img src="@/assets/images/logo.png" class="logo" />
      </a>

      <ul class="menu">
        <li><RouterLink to="/">Home</RouterLink></li>
        <li><RouterLink to="/about">About</RouterLink></li>
        <li><RouterLink to="/work">Work</RouterLink></li>
        <li><RouterLink to="/contact">Contact</RouterLink></li>
      </ul>
    </nav>

    <div class="intro">My name is Cole Brown<br />and I <span>design & code</span> websites!</div>
  </header>
</template>

<style>
@import '@/assets/base.css';

header {
  background: var(--brand-blue) url('@/assets/images/background.jpg') 50% 10% no-repeat;
  padding: 0 0 3em;
}

.nav {
  background: rgba(255, 255, 255, 0.6);
  margin: 0 0 3em;
  padding: 1em;
  width: 100%;
}

.logo {
  box-shadow: 0 3px 5px rgba(0, 0, 0, 0.3);
  border-radius: 50%;
  display: block;
  margin: -1em 0 -4em;
  height: auto;
  width: 100px;
}

.intro {
  font-size: 30px;
  line-height: 1.2;
}

.menu {
  list-style: none;
  margin: 0;
  padding: 0;
}

/* existing */
nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
}

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }

  nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;

    padding: 1rem 0;
    margin-top: 1rem;
  }
}
</style>
