# MANUFACTURING LINE PRODUCTIVITY

Analysis of manufacturing line downtimes for fictitious soft drinks manufacturer.

**Dataset source:** kaggle.com
**Technologies used:** Power Query, Power BI

## I. OBJECTIVES

 - Identify downtime patterns.
 - Come up with recommendations aiming to decrese downtime rate.

## II. ANALYTICAL PROCESS

### 1. DATASET

Dataset consists of 4 tables:
 - `Line productivity`
 - `Products`
 - `Downtime factors`
 - `Line downtime`

### 2. DATA VALIDATION AND PREPARATION

Power Query was used to review the data for potentially missing inputs or incorrect format.
On top, the following transformations have been done:
 a. Unpivoting table `Line downtime`. The table had a matrix format in the dataset. In order to enable full integration with data model, it has been converted to plain table.
 b. Adding `Batch duration` column to `Line productivity` table.

 ### 3. POWER BI ANALYSIS

Power BI report is divided into 2 sections.
First section describes key measures and statistics regarding line productivity and downtimes.
The second section summarizes main conclusions, recommendations and simulates improvements expected after eliminating selected downtime factors.

### 4. KEY TAKEAWAYS
- Almost all batches (35 out of 38) were completed with delay. 25 out of 38 batches were at least partially delayed due to operator error.
- All delays sum up to 23h 08m, of which 12h 56m (56%) were caused by operator error.
- The most common downtime reason is the need for machine adjustment (operator error), with 12 occurrences causing 05h 32m of downtime. This is followed by two factors outside operator control: machine failure and inventory shortage. Together, these three factors account for 58% of time lost.
- Batch change and machine adjustment are the factors causing the longest downtimes, each lasting up to 60 minutes. The other two, causing up to 44 minutes of downtime, are batch coding error and inventory shortage.

### 5. RECOMMENDATIONS
- Gather operator feedback on root causes of machine adjustments, batch change, and batch coding errors, then develop and train on targeted solutions.
- Check with maintenance whether any action can be taken to reduce machine failures.
- Work out a solution with the warehouse team to address inventory shortage issues.




