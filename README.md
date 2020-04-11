# Software-Measurement-Project---F

1)File structure of the repo

  1. Metric 1- (Statement Coverage): It contains the raw data, commands to get the metric and results of the Statement coverage for each                                         project
  2. Metric 2 -(Branch Coverage) : It contains all the data, results and commands to get the metrics for the branch coverage of all the                                        projects
  3. Metric 3 - (Test Suite Effectiveness): It contains three sub-folders (Commands, configurations, PITest Reports) which have the                                                    information of the metric 3 for all the projects 
  4. Metric 4 -(Cyclomatic Compexity): It has all the resulted csv files for all projects of cyclomatic complexity and the tools and commands                                      used to extract the reports
  
 5. Metric 5 -(Adaptive Maintenance Effort): It has the result files for all the versions compared to each another, giving the total DLOC and then the calclated Effort for each pair of compared files. It also has the ruby script that is used to compare 2 versions of the project. There is no pre-requisite to run the script, just take the terminal node to the base folder where the project is and then run the script with two version names in the following command
   - **git log version1..version2 --pretty=format:\"%an\" -- shortstat #{ARGV.join(' ')}**

 6. Metric 6 -(Post Release Defect Density): It has the screenshots of  the file that records the number of bugs and and the version size(CLOC) and this gives the defect density for each version of the selected project. 
 
 7. POM FIles: It contains Pom Files for each of the project used for extracting Data for Code Coverage.
  
2)Requirements for running the script
 For Post Release Defect Density, we need to run  the following commandon Mac Terminal :
   - **brew install cloc**
   - **git checkout version**
 Then going to the version that we want to analyze we run the command 
   - **cloc**
 It will give the data as shown in the screenshots for total number of source code lines.
 For number of bugs we have used Jira.
 
 Correlation(Python Script)
 numpy, pandas, scipy

3)Team F:
  Uchechukwu Iroegbu , Adeola Adeniji, Navjot Kaur, Mohammad Ali Hasheminezhad, Bhavpreet Kaur       
