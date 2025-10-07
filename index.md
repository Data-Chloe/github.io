---
layout: single
title: "G'day, I'm Chloe."
classes: home
---

<div class="hero-section" style="background: linear-gradient(135deg, #2d5a3d 0%, #1e3d2b 100%); color: white; padding: 60px 0; text-align: center;">
  <div style="max-width: 1400px; margin: 0 auto; padding: 0 50px;">
    <div style="display: flex; align-items: center; justify-content: center; gap: 10px; flex-wrap: wrap;">
      <div style="flex: 0 0 auto; text-align: right;">
        <h1 style="font-size: 3rem; margin: 0; font-weight: 700; line-height: 1.2;">G'day, I'm Chloe.</h1>
      </div>
      <div style="flex: 0 0 auto; text-align: left;">
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
  max-width: 1400px !important;
  margin: 0 auto !important;
  padding: 0 50px !important;
  width: 100% !important;
}

.hero-section > div > div {
  display: flex !important;
  align-items: center !important;
  justify-content: center !important;
  gap: 10px !important;
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
  <div style="max-width: 1400px; margin: 0 auto; padding: 0 50px;">
    <div style="display: flex; justify-content: space-between; align-items: center; flex-wrap: wrap;">
      <a href="/" style="color: #2d5a3d; text-decoration: none; font-weight: 800; font-size: 28px; padding: 22px 35px; border-radius: 15px; transition: all 0.3s ease; letter-spacing: 1.2px;">Home</a>
      <a href="/about/" style="color: #2d5a3d; text-decoration: none; font-weight: 800; font-size: 28px; padding: 22px 35px; border-radius: 15px; transition: all 0.3s ease; letter-spacing: 1.2px;">About</a>
      <a href="/portfolio/" style="color: #2d5a3d; text-decoration: none; font-weight: 800; font-size: 28px; padding: 22px 35px; border-radius: 15px; transition: all 0.3s ease; letter-spacing: 1.2px;">Portfolio</a>
      <a href="/blog/" style="color: #2d5a3d; text-decoration: none; font-weight: 800; font-size: 28px; padding: 22px 35px; border-radius: 15px; transition: all 0.3s ease; letter-spacing: 1.2px;">Blog</a>
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
  max-width: 1400px !important;
  margin: 0 auto !important;
  padding: 0 50px !important;
  width: 100% !important;
}

.nav-section > div > div {
  display: flex !important;
  justify-content: space-between !important;
  align-items: center !important;
  flex-wrap: wrap !important;
  width: 100% !important;
}

.nav-section a {
  color: #2d5a3d !important;
  text-decoration: none !important;
  font-weight: 800 !important;
  font-size: 28px !important;
  padding: 22px 35px !important;
  border-radius: 15px !important;
  transition: all 0.3s ease !important;
  letter-spacing: 1.2px !important;
}

/* 手机导航响应式 */
@media (max-width: 768px) {
  .nav-section > div > div {
    gap: 50px !important;
    flex-wrap: wrap !important;
  }
  .nav-section a {
    font-size: 22px !important;
    padding: 18px 28px !important;
    font-weight: 800 !important;
  }
}

/* 平板导航响应式 */
@media (min-width: 769px) and (max-width: 1024px) {
  .nav-section > div > div {
    gap: 80px !important;
  }
  .nav-section a {
    font-size: 25px !important;
    padding: 20px 32px !important;
  }
}

/* 文章列表样式 - 主页使用宽屏 */
.blog-posts {
  text-align: center !important;
  max-width: 1400px !important;
  margin: 0 auto !important;
  padding: 0 20px !important;
}

.blog-posts ul {
  list-style: none !important;
  padding: 0 !important;
  margin: 20px 0 !important;
}

.blog-posts li {
  margin: 15px 0 !important;
  padding: 10px 0 !important;
  border-bottom: 1px solid #f0f0f0 !important;
}

.blog-posts li:last-child {
  border-bottom: none !important;
}

.blog-posts a {
  color: #2d5a3d !important;
  text-decoration: none !important;
  font-weight: 600 !important;
  font-size: 18px !important;
}

.blog-posts a:hover {
  color: #1e3d2b !important;
  text-decoration: underline !important;
}

/* 隐藏RSS feed */
.page__footer-feed,
.feed__icon,
a[href*="feed.xml"],
a[href*="rss.xml"],
a[href*="atom.xml"] {
  display: none !important;
}

/* 居中footer版权信息 */
.page__footer {
  text-align: center !important;
}

.page__footer-copyright {
  text-align: center !important;
  margin: 0 auto !important;
}

/* 主页宽屏布局 - 保持原来的宽屏效果 */
.page__content {
  max-width: 1400px !important;
  margin: 0 auto !important;
  padding: 0 !important;
}

.single .page__content {
  max-width: 1400px !important;
  margin: 0 auto !important;
  padding: 0 !important;
}

.single .page__inner {
  max-width: 1400px !important;
  margin: 0 auto !important;
}

/* 确保主页内容区域不受其他样式影响 */
body.home .page__content,
body.home .page__inner,
body.home .single .page__content,
body.home .single .page__inner {
  max-width: 1400px !important;
  margin: 0 auto !important;
  padding: 0 !important;
}

/* 主页特有样式 - 强制宽屏布局 */
.hero-section,
.nav-section,
.blog-posts {
  max-width: 1400px !important;
  margin: 0 auto !important;
}

/* 强制覆盖所有可能的容器限制 */
.home .page__inner,
.home .page__content,
.home .single .page__inner,
.home .single .page__content,
.home .page {
  max-width: 1400px !important;
  width: 100% !important;
  margin: 0 auto !important;
  padding: 0 !important;
}

/* 确保主页的各个部分都使用宽屏 */
.home .hero-section > div {
  max-width: 1400px !important;
  width: 100% !important;
}

.home .nav-section > div {
  max-width: 1400px !important;
  width: 100% !important;
}

.home .blog-posts > div {
  max-width: 1400px !important;
  width: 100% !important;
}

/* 主页强制宽屏 - 最高优先级 */
body.home .blog-posts {
  max-width: 1400px !important;
  width: 100% !important;
}

body.home .blog-posts > div {
  max-width: 1400px !important;
  width: 100% !important;
}

/* 确保主页不受其他页面样式影响 */
.home .page__content.blog-posts,
.home .single .page__content.blog-posts {
  max-width: 1400px !important;
  width: 100% !important;
}
</style>

<div class="blog-posts">
<div style="max-width: 1400px; margin: 0 auto; padding: 0 50px;">
  <div style="margin: 25px 0; padding: 0;">
    <div style="display: flex; align-items: center;">
      <span style="color: #2d5a3d; font-weight: 700; font-size: 24px; width: 60px; text-align: left;">1.</span>
      <div style="flex: 1; display: flex; justify-content: space-between; align-items: center; padding-left: 15px;">
        <a href="/blog/tableau-basics/" style="color: #2d5a3d; text-decoration: none; font-weight: 600; font-size: 26px;">My Tableau Learning Journey</a>
        <span style="color: #888; font-size: 22px; font-weight: normal;">January 15, 2025</span>
      </div>
    </div>
  </div>
  <div style="margin: 25px 0; padding: 0;">
    <div style="display: flex; align-items: center;">
      <span style="color: #2d5a3d; font-weight: 700; font-size: 24px; width: 60px; text-align: left;">2.</span>
      <div style="flex: 1; display: flex; justify-content: space-between; align-items: center; padding-left: 15px;">
        <a href="/blog/pte-learning-experience/" style="color: #2d5a3d; text-decoration: none; font-weight: 600; font-size: 26px;">PTE Certification Experience</a>
        <span style="color: #888; font-size: 22px; font-weight: normal;">January 10, 2025</span>
      </div>
    </div>
  </div>
  <div style="margin: 25px 0; padding: 0;">
    <div style="display: flex; align-items: center;">
      <span style="color: #2d5a3d; font-weight: 700; font-size: 24px; width: 60px; text-align: left;">3.</span>
      <div style="flex: 1; display: flex; justify-content: space-between; align-items: center; padding-left: 15px;">
        <a href="/blog/python-data-analysis/" style="color: #2d5a3d; text-decoration: none; font-weight: 600; font-size: 26px;">Python Data Analysis in Practice</a>
        <span style="color: #888; font-size: 22px; font-weight: normal;">January 5, 2025</span>
      </div>
    </div>
  </div>
  <div style="margin: 25px 0; padding: 0;">
    <div style="display: flex; align-items: center;">
      <span style="color: #2d5a3d; font-weight: 700; font-size: 24px; width: 60px; text-align: left;">4.</span>
      <div style="flex: 1; display: flex; justify-content: space-between; align-items: center; padding-left: 15px;">
        <a href="/blog/power-bi-advanced/" style="color: #2d5a3d; text-decoration: none; font-weight: 600; font-size: 26px;">Power BI Advanced Features</a>
        <span style="color: #888; font-size: 22px; font-weight: normal;">December 28, 2024</span>
      </div>
    </div>
  </div>
</div>
</div>

<div style="background: linear-gradient(135deg, #2d5a3d 0%, #1e3d2b 100%); color: white; padding: 30px 0; text-align: center; margin: 80px 0 0 0;">
  <div style="max-width: 1400px; margin: 0 auto; padding: 0 50px;">
    <h1 style="font-size: 2.5rem; margin: 0; font-weight: 700; line-height: 1.2;">Thanks for visiting!</h1>
  </div>
</div>



