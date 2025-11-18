Tamam, **en basit şekilde** anlatıyorum. Çok kısa, çok anlaşılır ve örnekli. 👇

---

# ⭐ HTML’de tablo nasıl yapılır? (Basit Anlatım)

HTML’de tablo yapmak için 3 şey bilmen yeterli:

### 1️⃣ `<table>` → Tabloyu başlatır

### 2️⃣ `<tr>` → Satır oluşturur

### 3️⃣ `<td>` → Hücre (kutucuk) oluşturur

Hepsi bu kadar!

---

# ⭐ En basit tablo örneği

### Kod:

```html
<table border="1">
    <tr>
        <td>Ali</td>
        <td>20</td>
    </tr>
</table>
```

### Çıktı:

| Ali | 20 |

---

# ⭐ Biraz daha büyük tablo

### Kod:

```html
<table border="1">
    <tr>
        <td>Ad</td>
        <td>Yaş</td>
    </tr>

    <tr>
        <td>Ali</td>
        <td>20</td>
    </tr>

    <tr>
        <td>Ayşe</td>
        <td>19</td>
    </tr>
</table>
```

### Çıktı:

| Ad   | Yaş |
| ---- | --- |
| Ali  | 20  |
| Ayşe | 19  |

---

# ⭐ Başlık eklemek istersen `<th>`

### Kod:

```html
<table border="1">
    <tr>
        <th>Ad</th>
        <th>Yaş</th>
    </tr>

    <tr>
        <td>Ali</td>
        <td>20</td>
    </tr>
</table>
```

### Çıktı:

| **Ad** | **Yaş** |
| ------ | ------- |
| Ali    | 20      |

---

# ⭐ Özet (kısacık)

* `<table>` = tablo
* `<tr>` = satır
* `<td>` = hücre
* `<th>` = başlık hücresi

Tamam! Sana **hiç HTML bilmeyen biri için**, **kolaydan zora doğru** tablo anlatacağım.
Her adım bir öncekinden biraz daha zor olacak.
Her adımda **kod + çıktı** da olacak.

Hazırsan başlıyoruz. 👇

---

# 🟢 **1. Adım — Tablo nedir? (En temel anlatım)**

Tablo, kutucuklardan oluşan bir yapıdır.

HTML’de tablo yapmak için 3 komut bilmen yeterli:

* `<table>` → tabloyu açar
* `<tr>` → bir satır oluşturur
* `<td>` → satır içindeki hücre (kutucuk)

---

# 🟢 **2. Adım — İlk tabelon (en basit)**

### Kod:

```html
<table border="1">
    <tr>
        <td>Ali</td>
        <td>20</td>
    </tr>
</table>
```

### Çıktı:

| Ali | 20 |

Bu kadar! 1 satır + 2 hücreli küçük bir tablo.

---

# 🟢 **3. Adım — 2 satırlı tablo**

### Kod:

```html
<table border="1">
    <tr>
        <td>Ad</td>
        <td>Yaş</td>
    </tr>

    <tr>
        <td>Ali</td>
        <td>20</td>
    </tr>
</table>
```

### Çıktı:

| Ad  | Yaş |
| --- | --- |
| Ali | 20  |

---

# 🟡 **4. Adım — 3 satırlı tablo**

### Kod:

```html
<table border="1">
    <tr>
        <td>Ad</td>
        <td>Yaş</td>
    </tr>

    <tr>
        <td>Ali</td>
        <td>20</td>
    </tr>

    <tr>
        <td>Ayşe</td>
        <td>19</td>
    </tr>
</table>
```

### Çıktı:

| Ad   | Yaş |
| ---- | --- |
| Ali  | 20  |
| Ayşe | 19  |

---

# 🟡 **5. Adım — Başlık eklemek (th kullanımı)**

Tablonun başlığını `<th>` ile yaparsın (kalın görünür).

### Kod:

```html
<table border="1">
    <tr>
        <th>Ad</th>
        <th>Yaş</th>
    </tr>

    <tr>
        <td>Ali</td>
        <td>20</td>
    </tr>
</table>
```

### Çıktı:

| **Ad** | **Yaş** |
| ------ | ------- |
| Ali    | 20      |

---

# 🟡 **6. Adım — Tüm tabloya başlık eklemek (caption)**

### Kod:

```html
<table border="1">
    <caption>Öğrenci Listesi</caption>

    <tr>
        <th>Ad</th>
        <th>Yaş</th>
    </tr>

    <tr>
        <td>Ali</td>
        <td>20</td>
    </tr>
</table>
```

### Çıktı:

Öğrenci Listesi

| Ad  | Yaş |
| --- | --- |
| Ali | 20  |

---

# 🔵 **7. Adım — Hücreleri birleştirmek (colspan)**

Bir hücrenin **yan yana iki sütunu kaplamasını** istiyorsan:

### Kod:

```html
<table border="1">
    <tr>
        <th colspan="2">Bilgi</th>
    </tr>

    <tr>
        <td>Ad</td>
        <td>Ali</td>
    </tr>
</table>
```

### Çıktı:

| **Bilgi (2 sütunu kaplar)** |     |
| --------------------------- | --- |
| Ad                          | Ali |

---

# 🔵 **8. Adım — Satır birleştirme (rowspan)**

Bir hücre **aşağı doğru 2 satırı kaplasın** istersen:

### Kod:

```html
<table border="1">
    <tr>
        <td rowspan="2">Çarşamba</td>
        <td>10:00</td>
    </tr>
    <tr>
        <td>11:00</td>
    </tr>
</table>
```

### Çıktı:

| Çarşamba | 10:00 |
|          | 11:00 |

---

# 🔵 **9. Adım — Daha güzel tablo yapmak (CSS ile)**

### Kod:

```html
<style>
    table {
        border-collapse: collapse;
        width: 40%;
    }
    th, td {
        border: 1px solid black;
        padding: 8px;
    }
    th {
        background-color: #eee;
    }
</style>

<table>
    <tr>
        <th>Ürün</th>
        <th>Fiyat</th>
    </tr>
    <tr>
        <td>Mouse</td>
        <td>150</td>
    </tr>
</table>
```

### Çıktı:

| Ürün  | Fiyat |
| ----- | ----- |
| Mouse | 150   |

Daha profesyonel görünür.

---

# 🔴 **10. Adım — En ileri seviye küçük tablo**

Hem başlık, hem rowspan, hem colspan var.

### Kod:

```html
<table border="1">
    <caption>Ders Programı</caption>

    <tr>
        <th>Gün</th>
        <th>Saat</th>
        <th>Ders</th>
    </tr>

    <tr>
        <td rowspan="2">Pazartesi</td>
        <td>10:00</td>
        <td>Matematik</td>
    </tr>

    <tr>
        <td colspan="2">Etüt</td>
    </tr>
</table>
```

### Çıktı:

| **Gün**             | **Saat**       | **Ders**  |
| ------------------- | -------------- | --------- |
| Pazartesi (2 satır) | 10:00          | Matematik |
|                     | colspan (Etüt) |           |

---

# 🎉 Tam özet:

1. `<table>` → tablo
2. `<tr>` → satır
3. `<td>` → hücre
4. `<th>` → başlık hücresi
5. `colspan` → yatay birleştirme
6. `rowspan` → dikey birleştirme
7. `caption` → tablo başlığı
8. CSS → tabloya tasarım

---

