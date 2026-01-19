# SARIMA-Analiza-stopy-bezrobocia
Projekt zaliczeniowy z analizy danych z AI - prognoza bezrobocia modelem SARIMA
# Analiza i Prognoza Stopy Bezrobocia w Polsce (2001-2026)

##  Opis Projektu
Celem projektu była analiza stopy bezrobocia rejestrowanego w Polsce na przestrzeni ostatnich 25 lat oraz stworzenie modelu prognostycznego. Projekt bada sezonowość rynku pracy, wpływ wejścia do UE oraz pandemii COVID-19 na gospodarkę.

##  Technologie i Narzędzia
* **Język:** Python 3.x
* **Środowisko:** Jupyter Notebook
* **Biblioteki:**
  * `pandas`, `numpy` (przetwarzanie danych)
  * `matplotlib`, `seaborn` (wizualizacja)
  * `pmdarima` (automatyczny dobór modelu SARIMA)
  * `statsmodels` (dekompozycja szeregów czasowych)

## Żródło Danych
Dane pochodzą z Głównego Urzędu Statystycznego (GUS) i obejmują miesięczną stopę bezrobocia rejestrowanego w latach 2001–2025. Dane zostały przetworzone do formatu szeregu czasowego.

##  Główne Wnioski
1. Transformacja trendu: Analiza wykazała przejście polskiego rynku pracy od wysokiego bezrobocia strukturalnego (ponad 20% w 2003 r.) do niskiego bezrobocia frykcyjnego (ok. 5% w 2024 r.), z kluczowym momentem przełomowym po wejściu do UE.
2. Istotność sezonowości: Zidentyfikowano statystycznie istotny komponent sezonowy, skorelowany z cyklem pór roku, co uzasadniło wybór modelu klasy SARIMA zamiast standardowej ARIMY.
3. Wyniki modelu: Model SARIMA osiągnął zadowalające metryki błędu (niskie MAE) na zbiorze walidacyjnym, poprawnie odwzorowując lokalne ekstrema.
4. Perspektywy: Prognoza na rok 2026 zakłada kontynuację stabilizacji wskaźnika bezrobocia z zachowaniem rocznej cykliczności wahań.
