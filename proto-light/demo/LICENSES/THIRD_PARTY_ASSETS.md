# Third-party assets: licences and sources (verified online 2026-10-20)

The original pack downloads (and their licence files) used to sit in `assets/thirdparty/<pack>/` (never exported).
They were removed from the repo on 2026-10-29 (cleanup 1029e, never loaded by the game); recover them with
`git checkout 5267328 -- assets/thirdparty`. Every pack below is CC0 1.0 (licence text: link at the bottom).
"Verified" means the OpenGameArt page was fetched on 2026-10-20 and showed the licence below.

| Pack | Author | Licence | Source (verified) | Local archive (until 1029e) | Used for (shipped, derived sprites) |
|---|---|---|---|---|---|
| Sideview Sci-Fi – Patreon Collection | Luis Zuno (ansimuz) | CC0 1.0 | https://opengameart.org/content/sideview-sci-fi-patreon-collection | `ansimuz_sideview_scifi/` (LICENSE.txt + author's public-license.txt) | Space Marine -> heroes `player`/`player2`, `soldier`, `soldier_life`, `sniper`, `shieldtrooper`, `jetter`; Sci-Fi Interior Platform -> metal rows of `tiles`, `tiles_snow`, `tiles_rail`, `tiles_citadel`. (Colour palettes sampled from other sprites of the pack: colours only.) |
| Mountain at Dusk Background | ansimuz | CC0 1.0 | https://opengameart.org/content/mountain-at-dusk-background | `ansimuz_mountain_dusk/` | nothing shipped any more (S2/S3 backgrounds are AI/PixelEngine art) |
| Industrial Parallax Background | ansimuz | CC0 1.0 | https://opengameart.org/content/industrial-parallax-background | `ansimuz_industrial/` | nothing shipped any more |
| Warped Sci-Fi Lab | ansimuz | CC0 1.0 | https://opengameart.org/content/warped-sci-fi-lab | `ansimuz_warped_scifi_lab/` | `bg_cit_shaft` (S4 lift shaft) |
| Animated Explosions | ansimuz | CC0 1.0 | https://opengameart.org/content/animated-explosions | `ansimuz_explosions/` | `explosion_b`, `explosion_s` (as is) |
| Warped Shooting FX | ansimuz | CC0 1.0 | https://opengameart.org/content/warped-shooting-fx | `ansimuz_warped_shooting_fx/` | `spark` (redrawn from hits-1) |

## No longer shipped (removed from the repo in 1029e)

| Pack | Author | Licence | Source | Local archive | Used for |
|---|---|---|---|---|---|
| Living Tissue Background | ansimuz | CC BY 3.0 | https://opengameart.org/content/living-tissue-background | `ansimuz_living_tissue_bg/` | nothing shipped since lot2 (2026-10-23) |
| Living Tissue Platform Tileset | ansimuz | CC BY 3.0 | https://opengameart.org/content/living-tissue-platform-tileset | `ansimuz_living_tissue_platform/` | nothing shipped since lot2 (2026-10-23) |

The derived files (`tiles_hive`, `bg3_mid`, `bg3_near`) are gone too; the S5 art is AI-made since v41. Only a colour palette sampled from these packs remains (v12 "flesh"
enemies: egg, larva, spitter), with no pixels reused.

## Licence texts
- CC BY 3.0: https://creativecommons.org/licenses/by/3.0/legalcode
- CC BY 4.0: https://creativecommons.org/licenses/by/4.0/legalcode
- CC0 1.0: https://creativecommons.org/publicdomain/zero/1.0/legalcode
- Godot Engine (MIT) and its third-party components: `GODOT_LICENSE.txt`, `GODOT_COPYRIGHT.txt` (from godotengine/godot).

## Not third-party
- Code, levels, music and SFX: written or generated for this project (`tools/audio`, numpy synthesis).
- Bitmap font: `tools/art/gen_font.py`.
- AI-assisted art: see `docs/ai_art.md`.

## Researched but NOT used in the game
`/workspace/boss_research/cc0_zips` (Alien_Bosses, SpaceShip_Boss_Sprites, UFO_Boss_Sprites). Nothing from these packs ships.

## Fonts (i18n, feat/i18n-midboss, 2026-10-25)

| Font | Author | Licence | Source | Local copy | Used for |
|---|---|---|---|---|---|
| Latin pixel font `pixel8` / `pixel16` (5x7 glyphs + accents) | GamDev (original, `tools/art/gen_font.py`) | project | — | `assets/fonts/pixel*.fnt` | every UI text, FR/ES/DE/PT-BR accents |
| Fusion Pixel Font 10px proportional, release 2026.10.25 | TakWolf | **SIL OFL 1.1** | https://github.com/TakWolf/fusion-pixel-font | `assets/fonts/cjk/` (subsets) + `LICENSES/fonts/FUSION_PIXEL_OFL.txt` | Japanese, Simplified and Traditional Chinese (fallback of the pixel font) |
| ↳ Ark Pixel Font (merged in Fusion Pixel) | TakWolf | SIL OFL 1.1 | https://github.com/TakWolf/ark-pixel-font | `LICENSES/fonts/ark-pixel_OFL.txt` | same |
| ↳ Galmuri (merged in Fusion Pixel) | Lee Minseo | SIL OFL 1.1 | https://github.com/quiple/galmuri | `LICENSES/fonts/galmuri_OFL.txt` | same |
| ↳ BoutiqueBitmap9x9 (merged in Fusion Pixel) | Luke Liu (fancy type foundry) | SIL OFL 1.1 | https://github.com/scott0107000/BoutiqueBitmap9x9 | `LICENSES/fonts/boutique-bitmap-9x9_OFL.txt` | same |

OFL 1.1 allows commercial use, bundling and modification (subsetting); the licence text must travel with the
font. The fonts are not sold on their own. Credited in-game in the credits panel ("FONTS: ...").
