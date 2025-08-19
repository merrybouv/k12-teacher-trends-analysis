# K-12 Teacher Workforce Trends Analysis

Exploring teacher staffing patterns across US states using eight years of 
federal education data (2016-2024)

---

## What This Project Is About

This repository contains an ongoing analysis of K-12 teacher workforce 
trends using National Center for Education Statistics (NCES) data. I'm 
exploring national patterns, state-level variations, and the impact of 
COVID-19 on teacher workforce size across 58 US jurisdictions.

## Key Findings So Far

### National Picture
- **COVID Impact**: Apparent 338,039 teacher reduction (5.2% drop) largely due to Illinois and Utah reporting gaps; actual workforce loss among consistently reporting states was ~12,000 teachers (0.2%) using comprehensive teacher category analysis
- **Recovery Pattern**: Steady workforce growth since 2021, approaching 
pre-pandemic levels
- **Current Status**: 6.57 million teachers nationally as of 2023-24 (comprehensive category analysis)
- **Data Quality**: Analysis revealed significant reporting inconsistencies that can lead to misleading interpretations of teacher workforce trends

### State Stories
**States facing the biggest challenges (2016-17 to 2023-24):**
- U.S. Virgin Islands: lost 246 teachers (21.3% decline)
- Florida: lost 30,539 teachers (16.4% decline)
- Puerto Rico: lost 4,308 teachers (14.9% decline)
- Alaska: lost 604 teachers (7.7% decline)

**States with growing teacher workforces (2016-17 to 2023-24):**
- District of Columbia: gained 1,608 teachers (23.9% growth)
- South Carolina: gained 6,453 teachers (12.7% growth)
- Indiana: gained 7,212 teachers (12.0% growth)
- Idaho: gained 1,761 teachers (10.9% growth)

### Interesting Data Patterns
- Bureau of Indian Education reporting shows evolving federal data 
collection methods that raise questions about how Native American 
education data is tracked
- Methodological Discovery: Initial analysis appeared to show massive COVID impact, but deeper investigation revealed the importance of distinguishing between actual workforce changes and data reporting inconsistencies.
- Missing values represent 7.4% of records, indicating generally strong 
state reporting compliance, though patterns of which states and staff 
categories have missing data could warrant further investigation
- State-level variations suggest multiple factors at play, warranting 
further investigation

### Methodology Refinement

**Analysis Evolution**: Initial analysis used single "Teachers" category (~6K loss), refined approach combines all teacher categories (Elementary, Secondary, Kindergarten, Pre-K, Ungraded) for comprehensive workforce analysis (~12K loss). Both methods confirm the core finding: apparent teacher shortage was primarily a data reporting artifact.

**Data Quality Issues**: Illinois (265K teachers → 0 in 2020-21) and Utah (60K teachers → 0 in 2020-21) accounted for 96% of apparent national loss during COVID period.

## What You'll Find Here

Current analysis includes:
- National workforce trend analysis with COVID period highlighted
- State-by-state comparison of teacher count changes
- Professional visualizations for LinkedIn and presentations
- Investigation of unusual data patterns and reporting inconsistencies

## About the Data

- **Source**: NCES Common Core of Data, Staff Files
- **Years Covered**: Academic years 2016-17 through 2023-24
- **Geographic Scope**: All 50 states, DC, territories, and federal 
education systems
- **Scale**: 11,407 observations across 27 staff categories
- **Teacher Categories**: Analysis includes general "Teachers" category as 
well as Elementary Teachers, Secondary Teachers, Kindergarten Teachers, 
Pre-kindergarten Teachers, and Ungraded Teachers
- **Jurisdictions**: 58 different education systems
- **Data Selection Note**: Originally planned to analyze 10 years of data 
(2014-2024), but early datasets used significantly different reporting 
structures. Current analysis focuses on the 8 years with consistent data 
formatting, though earlier years may be incorporated in future work as 
methodology develops.

## Technical Details

- **Language**: Python
- **Main Tools**: pandas, matplotlib, seaborn, numpy
- **Environment**: Jupyter Notebook
- **Methods**: Time-series analysis, comparative statistics, data 
validation
- **Approach**: Multi-year consolidation, missing value analysis, outlier 
investigation

## How It's Organized

```
k12-teacher-trends-analysis/
├── data/                          # NCES source data files (2016-2024)
├── outputs/                       # Generated visualizations and charts
├── notebooks/                     # Jupyter analysis notebooks
├── 01_teacher_data_exploration.ipynb  # Primary analysis notebook
└── README.md                      # Project documentation
```

## Research Approach

The analysis follows a systematic approach:
1. **Data Consolidation**: Combined eight years of NCES staff data with 
consistent formatting
2. **Quality Assessment**: Evaluated missing values and reporting patterns
3. **Trend Analysis**: Calculated year-over-year changes and identified 
patterns
4. **Comparative Analysis**: Examined state-level workforce changes and 
variations
5. **Impact Assessment**: Focused analysis on COVID-19 pandemic effects

## What's Coming Next

This is an active project with several areas I'm excited to explore:

### Planned Deep Dives
- **Teacher Categories**: Breaking down by elementary, secondary, and 
specialized roles
- **State Spotlights**: Focused analysis of states with interesting 
patterns
- **Demographics**: Bringing in population and economic data for context
- **Salary Analysis**: Comparing teacher workforce changes with state salary levels and salary progression patterns to identify potential correlations
- **Policy Connections**: Looking at how state education policies relate 
to teacher workforce trends

### Questions I'm Curious About
- How do teacher shortage patterns vary by grade level and subject area?
- What demographic and economic factors might explain the state 
differences?
- Which states are successfully growing their teacher workforce?

## Why This Matters

These findings could inform:
- Teacher workforce planning strategies
- Better coordination between federal and state education systems
- Resource allocation for teacher recruitment and workforce growth

## About Me

I'm Meredith Bouvier, and I bring 13+ years of experience in K-12 
education research and policy. My background includes work with 
international organizations (World Bank, Global Partnership for Education, 
OECD) and direct classroom experience as a certified high school teacher 
in New York City. I hold a PhD in Adult Education, MA in Mathematics, and 
BS in Mathematics.

I'm particularly interested in education workforce analytics, 
international education policy, and using data to support better 
decision-making in education.

## Connect

- GitHub: [github.com/merrybouv](https://github.com/merrybouv)
- LinkedIn: 
[linkedin.com/in/meredithbouvier](https://www.linkedin.com/in/meredithbouvier/)
- Email: merrybouv@gmail.com

---

## Using This Work

If this analysis is helpful for your research, please cite it as:
```
Bouvier, M. (2024). K-12 Teacher Workforce Trends Analysis: Eight-Year 
Study of US Teacher Staffing Patterns (2016-2024). GitHub Repository.
```

## License

This project is licensed under the MIT License.

---

*Last updated: August 19, 2025*  
*This analysis is ongoing - check back for updates and new findings*
