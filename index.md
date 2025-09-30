---
layout: default
title: "G'day, I'm Chloe."
---

<div class="hero-section" style="background: linear-gradient(135deg, #2d5a3d 0%, #1e3d2b 100%); color: white; padding: 60px 0; text-align: center;">
  <div style="max-width: 1200px; margin: 0 auto; padding: 0 30px;">
    <div style="display: flex; align-items: center; justify-content: center; gap: 0px; flex-wrap: wrap;">
      <div style="flex: 1; min-width: 350px; text-align: right; padding-right: 10px;">
        <h1 style="font-size: 3rem; margin: 0; font-weight: 700; line-height: 1.2;">G'day, I'm Chloe.</h1>
      </div>
      <div style="flex: 0 0 auto; text-align: left; padding-left: 10px;">
        <img src="/assets/images/profile.jpg" alt="Chloe" style="width: 200px; height: 200px; border-radius: 50%; border: 3px solid rgba(255,255,255,0.5); object-fit: cover; object-position: center; image-rendering: -webkit-optimize-contrast; image-rendering: crisp-edges; box-shadow: 0 6px 20px rgba(0,0,0,0.15);">
      </div>
    </div>
  </div>
</div>

<style>
/* 强制覆盖Jekyll默认样式 */
.hero-section {
  width: 100% !important;
  max-width: none !important;
  margin: 0 !important;
  padding: 60px 0 !important;
  background: linear-gradient(135deg, #2d5a3d 0%, #1e3d2b 100%) !important;
  color: white !important;
  text-align: center !important;
}

.hero-section > div {
  max-width: 1200px !important;
  margin: 0 auto !important;
  padding: 0 30px !important;
  width: 100% !important;
}

.hero-section > div > div {
  display: flex !important;
  align-items: center !important;
  justify-content: center !important;
  gap: 0px !important;
  flex-wrap: wrap !important;
  width: 100% !important;
}

/* 笔记本电脑响应式 */
@media (min-width: 769px) {
  .hero-section > div > div {
    flex-direction: row !important;
  }
  .hero-section h1 {
    font-size: 3rem !important;
  }
  .hero-section img {
    width: 200px !important;
    height: 200px !important;
    image-rendering: -webkit-optimize-contrast !important;
    image-rendering: crisp-edges !important;
    object-fit: cover !important;
    object-position: center !important;
  }
}

/* 手机响应式 */
@media (max-width: 768px) {
  .hero-section {
    padding: 50px 20px !important;
  }
  .hero-section > div > div {
    flex-direction: column !important;
    gap: 5px !important;
    text-align: center !important;
  }
  .hero-section h1 {
    font-size: 2.5rem !important;
  }
  .hero-section p {
    font-size: 1rem !important;
  }
  .hero-section img {
    width: 160px !important;
    height: 160px !important;
    image-rendering: -webkit-optimize-contrast !important;
    image-rendering: crisp-edges !important;
    object-fit: cover !important;
    object-position: center !important;
  }
}
</style>

<div class="nav-section" style="text-align: center; margin: 30px 0; padding: 20px 0; border-top: 1px solid #e8e8e8; border-bottom: 1px solid #e8e8e8; background: #fafafa;">
  <div style="max-width: 1200px; margin: 0 auto; padding: 0 30px;">
    <div style="display: flex; justify-content: center; align-items: center; gap: 70px; flex-wrap: wrap;">
      <a href="/" style="color: #2d5a3d; text-decoration: none; font-weight: 600; font-size: 24px; padding: 18px 30px; border-radius: 12px; transition: all 0.3s ease; letter-spacing: 1px;">首页</a>
      <a href="/about/" style="color: #2d5a3d; text-decoration: none; font-weight: 600; font-size: 24px; padding: 18px 30px; border-radius: 12px; transition: all 0.3s ease; letter-spacing: 1px;">关于我</a>
      <a href="/portfolio/" style="color: #2d5a3d; text-decoration: none; font-weight: 600; font-size: 24px; padding: 18px 30px; border-radius: 12px; transition: all 0.3s ease; letter-spacing: 1px;">作品集</a>
      <a href="/blog/" style="color: #2d5a3d; text-decoration: none; font-weight: 600; font-size: 24px; padding: 18px 30px; border-radius: 12px; transition: all 0.3s ease; letter-spacing: 1px;">学习日志</a>
      <a href="/certifications/" style="color: #2d5a3d; text-decoration: none; font-weight: 600; font-size: 24px; padding: 18px 30px; border-radius: 12px; transition: all 0.3s ease; letter-spacing: 1px;">认证</a>
    </div>
  </div>
</div>

<style>
/* 导航栏样式 */
.nav-section {
  width: 100% !important;
  max-width: none !important;
  margin: 30px 0 !important;
  padding: 20px 0 !important;
  text-align: center !important;
  border-top: 1px solid #e8e8e8 !important;
  border-bottom: 1px solid #e8e8e8 !important;
  background: #fafafa !important;
}

.nav-section > div {
  max-width: 1200px !important;
  margin: 0 auto !important;
  padding: 0 30px !important;
  width: 100% !important;
}

.nav-section > div > div {
  display: flex !important;
  justify-content: center !important;
  align-items: center !important;
  gap: 70px !important;
  flex-wrap: wrap !important;
  width: 100% !important;
}

.nav-section a {
  color: #2d5a3d !important;
  text-decoration: none !important;
  font-weight: 600 !important;
  font-size: 24px !important;
  padding: 18px 30px !important;
  border-radius: 12px !important;
  transition: all 0.3s ease !important;
  letter-spacing: 1px !important;
}

/* 手机导航响应式 */
@media (max-width: 768px) {
  .nav-section > div > div {
    gap: 40px !important;
    flex-wrap: wrap !important;
  }
  .nav-section a {
    font-size: 20px !important;
    padding: 15px 25px !important;
    font-weight: 600 !important;
  }
}

/* 平板导航响应式 */
@media (min-width: 769px) and (max-width: 1024px) {
  .nav-section > div > div {
    gap: 60px !important;
  }
  .nav-section a {
    font-size: 22px !important;
    padding: 16px 28px !important;
  }
}
</style>

## 欢迎来到我的数据分析世界

我是一名热爱数据分析的专业人士，专注于将复杂的数据转化为有价值的商业洞察。

### 🎯 我的专长
- **数据可视化**: Tableau、Power BI 仪表板设计
- **数据分析**: Python、R、SQL 数据处理
- **商业智能**: KPI监控、业务报告自动化
- **预测建模**: 销售预测、客户行为分析

### 📊 最新动态
- ✅ 获得 Tableau Desktop Specialist 认证
- ✅ 获得 Microsoft Power BI Data Analyst 认证
- 📝 正在学习 Tableau Server 管理
- 🔄 持续更新 [学习日志](/blog/) 和 [作品集](/portfolio/)

### 💡 为什么选择数据分析？
数据不会说谎，但需要我们用心去解读。我相信通过专业的数据分析，可以帮助企业发现隐藏的机会，优化业务流程，做出更明智的决策。
