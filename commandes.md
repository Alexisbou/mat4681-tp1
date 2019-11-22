# Commandes utilisées pour TP1 #

\***donnees est le nom de ma variable**\*

## Probleme 1 ##

#### Question 1 #####
a)  `min(donnees$Debut)`= 1333.9, `max(donnees$Debut)`=1564.98,`median(donnees$Debut)` = 1475.745, `mean(donnees$Debut)`= 1476.514
			

b)  `hist(donnees$Debut, xlab="Valeur", ylab = "Fréquence", main = "Histogramme de l'indice S&P/TSX en début de journée")`

c)  `boxplot(donnees$Debut,horizontal = TRUE, xlab="Valeur",main = "Diagramme en moustache de l'indice S&P/TSX en début de journée")`

d)  `boxplot.stats(donnees$Debut,do.conf=TRUE, do.out=TRUE)` = donnees extremement faibles < 1374.060  et extremement hautes > 1564.980 <br>
`sum(donnees$Debut < 1374.060)` = 1 <br>

#### Question 2 ####
a)  `min(donnees$Fin)`=1325.19, `max(donnees$Fin)` = 1565.15, `mean(donnees$Fin)` = 1476.142, `median(donnees$Fin)` = 1476.46

b) `hist(donnees$Fin, xlab="Valeur", ylab = "Fréquence", main = "Histogramme de l'indice S&P/TSX en fin de journée")`

c) `sd(donnees$Fin)`= 47.30821 donc les extremes sont si x < 1381.526 ou x > 1570.758. donc `sum(donnees$Fin < 1381.526)` = 6

d) `(sum(donnees$Fin > donnees$Debut*1.01) * 100) /250` = 11.6%

#### Question 3 ####
`qnorm(.99)` est la valeur pour 0.98 de confiance
`mean(donnees$Debut) + qnorm(.99) * sd(donnees$Debut)/sqrt(250)` et `mean(donnees$Debut) - qnorm(.99) * sd(donnees$Debut)/sqrt(250)`, donc pour notre distribution, il y a 98% de probabilite que la moyenne se situe entre entre 1469.675 et 1483.352.

####Question 4####
2.33 est la valeur pour 0.98 de confiance
`mean(donnees$Fin) - qnorm(.99) * sd(donnees$Fin)/sqrt(250)` et `mean(donnees$Fin) + qnorm(.99) * sd(donnees$Fin)/sqrt(250)`, donc pour notre distribution, il y a 98% de probabilite que la moyenne se situe entre entre 1469.182 et 1483.103.

# Probleme 2 #

#### Question 1 ####
qnorm


n2=100, x2(fumeurs)=25

