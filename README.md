# Bern: law history in git

The law of the canton of Bern (Kanton Bern, Switzerland) as a git history: existing article-based histories use one file per article, while the 189 current consolidated additions each use a single `text.md` file. Dated histories record amending acts when they took effect and credit them as commit authors. `git blame` names the act behind a paragraph; `git log` lists changes to a file; checking out a date gives the text recorded for that day.

It follows the shared design of [lexifina/global-law](https://github.com/lexifina/global-law), which places it at `ch-be/`. The federal law is in [lexifina/switzerland-law](https://github.com/lexifina/switzerland-law).

The text is in German, the canton's first official language in the collection, exactly as the canton publishes it.

## What this repository holds

691 acts with 2028 versions in the assembled corpus: the original constitution, cantonal laws, ordinances and regulations, plus 189 current consolidated acts from the systematic collection. The current-text addition includes continuing decrees, decisions and intercantonal agreements. Approval-only entries, a spent term extension and references without normative text are excluded. Older histories retain their existing labels. Separate textual annexes are included for the new acts and the proposed DAFAV correction; other annex sets and normative illustrations remain outside this addition.

The existing published history contains 502 acts with 1839 versions. The addition of 189 current consolidated texts and a separate correction restoring the textual annex of DAFAV (BSG 861.112) at its already recorded date of 1 November 2026 awaits independent review. Five proposed same-date updates had no text changes and are reconciled to the published inputs.

| Folder | Act | Versions | History |
| --- | --- | ---: | --- |
| `101-1-kv/` | Verfassung des Kantons Bern (BSG 101.1) | 6 | oldest version available, then each consolidated version: 11 December 2013 to 1 January 2026 |
| `103-1-pug/` | Publikationsgesetz (BSG 103.1) | 2 | oldest version available, then each consolidated version: 1 July 2014 to 1 December 2021 |
| `105-41-clavaleyres-gesetz-clag/` | Gesetz betreffend den Kantonswechsel der Einwohnergemeinde Clavaleyres im Rahmen eines Zusammenschlusses mit der freiburgischen Gemeinde Murten (BSG 105.41) | 2 | as enacted, then each consolidated version: 1 March 2018 to 1 November 2020 |
| `105-233-kbjg/` | Gesetz betreffend die Durchführung von Abstimmungen über die Kantonszugehörigkeit bernjurassischer Gemeinden (BSG 105.233) | 1 | as enacted, 1 August 2016 |
| `107-1-img/` | Gesetz über die Information und die Medienförderung (BSG 107.1) | 4 | oldest version available, then each consolidated version: 1 June 2014 to 1 September 2026 |
| `108-1-archg/` | Archivierungsgesetz (BSG 108.1) | 5 | as enacted, then each consolidated version: 1 January 2010 to 1 September 2026 |
| `109-1-dvg/` | Gesetz über die digitale Verwaltung (BSG 109.1) | 2 | as enacted, then each consolidated version: 1 March 2023 to 1 September 2026 |
| `121-1-kantonales-burgerrechtsgesetz-kbug/` | Gesetz über das Kantons- und Gemeindebürgerrecht (BSG 121.1) | 3 | oldest version available, then each consolidated version: 1 January 2013 to 1 September 2026 |
| `122-11-nag/` | Gesetz über Niederlassung und Aufenthalt der Schweizerinnen und Schweizer (BSG 122.11) | 3 | oldest version available, then each consolidated version: 1 January 2013 to 1 September 2026 |
| `122-20-eg-aig-und-asylg/` | Einführungsgesetz zum Ausländer- und Integrationsgesetz sowie zum Asylgesetz (BSG 122.20) | 9 | oldest version available, then each consolidated version: 1 November 2013 to 1 September 2026 |
| `124-1-integrationsgesetz-intg/` | Gesetz über die Integration der ausländischen Bevölkerung (BSG 124.1) | 3 | as enacted, then each consolidated version: 1 January 2015 to 1 March 2021 |
| `141-1-prg/` | Gesetz über die politischen Rechte (BSG 141.1) | 14 | oldest version available, then each consolidated version: 1 January 2014 to 1 June 2025 |
| `151-21-grossratsgesetz-grg/` | Gesetz über den Grossen Rat (BSG 151.21) | 4 | as enacted, then each consolidated version: 1 January 2014 to 1 April 2024 |
| `152-01-organisationsgesetz-org/` | Gesetz über die Organisation des Regierungsrates und der Verwaltung (BSG 152.01) | 15 | oldest version available, then each consolidated version: 1 January 2015 to 1 September 2026 |
| `152-04-kdsg/` | Kantonales Datenschutzgesetz (BSG 152.04) | 7 | oldest version available, then each consolidated version: 1 June 2013 to 1 September 2026 |
| `152-05-personendatensammlungsgesetz-pdsg/` | Gesetz über die zentralen Personendatensammlungen (BSG 152.05) | 9 | oldest version available, then each consolidated version: 1 January 2013 to 1 September 2026 |
| `152-031-2-bedag-gesetz-big/` | Gesetz über die Aktiengesellschaft Bedag Informatik (BSG 152.031.2) | 2 | as enacted, then each consolidated version: 1 January 2003 to 1 January 2023 |
| `152-072-eg-glg/` | Einführungsgesetz zum Bundesgesetz über die Gleichstellung von Frau und Mann (BSG 152.072) | 1 | one version (the oldest available), 1 June 2013 |
| `152-321-rstg/` | Gesetz über die Regierungsstatthalterinnen und Regierungsstatthalter (BSG 152.321) | 4 | oldest version available, then each consolidated version: 1 January 2014 to 1 September 2026 |
| `153-01-pg/` | Personalgesetz (BSG 153.01) | 9 | oldest version available, then each consolidated version: 1 September 2014 to 1 September 2026 |
| `153-31-flrg/` | Gesetz über die finanziellen Leistungen an die Mitglieder des Regierungsrates (BSG 153.31) | 2 | as enacted, then each consolidated version: 1 January 2003 to 1 June 2022 |
| `153-41-pkg/` | Gesetz über die kantonalen Pensionskassen (BSG 153.41) | 3 | as enacted, then each consolidated version: 1 January 2015 to 1 September 2026 |
| `155-21-vrpg/` | Gesetz über die Verwaltungsrechtspflege (BSG 155.21) | 6 | oldest version available, then each consolidated version: 1 August 2014 to 1 September 2026 |
| `161-1-gsog/` | Gesetz über die Organisation der Gerichtsbehörden und der Staatsanwaltschaft (BSG 161.1) | 8 | oldest version available, then each consolidated version: 1 June 2013 to 1 May 2026 |
| `168-11-kag/` | Kantonales Anwaltsgesetz (BSG 168.11) | 4 | oldest version available, then each consolidated version: 1 June 2013 to 1 May 2026 |
| `169-11-ng/` | Notariatsgesetz (BSG 169.11) | 2 | oldest version available, then each consolidated version: 1 January 2012 to 1 June 2021 |
| `170-11-gg/` | Gemeindegesetz (BSG 170.11) | 6 | oldest version available, then each consolidated version: 1 January 2014 to 1 February 2025 |
| `170-12-gemeindefusionsgesetz-gfg/` | Gesetz zur Förderung von Gemeindezusammenschlüssen (BSG 170.12) | 4 | oldest version available, then each consolidated version: 1 January 2013 to 1 January 2025 |
| `211-1-eg-zgb/` | Gesetz betreffend die Einführung des Schweizerischen Zivilgesetzbuches (BSG 211.1) | 12 | oldest version available, then each consolidated version: 1 January 2015 to 1 January 2026 |
| `212-223-bbsag/` | Gesetz über die Bernische BVG- und Stiftungsaufsicht (BSG 212.223) | 1 | as enacted, 1 January 2015 |
| `212-225-1/` | Gesetz über die Familienkisten und Familienstiftungen (BSG 212.225.1) | 1 | as enacted, 6 May 1837 |
| `213-22/` | Gesetz über Inkassohilfe und Bevorschussung von Unterhaltsbeiträgen (BSG 213.22) | 2 | oldest version available, then each consolidated version: 1 January 2015 to 1 November 2020 |
| `213-316-kesg/` | Gesetz über den Kindes- und Erwachsenenschutz (BSG 213.316) | 5 | oldest version available, then each consolidated version: 1 January 2014 to 1 September 2026 |
| `213-319-kfsg/` | Gesetz über die Leistungen für Kinder mit besonderem Förder- und Schutzbedarf (BSG 213.319) | 2 | as enacted, then each consolidated version: 1 January 2022 to 1 September 2026 |
| `215-124-1-bpg/` | Gesetz über das bäuerliche Boden- und Pachtrecht (BSG 215.124.1) | 3 | oldest version available, then each consolidated version: 1 January 2013 to 1 April 2021 |
| `215-126-1-eg-bewg/` | Einführungsgesetz zum Bundesgesetz vom 16. Dezember 1983 über den Erwerb von Grundstücken durch Personen im Ausland (BSG 215.126.1) | 5 | oldest version available, then each consolidated version: 1 January 2010 to 1 August 2023 |
| `215-326-2-hstg/` | Handänderungssteuergesetz (BSG 215.326.2) | 4 | oldest version available, then each consolidated version: 1 January 2015 to 1 April 2023 |
| `215-341-kgeoig/` | Kantonales Geoinformationsgesetz (BSG 215.341) | 3 | oldest version available, then each consolidated version: 1 January 2010 to 1 November 2020 |
| `281-1-egschkg/` | Einführungsgesetz zum Bundesgesetz über Schuldbetreibung und Konkurs (BSG 281.1) | 4 | oldest version available, then each consolidated version: 1 January 2011 to 1 January 2026 |
| `311-1-kstrg/` | Gesetz über das kantonale Strafrecht (BSG 311.1) | 4 | as enacted, then each consolidated version: 1 January 2011 to 1 August 2024 |
| `324-1/` | Gesetz betreffend die Einführung des Bundesgesetzes vom 24. Juni 1970 über Ordnungsbussen im Strassenverkehr und die Erhebung von anderen Ordnungsbussen (BSG 324.1) | 1 | one version (the oldest available), 1 January 2003 |
| `326-1-eg-ohg/` | Einführungsgesetz zum Bundesgesetz über die Hilfe an Opfer von Straftaten (BSG 326.1) | 3 | oldest version available, then each consolidated version: 1 January 2011 to 1 March 2021 |
| `341-1-justizvollzugsgesetz-jvg/` | Gesetz über den Justizvollzug (BSG 341.1) | 5 | oldest version available, then each consolidated version: 1 November 2013 to 1 May 2026 |
| `341-13-fmjg/` | Gesetz über freiheitsbeschränkende Massnahmen im Justizvollzug bei Jugendlichen und im Vollzug von Kindesschutzmassnahmen (BSG 341.13) | 3 | oldest version available, then each consolidated version: 1 January 2013 to 1 April 2021 |
| `410-11-landeskirchengesetz-lkg/` | Gesetz über die bernischen Landeskirchen (BSG 410.11) | 3 | oldest version available, then each consolidated version: 1 January 2014 to 1 September 2026 |
| `410-51/` | Gesetz über die jüdischen Gemeinden (BSG 410.51) | 3 | as enacted, then each consolidated version: 1 September 1997 to 1 November 2020 |
| `415-0-kstg/` | Kirchensteuergesetz (BSG 415.0) | 3 | oldest version available, then each consolidated version: 1 January 2013 to 1 November 2020 |
| `423-11-kkfg/` | Kantonales Kulturförderungsgesetz (BSG 423.11) | 3 | as enacted, then each consolidated version: 1 January 2013 to 1 November 2021 |
| `426-11-nschg/` | Naturschutzgesetz (BSG 426.11) | 4 | oldest version available, then each consolidated version: 1 January 2013 to 1 January 2023 |
| `426-41-denkmalpflegegesetz-dpg/` | Gesetz über die Denkmalpflege (BSG 426.41) | 2 | oldest version available, then each consolidated version: 1 September 2009 to 1 November 2021 |
| `426-51-pwg/` | Gesetz über die Pärke von nationaler Bedeutung und das Weltnaturerbe (BSG 426.51) | 2 | as enacted, then each consolidated version: 1 January 2013 to 1 November 2020 |
| `430-121-blmvg/` | Gesetz über die Aktiengesellschaft Berner Lehrmittel- und Medienverlag (BSG 430.121) | 1 | as enacted, 1 January 2003 |
| `430-250-lag/` | Gesetz über die Anstellung der Lehrkräfte (BSG 430.250) | 4 | oldest version available, then each consolidated version: 1 January 2015 to 1 January 2022 |
| `432-31-msg/` | Musikschulgesetz (BSG 432.31) | 2 | as enacted, then each consolidated version: 1 January 2012 to 1 March 2020 |
| `432-210-vsg/` | Volksschulgesetz (BSG 432.210) | 9 | oldest version available, then each consolidated version: 1 August 2013 to 1 September 2026 |
| `433-12-misg/` | Mittelschulgesetz (BSG 433.12) | 6 | oldest version available, then each consolidated version: 1 August 2015 to 1 September 2026 |
| `435-11-berg/` | Gesetz über die Berufsbildung, die Weiterbildung und die Berufsberatung (BSG 435.11) | 5 | oldest version available, then each consolidated version: 1 January 2015 to 1 September 2026 |
| `435-311-ifzg/` | Gesetz über das Interregionale Fortbildungszentrum (BSG 435.311) | 2 | oldest version available, then each consolidated version: 1 January 2006 to 1 November 2021 |
| `435-411-fag/` | Gesetz über die Berner Fachhochschule (BSG 435.411) | 3 | oldest version available, then each consolidated version: 1 August 2015 to 1 January 2023 |
| `436-11-unig/` | Gesetz über die Universität (BSG 436.11) | 3 | oldest version available, then each consolidated version: 1 August 2015 to 1 January 2023 |
| `436-91-phg/` | Gesetz über die deutschsprachige Pädagogische Hochschule (BSG 436.91) | 4 | oldest version available, then each consolidated version: 1 August 2015 to 1 January 2023 |
| `437-11-kspofog/` | Kantonales Sportförderungsgesetz (BSG 437.11) | 5 | oldest version available, then each consolidated version: 1 January 2004 to 1 September 2026 |
| `438-31-abg/` | Gesetz über die Ausbildungsbeiträge (BSG 438.31) | 2 | oldest version available, then each consolidated version: 1 August 2013 to 1 November 2021 |
| `521-1-kbsg/` | Kantonales Bevölkerungsschutzgesetz (BSG 521.1) | 4 | as enacted, then each consolidated version: 1 January 2015 to 1 January 2026 |
| `522-1-kzsg/` | Kantonales Zivilschutzgesetz (BSG 522.1) | 1 | as enacted, 1 January 2026 |
| `525-2/` | Gesetz über Beiträge an Schiessanlagen und an das ausserdienstliche Schiesswesen (BSG 525.2) | 2 | oldest version available, then each consolidated version: 1 January 2002 to 1 April 2021 |
| `551-1-polg/` | Polizeigesetz (BSG 551.1) | 8 | oldest version available, then each consolidated version: 1 January 2013 to 1 November 2026 |
| `551-4-sdpg/` | Gesetz über das Erbringen von Sicherheitsdienstleistungen durch Private (BSG 551.4) | 2 | as enacted, then each consolidated version: 1 January 2020 to 1 September 2026 |
| `555-1-frg/` | Gesetz über die Ruhe an öffentlichen Feiertagen (BSG 555.1) | 3 | oldest version available, then each consolidated version: 1 January 2010 to 1 April 2021 |
| `620-0-fhg/` | Finanzhaushaltsgesetz (BSG 620.0) | 7 | oldest version available, then each consolidated version: 1 January 2015 to 1 September 2026 |
| `621-2-investitionsfondsgesetz-invfg/` | Gesetz über den Fonds zur Deckung von Investitionsspitzen (BSG 621.2) | 1 | as enacted, 1 April 2010 |
| `621-3-snbfg/` | Gesetz über den SNB-Gewinnausschüttungsfonds (BSG 621.3) | 3 | as enacted, then each consolidated version: 31 December 2015 to 1 January 2023 |
| `622-1-kfkg/` | Kantonales Finanzkontrollgesetz (BSG 622.1) | 6 | oldest version available, then each consolidated version: 1 September 2014 to 1 September 2026 |
| `631-1-filag/` | Gesetz über den Finanz- und Lastenausgleich (BSG 631.1) | 7 | oldest version available, then each consolidated version: 1 August 2013 to 1 January 2025 |
| `641-1-stbg/` | Staatsbeitragsgesetz (BSG 641.1) | 3 | oldest version available, then each consolidated version: 1 January 2014 to 1 March 2020 |
| `661-11-stg/` | Steuergesetz (BSG 661.11) | 9 | oldest version available, then each consolidated version: 1 January 2016 to 1 January 2026 |
| `661-611-strkg/` | Gesetz über die Steuerrekurskommission (BSG 661.611) | 1 | one version (the oldest available), 1 January 2011 |
| `662-1-eschg/` | Gesetz über die Erbschafts- und Schenkungssteuer (BSG 662.1) | 1 | one version (the oldest available), 1 January 2014 |
| `682-1/` | Gesetz über das Salzregal (BSG 682.1) | 1 | one version (the oldest available), 1 January 2007 |
| `704-1-see-und-flussufergesetz-sfg/` | Gesetz über See- und Flussufer (BSG 704.1) | 2 | oldest version available, then each consolidated version: 1 January 2009 to 1 November 2020 |
| `711-0-kentg/` | Kantonales Gesetz über die Enteignung (BSG 711.0) | 3 | oldest version available, then each consolidated version: 1 January 2011 to 1 January 2026 |
| `721-0-baug/` | Baugesetz (BSG 721.0) | 9 | oldest version available, then each consolidated version: 1 January 2015 to 1 September 2026 |
| `724-1-kog/` | Koordinationsgesetz (BSG 724.1) | 2 | oldest version available, then each consolidated version: 1 September 2009 to 1 April 2023 |
| `732-11-sg/` | Strassengesetz (BSG 732.11) | 4 | oldest version available, then each consolidated version: 1 January 2012 to 1 February 2024 |
| `741-1-keng/` | Kantonales Energiegesetz (BSG 741.1) | 4 | as enacted, then each consolidated version: 1 January 2012 to 1 January 2026 |
| `741-3-bkw-gesetz-bkwg/` | Gesetz über die Beteiligung des Kantons an der BKW AG (BSG 741.3) | 1 | as enacted, 1 October 2018 |
| `751-11-wasserbaugesetz-wbg/` | Gesetz über Gewässerunterhalt und Wasserbau (BSG 751.11) | 4 | oldest version available, then each consolidated version: 1 January 2015 to 1 January 2025 |
| `752-32-wvg/` | Wasserversorgungsgesetz (BSG 752.32) | 3 | oldest version available, then each consolidated version: 1 January 2003 to 1 August 2020 |
| `752-41-wng/` | Wassernutzungsgesetz (BSG 752.41) | 4 | oldest version available, then each consolidated version: 1 August 2011 to 1 August 2020 |
| `761-11-ksvg/` | Kantonales Strassenverkehrsgesetz (BSG 761.11) | 1 | one version (the oldest available), 1 January 2011 |
| `761-611-bsfg/` | Gesetz über die Besteuerung der Strassenfahrzeuge (BSG 761.611) | 2 | oldest version available, then each consolidated version: 1 January 2013 to 1 April 2021 |
| `762-4/` | Gesetz über den öffentlichen Verkehr (BSG 762.4) | 2 | oldest version available, then each consolidated version: 1 January 2008 to 1 August 2020 |
| `762-5-blsg/` | Gesetz über die Beteiligung des Kantons an der BLS AG und an der BLS Netz AG (BSG 762.5) | 1 | as enacted, 1 November 2025 |
| `767-1-schifffahrtsgesetz/` | Gesetz über die Schifffahrt und die Besteuerung der Schiffe (BSG 767.1) | 3 | oldest version available, then each consolidated version: 1 July 2005 to 1 August 2024 |
| `811-01-gesg/` | Gesundheitsgesetz (BSG 811.01) | 8 | oldest version available, then each consolidated version: 1 January 2014 to 1 September 2026 |
| `811-51-schpg/` | Gesetz zum Schutz vor Passivrauchen (BSG 811.51) | 2 | as enacted, then each consolidated version: 1 July 2009 to 1 July 2021 |
| `812-11-spvg/` | Spitalversorgungsgesetz (BSG 812.11) | 7 | as enacted, then each consolidated version: 1 January 2014 to 1 September 2026 |
| `815-21-eg-krg/` | Einführungsgesetz zur eidgenössischen Krebsregistrierungsgesetzgebung (BSG 815.21) | 2 | as enacted, then each consolidated version: 1 January 2020 to 1 March 2021 |
| `821-0-kgschg/` | Kantonales Gewässerschutzgesetz (BSG 821.0) | 3 | oldest version available, then each consolidated version: 1 January 2007 to 1 August 2020 |
| `822-1-abfallgesetz-abfg/` | Gesetz über die Abfälle (BSG 822.1) | 4 | oldest version available, then each consolidated version: 1 July 2008 to 1 August 2020 |
| `823-1-lufthygienegesetz-lhg/` | Gesetz zur Reinhaltung der Luft (BSG 823.1) | 3 | oldest version available, then each consolidated version: 1 January 2011 to 1 August 2025 |
| `832-71-kfamzg/` | Gesetz über die Familienzulagen (BSG 832.71) | 3 | oldest version available, then each consolidated version: 1 January 2015 to 1 November 2020 |
| `833-21-eag/` | Gesetz über das Einigungsamt (BSG 833.21) | 2 | oldest version available, then each consolidated version: 1 June 2013 to 1 April 2021 |
| `836-11-amg/` | Arbeitsmarktgesetz (BSG 836.11) | 7 | oldest version available, then each consolidated version: 1 January 2010 to 1 September 2026 |
| `841-11-eg-ahvg/` | Einführungsgesetz zum Bundesgesetz über die Alters- und Hinterlassenenversicherung (BSG 841.11) | 2 | oldest version available, then each consolidated version: 1 January 2008 to 1 November 2020 |
| `841-21-eg-ivg/` | Einführungsgesetz zum Bundesgesetz über die Invalidenversicherung (BSG 841.21) | 1 | one version (the oldest available), 1 January 2008 |
| `841-31-eg-elg/` | Einführungsgesetz zum Bundesgesetz über Ergänzungsleistungen zur Alters-, Hinterlassenen- und Invalidenversicherung (BSG 841.31) | 3 | oldest version available, then each consolidated version: 1 January 2012 to 1 January 2025 |
| `842-11-eg-kumv/` | Gesetz betreffend die Einführung der Bundesgesetze über die Kranken-, die Unfall- und die Militärversicherung (BSG 842.11) | 5 | oldest version available, then each consolidated version: 1 January 2014 to 1 September 2026 |
| `854-1/` | Gesetz über die Verbesserung des Wohnungsangebotes (BSG 854.1) | 2 | oldest version available, then each consolidated version: 1 January 2012 to 1 April 2021 |
| `860-1-sozialhilfegesetz-shg/` | Gesetz über die öffentliche Sozialhilfe (BSG 860.1) | 9 | oldest version available, then each consolidated version: 1 January 2014 to 1 September 2026 |
| `860-2-slg/` | Gesetz über die sozialen Leistungsangebote (BSG 860.2) | 3 | as enacted, then each consolidated version: 1 January 2022 to 1 September 2026 |
| `860-3-blg/` | Gesetz über die Leistungen für Menschen mit Behinderungen (BSG 860.3) | 2 | as enacted, then each consolidated version: 1 January 2024 to 1 September 2026 |
| `861-1-safg/` | Gesetz über die Sozialhilfe im Asyl- und Flüchtlingsbereich (BSG 861.1) | 3 | as enacted, then each consolidated version: 1 July 2020 to 1 September 2026 |
| `871-11-ffg/` | Feuerschutz- und Feuerwehrgesetz (BSG 871.11) | 4 | oldest version available, then each consolidated version: 1 January 2014 to 1 April 2021 |
| `873-11-gvg/` | Gebäudeversicherungsgesetz (BSG 873.11) | 2 | oldest version available, then each consolidated version: 1 January 2012 to 1 April 2021 |
| `901-1-wfg/` | Wirtschaftsförderungsgesetz (BSG 901.1) | 2 | oldest version available, then each consolidated version: 1 January 2005 to 1 April 2021 |
| `901-6-ifg/` | Innovationsförderungsgesetz (BSG 901.6) | 3 | as enacted, then each consolidated version: 1 October 2016 to 1 January 2026 |
| `901-41-bmbg/` | Gesetz über die Beteiligung an der Messepark Bern AG (BSG 901.41) | 1 | as enacted, 1 December 2005 |
| `902-1-kihg/` | Kantonales Gesetz über Investitionshilfe für Berggebiete (BSG 902.1) | 2 | oldest version available, then each consolidated version: 1 January 2010 to 1 April 2021 |
| `910-1-klwg/` | Kantonales Landwirtschaftsgesetz (BSG 910.1) | 6 | oldest version available, then each consolidated version: 1 January 2013 to 1 September 2026 |
| `913-1-vbwg/` | Gesetz über das Verfahren bei Boden- und Waldverbesserungen (BSG 913.1) | 4 | oldest version available, then each consolidated version: 1 January 2012 to 1 April 2021 |
| `916-31/` | Hundegesetz (BSG 916.31) | 2 | as enacted, then each consolidated version: 1 January 2013 to 1 April 2021 |
| `916-141-1-rebg/` | Gesetz über den Rebbau (BSG 916.141.1) | 3 | oldest version available, then each consolidated version: 1 January 2009 to 1 January 2024 |
| `921-11-kwag/` | Kantonales Waldgesetz (BSG 921.11) | 2 | oldest version available, then each consolidated version: 1 January 2014 to 1 April 2021 |
| `922-11-jwg/` | Gesetz über Jagd und Wildtierschutz (BSG 922.11) | 4 | oldest version available, then each consolidated version: 1 June 2011 to 1 February 2026 |
| `923-11-fig/` | Fischereigesetz (BSG 923.11) | 4 | oldest version available, then each consolidated version: 1 November 2009 to 1 December 2021 |
| `930-1-hgg/` | Gesetz über Handel und Gewerbe (BSG 930.1) | 5 | oldest version available, then each consolidated version: 1 January 2014 to 1 March 2027 |
| `931-1-brsg/` | Gesetz über das Bergregal und die Sondernutzung des öffentlichen Untergrunds (BSG 931.1) | 4 | oldest version available, then each consolidated version: 1 January 2009 to 1 December 2021 |
| `935-11-ggg/` | Gastgewerbegesetz (BSG 935.11) | 5 | oldest version available, then each consolidated version: 1 April 2013 to 1 August 2024 |
| `935-52-kgsg/` | Kantonales Geldspielgesetz (BSG 935.52) | 4 | oldest version available, then each consolidated version: 1 January 2013 to 1 September 2026 |
| `935-90-pgg/` | Gesetz über das Prostitutionsgewerbe (BSG 935.90) | 4 | as enacted, then each consolidated version: 1 April 2013 to 1 September 2026 |
| `935-211-teg/` | Tourismusentwicklungsgesetz (BSG 935.211) | 3 | oldest version available, then each consolidated version: 1 July 2012 to 1 April 2021 |
| `951-10-agbekbg/` | Gesetz über die Aktiengesellschaft Berner Kantonalbank (BSG 951.10) | 1 | one version (the oldest available), 1 January 2006 |
| `102-111-sonderstatutsverordnung-sstv/` | Verordnung über das Sonderstatut des Berner Juras und über die französischsprachige Minderheit des Verwaltungskreises Biel/Bienne (BSG 102.111) | 9 | oldest version available, then each consolidated version: 1 September 2013 to 1 January 2026 |
| `102-111-3-r-bjr-rfb/` | Gemeinsames Reglement des Bernjurassischen Rats und des Rats für französischsprachige Angelegenheiten des Verwaltungskreises Biel/Bienne (BSG 102.111.3) | 4 | oldest version available, then each consolidated version: 1 October 2014 to 1 January 2023 |
| `103-11-puv/` | Publikationsverordnung (BSG 103.11) | 3 | oldest version available, then each consolidated version: 1 July 2014 to 1 June 2024 |
| `105-31-ev-wschg/` | Einführungsverordnung zur eidgenössischen Wappenschutzgesetzgebung (BSG 105.31) | 2 | as enacted, then each consolidated version: 1 January 2017 to 1 January 2026 |
| `107-111-imv/` | Verordnung über die Information und die Medienförderung (BSG 107.111) | 5 | oldest version available, then each consolidated version: 1 June 2014 to 1 September 2026 |
| `108-111-archv/` | Archivierungsverordnung (BSG 108.111) | 6 | oldest version available, then each consolidated version: 1 June 2014 to 1 May 2026 |
| `109-111-dvv/` | Verordnung über die digitale Verwaltung (BSG 109.111) | 3 | as enacted, then each consolidated version: 1 March 2023 to 1 November 2026 |
| `121-111-kantonale-burgerrechtsverordnung-kbuv/` | Verordnung über das Kantons- und Gemeindebürgerrecht (BSG 121.111) | 5 | oldest version available, then each consolidated version: 1 July 2014 to 1 September 2026 |
| `122-26-ev-gebv-aig/` | Einführungsverordnung zur Verordnung über die Gebühren zum Ausländer- und Integrationsgesetz (BSG 122.26) | 4 | oldest version available, then each consolidated version: 1 March 2011 to 1 August 2026 |
| `122-161-nav/` | Verordnung über Niederlassung und Aufenthalt der Schweizerinnen und Schweizer (BSG 122.161) | 4 | oldest version available, then each consolidated version: 1 January 2014 to 1 February 2024 |
| `122-201-ev-aig-und-asylg/` | Einführungsverordnung zum Ausländer- und Integrationsgesetz sowie zum Asylgesetz (BSG 122.201) | 4 | oldest version available, then each consolidated version: 1 January 2015 to 1 February 2024 |
| `123-22-ev-awg/` | Einführungsverordnung zum eidgenössischen Ausweisgesetz (BSG 123.22) | 5 | oldest version available, then each consolidated version: 1 August 2012 to 1 February 2024 |
| `124-111-integrationsverordnung-intv/` | Verordnung über die Integration der ausländischen Bevölkerung (BSG 124.111) | 2 | as enacted, then each consolidated version: 1 January 2015 to 1 March 2021 |
| `141-111-skv/` | Verordnung über die Stimmkreise (BSG 141.111) | 6 | as enacted, then each consolidated version: 1 January 2014 to 1 July 2023 |
| `141-112-prv/` | Verordnung über die politischen Rechte (BSG 141.112) | 5 | oldest version available, then each consolidated version: 1 January 2014 to 1 June 2025 |
| `141-113/` | Verordnung über das Stimmregister (BSG 141.113) | 4 | oldest version available, then each consolidated version: 1 January 2014 to 1 February 2024 |
| `141-114-esasv/` | Verordnung über die elektronische Stimmabgabe von Auslandschweizerinnen und Auslandschweizern (BSG 141.114) | 3 | oldest version available, then each consolidated version: 1 January 2014 to 1 March 2021 |
| `141-115-twav/` | Verordnung über die Transparenz bei der Finanzierung von Wahl- und Abstimmungskampagnen (BSG 141.115) | 1 | as enacted, 30 March 2025 |
| `152-11-organisationsverordnung-rr-orv-rr/` | Verordnung über die Organisation des Regierungsrates (BSG 152.11) | 6 | oldest version available, then each consolidated version: 1 March 2014 to 1 March 2023 |
| `152-17-klassifizierungsverordnung-krgv/` | Verordnung über die Klassifizierung, die Veröffentlichung und die Archivierung von Dokumenten zu Regierungsratsgeschäften (BSG 152.17) | 5 | as enacted, then each consolidated version: 1 October 2013 to 1 February 2025 |
| `152-021-begv/` | Verordnung über die Beglaubigung von Unterschriften (BSG 152.021) | 1 | one version (the oldest available), 1 January 2011 |
| `152-025-vmv/` | Verordnung über das Vernehmlassungs- und das Mitberichtsverfahren (BSG 152.025) | 5 | oldest version available, then each consolidated version: 1 February 2015 to 1 September 2026 |
| `152-040-1-kdsv/` | Kantonale Datenschutzverordnung (BSG 152.040.1) | 3 | as enacted, then each consolidated version: 1 January 2009 to 1 September 2026 |
| `152-040-2-isds-dv/` | Direktionsverordnung über Informationssicherheit und Datenschutz (BSG 152.040.2) | 1 | as enacted, 1 April 2011 |
| `152-041-1-personaldatenbekanntgabeverordnung-pdbv/` | Verordnung über die Bekanntgabe von Personaldaten (BSG 152.041.1) | 3 | oldest version available, then each consolidated version: 1 January 2015 to 1 September 2026 |
| `152-051-geres-v/` | Verordnung über die Gemeinderegistersysteme-Plattform (BSG 152.051) | 9 | oldest version available, then each consolidated version: 1 January 2015 to 1 September 2026 |
| `152-052-zpv-v/` | Verordnung über die Zentrale Personenverwaltung (BSG 152.052) | 3 | as enacted, then each consolidated version: 1 March 2021 to 1 September 2026 |
| `152-053-1-pds-dv-fin/` | Direktionsverordnung über die Berechtigungen der Finanzdirektion für die zentralen Personendatensammlungen (BSG 152.053.1) | 2 | as enacted, then each consolidated version: 1 October 2021 to 1 October 2025 |
| `152-053-2-pds-dv-dij/` | Direktionsverordnung über die Berechtigungen der Direktion für Inneres und Justiz für die zentralen Personendatensammlungen (BSG 152.053.2) | 2 | as enacted, then each consolidated version: 1 November 2021 to 1 February 2022 |
| `152-053-3-pds-dv-sid/` | Direktionsverordnung über die Berechtigungen der Sicherheitsdirektion für die zentralen Personendatensammlungen (BSG 152.053.3) | 2 | as enacted, then each consolidated version: 1 March 2022 to 1 May 2022 |
| `152-053-4-pds-dv-gsi/` | Direktionsverordnung über die Berechtigungen der Gesundheits-, Sozial- und Integrationsdirektion für die zentralen Personendatensammlungen (BSG 152.053.4) | 2 | as enacted, then each consolidated version: 1 March 2022 to 1 May 2022 |
| `152-053-5-pds-dv-bkd/` | Direktionsverordnung über die Berechtigungen der Bildungs- und Kulturdirektion für die zentralen Personendatensammlungen (BSG 152.053.5) | 2 | as enacted, then each consolidated version: 1 March 2022 to 1 April 2022 |
| `152-053-6-pds-r-jus/` | Reglement über die Berechtigungen der Gerichtsbehörden und der Staatsanwaltschaft für die zentralen Personendatensammlungen (BSG 152.053.6) | 3 | as enacted, then each consolidated version: 1 March 2022 to 1 January 2024 |
| `152-053-7-pds-dv-weu/` | Direktionsverordnung über die Berechtigungen der Wirtschafts-, Energie- und Umweltdirektion für die zentralen Personendatensammlungen (BSG 152.053.7) | 2 | as enacted, then each consolidated version: 1 March 2022 to 1 October 2022 |
| `152-061/` | Verordnung über den Repräsentationskredit des Regierungsrates (BSG 152.061) | 2 | oldest version available, then each consolidated version: 1 January 2010 to 1 January 2021 |
| `152-141-arv/` | Verordnung über den Auslagenersatz für die Mitglieder des Regierungsrates (BSG 152.141) | 3 | as enacted, then each consolidated version: 1 January 2003 to 1 January 2025 |
| `152-211-organisationsverordnung-sta-orv-sta/` | Verordnung über die Organisation und die Aufgaben der Staatskanzlei (BSG 152.211) | 11 | oldest version available, then each consolidated version: 1 January 2015 to 1 January 2024 |
| `152-211-2-deldv-sta/` | Direktionsverordnung über die Delegation von Befugnissen der Staatskanzlei (BSG 152.211.2) | 5 | oldest version available, then each consolidated version: 1 January 2015 to 1 August 2020 |
| `152-221-111-organisationsverordnung-weu-orv-weu/` | Verordnung über die Organisation und die Aufgaben der Wirtschafts-, Energie- und Umweltdirektion (BSG 152.221.111) | 9 | oldest version available, then each consolidated version: 1 July 2015 to 1 November 2025 |
| `152-221-111-1/` | Verordnung über die Volkswirtschaftskommission (BSG 152.221.111.1) | 4 | oldest version available, then each consolidated version: 1 January 2011 to 1 March 2022 |
| `152-221-111-2-deldv-weu/` | Direktionsverordnung über die Delegation von Befugnissen der Wirtschafts-, Energie- und Umweltdirektion (BSG 152.221.111.2) | 3 | oldest version available, then each consolidated version: 1 January 2015 to 1 July 2023 |
| `152-221-121-organisationsverordnung-gsi-orv-gsi/` | Verordnung über die Organisation und die Aufgaben der Gesundheits-, Sozial- und Integrationsdirektion (BSG 152.221.121) | 18 | oldest version available, then each consolidated version: 1 January 2015 to 1 September 2026 |
| `152-221-121-2-deldv-gsi/` | Direktionsverordnung über die Delegation von Befugnissen der Gesundheits-, Sozial- und Integrationsdirektion (BSG 152.221.121.2) | 9 | oldest version available, then each consolidated version: 1 March 2008 to 1 January 2024 |
| `152-221-131-organisationsverordnung-dij-orv-dij/` | Verordnung über die Organisation und die Aufgaben der Direktion für Inneres und Justiz (BSG 152.221.131) | 9 | oldest version available, then each consolidated version: 1 March 2014 to 1 May 2024 |
| `152-221-131-1-deldv-dij/` | Direktionsverordnung über die Delegation von Befugnissen der Direktion für Inneres und Justiz (BSG 152.221.131.1) | 5 | oldest version available, then each consolidated version: 1 January 2015 to 1 September 2022 |
| `152-221-131-2-spev/` | Verordnung über die stationären und pädagogischen Einrichtungen der Direktion für Inneres und Justiz (BSG 152.221.131.2) | 1 | as enacted, 1 September 2022 |
| `152-221-141-organisationsverordnung-sid-orv-sid/` | Verordnung über die Organisation und die Aufgaben der Sicherheitsdirektion (BSG 152.221.141) | 7 | oldest version available, then each consolidated version: 1 January 2015 to 1 January 2026 |
| `152-221-141-1-deldv-sid/` | Direktionsverordnung über die Delegation von Befugnissen der Sicherheitsdirektion (BSG 152.221.141.1) | 6 | oldest version available, then each consolidated version: 1 February 2014 to 1 March 2025 |
| `152-221-171-organisationsverordnung-fin-orv-fin/` | Verordnung über die Organisation und die Aufgaben der Finanzdirektion (BSG 152.221.171) | 8 | oldest version available, then each consolidated version: 1 January 2015 to 1 July 2025 |
| `152-221-171-1-deldv-fin/` | Direktionsverordnung über die Delegation von Befugnissen der Finanzdirektion (BSG 152.221.171.1) | 3 | oldest version available, then each consolidated version: 1 February 2009 to 1 October 2021 |
| `152-221-181-organisationsverordnung-bkd-orv-bkd/` | Verordnung über die Organisation und die Aufgaben der Bildungs- und Kulturdirektion (BSG 152.221.181) | 8 | oldest version available, then each consolidated version: 1 August 2015 to 1 January 2023 |
| `152-221-181-1-deldv-bkd/` | Direktionsverordnung über die Delegation von Befugnissen der Bildungs- und Kulturdirektion (BSG 152.221.181.1) | 2 | oldest version available, then each consolidated version: 1 August 2008 to 1 November 2022 |
| `152-221-191-organisationsverordnung-bvd-orv-bvd/` | Verordnung über die Organisation und die Aufgaben der Bau- und Verkehrsdirektion (BSG 152.221.191) | 8 | oldest version available, then each consolidated version: 1 January 2015 to 1 September 2026 |
| `152-221-191-1-deldv-bvd/` | Direktionsverordnung über die Delegation von Befugnissen der Bau- und Verkehrsdirektion (BSG 152.221.191.1) | 3 | oldest version available, then each consolidated version: 1 January 2015 to 1 January 2020 |
| `152-256/` | Verordnung über die Taggelder und Reiseentschädigungen der Mitglieder staatlicher Kommissionen (BSG 152.256) | 1 | one version (the oldest available), 1 January 2011 |
| `152-321-2-rstsv/` | Verordnung über die Stellvertretung der Regierungsstatthalterinnen und Regierungsstatthalter (BSG 152.321.2) | 2 | as enacted, then each consolidated version: 1 January 2010 to 1 November 2020 |
| `152-321-4/` | Verordnung über die Amtssitze der Regierungsstatthalterämter (BSG 152.321.4) | 1 | as enacted, 1 January 2010 |
| `152-322-1-osdv/` | Verordnung über die Organisation und die Steuerung der dezentralen Verwaltung der Direktion für Inneres und Justiz (BSG 152.322.1) | 8 | oldest version available, then each consolidated version: 1 January 2013 to 1 May 2024 |
| `152-381-srv/` | Verordnung über die Sprachenregelung im Verwaltungskreis Biel/Bienne und für die regionalen Behörden im Verwaltungskreis Seeland (BSG 152.381) | 3 | oldest version available, then each consolidated version: 1 January 2011 to 1 January 2026 |
| `153-011-1-pv/` | Personalverordnung (BSG 153.011.1) | 15 | oldest version available, then each consolidated version: 1 January 2015 to 1 September 2026 |
| `153-011-2-stvv/` | Stellenvermittlungsverordnung (BSG 153.011.2) | 3 | oldest version available, then each consolidated version: 1 August 2014 to 1 January 2024 |
| `153-011-4/` | Verordnung über die personalrechtliche Stellung von verdeckten Ermittlerinnen und Ermittlern (BSG 153.011.4) | 1 | as enacted, 1 January 2011 |
| `153-011-5-rdv/` | Randdatenverordnung (BSG 153.011.5) | 3 | as enacted, then each consolidated version: 1 January 2020 to 1 September 2026 |
| `153-012-1-praktikantenverordnung-pav/` | Verordnung über das Arbeitsverhältnis der Praktikantinnen und Praktikanten (BSG 153.012.1) | 2 | as enacted, then each consolidated version: 1 January 2009 to 1 January 2025 |
| `153-15/` | Verordnung über die Kantonsvertreterinnen und Kantonsvertreter (BSG 153.15) | 4 | oldest version available, then each consolidated version: 1 June 2013 to 1 January 2024 |
| `153-411-101/` | Reglemente der Bernischen Pensionskasse (BPK) (BSG 153.411.101) | 1 | as enacted, 1 December 2015 |
| `153-421/` | Verordnung über die Aufnahme der Forstwarte und Waldarbeiter des Staates im Stundenlohn in die Versicherungskasse der bernischen Staatsverwaltung (BSG 153.421) | 1 | as enacted, 1 January 1982 |
| `153-471-zulagenverordnung/` | Verordnung über die Gewährung von festen Zulagen an Rentenbezügerinnen und Rentenbezüger der Versicherungskasse der bernischen Staatsverwaltung und der bernischen Lehrerversicherungskasse mit bescheidenen Renten der AHV/IV (BSG 153.471) | 1 | as enacted, 1 January 1990 |
| `154-21-gebuhrenverordnung-gebv/` | Verordnung über die Gebühren der Kantonsverwaltung (BSG 154.21) | 9 | oldest version available, then each consolidated version: 1 February 2015 to 1 September 2026 |
| `154-61-bvgv/` | Verordnung über den Bezug und die Verrechnung von Gebühren und Kosten durch die Verwaltungsbehörden (BSG 154.61) | 1 | one version (the oldest available), 1 January 2013 |
| `154-62/` | Verordnung zur Einführung der Mehrwertsteuer (BSG 154.62) | 1 | as enacted, 1 January 1995 |
| `161-16-jpersr/` | Personalreglement der Gerichtsbehörden und der Staatsanwaltschaft (BSG 161.16) | 2 | as enacted, then each consolidated version: 1 January 2011 to 1 January 2024 |
| `161-17-jwbr/` | Reglement über die Aus- und Weiterbildung in den Gerichtsbehörden und in der Staatsanwaltschaft (BSG 161.17) | 3 | as enacted, then each consolidated version: 1 January 2011 to 1 January 2024 |
| `161-111-1-jlr/` | Reglement der Justizverwaltungsleitung (BSG 161.111.1) | 3 | as enacted, then each consolidated version: 1 January 2011 to 1 January 2024 |
| `161-111-2-jfinr/` | Reglement über Steuerung von Finanzen und Leistungen der Justiz (BSG 161.111.2) | 2 | as enacted, then each consolidated version: 1 January 2011 to 1 January 2024 |
| `162-11-orr-og/` | Organisationsreglement des Obergerichts (BSG 162.11) | 4 | oldest version available, then each consolidated version: 1 June 2013 to 1 January 2025 |
| `162-12-aufsr-og/` | Aufsichtsreglement des Obergerichts (BSG 162.12) | 2 | oldest version available, then each consolidated version: 1 June 2013 to 1 January 2024 |
| `162-13-ir-zsg/` | Informationsreglement der Zivil- und Strafgerichtsbarkeit (BSG 162.13) | 4 | oldest version available, then each consolidated version: 1 June 2013 to 1 January 2026 |
| `162-14/` | Reglement über die Aufgaben und Kompetenzen der als Gerichtsschreiberinnen und Gerichtsschreiber tätigen Personen der Zivil- und Strafgerichtsbarkeit (BSG 162.14) | 2 | as enacted, then each consolidated version: 1 January 2011 to 1 January 2024 |
| `162-16-aufbewahrungsreglement-ar-zsg/` | Reglement über die Aufbewahrung der Unterlagen der erst- und oberinstanzlichen Zivil- und Strafgerichte (BSG 162.16) | 4 | as enacted, then each consolidated version: 1 January 2011 to 1 April 2026 |
| `162-17-delr-og/` | Reglement über die Delegation von Personalbefugnissen des Obergerichts (BSG 162.17) | 4 | as enacted, then each consolidated version: 1 April 2015 to 1 January 2025 |
| `162-18-rsr-zsg/` | Reglement über das Tragen sichtbarer religiöser Symbole und religiöser Kleidung in der Zivil- und Strafgerichtsbarkeit (BSG 162.18) | 1 | as enacted, 1 January 2025 |
| `162-121-geschr-kzmg/` | Geschäftsreglement des kantonalen Zwangsmassnahmengerichts (BSG 162.121) | 2 | as enacted, then each consolidated version: 1 January 2011 to 1 January 2024 |
| `162-122-geschr-wsg/` | Geschäftsreglement des Wirtschaftsstrafgerichts (BSG 162.122) | 2 | as enacted, then each consolidated version: 1 January 2011 to 1 January 2024 |
| `162-511-geschr-jg/` | Geschäftsreglement des Jugendgerichts (BSG 162.511) | 2 | as enacted, then each consolidated version: 1 September 2013 to 1 January 2024 |
| `162-621-orr-vg/` | Organisationsreglement des Verwaltungsgerichts (BSG 162.621) | 4 | oldest version available, then each consolidated version: 1 January 2014 to 1 January 2024 |
| `162-621-1-orr-sva/` | Reglement über die Organisation der Rechtsprechung der sozialversicherungsrechtlichen Abteilung des Verwaltungsgerichts des Kantons Bern (BSG 162.621.1) | 2 | as enacted, then each consolidated version: 1 January 2011 to 1 January 2023 |
| `162-621-2-orr-vra/` | Reglement über die Organisation der Rechtsprechung der verwaltungsrechtlichen Abteilung des Verwaltungsgerichts (BSG 162.621.2) | 1 | one version (the oldest available), 17 May 2018 |
| `162-621-3-orr-calf/` | Reglement über die Organisation der Rechtsprechung der Abteilung für französischsprachige Geschäfte des Verwaltungsgerichts (BSG 162.621.3) | 1 | as enacted, 1 January 2011 |
| `162-622-aufsr-vg/` | Aufsichtsreglement des Verwaltungsgerichts (BSG 162.622) | 1 | as enacted, 1 January 2011 |
| `162-624-geschr-strk/` | Geschäftsreglement der Steuerrekurskommission (BSG 162.624) | 1 | as enacted, 1 January 2011 |
| `162-625-geschr-rkmf/` | Geschäftsreglement der Rekurskommission für Massnahmen gegenüber Fahrzeugführerinnen und Fahrzeugführern (BSG 162.625) | 3 | as enacted, then each consolidated version: 1 January 2011 to 1 January 2024 |
| `162-626-geschr-eschk/` | Geschäftsreglement der Enteignungsschätzungskommission (BSG 162.626) | 1 | as enacted, 1 January 2011 |
| `162-627-geschr-bvk/` | Geschäftsreglement der Bodenverbesserungskommission (BSG 162.627) | 2 | as enacted, then each consolidated version: 1 January 2011 to 1 January 2024 |
| `162-628-archr-vg/` | Reglement über die Archivführung des Verwaltungsgerichts und der übrigen verwaltungsunabhängigen Justizbehörden (BSG 162.628) | 1 | as enacted, 1 January 2011 |
| `162-711-1-orr-staw/` | Organisationsreglement der Staatsanwaltschaft (BSG 162.711.1) | 6 | as enacted, then each consolidated version: 1 January 2011 to 1 December 2025 |
| `162-711-2-ir-staw/` | Informationsreglement der Staatsanwaltschaft (BSG 162.711.2) | 1 | as enacted, 1 January 2011 |
| `162-711-3-archr-staw/` | Archivreglement der Staatsanwaltschaft (BSG 162.711.3) | 1 | as enacted, 1 January 2011 |
| `163-21-geschr-rg-bjs/` | Geschäftsreglement des Regionalgerichts Berner Jura-Seeland (BSG 163.21) | 2 | oldest version available, then each consolidated version: 1 January 2015 to 1 January 2024 |
| `163-22-geschr-rg-eo/` | Geschäftsreglement des Regionalgerichts Emmental-Oberaargau (BSG 163.22) | 2 | as enacted, then each consolidated version: 1 May 2012 to 1 January 2024 |
| `163-23-geschr-rg-bm/` | Geschäftsreglement des Regionalgerichts Bern-Mittelland (BSG 163.23) | 2 | as enacted, then each consolidated version: 1 January 2011 to 1 January 2024 |
| `163-24-geschr-rg-ol/` | Geschäftsreglement des Regionalgerichts Oberland (BSG 163.24) | 2 | oldest version available, then each consolidated version: 1 January 2015 to 1 January 2024 |
| `164-211-geschr-sb-bjs/` | Geschäftsreglement der regionalen Schlichtungsbehörde Berner Jura-Seeland (BSG 164.211) | 2 | as enacted, then each consolidated version: 1 January 2011 to 1 January 2024 |
| `164-212-geschr-sb-eo/` | Geschäftsreglement der regionalen Schlichtungsbehörde Emmental-Oberaargau (BSG 164.212) | 2 | as enacted, then each consolidated version: 1 January 2011 to 1 January 2024 |
| `164-213-geschr-sb-bm/` | Geschäftsreglement der regionalen Schlichtungsbehörde Bern-Mittelland (BSG 164.213) | 2 | as enacted, then each consolidated version: 1 January 2011 to 1 January 2024 |
| `164-214-geschr-sb-ol/` | Geschäftsreglement der regionalen Schlichtungsbehörde Oberland (BSG 164.214) | 2 | as enacted, then each consolidated version: 1 January 2011 to 1 January 2024 |
| `166-21-empv/` | Verordnung über die Entschädigung der Mitglieder der Anwalts- und Notariatsprüfungskommission (BSG 166.21) | 2 | as enacted, then each consolidated version: 1 January 2007 to 1 November 2020 |
| `168-221-1-apv/` | Verordnung über die Anwaltsprüfung (BSG 168.221.1) | 2 | oldest version available, then each consolidated version: 1 October 2014 to 1 March 2020 |
| `168-461-gebv-ab/` | Verordnung über die Gebühren der Anwaltsaufsichtsbehörde (BSG 168.461) | 1 | one version (the oldest available), 1 January 2011 |
| `168-711-eav/` | Verordnung über die Entschädigung der amtlichen Anwältinnen und Anwälte (BSG 168.711) | 2 | as enacted, then each consolidated version: 1 January 2011 to 1 January 2027 |
| `168-811-parteikostenverordnung-pkv/` | Verordnung über die Bemessung des Parteikostenersatzes (BSG 168.811) | 1 | one version (the oldest available), 1 January 2012 |
| `169-81-gebvn/` | Verordnung über die Notariatsgebühren (BSG 169.81) | 2 | as enacted, then each consolidated version: 1 July 2006 to 1 June 2021 |
| `169-112-nv/` | Notariatsverordnung (BSG 169.112) | 5 | oldest version available, then each consolidated version: 1 January 2013 to 1 February 2025 |
| `169-221-npv/` | Verordnung über die Notariatsprüfung (BSG 169.221) | 3 | oldest version available, then each consolidated version: 1 October 2014 to 1 November 2020 |
| `170-111-gv/` | Gemeindeverordnung (BSG 170.111) | 6 | oldest version available, then each consolidated version: 1 January 2014 to 1 January 2026 |
| `170-211-rkv/` | Verordnung über die Regionalkonferenzen (BSG 170.211) | 12 | oldest version available, then each consolidated version: 1 January 2015 to 1 January 2026 |
| `170-212-rkgv/` | Verordnung über das Geschäftsreglement für die Regionalkonferenzen (BSG 170.212) | 3 | oldest version available, then each consolidated version: 1 January 2013 to 1 March 2023 |
| `170-511-fhdv/` | Direktionsverordnung über den Finanzhaushalt der Gemeinden (BSG 170.511) | 5 | oldest version available, then each consolidated version: 1 January 2013 to 1 January 2026 |
| `170-711-archdv-gemeinden/` | Direktionsverordnung über die Verwaltung und Archivierung der Unterlagen von öffentlich-rechtlichen Körperschaften nach Gemeindegesetz und deren Anstalten (BSG 170.711) | 2 | as enacted, then each consolidated version: 1 January 2015 to 1 July 2016 |
| `211-111-1/` | Direktionsverordnung über die Amtssitze der Betreibungs- und Konkursämter sowie Grundbuchämter (BSG 211.111.1) | 2 | as enacted, then each consolidated version: 1 January 2010 to 1 January 2026 |
| `212-121-kzstv/` | Kantonale Zivilstandsverordnung (BSG 212.121) | 3 | oldest version available, then each consolidated version: 23 December 2013 to 1 September 2026 |
| `212-223-1-asvv/` | Verordnung über die Aufsicht über die Stiftungen und die Vorsorgeeinrichtungen (BSG 212.223.1) | 3 | oldest version available, then each consolidated version: 1 January 2012 to 1 January 2023 |
| `212-223-3-gebr-bbsa/` | Gebührenreglement der Bernischen BVG- und Stiftungsaufsicht (BSG 212.223.3) | 5 | as enacted, then each consolidated version: 1 January 2015 to 1 January 2025 |
| `213-221-ibv/` | Verordnung über Inkassohilfe und Bevorschussung von Unterhaltsbeiträgen (BSG 213.221) | 3 | as enacted, then each consolidated version: 1 January 2015 to 1 November 2020 |
| `213-316-1-kesv/` | Verordnung über den Kindes- und Erwachsenenschutz (BSG 213.316.1) | 5 | oldest version available, then each consolidated version: 1 March 2014 to 1 February 2025 |
| `213-318-zav/` | Verordnung über die Zusammenarbeit der kommunalen Dienste mit den Kindes- und Erwachsenenschutzbehörden und die Abgeltung der den Gemeinden anfallenden Aufwendungen (BSG 213.318) | 5 | as enacted, then each consolidated version: 1 January 2013 to 1 January 2024 |
| `213-319-1-kfsv/` | Verordnung über die Leistungen für Kinder mit besonderem Förder- und Schutzbedarf (BSG 213.319.1) | 3 | as enacted, then each consolidated version: 1 January 2022 to 1 August 2025 |
| `213-319-2-alkv/` | Verordnung über die Aufsicht über stationäre Einrichtungen und ambulante Leistungen für Kinder (BSG 213.319.2) | 3 | as enacted, then each consolidated version: 1 January 2022 to 1 August 2025 |
| `213-321-owkv/` | Verordnung über die Organisation der Oberwaisenkammer (BSG 213.321) | 1 | one version (the oldest available), 1 January 2013 |
| `213-361-esbv/` | Verordnung über die Entschädigung und den Spesenersatz für die Führung einer Beistandschaft (BSG 213.361) | 3 | as enacted, then each consolidated version: 1 January 2013 to 1 January 2022 |
| `214-431-1/` | Verordnung über die Errichtung des Inventars (BSG 214.431.1) | 1 | one version (the oldest available), 1 January 2013 |
| `215-129-1-schatzungsverordnung-schv/` | Verordnung über die amtliche und ausseramtliche Schätzung von Grundstücken (BSG 215.129.1) | 2 | oldest version available, then each consolidated version: 1 January 2012 to 1 December 2015 |
| `215-231/` | Verordnung betreffend die Viehverpfändung (BSG 215.231) | 1 | one version (the oldest available), 1 January 2010 |
| `215-321-2/` | Verordnung betreffend das kantonale Grundbuch und die Einführung des schweizerischen Grundbuches (BSG 215.321.2) | 3 | oldest version available, then each consolidated version: 1 January 2010 to 1 January 2023 |
| `215-321-3-edvgb-dv/` | Direktionsverordnung über die Führung des Grundbuches mit elektronischer Datenverarbeitung (BSG 215.321.3) | 1 | one version (the oldest available), 1 January 2010 |
| `215-321-5-grudis-verordnung/` | Verordnung über das Grundstückdateninformationssystem (BSG 215.321.5) | 5 | oldest version available, then each consolidated version: 1 January 2014 to 1 September 2026 |
| `215-321-6-egvv/` | Verordnung über den elektronischen Geschäftsverkehr mit den Grundbuchämtern und dem Handelsregisteramt (BSG 215.321.6) | 2 | as enacted, then each consolidated version: 1 January 2014 to 1 November 2020 |
| `215-331-seyv/` | Verordnung über das Seybuch (BSG 215.331) | 2 | oldest version available, then each consolidated version: 1 November 2010 to 1 January 2023 |
| `215-341-1-kvav/` | Kantonale Verordnung über die amtliche Vermessung (BSG 215.341.1) | 5 | oldest version available, then each consolidated version: 1 January 2013 to 1 January 2026 |
| `215-341-2-kgeoiv/` | Kantonale Geoinformationsverordnung (BSG 215.341.2) | 6 | oldest version available, then each consolidated version: 1 January 2015 to 1 September 2026 |
| `215-341-3-nkv/` | Verordnung über die Nomenklaturkommission (BSG 215.341.3) | 3 | as enacted, then each consolidated version: 1 January 2011 to 1 January 2022 |
| `215-341-4-ev-orebkv/` | Einführungsverordnung zur eidgenössischen Verordnung über den Kataster der öffentlich-rechtlichen Eigentumsbeschränkungen (BSG 215.341.4) | 6 | as enacted, then each consolidated version: 1 January 2014 to 1 November 2025 |
| `215-341-5-vlk/` | Verordnung über den Leitungskataster (BSG 215.341.5) | 1 | as enacted, 1 January 2016 |
| `222-100-exmv/` | Exmissionsverordnung (BSG 222.100) | 3 | as enacted, then each consolidated version: 1 January 2019 to 1 September 2026 |
| `222-153-11/` | Verordnung über die Allgemeinverbindlicherklärung von Gesamtarbeitsverträgen (BSG 222.153.11) | 2 | as enacted, then each consolidated version: 1 January 2004 to 1 April 2021 |
| `271-111-zfitv/` | Verordnung über das Pilotprojekt «Angeordnete Beratung in familienrechtlichen Gerichtsverfahren mit strittigen Kinderbelangen und Zentrum für Familien in Trennung (ZFIT)» (BSG 271.111) | 2 | as enacted, then each consolidated version: 1 September 2023 to 1 September 2025 |
| `282-222-auv/` | Verordnung über die Ausbildung der Betreibungs- und Konkursbeamtinnen sowie Betreibungs- und Konkursbeamten (BSG 282.222) | 2 | oldest version available, then each consolidated version: 1 January 2012 to 1 November 2020 |
| `282-321-eev/` | Verordnung über die Ernennung und Entschädigung der nebenamtlichen Betreibungsweibelinnen und -weibel (BSG 282.321) | 1 | one version (the oldest available), 1 January 2010 |
| `284-11/` | Vollziehungsverordnung zum Bundesgesetz vom 4. Dezember 1947 über die Schuldbetreibung gegen Gemeinden und andere Körperschaften des kantonalen öffentlichen Rechts (BSG 284.11) | 1 | as enacted, 1 January 1949 |
| `321-211-datenvernichtungsverordnung-pdvv/` | Verordnung über die Ausnahmen von der Pflicht zur Vernichtung polizeilicher Daten (BSG 321.211) | 2 | oldest version available, then each consolidated version: 1 January 2011 to 1 March 2023 |
| `324-111-kobv/` | Kantonale Ordnungsbussenverordnung (BSG 324.111) | 6 | oldest version available, then each consolidated version: 1 February 2014 to 1 March 2023 |
| `326-111-kohv/` | Kantonale Opferhilfeverordnung (BSG 326.111) | 4 | oldest version available, then each consolidated version: 1 January 2011 to 1 March 2021 |
| `341-11-justizvollzugsverordnung-jvv/` | Verordnung über den Justizvollzug (BSG 341.11) | 8 | oldest version available, then each consolidated version: 1 January 2013 to 1 January 2026 |
| `341-12-vemv/` | Verordnung über den Vollzug von Electronic Monitoring (BSG 341.12) | 4 | oldest version available, then each consolidated version: 1 January 2011 to 1 September 2026 |
| `410-111-lkv/` | Verordnung über die bernischen Landeskirchen (BSG 410.111) | 5 | oldest version available, then each consolidated version: 1 January 2020 to 1 January 2026 |
| `412-111-epzv/` | Verordnung über die Zuordnung der vom Kanton besoldeten evangelisch-reformierten Pfarrstellen (BSG 412.111) | 1 | as enacted, 1 April 2015 |
| `412-112-rpzv/` | Verordnung über die Zuordnung der vom Kanton besoldeten römisch-katholischen Pfarrstellen (BSG 412.112) | 1 | as enacted, 1 April 2015 |
| `414-54-fgjgv/` | Verordnung über die Finanzierung der Geistlichen der jüdischen Gemeinden (BSG 414.54) | 3 | as enacted, then each consolidated version: 1 September 1997 to 1 November 2020 |
| `414-110-tppkv/` | Verordnung über die theologischen Prüfungen und die Prüfungskommissionen (BSG 414.110) | 2 | as enacted, then each consolidated version: 1 January 2020 to 1 November 2020 |
| `414-111/` | Verordnung über die Weiterbildung und den Studienurlaub für Pfarrerinnen und Pfarrer der Landeskirchen (BSG 414.111) | 2 | as enacted, then each consolidated version: 1 January 2006 to 1 November 2020 |
| `414-311-aphv/` | Verordnung über das Arbeitsverhältnis der Inhaberinnen und Inhaber von Pfarr- und Hilfspfarrstellen (BSG 414.311) | 2 | oldest version available, then each consolidated version: 1 February 2014 to 1 November 2020 |
| `414-522-stellvertretungsentschadigungsverordnung-stev/` | Verordnung über die Entschädigungen für pfarramtliche Funktionen bei Stellvertretungen (BSG 414.522) | 1 | one version (the oldest available), 1 July 2013 |
| `423-411-1-kkfv/` | Kantonale Kulturförderungsverordnung (BSG 423.411.1) | 15 | oldest version available, then each consolidated version: 1 November 2015 to 1 August 2026 |
| `423-411-11-jtmv/` | Verordnung über den Vollzug des eidgenössischen Förderungskonzepts zum Programm «Junge Talente Musik» (BSG 423.411.11) | 1 | as enacted, 1 November 2023 |
| `426-111-nschv/` | Naturschutzverordnung (BSG 426.111) | 6 | oldest version available, then each consolidated version: 1 July 2012 to 1 January 2023 |
| `426-112-ftv/` | Verordnung über Beiträge an Trockenstandorte und Feuchtgebiete (BSG 426.112) | 2 | oldest version available, then each consolidated version: 1 January 2014 to 1 January 2018 |
| `426-221-olkv/` | Verordnung über die Kommission zur Pflege der Orts- und Landschaftsbilder (BSG 426.221) | 4 | as enacted, then each consolidated version: 1 January 2011 to 1 April 2023 |
| `426-411-denkmalpflegeverordnung-dpv/` | Verordnung über die Denkmalpflege (BSG 426.411) | 7 | oldest version available, then each consolidated version: 1 January 2009 to 1 August 2026 |
| `430-41-sdv/` | Verordnung über den schulärztlichen Dienst (BSG 430.41) | 4 | oldest version available, then each consolidated version: 1 January 2014 to 1 August 2026 |
| `430-210-141-1-hep-bejune/` | Règlements de la Haute École Pédagogique Berne, Jura, Neuchâtel (BSG 430.210.141.1) | 1 | as enacted, 1 November 2015 |
| `430-251-0-lav/` | Verordnung über die Anstellung der Lehrkräfte (BSG 430.251.0) | 15 | oldest version available, then each consolidated version: 1 August 2015 to 1 September 2026 |
| `430-251-1-ladv/` | Direktionsverordnung über die Anstellung der Lehrkräfte (BSG 430.251.1) | 5 | oldest version available, then each consolidated version: 1 August 2015 to 1 January 2023 |
| `430-261-11/` | Reglemente der Bernischen Lehrerversicherungskasse (BLVK) (BSG 430.261.11) | 1 | as enacted, 1 December 2015 |
| `431-51-ebav/` | Verordnung über die Ausbildung und die Diplomierung in Erziehungsberatung-Schulpsychologie (BSG 431.51) | 3 | as enacted, then each consolidated version: 1 August 2003 to 1 April 2024 |
| `431-511/` | Prüfungsreglement für den Erwerb des Diploms in Erziehungsberatung-Schulpsychologie (BSG 431.511) | 1 | as enacted, 1 July 2007 |
| `432-211-1-vsv/` | Volksschulverordnung (BSG 432.211.1) | 9 | as enacted, then each consolidated version: 1 August 2013 to 1 August 2026 |
| `432-211-2-tsv/` | Tagesschulverordnung (BSG 432.211.2) | 15 | oldest version available, then each consolidated version: 1 August 2014 to 1 August 2026 |
| `432-211-10-vsdv/` | Volksschuldirektionsverordnung (BSG 432.211.10) | 2 | as enacted, then each consolidated version: 1 August 2022 to 1 August 2024 |
| `432-213-11-dvbs/` | Direktionsverordnung über die Beurteilung und Schullaufbahnentscheide in der Volksschule (BSG 432.213.11) | 5 | as enacted, then each consolidated version: 1 August 2013 to 1 August 2022 |
| `432-213-12-dvad/` | Direktionsverordnung über Absenzen und Dispensationen in der Volksschule (BSG 432.213.12) | 3 | oldest version available, then each consolidated version: 1 August 2008 to 1 August 2022 |
| `432-213-15-od-per/` | Ordonnance de Direction concernant le Plan d'études romand et les dispositions générales complétant le Plan d'études romand (BSG 432.213.15) | 4 | oldest version available, then each consolidated version: 1 August 2013 to 1 August 2023 |
| `432-213-16-dvlp-21/` | Direktionsverordnung über den Lehrplan 21 des Kantons Bern (BSG 432.213.16) | 3 | as enacted, then each consolidated version: 1 August 2018 to 1 August 2026 |
| `432-271-1-vmr/` | Verordnung über die einfachen sonderpädagogischen und unterstützenden Massnahmen im Regelschulangebot (BSG 432.271.1) | 6 | oldest version available, then each consolidated version: 1 August 2013 to 1 August 2025 |
| `432-271-11-mrdv/` | Direktionsverordnung über die einfachen sonderpädagogischen und unterstützenden Massnahmen im Regelschulangebot (BSG 432.271.11) | 4 | as enacted, then each consolidated version: 1 August 2009 to 1 August 2024 |
| `432-282-bvsv/` | Verordnung über das besondere Volksschulangebot (BSG 432.282) | 3 | as enacted, then each consolidated version: 1 January 2022 to 1 September 2022 |
| `432-282-1-bvsdv/` | Direktionsverordnung über das besondere Volksschulangebot (BSG 432.282.1) | 2 | as enacted, then each consolidated version: 1 January 2022 to 1 January 2026 |
| `432-282-2-dvlp-21-bvsa/` | Direktionsverordnung über den Lehrplan 21 des Kantons Bern für das besondere Volksschulangebot (BSG 432.282.2) | 1 | as enacted, 1 August 2022 |
| `432-282-3-od-pe-oseo/` | Ordonnance de Direction concernant le Plan d'études du canton de Berne sur l'offre spécialisée de l'école obligatoire (BSG 432.282.3) | 1 | as enacted, 1 August 2022 |
| `432-311-msv/` | Musikschulverordnung (BSG 432.311) | 2 | as enacted, then each consolidated version: 1 January 2012 to 1 August 2020 |
| `433-121-misv/` | Mittelschulverordnung (BSG 433.121) | 9 | oldest version available, then each consolidated version: 1 August 2015 to 1 September 2026 |
| `433-121-1-misdv/` | Mittelschuldirektionsverordnung (BSG 433.121.1) | 12 | oldest version available, then each consolidated version: 1 August 2015 to 1 August 2024 |
| `433-121-2/` | Direktionsverordnung über den Lehrplan 17 für den gymnasialen Bildungsgang (BSG 433.121.2) | 2 | as enacted, then each consolidated version: 1 August 2017 to 1 August 2019 |
| `433-121-3/` | Direktionsverordnung über den Lehrplan für den zweisprachigen gymnasialen Bildungsgang Deutsch-Französisch der Gymnasien der Regionen Biel-Seeland und Bienne-Jura bernois (BSG 433.121.3) | 2 | as enacted, then each consolidated version: 1 August 2017 to 1 August 2020 |
| `433-121-6/` | Ordonnance de Direktion concernant le plan d'études cantonal francophone pour la formation gymnasiale (BSG 433.121.6) | 1 | as enacted, 1 August 2020 |
| `433-121-41/` | Direktionsverordnung über den Lehrplan 2021 für die Fachmittelschulbildungsgänge (BSG 433.121.41) | 2 | as enacted, then each consolidated version: 1 August 2021 to 1 August 2024 |
| `433-121-42/` | Ordonnance de Direction concernant le plan d'études francophone 2021 pour la formation en école de culture générale (BSG 433.121.42) | 2 | as enacted, then each consolidated version: 1 August 2021 to 1 August 2024 |
| `435-111-berv/` | Verordnung über die Berufsbildung, die Weiterbildung und die Berufsberatung (BSG 435.111) | 13 | oldest version available, then each consolidated version: 1 August 2015 to 1 August 2025 |
| `435-111-1-berdv/` | Direktionsverordnung über die Berufsbildung, die Weiterbildung und die Berufsberatung (BSG 435.111.1) | 19 | oldest version available, then each consolidated version: 1 July 2015 to 1 August 2026 |
| `435-111-2/` | Direktionsverordnung über den Lehrplan Berufsvorbereitendes Schuljahr (BSG 435.111.2) | 3 | as enacted, then each consolidated version: 1 January 2016 to 1 August 2019 |
| `435-111-4/` | Direktionsverordnung über den Lehrplan Berufsmaturität Technik, Architektur, Life Sciences (BSG 435.111.4) | 2 | as enacted, then each consolidated version: 1 January 2018 to 1 August 2026 |
| `435-111-5/` | Direktionsverordnung über den Lehrplan Berufsmaturität Natur, Landschaft und Lebensmittel (BSG 435.111.5) | 2 | as enacted, then each consolidated version: 1 January 2018 to 1 August 2026 |
| `435-111-6/` | Direktionsverordnung über den Lehrplan Berufsmaturität Wirtschaft und Dienstleistungen, Typ Wirtschaft (BSG 435.111.6) | 2 | as enacted, then each consolidated version: 1 January 2018 to 1 August 2026 |
| `435-111-7/` | Direktionsverordnung über den Lehrplan Berufsmaturität Wirtschaft und Dienstleistungen, Typ Dienstleistungen (BSG 435.111.7) | 2 | as enacted, then each consolidated version: 1 January 2018 to 1 August 2026 |
| `435-111-8/` | Direktionsverordnung über den Lehrplan Berufsmaturität Gestaltung und Kunst (BSG 435.111.8) | 2 | as enacted, then each consolidated version: 1 January 2018 to 1 August 2026 |
| `435-111-9/` | Direktionsverordnung über den Lehrplan Berufsmaturität Gesundheit und Soziales, Variante Gesundheit (BSG 435.111.9) | 2 | as enacted, then each consolidated version: 1 January 2018 to 1 August 2026 |
| `435-111-10/` | Direktionsverordnung über den Lehrplan Berufsmaturität Gesundheit und Soziales, Variante Soziale Arbeit (BSG 435.111.10) | 2 | as enacted, then each consolidated version: 1 January 2018 to 1 August 2026 |
| `435-111-11/` | Direktionsverordnung über den Lehrplan Allgemeinbildung in der beruflichen Grundbildung (BSG 435.111.11) | 1 | as enacted, 1 August 2026 |
| `435-111-20/` | Direktionsverordnung über den Lehrplan Vorlehre 22 (BSG 435.111.20) | 2 | as enacted, then each consolidated version: 1 August 2018 to 1 August 2022 |
| `435-112-1/` | Ordonnance de Direction concernant le plan d’études cantonal pour l’enseignement de culture générale dans la formation professionnelle initiale (BSG 435.112.1) | 1 | as enacted, 1 August 2026 |
| `435-112-2/` | Ordonnance de Direction sur le plan d'études pour la maturité professionnelle Technique, architecture et sciences de la vie (BSG 435.112.2) | 1 | as enacted, 1 August 2026 |
| `435-112-3/` | Ordonnance de Direction sur le plan d'études pour la maturité professionnelle Économie et services, type économie (BSG 435.112.3) | 1 | as enacted, 1 August 2026 |
| `435-112-4/` | Ordonnance de Direction sur le plan d'études pour la maturité professionnelle Économie et services, type services (BSG 435.112.4) | 1 | as enacted, 1 August 2026 |
| `435-112-5/` | Ordonnance de Direction sur le plan d’études pour la maturité professionnelle Arts visuels et arts appliqués (BSG 435.112.5) | 1 | as enacted, 1 August 2026 |
| `435-112-6/` | Ordonnance de Direction sur le plan d'études pour la maturité professionnelle Santé et social, type santé (BSG 435.112.6) | 1 | as enacted, 1 August 2026 |
| `435-112-7/` | Ordonnance de Direction sur le plan d'études pour la maturité professionnelle Santé et social, type travail social (BSG 435.112.7) | 1 | as enacted, 1 August 2026 |
| `436-111-1-univ/` | Verordnung über die Universität (BSG 436.111.1) | 11 | oldest version available, then each consolidated version: 1 May 2015 to 1 January 2026 |
| `436-111-3-gebdv-phab/` | Direktionsverordnung über die Gebühren für die Promotion und die Habilitation an der Universität Bern (BSG 436.111.3) | 1 | as enacted, 1 February 2011 |
| `436-111-4-uldv/` | Direktionsverordnung über das Verfahren zur Wahl oder Anstellung der Mitglieder der Universitätsleitung (BSG 436.111.4) | 2 | as enacted, then each consolidated version: 1 June 2013 to 1 November 2021 |
| `436-111-5/` | Reglemente der Universität (BSG 436.111.5) | 1 | as enacted, 1 January 2019 |
| `436-723/` | Verordnung über die kirchlich-theologischen Maturitätsprüfungen des Kantons Bern (BSG 436.723) | 2 | oldest version available, then each consolidated version: 1 April 1995 to 1 July 2020 |
| `436-811-fachhochschulverordnung-fav/` | Verordnung über die Berner Fachhochschule (BSG 436.811) | 7 | oldest version available, then each consolidated version: 1 January 2016 to 1 January 2026 |
| `436-811-1-bfh/` | Reglemente der Berner Fachhochschule (BSG 436.811.1) | 1 | as enacted, 1 November 2015 |
| `436-812-1-he-arc/` | Règlements de la Haute École Arc Berne-Jura-Neuchâtel (BSG 436.812.1) | 1 | as enacted, 1 November 2015 |
| `436-911-phv/` | Verordnung über die deutschsprachige Pädagogische Hochschule (BSG 436.911) | 9 | oldest version available, then each consolidated version: 1 August 2015 to 1 January 2026 |
| `436-911-0-phbern/` | Reglemente der deutschsprachigen Pädagogischen Hochschule (BSG 436.911.0) | 1 | as enacted, 1 November 2015 |
| `437-111-kspofov/` | Kantonale Sportförderungsverordnung (BSG 437.111) | 1 | as enacted, 1 August 2022 |
| `438-312-abv/` | Verordnung über die Ausbildungsbeiträge (BSG 438.312) | 5 | oldest version available, then each consolidated version: 1 January 2013 to 1 August 2024 |
| `439-182-5-gdk/` | Gebührenverordnung der Schweizerischen Konferenz der kantonalen Gesundheitsdirektorinnen und -direktoren (BSG 439.182.5) | 1 | one version (the oldest available), 22 November 2012 |
| `439-182-6/` | Reglement der Schweizerischen Konferenz der kantonalen Gesundheitsdirektorinnen und -direktoren (GDK) für die interkantonale Prüfung von Osteopathinnen und Osteopathen in der Schweiz (BSG 439.182.6) | 2 | oldest version available, then each consolidated version: 22 November 2012 to 25 May 2018 |
| `439-182-7/` | Reglement der Schweizerischen Konferenz der kantonalen Gesundheitsdirektorinnen und -direktoren (GDK) über die Gebühren für die interkantonale Prüfung der Osteopathinnen und Osteopathen (BSG 439.182.7) | 1 | one version (the oldest available), 10 April 2014 |
| `439-182-61-verordnung-ausland-vo-ausland/` | Verordnung der Schweizerischen Konferenz der kantonalen Gesundheitsdirektorinnen und –direktoren (GDK) über die Anerkennung und Nachprüfung von ausländischen Berufsqualifikationen in Osteopathie (BSG 439.182.61) | 1 | as enacted, 1 May 2013 |
| `439-322-hes-so/` | Règlements de la Haute Ecole Spécialisée de Suisse occidentale (BSG 439.322) | 1 | as enacted, 1 November 2015 |
| `515-811/` | Reglement über die Organisation und Verwaltung der «Laupenstiftung» (BSG 515.811) | 2 | oldest version available, then each consolidated version: 1 January 1993 to 1 April 2021 |
| `521-10-kbsv/` | Kantonale Bevölkerungsschutzverordnung (BSG 521.10) | 6 | as enacted, then each consolidated version: 1 January 2015 to 1 January 2026 |
| `521-12-ebdv/` | Direktionsverordnung über den Ersatzbeitragsfonds des Kantons Bern (BSG 521.12) | 2 | as enacted, then each consolidated version: 1 January 2016 to 1 January 2021 |
| `521-14-einsatzkostenversicherungsverordnung-ekvv/` | Verordnung über die Einsatzkostenversicherung der Einwohnergemeinden bei Katastrophen und in Notlagen (BSG 521.14) | 2 | oldest version available, then each consolidated version: 1 January 2010 to 1 January 2026 |
| `522-10-kzsv/` | Kantonale Zivilschutzverordnung (BSG 522.10) | 1 | as enacted, 1 January 2026 |
| `525-31/` | Verordnung über die Sportschiessanlagen (BSG 525.31) | 3 | as enacted, then each consolidated version: 1 January 2007 to 1 January 2022 |
| `551-111-polv/` | Polizeiverordnung (BSG 551.111) | 5 | oldest version available, then each consolidated version: 1 January 2011 to 1 August 2024 |
| `551-212/` | Einführungsverordnung zum Konkordat über Massnahmen gegen Gewalt anlässlich von Sportveranstaltungen (BSG 551.212) | 1 | one version (the oldest available), 12 March 2014 |
| `551-213-smsv/` | Kantonale Verordnung über Massnahmen zur Unterstützung der Sicherheit von Minderheiten mit besonderen Schutzbedürfnissen (BSG 551.213) | 2 | as enacted, then each consolidated version: 1 June 2020 to 1 January 2023 |
| `551-331/` | Verordnung über den polizeilichen Erkennungsdienst (BSG 551.331) | 2 | oldest version available, then each consolidated version: 1 January 1998 to 1 April 2021 |
| `551-411-sdpv/` | Verordnung über das Erbringen von Sicherheitsdienstleistungen durch Private (BSG 551.411) | 1 | as enacted, 1 January 2020 |
| `621-1-fhav/` | Finanzhaushaltsverordnung (BSG 621.1) | 7 | oldest version available, then each consolidated version: 1 January 2015 to 1 January 2023 |
| `621-5-statistikverordnung-statv/` | Verordnung über die Statistik (BSG 621.5) | 2 | oldest version available, then each consolidated version: 1 January 2009 to 1 March 2023 |
| `621-11/` | Verordnung über die Besondere Rechnung des Regierungsrates (BSG 621.11) | 3 | as enacted, then each consolidated version: 1 January 2005 to 1 January 2023 |
| `631-111-filav/` | Verordnung über den Finanz- und Lastenausgleich (BSG 631.111) | 7 | oldest version available, then each consolidated version: 1 January 2015 to 1 January 2025 |
| `641-111-stbv/` | Staatsbeitragsverordnung (BSG 641.111) | 3 | oldest version available, then each consolidated version: 1 January 2005 to 1 January 2019 |
| `661-113-dstv/` | Verordnung über die Vergütung von Dienstleistungen im Steuerverfahren (BSG 661.113) | 3 | oldest version available, then each consolidated version: 1 July 2011 to 1 January 2020 |
| `661-261-sbv/` | Verordnung über die Steuerbefreiung juristischer Personen (BSG 661.261) | 1 | one version (the oldest available), 1 January 2012 |
| `661-312-21-vba/` | Verordnung über die Besteuerung nach dem Aufwand (BSG 661.312.21) | 3 | as enacted, then each consolidated version: 1 January 2001 to 1 January 2021 |
| `661-312-51-vubv/` | Verordnung über die Unterhalts-, Betriebs- und Verwaltungskosten von Grundstücken (BSG 661.312.51) | 3 | oldest version available, then each consolidated version: 1 January 2010 to 1 January 2024 |
| `661-312-56-berufskostenverordnung-bkv/` | Verordnung über die Berufskosten (BSG 661.312.56) | 4 | oldest version available, then each consolidated version: 1 January 2014 to 1 January 2024 |
| `661-312-57-vv/` | Verordnung über den Verlustvortrag bei geschäftlichen Betrieben (BSG 661.312.57) | 2 | as enacted, then each consolidated version: 1 January 2001 to 1 January 2020 |
| `661-312-59-abv/` | Abschreibungsverordnung (BSG 661.312.59) | 1 | one version (the oldest available), 1 January 2011 |
| `661-312-60-nbv/` | Verordnung über die Nachbesteuerung von ertragsbesteuertem Bauland (BSG 661.312.60) | 1 | as enacted, 1 January 2001 |
| `661-521-1-vvv/` | Verordnung über das Veranlagungsverfahren (BSG 661.521.1) | 3 | oldest version available, then each consolidated version: 1 January 2008 to 1 January 2019 |
| `661-543-1-newab-vv/` | Versuchsverordnung über das neue amtliche Bewertungssystem NewAB (BSG 661.543.1) | 1 | as enacted, 1 May 2025 |
| `661-711-1-qsv/` | Quellensteuerverordnung (BSG 661.711.1) | 4 | oldest version available, then each consolidated version: 1 January 2015 to 1 January 2021 |
| `661-733-bezugsverordnung-bezv/` | Verordnung über den Bezug und die Verzinsung von Abgaben und anderen zum Inkasso übertragenen Forderungen, über Zahlungserleichterungen, Erlass sowie Abschreibungen infolge Uneinbringlichkeit (BSG 661.733) | 7 | oldest version available, then each consolidated version: 1 January 2013 to 1 January 2026 |
| `668-11-bstv/` | Verordnung über den Vollzug der direkten Bundessteuer (BSG 668.11) | 1 | one version (the oldest available), 1 January 2008 |
| `668-21-vrv/` | Verordnung über die Rückerstattung der Verrechnungssteuer (BSG 668.21) | 1 | as enacted, 1 January 2001 |
| `668-31-ev-oecd-zwei-saulen-modell/` | Einführungsverordnung zur Besteuerung der digitalen Wirtschaft im OECD-Zwei-Säulen-Modell (BSG 668.31) | 1 | as enacted, 1 January 2024 |
| `668-61-bwpev/` | Verordnung betreffend den Vollzug des Bundesgesetzes über die Wehrpflichtersatzabgabe (BSG 668.61) | 2 | oldest version available, then each consolidated version: 1 May 2012 to 1 January 2019 |
| `669-721-qstav/` | Verordnung über die Anrechnung ausländischer Quellensteuern (BSG 669.721) | 2 | as enacted, then each consolidated version: 1 January 2001 to 1 April 2021 |
| `669-791-vrv-usa/` | Verordnung über die Rückerstattung des zusätzlichen Steuerrückbehalts der Vereinigten Staaten von Amerika (BSG 669.791) | 1 | as enacted, 1 January 2001 |
| `669-811-1-grenzgangerverordnung-bgv/` | Verordnung betreffend die schweizerisch-französische Vereinbarung über die Besteuerung der Erwerbseinkünfte von Grenzgängerinnen und Grenzgängern (BSG 669.811.1) | 1 | one version (the oldest available), 1 July 2011 |
| `702-1-ev-rpg2/` | Einführungsverordnung zur Umsetzung der zweiten Etappe der Änderung des Raumplanungsgesetzes (BSG 702.1) | 1 | as enacted, 1 July 2026 |
| `706-111-pfv/` | Planungsfinanzierungsverordnung (BSG 706.111) | 3 | oldest version available, then each consolidated version: 1 January 2014 to 1 February 2020 |
| `711-1-entv/` | Verordnung über die Enteignung (BSG 711.1) | 3 | oldest version available, then each consolidated version: 1 January 2010 to 1 February 2025 |
| `712-1/` | Vollziehungsverordnung zum Bundesgesetz vom 20. Juni 1930 über die Enteignung (BSG 712.1) | 1 | one version (the oldest available), 1 January 2011 |
| `721-1-bauv/` | Bauverordnung (BSG 721.1) | 12 | oldest version available, then each consolidated version: 1 January 2015 to 1 May 2024 |
| `721-3-bmbv/` | Verordnung über die Begriffe und Messweisen im Bauwesen (BSG 721.3) | 4 | oldest version available, then each consolidated version: 1 January 2012 to 1 January 2024 |
| `721-4-smwav/` | Verordnung über die Spezialfinanzierung Mehrwertabgabe (BSG 721.4) | 2 | as enacted, then each consolidated version: 1 April 2020 to 1 July 2026 |
| `731-21-ivobv/` | Verordnung zur Interkantonalen Vereinbarung über das öffentliche Beschaffungswesen (BSG 731.21) | 7 | oldest version available, then each consolidated version: 1 January 2015 to 1 September 2024 |
| `731-22-oobv/` | Verordnung über die Organisation des öffentlichen Beschaffungswesens (BSG 731.22) | 7 | as enacted, then each consolidated version: 1 January 2015 to 1 July 2025 |
| `732-111-1-sv/` | Strassenverordnung (BSG 732.111.1) | 5 | oldest version available, then each consolidated version: 1 January 2011 to 1 October 2026 |
| `741-11-ev-photovoltaik-grossanlagen/` | Einführungsverordnung zum eidgenössischen Energiegesetz und zur eidgenössischen Energieverordnung betreffend Photovoltaik-Grossanlagen (BSG 741.11) | 1 | as enacted, 1 June 2023 |
| `741-111-kenv/` | Kantonale Energieverordnung (BSG 741.111) | 6 | as enacted, then each consolidated version: 1 January 2012 to 1 January 2026 |
| `751-111-1-wbv/` | Wasserbauverordnung (BSG 751.111.1) | 4 | oldest version available, then each consolidated version: 1 January 2015 to 1 January 2025 |
| `752-321-1-wvv/` | Wasserversorgungsverordnung (BSG 752.321.1) | 2 | oldest version available, then each consolidated version: 1 January 2009 to 1 January 2020 |
| `752-467-vwo/` | Verordnung über die Wasserentnahmen aus Oberflächengewässern (BSG 752.467) | 2 | oldest version available, then each consolidated version: 1 January 2010 to 1 August 2020 |
| `761-111-strvv/` | Strassenverkehrsverordnung (BSG 761.111) | 6 | oldest version available, then each consolidated version: 1 January 2012 to 1 March 2023 |
| `761-611-1-bsfv/` | Verordnung über die Besteuerung der Strassenfahrzeuge und den Bezug von Forderungen durch das Strassenverkehrs- und Schifffahrtsamt (BSG 761.611.1) | 4 | oldest version available, then each consolidated version: 28 October 2013 to 1 September 2026 |
| `761-612-1-bpv/` | Verordnung über die Bewirtschaftung der Parkplätze des Kantons (BSG 761.612.1) | 1 | one version (the oldest available), 1 January 2005 |
| `762-412-angebotsverordnung-agv/` | Verordnung über das Angebot im öffentlichen Verkehr (BSG 762.412) | 3 | oldest version available, then each consolidated version: 1 January 2015 to 1 February 2022 |
| `762-413-rvkv/` | Verordnung über die regionalen Verkehrskonferenzen (BSG 762.413) | 11 | oldest version available, then each consolidated version: 1 January 2015 to 1 January 2026 |
| `762-415-kbv/` | Verordnung über die Beiträge der Gemeinden an die Kosten des öffentlichen Verkehrs (BSG 762.415) | 3 | oldest version available, then each consolidated version: 1 January 2015 to 1 December 2023 |
| `764-2-ptv/` | Personentransportverordnung (BSG 764.2) | 1 | one version (the oldest available), 1 January 2015 |
| `766-11-krlv/` | Kantonale Rohrleitungsverordnung (BSG 766.11) | 2 | as enacted, then each consolidated version: 1 January 2013 to 1 August 2020 |
| `767-21-vabs/` | Verordnung über die Ausnahmen in der Besteuerung der Schiffe (BSG 767.21) | 2 | as enacted, then each consolidated version: 1 January 1991 to 1 April 2021 |
| `767-22-slpv/` | Schiffsliegeplatzverordnung (BSG 767.22) | 1 | as enacted, 1 September 2013 |
| `767-25-agsgv/` | Verordnung über die Erhebung von Abgaben bei gesteigertem Gemeingebrauch oder Sondernutzung von öffentlichen Gewässern (BSG 767.25) | 2 | oldest version available, then each consolidated version: 1 January 2015 to 1 August 2020 |
| `767-31-vbs/` | Verordnung über die Ausrichtung von Beiträgen in der Schifffahrt (BSG 767.31) | 2 | oldest version available, then each consolidated version: 1 January 1993 to 1 April 2021 |
| `767-32-srdv/` | Seerettungsdienstverordnung (BSG 767.32) | 1 | as enacted, 1 January 2021 |
| `767-111-smrpv/` | Verordnung über die Schiffsmelde- und -reinigungspflicht (BSG 767.111) | 1 | as enacted, 1 January 2025 |
| `768-1-klfv/` | Kantonale Luftfahrtverordnung (BSG 768.1) | 3 | oldest version available, then each consolidated version: 1 January 2015 to 1 June 2022 |
| `811-05-kekv/` | Verordnung über die Kantonale Ethikkommission für die Forschung (BSG 811.05) | 4 | as enacted, then each consolidated version: 1 September 2014 to 1 August 2021 |
| `811-011-patientenrechtsverordnung-patv/` | Verordnung über die Rechte und Pflichten der Patientinnen und Patienten und der Gesundheitsfachpersonen (BSG 811.011) | 4 | oldest version available, then each consolidated version: 1 January 2013 to 1 January 2023 |
| `811-111-gesundheitsverordnung-gesv/` | Verordnung über die beruflichen Tätigkeiten im Gesundheitswesen (BSG 811.111) | 8 | oldest version available, then each consolidated version: 1 January 2011 to 1 January 2026 |
| `811-511-schpv/` | Verordnung zum Schutz vor Passivrauchen (BSG 811.511) | 1 | as enacted, 1 July 2009 |
| `811-811-bestattungsverordnung-bestv/` | Verordnung über das Bestattungswesen (BSG 811.811) | 2 | as enacted, then each consolidated version: 1 January 2011 to 1 August 2021 |
| `811-941-etv/` | Verordnung über die Entschädigungsansätze für amtliche Verrichtungen im Rahmen der Tierseuchenbekämpfung (BSG 811.941) | 2 | as enacted, then each consolidated version: 1 January 2013 to 1 January 2021 |
| `812-112-spvv/` | Spitalversorgungsverordnung (BSG 812.112) | 11 | oldest version available, then each consolidated version: 1 January 2014 to 1 July 2025 |
| `812-113-spvdv/` | Direktionsverordnung über die Spitalversorgung (BSG 812.113) | 3 | as enacted, then each consolidated version: 1 January 2022 to 1 January 2026 |
| `813-131-ev-betmg/` | Einführungsverordnung zur eidgenössischen Betäubungsmittelgesetzgebung (BSG 813.131) | 2 | as enacted, then each consolidated version: 1 September 2012 to 1 August 2021 |
| `813-151-ev-chemg/` | Einführungsverordnung zur eidgenössischen Chemikaliengesetzgebung (BSG 813.151) | 3 | oldest version available, then each consolidated version: 1 January 2009 to 1 April 2021 |
| `815-122-ev-epg/` | Einführungsverordnung zur eidgenössischen Epidemiengesetzgebung (BSG 815.122) | 6 | oldest version available, then each consolidated version: 1 January 2013 to 1 January 2026 |
| `815-210-ev-krg/` | Einführungsverordnung zur eidgenössischen Krebsregistrierungsgesetzgebung (BSG 815.210) | 2 | as enacted, then each consolidated version: 1 January 2020 to 1 August 2021 |
| `817-191-flkv/` | Fleischkontrollverordnung (BSG 817.191) | 5 | oldest version available, then each consolidated version: 1 January 2014 to 1 November 2025 |
| `820-111-kuvpv/` | Verordnung über die Umweltverträglichkeitsprüfung (BSG 820.111) | 6 | oldest version available, then each consolidated version: 1 November 2010 to 1 January 2023 |
| `820-131-ev-stfv/` | Einführungsverordnung zur eidgenössischen Störfallverordnung (BSG 820.131) | 4 | oldest version available, then each consolidated version: 1 July 2015 to 1 August 2021 |
| `821-1-kgv/` | Kantonale Gewässerschutzverordnung (BSG 821.1) | 3 | oldest version available, then each consolidated version: 1 January 2009 to 1 January 2020 |
| `821-2-olwehrverordnung/` | Verordnung über die Gewässerschutzmassnahmen bei Verlust von Mineralöl und andern gefährlichen Flüssigkeiten (BSG 821.2) | 3 | oldest version available, then each consolidated version: 1 January 2009 to 1 January 2026 |
| `822-111-abfv/` | Abfallverordnung (BSG 822.111) | 3 | oldest version available, then each consolidated version: 1 January 2009 to 1 August 2020 |
| `823-111-lufthygieneverordnung-lhv/` | Verordnung zur Reinhaltung der Luft (BSG 823.111) | 4 | oldest version available, then each consolidated version: 1 January 2015 to 1 January 2026 |
| `824-761-klsv/` | Kantonale Lärmschutzverordnung (BSG 824.761) | 4 | oldest version available, then each consolidated version: 1 January 2015 to 1 January 2025 |
| `832-011-ev-arg/` | Einführungsverordnung zur eidgenössischen Arbeitsgesetzgebung (BSG 832.011) | 3 | oldest version available, then each consolidated version: 1 January 2010 to 1 April 2021 |
| `832-521-chauffeurverordnung/` | Verordnung über den Vollzug der Eidgenössischen Verordnung über die Arbeits- und Ruhezeit der berufsmässigen Motorfahrzeugführer (BSG 832.521) | 2 | oldest version available, then each consolidated version: 1 January 2011 to 1 April 2021 |
| `832-711-kfamzv/` | Verordnung über die Familienzulagen (BSG 832.711) | 2 | oldest version available, then each consolidated version: 1 January 2012 to 1 January 2019 |
| `836-111-amv/` | Arbeitsmarktverordnung (BSG 836.111) | 7 | oldest version available, then each consolidated version: 1 January 2013 to 1 January 2025 |
| `841-111-akbv/` | Verordnung über die Ausgleichskasse des Kantons Bern und ihre Zweigstellen (BSG 841.111) | 2 | oldest version available, then each consolidated version: 1 January 2012 to 1 November 2026 |
| `841-311-ev-elg/` | Einführungsverordnung zum Bundesgesetz über Ergänzungsleistungen zur Alters-, Hinterlassenen- und Invalidenversicherung (BSG 841.311) | 12 | oldest version available, then each consolidated version: 1 January 2016 to 1 January 2026 |
| `842-111-1-kkvv/` | Kantonale Krankenversicherungsverordnung (BSG 842.111.1) | 12 | oldest version available, then each consolidated version: 1 July 2014 to 1 December 2025 |
| `842-111-5-zulav/` | Verordnung über die Zulassung zur Tätigkeit zulasten der obligatorischen Krankenpflegeversicherung (BSG 842.111.5) | 6 | as enacted, then each consolidated version: 1 February 2014 to 1 January 2024 |
| `854-171/` | Verordnung über die Wohnbau- und Eigentumsförderung (BSG 854.171) | 2 | oldest version available, then each consolidated version: 1 May 2003 to 1 April 2021 |
| `860-21-slv/` | Verordnung über die sozialen Leistungsangebote (BSG 860.21) | 7 | as enacted, then each consolidated version: 1 January 2022 to 1 November 2026 |
| `860-22-fkjv/` | Verordnung über die Leistungsangebote der Familien-, Kinder- und Jugendförderung (BSG 860.22) | 7 | oldest version available, then each consolidated version: 1 January 2022 to 1 August 2026 |
| `860-31-blv/` | Verordnung über die Leistungen für Menschen mit Behinderungen (BSG 860.31) | 5 | as enacted, then each consolidated version: 1 January 2024 to 1 November 2026 |
| `860-111-sozialhilfeverordnung-shv/` | Verordnung über die öffentliche Sozialhilfe (BSG 860.111) | 22 | oldest version available, then each consolidated version: 1 January 2015 to 1 January 2026 |
| `860-111-1-sildv/` | Direktionsverordnung über die Bemessung von situationsbedingten Leistungen (BSG 860.111.1) | 3 | as enacted, then each consolidated version: 1 October 2015 to 1 January 2022 |
| `860-211-sldv/` | Direktionsverordnung über die sozialen Leistungsangebote (BSG 860.211) | 1 | as enacted, 1 January 2022 |
| `860-221-fkjdv/` | Direktionsverordnung über die Leistungsangebote der Familien-, Kinder- und Jugendförderung (BSG 860.221) | 1 | as enacted, 1 January 2022 |
| `860-311-bldv/` | Direktionsverordnung über die Leistungen für Menschen mit Behinderungen (BSG 860.311) | 1 | as enacted, 1 May 2024 |
| `861-111-safv/` | Verordnung über die Sozialhilfe im Asyl- und Flüchtlingsbereich (BSG 861.111) | 1 | as enacted, 1 July 2020 |
| `861-111-1-sadv/` | Direktionsverordnung über die Sozialhilfe im Asylbereich (BSG 861.111.1) | 2 | as enacted, then each consolidated version: 1 July 2020 to 1 January 2024 |
| `861-112-dafav/` | Verordnung über die Datenbearbeitung im Asyl-, Flüchtlings- und Ausländerbereich (BSG 861.112) | 4 | as enacted, then each consolidated version: 1 July 2020 to 1 November 2026 |
| `873-111-gvv/` | Gebäudeversicherungsverordnung (BSG 873.111) | 2 | as enacted, then each consolidated version: 1 January 2011 to 1 September 2026 |
| `901-112-kantonale-hartefallverordnung/` | Kantonale Verordnung über Härtefallmassnahmen für Unternehmen im Zusammenhang mit der Covid-19-Epidemie (BSG 901.112) | 9 | as enacted, then each consolidated version: 18 December 2020 to 23 December 2021 |
| `901-113-kantonale-hartefallverordnung-2022/` | Kantonale Verordnung über Härtefallmassnahmen für Unternehmen im Zusammenhang mit der Covid-19-Epidemie im Jahr 2022 (BSG 901.113) | 1 | as enacted, 1 March 2022 |
| `902-111-kihv/` | Kantonale Verordnung über Investitionshilfe für Berggebiete (BSG 902.111) | 3 | as enacted, then each consolidated version: 1 July 2008 to 1 April 2021 |
| `910-111-pvlv/` | Verordnung über Produktion und Vermarktung in der Landwirtschaft (BSG 910.111) | 5 | oldest version available, then each consolidated version: 1 August 2011 to 1 March 2026 |
| `910-112-elkv/` | Verordnung über die Erhaltung der Lebensgrundlagen und der Kulturlandschaft (BSG 910.112) | 7 | oldest version available, then each consolidated version: 1 January 2014 to 1 March 2023 |
| `910-113-svv/` | Verordnung über Strukturverbesserungen in der Landwirtschaft (BSG 910.113) | 3 | oldest version available, then each consolidated version: 1 January 2014 to 1 January 2022 |
| `913-111-vbwv/` | Verordnung über das Verfahren bei Boden- und Waldverbesserungen (BSG 913.111) | 5 | oldest version available, then each consolidated version: 1 January 2014 to 1 January 2023 |
| `915-11-lbv/` | Verordnung über die landwirtschaftliche und bäuerlich-hauswirtschaftliche Beratung (BSG 915.11) | 2 | oldest version available, then each consolidated version: 1 January 2006 to 1 April 2021 |
| `916-51-ktsv/` | Kantonale Tierseuchenverordnung (BSG 916.51) | 5 | oldest version available, then each consolidated version: 1 January 2013 to 1 August 2026 |
| `916-141-111-rebv/` | Rebbauverordnung (BSG 916.141.111) | 4 | oldest version available, then each consolidated version: 1 March 2011 to 1 January 2023 |
| `916-141-111-1-rebdv/` | Direktionsverordnung über den Rebbau (BSG 916.141.111.1) | 2 | oldest version available, then each consolidated version: 1 March 2014 to 1 January 2019 |
| `916-141-111-3-kubr/` | Reglement über die kontrollierten Ursprungsbezeichnungen (BSG 916.141.111.3) | 3 | oldest version available, then each consolidated version: 1 June 2015 to 1 July 2024 |
| `916-812-thv/` | Verordnung über den Tierschutz und die Hunde (BSG 916.812) | 6 | oldest version available, then each consolidated version: 1 January 2013 to 1 March 2022 |
| `916-911-ktamv/` | Kantonale Verordnung über die Tierarzneimittel (BSG 916.911) | 2 | as enacted, then each consolidated version: 1 January 2012 to 1 April 2021 |
| `921-111-kwav/` | Kantonale Waldverordnung (BSG 921.111) | 4 | oldest version available, then each consolidated version: 1 January 2014 to 1 January 2023 |
| `922-51-wildschadenverordnung-wsv/` | Verordnung über die Verhütung und Entschädigung von Wildschäden (BSG 922.51) | 3 | oldest version available, then each consolidated version: 1 January 2010 to 1 March 2023 |
| `922-63-wtschv/` | Verordnung über den Wildtierschutz (BSG 922.63) | 5 | oldest version available, then each consolidated version: 1 January 2010 to 1 August 2024 |
| `922-111-jav/` | Jagdverordnung (BSG 922.111) | 7 | oldest version available, then each consolidated version: 1 June 2013 to 1 March 2023 |
| `922-111-1-jadv/` | Direktionsverordnung über die Jagd (BSG 922.111.1) | 5 | oldest version available, then each consolidated version: 1 December 2009 to 1 March 2023 |
| `922-111-2-jdv/` | Direktionsverordnung über die Jagdprüfung (BSG 922.111.2) | 4 | oldest version available, then each consolidated version: 1 May 2017 to 1 October 2023 |
| `923-111-fiv/` | Verordnung über die Fischerei (BSG 923.111) | 4 | oldest version available, then each consolidated version: 1 November 2009 to 1 January 2026 |
| `923-111-1-fidv/` | Direktionsverordnung über die Fischerei (BSG 923.111.1) | 5 | oldest version available, then each consolidated version: 1 January 2015 to 1 January 2026 |
| `930-11-hgv/` | Verordnung über Handel und Gewerbe (BSG 930.11) | 6 | oldest version available, then each consolidated version: 1 August 2008 to 1 April 2022 |
| `935-111-ggv/` | Gastgewerbeverordnung (BSG 935.111) | 5 | oldest version available, then each consolidated version: 1 July 2009 to 1 March 2023 |
| `935-211-1-tev/` | Tourismusentwicklungsverordnung (BSG 935.211.1) | 3 | oldest version available, then each consolidated version: 1 January 2015 to 1 April 2021 |
| `935-520-kgsv/` | Kantonale Geldspielverordnung (BSG 935.520) | 6 | oldest version available, then each consolidated version: 1 January 2015 to 1 May 2026 |
| `935-901-pgv/` | Prostitutionsgewerbeverordnung (BSG 935.901) | 6 | as enacted, then each consolidated version: 1 April 2013 to 1 September 2026 |
| `935-976-1-taxiv/` | Taxiverordnung (BSG 935.976.1) | 2 | as enacted, then each consolidated version: 1 June 2012 to 1 January 2022 |
| `941-11-mgv/` | Verordnung über das Mass- und Gewichtswesen (BSG 941.11) | 11 | oldest version available, then each consolidated version: 1 January 2014 to 1 January 2026 |
| `943-511-1-kantonale-waffenverordnung-kwv/` | Verordnung über den Vollzug des eidgenössischen Waffenrechts (BSG 943.511.1) | 3 | oldest version available, then each consolidated version: 1 January 2012 to 1 April 2021 |
| `943-521-kantonale-sprengstoffverordnung-ksprstv/` | Verordnung zum Bundesgesetz über explosionsgefährliche Stoffe (BSG 943.521) | 2 | oldest version available, then each consolidated version: 1 January 2009 to 1 April 2021 |
| `bsg-102-1/` | Gesetz über das Sonderstatut des Berner Juras und über die französischsprachige Minderheit des Verwaltungskreises Biel/Bienne (BSG 102.1) | 1 | current consolidated text (oldest version available), 2025-03-01 |
| `bsg-102-111-1/` | Geschäftsordnung des Bernjurassischen Rats (BSG 102.111.1) | 1 | current consolidated text (oldest version available), 2026-06-01 |
| `bsg-102-111-2/` | Geschäftsordnung des Rats für französischsprachige Angelegenheiten des Verwaltungskreises Biel/Bienne (BSG 102.111.2) | 1 | current consolidated text (oldest version available), 2026-06-01 |
| `bsg-105-234-1/` | Konkordat zwischen den Kantonen Bern und Jura über den Wechsel der Einwohnergemeinde Moutier zum Kanton Jura (BSG 105.234-1) | 1 | current consolidated text (oldest version available), 2026-01-01 |
| `bsg-105-235-1-1/` | Vollzugsvereinbarung zwischen den Kantonen Bern und Jura im Zusammenhang mit dem Kantonswechsel der Einwohnergemeinde Moutier betreffend die evangelisch-reformierte Kirchgemeinde Moutier (BSG 105.235.1-1) | 1 | current consolidated text (oldest version available), 2025-01-01 |
| `bsg-105-235-1-10/` | Vollzugsvereinbarung zwischen den Kantonen Bern und Jura im Zusammenhang mit dem Kantonswechsel der Einwohnergemeinde Moutier betreffend die Besteuerung und Zulassungsänderung von Fahrzeugen (BSG 105.235.1-10) | 1 | current consolidated text (oldest version available), 2026-01-01 |
| `bsg-105-235-1-11/` | Vollzugsvereinbarung zwischen den Kantonen Bern und Jura im Zusammenhang mit dem Kantonswechsel der Einwohnergemeinde Moutier betreffend die Übertragung der Kantonsstrassen und den Winterdienst (BSG 105.235.1-11) | 1 | current consolidated text (oldest version available), 2025-10-01 |
| `bsg-105-235-1-12/` | Vollzugsvereinbarung zwischen den Kantonen Bern und Jura im Zusammenhang mit dem Kantonswechsel der Einwohnergemeinde Moutier betreffend die Modalitäten der Übertragung an den Kanton Jura von Grundstücken des Kantons Bern (BSG 105.235.1-12) | 1 | current consolidated text (oldest version available), 2025-10-01 |
| `bsg-105-235-1-13/` | Vollzugsvereinbarung zwischen den Kantonen Bern und Jura im Zusammenhang mit dem Kantonswechsel der Einwohnergemeinde Moutier betreffend archäologische Objekte und Baudenkmäler (BSG 105.235.1-13) | 1 | current consolidated text (oldest version available), 2025-10-01 |
| `bsg-105-235-1-14/` | Vollzugsvereinbarung zwischen den Kantonen Bern und Jura im Zusammenhang mit dem Kantonswechsel der Einwohnergemeinde Moutier betreffend das Zivilstandswesen (BSG 105.235.1-14) | 1 | current consolidated text (oldest version available), 2025-10-01 |
| `bsg-105-235-1-15/` | Vollzugsvereinbarung zwischen den Kantonen Bern und Jura im Zusammenhang mit dem Kantonswechsel der Einwohnergemeinde Moutier betreffend die Anerkennung von Konzessionen für Wasserkraft- und Gebrauchswassernutzungen in der Gemeinde Moutier (BSG 105.235.1-15) | 1 | current consolidated text (oldest version available), 2026-01-01 |
| `bsg-105-235-1-16/` | Vollzugsvereinbarung zwischen den Kantonen Bern und Jura im Zusammenhang mit dem Kantonswechsel der Einwohnergemeinde Moutier betreffend die Übertragung von Archiven (BSG 105.235.1-16) | 1 | current consolidated text (oldest version available), 2026-01-01 |
| `bsg-105-235-1-17/` | Vollzugsvereinbarung zwischen den Kantonen Bern und Jura im Zusammenhang mit dem Kantonswechsel der Einwohnergemeinde Moutier betreffend den polizeilichen Bereich (BSG 105.235.1-17) | 1 | current consolidated text (oldest version available), 2025-11-15 |
| `bsg-105-235-1-18/` | Vollzugsvereinbarung zwischen den Kantonen Bern und Jura im Zusammenhang mit dem Kantonswechsel der Einwohnergemeinde Moutier betreffend die Aufnahme und Unterbringung von Personen aus dem Asylbereich, die in Privatunterkünften in Moutier untergebracht sind (BSG 105.235.1-18) | 1 | current consolidated text (oldest version available), 2026-01-01 |
| `bsg-105-235-1-19/` | Vollzugsvereinbarung zwischen den Kantonen Bern und Jura im Zusammenhang mit dem Kantonswechsel der Einwohnergemeinde Moutier betreffend die Vermögensausscheidung (BSG 105.235.1-19) | 1 | current consolidated text (oldest version available), 2026-01-01 |
| `bsg-105-235-1-2/` | Vollzugsvereinbarung zwischen den Kantonen Bern und Jura im Zusammenhang mit dem Kantonswechsel der Einwohnergemeinde Moutier betreffend die römisch-katholische Kirchgemeinde Moutier (BSG 105.235.1-2) | 1 | current consolidated text (oldest version available), 2025-01-01 |
| `bsg-105-235-1-20/` | Vollzugsvereinbarung zwischen den Kantonen Bern und Jura im Zusammenhang mit dem Kantonswechsel der Einwohnergemeinde Moutier betreffend die Anpassung der Finanzflüsse (BSG 105.235.1-20) | 1 | current consolidated text (oldest version available), 2026-01-01 |
| `bsg-105-235-1-21/` | Vollzugsvereinbarung zwischen den Kantonen Bern und Jura im Zusammenhang mit dem Kantonswechsel der Einwohnergemeinde Moutier betreffend den Bereich der Musikschulen (BSG 105.235.1-21) | 1 | current consolidated text (oldest version available), 2026-01-01 |
| `bsg-105-235-1-22/` | Vollzugsvereinbarung zwischen den Kantonen Bern und Jura im Zusammenhang mit dem Kantonswechsel der Einwohnergemeinde Moutier betreffend den Bereich Natur- und Waldschutz (BSG 105.235.1-22) | 1 | current consolidated text (oldest version available), 2026-01-01 |
| `bsg-105-235-1-23/` | Vollzugsvereinbarung zwischen den Kantonen Bern und Jura im Zusammenhang mit dem Kantonswechsel der Einwohnergemeinde Moutier betreffend die Änderung von rechtskräftigen öffentlich-rechtlichen Entscheiden und Urteilen (BSG 105.235.1-23) | 1 | current consolidated text (oldest version available), 2026-01-01 |
| `bsg-105-235-1-24/` | Vollzugsvereinbarung zwischen den Kantonen Bern und Jura im Zusammenhang mit dem Kantonswechsel der Einwohnergemeinde Moutier betreffend die Bereiche des Grundbuchs und des Notariatsrechts (BSG 105.235.1-24) | 1 | current consolidated text (oldest version available), 2026-01-01 |
| `bsg-105-235-1-25/` | Vollzugsvereinbarung zwischen den Kantonen Bern und Jura im Zusammenhang mit dem Kantonswechsel der Einwohnergemeinde Moutier betreffend das Rettungswesen (BSG 105.235.1-25) | 1 | current consolidated text (oldest version available), 2026-01-01 |
| `bsg-105-235-1-26/` | Vollzugsvereinbarung zwischen den Kantonen Bern und Jura im Zusammenhang mit dem Kantonswechsel der Einwohnergemeinde Moutier betreffend die Ausbildung von medizinischem und Pflegepersonal (BSG 105.235.1-26) | 1 | current consolidated text (oldest version available), 2026-01-01 |
| `bsg-105-235-1-27/` | Vollzugsvereinbarung zwischen den Kantonen Bern und Jura im Zusammenhang mit dem Kantonswechsel der Einwohnergemeinde Moutier betreffend die Landwirtschaft (BSG 105.235.1-27) | 1 | current consolidated text (oldest version available), 2026-01-01 |
| `bsg-105-235-1-28/` | Vollzugsvereinbarung zwischen den Kantonen Bern und Jura im Zusammenhang mit dem Kantonswechsel der Einwohnergemeinde Moutier betreffend die vor Gerichtsbehörden hängigen Verfahren (BSG 105.235.1-28) | 1 | current consolidated text (oldest version available), 2026-01-01 |
| `bsg-105-235-1-29/` | Vollzugsvereinbarung zwischen den Kantonen Bern und Jura im Zusammenhang mit dem Kantonswechsel der Einwohnergemeinde Moutier betreffend den Bereich des Sozialwesens (BSG 105.235.1-29) | 1 | current consolidated text (oldest version available), 2026-01-01 |
| `bsg-105-235-1-3/` | Vollzugsvereinbarung zwischen den Kantonen Bern und Jura im Zusammenhang mit dem Kantonswechsel der Einwohnergemeinde Moutier betreffend den Steuerbereich (BSG 105.235.1-3) | 1 | current consolidated text (oldest version available), 2025-01-01 |
| `bsg-105-235-1-30/` | Vollzugsvereinbarung zwischen den Kantonen Bern und Jura im Zusammenhang mit dem Kantonswechsel der Einwohnergemeinde Moutier betreffend die Behandlung hängiger Schuldbetreibungs- und Konkursverfahren (BSG 105.235.1-30) | 1 | current consolidated text (oldest version available), 2026-01-01 |
| `bsg-105-235-1-31/` | Vollzugsvereinbarung zwischen den Kantonen Bern und Jura im Zusammenhang mit dem Kantonswechsel der Einwohnergemeinde Moutier betreffend Strafverfahren in der Phase des Vorverfahrens (BSG 105.235.1-31) | 1 | current consolidated text (oldest version available), 2026-01-01 |
| `bsg-105-235-1-32/` | Vollzugsvereinbarung zwischen den Kantonen Bern und Jura im Zusammenhang mit dem Kantonswechsel der Einwohnergemeinde Moutier betreffend den Gesundheitsbereich (BSG 105.235.1-32) | 1 | current consolidated text (oldest version available), 2026-01-01 |
| `bsg-105-235-1-4/` | Vollzugsvereinbarung zwischen den Kantonen Bern und Jura im Zusammenhang mit dem Kantonswechsel der Einwohnergemeinde Moutier betreffend den Volksschulbereich (BSG 105.235.1-4) | 1 | current consolidated text (oldest version available), 2025-07-01 |
| `bsg-105-235-1-5/` | Vollzugsvereinbarung zwischen den Kantonen Bern und Jura im Zusammenhang mit dem Kantonswechsel der Einwohnergemeinde Moutier betreffend die Sekundarstufe II (BSG 105.235.1-5) | 1 | current consolidated text (oldest version available), 2026-05-01 |
| `bsg-105-235-1-6/` | Rahmenvereinbarung zwischen den Kantonen Bern und Jura für sämtliche Vollzugsvereinbarungen im Zusammenhang mit dem Kantonswechsel der Einwohnergemeinde Moutier (BSG 105.235.1-6) | 1 | current consolidated text (oldest version available), 2025-07-01 |
| `bsg-105-235-1-7/` | Vollzugsvereinbarung zwischen den Kantonen Bern und Jura im Zusammenhang mit dem Kantonswechsel der Einwohnergemeinde Moutier betreffend die Burgergemeinde Moutier (BSG 105.235.1-7) | 1 | current consolidated text (oldest version available), 2025-07-01 |
| `bsg-105-235-1-8/` | Vollzugsvereinbarung zwischen den Kantonen Bern und Jura im Zusammenhang mit dem Kantonswechsel der Einwohnergemeinde Moutier betreffend das Bürgerrecht (BSG 105.235.1-8) | 1 | current consolidated text (oldest version available), 2025-10-01 |
| `bsg-105-235-1-9/` | Vollzugsvereinbarung zwischen den Kantonen Bern und Jura im Zusammenhang mit dem Kantonswechsel der Einwohnergemeinde Moutier betreffend die Verwaltung der in der Gemeinde Moutier gelegenen belasteten Standorte (BSG 105.235.1-9) | 1 | current consolidated text (oldest version available), 2025-10-01 |
| `bsg-105-42-1/` | Gebietsänderungskonkordat über den Wechsel der bernischen Einwohnergemeinde Clavaleyres zum Kanton Freiburg (BSG 105.42-1) | 1 | current consolidated text (oldest version available), 2022-01-01 |
| `bsg-105-43-1/` | Vereinbarung zwischen den Kantonen Bern und Freiburg über den Vollzug des Wechsels der Gemeinde Clavaleyres zum Kanton Freiburg (BSG 105.43-1) | 1 | current consolidated text (oldest version available), 2022-01-01 |
| `bsg-122-30/` | Grossratsbeschluss betreffend den Beitritt zur Vereinbarung zwischen Bund und Kantonen betreffend Umsetzung, Anwendung und Entwicklung des Schengen/Dublin-Besitzstands (BSG 122.30) | 1 | current consolidated text (oldest version available), 2008-11-01 |
| `bsg-122-30-1/` | Vereinbarung zwischen Bund und Kantonen betreffend Umsetzung, Anwendung und Entwicklung des Schengen/Dublin-Besitzstands (BSG 122.30-1) | 1 | current consolidated text (oldest version available), 2008-11-01 |
| `bsg-141-221/` | Regierungsratsbeschluss betreffend die Nummerierung der Listen bei Nationalratswahlen (BSG 141.221) | 1 | current consolidated text (oldest version available), 1987-08-12 |
| `bsg-151-211/` | Geschäftsordnung des Grossen Rates (BSG 151.211) | 1 | current consolidated text (oldest version available), 2026-09-01 |
| `bsg-151-212/` | Geschäftsordnung der Deputation des Berner Juras und Welschbiels (BSG 151.212) | 1 | current consolidated text (oldest version available), 2014-10-22 |
| `bsg-151-41-1/` | Vereinbarung über die Interparlamentarische Konferenz der Nordwestschweiz (BSG 151.41-1) | 1 | current consolidated text (oldest version available), 2023-02-25 |
| `bsg-151-42-1/` | Vereinbarung über die Nordwestschweizer Regierungskonferenz (BSG 151.42-1) | 1 | current consolidated text (oldest version available), 2025-07-01 |
| `bsg-151-43-1/` | Leitbild der Westschweizer Regierungskonferenz (BSG 151.43-1) | 1 | current consolidated text (oldest version available), 2005-06-09 |
| `bsg-152-010/` | Dekret über die Aufgaben der Direktionen und der Staatskanzlei und die Direktionsbezeichnungen (BSG 152.010) | 1 | current consolidated text (oldest version available), 2024-01-01 |
| `bsg-152-09/` | Gesetz über die Informations- und Cybersicherheit (BSG 152.09) | 1 | current consolidated text (oldest version available), 2026-11-01 |
| `bsg-152-091/` | Verordnung über die Informations- und Datensicherheit (BSG 152.091) | 1 | current consolidated text (oldest version available), 2026-11-01 |
| `bsg-154-11/` | Dekret über die Gebühren des Grossen Rates und des Regierungsrates (BSG 154.11) | 1 | current consolidated text (oldest version available), 2020-10-01 |
| `bsg-161-12/` | Dekret betreffend die Verfahrenskosten und die Verwaltungsgebühren der Gerichtsbehörden und der Staatsanwaltschaft (BSG 161.12) | 1 | current consolidated text (oldest version available), 2026-05-01 |
| `bsg-161-13/` | Dekret über die Gerichtssprachen (BSG 161.13) | 1 | current consolidated text (oldest version available), 2026-05-01 |
| `bsg-162-111/` | Grossratsbeschluss betreffend die Verlängerung der Amtsdauer der Mitglieder und Ersatzmitglieder des Obergerichtes und Festlegung des Beginns der Amtsdauer auf den 1. Januar (BSG 162.111) | 1 | current consolidated text (oldest version available), 1986-08-25 |
| `bsg-166-1/` | Dekret über die Entschädigung der nebenamtlichen Richterinnen und Richter (BSG 166.1) | 1 | current consolidated text (oldest version available), 2024-01-01 |
| `bsg-173-11/` | Grossratsbeschluss betreffend den Beitritt zum Karlsruher Übereinkommen (BSG 173.11) | 1 | current consolidated text (oldest version available), 2005-10-01 |
| `bsg-173-11-1/` | Übereinkommen zwischen der Regierung der Bundesrepublik Deutschland, der Regierung der Französischen Republik, der Regierung des Grossherzogtums Luxemburg und dem Schweizerischen Bundesrat, handelnd im Namen der Kantone Solothurn, Basel-Stadt, Basel-Landschaft, Aargau und Jura, über die grenzüberschreitende Zusammenarbeit zwischen Gebietskörperschaften und örtlichen öffentlichen Stellen (BSG 173.11-1) | 1 | current consolidated text (oldest version available), 2005-10-01 |
| `bsg-212-223-4/` | Grossratsbeschluss betreffend die Genehmigung der Vereinbarung zwischen dem Kanton Bern und dem Kanton Freiburg über die Aufsicht über die Einrichtungen der beruflichen Vorsorge mit Sitz im Kanton Freiburg (BSG 212.223.4) | 1 | current consolidated text (oldest version available), 2012-01-01 |
| `bsg-212-223-4-1/` | Interkantonale Vereinbarung zwischen dem Kanton Bern und dem Kanton Freiburg über die Aufsicht über die Einrichtungen der beruflichen Vorsorge mit Sitz im Kanton Freiburg (BSG 212.223.4-1) | 1 | current consolidated text (oldest version available), 2012-01-01 |
| `bsg-212-225-11/` | Dekret über die Bestätigung von Legaten (BSG 212.225.11) | 1 | current consolidated text (oldest version available), 1994-01-01 |
| `bsg-222-153-21/` | Normalarbeitsvertrag für die Landwirtschaft (BSG 222.153.21) | 1 | current consolidated text (oldest version available), 2012-01-01 |
| `bsg-222-153-22/` | Normalarbeitsvertrag für den Hausdienst (BSG 222.153.22) | 1 | current consolidated text (oldest version available), 2020-01-01 |
| `bsg-222-153-23/` | Normalarbeitsvertrag für den Detailhandel (BSG 222.153.23) | 1 | current consolidated text (oldest version available), 2012-01-01 |
| `bsg-222-153-24/` | Normalarbeitsvertrag für die 24-Stunden-Betreuung (BSG 222.153.24) | 1 | current consolidated text (oldest version available), 2020-01-01 |
| `bsg-224-11/` | Dekret über die Organisation des Handelsregisters (BSG 224.11) | 1 | current consolidated text (oldest version available), 2020-11-01 |
| `bsg-271-1/` | Einführungsgesetz zur Zivilprozessordnung, zur Strafprozessordnung und zur Jugendstrafprozessordnung (BSG 271.1) | 1 | current consolidated text (oldest version available), 2026-09-01 |
| `bsg-322-1/` | Grossratsbeschluss betreffend den Beitritt zur Vereinbarung zwischen den Kantonen und dem Bund über die Harmonisierung der Informatik in der Strafjustiz (BSG 322.1) | 1 | current consolidated text (oldest version available), 2025-07-01 |
| `bsg-322-1-1/` | Vereinbarung zwischen den Kantonen und dem Bund über die Harmonisierung der Informatik in der Strafjustiz (BSG 322.1-1) | 1 | current consolidated text (oldest version available), 2025-07-01 |
| `bsg-349-1/` | Grossratsbeschluss betreffend den Beitritt zum Konkordat der Kantone der Nordwest- und Innerschweiz über den Vollzug von Strafen und Massnahmen (BSG 349.1) | 1 | current consolidated text (oldest version available), 2008-01-01 |
| `bsg-349-1-1/` | Konkordat der Kantone der Nordwest- und Innerschweiz über den Vollzug von Strafen und Massnahmen (BSG 349.1-1) | 1 | current consolidated text (oldest version available), 2008-01-01 |
| `bsg-410-291-1/` | Konvention zwischen dem Staat Bern und der Evangelischreformierten Landeskirche des Kantons Bern, einerseits, und der Evangelisch-reformierten Kirche des Kantons Jura, anderseits, über den Synodalverband (BSG 410.291-1) | 1 | current consolidated text (oldest version available), 1981-01-01 |
| `bsg-410-331/` | Übereinkunft wegen der Herstellung und neuen Umschreibung des Bistums Basel (BSG 410.331) | 1 | current consolidated text (oldest version available), 1828-03-26 |
| `bsg-410-332/` | Übereinkunft zwischen den hohen Ständen Luzern, Bern, Solothurn und Zug für die Organisation des Bistums Basel (BSG 410.332) | 1 | current consolidated text (oldest version available), 1828-03-28 |
| `bsg-410-333/` | Dekret über Promulgation der päbstlichen Bulle (BSG 410.333) | 1 | current consolidated text (oldest version available), 1828-08-17 |
| `bsg-410-334/` | Übereinkunft betreffend die Einverleibung des alten Kantonsteiles Bern in das Bistum Basel (BSG 410.334) | 1 | current consolidated text (oldest version available), 1864-06-22 |
| `bsg-411-231-91/` | Übereinkunft mit dem hohen Stande Freiburg zu näherer Bestimmung der kirchlichen Verhältnisse der gemischten Gemeinden Ferenbalm, Kerzers und Murten (BSG 411.231.91) | 1 | current consolidated text (oldest version available), 1889-02-06 |
| `bsg-411-232-11/` | Übereinkunft mit Solothurn betreffend die Verhältnisse der ehemaligen Kollaturpfarrei Oberwil (BSG 411.232.11) | 1 | current consolidated text (oldest version available), 1851-07-04 |
| `bsg-411-232-12/` | Grossratsbeschluss zur Übereinkunft zwischen den Ständen Bern und Solothurn vom 23. Dezember 1958 betreffend die kirchlichen Verhältnisse in den evangelisch-reformierten Kirchgemeinden des Bucheggberges und der Bezirke Solothurn, Lebern und Kriegstetten; Änderung und Ergänzung vom 24. September 1979 (BSG 411.232.12) | 1 | current consolidated text (oldest version available), 1980-01-08 |
| `bsg-411-232-12-1/` | Übereinkunft zwischen den Ständen Bern und Solothurn betreffend die kirchlichen Verhältnisse in den evangelisch-reformierten Kirchgemeinden des Bucheggberges und der Bezirke Solothurn, Lebern und Kriegstetten vom 23. Dezember 1958 (BSG 411.232.12-1) | 1 | current consolidated text (oldest version available), 1959-02-18 |
| `bsg-412-11/` | Grossratsbeschluss über die Zahl der vom Kanton besoldeten Pfarrstellen (BSG 412.11) | 1 | current consolidated text (oldest version available), 2015-01-01 |
| `bsg-421-228/` | Vereinbarung zwischen dem Eidgenössischen Departement des Innern und dem Regierungsrat des Kantons Bern betreffend die Archivierung der Akten, die von der Pro Juventute im Zusammenhang mit der Aktion «Kinder der Landstrasse» angelegt wurden (BSG 421.228) | 1 | current consolidated text (oldest version available), 1996-03-06 |
| `bsg-439-12-1/` | Vertrag zwischen den Kantonen Bern und Jura über die Sekundarschule La Courtine in Bellelay (BSG 439.12-1) | 1 | current consolidated text (oldest version available), 2002-01-01 |
| `bsg-439-121-1/` | Convention entre le Canton de Berne et la République et Canton du Jura concernant les écolages liés aux fréquentations scolaires transfrontalières dans le cadre de la scolarité obligatoire (BSG 439.121-1) | 1 | current consolidated text (oldest version available), 2022-08-01 |
| `bsg-439-13/` | Grossratsbeschluss über den Beitritt des Kantons Bern zum Konkordat vom 29. Oktober 1970 über die Schulkoordination (BSG 439.13) | 1 | current consolidated text (oldest version available), 1988-11-22 |
| `bsg-439-13-1/` | Konkordat über die Schulkoordination (BSG 439.13-1) | 1 | current consolidated text (oldest version available), 1988-11-22 |
| `bsg-439-14/` | Grossratsbeschluss betreffend den Beitritt zum Regionalen Schulabkommen über die gegenseitige Aufnahme von Auszubildenden und Ausrichtung von Beiträgen (RSA 2009) (BSG 439.14) | 1 | current consolidated text (oldest version available), 2020-11-01 |
| `bsg-439-14-1/` | Regionales Schulabkommen über die gegenseitige Aufnahme von Auszubildenden und Ausrichtung von Beiträgen (BSG 439.14-1) | 1 | current consolidated text (oldest version available), 2025-08-01 |
| `bsg-439-15/` | Regierungsratsbeschluss über die Vereinbarung zwischen den Kantonen Bern, Jura und Neuenburg über die Beiträge an die Unterrichtskosten (BSG 439.15) | 1 | current consolidated text (oldest version available), 2020-11-01 |
| `bsg-439-15-1/` | Vereinbarung zwischen den Kantonen Bern, Jura und Neuenburg über die Beiträge an die Unterrichtskosten (BSG 439.15-1) | 1 | current consolidated text (oldest version available), 2025-08-01 |
| `bsg-439-16/` | Regierungsratsbeschluss betreffend den Beitritt zur Interkantonalen Vereinbarung über die Beiträge an die Ausbildungskosten in der beruflichen Grundbildung (Berufsfachschulvereinbarung, BFSV) (BSG 439.16) | 1 | current consolidated text (oldest version available), 2007-08-01 |
| `bsg-439-16-1/` | Interkantonale Vereinbarung über die Beiträge an die Ausbildungskosten in der beruflichen Grundbildung (BSG 439.16-1) | 1 | current consolidated text (oldest version available), 2026-08-01 |
| `bsg-439-175/` | Regierungsratsbeschluss betreffend den Beitritt zur Interkantonalen Vereinbarung über die Beiträge an die Bildungsgänge der höheren Fachschulen (HFSV) (BSG 439.175) | 1 | current consolidated text (oldest version available), 2020-11-01 |
| `bsg-439-175-1/` | Interkantonale Vereinbarung über Beiträge an die Bildungsgänge der höheren Fachschulen (BSG 439.175-1) | 1 | current consolidated text (oldest version available), 2014-10-01 |
| `bsg-439-179/` | Regierungsratsbeschluss betreffend den Beitritt zur Interkantonalen Vereinbarung zwischen dem Kanton Bern und dem Kanton Solothurn betreffend Höhere Fachschule für Technik Mittelland (HFTM-AG) (BSG 439.179) | 1 | current consolidated text (oldest version available), 2020-11-01 |
| `bsg-439-179-1/` | Interkantonale Vereinbarung zwischen dem Kanton Bern und dem Kanton Solothurn betreffend Höhere Fachschule für Technik Mittelland (HFTM-AG) (BSG 439.179-1) | 1 | current consolidated text (oldest version available), 2012-08-01 |
| `bsg-439-18/` | Grossratsbeschluss betreffend den Beitritt des Kantons Bern zur interkantonalen Vereinbarung über die Anerkennung von Ausbildungsabschlüssen (Diplomanerkennungsvereinbarung) (BSG 439.18) | 1 | current consolidated text (oldest version available), 2015-05-20 |
| `bsg-439-18-1/` | Interkantonale Vereinbarung über die Anerkennung von Ausbildungsabschlüssen (BSG 439.18-1) | 1 | current consolidated text (oldest version available), 2020-02-01 |
| `bsg-439-182-8/` | Grossratsbeschluss betreffend den Beitritt zur Interkantonalen Vereinbarung zur Harmonisierung von Ausbildungsbeiträgen (BSG 439.182.8) | 1 | current consolidated text (oldest version available), 2021-11-01 |
| `bsg-439-182-8-1/` | Interkantonale Vereinbarung zur Harmonisierung von Ausbildungsbeiträgen (BSG 439.182.8-1) | 1 | current consolidated text (oldest version available), 2011-08-01 |
| `bsg-439-20/` | Regierungsratsbeschluss betreffend den Beitritt zur Interkantonalen Vereinbarung über die Beiträge an die Ausbildungskosten von universitären Hochschulen (BSG 439.20) | 1 | current consolidated text (oldest version available), 2020-01-01 |
| `bsg-439-20-1/` | Interkantonale Vereinbarung über die Beiträge an die Ausbildungskosten von universitären Hochschulen (BSG 439.20-1) | 1 | current consolidated text (oldest version available), 2022-01-01 |
| `bsg-439-21/` | Grossratsbeschluss über den Beitritt des Kantons Bern zur Interkantonalen Fachhochschulvereinbarung vom 12. Juni 2003 (BSG 439.21) | 1 | current consolidated text (oldest version available), 2005-09-01 |
| `bsg-439-21-1/` | Interkantonale Fachhochschulvereinbarung ab 2005 (BSG 439.21-1) | 1 | current consolidated text (oldest version available), 2005-09-01 |
| `bsg-439-27/` | Grossratsbeschluss betreffend den Beitritt zur Interkantonalen Vereinbarung über den schweizerischen Hochschulbereich (Hochschulkonkordat) (BSG 439.27) | 1 | current consolidated text (oldest version available), 2015-01-01 |
| `bsg-439-27-1/` | Interkantonale Vereinbarung über den schweizerischen Hochschulbereich (BSG 439.27-1) | 1 | current consolidated text (oldest version available), 2015-01-01 |
| `bsg-439-28/` | Gesetz über den Beitritt zum Konkordat über die gemeinsame Pädagogische Hochschule der Kantone Bern, Jura und Neuenburg (BSG 439.28) | 1 | current consolidated text (oldest version available), 2021-08-01 |
| `bsg-439-28-1/` | Konkordat über die gemeinsame Pädagogische Hochschule der Kantone Bern, Jura und Neuenburg (BSG 439.28-1) | 1 | current consolidated text (oldest version available), 2021-08-01 |
| `bsg-439-31-1/` | Zusammenarbeitsvereinbarung zwischen den Kantonen Bern und Jura mit dem Ziel, jungen Artistinnen und Artisten sowie jungen Sportlerinnen und Sportlern zu ermöglichen, Schulausbildung und Künstler- oder Sportlerkarriere zu vereinbaren (BSG 439.31-1) | 1 | current consolidated text (oldest version available), 2001-11-21 |
| `bsg-439-32/` | Gesetz über den Beitritt des Kantons Bern zur interkantonalen Vereinbarung über die Fachhochschule der Westschweiz und zur interkantonalen Vereinbarung über die Hochschule Arc Bern-Jura-Neuenburg (BSG 439.32) | 1 | current consolidated text (oldest version available), 2014-08-01 |
| `bsg-439-32-1/` | Interkantonale Vereinbarung über die Fachhochschule der Westschweiz (BSG 439.32-1) | 1 | current consolidated text (oldest version available), 2014-08-01 |
| `bsg-439-32-2/` | Interkantonale Vereinbarung über die Hochschule Arc Bern-Jura-Neuenburg (BSG 439.32-2) | 1 | current consolidated text (oldest version available), 2014-08-01 |
| `bsg-439-33-1/` | Interkantonale Vereinbarung vom 27. September 2001 über die Herstellung und den Vertrieb von Informationsmitteln in der Studien- und Berufsberatung (BSG 439.33-1) | 1 | current consolidated text (oldest version available), 2003-04-01 |
| `bsg-439-34/` | Grossratsbeschluss betreffend den Abschluss der Vereinbarung zwischen dem Kanton Bern und der Interkantonalen Hochschule für Heilpädagogik Zürich (HfH) (BSG 439.34) | 1 | current consolidated text (oldest version available), 2026-03-01 |
| `bsg-439-34-1/` | Vereinbarung zwischen dem Kanton Bern und der Interkantonalen Hochschule für Heilpädagogik Zürich (HfH) (BSG 439.34-1) | 1 | current consolidated text (oldest version available), 2026-08-01 |
| `bsg-439-35-1/` | Vereinbarung über den Sprachaustausch von Schülerinnen und Schülern in den Regionen Pays-d'Enhaut und Obersimmental-Saanen (BSG 439.35-1) | 1 | current consolidated text (oldest version available), 2020-05-01 |
| `bsg-439-36/` | Grossratsbeschluss über den Beitritt zur Vereinbarung über die Vetsuisse-Fakultät der Universitäten Bern und Zürich (BSG 439.36) | 1 | current consolidated text (oldest version available), 2020-07-01 |
| `bsg-439-36-1/` | Vereinbarung über die Vetsuisse-Fakultät der Universitäten Bern und Zürich (BSG 439.36-1) | 1 | current consolidated text (oldest version available), 2006-09-01 |
| `bsg-439-38/` | Gesetz betreffend den Beitritt zur Interkantonalen Vereinbarung für Schulen mit spezifisch-strukturierten Angeboten für Hochbegabte (BSG 439.38) | 1 | current consolidated text (oldest version available), 2013-08-01 |
| `bsg-439-38-1/` | Interkantonale Vereinbarung für Schulen mit spezifisch-strukturierten Angeboten für Hochbegabte (BSG 439.38-1) | 1 | current consolidated text (oldest version available), 2022-08-01 |
| `bsg-439-51-1/` | Vereinbarung zwischen den Kantonen Bern und Jura zur Errichtung der interjurassischen Kommission für die land- und hauswirtschaftliche Berufsbildung (IKOLAB) (BSG 439.51-1) | 1 | current consolidated text (oldest version available), 2026-01-01 |
| `bsg-439-52-1/` | Vertrag zwischen den Kantonen Bern und Jura über das interjurassische MIKT-Zentrum (BSG 439.52-1) | 1 | current consolidated text (oldest version available), 2007-03-01 |
| `bsg-439-54/` | Regierungsratsbeschluss betreffend den Beitritt zur interkantonalen Vereinbarung für schulische Angebote in Spitälern (BSG 439.54) | 1 | current consolidated text (oldest version available), 2025-03-01 |
| `bsg-439-54-1/` | Interkantonale Vereinbarung für schulische Angebote in Spitälern (BSG 439.54-1) | 1 | current consolidated text (oldest version available), 2026-01-01 |
| `bsg-439-60/` | Grossratsbeschluss betreffend den Beitritt zur Interkantonalen Vereinbarung über die Harmonisierung der Volksschule (BSG 439.60) | 1 | current consolidated text (oldest version available), 2009-08-01 |
| `bsg-439-60-1/` | Interkantonale Vereinbarung über die Harmonisierung der Volksschule (BSG 439.60-1) | 1 | current consolidated text (oldest version available), 2009-08-01 |
| `bsg-439-61/` | Grossratsbeschluss betreffend den Beitritt zur Westschweizer Schulvereinbarung (BSG 439.61) | 1 | current consolidated text (oldest version available), 2009-08-01 |
| `bsg-439-61-1/` | Westschweizer Schulvereinbarung (BSG 439.61-1) | 1 | current consolidated text (oldest version available), 2009-08-01 |
| `bsg-439-63/` | Grossratsbeschluss betreffend die Genehmigung des Statuts der Interkantonalen Lehrmittelzentrale ilz (ilz-Statut) (BSG 439.63) | 1 | current consolidated text (oldest version available), 2021-11-01 |
| `bsg-439-63-1/` | Statut der Interkantonalen Lehrmittelzentrale ilz (BSG 439.63-1) | 1 | current consolidated text (oldest version available), 2014-01-01 |
| `bsg-439-71-1/` | Accord entre les cantons de Berne, du Jura et de Neuchâtel instituant la Commission intercantonale de littérature (BSG 439.71-1) | 1 | current consolidated text (oldest version available), 2025-04-01 |
| `bsg-515-81/` | Grossratsbeschluss über die Errichtung der Laupenstiftung (BSG 515.81) | 1 | current consolidated text (oldest version available), 2021-04-01 |
| `bsg-521-91-1/` | Vertrag zwischen dem Kanton Bern, vertreten durch den Regierungsrat, und der Republik und dem Kanton Jura, vertreten durch die Regierung, betreffend die Benützung der Zivilschutz-Ausbildungszentren von Tramelan, Laufen und Lyss/Kappelen (BSG 521.91-1) | 1 | current consolidated text (oldest version available), 1981-01-01 |
| `bsg-559-11-1/` | Konkordat über die polizeiliche Zusammenarbeit in der Nordwestschweiz (BSG 559.11-1) | 1 | current consolidated text (oldest version available), 1999-04-01 |
| `bsg-559-12/` | Grossratsbeschluss betreffend den Beitritt zum Konkordat über Errichtung und Betrieb einer interkantonalen Polizeischule Hitzkirch (BSG 559.12) | 1 | current consolidated text (oldest version available), 2005-01-01 |
| `bsg-559-12-1/` | Konkordat über Errichtung und Betrieb einer interkantonalen Polizeischule Hitzkirch (BSG 559.12-1) | 1 | current consolidated text (oldest version available), 2005-01-01 |
| `bsg-559-13-1/` | Vereinbarung über die interkantonalen Polizeieinsätze (BSG 559.13-1) | 1 | current consolidated text (oldest version available), 2024-07-01 |
| `bsg-559-14/` | Grossratsbeschluss betreffend den Beitritt zum Konkordat über Massnahmen gegen Gewalt anlässlich von Sportveranstaltungen (BSG 559.14) | 1 | current consolidated text (oldest version available), 2014-03-12 |
| `bsg-559-14-1/` | Konkordat über Massnahmen gegen Gewalt anlässlich von Sportveranstaltungen (BSG 559.14-1) | 1 | current consolidated text (oldest version available), 2014-03-12 |
| `bsg-559-15/` | Grossratsbeschluss betreffend den Beitritt zur Interkantonalen Vereinbarung über die computergestützte Zusammenarbeit der Kantone bei der Aufklärung von Gewaltdelikten (ViCLAS-Konkordat) (BSG 559.15) | 1 | current consolidated text (oldest version available), 2010-05-01 |
| `bsg-559-15-1/` | Interkantonale Vereinbarung (bzw. Konkordat) über die computergestützte Zusammenarbeit der Kantone bei der Aufklärung von Gewaltdelikten (BSG 559.15-1) | 1 | current consolidated text (oldest version available), 2010-05-01 |
| `bsg-559-16/` | Grossratsbeschluss betreffend den Beitritt zur interkantonalen bzw. interbehördlichen Vereinbarung über den Datenaustausch zum Betrieb von Lage- und Analysesystemen im Bereich der seriellen Kriminalität (BSG 559.16) | 1 | current consolidated text (oldest version available), 2020-09-01 |
| `bsg-559-16-1/` | Interkantonale bzw. interbehördliche Vereinbarung über den Datenaustausch zum Betrieb von Lage- und Analysesystemen im Bereich der seriellen Kriminalität (BSG 559.16-1) | 1 | current consolidated text (oldest version available), 2020-09-01 |
| `bsg-559-17/` | Grossratsbeschluss betreffend den Beitritt zur Vereinbarung zwischen dem Bund und den Kantonen über die Harmonisierung und die gemeinsame Bereitstellung der Polizeitechnik und -informatik in der Schweiz (VPTI) (BSG 559.17) | 1 | current consolidated text (oldest version available), 2021-04-01 |
| `bsg-559-17-1/` | Vereinbarung zwischen dem Bund und den Kantonen über die Harmonisierung und die gemeinsame Bereitstellung der Polizeitechnik und -informatik in der Schweiz (BSG 559.17-1) | 1 | current consolidated text (oldest version available), 2021-01-01 |
| `bsg-620-03/` | Dekret über die Besondere Rechnung der kantonalen Aufsichtsstelle für Datenschutz (BSG 620.03) | 1 | current consolidated text (oldest version available), 2020-11-01 |
| `bsg-621-4/` | Dekret über die Verwaltung von Geldhinterlagen und Wertsachen durch die Gerichte, Grundbuch-, Betreibungs- und Konkursämter (BSG 621.4) | 1 | current consolidated text (oldest version available), 2010-01-01 |
| `bsg-632-1-1/` | Rahmenvereinbarung für die interkantonale Zusammenarbeit mit Lastenausgleich (BSG 632.1-1) | 1 | current consolidated text (oldest version available), 2007-07-01 |
| `bsg-661-543/` | Dekret über die allgemeine Neubewertung der nichtlandwirtschaftlichen Grundstücke und Wasserkräfte (BSG 661.543) | 1 | current consolidated text (oldest version available), 2021-12-21 |
| `bsg-669-11/` | Grossratsbeschluss über den Beitritt des Kantons Bern zum Konkordat zwischen den Kantonen über den Ausschluss von Steuerabkommen (BSG 669.11) | 1 | current consolidated text (oldest version available), 1949-02-21 |
| `bsg-669-811/` | Grossratsbeschluss betreffend die Vereinbarung zwischen dem Schweizerischen Bundesrat und der Regierung der Französischen Republik über die Besteuerung der Erwerbseinkünfte von Grenzgängern vom 11. April 1983 (BSG 669.811) | 1 | current consolidated text (oldest version available), 1986-09-10 |
| `bsg-682-2/` | Gesetz über den Beitritt des Kantons Bern zur Interkantonalen Vereinbarung vom 22. November 1973 über den Salzverkauf in der Schweiz (BSG 682.2) | 1 | current consolidated text (oldest version available), 1974-12-25 |
| `bsg-682-2-1/` | Interkantonale Vereinbarung über den Salzverkauf in der Schweiz (BSG 682.2-1) | 1 | current consolidated text (oldest version available), 1975-10-01 |
| `bsg-704-111/` | See- und Flussuferverordnung (BSG 704.111) | 1 | current consolidated text (oldest version available), 2023-01-01 |
| `bsg-721-2-1/` | Interkantonale Vereinbarung über die Harmonisierung der Baubegriffe (BSG 721.2-1) | 1 | current consolidated text (oldest version available), 2015-05-01 |
| `bsg-723-13/` | Dekret über das Normalbaureglement (BSG 723.13) | 1 | current consolidated text (oldest version available), 2025-05-01 |
| `bsg-725-1/` | Dekret über das Baubewilligungsverfahren (BSG 725.1) | 1 | current consolidated text (oldest version available), 2023-04-01 |
| `bsg-728-1/` | Dekret über die Umlegung von Baugebiet, die Grenzregulierung und die Ablösung oder Verlegung von Dienstbarkeiten (BSG 728.1) | 1 | current consolidated text (oldest version available), 2023-01-01 |
| `bsg-731-2/` | Gesetz über den Beitritt zur Interkantonalen Vereinbarung über das öffentliche Beschaffungswesen (BSG 731.2) | 1 | current consolidated text (oldest version available), 2022-02-01 |
| `bsg-731-2-1/` | Interkantonale Vereinbarung über das öffentliche Beschaffungswesen (BSG 731.2-1) | 1 | current consolidated text (oldest version available), 2022-02-01 |
| `bsg-732-123-44/` | Dekret über die Beiträge der Grundeigentümer an Erschliessungsanlagen und an weitere öffentliche Werke und Massnahmen (BSG 732.123.44) | 1 | current consolidated text (oldest version available), 2017-04-01 |
| `bsg-751-112-1/` | Interkantonale Vereinbarung zwischen den Kantonen Freiburg, Waadt, Neuenburg, Bern und Solothurn über den gemeinsamen Unterhalt und die Aufsicht des interkantonalen Werkes der II. Juragewässerkorrektion sowie über die Regulierung der dadurch betroffenen Gewässer (Interkantonale Vereinbarung 1985 über die II. Juragewässerkorrektion) (BSG 751.112-1) | 1 | current consolidated text (oldest version available), 1994-01-01 |
| `bsg-752-413/` | Renaturierungsdekret (BSG 752.413) | 1 | current consolidated text (oldest version available), 2021-04-01 |
| `bsg-752-461/` | Dekret über die Wassernutzungsabgaben (BSG 752.461) | 1 | current consolidated text (oldest version available), 2020-08-01 |
| `bsg-752-511/` | Beschluss des Regierungsrates betreffend Verbot der Verwendung von Tritium für hydrologische Untersuchungen (BSG 752.511) | 1 | current consolidated text (oldest version available), 1971-09-22 |
| `bsg-763-1/` | Regierungsratsbeschluss betreffend den Beitritt des Kantons Bern zum Konkordat über die nicht eidgenössisch konzessionierten Seilbahnen und Skilifte (BSG 763.1) | 1 | current consolidated text (oldest version available), 2020-08-01 |
| `bsg-763-1-1/` | Konkordat über die nicht eidgenössisch konzessionierten Seilbahnen und Skilifte (BSG 763.1-1) | 1 | current consolidated text (oldest version available), 2018-05-09 |
| `bsg-767-11/` | Dekret über die Beschränkungen der Schifffahrt (BSG 767.11) | 1 | current consolidated text (oldest version available), 2025-01-01 |
| `bsg-767-2/` | Dekret über die Besteuerung der Schiffe (BSG 767.2) | 1 | current consolidated text (oldest version available), 2021-04-01 |
| `bsg-811-08/` | Grossratsbeschluss betreffend den Beitritt zur Interkantonalen Vereinbarung über die hoch spezialisierte Medizin (IVHSM) (BSG 811.08) | 1 | current consolidated text (oldest version available), 2009-01-01 |
| `bsg-811-08-1/` | Interkantonale Vereinbarung über die hoch spezialisierte Medizin (BSG 811.08-1) | 1 | current consolidated text (oldest version available), 2009-01-01 |
| `bsg-812-12/` | Grossratsbeschluss betreffend den Beitritt zur Interkantonalen Vereinbarung über die kantonalen Beiträge an die Spitäler zur Finanzierung der ärztlichen Weiterbildung und deren Ausgleich unter den Kantonen (BSG 812.12) | 1 | current consolidated text (oldest version available), 2018-04-01 |
| `bsg-812-12-1/` | Interkantonale Vereinbarung über die kantonalen Beiträge an die Spitäler zur Finanzierung der ärztlichen Weiterbildung und deren Ausgleich unter den Kantonen (BSG 812.12-1) | 1 | current consolidated text (oldest version available), 2022-01-25 |
| `bsg-813-113/` | Grossratsbeschluss betreffend den Beitritt zur Vereinbarung der nordwestschweizerischen Kantone über die Führung eines regionalen Heilmittelinspektorats (BSG 813.113) | 1 | current consolidated text (oldest version available), 2003-02-13 |
| `bsg-813-113-1/` | Vereinbarung der nordwestschweizerischen Kantone über die Führung eines regionalen Heilmittelinspektorates (BSG 813.113-1) | 1 | current consolidated text (oldest version available), 2003-02-13 |
| `bsg-854-13/` | Dekret über die Verbesserung der Wohnverhältnisse in Berggebieten (BSG 854.13) | 1 | current consolidated text (oldest version available), 2021-04-01 |
| `bsg-854-17/` | Dekret über die Wohnbau- und Eigentumsförderung (BSG 854.17) | 1 | current consolidated text (oldest version available), 2021-04-01 |
| `bsg-862-71/` | Regierungsratsbeschluss betreffend den Beitritt des Kantons Bern zur Interkantonalen Vereinbarung für soziale Einrichtungen (IVSE) (BSG 862.71) | 1 | current consolidated text (oldest version available), 2021-08-01 |
| `bsg-862-71-1/` | Interkantonale Vereinbarung für soziale Einrichtungen (BSG 862.71-1) | 1 | current consolidated text (oldest version available), 2020-06-01 |
| `bsg-871-111/` | Feuerschutz- und Feuerwehrverordnung (BSG 871.111) | 1 | current consolidated text (oldest version available), 2025-04-01 |
| `bsg-873-111-2/` | Prämientarif der Gebäudeversicherung (BSG 873.111.2) | 1 | current consolidated text (oldest version available), 2025-01-01 |
| `bsg-923-919-1/` | Vereinbarung zwischen den Kantonen Bern und Freiburg betreffend die Fischerei in den Grenzgewässern der Sense und Saane (BSG 923.919.1) | 1 | current consolidated text (oldest version available), 2010-01-01 |
| `bsg-923-921-1/` | Vereinbarung zwischen den Kantonen Bern und Solothurn betreffend die Fischerei in den Grenzgewässern der Aare (BSG 923.921.1) | 1 | current consolidated text (oldest version available), 2026-01-01 |
| `bsg-923-933-1/` | Vereinbarung zwischen den Kantonen Bern und Neuenburg betreffend die Fischerei im Grenzgewässer des Zihlkanals (BSG 923.933.1) | 1 | current consolidated text (oldest version available), 1996-01-01 |
| `bsg-923-941-1-1/` | Vereinbarung zwischen den Kantonen Bern und Jura über die Fischerei im interkantonalen Abschnitt der Birs (BSG 923.941.1-1) | 1 | current consolidated text (oldest version available), 2026-02-01 |
| `bsg-945-1/` | Grossratsbeschluss betreffend den Beitritt zur interkantonalen Vereinbarung zum Abbau technischer Handelshemmnisse (BSG 945.1) | 1 | current consolidated text (oldest version available), 2001-11-05 |
| `bsg-945-1-1/` | Interkantonale Vereinbarung zum Abbau technischer Handelshemmnisse (BSG 945.1-1) | 1 | current consolidated text (oldest version available), 2001-11-05 |
| `bsg-945-3/` | Grossratsbeschluss betreffend den Beitritt zur Interkantonalen Vereinbarung betreffend die gemeinsame Durchführung von Geldspielen (IKV 2020) (BSG 945.3) | 1 | current consolidated text (oldest version available), 2020-09-01 |
| `bsg-945-3-1/` | Interkantonale Vereinbarung betreffend die gemeinsame Durchführung von Geldspielen (BSG 945.3-1) | 1 | current consolidated text (oldest version available), 2021-01-01 |
| `bsg-945-4/` | Grossratsbeschluss betreffend den Beitritt zum Gesamtschweizerischen Geldspielkonkordat (GSK) (BSG 945.4) | 1 | current consolidated text (oldest version available), 2020-09-01 |
| `bsg-945-4-1/` | Gesamtschweizerisches Geldspielkonkordat (BSG 945.4-1) | 1 | current consolidated text (oldest version available), 2021-01-01 |

## Source

The BSG (systematic collection) of the canton, published by the canton at <https://www.belex.sites.be.ch/>. For each act it gives every consolidated version it holds, with the day each version took effect, and a change table listing each amendment: its decision date, the day it took effect, the provision it touched and its entry in the chronological collection (BAG). Text-layer annexes for the current-text addition and the November 2026 updates are included. Separate PDF annexes attached to other existing histories are not included in this addition.

## Dates

- Each commit is dated at **noon, Europe/Zurich, on the day the version took effect**, as the collection gives it ("in Kraft seit / von"). The decision date of each amending act is the `Enacted:` trailer.
- An act's first commit is its oldest version in the collection. It is credited to the act as enacted only when the change table shows no amendment in force before it; otherwise it is the "oldest version available", naming the earlier amendments.
- Versions that take effect after the retrieval day are on the `zukunft` branch, never merged into `main`.
- `--before="YYYY-MM-DD"` alone uses your clock's time of day; use `T23:59:59Z` or `tools/on.py`.

## Files

In article-based histories, `<act>/art-005.md` is Art. 5 (or § 5), `art-005a.md` Art. 5a; `ingress.md` holds the title, date and preamble; `gliederung.md` the section headings; `schluss.md` the closing formula and signatures. These files use one paragraph or list item per line. Amendment markers (`*`), footnote numbers and the "Stand" date are left out.

Each of the 189 current consolidated additions keeps the official document and reference footnotes in a single `<act>/text.md` file. Where a textual PDF annex is included, it is separate at `<act>/annex-text.md`.

## How it is checked

- Every version of every act is read back from git on the day it took effect and on the day before (`tools/check_repo.py`); both must match `corpus.json`.
- The letters and digits of every version equal those of the canton's own text of that version, and every article's text appears in it in order.
- Health checks: no merge commits, commit dates never go backwards, nothing dated in the future, and every commit's trailers parse.

## What "author" means

The author of a commit is the amending act, named by its entry in the chronological collection (BAG), with an e-mail address that cannot exist (`<act key>@www.belex.sites.be.ch.invalid`). Where one version holds changes by several amending acts and the change table does not say which provision each one touched, the commit names them all. The committer is always Lexifina.

## Limits

This is not an official publication. The binding text is the one the canton publishes as binding (its chronological collection, or its systematic collection where cantonal law makes that binding). The history starts with the oldest consolidated version the collection holds for each act, which for many acts is later than the act's enactment. Only the acts listed above are included.
