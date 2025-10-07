---
title: "Python 数据分析实战"
permalink: /blog/python-data-analysis/
date: 2024-01-20
categories: [技术分享]
tags: [Python, 数据分析, Pandas, 实战案例]
layout: single
---

<div class="nav-section" style="text-align: center; margin: 30px 0; padding: 20px 0; border-top: 1px solid #e8e8e8; border-bottom: 1px solid #e8e8e8; background: #fafafa;">
  <div style="max-width: 1400px; margin: 0 auto; padding: 0 50px;">
    <div style="display: flex; justify-content: space-between; align-items: center; flex-wrap: wrap;">
      <a href="/" style="color: #2d5a3d; text-decoration: none; font-weight: 800; font-size: 28px; padding: 22px 35px; border-radius: 15px; transition: all 0.3s ease; letter-spacing: 1.2px;">Home</a>
      <a href="/about/" style="color: #2d5a3d; text-decoration: none; font-weight: 800; font-size: 28px; padding: 22px 35px; border-radius: 15px; transition: all 0.3s ease; letter-spacing: 1.2px;">About</a>
      <a href="/portfolio/" style="color: #2d5a3d; text-decoration: none; font-weight: 800; font-size: 28px; padding: 22px 35px; border-radius: 15px; transition: all 0.3s ease; letter-spacing: 1.2px;">Portfolio</a>
      <a href="/blog/" style="color: #2d5a3d; text-decoration: none; font-weight: 800; font-size: 28px; padding: 22px 35px; border-radius: 15px; transition: all 0.3s ease; letter-spacing: 1.2px; background: #e8f5e8;">Blog</a>
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

/* 文章页面经典布局 */
.page__content {
  max-width: 800px !important;
  margin: 0 auto !important;
  padding: 0 20px !important;
  font-size: 16px !important;
  line-height: 1.7 !important;
}

.page__content h1 {
  font-size: 2.5rem !important;
  margin-bottom: 1rem !important;
  color: #2d5a3d !important;
  border-bottom: 2px solid #e8e8e8 !important;
  padding-bottom: 0.5rem !important;
}

.page__content h2 {
  font-size: 1.8rem !important;
  margin-top: 2rem !important;
  margin-bottom: 1rem !important;
  color: #2d5a3d !important;
}

.page__content h3 {
  font-size: 1.4rem !important;
  margin-top: 1.5rem !important;
  margin-bottom: 0.8rem !important;
  color: #333 !important;
}

.page__content p {
  margin-bottom: 1.2rem !important;
  color: #444 !important;
}

.page__content ul, .page__content ol {
  margin-bottom: 1.2rem !important;
  padding-left: 2rem !important;
}

.page__content li {
  margin-bottom: 0.5rem !important;
  color: #444 !important;
}

.page__content blockquote {
  border-left: 4px solid #2d5a3d !important;
  padding-left: 1.5rem !important;
  margin: 1.5rem 0 !important;
  font-style: italic !important;
  color: #666 !important;
}

.page__content code {
  background: #f5f5f5 !important;
  padding: 0.2rem 0.4rem !important;
  border-radius: 3px !important;
  font-family: 'Courier New', monospace !important;
}

.page__content pre {
  background: #f8f8f8 !important;
  padding: 1rem !important;
  border-radius: 5px !important;
  overflow-x: auto !important;
  border: 1px solid #e8e8e8 !important;
}

/* 强制覆盖Jekyll主题样式 */
body .single .page__content,
body .page__content {
  max-width: 800px !important;
  margin: 0 auto !important;
  padding: 0 20px !important;
  width: auto !important;
}

body .single .page__inner,
body .page__inner {
  max-width: 800px !important;
  margin: 0 auto !important;
  width: auto !important;
}

/* 确保页面容器正确 */
.single .page,
.page {
  max-width: 800px !important;
  margin: 0 auto !important;
}

/* 覆盖主题的默认样式 */
.single .page__inner .page__content {
  max-width: 800px !important;
  margin: 0 auto !important;
  padding: 0 20px !important;
}
</style>

# Python 数据分析实战

在实际业务中，数据分析往往需要处理复杂的真实数据。这篇文章分享一个完整的Python数据分析项目，从数据清洗到可视化呈现的全过程。

## 🎯 项目背景

某电商公司希望分析用户购买行为，优化营销策略。数据包含：
- 用户基本信息
- 购买记录
- 商品信息
- 营销活动参与情况

## 📊 数据探索

### 数据概览
```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns

# 读取数据
df_users = pd.read_csv('users.csv')
df_orders = pd.read_csv('orders.csv')
df_products = pd.read_csv('products.csv')

# 数据基本信息
print("用户数据形状:", df_users.shape)
print("订单数据形状:", df_orders.shape)
print("商品数据形状:", df_products.shape)
```

### 数据质量检查
```python
# 检查缺失值
print("用户数据缺失值:")
print(df_users.isnull().sum())

# 检查重复值
print("重复用户数:", df_users.duplicated().sum())
print("重复订单数:", df_orders.duplicated().sum())
```

## 🔧 数据清洗

### 处理缺失值
```python
# 用户年龄缺失值用中位数填充
df_users['age'].fillna(df_users['age'].median(), inplace=True)

# 删除关键字段缺失的记录
df_orders = df_orders.dropna(subset=['user_id', 'product_id', 'order_amount'])
```

### 数据转换
```python
# 转换日期格式
df_orders['order_date'] = pd.to_datetime(df_orders['order_date'])

# 创建衍生字段
df_orders['order_month'] = df_orders['order_date'].dt.to_period('M')
df_orders['order_weekday'] = df_orders['order_date'].dt.day_name()
```

## 📈 数据分析

### 用户行为分析
```python
# 用户购买频次分析
user_purchase_freq = df_orders.groupby('user_id').agg({
    'order_id': 'count',
    'order_amount': ['sum', 'mean']
}).round(2)

# 可视化用户购买分布
plt.figure(figsize=(12, 5))

plt.subplot(1, 2, 1)
plt.hist(user_purchase_freq[('order_id', 'count')], bins=20, alpha=0.7)
plt.title('用户购买频次分布')
plt.xlabel('购买次数')
plt.ylabel('用户数量')

plt.subplot(1, 2, 2)
plt.hist(user_purchase_freq[('order_amount', 'sum')], bins=20, alpha=0.7)
plt.title('用户总消费分布')
plt.xlabel('总消费金额')
plt.ylabel('用户数量')

plt.tight_layout()
plt.show()
```

### 商品销售分析
```python
# 商品销售排行
product_sales = df_orders.groupby('product_id').agg({
    'order_id': 'count',
    'order_amount': 'sum'
}).sort_values(('order_id', 'count'), ascending=False)

# 合并商品信息
product_sales = product_sales.merge(df_products, left_index=True, right_on='product_id')

print("热销商品TOP10:")
print(product_sales[['product_name', ('order_id', 'count'), ('order_amount', 'sum')]].head(10))
```

### 时间趋势分析
```python
# 月度销售趋势
monthly_sales = df_orders.groupby('order_month').agg({
    'order_id': 'count',
    'order_amount': 'sum'
})

# 可视化趋势
fig, (ax1, ax2) = plt.subplots(2, 1, figsize=(12, 8))

# 订单数量趋势
monthly_sales[('order_id', 'count')].plot(kind='line', ax=ax1, marker='o')
ax1.set_title('月度订单数量趋势')
ax1.set_ylabel('订单数量')

# 销售金额趋势
monthly_sales[('order_amount', 'sum')].plot(kind='line', ax=ax2, marker='s', color='orange')
ax2.set_title('月度销售金额趋势')
ax2.set_ylabel('销售金额')
ax2.set_xlabel('月份')

plt.tight_layout()
plt.show()
```

## 🎯 关键发现

### 1. 用户分层
- **高价值用户** (20%): 贡献了80%的销售额
- **普通用户** (60%): 购买频次中等，有增长潜力
- **新用户** (20%): 首次购买，需要重点关注

### 2. 商品特征
- **爆款商品**: 价格适中的日常用品
- **高价值商品**: 虽然销量不高，但利润丰厚
- **季节性商品**: 有明显的销售周期

### 3. 时间模式
- **工作日**: 订单量稳定
- **周末**: 订单量增加30%
- **节假日**: 销售高峰，需要提前备货

## 💡 业务建议

### 营销策略
1. **精准营销**: 针对高价值用户推出VIP服务
2. **用户留存**: 为新用户设计专属优惠活动
3. **商品组合**: 基于关联分析推荐商品搭配

### 运营优化
1. **库存管理**: 根据销售趋势优化库存配置
2. **客服配置**: 周末增加客服人员
3. **促销时机**: 在工作日推出促销活动提升销量

## 🛠️ 技术总结

### 使用的工具
- **数据处理**: Pandas, NumPy
- **可视化**: Matplotlib, Seaborn
- **统计分析**: SciPy
- **机器学习**: Scikit-learn (后续分析)

### 关键技能
- 数据清洗和预处理
- 探索性数据分析 (EDA)
- 统计分析和假设检验
- 数据可视化设计

## 📚 学习资源

- [Pandas官方文档](https://pandas.pydata.org/docs/)
- [Matplotlib教程](https://matplotlib.org/stable/tutorials/)
- [数据分析最佳实践](https://github.com/jakevdp/PythonDataScienceHandbook)

---

*"数据不会说谎，但需要我们用心去解读。每一次分析都是对业务的深入理解。"*
