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

- Neue Datei erstellen oder ändern, dann hinzufügen:
  
  - `git add <dateiname>`
  - `git add -p` "patch mode", einzelne Änderungen werden angezeigt und können hinzugefügt oder ignoriert werden

- Commit erstellen:
  
  - `git commit` oder
  
  - `git commit -m "Beschreibung"`

- Commits veröffentlichen:
  
  - `git push`
  
  - remote-tracking dabei aktivieren für den aktuellen Branch
    
    - `git push -u origin HEAD`

- Änderungen von remote holen und mergen:
  
  - `git pull`

- `HEAD` ist das, was ich gerade lokal ausgecheckt habe

- Historie anzeigen:
  
  - `git log`
  - `git log --graph --pretty=oneline`
    - Alias anlegen:
      - `git config alias.logg "log --graph --pretty=oneline"`

- mergen mit potentiell "fast forward" oder merge commit
  
  - `git merge <anderer branch>`

- mergen mit squash (alle Änderungen in einen neuen Commit packen)
  
  - `git merge --squash <anderer branch>`
    `git commit`

- rebase um den branch von einem neueren punkt abzweigen zu lassen
  
  - `git switch <anderer branch>`
    `git rebase <zielbranch>` (also z.B. `git rebase main`)
    `git switch <zielbranch>`
    `git merge <anderer branch>`
    

- Alle lokalen Aktionen sehen mit `git reflog`

- einzelnen Commit auschecken und anschauen `git checkout <commit-id>`

- Branch auf einen anderen Stand zurücksetzen: `git reset --hard <commit-id>`

- 
