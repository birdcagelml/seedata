<template>
  <section id="home" class="hero">
    <!-- 视频背景 (动态绑定src可以跳过Vite在编译时的import检查) -->
    <video class="hero-bg-video" :src="'/video/section1.mp4'" poster="/video/poster_section1.jpg" autoplay loop muted playsinline></video>
    <div class="hero-overlay"></div>

    <div class="container hero-content">
      <div class="subtitle-badge">Seedata 智数起源</div>
      <h1 class="title">
        种下数据，长出智能
      </h1>
      <div class="title-divider"></div>
      <p class="subtitle">
        科技驱动的高质量 AI 数据与标注服务商
      </p>
    </div>
    <!-- 装饰球 -->
    <div class="glow-orb orb-1"></div>
    <div class="glow-orb orb-2"></div>
  </section>
</template>

<style scoped>
.hero {
  min-height: 65vh;
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
  text-align: left;
  max-width: 800px;
}

.subtitle-badge {
  position: relative;
  display: inline-block;
  padding: 8px 20px;
  color: #00f2fe;
  font-size: 14px;
  font-weight: 600;
  margin-bottom: 30px;
  background: rgba(0, 242, 254, 0.05);
  border: 1px dashed rgba(0, 242, 254, 0.6);
}

.subtitle-badge::before {
  content: "";
  position: absolute;
  top: -4px;
  left: -4px;
  right: -4px;
  bottom: -4px;
  pointer-events: none;
  background: 
    linear-gradient(#00f2fe, #00f2fe) top left / 6px 6px no-repeat,
    linear-gradient(#00f2fe, #00f2fe) top right / 6px 6px no-repeat,
    linear-gradient(#00f2fe, #00f2fe) bottom left / 6px 6px no-repeat,
    linear-gradient(#00f2fe, #00f2fe) bottom right / 6px 6px no-repeat;
}

.title-divider {
  width: 60px;
  height: 4px;
  background: linear-gradient(90deg, #00f2fe, #0055ff);
  border-radius: 2px;
  margin-bottom: 24px;
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
  margin-bottom: 20px;
  opacity: 0.9;
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
