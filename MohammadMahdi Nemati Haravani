#include <stdio.h>
#include <math.h>
int win(char c[]){
    if(c[0]==c[1] && c[1]==c[2] && c[0]!='\0')
           return 1;
        else if(c[3]==c[4] && c[4]==c[5] && c[3]!='\0')
           return 1;
        else if(c[6]==c[7] && c[7]==c[8] && c[6]!='\0')
            return 1;
        else if(c[0]==c[3] && c[3]==c[6] && c[0]!='\0')
            return 1;
        else if(c[1]==c[4] && c[4]==c[7] && c[1]!='\0')
            return 1;
        else if(c[2]==c[5] && c[5]==c[8] && c[2]!='\0')
            return 1;
        else if(c[0]==c[4] && c[4]==c[8] && c[4]!='\0')
            return 1;
        else if(c[2]==c[4] && c[4]==c[6] && c[4]!='\0')
            return 1;
        return 0;
}
int main(){
    int counter = 0 , input;
    char tabel_xo[9]={'\0'};
    while(counter < 9){
        if(counter%2 == 0){
            printf("Player X: \n");
            scanf("%d" ,&input);
            if(tabel_xo[input-1] == '\0')
                tabel_xo[input-1] = 'X';
            else
                counter--;
        }
        else{
            printf("Player O: \n");
            scanf("%d" ,&input);
            if(tabel_xo[input-1] == '\0')
                tabel_xo[input-1] = 'O';
            else
                counter--;
        }
        printf("%c | %c | %c\n" ,tabel_xo[0],tabel_xo[1],tabel_xo[2]);
        printf("%c | %c | %c\n" ,tabel_xo[3],tabel_xo[4],tabel_xo[5]);
        printf("%c | %c | %c\n" ,tabel_xo[6],tabel_xo[7],tabel_xo[8]);
        if(win(tabel_xo)==1)
            break;
        counter++;
    }
    if(counter%2 == 0)
        printf("Player X has won the game \n");
    else
        printf("Player O has won the game \n");

}
