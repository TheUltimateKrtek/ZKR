# ZKR
ZKB seminárka

# Zadání
Implementovat **2 vybrané algoritmy** = **1 algoritmus klasické kryptografie** + **1 algoritmus moderní kryptografie**. Implementaci doplnit textem s informacemi o zvoleném kryptografickém systému (kdy vznikl a proč), jeho autoři, pravidla použití, důsledky porušení kryptografického protokolu, jak se dá luštit, ...) a na příkladu ukázat jeho funkčnost (tj. několik odstavců textu v ČJ/AJ zašifrovat, poté dešifrovat, a také ukázat neúzpěšnist dešifrování při drobné úpravě klíče).

# Césarova šifra (klassická kryptografie)

**Vznik a autoři**: Tato šifra je jedním z nejstarších známých šifrovacích systémů, která byla používána už v antickém Římě. Její název pochází od Julia Cézara, který ji používal pro bezpečnou komunikaci.

**Princip**: Je to substituční šifra, kde každé písmeno v textu je posunuto o určitou pevně danou hodnotu v abecedě. Například s posunem o 3 se "A" stane "D", "B" se stane "E" atd.

**Použití**: Ve své době byla velmi efektivní pro šifrování textů, dnes je to ale velmi slabý algoritmus, který lze snadno prolomit pomocí frekvenční analýzy nebo prostým vyzkoušením všech možných posunů (tzv. brute force).

**Porušení protokolu**: Pokud dojde k úniku klíče (posunu), je šifra snadno rozluštitelná. To činí systém zranitelným pro útočníky.

### Příklad
```python
# Kód ze souboru ZKR.py ...
original = ""
```

2. AES (moderní kryptografie)

Vznik a autoři: AES (Advanced Encryption Standard) byl vyvinut v roce 2001 Národním institutem standardů a technologie (NIST) jako náhrada za starší DES. AES byl navržen belgickými kryptografy Vincentem Rijmenem a Joanem Daemenem.

Princip: AES je bloková šifra, která šifruje data v blocích o velikosti 128 bitů. Používá tajný klíč, jehož délka může být 128, 192 nebo 256 bitů. AES využívá několik šifrovacích kroků, jako je substituce, permutace a smíchání.

Použití: AES je v současnosti jedním z nejpoužívanějších algoritmů pro šifrování, a to jak v komerční sféře, tak i v různých vládních aplikacích. Používá se například v HTTPS pro šifrování webového provozu.

Porušení protokolu: Pokud útočník získá tajný klíč, může dešifrovat všechny zašifrované zprávy. AES je však odolný proti většině běžných útoků, pokud je správně implementován a používán s dostatečně silným klíčem.

Příklad: Zašifrování a dešifrování textu pomocí AES se obvykle provádí pomocí knihoven v programovacích jazycích, jako je Python nebo C++.
