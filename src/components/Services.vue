<script setup>
</script>
<template>
  <section id="services" class="services">
    <div class="container">
      <div class="section-header">
        <h2 class="section-title">为什么选择 <span class="text-gradient">Seedata</span></h2>
      </div>
      <div class="service-list">
        <div class="service-row">
          <div class="row-content">
            <h3>精准标注</h3>
            <p>支持图像、文本、音频、视频多模态标注<br/>行业平均准确率高达99.3%</p>
          </div>
          <div class="row-media">
            <video src="/video/1.mp4" poster="/video/poster_1.png" autoplay loop muted playsinline></video>
          </div>
        </div>
        <div class="service-row reverse">
          <div class="row-content">
            <h3>高效交付</h3>
            <p>智能辅助标注工具 + 专业标注团队<br/>交付周期缩短60%</p>
          </div>
          <div class="row-media">
            <video src="/video/2.mp4" poster="/video/poster_2.png" autoplay loop muted playsinline></video>
          </div>
        </div>
        <div class="service-row">
          <div class="row-content">
            <h3>数据安全，架构先行</h3>
            <!-- <p class="subtitle">--为数据提供全生命周期的安全防护。</p> -->
            <ul class="feature-list">
              <li><span class="hl-dot"></span>支持完全私有化部署</li>
              <li><span class="hl-dot"></span>动态防泄密技术，全层级指纹留证</li>
              <li><span class="hl-dot"></span>高防数据专线，物理级链路保障，确保数据传输无忧</li>
            </ul>
          </div>
          <div class="row-media">
            <img src="/SECURITY.png" alt="数据安全" />
          </div>
        </div>
        <div class="service-row reverse">
          <div class="row-content">
            <h3>智能工具</h3>
            <p>AI辅助预标注，人工审核复验<br/>标注效率提升3倍</p>
          </div>
          <div class="row-media">
            <video src="/video/4.mp4" poster="/video/poster_4.jpg" autoplay loop muted playsinline></video>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
<style scoped>
.section-header {
  text-align: center;
  margin-bottom: 60px;
}
.section-title {
  font-size: 36px;
  margin-bottom: 16px;
}
.section-subtitle {
  color: var(--color-text-muted);
  font-size: 18px;
}

.services {
  padding: 100px 0;
}
.section-header {
  text-align: center;
  margin-bottom: 80px;
}
.section-title {
  font-size: 36px;
  margin-bottom: 16px;
}
.section-subtitle {
  color: var(--color-text-muted);
  font-size: 18px;
}
.service-list {
  display: flex;
  flex-direction: column;
  gap: 100px;
}
.service-row {
  display: flex;
  align-items: center;
  gap: 60px;
}
.service-row.reverse {
  flex-direction: row-reverse;
}
.row-content {
  flex: 1;
}
.row-content h3 {
  font-size: 36px;
  margin-bottom: 24px;
  color: var(--color-text-main);
  position: relative;
  display: inline-block;
  padding-bottom: 12px;
}

.row-content h3::after {
  content: "";
  position: absolute;
  left: 0;
  bottom: 0;
  width: 50px;
  height: 6px;
  background: linear-gradient(90deg, var(--color-primary), var(--color-secondary));
  border-radius: 3px;
}
.row-content p {
  color: var(--color-text-muted);
  line-height: 1.8;
  font-size: 18px;
}
.row-content p.subtitle {
  margin-top: -12px;
  margin-bottom: 24px;
  color: var(--color-primary);
  font-weight: 500;
  font-size: 16px;
  opacity: 0.8;
}
.feature-list {
  list-style: none;
  padding: 0;
  margin: 0;
}
.feature-list li {
  color: var(--color-text-muted);
  font-size: 16px;
  line-height: 1.6;
  margin-bottom: 12px;
  display: flex;
  align-items: center;
}
.hl-dot {
  display: inline-block;
  width: 8px;
  height: 8px;
  background: var(--color-secondary);
  border-radius: 50%;
  box-shadow: 0 0 8px var(--color-secondary);
  margin-right: 12px;
  flex-shrink: 0;
}
.row-media {
  flex: 1.2;
  border-radius: 20px;
  overflow: hidden;
  position: relative;
  box-shadow: 0 20px 40px rgba(0, 0, 0, 0.1);
  border: 1px solid var(--color-border);
  min-height: 280px;
  background: rgba(0, 0, 0, 0.05); /* 添加背景以防止视频未加载时完全不可见 */
}
.row-media::after {
  content: "";
  position: absolute;
  top: 0; left: 0; width: 100%; height: 100%;
  box-shadow: inset 0 0 20px rgba(0, 242, 254, 0.2);
  pointer-events: none;
}
.row-media video,
.row-media img {
  width: 100%;
  display: block;
  object-fit: cover;
  opacity: 0.9;
  transition: opacity 0.5s ease, transform 0.8s ease;
}
.service-row:hover .row-media video,
.service-row:hover .row-media img {
  opacity: 1;
  transform: scale(1.02);
}
@media (max-width: 992px) {
  .service-row, .service-row.reverse {
    flex-direction: column;
    gap: 40px;
  }
  .row-media {
    width: 100%;
  }
}
</style>
