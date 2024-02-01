#include <iostream>
using namespace std;

int linearSearch(const int arr[], int n, int key, int &comparisons) {
    for (int i = 0; i < n; ++i) {
        comparisons++; 
        if (arr[i] == key) {
            return i;
        }
    }
    return -1;
}

int main() {
    int n;

    cout << "Enter the size of the array: ";
    cin >> n;

    int arr[n];

    
    cout<<"Enter the elements of the array:"<<endl;
    for (int i = 0; i < n; ++i) {
        cout << "Enter element " << i + 1 << ": ";
        cin >> arr[i];
    }

    int key;

  
    cout << "Enter the key to search: ";
    cin >> key;

    int comparisons = 0;

    int result = linearSearch(arr, n, key, comparisons);

    if (result != -1) {
        cout << "Element found at index " << result <<endl;
    } else {
        cout << "Element not found" << endl;
    }

    cout << "Total comparisons: " << comparisons << endl;

    return 0;
}
