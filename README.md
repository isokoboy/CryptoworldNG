---
title: "cars analysis"
author: "onome"
date: "2025-08-06"
output: html_document
---

```{r setup, include=FALSE}
knitr::opts_chunk$set(echo = TRUE)
```


```{r}
library(readr) 
library(ggplot2)
```

```{r}
carsdf<- read.csv("cars.csv")
``` 


```{r}
attributes(carsdf)
```

```{r}
summary(carsdf) 
```

```{r}
str(carsdf) 
```

```{r}
names(carsdf) 
```

#data preprocecessing/data cleaning
```{r}
duplicated(carsdf)
```

```{r}
is.na(carsdf)
```


##inconsistencies check for inconsistencies 
# binning


```{r}
boxplot(carsdf$speed.of.car)
```

```{r}
boxplot(carsdf$distance.of.car)
```


```{r}
carsdf$name.of.car
```

```{r}
carsdf$speed.of.car
```


```{r}
carsdf$distance.of.car
```

```{r}
hist(carsdf$speed.of.car)
```

```{r}
hist(carsdf$distance.of.car)
```

```{r}
plot(carsdf$distance.of.car,carsdf$speed.of.car )
```

```{r}
qqnorm(carsdf$speed.of.car)
```


```{r}
c <- ggplot(carsdf, aes(speed.of.car))
```




 
