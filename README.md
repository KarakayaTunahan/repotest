# Autovermietung - Light

## FahrzeugProtocol.swift
### Protocol
- Protokoll "FahrzeugProtocol" welches Identifiable erbt
- associatedtype Fahrzeugart
- Ein fahrzeugart vom Typ Fahrzeugart
- Ein name vom Typ String
- preisProStunde vom Typ Double
- treibstoff vom Typ String

### Struct Auto, LKW, Motorrad
- Auto soll zusätzlich noch eine Variable türe beinhalten, welches vom Typ Int ist
- LKW soll zusätzlich noch eine Variable anhänger beinhalten, welches vom Typ Int ist
- berechneMiete soll den preisProStunde mal die Zeit zurückgeben
- Alle Structs sollen von dem erstellen „FahrzeugProtocol“ erben



## FahrzeugAnzeigeView.swift

- 3 Arrays in die View für die Weiterverarbeitung hineinkopieren (ggf. selber die Arrays erstellen)

```
private var autos = [Auto(fahrzeugart: "Kombi", name: "Volkswagen Golf GTI", preisProStunde: 23.0, treibstoff: "Diesel", türe: 5),Auto(fahrzeugart: "Liomsine", name: "BMW M3", preisProStunde: 33.0, treibstoff: "Diesel", türe: 4),Auto(fahrzeugart: "SUV", name: "Mercedes G Klasse", preisProStunde: 40.0, treibstoff: "Diesel", türe: 5)]

private var lkws = [LKW(fahrzeugart: "Groß", name: "Volvo C560", preisProStunde: 40.0, treibstoff: "Benzin", anhänger: 2),LKW(fahrzeugart: "Mittel", name: "MAN", preisProStunde: 50.0, treibstoff: "Benzin", anhänger: 1),LKW(fahrzeugart: "Klein", name: "Mercedes", preisProStunde: 30.0, treibstoff: "Diesel", anhänger: 0)]

private var motorräder = [Motorrad(fahrzeugart: "Touer", name: "KTM1290 Duke", preisProStunde: 13.0, treibstoff: "Benzin"),Motorrad(fahrzeugart: "Tourer", name: "HarleyDavidson Ultimate Black", preisProStunde: 30000.0, treibstoff: "Benzin")]
```

- Die View soll wie folgt aussehen:

![](https://cdn.discordapp.com/attachments/692705542405226587/929828967786115072/Bildschirmfoto_2022-01-09_um_21.08.12.png)


## MietWagenView.swift
- Dem MietWagenView als Generics <Datentyp: FahrzeugProtocol> um in Zukunft noch weitere Fahrzeuge hinzufügen zu können
- In der View soll der Name vom Fahrzeug und der Mietpreis, je nach eingegebener Stunde angezeigt werden
- Der Mietpreis soll auf zwei Nachkommastellen abgegrenzt werden
- Am Ende soll die View wie folgt aussehen:

![](https://cdn.discordapp.com/attachments/692705542405226587/929829267825627136/Bildschirmfoto_2022-01-09_um_21.09.25.png)




