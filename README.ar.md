<div align="center">

# XXD Panel 110｜日系生活场景图鉴

把日常里值得记住的小物，整理成一张会呼吸的生活地图

[![Codex Skill](https://img.shields.io/badge/Codex-Skill-000000?style=flat-square)](./SKILL.md)

</div>

## 样张展示 / Sample works

当前仓库暂不放入未经审核或借用其他 Panel 的图片。首批独立生成并完成方向审核后，再将样张补入此处。

تحمل الصور هوية ومشاعر قوية، لكنها قد تحتاج إلى إعادة تنظيم أكثر قصداً. يحافظ **Panel 110** على واقع الصورة ويترجم النصف الآخر بلغته البصرية المستقلة، لملصقات الفن والنشر المستقل والمعارض والمحتوى الاجتماعي والتصميم الخالص.

يعالج انفصال الصورة عن التصميم، والزخرفة الزائدة، ونقص المساحات البيضاء، وعدم ثبات التسليم بين النسب المختلفة.

- كل صورة تصبح نتيجة مستقلة؛ لا تُدمج الصور.
- المقارنة العمودية أو الأفقية بنسبة 50:50 بدقة ومن دون شريط ثالث.
- تُعالج الصور داخل المجلدات بشكل معزول بلا خلط للموضوع أو النص أو النتائج.
- في `design-only` والخلفيات تُستخدم الصورة كمرجع فقط ولا تظهر الصورة غير المحوّلة.

## الموجّه الأصلي · خمس لغات

[简体中文](references/original-prompt/zh-CN.md) · [English](references/original-prompt/en.md) · [日本語](references/original-prompt/ja.md) · [한국어](references/original-prompt/ko.md) · [العربية](references/original-prompt/ar.md)

简体中文文件逐字保存本项目的原始提示词，并且是运行时唯一的创作与审美权威；其他版本用于阅读、文档与分享。

**关键词：** 生活碎片 · Scene Map · 亚克力收藏质感 · 真实物件 · 动态路线 · 日系治愈留白

## 四种输出模式

- `top-bottom`：3:4 竖版原生结构，现实照片在上，Panel 110 设计在下，严格各占 50%。
- `left-right`：现实照片在左，设计在右，严格各占 50%，不会旋转成上下结构。
- `design-only`：整张画布只呈现本 Panel 的设计转译，照片只作为参考。
- `wallpaper-pack`：按设备分别生成完整画布，不把一张图机械裁成多台设备。

支持多比例、准确像素、文字自动生成／准确文字／无文字、图片目录批量处理，以及 `linked` 或 `independent` 壁纸关系。每次调用只创建一个新任务目录，最终交付为 PNG。

## 开始使用 / Getting started

```bash
git clone https://github.com/nevertoday/xxd-panel-110.git
mkdir -p ~/.codex/skills
ln -s "$(pwd)/xxd-panel-110" ~/.codex/skills/xxd-panel-110
```

也可以直接使用 `npx skills` 安装：

```bash
npx skills add https://github.com/nevertoday/xxd-panel-110 --skill xxd-panel-110
```

该命令会从 GitHub 获取仓库并安装同名 Skill；需要用户级 Codex 安装时，可追加 `--global --agent codex --yes`。安装后重新启动 Agent 会话，然后调用：

```text
$xxd-panel-110
```

完整规范：[SKILL.md](SKILL.md) · [运行适配器](references/xxd-panel-110-prompt.en.md) · [原始提示词](references/original-prompt/zh-CN.md)

## 许可证

本项目采用 **PolyForm Noncommercial License 1.0.0**。完整法律文本见 [LICENSE](LICENSE)，官方页面：<https://polyformproject.org/licenses/noncommercial/1.0.0>。

- 允许个人学习、研究、实验、测试、兴趣项目、私人娱乐，以及符合协议定义的非商业组织使用。
- 非商业用途可以使用、复制、修改、制作衍生作品和分发，但分发时必须附带许可证及作者提供的 `Required Notice:`。
- 禁止商业产品、商业服务、收费交付、出售访问权或预期商业应用；商业使用需另行取得版权方书面许可。
- 仅授予明确写出的著作权与有限专利权，不授予商标权等其他权利，也不能擅自转授权或转让。
- 违约通知后须在 32 天内纠正，否则许可终止；内容按现状提供，不作担保。
