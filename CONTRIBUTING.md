# 贡献指南

感谢你对通用因果解释协议的关注！

## 协议改进流程

本协议以实证方式构建——每条规则都是为了解决*实际观察到的*错误。

### 提议修改协议

1. 先用 [Bug Report](https://github.com/20kiki/causal-explanation-protocol/issues/new?template=bug_report.md) 模板提交 Issue，描述协议在什么场景下给出了错误分类或错误解释
2. 在 Issue 中讨论确认后，再提交 PR
3. PR 中必须包含：协议修改内容 + 验证该修改的 Before / After 案例

### 贡献案例

如果你有新的因果解释案例（Before / After 对比），请用 [Feature Request](https://github.com/20kiki/causal-explanation-protocol/issues/new?template=feature_request.md) 模板提交。

案例要求：
- 同一个问题，展示「不使用协议」和「使用协议」两种回答
- 标注协议具体捕捉到了什么错误（循环论证？错误类比？伪根本因？模式选择错误？）
- 尽量覆盖边缘场景

## 本地开发

本协议是一个纯 Markdown 项目，无需构建工具。

```bash
# 克隆项目
git clone https://github.com/20kiki/causal-explanation-protocol.git
cd causal-explanation-protocol

# 用你喜欢的编辑器打开
code .
```

## 提交信息规范

```
feat: 添加 XX 案例
fix: 修复模式 X 的分类规则
docs: 更新中文翻译
```

## 许可证

贡献即表示你同意将代码按 MIT 协议开源。
