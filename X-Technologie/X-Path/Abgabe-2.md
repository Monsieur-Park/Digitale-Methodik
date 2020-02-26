---

title:        X-Path-Übung2
author:       Yohan Park
tags:         X-Technologie, X-Path, XML
---

<h2>Hausaufgabe: XPath</h2>
                <ul>
                    <li class="small"><strong>Öffnen</strong> Sie die <strong>Datei</strong>
                        <code>Hausaufgaben/Sitzung_02/di-34.xml</code> im Oxygen-XML-Editor.</li>
                    <li class="small"><strong>Verschaffen</strong> Sie sich einen
                            <strong>Überblick</strong> über die XML-Struktur der Datei.</li>
                    <li class="small line-height-one-five"><strong>Beantworten</strong> Sie die folgende Fragen mittels XPath:<ul>
                            <li class="line-height-one-five">An welchem Ort befinden sich die älteste sowie die jüngste Inschrift in der Datei? Geben Sie auch Ihren eingesetzten XPath an.</li>
                            <li class="line-height-one-five"> <strong>Antwort:</strong> //dateEnd/substring-before(., '-'). oder
                       //dateStart/substring-before(., '-'). <br> 
                              Die älteste Schrift befindet sich in Sponheim, ehem. Klosterkirche
                              Die jüngste Schrift befindet sich in Pfaffen-Schwabenheim, Haus Mühlengasse 10
                      </li>                       
                            <li class="line-height-one-five">Wie viele Einträge besitzen eine Schriftzuordnung zur Schriftfamilie <em>Kapitalis</em>? Geben Sie auch Ihren eingesetzten XPath an.</li>
                         <li class="line-height-one-five"> <strong>Antwort:</strong> 244 Einträge <br>
                           //typeface[contains(text(), 'Kapitalis')]</li>
                            <li class="line-height-one-five">Geben Sie einen XPath an, mit dem man alle Einträge aggregieren kann, die sich möglicherweise mit Inschriftenträgern aus Holz beschäftigen.</li>
                      <li class="line-height-one-five"> <strong>Antwort:</strong> 12 Einträge </br>
  //description[contains(., 'Holz')] </li>
                            <li class="line-height-one-five">Geben Sie einen Xpath an, der alle Einträge aggregiert, die sich möglicherweise in einer Kirche befinden.</li>
 <li class="line-height-one-five"><strong>Antwort:</strong> 85 Einträge </br>
  //location[contains(text(),'Kirche')] </li>
                            <li class="line-height-one-five">Geben Sie die Anzahl und den dazugehörigen Xpath aller Einträge an, bei denen das auf der Inschrift eingemeißelte Datum den Monat Mai angibt.</li>
   <li class="line-height-one-five"><strong>Antwort:</strong> 5 Einträge</br>
   count(//dateoninscription[contains(., 'Mai')])</li>
                            <li class="line-height-one-five">Geben Sie einen Xpath an, der alle Einträge aggregiert, bei denen es sich bei dem Inschriftenträger möglicherweise um eine Grabplatte handelt.</li>
  <li class="substep"><strong>Antwort:</strong> 185 Einträge </br>
  //description[matches(., 'Grabplatte')]</li>                          
                        </ul>
                    </li>

