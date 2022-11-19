# C-Timer
A header only library for timing blocks of code in the C language


Example usage
````C
#include "timer.h"

int main()
{
  Timer t;
  StartTimer(&t);
  \\Do Stuff
  StopTimer(&t);
  printf("Wall Time: %.6f\n", t.time_taken);
  printf("Cpu Time: %.6f\n", t.cpu_time_taken);
  return 0;
}
```
