# rust-by-practice 维护说明

Rust 练习、示例和参考解答，包含中英文 mdBook。

- 上游：https://github.com/origin-brain/rust-by-practice
- 在线文档：https://xiaoshecode.github.io/xiaoshecode/repos/rust-by-practice/
- 检查日期：2026-10-30

## 环境与使用

- 安装 Rust 和 mdBook；依具体 book.toml 准备额外预处理器。

使用/检查入口（需先满足依赖条件）：

- `mdbook serve zh-CN`
- `mdbook build en`

## 目录职责

- zh-CN/ — 中文 mdBook
- en/ — 英文 mdBook
- practices/ — 实践项目
- solutions/ — 参考解答
- scripts/ — 维护脚本

## 本次整理

- 新增维护文档和在线文档入口，补全用途、目录、使用路径及验证边界。

## 检查记录

- **仓库目录与入口盘点**（passed）：检查 Git 索引中的 295 个路径、README 和项目配置；不等于功能验收。
- **JavaScript syntax**（passed）：4 个文件通过解析；不导入依赖、不执行应用。
- **TOML parse**（passed）：5 个文件通过解析；不导入依赖、不执行应用。
- **完整构建与端到端运行**（not_run）：教学练习可能故意无法编译；本机未安装 Rust/mdBook，未执行书籍构建与练习测试。

## 验证边界与待办

- 教学练习可能故意无法编译；本机未安装 Rust/mdBook，未执行书籍构建与练习测试。

## 后续维护约定

保留上游许可证与作者信息。沿用现有模块边界和格式配置；修复功能时同步最小回归验证。依赖或接口变更需写明迁移步骤，避免仅为目录美观搬动公开入口。
