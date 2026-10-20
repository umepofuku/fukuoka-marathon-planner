# Fukuoka Marathon 2026 Pace Planner

**Unofficial** cut-off time planner for the Fukuoka Marathon 2026 (Nov 8, 2026).
Enter your planned pace for each section and see when you will reach each checkpoint, and how much margin you have before it closes.

🇯🇵 日本語の説明は[下](#日本語)にあります。

**Live site:** `https://umepofuku.github.io/fukuoka-marathon-planner/` (Japanese) · `https://umepofuku.github.io/fukuoka-marathon-planner/en.html` (English)

## Features

- Set your pace (per km) for the section leading to each checkpoint, from 3:00 to 12:00 in 5-second steps
- "Same below" button copies a pace to all following sections; "Apply to all" sets one pace for every section
- Shows your expected pass time, the official closing time, and your margin at all 10 checkpoints (including the finish)
- Estimated finish time (net), average pace, and clock finish time
- Adjustable delay between the gun and the start line (0–25 min)
- Color-coded margin: yellow under 10 min, red under 5 min
- Mobile-friendly, dark-mode aware, printable (Print / Save as PDF)
- Japanese and English versions

## How it works

- Gun time is 8:20 and the time limit is 7 hours (15:20). Checkpoints close based on the **gun time**.
- Pass time at a checkpoint = gun time + start delay + sum of (section length × section pace).
- Pass times are **rounded up to the minute** (safe side), and margin = closing time − pass time, in whole minutes.
- Section lengths are the distances between consecutive checkpoints; the first section starts at the start line.

## Checkpoints

| Checkpoint | Distance | Closes |
|---|---|---|
| Momochi Central Park (百道中央公園) | 5.3 km | 9:25 |
| Odonishi Intersection, before (小戸西交差点手前) | 9.9 km | 10:09 |
| Imajuku Station Intersection, past (今宿駅前交差点先) | 14.3 km | 10:52 |
| Kyushu University Ito Campus (九州大学伊都キャンパス) | 19.8 km | 11:44 |
| Imazu Sports Park (今津運動公園) | 25.0 km | 12:33 |
| Kitazaki Elementary School (北崎小学校) | 29.8 km | 13:20 |
| Showa Bus Nishiura Depot (昭和バス西浦待機所) | 32.9 km | 13:50 |
| Imuta Intersection, before (伊牟田交差点手前) | 36.9 km | 14:28 |
| Yoshida Sanyaro, before (吉田三叉路手前) | 40.1 km | 14:59 |
| Finish (フィニッシュ) | 42.195 km | 15:20 |

Source: [Fukuoka Marathon official website](https://www.f-marathon.jp/about/) (race guidelines). Checked against the official page; the organizers may change details, so **always confirm on the official site before race day.**

## Notes and limitations

- **Unofficial.** This tool is not affiliated with or endorsed by the Fukuoka Marathon organizers. Use it as a rough guide only.
- The start delay depends on your start block and is not officially published. The preset values are estimates; if you have a past race, use your gun time minus net time.
- The planner does not account for course elevation, aid stations, or your fatigue.
- Closing times shown here may differ from the final official information.

## Privacy

Everything runs in your browser. No data is sent anywhere. Your pace settings are saved only in your own browser (`localStorage`).

## Run locally

No build step. Open `index.html` (Japanese) or `en.html` (English) in a browser. Keep both files in the same folder so the language links work.

## Files

- `index.html` – Japanese version
- `en.html` – English version

---

# 日本語

福岡マラソン2026（2026年11月8日）の**非公式**関門ペースプランナーです。
関門に向かう区間ごとに予定ペースを入力すると、各関門の通過予定時刻と、閉鎖までの余裕が分かります。

## 主な機能

- 各関門に向かう区間の1kmあたりのペースを、3:00〜12:00（5秒刻み）で入力
- 「↓ 以降同じ」ボタンでその区間以降すべてを同じペースに、「全区間に反映」で一括入力
- 10か所（フィニッシュ含む）の通過予定・閉鎖時刻・余裕を表示
- 予想ゴールタイム（ネット）、平均ペース、ゴール予定時刻
- 号砲からスタートラインまでのロス時間を0〜25分で調整
- 余裕10分未満は黄、5分未満は赤で表示
- スマホ対応、ダークモード対応、印刷／PDF保存に対応
- 日本語版・英語版

## 計算方法

- 号砲8:20、制限時間7時間（15:20）。関門の閉鎖は**号砲時刻**が基準です。
- 通過予定時刻 ＝ 号砲時刻 ＋ スタートロス ＋（各区間の距離 × 区間ペース）の合計
- 通過予定は**分単位で切り上げ**（安全側）で表示し、余裕＝閉鎖時刻−通過予定（分）です。

## 注意

- **非公式のツールです。** 福岡マラソンの主催者とは関係ありません。目安としてお使いください。
- ブロック別のスタートロスは公式発表がないため、目安の値です。前年の記録（グロス−ネット）があれば、それに合わせてください。
- 関門データは[公式サイト](https://www.f-marathon.jp/about/)の大会要項と照合済みですが、変更される可能性があります。**大会直前に、必ず公式サイトで最新情報を確認してください。**
- 高低差、給水所、疲労による変化は考慮していません。

## プライバシー

すべてブラウザの中で動作し、入力内容はどこにも送信されません。ペースの設定は、お使いのブラウザ内（`localStorage`）にのみ保存されます。

## ローカルで開く

ビルド不要です。`index.html`（日本語）か `en.html`（英語）をブラウザで開いてください。言語切替リンクのため、2つのファイルは同じフォルダに置いてください。
