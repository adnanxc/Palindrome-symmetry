# Palindrome-symmetry

#include <iostream>
using namespace std;

int main(){

    int x , n , rev = 0 , rem;
    cout << "Enter a number: ";
    cin >> x;
    n = x;

    while(n != 0){
        rem = n % 10;
        rev = (rev * 10) + rem;
        n = n / 10;
    }

    if (rev==x){
        cout << "Symmetric.";
    }

    else {
        cout << "Not symmetric.";
    }




    return 0;
}

