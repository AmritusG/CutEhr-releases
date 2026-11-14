# CutEhr

Live person cutout and colour correction for **Resolume Arena** on Apple silicon Macs. Free download, by Creativeations.

CutEhr finds the people in your live feed or clip, on the Mac itself, with no model download and no internet connection. It ships with
a second plugin, **GradEhr**, which is the same colour corrector without the people detection, for any feed.

**[Download the latest release](https://github.com/AmritusG/CutEhr-releases/releases/latest)**

| Bundle | Shows up in Arena as | What it does |
|---|---|---|
| `CutEhr.bundle` | **CutEhr** (Effects) | Person cutout, matte, skeleton, hands and face, plus live colour correction that can target the person or the background. |
| `GradEhr.bundle` | **GradEhr** (Effects) | The same colour corrector for any clip, layer or camera. |

## CutEhr

- **Person cutout and matte.** Cut the people out of the picture with a clean alpha edge, or show the mask itself as a grey matte.
  Feather, Choke, Threshold and Invert shape the edge.
- **Skeleton, hands and face.** Draw the body pose, the hands (up to 6) and the face landmarks over the picture, over the cutout or on
  their own, each with its own colour, line width, glow and trail. Smoothing keeps the lines steady.
- **Per-person colours.** Give every tracked person their own colour, or pull out one person's matte. Each person keeps their colour
  as they move around.
- **Edge treatments.** Edge Refine (the mask follows hair and fine edges in the picture), Fill Holes, Speck Removal, Temporal Smooth
  (a steady edge with no flicker), Mask Motion Comp (the edge keeps up with fast motion) and an Edge Glow around the person.
- **Live colour correction.** Exposure, temperature and tint, a white-balance picker, lift / gamma / gain and shadows / midtones /
  highlights wheels, contrast, saturation, vibrance, highlight roll-off, black and white point, and dehaze.
- **Automatic white balance.** Gray World, White Patch, Gray Edge, or **Skin**: white balance taken from the faces in the picture.
  The estimate adapts smoothly, and you can hold it or reset it.
- **Person-only correction.** Correct the whole frame, only the person, only the background, or each by its own amount. Skin Protect
  keeps skin natural while the grade changes the rest.
- **Detection boost.** On dark or smoky stages, CutEhr can show its detector a brightened, corrected copy of the picture, so it still
  finds the people. The picture you output stays as you graded it.
- **Picture + Mask in Alpha.** Outputs the corrected full picture with the person mask in the alpha channel, ready for the next effect
  in the chain to use.

## GradEhr

The full CutEhr colour corrector (manual controls, wheels, tone, dehaze and automatic white balance with Gray World, White Patch or
Gray Edge) as its own effect for any feed. It does no people detection.

## Requirements

- A Mac with **Apple silicon** (M1 or later). There is no Intel build.
- **macOS 12** Monterey or later (tested on macOS 27).
- **Resolume Arena 7** (tested on Arena 7.28.1).

The bundles are signed with a Developer ID and notarised by Apple.

## Install

1. Download `CutEhr-<version>.zip` from [Releases](https://github.com/AmritusG/CutEhr-releases/releases) and unzip it.
2. Quit Arena.
3. Copy `CutEhr.bundle` and `GradEhr.bundle` into `~/Documents/Resolume Arena/Extra Effects/` (create the folder if it is not there).
4. Start Arena. **CutEhr** and **GradEhr** appear under Effects. Arena loads a new or replaced plugin only at start.

## Coming soon: CamEhr

CamEhr is a family of live camera looks for Arena. It reads CutEhr's person mask, so each look can hit the whole frame, only the
person, or only the background.

## Licence

Free to use, including paid and commercial VJ work. Not open source: see [LICENSE](LICENSE). Parts made by others are listed in
[THIRD-PARTY-NOTICES.md](THIRD-PARTY-NOTICES.md).

© 2026 Creativeations / Amrit Rosell. Resolume and Arena are trademarks of Resolume. CutEhr is an independent product and is not made
or endorsed by Resolume.
