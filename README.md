# Praktikum 4: agent suhtleb serveriga

Juhend: <https://hkhk-monitoring.github.io/monitoring/week04/lab/>

Kirjuta vastused `_vastus_` asemele, ühe-kahe lausega. Täida playbook `konf/agent.yml` (kohad `<TÄIDA>`), tõendid lähevad kausta `logid/` (juhendi osa „Töö esitamine“).

## Osa 2 · Agent playbook'iga kahes masinas

**`ansible-doc ansible.posix.firewalld`: mida teeb `immediate` ja mis juhtub, kui on ainult `permanent: true`?**

> _vastus_

**Kas esimesel käivitusel oli `changed` arv mõlemas masinas sama? Miks handler teisel käivitusel ei käivitunud?**

> _vastus_

**Mis juhtuks, kui playbook'is poleks tulemüüri ülesannet? Kumma hosti andmed jääksid tulemata?**

> _vastus_

## Osa 3 · Template'id: passiivne ja aktiivne

**Mis on veerus Type `proxmox2` ja `proxmox3` item'ite erinevus ja mida see ütleb selle kohta, kes ühenduse avab?**

> _vastus_

| Item (`proxmox2`) | Last value | Last check | Last check 1–2 min hiljem |
|---|---|---|---|
| Available memory | _vastus_ | _vastus_ | _vastus_ |
| CPU utilization | _vastus_ | _vastus_ | _vastus_ |
| FS [/]: Space: Available | _vastus_ | _vastus_ | _vastus_ |

**Kas `zabbix_agent2 -t 'vm.memory.size[available]'` ja veebiliidese väärtus klapivad? Kui ei, siis miks?**

> _vastus_

## Osa 4 · Kes avab ühenduse

**Miks tulid `proxmox3` andmed edasi ja kuidas playbook'i uus käivitus triivi parandas?**

> _vastus_

## Osa 5 · Oma trigger: vaba kettaruum alla 20%

**Mitu minutit kulus täitmisest probleemini ja kustutamisest lahenemiseni? Miks see ei juhtunud kohe?**

> _vastus_

## Kodutöö

Juhend: <https://hkhk-monitoring.github.io/monitoring/week04/homework/>. Failid `konf/varundus.conf` ja `logid/kodutoo-varundus.txt`.

1. Kirjuta oma trigger'i avaldis.

    > _kodutöö_

2. Mitu minutit pärast cron'i keelamist tekkis probleem ja miks just siis?

    > _kodutöö_

3. Mis juhtub, kui keegi kustutab faili `/var/tmp/varundus.ok`? Kas see on hea või halb?

    > _kodutöö_

4. Miks sobib aktiivne kontroll võrku, kus server ei pääse varundusmasinasse? Kas sama võtit saaks kasutada ka passiivse kontrollina?

    > _kodutöö_

5. Probleemi ajalugu: host, algusaeg, lahenemise aeg, cron'i keelamise ja taastamise kellaaeg.

    > _kodutöö_

6. Mida see kontroll tõendab ja mida peaksid veel kontrollima, et teada, kas varukoopiast saab andmed taastada?

    > _kodutöö_
