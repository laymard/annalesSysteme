# Salle de bains

# 7.1

```c
init(mutex[2],1);
init(bathroom,1);
int boys = 0;
int girls = 0;

boy_want_to_use_bathroom(){
  P(mutex[0]);
  if(boys==0){
    P(bathroom);
  }
  boys++;
  V(mutex[0]);
}

boy_leaves_bathroom(){
  P(mutex[0]);
  boys--;
  if(boys==0){
    V(bathroom);
  }
  V(mutex[0]);
}
```

## 7.2

```c
// initialisation
init(boy,1);
init(bathroom,1);
init(S,0);
init(Mb,1);

// Fonctions
boy_leaves_bathroom(){
  P(boys);
  nbPers--;
  if (nbBoys==0) {
     V(bathroom);  
  }
  V(boys);
}

boy_want_to_use_bathroom(){

    P(Mb);
    P(boys);
    if(nbPers==0){
      P(bathroom));
      V(s);
      V(s);

    }
    V(boy);
    if (girls>0){
      P(S);
    }
    nbPers++;
    V(Mb);
}
girl_leaves_bathroom(){

}

girl_want_to_use_bathroom(){

}

```
