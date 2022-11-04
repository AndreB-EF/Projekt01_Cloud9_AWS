# Projekt01_Cloud9_AWS
Cloud9_AWS
# Git Repository lokal erstellen

https://eu-central-1.console.aws.amazon.com/ec2/home?region=eu-central-1#ConnectToInstance:instanceId=i-0144cfa093501fb33

## Projekt Umgebung vorbereiten


#### Erstellen Sie ein Vezeichnis mit dem Name Projekt1

    cd
    mkdir Projekt1

#### Dateien und Verzeichnisse fuer das Projekt "Statische Webseite"

    touch index.html style.css backend.py 
    mkdir Secret
    cd Secret
    touch Geheimnisse.txt
    cd ..
    mkdir Bilder
    cd Bilder
    touch Bild1.jpg Bild2.jpg Bild3.jpg Bild1.png Bild2.png
    cd ..
    touch .gitignore

#### Falls dass Sie sensibel Daten Verstecken wollen, schreiben Sie welche in .gitignore File und speicher die Aenderungen

    nano .gitignore

Code-Blocke

    Secret/
    Bilder/*.png

####SSH anmelden

    chmod 400 vw-vm-key2.pem
    kitty +kitten ssh -i "vm-key.pem" ubuntu@ABCDEFGH...eu-central-1.compute.amazonaws.com  

    tmux

###SSH Key mit Bash erstellen

    ssh-keygen
    cat .ssh/id_rsa.pub

### SSH key aus der bash mit Github verknüpfen

    ssh -T git@github.com
    git remote add origin git@github.com:GIT-PROFILNAME/REPOSITORY-NAME.git

#### Git Umgebung vorbereiten

    git config --global user.name "Name Nachname"
    git config --global user.email "valid-email"

#### git Kontrollversionierung initialisiren

    git init

#### From Working Area nach Stagin Area nach Repositoty

    git status
    git add -A
    git commit -m "Erstes Commit"
    git status
    
### well known shortcuts

## install tree 

    sudo yum install tree 		
    sudo apt install tree

## gliederung inhalt

    tree 

## inhalt mit versteckten dateien

    ls -lah

## directory löschen

    rmdir 				

## file löschen

    rm -rf gitingor 		

## file umbenennen

    mv gitingore .gitignore 
