# Portál pre pacientov, na ktorom sa môžu objednať na dobrovoľné očkovanie

### Zadanie projektu + prípady použitia
Ako pacient, ktorý sa chcem podrobiť dobrovoľnému očkovaniu. Si vytvorím požiadavku v portáli kde budem mať práve dostupné termíny očkovania k danej očkovacej látke (CREATE).  Ako pacient sa budem vedieť informovať o očkovaniach, ktoré mi boli vykonané alebo ma čakajú a taktiež aby sestrička vedela pripraviť dostatočne množstvo očkovacích látok na daný deň vopred na základe objednaných pacientov pre daný deň (READ). Sestrička má možnosť v prípade nedostupnosti očkovacej látky alebo naplneniu harmonogramu lekára zmeniť termín očkovania (UPDATE).  Pacient sa môže odhlasiť z očkovania do určitého termínu pred očkovaním (DELETE)

### Mená členov tímu, ktorý sa podieľali na projekte
- Peter Koszorús

### Názov vašej aplikácie na spoločnom klastri
- Portál na registráciu očkovaní pko

### Linka na Github repozitáre obsahujúce FE,BE a gitops
- https://github.com/PeterKoszorus/ambulance-gitops
- https://github.com/PeterKoszorus/ambulance-webapi-vaccination
- https://github.com/PeterKoszorus/ambulacne-vaccination

### Linka na DockerHub registry
- https://hub.docker.com/repository/docker/peterkoszorus/ambulance-webapi-vaccination/general
- https://hub.docker.com/repository/docker/peterkoszorus/ambulance-vaccination/general

### Linka k FE aplikácii na spločnom klastri
- https://wac-24.westeurope.cloudapp.azure.com/ui/pko-ambulance-vc/

### Názov deployment objektu pre UI
- pko-ambulance-vaccination-deployment-86c464d9bb-6bmr6

### Názov deploymentu pre webapi
- pko-ambulance-webapi-vaccination-568df654fb-nsh9c

### Stručný opis riešenie k vyhodnoteteniu
- Aplikacia je velmi podobna s aplikaciou vyvyjanou na cviceniach, kedze som nasledoval kroky z cviceni.
- Aplikaciu sa mi nepodarilo nahodit cez webcomponent na spolocny kluster avsak da sa portforardnut pod na lokalhost a tak sa ju da spustit. Dovod tochto neuspechu prikladam za to ze som sa snazil pouzit jeden gitops repozitar na viacero aplikacii.
- Rozdiel je v:
  - pacienti maju pri mene zobrazovane dostupne ockovacie latky
  - datum navstevy je zobrazovany termin ockovania
- Aplikacia neobsahuje vsetky funkcionality z zadania, ale obsahuje zakladne CRUD operacie

### Linka na nasadenie samostatného web UI v Azure Cloud
- https://pko-ambulance.azurewebsites.net/