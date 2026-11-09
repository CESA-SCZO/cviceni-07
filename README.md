# Cvičení 7

**Klonování repozitáře:**
- Klávesa Windows + R -> cmd -> Enter
```
mkdir c:\SCZO_2026
cd C:\SCZO_2026
git clone https://cesta.ke.forked.git.repozitari
uv sync
```

**Úkol 1:**
- Načtěte obraz 'texture.png' a převeďte jej na šedotónový. Zobrazte ho i s jeho histogramem. 
- Transformujte originální obraz na parametrické obraz:
  - Připravte novou prázdnou výstupní proměnnou o stejné velikosti jako je vstupní obraz a s datovým typem float. 
  - Pomocí dvou vnořených for cyklů projděte celý obraz a vybírejte submatice o velikosti 9x9 px. Ze submatic vypočtěte parametr:
    - Směrodatné odchylky a uložte na odpovídající pozici ve výstupní matici 
    - Rozsahu pomocí nelineárního rozsahového filtru, jehož principem je nalezení lokálního rozdílu mezi maximem a minimem v submatici. 
  - Zobrazte parametrický obraz a jeho histogram


**Úkol 2:**
- Načtěte obraz ‘monsters.png’ a převeďte jej na šedotónový a zobrazte. 
- Vytvořte hrubou hranovou reprezentaci s využitím první parciální derivace:
  - Vytvořte gradientní obraz 
  - Vypočtěte první parciální derivaci pomocí Sobelovy masky ve směru x a y 
  - Vytvořte gradientní obraz pomocí výpočtu euklidovské vzdálenosti 
  - Gradientní obraz vhodně nafiltrujte a zobrazte

**Úkol 3:**
- Vytvořte hrubou hranovou reprezentaci obrazu monsters s využitím Laplacianu obrazu:
- Prozkoumejte priloženou funkci 'zero_crossing_detection()'
- S využitím funkce 'zero_crossing_detection()' vytvořte hrubou hranovou reprezentaci z Laplacianu

**Závěr cvičení:**
```
git add .
git commit –m „message“
git push origin main
```