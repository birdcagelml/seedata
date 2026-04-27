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
            <div class="screen-frame">
              <div class="screen-bar">
                <div class="screen-dots">
                  <span></span><span></span><span></span>
                </div>
                <div class="screen-title-bar">ZhiBiao Platform</div>
              </div>
              <div class="screen-body">
                <img src="/zhibiao.png" alt="智标平台演示界面" class="product-img" />
                <div class="scan-line"></div>
              </div>
            </div>
            <div class="corner tl"></div>
            <div class="corner tr"></div>
            <div class="corner bl"></div>
            <div class="corner br"></div>
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
            <!-- <button class="glow-btn small-btn outline-mode">了解系统详情</button> -->
          </div>
          <div class="product-media-large alt">
            <div class="screen-frame">
              <div class="screen-bar">
                <div class="screen-dots">
                  <span></span><span></span><span></span>
                </div>
                <div class="screen-title-bar">Synergy Hub</div>
              </div>
              <div class="screen-body">
                <img src="/juhe.png" alt="聚合管理平台演示界面" class="product-img" />
                <div class="scan-line"></div>
              </div>
            </div>
            <div class="corner tl"></div>
            <div class="corner tr"></div>
            <div class="corner bl"></div>
            <div class="corner br"></div>
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

/* ===== 产品媒体区域 ===== */
.product-media-large {
  flex: 1.4;
  position: relative;
  border-radius: 20px;
  padding: 20px;
  background: linear-gradient(135deg, rgba(0, 242, 254, 0.04) 0%, rgba(0, 85, 255, 0.06) 100%);
  border: 1.5px dashed rgba(0, 242, 254, 0.3);
  box-shadow: 0 24px 60px rgba(0, 0, 0, 0.2);
  transition: border-color 0.4s ease, box-shadow 0.4s ease;
}

.product-media-large.alt {
  background: linear-gradient(135deg, rgba(0, 85, 255, 0.06) 0%, rgba(0, 242, 254, 0.04) 100%);
  border-color: rgba(0, 85, 255, 0.3);
}

.product-row:hover .product-media-large {
  border-color: rgba(0, 242, 254, 0.65);
  box-shadow: 0 30px 70px rgba(0, 0, 0, 0.25), 0 0 40px rgba(0, 242, 254, 0.08) inset;
}

.product-row:hover .product-media-large.alt {
  border-color: rgba(0, 85, 255, 0.65);
  box-shadow: 0 30px 70px rgba(0, 0, 0, 0.25), 0 0 40px rgba(0, 85, 255, 0.08) inset;
}

/* 四角装饰 */
.corner {
  position: absolute;
  width: 20px;
  height: 20px;
  z-index: 2;
  transition: opacity 0.4s ease;
  opacity: 0.5;
}

.product-row:hover .corner { opacity: 1; }

.corner.tl { top: 8px; left: 8px; border-top: 2px solid var(--color-secondary); border-left: 2px solid var(--color-secondary); border-radius: 4px 0 0 0; }
.corner.tr { top: 8px; right: 8px; border-top: 2px solid var(--color-secondary); border-right: 2px solid var(--color-secondary); border-radius: 0 4px 0 0; }
.corner.bl { bottom: 8px; left: 8px; border-bottom: 2px solid var(--color-secondary); border-left: 2px solid var(--color-secondary); border-radius: 0 0 0 4px; }
.corner.br { bottom: 8px; right: 8px; border-bottom: 2px solid var(--color-secondary); border-right: 2px solid var(--color-secondary); border-radius: 0 0 4px 0; }

.product-media-large.alt .corner.tl,
.product-media-large.alt .corner.tr,
.product-media-large.alt .corner.bl,
.product-media-large.alt .corner.br {
  border-color: var(--color-primary);
}

/* 模拟屏幕镜框 */
.screen-frame {
  border-radius: 12px;
  overflow: hidden;
  box-shadow: 0 8px 30px rgba(0, 0, 0, 0.4);
  border: 1px solid rgba(255, 255, 255, 0.08);
}

.screen-bar {
  display: flex;
  align-items: center;
  gap: 12px;
  padding: 10px 16px;
  background: rgba(20, 20, 30, 0.95);
  border-bottom: 1px solid rgba(255, 255, 255, 0.06);
}

.screen-dots {
  display: flex;
  gap: 6px;
  flex-shrink: 0;
}

.screen-dots span {
  display: inline-block;
  width: 10px;
  height: 10px;
  border-radius: 50%;
}

.screen-dots span:nth-child(1) { background: #ff5f57; }
.screen-dots span:nth-child(2) { background: #ffbd2e; }
.screen-dots span:nth-child(3) { background: #28ca41; }

.screen-title-bar {
  font-size: 12px;
  color: rgba(255, 255, 255, 0.35);
  letter-spacing: 0.04em;
  font-family: monospace;
}

.screen-body {
  position: relative;
  overflow: hidden;
  background: #0d0f1a;
  line-height: 0;
}

/* 扫光动画 */
.scan-line {
  position: absolute;
  top: -100%;
  left: 0;
  width: 100%;
  height: 40%;
  background: linear-gradient(180deg, transparent 0%, rgba(0, 242, 254, 0.04) 50%, transparent 100%);
  animation: scan 4s linear infinite;
  pointer-events: none;
}

.product-media-large.alt .scan-line {
  background: linear-gradient(180deg, transparent 0%, rgba(0, 85, 255, 0.04) 50%, transparent 100%);
}

@keyframes scan {
  0%   { top: -40%; }
  100% { top: 110%; }
}

.product-img {
  width: 100%;
  height: auto;
  display: block;
  transition: transform 0.6s ease;
}

.product-row:hover .product-img {
  transform: scale(1.03);
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
