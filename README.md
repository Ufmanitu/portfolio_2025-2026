# C# Portfólió – Futtatási útmutató

## Megnyitás https://ufmanitu.github.io/portfolio_2025-2026/

Az oldal közvetlenül elérhető a GitHub Pages linkre kattintva – telepítés vagy beállítás nem szükséges.

Azonban ha letölti a fájlt és nem a githubon keresztül futtatja, 
akkor Live Server extensionnel kell megnyitni, ha szeretnénk az oldalon futtatni a feladatok eredményét.

MINDKÉT ESETBEN internet kapcsolat szükséges, hogy az oldalon belül 
a feladatok kódja lefusson.

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
| `429` hibakód | Napi limit elérve, másnap újraindul |
| `401` hibakód | API credentials hiba – kérjük, értesítse a készítőt |
| Üres konzol | Ellenőrizze a BEMENET mezőt, lehetséges, hogy hiányzik egy érték |
