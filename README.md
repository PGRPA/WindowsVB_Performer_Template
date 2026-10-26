## To modify:

1. Change 2 files names:
   * Data/Config_Process_Name_Performer.xlsx
   * Tests/TS_Process_Name_Performer.xlsx
2. In 3 Workflows change 2 variables:
   * Initialization/Init Configs
   * _Sandbox/Init Configs
   * TC_WorkflowName/Init Configs
     * Assign - strConfigFilePathLocal
     * Get Asset - strConfigFilePath

* Edit process: name, description, author here and in project.json
* Edit Main Workflow properties name
* Edit Config values and move file to another directory if needed
* Edit Project Settings
* Add assets to Orchestrator if needed
* Add Queue to Orchestrator
* Re-add test data Excel file, to TC workflows if needed
* Update packages if needed
* Open each file & Workflow for error check
* Remove unused imports
* Remove unused Workflows
* Remove unnecessary Then-Else sequences
* Remove unused entries in Config
* Remove marked in yellow Settings & Constants entries in Config
* Run analyzer
* Run parse XAML

## Delete if not used:

##### Activities\Workflows <> Files <> Config entries

* Build Data Table - dtExcelReportTable <> <>
* TC_WorkflowName.xaml <> TS_Process_Name.xlsx <>
* AppXYLogin.xaml <> <> AppXYLogin
* AppXYLogout.xaml <> <>
* ExcelGetTable.xaml <> Input_File.xlsx <> ExcelInputFilePath, ExcelInputSheet, RequiredColumnNames, ExcelGetTable
* ExcelAddToReport.xaml <> yyyy-MM-dd_Template.xlsx <> ExcelReportTempPath, ExcelReportTempSheet, ExcelReportFolder, ExcelReportName, ExcelAddToReport
* OutlookGetEmails.xaml <> <> OutlookInboxFolderPath, OutlookEmailsAmount, OutlookGetEmails
* OutlookMoveEmail.xaml <> <> OutlookInboxFolderPath, OutlookEmailsAmount, OutlookGetEmails
* APIRunQuery.xaml <> <> APIRunQuery
* AssetBlockAndRelease <> <> BlockAssetNameB4UseReport, BlockAssetB4UseReport, AssetBlockAndRelease
* FolderForReportsCreate.xaml <> <>
* FoldersCreate.xaml <> <>
* QueueGetAllItems.xaml <> <>
* ShowRobotStatus.xaml <> Robot_Zakończył_Pracę.txt <> RobotStatusFolderPath, ShowRobotStatus
* SQLRunQuery.xaml <> <> SQLRunQuery
##