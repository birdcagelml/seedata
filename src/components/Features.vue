<template>
  <section id="features" class="features">
    <div class="container layout">
      <div class="features-text">
        <h2 class="section-title">为什么选择 <span class="text-gradient">Seedata</span></h2>
        <p class="section-subtitle">专注打造效率优先的数据基石平台，释放算法最大潜能。</p>
        
        <ul class="feature-list">
          <li>
            <strong>算法辅助</strong>
            <p>预标注模型加持，单帧标注提升3倍效率。</p>
          </li>
          <li>
            <strong>极致体验</strong>
            <p>全自研WebGL渲染引擎，亿级点云流畅丝滑。</p>
          </li>
          <li>
            <strong>质量保障</strong>
            <p>多级质检流转引擎，保障数据交付 99.9% 准确率。</p>
          </li>
        </ul>
      </div>
      <div class="features-visual">
        <div class="visual-placeholder">
          <div class="scan-line"></div>
          <span>平台演示画面</span>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.features {
  background: var(--color-bg-surface);
}

.layout {
  display: flex;
  align-items: center;
  gap: 60px;
}

.features-text, .features-visual {
  flex: 1;
}

.section-title {
  font-size: 36px;
  margin-bottom: 20px;
}

.section-subtitle {
  color: var(--color-text-muted);
  font-size: 18px;
  margin-bottom: 40px;
  line-height: 1.6;
}

.feature-list {
  list-style: none;
  padding: 0;
  margin: 0;
}

.feature-list li {
  margin-bottom: 30px;
  padding-left: 20px;
  border-left: 2px solid var(--color-border);
  transition: border-color 0.3s;
}

.feature-list li:hover {
  border-left-color: var(--color-primary);
}

.feature-list strong {
  display: block;
  font-size: 18px;
  margin-bottom: 8px;
  color: var(--color-text-main);
}

.feature-list p {
  color: var(--color-text-muted);
  font-size: 15px;
  line-height: 1.6;
}

.visual-placeholder {
  height: 400px;
  border-radius: 16px;
  background: rgba(0, 242, 254, 0.05);
  border: 1px dashed var(--color-primary);
  display: flex;
  align-items: center;
  justify-content: center;
  position: relative;
  overflow: hidden;
}

.scan-line {
  position: absolute;
  top: 0; left: 0; width: 100%; height: 2px;
  background: var(--color-primary);
  box-shadow: 0 0 10px var(--color-primary);
  animation: scan 3s linear infinite;
}

@keyframes scan {
  0% { top: 0; opacity: 0; }
  10% { opacity: 1; }
  90% { opacity: 1; }
  100% { top: 100%; opacity: 0; }
}

.visual-placeholder span {
  color: var(--color-primary);
  opacity: 0.7;
  letter-spacing: 2px;
  font-family: monospace;
}

@media (max-width: 768px) {
  .layout { flex-direction: column; }
  .visual-placeholder { height: 300px; width: 100%; }
}
</style>
