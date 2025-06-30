# ****ZFB -- Zero Frame Buffer****

**ZFB** ist eine minimalistische Game Engine, entwickelt von der
GitHub-Gruppe ****[**The-Sigmas**](https://github.com/The-Sigmas)****.\
Was ZFB von anderen Game Engines unterscheidet**** ist, dass sie ****
**direkt auf den Framebuffer** zu****greift**** ganz ohne
Fenster-Manager, Grafikserver oder GPU-Abstraktionen.****

### Plattformverhalten:

-   **Linux:** Direkter Zugriff auf den echten Kernel-Framebuffer
    (*/dev/fb0*), um die Grafikausgabe pixelgenau zu steuern.
-   **Windows:** Da der Windows-Kernel keinen direkten
    Framebuffer-Zugriff erlaubt, verwendet ZFB eine **Simulation**, die
    sich wie ein echter Framebuffer verhält.

Dadurch ist ZFB ****ultraleicht, schnell und unabhängig von grossen
Grafik-Stacks**** -- perfekt für Retro-Style-Projekte, Tools, Lernzwecke
oder Low-Level-Games.

## ****Ziel der Engine****

****Das Ziel von **ZFB** ist es, **so performant wie möglich** zu sein
**ohne externe Abhängigkeiten** (keine Libraries, keine Frameworks). Die
Engine setzt vollständig auf **Standard-C** und nutzt
ausschlie****ss****lich **Systemfunktionen**, wodurch sie besonders
leichtgewichtig und portabel bleibt.****

Ausserdem ist ZFB bewusst ****modular aufgebaut****, sodass Entwickler
einzelne Komponenten ****einfach erweitern oder austauschen**** können ,
ohne tief ins System eingreifen zu müssen.
