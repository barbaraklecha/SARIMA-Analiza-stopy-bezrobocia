# Analiza i Prognoza Stopy Bezrobocia w Polsce (2001-2026)

##  Opis Projektu
Celem projektu była analiza stopy bezrobocia rejestrowanego w Polsce na przestrzeni ostatnich 25 lat oraz stworzenie modelu prognostycznego. Projekt bada sezonowość rynku pracy, wpływ wejścia do UE oraz pandemii COVID-19 na gospodarkę.

##  Technologie i Narzędzia
* **Język:** Python 3.x
* **Środowisko:** Jupyter Notebook
* **Biblioteki:**
  * `pandas`, `numpy` (przetwarzanie danych)
  * `matplotlib`, `seaborn` (wizualizacja)
  * `pmdarima` (automatyczny dobór modelu SARIMA) - automatycznie identyfikuje optymalną konfigurację SARIMA poprzez minimalizację kryterium informacyjnego AIC.(https://www.rdocumentation.org/packages/forecast/versions/8.24.0/topics/auto.arima)
  * `statsmodels` (dekompozycja szeregów czasowych)

## Żródło Danych
Dane pochodzą z Głównego Urzędu Statystycznego (GUS) i obejmują miesięczną stopę bezrobocia rejestrowanego w latach 2001–2025. Dane zostały przetworzone do formatu szeregu czasowego.

##  Główne Wnioski
1. Analiza historii z lat 2001–2025 pokazuje dwie zupełnie różne epoki w polskiej gospodarcze. Na początku wieku zmagaliśmy się z gigantycznym bezrobociem (sięgającym 20%). Punktem zwrotnym było wejście Polski do Unii Europejskiej – od tego momentu bezrobocie systematycznie spadało i obecnie utrzymuje się na stabilnym, niskim poziomie.
2. Dane potwierdziły to, co obserwujemy na co dzień – bezrobocie w Polsce zawsze rośnie zimą (gdy stają budowy i rolnictwo) i spada latem. Właśnie dlatego wybrano model SARIMA. W przeciwieństwie do prostszych modeli, ten "rozumie" pory roku i nie traktuje zimowego wzrostu jako kryzysu, lecz jako naturalne zjawisko.
3. Model został on sprawdzony na danych z ostatnich 2 lat (tzw. test wsteczny). Porównanie prognozy z rzeczywistością pokazało, że model myli się średnio o zaledwie 0.31 punktu procentowego. Tak mały błąd to twardy dowód na to, że model jest precyzyjny i można mu zaufać.
4. Model przewiduje spokój i stabilizację. W 2026 roku nie spodziewamy się żadnych nagłych wstrząsów - lekki, sezonowy wzrost bezrobocia w pierwszym kwartale, a następnie spadki w miesiącach letnich – dokładnie tak, jak w latach poprzednich.


