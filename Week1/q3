#include <iostream>
#include <cmath>
using namespace std;

string jumpSearch(const int arr[], int n, int key, int &comparisons) {
    int step = sqrt(n); 

    
    int prev = 0, curr = step;
    while (curr < n && arr[curr] < key) {
        prev = curr;
        curr += step;
        comparisons++;
    }

    
    for (int i = prev; i < min(curr, n); ++i) {
        comparisons++;
        if (arr[i] == key) {
            return "Present";
        }
    }

    return "Not Present";
}

int main() {
    int t;
    cout << "Enter the number of test cases: ";
    cin >> t;

    while (t--) {
        int n;
        cout << "Enter the size of the array: ";
        cin >> n; 

        int arr[n];
        cout << "Enter " << n << " space-separated integers describing the array: ";
        for (int i = 0; i < n; ++i) {
            cin >> arr[i];
        }

        int key;
        cout << "Enter the key element to be searched: ";
        cin >> key;

        int comparisons = 0;
        string result = jumpSearch(arr, n, key, comparisons);

        cout << result << endl;
        cout << "Comparisons: " << comparisons << endl;
    }

    return 0;
}
