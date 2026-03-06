# README
## Site personal

### Homepage (Acasă)
Pagina principală servește ca punct central al portofoliului și conține următoarele secțiuni:
- **Bară de navigare interactivă**: 
  - Pe desktop, afișează un meniu orizontal.
  - Pe mobil, se transformă într-un **Meniu Hamburger** animat. 
- **Secțiunea Hero**: Un design de tip "Split Layout", prezentând o scurtă biografie și o imagine de profil.
- **Educație**: Afișează parcursul academic folosind același layout consistent stânga-dreapta.
- **Competențe**: Un grid responsive care prezintă abilitățile tehnice. La trecerea mouse-ului, casetele au o animație subtilă a bordurii folosind culoarea de accent a site-ului.
- **Teaser Fotografie**: O secțiune "Call-to-action" care invită utilizatorii să viziteze galeria foto completă.
- **Hobby-uri**: Un slider interactiv realizat **exclusiv din CSS**. Folosește butoane radio pentru a expanda secțiunea selectată și a le comprima pe celelalte, dezvăluind imaginea de fundal.
- **Footer**: Conține iconițe pentru rețelele sociale care își schimbă culoarea la hover și logo-ul site-ului.
- **Buton Back-to-top**: Un buton plutitor care apare în colțul ecranului, permițând navigarea rapidă la începutul paginii.

### About (Despre)
O pagină dedicată detaliilor personale și poveștii din spatele portofoliului.
- **Secțiunea Bio**: Text detaliat despre parcursul personal.
- **Colaj Foto**: Un layout personalizat de tip CSS Grid care afișează un colaj de 4 imagini
- **Interese**: O secțiune secundară care listează interesele tehnice și personale, însoțită de o imagine tematică.

### Colecție imagini (Portofoliu)
O galerie dinamică dedicată pasiunii pentru fotografie.
- **Layout tip Masonry**: Implementat folosind CSS Grid cu proprietatea `grid-auto-flow: dense`.
- **Dimensionare Dinamică**: Imaginile au dimensiuni variate (unele ocupă două coloane, altele două rânduri) pentru a crea un aspect modern, evitând monotonia unui tabel clasic.
- **Efecte Hover**: Fiecare "card" foto are o descriere care glisează de jos în sus la hover, afișând locația și anul fotografiei.

### Contact
O pagină de contact complet funcțională.
- **Layout**: Prezintă datele de contact în stânga și formularul în dreapta.
- **Funcționalitate Formular**: Formularul este conectat la **Web3Forms API**, permițând trimiterea reală a emailurilor direct din pagina HTML, fără a necesita un server backend propriu (PHP/Node.js).
- **Stilizare**: Câmpurile de input și textarea sunt stilizate modern, având focus vizual în culoarea de accent a site-ului.

### Implementare Tehnică și Responsivitate
Site-ul este construit pentru a fi complet responsive și adaptabil la orice dimensiune a ecranului, utilizând tehnici moderne CSS:

1.  **Variabile CSS (:root)**: Utilizate pentru a menține o temă de culoare consistentă (Fundal întunecat cu accente Turcoaz) și tipografie uniformă pe toate paginile.
2.  **Arhitectură Flexbox**: Layout-ul de bază se bazează pe clasa `.split-layout`.
    -   *Desktop*: Elementele sunt afișate unul lângă altul (`row`).
    -   *Mobil*: Elementele se așează vertical (`column`) sau invers-vertical (`column-reverse`) folosind media queries, pentru a optimiza ordinea vizuală.
3.  **CSS Grid**: Folosit pentru secțiunea "Competențe" și galeria foto. Acest lucru permite elementelor să se aranjeze automat pe rânduri noi în funcție de spațiul disponibil.
4.  **Media Queries**: Site-ul folosește breakpoint la **768px**.
    -   Sub această lățime, bara de navigare devine meniu hamburger.
    -   Grid-urile devin o singură coloană.
    -   Padding-urile și dimensiunile fonturilor sunt ajustate pentru lizibilitate pe ecrane mici.
    -   Proprietatea `overflow-wrap` asigură că textele lungi (precum adresele de email) nu strică layout-ul pe mobil.
