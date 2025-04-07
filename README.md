## 🇵🇱 Projekt: Analiza szeregów czasowych – akcje Coca-Cola (1962–2021)

W tym projekcie przeanalizowałem dane dotyczące **cen akcji Coca-Cola** z okresu od **2 stycznia 1962 roku do 17 grudnia 2021 roku**.  
Dane pochodzą ze strony [Kaggle](https://www.kaggle.com/datasets/meetnagadia/coco-cola-stock-data-19622021).  
Z uwagi na specyfikę rynku, dane obejmują jedynie sesje giełdowe (poniedziałek–piątek, bez dni wolnych).

---

### 📊 Cel projektu:
- Analiza szeregu czasowego cen akcji
- Identyfikacja trendu i sezonowości
- Sprawdzenie stacjonarności oraz właściwości reszt
- Budowa i ocena modelu prognostycznego (ARIMA)

---

### ⚙️ Technologie:
- **Język R**
- Pakiety: `forecast`, `tseries`, `fpp3`, `ggplot2`

---

### 🔍 Etapy analizy:
1. **Wczytanie i wstępna eksploracja danych**
2. **Wizualna analiza szeregu czasowego**
3. **Sprawdzenie właściwości szeregu**:
   - stacjonarność (analiza wykresów acf, średniej i wariancji ruchomej oraz test kpss)
   - obecność trendu i sezonowości
   - analiza reszt
4. **Dopasowanie modelu ARIMA**
5. **Prognoza cen akcji i ocena jakości predykcji**

---

### 📁 Struktura plików:
- `Coca_Cola_forecast.rmd` – skrypt z analizą i prognozą
- `COCO COLA.csv` – zbiór danych (jeśli dołączony)

---

### 🧠 Wnioski:
Model ARIMA pozwolił na stworzenie krótkoterminowej prognozy zmian cen akcji, dobrze odzwierciedlając ogólne trendy, nie radząc sobie z sezonowość szeregu. 
Należałoby spróbować dokonać prognozy przy pomocy modelu GARCH który lepiej radzi sobie w analizie zmienności cen instrumentów finansowych.

---

## 🇬🇧 Project: Time Series Analysis – Coca-Cola Stock Prices (1962–2021)

In this project, I analyzed **Coca-Cola stock price data** from **January 2, 1962 to December 17, 2021**.  
The dataset was sourced from [Kaggle](https://www.kaggle.com/datasets/meetnagadia/coco-cola-stock-data-19622021).  
Due to the nature of the stock market, the data includes only trading days (Monday–Friday, excluding holidays).

---

### 📊 Project Goals:
- Time series analysis of stock prices  
- Identifying trend and seasonality  
- Checking stationarity and residual properties  
- Building and evaluating a forecasting model (ARIMA)

---

### ⚙️ Technologies:
- **R programming language**  
- Packages: `forecast`, `tseries`, `fpp3`, `ggplot2`

---

### 🔍 Analysis Steps:
1. **Data import and initial exploration**  
2. **Visual analysis of the time series**  
3. **Checking series properties**:
   - stationarity (using ACF plots, rolling mean and variance, and KPSS test)
   - presence of trend and seasonality  
   - residual diagnostics  
4. **Fitting the ARIMA model**  
5. **Forecasting stock prices and evaluating prediction quality**

---

### 📁 File Structure:
- `Coca_Cola_forecast.rmd` – R Markdown script with analysis and forecasting  
- `COCO COLA.csv` – dataset file (if included)

---

### 🧠 Conclusions:
The ARIMA model enabled short-term forecasting of stock price changes, successfully capturing overall trends, but struggled with the seasonality of the series.
Further improvements could involve using a **GARCH model**, which is better suited for modeling the volatility of financial time series.
