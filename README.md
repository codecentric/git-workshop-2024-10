# Git Workshop 2024-10-28

## Basics

- vorhandenes git-repository auschecken mit
  
  - `git clone git@github.com:codecentric/git-workshop-2024-10.git` oder
  - `git clone https://github.com/codecentric/git-workshop-2024-10.git`

- Grundlegende Konfiguration:
  
  - Eigenen Namen und Email konfigurieren:
    
    - `git config --global user.name "Max Mustermann"`
    
    - `git config --global user.email max.mustermann@example.com`
  
  - Pull immer mit merge:
    
    - `git config --global pull.rebase false`
  - conflict resolutions merken und ggf wiederverwenden:
    - `git config --global rerere.enabled true`

- Neue Datei erstellen, dann hinzufügen:
  
  - `git add <dateiname>`

- Commit erstellen:
  
  - `git commit` oder
  
  - `git commit -m "Beschreibung"`

- Commits veröffentlichen:
  
  - `git push`

- Änderungen von remote holen und mergen:
  
  - `git pull`



- `HEAD` ist das, was ich gerade lokal ausgecheckt habe
