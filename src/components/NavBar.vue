<template>
  <div class="nav-bar-section">
    <img src="/public/images/Vector.png" class="nav-clipper" />
    <div class="logo-design">
      <img src="/public/images/logo.svg" alt="logo" />
      <p>Houter</p>
    </div>
    <div class="nav-list">
      <ul>
        <li>About Us</li>
        <li>Article</li>
        <li>Property</li>
      </ul>
      <button class="btn-light">Sign up!</button>
    </div>
  </div>
</template>

<script>
export default {
  name: 'NavBar.vue'
}
</script>

<style scoped>
.nav-bar-section {
  height: 50px;
  padding: 9px 7rem 0;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.logo-design {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 12px;
}

.nav-clipper {
  z-index: -10;
  position: absolute;
  transform: translateY(35%) translateX(-40%);
}
.logo-design p {
  font-size: 16px;
  font-weight: 700;
}
.nav-list {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 25px;
}

.nav-list li {
  display: inline;
  color: red;
  padding: 8px 16px;
  margin: 0 10px;
  background: green;
  outline: 1px solid #fff;
  background: transparent;
  color: #fff;
  border-radius: 32px;
  list-style: none;
  /* font-size: 1.3vw; */
  font-size: (90%, 1.3rem);
}

.nav-list li:hover {
  background: var(--deep-color);
  opacity: 0.7;
}

.btn-light {
  border-radius: 32px;
  font-size: 1rem;
  font-weight: 600;
  color: var(--par-color);
  background: #d1fae5;
  padding: 12px 24px;
  border: none;
}
.btn-light:hover {
  background: var(--deep-color);
  color: #fff;
}
</style>
