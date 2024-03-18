# Klausur 2023 DHBW HDH

## Erkläre in eigenen Worten:
   ### Welche Vorteile ein Kubernetes Deployment gegenüber einem Kubernetes Pod hat **(2 Punkte)**

Automatische Verwaltung
   Ein Deployment kümmert sich um die automatische Erstellung, Löschung und Aktualisierung der Pods. 
   Wenn man die Version aktualisieren möchte, kann das Deployment neue Pods mit der neuen Version starten und die alten nach und nach entfernen, ohne dass Downtime entsteht. 
   Ein einzelner Pod bietet diese Art von Verwaltung oder Selbstheilung nicht.

Skalierung
   Man kann einfach Replikate erhöhen und verringern, je nachdem wie viele man benötigt.
   inzelne Pods kann man nicht scalen.


   ### Wofür ein Kubernetes Service gut ist **(2 Punkte)**

   Beständige Netzwerkadresse
    Man bekommt eine beständige Adresse für den Zugriff auf andere Pods, auch bei Neustarts oder Ersetzungen.

   Lastverteilung
    Ein Service verteilt eingehende Anfragen automatisch auf alle Pods nach dem Round Robin Prinzip.
    So werden die Pods nicht überlastet.



   ### Mehrere Wege wie man eine Kubernetes Anwendung von außen erreichen kann **(3 Punkte)**

   NodePort
     Zugriff auf einen Service von außerhalb des Kubernetes Clusters, indem ein spezifischer Port auf jedem Node im Cluster geöffnet wird

   LoadBalancer
     Einen externen Load Balancer der den Verkehr auf die Kubernetes Services verteilt
      
   Ingress
    Für das Routing und die Verwaltung des externen Zugriffs auf deine Services innerhalb des Kubernetes Clusters
    Durch Routing Regeln steuerbar



## Zusatzaufgabe:

Definiere einen Kubernetes Job **(2 Punkte)**
Siehe kurbernetes\Job.yaml 
