---

## **Övning 1: Skapa en Container och Använd Container Queries**

### **Beskrivning**
Du ska skapa en responsiv kortkomponent (`.card`) som ändrar utseende beroende på storleken på dess förälder (containern). Använd `@container` för att sätta olika stilar.

---

### **Mål**
1. Definiera en container med `container: inline-size;`.  
2. Använd **Container Queries** för att ändra bakgrundsfärg och textstorlek beroende på containerns storlek.  
3. Testa med olika storlekar på containern.

---

### **Steg-för-steg**
1. Skapa en HTML-fil med följande struktur:

```html
<!DOCTYPE html>
<html lang="sv">
<head>
  <meta charset="UTF-8">
  <title>Övning 1 - Container Queries</title>
  <style>
    /* Din CSS här */
  </style>
</head>
<body>
  <div class="card-container">
    <div class="card">Detta är ett kort.</div>
  </div>
</body>
</html>
```

2. I CSS, gör följande:  
   - Sätt `.card-container` till en viss bredd (ex. 300px eller 600px).  
   - Definiera `.card` som en **container** med `container: inline-size;`.  
   - Skapa två **Container Queries**:  
     - En för små containrar (mindre än 400px).  
     - En för stora containrar (mer än 400px).  

---

### **Exempeloutput**
- Om containern är **< 400px** → Bakgrund: **ljusblå**, textstorlek: **14px**.  
- Om containern är **>= 400px** → Bakgrund: **ljusgrön**, textstorlek: **18px**.

---
