Втора лабораториска вежба по предметот Софтверско инженерство

Stefan Petrov 215023

Control Flow Graph
![215023 Lab2](https://github.com/stefaanpetrov/SI_2024_lab2_215023/assets/163160165/0a82670d-a2ea-41e4-b4c0-b2dafbde02ce)

Цикломатска комплексност
Цикломатската комплексност на овој код е 10, истата ја добив преку формулата P+1, каде што P е бројот на предикатни јазли. Во случајoв P=9, па цикломатската комплексност изнесува 10.


Every Branch

1.allItems == null, се праќа null вредност.
2.item.getBarcode() != null, фрла exception доколку има вредност null.
3.allowed.indexOf(c) == -1, фрла exception доколку баркодот е невалиден.
4.sum <= payment, прави проверка дали сумата на сите производи е помала или еднаква од 'payment'. 
5.sum > payment, прави проверка дали сумата на сите производи е поголем од 'payment'.

Multiple Condition

Проверка на условите: item.getPrice() > 300 && item.getDiscount() > 0 && item.getBarcode().charAt(0) == '0'

TTT(доколку сите услови се исполнети-assertTrue)
ТТF(доколку цената на сите производи е поголема од 300,има попуст поголем од 0 и не почнува со карактер '0'-assertTrue)
TFX(доколку цената на сите производи е поголема од 300 и нема попуст поголем од 0 -assertTrue)
FXX(доколку цената на сите производи не е поголема од 300-assertTrue)
