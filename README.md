# Cloud-init

Beispiel für eine Alternative Verwendung von Cloud-init ohne [lernmaas](https://github.com/mc-b/lernmaas).

Um diese Cloud-init Anweisungen statt [lernmaas](https://github.com/mc-b/lernmaas) zu Verwenden ist wie folgt vorzugehen:
* Machine im [MAAS UI](https://maas.io) anlegen
* Tags `cloud-init`  setzen
* Bei der Machine im Feld `Note` den URL dieses Repository eintragen - https://github.com/tbz-it/my-cloud-init
* Für den Zugriff via VPN (WireGuard) zusätzlich Tag `wireguard` und AZ setzen

Für eigene Implementierungen ist dieses Repository zu forken und die Datei `cloud.cfg.d/99_myinit.cfg` anzupassen.

Abhandlung im MAAS siehe Datei [curtin_userdata_ubuntu](https://github.com/mc-b/lernmaas/blob/master/preseeds/curtin_userdata_ubuntu).

## Links

* [MAAS](https://maas.io)
* [Cloud-init](https://cloudinit.readthedocs.io/)
* [curtin](https://curtin.readthedocs.io/)
* [Projekt lernmaas](https://github.com/mc-b/lernmaas)
