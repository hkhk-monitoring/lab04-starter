# Labor 4: agent räägib serverile

Juhend: <https://hkhk-monitoring.github.io/monitoring/week04/lab/>

Kirjuta vastused `_vastus_` asemele, ühe-kahe lausega. Playbook läheb faili `konf/agent.yml`, tõendid kausta `logid/` (juhendi osa "Esitamine").

---

## A1 · Agent käsitsi proxmox2-s

**Mida näitas `sudo zabbix_agent2 -t 'vfs.fs.size[/,pfree]'`?**

> _vastus_

**Miks oli port 10050 kinni, kuigi `ss` näitas, et agent kuulab?**

> _vastus_

## A2 · Sama playbook'iga kahes masinas

**`ansible-doc ansible.posix.firewalld`: mida teeb `immediate` ja mis juhtub, kui on ainult `permanent: true`?**

> _vastus_

**Miks oli esimesel käivitusel `proxmox2` ja `proxmox3` `changed` arv erinev?**

> _vastus_

## A3 · Template'id: passiivne ja aktiivne

**Mis on veerus Type `proxmox2` ja `proxmox3` item'ite erinevus ja mida see ütleb selle kohta, kes ühenduse avab?**

> _vastus_

## A4 · Kes avab ühenduse

**Miks tulid `proxmox3` andmed edasi ja kuidas playbook'i uus käivitus triivi parandas?**

> _vastus_

## A5 · Oma trigger: vaba kettaruum alla 20%

**Mitu minutit kulus täitmisest probleemini ja kustutamisest lahenemiseni? Miks see ei juhtunud kohe?**

> _vastus_

---

## Kodutöö

Juhend: <https://hkhk-monitoring.github.io/monitoring/week04/homework/>. Failid `konf/varundus.conf` ja `logid/kodutoo-varundus.txt`. Need kontrollid annavad lisapunkte (BOONUS) ega muuda labori punkte.

1. Kirjuta oma trigger'i avaldis.

    > _kodutöö_

2. Mitu minutit pärast cron'i väljalülitamist tekkis probleem ja miks just siis?

    > _kodutöö_

3. Mis juhtub, kui keegi kustutab faili `/var/tmp/varundus.ok`? Kas see on hea või halb?

    > _kodutöö_

4. Miks sobib see kontroll paremini aktiivsele agendile?

    > _kodutöö_
