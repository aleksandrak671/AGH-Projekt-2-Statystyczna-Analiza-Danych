# Statystyczna-Analiza-Danych-AGH-Projekt-2

Projekt zaliczeniowy z przedmiotu **Statystyczna analiza danych** (AGH).  
Temat: **skalowanie wielowymiarowe (MDS)** i **analiza składowych głównych (PCA)** na danych o krajach świata.

---

## Cel

- wykonać MDS dwiema metodami:  
  - klasyczne MDS – `cmdscale()`,  
  - skalowanie Sammona – `MASS::sammon()`;
- przeprowadzić PCA na macierzy korelacji (`eigen()`, `prcomp()`),
- porównać wyniki MDS i PCA oraz zinterpretować różnice między krajami.

---

## Dane

Plik: **`countries of the world.csv`**  
Jedna obserwacja = 1 kraj.

Użyte zmienne (wskaźniki rozwoju):

- `GDP ($ per capita)`, `Infant mortality`, `Literacy`, `Phones`,
- `Birthrate`, `Deathrate`,
- `Agriculture`, `Industry`, `Service`.

W repo jest też **`countries_clean_scaled.csv`** – dane po czyszczeniu i standaryzacji.

---

## Pliki

- `Projekt 2.Rmd` – kod + opis (R Markdown),
- `Projekt-2.html` – wyrenderowany raport,
- `countries of the world.csv` – surowe dane,
- `countries_clean_scaled.csv` – dane przygotowane.

---

## Co robimy w analizie

- **EDA**: statystyki, histogramy, boxploty, korelacje, test Bartletta.  
- **MDS**: cmdscale 2D/3D i Sammon 2D, obliczenie STRESS, porównanie jakości.  
- **PCA**: wartości własne, scree plot, biplot, interpretacja PC1–PC3.  
- **Porównanie MDS vs PCA**: korelacje współrzędnych, wnioski, które zmienne najmocniej różnicują kraje i ile składowych wystarczy (PC1–PC3 ≈ 85% wariancji).
