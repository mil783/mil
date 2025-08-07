#include <iostream>
using namespace std;

int main() {
    double sayi1, sayi2;
    char islem;

    cout << "Birinci sayıyı girin: ";
    cin >> sayi1;

    cout << "İşlem türünü girin (+, -, *, /): ";
    cin >> islem;

    cout << "İkinci sayıyı girin: ";
    cin >> sayi2;

    switch(islem) {
        case '+':
            cout << "Sonuç: " << (sayi1 + sayi2) << endl;
            break;
        case '-':
            cout << "Sonuç: " << (sayi1 - sayi2) << endl;
            break;
        case '*':
            cout << "Sonuç: " << (sayi1 * sayi2) << endl;
            break;
        case '/':
            if (sayi2 != 0)
                cout << "Sonuç: " << (sayi1 / sayi2) << endl;
            else
                cout << "Hata: Sıfıra bölme yapılamaz!" << endl;
            break;
        default:
            cout << "Geçersiz işlem!" << endl;
    }

    return 0;
}
