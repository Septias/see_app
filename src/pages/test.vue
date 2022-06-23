<template lang="pug">
main.flex.flex-col.justify-center.items-center
  div.max-width
    h1 Einleitungen
    table
      tr
        th Frage
        th 1
        th 2
        th 3
        th 4
        th 5
      tr
        td Herkunft
        td Vauban
        td Freiburg
        td Neunburg
        td Freiburg
        td Innenstadt
      tr
        td Häufigkeit
        td 5-6 mal Monatlich
        td Wöchentlich
        td sehr selten
        td hin und wieder
        td Ist eher an anderem See
      tr
        td Anreisezeit
        td 30-40min (Auto)
        td 15-20min (Auto)
        td 30min (Auto)
        td 15-20min (Auto)
        td 10-15min (Mopet)
      tr
        td würdest du mit Öffies zum See kommen?
        td Ja, aber
        td Ja, aber
        td Nein
        td Nein
        td Nein
      tr
        td Warum nicht?
        td Transport von Standupboard
        td Verletzung
        td -
        td Hasst Öffies und wusste es nichtmal
        td Erschöpfung nach langem Tag
      tr
        td Kommst du mit anderen Ferkehrsmitteln?
        td Fahrrad, Auto
        td Fahrrad
        td Fahrrad
        td Nein
        td Nein
      tr
        td Würdest du auch mal mit dem Fahrrad kommen?
        td Ja
        td Ja
        td Ja
        td Vielleicht
        td Vielleicht
      tr
        td Warum fährst du mit dem Auto zum See
        td Veretzung
        td Transport von Gütern
        td Distanz
        td Hasst Öffies
        td Erschöpfung & Spontanität

    h2 Was müsste man ändern?
    ul
      li Verleih von Standupboards
      li Nichts
      li Möglichkeit zum Lagern von benötigten Sachen
      li E-bike oder E-Skateboard

    h2 Weiteres
    ul
      li Fährt sowieso viel Fahrrad (1. und 2.)
      li Anreise aus Neuenburg geht eig. nur mit dem Auto
      li Für die Meisten ist die Streckenauswahl nicht das Problem (App oder Google etc.)
      li Interviewee 1 war überrascht über die Möglichkeiten von Öffies
      li Klimatisierung in Bussen wird als schlecht empfunden
      li Rückweg bei Nacht ist gefährlich für junge Frauen
</template>

<style >
  table {
  font-family: arial, sans-serif;
  border-collapse: collapse;
  width: 100%;
}

td, th {
  border: 1px solid #dddddd;
  text-align: left;
  padding: 8px;
}

tr:nth-child(even) {
  background-color: #dddddd;
}

.max-width {
  max-width: 1050px
}
</style>
