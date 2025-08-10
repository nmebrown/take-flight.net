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
  background-size: cover;
  padding: 0 0 3em;
}

.nav {
  background: rgba(255, 255, 255, 0.6);
  display: grid;
  grid-template-columns: 1fr 100px auto 1fr;
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

.menu {
  grid-column: 3;
  display: flex;
  grid-gap: 20px;
  list-style: none;
  margin: 0;
  padding: 0;
}

.menu a {
  color: var(--brand-blue);
  font-weight: 600;
  text-decoration: none;
  text-transform: uppercase;
}

.menu a.router-link-exact-active {
  color: var(--color-text);
}

.menu a.router-link-exact-active:hover {
  background-color: transparent;
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
  #header {
    padding: 0 0 4em;

    .top-bar {
      margin: 0 0 4em;
      padding: 1em 0;

      .logo {
        float: left;
        margin: 0 0 -72px;
      }
    }
  }

  .menu {
    ul {
      li {
        a {
          background: rgba(255, 255, 255, 0.5);
          border-radius: 1px;
          display: block;
          margin: 0;
          padding: 0.5em 1em;

          &:hover {
            background: #fff;
            transition: background 0.5s;
          }
        }
      }
    }
  }
}
</style>
