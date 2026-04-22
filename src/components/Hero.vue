<template>
  <section id="home" class="hero">
    <!-- 视频背景 (动态绑定src可以跳过Vite在编译时的import检查) -->
    <video class="hero-bg-video" :src="'/video/section1.mp4'" autoplay loop muted playsinline></video>
    <div class="hero-overlay"></div>

    <div class="container hero-content">
      <h1 class="title">
        种下数据，生长智能
      </h1>
      <p class="subtitle">
        Seedata 智数起源 — 为AI产品提供高质量数据标注解决方案<br />
        伟大的AI，始于一份精准的数据
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

.hero-bg-video {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  object-fit: cover;
  z-index: 0;
  transform: scale(1.1); /* 整体放大10%，把右下角的水印挤出屏幕外 */
  transform-origin: center center;
}

.hero-overlay {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: rgba(0, 0, 0, 0.3); /* 改为亮色玻璃质感遮罩，适配亮色科技风格 */
  backdrop-filter: blur(2px);
  -webkit-backdrop-filter: blur(2px);
  z-index: 1;
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
  color: var(--color-bg-surface);
}

.subtitle {
  font-size: 20px;
  color: var(--color-bg-surface);
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
  color: var(--color-bg-surface);
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
  z-index: 2; /* 调高z-index，置于视频遮罩之上 */
  opacity: 0.4;
  animation: pulse-glow 8s infinite alternate ease-in-out;
}

.orb-1 {
  width: 450px;
  height: 450px;
  background: #00ff88;
  top: 10%;
  left: -100px;
  animation-delay: 0s;
}

.orb-2 {
  width: 350px;
  height: 350px;
  background: #00f2fe;
  bottom: 15%;
  right: -50px;
  animation-delay: 4s;
}

@keyframes pulse-glow {
  0% { transform: scale(1) translate(0, 0); opacity: 0.3; }
  100% { transform: scale(1.1) translate(20px, -20px); opacity: 0.6; filter: blur(120px); }
}
@media (max-width: 768px) {
  .title { font-size: 42px; }
  .subtitle { font-size: 16px; }
}
</style>
