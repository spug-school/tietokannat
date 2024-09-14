

### Tehtävä 1: Tee kysely, joka tulostaa kaikki sarakkeet goal-talusta.
![Alt text]([https://drive.google.com/file/d/12_AJ-Fw71dwKgq77es2eL7uXemM6SLxS/view?usp=drive_link](https://drive.google.com/file/d/12_AJ-Fw71dwKgq77es2eL7uXemM6SLxS/view?usp=sharing))

SELECT * FROM goal;

### Tehtävä 2: Tee kysely, joka tulostaa nimen ja tyypin kaikista Suomessa sijaitsevista lentokentistä. Suomen maatunnus on: FI
![Alt text](https://drive.google.com/file/d/1y9bUk9qqmkIz6gh1Hfq4465XIjdkKxLJ/view?usp=drive_link)

SELECT name, type FROM airport WHERE iso_country = 'FI';

### Tehtävä 3: Tee kysely, joka tulostaa suomalaisten lentokenttien nimet aakkosjärjestyksessä. Suomen maatunnus: FI
![Alt text](https://drive.google.com/file/d/1mabbOfDlhQ_GjjdQ9IBb2V_dZyRvh09S/view?usp=drive_link)

SELECT name FROM airport WHERE iso_country = 'FI' ORDER BY name ASC;

### Tehtävä 4: Tee kysely, joka tulostaa nimen ja tyypin kaikista Suomessa sijaitsevista lentokentistä. Järjestä tulos ensisijaisesti tyypin mukaan ja toissijaisesti nimen mukaan.
![Alt text](https://drive.google.com/file/d/14QB3EHBVROxMujsD2-criFFSP-XXHYW6/view?usp=drive_link)

SELECT name, type FROM airport WHERE iso_country = 'FI' ORDER BY type ASC, name ASC;

### Tehtävä 5: Tee kysely, joka tulostaa kaikki F-kirjaimella alkavat maan nimet country-taulusta.
![Alt text](https://drive.google.com/file/d/1WKA5a3K2gRRC_Kw5KgpEyL6Byqe0ehW4/view?usp=drive_link)

SELECT name FROM country WHERE name LIKE 'f%';

### Tehtävä 6: Tee kysely, joka tulostaa kaikki country-taulun maiden nimet, joissa esiintyy F-kirjain.
![Alt text](https://drive.google.com/file/d/1Xm-p4MgPb2TTPjv9QUawLcj4iOdLoLBb/view?usp=drive_link)

SELECT name FROM country WHERE name LIKE '%f%';

### Tehtävä 7: Missä locationissa Vesa sijaitsee?!
![Alt text](https://drive.google.com/file/d/1uHCtYdg4meHsEEGb7HTflviB-xn9CTXI/view?usp=drive_link)

SELECT location FROM game WHERE screen_name = 'Vesa';

### Tehtävä 8: Kuinkan paljon Ilkka on kuluttanut CO2 budjettia?
![Alt text](https://drive.google.com/file/d/15VZFsuOU7GnXoIcEPAz8mmZKta5C_1lP/view?usp=drive_link)

SELECT co2_consumed FROM game WHERE screen_name = 'Ilkka';

### Tehtävä 9: Kuinka paljon alkuperäinen CO2 budjetti on (tulosta CO2 budjetin arvo vain kerran)?
![Alt text](https://drive.google.com/file/d/1_2WtUCkcFdlC9_lHGlIswkRkHHYA7_hc/view?usp=drive_link)

SELECT DISTINCT co2_budget FROM game;
