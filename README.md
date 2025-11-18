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

---

İstersen **hazır tablo tasarımı** da yapayım (renkli, şık).
“Öğrenci tablosu yap” veya “Fiyat tablosu yap” diyebilirsin.
