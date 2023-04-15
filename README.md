# Strings
## Cos'è:
Strings è un programma C# per lo studio delle stringhe senza l'ausilio della classe StringBuilder e dei metodi predefiniti forniti dalle librerie di C#. Nella scrittura di questo progamma abbiamo immaginato di troarci in un ambiente di sviluppo completamente privo di qualsiasi vantaggio fornito da C#, python o C++.
Tutte le funzioni necessarie quali String.Length(), String.ToUpper() ed analoghe sono state ricreate completamente tramite l'uso di operatori Bit a Bit e dei cicli forniti; di seguito un esempio:

```
  public static char ToUpper(char c)
  {
      if (c >= 'a' && c <= 'z')
          c = (Char)(c & 0x5f);
      return c;
  }
  ```

Lo scopo di questo esercizio è la consolidazione delle conoscense sui vettori, sui cicli, sulla tabella ASCII e sulla mascheratura dei bit mediante gli operatori '&', '|' e '^'.
In questo esercizio dovranno essere presenti funzioni per la manipolazione di stringhe e la loro analisi:

Funzioni per la manipolazione:
* stringa tutta in maiuscolo;
* stringa tutta in minnuscolo;
* stringa capitalizzata;
* stringa inversa.

Funzioni per l'analisi:
* se è alfabetica;
* se è alfanumerica;
* se è palindroma;
* la quantità di lettere;
* la quantità di parole.

**NOTA BENE: le funzioni non potranno lavorare sulle stringhe, ma dovranno lavorare su array di char creati mediante la funzione String.ToCharArray().**

**È consentito l'uso della funzione String.ToCharArray() per la trasformazione della stringa in array di char e la creazione di una nuova stringa a partire dall'array per il risultato della funzione.**

Esempio:
  ```
  public string UpperOutput(string input)
  {
      char[] caratteri = input.ToCharArray();
      for (int i = 0; i < lunghezza(input); i++)
          caratteri[i] = ToUpper(caratteri[i]);
      //Creazione di una nuova stringa mediante la creazione di una nuova istanza della classe System.String.
      return new String(caratteri);
  }
```
Di seguito viene allegato il [link](https://classroom.google.com/u/1/c/NTQ4MDI3ODM0Nzgw/a/NTk2NTAzNjU5ODU1/details).
## Change Log
**NOTA BENE: nei change log saranno inserite solo i cambiamenti riguardanti le funzioni e gli elementi del codice effettivamente modificati.**
