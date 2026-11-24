# 产品图工作室 · Product Image Studio

一个用于产品概念图、套图和局部修图的中文 Codex Skill。从手机壳、创口贴、挂钟与头盔的概念图实践中，提炼如何锁定同一产品、按用途安排镜头，并逐张核对结构与文字。

同一产品换了视角或配色，仍需要保留可辨认的设计细节。手机壳换到侧面后，按键和镜头孔应与主图对应。挂钟换配色后，刻度和轴心应留在原位。每张图先写清用途、必须保留的细节和允许的变化，再据此检查结果。

## 使用

在启用了生图或编辑能力的 Codex 中，将此仓库放入个人技能目录。Codex 的目录规则见 [官方 Skill 文档](https://learn.chatgpt.com/docs/build-skills)。

```bash
mkdir -p ~/.agents/skills
git clone https://github.com/lilyallison5470-commits/product-image-studio.git ~/.agents/skills/product-image-studio
```

上传自己的参考图，在新会话中尝试以下请求。

```text
用 $product-image-studio 为附件中的手机壳做三张产品图。
先展示完整背面，再展示侧键和镜头边框。三张保持开孔、配色和版式一致。
用浅灰背景和大面积柔光，按 4:5 分别交付。
```

需要局部修改时也可直接说明范围，例如「只去掉左上角的杂光，沿用原构图」。只需要提示词时可在请求中指定。实际出图依赖当前会话可用的生成或编辑工具。

## 仓库内容

- [核心 Skill](SKILL.md) 包含任务判断、参考图使用、文字控制、成图检查和交付要求。
- [拍摄方案](references/shot-recipes.md) 包含四类产品的镜头安排与具体检查点，可按项目选用。

仓库公开的是工作流程和文字示例。参考照片与原始项目图由使用者从自己的素材中提供。

## 许可证

[MIT License](LICENSE)
