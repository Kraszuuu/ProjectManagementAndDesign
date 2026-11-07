# Checklist wymagań kursu ISL443E – Project Design and Management (ITU, semestr 2026/2027 Fall)

Dokument porównuje wymagania sylabusa ISL443E oraz artefaktów w folderze `TR_artifacts`
z aktualnym stanem projektu ICT z Politechniki Wrocławskiej (`ICT_Project` —
„Zintegrowany system medyczny wspierający zarządzanie informacjami (EMR)”, 4EDM, czerwiec 2026).

**Legenda statusów:**

| Symbol | Znaczenie |
|--------|-----------|
| ✅ | Wymaganie spełnione / artefakt gotowy |
| ⚠️ | Spełnione częściowo – wymaga uzupełnienia lub adaptacji do formatu ITU |
| ❌ | Niezrealizowane – wymagane do wykonania od zera |
| ➖ | Nie dotyczy artefaktów projektu (działalność czysto administracyjna / kursowa) |

---

## 1. Wymagania ogólne projektu (TERM PROJECT)

### 1.1 Idea projektu

| # | Wymaganie | Status | Opis stanu w projekcie PWr |
|---|-----------|--------|----------------------------|
| 1.1.1 | Zrównoważony pomysł na przedsięwzięcie biznesowe lub projekt społeczny (sustainable entrepreneurial business or social project idea) wygenerowany przez studentów | ⚠️ | Projekt PWr to studium wdrożeniowe systemu EMR dla istniejącego szpitala (Szpital im. Bajgla), nie samodzielny pomysł przedsiębiorczy typu startup. Da się go obronić jako projekt społeczny (dostęp do opieki zdrowotnej), ale wymaga to ujęcia w ramy „społecznej wartości" i wskazania modelu działania / finansowania – obecnie jest to zamówienie publiczne, nie pomysł biznesowy. |
| 1.1.2 | Powiązanie z Sustainable Development Goal (SDG) – każde projekt musi przyczyniać się do realizacji celu zrównoważonego rozwoju | ❌ | Zero wzmianki o SDG w rozdziałach i prezentacji. Temat e-zdrowia aż się prosi o **SDG 3 (Dobre zdrowie i dobrostan)**, ewentualnie SDG 9/10 – ale nie jest to w żaden sposób ujęte. Wymagane: jawne wskazanie celu(iów), uzasadnienie związku i pomiar wkładu. |

### 1.2 Zespół

| # | Wymaganie | Status | Opis stanu w projekcie PWr |
|---|-----------|--------|----------------------------|
| 1.2.1 | Liczba członków zespołu ściśle między 7 a 8 osób | ❌ | Zespół PWr liczy **6 osób** (Pola Polańska, Piotr Bonar, Kacper Kurp, Wiktor Szajerka, Roch Szewczyk, Robert Rubaszek). Na ITU konieczne dopełnienie zespołu o 1–2 osoby. |
| 1.2.2 | Zespoły utworzone do 12.10.2026 przez live Excel prowadzony przez RA | ➖ | Kwestia administracyjna ITU; w projekcie PWr nieistotna, ale przy przenoszeniu na ITU trzeba dopełnić formalność rejestracji. |
| 1.2.3 | Podział pracy w zespole widoczny w raporcie | ✅ | `Chapters/work_table.tex` — tabela „Podział pracy członków zespołu" z numerami albumu i zakresem prac (6 wierszy). Uwaga: pokazuje autorstwo rozdziałów, nie zarządzanie projektem. |

### 1.3 Formalności raportowe

| # | Wymaganie | Status | Opis stanu w projekcie PWr |
|---|-----------|--------|----------------------------|
| 1.3.1 | Kompletna lista autorów na stronie tytułowej raportu (bez późniejszych zmian) | ✅ | `main.tex` — na stronie tytułowej wymienieni wszyscy członkowie z numerami albumu. Przy przenoszeniu na ITU: uzupełnić o nowych członków (patrz 1.2.1). |
| 1.3.2 | Wersja finalna raportu wg guideline z Ninova (tydzień ~14) | ⚠️ | Raport PPr istnieje i jest kompletny jako dokument 8 rozdziałów, ale został napisany pod inny przedmiot (bezpieczeństwo architektury ICT). Brak: struktury wg wytycznych ITU (w tym WBS, harmonogramu, planu ryzyk – patrz sekcje 2–4), deklaracji AI, przepisania pod kątem „term project" ITU. |
| 1.3.3 | Praca wyłącznie przez Ninova (brak submitów mailowych) | ➖ | Kwestia administracyjna. |

---

## 2. Project Proposal and Presentation (15% oceny: 7,5% prezentacja + 7,5% raport)

Wymagania z sylabusa (tydzień 7) i `Project Proposal Sample.pptx`:

### 2.1 Składniki merytoryczne proposalu

| # | Wymaganie | Status | Opis stanu w projekcie PWr |
|---|-----------|--------|----------------------------|
| 2.1.1 | **Project Selection** – kryteria wyboru, modele selekcji, scoring | ⚠️ | `Chapters/project-idea.tex` — trzy warianty systemu EMR (podstawowy/optymalny/rozszerzony), tabela porównawcza 20 kryteriów, wybór Wariantu II z uzasadnieniem. **Brak formalnego modelu scoringowego** z wagami kryteriów i punktacją (scoring model), którego wymaga tydzień 3 sylabusa; ocena wariantów jest jakościowa (tak/częściowy/niski…). Do uzupełnienia: macierz wagowana + punktacja + wrażliwość na wagi. |
| 2.1.2 | **Business Model Canvas** (ew. Lean Canvas / Social Business Model Canvas) | ❌ | Brak jakiegokolwiek canvasu. `Project Proposal Sample.pptx` pokazuje dokładnie taki slajd jako obowiązkowy. Do zbudowania od zera: 9 bloczków (segmenty klientów, propozycja wartości, kanały, relacje, strumienie przychodów, zasoby, kluczowe działania, partnerzy, struktura kosztów) – dla projektu społecznego w wariancie Social BMC. |
| 2.1.3 | **Value Proposition Canvas** (omawiany w tyg. 1) | ❌ | Nieobecny; wymagany jako narzędzie pracy nad propozycją wartości (mapa profili klientów + mapy korzyści). |
| 2.1.4 | **Elevator Pitch** | ❌ | Brak. Prezentacja PWr ma 25 slajdów i charakter raportu technicznego, nie pitchu. Do przygotowania: zwięzła narracja (problem → rozwiązanie → rynek → wartość → zespół) w ok. 60–90 sekund. |
| 2.1.5 | **Draft WBS** (Work Breakdown Structure) | ❌ | Brak struktury rozbicia pracy. Jedyny element zbliżony: harmonogram płatności M0–M6 w `cost-estimate.tex` (kamienie milowe: kontrakt, architektura, infrastruktura, UAT, urządzenia, pilotaż, go-live) – to lista kamieni milowych, nie WBS. Do zbudowania: hierarchia 2–3 poziomów (np. 1. Inicjacja → 2. Analiza → 3. Projektowanie → 4. Wdrożenie → 5. Odbiór → 6. Zamknięcie) z identyfikatorami pakietów. |
| 2.1.6 | **Project Organization** (struktura organizacyjna projektu) | ⚠️ | `work_table.tex` dzieli prace między 6 osób wg rozdziałów raportu. Brak natomiast **struktury organizacyjnej projektu**: roli Kierownika projektu, zespołów funkcyjnych, raportowania, modelu współpracy z klientem (szpitalem). Część ról pojawia się tylko jako pozycje kosztorysowe (Kierownik projektu, Architekt, DevOps…) w kategorii A CAPEX – to role fikcyjnego wykonawcy, nie podział zadań w zespole studenckim. Do uzupełnienia: wykres organizacyjny + opis ról zespołu projektowego. |
| 2.1.7 | **Stakeholder Analysis** (analiza interesariuszy) | ✅ | `Chapters/empathization.tex` — bardzo rozbudowana: mapa interesariuszy (kluczowi gracze, główni/potencjalni użytkownicy, uśpieni, obserwatorzy) oraz 10 person (dyrektor, zarząd, pracownik IT, lekarz, studentka medycyny, pielęgniarka, pacjent 72 l., pacjent 35 l., złośliwy użytkownik, CEO startupu, media, ministerstwo) z profilami, oczekiwaniami, obawami i implikacjami projektowymi. Realizacja ponad standard wymagany przez ITU – konieczna jedynie adaptacja formatu (macierz wpływu/zaangażowania). |
| 2.1.8 | **RACI matrix** | ❌ | Brak. `work_table.tex` wskazuje autora rozdziału (de facto Responsible), ale nie zawiera R (Responsible), A (Accountable), C (Consulted), I (Informed) dla zadań/aktywności projektowych. Do zbudowania: wiersze = pakiety WBS, kolumny = członkowie zespołu (7–8 osób), komórki = R/A/C/I. |
| 2.1.9 | **Team qualifications** (kwalifikacje zespołu) | ❌ | Brak sekcji opisującej kompetencje członków (wykształcenie, umiejętności techniczne, doświadczenie, certyfikaty, role w projekcie). Do dodania: tabela lub profil każdego członka – dlaczego ten zespół jest zdolny zrealizować projekt. |
| 2.1.10 | **Business Plan Submission** (tydzień 2 – template z Ninova) | ❌ | Brak. Wzór z `Project Proposal Sample.pptx` sugeruje strukturę: grupa/nazwa firmy, need/problem, canvas, benchmark konkurencji. |
| 2.1.11 | **Benchmark / analiza konkurencji** (slajd 7 sample'u: Your company vs competitors, feature comparison) | ⚠️ | `cost-estimate.tex` zawiera benchmarki wdrożeń EMR/EHR (Oracle Cerner, Epic, koszt/łóżko z korektą PPP) – to benchmark **kosztowy**, nie konkurencyjny produktowy. Do uzupełnienia: porównanie z realnymi konkurentami/rozwiązaniami (np. Comarch, Asseco, dedykowane EMR) po cechach. |
| 2.1.12 | **Prezentacja proposalu z udziałem każdego członka (mówienie), obowiązkowa obecność** | ⚠️ | `presentation/ict_presentation.pdf` istnieje (25 slajdów) i na slajdzie końcowym wymienionych jest 6 osób. Nie wiadomo, kto faktycznie prezentował i czy każdy mówił; format nie jest „proposal presentation" ITU. Przy przenoszeniu: skrócić do formatu proposalu, przypisać segmenty, przygotować mówienie każdego członka. |

---

## 3. Final Report and Presentation (30% oceny: 10% prezentacja + 20% raport)

### 3.1 Zawartość raportu finalnego (spodziewana wg sylabusa i przebiegu kursu)

| # | Obszar / artefakt | Status | Opis stanu w projekcie PWr |
|---|-------------------|--------|----------------------------|
| 3.1.1 | Opis problemu i analiza obecnej sytuacji (as-is) | ✅ | `Chapters/introduction.tex` — kontekst eHealth UE (Digital Decade 2030), opis Szpitala im. Bajgla, perspektywy dyrekcji/personelu/pacjenta, analiza bezpieczeństwa, problemy techniczne i organizacyjne, kryteria sukcesu. Źródła cytowane (raport eHealth 2024). |
| 3.1.2 | Wymagania funkcjonalne i niefunkcjonalne | ✅ | `empathization.tex` (synteza wymagań: dostęp rolowy, mobilność, offline, szybkość 3 kliknięć, portal pacjenta, 2FA, audit log, szyfrowanie AES-256/TLS 1.3…) oraz `functionalities.tex` (opis funkcjonalny: panele, aktorzy, uprawnienia, akcje). Ponad standard ITU. |
| 3.1.3 | Warianty rozwiązania i project selection (final) | ⚠️ | Jest (2.1.1) – brak scoring modelu z wagami. |
| 3.1.4 | Architektura systemu | ✅ | `cost-estimate.tex` (sekcja „Architektura i SLA wariantów") + slajdy prezentacji (mikrousługi, Azure, offline sync, SLA 99,9%). |
| 3.1.5 | Opis funkcjonalności / use cases / user stories | ✅ | `functionalities.tex` (systemowe opisy aktorów i akcji) + `user_story.tex` (9 slajdów z dubbingiem głosowym – scenaże użycia). Scenariusze również w prezentacji (lekarz, pacjent, administrator). |
| 3.1.6 | Makieci / prototyp UI | ⚠️ | W `work_table.tex` Roch Szewczyk ma „przygotowanie makiet (mock-upów)"; w rozdziałach makiet brak (Grafiki zawierają tylko slajdy user story). Prezentacja ma slajd „Przykład działania" (pusty tekst – prawdopodobnie zrzuty). Do ujęcia w raporcie: makiety w rozdziale. |
| 3.1.7 | **Scope Management** – plan zarządzania zakresem, WBS, słownik WBS | ❌ | Brak (tylko draft WBS proposalowy patrz 2.1.5). Do zbudowania: pełny WBS, WBS dictionary, baseline scope. |
| 3.1.8 | **Harmonogram projektu** (PERT/CPM, sieć, Gantt) w MS Project | ❌ | Brak jakiejkolwiek sieci zadań, ścieżki krytycznej, wykresu Gantta. W TR_artifacts jest przykładowy `Example of Term Project schedule via MS Project.mpp` – stanowi wzorzec do odtworzenia. Do zbudowania: sieć PERT/CPM, kalkulacja ES/EF/LS/LF, ścieżka krytyczna, harmonogram Gantta w MS Project (tydzień 9–10 sylabusa). |
| 3.1.9 | **Resource Allocation / Resource Levelling / Crashing** | ❌ | Brak. Do zrobienia: macierz zasobów, alokacja, wygładzanie konfliktów, crashed variants z kosztem skrócenia (tydzień 10). |
| 3.1.10 | **Cost Management** – kosztorys z referencjami kosztowymi | ✅ | `cost-estimate.tex` — exceptionally rozbudowany: założenia wejściowe (USK Wrocław), benchmarki rynkowe z cytowanymi źródłami (Hays 2026, NoFluffJobs, Azure Pricing, Cerner/Epic), CAPEX detail (kategorie A–H, osobo-miesiące ze stawkami), OPEX roczny, TCO 5 lat, model komercyjny (narzut+marża), scenariusze optymistyczny/bazowy/pesymistyczny, analiza wrażliwości (tornado), macierz ryzyk kosztowych, koszty adopcji organizacyjnej, harmonogram płatności wg kamieni milowych, wskaźniki jednostkowe (koszt/łóżko z korektą PPP). Spełnia i przekracza wymóg „cost estimation with cost references" (tydzień 6). |
| 3.1.11 | **Earned Value Management** (EVM) | ❌ | Brak. Kosztorys jest statyczny (estymata), nie ma PV/EV/AC, CPI/SPI, forecastów EAC/ETC. Do dodania: rozdział lub sekcja EVM z przykładem monitorowania (tydzień 6). |
| 3.1.12 | **Risk Management** – pełny rejestr ryzyk projektowych | ⚠️ | `cost-estimate.tex` zawiera: macierz scenariuszy ryzyka kosztowego (wpływ na TCO), dwuwarstwową rezerwę (techniczna + zarządcza), analizę wrażliwości. **Brak klasycznego rejestru ryzyk PM**: identyfikacja ryzyk (nie tylko kosztowych – organizacyjne, techniczne, regulacyjne, adopcji), ocena prawdopodobieństwo × wpływ, właściciel ryzyka, strategia (unikanie/przenoszenie/łagodzenie/akceptacja), plan triggerów. Do zbudowania: risk register + probability/impact matrix (tydzień 11). |
| 3.1.13 | **Communication Management** – plan komunikacji | ❌ | Brak. Do zbudowania: stakeholder communication matrix (kto, co, kiedy, jak, kanał, częstotliwość), eskalacja (tydzień 11). |
| 3.1.14 | **Agile Project Management** – elementy zwinne | ❌ | Brak. Sylabus tydzień 12 wymaga podejścia agility; do ujęcia: uzasadnienie wyboru modelu (hybrydowy/wodospadowy/agile), backlog, sprinty, retrospektywa – lub analiza „need for agility" w kontekście projektu. |
| 3.1.15 | **Project Life Cycle / Project Organization (finalna)** | ⚠️ | Idea projektu opisuje warianty wdrożenia; `implementation.tex` opisuje wdrożenie etapowe (pilotaż → rozszerzenie), migrację, szkolenia, bezpieczeństwo, tryb awaryjny – to dobre podłoże, ale brak ujęcia w ramy PLC i struktury organizacyjnej projektu (patrz 2.1.6). |
| 3.1.16 | Założenia organizacyjne wdrożenia, migracja, szkolenia, BCP | ✅ | `Chapters/implementation.tex` — wdrożenie etapowe, migracja danych, szkolenia grupowe, indywidualne konta, backup, monitoring aktywności, procedury awaryjne, wsparcie powdrożeniowe. Spójne z wymaganiami z empatyzacji. |
| 3.1.17 | Jakość / odbiór (UAT, acceptance criteria) | ⚠️ | Kryteria oceny rozwiązania po wdrożeniu opisane w `project-idea.tex` (sekcja „Kryteria oceny": % cyfryzacji, czas dostępu, dostępność, bezpieczeństwo). Brak planu jakości, kryteriów akceptacji UAT (wymienione w harmonogramie płatności M3, ale bez szczegółów), testów. |
| 3.1.18 | Zamknięcie projektu / lessons learned / kryteria sukcesu | ⚠️ | Kryteria sukcesu opisane w `introduction.tex` (sekcja „Docelowa funkcjalność"). Brak sekcji zamknięcia, transition do utrzymania, lessons learned (project nie został zrealizowany – to studium, co jest naturalne dla term project design, ale plan zamknięcia powinien być). |
| 3.1.19 | Bibliografia / źródła | ✅ | `bibliography.bib` — 11 pozycji (raport UE, Hays, NoFluffJobs, Azure, CeZ, USK raport 2014, AACE, World Bank, Software Finder, ThePricer). Styl `abbrv`. |
| 3.1.20 | **Prezentacja finalna** – każdy członek mówi, obowiązkowa obecność | ⚠️ | Prezentacja istnieje (`ict_presentation.pdf`, 25 slajdów: problem, empatyzacja, warianty, architektura, funkcjonalności, scenariusze, kosztorys CAPEX/OPEX/TCO, założenia wdrożenia, korzyści, bibliografia). Na slajdzie tytułowym i końcowym 6 osób; brak potwierdzenia, że każdy mówił; wymagana restrukturyzacja pod kątem wystąpienia końcowego ITU. |

---

## 4. Wymagania administracyjne i kursowe

| # | Wymaganie | Status | Opis stanu w projekcie PWr |
|---|-----------|--------|----------------------------|
| 4.1 | **ISL 443E AI Conduct and Declaration** – podpisana deklaracja każdej osoby, dołączona do każdego raportu | ❌ | Brak w artefaktach. Wzór w `TR_artifacts/ISL 443E AI Conduct and Declaration.pdf` (indywidualna deklaracja: narzędzia AI, zakres użycia, wkład własny, podpis). Każdy z 7–8 członków musi wypełnić i dołączyć. |
| 4.2 | **Peer evaluation** po prezentacji pośredniej i finalnej | ➖ | Procedura ITU (platforma/Ninova), nie artefakt raportowy – ale trzeba pamiętać o obowiązku uczestnictwa. |
| 4.3 | **AI check** prac | ➖ | Procedura ITU; deklaracja z 4.1 jest tego elementem. |
| 4.4 | **In-class practice/case studies** – obecność min. 3 z 5 + raporty na Ninova | ➖ | Aktywności czysto kursowe ITU, poza zakresem artefaktów projektu. |
| 4.5 | **Midterm** (40% oceny) | ➖ | Egzamin kursowy, poza zakresem projektu. |
| 4.6 | Samodzielna nauka **MS Project** | ❌ | W TR_artifacts dostępny wzorzec `Example of Term Project schedule via MS Project.mpp`; projekt PWr nie zawiera harmonogramu MS Project (patrz 3.1.8). |

---

## 5. Podsumowanie

### Spełnione (✅) – 6 pozycji
1. Stakeholder Analysis (empatyzacja – ponad standard)
2. Kosztorys z referencjami (CAPEX/OPEX/TCO, benchmarki, scenariusze – ponad standard)
3. Opis problemu / analiza as-is
4. Wymagania funkcjonalne i niefunkcjonalne
5. Opis funkcjonalności / use case'y / user stories
6. Założenia organizacyjne wdrożenia + bibliografia + strona tytułowa z autorami + podział pracy

### Częściowo spełnione (⚠️) – 8 pozycji
1. Idea przedsiębiorcza/społeczna (wdrożeniowa, nie startupowa)
2. Project Selection (brak scoring modelu z wagami)
3. Project Organization (brak struktury PM)
4. Makieci UI (zapowiedziane, brak w rozdziałach)
5. Ryzyko (tylko ryzyka kosztowe, brak rejestru ryzyk PM)
6. Jakość/odbiór/kryteria jakości (kryteria oceny są, planu jakości brak)
7. Raport finalny w formacie ITU (istnieje, wymaga przebudowy)
8. Prezentacje (istnieją, wymagają restrukturyzacji i potwierdzenia udziału wszystkich)

### Do wykonania od zera (❌) – kluczowe braki
1. **SDG** – wskazanie i uzasadnienie powiązania (SDG 3)
2. **Business Model Canvas** (+ ew. Value Proposition Canvas)
3. **Elevator Pitch**
4. **Draft WBS + pełny WBS ze słownikiem**
5. **RACI matrix**
6. **Team qualifications**
7. **Harmonogram PERT/CPM + Gantt w MS Project** (wzór w TR_artifacts)
8. **Resource Allocation / Levelling / Crashing**
9. **Earned Value Management**
10. **Pełny rejestr ryzyk projektowych** (P×W, właściciel, strategie)
11. **Plan komunikacji**
12. **Elementy agile** (uzasadnienie podejścia / backlog / retrospektywa)
13. **Deklaracje AI** (przez każdego członka, wzór w TR_artifacts)
14. **Uzupełnienie zespołu do 7–8 osób**
15. **Benchmark konkurencyjny po cechach** (nie tylko kosztowy)

### Rekomendowana kolejność prac przy przenoszeniu projektu PWr na ITU
1. Utworzyć scoring model dla wariantów (uzupełnienie selection) → 2. Napisać SDG mapping → 3. Zbudować BMC/Social BMC + elevator pitch → 4. Rozpisać WBS (na bazie kamieni milowych M0–M6 i rozdziałów) → 5. Zbudować RACI na bazie WBS i nowego składu zespołu → 6. Harmonogram MS Project na bazie WBS + resource levelling → 7. Rejestr ryzyk + plan komunikacji + sekcja EVM → 8. Kwalifikacje zespołu + struktura organizacyjna → 9. Deklaracje AI (każdego członka) → 10. Restrukturyzacja prezentacji proposal/final z przypisanymi mówcami.
