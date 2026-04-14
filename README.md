# SBTI 测试（多语言衍生版）

基于原项目做的静态页衍生版，当前支持三种体验模式：

- `纯中文原版`：尽量保持原始中文互联网语感
- `中英对照`：中文为主，附自然英文，少量必要解释
- `纯英文`：把明显本土梗和例子换成更国际化的说法

另外加了一个可选 `gender` 设置，会轻量影响少数带明显男女语境的题目文案；选 `不透露` 则回到原题写法。

在线地址：

- [https://sbti-test-sigma-flax.vercel.app](https://sbti-test-sigma-flax.vercel.app)

独立仓库：

- [https://github.com/CarlinJunHuang/SBTI-test-multilingual](https://github.com/CarlinJunHuang/SBTI-test-multilingual)

可分享参数：

- `?lang=zh`：中文原版
- `?lang=bi`：中英对照
- `?lang=en`：纯英文
- `?gender=male|female|unspecified`：可选性别文案开关

例如：

- `https://sbti-test-sigma-flax.vercel.app/?lang=en`
- `https://sbti-test-sigma-flax.vercel.app/?lang=bi&gender=female`

已知限制：

- 人格结果海报图仍然沿用原版图片资源，所以图内嵌的字还是中文
- 项目仍然是纯静态站点，核心逻辑集中在 `index.html`

SEO / 分享卡片：

- 已补基础 meta tags、Open Graph、Twitter Card、canonical、robots.txt、sitemap.xml
- 首页会根据 `lang` 参数同步标题、描述和 canonical
- 首页 footer 有一条很轻的 trust 文案，说明本项目保持原题体验，只做多语化衍生，并附 repo 链接

本地预览：

```bash
python3 -m http.server 4173
```

然后打开 [http://127.0.0.1:4173](http://127.0.0.1:4173)。

注意：建立这个 repo 只是因为网页本身就是全部源码。原作者并未声明 license，所以本仓库也不附带 license；如果你要继续传播、改编或商用，请自行斟酌，尽量不要给原作者添麻烦。

原项目地址：https://sbti.unun.dev  
原作者：[B站@蛆肉儿串儿](https://www.bilibili.com/video/BV1LpDHByET6/)
