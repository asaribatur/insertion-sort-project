# Proje 1: Insertion Sort

[Proje linki](https://app.patika.dev/courses/veri-yapilari-ve-algoritmalar/insertion-sort-proje)

### **A)**  **Verilen dizi:** **[22,27,16,2,18,6]**

  

#### 1) İşlem Adımları:

-   İlk elemandan sonra sıralanmış kısım için bir işaretçi yerleştir. Bu işaretçi sol taraftaki sıralı alt diziyi sağ taraftaki sıralı olmayan alt diziden ayıracak.
    
-   Insertion sort’ta başlangıçta dizinin ilk iki elemanı karşılaştırılır:
    

  

**22** **|** **27 16 2 18 6**

-   Burada, 22 27’den küçüktür. Yani artan sıradadır ve iki elemanın konumu doğrudur. Bu elemanlar sıralı alt diziye eklenir.
    

  

**22 27** **|** **16 2 18 6**

  

-   Şimdi sonraki iki elemana geç ve onları karşılaştır:
    

**22 27** **|** **16 2 18 6**

-   Burada 16 27’den küçüktür. Dolayısıyla bu ikisinin yer değiştirmesi gerekir:
    

**22 16 27 2 18 6**

  

-   **Bu haliyle de 16 22’den küçük. Bu ikisini de takas edelim:**
    

**16 22 27 2 18 6**

  

-   **Solda eleman kalmadığı için tekrar işaretçiyi yerleştirebiliriz:**
    

**16 22 27** **|** **2 18 6**

  

-   **Şimdi sonraki iki elemana** **(27 ile 2)** **geç ve onları karşılaştır:**
    

-   Burada 2 27’den küçük. Takas edelim:
    

**16 22 2 2****7** **18 6**

  

-   2 22’den küçük..
    

**16 2 2****2** **2****7** **18 6**

  

-   ve 16’dan da..
    

**2**  **16** **2****2** **2****7** **18 6**

  

-   **Solda eleman kalmadığı için tekrar işaretçiyi yerleştirebiliriz:**
    

**2 16 22 2****7** **|** **18 6**

  

-   **Şimdi sonraki iki elemana** **(27 ile 18)** **geç ve onları karşılaştır:**
    

  

-   Burada 18 27’den küçük. Takas edelim:
    

**2**  **16** **2****2** **18** **2****7** **6**

  

-   18 22’den küçük..
    

**2**  **16**  **18** **2****2** **2****7** **6**

-   **ama 16’dan büyük. Sıralı alt dizimiz güncellendi. İşaretçiyi yerleştirelim:**
    

**2**  **16**  **18** **2****2** **2****7** **|** **6**

  

-   **Şimdi sırasız alt dizide kalan son eleman (6) için de aynı işlemleri yapalım.**
    
-   **27 ile 6’yı karşılaştır. 6 27’den küçük olduğundan ikisini takas et:**
    
    **2**  **16**  **18** **2****2**  **6** **2****7**
    
-   **6 22’den küçük..**
    
    **2**  **16**  **18**  **6** **22**  **2****7**
    
-   **18’den de..**
    
    **2**  **16**  **6** **18**  **22**  **2****7**
    

  

-   Hatta 16’dan da..
    
    **2**  **6**  **16** **18**  **22**  **2****7**
    

  

-   **Ancak 2’den büyük. Burda takas yok. Daha fazla kaydırma yapmamıza gerek yok. İşaretçiyi bir eleman daha kaydıralım:**
    

**2**  **6**  **16** **18**  **22**  **2****7** **|**

  

Nihayet işaretçi dizinin sonuna ulaştı. Bunun anlamı sağdaki sırasız alt dizideki tüm elemanlar soldaki sıralı alt diziye eklendi. Yani sıralama işlemi sona erdi. Artık sıralı bir listemiz var! :)

**2**  **6**  **16** **18**  **22**  **2****7**

  

  

#### 2) Big-O Gösterimi

-   En iyi durum (Best case) : O(n)
    
-   Ortalama durum (average case) : O(n2)
    
-   En kötü durum (worst case) : O(n2)
    

  

  

#### 3) Time Complexity

-   Average case: Aradığımız sayının ortada olması
    

  

-   Worst case: Aradığımız sayının sonda olması,
    
-   Best case: Aradığımız sayının dizinin en başında olması.
    


#### 4) Dizi sıralandıktan sonra 18 sayısı hangi case kapsamına girer?

**Cevap:** Average case

  

 

### B) **[7,3,5,8,2,9,4,15,6**] dizisinin Insertion Sort'a göre ilk 4 adımını yazınız.

  

**1) 3**  **7** **5 8 2 9 4 15 6**

**2) 3**  **5**  **7** **8 2 9 4 15 6**

**3) 3**  **5**  **7** **8 2 9 4 15 6** **(değişiklik yok)**

**4) 3**  **5**  **7**  **2**  **8** **9 4 15 6**
