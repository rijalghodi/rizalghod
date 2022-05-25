---
{"dg-publish":true,"permalink":"/tutorial-obsidian/","tags":"gardenEntry","dgHomeLink":true,"dgPassFrontmatter":false}
---

# Tutorial Obsidian DataView

category:: selfImprovement
tanggal:: 24 May 2022

## Anotasi Data
Menyimpan data dengan atribut tertentu. Ada dua cara:
1. Dengan metadata seperti di atas (source, youtuber, note, link)
2. Menggunakan dua titik dua :: atau tag langsung (khusus tag) **seperti** pada atribut category dan tanggal



#### JikA aku menjadi 

## Querying Data
Mengambil data dari anotasi data. Caranya:
### TABLE
```dataview
	TABLE asal, email
	WHERE type = "person"
```
Gunakan keyword <mark style="background: #FFF3A3A6;">TABLE, FROM, WHERE, SORT</mark> 
```dataview
TABLE asal as "Kota", email as "Email" FROM "Others/Free Notes"
WHERE type = "person" and tag = "DTM"
SORT file.name asc

```
### LIST
```dataview
LIST noHp
WHERE type = "person"
SORT file.name desc
```
### TASK
```dataview
TASK
WHERE type = "person"
```

