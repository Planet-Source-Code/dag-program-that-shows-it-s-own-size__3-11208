<div align="center">

## Program that shows it's own size\.\.\.


</div>

### Description

A program that shows it's own size.
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Dag\.\.](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/dag.md)
**Level**          |Beginner
**User Rating**    |3.8 (19 globes from 5 users)
**Compatibility**  |C
**Category**       |[Miscellaneous](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/miscellaneous__3-1.md)
**World**          |[C / C\+\+](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/c-c.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/dag-program-that-shows-it-s-own-size__3-11208/archive/master.zip)

### API Declarations

```
#include &lt;stdio.h&gt;
#include &lt;stdlib.h&gt;
```


### Source Code

```
#include <stdio.h>
#include <stdlib.h>
FILE *fichero;
char letra;
int contador=0;
int main(int argc,char *argv[])
   {
   fichero=fopen(argv[0],"rb");
   letra=getc(fichero);
   while(feof(fichero)==0)
     {
     contador=contador+1;
     letra=getc(fichero);
     }
   printf("My size is %i Bytes.\n",contador);
   system("pause");
   }
```

