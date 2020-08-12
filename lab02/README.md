# Tarefa sobre catálogo de componentes
Aqui vai o link

# Tarefa Web Components 1
<!--
<dcc-trigger label="Mundo P"
             action="noticia/mundo/politica"
             value="Mundo Política">
</dcc-trigger>

<dcc-trigger label="Brasil P"
             action="noticia/brasil/politica"
             value="Brasil Política">
</dcc-trigger>

<dcc-trigger label="Brasil E"
             action="noticia/brasil/esporte"
             value="Brasil Esporte">
</dcc-trigger>

<dcc-trigger label="Bahia E"
             action="noticia/bahia/esporte"
             value="Bahia Esporte">
</dcc-trigger>

<dcc-lively-talk duration="0s"
                 character="doctor"
                 speech="I heard about a ">
  <subscribe-dcc topic="noticia/+/politica"></subscribe-dcc>
</dcc-lively-talk>

<dcc-lively-talk duration="0s"
                 character="nurse"
                 speech="I heard about a ">
  <subscribe-dcc topic="noticia/brasil/+"></subscribe-dcc>
</dcc-lively-talk>

<dcc-lively-talk duration="0s"
                 character="patient"
                 speech="I heard about a ">
  <subscribe-dcc topic="noticia/#"></subscribe-dcc>
</dcc-lively-talk>
-->

#Tarefa Web Components 2
<dcc-trigger label="Next Item" action="next/rss">
</dcc-trigger>

<dcc-rss publish="rss/science" source="https://www.wired.com/category/science/feed">
  <subscribe-dcc topic="next/rss" role="step"></subscribe-dcc>
</dcc-rss>

<dcc-rss publish="rss/design" source="https://www.wired.com/category/design/feed">
  <subscribe-dcc topic="next/rss" role="step"></subscribe-dcc>
</dcc-rss>

<dcc-aggregator publish="aggregate/science" quantity="3">
  <subscribe-dcc topic="rss/science"></subscribe-dcc>
</dcc-aggregator>

<dcc-lively-talk id="doctor"
                 duration="0s"
                 character="doctor"
                 speech="News ">
  <subscribe-dcc topic="aggregate/science"></subscribe-dcc>
</dcc-lively-talk>

<dcc-lively-talk id="nurse"
                 duration="0s"
                 character="nurse"
                 speech="News ">
  <subscribe-dcc topic="rss/science"></subscribe-dcc>
</dcc-lively-talk>

<dcc-lively-talk id="patient"
                 duration="0s"
                 character="patient"
                 speech="News ">
  <subscribe-dcc topic="rss/design"></subscribe-dcc>
</dcc-lively-talk>
