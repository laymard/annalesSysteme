# Cours

## Comment le systeme détermine la réponse à un signal donné ?
Chaque signal est identifié. Il est associé à un "handler" chargé de son traitement ( un handler est formé par défaut). Entre chaque instruction, les éventuels signaux reçus sontexaminés et les handler associé exécutés.

## b Que signifie qu'un processus est arriere plan ? Le processus peut-il changer de plan d'execution ?

Un processus en arrière plan est un processus maintenue en vie par le systeme. Un processus est maintenue en arriere plan lors de son exécution à l'aide de "commande&" et peut etre ramené au 1er plan à l'aide de "fg % job".

Note Marin : un procesuss ne Arriere plan de monopolise pas le terminal.

## c

pipe anoynme, pas de réference possible en dehors de là ou on la crée. Les informations qu'il crée  n'ont de ens que dans ce procesuss
si on fork avec le meme pipe, le pere et le fils ont accès au pipe


## d

Sa fait référence à des périphériques où on peut acceder à n'importe quelle donnée sur le périphériques
Périf sur lequel on peut lire/ecrire ne donnée à n'importe quel emplacement.

opposition à des périférique qui gerent des flux.

clé usb , DDE,

## e Que sont les déroutements ?

quand l'OS prend la main sur l'éctuion du programme pour gérer un évenement issue du programme tel qu'une erreur, une exception

ex : une div par 0, stack overflow ( trop de flow mon gars !! )

## f
1
```c

int pid=fork();
  if(pid==0){
    //code du fils
  }else {
    // code du pere
  }
```
##

```c
getppid(); //donne le pid du process pere

```

## g

* sauvegarder les chgts éventuels si la page à retirer a été notifiée
* Maj de a table des pages
* charger la nouvelle page

## h DMA ?

* gere les transferts des données du disque à la RAM à la place du CPU, celui ci peut donc effectuer d'autre taches en meme temps

## i

Les threads ont une zone mémoire réduite (pile et flot de controle). Ils dépendent d'un processus et ont un espace d'adressage partagé.

## j
Le processus attent d'avoir reçu un certain nombre de caractères à la suite avant de passer à la suite des programmes.
