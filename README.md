# Phishing_risk_analysis

*Zusammenfassung d. Ergebnisse*
Anomale TLS-Verbindungen unterscheiden sich deutlich von normalen Verbindungen, insbesondere hinsichtlich der Verbindungsdauer und übertragenen Datenmenge. Während normale Sessions im Mittel sehr kurze Dauer aufweisen (~6 ms), zeigen anomale Sessions eine stark erhöhte Dauer (~326 ms). Gleichzeitig ist das übertragene Datenvolumen bei Anomalien deutlich reduziert. Diese Muster deuten darauf hin, dass anomale Verbindungen häufiger ineffizient oder unvollständig verlaufen. 

 

Die logistische Regression zeigte, dass die Dauer der Verbindung ein signifikanter Prädiktor für anomale TLS-Sessions ist (β = 0.045, p < .001). Längere Verbindungen gingen mit einer erhöhten Wahrscheinlichkeit für Anomalien einher. 

Zudem war die Länge des Server-Records negativ mit der Anomaliewahrscheinlichkeit assoziiert (β = -0.105, p < .001), was darauf hindeutet, dass kürzere Server-Antworten häufiger in anomalen Verbindungen auftreten. 

Das Gesamtmodell war signifikant und erklärte einen substantiellen Anteil der Varianz (Pseudo-R² = 0.556). 

 

Die logistische Regression zeigte, dass die Verbindungsdauer ein signifikanter Prädiktor für anomale TLS-Sessions ist. Eine Erhöhung der Dauer um eine Einheit ging mit einer etwa 4.6%igen Zunahme der Odds für eine Anomalie einher (OR = 1.046). 

Darüber hinaus war die Länge des Server-Records negativ mit der Anomaliewahrscheinlichkeit assoziiert (OR = 0.90), was darauf hinweist, dass kürzere Server-Antworten häufiger in anomalen Verbindungen auftreten. 

Der Einfluss der übertragenen Datenmenge war hingegen vergleichsweise gering. 

 

Die Interaktion zwischen Verbindungsdauer und Datenvolumen war signifikant (β = 0.0000385, p < .001), was darauf hindeutet, dass sich beide Variablen in ihrem Einfluss auf die Anomaliewahrscheinlichkeit gegenseitig verstärken. Allerdings führte die Aufnahme des Interaktionsterms zu keiner Verbesserung der Modellgüte, was darauf hinweist, dass der zusätzliche Erklärungswert begrenzt ist. 

 

Mit zunehmender Länge des Server-Records nimmt die Wahrscheinlichkeit für eine anomale Verbindung deutlich ab. 
