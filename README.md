#include "stdafx.h"
#include <stdio.h>
#include <stdlib.h>

int main()
{
  int array[11] = { 0 };
  int k;
  for (int i = 0; i < 500000; i++)
  {
    k = rand()% 11 - 5;
        array[k + 5]++;
  }
  for (int i = 0; i < 11; i++)
  {
    printf("%d-is %d\n", i - 5, array[i]);
  }
  system("pause");
  return 0;
}
