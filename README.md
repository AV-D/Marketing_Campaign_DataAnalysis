# Marketing_Campaign_DataAnalysis

Comprehensive analysis of multi-channel marketing campaign performance with advanced KPI calculations and strategic insights.

## 📌 Overview
This project analyzes February 2021 marketing data from:
- Social Media (Facebook)
- Search Engine (Google)
- YouTube Influencer campaigns

Key features:
✅ ROAS & ROI calculations  
✅ Conversion funnel analysis  
✅ Cost efficiency metrics (CPC/CPL/CPO)  
✅ Platform comparison visualizations  
✅ Holiday impact assessment

## 🚀 Features
```
# Sample code from analysis notebook
df['roas'] = df.revenue / df.mark_spent
df['cpl'] = df.mark_spent / df.leads
```
- **Data Processing**  
  - Date feature engineering
  - Holiday detection
  - Data validation checks

- **Key Metrics**  
  | Metric | Formula |
  |--------|---------|
  | ROAS | `revenue / mark_spent` |
  | CTR | `(clicks/impressions)*100` |
  | CPO | `mark_spent / orders` |

## 📥 Installation
1. Clone repo:
   ```
   git clone https://github.com/yourusername/marketing-campaign-analysis.git
   ```
2. Install requirements:
   ```
   pip install pandas numpy matplotlib seaborn holidays
   ```
3. Add your marketing data to `/data` directory

## 📊 Dataset
**Columns Analyzed** ([sample data](Marketing.csv)):

| Column | Description | Example Value |
|--------|-------------|---------------|
| `campaign_name` | Campaign identifier | "facebook_tier2" |
| `mark_spent` | Advertising budget | $16,300.20 |
| `revenue` | Generated income | $14,962.00 |
| `ctr` | Click-through rate | 0.74% |

## 💡 Usage
Run Jupyter notebook:
```
jupyter notebook marketing_analysis.ipynb
```

**Analysis Workflow**:
1. Import data
2. Calculate KPIs:
   ```
   df['conversion_rate'] = (df.leads/df.clicks)*100
   ```
3. Generate visualizations:
   ```
   sns.barplot(x='platform', y='roas', data=df)
   ```

## 📈 Results
**Key Findings**:
- YouTube influencer campaigns achieved **2.82x ROAS**  
- Social media Tier2 campaigns showed **3:1 spend-to-revenue ratio**  
- Search "hot" keywords delivered **1.53x ROAS**

![Metrics Comparison](https://via.placeholder.com/600x400?text=Platform+Performance+Comparison)

## 🤝 Contributing
1. Fork the project
2. Create your feature branch:
   ```
   git checkout -b feature/amazing-feature
   ```
3. Commit changes:
   ```
   git commit -m 'Add some amazing feature'
   ```
4. Push to branch:
   ```
   git push origin feature/amazing-feature
   ```
5. Open a Pull Request

## 📄 License
Distributed under MIT License. See `LICENSE` for more information.
