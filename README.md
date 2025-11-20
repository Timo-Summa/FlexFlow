# FlexFlow

Een flexibel planning- en boekingssysteem voor ski- en snowboardlessen, ontworpen voor particulieren die zich willen voorbereiden op hun wintersportvakantie.

## Projectoverzicht

FlexFlow is een all-in-one platform voor het beheren van lessen, klanten, instructeurs en roosters voor ski- en snowboardscholen. Het systeem biedt ondersteuning voor meerdere locaties en is uitbreidbaar naar andere sportactiviteiten.

### Doelgroep

- **Primaire doelgroep**: Particulieren die zich willen voorbereiden op hun wintersportvakantie
- **Niveaus**: Van complete beginner tot zwaar gevorderd
- **Gebruikersrollen**: Klanten, instructeurs, skischool administrators, super administrators

## Kernfunctionaliteiten

### Lesboekingssysteem
- **Twee lestypen**:
  - Baanhuur: Een persoon huurt een baan voor meerdere mensen (groep kan toegevoegd worden)
  - Groepslessen: Prive of met meerdere personen
- Les duur: 1 uur standaard
- Flexibele cursussen: 1 tot 20 lessen met verschillende prijsmodellen
- Boekingen mogelijk ver van tevoren
- Annulering tot 3 dagen voor de les mogelijk

### Gebruikersbeheer
- Account registratie en profielbeheer
- Verzameling van:
  - NAW gegevens
  - Leeftijd en geslacht
  - Email en telefoon
  - Niveau/ervaring
  - Extra notities en markeringen

### Roostersysteem
- Roosterplanning voor instructeurs
- Maximum 100 lessen per dag (schaalbaar)
- Ondersteuning voor maximaal 500 gelijktijdige gebruikers
- Instelbare minimum/maximum deelnemers per les
- Optionele koppeling aan specifieke locaties/pistes

### Klantvolgsysteem
- Instructeurs kunnen per klant/student een leerlingvolgsysteem invullen
- Voortgang en feedback per les bijhouden
- Ondersteuning voor lange termijn tracking (7 jaar gegevensretentie)

### Facturatie & Betalingen
- Betaalmethoden: Cash, PIN, bankoverdracht
- Betaling vooraf of achteraf mogelijk
- Instellbare prijzen per les
- Automatische prijsaanpassingen
- Exact Online integratie voor accounting

### Communicatie
- Email notificaties voor:
  - Boekingsbevestigingen
  - Herinneringen
  - Annuleringen
- Meertalige emails (Nederlands en Engels, uitbreidbaar naar Duits en Frans)
- Gebruikersvoorkeuren voor taal per klant

### Rapportage
- Statistieken over:
  - Boekingen
  - Omzet
  - Bezettingsgraad
- Rapporten op aanvraag
- Focus op klantcontact en leskwaliteit

## Technische Stack

### Frontend
- **Mobiele App**: React Native (iOS & Android)
- **Web Admin Panel**: Web-based interface

### Gebruikersrollen & Toegang

#### Klanten/Studenten
- Account registratie en profielbeheer
- Les zoeken en boeken
- Geplande afspraken inzien

#### Instructeurs/Leraren
- Alle functionaliteit van klanten
- Rooster/planning bekijken
- Leerlingvolgsysteem invullen per klant

#### Skischool Administrators
- Account registratie en profielbeheer
- Les zoeken en boeken
- Rooster/planning bekijken
- Betalingen verwerken
- Communicatie tussen partijen
- Rapportages en statistieken
- Instructeurprofielen beheren

#### Super Administrators
- Beheer van verschillende ski/snowboard scholen
- Multi-locatie ondersteuning

### Infrastructuur
- Docker omgeving voor hosting
- CI/CD pipeline voor continue updates
- GDPR/AVG compliant
- Toekomstige ondersteuning voor 2FA en OnePass

## Meertaligheid

- **Huidige ondersteuning**: Nederlands en Engels
- **Toekomstige uitbreiding**: Duits en Frans

## Integraties

### Huidig
- Exact Online (accounting en facturatie)

### Toekomstig
- Website koppeling voor:
  - Prijzen
  - Openingstijden
  - Lesinformatie

## Data & Privacy

- **Gegevensretentie**: 7 jaar voor NAW gegevens
- **GDPR/AVG compliant**: Volledige naleving van privacywetgeving
- **Beveiliging**: Veilige opslag van persoonlijke gegevens

## Design Filosofie

- **Stijl**: Professioneel en minimalistisch
- **Kleurenschema**: Voorkeur voor weinig kleur
- **Toegankelijkheid**: Online-first (vereist internet connectie)

## Development & Testing

### Test Omgeving
- Factory systeem voor lokaal testen
- Volledige simulatie van productieomgeving
- Mogelijkheid tot uitgebreid testen met testdata

### Deployment
- CI/CD pipeline voor snelle updates
- Feedback-gedreven ontwikkeling
- Iteratieve verbeteringen op basis van gebruikerservaringen

## Roadmap

### Launch Doelen
- **Target datum**: 1 maart
- Focus op core functionaliteiten
- Stabiel en schaalbaar platform

### Toekomstige Uitbreidingen
- Uitbreiding naar andere sportactiviteiten (niet alleen wintersport)
- Verdere optimalisatie op basis van gebruiksfeedback
- 2FA en OnePass authenticatie
- Instructeur beschikbaarheidsinstellingen

## Schaalbaarheid

- **Huidige capaciteit**:
  - 500 gelijktijdige gebruikers
  - 100 lessen per dag
- **Groei potentieel**: Systeem ontworpen voor schaalbare uitbreiding
- **Multi-locatie**: Ondersteuning voor meerdere scholen en locaties

## KPI's & Doelstellingen

1. **Klantcontact**: Optimaal onderhouden van klantrelaties
2. **Leskwaliteit**: Waarborgen van hoge kwaliteit lessen
3. **Bezettingsgraad**: Maximale benutting van beschikbare capaciteit
4. **Omzet**: Financi�le groei en stabiliteit

## Contact
- Timo Terpstra <TETI@summacollege.nl>
