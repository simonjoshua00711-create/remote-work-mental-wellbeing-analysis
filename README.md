# Impact of Remote Work on Mental Well-Being

## Introduction
A global HR consultancy asked Datafied Technologies to look into how remote work affects employee mental well-being. They provided data on 5,000 employees worldwide and wanted to know what's actually driving stress, isolation, and job satisfaction.

## The Data
20 columns, 5,000 rows. Demographics (age, gender, job role, industry, region), work setup (location, years of experience, hours worked, virtual meetings), and well-being measures (stress level, social isolation rating, satisfaction with remote work, mental health condition, sleep quality).

Two columns had missing values. Mental_Health_Condition was missing 1,196 values, Physical_Activity was missing 1,629. Neither looked like true missing data on closer inspection. A blank in Mental_Health_Condition most likely means no condition was reported, so it was filled as "None." Physical_Activity already had "Weekly" and "Daily" as options, so the blanks became a third category, "Rarely/Never." No duplicate rows were found.

## Approach
The analysis started broad: who is in the dataset, and what does the overall distribution of stress, isolation, and satisfaction look like. It then narrowed to group comparisons, checking whether those outcomes differ by work location, company support level, mental health condition, job role, gender, or region. Finally, a full correlation matrix was run across all numeric variables to check for relationships the group comparisons might have missed.

## Findings
Employee counts are close to even across groups. Remote workers: 1,714. Hybrid: 1,649. Onsite: 1,637. Stress levels split about the same way, with High, Medium, and Low all within a few dozen of each other.

No single factor tested shows a meaningful relationship with well-being outcomes. Stress, isolation, and satisfaction remain nearly identical across work location, company support level, mental health condition, job role, gender, and region. Differences between groups are a few percentage points at most.

The correlation matrix confirms this. Every pairwise correlation between numeric variables fell between -0.03 and 0.03, indicating no meaningful linear relationship between any individual factor and stress, isolation, or satisfaction.

## Recommendations
The data does not support attributing stress or isolation to any single factor, so a few implications follow:

Personalized, employee-level support (regular check-ins, opt-in wellness resources) is likely more effective than broad policy changes, since no single lever in this dataset explains the variation in outcomes.

Factors not captured here, such as manager relationship quality, workload intensity, or personal circumstances, are more likely explanations for individual variation in well-being than the demographic and structural variables available in this dataset.

There is no basis in this data for assuming that remote work itself, as opposed to hybrid or onsite arrangements, drives stress or isolation. Policy decisions about work location should not rely on this dataset alone.

## Links
Power BI File (.pbix): https://github.com/simonjoshua00711-create/remote-work-mental-wellbeing-analysis/blob/main/Remote_Work_Mental_Wellbeing_Analysis.pbix

GitHub Repository: https://github.com/simonjoshua00711-create/remote-work-mental-wellbeing-analysis

