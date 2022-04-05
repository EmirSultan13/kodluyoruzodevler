## Insertion Sort Algoritma Ödevi
[22,27,16,2,18,6]
Soru:
1.  Yukarı verilen dizinin sort türüne göre aşamalarını yazınız.
2.  Big-O gösterimini yazınız.
3.  Time Complexity: Average case: Aradığımız sayının ortada olması,Worst case: Aradığımız sayının sonda olması, Best case: Aradığımız sayının dizinin en başında olması.
4.  Dizi sıralandıktan sonra 18 sayısı hangi case kapsamına girer? Yazınız.

Cevap 1:

	 A. Insertion Sort:
1. | 22 | 27 | 16 | 2 | 18 | 6 | --- 22, 27'den küçük olduğu için yer değiştirmezler.
2. | **16** | 22 | 27 | 2 | 18 | 6 | --- 16 numarası 22 ve 27 ile karşılaştırıldığında en küçük olduğu için en sola alınır.
3. | **2** | 16 | 22 | 27 | 18 | 6 | --- 2 numarası 27,22 ve 16 ile karşılaştırıldığında en küçük olduğu için en sola alınır.
4. | 2 | 16 | **18** | 22 | 27 | 6 | --- 18 numarası 27 ve 22  ile karşılaştırıldığında en küçük olduğu için bu iki sayının soluna alınır.
5. | 2 | **6** | 16 | 18 | 22 | 27 | --- 6 numarası 27,22,18 ve 16 ile karşılaştırıldığında en küçük olduğu için bu üç sayının en soluna alınır.

	|2|6|16|18|22|27| Son durum.
 
Cevap 2:
n+(n-1)+(n-2)+(n-3)+...+1 
= n x (n+1) / 2 
= (n^2+n) / 2 = Big o değeri en büyük n olduğundan dolayı buradaki değerimiz n ^2'dir.

	Big O gösterimi: O(n^2)
Cevap 3:
Avarage Case: 16 numarası bu örnekteki avarage case olarak zaten ortada olduğundan sadece bir adım sola geçmiştir.

	Big O gösterimi: o(n^2)  

Worst Case: 6 numarası hem en küçük sayı hem de en sağda olması bu örnekte worst case olarak göze çarpmaktadır.

	Big O gösterimi: o(n^2) 
Best Case: 22 numarası hiç işlem görmediği için bu örnekte best case olarak göze çarpmaktadır. 
	
	Big O gösterimi: o(n) 

Cevap:4 

18 sayısı diğer numaralara göre hem orta büyüklükte hem de sıra olarak da ortalarda yer aldığından dolayı avarage case kapsamına girer.

[7,3,5,8,2,9,4,15,6] dizisinin Insertion Sort'a göre ilk 4 adımını yazınız.

| 7 | 3 | 5 | 8 | 2 | 9 | 4 | 15 | 6 |
1. | **3** | 7| 5 | 8 | 2 | 9 | 4 | 15 | 6 |  --- 7 ile 3 karşılaştırılır. 3 sola alınır.
2. | 3 | **5** | 7 | 8 | 2 | 9 | 4 | 15 | 6 | --- 5 ile 7 ve 3 karşılaştırılır. 7'nin soluna alınır.
3. | 3 | 5 | 7 | **8** | 2 | 9 | 4 | 15 | 6 | --- 8 ile solundaki sayılar karşılaştırılır. 8 sabit kalır.
4. | **2** | 3 | 5 | 7 | 8 | 9 | 4 | 15 | 6 | --- 2 ile solundaki sayılar karşılaştırılır. En sola alınır.

## Merge Sort Algoritma Ödevi
 [16,21,11,8,12,22]
 Soru: 
 1. Yukarıdaki dizinin sort türüne göre aşamalarını yazınız.
 2. Big-O gösterimini yazınız.
 
 Cevap:
```

	    [16, 21, 11, 8, 12, 22]
	        /             \
	  [16, 21, 11]     [8, 12, 22]
	      /   \           /   \
	  [16, 21] [11]   [8, 12] [22]
	    /  \     |      /  \    |
	 [16] [21]  [11]  [8] [12] [22]
	   \    /    |     \   /    |
	  [16, 21]  [11]  [8, 12]  [22]
	     \       /       \      /    
	   [11, 16, 21]    [8, 12, 22]
	         \             /
	      [8, 11, 12, 16, 21, 22 ]
```
```
O(nlogn)
```

## Binary Search Tree Ödevi
[7,5,1,8,3,6,0,9,4,2]

Soru: Yukarıdaki dizinin Binary Search Tree aşamalarını yazınız.

Cevap: 
		
    7,5,1,8,3,6,0,9,4,2 
    0,1,2,3,4,5,6,7,8,9 Root:5
                  5
                 /  \
                2     7
               / \   /  \
              1   3 6     8
             /              \
            0                 9
		
