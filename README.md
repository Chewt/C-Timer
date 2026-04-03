# C-Timer
A header only library for timing blocks of code in the C language

Example usage
```c
#include <stdio.h>

#define TIMER_IMPLEMENTATION
#include "timer.h"

int main()
{
  // Initialize and start timer
  Timer t;

  timer_start(&t);
  // Do Stuff
  timer_stop(&t);

  // Print results
  printf("Wall Time: %.6f\n", t.time_taken);
  printf("Cpu Time: %.6f\n", t.cpu_time_taken);
  return 0;
}
```
