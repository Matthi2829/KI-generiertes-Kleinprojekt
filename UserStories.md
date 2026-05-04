# 🧑‍🌾 User Stories – SmartCool (Hofladen Lagerverwaltung)

---

## 1. Produktverwaltung

### 🧑 User Story  
Als Hofladen-Betreiber möchte ich Produkte mit Name, Menge, Preis und Haltbarkeitsdatum erfassen, damit ich einen vollständigen Überblick über meinen Lagerbestand habe.

### 🔧 Tasks  
- Datenbanktabelle `products` erstellen  
- Felder definieren:  
  - id  
  - name  
  - quantity  
  - price  
  - expiry_date  
- CRUD-API implementieren:  
  - Produkt anlegen  
  - Produkt anzeigen  
  - Produkt aktualisieren  
  - Produkt löschen  
- Einfaches Eingabeformular im Frontend erstellen  

---

## 2. Lagerübersicht anzeigen

### 🧑 User Story  
Als Betreiber möchte ich alle Produkte in einer übersichtlichen Liste sehen, damit ich jederzeit weiß, welche Waren im Lager verfügbar sind.

### 🔧 Tasks  
- API Endpoint erstellen: `GET /products`  
- Frontend-Tabelle zur Anzeige der Produkte erstellen  
- Sortierung implementieren:  
  - nach Ablaufdatum  
  - nach Menge  
- Filterfunktion hinzufügen:  
  - z. B. nur Produkte anzeigen, die bald ablaufen  

---

## 3. Ablaufdatum-Überwachung

### 🧑 User Story  
Als Betreiber möchte ich erkennen, welche Produkte bald ablaufen, damit ich rechtzeitig Maßnahmen ergreifen und Verluste vermeiden kann.

### 🔧 Tasks  
- Logik zur Berechnung der verbleibenden Haltbarkeit implementieren  
- Regel definieren:  
  - < 2 Tage → kritisch  
  - < 5 Tage → Warnung  
- UI-Markierung einbauen:  
  - rot = kritisch  
  - gelb = bald ablaufend  
- Filter: „nur kritische Produkte anzeigen“  

---

## 4. Bestandskontrolle & Nachbestellung

### 🧑 User Story  
Als Betreiber möchte ich informiert werden, wenn der Bestand eines Produkts unter einen Mindestwert fällt, damit ich rechtzeitig nachbestellen kann.

### 🔧 Tasks  
- Feld `min_stock` zur Produktstruktur hinzufügen  
- Regel implementieren:  
  - IF quantity < min_stock → Warnung ausgeben  
- UI-Hinweis hinzufügen: „Nachbestellen erforderlich“  
- Filter für „unter Mindestbestand“ erstellen  

---

## 5. Rabatt- und Verkaufsunterstützung

### 🧑 User Story  
Als Betreiber möchte ich Empfehlungen für Rabatte auf Produkte erhalten, die bald ablaufen, damit ich diese schneller verkaufen und Lebensmittelverschwendung reduzieren kann.

### 🔧 Tasks  
- Regel definieren:  
  - IF expiry_date ≤ 2 Tage → Rabatt = 20%  
- Rabattfeld berechnen oder dynamisch anzeigen  
- UI-Anzeige für empfohlene Aktionen erstellen  
- Badge hinzufügen: „Aktion empfohlen“  
