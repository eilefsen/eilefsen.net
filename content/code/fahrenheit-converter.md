+++
title = "Fahrenheit-Converter"
date = 2023-10-24T21:06:30+02:00
draft = false
+++

I am currently learning C and i would like to share my first "proper" program.  
It's not much, but i am quite happy with this.  
  

```
#include <stdio.h>
#include <stdlib.h>

int celsius(int fahrenheit)
{
    return 5 * (fahrenheit - 32) / 9;
}

int main(int argc, char *argv[])
{
    if (argc >= 2) {
        int fahrenheit = atoi(argv[1]);
        printf("%d°F is equal to %d°C\n",
               fahrenheit, celsius(fahrenheit));
        return EXIT_SUCCESS;
    }
    printf("Not enough arguments supplied.\n");
    printf("Usage:\tcelsius <degrees fahrenheit>\n");
    return EXIT_FAILURE;
}
```
