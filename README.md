___

## 开发人员产品组合

#### 您是否正在努力创建一个专业的投资组合网站？不用再观望了！您可以立即使用 Developer Portfolio 模板并创建您自己的个性化投资组合！我的网站设计为用户友好且易于定制，非常适合开发人员和自由职业者。

___

## 演示 🎥

[![](https://github.com/luckyu2/developer-portfolio/raw/main/public/image/screen.png)](https://github.com/luckyu2/developer-portfolio/blob/main/public/image/screen.png)

___

## 目录 📜

-   [部分](https://github.com/luckyu2/developer-portfolio#sections-bookmark)
-   [演示](https://github.com/luckyu2/developer-portfolio#demo-movie_camera)
-   [安装](https://github.com/luckyu2/developer-portfolio#installation-arrow_down)
-   [开始](https://github.com/luckyu2/developer-portfolio#getting-started-dart)
-   [用法](https://github.com/luckyu2/developer-portfolio#usage-joystick)
-   [部署](https://github.com/luckyu2/developer-portfolio#deployment-rocket)
-   [教程](https://github.com/luckyu2/developer-portfolio#tutorials-wrench)
    -   [Gmail 应用密码设置](https://github.com/luckyu2/developer-portfolio#gmail-app-password-setup)
    -   [创建 Telegram 机器人](https://github.com/luckyu2/developer-portfolio#create-a-telegram-bot)
    -   [从 dev.to 获取博客](https://github.com/luckyu2/developer-portfolio#fetching-blog-from-devto)
-   [使用的软件包](https://github.com/luckyu2/developer-portfolio#packages-used-package)

___

## 部分 🔖

-   英雄部分
-   关于我
-   经验
-   技能
-   项目
-   教育
-   博客
-   接触

___

## 安装 ⬇️

### 您需要下载 Git 和 Node 才能运行此项目

-   [Git](https://git-scm.com/downloads)
-   [节点](https://nodejs.org/en/download/)

#### 确保您的计算机上装有最新版本的 Git 和 Node。

```shell
node --version
git --version
```

## 开始 🎯

### Fork 和 Clone 存储库

要 Fork 仓库，请单击页面右上角的 fork 按钮。分叉存储库后，打开您的终端并执行以下命令

```shell
git clone https://github.com/<YOUR GITHUB USERNAME>/developer-portfolio.git

cd developer-portfolio
```

### 从根目录安装软件包

```shell
npm install
# or
yarn install
```

然后，运行开发服务器：

```shell
npm run dev
# or
yarn dev
```

使用浏览器打开 [http://localhost:3000](http://localhost:3000/) 以查看结果。

___

### 使用 Docker Compose 运行

1.  **构建 Docker 镜像并运行容器**：
    
    ```shell
    docker-compose up --build
    ```
    
2.  **访问应用程序**： 在 Web 浏览器中访问 [http://localhost:3000](http://localhost:3000/) 以查看正在运行的应用程序。
    

___

### 构建 Docker 镜像

1.  **使用 Dockerfile.dev 构建 Docker 镜像**：
    
    ```shell
    docker build -t nextjs-app -f Dockerfile.dev .
    ```
    
2.  **运行 Docker 容器**：
    
    ```shell
    docker run -p 3000:3000 nextjs-app
    ```
    
3.  **访问应用程序**： 在 Web 浏览器中访问 [http://localhost:3000](http://localhost:3000/) 以查看正在运行的应用程序。
    

___

## Usage 🕹️

请从 `.env.example` file 创建新`.env`文件。

Eg:

```dotenv
NEXT_PUBLIC_GTM =
NEXT_PUBLIC_APP_URL =
TELEGRAM_BOT_TOKEN =
TELEGRAM_CHAT_ID =
GMAIL_PASSKEY =
EMAIL_ADDRESS =
```

### Then, Customize data in the `utils/data` [folder](https://github.com/said7388/developer-portfolio/tree/main/utils/data).

Eg:

```js
export const personalData = {
  name: "ABU SAID",
  profile: "/profile.png",
  designation: "Full-Stack Software Developer",
  description: "My name is ABU SAID....",
  email: "abusaid7388@gmail.com",
  phone: "+8801608797655",
  address: "Dhaka, Bangladesh",
  github: "https://github.com/said7388",
  facebook: "https://www.facebook.com/abusaid.riyaz/",
  linkedIn: "https://www.linkedin.com/in/abu-said-bd/",
  twitter: "https://twitter.com/said7388",
  stackOverflow: "https://stackoverflow.com/users/16840768/abu-said",
  leetcode: "https://leetcode.com/said3812/",
  devUsername: "said7388",
  resume: "...",
};
```

`devUsername`用于从 `dev.to`中获取博客文章。

___

## Deployment 🚀

将应用程序部署到 Vercel 或 Netlify 等平台既快速又简单。

## Deploying to Vercel:

1.  **Sign up or log in** to [Vercel](https://vercel.com/).
2.  登录后，单击 **“New Project”。**
3.  选择您的 **GitHub 存储库**（包含您的分叉项目的存储库），然后单击 **Import（导入**）。
4.  通过添加`.env`文件中的每个键，在 Vercel 控制面板中配置环境变量。
    -   E.g., `NEXT_PUBLIC_GTM`, `NEXT_PUBLIC_APP_URL`, `TELEGRAM_BOT_TOKEN`, etc.
5.  单击 **Deploy**。Vercel 将自动检测您的 Next.js 应用程序并构建它。
6.  部署完成后，您可以访问您的实时网站！

### 部署后更新

每当您将更改推送到 GitHub 存储库时，Vercel 都会自动重新部署应用程序，使您的投资组合保持最新状态。

## 部署到 Netlify：

1.  **注册或登录** [Netlify](https://www.netlify.com/)。
2.  在 **Netlify 仪表板**中，单击**“从 Git 新建站点”。**
3.  连接 **GitHub** 帐户并选择存储库。
4.  通过转到**站点设置>构建和部署>环境**并从您的`.env`文件中添加密钥来配置您的环境变量。
5.  单击 **Deploy Site**。Netlify 将构建和部署您的投资组合。

___

## 教程 🔧

## Gmail 应用密码设置

1.  在 [https://myaccount.google.com/](https://myaccount.google.com/)上**登录您的 Google 帐户**。
2.  导航到 **安全** 从左侧边栏。
3.  向下滚动到**“登录 Google”**部分，并确保两**步验证**已开启。
4.  启用两步验证后，您将看到**一个 App Passwords （应用密码）** 选项。
5.  点击 **App Passwords**。您可能需要再次输入您的 Google 帐户密码。
6.  在**“选择应用程序**”下拉列表中，选择“邮件”，对于**“选择设备**”，选择“其他（自定义名称）”并为其命名（例如，“投资组合”）。
7.  单击 **Generate**。将显示一个 16 个字符的应用程序密码。保存此密码以供以后在环境变量中使用（例如 `GMAIL_PASSKEY`）。

## 创建 Telegram 机器人

1.  **打开 Telegram** 并搜索用户**@BotFather**。
2.  开始与 BotFather 聊天，并使用该`/newbot`命令创建新的机器人。
3.  为您的自动程序选择一个名称。
4.  为您的机器人设置一个唯一的用户名（必须以 结尾，`bot`例如 `PortfolioAssistantBot`， ）。
5.  创建机器人后，BotFather 将向您发送一个 **Token**。保存此令牌，因为您的环境变量（例如 `TELEGRAM_BOT_TOKEN`）将需要它。
6.  要获取您的聊天 ID：
    -   在 Telegram 中打开您的机器人并向其发送消息。
    -   访问以下 URL，替换为`BOT_TOKEN`您的实际机器人令牌：  
        `https://api.telegram.org/bot<BOT_TOKEN>/getUpdates`
    -   在响应中查找包含您的**聊天 ID** `chat` 的对象（您可以将此值用于 `TELEGRAM_CHAT_ID`）。

## 从 dev.to 获取博客

要在作品集中显示 dev.to 的博客文章，请执行以下操作：

1.  将 your `devUsername` in the `utils/data.js` file 设置为 dev.to 用户名。
2.  该应用程序将自动获取您的最新博客文章并将其显示在 **BLOG** 部分。
3.  确保您的博客在 dev.to 上公开可见，并且应用程序将使用 dev.to API 获取它们。

___

## 使用的依赖包📦


[](https://github.com/said7388/developer-portfolio#packages-used-package)

| Used Package List |
| :-: |
| @emailjs/browser |
| @next/third-parties |
| axios |
| lottie-react |
| next |
| nodemailer |
| react |
| react-dom |
| react-fast-marquee |
| react-google-recaptcha |
| react-icons |
| react-toastify |
| sharp |
| sass |
| tailwindcss |

___

## 常见问题：

[](https://github.com/said7388/developer-portfolio#faq)

1.  For those facing the issue of "`next` is not recognized as an internal or external command, operable program or batch file."

Run the following command:

This installs Next.js globally

then do the usual `npm run dev`
