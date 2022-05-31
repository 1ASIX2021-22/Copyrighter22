<h1 align="center">
  <b>Instal·lació sistema gestor de base de dades - MySQL</b>
</h1>
<p align="center">
<img src="https://user-images.githubusercontent.com/59867802/171252284-d6cc87b0-3d37-4a9e-8171-d0ee726903b4.jpg">
</p>

---
<br>
<p align="center">
  Usarem la següent comanda per a instal·lar el MYSQL Server:
</p>

```bash
sudo apt-get install mysql-server
```
<p align="center">
<img src="https://user-images.githubusercontent.com/59867802/171252838-39eb6939-ba19-4f9d-abfe-37f31cc99944.png">
</p>

<p align="center">
  Com no podrem iniciar sessió al MYSQL amb el nostre usuari, amb ula comanda <b>cat</b> obtindrem l'usuari i password del usuari debyan-sys-maint.
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/59867802/171253279-4656fd3b-a85e-47ba-a088-029bce8d19a9.png">
</p>

<p align="center">
  Amb aquest usuari tenim que iniciar sessió, amb la següent comanda:
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/59867802/171253566-0435cff3-b6c7-48ca-a0ae-9c8061f4e37f.png">
</p>

<p align="center">
  Ja dins del MYSQL, crearem una base de dades amb la comanda <b>CREATE DATABASE</b> i comprovarem que s'ha creat amb la comanda <b>SHOW DATABASES</b>
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/59867802/171253890-4c1ccf6d-9bcf-4e9d-888c-3d32ea9c0796.png">
</p>

<p align="center">
  Accedirem dins la base de dades que hem creat amb la comanda <b>use</b>, crearem una taula amb la comanda <b>create table</b> i comprovarem que s'ha creat aquesta base de dades amb la comanda <b>SHOW TABLES</b>
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/59867802/171254192-649ab893-ca02-4f4f-be58-67669c9818ac.png">
</p>

<h2 align="center">
  <b>Instal·lació i configuració MYSQL Workbench</b>
</h2>

<p align="center">
   Abans de res anirem a la pàgina de descàrregues del MYSQL Community per baixar el seu repositori.
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/59867802/171254507-94b3bd2d-aea5-4c37-a59c-a0adbf31935a.png">
</p>

<p align="center">
  Un cop dins de la carpeta <b>Baixades</b>  instal·lem el repositori.
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/59867802/171254870-0445d615-d7ca-4882-839a-edce14220c07.png">
</p>

<p align="center">
  Escollirem la opció <b>MySQL Server & Cluster</b> i continuarem.
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/59867802/171255276-67cb4e49-ac95-482e-9868-429f44ec93bc.png">
</p>

<p align="center">
  Aquí escollim la primera opció i continuarem.
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/59867802/171255913-1042e969-e517-417a-bec4-a370525f4529.png">
</p>

<p align="center">
 Acte seguit començara a descargar-se.
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/59867802/171256255-049b5235-1992-41e2-ab37-174d0720f516.png">
</p>

<p align="center">
  Quan ja tenim el repositori instal·lat farem un apt-get update.
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/59867802/171256459-09ffafa6-57bd-41b1-951a-6afdc62d0755.png">
</p>

<p align="center">
  Després amb la comanda <b>apt install mysql-workbench-community</b> ho instal·larem.
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/59867802/171256831-0047889c-cd49-48a3-b3ef-11d2b87b73f4.png">
</p>

<p align="center">
  Un cop instal·lat, iniciarem el programa amb la comanda <b>sudo mysql-workbench</b>.
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/59867802/171257173-0b1dabc3-20a3-40cb-87d2-ad2570aa5008.png">
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/59867802/171257405-f403e16f-8027-4399-a456-79dc701d53f5.png">
</p>

<p align="center">
  Ja dins del MYSQL Workbench farem una prova per connectar-nos a la base de dades que hem creat anteriorment, li donarem clic dret amb el ratolí al recuadre que es veu en l'imatge i clic  a <b>Edit Connection</b> per editar la configuració.
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/59867802/171257940-6f9a90ff-ae3b-4aaa-9cc5-da9cf8de411b.png">
</p>

<p align="center">
  Per defecte l'usuari es el root però ho cambiarem per a que ens connecte amb l'usuari que hem utilitzat abans, el <b>debian-sys-maint</b>.
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/59867802/171259243-76dfba4b-9571-41ec-b7e5-e33a0137fa26.png">
</p>

<p align="center">
  I al realitzar un <b>Test Connection</b> ens demanara la  contrasenya.
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/59867802/171259757-697de30f-4383-44b1-b880-90c60e30c769.png">
</p>

<p align="center">
 Probem de connectar i que ens funciona.
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/59867802/171260731-a0c57be5-c707-484d-9793-b17d75ee1c66.png">
</p>

<p align="center">
  Ara ja estem dins de la base de dades.
</p>

<p align="center">
  Al lateral esquerre podem veure el apartat de <b>Schemas</b> , allí podem veure com està la base de dades i la taula que hem creat abans.
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/59867802/171262048-827bdaab-0431-4213-8e2c-398c8d4bc0bd.png">
</p>

<h2 align="center">
  <b>Configuració PHP STORM</b>
</h2>

<p align="center">
<img src="https://user-images.githubusercontent.com/59867802/171263437-65ff9507-f714-4eb2-9eaa-143502477946.png">
</p>

<p align="center">
Obrirem el <b>PHPStorm</b> i crearem un nou projecte.
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/59867802/171263912-27241963-d6ac-4647-a635-244b60b456e9.png">
</p>

<p align="center">
  Al lateral dret obrirem la pestanya <b>Database</b>, <b>Data source</b>, <b>MySQL</b>. 
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/59867802/171264686-ce9880ec-81cc-4f0d-b66d-b3dc74835723.png">
</p>

<p align="center">
  Com hem fet abans, utilitzarem l'usuari <b>debian-sys-maint</b> per connectar-nos. I ho comprovarem fen un <b>Test Connection</b>
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/59867802/171265438-6d95bfcf-01bf-407b-9737-b23028562872.png">
</p>

<p align="center">
  Per guardar els canvis clic al botó qe diu <b>Apply</b>
</p>

<p align="center">
  Com podem veure, ja tindrem accés al Mysql i a la base de dades que habiem creat.
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/59867802/171266208-f0b4a106-0f40-415c-88a5-b516403e9415.png">
</p>

