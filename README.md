# K-12 Teacher Workforce Trends Analysis

**Status: Analysis complete and paused (October 2025)**  
*This project analyzed 8 years of teacher workforce and student-teacher ratio data. Currently focusing on international adult education research with UNESCO's GRALE datasets.*

---

## What This Project Is About

Analysis of K-12 teacher workforce trends using National Center for Education Statistics (NCES) data, exploring national patterns, state-level variations, and COVID-19 impacts across 58 US jurisdictions (2016-2024).

## Key Findings

### National Workforce Trends
- **COVID Impact**: Apparent 338,039 teacher reduction (5.2% drop) was largely due to Illinois and Utah reporting gaps; actual workforce loss among consistently reporting states was ~6,000 teachers (0.2%)
- **Recovery Pattern**: Steady workforce growth since 2021, approaching pre-pandemic levels
- **Current Status**: 6.57 million teachers nationally as of 2023-24
- **Data Quality Discovery**: Analysis revealed significant reporting inconsistencies that can lead to misleading interpretations of workforce trends

### State-Level Changes (2016-17 to 2023-24)

**Largest Declines:**
- U.S. Virgin Islands: -246 teachers (21.3% decline)
- Florida: -30,539 teachers (16.4% decline)
- Puerto Rico: -4,308 teachers (14.9% decline)
- Alaska: -604 teachers (7.7% decline)

**Largest Growth:**
- District of Columbia: +1,608 teachers (23.9% growth)
- South Carolina: +6,453 teachers (12.7% growth)
- Indiana: +7,212 teachers (12.0% growth)
- Idaho: +1,761 teachers (10.9% growth)

### Teacher-Student Ratio Analysis

**Elementary Education Shows Improvement:**
- 7 out of 8 states with highest ratios improved over 8 years
- Average improvement: 1.6 fewer students per teacher
- Notable successes: Idaho (-5.8), Alabama (-2.4), California (-1.8), Illinois (-2.2)

**Secondary Education Mixed Results:**
- No clear pattern: equal numbers improving, stable, and worsening
- Suggests persistent workforce challenges in secondary grades

**Methodological Discovery:**
- Teacher-student ratios ≠ actual class sizes (ratios include all instructional staff, not just classroom teachers)
- California showed 22:1 in calculations but 23-27 students per actual classroom
- Some states had systematic reporting problems requiring exclusion (Florida, Kansas)

### Methodology Validation

**Category Structure:** NCES "Teachers" category represents complete teacher workforce total, with specific categories (Elementary, Secondary, Kindergarten, Pre-kindergarten, Ungraded) serving as mutually exclusive breakdowns rather than additional categories.

**Data Quality Issues:** Illinois (265K teachers → 0 in 2020-21) and Utah (60K teachers → 0 in 2020-21) accounted for 96% of apparent national loss during COVID period.

## What's Included

- National workforce trend analysis with COVID period focus
- State-by-state comparison of teacher count changes
- Teacher-student ratio analysis across grade levels (2016-2024)
- Analysis of states with highest ratios to test if improvements were universal
- Investigation of data reporting inconsistencies
- Systematic validation of NCES teacher category structure

## Data Sources

- **Source**: NCES Common Core of Data (Staff Files and Enrollment Files)
- **Years Covered**: Academic years 2016-17 through 2023-24
- **Geographic Scope**: All 50 states, DC, territories, and federal education systems
- **Scale**: 11,407 observations across 27 staff categories, 58 jurisdictions
- **Data Selection**: Focused on 8 years with consistent reporting structures

## Technical Details

- **Language**: Python
- **Tools**: pandas, matplotlib, seaborn, numpy
- **Environment**: Jupyter Notebook
- **Methods**: Time-series analysis, comparative statistics, data validation, longitudinal analysis
- **Data Integration**: Combined teacher workforce and enrollment data for ratio calculations
- **Quality Control**: Systematic filters for data reporting inconsistencies

## Project Structure

```
k12-teacher-trends-analysis/
├── data/
│   ├── staff/                     # Teacher workforce data (2016-2024)
│   └── enrollment/                # Student enrollment data (2016-2024)
├── outputs/                       # Visualizations and charts
├── 01_teacher_data_exploration.ipynb  # Primary workforce analysis
├── 02_state_level_deep_dive.ipynb     # Category structure investigation  
├── 03_teacher_student_ratios.ipynb    # Ratio analysis and trends
└── README.md
```

## Research Approach

1. **Data Consolidation**: Combined eight years of NCES data with consistent formatting
2. **Quality Assessment**: Evaluated missing values and reporting patterns
3. **Methodology Validation**: Investigated NCES category structure for accurate measurement
4. **Trend Analysis**: Calculated year-over-year changes and identified patterns
5. **Comparative Analysis**: Examined state-level workforce changes
6. **Impact Assessment**: Focused on COVID-19 pandemic effects

## Why This Matters

These findings inform:
- Teacher workforce planning strategies
- Better coordination between federal and state education systems
- Resource allocation for teacher recruitment and retention
- Understanding the difference between administrative ratios and actual classroom conditions

## About Me

I'm Meredith Bouvier, a quantitative researcher with 13+ years in the education sector, including analyzing complex social systems through education research and policy. My background spans international organizations (World Bank, Global Partnership for Education, OECD) and direct field experience as a certified high school teacher in New York City.

I hold a PhD in Adult Education, MA in Mathematics, and BA in Mathematics, with expertise in statistical analysis, survey methodology, and large-scale administrative data.

**Research Interests**: Social science analytics, survey research methodology, big data applications in understanding human behavior, and translating complex statistical findings into actionable insights.

**Technical Skills**: Python (pandas, statistical analysis), SQL, survey design, longitudinal data analysis, data visualization, large administrative datasets.

Currently applying quantitative social science methods to international adult education research with UNESCO's GRALE datasets.

## Connect

- GitHub: [github.com/merrybouv](https://github.com/merrybouv)
- LinkedIn: [linkedin.com/in/meredithbouvier](https://www.linkedin.com/in/meredithbouvier/)
- Email: merrybouv@gmail.com

---

## Citation

If this analysis is helpful for your research:
```
Bouvier, M. (2025). K-12 Teacher Workforce Trends Analysis: Eight-Year 
Study of US Teacher Staffing Patterns (2016-2024). GitHub Repository.
https://github.com/merrybouv/k12-teacher-trends-analysis
```

---

*Last updated: October 1, 2025*  
*Analysis complete - moving to international adult education research*
