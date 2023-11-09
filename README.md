# AutoUsate Database

## Descrizione
Questo database è progettato per memorizzare informazioni su auto usate messe in vendita da un concessionario.

## Struttura della Tabella

```sql
CREATE TABLE AutoUsate (
  id INIT AUTO_INCREMENT
  marca VARCHAR(255) NOT NULL, UNIQUE,
  Modello VARCHAR(255) NOT NULL, UNIQUE,
  AnnoFabbricazione YEAR NULL,
  Chilometraggio FLOAT(4, 2) NULL,
  Prezzo DECIMAL(10, 2) NULL,
  Descrizione TEXT NULL,
  DataInserimento DATETIME DEFAULT NOT NULL,
  NumeroProprietari INT NULL,
  Colore VARCHAR(255) NULL,
  TipoCarburante VARCHAR(20) NULL,
  TipoCambio VARCHAR(20) NULL,
  Cilindrata FLOAT(4, 2) NULL,
  Equipaggiamenti MEDIUMTEXT NULL,
  FotoPrincipale VARCHAR(255) NULL,
  ConsumoCitta FLOAT(4, 2) NULL,
  ConsumoAutostrada FLOAT(4, 2) NULL,
  PotenzaKW FLOAT(4, 2) NULL,
  NumeroPorte INT NULL,
  NumeroPosti INT NULL,
  AirbagNumero INT NULL,
  CondizioniGenerali LONGTEXT NULL,
  DataVendita DATETIME NULL,
);