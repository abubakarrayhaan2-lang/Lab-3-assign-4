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
> # Lab 3 work1
> df_data<- data.frame(
+   name= c("Alice", "Bob", "Hauwa", "Hassan", "Sulaiman"),
+   age= c(30, 25, 30, 27 ,28),
+   location= c("USA", "UK"," Nigeria","Niger", "Togo")
+  )
> filename <- "C:/data.csv"
> write.csv(df_data,filename)
> data<-read.csv("C:/data.csv")
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
