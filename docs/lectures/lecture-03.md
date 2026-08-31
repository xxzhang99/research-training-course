# 第3讲 · 科研方法

<span class="status status-ready">资料已发布</span>

## 从机理、解法到实现与证据

本讲承接第二讲形成的候选问题，完成一次缩小版研究闭环：界定问题、分析机理、提出可反驳假设、构思和估算方案、完成最小实现计划，再从研究主张反推实验和证据。

<div class="downloads">
<a href="../../assets/files/lecture-03/slides.pdf">下载PDF课件</a>
<a href="../../assets/files/lecture-03/slides.pptx">下载PPTX课件</a>
</div>

<div class="notice">
公开PPTX为课程完整版，包含授课备注、课堂任务和参考答案。课程示例用于教学，请根据具体研究方向重新判断其假设与证据边界。
</div>

## 学习目标

完成本讲后，学生应能够：

1. 区分现象、研究问题、机理和解法；
2. 使用第一性原理识别资源、约束、不变量和必要条件；
3. 将机理转化为可检验、可反驳的研究假设；
4. 形成多个候选方案，并说明方案如何作用于关键机理；
5. 使用back-of-the-envelope calculation判断数量级与可行性；
6. 用20/80原则设计最小可验证实现和快速迭代；
7. 从Claim反推基线、变量、指标、统计量和预期反证；
8. 识别相关当因果、不公平比较、选择性汇报等逻辑问题。

## 课堂结构

| 模块 | 脚手架任务 | 阶段产出 |
|---|---|---|
| 问题界定 | 现象/问题/方案分类 | Problem Statement |
| 机理分析 | 信息卡排序 | Mechanism Chain |
| 假设形成 | 条件—干预—预测—反证拼装 | Research Hypothesis |
| 方案构思 | 设计原则和备选方案比较 | Solution Sketch |
| 数量级估算 | 简单I/O耗时计算 | Feasibility Estimate |
| 最小实现 | Baseline-first与单变量改动 | MVP Plan |
| 实验设计 | Claim—Evidence Matrix | Evaluation Plan |
| 逻辑审查 | 实验与结论问题识别 | Logic Audit |

## 案例主线

课程继续使用MapReduce—RDD演进作为贯穿案例：

```text
迭代任务延迟高
→ 跨轮工作集经稳定存储共享
→ 重复I/O和序列化累积
→ 跨操作内存复用成为设计原则
→ 不可变分区数据与lineage提供一种具体实现
→ 通过延迟、I/O、内存与故障恢复实验验证
```

## 课后建议

围绕自己的候选问题提交：

- Solution Sketch；
- Back-of-the-envelope估算；
- MVP Plan；
- Evaluation Plan；
- Logic Audit与最大风险说明。
