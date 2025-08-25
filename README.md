# GZMet

[![GitHub Stars](https://img.shields.io/github/stars/Yilaixien/GZMet?style=social&label=Star)](https://github.com/Yilaixien/GZMet/stargazers)
[![GitHub Forks](https://img.shields.io/github/forks/Yilaixien/GZMet?style=social&label=Fork)](https://github.com/Yilaixien/GZMet/network/members)
[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

![项目演示图](https://raw.githubusercontent.com/Yilaixien/GZMet/main/docs/demo.gif)  <!-- 替换为实际GIF -->

## 📌 项目定位
基于WebGL的地铁数据可视化分析平台，通过三维建模和时空数据分析，为城市交通规划提供决策支持。项目包含：

- 📈 动态客流热力分布（实时模拟）
- 🗺️ 三维线路拓扑结构
- 🚉 换乘站效率评估模型
- 📊 多维度数据仪表盘

> ⚠️ 重要声明：演示数据为2025年Q2模拟数据，实际运营数据需通过[广州地铁开放平台](http://gzmtr.cn)申请

## 🔧 技术架构
```mermaid
graph TD
    A[数据层] --> B[静态JSON]
    A --> C[模拟数据生成器]
    B --> D[数据清洗模块]
    C --> D
    D --> E[可视化引擎]
    E --> F[ECharts GL]
    E --> G[Three.js]
    E --> H[D3.js]
