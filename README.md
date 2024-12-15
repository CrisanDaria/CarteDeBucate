Din carte de bucate controller
1. GET /listaCarti
   Tip Request: GET
   Parametri: Niciunul
   Funcționalitate: Afișează lista tuturor cărților de bucate.

2. GET /formCarte
   Tip Request: GET
   Parametri: Niciunul
   Funcționalitate: Afișează formularul pentru crearea unei cărți noi.

3. POST /saveCarte
   Tip Request: POST
   Parametri: Body - Obiect CarteDeBucate
              - numeAutor (String): Numele autorului.
              - titluCarte (String): Titlul cărții.
              - descriereCarte (String): Descrierea cărții.
              - retete (List<Reteta>): Lista de rețete asociate.
   Funcționalitate: Salvează o nouă carte de bucate.

4. GET /searchCarte
   Tip Request: GET
   Parametri: Query Parameter
              - query (String): Textul căutat.
   Funcționalitate: Caută cărți de bucate pe baza unui text în titlu sau descriere.

Pentru RetetaController
1. GET /lista
   Tip Request: GET
   Parametri: Niciunul
   Funcționalitate: Afișează lista tuturor rețetelor.

2. GET /form
   Tip Request: GET
   Parametri: Niciunul
   Funcționalitate: Afișează formularul pentru crearea unei rețete noi.

3. POST /save
   Tip Request: POST
   Parametri: Body - Obiect Reteta
              - nume (String): Numele rețetei.
              - descriere (String): Descrierea rețetei.
              - alte atribute relevante ale entității Reteta.
   Funcționalitate: Salvează o nouă rețetă.

4. GET /edit/{id}
   Tip Request: GET
   Parametri: Path Variable
              - id (UUID): ID-ul rețetei ce urmează să fie editată.
   Funcționalitate: Pregătește formularul pentru editarea unei rețete existente.

5. GET /delete/{id}
   Tip Request: GET
   Parametri: Path Variable
              - id (UUID): ID-ul rețetei ce urmează să fie ștearsă.
   Funcționalitate: Șterge o rețetă din baza de date și redirecționează către lista rețetelor.

6. GET /search
   Tip Request: GET
   Parametri: Query Parameter
              - query (String): Textul căutat.
   Funcționalitate: Caută rețete pe baza unui text în numele sau descrierea lor.

7. GET /Meniu
   Tip Request: GET
   Parametri: Niciunul
   Funcționalitate: Afișează pagina principală a meniului aplicației.

