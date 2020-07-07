# MBA Business Analytics & Big Data
## Desafios e Requisitos dos Projetos Analíticos
### Introduction to Azure & Apache Spark

#### Trabalho Final:


https://drive.google.com/file/d/1rQmivpO9Mgv25x7sXK_NvB5rTGJVmSI5/view?usp=sharing


#### Apache Spark:


https://spark.apache.org/downloads.html


#### Utilizando o Spark na sua máquina local:



```R
# Instalando para Jupyter Notebook
#install.packages("devtools")
#install.packages('IRkernel')
#IRkernel::installspec()


Sys.setenv(SPARK_HOME="C:\\Users\\user01\\Downloads\\spark-3.0.0-bin-hadoop2.7\\spark-3.0.0-bin-hadoop2.7")
## Set the library path
.libPaths(c(file.path(Sys.getenv("SPARK_HOME"),"R","lib"), .libPaths()))
## Load the SparkR library
library(SparkR, lib.loc="C:\\Users\\user01\\Downloads\\spark-3.0.0-bin-hadoop2.7\\spark-3.0.0-bin-hadoop2.7\\R\\lib")

