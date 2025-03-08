# MIDTERM LAB TASK 2
## 1. Task Description:
Company X would like to extract some useful information from the UnclenedDSJObs csv taken
from a Job Posting site available in Kaggle. There are a lot of columns available but focus only
on generating insights that will answer the following questions:
1. Which Job Roles pay the highest and least.
2. What size companies pay the best.
3. Where Job Roles or Job Titles pay the best and least in a specific state.
 
## 2. Screenshot Before Cleaning and Transformation  👇 
![Image](https://github.com/user-attachments/assets/5582453b-123d-4619-8f02-c17993a9db86)

## 3. Step-by-step process in Data Cleaning and Transformation
1. let
    Source = Excel.Workbook(File.Contents("C:\Users\Admin\Downloads\Uncleaned_DS_jobs (PENDING).xlsx"), null, true),
    Table_1_Table = Source{[Item="Table_1",Kind="Table"]}[Data],
    #"Changed Type" = Table.TransformColumnTypes(Table_1_Table,{{"index", Int64.Type}, {"Job Title", type text}, {"Salary Estimate", type text}, {"Job Description", type text}, {"Rating", type number}, {"Company Name", type text}, {"Location.1", type text}, {"Location.2", type text}, {"Headquarters", type any}, {"Size", type any}, {"Founded", Int64.Type}, {"Type of ownership", type any}, {"Industry", type any}, {"Sector", type any}, {"Revenue", type any}, {"Competitors", type any}, {"Min Sal", Int64.Type}, {"Max Sal", Int64.Type}, {"Role Type", type text}}),
    #"Added Custom" = Table.AddColumn(#"Changed Type", "Role Type.1", each if Text.Contains([Job Title], "Data Scientist") then
"Data Scientist"
else if Text.Contains([Job Title], "Data Analyst") then
"Data Analyst"
else if Text.Contains([Job Title], "Data Engineer") then
"Data Engineer"

else if Text.Contains([Job Title], "Machine Learning") then
"Machine Learning Engineer"
else
"other"),
    #"Changed Type1" = Table.TransformColumnTypes(#"Added Custom",{{"Role Type", type text}}),
    #"Removed Columns" = Table.RemoveColumns(#"Changed Type1",{"Role Type"}),
    #"Renamed Columns" = Table.RenameColumns(#"Removed Columns",{{"Role Type.1", "Role Type"}, {"Location.2", "State Abbreviations"}}),
    #"Duplicated Column" = Table.AddColumn(#"Renamed Columns", "MinCompanySize", each [Min Sal], type number),
    #"Duplicated Column1" = Table.DuplicateColumn(#"Duplicated Column", "MinCompanySize", "MinCompanySize - Copy"),
    #"Changed Type2" = Table.TransformColumnTypes(#"Duplicated Column1",{{"MinCompanySize - Copy", Int64.Type}}),
    #"Renamed Columns1" = Table.RenameColumns(#"Changed Type2",{{"MinCompanySize - Copy", "MaxCompanySize"}}),
    #"Competitors -1" = Table.SelectRows(#"Renamed Columns1", each ([Competitors] = -1)),
    #"Revenue 0 | Industry -1" = Table.SelectRows(#"Competitors -1", each ([Revenue] = "Unknown / Non-Applicable") and ([Industry] = -1)),
    #"Split Column by Character Transition" = Table.SplitColumn(#"Revenue 0 | Industry -1", "Company Name", Splitter.SplitTextByCharacterTransition((c) => not List.Contains({"0".."9"}, c), {"0".."9"}), {"Company Name.1", "Company Name.2", "Company Name.3"}),
    #"Removed Columns1" = Table.RemoveColumns(#"Split Column by Character Transition",{"Company Name.2", "Company Name.3"}),
    #"Renamed Columns2" = Table.RenameColumns(#"Removed Columns1",{{"Location.1", "Location"}, {"Company Name.1", "Company Name"}}),
    #"Removed Columns2" = Table.RemoveColumns(#"Renamed Columns2",{"Job Description"})
in
    #"Removed Columns2"

## Screenshot After Cleaning and Transformation (Final Output) 👇 
![Image]
