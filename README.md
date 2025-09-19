# Oppdrag1

# Nettverk og tilkobling

#### Jeg gikk til settings i raspberry pien for å endre ip til statisk ip (10.200.14.24)
<img width="739" height="628" alt="Manual Ip" src="https://github.com/user-attachments/assets/92a66c36-5fd7-460a-9d0e-5137218a8537" />

Greide å pinge begge pcene

Startet en python server på raspberry pien med koden:
    python3 -m http.server


<img width="673" height="74" alt="ServerTestImg" src="https://github.com/user-attachments/assets/48589e15-dcad-4372-af1e-57ff1a2e9703" />

Jeg greide å åpne nettsiden på laptopen og greide å hente filer fra den

<img width="960" height="504" alt="image" src="https://github.com/user-attachments/assets/49d6a52c-2ceb-40a4-b615-df0f22d052b0" />



## GitHub

#### Så opprettet jeg en github reposetory for å dele en enkel python fil til raspberry pien som sjekker operativsystem.

import platform

system_info = platform.uname()

print("Du bruker en pc med", system_info.system, "operativsystemet")
print(system_info.machine)

#### så initialiserte jeg en repository addet filen, commita den så pushet jeg filen til online repositoryen
<img width="693" height="322" alt="image" src="https://github.com/user-attachments/assets/d3ccd8e5-bc9d-4f7b-a041-7a8716eaf4fd" />


#### så gikk jeg inn i raspberry pien og clonet repositoryen 


<img width="480" height="125" alt="image" src="https://github.com/user-attachments/assets/999adfd8-b800-46bc-bec3-67b976249400" />




## SSH
Etter dette så sluttet skjermen min å fungere så jeg jobbet med ssh og satt set opp, både på cmd og PuTTY med port 1814

<img width="496" height="289" alt="image" src="https://github.com/user-attachments/assets/78046c37-933e-4d59-bea6-da37aecb0265" />

<img width="340" height="338" alt="image" src="https://github.com/user-attachments/assets/fdb5e429-7c7e-4d6d-a542-4b8186a76ebb" />

når jeg var ferdig så funket ikke python serveren lenger så jeg antok at det var brannmuren siden jeg hadde et lignende problem med ssh siden 1814 porten ikke var åpen.
så jeg skrudde av brannmuren for å se om det var problemet med komandoen sudo ufw disable.
Serveren funket etter det så jeg skrudde på firewallen igjen og åpnet port 8000 med sudo ufw allow 8000/tcp og sudo ufw allow 8000/udp

<img width="428" height="187" alt="image" src="https://github.com/user-attachments/assets/4c83195d-219e-4827-8b16-6e25f0634133" />







