# Traduction d'adresses

## 4.1

taille des pages : 4ko

adresses virtuelles codés sur 32 bits

  déplacement : log2(4096 = 4ko) = 12 bits
  nombre de pages virtuelles (32 -12 )= 20 bits

espace virtuel total : 2^20 * 4ko = 2^32 = 4Go

## 4.2

on évite ainsi les défaut de page, tout en accélérant les accès mémoires du systeme d'exploitation ( pas de traduction)

## 4.3

On a 2^20 pages, ce qui correspond à 2^20 entrées dans la table desp ages. Chaque entrée est sur 4 octets. La taille des pages fait donc
2^20 x 4o = 4 Mo


## 4.4

traduction :  802EFS -> 2EEF4EF5
              402AAF -> 34CEAAF
              5003  ->  34FE003
              403345  -> 64A345

## 4.5

100 ko : 100/4 = 25 âges

25 pages < 2^10 donc 1 ivre

1 table des livrs + 1 table des pages

1*2^10*4+1*2^10*4=8Ko

1Mo :

100/4 = 250 pages

1 livres -> 8Ko

10Mo: 2500 pages
3 livres
4 Ko+ 3*4Ko = 16Ko
