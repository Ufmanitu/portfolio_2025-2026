# C# Portfólió – Futtatási útmutató

## Megnyitás https://ufmanitu.github.io/portfolio_2025-2026/

Az oldal közvetlenül elérhető a GitHub Pages linkre kattintva – telepítés vagy beállítás nem szükséges.

Ha le van töltve a fájl, Live Server extensionnel kell megnyitni VS Code-ban (ne dupla kattintással), különben a Futtatás gomb nem működik.

Mindkét esetben internetkapcsolat szükséges.

---

## A feladatok futtatása

1. Kattintson egy feladatra – kinyílik a kódszerkesztő
2. A **⌨ BEMENET** mezőben módosítható a program bemenete (soronként egy érték)
3. Kattintson a **▶ Futtatás** gombra
4. Az eredmény az oldal alján megjelenő konzolban látható

---

## Technikai háttér

A kódok futtatása a **JDoodle API**-n keresztül történik, egy saját **Cloudflare Worker** proxyn át (`plain-lab-e94f.attika-eger.workers.dev`). Ez biztosítja, hogy a böngésző és a JDoodle szerver közötti kommunikáció akadálymentesen működjön.

- **Fordító** – C# / Mono (JDoodle API)
- **Proxy** – Cloudflare Worker (ingyenes, 100 000 kérés/nap)
- **Napi limit** – 200 futtatás / nap (JDoodle ingyenes csomag)
- **Visszaállítás** – minden éjfélkor (UTC)

---

## Hibaelhárítás

- `Failed to fetch` – A fájl `file://`-ból fut, Live Servert kell használni
- `429` hibakód – Napi limit elérve, másnap újraindul
- `401` hibakód – API credentials hiba, kérjük értesítse a készítőt
- Üres konzol – Ellenőrizze a BEMENET mezőt, lehetséges hogy hiányzik egy érték