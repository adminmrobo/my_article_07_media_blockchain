# 02번 「흔들림은 몰려온다」 이미지 제작 명세서

| 항목 | 내용 |
|---|---|
| 페이지 | 02_volatility_garch.html |
| 모드 / 주 앵커 | 논문 / D 일상: 비 오는 창가의 예보판 |
| 시즌 | 기본 |
| 대결 | 지난 60일 평균이면 충분할까? → 결과 R (Money-Robo 승), 차이 0.437 → 0.129 %p (상대 70%) |
| 새로 그릴 그림 | P1 3장 · P2 1장 · P3 0장 (외부 기준) |
| 제작 경로 | 직접 4장 (페이지에 넣음: 아웃트로 합성본, 대결 머리, 썸네일, 공유 미리보기) · 외부 의뢰 3장 (받을 것) |
| 의뢰 도구 | Genspark (기본) |
| 진행 | 받음 0 / 의뢰 3 · 마지막 반영 아직 |
| 캐릭터 팩 표정 | 22장 (팩 커밋 ea5da3f) |
| 재사용 | 0장 |
| 그림이 없을 때 | 페이지는 캐릭터 팩 표정과 CSS·캔버스 배경으로 이미 완성 상태 |

## 1. 그림체와 고정 외형
- 스타일: SKILL 18-3 (16비트 SNES 시대 픽셀 아트, 굵은 외곽선, 디더링 음영)
- 캐릭터 고정 외형: SKILL 18-4 표 그대로 (공식 저장소 `CHARACTER_CORE_EN`)
- 이 페이지 장소: 밤의 연구실 창가. 비구름이 낀 창문, 막대만 있는 예보판(글자 없음), 빨간 우산, 연구실 보라 조명이 한쪽에서 들어옴
- 장소 영어 묘사: *a rainy window corner inside the same night lab world, rain clouds outside the window, a forecast board showing only colored bars, a red umbrella on a stand, purple lab light spilling in from one side*

## 2. 필요한 그림 전체

| # | 키 | 판 | 크기 | 상태 | 제작 | 우선 | 들어가는 곳 | 대신 쓰는 그림 |
|---|---|---|---|---|---|---|---|---|
| 1 | bg_02 | F | 1920×720 | 의뢰 | 외부 | P1 | 히어로 배경 (`.hero-bg`) | CSS 그라데이션 + 벌집 무늬 |
| 2 | sc_02_hero | E | 1200×800 | 의뢰 | 외부 | P1 | 히어로 무대 (`.stage`) | 팩 캐릭터 + 캔버스 소품 합성본 (넣음) |
| 3 | cut_02_think | G | 960×540 | 의뢰 | 외부 | P1 | 논문 모드 히어로 생각 컷 (R14) | 히어로 대화창의 doc_think |
| 4 | sc_02_outro | E | 1200×800 | 넣음 (합성본) | 직접 → 외부 선택 | P2 | 아웃트로 무대 | 팩 캐릭터 + 캔버스 소품 합성본 |
| 5 | cut_02_versus | G | 960×540 | 넣음 | 직접 | P3 | 대결 머리 (팩 192px 마주 보기) | — |
| 6 | thumb_02 | I | 600×400 | 넣음 | 직접 (히어로 합성본 3:2 자르기) | P2 | 목차 카드 (index.html) | — |
| 7 | og_02 | K | 1200×630 | 넣음 | 직접 (히어로 화면 캡처) | P3 | 공유 미리보기 `img/og_02.jpg` | — |
| 8 | asst_firm → asst_e12 | B | 팩 96 | 팩 | — | — | 히어로·말풍선·대결 | — |
| 9 | asst_smile → asst_e13 | B | 팩 96 | 팩 | — | — | 히어로·말풍선·대결 | — |
| 10 | asst_spark → asst_e01 | B | 팩 96 | 팩 | — | — | 히어로·말풍선·대결 | — |
| 11 | doc_front → doc_e08 | A | 팩 96 | 팩 | — | — | 히어로·말풍선·대결 | — |
| 12 | doc_judge → doc_e10 | A | 팩 96 | 팩 | — | — | 히어로·말풍선·대결 | — |
| 13 | doc_magic → doc_e16 | A | 팩 96 | 팩 | — | — | 히어로·말풍선·대결 | — |
| 14 | doc_scale → doc_e13 | A | 팩 96 | 팩 (그림 없음 → 기본 표정) | — | — | 히어로·말풍선·대결 | — |
| 15 | doc_think → doc_e09 | A | 팩 96 | 팩 | — | — | 히어로·말풍선·대결 | — |
| 16 | fly_arms → fly_e16 | C | 팩 96·192 | 팩 | — | — | 히어로·말풍선·대결 | — |
| 17 | fly_clip → fly_e10 | C | 팩 96 | 팩 | — | — | 히어로·말풍선·대결 | — |
| 18 | fly_coffee → fly_e13 | C | 팩 96·192 | 팩 | — | — | 히어로·말풍선·대결 | — |
| 19 | fly_cry → fly_e21 | C | 팩 96·192 | 팩 | — | — | 히어로·말풍선·대결 | — |
| 20 | fly_point → fly_e08 | C | 팩 96·192 | 팩 | — | — | 히어로·말풍선·대결 | — |
| 21 | robo_coin → robo_e16 | D | 팩 96·192 | 팩 | — | — | 히어로·말풍선·대결 | — |
| 22 | robo_happy → robo_e12 | D | 팩 96·192 | 팩 | — | — | 히어로·말풍선·대결 | — |
| 23 | robo_meh → robo_e18 | D | 팩 96·192 | 팩 | — | — | 히어로·말풍선·대결 | — |
| 24 | robo_sigh → robo_e20 | D | 팩 96·192 | 팩 | — | — | 히어로·말풍선·대결 | — |
| 25 | robo_smile → robo_e13 | D | 팩 96 | 팩 | — | — | 히어로·말풍선·대결 | — |
| 26 | 행동으로 보기, NPC | — | — | 코드 | 직접 | — | 캔버스 (금화·사람·구름 픽셀) | — |

상태 값: `팩` · `넣음`(직접 그림, 페이지에 있음) · `의뢰`(외부, 받을 것) · `받음`(검수 전) · `반영`(페이지에 넣음) · `다시 의뢰`(검수 탈락).
그림 없음 역할 키(이 페이지): `doc_scale` — 기본 표정(E13)으로 대신. 새로 그릴지는 `IMG_00_index.md`에서 시리즈 단위로 정한다.

## 3. 새로 그릴 그림 상세

### 3-1. `bg_02`
| 항목 | 내용 |
|---|---|
| 판 · 크기 | F · 1920×720 (정수배 가능) |
| 제작 경로 | 외부: Genspark |
| 배경 | 그림 전체 |
| 구도 | 인물 없음. 왼쪽 45%는 어둡고 단순하게(제목 글자 자리), 장소의 핵심 소품은 오른쪽 |
| 표정·몸짓 | — |
| 소품 | 밤의 연구실 창가. 비구름이 낀 창문, 막대만 있는 예보판(글자 없음), 빨간 우산, 연구실 보라 조명이 한쪽에서 들어옴 (글자 없음) |
| 빛·분위기 | 밤의 연구실 보라 조명, 모니터 청록 불빛, 작은 분홍·초록 형광 |
| 피할 것 | 글자·숫자·로고, 실존 코인 기호나 브랜드 |
| 대체 글 (alt) | 비구름이 낀 창문과 예보판이 있는 밤의 연구실 |
| 대신 쓰는 그림 | CSS 그라데이션 + 벌집 무늬 |

**프롬프트 (복사해서 사용)**
```
detailed 16-bit SNES-era pixel art, limited palette, crisp pixels, dithering shading, thick dark outlines, cheerful comedy mood, consistent with the reference images, cozy night laboratory mood, purple light, soft magenta and green fluorescent accents, wide 8:3 background, left side simple and calm for title text, details on the right, a rainy window corner inside the same night lab world, rain clouds outside the window, a forecast board showing only colored bars, a red umbrella on a stand, purple lab light spilling in from one side, no characters, no text, no letters, no numbers, no logos, no weapons, no cigarettes, no alcohol, no blood, no real brands
```

### 3-2. `sc_02_hero`
| 항목 | 내용 |
|---|---|
| 판 · 크기 | E · 1200×800 (정수배 가능) |
| 제작 경로 | 외부: Genspark |
| 배경 | 그림 전체 |
| 구도 | 초파리 왼쪽(오른쪽을 봄), Money-Robo 오른쪽(왼쪽을 봄), 박사 가운데 뒤, 하루 한쪽 옆. 중요한 것은 위쪽 62% 안 |
| 표정·몸짓 | 박사 doc_think(턱에 손), 초파리 fly_point(의심하며 가리킴), 로봇 robo_coin(금화), 하루 asst_smile |
| 소품 | 밤의 연구실 창가. 비구름이 낀 창문, 막대만 있는 예보판(글자 없음), 빨간 우산, 연구실 보라 조명이 한쪽에서 들어옴 (글자 없음) |
| 빛·분위기 | 중간 밝기, 장면의 빛이 핵심 소품에 모임 |
| 피할 것 | 결과 전 장면이므로 승패를 짐작할 표정·배치 금지, 글자 |
| 대체 글 (alt) | 창밖에 비가 오는 연구실 무대 위의 네 캐릭터 |
| 대신 쓰는 그림 | 팩 캐릭터 + 캔버스 소품 합성본 |

**프롬프트 (복사해서 사용)**
```
detailed 16-bit SNES-era pixel art, limited palette, crisp pixels, dithering shading, thick dark outlines, cheerful comedy mood, consistent with the reference images, cozy night laboratory mood, purple light, soft magenta and green fluorescent accents, 3:2 landscape scene, medium brightness, the Professor, a chibi male scientist with a big head, dark charcoal spiky hair with a white streak at the front, a small low ponytail at the back, very thick bold black eyebrows, teal-framed rectangular glasses, light peach skin, white lab coat over a black vest, black tie and black slacks; the Fruit Fly, a tiny expressive cartoon fruit fly researcher with a dark charcoal-black segmented insect body, large glossy red compound eyes, a retro dark blue helmet with a yellow-white center stripe and small round side bolts, colorful dangling cables in magenta, purple and blue curving from the back of the helmet, a tiny white lab coat over a black vest, translucent veined wings, six thin black legs with the front pair used like hands; MONEY-ROBO, a cute small floating chibi robot with a large glossy rounded-square white head and a small rounded white body with thick black outlines, a black pill-shaped screen face showing golden-yellow pixel eyes and mouth, a small round knob antenna on a short stem, stubby rounded fingerless arms, no legs, a black oval chest panel with a bright cyan pill-shaped core light, hovering above a small dark oval shadow; Haru, a cute anime girl lab assistant, long straight pink hair with navy blue streaks including a thick navy streak down the center of the bangs, two round messy hair buns on top of the head, a small ahoge, big bright blue eyes, light peach skin, wearing a lavender hoodie with white drawstrings over a white t-shirt, under an open white knee-length lab coat; a rainy window corner inside the same night lab world, rain clouds outside the window, a forecast board showing only colored bars, a red umbrella on a stand, purple lab light spilling in from one side; the four characters look at a forecast board of colored bars next to a rainy window; the Professor at the back center with a hand on his chin; the Fruit Fly on the left looking right with a suspicious look; MONEY-ROBO on the right looking left beside a shiny gold coin; Haru at the side holding a blank clipboard, no text, no letters, no numbers, no logos, no weapons, no cigarettes, no alcohol, no blood, no real brands
```

### 3-3. `cut_02_think`
| 항목 | 내용 |
|---|---|
| 판 · 크기 | G · 960×540 (정수배 가능) |
| 제작 경로 | 외부: Genspark |
| 배경 | 그림 전체 |
| 구도 | 박사 한 명, 화면 왼쪽 40%. 생각 구름은 오른쪽 위 |
| 표정·몸짓 | 턱에 손, 한쪽 눈썹을 올림 (doc_e09) |
| 소품 | 생각 구름 안의 기호(글자 대신 그림) (글자 없음) |
| 빛·분위기 | 보라 조명 |
| 피할 것 | 구름 안 글자·숫자 |
| 대체 글 (alt) | 턱에 손을 얹고 생각하는 박사와 생각 구름 |
| 대신 쓰는 그림 | 히어로 대화창의 doc_think |

**프롬프트 (복사해서 사용)**
```
detailed 16-bit SNES-era pixel art, limited palette, crisp pixels, dithering shading, thick dark outlines, cheerful comedy mood, consistent with the reference images, cozy night laboratory mood, purple light, soft magenta and green fluorescent accents, 16:9 illustration panel, the Professor, a chibi male scientist with a big head, dark charcoal spiky hair with a white streak at the front, a small low ponytail at the back, very thick bold black eyebrows, teal-framed rectangular glasses, light peach skin, white lab coat over a black vest, black tie and black slacks, the Professor thinking; a thought cloud containing a single lightning bolt followed by a fading row of small rain clouds drawn as simple symbols, a rainy window corner inside the same night lab world, rain clouds outside the window, a forecast board showing only colored bars, a red umbrella on a stand, purple lab light spilling in from one side, no text, no letters, no numbers, no logos, no weapons, no cigarettes, no alcohol, no blood, no real brands
```

### 3-4. `sc_02_outro`
| 항목 | 내용 |
|---|---|
| 판 · 크기 | E · 1200×800 (정수배 가능) |
| 제작 경로 | 직접 합성본 넣음 → 외부 의뢰 선택 (P2) |
| 배경 | 그림 전체 |
| 구도 | 승자({win})가 앞·크게, 패자도 같은 화면에서 인정하는 몸짓. 박사 뒤, 하루 옆 |
| 표정·몸짓 | 아웃트로 말풍선 표정과 같게 |
| 소품 | 밤의 연구실 창가. 비구름이 낀 창문, 막대만 있는 예보판(글자 없음), 빨간 우산, 연구실 보라 조명이 한쪽에서 들어옴 (글자 없음) |
| 빛·분위기 | 밝은 마무리 분위기 |
| 피할 것 | 조롱하는 구도, 글자 |
| 대체 글 (alt) | 비구름이 걷히는 창가에서 Money-Robo가 두 팔을 들고 초파리 연구원이 커피를 든 연구실 장면 |
| 대신 쓰는 그림 | 팩 캐릭터 + 캔버스 소품 합성본 |

**프롬프트 (복사해서 사용)**
```
detailed 16-bit SNES-era pixel art, limited palette, crisp pixels, dithering shading, thick dark outlines, cheerful comedy mood, consistent with the reference images, cozy night laboratory mood, purple light, soft magenta and green fluorescent accents, 3:2 landscape scene, medium brightness, the Professor, a chibi male scientist with a big head, dark charcoal spiky hair with a white streak at the front, a small low ponytail at the back, very thick bold black eyebrows, teal-framed rectangular glasses, light peach skin, white lab coat over a black vest, black tie and black slacks; the Fruit Fly, a tiny expressive cartoon fruit fly researcher with a dark charcoal-black segmented insect body, large glossy red compound eyes, a retro dark blue helmet with a yellow-white center stripe and small round side bolts, colorful dangling cables in magenta, purple and blue curving from the back of the helmet, a tiny white lab coat over a black vest, translucent veined wings, six thin black legs with the front pair used like hands; MONEY-ROBO, a cute small floating chibi robot with a large glossy rounded-square white head and a small rounded white body with thick black outlines, a black pill-shaped screen face showing golden-yellow pixel eyes and mouth, a small round knob antenna on a short stem, stubby rounded fingerless arms, no legs, a black oval chest panel with a bright cyan pill-shaped core light, hovering above a small dark oval shadow; Haru, a cute anime girl lab assistant, long straight pink hair with navy blue streaks including a thick navy streak down the center of the bangs, two round messy hair buns on top of the head, a small ahoge, big bright blue eyes, light peach skin, wearing a lavender hoodie with white drawstrings over a white t-shirt, under an open white knee-length lab coat; a rainy window corner inside the same night lab world, rain clouds outside the window, a forecast board showing only colored bars, a red umbrella on a stand, purple lab light spilling in from one side; the rain clouds clear and a small sun appears in the window; MONEY-ROBO in front, larger, raising both arms; the Fruit Fly on the left holding a coffee cup and nodding; the Professor with small purple flames; Haru smiling at the side, no text, no letters, no numbers, no logos, no weapons, no cigarettes, no alcohol, no blood, no real brands
```

### 3-5. 직접 그림 (페이지에 이미 들어감)
- `cut_02_versus`: 대결 머리. 팩 192px 초파리(`data-face="right"`)와 Money-Robo(`data-face="left"`)가 마주 보게 배치.
- `thumb_02`: 히어로 합성본(`.stage`)을 3:2로 잘라 600×400 WebP → `index.html` 목차 카드에 base64로 넣음.
- `og_02`: 1200×630 히어로 화면 캡처 → `img/og_02.jpg`, 페이지 `<meta property="og:image">`.

## 4. 일관성 지침
- 참고 이미지: 공식 저장소 `refs/original/keyart_rivals.png`(넷이 함께) + 장면에 나오는 캐릭터의 표정 원본 PNG (`images/doctor/E09_thinking.png`, `images/haru/E13_neutral.png`, `images/fruitfly/E08_guiding.png`, `images/money_robo/E16_proud.png`)
- 같은 캐릭터는 같은 세션에서, 시드 고정 가능하면 고정: 박사 1101, 조수 2202, 초파리 3303, 로봇 4404
- 표정만 바꿀 때 추가 문장: *same character, same size and position, only change the facial expression and pose to ...*
- 투명 배경이 안 되면: *solid flat #00ff00 background*

## 5. 넘겨받은 뒤 처리
SKILL 18-15 절차 그대로 (키 맞추기 → 눈으로 검수 → `--ingest` → 페이지에 넣기 → 상태 갱신 → 점검 → 전달).
```bash
python3 build_character_pack.py --ingest 받은폴더/ --plates bg_02=F,sc_02_hero=E,cut_02_think=G --out received_02
```

## 6. 체크리스트
- [x] HTML의 모든 `data-img` 키가 명세서에 있음 (`bg_02`, `cut_02_think`, `cut_02_versus`, `sc_02_hero`, `sc_02_outro` + 팩 표정)
- [x] 대결 결과 후 표정이 5-8절 표와 일치 (결과 R, 차이 규칙 적용)
- [x] 결과 전 그림(히어로, 대결 전)에 승패 암시 없음
- [x] 모든 프롬프트에 18-4 고정 외형 영어 묘사와 금지 구절
- [x] 팩에 있는 표정을 “새로 그림”에 넣지 않음
- [x] 직접 그림은 이미 페이지에 들어가 있음
- [x] 장소가 주 앵커와 일치, 초파리 해부·현미경 소품 없음
- [x] P1 3장 (6장 이하)
- [x] 페이지 그림 합계 400 KB 이하 (팩 표정 base64 약 255 KB)

## 8. 외부 의뢰 묶음 (Genspark 에 그대로 붙여 넣기)

같은 페이지 그림은 **한 세션에서 이 순서대로** 의뢰한다(배경 → 장면 → 컷).

### 의뢰 1/3 · `bg_02`
- **올릴 참고 이미지:** 없음 (배경만)
- **크기·비율:** 1920×720 (8:3) 이상
- **배경:** 그림 전체
- **받을 파일 이름:** `bg_02.png`
- **프롬프트:**
```
detailed 16-bit SNES-era pixel art, limited palette, crisp pixels, dithering shading, thick dark outlines, cheerful comedy mood, consistent with the reference images, cozy night laboratory mood, purple light, soft magenta and green fluorescent accents, wide 8:3 background, left side simple and calm for title text, details on the right, a rainy window corner inside the same night lab world, rain clouds outside the window, a forecast board showing only colored bars, a red umbrella on a stand, purple lab light spilling in from one side, no characters, no text, no letters, no numbers, no logos, no weapons, no cigarettes, no alcohol, no blood, no real brands
```
- **네거티브 (넣을 칸이 있으면):** `blurry, smooth vector art, 3D render, photorealistic, anti-aliased painting, inconsistent character, off-model, text, letters, watermark`
- **확인할 것:** 왼쪽 45%가 단순한지, 그림 안에 글자나 코인 기호가 없는지

### 의뢰 2/3 · `sc_02_hero`
- **올릴 참고 이미지:** `refs/original/keyart_rivals.png`, `images/doctor/E09_thinking.png`, `images/haru/E13_neutral.png`, `images/fruitfly/E08_guiding.png`, `images/money_robo/E16_proud.png`
- **크기·비율:** 1200×800 (3:2) 이상
- **배경:** 그림 전체
- **받을 파일 이름:** `sc_02_hero.png`
- **프롬프트:**
```
detailed 16-bit SNES-era pixel art, limited palette, crisp pixels, dithering shading, thick dark outlines, cheerful comedy mood, consistent with the reference images, cozy night laboratory mood, purple light, soft magenta and green fluorescent accents, 3:2 landscape scene, medium brightness, the Professor, a chibi male scientist with a big head, dark charcoal spiky hair with a white streak at the front, a small low ponytail at the back, very thick bold black eyebrows, teal-framed rectangular glasses, light peach skin, white lab coat over a black vest, black tie and black slacks; the Fruit Fly, a tiny expressive cartoon fruit fly researcher with a dark charcoal-black segmented insect body, large glossy red compound eyes, a retro dark blue helmet with a yellow-white center stripe and small round side bolts, colorful dangling cables in magenta, purple and blue curving from the back of the helmet, a tiny white lab coat over a black vest, translucent veined wings, six thin black legs with the front pair used like hands; MONEY-ROBO, a cute small floating chibi robot with a large glossy rounded-square white head and a small rounded white body with thick black outlines, a black pill-shaped screen face showing golden-yellow pixel eyes and mouth, a small round knob antenna on a short stem, stubby rounded fingerless arms, no legs, a black oval chest panel with a bright cyan pill-shaped core light, hovering above a small dark oval shadow; Haru, a cute anime girl lab assistant, long straight pink hair with navy blue streaks including a thick navy streak down the center of the bangs, two round messy hair buns on top of the head, a small ahoge, big bright blue eyes, light peach skin, wearing a lavender hoodie with white drawstrings over a white t-shirt, under an open white knee-length lab coat; a rainy window corner inside the same night lab world, rain clouds outside the window, a forecast board showing only colored bars, a red umbrella on a stand, purple lab light spilling in from one side; the four characters look at a forecast board of colored bars next to a rainy window; the Professor at the back center with a hand on his chin; the Fruit Fly on the left looking right with a suspicious look; MONEY-ROBO on the right looking left beside a shiny gold coin; Haru at the side holding a blank clipboard, no text, no letters, no numbers, no logos, no weapons, no cigarettes, no alcohol, no blood, no real brands
```
- **네거티브:** `blurry, smooth vector art, 3D render, photorealistic, anti-aliased painting, inconsistent character, off-model, text, letters, watermark`
- **확인할 것:** 박사 안경이 청록 사각인지(둥글면 다시), 하루 머리에 남색 줄과 번 2개가 있는지, 결과를 짐작할 표정이 없는지

### 의뢰 3/3 · `cut_02_think`
- **올릴 참고 이미지:** `images/doctor/E09_thinking.png`, `refs/original/doctor_sheet.png`
- **크기·비율:** 960×540 (16:9) 이상
- **배경:** 그림 전체
- **받을 파일 이름:** `cut_02_think.png`
- **프롬프트:**
```
detailed 16-bit SNES-era pixel art, limited palette, crisp pixels, dithering shading, thick dark outlines, cheerful comedy mood, consistent with the reference images, cozy night laboratory mood, purple light, soft magenta and green fluorescent accents, 16:9 illustration panel, the Professor, a chibi male scientist with a big head, dark charcoal spiky hair with a white streak at the front, a small low ponytail at the back, very thick bold black eyebrows, teal-framed rectangular glasses, light peach skin, white lab coat over a black vest, black tie and black slacks, the Professor thinking; a thought cloud containing a single lightning bolt followed by a fading row of small rain clouds drawn as simple symbols, a rainy window corner inside the same night lab world, rain clouds outside the window, a forecast board showing only colored bars, a red umbrella on a stand, purple lab light spilling in from one side, no text, no letters, no numbers, no logos, no weapons, no cigarettes, no alcohol, no blood, no real brands
```
- **네거티브:** `blurry, smooth vector art, 3D render, photorealistic, anti-aliased painting, inconsistent character, off-model, text, letters, watermark`
- **확인할 것:** 생각 구름 안에 글자·숫자가 없는지

## 7. 매니페스트
```json
{
 "page": "02_volatility_garch",
 "anchor": "D 일상: 비 오는 창가의 예보판",
 "season": "default",
 "duel": {
  "result": "R",
  "gap": "0.437 → 0.129 %p (상대 70%)"
 },
 "images": [
  {
   "key": "bg_02",
   "plate": "F",
   "size": [
    1920,
    720
   ],
   "maker": "external",
   "tool": "genspark",
   "status": "requested",
   "priority": "P1",
   "slot": "hero-bg",
   "fallback": "css",
   "alt": "비구름이 낀 창문과 예보판이 있는 밤의 연구실"
  },
  {
   "key": "sc_02_hero",
   "plate": "E",
   "size": [
    1200,
    800
   ],
   "maker": "external",
   "tool": "genspark",
   "status": "requested",
   "priority": "P1",
   "slot": "hero-stage",
   "fallback": "composite",
   "alt": "창밖에 비가 오는 연구실 무대 위의 네 캐릭터"
  },
  {
   "key": "cut_02_think",
   "plate": "G",
   "size": [
    960,
    540
   ],
   "maker": "external",
   "tool": "genspark",
   "status": "requested",
   "priority": "P1",
   "slot": "hero-think",
   "fallback": "doc_think",
   "alt": "턱에 손을 얹고 생각하는 박사와 생각 구름"
  },
  {
   "key": "sc_02_outro",
   "plate": "E",
   "size": [
    1200,
    800
   ],
   "maker": "claude",
   "status": "placed",
   "priority": "P2",
   "slot": "outro",
   "fallback": "composite",
   "alt": "비구름이 걷히는 창가에서 Money-Robo가 두 팔을 들고 초파리 연구원이 커피를 든 연구실 장면"
  },
  {
   "key": "cut_02_versus",
   "plate": "G",
   "size": [
    960,
    540
   ],
   "maker": "claude",
   "status": "placed",
   "priority": "P3",
   "slot": "duel-head",
   "alt": ""
  },
  {
   "key": "thumb_02",
   "plate": "I",
   "size": [
    600,
    400
   ],
   "maker": "claude",
   "status": "placed",
   "priority": "P2",
   "slot": "index-card",
   "alt": "흔들림은 몰려온다 썸네일"
  },
  {
   "key": "og_02",
   "plate": "K",
   "size": [
    1200,
    630
   ],
   "maker": "claude",
   "status": "placed",
   "priority": "P3",
   "slot": "og",
   "alt": "흔들림은 몰려온다 미리보기"
  },
  {
   "key": "asst_firm",
   "pack": "asst_e12",
   "plate": "B",
   "size": 96,
   "status": "pack",
   "slot": "dialog/duel",
   "alt": ""
  },
  {
   "key": "asst_smile",
   "pack": "asst_e13",
   "plate": "B",
   "size": 96,
   "status": "pack",
   "slot": "dialog/duel",
   "alt": ""
  },
  {
   "key": "asst_spark",
   "pack": "asst_e01",
   "plate": "B",
   "size": 96,
   "status": "pack",
   "slot": "dialog/duel",
   "alt": ""
  },
  {
   "key": "doc_front",
   "pack": "doc_e08",
   "plate": "A",
   "size": 96,
   "status": "pack",
   "slot": "dialog/duel",
   "alt": ""
  },
  {
   "key": "doc_judge",
   "pack": "doc_e10",
   "plate": "A",
   "size": 96,
   "status": "pack",
   "slot": "dialog/duel",
   "alt": ""
  },
  {
   "key": "doc_magic",
   "pack": "doc_e16",
   "plate": "A",
   "size": 96,
   "status": "pack",
   "slot": "dialog/duel",
   "alt": ""
  },
  {
   "key": "doc_scale",
   "pack": "doc_e13",
   "plate": "A",
   "size": 96,
   "status": "pack-substitute",
   "slot": "dialog/duel",
   "alt": ""
  },
  {
   "key": "doc_think",
   "pack": "doc_e09",
   "plate": "A",
   "size": 96,
   "status": "pack",
   "slot": "dialog/duel",
   "alt": ""
  },
  {
   "key": "fly_arms",
   "pack": "fly_e16",
   "plate": "C",
   "size": 96,
   "status": "pack",
   "slot": "dialog/duel",
   "alt": ""
  },
  {
   "key": "fly_clip",
   "pack": "fly_e10",
   "plate": "C",
   "size": 96,
   "status": "pack",
   "slot": "dialog/duel",
   "alt": ""
  },
  {
   "key": "fly_coffee",
   "pack": "fly_e13",
   "plate": "C",
   "size": 96,
   "status": "pack",
   "slot": "dialog/duel",
   "alt": ""
  },
  {
   "key": "fly_cry",
   "pack": "fly_e21",
   "plate": "C",
   "size": 96,
   "status": "pack",
   "slot": "dialog/duel",
   "alt": ""
  },
  {
   "key": "fly_point",
   "pack": "fly_e08",
   "plate": "C",
   "size": 96,
   "status": "pack",
   "slot": "dialog/duel",
   "alt": ""
  },
  {
   "key": "robo_coin",
   "pack": "robo_e16",
   "plate": "D",
   "size": 96,
   "status": "pack",
   "slot": "dialog/duel",
   "alt": ""
  },
  {
   "key": "robo_happy",
   "pack": "robo_e12",
   "plate": "D",
   "size": 96,
   "status": "pack",
   "slot": "dialog/duel",
   "alt": ""
  },
  {
   "key": "robo_meh",
   "pack": "robo_e18",
   "plate": "D",
   "size": 96,
   "status": "pack",
   "slot": "dialog/duel",
   "alt": ""
  },
  {
   "key": "robo_sigh",
   "pack": "robo_e20",
   "plate": "D",
   "size": 96,
   "status": "pack",
   "slot": "dialog/duel",
   "alt": ""
  },
  {
   "key": "robo_smile",
   "pack": "robo_e13",
   "plate": "D",
   "size": 96,
   "status": "pack",
   "slot": "dialog/duel",
   "alt": ""
  }
 ],
 "character_pack": {
  "repo": "adminmrobo/fruitfly-lab-expressions",
  "commit": "ea5da3f"
 },
 "status_values": "pack | placed(직접, 넣음) | requested(의뢰) | received(받음) | applied(반영) | rejected(다시 의뢰)"
}
```
