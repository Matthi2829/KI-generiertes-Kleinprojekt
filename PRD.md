---

# 📄 Product Requirements Document (PRD)

---

## 🧾 Product Name
**SmartCool – Digitale Lager- & Kühlschrankverwaltung für Hofläden**

---

## 📌 Overview
SmartCool ist ein einfaches, regelbasiertes System zur Verwaltung von Lager- und Kühlschrankbeständen in einem Hofladen. Es hilft dabei, Produkte zu überwachen, Ablaufdaten im Blick zu behalten und Nachbestellungen effizient zu planen.

Das System ersetzt keine komplexe ERP-Software, sondern bietet eine leicht verständliche Lösung für kleine Betriebe.

---

## ❗ Problem
Hofläden haben oft Probleme mit:

- unübersichtlichen Lagerbeständen  
- ablaufenden Lebensmitteln ohne rechtzeitigen Verkauf  
- manueller und fehleranfälliger Bestandskontrolle  
- fehlender Planung für Nachbestellungen  
- unnötiger Lebensmittelverschwendung  

---

## 💡 Solution
SmartCool löst diese Probleme durch ein strukturiertes, regelbasiertes System:

- zentrale Erfassung aller Produkte im Lager  
- automatische Überwachung von Haltbarkeitsdaten  
- klare Regeln für Warnungen und Aktionen (z. B. Rabatt bei bald ablaufenden Produkten)  
- einfache Auswertungen zu Verkauf und Bestand  
- Vorschläge basierend auf festen Logiken (keine KI, keine Vorhersagemodelle)  

---

## 👥 Target Users

- Hofladen-Betreiber  
- kleine landwirtschaftliche Direktvermarkter  
- Familienbetriebe mit Eigenproduktion  
- kleine regionale Lebensmittelgeschäfte  
- Betriebe ohne bestehende digitale Warenwirtschaft  

---

## ⚙️ Core Features

- 📦 Produktverwaltung (Name, Menge, Preis, Haltbarkeitsdatum)  
- 🏷️ Lagerübersicht in Echtzeit  
- ⏰ Ablaufdatum-Tracking  
- ⚠️ Regelbasierte Warnungen (z. B. „Produkt läuft in 2 Tagen ab“)  
- 💸 Rabattvorschläge auf Basis fixer Regeln (z. B. „< 2 Tage → 20% Rabatt“)  
- 🛒 Nachbestellvorschläge auf Basis Mindestbestand  
- 📊 Einfaches Dashboard mit Lagerstatus  
- 📈 Verkaufsübersicht (manuell oder importiert)  

---

## 🚫 Non-Goals

- keine künstliche Intelligenz oder Machine Learning  
- keine komplexe Prognose- oder Vorhersagefunktion  
- keine ERP-Integration für große Unternehmen  
- keine Automatisierung von Bestellungen bei Lieferanten  
- kein Online-Shop-System (optional später möglich)  

---

## 📈 Success Criteria

- Reduzierung von abgelaufenen Produkten  
- schnellere und einfachere Lagerverwaltung  
- weniger manuelle Fehler bei Beständen  
- bessere Übersicht über verfügbare Produkte  
- einfache Bedienbarkeit für nicht-technische Nutzer  
- regelmäßige Nutzung im Hofladen-Alltag  

---

## 🧰 Suggested Tech Stack

### Frontend
- React oder einfache Weboberfläche (HTML/CSS/JS)  
- alternativ: Excel-/Dashboard-Lösung  

### Backend
- Python (Flask / FastAPI) oder Node.js  
- einfache Regel-Logik (IF-ELSE Strukturen)  

### Database
- SQLite (lokal & einfach)  
- oder PostgreSQL (skalierbar)  

### Logic Layer
Regelbasierte Engine (keine KI), z. B.:

- IF Ablaufdatum < 2 Tage → Rabatt = 20%  
- IF Bestand < Mindestwert → Nachbestellung  

### Deployment (optional)
- lokal auf Hofladen-PC  
- oder Cloud (Render / Railway)  

---
