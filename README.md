# Ada Projects

Benvenuto in **Ada Projects**! Questo repository contiene una raccolta di progetti di esempio scritti nel linguaggio di programmazione **Ada**, sviluppati durante l'attività lavorativa. L'obiettivo è fornire esempi pratici e funzionanti per chi si avvicina ad Ada o desidera vedere applicazioni concrete.

## 📁 Struttura del Progetto

Al momento, il repository contiene il seguente progetto:

*   **`hello/`**: Directory che contiene il classico programma "Hello, World!" in Ada. È il punto di partenza ideale per verificare la corretta configurazione dell'ambiente di sviluppo e compilazione.

## 🚀 Istruzioni per l'Installazione e l'Uso (su CentOS 7)

Le istruzioni seguenti sono state testate su un sistema **CentOS 7**, ma dovrebbero essere simili per altre distribuzioni Linux.

### 1. Prerequisiti: Installazione degli Strumenti di Sviluppo

Prima di tutto, aggiorna il sistema e installa il gruppo di strumenti di sviluppo, che include **gcc** (il compilatore GNU) e **gnatmake** (il build tool per Ada).

```bash
# Aggiorna i pacchetti del sistema
sudo yum update

# Installa il gruppo "Development Tools" (include gcc, gnat, make, ecc.)
sudo yum group install "Development Tools"
```

### 2. Verifica delle Versioni Installate (Opzionale)

Per assicurarti che gli strumenti siano installati correttamente, puoi controllare le versioni:

```bash
gcc --version      # Dovresti vedere la versione di GCC
gnatmake --version # Dovresti vedere la versione di GNAT (Ada)
git --version      # Versione di Git, se necessario
```

### 3. Clonare il Repository e Compilare il Progetto

```bash
# Clona il repository
git clone https://github.com/msabetta/ada_projects.git

# Entra nella directory del progetto "hello"
cd ada_projects/hello

# Compila il file Ada (due modi equivalenti)
# 1. Compilazione separata (produce file oggetto .o)
gcc -c helloworld.adb
# 2. Build completa (link ed eseguibile finale)
gnatmake helloworld.adb
```

### 4. Eseguire il Programma

Dopo la compilazione, troverai un eseguibile con lo stesso nome del file sorgente (senza estensione). Eseguilo:

```bash
./helloworld
```

Dovresti vedere il messaggio:
```
Hello, world!
```

## 📦 Esempi Inclusi

### Hello World (`/hello/helloworld.adb`)
Questo semplice programma dimostra la struttura base di un'applicazione Ada:
*   Dichiarazione del procedimento principale (`procedure HelloWorld is ...`).
*   Uso della libreria `Ada.Text_IO` per l'input/output.
*   La funzione `Put_Line` per stampare una stringa a video.

```ada
with Ada.Text_IO;

procedure HelloWorld is
begin
   Ada.Text_IO.Put_Line("Hello, world!");
end HelloWorld;
```

## 🛠️ Prossimi Progetti

Nei prossimi commit, il repository potrebbe essere arricchito con nuovi esempi, come:
*   Gestione di tipi di dati e record.
*   Programmazione concorrente con task Ada.
*   Esempi di interfacciamento con librerie C.
*   Progetti più complessi tratti dall'esperienza lavorativa.

## 📚 Risorse Utili per Imparare Ada

*   [Learn Ada](https://learn.adacore.com/) - Corso interattivo ufficiale di AdaCore.
*   [Ada Reference Manual](http://www.ada-auth.org/standards/rm12_w_tc1/html/RM-TOC.html) - Il manuale di riferimento del linguaggio.
*   [Rosetta Code: Ada](https://rosettacode.org/wiki/Category:Ada) - Esempi di codice per problemi comuni.

Spero che questo README sia chiaro e completo. Se in futuro verranno aggiunti altri progetti nella cartella `ada_projects`, ti consiglio di aggiornare la sezione "Esempi Inclusi" per elencarli brevemente, magari con una riga di descrizione ciascuno.
