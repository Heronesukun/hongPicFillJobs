# J09 ShouldersUpperArms：肩胸与上臂（P2，建议）

## 结构说明

**肩胸皮肤 TorsoSkin 和上臂 UpperArmR / UpperArmL。** 补的是一字肩荷叶边下面的部分。去掉荷叶边和胸前红带之后，抬臂和呼吸时会露出。

要画的区域（绿色）：

![要画的区域](preview.png)

## 要用的文件

本作业的文件都在这个文件夹里：

- **用 API 的图片编辑功能（可以带蒙版）**：上传 [`input.png`](input.png) 和 [`mask.png`](mask.png)。蒙版中透明的地方就是要画的地方。
- **用对话界面（不能传蒙版）**：上传 [`input_marked.png`](input_marked.png)。图中纯绿色 #00FF00 的区域就是要画的地方。
- **原画参考**：[`context.png`](context.png) 是同一位置的原画；[`preview.png`](preview.png) 在原画上标出了要画的范围。
- **其他工具用的黑白蒙版**：[`mask_bw.png`](mask_bw.png)，白色是要画的地方。
- **尺寸**：1536×1024。生成结果只要保持这个比例，分辨率可以更高。
- **回传文件名**：`returns/J09.png`（放在仓库根目录的 `returns/` 下）

## 提示词

```text
Style lock: this is a crop of an existing anime character illustration (a pastel healing-angel girl). Match it exactly: soft anime cel shading with gentle airbrushed gradients, thin coloured line art (rose-brown on skin, deeper pink on hair, lilac-grey on white cloth), light from the upper left, pastel palette - hair #F5BCCD (shadow #E4A0B7, highlight #FEDFE5), skin #FEF0EC (shadow #F3D1D2, blush #FBD6D5), white cloth #F7F1F5 (lilac shadow #DDCEDB), red ribbon #E53B40, iris blue #7893DB.

This layer shows bare shoulders, chest skin, the arms and the dress bodice; the off-shoulder ruffle and the red ribbon have been removed. Fill the transparent area with continuous bare skin: the shoulders rounding into the upper arms, the upper chest down to the top edge of the bodice, smooth skin where the ribbon was. Keep the light shading (#FEF0EC with #F3D1D2 shadows under the collarbones and at the armpits). Do not draw the ruffle or any clothing.

Edit rules: change ONLY the transparent area (or the pure green #00FF00 area in the marked version). Every other pixel must stay exactly as it is. Keep the flat grey #808080 background; keep the existing outlines of the body and hair, and wherever this part should not exist (outside the body or hair silhouette), paint flat grey #808080 (for full-artwork crops keep the white background). Do not add any other objects, text, borders, drop shadows or glow. Keep the same framing, scale and image size.
```
