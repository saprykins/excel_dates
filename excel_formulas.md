from date ~ 01/07/2023 and time ~ 08h00 -> 07/14/2023 08:00:00
date:  
```
=TEXT(DAY(AE2),"00") & "/" & TEXT(MONTH(AE2), "00") & "/" & YEAR(AE2)
```
time:  
```
=IF(ISBLANK(U2),"00:00:00",TEXT(SUBSTITUTE(U2,"h",":"),"hh:mm:ss"))
```

total:  
```
=CONCAT(TEXT(DAY(AE2),"00") & "/" & TEXT(MONTH(AE2), "00") & "/" & YEAR(AE2), " ", IF(ISBLANK(U2),"00:00:00",TEXT(SUBSTITUTE(U2,"h",":"),"hh:mm:ss")))
```
