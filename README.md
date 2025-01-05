# -Implement-a-program-to-print-only-diagonal-elements-in-2-D-array
#include <iostream>
using namespace std;

int main() {
    int n;

    // Ask for the size of the matrix (square matrix)
    cout << "Enter the size of the matrix (n x n): ";
    cin >> n;

    // Declare a 2D array (matrix) of size n x n
    int matrix[n][n];

    // Input the elements of the matrix
    cout << "Enter the elements of the matrix:" << endl;
    for (int i = 0; i < n; i++) {
        for (int j = 0; j < n; j++) {
            cin >> matrix[i][j];
        }
    }

    // Print diagonal elements (main diagonal and anti-diagonal)
    cout << "Diagonal elements are:" << endl;
    
    // Main diagonal elements (i == j)
    cout << "Main diagonal: ";
    for (int i = 0; i < n; i++) {
        cout << matrix[i][i] << " ";
    }
    cout << endl;

    // Anti-diagonal elements (i + j == n - 1)
    cout << "Anti-diagonal: ";
    for (int i = 0; i < n; i++) {
        cout << matrix[i][n - i - 1] << " ";
    }
    cout << endl;

    return 0;
