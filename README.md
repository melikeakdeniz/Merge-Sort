# Merge-Sort### Merge Sort Aşamaları

Verilen dizi: \([16, 21, 11, 8, 12, 22]\)

Merge Sort, diziyi sürekli olarak ikiye bölerek ve ardından bu alt dizileri sıralı bir şekilde birleştirerek çalışan bir algoritmadır.

1. **Diziyi ikiye böl:**
   \[
   [16, 21, 11, 8, 12, 22] \rightarrow [16, 21, 11] \text{ ve } [8, 12, 22]
   \]

2. **Alt dizileri tekrar ikiye böl:**
   \[
   [16, 21, 11] \rightarrow [16] \text{ ve } [21, 11]
   \]
   \[
   [8, 12, 22] \rightarrow [8] \text{ ve } [12, 22]
   \]

3. **Alt dizileri tekrar ikiye böl:**
   \[
   [21, 11] \rightarrow [21] \text{ ve } [11]
   \]
   \[
   [12, 22] \rightarrow [12] \text{ ve } [22]
   \]

4. **Alt dizileri birleştir ve sırala:**
   \[
   [21] \text{ ve } [11] \rightarrow [11, 21]
   \]
   \[
   [12] \text{ ve } [22] \rightarrow [12, 22]
   \]

5. **Alt dizileri birleştir ve sırala:**
   \[
   [16] \text{ ve } [11, 21] \rightarrow [11, 16, 21]
   \]
   \[
   [8] \text{ ve } [12, 22] \rightarrow [8, 12, 22]
   \]

6. **Son alt dizileri birleştir ve sırala:**
   \[
   [11, 16, 21] \text{ ve } [8, 12, 22] \rightarrow [8, 11, 12, 16, 21, 22]
   \]

Bu aşamalarda diziyi önce bölüyor, sonra tekrar birleştirip sıralıyoruz. İşte Merge Sort'un ayrıntılı adımları:

- **Başlangıç:**
  \[
  [16, 21, 11, 8, 12, 22]
  \]

- **Bölme 1:**
  \[
  [16, 21, 11] \quad \text{ve} \quad [8, 12, 22]
  \]

- **Bölme 2:**
  \[
  [16] \quad \text{ve} \quad [21, 11]
  \]
  \[
  [8] \quad \text{ve} \quad [12, 22]
  \]

- **Bölme 3:**
  \[
  [21] \quad \text{ve} \quad [11]
  \]
  \[
  [12] \quad \text{ve} \quad [22]
  \]

- **Birleştirme 1:**
  \[
  [11, 21]
  \]
  \[
  [12, 22]
  \]

- **Birleştirme 2:**
  \[
  [16] \quad \text{ve} \quad [11, 21] \rightarrow [11, 16, 21]
  \]
  \[
  [8] \quad \text{ve} \quad [12, 22] \rightarrow [8, 12, 22]
  \]

- **Son Birleştirme:**
  \[
  [11, 16, 21] \quad \text{ve} \quad [8, 12, 22] \rightarrow [8, 11, 12, 16, 21, 22]
  \]

### Big-O Gösterimi
Merge Sort'un zaman karmaşıklığı:

- **En iyi durum (Best case):** \(O(n \log n)\)
- **Ortalama durum (Average case):** \(O(n \log n)\)
- **En kötü durum (Worst case):** \(O(n \log n)\)

Merge Sort'un her durumda zaman karmaşıklığı \(O(n \log n)\) olarak ifade edilir.
