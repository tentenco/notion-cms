<img src="Nobelium-Logo.svg" width="50" height="50">

# Nobelium

一個使用 NextJS + Notion API 實現的，部署在 Vercel 上的靜態部落格系統。為 Notion 和所有創作者設計。

<p>
  <a aria-label="GitHub commit activity" href="https://github.com/craigary/nobelium/commits/main" title="GitHub commit activity">
    <img src="https://img.shields.io/github/commit-activity/m/craigary/nobelium?style=for-the-badge">
  </a>
  <a aria-label="GitHub contributors" href="https://github.com/craigary/nobelium/graphs/contributors" title="GitHub contributors">
    <img src="https://img.shields.io/github/contributors/craigary/nobelium?color=orange&style=for-the-badge">
  </a>
  <a aria-label="Build status" href="#" title="Build status">
    <img src="https://img.shields.io/github/deployments/craigary/nobelium/Preview?logo=Vercel&style=for-the-badge">
  </a>
</p>

[中文說明 / [English](README.md)]

Demo地址：[https://knowledge.tenten.co/](https://knowledge.tenten.co/)

<details><summary> 截圖</summary>
<img src="https://github.com/craigary/nobelium/blob/main/desktop.png?raw=true">
</details>

## 亮點 ✨

**🚀 &nbsp;秒開，設備全適配**

- 快速的頁面渲染和響應式設計
- 高效編譯器的快速靜態頁面生成

**🤖 &nbsp;自動，無需重新部署**

- 部署在免費、高速的 Vercel 平台
- 支持增量式更新，更新文章后無需重複部署

**🚙 &nbsp;全功能，完全不操心**

- 評論、寬頁面、搜索和標籤
- 訂閱、網站統計、Web Vital 分析…… 還有更多功能待你發現

**🎨 &nbsp;美觀，輕鬆自定義**

- 豐富的配置項，更支持多語言
- 使用 Tailwind CSS，輕鬆實現二次開發

**🕸 &nbsp;網址美觀、搜索引擎優化**

## 快速起步

- 給這個項目點個小星星 😉
- 將 [這個 Notion 模板](https://www.notion.so/68be9021bca34b8e89f0246f27e608df) 製作副本，並分享這個頁面給所有人
- [Fork](https://github.com/craigary/nobelium/fork) 這個項目
- 在 `blog.config.js` 配置相關選項
- _(可選)_ 用自己的圖片替換 `/public` 資料夾里的 `avatar.svg`、`favicon.svg` 和 `favicon.ico`
- 在 [Vercel](https://vercel.com) 上部署這個項目, 設定一下環境變數：
  - `NOTION_PAGE_ID`: 你剛剛分享出去的 Notion 頁面網址中的頁面 ID，通常是網址中工作區地址后的 32 位字元串
  - `NOTION_ACCESS_TOKEN`（可選）: 如果你決定不分享你的資料庫，你可以使用 token 來讓 Nobelium 從 Notion 資料庫中抓取數據。你可以在你的瀏覽器 cookies 中找到它，名稱是 `token_v2'。
    - Notion token 的有效期只有 180 天，請確保在 Vercel Dashboard 上手動更新，我們可能會在未來切換到官方 API 來解決這個問題。此外，如果資料庫是非公開到，Notion 中的圖片可能無法正常顯示到網頁上。
- **稍微等等就可以訪問了！** 簡單嗎?

<details><summary>等等，什麼是 Page ID？</summary>
  <img src="https://github.com/craigary/nobelium/blob/main/pageid.png?raw=true">
</details>

## Roadmap

在這裡看看我們的 [Roadmap](https://www.notion.so/craigary/Public-Roadmap-3cfc4d0f0ca642ef8f652673c37add22)

- [x] 搜索引擎優化
- [x] 深色模式
- [x] Open Graph 支持
- [x] 切換到 react-notion-x
- [ ]  網站地圖
- [ ] ...

## 技術細節

- **生成**: Next.js SSG 和 Incremental Static Regeneration
- **頁面渲染**: [React-notion-x](https://github.com/NotionX/react-notion-x)
- **樣式**: Tailwind CSS 和 `@tailwindcss/jit` compiler
- **評論**: Gitalk，更多評論系統還在路上

## 特別感謝

<table>
<tr align="left">
    <td align="center"><a href="https://notion.so/cnotion"><img src="https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F815be1aa-a8bf-46d0-887e-a1c9d18d8ae9%2Fnotion-logo-no-background.png?table=block&id=e1826899-1cd1-4de8-9b1c-ad0de60baa91&width=250&userId=1f77c970-e682-4c02-b9e8-4164924f04ab&cache=v2" width="80px;" alt=""/><br /><sub><b>Notion 中文社區</b></sub></a></td>
    <td align="center"><a href="https://twitter.com/SilentDepthCN"><img src="https://avatars.githubusercontent.com/u/7194254?s=460&u=d8c805acedf5c49ab8e1bfde58b16d7b7fe2b1bb&v=4" width="80px;" alt=""/><br /><sub><b>SilentDepth</b></sub></a></td>
    <td align="center"><a href="https://leerob.io"><img src="https://avatars.githubusercontent.com/u/9113740?s=460&u=6b5c9843f6d345ee178d1171dd3025610312af35&v=4" width="80px;" alt=""/><br /><sub><b>Lee Rob</b></sub></a></td>
    <td align="center"><a href="https://spencerwoo.com"><img src="https://avatars.githubusercontent.com/u/32114380?s=460&u=81d1f9754f354c63ece17a83196be14b51ee1056&v=4" width="80px;" alt=""/><br /><sub><b>Spencer Woo</b></sub></a></td>
  </tr>
</table>

## 貢獻者

<table>
<tr align="left">
    <td align="center"><a href="https://github.com/craigary"><img src="https://avatars.githubusercontent.com/u/10571717?s=64&v=4" width="80px;" alt=""/><br /><sub><b>Craig Hart</b></sub></a><br /><a href="https://github.com/craigary/nobelium/commits?author=craigary" title="Owner">🎫 🔧 🎨 🐛</a></td>
    <td align="center"><a href="https://github.com/reycn"><img src="https://avatars.githubusercontent.com/u/11225092?s=64&v=4" width="80px;" alt=""/><br /><sub><b>Reynard</b></sub></a><br /><a href="https://github.com/craigary/nobelium/commits?author=reycn" title="Owner"> 🎨 🐛</a></td>
    <td align="center"><a href="https://github.com/Niinjoy"><img src="https://avatars.githubusercontent.com/u/39721307?s=64&v=4" width="80px;" alt=""/><br /><sub><b>Niin</b></sub></a><br /><a href="https://github.com/craigary/nobelium/commits?author=Niinjoy" title="Owner">🔧 🐛</a></td>
    <td align="center"><a href="https://github.com/ruter"><img src="https://avatars.githubusercontent.com/u/8568876?s=64&v=4" width="80px;" alt=""/><br /><sub><b>Ruter</b></sub></a><br /><a href="https://github.com/craigary/nobelium/commits?author=ruter" title="Owner">🔧 🐛</a></td>
  </tr>
</table>

## License

The MIT License.
