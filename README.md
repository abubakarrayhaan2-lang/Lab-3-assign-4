> # Rayhaan Abubakar
> # Rayhaan Abubakar

R version 4.5.1 (2025-06-13 ucrt) -- "Great Square Root"
Copyright (C) 2025 The R Foundation for Statistical Computing
Platform: x86_64-w64-mingw32/x64

R is free software and comes with ABSOLUTELY NO WARRANTY.
You are welcome to redistribute it under certain conditions.
Type 'license()' or 'licence()' for distribution details.

  Natural language support but running in an English locale

R is a collaborative project with many contributors.
Type 'contributors()' for more information and
'citation()' on how to cite R or R packages in publications.

Type 'demo()' for some demos, 'help()' for on-line help, or
'help.start()' for an HTML browser interface to help.
Type 'q()' to quit R.

[Previously saved workspace restored]

> # Rayhaan Abubakar
> # Rayhaan Abubakar
> # Lab 3 work1
> df_data<- data.frame(
+   name= c("Alice", "Bob", "Hauwa", "Hassan", "Sulaiman"),
+   age= c(30, 25, 30, 27 ,28),
+   location= c("USA", "UK"," Nigeria","Niger", "Togo")
+  )
> write.csv(df_data, file = "data.csv")
> 
> data <- read.csv("~/data.csv")
> View(data)
> 
> install.packages("readxl")
Warning in install.packages("readxl") :
  'lib = "C:/Program Files/R/R-4.5.1/library"' is not writable
--- Please select a CRAN mirror for use in this session ---
Warning: failed to download mirrors file (cannot open URL 'https://cran.r-project.org/CRAN_mirrors.csv'); using local file 'C:/PROGRA~1/R/R-45~1.1/doc/CRAN_mirrors.csv'
Warning: unable to access index for repository https://muug.ca/mirror/cran/src/contrib:
  cannot open URL 'https://muug.ca/mirror/cran/src/contrib/PACKAGES'
Warning: unable to access index for repository https://muug.ca/mirror/cran/bin/windows/contrib/4.5:
  cannot open URL 'https://muug.ca/mirror/cran/bin/windows/contrib/4.5/PACKAGES'
Warning messages:
1: In download.file(url, destfile = f, quiet = TRUE) :
  URL 'https://cran.r-project.org/CRAN_mirrors.csv': status was 'Could not resolve hostname'
2: package ‘readxl’ is not available for this version of R

A version of this package for your version of R might be available elsewhere,
see the ideas at
https://cran.r-project.org/doc/manuals/r-patched/R-admin.html#Installing-packages 
> library(readxl)
Error in library(readxl) : there is no package called ‘readxl’
> 
> library(readxl)
Error in library(readxl) : there is no package called ‘readxl’
> Score <- read_excel("Score.xlsx")
Error in read_excel("Score.xlsx") : could not find function "read_excel"
> View(Score)
Error: object 'Score' not found
> 
> library(dplyr)
Error in library(dplyr) : there is no package called ‘dplyr’
> df_data_filtered<- filter(df_data, age>20)
Error: object 'age' not found
> df_data_selected<- select(Score, Score)
Error in select(Score, Score) : could not find function "select"
> print(df_data_selected)
Error: object 'df_data_selected' not found
> data_selected<- summarise(df_data_selected, mean_score=mean(Score))
Error in summarise(df_data_selected, mean_score = mean(Score)) : 
  could not find function "summarise"
> data_filtered<- filter(Score, Score > data_selected)
Error: object 'Score' not found
> print(data_filtered)  
Error: object 'data_filtered' not found
> # Rayhaan Abubakar
> # Lab 3 work1
> df_data<- data.frame(
+   name= c("Alice", "Bob", "Hauwa", "Hassan", "Sulaiman"),
+   age= c(30, 25, 30, 27 ,28),
+   location= c("USA", "UK"," Nigeria","Niger", "Togo")
+  )
> filename <- "C:/data.csv"
> write.csv(df_data,filename)
Error in file(file, ifelse(append, "a", "w")) : 
  cannot open the connection
In addition: Warning message:
In file(file, ifelse(append, "a", "w")) :
  cannot open file 'C:/data.csv': Permission denied
> data<-read.csv("C:/data.csv")
Error in file(file, "rt") : cannot open the connection
In addition: Warning message:
In file(file, "rt") :
  cannot open file 'C:/data.csv': No such file or directory
> print(head(data))
  X     name age location
1 1    Alice  30      USA
2 2      Bob  25       UK
3 3    Hauwa  30  Nigeria
4 4   Hassan  27    Niger
5 5 Sulaiman  28     Togo
> library(readxl)
Error in library(readxl) : there is no package called ‘readxl’
> file_path <- "C:/score.xlsx.xslx"
> data <- read_excel(file_path)
Error in read_excel(file_path) : could not find function "read_excel"
> data <- read_excel(file_path)
Error in read_excel(file_path) : could not find function "read_excel"
> print(data)
  X     name age location
1 1    Alice  30      USA
2 2      Bob  25       UK
3 3    Hauwa  30  Nigeria
4 4   Hassan  27    Niger
5 5 Sulaiman  28     Togo
> print(data)
  X     name age location
1 1    Alice  30      USA
2 2      Bob  25       UK
3 3    Hauwa  30  Nigeria
4 4   Hassan  27    Niger
5 5 Sulaiman  28     Togo
> save.image("C:\\Users\\HP\\OneDrive\\Documentos\\Lab 4.R")
> save.image("C:\\Users\\HP\\OneDrive\\Desktop\\Assignment 4")
> save.image("C:\\Users\\HP\\OneDrive\\Desktop\\Assignment 4.R")
> 
