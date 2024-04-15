# Jalali Date in google sheet

Calculate today:
```
=CONCATENATE((INT((TODAY()-7385)/365.25)+1299),"-",(MOD(IF(INT(MOD((TODAY()-7385)*100,36525)/100)<186,INT(INT(MOD((TODAY()-7385)*100,36525)/100)/31),IF(MOD(INT((TODAY()-7385)/365.25),4)=0,INT((INT(MOD((TODAY()-7385)*100,36525)/100)-186)/30)+6,IF(INT(MOD((TODAY()-7385)*100,36525)/100)<336,INT((INT(MOD((TODAY()-7385)*100,36525)/100)-186)/30)+6,INT((INT(MOD((TODAY()-7385)*100,36525)/100)-336)/29)+11))),12)+1),"-",(IF(INT(MOD((TODAY()-7385)*100,36525)/100)<186,MOD(INT(MOD((TODAY()-7385)*100,36525)/100),31)+1,IF(MOD(INT((TODAY()-7385)/365.25),4)=0,MOD(INT(MOD((TODAY()-7385)*100,36525)/100)-186,30)+1,IF(INT(MOD((TODAY()-7385)*100,36525)/100)<336,MOD(INT(MOD((TODAY()-7385)*100,36525)/100)-186,30)+1,MOD(INT(MOD((TODAY()-7385)*100,36525)/100)-336,29)+1)))))
```

Calculate for cell:
```
=CONCATENATE((INT((A1-7385)/365.25)+1299),"-",(MOD(IF(INT(MOD((A1-7385)*100,36525)/100)<186,INT(INT(MOD((A1-7385)*100,36525)/100)/31),IF(MOD(INT((A1-7385)/365.25),4)=0,INT((INT(MOD((A1-7385)*100,36525)/100)-186)/30)+6,IF(INT(MOD((A1-7385)*100,36525)/100)<336,INT((INT(MOD((A1-7385)*100,36525)/100)-186)/30)+6,INT((INT(MOD((A1-7385)*100,36525)/100)-336)/29)+11))),12)+1),"-",(IF(INT(MOD((A1-7385)*100,36525)/100)<186,MOD(INT(MOD((A1-7385)*100,36525)/100),31)+1,IF(MOD(INT((A1-7385)/365.25),4)=0,MOD(INT(MOD((A1-7385)*100,36525)/100)-186,30)+1,IF(INT(MOD((A1-7385)*100,36525)/100)<336,MOD(INT(MOD((A1-7385)*100,36525)/100)-186,30)+1,MOD(INT(MOD((A1-7385)*100,36525)/100)-336,29)+1)))))
```

Tags:
```
#google_sheet #google #sheet
```

Related:
```
* https://googleche.ir/%D8%AA%D8%A8%D8%AF%DB%8C%D9%84-%D8%AA%D8%A7%D8%B1%DB%8C%D8%AE-%D9%85%DB%8C%D9%84%D8%A7%D8%AF%DB%8C-%D8%A8%D9%87-%D8%B4%D9%85%D8%B3%DB%8C-%D8%AF%D8%B1-%DA%AF%D9%88%DA%AF%D9%84-%D8%B4%DB%8C%D8%AA/
```