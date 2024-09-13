

### Tehtävä 1: Tee kysely, joka tulostaa kaikki sarakkeet goal-talusta.

SELECT * FROM goal;

### Tehtävä 2: Tee kysely, joka tulostaa nimen ja tyypin kaikista Suomessa sijaitsevista lentokentistä. Suomen maatunnus on: FI

SELECT name, type FROM airport WHERE iso_country = 'FI';

### Tehtävä 3: Tee kysely, joka tulostaa suomalaisten lentokenttien nimet aakkosjärjestyksessä. Suomen maatunnus: FI

SELECT name FROM airport WHERE iso_country = 'FI' ORDER BY name ASC;

### Tehtävä 4: Tee kysely, joka tulostaa nimen ja tyypin kaikista Suomessa sijaitsevista lentokentistä. Järjestä tulos ensisijaisesti tyypin mukaan ja toissijaisesti nimen mukaan.

SELECT name, type FROM airport WHERE iso_country = 'FI' ORDER BY type ASC, name ASC;

### Tehtävä 5: Tee kysely, joka tulostaa kaikki F-kirjaimella alkavat maan nimet country-taulusta.

SELECT name FROM country WHERE name LIKE 'f%';

### Tehtävä 6: Tee kysely, joka tulostaa kaikki country-taulun maiden nimet, joissa esiintyy F-kirjain.

SELECT name FROM country WHERE name LIKE '%f%';

### Tehtävä 7: Missä locationissa Vesa sijaitsee?

SELECT location FROM game WHERE screen_name = 'Vesa';

### Tehtävä 8: Kuinkan paljon Ilkka on kuluttanut CO2 budjettia?

SELECT co2_consumed FROM game WHERE screen_name = 'Ilkka';

### Tehtävä 9: Kuinka paljon alkuperäinen CO2 budjetti on (tulosta CO2 budjetin arvo vain kerran)?

SELECT DISTINCT co2_budget FROM game;
