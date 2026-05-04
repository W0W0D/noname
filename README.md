# noname
## 简介

- 本仓库为基于基于 [adeFuLoDgu](https://github.com/adeFuLoDgu) 的无名杀仓库的(https://github.com/Viridian8520/noname)无名杀仓库自改的无名杀
- [本体仓库](https://github.com/libnoname/noname) 或者 [adeFuLoDgu仓库](https://github.com/adeFuLoDgu/noname) 有更新会基本保持同步更新
- 斯~本体库是原版，这就有兼容性问题。隔壁的β版更新慢，不过公众号很活跃，新武将的扩展都有。我先试试本体库更新后能不能用 不能用就换成β试试 反正五一闲着没事干
- 

## 项目本体版本

- v1.11.0

## 自改内容






## 启动方法

- 环境要求
> **提示：** 请参考 [本地文档](./docs/how-to-start.md) 或 [github文档](https://github.com/libnoname/noname/wiki/%E5%A6%82%E4%BD%95%E8%BF%90%E8%A1%8C%E6%97%A0%E5%90%8D%E6%9D%80%EF%BC%88%E7%A8%8B%E5%BA%8F%E5%91%98%E7%89%88%EF%BC%89) 配置环境。
  - [Node.js](https://nodejs.org/) ^20.19.0 || >=22.12.0
  - [pnpm](https://pnpm.io/) >= 9
  - Webview: Chromium >= 91 || Safari >=16.4.0 (暂不支持Firefox)

- 安装环境完成后，下载/克隆仓库到本地，用终端打开项目根目录后，输入如下命令后即可本地游玩

  ```
  pnpm install
  pnpm start
  ```

  之后再启动只需输入 `pnpm serve` 即可本地游玩

- 如果想要在线游玩/在客户端游玩，需要输入如下命令对项目进行构建，构建后的产物均位于 `dist` 目录下

  ```
  pnpm build:full
  ```

- 启动联机服务：将 `scripts/server.js` 重命名为 `server.cjs` 后，在根目录输入如下命令即可

  ```
  node scripts/server.cjs
  ```

- 将构建后的产物部署至服务器后即可在线游玩

- 将构建后的产物打包成压缩包，然后通过本体官方客户端进行导入即可在客户端游玩

## 客户端下载

- 安卓： <https://github.com/nonameShijian/noname-shijian-android/releases/tag/v1.6.8>
- PC:  <https://github.com/nonameShijian/noname/releases/tag/v1.75>

## 游玩环境

- 网页端推荐使用 Chrome 系内核浏览器游玩，暂不支持 Firefox 浏览器
- 请尽量保证游玩的 Chrome 系浏览器或手机 Webview 的内核版本大于等于91

## 已知问题

- 皮肤切换扩展报错 `Cannot read properties of undefined (reading 'chuchang')`（解决方法：菜单 -> 选项 -> 其他 -> 重置游戏设置）
- 开启皮肤切换扩展会导致动皮出框特效偏移（解决方法：PC端请将游戏本体内置的缩放率调整回100%，再用浏览器自带的缩放功能进行缩放即可；移动端请参考 [无名杀特效偏移/特效错位的解决方法](https://www.bilibili.com/video/BV1Ggwze4EAN) 对手机 WebView 降级至 128 以下版本即可）

## 在线部署地址

- Github Pages：https://viridian8520.github.io/noname/
