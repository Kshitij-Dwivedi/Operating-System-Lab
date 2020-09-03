#include<stdio.h>
#include<sys/types.h>
#include<sys/wait.h>
#include<unistd.h>
#include<stdlib.h>

int main() {
    pid_t pid = fork();

    if(pid > 0) {
        wait(NULL);
        printf("End of Parent Process\n");
    }

    else if(pid == 0) {
        pid_t pid1 = fork();

        if(pid1 > 0) {
            wait(NULL);
            printf("End of Child Process 1\n");
        }

        else if(pid1 == 0) {
            pid_t pid2 = fork();

            if(pid2 > 0) {
                wait(NULL);
                printf("End of Child Process 2\n");
            }

            else if(pid2 == 0) {
                printf("End of Child Process 3\n");
            }
        }
    }
} 
