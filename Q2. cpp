#include <iostream>

int binarySearch(const int arr[], int low, int high, int key, int &comparisons) {
    while (low <= high) {
        int mid = low + (high - low) / 2;
        comparisons++; 

        if (arr[mid] == key) {
            return mid; 
        } else if (arr[mid] < key) {
            low = mid + 1; 
        } else {
            high = mid - 1; 
        }
    }

    return -1;
}

int main() {
    int n;

    
    cout << "Enter the size of the sorted array: ";
    cin >> n;

    int arr[n];

    
    cout << "Enter the sorted elements of the array:" << endl;
    for (int i = 0; i < n; ++i) {
        cout << "Enter element " << i + 1 << ": ";
        cin >> arr[i];
    }

    int key;

    
    cout << "Enter the key to search: ";
    cin >> key;

    int comparisons = 0;

    int result = binarySearch(arr, 0, n - 1, key, comparisons);

    if (result != -1) {
        cout << "Element found at index " << result << endl;
    } else {
        cout << "Element not found" << endl;
    }

    cout << "Total comparisons: " << comparisons << endl;

    return 0;
}
