---
title: "SQM 16/24: Mutationsabdeckung [Crashkurs Softwarequalität] [eng sub]"
date: 2024-01-31T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/WYWSv_PucHc/maxresdefault.jpg"
  alt: "SQM 16/24: Mutationsabdeckung [Crashkurs Softwarequalität] [eng sub]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=WYWSv_PucHc](https://www.youtube.com/watch?v=WYWSv_PucHc)

## Zusammenfassung
In dieser umfassenden Vorlesung aus dem Crashkurs Software Quality Metrics (SQM) kritisiert Yegor Bugayenko systematisch das Vertrauen der Softwareindustrie auf traditionelle Metriken zur Codeabdeckung, wie etwa die Zeilen- und Zweigabdeckung. Er argumentiert, dass diese herkömmlichen Metriken grundlegend fehlerhaft sind, da sie lediglich die Ausführung des Codes verfolgen und keine echte Verifizierung der Logik bieten. So kann eine Testsuite beispielsweise problemlos eine 100-prozentige Zeilenabdeckung erreichen, indem sie alle Codepfade ausführt, ohne auch nur eine einzige Assertion (Zusicherung) zu enthalten, was ein trügerisches Gefühl der Sicherheit vermittelt. Um dieses kritische Defizit zu beheben, stellt Bugayenko die Mutationsabdeckung (Mutation Testing) als eine wesentlich strengere und zuverlässigere Alternative zur Bewertung der Qualität von Testsuites vor.

Die Methodik des Mutation Testing besteht darin, absichtlich kleine, künstliche Fehler – sogenannte „Mutanten“ – in den Quellcode einzuschleusen. Diese Mutationen können das Ändern mathematischer Operatoren, das Anpassen relationaler Operatoren oder das Umkehren boolescher Logik umfassen. Das Ziel ist es, die Reaktion der Testsuite zu beobachten. Wenn als Reaktion auf den injizierten Fehler mindestens ein Test fehlschlägt, gilt der Mutant als „getötet“, was bedeutet, dass die Tests das Verhalten des Codes effektiv validieren. Wenn jedoch alle Tests trotz der Mutation weiterhin erfolgreich durchlaufen, „überlebt“ der Mutant. Ein überlebender Mutant deckt einen blinden Fleck in der Testsuite auf, an dem der Code zwar ausgeführt, sein spezifisches Verhalten jedoch nicht genau verifiziert wird. Obwohl Mutation Testing aufgrund der hohen Anzahl erforderlicher Testausführungen rechenintensiv ist, betont Bugayenko, dass es äußerst nützliches Feedback und einen objektiven „Mutations-Score“ liefert, der für Entwickler extrem schwer zu manipulieren ist und letztlich zu einer deutlich höheren Softwarezuverlässigkeit führt.

## Kernaussagen
1. „Traditionelle Codeabdeckung misst nur die Ausführung, nicht die Verifizierung – Tests können ohne eine einzige Assertion erfolgreich sein.“
2. „Ein getöteter Mutant beweist, dass Ihre Testsuite die Logik und das Verhalten des Codes aktiv validiert, anstatt ihn nur auszuführen.“
3. „Der Mutations-Score bietet eine objektive, manipulationssichere Metrik, die für Entwickler extrem schwer zu verfälschen ist.“
4. „Obwohl rechenintensiv, liefert Mutation Testing äußerst nützliches Feedback, indem es genaue blinde Flecken in der Testverifizierung aufdeckt.“

## Relevanz: 5/5
Hochrelevant für Softwareentwicklung, Testing und Teamführung, da es fundierte QA-Praktiken fördert und eine konkrete Lösung für das weit verbreitete Problem der Manipulation von Testmetriken bietet.
