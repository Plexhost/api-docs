---
description: >-
  Indbyggede Placeholders kan bruges overalt i GUI's hvor at et Bande objekt er
  tilstede.
---

# Indbygget Placeholders

**Placeholder:** \<placeholder>

<table><thead><tr><th width="275.1757214648392">Placeholder</th><th width="242.90025867747383">Beskrivelse</th><th>Eksempel</th></tr></thead><tbody><tr><td><code>&#x3C;name></code><br><code>&#x3C;name_upper></code><br><code>&#x3C;name_lower></code><br><code>&#x3C;name_capitalized></code></td><td>Viser bandens navn.</td><td>-</td></tr><tr><td><code>&#x3C;id></code><br><code>&#x3C;level></code><br><code>&#x3C;bank></code><br><code>&#x3C;owner></code><br><code>&#x3C;created></code><br><code>&#x3C;lastseen></code></td><td>Viser bandens id.<br>Viser bandens level.<br>Viser bandens bank.<br>Viser bandens ejer (navn)<br>Viser bandens oprettelse.<br>Viser bandens sidst set.</td><td>-</td></tr><tr><td></td><td></td><td></td></tr><tr><td><code>&#x3C;stat_{stat}></code></td><td>Viser en bandens stat.</td><td><code>&#x3C;stat_kills></code></td></tr><tr><td><code>&#x3C;amount_{type}></code></td><td>Viser antallet af henholdsvis,<br><code>members</code>, <code>allies</code>, <code>rivals_own</code>, <code>rivals_against</code></td><td><code>&#x3C;amount_members></code><br><code>&#x3C;amount_rivals_own></code></td></tr><tr><td><code>&#x3C;max_{type}></code></td><td>Viser max af henholdsvis,<br><code>members</code>, <code>allies</code>, <code>rivals</code></td><td><code>&#x3C;max_allies></code></td></tr><tr><td><code>&#x3C;permission_{type}></code></td><td>Viser hvilken rank man mindst skal være for en permission.</td><td><code>&#x3C;permission_invitations></code></td></tr><tr><td><code>&#x3C;shop_{type}></code></td><td>Viser antallet af et af shop itemsne: <br><code>bandeskade</code>, <code>allyskade</code></td><td></td></tr></tbody></table>

