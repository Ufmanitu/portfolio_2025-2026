# C# Portfólió – Futtatási útmutató

## Mire van szükség?

- **Visual Studio Code** – [letöltés](https://code.visualstudio.com/)
- **Live Server** extension (VS Code-on belül telepíthető, ingyenes)
- Internetkapcsolat (a kódok futtatása JDoodle API-n keresztül történik)

---

## Telepítés – egyszer kell elvégezni

1. Nyissa meg a VS Code-ot
2. Kattintson a bal oldali **Extensions** ikonra (vagy `Ctrl+Shift+X`)
3. Keressen rá: `Live Server`
4. Telepítse a **Ritwick Dey** által írt verziót (zöld Install gomb)

---

## Futtatás

1. Nyissa meg a `portfolio.html` fájlt VS Code-ban
2. Kattintson jobb gombbal a fájlra az Explorer panelben
3. Válassza: **Open with Live Server**
4. A böngésző automatikusan megnyitja az oldalt `http://127.0.0.1:5500/portfolio.html` címen

> ⚠️ **Fontos:** Kérjük, ne dupla kattintással nyissa meg a fájlt! Ha `file://`-ból töltődik be (pl. a böngészőbe húzva), a Futtatás gomb nem fog működni.

---

## A feladatok futtatása

1. Kattintson egy feladatra – kinyílik a kódszerkesztő
2. A **⌨ BEMENET** mezőben módosítható a program bemenete (soronként egy érték)
3. Kattintson a **▶ Futtatás** gombra
4. Az eredmény az oldal alján megjelenő konzolban látható

---

## Korlátok

| Limit | Érték |
|---|---|
| Napi futtatások | 200 / nap |
| Visszaállítás | minden éjfélkor (UTC) |
| Fordító | C# / Mono (JDoodle API) |

Ha a napi limit elérésre kerül, másnap automatikusan folytatható a használat.

---

## Hibaelhárítás

| Hiba | Megoldás |
|---|---|
| `Failed to fetch` | A fájl `file://`-ból fut – Live Servert kell használni |
| `429` hibakód | Napi limit elérve, másnap újraindul |
| `401` hibakód | API credentials hiba – kérjük, értesítse a készítőt |
| Üres konzol | Ellenőrizze a BEMENET mezőt, lehetséges, hogy hiányzik egy érték |