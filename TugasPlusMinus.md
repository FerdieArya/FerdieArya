<h1>Tugas Plus Minus</h1>
Nama: Ferdie Arya Jantanu<br>
Kelas: TIF22A<br>
NIM: 23422057
<h1>Tugas</h1>
Selesaikan Tantangan yang ada dilink berikut (https://www.hackerrank.com/challenges/plus-minus/problem). Tantangan tersebut berupa membuat Codingan untuk menghitung proporsi elemen positif, negatif, nol dalam array. Cetak nilai desimal dari setiap pecahan pada baris baru minimal 6 tempat setelah nilai desimal. hasil output harus sesuai dengan sampel hasil output yakni:
<br><br>Kasus 1

```
0.500000
0.333333
0.166667
```
Kasus 2
```
0.375000
0.375000
0.250000
```
<h1>Jawaban</h1>
Untuk tugas kali saya menggunakan bahasa phython 3. berikut adalah kodingan yang saya buat beserta hasil inputnya :

```
#!/bin/python3

import math
import os
import random
import re
import sys

# Complete the plusMinus function below.
def plusMinus(arr):
    x,z,y=0,0,0
    for i in range(0,len(arr)):
        if arr[i]>0:
            x = x + 1
        elif arr[i]<0:
            y = y + 1
        else:
            z = z + 1
    print("{:.6f}".format(x/len(arr)))
    print("{:.6f}".format(y/len(arr)))
    print("{:.6f}".format(z/len(arr)))

if __name__ == '__main__':
    n = int(input())

    arr = list(map(int, input().rstrip().split()))

    plusMinus(arr)
```

Kasus 1<br>
Sampel Input:
```
6
-4 3 -9 0 4 1
```
Output yang diharapkan:
```
0.500000
0.333333
0.166667
```
Output dari kode saya:
```
0.500000
0.333333
0.166667
```

Kasus 2<br>
Sampel Input:
```
8
1 2 3 -1 -2 -3 0 0
```
Output yang diharapkan:
```
0.375000
0.375000
0.250000
```
Output dari kode saya:
```
0.375000
0.375000
0.250000
```
