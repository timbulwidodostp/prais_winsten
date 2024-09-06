# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Prais-Winsten estimator for AR(1) serial correlation Use prais_winsten (prais) With (In) R Software
install.packages("prais")
install.packages("wooldridge")
library("prais")
library("wooldridge")
library("lmtest")
prais_winsten = read.csv("https://raw.githubusercontent.com/timbulwidodostp/prais_winsten/main/prais_winsten/prais_winsten.csv",sep = ";")
# Estimation Prais-Winsten estimator for AR(1) serial correlation Use prais_winsten (prais) With (In) R Software
prais_winsten <- prais_winsten(lchnimp ~ lchempi + lgas + lrtwex + befile6 + affile6 + afdec6, data = prais_winsten, index = "t")
summary(prais_winsten)
coeftest(prais_winsten, vcov. = vcovHC(prais_winsten, "HC1"))
# Prais-Winsten estimator for AR(1) serial correlation Use prais_winsten (prais) With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished