sequenceDiagram

  Participant A:Repo A
  Participant B:Repo B
  Participant G:GitHub (pour les actions)
  
  A->B: Notification de changement
  B->B: Déclenchement de l'action GitHub
  B->G: Déploiement du site
