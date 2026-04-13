# GROUP-B 宸ヤ綔鍖?

## 馃搵 灏忕粍鎴愬憳

| 缂栧彿 | 濮撳悕 | GitHub 鐢ㄦ埛鍚?| 瑙掕壊 |
|------|------|--------------|------|
| 01 |  |  |  |
| 02 |  |  |  |
| 03 |  |  |  |
| 04 |  |  |  |
| 05 |  |  |  |
| 06 |  |  |  |
| 07 |  |  |  |
| 08 |  |  |  |
| 09 |  |  |  |
| 10 |  |  | 缁勯暱 |

---

## 馃幆 浠诲姟鍒嗛厤

### M1 妯″潡锛氭姇鐮旈棶绛斿姪鎵?
- 璐熻矗浜猴細`01`, `02`
- 鎴鏃ユ湡锛欴ay 3

### M2 妯″潡锛氬婧愭暟鎹泦鎴?
- 璐熻矗浜猴細`03`, `04`
- 鎴鏃ユ湡锛欴ay 4

### M3 妯″潡锛氱煡璇嗗簱涓庨棶绛?
- 璐熻矗浜猴細`05`, `06`
- 鎴鏃ユ湡锛欴ay 4

### M4 妯″潡锛氶€氱煡绯荤粺
- 璐熻矗浜猴細`07`, `08`
- 鎴鏃ユ湡锛欴ay 5

### M5 妯″潡锛氬 Agent 鍗忎綔
- 璐熻矗浜猴細`09`, `10`
- 鎴鏃ユ湡锛欴ay 5

---

## 馃搧 鐩綍缁撴瀯

```
GROUP-B/
鈹溾攢鈹€ 01/
鈹?  鈹溾攢鈹€ backend/          # 鍚庣浠ｇ爜
鈹?  鈹?  鈹斺攢鈹€ tests/        # 娴嬭瘯浠ｇ爜
鈹?  鈹斺攢鈹€ docs/             # Spec 鏂囨。
鈹溾攢鈹€ 02/
鈹?  鈹溾攢鈹€ backend/
鈹?  鈹?  鈹斺攢鈹€ tests/
鈹?  鈹斺攢鈹€ docs/
鈹斺攢鈹€ ... (03-10)
```

---

## 馃殌 宸ヤ綔娴佺▼

### 1. Fork 涓讳粨搴?

```bash
# 鍦?GitHub 涓婅闂富浠撳簱
https://github.com/lvzhaobo/ira-workshop

# 鐐瑰嚮鍙充笂瑙?"Fork" 鎸夐挳锛屽垱寤轰綘鑷繁鐨勫壇鏈?
```

### 2. 鍏嬮殕鍒版湰鍦?

```bash
# 浣跨敤 SSH 鍏嬮殕锛堟帹鑽愶級
git clone git@github.com:浣犵殑鐢ㄦ埛鍚?ira-workshop.git

# 鎴栦娇鐢?HTTPS
git clone https://github.com/浣犵殑鐢ㄦ埛鍚?ira-workshop.git
```

### 3. 娣诲姞涓婃父杩滅▼浠撳簱

```bash
cd ira-workshop

# 娣诲姞涓讳粨搴撲负 upstream
git remote add upstream git@github.com:lvzhaobo/ira-workshop.git

# 楠岃瘉
git remote -v
# origin    => 浣犵殑 Fork
# upstream  => 涓讳粨搴?
```

### 4. 鍒涘缓鍒嗘敮

```bash
# 淇濇寔涓庝富浠撳簱鍚屾
git checkout main
git pull upstream main

# 鍒涘缓浣犵殑宸ヤ綔鍒嗘敮
git checkout -b feature/GROUP-B-01-m1

# 鍛藉悕瑙勮寖锛?
# feature/GROUP-B-{缂栧彿}-{妯″潡鍚峿
# 绀轰緥锛歠eature/GROUP-B-01-m1
#       feature/GROUP-B-03-m2
```

### 5. 寮€鍙戜笌鎻愪氦

```bash
# 鍦ㄤ綘鐨勭洰褰曚腑宸ヤ綔
# 渚嬪锛?1 鎴愬憳缂栬緫 GROUP-B/01/ 鐩綍

# 鏌ョ湅鐘舵€?
git status

# 娣诲姞鏂囦欢
git add GROUP-B/01/

# 鎻愪氦
git commit -m "feat: 瀹屾垚 M1 妯″潡 Spec 鏂囨。

- 娣诲姞 03-绔嬮」鎻愭.md
- 娣诲姞 05-鐢ㄦ埛鏁呬簨.md
- 娣诲姞 09-API鎺ュ彛瑙勬牸.md"

# 鎺ㄩ€佸埌浣犵殑 Fork
git push origin feature/GROUP-B-01-m1
```

### 6. 鎻愪氦 PR锛圥ull Request锛?

```bash
# 鏂瑰紡 1锛氫娇鐢?GitHub 缃戦〉
1. 璁块棶浣犵殑 Fork锛歨ttps://github.com/浣犵殑鐢ㄦ埛鍚?ira-workshop
2. 鐐瑰嚮 "Compare & pull request"
3. 璁剧疆锛?
   - base repository: lvzhaobo/ira-workshop
   - base branch: main
   - head branch: feature/GROUP-B-01-m1
4. 濉啓 PR 鎻忚堪
5. 鐐瑰嚮 "Create pull request"

# 鏂瑰紡 2锛氫娇鐢?GitHub CLI
gh pr create \
  --base main \
  --head feature/GROUP-B-01-m1 \
  --title "GROUP-B-01: 瀹屾垚 M1 妯″潡" \
  --body "宸插畬鎴?M1 妯″潡鐨?Spec 鏂囨。鍜屽熀纭€浠ｇ爜"
```

---

## 馃摑 PR 鎻愪氦瑙勮寖

### PR 鏍囬鏍煎紡

```
Group-{缁勫悕}-{缂栧彿}: {绠€鐭弿杩皚

绀轰緥锛?
GROUP-B-01: 瀹屾垚 M1 妯″潡 Spec 鏂囨。
GROUP-B-03: 瀹炵幇澶氭簮鏁版嵁闆嗘垚
GROUP-B-05: 娣诲姞鐭ヨ瘑搴撻棶绛斿姛鑳?
```

### PR 鎻忚堪妯℃澘

```markdown
## 馃搵 浠诲姟淇℃伅

- **缁勫埆**: GROUP-B
- **鎴愬憳**: 01锛堝鍚嶏級
- **妯″潡**: M1 - 鎶曠爺闂瓟鍔╂墜
- **闃舵**: Spec 鏂囨。 / 浠ｇ爜瀹炵幇 / 娴嬭瘯

## 鉁?瀹屾垚鍐呭

- [ ] 03-绔嬮」鎻愭涓庤寖鍥磋鏄?
- [ ] 05-鐢ㄦ埛鏁呬簨涓庨獙鏀舵爣鍑?
- [ ] 09-API 鎺ュ彛瑙勬牸
- [ ] 13-娴嬭瘯绛栫暐涓庤川閲忛棬绂?
- [ ] 14-闇€姹傝拷韪煩闃?
- [ ] 鍚庣浠ｇ爜瀹炵幇
- [ ] 鍓嶇浠ｇ爜瀹炵幇
- [ ] 娴嬭瘯鐢ㄤ緥

## 馃敆 鐩稿叧鏂囨。

- Spec 鏂囨。璺緞锛歚GROUP-B/01/docs/`
- 浠ｇ爜璺緞锛歚GROUP-B/01/backend/`

## 馃摳 鎴浘锛堝鏈夛級

锛堟坊鍔犵晫闈㈡埅鍥炬垨杩愯缁撴灉锛?

## 馃挰 澶囨敞

锛堝叾浠栬鏄庢垨闂锛?
```

---

## 鈿狅笍 娉ㄦ剰浜嬮」

### 1. 鍙紪杈戣嚜宸辩殑鐩綍

- 鉁?鍙互缂栬緫锛歚GROUP-B/01/`, `GROUP-B/02/`, ...
- 鉂?涓嶈缂栬緫锛歚group-b/`, `group-c/`, 鍏朵粬缁勭殑鐩綍

### 2. 姣忓ぉ鍚屾涓讳粨搴?

```bash
# 姣忓ぉ鏃╀笂鎵ц
git checkout main
git pull upstream main
git push origin main
```

### 3. 鎻愪氦鍓嶆鏌?

```bash
# 纭繚鍙彁浜や簡鑷繁鐨勬枃浠?
git status

# 鏌ョ湅鍙樻洿鍐呭
git diff --staged

# 纭繚娌℃湁鎻愪氦鏁忔劅淇℃伅锛圓PI Key銆佸瘑鐮佺瓑锛?
```

### 4. 閬囧埌鍐茬獊鎬庝箞鍔烇紵

```bash
# 鎷夊彇鏈€鏂颁唬鐮?
git fetch upstream
git merge upstream/main

# 濡傛灉鏈夊啿绐侊紝鎵嬪姩瑙ｅ喅鍚庢彁浜?
git add <瑙ｅ喅鍐茬獊鐨勬枃浠?
git commit -m "merge: 瑙ｅ喅涓?main 鍒嗘敮鐨勫啿绐?
git push origin feature/GROUP-B-01-m1
```

---

## 馃搳 杩涘害杩借釜

| 鎴愬憳 | M1 | M2 | M3 | M4 | M5 | 鐘舵€?|
|------|----|----|----|----|----|------|
| 01 | 猬?| 猬?| 猬?| 猬?| 猬?| 鏈紑濮?|
| 02 | 猬?| 猬?| 猬?| 猬?| 猬?| 鏈紑濮?|
| 03 | 猬?| 猬?| 猬?| 猬?| 猬?| 鏈紑濮?|
| 04 | 猬?| 猬?| 猬?| 猬?| 猬?| 鏈紑濮?|
| 05 | 猬?| 猬?| 猬?| 猬?| 猬?| 鏈紑濮?|
| 06 | 猬?| 猬?| 猬?| 猬?| 猬?| 鏈紑濮?|
| 07 | 猬?| 猬?| 猬?| 猬?| 猬?| 鏈紑濮?|
| 08 | 猬?| 猬?| 猬?| 猬?| 猬?| 鏈紑濮?|
| 09 | 猬?| 猬?| 猬?| 猬?| 猬?| 鏈紑濮?|
| 10 | 猬?| 猬?| 猬?| 猬?| 猬?| 鏈紑濮?|

**鍥句緥**锛氣瑴 鏈紑濮?| 馃煛 杩涜涓?| 鉁?宸插畬鎴?| 鉂?鏈夐棶棰?

---

## 馃啒 鑾峰彇甯姪

### 甯歌闂

1. **鏃犳硶鍏嬮殕浠撳簱锛?*
   - 妫€鏌?SSH Key 閰嶇疆锛歚ssh -T git@github.com`
   - 鎴栦娇鐢?HTTPS锛歚git clone https://github.com/...`

2. **鎻愪氦 PR 澶辫触锛?*
   - 纭繚 Fork 浜嗕富浠撳簱
   - 纭繚鎺ㄩ€佸埌浜嗚嚜宸辩殑 Fork锛坥rigin锛?

3. **閬囧埌 Git 鍐茬獊锛?*
   - 鍏堟媺鍙栨渶鏂颁唬鐮侊細`git pull upstream main`
   - 鎵嬪姩瑙ｅ喅鍐茬獊鍚庡啀鎻愪氦

### 鑱旂郴璁插笀

- GitHub: @lvzhaobo
- 闂鍙嶉锛氬湪涓讳粨搴撳垱寤?Issue

---

## 馃摎 瀛︿範璧勬簮

- [Spec Coding 鏂囨。浣撶郴](../.templates/M1/)
- [Git 鎻愪氦瑙勮寖](https://www.conventionalcommits.org/)
- [GitHub PR 鏁欑▼](https://docs.github.com/en/pull-requests)

---

> **鏈€鍚庢洿鏂?*: 2026-04-13
> **缁存姢鑰?*: GROUP-B 鍏ㄤ綋鎴愬憳
