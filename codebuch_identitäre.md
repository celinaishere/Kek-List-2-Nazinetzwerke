# Datensatz Verbindung der Identitären Jugendbewegung und der Politik innerhalb der EU #
Codebuch Stand 2023-03
erstellt von Florian Frankenhuis (ff059@hdm-stuttgart.de)

## Inhalt
- Edges.csv (Edgelist)
- Nodes.csv (Nodelist)
- Codebuch.md (Codierung der Datensätze)

## Ursprung und Datenerhebung

Das Netzwerk soll die Vernetzung der identitären Jugendbewegung mit der Politik innerhalb der EU darstellen.

## Erklärung der Attributenauswahl im Codebuch

Bei der Ermittlung unserer Daten haben wir uns bei den Nodes auf die Attribute id, name, sector, party, role, country und ereignis festgelegt. Für diese Attribute haben wir uns entschieden, da es die Politiker*innen auf der Tätigkeitsebene kategorisiert und einordnet und es uns ermöglicht, diese nach der Parteizugehörigkeit zu filtern. Bei dem Attribut „role“ konnten wir einerseits die aktiven Mitglieder der Identitären Bewegung in Deutschland, Österreich und Frankreich klassifizieren und Politiker*innen kategorisieren, die mit IB-Mitgliedern im echten Leben durch Demonstrationsbesuche, verbale Verteidigung oder Spendenaufrufe, sowie auf Social Media öffentlich sympathisiert haben.
In der Edgelist haben wir uns aufgrund der Datenlage für die Attribute relation, weight und international entschieden. Bei der Beziehungsart haben wir über die Interaktion die Beziehungsstärke (weight) durch verschiedene Abstufungen definiert. Weitergehend haben wir die Förderung von Mitgliedern kategorisiert, da einige Politiker*innen IB-Mitglieder und/oder -Sympathisanten ein Beschäftigungsverhältnis mit ihnen eingegangen oder ihnen private Räumlichkeiten zur Verfügung gestellt haben. Das Attribut des Ereignisses haben wir gewählt, da sich einige Mitglieder politischer Parteien auf Demonstrationen aufgehalten haben, die von der Identitären Bewegung mitorganisiert wurden, wie der „Verteidiger Europas Kongress“ im Jahr 2016. Um internationale Verbindungen zu filtern und zu visualisieren, haben wir uns entschieden, das Attribut „international“ zusätzlich in unser Netzwerk aufzunehmen.


# Node-Attribute

id: Eindeutige Kodierung des Knotens: Initialen der Person bzw. der Partei				
name: Klarname				
				
Sector: In welchem Bereich die Personen tätig sind (außerhalb ihrer Beteiligung in der Identitären)				
1: Politik auf europäischer Ebene				
2: Politik auf nationaler Ebene				
3: Politik auf regionaler Ebene				
4: Medien- und Publizistik				
5: Nicht bekannt				
6: Wirtschaft				
				
party: Parteizugehörigkeit (auf nationaler Ebene)				
afd	Alternative für Deutschland			
fpö	Freiheitliche Partei Österreichs			
rn	Rassemblement National	
ja      Junge Alternative
				
role: Art der Beteiligung				
1: Gründer von der ganzen IB auf nationaler Ebene (heute noch aktiv)				
2: führende Mitglieder: Obere Führer				
3: aktive Mitglieder: Bestätigtes Mitglied				
4: Sympathisanten: Im realen Leben				
5: Sympathisanten: Auf Social Media/Propaganda/Spendenaufrufe				
6: Förderung von Mitgliedern				
				
country: Nationalität				
				
Ereignis: Demonstration/Versammlung ausschließlich von der Identitären organisiert (nur für den Ort, ab 4/5 Personen)
Orga: Identitäre Bewegung
Partei: Freiheitliche Partei Deutschlands (FPÖ)
				
				
# Edge-Attribute			
from: initiierender Knoten				
to: erhaltender Knoten				
				
relation: Beziehungsart				
1: Interaktion: Definierung über Weight				
2: Finanzielle Unterstützung				
3: Mitglied der Partei				
4: Förderung (Beschaffung von Arbeitsplätzen & Bereitstellung von Räumen)				
5: Anwesenheit				
				
				
weight: Beziehungsstärke				
1: Familie (Verwandschaft & Verheiratet)				
2: Intensive Beziehung (Öftere Treffen, Kaffee trinken, Intensiver Austausch, Vertrauensverhältnis)				
3: Gute Beziehung (Gelegentliche Treffen, Austausch)				
4: Oberflächliche Beziehung (einmalige Interaktion, im realen Leben (z.B. Foto, mündl. Verteidigung von IB-Mitgliedern), auf Social Media (z.B. Tweet, einmaliger (Re-)Post, schriftl. Verteidigung von IB-Mitgliedern)				
5: Spendenverhätnis				
6: Keine Beziehung	
