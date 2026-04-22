<template>
  <section id="products" class="features">
    <div class="container">
      <div class="products-header">
        <h2 class="section-title">两大核心产品，覆盖数据标注全链路</h2>
        <p class="section-subtitle">无论您是AI企业采购方，还是专业标注服务团队<br/>Seedata 都为您提供最适配的解决方案</p>
      </div>
      
      <div class="product-showcase">
        <!-- 智标平台 -->
        <div class="product-row">
          <div class="product-content">
            <div class="product-title-wrap">
              <div class="product-icon">
                <!-- Box SVG -->
                <svg xmlns="http://www.w3.org/2000/svg" width="36" height="36" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M21 16V8a2 2 0 0 0-1-1.73l-7-4a2 2 0 0 0-2 0l-7 4A2 2 0 0 0 3 8v8a2 2 0 0 0 1 1.73l7 4a2 2 0 0 0 2 0l7-4A2 2 0 0 0 21 16z"></path><polyline points="3.27 6.96 12 12.01 20.73 6.96"></polyline><line x1="12" y1="22.08" x2="12" y2="12"></line></svg>
              </div>
              <h3>智标平台</h3>
            </div>
            <div class="product-tags">
              <span class="tag">数据标注工具</span>
              <span class="tag outline">面向AI需求方</span>
            </div>
            <p class="product-desc">提供多模态高质量预标注工具与智能审核机制，为AI大模型需求方提供极佳的数据生成引擎，释放算法潜力。</p>
            <ul class="product-highlights">
              <li><span class="hl-dot"></span> 全模态支持：2D/3D点云、视频、文本RLHF</li>
              <li><span class="hl-dot"></span> AI预标注加持，单帧标注性能提效300%</li>
              <li><span class="hl-dot"></span> 自动化多级流水线质检，保障99.9%极致准确率</li>
            </ul>
            <button class="glow-btn small-btn">进入控制台</button>
          </div>
          <div class="product-media-large">
            <div class="media-placeholder">
              <svg class="placeholder-icon" xmlns="http://www.w3.org/2000/svg" width="64" height="64" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"><rect x="3" y="3" width="18" height="18" rx="2" ry="2"></rect><circle cx="8.5" cy="8.5" r="1.5"></circle><polyline points="21 15 16 10 5 21"></polyline></svg>
              <span class="placeholder-text">平台演示界面 / 数据可视化视频 占位<br/>(等待素材更新)</span>
            </div>
          </div>
        </div>

        <!-- 聚合管理平台 -->
        <div class="product-row reverse">
          <div class="product-content">
            <div class="product-title-wrap">
              <div class="product-icon">
                <!-- Network/Share SVG -->
                <svg xmlns="http://www.w3.org/2000/svg" width="36" height="36" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><circle cx="18" cy="5" r="3"></circle><circle cx="6" cy="12" r="3"></circle><circle cx="18" cy="19" r="3"></circle><line x1="8.59" y1="13.51" x2="15.42" y2="17.49"></line><line x1="15.41" y1="6.51" x2="8.59" y2="10.49"></line></svg>
              </div>
              <h3>聚合管理平台</h3>
            </div>
            <div class="product-tags">
              <span class="tag str">标注工会管理系统</span>
              <span class="tag outline">面向B端标注服务商</span>
            </div>
            <p class="product-desc">全面的团队协作、绩效统计及分发管理系统，赋能标注公会实现高效的数据作业调度和产出监控。</p>
            <ul class="product-highlights">
              <li><span class="hl-dot"></span> 千人级别精细化权限与角色分层管理</li>
              <li><span class="hl-dot"></span> 实时数据看板，精准统计结算成员工时与绩效</li>
              <li><span class="hl-dot"></span> 上下游任务一键智能分发与数据资产沉淀</li>
            </ul>
            <button class="glow-btn small-btn outline-mode">了解系统详情</button>
          </div>
          <div class="product-media-large">
            <div class="media-placeholder alt-bg">
              <svg class="placeholder-icon" xmlns="http://www.w3.org/2000/svg" width="64" height="64" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"><rect x="3" y="3" width="18" height="18" rx="2" ry="2"></rect><line x1="3" y1="9" x2="21" y2="9"></line><line x1="9" y1="21" x2="9" y2="9"></line></svg>
              <span class="placeholder-text">公会管理数据大屏 / 任务调度后台 占位<br/>(等待素材更新)</span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.features {
  background: var(--color-bg-surface);
  padding: 100px 0;
}

.products-header {
  text-align: center;
  margin-bottom: 80px;
}

.section-title {
  font-size: 36px;
  margin-bottom: 20px;
}

.section-subtitle {
  color: var(--color-text-muted);
  font-size: 18px;
  line-height: 1.6;
}

.product-showcase {
  display: flex;
  flex-direction: column;
  gap: 120px;
}

.product-row {
  display: flex;
  align-items: center;
  gap: 60px;
}

.product-row.reverse {
  flex-direction: row-reverse;
}

.product-content {
  flex: 1;
}

.product-title-wrap {
  display: flex;
  align-items: center;
  gap: 20px;
  margin-bottom: 24px;
}

.product-icon {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  width: 64px;
  height: 64px;
  border-radius: 16px;
  background: rgba(0, 242, 254, 0.1);
  color: var(--color-secondary);
}

.product-row.reverse .product-icon {
  background: rgba(0, 85, 255, 0.1);
  color: var(--color-primary);
}

.product-content h3 {
  font-size: 36px;
  color: var(--color-text-main);
  margin: 0;
}

.product-tags {
  display: flex;
  gap: 12px;
  margin-bottom: 24px;
  align-items: center;
}

.tag {
  background: var(--color-primary);
  color: #fff;
  padding: 6px 14px;
  border-radius: 6px;
  font-size: 14px;
  font-weight: 500;
}

.tag.outline {
  background: transparent;
  color: var(--color-primary);
  border: 1px solid var(--color-primary);
}

.tag.str {
  background: var(--color-secondary);
}

.product-desc {
  color: var(--color-text-muted);
  font-size: 18px;
  line-height: 1.8;
  margin-bottom: 30px;
}

.product-highlights {
  list-style: none;
  padding: 0;
  margin: 0 0 40px 0;
}

.product-highlights li {
  font-size: 16px;
  color: var(--color-text-main);
  margin-bottom: 16px;
  display: flex;
  align-items: center;
  gap: 12px;
}

.hl-dot {
  display: inline-block;
  width: 8px;
  height: 8px;
  background: var(--color-secondary);
  border-radius: 50%;
  box-shadow: 0 0 8px var(--color-secondary);
}

.product-row.reverse .hl-dot {
  background: var(--color-primary);
  box-shadow: 0 0 8px var(--color-primary);
}

.small-btn {
  padding: 12px 32px;
}

.outline-mode {
  background: transparent;
  color: var(--color-primary);
  border: 1px solid var(--color-primary);
}
.outline-mode::before { display: none; }
.outline-mode:hover { background: rgba(0, 85, 255, 0.05); }

.product-media-large {
  flex: 1.4;
  height: 480px;
  border-radius: 24px;
  overflow: hidden;
  box-shadow: 0 30px 60px rgba(0, 0, 0, 0.08);
  background: var(--color-bg-dark);
}

.media-placeholder {
  width: 100%;
  height: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  background: linear-gradient(135deg, rgba(0, 242, 254, 0.05) 0%, rgba(0, 85, 255, 0.05) 100%);
  border: 2px dashed rgba(0, 242, 254, 0.3);
  border-radius: 24px;
  color: var(--color-text-muted);
  text-align: center;
}

.media-placeholder.alt-bg {
  background: linear-gradient(135deg, rgba(0, 85, 255, 0.05) 0%, rgba(0, 242, 254, 0.05) 100%);
  border-color: rgba(0, 85, 255, 0.3);
}

.placeholder-icon {
  color: var(--color-text-muted);
  opacity: 0.5;
  margin-bottom: 20px;
}

.placeholder-text {
  font-size: 18px;
  line-height: 1.6;
  opacity: 0.8;
}

@media (max-width: 992px) {
  .product-row, .product-row.reverse {
    flex-direction: column;
    gap: 40px;
  }
  .product-media-large {
    width: 100%;
    height: 300px;
  }
}
</style>
