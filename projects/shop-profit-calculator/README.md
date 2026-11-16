# 🛒 QuickMart Shop Profit Calculator

A beginner Python project that turns one month of sales data from a small stationery shop into a clear profit report, and checks whether the shop reached its profit target.

---

## 🎯 Business Problem

> "Which products make us the most money, and did the shop reach its profit target this month?"

The shop's system exports sales numbers as **text**, so the data has to be converted to numbers before any calculation.

---

## 📊 Data

The data is **made up** for practice. It mimics a system export, where every value arrives as text.

| Product | Units sold | Selling price (₹) | Cost price (₹) |
|---|---:|---:|---:|
| Notebook | 120 | 45 | 30 |
| Pen pack | 200 | 20 | 12 |
| School bag | 35 | 650 | 480 |

- **Monthly expenses** (rent, wages, electricity): ₹6,000
- **Monthly net profit target:** ₹5,000

---

## 🧰 Skills Used

| Skill | Where it is used |
|---|---|
| Variables and comments | Storing raw data and explaining the reason for each step |
| Data types | `int` for units, `float` for prices and money |
| Type conversion | Turning the text export into numbers with `int()` and `float()` |
| Arithmetic operators | Revenue, cost, profit, margins, totals |
| Comparison and logical operators | Target checks using `>=`, `>` and `and` |
| `input()` | Adding a new product while the program runs |
| `print()` and f-strings | A neat, formatted report |
> **Scope:** This project uses only the Python topics I had learned at the time: variables, data types, type conversion, operators and input/output. It deliberately avoids `if/else`, loops and functions, which is why the calculations repeat for each product and the checks print `True` / `False` instead of messages. I plan to rebuild it with those tools later.
---

## ▶️ How to Run

1. Open `shop_profit_calculator.ipynb` in Jupyter Notebook or VS Code.
2. Choose **Restart & Run All**.
3. When asked, enter the details of a new product (for example: `Marker`, `50`, `15`, `9`).

---

## 📈 Key Results

| Product | Revenue (₹) | Profit (₹) | Margin | Profit per unit (₹) |
|---|---:|---:|---:|---:|
| Notebook | 5,400 | 1,800 | 33.3% | 15 |
| Pen pack | 4,000 | 1,600 | 40.0% | 8 |
| School bag | 22,750 | 5,950 | 26.2% | 170 |

| Overall | Value |
|---|---:|
| Total revenue | ₹32,150 |
| Total cost | ₹22,800 |
| Gross profit | ₹9,350 |
| Monthly expenses | ₹6,000 |
| **Net profit** | **₹3,350** |
| Gross margin | 29.1% |
| Net margin | 10.4% |

| Check | Result |
|---|:--:|
| Net profit at or above ₹5,000 target | ❌ False |
| School bag profit higher than notebook profit | ✅ True |
| Gross margin above 25% **and** target met | ❌ False |

**Insight:** The school bag earns the most profit (₹5,950, about 64% of gross profit), while the pen pack has the best margin (40%). The shop's gross margin is healthy at 29%, but fixed expenses of ₹6,000 leave a net profit of ₹3,350, which is ₹1,650 short of the ₹5,000 target.

**Interactive example:** a new product, Marker (50 units at ₹15, cost ₹9), gives ₹750 revenue, ₹300 profit and a 40% margin.

---

## 💡 What I Learned

- Data from a system often arrives as text, so converting it to the right type comes before any calculation.
- A clear variable name (for example `notebook_units_text` and `notebook_units`) makes it easy to tell raw data from clean data.
- Hard-coded numbers in labels can go out of date, so I used variables inside f-strings instead.
- `input()` keeps every character typed, including stray spaces. Cleaning text is something I will learn next in Strings.

---

## 🔜 Possible Improvements

- Add a second month and calculate revenue growth %.
- Use loops and functions to avoid repeating the same calculations for each product.
- Read the data from a CSV file instead of typing it into the notebook.

---

## 📁 Files

```
shop-profit-calculator/
├── README.md
└── shop_profit_calculator.ipynb
```

*Built with Python as part of my [Data Analytics Journey](../../README.md).*