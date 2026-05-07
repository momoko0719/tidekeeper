# GameName: Tidekeeper

## Course & Team

**Course Project:** DESIGN 6197/4197 - Designing Games for Research (Spring 2026, Cornell Tech)  
**Team Members:** Mengting Bao (mb2755), Yifei Tao (yt684), Ruowen Lou (rl948), Yusen Guo (yg684)

- **Game link:** [https://momoko0719.itch.io/tidekeeper](https://momoko0719.itch.io/tidekeeper)  
- **Game Trailer Video:** [https://www.youtube.com/watch?v=wgr85uj6pvE](https://www.youtube.com/watch?v=wgr85uj6pvE)
- **Game Presentation Slide:** [https://docs.google.com/presentation/d/1j_P_3pW9UUqyDZNS6VzoZ-HNN89paVZe8ksb7NAqBsY/edit?usp=sharing](https://docs.google.com/presentation/d/1j_P_3pW9UUqyDZNS6VzoZ-HNN89paVZe8ksb7NAqBsY/edit?usp=sharing)


![Tidekeeper Banner](gamePictures/banner.png)

Tidekeeper is a multiplayer game where four coastal creatures compete and interact within a shared ecosystem while racing to earn the most money.  Through actions like stealing, selling, cooking, and releasing fish, players reveal dynamic strategies that shape both competition and environmental outcomes. Each round mixes cooperation and conflict, then uses a group vote to adjust how often police appear in the next round.

## Repository Overview

### Root Files and Folders

- `index.html`: Main game file containing gameplay logic, UI flow, rendering, controls, round/vote systems, and in-game rules.
- `start-page.css`: Styles for the start screen and visual theme elements used by `index.html`.
- `GAMEPAD.md`: Gamepad and input mapping documentation aligned with the current control rules.
- `RULE.md`: Project/game rules or assignment guideline notes.
- `assets/`: Runtime game assets used by the game client (images, audio, fonts).
- `gamePictures/`: Submission media folder required by the instructor.

### `assets/` Folder Details

- `assets/bgm.mp3`: Background music track.
- `assets/dialog-bubble.png`: Dialogue bubble UI graphic.
- `assets/dust.gif`: Dust visual effect used for player movement animation.
- `assets/police.png`: Police character sprite/image.
- `assets/policestation.png`: Police station building image.
- `assets/resultbg.png`: End-of-round or result screen background image.
- `assets/salmon.png`: Salmon fish icon/sprite.
- `assets/tuna.png`: Tuna fish icon/sprite.
- `assets/player1-raise.png`: P1 vote/raise-hand variant image.
- `assets/player2-raise.png`: P2 vote/raise-hand variant image.
- `assets/player3-raise.png`: P3 vote/raise-hand variant image.
- `assets/player4-raise.png`: P4 vote/raise-hand variant image.

#### `assets/voices/`

- `assets/voices/collect.mp3`: Voice/SFX for collecting.
- `assets/voices/cook.mp3`: Voice/SFX for cooking.
- `assets/voices/release.mp3`: Voice/SFX for releasing fish.
- `assets/voices/sell.mp3`: Voice/SFX for selling.
- `assets/voices/steal.mp3`: Voice/SFX for stealing.

#### `assets/PixelOperator/`

- `assets/PixelOperator/LICENSE.txt`: Font license document.
- `assets/PixelOperator/PixelOperator.ttf`: PixelOperator base font.
- `assets/PixelOperator/PixelOperator-Bold.ttf`: Bold variant.
- `assets/PixelOperator/PixelOperator8.ttf`: 8px style variant.
- `assets/PixelOperator/PixelOperator8-Bold.ttf`: 8px bold variant.
- `assets/PixelOperator/PixelOperatorHB.ttf`: Heavy/bold style variant.
- `assets/PixelOperator/PixelOperatorHB8.ttf`: Heavy 8px style variant.
- `assets/PixelOperator/PixelOperatorHBSC.ttf`: Heavy small-caps style variant.
- `assets/PixelOperator/PixelOperatorSC.ttf`: Small-caps style variant.
- `assets/PixelOperator/PixelOperatorSC-Bold.ttf`: Small-caps bold variant.
- `assets/PixelOperator/PixelOperatorMono.ttf`: Monospace variant.
- `assets/PixelOperator/PixelOperatorMono-Bold.ttf`: Monospace bold variant.
- `assets/PixelOperator/PixelOperatorMono8.ttf`: Monospace 8px variant.
- `assets/PixelOperator/PixelOperatorMono8-Bold.ttf`: Monospace 8px bold variant.
- `assets/PixelOperator/PixelOperatorMonoHB.ttf`: Monospace heavy variant.
- `assets/PixelOperator/PixelOperatorMonoHB8.ttf`: Monospace heavy 8px variant.

### `gamePictures/` Folder

This folder is for instructor-required submission material: **a folder with all original high resolution images, drawings, renderings, diagrams, photographs, etc.**

Current contents:

- `gamePictures/banner.png`
- `gamePictures/Screenshot-build.jpg`
- `gamePictures/Screenshot-police.jpg`
- `gamePictures/Screenshot-scoreboard.jpg`
- `gamePictures/Screenshot-sell.jpg`
- `gamePictures/Screenshot-steal.jpg`
- `gamePictures/Screenshot-vote.jpg`

## Playtest Documentations


