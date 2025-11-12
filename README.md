# szorg2.1

Feladat célja
A program az `ascii_art` mappában található `.txt` fájlokat tömöríti, majd kiírja mindegyikhez:
- az eredeti fájlméretet,
- a tömörített méretet,
- valamint a tömörítési arányt százalékban.

A tömörítéshez a Python beépített `zlib` modulja kerül felhasználásra.

Használt modulok
- `os` – fájlok és könyvtárak bejárása, útvonalak kezelése  
- `zlib` – veszteségmentes tömörítés és visszafejtés  

Működés röviden
1. A `be_tomorit()` függvény tömöríti a szöveget (`zlib.compress`).
2. A `ki_tomorit()` visszaalakítja az adatot szöveggé (`zlib.decompress`).
3. A `fajl_meret()` meghatározza a fájl méretét bájtban.
4. A program bejárja az `ascii_art` mappát, feldolgozza a `.txt` fájlokat, és mindegyikről kiszámítja a tömörítési arányt.
5. Az eredményeket a konzolra írja ki a következő formátumban:
név, eredeti méret, tömörített méret, tömörítési arány %
kave.txt, 262, 89, 34.0%
kutya.txt, 300, 160, 53.3%
madar.txt, 34, 36, 105.9%
nlabda.txt, 2102, 462, 22.0%
