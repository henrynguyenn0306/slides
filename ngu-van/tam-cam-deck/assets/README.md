# Tấm Cám deck assets

Source assets for the Ngữ văn web deck of the Vietnamese folk tale *Tấm Cám*.

Intended repo path: `ngu-van/tam-cam-deck/assets/`

That path follows the existing subject/deck layout seen in the published `henrynguyenn0306/slides` repo (`lich-su/phuc-hung-deck/`, `sinh-hoc/golgi-deck/`). There is no existing `ngu-van` (or `van`) folder in the published slides tree. `henrynguyenn0306/class-projects` could not be listed from this session (see access note below), so if that repo already uses a different Văn folder name, put these files there instead.

These files are reference material for building the web deck. They are not the deck itself.

## Files

| File | What it is |
|---|---|
| `narration.mp3` | Clean story narration, 1:40.44 (100.441 s), 44.1 kHz mono MP3 at 128 kbps. A VBee mid-roll watermark ("Giải pháp chuyển văn bản thành giọng nói hàng đầu Việt Nam từ vb.vn.") was cut from the original 1:45.46 file, with a 40 ms crossfade at the splice. The splice sits inside part 4, after "xin gặp người têm" and before "Khi Tấm bước ra." |
| `script.txt` | Full narration script in Vietnamese, with obvious ASR typos corrected and the ad removed. Same wording as the clean audio. |
| `cues.json` | Zoom/section cue times on the **clean** `narration.mp3` timeline. Parts 0–4 have start/end times; part 5 (Thông điệp / Ý nghĩa) is not spoken in the narration (`start`/`end` are null). |
| `clean-segments.json` | Word- and segment-level timestamps for the clean file (seconds), with the same typo corrections as `script.txt`. |
| `slide1.png` | Full Canva editor screenshot of the one-page TẤM CÁM mind map (includes Canva chrome: template sidebar, top bar, "Add page" bar). Best uncropped original. |
| `canva-mind-map.png` | The same slide, cropped to the parchment canvas only (no editor chrome). Use this as the visual reference when rebuilding the infographic. |

Other screenshots in the working folder (`reverted.png`, `anim-order.png`, `anim-timing.png`, `timeline.png`, `audio.png`) show the same mind map but with more Canva UI (Animate panel and/or timeline) covering the edges, so they were not copied here.

## Mind-map layout (from the screenshots)

Antique torn-map / parchment background. A large ticket-style title sits in the **center**. Five dark olive-green content cards with a cream title pill sit around it. Stickers (characters and objects) overlap the cards.

Approximate positions, looking at the slide:

- **Center:** title card
- **Top left:** Biến cố & Mất cá bống, with Tấm (girl with a basket) and Bụt on a cloud
- **Top right:** Thử thách & Trở thành Hoàng hậu, with a parasol, a crown, and a pocket watch over a coastal map
- **Middle left:** Chuỗi hóa thân không khuất phục, with a loom, xoan đào blossoms, a vàng anh (yellow oriole), and a thị fruit (persimmon) above the bird
- **Bottom center:** Đoàn tụ & Trả giá, with a thị fruit and a colorful bird
- **Middle right:** Thông điệp / Ý nghĩa, with a pink lotus and a white cloud

## Verbatim text on the slide

Title (center, large cream letters on a tan ticket/banner):

```
TẤM CÁM
```

### 1. Top left — Biến cố & Mất cá bống

Title:

```
Biến cố & Mất cá bống
```

Bullets:

```
• Tấm bị lừa mất giỏ tép
• Bụt hiện lên
• Mẹ con Cám giết cá bống.
```

### 2. Top right — Thử thách & Trở thành Hoàng hậu

Title (two lines on the cream pill):

```
Thử thách & Trở
thành Hoàng hậu
```

Bullets:

```
• Nhặt thóc gạo
• Đi trẩy hội
• Đánh rơi hài
• Vào cung.
```

### 3. Middle left — Chuỗi hóa thân không khuất phục

Title (two lines on the cream pill):

```
Chuỗi hóa thân
không khuất phục
```

Bullets (the second bullet wraps onto a second line):

```
• Bị chặt cây cau
• Hóa thân liên tiếp
  để giữ lẽ phải
```

### 4. Bottom center — Đoàn tụ & Trả giá

Title:

```
Đoàn tụ & Trả giá
```

Bullets:

```
• Bà lão giữ thị
• Miếng trầu cánh phượng
• Tấm trở lại.
```

### 5. Middle right — Thông điệp / Ý nghĩa

Title:

```
Thông điệp / Ý nghĩa
```

Bullets (the second bullet wraps onto a second line):

```
• Ở hiền gặp lành
• Kiên trì đấu tranh
  cho hạnh phúc.
```

Punctuation is as shown on the slide: a period at the end of "Mẹ con Cám giết cá bống.", "Vào cung.", "Tấm trở lại.", and "cho hạnh phúc." The other bullets have no final period.

## Narration cues (clean timeline)

From `cues.json`. Use these to zoom to the matching box while the narration plays.

| Part | Label | Start | End |
|---|---|---|---|
| 0 | Mở đầu (hoàn cảnh Tấm) | 0:00.00 | 0:11.82 |
| 1 | Biến cố & Mất cá bống | 0:12.34 | 0:36.22 |
| 2 | Thử thách & Trở thành Hoàng hậu | 0:36.72 | 0:58.50 |
| 3 | Chuỗi hóa thân không khuất phục | 0:58.62 | 1:18.32 |
| 4 | Đoàn tụ & Trả giá | 1:18.32 | 1:39.94 |
| 5 | Thông điệp / Ý nghĩa | — | Not spoken. The slide bullets are not in the audio. The closing sentences (reunion and Cám's punishment) stay in part 4. |

A couple of wording differences between the slide and the narration (keep the audio as spoken; do not rewrite it to match the bullets): the slide says "giỏ tép" and "Nhặt thóc gạo"; the narration says "giỏ tôm cá" and "lựa đậu".

## Access note

These files were prepared locally and were not pushed in the session that created them. `cursor-github` could read `henrynguyenn0306/slides` but not `henrynguyenn0306/class-projects` (`scm_repo_not_accessible`: the repo is not in the Cursor GitHub App's granted set for the connected accounts). The connector also has no create-file / commit / upload-blob API, only `create_branch` plus read and PR/issue tools.
