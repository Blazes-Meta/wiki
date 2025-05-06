# Aliasse

Mit Befehls-Aliassen können einfach Befehle hinzugefügt werden, die dann als Alternative für einen anderen Befehl fungieren.

{% hint style="info" %}
Aliasse werden in `commands.yml` definiert. Dort können allerdings keine Berechtigungen verändert werden. Wenn der umschriebene Befehl nur von Operatoren benutzt werden kann, gilt das auch für den Alias.
{% endhint %}

## Beispiele

### Alternative hinzufügen

```yaml
aliases:
  sleeppls:
  - function st:broadcast/sleep
```

fügt den Befehl `/sleeppls` hinzu, der eine bestimmte Funktion ausführt.

### Befehl entfernen

```yaml
aliases:
    summon:
    - []
```

entfernt den Befehl `/summon` aus der Befehlsliste

### Befehl ersetzen

```yaml
aliases:
    icanhasversion:
    - "bukkit:version"
    version:
    - []
```

fügt den Befehl `/icanhasbukkit` hinzu, der `bukkit:version` ausführt und entfernt `version` aus der Befehlsliste

### Verwendung von Argumenten

```yaml
aliases:
    time:
    - "bukkit:time $1-"
```

überschreibt Minecrafts `/time` Befehl und nutzt den von Bukkit mit dem ersten Argument

{% hint style="warning" %}
Der Befehl kann so zwar genutzt werden, im Chat findet allerdings keine Syntaxkontrolle mehr statt und man erhält keine Vorschläge mehr
{% endhint %}



