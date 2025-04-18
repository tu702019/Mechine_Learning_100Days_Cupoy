# 指數模型與投資組合風險分析 - 投資學解析

以下將針對第5-16題進行詳細解說，這些問題主要關注指數模型在投資組合分析中的應用，以及如何分析股票的系統性與非系統性風險。

## 問題5：投資組合優化所需的參數估計

**問題**：一個投資組合管理組織分析了60支股票，並使用這60支證券構建了一個均值-方差有效投資組合。
a. 優化此投資組合需要多少個預期報酬率、方差和協方差的估計值？
b. 如果可以安全地假設股票市場報酬率與單一指數模型結構相似，需要多少個估計值？

**解答**：

### a. 傳統Markowitz模型所需參數

傳統的Markowitz投資組合理論需要估計：
- 60個預期報酬率（每支股票一個）
- 60個方差（每支股票風險的平方）
- 1,770個協方差 (n²-n)/2，其中n=60

總共需要1,890個參數估計 = (n²+3n)/2 = (60²+3×60)/2 = 1,890

### b. 單一指數模型所需參數

單一指數模型的基本形式：ri - rf = αi + βi(rM - rf) + ei
或用超額報酬表示：Ri = αi + βiRM + ei

在此模型中，股票報酬率的方差可以分解為：
1. 由共同市場因素引起的方差：βi²σM²
2. 由公司特定非預期事件引起的方差：σ²(ei)

在單一指數模型中，股票間的協方差：Cov(ri,rj) = βiβjσM²

因此需要的參數估計數量為：
- 60個預期報酬率 E(ri)
- 60個敏感度係數 βi
- 60個公司特定方差 σ²(ei)
- 1個市場平均報酬率 E(rM)
- 1個市場方差 σM²

總共需要182個參數估計。

**為什麼這很重要？** 單一指數模型將需要的估計參數從1,890個減少到182個，大幅降低了估計誤差的可能性和計算複雜度。一般來說，參數估計數量從(n²+3n)/2減少到(3n+2)，這是單一指數模型的主要優勢之一。

## 問題6：股票標準差與投資組合風險分析

**問題**：以下是兩支股票的估計值。

| 股票 | 預期報酬率 | 貝塔 | 公司特定標準差 |
|------|------------|------|----------------|
| A    | 13%        | 0.8  | 30%            |
| B    | 18%        | 1.2  | 40%            |

市場指數的標準差為22%，無風險利率為8%。

a. A股和B股的標準差是多少？
b. 假設我們構建一個比例為：股票A：0.30，股票B：0.45，國庫券：0.25的投資組合。計算投資組合的預期報酬率、貝塔、非系統性標準差和總標準差。

**解答**：

### a. 各股票的標準差

股票的總標準差由系統性風險和非系統性風險組成：
σi = [βi²σM² + σ²(ei)]^(1/2)

股票A：σA = [(0.8² × 22²) + 30²]^(1/2) = [310.4 + 900]^(1/2) = 34.78%

股票B：σB = [(1.2² × 22²) + 40²]^(1/2) = [696.96 + 1600]^(1/2) = 47.93%

### b. 投資組合分析

**投資組合預期報酬率**：
E(rP) = wA × E(rA) + wB × E(rB) + wf × rf
     = (0.30 × 13%) + (0.45 × 18%) + (0.25 × 8%) 
     = 3.9% + 8.1% + 2% 
     = 14%

**投資組合貝塔**：
βP = wA × βA + wB × βB + wf × βf
   = (0.30 × 0.8) + (0.45 × 1.2) + (0.25 × 0)
   = 0.24 + 0.54 + 0
   = 0.78

**投資組合非系統性方差**：
由於殘差(ei)是不相關的，非系統性方差是：
σ²(eP) = wA² × σ²(eA) + wB² × σ²(eB) + wf² × σ²(ef)
       = (0.30² × 30²) + (0.45² × 40²) + (0.25² × 0)
       = 81 + 324 + 0
       = 405

**投資組合非系統性標準差**：
σ(eP) = √405 = 20.12%

**投資組合總方差**：
σP² = βP²σM² + σ²(eP)
    = (0.78² × 22²) + 405
    = 294.47 + 405
    = 699.47

**投資組合總標準差**：
σP = √699.47 = 26.45%

**這告訴我們什麼？** 投資組合的風險來自兩部分：系統性風險(貝塔反映的市場風險)和非系統性風險(公司特定風險)。即使投資組合的貝塔(0.78)小於市場的貝塔(1.0)，由於存在非系統性風險，總風險仍然相當可觀。這顯示了風險分散的重要性，但也說明僅通過少數幾支股票難以完全消除非系統性風險。

## 問題7：股票特性線分析

**問題7**：考慮下圖中股票A和B的兩條回歸線。

<img width="440" alt="截圖 2025-04-16 下午3 30 10" src="https://github.com/user-attachments/assets/849da807-e130-453c-ac20-d84a3e17256d" />

a. 哪支股票具有較高的公司特定風險？
b. 哪支股票具有較大的系統性(市場)風險？
c. 哪支股票的R²值較高？
d. 哪支股票的阿爾法值較高？
e. 哪支股票與市場的相關性較高？

## 詳細解答

### a. 公司特定風險分析

**答案**：股票A具有較高的公司特定風險。

**初學者解釋**：
圖中的藍點代表真實的歷史收益數據，而紅線是最佳擬合線（證券特性線）。公司特定風險就是指那些不能由市場整體變動解釋的風險，在圖中表現為數據點與紅線的距離。

觀察圖形，你會發現：
- 股票A的數據點（藍點）散布得更廣，與紅線的垂直距離較大
- 股票B的數據點更接近其紅線

這些垂直距離越大，表示該股票有更多的價格變動無法用市場整體趨勢解釋，而是來自於公司自身的特定因素，如管理層決策、產品問題、競爭壓力等。因此，股票A的公司特定風險更高。

### b. 系統性風險分析

**答案**：股票B具有較大的系統性風險。

**初學者解釋**：
系統性風險反映了股票對整體市場變動的敏感度，由證券特性線的斜率（貝塔係數）衡量。斜率越陡，表示當市場變動時，股票價格變動幅度越大。

從圖中可以看出：
- 股票B的紅線斜率更陡峭
- 股票A的紅線斜率較平緩

這表示當市場上漲或下跌時，股票B的價格變動幅度比股票A更大。例如，當市場上漲1%時，股票B可能上漲1.5%，而股票A可能只上漲0.8%。因此，股票B的系統性風險更大。

### c. R²值分析

**答案**：股票B的R²值較高。

**初學者解釋**：
R²（決定係數）衡量了市場因素能解釋股票收益變動的程度。R²越高，表示股票的價格變動越多地由市場整體趨勢解釋，而非公司特定因素。

R²的計算公式為：
R² = 由市場解釋的方差 / 總方差 = β²σ²M / (β²σ²M + σ²(e))

$$
R^2 = \frac{\beta_i^2 \sigma_M^2}{\beta_i^2 \sigma_M^2 + \sigma^2(e_i)}
$$

股票B的R²更高，是因為：
1. 其貝塔值更高，使β²σ²M（解釋方差）更大
2. 其公司特定風險σ²(e)更小

從圖形上看，股票B的數據點更緊密地圍繞在回歸線周圍，表示市場因素能更好地解釋其價格變動。

### d. 阿爾法值分析

**答案**：股票A的阿爾法值較高。

**初學者解釋**：
阿爾法（α）是證券特性線與Y軸的交點，表示當市場沒有變動（超額收益為零）時，股票的預期超額收益。正的阿爾法表示股票表現優於其風險水平所預期的收益，負的阿爾法則相反。

從圖中可以看出：
- 股票A的紅線與Y軸相交於正值位置（小的正阿爾法）
- 股票B的紅線與Y軸相交於負值位置（負阿爾法）

這表示在考慮到風險因素後，股票A的表現超出預期，而股票B的表現不及預期。因此，股票A的阿爾法值較高。

### e. 市場相關性分析

**答案**：股票B與市場的相關性較高。

**初學者解釋**：
相關性衡量了股票價格變動與市場整體趨勢的一致程度。在單指數模型中，相關係數是R²的平方根。

由於股票B的R²更高，因此其相關係數（√R²）也更高。這表示股票B的價格變動更緊密地跟隨市場趨勢，而股票A的價格變動較為獨立。

高相關性並不一定意味著高風險，它只表示價格變動方向與市場高度一致。

## 問題8：股票特性線分析

**問題8**：考慮A和B的兩個（超額報酬）指數模型回歸結果：

RA = 1% + 1.2RM     R平方 = 0.576     殘差標準差 = 10.3%

RB = -2% + 0.8RM     R平方 = 0.436     殘差標準差 = 9.1%

a. 哪支股票有更高的公司特定風險？
b. 哪支股票有更大的市場風險？
c. 哪支股票的R²更高？
d. 哪支股票的阿爾法更高？
e. 哪支股票與市場的相關性更高？

**解答**：

### a. 公司特定風險比較

公司特定風險由殘差標準差衡量。股票A的殘差標準差為10.3%，股票B為9.1%。因此，**股票A有更高的公司特定風險**。

這表示股票A的價格波動中，有更大部分不能由市場整體波動解釋，而是由公司自身特定因素引起的。

### b. 系統性(市場)風險比較

系統性風險由貝塔係數衡量。股票A的貝塔為1.2，股票B的貝塔為0.8。因此，**股票A有更大的系統性風險**。

這意味著市場每變動1%，股票A平均會變動1.2%，而股票B僅變動0.8%。股票A對市場波動更敏感。

### c. R²比較

R²衡量由市場因素解釋的股票報酬率變異比例。股票A的R²為0.576，股票B的R²為0.436。因此，**股票A的R²更高**。

這表示市場因素能解釋股票A約57.6%的價格波動，而對股票B只能解釋43.6%。股票A的價格行為更受市場整體趨勢影響。

### d. 阿爾法比較

阿爾法是證券特性線與預期報酬軸的截距。股票A的阿爾法為1%，股票B的阿爾法為-2%。因此，**股票A的阿爾法更高**。

正阿爾法意味著相對於其承擔的系統性風險，股票A提供了超額收益，而股票B表現不佳。

### e. 與市場相關性比較

與市場的相關係數是R²的平方根。股票A的相關係數為√0.576 = 0.759，股票B的相關係數為√0.436 = 0.66。因此，**股票A與市場的相關性更高**。

**這告訴我們什麼？** 股票A與市場的聯動性更強，但也提供了正阿爾法(額外報酬)，雖然具有較高的非系統性風險。股票B與市場的聯動性較弱，但有負阿爾法，意味著其表現不及同等系統性風險的資產。

## 問題9-14：使用指數模型進行股票分析

這些問題使用以下數據：
- 股票A的指數模型：RA = 3% + 0.7RM + eA
- 股票B的指數模型：RB = -2% + 1.2RM + eB
- σM = 20%
- R平方A = 0.20
- R平方B = 0.12

### 問題9：計算每支股票的標準差

**解答**：
股票標準差可以從R²計算：
R² = 系統性方差/總方差 = β²σM²/σ²

股票A：
σA² = β²A × σM²/R²A = (0.7² × 20²)/0.20 = 196/0.20 = 980
     σA = √980 = 31.30%

股票B：
σB² = β²B × σM²/R²B = (1.2² × 20²)/0.12 = 576/0.12 = 4800
     σB = √4800 = 69.28%

### 問題10：將每支股票的方差分解為系統性和公司特定成分

**解答**：
股票A：
- 系統性風險 = β²A × σM² = 0.7² × 20² = 196
- 公司特定風險 = 總風險 - 系統性風險 = 980 - 196 = 784

股票B：
- 系統性風險 = β²B × σM² = 1.2² × 20² = 576
- 公司特定風險 = 總風險 - 系統性風險 = 4800 - 576 = 4224

### 問題11：計算兩支股票之間的協方差和相關係數

**解答**：
假設殘差不相關，協方差為：
Cov(rA, rB) = βA × βB × σM² = 0.7 × 1.2 × 20² = 0.7 × 1.2 × 400 = 336

相關係數：
ρAB = Cov(rA, rB)/(σA × σB) = 336/(31.30 × 69.28) = 336/2168.44 = 0.1549

### 問題12：計算每支股票與市場指數的協方差

**解答**：
相關係數是R²的平方根：
股票A與市場的協方差：
Cov(rA, rM) = ρA,M × σA × σM = √0.20 × 31.30 × 20 = 0.447 × 31.30 × 20 = 280

股票B與市場的協方差：
Cov(rB, rM) = ρB,M × σB × σM = √0.12 × 69.28 × 20 = 0.346 × 69.28 × 20 = 480

### 問題13：投資組合P分析

投資組合P的投資比例：60%在A，40%在B

**解答**：
標準差：
σP = [(0.6² × 980) + (0.4² × 4800) + (2 × 0.6 × 0.4 × 336)]^(1/2)
   = [352.8 + 768 + 161.28]^(1/2)
   = [1282.08]^(1/2)
   = 35.81%

貝塔：
βP = 0.6 × 0.7 + 0.4 × 1.2 = 0.42 + 0.48 = 0.90

非系統性方差：
σ²(eP) = σP² - βP²σM² = 1282.08 - (0.90² × 400) = 1282.08 - 324 = 958.08

與市場的協方差：
Cov(rP, rM) = βP × σM² = 0.90 × 400 = 360

也可以通過個別股票與市場的協方差計算：
Cov(rP, rM) = 0.6 × Cov(rA, rM) + 0.4 × Cov(rB, rM)
            = 0.6 × 280 + 0.4 × 480
            = 168 + 192
            = 360

### 問題14：投資組合Q分析

投資組合Q的投資比例：50%在P，30%在市場指數，20%在國庫券

**解答**：
標準差：
σQ = [0.5² × 1282.08 + 0.3² × 400 + 2 × 0.5 × 0.3 × 360]^(1/2)
   = [320.52 + 36 + 108]^(1/2)
   = [464.52]^(1/2)
   = 21.55%

貝塔：
βQ = 0.5 × 0.90 + 0.3 × 1 + 0.2 × 0 = 0.45 + 0.3 = 0.75

非系統性方差：
σ²(eQ) = σQ² - βQ²σM² = 464.52 - (0.75² × 400) = 464.52 - 225 = 239.52

與市場的協方差：
Cov(rQ, rM) = βQ × σM² = 0.75 × 400 = 300

## 問題15：貝塔估計與調整

**問題**：一支股票最近被估計其貝塔為1.24：
a. 這支股票的「調整貝塔」是多少？
b. 假設你估計了描述貝塔隨時間演變的以下回歸式：βt = 0.3 + 0.7βt-1，你對明年的貝塔預測是多少？

**解答**：

### a. 調整貝塔

Beta Books調整貝塔的方法是將樣本估計的貝塔與1.0取加權平均，權重分別為2/3和1/3：
調整貝塔 = [(2/3) × 1.24] + [(1/3) × 1.0] = 0.827 + 0.333 = 1.16

### b. 使用演變模型預測貝塔

使用當前貝塔估計βt-1 = 1.24，代入模型：
βt = 0.3 + (0.7 × 1.24) = 0.3 + 0.868 = 1.168

**這告訴我們什麼？** 調整貝塔方法反映了貝塔值隨時間「均值回歸」的趨勢。高貝塔股票會向下調整，低貝塔股票會向上調整，兩種調整方法得出的結果非常接近(1.16和1.168)，這顯示了這種均值回歸趨勢是業界公認的現象。

## 問題16：股票估值與選擇

**問題**：根據當前股息收益率和預期增長率，股票A和B的預期報酬率分別為11%和14%。股票A的貝塔為0.8，而股票B的貝塔為1.5。國庫券利率目前為6%，而標準普爾500指數的預期報酬率為12%。股票A的年標準差為10%，而股票B的年標準差為11%。如果你目前持有被動指數投資組合，你會選擇將這些股票中的任何一支添加到你的持股中嗎？

**解答**：
要決定是否添加這些股票，我們需要計算它們的阿爾法值。

對於股票A：
αA = rA - [rf + βA × (rM - rf)]
   = 11% - [6% + 0.8 × (12% - 6%)]
   = 11% - [6% + 0.8 × 6%]
   = 11% - [6% + 4.8%]
   = 11% - 10.8%
   = 0.2%

對於股票B：
αB = rB - [rf + βB × (rM - rf)]
   = 14% - [6% + 1.5 × (12% - 6%)]
   = 14% - [6% + 1.5 × 6%]
   = 14% - [6% + 9%]
   = 14% - 15%
   = -1%

股票A的阿爾法為正(0.2%)，表示相對於其風險水平，它提供了超額收益。因此，**股票A是對被動指數投資組合的良好補充**。

股票B的阿爾法為負(-1%)，表示它的報酬率低於其風險水平所應得的回報。因此，不應將其添加到投資組合中，甚至可能考慮在B股上建立空頭頭寸。

**這告訴我們什麼？** 在決定是否將股票添加到投資組合時，不僅要看絕對報酬率，還要考慮風險調整後的表現(阿爾法)。股票B的預期報酬率(14%)高於股票A(11%)，但考慮到其更高的風險水平，實際上它的表現較差。這展示了資本資產定價模型(CAPM)在投資決策中的應用。

---

這些問題和解答展示了如何使用指數模型來分析股票和投資組合的風險特性。單一指數模型大幅簡化了投資組合分析所需的計算和參數估計，同時提供了關於系統性風險和非系統性風險的有價值見解。通過了解這些概念，投資者可以構建更有效的投資組合，並做出更明智的投資決策。
