# 🧠 Narzędzia Pomocnicze Unity – Heightmap Dev Tools

Zestaw zaawansowanych narzędzi wspierających pracę w Unity przy edycji scen, debugowaniu hierarchii obiektów, analizie błędów oraz automatyzacji zadań.

---

## 📦 Zawartość projektu

Projekt zawiera wyłącznie **narzędzia deweloperskie** – bez kodu gry. Każdy skrypt ma jasno określoną odpowiedzialność i działa zgodnie z zasadami czystej architektury Unity.

### 🔧 Główne moduły

| Folder | Opis |
|--------|------|
| `Scripts/Narzędzia/Automatyzacja/` | Eksport sceny, analiza hierarchii, generowanie raportów |
| `Scripts/Narzędzia/AI/` | Generatory promptów, dokumentacja API, analiza klas |
| `Scripts/Narzędzia/Edytor/` | Skanery duplikatów, kreatory klas, eksport prefabów |
| `Scripts/Narzędzia/Backup/` | Narzędzia do robienia kopii i śledzenia wersji |
| `Scripts/Narzędzia/Walidacja/` | Checklisty, liczniki tagów, walidacja danych heightmap |
| `Docs/` & `Dokumentacja/` | Checklisty, mapy klas, zasady projektu, plany testów |

---

## 🧪 System debugowania sceny

Główne narzędzie do testów struktury sceny:

### 🔹 `🧠 Debuguj aktywną scenę`

Uruchamia:
1. Eksport hierarchii aktywnej sceny
2. Oczekiwanie na zapis pliku
3. Automatyczną analizę i raport `.md`

🔁 Znajdziesz w:  
`Scripts/Narzędzia/Automatyzacja/Wspólne/DebugerSceny.cs`

---

## 📊 Przykładowy raport (`*.md`)

```markdown
# 🧪 Raport: HierarchiaDebug – scena: `SampleScene`
Data: 2025-07-10 14:24:43

## 📊 Statystyki ogólne
- 🎮 Liczba GameObjectów: 2
- 🧩 Komponentów: 5
- ⚠️ Null komponentów: 0

## 🚨 Problemy potencjalne:
- 🏷️ Untagged: 1
- 🧱 Warstwa Default: 2

## ⚙️ Diagnostyka systemowa:
- 🎧 AudioListener: 1
- 🧭 EventSystem: ❌ brak

✅ Analiza zakończona.
