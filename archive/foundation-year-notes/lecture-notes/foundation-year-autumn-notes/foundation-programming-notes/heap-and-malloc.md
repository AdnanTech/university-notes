# Heap and Malloc

## Heap

{% embed url="https://en.wikipedia.org/wiki/Binary_heap" %}

[Stack vs heap](https://www.guru99.com/stack-vs-heap.html)

## Malloc

```c
#include <stdio.h>
#include <stdlib.h>

int main () {
   char *str;

   /* Initial memory allocation */
   str = (char *) malloc(15); /* 15 bytes */
   strcpy(str, "tutorialspoint");
   printf("String = %s,  Address = %u\n", str, str);

   /* Reallocating memory */
   str = (char *) realloc(str, 25); /* 25 bytes */
   strcat(str, ".com");
   printf("String = %s,  Address = %u\n", str, str);

   free(str);
   
   return(0);
}
```

{% embed url="http://www.cplusplus.com/reference/cstdlib/malloc/" %}

{% embed url="https://www.design-reuse.com/articles/25090/dynamic-memory-allocation-fragmentation-c.html" %}



