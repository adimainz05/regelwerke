# Regelwerk zum Umgang mit personenbezogenen Daten in KI-Werkzeugen

**Verantwortlich:** Adalbert Pojda  
**Version:** 1.0  
**Stand:** 31.08.2026  
**Status:** Verbindlicher persönlicher Arbeitsstandard

## 1. Zweck

Dieses Regelwerk legt fest, welche personenbezogenen Daten unter welchen Voraussetzungen in KI-Werkzeuge eingegeben werden dürfen. Ziel ist, die Grundsätze der Verordnung (EU) 2016/679 (Datenschutz-Grundverordnung, DSGVO) beim Einsatz von KI-Werkzeugen einzuhalten und vertragliche Vertraulichkeitspflichten gegenüber Kunden und Arbeitgebern nicht durch KI-Nutzung zu verletzen.

Die Nutzung eines KI-Werkzeugs entbindet nicht von der datenschutzrechtlichen Verantwortung. Fehlt eine Rechtsgrundlage oder eine erforderliche vertragliche Absicherung, dürfen die betroffenen Daten nicht eingegeben werden, unabhängig davon, wie nützlich das Ergebnis wäre.

## 2. Geltungsbereich

Das Regelwerk gilt für alle KI-Werkzeuge (Chat-Oberflächen, APIs, Agenten, MCP-Server, lokal betriebene Modelle), die Adalbert Pojda geschäftlich oder privat einsetzt, sowie für alle personenbezogenen Daten, die dabei verarbeitet werden könnten – eigene, von Kunden, Arbeitgebern, Kollegen oder Dritten.

Es gilt unabhängig davon, ob die Eingabe als Text, Datei-Upload, Bildschirmfreigabe, Sprachnachricht oder über einen verbundenen Konnektor (E-Mail, Kalender, CRM u. Ä.) erfolgt.

Dieses Regelwerk ersetzt keine unternehmens- oder kundenspezifischen Datenschutzvorgaben. Sind solche strenger, haben sie Vorrang.

## 3. Grundsätze

1. Verarbeitung personenbezogener Daten in einem KI-Werkzeug braucht eine Rechtsgrundlage nach Art. 6 DSGVO – "es könnte nützlich sein" genügt nicht.

2. Datenminimierung gilt auch gegenüber KI-Werkzeugen: nur eingeben, was für die konkrete Aufgabe erforderlich ist, nicht ganze Datensätze aus Bequemlichkeit.

3. Zweckbindung gilt fort: Daten, die zu einem bestimmten Zweck erhoben wurden, dürfen nicht ohne Weiteres für eine KI-gestützte Auswertung zu einem anderen Zweck verwendet werden.

4. Vertrauliche Informationen Dritter (Kunden, Arbeitgeber) unterliegen zusätzlich zur DSGVO häufig eigenen Geheimhaltungspflichten (NDA, Arbeitsvertrag, Kundenvertrag) – diese gelten unabhängig vom Personenbezug und sind gesondert zu prüfen.

5. Bei Zweifeln an der Zulässigkeit gilt die strengere Einstufung, nicht die praktikablere.

6. Anonymisierung oder Pseudonymisierung vor der Eingabe ist die bevorzugte Lösung, wenn sie den Zweck der Aufgabe nicht vereitelt.

## 4. Datenkategorien und Freigabestufen

### 4.1 Stufe A: Unbedenklich

Anonymisierte, aggregierte oder ohnehin öffentlich zugängliche Informationen ohne Personenbezug im Einzelfall. Beispiele: allgemeine Marktdaten, veröffentlichte Fachartikel, technische Spezifikationen ohne Namen.

Freie Eingabe in KI-Werkzeuge zulässig, soweit keine anderen vertraglichen Beschränkungen bestehen.

### 4.2 Stufe B: Eingeschränkt

Personenbezogene Daten ohne besondere Kategorien nach Art. 9 DSGVO, z. B. Name, geschäftliche E-Mail-Adresse, Funktion, Telefonnummer im geschäftlichen Kontext.

Eingabe nur zulässig, wenn:

- eine Rechtsgrundlage nach Art. 6 DSGVO vorliegt (z. B. Vertragserfüllung, berechtigtes Interesse mit dokumentierter Abwägung), und
- das eingesetzte KI-Werkzeug vertraglich als Auftragsverarbeiter eingebunden ist (Auftragsverarbeitungsvertrag nach Art. 28 DSGVO oder gleichwertige Vereinbarung), und
- bei Übermittlung in ein Drittland (z. B. USA) eine geeignete Garantie nach Art. 44 ff. DSGVO besteht (z. B. Standardvertragsklauseln, Angemessenheitsbeschluss), und
- die Trainingsnutzung der Eingaben durch den Anbieter ausgeschlossen oder abgeschaltet ist, soweit das Werkzeug das anbietet.

Vor der ersten Nutzung eines neuen KI-Werkzeugs für Stufe-B-Daten sind diese vier Punkte zu prüfen und das Ergebnis festzuhalten.

### 4.3 Stufe C: Gesperrt

Besondere Kategorien personenbezogener Daten nach Art. 9 DSGVO (Gesundheit, Gewerkschaftszugehörigkeit, biometrische Daten, sexuelle Orientierung, religiöse/politische Überzeugung u. Ä.), strafrechtlich relevante Daten nach Art. 10 DSGVO, sowie jede personenbezogene Angabe, für die keine Rechtsgrundlage oder keine ausreichende vertragliche Absicherung nach Stufe B vorliegt.

Keine Eingabe in extern betriebene KI-Werkzeuge. Zulässig nur in lokal/on-prem betriebenen Modellen ohne Datenabfluss an Dritte, und auch dort nur mit dokumentierter Rechtsgrundlage.

## 5. Entscheidungslogik

Vor jeder Eingabe personenbezogener Daten in ein KI-Werkzeug:

### Schritt 1: Personenbezug feststellen

Enthält die geplante Eingabe Informationen, die eine natürliche Person direkt oder indirekt identifizierbar machen? Wenn nein, Stufe A, keine weitere Prüfung nach diesem Regelwerk nötig.

### Schritt 2: Kategorie prüfen

Handelt es sich um besondere Kategorien nach Art. 9 DSGVO oder strafrechtliche Daten nach Art. 10 DSGVO? Wenn ja, Stufe C – keine Eingabe in externe Werkzeuge.

### Schritt 3: Rechtsgrundlage und Vertragslage prüfen

Liegt eine Rechtsgrundlage nach Art. 6 DSGVO vor, und ist das Werkzeug vertraglich als Auftragsverarbeiter eingebunden (Art. 28 DSGVO) mit geeigneter Garantie bei Drittlandtransfer? Wenn ja, Stufe B zulässig. Wenn nein, entweder Datengrundlage schaffen, anonymisieren/pseudonymisieren, oder auf die Eingabe verzichten.

### Schritt 4: Trainingsnutzung prüfen

Kann ausgeschlossen werden, dass die Eingabe zum Training des Modells verwendet wird (Anbieter-Einstellung, API- statt Consumer-Zugang, explizites Opt-out)? Wenn nein, ist dies vor der Eingabe von Stufe-B-Daten gesondert zu klären und zu dokumentieren, nicht zu unterstellen.

### Schritt 5: Vertragliche Vertraulichkeit gesondert prüfen

Unabhängig vom DSGVO-Ergebnis: Unterliegen die Daten einer NDA, einer Kundenvertraulichkeitsklausel oder einer arbeitsvertraglichen Geheimhaltungspflicht? Wenn ja, gilt die strengere dieser Vorgaben zusätzlich zur DSGVO-Einstufung.

## 6. Anonymisierung und Pseudonymisierung

Wo immer der Zweck der Aufgabe es zulässt, sind Namen, Kontaktdaten und andere direkte Identifikatoren vor der Eingabe zu entfernen oder durch Platzhalter zu ersetzen (z. B. "Kunde A" statt Firmenname, "Mitarbeiter 1" statt Klarname).

Eine erfolgreiche Anonymisierung setzt voraus, dass die betroffene Person auch durch Kombination mit anderen verfügbaren Informationen nicht mehr identifizierbar ist. Bloßes Entfernen des Namens bei sehr spezifischem Kontext (z. B. eindeutige Projektdetails, seltene Kombination von Merkmalen) genügt nicht.

## 7. KI-Werkzeuge mit Verbindung zu Drittsystemen (Konnektoren/MCP)

Werkzeuge, die lesenden oder schreibenden Zugriff auf E-Mail-Postfächer, Kalender, CRM-Systeme oder andere Datenquellen mit personenbezogenen Daten haben, unterliegen diesem Regelwerk in vollem Umfang für jede Information, die dabei tatsächlich verarbeitet wird – unabhängig davon, ob sie manuell eingegeben oder automatisiert abgerufen wurde.

Vor der Freischaltung eines neuen Konnektors ist zu prüfen, welche Datenkategorien er potenziell offenlegt, und die Freigabe entsprechend Abschnitt 4 einzustufen.

## 8. Aufbewahrung und Löschung

Chatverläufe und Konversationshistorien mit personenbezogenen Daten der Stufe B unterliegen denselben Löschungspflichten wie andere Verarbeitungen dieser Daten. Wo das KI-Werkzeug eine Historie dauerhaft speichert, ist zu prüfen, ob eine Löschmöglichkeit besteht und diese bei Wegfall des Verarbeitungszwecks zu nutzen.

## 9. Rechtsquellen

Für dieses Regelwerk sind insbesondere folgende Vorschriften maßgeblich:

1. [Verordnung (EU) 2016/679 (Datenschutz-Grundverordnung)](https://eur-lex.europa.eu/eli/reg/2016/679), insbesondere Art. 5 (Grundsätze), Art. 6 (Rechtmäßigkeit), Art. 9 (besondere Kategorien), Art. 10 (strafrechtliche Daten), Art. 28 (Auftragsverarbeitung), Art. 44 ff. (Drittlandtransfer).

2. Bundesdatenschutzgesetz (BDSG) in der jeweils geltenden Fassung, ergänzend zur DSGVO.

Anbieterspezifische Regelungen (Auftragsverarbeitungsverträge, Trainingsnutzungs-Einstellungen, Sitz der Datenverarbeitung) ändern sich häufig und sind vor jeder neuen Werkzeug-Nutzung anhand der aktuellen Anbieter-Dokumentation zu prüfen, nicht aus früheren Prüfungen zu unterstellen.

Dieses Regelwerk ist ein Arbeitsstandard und keine individuelle Rechtsberatung.

## 10. Maschinenlesbare Regeln für andere Sprachmodelle

Der folgende JSON Abschnitt ist normativ. Ein Sprachmodell soll die Regeln in der angegebenen Prioritätsreihenfolge anwenden. Bei einem Widerspruch zwischen dem JSON Abschnitt und dem übrigen Regelwerk gilt die strengere Einstufung.

```json
{
  "policy_id": "ki_datenschutz_adalbert_pojda",
  "version": "1.0",
  "valid_as_of": "2026-08-31",
  "language": "de",
  "owner": "Adalbert Pojda",
  "scope": [
    "chat_input",
    "file_upload",
    "connector_data",
    "api_call"
  ],
  "levels": {
    "A": {
      "name": "Unbedenklich",
      "condition": "No personal data in the individual case, or already public/aggregated information.",
      "action": "May be entered freely, subject to any separate contractual restrictions."
    },
    "B": {
      "name": "Eingeschränkt",
      "condition": "Personal data without special categories under GDPR Art. 9, e.g. business contact details.",
      "action": "Enter only if a legal basis (Art. 6 GDPR), a data processing agreement (Art. 28 GDPR), an adequate third-country transfer safeguard (Art. 44 ff. GDPR), and exclusion of training use are all confirmed and documented."
    },
    "C": {
      "name": "Gesperrt",
      "condition": "Special category data (GDPR Art. 9), criminal offense data (GDPR Art. 10), or personal data lacking a legal basis or adequate contractual safeguard.",
      "action": "Do not enter into externally operated AI tools. Only permissible in locally/on-premise operated models without data leaving the controller's environment, with a documented legal basis."
    }
  },
  "decision_rules": [
    {
      "priority": 10,
      "if": "The planned input contains no personal data.",
      "then": "Apply level A, no further check required under this policy."
    },
    {
      "priority": 20,
      "if": "The data falls under GDPR Article 9 (special categories) or Article 10 (criminal offense data).",
      "then": "Apply level C. Do not enter into external tools."
    },
    {
      "priority": 30,
      "if": "A legal basis under Article 6 exists and the tool is bound by a data processing agreement under Article 28 with adequate third-country safeguards, and training use is excluded or disabled.",
      "then": "Apply level B."
    },
    {
      "priority": 40,
      "if": "Any of the level B conditions cannot be confirmed.",
      "then": "Anonymize or pseudonymize the data before entry, obtain the missing legal or contractual basis, or refrain from entering the data."
    },
    {
      "priority": 50,
      "if": "The data is also subject to a non-disclosure agreement, client confidentiality clause, or employment confidentiality obligation.",
      "then": "Apply the stricter of the GDPR-based level and the contractual confidentiality obligation."
    },
    {
      "priority": 60,
      "if": "The correct level remains uncertain.",
      "then": "Apply the stricter level."
    }
  ],
  "connector_rule": "Any connector or MCP server with read or write access to a data source containing personal data is subject to this policy for every piece of information it actually processes, regardless of whether it was entered manually or retrieved automatically.",
  "retention_rule": "Chat histories and conversation logs containing level B personal data are subject to the same deletion obligations as other processing of that data.",
  "conflict_rule": "If any rule conflicts with a legal requirement or a stricter organization-specific or client-specific data protection policy, apply the stricter requirement and document the deviation from this policy."
}
```

## 11. Veröffentlichung und dauerhafter Zugriff

Diese Datei ist Teil des öffentlichen Regelwerk-Katalogs (siehe README des Repositories) und soll als zentrale, versionierte Quelle verwendet werden.

Kanonische Adresse:

`https://raw.githubusercontent.com/adimainz05/regelwerke/main/KI_Datenschutzregelwerk_Adalbert_Pojda.md`

Repository-Übersicht: `https://github.com/adimainz05/regelwerke`

Anweisung für ein anderes Sprachmodell:

> Lade vor der Eingabe personenbezogener Daten in ein KI-Werkzeug das Regelwerk unter https://raw.githubusercontent.com/adimainz05/regelwerke/main/KI_Datenschutzregelwerk_Adalbert_Pojda.md. Wende die maschinenlesbaren Entscheidungsregeln verbindlich an. Verwende bei Unsicherheit die strengere Einstufung.

Bei jeder Änderung sind Versionsnummer und Stand zu aktualisieren.

## 12. Inkrafttreten und Überprüfung

Dieses Regelwerk gilt ab dem 31.08.2026.

Es ist bei Änderungen der Rechtslage, bei neuen anbieterseitigen Vertragsbedingungen der eingesetzten KI-Werkzeuge oder der eigenen Arbeitsprozesse zu überprüfen. Unabhängig davon wird eine jährliche Prüfung empfohlen.

**Verantwortlich für Pflege und Freigabe:** Adalbert Pojda
