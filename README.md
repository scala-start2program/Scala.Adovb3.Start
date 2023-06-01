# Voorbeeld 3  

Deze keer gaan we gegevens bijhouden van elektro toestellen.  
Je gaat terug zelf op SQL Server een nieuwe dtabase aanmaken.  
  
  * Naam database = **ScalaAdovb2**  
  * Je maakt in deze database 1 tabel aan met de naam **Toestellen**  
  * In deze tabel maak je volgende kolommen aan :   
    * **Id** : nvarchar(50), primaire sleutel  
    * **Merk** : nvarchar(50), vereist  
    * **Serie** : nvarchar(50), vereist  
    * **Prijs** : decimal(18,2), vereist  
    * **Stock** : int, vereist  
    * **Soort** : nvarchar(50), vereist  
  
In de starterscode zit enkel een WPF project (XAML code + event handlers)  
Je maak dus zelf een class-library aan : **Scala.Adovb3.Core**  
Je voegt 2 mapjes toe aan deze class-library : **Entities** en **Services**  
Kopieer uit een voorgaand project of uit de cursus de klassen **Helper** en **DBServices** (en plaats die in de mapjes in het mapje **Services**) : pas in **Helper** de connectiestring aan.  
Installeer via Nuget Packages **System.Data.SqlClient**  
Voorzie in het mapje **Entities** 1 entiteitsklasse **Toestel** die een weerspiegeling is van de tabel die je zonet maakte.  
Voorzie in het mapje **Services** nog een klasse **ToestelService** die :  
  * De beschikbare toestellen aanlevert, al dan niet gefilterd op soort.  
  * Een toestel toevoegt  
  * Een toestel wijzigt  
  * Een toestel verwijdert  
  * De totale stockwaarde berekent (prijs * stock van alle toestellen samen)  
  
Het WPF project ligt voor de hand : toestellen afbeelden, toevoegen, wijzigen en verwijderen.
Bijkomend : toestellen moeten kunnen gefilterd worden op soort. We voorzien hiervoor een combobox (cmbFilter) waarin we tijdens het opstarten 5 waarden steken :
  * Vaatwas  
  * Wasmachine  
  * Droogkast  
  * Diepvries  
  * Ijskast  
  
De code wordt uiteraard uitvoerig tijdens de les besproken.  
