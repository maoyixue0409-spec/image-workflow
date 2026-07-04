# Install And Use / 安装与使用

## Who Can Use This Skill? / 谁可以使用？

Anyone using Codex with local file access can use `image-workflow` to turn local photos and a style library into social-media collage images.

任何使用 Codex 且可以读取本地文件的人，都可以用 `image-workflow` 把本地照片和风格素材库整理成社交媒体拼贴图片。

## Where Can It Be Installed? / 可以安装在哪里？

### 1. Global Codex Skills Folder / Codex 全局 Skills 目录

Install here if you want the skill available in all Codex projects:

如果希望所有 Codex 项目都能使用，安装到这里：

```text
~/.codex/skills/image-workflow/
```

Command:

```bash
mkdir -p ~/.codex/skills
cp -R image-workflow ~/.codex/skills/image-workflow
```

Restart Codex after installation.

安装后重启 Codex。

### 2. Project Skills Folder / 项目内 Skills 目录

Install inside one project if you only want that project to use it:

如果只想让某一个项目使用，可以放在项目内：

```text
your-project/skills/image-workflow/
```

### 3. GitHub Repository / GitHub 仓库

After uploading this folder to GitHub, other users can download it and copy it into their Codex skills folder.

上传到 GitHub 后，其他人可以下载这个文件夹，再复制到自己的 Codex skills 目录。

## How Other People Use It After GitHub Upload / 上传 GitHub 后别人怎么用

### GitHub Website Download / 网页下载

1. Open your GitHub repository.
2. Click `Code`.
3. Click `Download ZIP`.
4. Unzip the file.
5. Copy the `image-workflow` folder into `~/.codex/skills/`.
6. Restart Codex.

中文：

1. 打开你的 GitHub 仓库。
2. 点击 `Code`。
3. 点击 `Download ZIP`。
4. 解压文件。
5. 把 `image-workflow` 文件夹复制到 `~/.codex/skills/`。
6. 重启 Codex。

### Git Clone / Git 命令下载

```bash
git clone https://github.com/YOUR_USERNAME/image-workflow.git
mkdir -p ~/.codex/skills
cp -R image-workflow ~/.codex/skills/image-workflow
```

Replace `YOUR_USERNAME` with the repository owner name.

把 `YOUR_USERNAME` 替换成真实 GitHub 用户名。

## How To Use In Codex / 在 Codex 里怎么用

After installation and restart, start a new Codex thread and write:

安装并重启后，在新的 Codex 对话里输入：

```text
Use image-workflow.
Style keywords: clean multi-photo layout, food cutout
Title: Nan Chang·Jing Dezhen·Xiang Yang
Source photos: /path/to/source-photos
Output count: 2
Confirm the plan before generating.
```

Copy-paste starter:

```text
Use image-workflow.

I want to create social-media collage images from my local photos.
Please help me find matching style references, inspect them, choose a clean background, avoid repeated source photos, and add natural cutouts/text/doodles when suitable.
Show me a short plan first. Do not generate final images until I confirm.

Style keywords:
Title:
Small text:
Source photos folder:
Output count:
Special requirements:
```

中文示例：

```text
使用 image-workflow。
风格关键词：清爽 多图排版，食物抠图
标题：Nan Chang·Jing Dezhen·Xiang Yang
原始照片：/path/to/source-photos
输出数量：2 张
生成前先给我方案确认。
```

中文复制版：

```text
使用 image-workflow。

我想用本地照片生成社交媒体拼贴图片。
请你根据我的风格关键词查找参考图，先查看参考图，再选择干净背景，避免同一张原始照片重复出现，并在合适时加入自然的抠图、文字和涂鸦。
先给我简短方案，等我确认后再生成最终图片。

风格关键词：
标题：
小字：
原始照片文件夹：
输出数量：
特殊要求：
```

## Use Cases / 使用场景

- Travel covers / 旅行封面
- Food and cafe collages / 美食和咖啡馆拼贴
- Lifestyle diary posts / 生活日记图文
- Scrapbook layouts / 手帐拼贴
- Moodboard-based visual exploration / 根据 moodboard 生成视觉方案
- RedNote / Xiaohongshu image posts / 小红书图文
- Personal archive images / 个人照片整理

## What Users Need To Prepare / 使用者需要准备什么

At minimum:

最低需要：

- A folder of source photos.
- A title or theme.
- A requested output count.

Better results:

效果更好时建议准备：

- A style library folder.
- A style index file.
- Element images such as stickers, ribbons, frames, handwritten marks.
- Background images if specific backgrounds are desired.

## If Users Have No Style Library / 如果还没有风格素材库

They can still use the skill. Codex should ask whether to:

没有风格素材库也能用。Codex 应该询问是否：

- Use a simple clean background.
- Use source photos as style references.
- Generate a style description first.
- Use an upstream tool such as Zine Studio to create an original reference board.
