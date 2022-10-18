# Veri Yapilari ve Algoritmalar Kursu Bitirme Projesi

## Binary-Search-Tree Projesi

Proje 3

1. [7, 5, 1, 8, 3, 6, 0, 9, 4, 2] dizisinin Binary-Search-Tree aşamalarını yazınız?

Örnek: root x'dir. root'un sağından y bulunur. Solunda z bulunur vb.

## CEVAP
Big-O= Average case de O(logn), Worst case de O(n). Random accessi yoktur.

Binary-Search-Tree ile arama islemlerine baslanirken bir root belirlenir ve her seferinde elimizdeki sayiya bu sayidan büyük mü kücük mü diye sorulur ve büyükse sag tarfa kücükse sol tarafa yazilir. Örnegin Root sayimiz "8" olsun.  En basa "8" yazilir. Sonra "7" sayisini aliriz ve sorariz "8"den büyuksen saga gec kücüksen sola gec. Kücük oldugu icin sola gecer.
                          8
                      7
daha sonra 5 sayisina ayni soruyu sorariz ve "8" den kücük oldugu icin sola gecer. Solda "7" sayisi oldugu icin bu sefer de "5" sayisini "7" sayisi ile karsilastiririz ve 5<7 oldugu icin "5" sayisini "7 nin soluna ekleriz.
                     
"1" e de ayni sorular sorulur 1<8 sola gec, 1<7 sola gec, 1<5 sola gec ve en sola gecer, baska sayi kalmadigi icin orda kal.
                
Sonra "3" e ayni sorular sorulur. 3<8 sola gec, 3<7 sola gec, 3<5 sola gec, 3>1 "1" in sagina gec, baska sayi kalmadigi icin orda kal.
                           8
                        7
                    5       
                 1 
                    3
Sonra "6" ya ayni sorular sorulur. 6<8 sola gec, 6<7 sola gec, 6>5 "7" in sagina gec, baska sayi kalmadigi icin orda kal.
      
Sonra "0" a ayni sorular sorulur. 0<8 sola gec, 0<7 sola gec, 0<5 sola gec, 0<1 sola gec ve en sola gecer, baska sayi kalmadigi icin orda kal.     
Sonra "9" a ayni sorular sorulur. 9>8 saga gec ve en saga gecer, baska sayi kalmadigi icin orda kal.        
Sonra "4" e ayni sorular sorulur. 4<8 sola gec, 4<7 sola gec, 4<5 sola gec, 4>1 "1" in sagina gec. orda "3" var 4>3 oldugundan "4" "3" ün sagina gecer, baska sayi kalmadigi icin orda kal.
           
En son olarak "2y" e ayni sorular sorulur. 2<8 sola gec, 2<7 sola gec, 2<5 sola gec, 2>1 "1" in sagina gec. orda "3" var 2<3 oldugundan "2" "3" ün soluna gecer, baska sayi kalmadigi icin orda kal. Boylece search islemi biter. Eleman eklemek veya cikarmak istersek de ayni sorulari sorarak ilerleriz ve aradigimiz elemani bulup islemi yapariz.
                          8
                        7   9
                    5       
                 1    6
              0    3
                 2   4
![Proje Görseli]("C:\Users\yilma\OneDrive\Documents\VS Code\Project 1\kodluyoruzilkrepo\BinarySearchTreeProjesi.png")
[www.patika.dev](https://www.patika.dev/)
