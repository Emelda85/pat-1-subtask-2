#include <iostream>
using namespace std;

int main() {
    int temp1, temp2, temp3;
 // Input 1st reading
    cout << "Enter the first temperature reading: ";
    cin >> temp1;

    // Input 2nd reading
    cout << "Enter the second temperature reading (5 minutes later): ";
    cin >> temp2;

    // Check difference between first and second readings
    int diff = temp2 - temp1;

    if (diff > 50) {
        cout << "Reduce fryer heat before taking the third reading." << endl;
    } else if (diff < 10) {
        cout << "Increase the Fryer heat before taking the third reading." << endl;
    }

    // Input 3rd reading
    cout << "Enter the third temperature reading (5 minutes later): ";
    cin >> temp3;

    // Check if the oil is ready
    if (temp3 >= 150 && temp3 <= 190) {
        cout << "You may start frying the Magwinyas." << endl;
    } else {
        cout << "Oil is not ready for frying!" << endl;
    }

    return 0;
}
