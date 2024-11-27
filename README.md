#include <stdio.h>
#include <stdlib.h>
#include <time.h>

int main() {
    int friendNumber, total;
    char confirmation;
    int randomNumber;

 
    
     srand(time(0)); 
     randomNumber = (rand() % 90) + 10;
    

    
    printf("Step 1: Think of a number in your mind (you don't need to tell me).\n");
    printf("Did you think of a number? (y/n): ");
    scanf(" %c", &confirmation);
    if (confirmation != 'y') {
        printf("Please think of a number first. Restart the game.\n");
        return 0;
    }

    
    printf("\nStep 2: take the same number from your friend.\n");
    

    printf("Did you take the number from your friend? (y/n): ");
    scanf(" %c", &confirmation);
    if (confirmation != 'y') {
        printf("Please take the number from your friend to proceed. Restart the game.\n");
        return 0;
    }

    
    printf("\nStep 3: I am giving you a random number.\n");
    printf("My random number is: %d\n", randomNumber);

    printf("Did you note down my random number? (y/n): ");
    scanf(" %c", &confirmation);
    if (confirmation != 'y') {
        printf("Please note down my random number to proceed. Restart the game.\n");
        return 0;
    }

 
    printf("\nStep 4: Add your number, your friend's number, and my random number.\n");
    printf("Did you add them all? (y/n): ");
    scanf(" %c", &confirmation);
    if (confirmation != 'y') {
        printf("Please add the numbers to proceed. Restart the game.\n");
        return 0;
    }

    
    printf("\nStep 5: Divide the total by 2 and give one part to God.\n");
    printf("have you divide the total and give one part to God? (y/n): ");
    scanf(" %c", &confirmation);
    if (confirmation != 'y') {
        printf("Please divide the total to proceed. Restart the game.\n");
        return 0;
    }

    
    printf("\nStep 6: Now, return the number you took from your friend.\n");
    printf("Did you return the number to your friend? (y/n): ");
    scanf(" %c", &confirmation);
    if (confirmation != 'y') {
        printf("Please return the number to your friend to proceed. Restart the game.\n");
        return 0;
    }

  
    printf("\nFinal Step: now i am gonna to say your number...\n");
    printf("The final number left with you: %2f\n", (float)randomNumber / 2);

    printf("Game over. Thank you for playing!\n");
    return 0;
}
