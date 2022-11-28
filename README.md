- 👋 Hi, I’m @moatezbk
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
moatezbk/moatezbk is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
/******************************************************************************

Welcome to GDB Online.
GDB online is an online compiler and debugger tool for C, C++, Python, PHP, Ruby, 
C#, OCaml, VB, Perl, Swift, Prolog, Javascript, Pascal, HTML, CSS, JS
Code, Compile, Run and Debug online from anywhere in world.

*******************************************************************************/
#include <stdio.h>
#include <string.h>
typedef struct {
    int id ;
    int Nbr_Rayon_Depot ;
    char ville[15];
    char type_Produit[15];
    int Tab_Nbr_Pr_Rayon[10];
    char Nom_Resp[20] ;
    
} depot ;
depot list[20];
int main()
{ int i=0,j,choix;
char prod1[10];
   do {
    do {
    /* print instroction for the user */
 printf("1. Ajouter un nouveau dépôt.\n");
 printf("2. Afficher la liste des dépôts.\n");
 printf("3. Ajouter des produits dans le premier rayon.\n");
 printf("4. Lister les dépôts contenant des produits.\n") ;
 printf("5. Afficher le nom du responsable et la ville du dépôt contenant le plus de produits.\n");
 printf("6. Modifier le responsable d'un dépôt.\n");
 printf("7. Calculer le nombre de dépôts situés à une ville saisie au clavier.\n");
 printf("8. Afficher les dépôts où le nombre de produits dans chaque rayon est ");
 printf("inférieur à un seuil max saisi par l’utilisateur.\n");
 printf("9. Supprimer le premier dépôt vide (Tous les rayons sont vides).\n");
 /* print instruction for the user */
 /*scanf the value entred by the user */
 scanf("%d",&choix);
    } while (choix<0 || choix>9);
 /* instruction to execute switch the entred value */
switch (choix)
{
case 1:
/*Ajouter un nouveau dépôt*/
printf("donner l'identfiant \n");
scanf("%d",&list[i].id);
printf("l'identfiant %d \n",list[i].id);
printf("donner le nombre de rayon \n");
scanf("%d",&list[i].Nbr_Rayon_Depot);
printf("nombre de rayon%d \n",list[i].Nbr_Rayon_Depot);
 // fflush(stdin);
puts("donner la ville");
scanf("%s",list[i].ville);
puts("donner le nom de responsable");
scanf("%s",list[i].Nom_Resp);
puts("donner le type du produit");
scanf("%s",list[i].type_Produit);
for (int j=0;j<10;j++){
 list[i].Tab_Nbr_Pr_Rayon[j]=0;   
}
i++;
/*ajouter un nauveau depot i++  */
break;

/*Afficher la liste des dépôts. */
case 2:
for (int j=0;j<i;j++){
  printf("depot num %d l'identfiant %d",j,list[j].id);
}
break;
/*Afficher la liste des dépôts. */

case 3:
printf("donner nombre rayon/ n");
scanf("%d",&list[i].Nbr_Rayon_Depot);
    if (list[i].Nbr_Rayon_Depot==1);
  {
for(j=0;j<200;j++)
{printf("donner les produits ");
scanf("%d",&list[i].Nbr_Rayon_Depot);}}
break;
/**/
case 4:
printf("donner le  type de produit ");
scanf("%s",prod1);
for(j=0;j<i;j++)
{if (strcmp(prod1,list[i].type_Produit)==0)
printf("les depots %d  choisi %d,%s,%s",list[i].id,list[i].Nbr_Rayon_Depot,list[i].ville,list[i].Nom_Resp);
 else
        printf("le depot n'existe pas");
}
break;
/* */
case 5:
break;
/* */
case 6:
break;
/* */
case 7:
break;
/* */
case 8:
break;
/* */
case 9:
break;
/* */
}

 //Clrscr ();  
}while(1);
return 0;
}
