# Impact of Remote Work on Mental Well-Being

## Introduction

A global HR consultancy asked Datafied Technologies to look into how remote work affects employee mental well-being. They provided data on 5,000 employees worldwide and wanted to know what's actually driving stress, isolation, and job satisfaction.

## The Data

20 columns, 5,000 rows. Demographics (age, gender, job role, industry, region), work setup (location, years of experience, hours worked, virtual meetings), and well-being measures (stress level, social isolation rating, satisfaction with remote work, mental health condition, sleep quality).

Two columns had missing values. Mental_Health_Condition was missing 1,196 values, Physical_Activity was missing 1,629. Neither looked like true missing data on closer inspection. A blank in Mental_Health_Condition most likely means no condition was reported, so it was filled as "None." Physical_Activity already had "Weekly" and "Daily" as options, so the blanks became a third category, "Rarely/Never." No duplicate rows were found.

## Approach

The analysis started broad: who is in the dataset, and what does the overall distribution of stress, isolation, and satisfaction look like. It then narrowed to group comparisons, checking whether those outcomes differ by work location, company support level, mental health condition, job role, gender, or region. A full correlation matrix across all numeric variables checked for relationships the group comparisons might have missed.

The Power BI dashboard was then built around one question: does the remote work experience itself (hours worked, virtual meetings, company support, work-life balance) change stress or satisfaction? It has two pages. Page 1 looks at the remote work factors directly. Page 2 compares stress, mental health, and sleep across work location, industry, and job role.

## Dashboard

### Remote work experience

- **Employees by Work Location:** Remote 1,714 (34.3%), Hybrid 1,649 (33.0%), Onsite 1,637 (32.7%). The split is close to even, so comparing the groups is fair.
- **Work Hours vs Stress Levels:** No trend between 20 and 60 hours a week. Average stress stays around 2.0 on the 1 to 3 scale.
- **Stress Level vs Number of Virtual Meetings:** Average stress moves up and down between about 1.95 and 2.10 with no consistent direction as meetings increase.
- **Satisfaction vs Work-Life Balance Rating:** Satisfaction stays near 2 at every rating from 1 to 5. A better work-life balance rating does not come with noticeably higher satisfaction here.
- **Stress Level vs Company Support for Remote Work:** Flat. More company support does not line up with lower stress.

### Location, industry, and role

- **Stress and Mental Health Condition by Work Location:** Each location's share of reported mental health conditions (about 34%, 33%, 33%) matches its share of employees. The line's axis starts at 32.5%, which makes the slope look steeper than it is. The gap between locations is under two percentage points.
- **Stress Level Distribution by Work Location:** Employees at stress levels 1, 2, and 3 are spread almost evenly across Remote, Hybrid, and Onsite, roughly 550 to 600 each. Remote workers are not over-represented at high stress.
- **Sleep Quality Distribution by Work Location:** Good, Average, and Poor sleep each cover roughly 500 to 600 employees in every location. No location stands out.
- **Stress Level by Job Role:** Average stress is about 2.0 for all seven roles.
- **Stress Level by Industry:** The only chart with a visible shape. Education has the highest average stress, and IT and Manufacturing the lowest. The whole spread is about 0.05 points on a 1 to 3 scale, so it is small. Average virtual meetings sit around 7 to 8 in every industry, so meetings don't explain the difference.

## Findings

Remote workers are not more stressed than hybrid or onsite workers. Stress, isolation, and satisfaction are nearly identical across work location, company support level, mental health condition, job role, gender, and region. Differences between groups are a few percentage points at most.

None of the remote work factors tested (hours worked, virtual meetings, company support, work-life balance) shows a meaningful relationship with stress or satisfaction. The correlation matrix agrees: every pairwise correlation between numeric variables fell between -0.03 and 0.03.

The one pattern worth a closer look is industry. Education sits above IT and Manufacturing on average stress. The gap is small, so it needs a larger sample or a significance test before anyone acts on it.

**Overall finding:** No clear driver of stress was identified in this dataset.

## Recommendations

Personalized, employee-level support (regular check-ins, opt-in wellness resources) is likely more effective than broad policy changes, since no single lever in this dataset explains the variation in outcomes.

Factors not captured here, such as manager relationship quality, workload intensity, or personal circumstances, are more likely explanations for individual variation in well-being than the demographic and structural variables available in this dataset.

There is no basis in this data for assuming that remote work itself, as opposed to hybrid or onsite arrangements, drives stress or isolation. Policy decisions about work location should not rely on this dataset alone.

The industry difference is worth testing in a follow-up with more data.

## Links

Power BI File (.pbix): <https://github.com/simonjoshua00711-create/remote-work-mental-wellbeing-analysis/blob/main/Remote_Work_Mental_Wellbeing_Analysis.pbix>

GitHub Repository: <https://github.com/simonjoshua00711-create/remote-work-mental-wellbeing-analysis>
