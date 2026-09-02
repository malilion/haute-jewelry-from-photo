# Haute Jewelry From Photo

一個將上傳圖片的配色、材質、形狀、光線與氛圍轉譯成頂級珠寶設計的 Codex Skill。每張圖片都會獨立生成一件項鍊、耳環、胸針、手鍊、皇冠或珠寶套組，並搭配專屬精品背景與展示台。

A Codex Skill that translates the palette, material cues, forms, lighting, and mood of each uploaded image into an original haute joaillerie design with a bespoke luxury campaign set.

## Examples

### Deep-Sea Ink Pattern Necklace

The source photograph's pearl white, smoky gray, charcoal patterning, translucent highlights, and cool blue iridescence are translated into platinum wave structures, pavé diamonds, black spinels, moonstones, and a central blue opal.

<p align="center">
  <img src="assets/cuttlefish-haute-jewelry-example.png" alt="Cuttlefish photograph transformed into a deep-sea haute joaillerie statement necklace" width="600">
</p>

The exact top half preserves the source photograph, while the bottom half presents the resulting necklace on a custom crystal-and-stone pedestal.

### Olive-Gold Fin Chandelier Earrings

The source photograph's olive gold, amber yellow, charcoal black, earthy brown, and rusty red palette is translated into yellow gold, black and cognac diamonds, yellow sapphires, chrysoberyl, smoky quartz, and garnets. Its patterned fins become three articulated fan-shaped tiers without literally reproducing a fish.

<p align="center">
  <img src="assets/olive-gold-fin-earrings-example.png" alt="Mottled fish photograph transformed into olive-gold haute joaillerie chandelier earrings" width="600">
</p>

The earrings are presented on a dark bronze stand above polished black-brown stone, with controlled amber reflections and a nocturnal campaign background.

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
├── assets/
│   ├── cuttlefish-haute-jewelry-example.png
│   └── olive-gold-fin-earrings-example.png
├── README.md
└── LICENSE
```

## License

Released under the MIT License. See [`LICENSE`](LICENSE).
