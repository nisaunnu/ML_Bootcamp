# Sıralama Algoritmaları

<br>

### İçerik
1. [Bubble Sort (Kabarcık Sıralama)](#1-bubble-sort-kabarcık-sıralama)
2. [Selection Sort (Seçmeli Sıralama)](#2-selection-sort-seçmeli-sıralama)
3. [Insertion Sort (Eklemeli Sıralama)](#3-insertion-sort-eklemeli-sıralama)
4. [Quick Sort (Hızlı Sıralama)](#4-quick-sort-hızlı-sıralama)
5. [Merge Sort (Birleştirme Sıralaması)](#5-merge-sort-birleştirme-sıralaması)
6. [Heap Sort (Hızlı Seçim Sıralaması)](#6-heap-sort-hızlı-seçim-sıralaması)
7. [Counting Sort (Sayma Sıralaması)](#7-counting-sort-sayma-sıralaması)
8. [Radix Sort (Radyal Sıralama)](#8-radix-sort-radyal-sıralama)
9. [Topological Sort (Topolojik Sıralama)](#9-topological-sort-topolojik-sıralama)

<br>

### 1. Bubble Sort (Kabarcık Sıralama)

* En basit sıralama algoritmasıdır.
* İki elemanı kıyaslayarak sıralama yapar ve gerektiğinde yer değiştirir.
* Ardışık karşılaştırmalar yaparken ve yer değiştirme sıralamalarında kullanılır.
* En büyük eleman yavaşça "kabarcıklar" ve en üstte kalır.
* En kötü durumda O(n^2), en iyi duruda O(n) zaman karmaşıklığına (Big O-nation) sahiptir.
* Büyük veri setlerinde verimli değildir.
* Örnek: çalma listesindeki müzikleri sıralamak.
<br>

### 2. Selection Sort (Seçmeli Sıralama)

* Bir veri setindeki en büyük veya en küçük elemanı seçip sıralama yapar. Listenin en küçük elemanını bulur ve listenin başına koyar.
* İlk eleman sıralanmış kabul edilir ve işlem tekrarlanır.
* Veri setini ikiye bölen bir algoritmadır.
* Büyük veri setlerinde mantıklı bir yaklaşım değildir.
* En kötü ve en iyi durumda O(n^2) zaman karmaşıklığına sahiptir.
* Örnek: gezegenlerin atmosfer basınçlarını sıralamak, sporcuların sıralanması, sınav notlarının sıralanması.
<br>

### 3. Insertion Sort (Eklemeli Sıralama)

* Veri setini sıralı veya sırasız bölgelere ayırır.
* Sırasız bölgeden bir elemanı alır, sıralı bölgede uygun konuma yerleştirir. Bu işlem veri seti tamamen bitene kadar devam eder.
* En iyi durumda O(n), en kötü durumda O(n^2) zaman karmaşıklığına sahiptir.
* Örnek: astronotların eipmanlarının sıralanması
<br>

### 4. Quick Sort (Hızlı Sıralama)

* Bir pivot eleman kullanarak veri setini ikiye böler.
* Pivot elemanın sol tarafı pivot elemandan küçük; sağ tarafı pivot elemandan büyük elemanlardan oluşur. Daha sonra bu işlemi her iki bölge için tekrar eder.
* Ortalama durumda O(n log n), en kötü durumda O(n^2) zaman karmaşıklığına sahiptir.
* Örnek: uzay teleskoplarından gelen verileri (parlaklık, uzaklık, büyüklük vb.) sıralamak, iş başvurusunda bulunan adayların seçimi (standart bir aday pivot olarak seçilir ve pivota göre üst veya alt olarak değerlendirilir).
<br>

### 5. Merge Sort (Birleştirme Sıralaması)

* Veriyi sürekli olarak ikiye böler. İki yarıyı da ayrı ayrı sıralar. Sonra birleştirme yapar.
* Birleştirme aşamasında iki alt liste sıralı bir şekilde birleştirilir.
* Bundan dolayı büyük veri setlerinde oldukça etkili bir yöntemdir.
* Bölme ve birleştirme işlemlerinde zaman karmaşıklığı (Big O-nation) kullanır. Her durumda O(n log n) zaman karmaşıklığına sahiptir.
* Örnek: yıldız sisteminin veya galaksinin daha eksiksiz bilgi edinmek veya resim oluşturmak için farklı teleskoplardaki verileri birleştirmek, farklı bölümlerdeki çalışanların listelenmesi.
<br>

### 6. Heap Sort (Hızlı Seçim Sıralaması)

* Bir dizi üzerinde heap (yığın) veri yapısı oluşturulur. Bir maksimum yığın (heap) veri yapısını kullanarak sıralar.
* Maksimum elemanı kökten alır ve kökü yeniden düzenler.
* Sıralama işlemi bu heap üzerinden yapılır.
* Büyük veri setlerinde zaman karmaşıklığı hafızada daha az yer kapladığı için daha efektif bir yaklaşım haline gelir.
* En iyi ve en kötü durumda O(nlogn) zaman karmaşıklığına sahiptir.
* Örnek: gezegen yüzeyinden madde madenciliği yapmak (değerli madenlere göre sıralamak).
<br>

### 7. Counting Sort (Sayma Sıralaması)

* Veri setinin aralığı dikkate alınır.
* Her bir elemanın kaç kez göründüğünü sayarak sıralama yapar (Elemanların frekanslarını sayarak sıralar).
* Pozitif tam sayılar için etkilidir.
* O(n+k) karmaşıklığına sahiptir (k, maksimum eleman değeridir).
* Örnek: uzay mekiklerinin kaçış hızlarının sıralanması, yaş grupları, sınıftaki kız ve erkeklerin sayısı.
<br>

### 8. Radix Sort (Radyal Sıralama)

* Elemanlar basamaklarına göre sıralanır ve elemanlar sayısal olarak temsil edilmelidir.
* Rakamlara göre sıralar, en az önemli rakamdan en çok önemli rakama doğru.
* Sayısal veriler için kullanılır.
* Pozitif tamsayılarda sıralama işlemlerinde etkilidir.
* Her durumda O(nk) karmaşıklığına sahiptir (k, rakam sayısıdır).
* Örnek: gezegenlerin yörünge önceliklerine (birincil, ikincil vb.) göre incelenmesi ve bu duruma göre yolculuk yapılması, üç farklı bankadan kredi çekildiğinde ödeme sırası olarak en çok faizi olanın seçilmesi.
<br>

### 9. Topological Sort (Topolojik Sıralama)

* Yönlendirilmiş ayrık grafikler üzerinde kullanılır.
* Grafik içindeki düğümlerin bağımlılık sırasına göre sıralama yapılır.
* Her düğüm, bağlı düğümlerden önce gelmelidir.
* Genellikle iş akışlarını, bağımlılıkları ve proje sıralamalarını modellemek için kullanılır.
* Örnek: bir görevin iş zamanlaması, devre analizi, uçak rotaları, sosyal medyada reklam verilecek hesabın belirlenmesi.
<br>
