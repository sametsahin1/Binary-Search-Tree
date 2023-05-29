# Binary-Search-Tree
Binary Search Tree (BST), bir ağaç veri yapısıdır ve özel bir özelliği vardır: Bir düğümün değeri, sol alt ağacındaki tüm düğümlerin değerlerinden büyük ve sağ alt ağacındaki tüm düğümlerin değerlerinden küçüktür.

Verilen diziyi BST'ye dönüştürme adımları genellikle aşağıdaki gibidir:

Verilen dizi: [7, 5, 1, 8, 3, 6, 0, 9, 4, 2]

İlk eleman (7), ağacın kökü olarak atanır.
Her bir sonraki eleman, şu kurala göre ağaca eklenir: Eğer eklenen eleman mevcut düğümün değerinden küçükse, bu eleman o düğümün sol alt ağacına eklenir. Eğer eklenen eleman mevcut düğümün değerinden büyükse, bu eleman o düğümün sağ alt ağacına eklenir.
Bu kurallara göre, BST'nin oluşturulma adımları aşağıdaki gibi olacaktır:

İlk elemanı ağacın kökü olarak atarız: 7
5, 7'den küçük olduğu için 7'nin soluna eklenir.
1, 7 ve 5'ten küçük olduğu için 5'in soluna eklenir.
8, 7'den büyük olduğu için 7'nin sağına eklenir.
3, 7 ve 5'ten küçük ancak 1'den büyük olduğu için 1'in sağına eklenir.
6, 7'den küçük ancak 5'ten büyük olduğu için 5'in sağına eklenir.
0, 7, 5 ve 1'den küçük olduğu için 1'in soluna eklenir.
9, 7 ve 8'den büyük olduğu için 8'in sağına eklenir.
4, 7 ve 5'ten küçük ancak 3'ten büyük olduğu için 3'ün sağına eklenir.
2, 7, 5 ve 3'ten küçük ancak 1'den büyük olduğu için 1'in sağına eklenir ancak 1'in sağında zaten bir düğüm (3) var. Bu durumda, 2, 3'ten küçük olduğu için 3'ün soluna eklenir.
Sonuç olarak ağaç yapısı aşağıdaki gibi olacaktır:

            7
           / \
          5   8
         / \   \
        1   6   9
       / \   \
      0   3   4
           \
            2

