# Patika Merge Sort Projesi - Proje 2
##### Bu repo [Patika](http://www.patika.dev) sitesi Veri Yapıları ve Algoritmalar dersi Projeler bölümünde bulunan Merge Sort Projesi - Proje 2 çalışması için oluşturulmuştur.

[16,21,11,8,12,22] dizinin sort türüne göre aşamalarını yazınız. 


- Öncelikle dizi ikiye bölünür. Bölme işlemi dizide tek eleman kalana dek bölünmeye devam eder.

Diziyi ikiye bölerek yeniden yazıyoruz

#### Adım 1

|16|21|11|8|12|22|
| :---: | :---: | :---: |:---: | :---: | :---: |
- Dizinin orta noktası bulunur.

#### Adım 2

|16|21|11| |<->| |8|12|22|
| :---: | :---: | :---: |:---: | :---: | :---: |:---: | :---: | :---: |
- Dizi orta noktasından ikiye bölünür.



#### Adım 3
|16|21|<->  |11|  | |8|<->  |12|22|
| :---: | :---: | :---: |:---: | :---: | :---: |:---: | :---: | :---: |:---: | 
- İkiye bölünen dizi tekrardan ikiye bölünür.


#### Adım 4
|16|  |21|  |11|  |8|  |12|  |22|
| :---: | :---: | :---: |:---: | :---: | :---: |:---: | :---: | :---: |:---: | :---: |
- Dizi elemanları tek tek ayrılmıştır. Dizi bu işlemden sonra elemanlarını ikişerli olarak birleştirmeye başlar.

#### Adım 5
|16|21|  |11|  |  |8|  |12|22|
| :---: | :---: | :---: |:---: | :---: | :---: |:---: | :---: | :---: |:---: |
- Elemanlar ikişerli olarak birleştirilir ve küçükten büyüğe doğru sıralanır.

#### Adım 6
|11|16|21|  |  |8 |12|22|
| :---: | :---: | :---: |:---: | :---: | :---: |:---: | :---: |
- Elemanlar tekrardan ikişerli olarak birleştirilir ve küçükten büyüğe doğru sıralanır.

#### Adım 7
|8 |11|12|16|21|22|
| :---: | :---: | :---: |:---: | :---: | :---: |
- Dizideki tüm elemanlar birleştirilmiş ve küçükten büyüğe doğru sıralanmış olarak dizinin son halini alır.
    

#### 2. Big-O gösterimini yazınız.
Recursive fonksiyon olduğundan dolayı kendisini çağırır ve diziyi sürekli olarak ikiye böler. Bölünen dizinin birleştirme işlemi yapılır.

```
O(nLogn)
```
