## 使用 Github Pages 搭建部署简单的网站

> [!INFO] Github pages 可以做什么？
> 1. 创建个人博客或简历等个人网页；
> 2. 托管团队项目文档和 API 文档以供大家浏览；
> 3. 备份和分享自己的代码作品；
> 4. 构建一个小型的电子商务网站、静态展示页面等。

> [!TIP] **注意**
> Github pages 仅支持静态网页——也就是说，您不能在上面运行动态（例如 PHP）网站

## 需要使用到的技术

HTML、CSS、JavaScript，Jekyll

## 如何开始?

1. 我们需要在 GitHub 上创建一个新的仓库，仓库的名称必须为 `<username>.github.io` (`<username>` 是你的 GitHub 用户名) 这个仓库是你的 GitHub Pages 站点的根目录 (最主要的目录). 具体细节可以使用 [Github pages](https://pages.github.com/) 的官方文档来查看.
2. 选择一个静态站点生成器作为博客的模板. 比较流行的工具.
	1. **Jekyll**: Jekyll 是 GitHub Pages 默认支持的静态网站生成器, 它基于 Ruby 语言，并且有很强的插件和主题支持.
	2. **Hugo**: Hugo 是一种用 Go 语言编写的静态网站生成器, 也被广泛用于部署博客和其他类似的应用.
	3. **GatsbyJS**: GatsbyJS 是一个 React 驱动的静态站点生成器，它提供了很多现代 Web 开发所需的最新功能和集成功能, 例如 GraphQL, 服务器渲染等.
3. 后面的主要内容就是定期更新您的博客.

> [!TIP] 注意
> 这个教程主要选择 Jekyll 搭建个人博客.

## 详细步骤

1. 安装环境 Jekyll, 需要 Linux 系统 安装环境, 但 Jekyll 也可以支持 windows 安装 Jekyll 环境. 我使用方案的是 Windows 平台中的 [WSL](https://learn.microsoft.com/en-us/windows/wsl/install) 来虚拟运行 Ubuntu
2. 使用 windows 命令行 启动 WSL ![](../../../附件/Pasted%20image%2020230706000156.png)
3. 安装
4. **选择一个合适的 jekyll 主题** (这里我选择了 [Chirpy]())

### 我需要那些功能?

1. [项目进度](博客项目进度功能.md)
2. [文章](博客文章功能.md)
3. [关于个人](博客关于个人信息功能)

 > [!INFO] 信息

> [!Tip] 提示

> [!Warning] 警告
