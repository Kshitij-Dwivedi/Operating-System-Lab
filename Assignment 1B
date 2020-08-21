#include <stdio.h>
#include <stdlib.h>
#include <sys/types.h>
#include <sys/wait.h>
#include <unistd.h>

int main(void) {
  pid_t pid = fork();

  if(pid == 0) {
    printf("Child process PID: %d\n",  getpid());

  }
  else if(pid > 0) {
    printf("Parent Process PID: %d\n", getpid());

  }
  return 0;
}
