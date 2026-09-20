# 项目名称

> 一句话描述项目功能

## ✨ 项目简介

基于 Maven 构建的 Java 项目，使用 VSCode + Extension Pack for Java 开发。
实现【xxx业务】，可用于学习、接口演示。

## 📋 环境要求

- JDK：JDK8 / JDK17
- 构建工具：Maven 3.6+
- IDE：VSCode + Java扩展包
- 数据库（可选）：MySQL 8.0

## 📁 项目目录结构

```plaintext
├── src
│ ├── main
│ │ ├── java # Java业务源码
│ │ └── resources # 资源/配置文件
│ └── test
│ └── java # 单元测试代码
├── pom.xml # Maven依赖、构建配置
├── .vscode # VSCode本地配置（加入gitignore，不上传）
├── .gitignore
└── README.md
```

## 🚀 快速启动

### 1. 克隆项目

```bash
git clone [https://github.com/](https://github.com/)你的用户名/仓库名.git
cd 仓库名
```

### 2. VSCode打开项目

1. VSCode `文件 → 打开文件夹`，选中项目根目录（pom.xml所在目录）
2. 等待Java扩展加载，自动识别Maven项目
3. 确认JDK版本和pom中配置保持一致

### 3. 运行项目

#### 方式1：VSCode图形化运行

找到包含`main()`的类，点击代码上方的「运行」按钮。

#### 方式2：Maven命令

```bash
# 清理编译产物
mvn clean
# 编译源码
mvn compile
# 执行单元测试
mvn test
# 打包，jar输出在 target 目录
mvn package
```

## 📦 Maven常用命令

```bash
mvn clean        # 删除target目录
mvn compile      # 编译java代码
mvn test         # 运行单元测试
mvn package      # 打包生成jar
mvn install      # 打包并安装到本地maven仓库
```

## 📌 功能清单

- 功能1
- 功能2
- 待开发功能

## 📝 开发规范

> Git提交规范：`type(scope): description`

- feat：新增功能
- fix：修复bug
- docs：文档修改
- refactor：代码重构
- style：代码格式调整
- test：新增/修改测试代码
- chore：修改pom、gitignore、构建相关配置

## ❗ 常见问题

1. Maven依赖加载失败
   
   > 在VSCode侧边Maven面板刷新项目；配置Maven阿里云镜像

2. JDK版本不匹配
   
   > VSCode `Ctrl+Shift+P` → Java: Configure Java Runtime 切换JDK

3. .vscode目录提交到远程仓库
   
   > 在.gitignore添加 `.vscode/` 忽略本地编辑器配置

## 📄 License

MIT

## 使用说明

1. 在项目根目录新建 `README.md`，粘贴内容
2. 修改项目名称、简介、功能列表
3. 搭配配套的 `.gitignore` 使用
