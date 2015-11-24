# 2 Hiérarchie de processus

```c
float val = 0.0;
int pidP = getpid(); // pid du pere
for (int i = 0; i <5;i++){
  if (pidP==getpid()){
    fork();
    if(i==0 && pidP != getPid()){
      int pidPP = getpid();
      val = i+1;
      for(int j = 0 ; j<2;j++){
        if (pidPP==getpid()){
          fork();
        }else{
          val = i+1 + ((j+1)/10)
        }
      }
    }else{
      val = i+1;
    }
  }
}

printf("%f\n",val );

```
