# Kenko MCP by 3agenteers

**Dein Kenko-Studio im KI-Assistenten.**

Kenko MCP by 3agenteers verbindet kompatible KI-Assistenten mit den Kenko-Studioinformationen, für die du berechtigt bist. Der unabhängige Dienst richtet sich an Fitness-, Yoga-, Pilates- und andere kursbasierte Studios.

**Free zum Lesen. Pro für freigegebene Änderungen. Kein eigener MCP-Server nötig.**

[Studio verbinden](https://kenko-mcp.com/app/) · [Website](https://kenko-mcp.com/) · [Preise](https://kenko-mcp.com/preise/) · [English](https://github.com/gerritjobrocks/kenko-mcp/blob/main/README.md)

## Free ausprobieren

- «Welche Kurse haben nächste Woche noch freie Plätze?»
- «Prüfe, ob diese Person bereits als Kontakt in Kenko existiert.»
- «Prüfe den Kurs und die vorhandenen Credits, bevor ich die Person einbuche.»

Das sind mögliche Beispielaufträge, keine Kundenzitate. Daten, Kenko-Rechte und die Unterstützung deines KI-Clients bestimmen, was möglich ist.

## Verbinden statt einen Server installieren

1. Im [Kundenbereich](https://kenko-mcp.com/app/) mit dem eigenen Kenko-Zugang anmelden.
2. Unternehmen und Studio ausdrücklich auswählen.
3. Im geeigneten Remote-MCP-Client `https://kenko-mcp.com/mcp` hinzufügen.
4. Die Client-Autorisierung abschliessen. Zum Ausprobieren genügt Lesezugriff.

Transport: Streamable HTTP. Autorisierung: OAuth mit S256-PKCE. Unterstützte Dialoge, Dateiformate und Funktionen hängen vom Client und Tarif ab. Das [Konfigurationsbeispiel](https://github.com/gerritjobrocks/kenko-mcp/blob/main/examples/mcp.json) gilt nur für Clients, die dieses Format akzeptieren.

[Einrichtung](https://kenko-mcp.com/docs/install/) · [Claude](https://kenko-mcp.com/docs/claude/) · [Weitere Clients](https://kenko-mcp.com/docs/cursor/)

Passwörter und Tokens gehören in die tatsächlichen Anmelde-/Autorisierungsdialoge, niemals in einen Chat, ein GitHub-Issue oder die MCP-Adresse.

## Von Free zu Pro

Lesen und Vorbereiten bleiben Free. Für freigegebene Änderungen gibt es Pro, zum Beispiel eine konkrete Kursbuchung mit vorhandenem Credit oder das Anlegen eines Kontakts nach Dublettenprüfung.

**CHF 19 pro Kenko-Unternehmen und Monat, exklusive MwSt.** Kenko und dein KI-Anbieter sind separate Angebote. Die Zahlung ersetzt weder die passende Kenko-Rolle noch die Schreibfreigabe des Clients oder deine Freigabe für eine konkrete Änderung.

[Pro ansehen](https://kenko-mcp.com/preise/) · [Im Kundenbereich freischalten](https://kenko-mcp.com/app/)

## Optionaler Agenten-Skill

Der [Studio-Skill](https://github.com/gerritjobrocks/kenko-mcp/blob/main/skills/kenko-studio/SKILL.md) hilft bei gemischten Lese-/Schreibaufträgen und dem sauberen Übergang zu Pro. Bei einem geeigneten Agenten separat installieren; eine MCP-Verbindung lädt den Skill nicht automatisch.

Dieses Repo enthält Einrichtung, Konfigurationsbeispiele und den optionalen Skill. **Es enthält keinen selbst hostbaren Server und keinen privaten Backendcode.** Klonen allein verbindet kein Studio und aktiviert kein Abo.

[Datenweg und Datenschutz](https://kenko-mcp.com/docs/datenschutz/) · [Anbieter und Bedingungen](https://kenko-mcp.com/nutzungsbedingungen/) · [Support](mailto:gerrit@3agenteers.com)

Die [MIT-Lizenz](https://github.com/gerritjobrocks/kenko-mcp/blob/main/LICENSE) gilt für die Inhalte dieses Repos, nicht für den gehosteten Dienst oder dessen privaten Servercode.

**Unabhängige Integration von [3agenteers](https://3agenteers.com/) / Chestnut Innovation GmbH. Kein offizielles Kenko-Angebot. Produktstatus: Beta.**
