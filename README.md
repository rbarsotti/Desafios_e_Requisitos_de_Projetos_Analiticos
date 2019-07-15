# MBA Business Analytics & Big Data
## Desafios e Requisitos dos Projetos Analíticos
### Introduction to Azure & Apache Spark


#### Watson Studio:


https://dataplatform.cloud.ibm.com/

#### Trabalho Final:


https://drive.google.com/file/d/1rQmivpO9Mgv25x7sXK_NvB5rTGJVmSI5/view?usp=sharing


#### Apache Spark:


https://spark.apache.org/downloads.html


#### Utilizando o Spark na sua máquina local:



```R
# Instalando para Jupyter Notebook
install.packages("devtools")
install.packages('IRkernel')
IRkernel::installspec()

```R
Sys.setenv(SPARK_HOME="C:/Users/B31060.ACAD/Desktop/spark-2.4.2-bin-hadoop2.7")
## Set the library path
.libPaths(c(file.path(Sys.getenv("SPARK_HOME"),"R","lib"), .libPaths()))
## load the sparkR library
library(SparkR, lib.loc="C:/Users/B31060.ACAD/Desktop/spark-2.4.2-bin-hadoop2.7/R/lib")
## Se necessário set o caminho do java.exe
## Sys.setenv(JAVA_HOME="C:\\Program Files\\Java\\jdk1.8.0_201\\jre")
## Create a spark context and a sql context
sc<-sparkR.init(master = "local")
sqlContext<-sparkRSQL.init(sc)
