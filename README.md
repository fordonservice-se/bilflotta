# 🚗 Bilflottehantering

En modern webbapplikation för att hantera företagets bilflotta med full funktionalitet för import, export och notifikationer.

## ✨ Funktioner

- ✅ **Hantera bilar** - Lägg till, redigera och ta bort fordon
- 📥 **Importera från Excel** - Massimportera hela bilflottan
- 📊 **Exportera till Excel & PDF** - Få ut rapporter enkelt
- 🔔 **Automatiska notifikationer** - Påminnelser 30 dagar innan besiktning/service
- 📸 **Bilduppladdning** - Ladda upp bilder på varje bil
- 🔍 **Sök & filtrera** - Hitta bilar snabbt
- 📱 **Responsiv design** - Funkar på mobil, surfplatta och dator

## 🚀 Kom igång

### Öppna lokalt

1. Ladda ner alla filer till samma mapp
2. Dubbelklicka på `index.html`
3. Appen öppnas i din webbläsare!

### Demo-inloggningar

- **Admin**: `admin` / `admin123`
- **Chef**: `chef` / `chef123`

## 📋 Excel-import

1. Klicka på "📋 Ladda ner mall" för att få en exempelfil
2. Fyll i dina bilar
3. Klicka på "📥 Importera Excel" och välj filen
4. Klart!

### Excel-format

Kolumnerna kan heta:
- Regnummer (RegNr, Reg, Registration)
- Märke (Make, Brand)
- Modell (Model)
- Enhet (Unit, Department)
- Placering (Location)
- Ansvarig Chef (Manager)
- Kontaktperson 1-3 (Contact 1-3)
- Besiktning (Inspection)
- Service (Service Date)

Datum i formatet: `2024-12-31` eller Excel-datumformat

## 💾 Data

Data sparas lokalt i webbläsarens localStorage. För att dela data mellan användare behöver du uppgradera till en molnlösning (Firebase, egen backend, etc).

## 🔒 Säkerhet

**OBS!** Demo-inloggningarna är endast för test. Ta bort eller ändra dessa innan du använder appen i produktion!

I `app.js`, raden ~15, ändra:
```javascript
const users = [
    { username: 'admin', password: 'admin123', name: 'Admin' }
];
