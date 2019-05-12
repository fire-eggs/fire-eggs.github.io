# Markdown und Tabelle  

## Markdown pur

Beispiele aus der GitHub Markdown Hilfe

#### Code  

\| First Header  | Second Header | Third Header  | Fourth Header |  
\| ------------- | ------------- | ------------- | ------------- |  
\| Content Cell  | Content Cell  | Content Cell  | Content Cell  |  
\| Content Cell  | Content Cell  | Content Cell  | Content Cell  |  
\| Content Cell  | Content Cell  | Content Cell  | Content Cell  |  
\| Content Cell  | Content Cell  | Content Cell  | Content Cell  |  

#### Ausgabe  

| First Header  | Second Header | Third Header  | Fourth Header |
| ------------- | ------------- | ------------- | ------------- |
| Content Cell  | Content Cell  | Content Cell  | Content Cell  |
| Content Cell  | Content Cell  | Content Cell  | Content Cell  |
| Content Cell  | Content Cell  | Content Cell  | Content Cell  |
| Content Cell  | Content Cell  | Content Cell  | Content Cell  |

Der Titel einer Spalte wird durch Bindestriche von den Zellen mit Daten getrennt. Drei Bindestriche sind das Minium. Die Spaltenbreite wird automatisch gesetzt.  

#### Code  

\| First Header  | Second Header | Third Header  | Fourth Header |  
\| --- | --- | --- | --- |  
\| Content Cell  | Content Cell  | Content Cell  | Content Cell  |  

#### Ausgabe  

| First Header  | Second Header | Third Header  | Fourth Header |
| --- | --- | --- | --- |
| Content Cell  | Content Cell  | Content Cell  | Content Cell  |

Text kann auch als Block formatiert werden. Dafür verwendet man [Gravis](https://de.wikipedia.org/wiki/Gravis_(Typografie)#Darstellung_auf_dem_Computer): `  
Das Beispiel aus der GitHub Hilfedatei:

![NoText](../images/markdown/triplebackticks.png)  

Markierungsmöglichkeiten sind dieselben wie in Markdown allgemein. * für kursiv, ** für fett, kann man auch kombinieren. Details dazu stehen in der [GitHub Helpdatei](https://help.github.com/en/articles/basic-writing-and-formatting-syntax#styling-text).

## HTML Tabelle in Markdown einbetten  

Eine einfache HTML Tabelle. 

#### Code  

\<table>  
  \<tr>  
    \<th>First</th>  
    \<th>Second</th>  
    \<th>Third</th>  
    \<th>Fourth</th>  
  \</tr>  
  \<tr>  
    \<td>  Content Cell </td>  
    \<td>  Content Cell\</td>  
    \<td>  Content Cell</td>  
    \<td>  Content Cell</td>  
  \</tr>  
  \<tr>  
    \<td>  Content Cell</td>  
    \<td>  Content Cell</td>  
    \<td>  Content Cell</td>  
    \<td>  Content Cell</td>  
  \</tr>  
  \<tr>  
    \<td>  Content Cell</td>  
    \<td>  Content Cell</td>  
    \<td>  Content Cell</td>  
    \<td>  Content Cell</td>  
  \</tr>  
  \<tr>  
    \<td>  Content Cell</td>  
    \<td>  Content Cell</td>  
    \<td>  Content Cell</td>  
    \<td>  Content Cell</td>  
  \</tr>  
\</table>  

Eine HTML Tabelle mit Kopf, Inhalt und Fuss.  

Mit dem Element "colspan" können Zellen zu einer zusammengefasst werden.  

\<table>  
    \<thead>  
        \<tr>  
          \<th>Head</th>  
        \</tr>  
    \</thead>  
    \<tbody>  
        \<tr>  
          \<td>Content Cell</td>  
          \<td>Content Cell</td>  
          \<td>Content Cell</td>  
          \<td>Content Cell</td>  
        \</tr>  
    \</tbody>  
    \<tfoot>  
        \<tr>  
          \<td>Foot</td>  
        \</tr>  
    \</tfoot>  
\</table>  

Mit dem Element "colspan" können Zellen zu einer zusammengefasst werden.  

\<table>  
    \<thead>  
        \<tr>  
          \<th>Head</th>  
        \</tr>  
    \</thead>  
    \<tbody>  
        \<tr>  
          \<td colspan="3">Content Cell 1</td>  
          \<td>Content Cell 4</td>  
        \</tr>  
    \</tbody>  
    \<tfoot>  
        \<tr>  
          \<td>Foot</td>  
        \</tr>  
    \</tfoot>  
\</table>  

\<table>  
    \<thead>  
        \<tr>  
          \<th>Head\</th>  
        </tr>  
    \</thead>  
    \<tbody>
        \<tr>  
          \<td rowspan="2">Content Cell Row 1\</td>  
          \<td>Content Cell</td>  
          \<td>Content Cell</td>  
          \<td>Content Cell</td>  
        \</tr>  
        \<tr>  
          \<td>Content Cell</td>  
          \<td>Content Cell</td>  
          \<td>Content Cell</td>  
          \<td>Content Cell</td>  
        \</tr>    
    \</tbody>  
    \<tfoot>  
        \<tr>  
          \<td>Foot</td>  
        \</tr>  
    \</tfoot>  
\</table>  

#### Ausgabe

Eine einfache HTML Tabelle. 

<table>
  <tr>
    <th>First </th>
    <th>Second</th>
    <th>Third</th>
    <th>Fourth</th>
  </tr>
  <tr>
    <td>Content Cell</td>
    <td>Content Cell</td>
    <td>Content Cell</td>
    <td>Content Cell</td>
  </tr>
  <tr>
    <td>Content Cell</td>
    <td>Content Cell</td>
    <td>Content Cell</td>
    <td>Content Cell</td>
  </tr>
  <tr>
    <td>Content Cell</td>
    <td>Content Cell</td>
    <td>Content Cell</td>
    <td>Content Cell</td>
  </tr>
  <tr>
    <td>Content Cell</td>
    <td>Content Cell</td>
    <td>Content Cell</td>
    <td>Content Cell</td>
  </tr>
</table>

Eine HTML Tabelle mit Kopf, Inhalt und Fuss.  

<table>  
    <thead>  
        <tr>  
          <th>Head</th>  
        </tr>  
    </thead>  
    <tbody>  
        <tr>  
          <td>Content Cell</td>  
          <td>Content Cell</td>  
          <td>Content Cell</td>  
          <td>Content Cell</td>  
        </tr>  
    </tbody>  
    <tfoot>  
        <tr>  
          <td>Foot</td>  
        </tr>  
    </tfoot>  
</table>  

Mit dem Element "colspan" können Zellen zu einer zusammengefasst werden.  

<table>  
    <thead>  
        <tr>  
          <th>Head</th>  
        </tr>  
    </thead>  
    <tbody>
        <tr>  
          <td>Content Cell</td>  
          <td>Content Cell</td>  
          <td>Content Cell</td>  
          <td>Content Cell</td>  
        </tr>    
        <tr>  
          <td colspan="3">Content Cell 1</td>  
          <td>Content Cell 4</td>  
        </tr>  
    </tbody>  
    <tfoot>  
        <tr>  
          <td>Foot</td>  
        </tr>  
    </tfoot>  
</table>  

Mit dem Element "rowspan" können Spalten zu einer zusammengefasst werden.  

<table>  
    <thead>  
        <tr>  
          <th>Head</th>  
        </tr>  
    </thead>  
    <tbody>
        <tr>  
          <td rowspan="2">Content Cell Row 1</td>  
          <td>Content Cell</td>  
          <td>Content Cell</td>  
          <td>Content Cell</td>  
        </tr>  
        <tr>  
          <td>Content Cell</td>  
          <td>Content Cell</td>  
          <td>Content Cell</td>  
          <td>Content Cell</td>  
        </tr>    
    </tbody>  
    <tfoot>  
        <tr>  
          <td>Foot</td>  
        </tr>  
    </tfoot>  
</table>  

## HTML mit CSS

#### Code

\<style type="text/css">  
\.tg  {border-collapse:collapse;border-spacing:0;}  
\.tg td{font-family:Arial, sans-serif;font-size:14px;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;border-color:black;}  
\.tg th{font-family:Arial, sans-serif;font-size:14px;font-weight:normal;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;border-color:black;}  
\.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}  
\</style>  
\<table class="tg">  
  \<tr>  
    \<th class="tg-0pky">First </th>  
    \<th class="tg-0pky">Second</th>  
    \<th class="tg-0pky">Third</th>  
    \<th class="tg-0pky">Fourth</th>  
  \</tr>  
  \<tr>  
    \<td class="tg-0pky">Content Cell</td>  
    \<td class="tg-0pky">Content Cell</td>  
    \<td class="tg-0pky">Content Cell</td>  
    \<td class="tg-0pky">Content Cell</td>  
  \</tr>  
  \<tr>  
    \<td class="tg-0pky"></td>  
    \<td class="tg-0pky"></td>  
    \<td class="tg-0pky"></td>  
    \<td class="tg-0pky"></td>  
  \</tr>  
  \<tr>  
    \<td class="tg-0pky"></td>  
    \<td class="tg-0pky"></td>  
    \<td class="tg-0pky"></td>  
    \<td class="tg-0pky"></td>  
  \</tr>  
  \<tr>  
    \<td class="tg-0pky"></td>  
    \<td class="tg-0pky"></td>  
    \<td class="tg-0pky"></td>  
    \<td class="tg-0pky"></td>  
  \</tr>  
\</table>  

#### Ausgabe

<style type="text/css">
.tg  {border-collapse:separate;border-spacing: 2em;}
.tg td{font-family:Arial, sans-serif;font-size:14px;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;border-color:black;}
</style>
<table class="tg">
  <tr>
    <th class="tg-13k7">First</th>
    <th class="tg-13k7">Second</th>
    <th class="tg-13k7">Third</th>
    <th class="tg-13k7">Fourth</th>
  </tr>
  <tr>
    <td class="tg-13k7">Content Cell</td>
    <td class="tg-13k7">Content Cell</td>
    <td class="tg-13k7">Content Cell</td>
    <td class="tg-13k7">Content Cell</td>
  </tr>
  <tr>
    <td class="tg-13k7">Content Cell</td>
    <td class="tg-13k7">Content Cell</td>
    <td class="tg-13k7">Content Cell</td>
    <td class="tg-13k7">Content Cell</td>
  </tr>
</table>

<style type="text/css">
</style>
<table class="tg">
  <tr>
    <th class="tg-13k7">First</th>
    <th class="tg-13k7">Second</th>
    <th class="tg-13k7">Third</th>
    <th class="tg-13k7">Fourth</th>
  </tr>
  <tr>
    <td class="tg-13k7">Content Cell</td>
    <td class="tg-13k7">Content Cell</td>
    <td class="tg-13k7">Content Cell</td>
    <td class="tg-13k7">Content Cell</td>
  </tr>
  <tr>
    <td class="tg-13k7">Content Cell</td>
    <td class="tg-13k7">Content Cell</td>
    <td class="tg-13k7">Content Cell</td>
    <td class="tg-13k7">Content Cell</td>
  </tr>
</table>

## Quellen  

1. [GitHub Help:  Organizing information with tables](https://help.github.com/en/articles/organizing-information-with-tables)  
2. [GitHub Help:  Organizing information with tables](https://help.github.com/en/articles/basic-writing-and-formatting-syntax)
3. [Tables Online Generator](https://www.tablesgenerator.com/html_tables)
