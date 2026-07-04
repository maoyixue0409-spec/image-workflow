# Zine Studio Integration / 和 Zine Studio 搭配

## Relationship / 两者关系

`Zine Studio` and `image-workflow` solve different parts of the creative process.

`Zine Studio`:

- Generates style descriptions.
- Helps build original reference boards.
- Plans zine structures, visual moods, and prompts.
- Works well as an upstream style-library builder.

`image-workflow`:

- Uses a local style library and source photos.
- Searches exact style-reference filenames.
- Creates confirmed image plans.
- Generates final social-media collage images.

中文理解：

- `Zine Studio` 更像“风格方案 / 原创参考板 / Prompt 生成器”。
- `image-workflow` 更像“根据素材和风格真正生成拼贴图的 Codex 工作流”。

## Recommended Workflow / 推荐流程

1. Use Zine Studio to generate a style description or original reference board.
2. Save the reference board into `style-library/styles/` or `素材库/风格/`.
3. Add a short note to `style-index.md` or `风格索引.md`.
4. Put reusable doodles, stickers, frames, and ribbons into `style-library/elements/` or `素材库/元素/`.
5. Ask Codex to use `image-workflow` with the matching style keywords.

## What Not To Do / 不建议

- Do not copy private Zine Studio user uploads into a public repository.
- Do not publish unlicensed inspiration images.
- Do not make `image-workflow` depend on a specific personal folder path.

## Future Integration Ideas / 后续可整合方向

- Add an export button in Zine Studio that writes `style-index.md` entries.
- Export style board images into a `style-library/styles/` folder.
- Export image-generation briefs that can be pasted directly into Codex.
- Add a "Use with image-workflow" prompt template.

