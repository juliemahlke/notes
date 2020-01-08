# HTML

1. **Wann `aside` innerhalb von `article`, wann außerhalb?**<br>
**In** `article` wenn innerhalb eines Artikels ein bestimmter Part abgegrenzt werden soll. Z.B. der Autor eines Artikels, das Erstellungsdatum etc. **Außerhalb** Wenn im Websitetemplate, also im Grundaufbau z.B. neben dem `main` eine Sidebar eingebunden werden soll. 

2. **Was kommt in `main` rein? Wie oft darf man main pro Seite verwenden?**<br>
In `main` kommt der gesammte Content-Bereich rein. Also alle Inhalte zwischen `header`und `footer`. Ebenso wie `header`und `footer`darf `main`nur ein mal pro Seite verwendet werden.

3. **Wann ist div geeigneter als section?**<br>
Wenn ein allgemeiner Container für Stylingzwecke benötigt wird.

4. **Wann verwendet man b und wann strong? Wann i und wann em?**
    - **`strong`** verwendet man wenn man für sehr wichtige Textabschnitte, z.B. Warnungen, Hinweise
    - **`b`** verwendet man um die Aufmerksamkeit auf bestimmten Text zu lenken, ohne auf eine höhere Wichtigkeit hinzuweisen
    - **`i`** für Text, der aus Gründen der Lesbarkeit von der normalen Form abweicht. Dies wäre ein Textbereich mit einer anderen semantischen Bedeutung als der umgebende Text
    - **`em`** verwendet man um ein Wort/eine Textpassage zu betonen
<br><br>

5. **Wie baut man eine figure mit einem Bild und Text auf?**
```
<figure>
    <img src="/media/examples/elephant-660-480.jpg"
         alt="Elephant at sunset">
    <figcaption>An elephant at sunset</figcaption>
</figure>
```

6. **Wofür steht dl, dd und dt**
    - **`<dl>`** Beschreibungsliste
    - **`<dt>`** Gibt einen Begriff in einer Beschreibungs- oder Definitionsliste an
    - **`<dd>`** Das Element enthält die Beschreibung, Definition oder den Wert für den vorhergehenden Begriff (`<dt>`) in einer Beschreibungsliste (`<dl>`).

```
<dl>
    <dt>Beast of Bodmin</dt>
    <dd>A large feline inhabiting Bodmin Moor.</dd>

    <dt>Morgawr</dt>
    <dd>A sea serpent.</dd>

    <dt>Owlman</dt>
    <dd>A giant owl-like creature.</dd>
</dl>
```

7. **Was sind 3 void Elemente, die du kennst?**
    - input
    - img
    - br


- **Wofür wird small verwendet?**<br>
Für kleine unbedeutende Texte, z.B. AGBs oder Copyright-Zeichen im footer einer Website

- **Was ist der Unterschied zwischen dem img- und dem picture-Element?**
Mit `<img>`wird ein einfaches Bild eingebunden. Ein `<picture` enthält null oder mehr <source> -Elemente und ein <img> -Element, um alternative Versionen eines Bildes für verschiedene Anzeige- / Geräteszenarien anzubieten. Es gruppiert also mehrere Bildelemente.

- **Welche 5 input-types kennst du neben `<input type="text">`?**
    - number
    - search
    - email
    - checkbox
    - radio 

- **Was macht man mit select und option?**
Ein select enthält mehrere options. Jede Menüoption wird durch ein `<option>` -Element definiert, das in `<select>` verschachtelt ist. Jedes `<option>` -Element sollte über ein value-Attribut verfügen, das den Datenwert enthält, der bei Auswahl dieser Option an den Server gesendet werden soll (default: enthaltener Text). Man kann einem `<option>` -Element ein ausgewähltes Attribut hinzufügen, damit es beim ersten Laden der Seite standardmäßig ausgewählt wird.`<option>` -Elemente können in `<optgroup>` verschachtelt werden, um Optionsgruppen in der Dropdown-Liste zu erstellen.

```
<label>Please choose one or more pets:
  <select name="pets" multiple size="4">
    <optgroup label="4-legged pets">
      <option value="dog">Dog</option>
      <option value="cat">Cat</option>
      <option value="hamster" disabled>Hamster</option>
    </optgroup>
    <optgroup label="Flying pets">
      <option value="parrot">Parrot</option>
      <option value="macaw">Macaw</option>
      <option value="albatross">Albatross</option>
    </optgroup>
  </select>
</label>
```