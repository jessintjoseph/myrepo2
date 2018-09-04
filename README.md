# myrepo2
this is a line from Rstudio pt final
(5^2)*(10-8)/3 + 1
x <- (5^2)*(10-8)/3 + 1
x
x+1
n <- 50
x/n
class(x)
x1 <- c(-0.1, 0.3, -0.9, 0.2, -0.6, -2.3, -0.1, 0.3, -0.9, 0.2, -0.6, -2.3)
x2 <- c("red", "blue", "green", "purple")
x3 <- x1 > 0
x3
names(x1) <- c("Michael", "Cameron", "Taylor", "Chad", "Jessin", "Shaowli", "Shama", "Meera", "Ashley", "Ximena", "Gavin", "Courtney")
x1
names(x1)
x1["Jessin"]
X <- matrix(x1, nrow = 2)
X
X1 <- matrix(rnorm(6), ncol=3)
X2 <- matrix(rnorm(6), ncol=3)
rbind(X1,X2)
cbind(X1,X2)
setwd("~/UKOneDrive/GLM")
directory <- setwd("~/UKOneDrive/GLM")
tips <- file.path(directory, "tips.txt")
tips2 <- read.delim(tips)
head(tips2)
with(tips2, mean(TotBill))
tips2$Rate <- with(tips2, Tip/TotBill)
library(tidyverse)
tips2 <- tips2 %>%
mutate(Tip20plus = Rate > 0.2)
