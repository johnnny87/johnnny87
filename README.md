#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
	int soldadosA, tanquesA, avioesA, lcmA;
	int soldadosB, tanquesB, avioesB, lcmB;
	int soldadosRB, tanquesRB, avioesRB, lcmRB;
	
	scanf("%d %d %d %d", &soldadosA, &tanquesA, &avioesA, &lcmA);
		scanf("%d %d %d %d", &soldadosB, &tanquesB, &avioesB, &lcmB);
		scanf("%d %d %d %d", &soldadosRB, &tanquesRB, &avioesRB, &lcmRB);
	
	if((soldadosA+tanquesA+avioesA+lcmA)<((soldadosB+tanquesB+avioesB+lcmB)+(soldadosRB+tanquesRB+avioesRB+lcmRB))){
		if(soldadosA<soldadosB+soldadosRB && tanquesA<tanquesB+tanquesRB || avioesA<avioesB+avioesRB && lcmA<lcmB+lcmRB)
		if(soldadosA<soldadosB+soldadosRB && avioesA<avioesB+avioesRB || lcmA<lcmB+lcmRB && tanquesA<tanquesB+tanquesRB)
		if(soldadosA<soldadosB+soldadosRB && lcmA<lcmB+lcmRB || avioesA<avioesB+avioesRB && tanquesA<tanquesB+tanquesRB )
			printf("Recuar\n");		
	}
	if((soldadosA+tanquesA+avioesA+lcmA)>((soldadosB+tanquesB+avioesB+lcmB)+(soldadosRB+tanquesRB+avioesRB+lcmRB))){
		if(soldadosA>soldadosB+soldadosRB && tanquesA>tanquesB+tanquesRB || avioesA>avioesB+avioesRB && lcmA>lcmB+lcmRB)
		if(soldadosA>soldadosB+soldadosRB && avioesA>avioesB+avioesRB || lcmA>lcmB+lcmRB && tanquesA>tanquesB+tanquesRB)
		if(soldadosA>soldadosB+soldadosRB && lcmA>lcmB+lcmRB || avioesA>avioesB+avioesRB && tanquesA>tanquesB+tanquesRB )
		printf("Avancar\n");
	
		}else if((soldadosA+tanquesA+avioesA+lcmA)==((soldadosB+tanquesB+avioesB+lcmB)+(soldadosRB+tanquesRB+avioesRB+lcmRB))){
		printf("Permanecer\n");
	} 
	}
