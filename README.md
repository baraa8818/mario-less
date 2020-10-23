#include <stdio.h>
#include <cs50.h>

int main(void){
    int n;
    int x = 1;

    do {
        n = get_int("Height :");
    }
    while(n < 1 );

    for(int i = 0; i < n ; i++){

        for(int j = 0; j < n ; j++){
            if (n - j == x ){
                printf("#");
                x++;
            }
            else if(n - j > x){
                printf(" ");
            }
            else {
                printf("#");
            }
        }
        printf("\n");
    }
}
