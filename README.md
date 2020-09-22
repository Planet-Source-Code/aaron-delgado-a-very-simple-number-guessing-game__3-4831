<div align="center">

## A Very Simple Number Guessing Game


</div>

### Description

The Number Guessing Game will generate a number between 1 and 100. The user will have infinite attempts to guess the number.
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Aaron Delgado](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/aaron-delgado.md)
**Level**          |Beginner
**User Rating**    |3.9 (31 globes from 8 users)
**Compatibility**  |C, C\+\+ \(general\)
**Category**       |[Complete Applications](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/complete-applications__3-7.md)
**World**          |[C / C\+\+](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/c-c.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/aaron-delgado-a-very-simple-number-guessing-game__3-4831/archive/master.zip)





### Source Code

```
#include <stdio.h>
#include <stdlib.h>
#include <time.h>
int main()
{
 int n;
 int num;
 srand(time(NULL)); //generate the random seed generator
 n = 1 + rand() % 100; //pick a number from 1 to 100
 printf("\nI have a number between 1 and 100\n");
 printf("Can you guess my number?\n");
 printf("Please type your first guess.\n");
 scanf("%d", &num);
 while (n != num){
   if (num > n){
      printf("Too High! Try again!\n");
      scanf("%d", &num);
     }
   else
   if (num < n){
      printf("Too Low! Try again!\n");
      scanf("%d", &num);
      }
   }/*end of while loop*/
      printf("Excellent! You guessed the number!\n");
    return 0;
}
```

