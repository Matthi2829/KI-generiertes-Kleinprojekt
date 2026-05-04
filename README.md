```markdown
# 🤖 KI-Kleinprojekt: Intelligente Kühlschrank- und Lagerverwaltung im Hofladen

---

## 💡 Idee
Entwicklung eines KI-gestützten Systems zur Verwaltung von Lager- und Kühlschrankbeständen in einem Hofladen, um Lebensmittel effizient zu nutzen und Verluste durch Verderb zu reduzieren.

---

## ❗ Problem
In Hofläden entstehen häufig Verluste, weil:

- Produkte zu spät verkauft werden  
- Ablaufdaten nicht rechtzeitig beachtet werden  
- Überproduktion oder falsche Nachbestellungen passieren  

---

## 🎯 Ziel
Das System soll:

- ablaufende Produkte frühzeitig erkennen  
- Lagerbestände optimieren  
- Nachbestellungen verbessern  
- Lebensmittelverschwendung reduzieren  
- wirtschaftliche Entscheidungen unterstützen  

---

## 🧠 Core Use Cases

- 🔍 Erkennung bald ablaufender Produkte  
- ⚠️ Warnung bei kritischen Lagerbeständen  
- 💸 Vorschläge für Rabattaktionen  
- 🛒 Empfehlung für Nachbestellungen  
- 📊 Analyse von Verkaufsdaten zur Optimierung  



# 🧑‍🌾 User Stories & Tasks

---

## 1. Produktverwaltung

### 🧑 User Story
Als Hofladen-Betreiber möchte ich Produkte mit Name, Menge, Preis und Haltbarkeitsdatum erfassen, damit ich einen Überblick über mein Lager habe.

### 🔧 Tasks

- Datenbanktabelle `products` erstellen  
- Felder definieren:
  - id  
  - name  
  - quantity  
  - price  
  - expiry_date  
- CRUD-API erstellen:
  - Produkt anlegen  
  - Produkt anzeigen  
  - Produkt aktualisieren  
  - Produkt löschen  
- Einfaches Eingabeformular im Frontend erstellen  

---

## 2. Lagerübersicht anzeigen

### 🧑 User Story
Als Betreiber möchte ich alle Produkte in einer Liste sehen, damit ich jederzeit weiß, was im Lager ist.

### 🔧 Tasks

- API Endpoint erstellen: `GET /products`  
- Frontend-Tabelle erstellen  
- Sortierung implementieren:
  - nach Ablaufdatum  
  - nach Menge  
- Filterfunktion hinzufügen:
  - z. B. nur ablaufende Produkte anzeigen  
```
