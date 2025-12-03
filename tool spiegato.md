# 🎲 Fantacalcio Luck Analyzer

Analizza quanto la **fortuna** (o sfortuna) ha influenzato la tua stagione di fantacalcio!

## 🎯 Cosa fa questo tool?

Risponde a domande come:
- "Ho vinto perché sono bravo o perché sono stato fortunato?"
- "Meritavo di più in base ai punteggi che ho fatto?"
- "Chi è la squadra più costante? E chi è imprevedibile?"

## 📊 Funzionalità

| Sezione | Descrizione |
|---------|-------------|
| **📊 Fortuna** | Calcola i punti attesi vs reali per ogni squadra |
| **📈 Stats** | Media, best/worst performance, posizione media |
| **🔬 Pitagorica** | Formula pitagorica adattata al fantacalcio |
| **📅 Calendario** | Analisi difficoltà del calendario (Strength of Schedule) |
| **🏆 Top** | Classifiche speciali: fortunati, sfortunati, più punti |
| **🎰 What If** | Simulazione Monte Carlo con migliaia di calendari casuali |
| **⚔️ Scontri Virtuali** | Matrice completa con Kryptonite e Victims |
| **📉 Varianza** | Analisi consistenza: Floor, Ceiling, CV%, trend |

## 🚀 Come usarlo

1. **Online**: Visita il [link GitHub Pages](#) (da configurare)
2. **Locale**: Scarica `index.html` e aprilo nel browser

### Inserimento dati

1. Imposta il numero di giornate
2. Per ogni squadra inserisci:
   - Nome
   - Punteggio fantacalcio di ogni giornata
   - Vittorie e Pareggi reali
3. Clicca "🎯 Calcola"

### Importazione CSV

Puoi importare i dati da CSV in due formati:

**Formato Tabella:**
```csv
Nome,G1,G2,G3,Vinte,Pareggi
Squadra A,72,68,75,5,2
Squadra B,65,70,72,4,3
```

**Formato Calendario:**
```csv
Giornata,HomeTeam,AwayTeam,HomePts,AwayPts,Result
1,Squadra A,Squadra B,72,68,H
1,Squadra C,Squadra D,70,70,D
```

## 📖 Spiegazione delle metriche

### Fortuna
- **Punti Attesi**: punti che avresti meritato giocando contro tutti ogni giornata
- **Fortuna = Punti Reali - Punti Attesi**
- Positiva = fortunato, Negativa = sfortunato

### Pitagorica
Formula: `Win% = PF^2.37 / (PF^2.37 + PS^2.37)`
- Predice le vittorie basandosi solo su punti fatti/subiti
- Esponente 2.37 ottimizzato per il fantacalcio

### Simulazione Monte Carlo
- Genera migliaia di calendari casuali
- Mantiene i punteggi reali, rimescola gli accoppiamenti
- **Luck Index (σ)**: quante deviazioni standard sei sopra/sotto la media

### Varianza
- **CV% (Coefficiente di Variazione)**: più basso = più costante
- **IQR**: dove cade il 50% centrale dei tuoi punteggi
- Classificazione: 🎯 Ultra Affidabile → 🎢 Rollercoaster

## 🛠️ Tecnologie

- HTML5 / CSS3 / JavaScript vanilla
- Nessuna dipendenza esterna
- Funziona offline
- Mobile responsive

## 📄 Licenza

MIT License - Usalo liberamente!

## 🤝 Contributi

Suggerimenti e miglioramenti sono benvenuti! Apri una Issue o una Pull Request.

---

Made with ❤️ per i fantacalcisti italiani
