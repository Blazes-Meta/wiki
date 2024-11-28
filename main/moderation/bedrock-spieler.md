---
icon: circle-nodes
---

# Bedrock Spieler

### `/fwhitelist` Error Fix

{% hint style="success" %}
Fix: XUID whitelisten, siehe Link und Tabelle unten
{% endhint %}

Es kommt gerne mal vor, dass Geyser beim `/fwhitelist`-Befehl kein Ergebnis findet. Alternativ kann man die formatierte XUID des XBOX Live Acounts whitelisten

{% embed url="https://www.cxkes.me/xbox/xuid" %}

<table><thead><tr><th width="177">XBOX Live Name</th><th width="195">XUID (dezimal)</th><th>XUID (formatiert)</th></tr></thead><tbody><tr><td>martula11</td><td><code>2535439236128288</code></td><td><code>00000000-0000-0000-2535-439236128288</code></td></tr></tbody></table>

### `/lp user` mit Bedrock Spielern Error Fix

{% hint style="success" %}
Fix: Spielernamen in Anführungszeichen setzen\
Fix: LuckPerms Editor nutzen
{% endhint %}

LuckPerms' `user`-Subcommand überprüft - wenn `allow-invalid-usernames` in den LuckPerms Configs deaktiviert ist, ob das angegebene Argument ein gültiger Minecraft Spielername oder eine gültige UUID ist, was bedeutet, dass bei Bedrock-Spielern ein Fehler zurückgemeldet wird. Als funktionierende Alternative können die Nodes des Spielers über den Editor (`/lp editor`) bearbeitet werden. Dem GeyserMC-Wiki nach kann man den Spielernamen auch in Anführungszeichen setzen.
