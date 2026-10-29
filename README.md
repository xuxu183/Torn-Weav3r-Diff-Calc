# Torn 市场 - Weav3r 差额计算器
Torn Market - Weav3r Difference Calculator

### 1. 脚本简介｜Overview

本脚本用于比较 Torn 官方物品市场（Item Market）与 Weav3r 市场的商品价格，计算扣除官方市场交易税后的单件差额、差额比例及预估总差额，帮助玩家寻找潜在的低买高卖机会。

This script compares item prices between Torn's Item Market and Weav3r. It calculates the per-item difference after accounting for the Item Market tax, the difference percentage, and the estimated total difference to help identify potential buy-low, sell-high opportunities.

### 2. 计算公式｜Calculation Formulas

**官方市场税后价格｜Item Market Price After Tax**

官方市场税率为 5%。

Item Market tax rate: 5%.

公式 / Formula:

`税后价格 = 官方市场价格 × 0.95`

`After-tax Price = Item Market Price × 0.95`

**单件差额｜Per-Item Difference**

公式 / Formula:

`单件差额 = 官方市场税后价格 − Weav3r 市场价格`

`Per-Item Difference = Item Market After-tax Price − Weav3r Price`

**差额比例｜Difference Percentage**

公式 / Formula:

`差额比例 = 单件差额 ÷ 官方市场税后价格 × 100%`

`Difference Percentage = Per-Item Difference ÷ Item Market After-tax Price × 100%`

**预估总差额｜Estimated Total Difference**

公式 / Formula:

`预估总差额 = 单件差额 × Weav3r 商品数量`

`Estimated Total Difference = Per-Item Difference × Weav3r Listing Quantity`

**计算示例｜Example**

假设官方市场价格为 $100,000，Weav3r 市场价格为 $90,000，Weav3r 商品数量为 10。

Suppose the Item Market price is $100,000, the Weav3r price is $90,000, and the Weav3r listing quantity is 10.

- 官方市场税后价格：$100,000 × 0.95 = $95,000  
  Item Market after-tax price: $100,000 × 0.95 = $95,000
- 单件差额：$95,000 − $90,000 = $5,000  
  Per-item difference: $95,000 − $90,000 = $5,000
- 差额比例：$5,000 ÷ $95,000 × 100% ≈ 5.26%  
  Difference percentage: $5,000 ÷ $95,000 × 100% ≈ 5.26%
- 预估总差额：$5,000 × 10 = $50,000  
  Estimated total difference: $5,000 × 10 = $50,000

**注意：预估总差额是基于当前显示价格和商品数量的计算结果，不代表实际利润。** 计算未考虑其他交易成本、价格变化或商品未能按预期售出的情况。

Note: The estimated total difference is based on the displayed prices and listing quantity. It does not represent guaranteed profit and does not account for other transaction costs, price fluctuations, or the possibility that items may not sell as expected.

### 3. 数据范围｜Data Scope

脚本比较官方物品市场的前 5 个卖家与 Weav3r 市场的前 5 个商品列表，帮助玩家快速查看两边的价格差异。

The script compares the first five sellers on Torn's Item Market with the first five listings on Weav3r, allowing users to quickly review price differences between the two markets.

### 4. 使用场景｜Use Cases

**寻找潜在套利机会｜Identifying Potential Arbitrage Opportunities**

通过比较官方市场税后价格与 Weav3r 价格，筛选可能存在正差额的商品，辅助判断是否值得买入并转售。

Compare the Item Market after-tax price with the Weav3r price to identify items with a positive difference and assess potential buy-and-resell opportunities.

**评估商品数量的影响｜Evaluating Listing Quantity**

通过预估总差额，快速了解按照当前价格和 Weav3r 商品数量计算出的理论差额总额。

Use the estimated total difference to assess the theoretical combined difference based on the current prices and Weav3r listing quantity.

**快速筛选商品｜Quick Item Screening**

利用差额、差额比例和排序功能，优先查看价格差异较大的商品，减少手动计算的工作量。

Use the difference, difference percentage, and sorting functions to prioritize items with larger price gaps and reduce manual calculations.

### 6. 术语统一｜Terminology

| 中文术语 | English Term |
|---|---|
| 官方物品市场 | Item Market |
| Weav3r 市场 | Weav3r Market |
| 官方市场价格 | Item Market Price |
| 官方市场税后价格 | Item Market After-tax Price |
| Weav3r 市场价格 | Weav3r Price |
| 单件差额 | Per-Item Difference |
| 差额比例 | Difference Percentage |
| Weav3r 商品数量 | Weav3r Listing Quantity |
| 预估总差额 | Estimated Total Difference |
| 交易税 | Market Tax |
| 潜在套利机会 | Potential Arbitrage Opportunity |

**重要说明｜Important Note**

正差额表示官方市场税后价格高于 Weav3r 价格；负差额表示官方市场税后价格低于 Weav3r 价格。正差额仅代表价格差异，不等同于已实现利润。

A positive difference means the Item Market after-tax price is higher than the Weav3r price. A negative difference means the Item Market after-tax price is lower than the Weav3r price. A positive difference indicates a price gap, not realized profit.
