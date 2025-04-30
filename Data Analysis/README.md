# 📊 Sales Team Performance Analysis

This report analyzes sales team performance, agent efficiency, quarterly trends, product success, sector-wise insights, and sales cycle durations.

---

## 🧑‍🤝‍🧑 Sales Teams Overview

There are six distinct sales teams, each defined by the unique combination of **regional office** and **manager** from the `sales_teams` table.

### 🔹 1. Sales Volume & Won Opportunities

| Regional Office | Manager           | Won Opportunities | Revenue ($) |
|-----------------|-------------------|-------------------|-------------|
| Central         | Melvin Marxen     | 882               | 2,251,930   |
| West            | Summer Sewald     | 828               | 1,964,750   |
| East            | Rocco Neubert     | 691               | 1,960,545   |
| West            | Celia Rouche      | 610               | 1,603,897   |
| East            | Cara Losch        | 480               | 1,130,049   |
| Central         | Dustin Brinkmann  | 747               | 1,094,363   |

### 🔹 2. Success Rate by Sales Team

| Regional Office | Manager          | Success Rate (%) |
|-----------------|------------------|------------------|
| East            | Cara Losch       | 64.43            |
| West            | Summer Sewald    | 64.34            |
| West            | Celia Rouche     | 63.41            |
| Central         | Dustin Brinkmann | 62.98            |
| Central         | Melvin Marxen    | 62.20            |
| East            | Rocco Neubert    | 62.08            |

---

## 🚨 Underperforming Sales Agents

### 🔹 1. Agents with No Opportunities

| Regional Office | Manager         | Sales Agent        |
|-----------------|-----------------|--------------------|
| Central         | Melvin Marxen   | Mei-Mei Johns      |
| East            | Cara Losch      | Elizabeth Anderson |
| East            | Rocco Neubert   | Natalya Ivanova    |
| West            | Celia Rouche    | Carol Thompson     |
| West            | Summer Sewald   | Carl Lin           |

### 🔹 2. Worst Revenue Performance

| Sales Agent      | Revenue ($) | Rank |
|------------------|-------------|------|
| Violet Mclelland | 123,431     | 30   |
| Wilburn Farren   | 157,640     | 29   |
| Niesha Huffines  | 176,961     | 28   |

### 🔹 3. Worst Won Opportunities

| Sales Agent      | Won Opp | Rank |
|------------------|---------|------|
| Wilburn Farren   | 55      | 30   |
| Rosalina Dieter  | 72      | 29   |
| Garret Kinder    | 75      | 28   |

### 🔹 4. Per-Team Worst Performers

| Regional Office | Manager         | Sales Agent       | Revenue | Poor Revenue? | Won Opp | Poor Won Opp? |
|-----------------|-----------------|-------------------|---------|---------------|---------|----------------|
| Central         | Dustin Brinkmann| Versie Hillebrand | 187,693 | ✅ Yes        | 176     | ❌ No          |
| Central         | Dustin Brinkmann| Cecily Lampkin    | 229,800 | ❌ No         | 107     | ✅ Yes         |
| Central         | Melvin Marxen   | Niesha Huffines   | 176,961 | ✅ Yes        | 105     | ✅ Yes         |
| East            | Cara Losch      | Violet Mclelland  | 123,431 | ✅ Yes        | 122     | ❌ No          |
| East            | Cara Losch      | Wilburn Farren    | 157,640 | ❌ No         | 55      | ✅ Yes         |
| East            | Rocco Neubert   | Boris Faz         | 261,631 | ✅ Yes        | 101     | ✅ Yes         |
| West            | Celia Rouche    | Rosalina Dieter   | 235,403 | ✅ Yes        | 72      | ✅ Yes         |
| West            | Summer Sewald   | Kami Bicknell     | 316,456 | ✅ Yes        | 174     | ❌ No          |
| West            | Summer Sewald   | James Ascencio    | 413,533 | ❌ No         | 135     | ✅ Yes         |

---

## 🧮 Success Rate by Agent (Team: Dustin Brinkmann)

| Sales Agent       | Agent Success Rate (%) | Team Avg (%) | Performance        |
|-------------------|------------------------|--------------|--------------------|
| Anna Snelling     | 61.90                  | 62.98        | ⬇️ Below Average   |
| Cecily Lampkin    | 66.88                  | 62.98        | ⬆️ Above Average   |
| Lajuana Vencill   | 54.98                  | 62.98        | ⬇️ Below Average   |
| Moses Frase       | 66.15                  | 62.98        | ⬆️ Above Average   |
| Versie Hillebrand | 66.67                  | 62.98        | ⬆️ Above Average   |

---

## 📈 Quarterly Trends

### 🔹 1. Won Opportunities & Revenue

| Quarter | Won Opp | Growth (%) | Revenue ($) | Growth (%) |
|---------|---------|------------|-------------|------------|
| Q1      | 531     | –          | 1,134,672   | –          |
| Q2      | 1,254   | +136.16    | 3,086,111   | +171.98    |
| Q3      | 1,257   | +0.24      | 2,982,255   | -3.37      |
| Q4      | 1,196   | -4.85      | 2,802,496   | -6.03      |

### 🔹 2. Quarterly Success Rate

| Quarter | Success Rate (%) | QoQ Change (%) |
|---------|------------------|----------------|
| Q1      | 82.07            | –              |
| Q2      | 61.71            | -24.81         |
| Q3      | 61.41            | -0.49          |
| Q4      | 60.25            | -1.89          |

---

## 🛍️ Product Performance

### 🔹 1. Success Rate by Product

| Product         | Success Rate (%) |
|------------------|------------------|
| MG Special       | 64.84            |
| GTX Plus Pro     | 64.30            |
| GTX Basic        | 63.72            |
| GTX Pro          | 63.56            |
| GTX Plus Basic   | 62.13            |
| MG Advanced      | 60.33            |
| GTK 500          | 60.00            |

### 🔹 2. Revenue by Product

| Product         | Revenue ($) | Revenue Share (%) |
|------------------|-------------|-------------------|
| GTX Pro          | 3,510,578   | 35.09             |
| GTX Plus Pro     | 2,629,651   | 26.28             |
| MG Advanced      | 2,216,387   | 22.15             |
| GTX Plus Basic   | 705,275     | 7.05              |
| GTX Basic        | 499,263     | 4.99              |
| GTK 500          | 400,612     | 4.00              |
| MG Special       | 43,768      | 0.44              |

---

## 🏢 Sector Performance

### 🔹 1. Revenue & Success Rate by Sector

| Sector      | Revenue ($) | Success Rate (%) |
|-------------|-------------|------------------|
| Retail      | 1,867,528   | 63.06            |
| Technology  | 1,515,487   | 63.42            |
| Medical     | 1,359,595   | 62.32            |
| Marketing   | 922,321     | 64.85            |
| Entertainment| 689,007    | 64.68            |
| Software    | 1,077,934   | 63.92            |

### 🔹 2. Opportunity Distribution

| Sector      | Won | Lost | Engaging | Prospecting | Total | Win Rate (%) | Win/Loss Ratio |
|-------------|-----|------|----------|-------------|-------|---------------|----------------|
| Retail      | 799 | 468  | 94       | 36          | 1,397 | 57.19         | 1.71           |
| Technology  | 671 | 387  | 71       | 36          | 1,165 | 57.60         | 1.73           |
| Medical     | 592 | 358  | 77       | 24          | 1,051 | 56.33         | 1.65           |
| Software    | 450 | 254  | 43       | 10          | 757   | 59.45         | 1.77           |
| Marketing   | 404 | 219  | 40       | 11          | 674   | 59.94         | 1.84           |

---

## ⏳ Sales Cycle Duration

### 🔹 1. Average Duration by Deal Outcome

| Deal Stage | Avg Days | Max Days | Min Days |
|------------|----------|----------|----------|
| Won        | 52       | 138      | 1        |
| Lost       | 41       | 138      | 1        |

### 🔹 2. Duration by Product

| Product         | Avg Won Days | Avg Lost Days |
|------------------|--------------|----------------|
| GTK 500          | 64           | 38             |
| GTX Basic        | 55           | 41             |
| GTX Plus Basic   | 52           | 46             |
| GTX Plus Pro     | 52           | 36             |
| MG Advanced      | 52           | 40             |

### 🔹 3. Duration by Sector (Shortest Avg)

| Sector         | Avg Won Days | Avg Lost Days |
|----------------|---------------|----------------|
| Marketing      | 49            | 41             |
| Entertainment  | 51            | 47             |
| Medical        | 52            | 38             |
| Technology     | 52            | 39             |
| Services       | 52            | 39             |

---

> ✨ This analysis offers insights into improving sales strategy, enhancing individual performance, and optimizing product-market fit. For visualizations or source code, feel free to fork or open an issue!
