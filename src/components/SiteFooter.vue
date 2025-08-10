<template>
  <footer class="footer">
    <div class="brand">
      <span>Take</span>Flight
      <small>© 2004 - 2015</small>
    </div>
  </footer>
</template>

<style>
footer {
  background: #ccc url('@/assets/images/background.jpg') 50% 100% no-repeat;
  background-size: cover;
  padding: 4em 1em 1em;
}

.brand {
  font-size: 20px;
  line-height: 24px;
  text-align: right;
  width: 100%;
  color: var(--text-color);
  text-transform: uppercase;
}

.brand span {
  color: rgba(255, 255, 255, 0.8);
}
</style>
