# 她分明是她自己｜莫里索拍卖市场

基于钟家沂、窦莉梅《她分明是她自己——莫里索作品的拍卖市场分析》制作的交互式视觉叙事网页。

## 本地预览

下载或克隆仓库后，直接使用 Chrome、Edge、Safari 或 Firefox 打开 `index.html`。

## 发布到 GitHub Pages

1. 在 GitHub 新建一个公开仓库。
2. 将本文件夹中的全部文件上传到仓库根目录。
3. 打开仓库的 `Settings` → `Pages`。
4. 在 `Build and deployment` 中选择 `Deploy from a branch`。
5. 分支选择 `main`，文件夹选择 `/ (root)`，然后点击 `Save`。
6. 等待 GitHub 完成发布，页面上会显示公开网址。

所有资源均使用相对路径，无需修改即可在 GitHub Pages 运行。

## 项目结构

- `index.html`：网页结构、文章内容及现有内联样式与交互
- `exhibition.css`：作品展览的响应式布局、画作卡片与放大浏览样式
- `exhibition.js`：30 件作品资料、题材筛选、放大切换与触屏手势
- `motion.js`、`motion.css`：视差、错峰入场、筛选重排及灯箱过渡；沿用原有视觉样式
- `INTERACTION_NOTES.md`：参考网页分析、动效参数与验证说明
- `style.css`、`app.js`：保留的旧版独立文件，当前页面不加载
- `assets/`：作品图片与原文图表
- `assets/exhibition/`：从《画作》文档提取的莫里索作品图片
- `article.pdf`：完整原文

## 数据说明

市场分析以所提供 PDF 为数据来源。原文正文与个别图表存在差异时，网页内已标明采用的数据口径。

“回到原文”之后的第 10 章为 Berthe Morisot 作品展览，作品图片、题名、年代、媒介、尺寸及拍卖记录来自《画作》与 Berthe_Morisot_auction_records.docx 两份文档；其中雷诺阿的《抱猫的孩子》未纳入莫里索个展。有成交记录的作品保留拍卖资料；无成交信息的作品不显示拍卖栏目或缺失提示。《午饭后》统一使用正文题名《午餐后》，图下注明这一差异。

展览支持题材筛选、点击放大、左右方向键切换、触屏滑动切换及 Escape 关闭。“减少动态”、系统减少动态设置和“连续阅读”模式均保留内容与浏览功能。图片使用本地相对路径；外部动画库加载失败时，页面使用原生渐入和滚动导航。

新增动效参考 Grotesque 的作品网格入场与灯箱反馈。桌面支持轻微滚动视差、作品悬停缩放、筛选后的平滑重排；手机保留短时渐入与横向滑动换图，纵向滚动不触发换图。动态仅使用位置、缩放和透明度，未改动原配色、字体、间距、作品顺序或内容。详细分析见 [交互说明](INTERACTION_NOTES.md)。

补充资料校对：《捕蝶》使用新增文档图片；原《捉迷藏》误配同一张图片，现使用用户提供的《6.捉迷藏 Cache-cache.jpg》作为配图，尺寸依据[苏富比拍品档案](https://www.sothebys.com/en/auctions/ecatalogue/2005/impressionist-and-modern-art-part-one-n08125/lot.9.html)校正。《捕蝶》的尺寸依据[奥赛博物馆](https://www.musee-orsay.fr/fr/oeuvres/chasse-aux-papillons-309)记录为 46 × 56 cm；《怀特岛上的尤金·马奈》的年代依据[奥赛博物馆展览资料](https://www.musee-orsay.fr/fr/programme/agenda/expositions/presentation/berthe-morisot-1841-1895)由文档的 1885 校正为 1875。新增拍卖记录保留原成交币种。
