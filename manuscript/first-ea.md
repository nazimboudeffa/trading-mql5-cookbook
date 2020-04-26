# Votre Premier Script

Nous allons créer un petit script pour emettre un commentaire à chaque fois que le prix de la paire EURUSD baisse ou augmente

```c
void onTick()
{

  MqlRates PriceInfromation[];

  ArraySetAsSeries(PriceInformation, true);

  int Data = CopyRates(Symbol(), Period(), 0 Bars(Symbol(), Period()), PriceInformation);

  if (PriceInformation[1].close > PriceInformation[2].close) comment ("A la hausse");
  if (PriceInformation[1].close < PriceInformation[2].close) comment ("A la baisse");

}
```

Pour executer ce sctript, voici mes étapes à suivre et qui seront valables tout au long de ce livre

![](manuscript/images/step1.png)
![](manuscript/images/step2.png)
![](manuscript/images/step3.png)
![](manuscript/images/step4.png)
![](manuscript/images/step5.png)
![](manuscript/images/step6.png)
![](manuscript/images/step7.png)
