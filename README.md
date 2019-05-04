# MBA Business Analytics & Big Data
## Desafios e Requisitos dos Projetos Analíticos
### Introduction to Azure & Apache Spark


Watson Studio:

https://dataplatform.cloud.ibm.com/

Trabalho Final:

https://pmbamay.blob.core.windows.net/mbamay/EFC_WAYSIDES.csv?sp=r&st=2019-05-04T11:43:26Z&se=2019-08-10T19:43:26Z&spr=https&sv=2018-03-28&sig=UmfbElFeLvEuAuQlvTx7oIvz2ctkUOqvAJpo8%2FzpIs0%3D&sr=b


Utilizando o Spark na sua máquina local:

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
