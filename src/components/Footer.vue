<template>
  <footer class="footer">
    <div class="container">
      <div class="footer-bottom">
        <div class="logo">
          <img src="/logo-website.png" alt="Seedata Logo" class="logo-img" />
        </div>
        <p>&copy; 2026 Seedata Inc. 保留所有权利. 效率优先的标注基建平台。</p>
      </div>
    </div>
  </footer>
</template>

<style scoped>
.footer {
  border-top: 1px solid var(--color-border);
  padding: 40px 0;
  background: var(--color-bg-dark);
}

.footer-bottom {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.logo {
  display: flex;
  align-items: center;
  font-size: 20px;
  font-weight: 800;
}

.logo-img {
  height: 40px;
  width: auto;
}

p {
  color: var(--color-text-muted);
  font-size: 14px;
}

@media (max-width: 768px) {
  .footer-bottom {
    flex-direction: column;
    gap: 16px;
    text-align: center;
  }
}
</style>
