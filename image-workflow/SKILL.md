---
name: image-workflow
description: Create social-media collage images from local photo folders and a user-maintained style library. Use when the user provides style keywords, image folders, title copy, or asks for Xiaohongshu/RedNote-style travel, lifestyle, food, diary, scrapbook, or multi-photo cover images with natural backgrounds, food cutouts, handwritten text, and non-stiff doodles.
---

# Image Workflow

## Purpose

Use this skill to create polished social-media collage images from local photos and a reusable style library. It is optimized for Xiaohongshu/RedNote-style travel, lifestyle, food, diary, scrapbook, and multi-photo cover images.

## Expected Project Structure

Prefer these folders under the current project root:

- `素材库/风格/` or `style-library/styles/`: reference style images.
- `素材库/元素/` or `style-library/elements/`: doodles, stickers, frames, ribbons, handwritten elements.
- `素材库/背景/` or `style-library/backgrounds/`: optional reusable backgrounds.
- `素材库/风格索引.md` or `style-library/style-index.md`: short style notes.
- `图文/图片/` or `images/`: final output images.

If the project uses different folders, ask the user for exact paths before generating.

## Required Workflow

1. Extract the user's style keywords, title text, small text, source photo folder, output count, and special requirements.
2. Search the style folder for real filenames matching the style keywords.
3. If multiple style files match, reference all of them and list the exact filenames in the plan.
4. If no style file matches, list nearby filenames and ask the user to choose.
5. Open the referenced style image files before designing. Do not rely only on filenames.
6. Give a short plan and wait for user confirmation before generating.
7. Generate the final image files only after confirmation.
8. Save final images only in the configured output image folder.
9. Remove temporary contact sheets, selection lists, and process images after confirmation or final delivery.

## Pre-Generation Plan

Before generating, show a concise plan:

- Style reference filenames.
- Background source: source photo, style-library background, or simple color background.
- Background treatment.
- Photo layout.
- Food cutout plan.
- Title and small text.
- Doodle and sticker direction.
- Output count and save folder.

## Image Use Rules

- In one final image, each source photo may be used only once.
- If a photo is used as the background, do not use it again as a collage photo, cutout, sticker, or decorative image in the same final image.
- Across a multi-image set, avoid repeating the same background photo when possible.
- If there are not enough suitable photos, ask whether to reduce photo count, add materials, or adjust the concept.

## Background Rules

- Follow explicit user instructions first.
- If the user does not specify a background source, ask whether to use a source photo, a style-library background, or a simple color background.
- Prefer clean scenery photos for backgrounds.
- Do not blur backgrounds by default.
- Use only light color correction, gentle overlays, darkening, or brightening to preserve readability.
- Avoid AI-template-looking backgrounds.

## Text Rules

- Title text may be Chinese or English depending on the content.
- Use the user's exact title when provided.
- Add small text only when useful; if the user does not provide it, generate concise supporting text such as date, place, `travel diary`, or `food & friends`.
- Match the reference style: handwritten, light, natural, attached to the image, or label-like only when the reference supports it.
- Avoid stiff system-font labels, heavy rounded rectangles, large dark text boxes, crowded letter spacing, and text covering the visual center.
- If an English title uses `·`, ensure it renders as a visible round separator. Draw the separator manually if the selected font displays it incorrectly.

## Food Cutout Rules

- Use white-edge sticker treatment by default.
- Do not make every food cutout circular.
- Prefer natural irregular cutouts, original food silhouettes, soft white borders, and subtle shadows.
- Food cutouts must support the visual center, not look randomly pasted.

## Doodle And Sticker Rules

- Prefer existing element images from the element library.
- Avoid stiff geometric shapes that look computer-drawn.
- Doodle density follows the reference style and user requirement.
- Avoid elements that look overly AI-generated, too rigid, or visually inconsistent.

## Output And Cleanup

- Final images go only to the configured output image folder.
- Do not keep contact sheets or temporary reference boards in the final output folder.
- A "version" means one generated set for the same topic.
- If a same-topic workflow reaches three or more generated versions, delete the first two generated versions after confirming the filenames belong to this topic.
- Never delete user source photos, style-library assets, or unrelated files.

## Quality Checklist

Before final delivery, check for:

- Background is not too blurry unless requested.
- Text is not stiff and does not cover faces, food, landmarks, or the visual center.
- The design has a clear center theme and visual weight.
- Style references are reflected.
- Colors are not too gray.
- Food cutouts are believable.
- Doodles are natural, not rigid.
- Layout is not too crowded.
- No source image repeats inside the same final image.
- The background image is not reused in the collage.

## Final Response

Keep the final response short:

- Final image paths.
- Inline previews when supported.
- One short note about the style references and important choices.

