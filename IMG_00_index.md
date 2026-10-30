# 시리즈 공용 이미지 명세서 — 미디어 토큰 경제 연구실

| 항목 | 내용 |
|---|---|
| 시리즈 | 미디어 토큰 경제 연구실 (안상선 논문 「미디어 콘텐츠 기반의 블록체인 토큰의 경제적 성과 분석」 해설), 페이지 4개 + 목차 |
| 시즌 | 기본 |
| 공용 표정 | 캐릭터 팩 96장 (커밋 ea5da3f) · 그림 없음 역할 키 1개 (doc_scale) |
| 대결 결과 | 01 R · 02 R · 03 F · 04 F → 2 : 2 균형 |

## 1. 공용 표정 현황
| 키 | 팩 키 | 상태 | 쓰는 페이지 | 프롬프트 (그림 없음만) |
|---|---|---|---|---|
| doc_scale | doc_e13 | 그림 없음 (E13로 대신) | 01~04 (대결 무승부 대비) | 아래 2-1 |

## 2. 새 표정 후보 (P2, 저장소에 E25~로 올린 뒤 팩 재빌드)
### 2-1. `doc_scale`
```
detailed 16-bit SNES-era pixel art, limited palette, crisp pixels, dithering shading, thick dark outlines, cheerful comedy mood, consistent with the reference images, single character, transparent background, centered with a small margin, facing front, bust, the Professor, a chibi male scientist with a big head, dark charcoal spiky hair with a white streak at the front, a small low ponytail at the back, very thick bold black eyebrows, teal-framed rectangular glasses, light peach skin, white lab coat over a black vest, black tie and black slacks, calm smile, holding a level brass balance scale with both hands, same character, same size and position as the reference, only change the facial expression and pose, no text, no letters, no numbers, no logos, no weapons, no cigarettes, no alcohol, no blood, no real brands
```

## 3. 목차·표지 그림
| 키 | 판 | 내용 | 우선 | 제작 | 상태 |
|---|---|---|---|---|---|
| cover_series | J | 밤의 연구실 전경, 넷이 함께 | P1 | 외부 | 의뢰 |
| bg_index | F | 연구실 복도, 문 네 개에서 각기 다른 색 빛 | P1 | 외부 | 의뢰 |
| lineup | G | 넷이 나란히 선 소개 컷 | P1 | 직접 (팩 96px 배치) | 넣음 (index.html) |
| thumb_01~04 | I | 각 페이지 히어로 합성본 3:2 | P2 | 직접 | 넣음 |
| icon_fly, icon_robo, icon_draw, icon_dq | H | 점수판 아이콘 | P1 | 직접 (CSS·글자 기호) | 넣음 (index.html 점수판) |
| og_index | K | 시리즈 표지 축소판 | P3 | 직접 (목차 화면 캡처) | 넣음 `img/og_index.jpg` |

### 3-1. `cover_series` (J, 1600×900)
```
detailed 16-bit SNES-era pixel art, limited palette, crisp pixels, dithering shading, thick dark outlines, cheerful comedy mood, consistent with the reference images, cozy night laboratory mood, purple light, soft magenta and green fluorescent accents, 16:9 series cover, all four characters together, the Professor, a chibi male scientist with a big head, dark charcoal spiky hair with a white streak at the front, a small low ponytail at the back, very thick bold black eyebrows, teal-framed rectangular glasses, light peach skin, white lab coat over a black vest, black tie and black slacks; the Fruit Fly, a tiny expressive cartoon fruit fly researcher with a dark charcoal-black segmented insect body, large glossy red compound eyes, a retro dark blue helmet with a yellow-white center stripe and small round side bolts, colorful dangling cables in magenta, purple and blue curving from the back of the helmet, a tiny white lab coat over a black vest, translucent veined wings, six thin black legs with the front pair used like hands; MONEY-ROBO, a cute small floating chibi robot with a large glossy rounded-square white head and a small rounded white body with thick black outlines, a black pill-shaped screen face showing golden-yellow pixel eyes and mouth, a small round knob antenna on a short stem, stubby rounded fingerless arms, no legs, a black oval chest panel with a bright cyan pill-shaped core light, hovering above a small dark oval shadow; Haru, a cute anime girl lab assistant, long straight pink hair with navy blue streaks including a thick navy streak down the center of the bangs, two round messy hair buns on top of the head, a small ahoge, big bright blue eyes, light peach skin, wearing a lavender hoodie with white drawstrings over a white t-shirt, under an open white knee-length lab coat; a wide night laboratory with a big wall map made of circles and lines without any text, a vault door and a rainy window on the sides, the Professor in the center pointing at the map, the Fruit Fly and MONEY-ROBO looking up from both sides, Haru holding a scoreboard with three blank panels, no text, no letters, no numbers, no logos, no weapons, no cigarettes, no alcohol, no blood, no real brands
```
### 3-2. `bg_index` (F, 1920×720)
```
detailed 16-bit SNES-era pixel art, limited palette, crisp pixels, dithering shading, thick dark outlines, cheerful comedy mood, consistent with the reference images, cozy night laboratory mood, purple light, soft magenta and green fluorescent accents, wide 8:3 background, left side simple and calm for title text, details on the right, a long night laboratory corridor with four doors in a row, each door leaking a different colored light (gold, blue, green, pink), no characters, no text, no letters, no numbers, no logos, no weapons, no cigarettes, no alcohol, no blood, no real brands
```
### 3-3. `lineup` (G, 960×540, 외부 의뢰 선택)
```
detailed 16-bit SNES-era pixel art, limited palette, crisp pixels, dithering shading, thick dark outlines, cheerful comedy mood, consistent with the reference images, cozy night laboratory mood, purple light, soft magenta and green fluorescent accents, 16:9 illustration panel, the Professor, a chibi male scientist with a big head, dark charcoal spiky hair with a white streak at the front, a small low ponytail at the back, very thick bold black eyebrows, teal-framed rectangular glasses, light peach skin, white lab coat over a black vest, black tie and black slacks; the Fruit Fly, a tiny expressive cartoon fruit fly researcher with a dark charcoal-black segmented insect body, large glossy red compound eyes, a retro dark blue helmet with a yellow-white center stripe and small round side bolts, colorful dangling cables in magenta, purple and blue curving from the back of the helmet, a tiny white lab coat over a black vest, translucent veined wings, six thin black legs with the front pair used like hands; MONEY-ROBO, a cute small floating chibi robot with a large glossy rounded-square white head and a small rounded white body with thick black outlines, a black pill-shaped screen face showing golden-yellow pixel eyes and mouth, a small round knob antenna on a short stem, stubby rounded fingerless arms, no legs, a black oval chest panel with a bright cyan pill-shaped core light, hovering above a small dark oval shadow; Haru, a cute anime girl lab assistant, long straight pink hair with navy blue streaks including a thick navy streak down the center of the bangs, two round messy hair buns on top of the head, a small ahoge, big bright blue eyes, light peach skin, wearing a lavender hoodie with white drawstrings over a white t-shirt, under an open white knee-length lab coat; the four characters standing in a row facing front, blank name plates below them, no text, no letters, no numbers, no logos, no weapons, no cigarettes, no alcohol, no blood, no real brands
```
네거티브: `blurry, smooth vector art, 3D render, photorealistic, anti-aliased painting, inconsistent character, off-model, text, letters, watermark` · 참고 이미지: `refs/original/keyart_rivals.png` + 네 캐릭터 시트

## 4. 페이지별 대표 그림 모음
| 페이지 | 앵커 | bg | hero | thumb | 상태 |
|---|---|---|---|---|---|
| 01_steem_reward_tokens | C 장부: 연구실 옆 회계실·금고실 | bg_01 | sc_01_hero | thumb_01 | bg·hero 의뢰, thumb 넣음 |
| 02_volatility_garch | D 일상: 비 오는 창가의 예보판 | bg_02 | sc_02_hero | thumb_02 | bg·hero 의뢰, thumb 넣음 |
| 03_efficient_market_news | D 일상: 교실처럼 꾸민 연구실 | bg_03 | sc_03_hero | thumb_03 | bg·hero 의뢰, thumb 넣음 |
| 04_decentralization_gini | C 장부: 금화 피라미드가 있는 금고실 | bg_04 | sc_04_hero | thumb_04 | bg·hero 의뢰, thumb 넣음 |

## 5. 매니페스트
```json
{
 "series": "미디어 토큰 경제 연구실",
 "shared": [
  {
   "key": "doc_scale",
   "pack": "doc_e13",
   "status": "missing"
  },
  {
   "key": "cover_series",
   "plate": "J",
   "maker": "external",
   "status": "requested",
   "priority": "P1"
  },
  {
   "key": "bg_index",
   "plate": "F",
   "maker": "external",
   "status": "requested",
   "priority": "P1"
  },
  {
   "key": "lineup",
   "plate": "G",
   "maker": "claude",
   "status": "placed",
   "priority": "P1"
  },
  {
   "key": "og_index",
   "plate": "K",
   "maker": "claude",
   "status": "placed",
   "priority": "P3"
  }
 ],
 "pages": [
  "01_steem_reward_tokens",
  "02_volatility_garch",
  "03_efficient_market_news",
  "04_decentralization_gini"
 ]
}
```
