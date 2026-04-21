<template>
  <section id="home" class="hero">
    <div class="container hero-content">
      <h1 class="title">
        重塑数据价值<br />
        致力 <span class="text-gradient">效率优先</span> 的标注平台
      </h1>
      <p class="subtitle">
        Seedata为您提供卓越的数据标注设施，涵括2D/3D点云、文本标注与具身智能视频标注，赋能AI前沿探索。
      </p>
      <div class="hero-actions">
        <button class="glow-btn">免费开始</button>
        <button class="outline-btn">了解更多</button>
      </div>
    </div>
    <!-- 装饰球 -->
    <div class="glow-orb orb-1"></div>
    <div class="glow-orb orb-2"></div>
  </section>
</template>

<style scoped>
.hero {
  min-height: 100vh;
  display: flex;
  align-items: center;
  position: relative;
  overflow: hidden;
  padding-top: var(--nav-height);
}

.hero-content {
  position: relative;
  z-index: 10;
  text-align: center;
  max-width: 800px;
}

.title {
  font-size: 64px;
  line-height: 1.2;
  margin-bottom: 24px;
  letter-spacing: -1px;
}

.subtitle {
  font-size: 20px;
  color: var(--color-text-muted);
  line-height: 1.6;
  margin-bottom: 40px;
}

.hero-actions {
  display: flex;
  gap: 20px;
  justify-content: center;
}

.outline-btn {
  background: transparent;
  color: var(--color-text-main);
  border: 1px solid var(--color-border);
  border-radius: 8px;
  padding: 12px 28px;
  font-size: 16px;
  font-weight: 600;
  cursor: pointer;
  transition: all 0.3s ease;
}

.outline-btn:hover {
  border-color: var(--color-primary);
  color: var(--color-primary);
}

.glow-orb {
  position: absolute;
  border-radius: 50%;
  filter: blur(100px);
  z-index: 1;
  opacity: 0.3;
}

.orb-1 {
  width: 400px;
  height: 400px;
  background: var(--color-primary);
  top: 10%;
  left: -100px;
}

.orb-2 {
  width: 300px;
  height: 300px;
  background: var(--color-secondary);
  bottom: 10%;
  right: -50px;
}

@media (max-width: 768px) {
  .title { font-size: 42px; }
  .subtitle { font-size: 16px; }
}
</style>
