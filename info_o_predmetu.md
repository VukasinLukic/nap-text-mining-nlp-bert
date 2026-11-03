Dobro došli u tim predmeta Napredna analiza podataka
Drage koleginice i kolege,
 
Dobro došli u tim predmeta Napredna analiza podataka!
 
U okviru ovog (General) kanala, tokom semestra i ispitnih rokova, biće objavljivana sva bitna obaveštenja vezana za predmet. Takođe, tokom semestra, u kanalu Nastava, za svaki termin nastave, biće postavljena objava sa temom i kratkim opisom tog termina nastave, kao i linkovima na materijale koji su korišćeni u tom terminu, tako da ćete tu imate pregled tema i materijala u redosledu kojim su rađeni tokom semestra. 

Napredna analiza podataka 2026/27
  Blok 1: Text Mining (1. deo)
Blok nastave 1 
 
Teme obuhvaćene ovim blokom nastave:
Klasifikacija teksta: osnovni koncepti i primeri primene
Preprocesiranje teksta (tokenizacija, lematizacija, stop-words,...) i spaCy biblioteka
Bag of Words (BoW) model za transformaciju teksta u numerički oblik pogodan za klasifikaciju
sklearn Pipeline: pristup, implementaran Pipeline klasom, za povezivanje niza komponenti potrebnih za kreiranje i fino podešavanje (fine-tuning) modela mašinskog učenja 
Primer klasifikacije teksta, kroz primenu gore navedenih koncepata i biblioteka 


Materijali za čas:
Slajdovi na temu klasifikacije teksta i BoW modela (Klasifikacija teksta (2026) Blok 1.pdf)
Notebook Mobile_App_Reviews_Classification_BoW, verzija sa kodom i verzija bez koda (za vežbu) 
Dataset: mobile_apps_reviews.csv
Zadaci za rad na času.pdf, Blok 1
NAP2026/tm/Mobile_App_Reviews_Classification_BoW.ipynb at main · jeljov/NAP2026
Materijali za predmet Napredna analiza podataka u 2026 godini - jeljov/NAP2026
   Drage koleginice i kolege,
 
U nastavku su date informacije o načinu polaganja predmeta Napredna analiza podataka, kao i linkovi na relevantne dodatne informacije i materijale.
 
Polaganje predmeta uključuje:
 
Predispitne obaveze u formi kolokvijuma koji nije obavezan, nosi do 35 poena i polaže se isključivo u prvoj kolokvijumskoj nedelji. Kolokvijum se sastoji od jednog praktičnog zadatka koji se radi u računskom centru. Zadatak je po tipu vrlo sličan zadacima koje ste imali na kolokvijumu i ispitu iz Veštačke inteligencije i odnosiće se na prvu oblast koja se radi u okviru predmeta, konkretno, oblast Text mining-a , tj. klasifikacije i klasterizacije teksta. Primeri zadataka (sa rešenjima) su raspoloživi u Shared sekciji kanala General, odnosno ovde: Primeri zadataka za kolokvijum.
 
Izradu i odbranu praktičnog projekta koji se radi samostalno i nosi do 65 poena. Bliže informacije o zahtevima vezanim za projekat, kao i pregled okvirnih tema dat je u sledećem Google Doc-u: Teme za projektne (ispitne) radove 2026 - Google Docs
Pored tema navedenih u ovom dokumentu, slobodni ste da predložite i druge teme, sve dok su one vezane za oblasti koje se obrađuju u okviru predmeta.    (Obavezno za sve teme
U okviru uvodnog dela rada obavezno je sledeće: 
Definisati šta su tema, predmet i svrha rada.
Navesti koji se podaci koriste i odakle su preuzeti (u slučaju da je dataset preuzet sa neke online data platforme) ili prikupljeni (u slučaju da ste sami prikupljali podatake i kreirali dataset).
Dati kratak opis metodologije koja će biti korišćena, uz obrazloženja za napravljene izbore. Na primer, u slučaju teme koja se tiče klasifikacije teksta, navesti i obrazložiti izabran(e) pristup(e) za predstavljanje teksta u numeričkom obliku, izabrane ML algoritme, hiper-parametre koji će biti podešavani radi kreiranja optimalnog modela; zatim, koje će se evaluacione metrike korisititi i koja metrika će biti primarna.  
Rad mora da sadrži interepretaciju rezultata uzimajući u obzir temu i kontekst iz koga dolaze podaci.
Poželjno je prodiskutovati ograničenja sprovedenih analiza i mogućnosti za poboljšanja.
Kompletan rad može biti u formi: 
Jupyter / colab notebook-a koji sadrži kod i prateća objašnjenja, interpretaciju i diskusiju rezultata, ILI
Kombinacije python skripti i Word dokumenta, u kom slučaju skripta sadrži kod i objašnjenja relevantnih segmenata koda, dok Word dokument sadrži prikaz rezultata i njihovu interpretaciju / diskusiju. 

Važna napomena u vezi korišćenje generativne veštačke inteligencije
Generativna veštačka inteligencija (GenAI) može se koristiti ukoliko se koristi na smislen način i ako se njena primena dokumentuje na način opisan u nastavku. Smislen način korišćenja GenAI podrazumeva njeno korišćenje kao pomoćnog alata za namene kao što su debagovanje koda, bolje razumevanje pojedinih metoda, algoritama, hiperparametara i sl., za iscrtavanje složenijih grafikona i tabela i sl.
Ako se koristi GenAI, neophodno je dokumentovati u koje svrhe je korišćena i priložiti promptove ili reprezentativne primere promptova ako je više promptova koriščeno u istu svrhu (npr. debagovanje koda). 
Za sve što nije dokumentovano da je urađeno uz pomoć GenAI, smatraće se da je potpuno samostalno urađeno i biće potrebno znati objasniti svaki segment takvog koda, odnosno rada generalno. 

Tema 1: Poređenje klasičnog ML pristupa klasifikaciji teksta, zero shot, i few shot klasifikacije
Potrebno je ili kreirati ili preuzeti sa nekog online repozitorjuma podataka (npr. Kaggle.com) dataset koji sadrži bar jednu varijablu koja je tekstualnog tipa (npr. tekst novinskih članaka, komentari korisnika, tekst poruka razmenjenih na online forumima i sl). 

Fokus u okviru ove teme je upravo na tekstualnim podacima kreiranog  / izabranog dataset-a, odnosno, zadatak klasifikacije bi trebalo da bude zasnovan primarno na korišćenju tekstualnih podataka kao ulaznih podataka za klasifikaciju, mada se mogu, uz tekstualne, koristiti i drugi raspoloživi podaci relevantni za izabrani zadatak klasifikacije.   

Polazeći od tako kreiranog / izabranog dataset-a, potrebno je kreirati i uporediti različite pristupe za klasifikaciju teksta, uključujući:
Klasičan machine learning (ML) pristup klasifikaciji koji podrazumeva primenu nekog od pristupa za transformaciju teksta u numerički oblik (TF / TF-IDF / word embedding / text embeddings) i nekog od ML algoritama klasifikacije, uz opciono podešavanje (fine-tuning) hiper-parametara. 
Zero-shot pristup klasifikaciji, zasnovan na promptovanju izabranog LLM modela
Few shot pristup koji proširuje Zero-shot uvođenjem u prompt nekoliko dobro selektovanih primera     

Kreirane modele i klasifikacione “lance” (LangChain’s chains) uporediti korišćenjem standardnih metrika za evaluaciju klasifikacionih modela. Pri tome, proceniti koja je metrika najznačajnija za konkretni kontekst klasifikacije i njoj dati prioritet pri poređenju. Interpretirati rezultate uzimajući u obzir kontekst iz koga dolaze podaci.



Tema 2: Klasterizacija teksta
Potrebno je ili kreirati ili preuzeti sa nekog online repozitorjuma podataka (npr. Kaggle.com) dataset koji sadrži barem jednu varijablu koja je tekstualnog tipa (npr. tekst novinskih članaka, komentari korisnika, tekst poruka razmenjenih na online forumima i sl). 

Fokus u okviru ove teme je na tekstualnim podacima iz kreiranog  / izabranog dataset-a, s obzirom da je cilj zadatka tematsko grupisanje (klasterizacija) tekstualnih podataka (novinskih članaka, komentara korisnika, opisa softverskih bagova i sl).

Potrebno je uraditi tematsko grupisanje (klasterizaciju) teksta (iz kreiranog / selektovanog dataset-a), primenom nekog od pristupa za numeričku reprezentaciju teksta  (TF / TF-IDF / word embedding / text embeddings) i izabranog algoritma klasterizacije (npr. aglomerativno hijerarhijsko klasterovanje ili k-means). Poželjno je isprobati 2-3 različita pristupa za izdvajanje klastera kako bi se odabrao onaj koji najviše odgovara podacima sa kojima se radi.

Rad bi trebalo da sadrži:
Obrazloženje učinjenih metodoloških izbora (numerička reprezentacija teksta, algoritam klasterizacije, izabrani broj klastera) 
Interpretaciju / tumačenje klastera na osnovu ključnih reči izvedenih iz teksta klastera.  



Tema 3: Ekstrakcija informacija iz teksta (primenom LLMs) i primena istih u daljim analizama
Potrebno je ili kreirati ili preuzeti sa nekog online repozitorjuma podataka (npr. Kaggle.com) dataset koji sadrži barem jednu varijablu koja je tekstualnog tipa (npr. tekst novinskih članaka, komentari korisnika, tekst poruka razmenjenih na online forumima i sl). 

Iz tekstualne kolone / kolona, primenom LLM-a, estrahovati relevantne informacije tj informacije koje upotpunjuju strukturirane podatke raspoložive u datom dataset-u. Te informacije mogu biti:
eksplicitno prisutne u tekstu - na primer, nazivi entiteta (osoba, organizacija, gradova, restorana, …) koji se pominju u tekstu, datumi, vreme i sl.
implicitno prisutne u tekstu, na primer, u slučaju komentara korisnika, iskazani sentiment za pojedine aspekte korisničkog iskustva (npr., u slučaju restorana, pozitivno / negativno  komentarisana hrana, usluga, atmosfera i sl)

Dopuniti polazni dataset estrahovanim informacijama i iskoristi tako proširen dataset za dalje analize. Te dalje analize mogu biti: 
eksploratorne prirode - npr. primena vizuelizacija za sagledavanje određenih entiteta (ili drugih estrahovanih podataka) tokom vremena, ILI
prediktivne - npr. kreiranje regresionog ili klasifikacionog modela uz uključivanje estrahovanih podataka (kao dodatnih ulaznih varijabli), ILI
mrežne - npr. formiranje mreže korisnika gde su dva korisnika povezana u mreži ako su koristila istu uslugu (npr. boravili u istom hotelu, posetili isti restoran, koristili istu aplikaciju, …), dok težina relacije (ivice) koja ih povezuje predstavlja neki oblik linearne / neliearne kombinacije iskazanog zadovoljstva korišćenom uslugom, ILI
neki drugi interesantan oblik analize koji osmislite.   


Tema 4: Mrežna analiza podataka sa online diskusionog foruma / društvene mreže
Potrebno je kreirati ili preuzeti postojeći skup mrežnih podataka, što se može postoći na jedan od sledećih načina: 
prikupiti sa interneta (online foruma, društvenih mreža, …) podatke za formiranje mrežne strukture (aktere (čvorove) mreže i relacije (ivice) u mreži koje povezuju te aktere ), ili
preuzeti mrežne podatke sa nekog od online repozitorjuma takvih podataka - na primer, Colorado Index of Complex Networks, Network Data Repository, ili UCINet datasets, ili
preuzeti tabelarne podatke (npr sa Kaggle.com) pa iz njih izvući podatke o akterima mreže i njiihovim relacijama.

Formirati mrežu na osnovu prikupljenih / preuzetih podataka i sprovesti mrežne analize, uključujući:
Određivanje osnovnih deskriptivnih mrežnih metrika, kao što su veličina mreže, gustina, povezanost, komponente mreže, i sl
Određivanje centralnosti čvorova mreže i identifikovanje centralnih čvorova po različitim kriterijumima (centralnost stepena, blizine, posredništva, …)
Identifikovati zajednica u mreži i brokere koji povezuju zajednice

Sve analize i njihove rezultate je potrebno interpretirati i prodiskutovati, uzimajući u obzir kontekst iz koga dolaze mrežni podaci.

 )

 Blok 2: Text Mining (2. deo)
Blok nastave 2 
 
Teme obuhvaćene ovim blokom nastave:
Vector Space Model (VSM) za transformaciju teksta u numerički oblik pogodan za dalje analize (npr. klasifikaciju) 
Klasifikacija primenom Logističke regresije
Podešavanje hiperparametara modela u okviru sklearn Pipeline-a
Primer klasifikacije teksta primenom gore navedenih koncepata i biblioteka
Materijali za čas:
Slajdovi na temu VSM modela: Klasifikacija teksta (2026) Blok 2.pdf
Slajdovi na temu Logističke regresije: Logistička regresija 2026.pdf
Notebook Mobile_App_Reviews_Classification_VSM: verzija sa kodom i verzija bez koda (za vežbu)
Podaci: mobile_apps_reviews.csv
Zadaci za vežbu, Blok 2
Materijali za predmet Napredna analiza podataka u 2026 godini - jeljov/NAP2026
  Blok 3: Text mining (3. deo)
Blok nastave 3 


Teme obuhvaćene ovim blokom nastave:
Vektori reči (word vectors / word embeddings) za transformaciju teksta u numerički oblik
SMOTE tehnika balansiranja skupa podataka
Support Vector Machines (SVM) algoritam klasifikacije
Primer klasifikacije teksta primenom gore navedenih pristupa

Materijali za čas:
Slajdovi na temu vektora reči: Klasifikacija teksta (2026) Blok 3.pdf
Slajdovi na temu SVM algoritma: Support Vector Machines (SVM) 2026.pdf
Slajdovi na temu SMOTE tehnike: SMOTE.pdf
Notebook Mobile_App_Reviews_Classification_WordVectors: verzija sa kodom i bez koda 
Dataset: mobile_apps_reviews.csv
Zadaci za rad vežbu - Blok 3
   Blok 4: Text mining (4. deo)
Blok nastave 4 
 
Teme obuhvaćene ovim blokom nastave:
BERT i SBERT modeli
Klasterizacija teksta primenom SBERT modela
Materijali za čas:
Slajdovi na temu BERT-a i SBERT-a: BERT_and_SBERT_2026.pdf
Interaktivna vizuelizacija aglomerativnog hijerahijskog klasterovanja: Agglomerative_clustering_step_by_step.html
Notebook sa primerom primene SBERT-a za klasterizaciju: BBC_News_Clustering_SBERT.ipynb  
Dataset: bbc_news.csv 
  

u folderu materijali_sa_Microsoft_teamsa su ti primeri kolokvijuma, slajdovi , i dodatna literatura... 

