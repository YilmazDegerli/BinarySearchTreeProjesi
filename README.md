# Veri Yapilari ve Algoritmalar Kursu Bitirme Projesi

## Binary-Search-Tree Projesi

Proje 3

1. [7, 5, 1, 8, 3, 6, 0, 9, 4, 2] dizisinin Binary-Search-Tree aşamalarını yazınız?

Örnek: root x'dir. root'un sağından y bulunur. Solunda z bulunur vb.

## CEVAP

1. Binary-Search-Tree ile arama islemlerine baslanirken bir root belirlenir ve her seferinde elimizdeki sayiyi bu sayidan büyük mü kücük mü diye sorulur ve büyükse sag tarfa kücükse sol tarafa yazilir. Örnegin Root sayimiz "8" olsun.  En basa "8" yazilir. Sonra "7" sayisini aliriz ve sorariz "8"den büyuksen saga gec kücüksen sola gec.Kücük oldugu icin sola gecer.
                          8
                      7
daha sonra 5 sayisina ayni soruyu sorariz ve "8" den kücük oldugu icin sola gecer. Solda "7" sayisi oldugu icin bu sefer de "5" sayisini "7" sayisi ile karsilastiririz ve 5<7 oldugu icin "5" sayisini "7 nin soluna ekleriz.
                          8
                      7
                   5
"1" e de ayni sorular sorulur 1<8 sola gec, 1<7 sola gec, 1<5 sola gec ve en sola gecer, baska sayi kalmadigi icin orda kal.
                          8
                        7
                    5       
                 1 
Sonra "3" e ayni sorular sorulur. 3<8 sola gec, 3<7 sola gec, 3<5 sola gec, 3>1 "1" in sagina gec, baska sayi kalmadigi icin orda kal.
                           8
                        7
                    5       
                 1 
                    3


Sonra "6" ya ayni sorular sorulur. 6<8 sola gec, 6<7 sola gec, 6>5 "7" in sagina gec, baska sayi kalmadigi icin orda kal.
                            8
                        7
                    5       
                 1    6
                   3


Sonra "0" a ayni sorular sorulur. 0<8 sola gec, 0<7 sola gec, 0<5 sola gec, 0<1 sola gec ve en sola gecer, baska sayi kalmadigi icin orda kal.
                          8
                        7
                    5       
                 1    6
              0    3
Sonra "9" a ayni sorular sorulur. 9>8 saga gec ve en saga gecer, baska sayi kalmadigi icin orda kal.
                          8
                        7   9
                    5       
                 1    6
              0    3
Sonra "4" e ayni sorular sorulur. 4<8 sola gec, 4<7 sola gec, 4<5 sola gec, 4>1 "1" in sagina gec. orda "3" var 4>3 oldugundan "4" "3" ün sagina gecer, baska sayi kalmadigi icin orda kal.
                          8
                        7   9
                    5       
                 1    6
              0    3
                     4
En son olarak "2y" e ayni sorular sorulur. 2<8 sola gec, 2<7 sola gec, 2<5 sola gec, 2>1 "1" in sagina gec. orda "3" var 2<3 oldugundan "2" "3" ün soluna gecer, baska sayi kalmadigi icin orda kal.
                          8
                        7   9
                    5       
                 1    6
              0    3
                 2   4
[www.patika.dev](https://www.patika.dev/)
