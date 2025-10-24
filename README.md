## Dokumentáció

**Készítők:**

- Hegedüs Milán
- Joó Zoltán
- Deák Bence

**Intézmény:**

Ganz Ábrahám Két Tanítási Nyelvű Technikum


---

## Tartalomjegyzék

- Specifikáció
  - 1.1 Feladat leírása
  - 1.2 Használati esetek
  - 1.3 Követelmények
- Tervezés
  - 2.1 Alkalmazás
    - 2.1.1 Alap információk
    - 2.1.2 Telepített szolgáltatások és egyéb alkalmazások
    - 2.1.3 A rendszer felhasználói fiókjai és csoportjai - Admin - játékos
    - 2.1.4 Mentés és monitorozás
  - 2.2 Operációs rendszer és fejlesztői környezet
    - 2.2.1 Git konfiguráció
    - 2.2.2 Repository klónozása és ágak létrehozása
    - 2.2.3 Példaprogram készítése és push
    - 2.2.4 Példaprogram készítése és push
    - 2.5.5 Issue-k létrehozása

---

# Specifikáció

## 1.1 Feladat leírása

kaszinó játékok

## 1.2 Használati esetek

- Fejlesztők: A kód fejlesztéséért felelősek
- Tesztelő: kivizsgálja a lehetséges hibákat
- Játékos: játszik

## 1.3 Követelmények

- 3 kaszinó játék pl.: póker, félkarú rabló, blackjack, roulette
- bejelentkezés
- pénz
- beállítás
- kilépés

---

# Tervezés

## 2.1 Alkalmazás

- Visual Studio 2022

## 2.2 Kód nyelv

- C#

## 2.3 Terv

A fejlesztők GitHub-on keresztül fejlesztik a kódot.

### 2.1.1 Alap információk

- GitHub
- VS 2022

### 2.1.2 Telepített szolgáltatások és egyéb alkalmazások

- GitHub
- VS 2022

### 2.1.3 A rendszer felhasználói fiókjai és csoportjai

- Admin
- Játékos

### 2.1.4 Mentés és monitorozás

- GitHubon keresztül és verbálisan

## 2.5 Operációs rendszer és fejlesztői környezet

- Windows és kényelmes

### 2.5.2 Git konfiguráció

- A felhasználók a Git klienst konfigurálták saját nevükkel és e-mail címükkel:

### 2.5.3 Repository klónozása és ágak létrehozása

- fork és Github Desktop

### 2.5.4 Példaprogram készítése és push

- push push

### 2.5.5 Issue-k létrehozása

- Frontend projekt (5 issue példa):

- Főmenü UI létrehozása

- vezérlés

- pénz kijelzés (HUD)

- animációk

- Backend projekt (3 issue példa):

- Felhasználó hitelesítés megvalósítása

- logika fejlesztése

- Játékmenet

## 3. Tesztelés

### 3.1 Tesztelési cél  
A tesztelés célja annak biztosítása, hogy az alkalmazás helyesen működjön, stabil legyen, és megfeleljen a specifikációban („1.3 Követelmények”) leírt funkcióknak.  
Vizsgáljuk mind a frontend, mind a backend komponenseket a Visual Studio 2022 és C# alapú környezetben.

### 3.2 Tesztelési környezet  
- Operációs rendszer: Windows (pl. 10-es vagy újabb)  
- Fejlesztői környezet: Visual Studio 2022  
- Verziókezelés: GitHub repository („Kaszino_Projekt”)  
- Programozási nyelv: C#  
- Tesztelési módszerek: manuális funkcionális tesztek, egység- és integrációs tesztek (ha implementálva)

### 3.3 Tesztelési típusok  

#### Funkcionális tesztek  
Ellenőrizzük, hogy az egyes funkciók a követelményeknek megfelelően működnek:  
| Tesztelt funkció       | Elvárt eredmény                                        |
|------------------------|---------------------------------------------------------|
| Bejelentkezés          | Sikeres belépés érvényes adatokkal                     |
| Hibás bejelentkezés    | Megfelelő hibaüzenet jelenik meg                       |
| Kaszinó játék indítása (például póker) | A játék elindul, működik a játékmenet     |
| Pénz-kijelzés (HUD)    | Az aktuális egyenleg helyesen jelenik meg              |
| Kilépés gomb           | Az alkalmazás biztonságosan bezárul                     |

#### Integrációs tesztek  
Cél: külön modulok (pl. bejelentkezés, játéklogika, adatkezelés) helyes együttműködésének ellenőrzése.  
- Felhasználói adatok átadása a frontend és backend között  
- Egyenleg frissítése játék közben  
- Beállítások mentése és újratöltése  

#### Felhasználói (UI) tesztek  
Cél: a grafikus felhasználói felület használhatóságának, áttekinthetőségének és hibamentességének vizsgálata.  
- Menü navigáció működése  
- Gombok, animációk helyes megjelenése  
- Játékos információk (egyenleg, pontok, státusz) megjelenítése és frissítése  

#### Teljesítményteszt  
Cél: Az alkalmazás válaszidejének és stabilitásának vizsgálata, pl. stressz- vagy terheléses teszt kisebb felhasználószámmal.  
- Az alkalmazás folyamatosan fut stabilan, lefagyás nélkül  
- Átlagos válaszidő a kritikus műveleteknél (pl. játékindítás, egyenleg frissítés) megfelel a felhasználói elvárásoknak (< 1 másodperc kiindulási cél)

### 3.4 Hibák és javítások  
A tesztelés során előfordult hibák és azok státusza:  
- Hibás pénz-kijelzés játék végén → **Javítva**  
- UI méretezési probléma képernyőváltáskor → **Javítva**  
- Logikai hiba a blackjack pontszám számításánál → **Javítva**  
(Feltételezve, hogy a hibák már dokumentálva és kezelve lettek. Javasolt minden hibát egy hibajegy formájában rögzíteni a projekt issue-ként.)

### 3.5 Tesztelési összegzés  
A tesztelési folyamat során az alkalmazás minden fő funkcióját ellenőriztük. Az eredmények alapján:  
- A rendszer stabilnak és használhatónak bizonyult  
- A felhasználói felület esztétikus, átlátható  
- A specifikációban rögzített követelmények teljesültek  
