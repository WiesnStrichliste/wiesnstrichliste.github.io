# Wiesn Strichliste V10.3

Neu:
- Teilnehmer-Session bleibt nach Browser-Refresh erhalten.
- Admin-Session bleibt nach Refresh erhalten, solange Firebase den Email/Password-Login noch kennt.
- Admin-Log wurde robuster gemacht und schreibt Actor-UID, Ziel-UID, Zeit, Artikel, Aktion und Mengenänderung.
- Admin kann Teilnehmer vollständig löschen:
  - Profil
  - Bestellungen
  - Favoriten
- Das Löschen eines Teilnehmerkontos wird im Audit-Log dokumentiert.
- Alte Audit-Logs des Teilnehmers bleiben erhalten, damit Änderungen nachvollziehbar bleiben.

Wichtig:
Die neue `database.rules.json` muss erneut in Firebase → Realtime Database → Rules veröffentlicht werden.

App Check:
- bleibt wie in V10.2 integriert.
- Enforcement erst nach erfolgreichem Test aktivieren.
