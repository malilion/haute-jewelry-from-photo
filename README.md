# Haute Jewelry From Photo

一個將上傳圖片的配色、材質、形狀、光線與氛圍轉譯成頂級珠寶設計的 Codex Skill。每張圖片都會獨立生成一件項鍊、耳環、胸針、手鍊、皇冠或珠寶套組，並搭配專屬精品背景與展示台。

A Codex Skill that translates the palette, material cues, forms, lighting, and mood of each uploaded image into an original haute joaillerie design with a bespoke luxury campaign set.

## What it does

- Processes every uploaded image independently.
- Extracts the image's visual DNA instead of copying it literally.
- Produces physically plausible, photorealistic haute joaillerie.
- Uses a strict vertical 3:4 canvas with an exact 50/50 horizontal split.
- Preserves the source image in the top half and presents the jewelry in the bottom half.
- Selects gemstones, precious metals, pedestal materials, background, and lighting from the source image.
- Avoids text, fake branding, copied luxury-house designs, and generic e-commerce styling.

## Install

Clone or copy this repository to:

```text
~/.codex/skills/haute-jewelry-from-photo
```

Keep `SKILL.md` and `agents/openai.yaml` together. Restart Codex if the new Skill is not detected immediately.

## Use

Upload one or more images and invoke:

```text
$haute-jewelry-from-photo

Turn this image into a statement necklace.
```

Or let the Skill choose the best jewelry category:

```text
$haute-jewelry-from-photo

Create an extravagant haute joaillerie design inspired by this image.
```

Each uploaded image produces one independent composition in the same order.

## Composition contract

- Canvas: vertical 3:4.
- Top 50%: original inspiration image.
- Bottom 50%: haute jewelry showcase.

The full generation behavior and quality checks are defined in [`SKILL.md`](SKILL.md). UI metadata lives in [`agents/openai.yaml`](agents/openai.yaml).

## Repository layout

```text
.
├── SKILL.md
├── agents/
│   └── openai.yaml
├── README.md
└── LICENSE
```

## License

Released under the MIT License. See [`LICENSE`](LICENSE).
