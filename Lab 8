#include <iostream>
using namespace std;

int main() {
    int numOfBooks;
    int totalFine = 0;
    cout << "Number of books to be returned: ";
    cin >> numOfBooks;
   
    for(int i=1;i<=numOfBooks;i++) {
        int days;
        cout << "Book number " << i << " late days: ";
        cin >> days;
        int bookFine=5;
        for(int j=1;j<days;j++) {
            bookFine = bookFine*2;
            if(bookFine>=1000) {
                bookFine=1000;
                break;
            }
        }
        cout << "Fine for book " << i << " : " << bookFine << endl;
        totalFine = totalFine + bookFine;
    }
    cout << "Total fine : " << totalFine;
    return 0;
}
