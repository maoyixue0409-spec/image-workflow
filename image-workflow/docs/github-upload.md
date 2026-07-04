# Upload To GitHub / 上传到 GitHub

## Before Uploading / 上传前检查

Make sure the repository does not include:

- Private photos.
- Personal travel albums.
- Unlicensed Pinterest images.
- API keys or `.env` files.
- Generated images that contain private people or copyrighted assets.

确认不要上传：

- 私人照片。
- 个人旅行相册。
- 未授权的 Pinterest 图片。
- API Key 或 `.env` 文件。
- 包含真人隐私或版权素材的生成图。

## Recommended Upload Methods / 推荐上传方式

### Option A: GitHub Website / 用 GitHub 网页上传

1. Create a new repository on GitHub.
2. Choose a repository name, for example `image-workflow`.
3. Keep it public if you want it open-source.
4. Upload all files from this folder.
5. Check that `README.md`, `SKILL.md`, `LICENSE`, and `.gitignore` are visible.

### Option B: Git Command Line / 用 Git 命令上传

Run these commands inside the `image-workflow` folder:

```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/image-workflow.git
git push -u origin main
```

Replace `YOUR_USERNAME` with your GitHub username.

## After Uploading / 上传后

Add topics to the repository:

- `codex`
- `skill`
- `image-workflow`
- `xiaohongshu`
- `rednote`
- `collage`
- `creative-tools`

You can also add screenshots later, but only use non-private examples.

