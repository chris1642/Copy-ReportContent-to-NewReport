# Copy & Export Non-Downloadable Power BI Reports

This PowerShell script lets you **clone the visuals and layout** (including bookmarks, report level measures, canvas size, etc) from a *non-downloadable* Power BI report into a *newly published blank report* that is **downloadable**.  

After copying, it also **exports** the new report as a `.pbix` file.

---

## ⚙️ Purpose & Steps

Some Power BI reports created in the service (especially web-authored ones) can’t be downloaded as `.pbix`.  

This script provides a clean workaround:


#### ✅ Step 1: Publish blank Power BI Report
> - Open a blank Power BI report
> - Go to Get Data → Power BI Semantic Models
> - Choose the same model that the non-downloadable report is connected to.
> - Save the report — no visuals are needed.
> - Publish the blank report to the same workspace as the original (or specify a different one later).


#### ✅ Step 2: Download Script file and Update Variables
> - Download CopyReportContentScript.txt
> - Add the Non-Downloadable Report's Workspace ID and Report ID under `$NonDownloadableReportWorkspaceID` and `$NonDownloadableReportID`
> - Add the Blank Report's ID (and Workspace if applicable) under `$BlankReportID`

#### ✅ Step 3: Run Script  
> Open PowerShell and run the CopyReportContentScript. You can:  
> - Copy/paste the full script, or  
> - Rename `CopyReportContentScript.txt` → `CopyReportContentScript.ps1` and run directly 
