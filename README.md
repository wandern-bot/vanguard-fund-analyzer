# vanguard-fund-analyzer
This project scrapes, processes, and visualizes Vanguard mutual fund and ETF data to identify cost-efficient funds that deliver strong long-term performance.

## 🔍 Project Goals

- Collect fund-level data from Vanguard’s official website using Python
- Compare fund performance across timeframes (YTD, 5Y, 10Y, Since Inception)
- Enable interactive filtering by fund type, risk level, and return period
- Highlight correlation between **low expense ratios** and **top-quartile returns**

---

## 🚀 Features

- ✅ Web scraping from Vanguard’s ETF & Mutual Fund listings  
- ✅ Structured data export (`.csv`) for easy dashboard use  
- ✅ Clean separation of fund types and investment metrics  
- ✅ Tableau Public dashboard for interactive exploration  
- ✅ Modern workflow using Google Colab + GitHub

## 📁 Files in This Repo

| File                             | Description                                      |
|----------------------------------|--------------------------------------------------|
| `vanguard_fund_scraper.ipynb`    | Google Colab notebook with scraping logic        |
| `vanguard_etfs.csv`              | Cleaned ETF data (automatically generated)       |
| `vanguard_mutual_funds.csv`      | Cleaned ETF data (automatically generated)       |
| `README.md`                      | Project overview and documentation               |
| `LICENSE`                        | MIT License for reuse and sharing                |

### 📓 Notebook

The data scraper (`vanguard_fund_scraper.ipynb`) collects the following from Vanguard's public site:
- Fund names, Symbol, Categories
- Annualized returns across multiple periods
- Expense ratios
- Risk scores

The data is output as a `.csv` file for use in Tableau or other analysis tools.

➡️ [View Notebook on GitHub](./vanguard_fund_scraper.ipynb)

### 📊 Tableau Dashboar

Interactive dashboard analyzing “best bang for buck” across fund types.
🔗 **[View the interactive dashboard on Tableau Public →](https://public.tableau.com/app/profile/nian.liu6717/viz/Vanguard_Funds_Best_Bang_Buck_Interactive_Analysis/VanguardUniverse)**  
> Filter by fund type, risk level, or time horizon to find funds that match your investment goals.
![image](https://github.com/user-attachments/assets/07bebc89-aac8-4de8-b6fb-bd4ea4348517)

Key Insight:
> "Across time horizons, a growing share of top-quartile Vanguard funds had expense ratios ≤ 0.1% — 59% YTD, 68% over 5 years, and 75% over 10 years. Cost efficiency increasingly correlates with sustained outperformance."

---

## 💻 How to Run Locally

1. Clone this repository
2. Install dependencies:
   ```bash
   pip install requests beautifulsoup4 pandas
