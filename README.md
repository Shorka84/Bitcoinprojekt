# Bitcoin Data pipeline för AI/ML

## 🎯 Mål
Hämta hem bitcoin data och validera samt normalisera den. Även beräkning av medelvärden samt skicka ut en linjegaf.

## 🛠️ Metod
*   **Datahämtning**: Använder CoinGecko API
*   **Datahantering**: Sparar rådata i `JSON` och bearbetad data i `CSV` (`pandas`).
*   **Feature Engineering**: Beräknar `MA20`, `MA50` och volatilitet. Medelvärden, Detta för att kunna beräkna risk för investerare.
*   **Visualiserar datan med matplotlib**
*   **Normalisering**: Skalar data med `MinMaxScaler` (`sklearn`) inför ML/AI.
*   **Felhantering**: `try-except` för API-anrop och filåtgärder.

## 📊 Resultat
Två huvudfiler genereras:
*   `data/bitcoin_raw.json`: Rådata från API.
*   `data/bitcoin_processed.csv`: Normaliserad och bearbetad data, redo för ML/AI.
*   Skriver ut en linjegraf med Matplotlib för att kunna se trenden klart och tydligt.

## 📈 Analys
*   Ger en stabil grund för AI-utveckling.
*   Minimerar problem som ofta uppstår i ML-projekt.
*   Gör det lättare att träna modeller effektivt.

## 💡 Reflektion
Projektet visar integrationen av API, Pandas, OOP och ML-förberedelse framgångsrikt.

**Vad var svårt?**
*   Att hantera tidsseriedata och få rätt tidsstämplar och sortering.
*   Att beräkna glidande medelvärden och volatilitet, eftersom det skapar tomma värden i början.
*   Att balansera felhantering med att koden fortfarande är lätt att läsa.
*   Att designa klasserna så att de fungerar bra för både allmän och specifik Bitcoin-data.

**Vad skulle jag göra annorlunda?**
*   Detta projekt känns för avancerat en grundkurs.
*   Men i ett större projekt skulle jag kanske bryta ut koden i fler mindre delar (moduler) för att göra det mer organiserat.
*   Jag skulle också kunna lägga till ännu mer avancerade beräkningar eller fler visualiseringar.

## 🔗 GitHub-länk
(https://github.com/Shorka84/Bitcoinprojekt)
## ⚙️ Installation & Körning
1.  **Klona repositoryt**.
2.  **Installera bibliotek**: `pip install requests pandas scikit-learn`
3.  **Kör i anteckningsboken** sekventiellt i Google Colab eller Jupyter.
