# 投資學概念解析：有效多元化投資組合

我將為你解說這些投資組合理論的問題，並以初學者能理解的方式說明。這些問題主要關於現代投資組合理論中的資產配置、風險與報酬的權衡，以及如何建構最佳投資組合。

## 第4-10題的基本資料
有三種共同基金：
- 股票基金(S)：預期報酬率20%，標準差30%
- 債券基金(B)：預期報酬率12%，標準差15%
- 貨幣市場基金：提供安全的8%報酬率
- 股票與債券基金之間的相關係數為0.10

## 問題4：最小變異數投資組合
**問題**：兩種風險性資產的最小變異數投資組合中，投資比例各為多少？其預期報酬率和標準差各為多少？

**解釋**：
最小變異數投資組合是指在所有可能的投資組合中，風險(標準差)最低的那個組合。

根據解答，要計算最小變異數投資組合，我們需要：
1. 首先計算協方差矩陣 (依據標準差與相關係數)
2. 使用公式計算股票基金的權重：wMin(S) = (σB² - Cov(rS, rB)) / (σS² + σB² - 2Cov(rS, rB))

代入數值：
- wMin(S) = (225 - 45) / (900 + 225 - (2 × 45)) = 0.1739 (17.39%)
- wMin(B) = 1 - 0.1739 = 0.8261 (82.61%)

這表示最小變異數投資組合應將17.39%資金投入股票基金，82.61%投入債券基金。

此投資組合的：
- 預期報酬率 = (0.1739 × 20%) + (0.8261 × 12%) = 13.39%
- 標準差 = 13.92%

## 問題5：投資機會集合
**問題**：製表並繪製兩種風險性資產的投資機會集合。使用股票基金的投資比例從0%到100%，每次增加20%。

**解釋**：
投資機會集合是所有可能投資組合的風險和報酬的組合。當我們改變股票與債券的投資比例時，會得到不同的預期報酬率和風險水平。

解答提供了表格，顯示了不同比例下的預期報酬率和標準差：
- 只投資債券 (0% 股票，100% 債券)：報酬率12%，標準差15%
- 最小變異數組合 (17.39% 股票，82.61% 債券)：報酬率13.39%，標準差13.92%
- 20% 股票，80% 債券：報酬率13.60%，標準差13.94%
...以此類推到
- 只投資股票 (100% 股票，0% 債券)：報酬率20%，標準差30%
<img width="719" alt="截圖 2025-04-16 下午2 59 49" src="https://github.com/user-attachments/assets/88d56141-7a94-477e-ac6a-af4209b6d242" />

這個表格和圖形展示了有效前緣(efficient frontier)，這是所有最佳風險報酬組合的曲線。

## 問題6：從無風險利率到機會集合的切線
**問題**：繪製從無風險利率到機會集合的切線。你的圖表對最佳投資組合的預期報酬率和標準差顯示什麼？

**解釋**：
當我們將無風險資產(貨幣市場基金)納入考量時，我們可以繪製資本配置線(CAL)，它是從無風險利率延伸到切點的直線，切點就是最佳風險投資組合。

從圖表可見，最佳投資組合是切點投資組合(tangency portfolio)，其：
- 預期報酬率約為15.6%
- 標準差約為16.5%

## 問題7：最佳風險投資組合的數值解
**問題**：計算最佳風險投資組合中各資產的比例，以及其預期報酬率和標準差。

**解釋**：
最佳風險投資組合(也稱為切點投資組合)是風險資產中能提供最佳風險報酬比的組合。

計算公式：

$$
w_S = \frac{[E(r_S) - r_f] \cdot \sigma_B^2 - [E(r_B) - r_f] \cdot \text{Cov}(r_S, r_B)}{
[E(r_S) - r_f] \cdot \sigma_B^2 + [E(r_B) - r_f] \cdot \sigma_S^2 - 
[E(r_S) - r_f + E(r_B) - r_f] \cdot \text{Cov}(r_S, r_B)}
$$

代入數值後：
- 股票基金比例 wS = 0.4516 (45.16%)

$$
w_S = \frac{(0.20 - 0.08) \cdot 225 - (0.12 - 0.08) \cdot 45}{
(0.20 - 0.08) \cdot 225 + (0.12 - 0.08) \cdot 900 - (0.20 - 0.08 + 0.12 - 0.08) \cdot 45}
= 0.4516
$$

- 債券基金比例 wB = 0.5484 (54.84%)

此投資組合的：
- 預期報酬率 = 15.61%
- 標準差 = 16.54%

## 問題8：最佳可行資本配置線的夏普比率
**問題**：最佳可行資本配置線的夏普比率是多少？

**解釋**：
夏普比率衡量投資組合的超額報酬與風險的比值，公式為：(E(rp) - rf) / σp

代入最佳投資組合的數值：
夏普比率 = (15.61% - 8%) / 16.54% = 0.4601

這個數值衡量了每承擔一單位風險所能獲得的超額報酬。

## 問題9：要求14%預期報酬的有效投資組合
**問題**：
a. 如果要求投資組合產生14%的預期報酬率，並且是有效的(在最陡峭的可行資本配置線上)，其標準差是多少？
b. 在貨幣市場基金和兩種風險性基金中的投資比例各是多少？

**解釋**：
a. 使用資本配置線的方程式：E(rc) = rf + [(E(rp) - rf)/σp] × σc
其中E(rc)=14%，可以計算出標準差σc = 13.04%

b. 設y為投資在最佳風險投資組合的比例，則：
14% = 8% + y × (15.61% - 8%)
解出y = 0.7884

所以，投資比例為：
- 貨幣市場基金：(1-y) = 0.2119 (21.19%)
- 股票基金：y × 0.4516 = 0.3560 (35.60%)
- 債券基金：y × 0.5484 = 0.4323 (43.23%)

## 問題10：僅使用兩種風險性基金
**問題**：如果你只使用兩種風險性基金，且要求14%的預期報酬率，投資比例會是多少？將其標準差與問題9的最佳化投資組合比較，你有何結論？

**解釋**：
要達到14%的報酬率，只用股票和債券基金的話：
14% = 20% × ws + 12% × (1-ws)
解出ws = 0.25

投資比例為：
- 股票基金：25%
- 債券基金：75%

此投資組合的標準差為14.13%，比問題9的13.04%高出許多。

結論：透過加入無風險資產(貨幣市場基金)並使用最佳風險投資組合，我們可以用更低的風險達到相同的預期報酬率。這體現了資本市場理論的核心優勢。

## 問題11：黃金與股票的投資決策
**問題**：
股票提供18%的預期報酬率和22%的標準差。黃金提供10%的預期報酬率和30%的標準差。
a. 考慮到黃金在平均報酬率和波動性方面的劣勢，有人會持有黃金嗎？若會，用圖形說明為什麼。
b. 假設黃金和股票的相關係數為1，重新回答(a)。
c. (b)部分的假設能代表證券市場的均衡嗎？

**解釋**：

a. 即使黃金似乎劣於股票，如果黃金與股票的相關性夠低(甚至是負的)，黃金仍然可以成為投資組合的有價值部分。這是因為多元化可以降低整體投資組合的風險。

<img width="365" alt="截圖 2025-04-16 下午3 05 53" src="https://github.com/user-attachments/assets/9c353689-0fca-466b-b428-64833e7e5453" />

b. 如果相關係數為1(完全正相關)，則黃金不會為投資組合帶來多元化效益。在這種情況下，沒有人會持有黃金，因為股票在相同的風險水平下提供更高的報酬。

<img width="354" alt="截圖 2025-04-16 下午3 06 04" src="https://github.com/user-attachments/assets/aa01549c-2e81-4aa5-8695-02bdb2ad9a7f" />

c. 這種情況不可能代表市場均衡。如果沒有人願意持有黃金，其價格會下跌，預期報酬率會上升，直到黃金變得足夠有吸引力為止。

## 問題12：完全負相關資產的無風險投資組合
**問題**：
假設市場上有許多股票，A股和B股的特性如下：
- A股：預期報酬率10%，標準差5%
- B股：預期報酬率15%，標準差10%
相關係數為-1
假設可以以無風險利率rf借款，無風險利率必須是多少？

**解釋**：
當兩種資產完全負相關時，可以構建一個無風險投資組合。設投資A股的比例為wA，B股為(1-wA)，要使標準差為零：

σP = |wA × σA - wB × σB| = 0
5% × wA - 10% × (1-wA) = 0
解出wA = 0.6667

此無風險投資組合的預期報酬率：
E(r) = 0.6667 × 10% + 0.3333 × 15% = 11.667%

在均衡狀態下，無風險投資組合的報酬應等於無風險利率，因此rf = 11.667%

## 問題13：所有投資者的最佳風險投資組合是否相同
**問題**：是非題：假設所有證券(包括無風險借貸利率)的預期報酬率和標準差都已知。在這種情況下，所有投資者都會有相同的最佳風險投資組合。

**解釋**：
答案：不正確。

如果借款和貸款利率不同，那麼根據投資者的風險偏好(即其無差異曲線的形狀)，借款者和貸款者可能會有不同的最佳風險投資組合。

## 問題14：投資組合標準差與資產標準差的關係
**問題**：是非題：投資組合的標準差總是等於投資組合內資產標準差的加權平均。

**解釋**：
答案：不正確。

投資組合的標準差只有在所有資產完全正相關(相關係數為1)的特殊情況下，才等於資產標準差的加權平均。在所有其他情況下，由於多元化效益，投資組合的標準差小於資產標準差的加權平均。

投資組合的方差是協方差矩陣元素的加權和，權重是投資組合比例的乘積。

---

通過這些問題，你可以理解現代投資組合理論的核心概念，如風險分散、有效前緣、最佳投資組合的構建，以及資產相關性對投資決策的影響。這些概念對於構建有效的投資策略至關重要。
