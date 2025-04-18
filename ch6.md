# 風險趨避與風險資產資本配置

## 第1題
**題目：** 
下列哪一個選項最能完成以下陳述？請解釋。與較低風險趨避程度的投資者相比，具有較高風險趨避程度的投資者會要求
a. 具有較高風險溢價的投資組合。
b. 較具風險（具有較高標準差）的投資組合。
c. 具有較低夏普比率的投資組合。
d. 具有較低交易成本的投資組合。

**解答：**
(d) 雖然較高或較低的交易成本不一定表明投資者對風險的承受能力，但風險趨避的投資者可能偏好與較低交易成本相關的投資組合（管理較不積極，因此風險較低）。具有較高風險趨避程度的投資者不會想要 (a) 較高的風險溢價（因為它們與較高風險相關），(b) 較具風險的投資組合（較高標準差），或 (c) 較低的夏普比率（任何投資者都會總是偏好具有較高夏普比率的投資組合）

**初學者解釋：**
這個問題測試你對風險趨避投資者偏好的理解。讓我們分析每個選項：

- 選項(a)：風險趨避的投資者不會特別要求較高的風險溢價，因為高風險溢價通常伴隨著更高的風險。
- 選項(b)：風險趨避的投資者肯定不會選擇更具風險的投資組合（高標準差）。
- 選項(c)：夏普比率測量每單位風險的回報，較高夏普比率更好，所有投資者都會偏好高夏普比率。
- 選項(d)：雖然交易成本與風險承受能力不直接相關，但風險趨避的投資者通常偏好管理較不積極的投資組合，這些投資組合往往有較低的交易成本。

因此，正確答案是(d)。風險趨避的投資者傾向於選擇低風險、被動管理的投資組合，這些投資組合通常有較低的交易成本。

## 第2題
**題目：** 
以下哪些陳述是正確的？請解釋。
a. 風險投資組合的較低配置會降低夏普（回報與波動性）比率。
b. 借款利率越高，槓桿投資組合的夏普比率越低。
c. 在固定無風險利率的情況下，將風險投資組合的預期回報和標準差翻倍將使夏普比率翻倍。
d. 在風險投資組合的風險溢價保持不變的情況下，較高的無風險利率將提高對風險資產有正配置的投資的夏普比率。

**解答：**
(b) 較高的借款利率是借款人違約風險的結果。在沒有額外違約成本的完美市場中，這種增量將等於借款人違約選擇權的價值，並且夏普指標（在適當處理違約選擇權的情況下）將保持不變。然而，違約會產生成本，因此這部分增量降低了夏普比率。另外，請注意答案(c)不正確，因為在固定無風險利率的情況下，將預期回報翻倍將使風險溢價和夏普比率增加一倍以上。

**初學者解釋：**
這個問題測試你對夏普比率的理解，夏普比率是測量每單位風險回報的重要指標：

```
夏普比率 = (預期回報 - 無風險利率) / 標準差
```

分析每個選項：

- 選項(a)：錯誤。降低風險資產配置不會改變夏普比率，因為夏普比率衡量的是風險資產本身的特性，與配置無關。

- 選項(b)：正確。更高的借款利率會增加投資者的成本，導致淨回報降低，因此夏普比率會下降。

- 選項(c)：錯誤。如果預期回報和標準差都翻倍，分子（預期回報-無風險利率）將增加不止一倍（因為無風險利率不變），而分母（標準差）正好翻倍，因此夏普比率增加但不會恰好翻倍。

- 選項(d)：不一定正確。如果風險溢價（預期回報-無風險利率）保持不變，那麼預期回報必須隨著無風險利率增加而增加，夏普比率分子不變而分母不變，所以夏普比率也不變。

因此，正確答案是(b)。

## 第3題
**題目：** 
如果投資者感知到股票市場的波動性更高，你認為股票的均衡預期回報會發生什麼變化？將你的答案與方程式6.7聯繫起來。

**解答：**
假設風險容忍度沒有變化，即風險趨避係數不變（且A通常大於零），感知到的更高波動性會增加風險投資組合最優投資方程式的分母：

$$
y^* = \frac{E(r_p) - r_f}{A \sigma_p^2}
$$

因此，投資於風險投資組合的比例將降低。

**初學者解釋：**
這個問題要求我們考慮市場波動性增加對股票預期回報的影響。

方程式6.7描述了投資者如何在風險資產和無風險資產之間進行最優資本配置：

```
y* = (E(rp) - rf) / (A × σp²)
```

其中：
- y* 是投資於風險資產的最優比例
- E(rp) 是風險投資組合的預期回報
- rf 是無風險利率
- A 是風險趨避係數
- σp² 是風險投資組合的方差

當市場波動性（σp）增加時，方程式分母增大，導致y*（配置於風險資產的比例）減少。

在均衡狀態下，為了吸引投資者在較高波動性環境中持有相同數量的風險資產，風險資產的預期回報率(E(rp))必須增加以抵消更高的風險。這樣，風險溢價(E(rp) - rf)會增加以補償投資者承擔更高的風險。

簡而言之，當感知到的市場波動性增加時，股票的均衡預期回報也會增加，以維持市場均衡。

## 第4題
**題目：** 
考慮一個風險投資組合。從該投資組合獲得的年終現金流將是$70,000或$200,000，各有0.5的相等概率。無風險國庫券的替代投資每年支付2%。
a. 如果你要求8%的風險溢價，你願意為該投資組合支付多少？
b. 假設可以按你在(a)中找到的金額購買投資組合。投資組合的預期回報率是多少？
c. 現在假設你要求12%的風險溢價。你願意支付什麼價格？
d. 比較你對(a)和(c)的回答，你對投資組合所需風險溢價與投資組合售價之間的關係有什麼結論？

**解答：**
a. 預期現金流是：(0.5 × $70,000) + (0.5 × $200,000) = $135,000。
   要求的風險溢價為8%加上2%的無風險利率，所需回報率為10%。因此，投資組合的現值為：
   $135,000 / 1.10 = $122,727

b. 如果投資組合購買價為$122,727並提供預期現金流入$135,000，則預期回報率(E[r])如下：
   $122,727 × (1 + E[r]) = $135,000
   因此，E(r) = 10%。投資組合價格設定為使預期回報率等於所需回報率。

c. 如果超過國庫券的風險溢價現在為12%，則所需回報率為：
   2% + 12% = 14%
   投資組合的現值現在為：$135,000 / 1.14 = $118,421

d. 對於給定的預期現金流，要求更高風險溢價的投資組合必須以較低價格出售。從預期值的額外折扣是風險的懲罰。

**初學者解釋：**
這個問題涉及風險溢價如何影響資產定價。讓我們一步步解釋：

a. 首先計算預期現金流：
   - 50%機會獲得$70,000
   - 50%機會獲得$200,000
   - 預期現金流 = 0.5 × $70,000 + 0.5 × $200,000 = $135,000
   
   你要求8%的風險溢價加上2%的無風險利率，總共是10%的必要回報率。
   因此，你願意支付的價格 = $135,000 / 1.10 = $122,727

b. 如果你以$122,727購買這個投資組合，一年後預期獲得$135,000，預期回報率為：
   ($135,000 - $122,727) / $122,727 = $12,273 / $122,727 = 10%
   
   注意這與所需回報率相同，這不是巧合。在有效市場中，資產價格會調整到使預期回報等於所需回報。

c. 如果你要求12%的風險溢價（總必要回報率為14%），你願意支付的價格為：
   $135,000 / 1.14 = $118,421

d. 比較a和c的結果，我們可以得出結論：所需風險溢價越高，投資者願意支付的價格越低。這反映了風險的基本特性 - 投資者需要通過支付較低價格（從而獲得較高潛在回報）來補償承擔額外風險。

## 第5題
**題目：** 
考慮一個提供7%預期回報率和18%標準差的投資組合。國庫券提供2%的無風險回報率。風險趨避程度的最大水平是多少，使得風險投資組合仍然優於國庫券？

**解答：**
當我們用U = E(r) - 0.5A×σ²來描述效用時，國庫券的效用水平為：0.02

風險投資組合的效用水平為：
U = 0.07 - 0.5 × A × (0.18)² = 0.07 - 0.0162 × A

為了使風險投資組合優於國庫券，必須滿足以下條件：
0.07 - 0.0162 × A > 0.02 → A < 0.05 / 0.0162 = 3.09

A必須小於3.09，風險投資組合才能優於國庫券。

**初學者解釋：**
這個問題涉及風險趨避係數(A)如何影響投資選擇。

首先，我們需要理解投資者的效用函數：U = E(r) - 0.5A×σ²，其中：
- E(r)是預期回報率
- σ是標準差（風險）
- A是風險趨避係數

1. 國庫券的效用計算：
   - 預期回報 = 2% = 0.02
   - 標準差 = 0（無風險）
   - 效用 = 0.02 - 0.5 × A × 0² = 0.02

2. 風險投資組合的效用計算：
   - 預期回報 = 7% = 0.07
   - 標準差 = 18% = 0.18
   - 效用 = 0.07 - 0.5 × A × (0.18)² = 0.07 - 0.0162 × A

3. 要使風險投資組合優於國庫券，其效用必須更高：
   0.07 - 0.0162 × A > 0.02

   -0.0162 × A > 0.02 - 0.07

   -0.0162 × A > -0.05

   A < 0.05 / 0.0162

   A < 3.09

因此，當風險趨避係數小於3.09時，投資者會選擇風險投資組合。當A大於3.09時，投資者會選擇國庫券。

這表明輕度至中度風險趨避的投資者（A < 3.09）會選擇風險投資組合，而高度風險趨避的投資者（A > 3.09）則會選擇國庫券。

## 第6題
**題目：** 
在預期回報-標準差平面上繪製對應於效用水平0.02、風險趨避係數為3的投資者的無差異曲線。（提示：選擇幾個可能的標準差，範圍從0到0.25，找出提供0.02效用水平的預期回報率。然後繪製由此得出的預期回報-標準差點。）

**解答：**
答案會有所不同。曲線上的點是通過解決以下方程式中的E(r)得出的：
U = 0.02 = E(r) ? .5σ² = E(r) - 0.5×3×σ²

給定σ²值的E(r)值因此為：

| σ | σ² | E(r) |
|---|-----|-------|
| 0.00 | 0.0000 | 0.0200 |
| 0.05 | 0.0025 | 0.0238 |
| 0.10 | 0.0100 | 0.0350 |
| 0.15 | 0.0225 | 0.0538 |
| 0.20 | 0.0400 | 0.0800 |
| 0.25 | 0.0625 | 0.1138 |

下一頁圖中的粗線（標記為Q6，代表問題6）描繪了無差異曲線。

**初學者解釋：**
無差異曲線是投資者認為同等有吸引力的風險和回報組合的集合。

對於這個問題，我們需要找出所有使投資者效用等於0.02的風險-回報組合。

使用效用函數：U = E(r) - 0.5A×σ²，其中A = 3，我們需要解出每個風險水平對應的預期回報率：

0.02 = E(r) - 0.5 × 3 × σ²
E(r) = 0.02 + 1.5 × σ²

現在，我們可以計算不同風險水平(σ)對應的預期回報率(E(r))：

1. 當σ = 0（無風險）：
   E(r) = 0.02 + 1.5 × 0² = 0.02 (2%)

2. 當σ = 0.05 (5%)：
   E(r) = 0.02 + 1.5 × 0.0025 = 0.02 + 0.00375 = 0.02375 ≈ 0.0238 (2.38%)

3. 當σ = 0.10 (10%)：
   E(r) = 0.02 + 1.5 × 0.01 = 0.02 + 0.015 = 0.035 (3.5%)

4. 當σ = 0.15 (15%)：
   E(r) = 0.02 + 1.5 × 0.0225 = 0.02 + 0.03375 = 0.05375 ≈ 0.0538 (5.38%)

5. 當σ = 0.20 (20%)：
   E(r) = 0.02 + 1.5 × 0.04 = 0.02 + 0.06 = 0.08 (8%)

6. 當σ = 0.25 (25%)：
   E(r) = 0.02 + 1.5 × 0.0625 = 0.02 + 0.09375 = 0.11375 ≈ 0.1138 (11.38%)

繪製這些點會得到一條向上彎曲的曲線，表示隨著風險增加，投資者需要更多的預期回報來維持相同的效用水平。

## 第7題
**題目：** 現在繪製對應於風險趨避係數A = 4的投資者0.02效用水平的無差異曲線。比較你的答案與問題6，你有什麼結論？

**解答：**
重複問題6的分析，效用現在為：
U = E(r) - 0.5Aσ² = E(r) - 0.5 × 4 × σ² = 0.02

下表中呈現的預期回報和標準差的等效用組合。下一頁圖中的上升斜率線是無差異曲線，標記為Q7（代表問題7）。

| σ | σ² | E(r) |
|---|-----|-------|
| 0.00 | 0.0000 | 0.0200 |
| 0.05 | 0.0025 | 0.0250 |
| 0.10 | 0.0100 | 0.0400 |
| 0.15 | 0.0225 | 0.0650 |
| 0.20 | 0.0400 | 0.1000 |
| 0.25 | 0.0625 | 0.1450 |

問題7中的無差異曲線與問題6中的曲線在斜率上有所不同。當A從3增加到4時，增加的風險趨避導致無差異曲線斜率更大，因為需要更多的預期回報來補償額外的σ。

**初學者解釋：**
在這個問題中，我們使用A = 4（而不是問題6中的A = 3）重複計算無差異曲線。

使用效用函數：U = E(r) - 0.5A×σ²，其中A = 4，我們需要解出：

0.02 = E(r) - 0.5 × 4 × σ²
E(r) = 0.02 + 2.0 × σ²

計算不同風險水平對應的預期回報：

1. 當σ = 0：E(r) = 0.02 + 2.0 × 0 = 0.02 (2%)
2. 當σ = 0.05：E(r) = 0.02 + 2.0 × 0.0025 = 0.025 (2.5%)
3. 當σ = 0.10：E(r) = 0.02 + 2.0 × 0.01 = 0.04 (4%)
4. 當σ = 0.15：E(r) = 0.02 + 2.0 × 0.0225 = 0.065 (6.5%)
5. 當σ = 0.20：E(r) = 0.02 + 2.0 × 0.04 = 0.10 (10%)
6. 當σ = 0.25：E(r) = 0.02 + 2.0 × 0.0625 = 0.145 (14.5%)

比較兩條無差異曲線，我們可以得出以下結論：

1. 兩條曲線都從相同點開始（無風險資產，回報2%）
2. A = 4的曲線比A = 3的曲線更陡峭
3. 這表明風險趨避度更高的投資者需要更多的額外回報才能接受相同的額外風險
4. 例如，對於20%的標準差，A = 3的投資者需要8%的回報，而A = 4的投資者需要10%的回報才能達到相同的效用水平

這反映了風險趨避的基本原理：風險趨避度越高的投資者要求更高的風險溢價來補償同等的風險增加。

## 第8題
**題目：** 為風險中性投資者繪製提供0.02效用水平的無差異曲線。

**解答：**
風險中性投資者的風險趨避係數為零。因此，對應的效用等於投資組合的預期回報。在預期回報-標準差平面上的相應無差異曲線是一條水平線，在上圖中標記為Q8（見問題6）。

| σ | σ² | E(r) |
|---|-----|-------|
| 0.00 | 0.0000 | 0.0200 |
| 0.05 | 0.0025 | 0.0200 |
| 0.10 | 0.0100 | 0.0200 |
| 0.15 | 0.0225 | 0.0200 |
| 0.20 | 0.0400 | 0.0200 |
| 0.25 | 0.0625 | 0.0200 |

**初學者解釋：**
風險中性投資者(A = 0)只關心預期回報，而不考慮風險。他們的效用函數簡化為：

U = E(r) - 0.5 × 0 × σ² = E(r)

因此，對於風險中性投資者，無差異曲線是一條水平線，表示無論風險水平如何，只要預期回報相同，投資者的效用也相同。

在這個例子中，對於效用水平0.02，所有回報為2%的投資組合對風險中性投資者來說都是同等有吸引力的，不管風險是0%、5%、10%、20%或任何其他水平。

風險中性投資者會總是選擇預期回報最高的投資，無論其風險如何。

## 第9題
**題目：** 風險愛好者的風險趨避係數的符號必須是什麼？為風險愛好者繪製提供0.02效用水平的無差異曲線。

**解答：**
風險愛好者（這裡，A = -3），不是為了考慮風險而降低投資組合效用，而是隨著方差增加而獲得更大效用。這相當於負的風險趨避係數。上圖中的相應無差異曲線是向下傾斜的（見問題6），標記為Q9。

| σ | σ² | E(r) |
|---|-----|-------|
| 0.00 | 0.0000 | 0.0200 |
| 0.05 | 0.0025 | 0.0163 |
| 0.10 | 0.0100 | 0.0050 |
| 0.15 | 0.0225 | (0.0138) |
| 0.20 | 0.0400 | (0.0400) |
| 0.25 | 0.0625 | (0.0738) |

**初學者解釋：**
風險愛好者是喜歡風險的投資者，他們的風險趨避係數為負值(A < 0)。他們的效用函數為：

U = E(r) - 0.5A×σ²，其中A < 0

為風險愛好者使用A = -3，效用方程式變為：

U = E(r) - 0.5 × (-3) × σ² = E(r) + 1.5 × σ²

求解0.02效用水平的E(r)：

0.02 = E(r) + 1.5 × σ²
E(r) = 0.02 - 1.5 × σ²

計算不同風險水平對應的預期回報：

1. 當σ = 0：E(r) = 0.02 - 1.5 × 0 = 0.02 (2%)
2. 當σ = 0.05：E(r) = 0.02 - 1.5 × 0.0025 = 0.0163 (1.63%)
3. 當σ = 0.10：E(r) = 0.02 - 1.5 × 0.01 = 0.005 (0.5%)
4. 當σ = 0.15：E(r) = 0.02 - 1.5 × 0.0225 = -0.0138 (-1.38%)
5. 當σ = 0.20：E(r) = 0.02 - 1.5 × 0.04 = -0.04 (-4%)
6. 當σ = 0.25：E(r) = 0.02 - 1.5 × 0.0625 = -0.0738 (-7.38%)

這產生一條向下傾斜的無差異曲線，表明風險愛好者願意接受較低的預期回報（甚至負回報）來換取更高的風險。這與風險趨避投資者的向上傾斜曲線形成鮮明對比。

風險愛好者實際上願意「支付」（以較低預期回報的形式）來獲得更多風險，這在大多數金融市場中是不典型的行為。

<img width="247" alt="截圖 2025-04-16 下午1 54 23" src="https://github.com/user-attachments/assets/17bff9c0-f704-4b9b-9e3f-1c4eeb772b29" />

## 第10-12題的背景資料

考慮歷史數據顯示，過去95年中S&P 500投資組合的平均年回報率大約比國庫券回報高8%，而S&P 500的標準差約為每年20%。假設這些數值代表投資者對未來表現的預期，且當前國庫券利率為2%。

## 第10題
**題目：** 計算投資於國庫券和S&P 500指數的投資組合，按以下權重的預期回報和方差：

| Wbills | Windex |
|--------|---------|
| 0      | 1.0     |
| 0.2    | 0.8     |
| 0.4    | 0.6     |
| 0.6    | 0.4     |
| 0.8    | 0.2     |
| 1.0    | 0       |

**解答：**
投資組合的預期回報和方差計算如下：

| (1)    | (2)    | (3)    | (4)     | rPortfolio        | σPortfolio  | σ²Portfolio |
|--------|--------|--------|---------|-------------------|-------------|-------------|
| WBills | rBills | WIndex | rIndex  | (1)×(2)+(3)×(4)   | (3) × 20%   |             |
| 0.0    | 2%     | 1.0    | 10.0%   | 10.00%            | 20.00%      | 0.0400      |
| 0.2    | 2      | 0.8    | 10.0    | 8.40%             | 16.00%      | 0.0256      |
| 0.4    | 2      | 0.6    | 10.0    | 6.80%             | 12.00%      | 0.0144      |
| 0.6    | 2      | 0.4    | 10.0    | 5.20%             | 8.00%       | 0.0064      |
| 0.8    | 2      | 0.2    | 10.0    | 3.60%             | 4.00%       | 0.0016      |
| 1.0    | 2      | 0.0    | 10.0    | 2.00%             | 0.00%       | 0.0000      |

**初學者解釋：**
這個問題要求我們計算不同配置下投資組合的預期回報率和風險。

首先，我們需要確定股票市場(S&P 500)的預期回報率：
- 無風險利率(國庫券) = 2%
- 股票風險溢價 = 8%
- 因此，股票預期回報率 = 2% + 8% = 10%

然後，我們可以計算不同投資組合的預期回報率和標準差：

1. 預期回報率 = (國庫券配置 × 國庫券回報率) + (股票配置 × 股票回報率)
2. 投資組合標準差 = 股票配置 × 股票標準差(20%)

例如，對於80%投資於股票、20%投資於國庫券的投資組合：
- 預期回報率 = (0.2 × 2%) + (0.8 × 10%) = 0.4% + 8% = 8.4%
- 標準差 = 0.8 × 20% = 16%

這個計算說明了多元化的效果：隨著你從全部股票轉向部分國庫券投資，風險（標準差）下降，但預期回報也下降。這是投資中風險與回報的基本權衡。

## 第11題
**題目：** 計算A = 2的投資者對問題10中每個投資組合的效用水平。你得出什麼結論？

**解答：**
從U = E(r) - 0.5Aσ² = E(r) - σ²計算效用，我們得到下表中標記為U(A = 2)列的值：

| WBills | WIndex | rPortfolio | σPortfolio | σ²Portfolio | U(A = 2) | U(A = 3) |
|--------|--------|------------|------------|-------------|----------|----------|
| 0.0    | 1.0    | 10.00%     | 20.00%     | 0.0400      | 0.0600   | 0.0400   |
| 0.2    | 0.8    | 8.40%      | 16.00%     | 0.0256      | 0.0584   | 0.0456   |
| 0.4    | 0.6    | 6.80%      | 12.00%     | 0.0144      | 0.0536   | 0.0464   |
| 0.6    | 0.4    | 5.20%      | 8.00%      | 0.0064      | 0.0456   | 0.0424   |
| 0.8    | 0.2    | 3.60%      | 4.00%      | 0.0016      | 0.0344   | 0.0336   |
| 1.0    | 0.0    | 2.00%      | 0.00%      | 0.0000      | 0.0200   | 0.0200   |

標記為U(A = 2)的列表明風險趨避係數A = 2的投資者相比表中的其他投資組合，更偏好100%投資於市場指數的投資組合。

**初學者解釋：**
這個問題要求我們評估風險趨避係數A = 2的投資者對不同投資組合的偏好。

投資者的效用計算公式為：U = E(r) - 0.5 × A × σ²

對於A = 2，這變為：U = E(r) - 1 × σ²

我們計算每個投資組合的效用：

1. 100%股票：U = 10% - 1 × 0.04 = 6%
2. 80%股票：U = 8.4% - 1 × 0.0256 = 5.84%
3. 60%股票：U = 6.8% - 1 × 0.0144 = 5.36%
4. 40%股票：U = 5.2% - 1 × 0.0064 = 4.56%
5. 20%股票：U = 3.6% - 1 × 0.0016 = 3.44%
6. 0%股票：U = 2% - 1 × 0 = 2%

結論：對於風險趨避係數A = 2的投資者，效用最高的投資組合是100%投資於股票。這表明，儘管該投資者有一定程度的風險趨避，但市場風險溢價足夠高，使全股票投資組合成為最佳選擇。

## 第12題
**題目：** 對風險趨避係數A = 3的投資者重複問題11。你得出什麼結論？

**解答：**
上表中標記為U(A = 3)的列是從以下公式計算的：
U = E(r) - 0.5Aσ² = E(r) - 1.5σ²

較風險趨避的投資者(A = 3)偏好投資60%於市場，而不是風險趨避係數A = 2的投資者偏好的100%市場權重。

**初學者解釋：**
現在我們考慮風險趨避度更高(A = 3)的投資者。

效用計算公式變為：U = E(r) - 0.5 × 3 × σ² = E(r) - 1.5 × σ²

對每個投資組合計算效用：

1. 100%股票：U = 10% - 1.5 × 0.04 = 10% - 6% = 4%
2. 80%股票：U = 8.4% - 1.5 × 0.0256 = 8.4% - 3.84% = 4.56%
3. 60%股票：U = 6.8% - 1.5 × 0.0144 = 6.8% - 2.16% = 4.64%
4. 40%股票：U = 5.2% - 1.5 × 0.0064 = 5.2% - 0.96% = 4.24%
5. 20%股票：U = 3.6% - 1.5 × 0.0016 = 3.6% - 0.24% = 3.36%
6. 0%股票：U = 2% - 1.5 × 0 = 2%

結論：對於風險趨避係數A = 3的投資者，最佳投資組合是60%投資於股票、40%投資於國庫券。與A = 2的投資者相比，這位投資者因風險趨避度更高，選擇了更保守的投資組合。

這說明風險趨避度如何影響投資選擇：風險趨避度越高，投資者傾向於在投資組合中減少風險資產配置。

## 第13題
**題目：** 你管理著一個風險投資組合，預期回報率為12%，標準差為28%。國庫券利率為2%。你的客戶選擇將投資組合的70%投資於你的基金，30%投資於實際上無風險的貨幣市場基金。他的投資組合的預期值和回報率標準差是多少？

**解答：**
預期回報率 = (0.7 × 12%) + (0.3 × 2%) = 9%
標準差 = 0.7 × 28% = 19.6%

**初學者解釋：**
這是一個組合投資計算的問題。客戶將資金分為兩部分：
- 70%投資於你的風險基金（回報率12%，標準差28%）
- 30%投資於無風險貨幣市場基金（回報率2%，標準差0%）

1. 計算組合投資的預期回報率：
   - 使用加權平均：E(r) = w₁ × r₁ + w₂ × r₂
   - E(r) = 0.7 × 12% + 0.3 × 2% = 8.4% + 0.6% = 9%

2. 計算組合投資的標準差：
   - 由於投資部分為無風險，標準差僅受風險資產影響：σₚ = w₁ × σ₁
   - σₚ = 0.7 × 28% = 19.6%

這種組合策略使客戶能夠實現比100%投資於風險基金更低的風險水平，但也獲得比100%投資於無風險資產更高的預期回報。

## 第14題
**題目：** 假設你的風險投資組合包括以下比例的投資：

股票A 25%

股票B 32%

股票C 43%

你的客戶的整體投資組合（包括國庫券的投資）中每種資產的投資比例是多少？

**解答：**
投資比例：

30.0%投資於國庫券

0.7 × 25% = 17.5%投資於股票A

0.7 × 32% = 22.4%投資於股票B

0.7 × 43% = 30.1%投資於股票C

**初學者解釋：**
這個問題要求我們計算客戶整體投資組合中每個單獨資產的配置比例。

我們知道客戶將70%資金投入風險基金，30%投入國庫券。風險基金內部有自己的資產分配。因此：

1. 國庫券配置 = 30%
2. 股票A配置 = 70% × 25% = 17.5%（客戶投入風險基金的比例 × 風險基金內股票A的比例）
3. 股票B配置 = 70% × 32% = 22.4%
4. 股票C配置 = 70% × 43% = 30.1%

檢查：17.5% + 22.4% + 30.1% + 30.0% = 100%，所以我們的計算是正確的。

這種分層配置方法在投資管理中很常見，投資者通常會選擇投資基金的組合，每個基金內部又有多種資產。

## 第15題
**題目：** 你的風險投資組合的回報與波動性（夏普）比率(S)是多少？你的客戶的比率是多少？

**解答：**
你的回報與波動性（夏普）比率：S = (0.12 - 0.02)/0.28 = 0.3571

客戶的回報與波動性（夏普）比率：S = (0.09 - 0.02)/0.196 = 0.3571

**初學者解釋：**
夏普比率是衡量每單位風險的超額回報的關鍵指標，計算公式為：

夏普比率 = (預期回報率 - 無風險利率) / 標準差

1. 風險基金的夏普比率：
   S = (12% - 2%) / 28% = 10% / 28% = 0.3571

2. 客戶投資組合的夏普比率：
   S = (9% - 2%) / 19.6% = 7% / 19.6% = 0.3571

有趣的是，兩個投資組合的夏普比率相同。這不是巧合！當投資者在無風險資產和相同的風險資產組合之間分配資金時，所有可能的投資組合都具有相同的夏普比率。這是資本配置線(CAL)的基本特性。

## 第16題
**題目：** 在預期回報-標準差圖上繪製你的投資組合的資本配置線(CAL)。CAL的斜率是多少？顯示你的客戶在你的基金CAL上的位置。

**解答：**

<img width="376" alt="截圖 2025-04-16 下午2 08 46" src="https://github.com/user-attachments/assets/7fb1a75e-b3d7-4b8b-a4e6-51f604c9a8f8" />


**初學者解釋：**
資本配置線(CAL)是通過將無風險資產與風險投資組合混合而產生的所有可能投資組合的圖形表示。

CAL的斜率等於夏普比率：0.3571

圖表中，CAL從無風險利率點(0%, 2%)開始，穿過風險基金點(28%, 12%)，並繼續延伸。客戶的投資組合位於CAL上，在點(19.6%, 9%)處，對應於70%投資於風險基金和30%投資於無風險資產。

這條線表示通過混合風險基金和無風險資產可以實現的最佳風險-回報組合。線上的每一點都是不同資金分配比例的結果。

## 第17題
**題目：** 假設你的客戶決定將總投資預算的一部分y投資於你的投資組合，使整體投資組合的預期回報率為10%。
a. 比例y是多少？
b. 你的客戶在你的三只股票和國庫券基金中的投資比例是多少？
c. 你的客戶投資組合的回報率標準差是多少？

**解答：**

a. E(rc) = rf + y × [E(rp) - rf] = 0.02 + y × (0.12 - 0.02)
   
   如果整體投資組合的預期回報率為10%，則：
   
   10% = 2% + 10% × y ⇒ y = (10% - 2%) / 10% = 0.8
   
   因此，為了使投資組合預期回報率等於10%，客戶必須將80%的資金投資於風險投資組合，20%投資於國庫券。

b. 客戶的投資比例：
   
   20.0%投資於國庫券
   
   0.8 × 25% = 20.0%投資於股票A
   
   0.8 × 32% = 25.6%投資於股票B
   
   0.8 × 43% = 34.4%投資於股票C

c. σc = 0.8 × 28% = 22.4%

**初學者解釋：**
這個問題要求我們確定需要多少比例投資於風險基金才能實現10%的目標回報率。

a. 我們使用資本配置線方程式：
   E(r) = rf + y × (E(rp) - rf)
   
   其中：
   - E(r)是目標回報率 = 10%
   - rf是無風險利率 = 2%
   - E(rp)是風險投資組合回報率 = 12%
   - y是投資於風險投資組合的比例
   
   10% = 2% + y × (12% - 2%)
   
   10% = 2% + y × 10%
   
   8% = y × 10%
   
   y = 80%
   
   因此，投資者需要投資80%於風險基金，20%於國庫券。

b. 計算每個資產的配置比例：
   - 國庫券: 20%
   - 股票A: 80% × 25% = 20%
   - 股票B: 80% × 32% = 25.6%
   - 股票C: 80% × 43% = 34.4%

c. 投資組合標準差:
   σ = y × σp = 0.8 × 28% = 22.4%
   
   這表示投資組合的風險（波動性）為22.4%。

## 第18題
**題目：** 假設你的客戶偏好將總投資預算的一部分y投資於你的基金，以最大化完整投資組合的預期回報，但限制條件是完整投資組合的標準差不超過12%。
a. 投資比例y是多少？
b. 完整投資組合的預期回報率是多少？

**解答：**
a. σc = y × 28%
   如果你的客戶偏好標準差最多為12%，則：
   y = 0.12 / 0.28 = 0.4286 = 42.86%投資於風險投資組合。
   
b. E(rc) = 0.02 + 0.1 × y = 0.02 + (0.1 × 0.4286) = 0.0629 = 6.29%

**初學者解釋：**
這個問題要求我們在風險限制下最大化投資組合回報。

a. 客戶的風險限制為12%標準差。
   由於投資組合標準差 = y × σp，其中σp = 28%
   12% = y × 28%
   y = 12% / 28% = 0.4286
   
   因此，客戶應該投資42.86%於風險基金，57.14%於國庫券。

b. 計算預期回報率：
   E(r) = rf + y × (E(rp) - rf)
   E(r) = 2% + 0.4286 × (12% - 2%)
   E(r) = 2% + 0.4286 × 10%
   E(r) = 2% + 4.29%
   E(r) = 6.29%
   
   在12%風險限制下，客戶的最大可能預期回報率為6.29%。

## 第19題
**題目：** 你的客戶的風險趨避程度為A = 3.5。
a. 應該將總投資的多少比例y投資於你的基金？
b. 你的客戶經過優化的投資組合的預期值和回報率標準差是多少？

**解答：**

a. 

$$
y^* = \frac{E(r_p) - r_f}{A \sigma_p^2}
$$

   y* = (0.12 - 0.02) / (3.5 × 0.28²) = 0.10 / 0.2744 = 0.3644
   因此，客戶的最優比例是：36.44%投資於風險投資組合，63.56%投資於國庫券。

b. E(rc) = 0.02 + 0.10 × y = 0.02 + (0.3644 × 0.1) = 0.05644 或 5.644%
   σc = 0.3644 × 28 = 10.203%

**初學者解釋：**
這個問題應用了風險趨避係數來確定最優投資比例。

a. 最優投資比例公式：
   
   $$
   y^* = \frac{E(r_p) - r_f}{A \sigma_p^2}
   $$
   
   代入數據：
   y* = (12% - 2%) / (3.5 × 0.28²)
   y* = 10% / (3.5 × 0.0784)
   y* = 10% / 0.2744
   y* = 0.3644
   
   因此，風險趨避係數為3.5的投資者應該投資36.44%於風險基金，63.56%於國庫券。

b. 計算預期回報率：
   E(r) = 2% + (36.44% × 10%) = 5.644%
   
   計算標準差：
   σ = 36.44% × 28% = 10.203%
   
   這是此風險趨避度下的最優投資組合特性。

## 第20題
**題目：** 查看表6.7中美國股票市場的平均超額回報和超額回報的標準差數據。假設美國市場是你的風險投資組合。
a. 如果你的風險趨避係數為A = 4，並且你相信整個1927-2021年期間代表未來預期表現，那麼你的投資組合應該分配多少比例給國庫券和多少給股票？
b. 如果你相信1975-1998年期間具有代表性呢？
c. 比較(a)和(b)的答案，你得出什麼結論？

**解答：**
a. 如果假設1927-2021年期間代表未來預期表現，那麼我們使用以下數據計算配置給股票的比例：A = 4, E(rM) - rf = 8.87%, σM = 20.25%（我們使用表6.7中風險溢價的標準差）。然後y*由以下公式給出：

   $$
   y^* = \frac{E(r_p) - r_f}{A \sigma_p^2}
   $$
   
   y*  = 0.0887 / (4 × 0.2025²) = 0.5408
   
   即54.08%的投資組合應配置給股票，45.92%應配置給國庫券。

b. 如果假設1975-1998年期間代表未來預期表現，那麼我們使用以下數據計算配置給股票的比例：A = 4, E(rM) - rf = 11.00%, σM = 14.40%，y*由以下公式給出：

   $$
   y^* = \frac{E(r_p) - r_f}{A \sigma_p^2}
   $$
   
   y* = .1100 / (4 × .1440²) = 1.3262
   
   因此，132.62%的完整投資組合應通過借入32.62%的國庫券配置給股票。

c. 在部分b中，市場風險溢價預期高於部分a，但市場風險低於部分a。因此，回報與波動性比率預期在部分b中高得多，這解釋了為什麼需要借入國庫券來擴大對股票的敞口。

**初學者解釋：**
這個問題展示了不同歷史時期數據如何影響投資決策。

a. 使用1927-2021年的長期數據：
   - 風險溢價(E(rM) - rf) = 8.87%
   - 標準差(σM) = 20.25%
   - 風險趨避係數(A) = 4
   
   最優配置：
   y* = 8.87% / (4 × 20.25%²) = 8.87% / (4 × 0.041) = 8.87% / 0.164 = 54.08%
   
   投資者應配置54.08%於股票，45.92%於國庫券。

b. 使用1975-1998年的數據：
   - 風險溢價 = 11%
   - 標準差 = 14.4%
   - 風險趨避係數 = 4
   
   最優配置：
   y* = 11% / (4 × 14.4%²) = 11% / (4 × 0.0207) = 11% / 0.0829 = 132.62%
   
   投資者應該借入32.62%資金（槓桿），並將132.62%投資於股票。

c. 比較這兩個結果，我們可以得出重要結論：
   - 1975-1998年期間，股票表現出更高的風險溢價和更低的波動性
   - 這導致更高的風險調整回報率（夏普比率）
   - 高夏普比率使槓桿投資更具吸引力
   - 市場條件的歷史變化對投資決策有重大影響
   
   這強調了投資前提的重要性：你對未來市場表現的假設將極大地影響你的最優資產配置。


## 第23-24題的背景資料
對於第23至26題：假設你的客戶面臨的借款利率是**9%**。假設股票市場指數的預期回報率為**13%**，標準差為25%，rf = **5%**，你的基金具有問題21中給出的參數。
## 第23題
**題目：** 
繪製考慮較高借款利率的客戶資本市場線(CML)圖。在圖上疊加兩組無差異曲線，一組用於將選擇借款的客戶，一組用於將同時投資於指數基金和貨幣市場基金的客戶。

**解答：**
數據：rf = 5%, E(rM) = 13%, σM = 25%, 借款利率 rfB = 9%

<img width="358" alt="截圖 2025-04-16 下午2 24 13" src="https://github.com/user-attachments/assets/d3c25e50-6a7a-4873-9255-ef3483238771" />

CML和無差異曲線的圖形會顯示：
- 從無風險資產(0%, 5%)到市場投資組合(25%, 13%)的第一段
- 從市場投資組合向上延伸的第二段，斜率較小，反映較高的借款成本
- 兩組無差異曲線：一組與CML的借款部分相切，一組與CML的貸款部分相切

**初學者解釋：**
這個問題探討當借款利率(9%)高於無風險利率(5%)時的投資決策。

資本市場線(CML)在這種情況下會呈現「折線」形狀：
- 第一段（從原點到市場投資組合）：斜率 = (13% - 5%)/25% = 0.32
- 第二段（借款部分）：斜率 = (r - 13%)/(σ - 25%)，其中r和σ是借款投資組合的回報率和標準差

第一段表示將資金在無風險資產和市場投資組合之間分配的所有可能組合。第二段表示通過借入資金（以9%的利率）來槓桿投資市場投資組合的所有可能組合。

無差異曲線代表投資者對具有相同效用水平的不同風險-回報組合的偏好。圖表上有兩組無差異曲線：
1. 一組對應於風險承受能力較低的投資者，他們的最優選擇是將資金分配在無風險資產和市場投資組合之間
2. 另一組對應於風險承受能力較高的投資者，他們願意通過借款來槓桿投資

這種圖形說明了借款成本對投資決策的重要影響。較高的借款利率降低了槓桿投資的吸引力，使更多投資者選擇在無風險資產和市場投資組合之間分配資金。

## 第24題
**題目：** 客戶既不借款也不貸款（即y = 1）的風險趨避範圍是多少？

**解答：**

   $$
   y^* = \frac{E(r_p) - r_f}{A \sigma_p^2}
   $$
   
對於y小於1（即投資者是貸款人），風險趨避係數(A)必須足夠大，使得：

y = (E(rM) - rf) / (A × σM²) < 1 ⇒ A > (E(rM) - rf) / σM² = (13% - 5%) / 0.25² = 1.28

對於y大於1（即投資者是借款人），風險趨避係數必須足夠小：

y = (E(rM) - rfB) / (A × σM²) > 1 ⇒ A < (E(rM) - rfB) / σM² = (13% - 9%) / 0.25² = 0.64

因此，在風險趨避係數在以下範圍內，客戶將既不借款也不貸款，而是持有僅由最優風險投資組合組成的投資組合：

y = 1，當 0.64 ≤ A ≤ 1.28

**初學者解釋：**
這個問題要求我們找出投資者會選擇完全投資於市場投資組合（不借款也不貸款）的風險趨避係數範圍。

在最優投資決策中，投資於風險資產的比例(y)由以下公式決定：

1. 對於貸款（y < 1）：y = (E(rM) - rf) / (A × σM²)
2. 對於借款（y > 1）：y = (E(rM) - rfB) / (A × σM²)

當y = 1（完全投資於市場）時，我們可以從這兩個方程導出風險趨避係數A的界限：

上界（貸款邊界）：
(E(rM) - rf) / (A × σM²) = 1
A = (E(rM) - rf) / σM²
A = (13% - 5%) / 0.25²
A = 8% / 0.0625
A = 1.28

下界（借款邊界）：
(E(rM) - rfB) / (A × σM²) = 1
A = (E(rM) - rfB) / σM²
A = (13% - 9%) / 0.25²
A = 4% / 0.0625
A = 0.64

因此，當風險趨避係數A在0.64到1.28之間時，投資者會選擇y = 1，即完全投資於市場投資組合，既不借款也不貸款。

- 如果A > 1.28（較高風險趨避），投資者會選擇部分資金投資於無風險資產(y < 1)
- 如果A < 0.64（較低風險趨避），投資者會借入資金擴大市場投資(y > 1)

值得注意的是，借款利率(9%)高於貸款利率(5%)擴大了「既不借款也不貸款」的風險趨避範圍。如果兩個利率相同，這個範圍會縮小。
