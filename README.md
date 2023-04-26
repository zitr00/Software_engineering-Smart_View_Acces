# SISTEM DE ACCES BAZAT PE PROCESARE VIDEO ȘI QR

Se cere realizarea unui sistem de gestiune a angajaților dintr-o firmă. Sistemul va ține
evidența prezenței angajaților, recunoașterea automobilului acestora la accesul în parcarea
firmei, precum și recunoașterea angajatului prin QR la intrarea în firmă. Aceasta se va
realiza prin citirea numărului de înmatriculare a automobilului ce intră în parcare, prin
intermediul unei camere conectate la RaspberryPi 4 Model B. Se va monitoriza numărul de
înmatriculare, precum și ora și data de intrare în parcare. Permiterea intrării în parcare va fi
semnalată prin deschiderea unui led verde – deschis 7 secunde, iar accesul neautorizat la
parcare va fi semnalat prin deschiderea unui led roșu – deschis 7 secunde. Pentru ca
utilizatorul să recunoască funcționalitatea acestui modul din sistem va vedea deschis un led
albastru. La ieșirea din parcare utilizatorul va trebui să apese un buton care va deschide
parcarea – led verde deschis 7 secunde. La intrarea/ieșirea din/în parcare se vor actualiza
locurile rămase libere.

La intrarea în firmă utilizatorul va trebui să genereze un cod QR pe telefonul acestuia
și să-l scaneze cu ajutorul unei camere aflate la intrare. Se va genera un alt cod QR la
fiecare intrare a angajatului. Dacă angajatul este recunoscut în sistem, un led verde conectat
la un modul Arduino Uno va fi deschis timp de 7 secunde, iar dacă nu este recunoscut un led
roșu va fi deschis timp de 5 secunde. Pentru ca utilizatorul să recunoască funcționalitatea
acestui modul din sistem va vedea deschis un led albastru. După ce s-a scanat codul QR și
angajatul primește acces la intrarea în firmă se va monitoriza cât timp acesta a fost prezent.
La ieșirea din firmă angajatul va apăsa un buton pentru a porni o altă cameră destinată
scanări QR de identificare a persoanei care dorește să plece. Monitorizarea timpului petrecut
la locul de muncă a acestuia se va opri.

Sistemul va permite administrarea listei angajaților din firmă, precum și monitorizarea
locului unde se găsesc aceștia în birou. Astfel administratorul va putea sa-i așeze la un birou
cu alți colegi printr-o interfață grafică. În contextul actual, Covid 19, administratorul va putea
să observe în mod grafic care sunt colegii de birou ai acestuia. Sistemul va permite
administratorului să genereze rapoarte grafice cu diferiți parametri măsurați pentru unul sau
mai mulți angajați.
În Figura 1 este prezentată arhitectura sistemului:

