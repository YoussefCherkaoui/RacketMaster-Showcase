# 🎾 Racket Master Score

![Swift](https://img.shields.io/badge/Swift-5.9-orange.svg)
![Platform](https://img.shields.io/badge/Platform-iOS%20%7C%20watchOS-lightgrey.svg)
![Framework](https://img.shields.io/badge/Framework-SwiftUI-blue.svg)

**Dall'idea al codice: l'evoluzione del segnapunti per il tennis.**

Questo progetto nasce da un concept originale di **Fabio Bernardi**. Il mio ruolo è stato quello di trasformare la sua visione in un'applicazione reale, nativa e performante, arricchendola con funzionalità tecniche avanzate come il monitoraggio della salute e l'assistente vocale.

---

## 📱 Anteprima del Progetto
-<img width="1206" height="2622" alt="Simulator Screenshot - iPhone 17 - 2025-12-24 at 12 06 14" src="https://github.com/user-attachments/assets/942baa7b-c1c0-4f6e-8be0-db7eb4a10355" />
<img width="1206" height="2622" alt="Simulator Screenshot - iPhone 17 - 2025-12-24 at 12 06 02" src="https://github.com/user-attachments/assets/bcb05d4b-f36f-4cd1-9b2e-dc52f96d0592" />
<img width="1206" height="2622" alt="Simulator Screenshot - iPhone 17 - 2025-12-24 at 12 06 27" src="https://github.com/user-attachments/assets/1ebab6bf-7ef8-4acc-8a1e-c8aa51648745" />
<img width="1206" height="2622" alt="Simulator Screenshot - iPhone 17 - 2025-12-24 at 12 07 05" src="https://github.com/user-attachments/assets/7c266f95-e729-46fd-8d96-7678202ed484" />
<img width="416" height="496" alt="Simulator Screenshot - Apple Watch Series 11 (46mm) - 2025-12-24 at 12 07 51" src="https://github.com/user-attachments/assets/2dc00aa1-782f-4be4-929b-f79c9f8db2f2" />
<img width="416" height="496" alt="Simulator Screenshot - Apple Watch Series 11 (46mm) - 2025-12-24 at 12 08 37" src="https://github.com/user-attachments/assets/773d9fef-382d-495b-b3ff-cdb9e4839fda" />




---

## 🚀 Il Mio Contributo Tecnico


Oltre a implementare l'intera logica di base richiesta da Fabio, ho voluto espandere il progetto aggiungendo personalmente queste funzionalità chiave:

* **🗣️ Arbitro Vocale (My Feature):** Ho integrato `AVFoundation` per dare voce all'app. Ora l'iPhone annuncia il punteggio (es. *"Quindici a Zero"*) rispettando la regola del server. Ho aggiunto anche un toggle per disattivarlo.
* **❤️ Integrazione HealthKit (My Feature):** Ho voluto che l'app fosse anche un tracker di fitness. Durante la partita, l'Apple Watch monitora battito cardiaco e calorie, salvando la sessione nell'app Salute.
* **📜 Storico Partite (My Feature):** Ho creato un sistema di archiviazione locale (`UserDefaults` + `Codable`) per salvare ogni partita conclusa in un database consultabile, creando una "bacheca dei trofei" per il giocatore.

---

## ✨ Funzionalità Core

Naturalmente, l'app include tutte le solide basi previste dal design originale:

* **🔄 Sincronizzazione Totale:** Utilizzo di `WatchConnectivity` per tenere allineati iPhone e Watch in tempo reale.
* **🛡️ Sistema "Paracadute":** Salvataggio automatico dello stato ad ogni punto. Se l'app si chiude, alla riapertura la partita riprende esattamente da dove era rimasta.
* **↩️ Funzione Undo:** Possibilità di annullare l'ultimo punto in caso di errore.
* **📢 Arbitro Logico:** Gestione automatica di Tie-Break, cambi campo e vantaggi.

---

## 🛠 Tecnologia Utilizzata

L'intero progetto è scritto in **Swift** e **SwiftUI**.
* **Architettura:** MVVM (Model-View-ViewModel) per una separazione pulita del codice.
* **Frameworks:** SwiftUI, WatchKit, HealthKit, AVFoundation.

---

## 👥 Crediti

* **Concept & Idea Originale:** Fabio Bernardi
* **Sviluppo iOS/watchOS & Nuove Features:** Youssef Cherkaoui

---
*Nota: Questa è una demo showcase. Il codice sorgente è privato.*
