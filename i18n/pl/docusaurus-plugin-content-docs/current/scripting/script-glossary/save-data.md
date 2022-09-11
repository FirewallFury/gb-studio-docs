---
sidebar_position: 2
#
# This file is autogenerated. DO NOT MODIFY DIRECTLY
#
---

import ScriptEventPreview from '@site/src/components/ScriptEventPreview';

# Zapis gry

## Stan gry: wczytaj
Load the saved game data from the selected slot.
<ScriptEventPreview title={"Stan gry: wczytaj"} fields={[{"label":"Wczytaj dane gry z pamięci."},{"key":"saveSlot","label":"Zapisz plik","description":"The save slot to use.","type":"togglebuttons","options":[[0,"Plik 1","Zapisz plik 1"],[1,"Plik 2","Zapisz plik 2"],[2,"Plik 3","Zapisz plik 3"]],"allowNone":false,"defaultValue":0}]} />

- **Zapisz plik**: The save slot to use.  

## Stan gry: czyść
Remove any previously saved game data in the selected slot.
<ScriptEventPreview title={"Stan gry: czyść"} fields={[{"label":"Czyści wszystkie wcześniejsze zapisane stany gry z pamięci."},{"key":"saveSlot","label":"Zapisz plik","description":"The save slot to use.","type":"togglebuttons","options":[[0,"Plik 1","Zapisz plik 1"],[1,"Plik 2","Zapisz plik 2"],[2,"Plik 3","Zapisz plik 3"]],"allowNone":false,"defaultValue":0}]} />

- **Zapisz plik**: The save slot to use.  

## Stan gry: zapisz
Save the current game data into the selected slot.
<ScriptEventPreview title={"Stan gry: zapisz"} fields={[{"label":"Zapisuje aktualny stan gry do pamięci. Wymagany jest kardridż z baterią."},{"key":"saveSlot","label":"Zapisz plik","description":"The save slot to use.","type":"togglebuttons","options":[[0,"Plik 1","Zapisz plik 1"],[1,"Plik 2","Zapisz plik 2"],[2,"Plik 3","Zapisz plik 3"]],"allowNone":false,"defaultValue":0},{"key":"__scriptTabs","type":"tabs","defaultValue":"save","values":{"save":"Przy zapisie"}},{"key":"true","label":"Przy zapisie","description":"A script to run after the save is completed. This won't be run on game load so you can use it show a 'Save Was Successful' message.","type":"events"}]} />

- **Zapisz plik**: The save slot to use.  
- **Przy zapisie**: A script to run after the save is completed. This won't be run on game load so you can use it show a 'Save Was Successful' message.  

## Warunek: stan gry zapisano
Conditionally run part of the script if save data is present within the specified save slot.
<ScriptEventPreview title={"Warunek: stan gry zapisano"} fields={[{"key":"saveSlot","label":"Zapisz plik","description":"The save slot to use.","type":"togglebuttons","options":[[0,"Plik 1","Zapisz plik 1"],[1,"Plik 2","Zapisz plik 2"],[2,"Plik 3","Zapisz plik 3"]],"allowNone":false,"defaultValue":0},{"label":"Uruchom, gdy gracz wykonał zapis gry."},{"key":"true","label":"Prawda","description":"The script to run if the condition is true.","type":"events"},{"key":"__collapseElse","label":"W innym wypadku","type":"collapsable","defaultValue":true,"conditions":[{"key":"__disableElse","ne":true}]},{"key":"false","label":"Fałsz","description":"The script to run if the condition is false.","conditions":[{"key":"__collapseElse","ne":true},{"key":"__disableElse","ne":true}],"type":"events"}]} />

- **Zapisz plik**: The save slot to use.  
- **Prawda**: The script to run if the condition is true.  
- **Fałsz**: The script to run if the condition is false.  

## Zmienna: wartość z zapisu do zmiennej
Read a variable's value from a specified save slot and store it in a variable.
<ScriptEventPreview title={"Zmienna: wartość z zapisu do zmiennej"} fields={[{"key":"variableDest","label":"Ustaw zmienną","description":"The variable to update.","type":"variable","defaultValue":"LAST_VARIABLE"},{"type":"group","fields":[{"key":"variableSource","label":"Dodaj do zmiennej","description":"The variable to read the value of.","type":"variable","defaultValue":"LAST_VARIABLE"},{"key":"saveSlot","label":"Zapisz z pliku","description":"The save slot to use.","type":"togglebuttons","options":[[0,"Plik 1","Zapisz plik 1"],[1,"Plik 2","Zapisz plik 2"],[2,"Plik 3","Zapisz plik 3"]],"allowNone":false,"defaultValue":0}]}]} />

- **Ustaw zmienną**: The variable to update.  
- **Dodaj do zmiennej**: The variable to read the value of.  
- **Zapisz z pliku**: The save slot to use.  
