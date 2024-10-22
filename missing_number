#include <iostream>
#include <ctime>
#include <algorithm> 
using namespace std;

void print(int a[], int x) {
    cout << "Array is: ";
    for (int i = 0; i < x-1; i++) {
        cout << a[i] << " ";
    }
    cout << endl;
}

bool existsInArray(int a[], int size, int value) {
    for (int i = 0; i < size; i++) {
        if (a[i] == value) {
            return true;
        }
    }
    return false;
}


int main() {
    int num;
    cout << "Enter the number of elements: " << endl;
    cin >> num;

    srand(time(0));  
    int arr[num];  

    for (int i = 0; i < num-1; i++) {
        int newValue;
        do {
            newValue = rand() % num;  
        } while (existsInArray(arr, i, newValue)); 
        arr[i] = newValue; 
    }


    print(arr, num);
    
  sort(arr, arr + num); 
    int count = 0;
    for(int i=0; i<num; i++){
       if (arr[i] == count){
            count++;
        }
        else{
            cout<<"The Missed Number is: "<< count<<endl;
        }
    }
    return 0;
}
