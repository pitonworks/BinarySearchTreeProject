﻿# BinarySearchTreeProject
Binary Search Tree (BST) oluşturma süreci, verilen diziyi adım adım BST'ye dönüştürme işlemini içerir. BST'nin temel kuralları gereği, her düğümün solundaki tüm elemanlar kendisinden küçük, sağındaki tüm elemanlar ise kendisinden büyük olmalıdır. Dizi sırasıyla elemanları ekleyerek BST'yi oluşturacağız.

Dizi: [7, 5, 1, 8, 3, 6, 0, 9, 4, 2]

BST Oluşturma Aşamaları
Başlangıç:

İlk eleman, kök (root) olarak kabul edilir.
Kök: 7
markdown
Copy code
    7
İkinci Eleman (5):

5, 7'den küçük olduğu için 7'nin soluna eklenir.
Kök: 7
Sol: 5
markdown
Copy code
    7
   /
  5
Üçüncü Eleman (1):

1, 7'den küçük olduğu için 7'nin soluna eklenir.
1, 5'ten de küçük olduğu için 5'in soluna eklenir.
Kök: 7
Sol: 5
Sol: 1
markdown
Copy code
    7
   /
  5
 /
1
Dördüncü Eleman (8):

8, 7'den büyük olduğu için 7'nin sağına eklenir.
Kök: 7
Sol: 5
Sol: 1
Sağ: 8
markdown
Copy code
    7
   / \
  5   8
 /
1
Beşinci Eleman (3):

3, 7'den küçük olduğu için 7'nin soluna eklenir.
3, 5'ten küçük olduğu için 5'in soluna eklenir.
3, 1'den büyük olduğu için 1'in sağında yer alır.
Kök: 7
Sol: 5
Sol: 1
Sağ: 3
Sağ: 8
markdown
Copy code
    7
   / \
  5   8
 /
1
 \
  3
Altıncı Eleman (6):

6, 7'den küçük olduğu için 7'nin soluna eklenir.
6, 5'ten büyük olduğu için 5'in sağına eklenir.
Kök: 7
Sol: 5
Sol: 1
Sağ: 3
Sağ: 6
Sağ: 8
markdown
Copy code
    7
   / \
  5   8
 / \
1   6
 \
  3
Yedinci Eleman (0):

0, 7'den küçük olduğu için 7'nin soluna eklenir.
0, 5'ten küçük olduğu için 5'in soluna eklenir.
0, 1'den küçük olduğu için 1'in soluna eklenir.
Kök: 7
Sol: 5
Sol: 1
Sol: 0
Sağ: 3
Sağ: 6
Sağ: 8
markdown
Copy code
    7
   / \
  5   8
 / \
1   6
/
0 3

markdown
Copy code

8. **Sekizinci Eleman (9):**
- 9, 7'den büyük olduğu için 7'nin sağına eklenir.
- 9, 8'den büyük olduğu için 8'in sağına eklenir.
- **Kök:** 7
  - Sol: 5
    - Sol: 1
      - Sol: 0
      - Sağ: 3
    - Sağ: 6
  - Sağ: 8
    - Sağ: 9

Copy code
   7
  / \
 5   8
/ \   \
1 6 9
/
0 3

markdown
Copy code

9. **Dokuzuncu Eleman (4):**
- 4, 7'den küçük olduğu için 7'nin soluna eklenir.
- 4, 5'ten küçük olduğu için 5'in soluna eklenir.
- 4, 1'den büyük olduğu için 1'in sağında yer alır.
- 4, 3'ten büyük olduğu için 3'ün sağında yer alır.
- **Kök:** 7
  - Sol: 5
    - Sol: 1
      - Sol: 0
      - Sağ: 3
        - Sağ: 4
    - Sağ: 6
  - Sağ: 8
    - Sağ: 9

Copy code
   7
  / \
 5   8
/ \   \
1 6 9
/
0 3
4

markdown
Copy code

### Özet

- **Kök (root):** 7
- **Kökün sağında:** 8 (ve sağında 9)
- **Kökün solunda:** 5
- **5'in sağında:** 6
- **5'in solunda:** 1
 - **1'in sağında:** 3
   - **3'ün sağında:** 4
 - **1'in solunda:** 0


