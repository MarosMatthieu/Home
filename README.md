# Home
Regroupe tout le code dont j'ai besoin en un seul projet

# Code de lancement oracle
    @echo off
    echo shutdown immediate>"oracle.sql"
    echo. startup open>>"oracle.sql"
    echo. exit>>"oracle.sql"

    sqlplus system/estran as sysdba @oracle.sql

    del /s oracle.sql
    cls

    echo Operation reussie
    pause
