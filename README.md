# diegozorzi.com — Istruzioni di setup

## Struttura della cartella
Metti tutti questi file nella stessa cartella:

```
/
├── index.html          ← il sito (questo file)
├── CV_Diego_Zorzi_ITA.pdf
├── IMG_6986.png
├── Frontale_PRISMA_CLG_4k_23.png
├── Prospettica_PRISMA_CLG_4k_22.png
├── Inspection_Table_2_6.png
├── Soufflè_Cafedesart_1_front.jpg
├── Soufflè_Cafedesart_2_front.jpg
├── Soufflè_Cafedesart_3_front.jpg
├── Soufflè_Cafedesart_gambe.jpg
├── top_diamond_chiaro.jpg
├── top_X_chiaro.jpg
├── top_X_scuro.jpg
└── README.md
```

## Cose da fare prima di pubblicare

### 1. Form di contatto (Formspree)
1. Vai su https://formspree.io e crea un account gratuito
2. Crea un nuovo form
3. Copia il tuo Form ID (formato: `xabc1234`)
4. Nel file index.html, cerca `XXXXXXXX` e sostituiscilo con il tuo ID

### 2. Pubblicare su GitHub Pages
1. Crea un account su https://github.com
2. Crea un nuovo repository chiamato `diegozorzi` (o qualsiasi nome)
3. Carica tutti i file trascinandoli nella pagina del repository
4. Vai su Settings → Pages → Source: seleziona "main" branch → Save
5. Il sito sarà online su `tuonome.github.io/diegozorzi`

### 3. Collegare il dominio diegozorzi.com (Namecheap)
1. Acquista il dominio su https://namecheap.com (~10€/anno)
2. In Namecheap → Manage → Advanced DNS, aggiungi questi record:
   - Type: A | Host: @ | Value: 185.199.108.153
   - Type: A | Host: @ | Value: 185.199.109.153
   - Type: A | Host: @ | Value: 185.199.110.153
   - Type: A | Host: @ | Value: 185.199.111.153
   - Type: CNAME | Host: www | Value: tuonome.github.io
3. In GitHub → repository → Settings → Pages → Custom domain: scrivi `diegozorzi.com`
4. Attendi 24-48h per la propagazione DNS

### 4. Cose opzionali da aggiornare nel codice
- Riga con `CV_Diego_Zorzi_ITA.pdf`: assicurati che il nome del file corrisponda
- Riga con `XXXXXXXX`: il tuo Formspree ID (obbligatorio per il form)
