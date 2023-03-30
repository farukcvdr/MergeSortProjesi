# Merge Sort Projesi

## Problem

Proje 2
[16,21,11,8,12,22] -> Merge Sort

Yukarıdaki dizinin sort türüne göre aşamalarını yazınız.
Big-O gösterimini yazınız.

## Çözüm

[16,21,11,8,12,22] -> Merge Sort

1. Diziyi ikiye bölerek yeniden yazarız.

16,21,11      ve        8,12,22

2. Şimdi sol ve sağdaki dizileri tekrar ikiye böleriz.

16,21  –   11       ve    8,12   –  22

3. şimdi tek eleman kalana kadar bir kez daha bölüyoruz.

16 –  21  –   11  –  8  –   12  –  22  oluyor.

4. şimdi ikili ikili sıralayarak birleştiriyoruz.

16,21  –  8-11   –   12,22   

5. şimdi bu ikilileri birleştiriyoruz.

8,11,16,21    –     12,22

6. şimdi bu son dizileri birleştiriyoruz ve sıralanmış dizimizi elde ediyoruz.

8,11,12,16,21,22 

### Big-O Gösterimi

Recursive bir fonksiyon olduğu için sürekli kendini çağırarak diziyi hep ikiye bölmektedir. Her bölünmüş dizinin Merge işlemi için de dizinin uzunluğu olan N işlem yapıldığından **O(n*logn)** olacaktır.