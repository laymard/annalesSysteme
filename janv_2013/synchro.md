# 6 Synchronisation entre processus

## 6.1

initialisation :
```c
init(A,1);
init(B,1);
init(C,1);
```


P1:
```c
while (1) {
  P(A);
  printf("A");
  V(B);
}
```
P2:
```c
while (1) {
  P(B);
  printf("B");
  V(C);
}
```
P3:
```c
while (1) {
  P(C);
  printf("C");
  V(A);
}
```


## 6.2

initialisation :
```c
init(A,1);
init(BC,0);
```


P1:
```c
while (1) {
  P(A);
  printf("A");
  V(BC);
}
```
P2:
```c
while (1) {
  P(BC);
  printf("B");
  V(A);
}
```
P3:
```c
while (1) {
  P(BC);
  printf("C");
  V(A);
}
```
## 6.3

initialisation :
```c
init(A,0);
init(B,0);
init(C,0);
```


P1:
```c
int i =0;
while (1) {

  printf("A");
  if(i++==0){
    V(B);
    P(A);
    V(C);
    P(A);
  }else{
    V(C);
    P(A);
    V(B);
    P(A);
  }
  i%=2
}
```
P2:
```c
while (1) {
  P(B);
  printf("B");
  V(A);
}
```
P3:
```c
while (1) {
  P(C);
  printf("C");
  V(A);
}
```
