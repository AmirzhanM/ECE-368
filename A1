#include <stdio.h>

void print_coin_combinations(int cents) {
    int quarters = 25, dimes = 10, nickels = 5, pennies = 1;

    for (int q = cents / quarters; q >= 0; q--) {
        int minus_quarters = cents - q * quarters;
        for (int d = minus_quarters / dimes; d >= 0; d--) {
            int minus_dimes = minus_quarters - d * dimes;
            for (int n = minus_dimes / nickels; n >= 0; n--) {
                int minus_nickels = minus_dimes - n * nickels;
                int p = minus_nickels;
                printf("%d quarter(s), %d dime(s), %d nickel(s), %d pennie(s)\n", q, d, n, p);
            }
        }
    }
}

int main() {
    int cents;
    scanf("%d", &cents);
    print_coin_combinations(cents);

    return 0;
}