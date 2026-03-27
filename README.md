# ⚙️ Programowanie CNC i Systemy CAM - Technologia Obróbki

Projekt inżynierski polegający na opracowaniu kompletnej technologii wytwarzania detalu metodą obróbki ubytkowej (skrawaniem). Projekt obejmuje dobór narzędzi, parametrów skrawania, zaprojektowanie ścieżek narzędzia oraz weryfikację procesu poprzez symulację kinematyki maszyny.

## 🎯 Cel Projektu
Opracowanie trójetapowego procesu technologicznego (toczenie i frezowanie) dla zadanego detalu. Głównym założeniem było wygenerowanie bezkolizyjnego programu obróbkowego oraz optymalizacja czasu maszynowego przy zachowaniu wymagań rysunku technicznego.

## 🛠 Wykorzystane technologie i oprogramowanie
* **System CAM:** [Wpisz nazwę programu, np. Siemens NX CAM / SolidCAM / Mastercam] (Generowanie ścieżek narzędzia, symulacja bryłowa).
* **Dobór narzędzi i parametrów:** Sandvik CoroPlus® ToolGuide (optymalizacja Vc, fz, ap).
* **Środowisko maszynowe:** Obrabiarka CNC HAAS VF-1.

## ⚙️ Opracowana technologia (Etapy obróbki)
Proces technologiczny podzielono na trzy główne zamocowania:
1. **Operacja I (Toczenie / Obróbka zgrubna):** Wstępne usunięcie naddatku materiału z powierzchni zewnętrznych, przygotowanie bazy do kolejnych chwytów.
2. **Operacja II (Frezowanie I):** Obróbka wzdłuż osi Z w nowym zamocowaniu. Frezowanie głównych cech geometrycznych detalu.
3. **Operacja III (Frezowanie II):** Ostatnie zamocowanie. Frezowanie wykańczające i obróbka pozostałych detali konstrukcyjnych.

## 📊 Weryfikacja i Symulacja
Przed wygenerowaniem finalnego G-Kodu, proces poddano ścisłej weryfikacji wirtualnej:
* **Detekcja kolizji:** Przeprowadzono symulację bryłową z włączonym stopem warunkowym. Program przeszedł walidację bez żadnych kolizji oprawki/narzędzia z materiałem i uchwytami.
* **Czas maszynowy:** Na podstawie dobranych parametrów z katalogu Sandvik wyestymowano całkowity czas obróbki na **42 minuty i 54 sekundy**.

## 📁 Zawartość Repozytorium
* `README.md` - opis założeń technologicznych projektu.
* `images/` - zrzuty ekranu prezentujące ścieżki narzędzia, zamocowania oraz raporty z detekcji kolizji.

## 📷 Wizualizacje Procesu CAM

### Pierwsza operacja - toczenie składa się z poniższych zabiegów:
<img width="661" height="228" alt="image" src="https://github.com/user-attachments/assets/c95a12ed-0519-470a-874c-f335e0c8e8b4" />

### Dla operacji pierwszej – toczenie, dla zabiegu zgrubnego toczenia powierzchni zewnętrznej dobrano narzędzie oraz parametry skrawania:
<img width="571" height="758" alt="{AFAD691A-E83C-4906-8D71-1E0FBE8E1DF8}" src="https://github.com/user-attachments/assets/dd3287d8-cc09-45c3-8cc2-446124ff24af" />

### Uchwyt - toczenie
<img width="363" height="401" alt="image" src="https://github.com/user-attachments/assets/395f9902-90c5-482a-a3dc-a969a29025ab" />

### Uchwyt - frezowanie I
<img width="537" height="414" alt="image" src="https://github.com/user-attachments/assets/917c04d3-70b0-422b-a977-9c53f455fda6" />

---
*Projekt zrealizowany w ramach zajęć "Systemy CAx w obróbce skrawaniem" na Politechnice Warszawskiej (Kierunek: Automatyzacja i Robotyzacja Procesów Produkcyjnych).*
