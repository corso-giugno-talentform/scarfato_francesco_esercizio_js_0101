## 2025 07 01 - Prima lezione su JavaScript

JavaScript è un linguaggio di programmazione interpretato che consente di rendere le pagine web interattive e dinamiche. È uno dei tre pilastri dello sviluppo web insieme a HTML e CSS.

**Caratteristiche principali:**

- Linguaggio interpretato (non compilato)
- Eseguito direttamente nel browser
- Sintassi flessibile e dinamica
- Ampiamente supportato

### **Come inserire JavaScript**

Ci sono tre modi per includere JavaScript:

1. **Inline** (sconsigliato):

```html
<button onclick="alert('Ciao!')">Clicca</button>

```

1. **Interno**:

```html
<!DOCTYPE html>
<html>
<head>
    <script>
        console.log("Hello, world!");
    </script>
</head>
<body>
    <h1>La mia pagina</h1>
</body>
</html>

```

1. **Esterno** (consigliato):

```html
<!DOCTYPE html>
<html>
<head>
    <title>JavaScript Esterno</title>
</head>
<body>
    <h1>La mia pagina</h1>
    <script src="script.js"></script>
</body>
</html>

```

### **La Console del Browser**

La console è uno strumento fondamentale per il debugging:

- **Chrome**: Ctrl + Shift + J (Windows) / Cmd + Option + J (Mac)
- **Firefox**: Ctrl + Shift + K (Windows) / Cmd + Option + K (Mac)

```jsx
console.log("Questo messaggio apparirà nella console");

```

### **Capitolo 2: Variabili e Costanti**

Le variabili sono "contenitori" che memorizzano valori. In JavaScript moderno utilizziamo `let` per le variabili e `const` per le costanti.

### **Dichiarazione di Variabili**

```jsx
// Dichiarazione
//var nome; vecchio metodo
let nome;

// Assegnazione
nome = "Mario";

// Dichiarazione e inizializzazione
let eta = 25;
let cognome = "Rossi";

console.log("Ciao mi chiamo "+ nome+' '+cognome+'. Ho '+ eta+ ' anni');

```

### **Dichiarazione di Costanti**

```jsx
const PI_GRECO = 3.14;
const NOME_SITO = "Il mio sito";

// ERRORE: non posso riassegnare una costante
// PI_GRECO = 3.15; // Questo causerebbe un errore
console.log(NOME_SITO);
```

### **Regole per i Nomi**

- Devono iniziare con una lettera, `_` o `$`
- Possono contenere lettere, numeri, `_` e `$`
- Sono case-sensitive (`nome` è diverso da `Nome`)
- Usare camelCase per più parole (`nomeCompleto`)

```jsx
// Esempi validi
let nome = "Mario";
let nomeCompleto = "Mario Rossi";
let eta2023 = 30;
let _privato = "segreto";
let $speciale = "valore";

// Esempi NON validi
// let 2nome = "errore"; // inizia con numero
// let nome-completo = "errore"; // contiene trattino

```

### **Esercizi**

**Esercizio 2.1**: Crea una pagina HTML con JavaScript interno che mostri "Benvenuto nel mondo JavaScript!" nella console.

**Esercizio 2.2**: Crea un file JavaScript esterno che mostri il tuo nome e la data corrente nella console, poi collegalo a una pagina HTML.

**Esercizio 2.3**: Crea 5 variabili che descrivano te stesso (nome, cognome, età, città, hobby) e stampale tutte nella console.

**Esercizio 2.4**: Crea delle costanti per i giorni della settimana e usale in frasi di benvenuto (es. "Buon lunedì!").