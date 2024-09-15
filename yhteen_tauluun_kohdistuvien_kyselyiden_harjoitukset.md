

### Tehtävä 1: Tee kysely, joka tulostaa kaikki sarakkeet goal-talusta.
![Alt text](https://i.imgur.com/iC4WjaW.png)

SELECT * FROM goal;

### Tehtävä 2: Tee kysely, joka tulostaa nimen ja tyypin kaikista Suomessa sijaitsevista lentokentistä. Suomen maatunnus on: FI
![Alt text](https://i.imgur.com/xE35bnS.png)

SELECT name, type FROM airport WHERE iso_country = 'FI';

### Tehtävä 3: Tee kysely, joka tulostaa suomalaisten lentokenttien nimet aakkosjärjestyksessä. Suomen maatunnus: FI
![Alt text](https://i.imgur.com/fzlfL9W.png)

SELECT name FROM airport WHERE iso_country = 'FI' ORDER BY name ASC;

### Tehtävä 4: Tee kysely, joka tulostaa nimen ja tyypin kaikista Suomessa sijaitsevista lentokentistä. Järjestä tulos ensisijaisesti tyypin mukaan ja toissijaisesti nimen mukaan.
![Alt text](https://i.imgur.com/rxWk1hQ.png)

SELECT name, type FROM airport WHERE iso_country = 'FI' ORDER BY type ASC, name ASC;

### Tehtävä 5: Tee kysely, joka tulostaa kaikki F-kirjaimella alkavat maan nimet country-taulusta.
![Alt text](https://i.imgur.com/PZWSr5k.png)

SELECT name FROM country WHERE name LIKE 'f%';

### Tehtävä 6: Tee kysely, joka tulostaa kaikki country-taulun maiden nimet, joissa esiintyy F-kirjain.
![Alt text](https://i.imgur.com/Ib2Bbaz.png)

SELECT name FROM country WHERE name LIKE '%f%';

### Tehtävä 7: Missä locationissa Vesa sijaitsee?!
![Alt text](https://i.imgur.com/uFm6kL6.png)

SELECT location FROM game WHERE screen_name = 'Vesa';

### Tehtävä 8: Kuinkan paljon Ilkka on kuluttanut CO2 budjettia?
![Alt text](https://i.imgur.com/Y6R9mxs.png)

SELECT co2_consumed FROM game WHERE screen_name = 'Ilkka';

### Tehtävä 9: Kuinka paljon alkuperäinen CO2 budjetti on (tulosta CO2 budjetin arvo vain kerran)?
![Alt text](https://i.imgur.com/1GH7yNa.png)

SELECT DISTINCT co2_budget FROM game;
