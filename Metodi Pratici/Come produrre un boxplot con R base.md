La sintassi è
```r
boxplot(var~grp) #base

boxplot(var~grp, data=dataset, col="color",...)
```
Dove `var` è la variabile in analisi, e `grp` è la variabile di raggruppamento.
È possibile produrre un unico boxplot usando la sintassi `boxplot(var)` dove `var` è un vettore singolo di dati.