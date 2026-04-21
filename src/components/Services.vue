<template>
  <section id="services" class="services">
    <div class="container">
      <div class="section-header">
        <h2 class="section-title">核心<span class="text-gradient">服务能力</span></h2>
        <p class="section-subtitle">满足多生态 AI 训练所需，高精高质</p>
      </div>
      <div class="service-grid">
        <div class="service-card">
          <div class="card-icon">🎯</div>
          <h3>2D/3D点云标注</h3>
          <p>持多传感器融合标注支持高精度3D点云目标检测、语义分割标注工具套件。</p>
        </div>
        <div class="service-card">
          <div class="card-icon">🤖</div>
          <h3>具身智能视频标注</h3>
          <p>针对视频流数据的目标追踪、行为识别，结合流式算法提升标注效率。</p>
        </div>
        <div class="service-card">
          <div class="card-icon">📝</div>
          <h3>文本标注</h3>
          <p>支持大模型RLHF意图识别、实体抽取等文本语义高质量对齐标注服务。</p>
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

.service-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 30px;
}

.service-card {
  background: var(--color-bg-surface);
  border: 1px solid var(--color-border);
  border-radius: 16px;
  padding: 40px 30px;
  transition: all 0.3s ease;
  position: relative;
  overflow: hidden;
}

.service-card::before {
  content: "";
  position: absolute;
  top: 0; left: 0; width: 100%; height: 2px;
  background: linear-gradient(90deg, var(--color-primary), var(--color-secondary));
  opacity: 0;
  transition: opacity 0.3s ease;
}

.service-card:hover {
  transform: translateY(-5px);
  border-color: rgba(0, 242, 254, 0.3);
  box-shadow: 0 10px 30px rgba(0, 242, 254, 0.05);
}

.service-card:hover::before {
  opacity: 1;
}

.card-icon {
  font-size: 40px;
  margin-bottom: 24px;
}

.service-card h3 {
  font-size: 20px;
  margin-bottom: 16px;
}

.service-card p {
  color: var(--color-text-muted);
  line-height: 1.6;
  font-size: 15px;
}
</style>
