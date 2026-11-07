<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="docs/brand/svg/hunter-prey-logo-on-dark.svg">
    <img src="docs/brand/svg/hunter-prey-logo-on-light.svg" alt="Hunter Prey Game" width="320">
  </picture>
</p>

<h1 align="center">Dodge the green circles. Count the seconds.</h1>

<p align="center">
  A first game written in 2016, archived as it was.<br>
  <b>Java Swing. Five hunters. One red square to keep alive.</b>
</p>

<p align="center">
  <img alt="Status: archived" src="https://img.shields.io/badge/status-archived-9E3B2E?style=flat-square">
  <img alt="Written in 2016" src="https://img.shields.io/badge/written-2016-1E2A38?style=flat-square">
  <img alt="Java 8" src="https://img.shields.io/badge/Java-8-ED8B00?style=flat-square&logo=openjdk&logoColor=white">
  <img alt="Five hunters" src="https://img.shields.io/badge/hunters-5-1E2A38?style=flat-square">
  <a href="https://github.com/mertkayacs/HunterPreyGame"><img alt="GitHub stars" src="https://img.shields.io/github/stars/mertkayacs/HunterPreyGame?style=flat-square&logo=github&color=C4A772"></a>
</p>

<p align="center">
  <a href="#quick-start"><img alt="Play it" src="https://img.shields.io/badge/Play%20it-9E3B2E?style=for-the-badge&logo=data%3Aimage%2Fsvg%2Bxml%3Bbase64%2CPHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgd2lkdGg9IjI0IiBoZWlnaHQ9IjI0Ij48cGF0aCBmaWxsPSJub25lIiBzdHJva2U9IiNmZmZmZmYiIHN0cm9rZS1saW5lY2FwPSJyb3VuZCIgc3Ryb2tlLWxpbmVqb2luPSJyb3VuZCIgc3Ryb2tlLXdpZHRoPSIyIiBkPSJNNSA1YTIgMiAwIDAgMSAzLjAwOC0xLjcyOGwxMS45OTcgNi45OThhMiAyIDAgMCAxIC4wMDMgMy40NThsLTEyIDdBMiAyIDAgMCAxIDUgMTl6Ii8%2BPC9zdmc%2B&logoColor=white"></a>
  <a href="src/Map.java"><img alt="Source" src="https://img.shields.io/badge/Source-1E2A38?style=for-the-badge&logo=data%3Aimage%2Fsvg%2Bxml%3Bbase64%2CPHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgd2lkdGg9IjI0IiBoZWlnaHQ9IjI0Ij48ZyBmaWxsPSJub25lIiBzdHJva2U9IiNmZmZmZmYiIHN0cm9rZS1saW5lY2FwPSJyb3VuZCIgc3Ryb2tlLWxpbmVqb2luPSJyb3VuZCIgc3Ryb2tlLXdpZHRoPSIyIj48cGF0aCBkPSJtMTYgMTggNi02LTYtNiIvPjxwYXRoIGQ9Im04IDYtNiA2IDYgNiIvPjwvZz48L3N2Zz4%3D&logoColor=white"></a>
  <a href="https://mertkayacs.com/?utm_source=github&utm_medium=readme&utm_campaign=HunterPreyGame-repo&utm_content=portfolio-badge"><img alt="Portfolio" src="https://img.shields.io/badge/Portfolio-1E2A38?style=for-the-badge&logo=data%3Aimage%2Fsvg%2Bxml%3Bbase64%2CPHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgd2lkdGg9IjI0IiBoZWlnaHQ9IjI0Ij48ZyBmaWxsPSJub25lIiBzdHJva2U9IiNmZmZmZmYiIHN0cm9rZS1saW5lY2FwPSJyb3VuZCIgc3Ryb2tlLWxpbmVqb2luPSJyb3VuZCIgc3Ryb2tlLXdpZHRoPSIyIj48Y2lyY2xlIGN4PSIxMiIgY3k9IjEyIiByPSIxMCIvPjxwYXRoIGQ9Ik0xMiAyYTE0LjUgMTQuNSAwIDAgMCAwIDIwYTE0LjUgMTQuNSAwIDAgMCAwLTIwTTIgMTJoMjAiLz48L2c%2BPC9zdmc%2B&logoColor=white"></a>
</p>

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="docs/assets/readme/hero-dark.webp">
    <img src="docs/assets/readme/hero-light.webp" alt="The Hunter Prey Game window: a black playfield with five green circles and a small red square, and the title bar reading &quot;HunterPreyGame v2.0 - 7 Seconds passed.&quot;" width="960">
  </picture>
</p>

Hunter Prey Game is a small survival game in Java Swing with no framework. You steer a red square while five green circles drift around the board in random directions, and the window title counts the seconds you stay alive. When a hunter touches you, the title shows how long you lived and the window closes after ten seconds. The game waits on a thread between steps and does not use intersects().

---

## Why Hunter Prey Game

The whole game is four Java files.

|  |  |
|---|---|
| <img src="docs/assets/readme/icons/keyboard.svg" width="18" height="18" alt=""> **Two ways to move** | Use W, A, S and D or the arrow keys. The key handling is in [Map.java](src/Map.java). |
| <img src="docs/assets/readme/icons/timer.svg" width="18" height="18" alt=""> **A live score** | The title bar shows the seconds you have survived and updates once per second. |
| <img src="docs/assets/readme/icons/package.svg" width="18" height="18" alt=""> **Plain Java** | No framework and no dependencies. The Eclipse project targets Java 8. |

## A quick tour

<table>
  <tr>
    <td width="50%" valign="top">
      <picture>
        <source media="(prefers-color-scheme: dark)" srcset="docs/assets/readme/tour/start-dark.webp">
        <img src="docs/assets/readme/tour/start-light.webp" alt="The game window with five green circles and a red square, titled with the seconds passed">
      </picture>
      <h3>Round start</h3>
      Five hunters drift around the board while the title bar counts seconds. The prey is the small red square.
    </td>
    <td width="50%" valign="top">
      <picture>
        <source media="(prefers-color-scheme: dark)" srcset="docs/assets/readme/tour/moved-dark.webp">
        <img src="docs/assets/readme/tour/moved-light.webp" alt="The game window a few seconds later with the red square moved">
      </picture>
      <h3>Moving the prey</h3>
      W, A, S, D or the arrow keys move the red square.
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <picture>
        <source media="(prefers-color-scheme: dark)" srcset="docs/assets/readme/tour/over-dark.webp">
        <img src="docs/assets/readme/tour/over-light.webp" alt="The game window with the title &quot;Game Over - Lived 32 secs -Closing in 10 secs&quot;">
      </picture>
      <h3>Game over</h3>
      When a hunter touches the prey, the title shows how long you lived and the window closes ten seconds later.
    </td>
    <td width="50%" valign="top">
      <picture>
        <source media="(prefers-color-scheme: dark)" srcset="docs/assets/readme/tour/code-dark.webp">
        <img src="docs/assets/readme/tour/code-light.webp" alt="Code card showing changeHunterDirection in Game.java">
      </picture>
      <h3>Random hunters</h3>
      Every few steps each hunter gets a new random direction out of eight.
    </td>
  </tr>
</table>

<p align="center"><sub>Captured from the running game on a virtual display. The window frames are drawn by Swing because that display has no window manager.</sub></p>

## Features

**Gameplay**

- Five hunters move in random directions around a single prey.
- The window closes itself ten seconds after the game ends.

**Code**

- Map.java holds the window, the game loop and the keys.
- Game.java draws the board and detects when a hunter touches you.
- Hunter.java and Prey.java hold the two kinds of piece.

## Quick start

```sh
cd src
javac *.java
java Map
```

### Requirements

- A Java JDK. The Eclipse project settings use Java 8.

## FAQ

<details>
<summary><b>How do I move?</b></summary>

With W, A, S and D or the arrow keys.
</details>

<details>
<summary><b>How long does a round last?</b></summary>

Until a hunter touches you. The title bar counts the seconds, then the window closes ten seconds after the game ends.
</details>

<details>
<summary><b>Is this coursework?</b></summary>

No. It is a first personal game from 2016 that was uploaded in 2019.
</details>

If Hunter Prey Game is useful to you, a ⭐ helps other people find it.

Photos behind the screenshots are credited in [docs/assets/readme/CREDITS.md](docs/assets/readme/CREDITS.md).

[![views](https://hits.sh/github.com/mertkayacs/HunterPreyGame.svg?view=today-total&style=flat-square&label=views&color=9E3B2E&labelColor=1E2A38)](https://github.com/mertkayacs/HunterPreyGame)
