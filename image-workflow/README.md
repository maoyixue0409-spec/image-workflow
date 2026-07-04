# image-workflow

English | [中文](#中文)

`image-workflow` is a Codex skill for creating social-media collage images from local photos and a user-maintained style library.

It is designed for:

- Xiaohongshu / RedNote travel covers
- Lifestyle diary collages
- Food and cafe photo layouts
- Scrapbook-style multi-photo posts
- Clean handwritten-title image compositions

## What It Does

The skill guides Codex to:

1. Search real style-reference filenames from a local style library.
2. Inspect selected reference images before designing.
3. Propose a short plan before generating.
4. Avoid repeating the same source photo in one final image.
5. Use natural backgrounds, food cutouts, handwritten text, and non-stiff doodles.
6. Save only final images to the configured output folder.

## Recommended Project Structure

```text
your-project/
├── style-library/
│   ├── styles/
│   ├── elements/
│   ├── backgrounds/
│   └── style-index.md
├── source-photos/
└── images/
```

Chinese folder names are also supported:

```text
your-project/
├── 素材库/
│   ├── 风格/
│   ├── 元素/
│   ├── 背景/
│   └── 风格索引.md
├── 原始照片/
└── 图文/图片/
```

## Install

Copy this folder into your Codex skills directory:

```bash
mkdir -p ~/.codex/skills
cp -R image-workflow ~/.codex/skills/image-workflow
```

Restart Codex after installation.

More install options are documented in [docs/install-and-use.md](docs/install-and-use.md).

## Example Prompt

```text
Use image-workflow.
Style keywords: clean multi-photo layout, food cutouts
Title: Nan Chang·Jing Dezhen·Xiang Yang
Small text: 2025 travel diary
Source photos: /path/to/source-photos
Output: 2 images
Confirm the plan before generating.
```

## Copy-Paste Starter Prompt

Use this prompt after installing the skill:

```text
Use image-workflow.

I want to create social-media collage images from my local photos.
Please help me:
1. Find matching style references from my style library based on my style keywords.
2. Inspect the reference images before designing.
3. Choose a clean background without heavy blur unless I ask for blur.
4. Make sure each source photo appears only once in each final image.
5. Add natural food cutouts, handwritten-style text, and non-stiff doodles when suitable.
6. Show me a short plan first. Do not generate final images until I confirm.

Style keywords:
Title:
Small text:
Source photos folder:
Output count:
Special requirements:
```

Short trigger:

```text
Use image-workflow. Help me turn this photo folder into clean social-media collage images. Ask for missing details and show a plan before generating.
```

## Use Cases

`image-workflow` can be used for:

- Travel diary covers.
- Food trip collages.
- Cafe and lifestyle posts.
- Scrapbook-style photo layouts.
- RedNote / Xiaohongshu image posts.
- Moodboard-guided social media visuals.
- Personal archive and memory collage images.

See [docs/install-and-use.md](docs/install-and-use.md) for detailed usage scenarios.

## Style Library

Users should create their own style library with images they own or are allowed to use.

Recommended categories:

- `styles/`: complete reference layouts.
- `elements/`: stickers, doodles, ribbons, frames, handwritten marks.
- `backgrounds/`: clean scenery, texture, paper, fabric, or color backgrounds.
- `style-index.md`: short notes describing when each style image works best.

Do not include private photos, copyrighted Pinterest images, or unlicensed assets in a public repository.

## Zine Studio Integration

If you use a tool like Zine Studio to generate style descriptions or original reference boards, use it as an upstream style-library builder:

1. Generate a style description or original reference board in Zine Studio.
2. Save the reference board into `style-library/styles/`.
3. Add a short note to `style-library/style-index.md`.
4. Ask Codex to use `image-workflow` with those style keywords.

See [docs/zine-studio-integration.md](docs/zine-studio-integration.md).

## Privacy And Copyright

This repository intentionally does not include personal photos or proprietary reference images. Use your own source photos and assets, or materials you have permission to use.

## License

This project uses the MIT License. In simple terms: people can use, copy, modify, and share it, but the original license notice should remain, and the project is provided without warranty.

See [docs/license-explained.md](docs/license-explained.md).

---

# 中文

`image-workflow` 是一个 Codex skill，用于根据本地照片和用户自己的风格素材库，生成社交媒体拼贴图片。

适合：

- 小红书 / RedNote 旅行封面
- 生活日记拼贴
- 美食和咖啡馆图文
- 手帐 / 拼贴 / Scrapbook 风格多图
- 清爽手写标题图片

## 它能做什么

这个 skill 会引导 Codex：

1. 根据风格关键词，从本地风格库里检索真实文件名。
2. 先查看选中的参考图，再进行设计。
3. 生成前先给出简短方案。
4. 避免同一张照片在一张成品里重复出现。
5. 使用自然背景、食物抠图、手写感文字和不生硬的涂鸦。
6. 只把最终图保存到指定图片文件夹。

## 推荐目录结构

```text
你的项目/
├── 素材库/
│   ├── 风格/
│   ├── 元素/
│   ├── 背景/
│   └── 风格索引.md
├── 原始照片/
└── 图文/图片/
```

也支持英文目录：

```text
your-project/
├── style-library/
│   ├── styles/
│   ├── elements/
│   ├── backgrounds/
│   └── style-index.md
├── source-photos/
└── images/
```

## 安装

把整个文件夹复制到 Codex skills 目录：

```bash
mkdir -p ~/.codex/skills
cp -R image-workflow ~/.codex/skills/image-workflow
```

安装后重启 Codex。

更多安装方式见 [docs/install-and-use.md](docs/install-and-use.md)。

## 示例指令

```text
使用 image-workflow。
风格关键词：清爽 多图排版，食物抠图
标题：Nan Chang·Jing Dezhen·Xiang Yang
小字：2025 travel diary
原始照片：/path/to/source-photos
输出：2 张
生成前先给我方案确认。
```

## 复制即用启动词

安装 skill 后，可以直接复制这段：

```text
使用 image-workflow。

我想用本地照片生成社交媒体拼贴图片。
请你帮我：
1. 根据我的风格关键词，从我的风格素材库里找到匹配的参考图。
2. 先查看参考图，再设计。
3. 背景默认保持干净，不要明显模糊，除非我明确要求模糊。
4. 每张成品图里，同一张原始照片只能出现一次。
5. 合适时加入自然的食物抠图、手写感文字和不生硬的涂鸦。
6. 先给我简短方案，等我确认后再生成最终图片。

风格关键词：
标题：
小字：
原始照片文件夹：
输出数量：
特殊要求：
```

最短触发词：

```text
使用 image-workflow。帮我把这个照片文件夹做成清爽的社交媒体拼贴图，缺什么先问我，生成前先给方案。
```

## 使用场景

`image-workflow` 可以用于：

- 旅行图文封面。
- 美食旅行拼贴。
- 咖啡馆 / 生活方式图文。
- 手帐拼贴风图片。
- 小红书 / RedNote 图文。
- 根据 moodboard 生成社媒视觉。
- 个人照片整理和回忆拼贴。

详细场景见 [docs/install-and-use.md](docs/install-and-use.md)。

## 风格素材库

建议用户自己建立风格素材库，并只使用自己拥有或有权使用的素材。

推荐分类：

- `风格/`：完整排版参考图。
- `元素/`：贴纸、涂鸦、丝带、边框、手写字元素。
- `背景/`：干净风景、纸张、布料、墙面、天空或纯色背景。
- `风格索引.md`：记录每张风格图适合什么场景。

不要把私人照片、未经授权的 Pinterest 图、未授权素材上传到公开仓库。

## 和 Zine Studio 搭配

如果你有类似 Zine Studio 的网页工具，可以把它作为上游“风格描述 / 原创参考板生成器”：

1. 在 Zine Studio 里生成风格描述或原创参考板。
2. 把参考板保存到 `素材库/风格/` 或 `style-library/styles/`。
3. 在 `风格索引.md` 或 `style-index.md` 里写一句用途说明。
4. 再让 Codex 用 `image-workflow` 根据这些关键词生成图片。

详见 [docs/zine-studio-integration.md](docs/zine-studio-integration.md)。

## 隐私和版权

这个仓库默认不包含私人照片或专有参考图。请使用自己的照片、自己生成的素材，或已经获得授权的素材。

## License

本项目使用 MIT License。简单说：别人可以使用、复制、修改和分享，但要保留原始许可说明；作者不对使用结果承担保证责任。

详见 [docs/license-explained.md](docs/license-explained.md)。
