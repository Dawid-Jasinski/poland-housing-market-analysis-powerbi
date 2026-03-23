# Poland Housing Market Analysis (2013–2023) – Power BI Dashboard
Author: Dawid Jasiński 
---
Technologies: Power BI Desktop, Power Query, Excel 
---
Source: GUS
---

## 📁 8. Struktura repozytorium
```
poland-housing-market-analysis-powerbi 
│── README.md 
│── dashboard-poland-housing-market-analysis.pbix
│── /data
│   ├── Dane.xlsx
│   ├── Liczba i kwoty wypłaconych dodatków mieszkaniowych użytkownikom lokali.xlsx
│   ├── Liczba lokali mieszkalnych sprzedanych w ramach transakcji rynkowych.xlsx
│   ├── Mieszkania oddane do użytkowania.xlsx
│   ├── Remonty mieszkań.xlsx
│   ├── Zasoby mieszkaniowe.xlsx
│── /results
│   ├── dashboard-poland-housing-market-analysis.pdf
```
--- 


## 🏢 1. Cel biznesowy
Celem projektu jest przeprowadzenie kompleksowej analizy rynku mieszkaniowego w Polsce w latach 2013-2023, obejmującej zarówno zasoby mieszkaniowe, jak i aktywność inwestycyjną oraz poziom wydatków publicznych.  
Analiza ma odpowiedzieć na pytania dotyczące dynamiki podaży mieszkań, tempa remontów zasobów komunalnych oraz efektywności wydatków mieszkaniowych w różnych powiatach.

Projekt został wykonany w Power BI jako studium przypadku typu housing market intelligence, które mogłoby wspierać:
- jednostki samorządowe,  
- organizacje publiczne,  
- analityków rynku nieruchomości.

---

## 📊 2. Zakres analizy
Projekt obejmuje następujące obszary:

- **Zasoby mieszkaniowe** (liczba mieszkań w powiatach)
- **Mieszkania oddane do użytkowania** (trend 2013–2023)
- **Sprzedaż rynkowa lokali** (aktywność popytowa)
- **Remonty mieszkań komunalnych** (2013–2022)
- **Kwoty wypłaconych dodatków mieszkaniowych** (2016–2023)
- **Porównania regionalne na poziomie powiatów**
- **Zmiana zasobów mieszkaniowych między 2013 a 2023**

Dashboard umożliwia filtrowanie danych po:
- powiecie,
- roku.

---

## 🗂 3. Źródła danych
Dane pochodzą z **GUS (Główny Urząd Statystyczny)** i obejmują oficjalne statystyki mieszkaniowe publikowane w latach 2013–2023.

Zestawy danych połączono w jedną strukturę analityczną, aby umożliwić agregację, porównania i modelowanie trendów.

---

## 🔧 4. Przygotowanie danych (ETL – Power Query)
W ramach modelowania danych wykonano:

### **Integrację rozproszonych plików**
- połączenie wielu arkuszy z różnych lat,
- standardyzację nazw kolumn,
- sprowadzenie lat do jednej kolumny typu „Year”.

### **Usuwanie braków i ujednolicanie struktur**
- identyfikacja brakujących obserwacji,
- usunięcie lat z niekompletnymi danymi,
- konwersje typów liczbowych.

### **Budowa relacji**
Model oparto na jednej głównej tabeli faktów oraz kilku wymiarach (Powiat, Rok).

---

## 📌 5. Kluczowe wskaźniki 

### **Zmiana zasobów mieszkaniowych (2013 - 2023)**  
Pokazuje różnicę w liczbie mieszkań w danym powiecie na przestrzeni 10 lat.

### **Mieszkania oddane do użytkowania**  
Trend budownictwa mieszkaniowego.

### **Dynamika wydatków mieszkaniowych**  
Analiza zmian kwot dodatków mieszkaniowych wypłacanych gospodarstwom domowym.

### **Remonty zasobów komunalnych**  
Łączna liczba remontów jako wskaźnik modernizacji zasobów publicznych.

---

## 📈 6. Najważniejsze wnioski biznesowe

### **Rosnące zasoby mieszkaniowe, ale duże różnice regionalne**
W większości powiatów odnotowano wzrost liczby mieszkań, lecz tempo przyrostu jest nierównomierne. Największe wzrosty koncentrują się w miastach wojewódzkich.

### **Zmienna dynamika oddawania nowych mieszkań**
W latach 2020–2022 tempo budowy mieszkań osiągnęło najwyższe wartości, natomiast lata wcześniejsze charakteryzowały się niższą aktywnością inwestorów.

### **Wydatki mieszkaniowe rosną szybciej niż efekty inwestycyjne**
Kwoty dodatków mieszkaniowych wykazują trend wzrostowy, jednak wzrost ten nie przekłada się proporcjonalnie na poprawę jakości zasobów komunalnych.

### **Remonty mieszkań komunalnych mają charakter cykliczny**
Liczba przeprowadzonych remontów znacząco różni się między latami, co może wskazywać na zmienność budżetową lub zależność od programów centralnych.

---

## 🧭 7. Rekomendacje

**Uzupełnienie analizy o dane społeczno ekonomiczne**
- wynagrodzenia,  
- migracje,  
- demografia,  
- bezrobocie.  
Pozwoliłoby to ocenić, czy budownictwo odpowiada na zmiany w popycie.

**Włączenie wskaźników efektywności inwestycji publicznych**
Zestawienie wydatków mieszkaniowych z efektami (mieszkania komunalne, remonty).

**Możliwość zbudowania modelu prognostycznego**




