# 云账审计

单页静态站。入口是 `index.html`，样式在 `style.css`，提交成功页是 `thanks.html`。

上线前替换这三处：

1. `index.html` 里表单的 `FORMSPREE_ENDPOINT`，换成 `https://formspree.io/f/你的表单ID`
2. 页脚的 `[你的名字]`
3. 页脚和表单旁的 `[你的邮箱]`，以及两处 `mailto:you@example.com`

## GitHub Pages

仓库根目录就是本目录，`index.html` 放在根上，不要再套一层文件夹。

1. 在 GitHub 新建空仓库，把本目录推上去。
2. Settings → Pages → Build and deployment → Source 选 `Deploy from a branch`。
3. Branch 选 `main`，文件夹选 `/ (root)`，保存。
4. 等一两分钟，打开 `https://<用户名>.github.io/<仓库名>/`。

`.nojekyll` 用来避开 Jekyll 处理。页面没有构建步骤。

Formspree 第一次提交要到邮箱里确认激活。站点域名确定后，把 `thanks.html` 的完整地址填进 Formspree 的跳转允许范围。页面脚本会按当前域名自动写绝对地址，项目页（带仓库名的路径）也能跳对。

弱字和链接色比原稿各深了一档（`#72716e`、`#5e6e6a`），米白底上才读得清。案例里的比例是按需求写的脱敏示例，上线前换成你自己的真实案例。
