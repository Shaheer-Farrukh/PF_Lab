#include <iostream>
using namespace std;
void menu(){
    cout << "1)even/odd" << endl;
    cout << "2)count digits" << endl;
    cout << "3)sum of digits" << endl;
    cout << "4)check prime" << endl;
    cout << "5)exit" << endl;
}
int countdigits(int n) {
    int count = 0;
    while(n!=0){
        count ++;
        n/=10;
    }
    return count;
}
bool checkEvenOdd(int n) {
    if(n%2== 0) {
    return true;
    }
    else { 
        return false;
    }
}
int sumdigits(int n) {
    int sum = 0;
    while(n>0) {
        sum += n%10;
        n/=10;
    }
    return sum;
}
bool isprime(int n) {
    if(n<2) return false;
    for(int i=2;i<=n/2;i++) {
        if(n%i==0)
        return false;
    }
    return true;
}
int getnumber() {
    int n;
    cout << "enter number \n";
    cin >> n;
    return n;
}
void options() {
    int n, count,sum;
    int c;
    bool istrue=true;
    
    do {
        cout << "enter number from menu \n";
        cin >> c;
        n = getnumber();
        switch(c) {
            case 1:
            if(checkEvenOdd(n)) {
                cout << n << " is even \n";
            } else {
                cout << n << "is odd \n";
            }
            break;
            case 2: count = countdigits(n);
            cout << count << endl;
            break;
            case 3: sum=sumdigits(n);
            cout << sum << endl;
            break;
            case 4:
            if(isprime(n)) {
                cout << n << " is prime \n";
            } else {cout << n << " is not prime \n";
            }
            break;
            case 5: istrue=false;
        }
    } while(istrue);
} 
int main(){
    menu();
    options();
    return 0;
}
