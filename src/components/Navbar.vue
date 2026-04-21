<template>
  <header class="navbar">
    <div class="container nav-content">
      <div class="logo">
        <img src="/logo-website.png" alt="Seedata Logo" class="logo-img" />
        <span class="logo-text">See<span class="text-gradient">data</span></span>
      </div>
      <nav class="nav-links">
        <a href="#home">首页</a>
        <a href="#services">核心服务</a>
        <a href="#features">平台优势</a>
      </nav>
      <div class="nav-actions">
        <button class="glow-btn">立即体验</button>
      </div>
    </div>
  </header>
</template>

<script setup>
</script>

<style scoped>
.navbar {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: var(--nav-height);
  background: rgba(7, 9, 17, 0.7);
  backdrop-filter: blur(10px);
  -webkit-backdrop-filter: blur(10px);
  border-bottom: 1px solid var(--color-border);
  z-index: 100;
  display: flex;
  align-items: center;
}

.nav-content {
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex: 1;
}

.logo {
  display: flex;
  align-items: center;
  gap: 10px;
  font-size: 24px;
  font-weight: 800;
  letter-spacing: 1px;
}

.logo-img {
  height: 32px;
  width: auto;
}

.nav-links {
  display: flex;
  gap: 30px;
}

.nav-links a {
  font-size: 15px;
  color: var(--color-text-main);
  transition: color 0.3s ease;
  font-weight: 500;
}

.nav-links a:hover {
  color: var(--color-primary);
}

@media (max-width: 768px) {
  .nav-links {
    display: none;
  }
}
</style>
