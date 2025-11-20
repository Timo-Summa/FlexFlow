## 1. Project Scope & Doelgroep

**Algemene functionaliteit:**
- Voor welke doelgroep is dit systeem bedoeld? (skiërs/snowboarders, instructeurs, skischolen, particulieren)
Voornamelijk voor particulieren die zich willen voor bereiden op hun winter sport vakantie. Hierbij hebben we een compleet beginner tot zwaar gevorderd rond lopen.

- Welke hoofdfuncties moet het systeem hebben? (les boeken, rooster beheer, betalingen, etc.)
Lessen boeken, klanten en leraren beheren, Rooster maken, facturatie + betallingen noteren, Klant contact onderhoud ( denk aan het notificeren van lessen of het uitsturen van een nieuwsbrief), klant volg systeem.

- Moet het systeem werken voor één skischool of meerdere scholen/locaties?
Het liefst voor meerdere.

- Welke talen moet het systeem ondersteunen?
Nederlands en engels, maar de uitbreiding naar duits en frans zou belangerijk zijn.

**Platform vereisten:**

- Moet de React Native app werken op iOS, Android, of beide? beide
- Heb je ook een web admin panel nodig naast de mobiele app? ja
- Moeten instructeurs en klanten dezelfde app gebruiken of aparte interfaces? Ik wil dat de instructeur in eerst instantie een klant is die meer toegang krijgt om bijvoorbeeld zijn rooster te zien en feedback achter te laten per klant over de voortgang van de les.

## 2. Gebruikersrollen & Functionaliteiten

**Welke gebruikersrollen heb je nodig?**

- Klanten/studenten
- Instructeurs/leraren
- Skischool administrators
- Super administrators

**Voor elke rol, welke functionaliteiten zijn nodig?**

- Klanten/studenten
	- Account registratie en profiel beheer
	- Les zoeken en boeken
	- Zijn geplande afspraken inzien
- Instructeurs/leraren
	- Rooster/planning bekijken
	- per klant/student moeten een instructeur/leraar een leerling volg systeem invullen. 
- Skischool administrators
	- Account registratie en profiel beheer
	- Les zoeken en boeken
	- Rooster/planning bekijken
	- Betalingen verwerken
	- Communicatie tussen partijen
	- Rapportages en statistieken
- Super administrators
	- Moeten de verschillende ski/snowboard schollen kunnen beheren.
 


## 3. Les Planning Functionaliteiten

**Les types en structuur:**

- Welke soorten lessen bied je aan? (privé, groep, beginners, gevorderden, kinderen, volwassenen)
	- we bieden 2 type lessen: 1 baan huur waarbij 1 persoon de baan afneemt voor meerdere mensen. deze mensen willen we wel toe kunnen voegen aan de groep die de baan huurt. optie 2 is dat mensen in een groep geplaast worden. dit kan als prive of met meerdere mensen.
- Hoe lang duren lessen standaard? (1 uur, halve dag, hele dag)
	- 1 uur
- Kunnen lessen herhaald worden? (cursussen over meerdere dagen)
	- ja je kan 1 tot 20 lessen nemen. x aantal lessen zit wel verschillende prijs modelen op.
- Moeten lessen gekoppeld zijn aan specifieke locaties/pistes?
	- de optie moet er wel zijn

**Planning en beschikbaarheid:**

- Hoe ver van tevoren kunnen lessen geboekt worden?
	- in princiepe maakt het me niet uit hoever van te voren.
- Kunnen instructeurs hun eigen beschikbaarheid instellen?
	- het liefst wel maar geen hoge prio.
- Moeten er minimum/maximum deelnemers per les zijn?
	- ja maar dit moet instellbaar zijn per les
- Hoe wordt omgegaan met annuleringen en wijzigingen?
	- tot 3 dagen van te voren kan een les afgezecht worden en/of gewijziged. erna vervald de les.
- Moeten weersomstandigheden meegenomen worden in de planning?
	- nee

## 4. Betaling & Prijsstelling

**Betaalsysteem:**

- Welke betaalmethoden moet je ondersteunen? (iDeal, creditcard, PayPal, etc.)
	- cash, pin of bank betalling
- Moet betaling vooraf, achteraf, of beide mogelijk zijn?
	- beide
- Moeten er kortingscodes of seizoenspassen ondersteund worden?
	- nee
- Heb je verschillende prijzen voor verschillende periodes? (hoogseizoen/laagseizoen)
	- nee

**Prijsstructuur:**

- Hoe bepaal je de prijs per les? (per persoon, per groep, per uur)
	- op basis van de les moet de prijs ingesteld worden
- Zijn er toeslagen voor specifieke instructeurs of tijdsloten?
	- nee
- Moeten er automatische prijsaanpassingen zijn?
	- ja

## 5. Communicatie & Notificaties

**Communicatiesysteem:**

- Moeten gebruikers berichten kunnen sturen naar instructeurs/administrators?
	- nee
- Welke notificaties zijn belangrijk? 
	- bevestigingen, herinneringen, annuleringen
- Via welke kanalen: push notifications, email, SMS?
	- alleen email voor nu
- In welke talen moeten communicatie plaatsvinden?
	- we moeten de optie hebben om het in engels en nederlands de mails op te kunnen stellen. Liefst zouden we bij houden welke taal de gebruiker zijn mail wil hebben en die taal die versturen.

## 6. Data & Integraties

**Gebruikersdata:**

- Welke informatie moet je van klanten verzamelen? (niveau, ervaring, medische info)
	- NAW gegevens
	- leeftijd / geslacht
	- email + telefoon
	- Niveau / ervaring
	- extra notities en/of een optie om iemand te markeren
- Moeten instructeur certificaten en kwalificaties bijgehouden worden?
	- zou fijn zijn als dat kan niet noodzakelijk
- Heb je een CRM integratie nodig?
	- nee

**Externe integraties:**

- Moet het systeem integreren met bestaande boekingssystemen?
	- nee 
- Heb je weer-APIs nodig voor omstandigheden?
	- nee
- Moeten skischool websites gekoppeld worden?
	- ja, ik zou graag de prijzen, openingstijden en les informatie met de websites kunnen delen
- Integratie met accounting software voor facturen?
	- we zouden graag met exact online willen werken. 

## 7. Technische Vereisten

**Performance en schaalbaarheid:**

- Hoeveel gebruikers verwacht je gelijktijdig?
	- max 500
- Hoeveel lessen per dag/week moeten gepland kunnen worden?
	- max 100 per dag maar kan overtijd uitgroeien
- Welke response tijden zijn acceptabel?
	- dag of 3

**Beveiliging en privacy:**

- Welke persoonlijke data wordt verzameld en hoe lang bewaard?
	- alleen naam, leeftijd en NAW dit moet tot 7 jaar bewaard worden
- Moeten er GDPR/AVG maatregelen geïmplementeerd worden?
	- ja
- Welke authenticatie methoden zijn vereist? (2FA, social login)
	- nee maar wil in de toekomst wel graag 2fa en/of onepass toepassen

## 8. Design & Gebruikerservaring

**UI/UX voorkeuren:**

- Heb je een bestaande huisstijl of kleurenschema?
	- Ik ben zelfs fan van weinig kleur maar er staat nog niks vast.
- Welke sfeer moet de app uitstralen? (professioneel, speels, minimalistisch)
	- professioneel
- Zijn er referentie-apps die je mooi vindt?
	- nee
- Moeten er foto's/video's van instructeurs en locaties getoond worden?
	- nee

**Toegankelijkheid:**

- Moeten er toegankelijkheidsfuncties ingebouwd worden?
	- nee
- Moet de app werken in offline modus voor bepaalde functies?
	- nee altijd met connectie.

## 9. Content Management

**Content beheer:**

- Wie gaat instructeur profielen en beschrijvingen beheren?
	- bedrijfs admin
- Moeten er foto's van locaties/pistes geüpload kunnen worden?
	- nee
- Heb je een blog of nieuws sectie nodig?
	- nee
- Moeten er reviews en beoordelingen mogelijk zijn?
	- nee

## 10. Analytics & Reporting

**Rapportage behoeften:**

- Welke statistieken wil je kunnen inzien? (boekingen, omzet, populaire tijden)
	- boekingen, omzet, hoeveel tijd gevuld is
- Moeten er automatische rapporten gegenereerd worden?
	- nee alleen op aanvraag
- Welke KPI's zijn belangrijk voor jouw business?
	- We willen vooral het klanten contact zo goed mogelijk behouden.
	- Ook willen we de kwaliteit van de lessen waarborgen.

## 11. Launch & Onderhoud

**Go-live planning:**

- Wanneer wil je het systeem live hebben?
	- zo snel mogelijk.
- Heb je een test periode nodig met echte gebruikers?
	- we willen een ci/cd pipeline hebben zodat we de app kunnen update op basis van de feedback die we terug krijgen.
- Moet er data gemigreerd worden uit bestaande systemen?
	- nee, ik wil voor local gebruik wel factories hebben om het systeem volledig te kunnen testen alsof het gebruik word.

**Toekomstige uitbreidingen:**

- Welke functies zouden in de toekomst toegevoegd kunnen worden?
	- nog niet bekend we willen vooral op basis van gebruik dingen verbeteren.
- Moet het systeem uitbreidbaar zijn naar andere wintersportactiviteiten?
	- ja en niet alleen wintersport. 
- Zijn er plannen voor internationale uitbreiding?
	- nee

## 12. Budget & Resources

**Project constraints:**

- Wat is je budget voor dit project?
	- onbekend
- Heb je een team beschikbaar of werk je alleen?
	- ik werk alleen
- Welke deadline heb je in gedachten?
	- 1 maart
- Heb je al hosting/server infrastructure?
	- ja we hebben een docker omgeving.