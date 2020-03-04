# L0-tracking-backup

This repo stores all the raw files needed for the Blizzard Sensor Health tab and Domain Report emails.  

:rotating_light: **2019 data have been moved to the N:/ Drive**  :rotating_light:  
_2019 data are now located in `N:/Common/FIU-FSU/Monitoring/Sensor Health Data/2019/`. 2020 Data will be archived in `N:/Common/FIU-FSU/Monitoring/Sensor Health Data/2020/` in January of 2021._

## File structure
Files in this repo mirror the directory used by the Sensor Health app. Server files are located at `/scratch/SOM/rollingAnalysis/` on the `den-devissom-1` VM.
> - **/RptDp00/alerts/**: Tables of percent of data product affected, by sites and report type. Stored as RDS files, one for each date.
- **/RptDp00/history/**: Tables showing the length of time an issue has persisted for each site, saved as and RDS, one for each report and date.
- **/RptDp00/reports/**: Tables of report values on a stream site basis, in nested lists by report type. One RDS file per day.
- **/RptDp00/smartAlerts/**: Files for Domain Report email generation. Markdown and HTML versions of DR output, as well DR text in table format as RDS files.
- **/RptDp00/test/**: Unfortunately named. The raw statistics for all streams, saved on a site-date basis as CSV.
- **/RptDp00/warnings/**: Tables of percent of data product affected, by sites and report type. Stored as RDS files, one for each date.
- **/RptDp00/www/**: Files used in the "Learn how to use this tab" box.
