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
- **COVID Impact**: Apparent 338,039 teacher reduction (5.2% drop) largely due to Illinois and Utah reporting gaps; actual workforce loss among consistently reporting states was ~6,000 teachers (0.2%) using validated NCES methodology
- **Recovery Pattern**: Steady workforce growth since 2021, approaching 
pre-pandemic levels
- **Current Status**: 6.57 million teachers nationally as of 2023-24
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

### Teacher-Student Ratio Analysis (2024)

**Elementary Education Shows Promise:**
- Analysis of states with highest teacher-student ratios (Alabama, California, Arizona, Illinois, etc.) reveals **7 out of 8 states improved** elementary ratios over 8 years
- Average improvement of **1.6 fewer students per teacher** in these challenging contexts
- Notable successes: Idaho (-5.8), Alabama (-2.4), California (-1.8), Illinois (-2.2)

**Secondary Education Challenges Persist:**
- Mixed results in secondary grades: equal numbers improving, stable, and worsening
- Average change near zero, suggesting persistent workforce challenges
- Arizona and Idaho showing increases in secondary ratios

**Key Methodological Discovery:**
- Teacher-student ratios ≠ actual class sizes (ratios include all instructional staff)
- National enrollment data reveals classification inconsistencies between states
- Some states require exclusion due to systematic reporting anomalies (Florida, Kansas,...)

### Methodology Validation

**Category Structure Investigation**: Comprehensive analysis of NCES teacher categories revealed that the general "Teachers" category represents the complete teacher workforce total, with specific categories (Elementary Teachers, Secondary Teachers, Kindergarten Teachers, Pre-kindergarten Teachers, Ungraded Teachers) serving as breakdowns of this total rather than additional categories. Mathematical analysis across all states and years confirms perfect 1:1 relationship (ratio = 1.00) between general "Teachers" count and sum of specific categories.

**Validated Approach**: Analysis uses NCES "Teachers" category as the definitive measure of total teacher workforce. This methodology prevents double-counting and aligns with NCES data structure where specific teacher categories are mutually exclusive breakdowns of the total.

**Data Quality Issues**: Illinois (265K teachers → 0 in 2020-21) and Utah (60K teachers → 0 in 2020-21) accounted for 96% of apparent national loss during COVID period.

## What You'll Find Here

- Current analysis includes:
- National workforce trend analysis with COVID period highlighted
- State-by-state comparison of teacher count changes
- **Teacher-student ratio analysis across grade levels (2016-2024)**
- **Focus on states with highest ratios to test improvement universality**
- Professional visualizations for LinkedIn and presentations
- Investigation of unusual data patterns and reporting inconsistencies
- Systematic validation of NCES teacher category structure

## About the Data

- **Source**: NCES Common Core of Data, Staff Files
- **Years Covered**: Academic years 2016-17 through 2023-24
- **Geographic Scope**: All 50 states, DC, territories, and federal 
education systems
- **Scale**: 11,407 observations across 27 staff categories
- **Teacher Categories**: Analysis uses NCES "Teachers" category as total workforce measure, with breakdowns available by Elementary Teachers, Secondary Teachers, Kindergarten Teachers, Pre-kindergarten Teachers, and Ungraded Teachers
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
validation, category structure investigation
- **Approach**: Multi-year consolidation, missing value analysis, outlier 
investigation, methodological validation
- **Data Integration**: Combined teacher workforce and enrollment data for ratio calculations
- **Quality Control**: Applied systematic filters for data reporting inconsistencies

## How It's Organized

```
k12-teacher-trends-analysis/
├── data/                          # NCES source data files (2016-2024)
│   ├── staff/                     # Teacher workforce data
│   └── enrollment/                # Student enrollment data
├── outputs/                       # Generated visualizations and charts
├── 01_teacher_data_exploration.ipynb  # Primary workforce analysis
├── 02_state_level_deep_dive.ipynb    # Category structure investigation  
├── 03_teacher_student_ratios.ipynb   # Ratio analysis and grade-level trends
└── README.md                      # Project documentation
```

## Research Approach

The analysis follows a systematic approach:
1. **Data Consolidation**: Combined eight years of NCES staff data with 
consistent formatting
2. **Quality Assessment**: Evaluated missing values and reporting patterns
3. **Methodology Validation**: Investigated NCES category structure to ensure accurate workforce measurement
4. **Trend Analysis**: Calculated year-over-year changes and identified 
patterns
5. **Comparative Analysis**: Examined state-level workforce changes and 
variations
6. **Impact Assessment**: Focused analysis on COVID-19 pandemic effects

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

I'm Meredith Bouvier, a quantitative researcher with 13+ years of experience analyzing complex social systems through education research and policy. My background spans international organizations (World Bank, Global Partnership for Education, OECD) and direct field experience as a certified high school teacher in New York City.

I hold a PhD in Adult Education, MA in Mathematics, and BA in Mathematics, with expertise in statistical analysis, survey methodology, and large-scale administrative data. My work focuses on using quantitative methods to understand social patterns, policy impacts, and behavioral trends across diverse populations.

**Research Interests**: Social science analytics, survey research methodology, big data applications in understanding human behavior, and translating complex statistical findings into actionable insights for organizations and policymakers.

**Technical Skills**: Python (pandas, statistical analysis), survey design, longitudinal data analysis, data visualization, and working with large administrative datasets.

I'm particularly interested in roles where I can apply quantitative social science methods to understand user behavior, social trends, and policy outcomes - whether in tech, government, or research institutions.

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

---

*Last updated: September 14, 2025*  
*This analysis is ongoing - check back for updates and new findings*
