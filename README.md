# Python-Temel-Proje

patika.dev -> https://app.patika.dev/cataldirect

1 -  Bir listeyi düzleştiren (flatten) fonksiyon yazın. Elemanları birden çok katmanlı listelerden ([[3],2] gibi) oluşabileceği gibi, non-scalar verilerden de oluşabilir. Örnek olarak:

input: [[1,'a',['cat'],2],[[[3]],'dog'],4,5]

output: [1,'a','cat',2,3,'dog',4,5]

CEVAP:

    l = [[1,'a',['cat'],2],[[[3]],'dog'],4,5]
    lnew = []
    def flatten(n):
        for i in n:
          if isinstance(i, list):
            flatten(i)
          else:
            lnew.append(i)

    flatten(l)
    print(lnew)


2 - Verilen listenin içindeki elemanları tersine döndüren bir fonksiyon yazın. Eğer listenin içindeki elemanlar da liste içeriyorsa onların elemanlarını da tersine döndürün. Örnek olarak:

input: [[1, 2], [3, 4], [5, 6, 7]]

output: [[[7, 6, 5], [4, 3], [2, 1]]

CEVAP:

    l =[[1, 2], [3, 4], [5, 6, 7]]
    l=l[::-1]
    for i in range(len(l)):
      (l[i])=(l[i])[::-1]
    print(l)
    
# NOT: Tüm cevaplar tamamen alıntıdır. 
