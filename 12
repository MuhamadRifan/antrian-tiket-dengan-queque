#include <stdio.h>
#include <conio.h>
#include <stdlib.h>

int main() {
    int queue[10], i, head=-1, tail=-1, enqueue, pil, urut=0, tmp;
   
    do {
        system("pause");
        system("cls");
        printf("1. Masukkan Antrian\n");
        printf("2. Keluarkan Antrian\n");
        printf("3. Lihat Antrian\n");
        printf("4. Keluar\n\n");
        printf("Silahkan masukkan pilihan anda : ");
        scanf("%d", &pil);
        printf("\n");

       
        if(pil==1) {if(tail==9) {printf("Antrian Penuh\n\n");}
                    else if(tail==-1) {head++;tail++;
                                       printf("Masukkan nilai : ");
                                       scanf("%d", &enqueue);
                                       queue[tail]=enqueue;
                                       urut++;
                                       printf("\nNomor urut : %d\n", urut);
                                       printf("Langsung dilayani\n\n");}
                    else {tail++;
                          printf("Masukkan nilai : ");
                          scanf("%d", &enqueue);
                          queue[tail]=enqueue;
                          urut++;
                          printf("\nNomor urut : %d\n", urut);
                          printf("Anda harus menunggu %d antrian lagi\n\n", tail);}}
                         
        else if(pil==2) {if(tail==-1) {printf("Antrian kosong\n\n");}
                         else {printf("Data dengan nilai %d sudah dilayani\n\n", queue[head]);
                               tmp=queue[head];
                               for(i=head;i<=tail;i++) {queue[i]=queue[i+1];}
                               queue[tail]=tmp;
                               urut++;
                               printf("Data dengan nilai %d masuk antrian kembali dengan no. urut %d\n", queue[tail], urut);
                               if(tail==0) {printf("Yang bersangkutan langsung dilayani\n\n");}
                               else {printf("Yang bersangkutan harus menunggu %d antrian lagi\n\n", tail);}}}
                              
        else if(pil==3) {if(tail==-1) {printf("Antrian kosong\n\n");}
                         else {for(i=head;i<=tail;i++) {printf("Antrian ke-%d : %d\n", i+1, queue[i]);}
                         printf("\n");}}

        else if(pil==4) {printf("Anda telah selesai menggunakan program Queue Circular\n\n");}

        else {printf("Pilihan yang anda masukkan tidak valid\n\n");}
        } while(pil!=4);

    getch();
}
