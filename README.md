# 186HW2
## part 1 
need to O(4) to find the number 8

## part 2
need O（1）to find the number 8 by using the binary search .

## part 3

The maximum of steps of 100,000 is 17.

## part 4

```c++

#include <iostream>
int BinarCal(int array[] , int *step , int size,int target) {


    int firstNum = 0;
    int lastNumber = size-1;
    while (firstNum <= lastNumber) {

        int mid = firstNum + (lastNumber - firstNum)/2;



        (*step) ++;

        if(array[mid] == target) {
            printf("use the to find is %d ",*step);
            return *step;
        }


        if(array[mid] > target) {
            lastNumber = mid -1;
        }else {
            firstNum = mid + 1;
        }
    }
    return *step;



}



using namespace std;
int main() {
// linear
    int myArray[100];
    int step = 0;
    int searchNume ;

    // linear

    cin >>  searchNume;
    for (int i = 0; i < size(myArray); ++i) {
        step++;
        if (searchNume == myArray[i]){
            printf("%d",step);
            break;

        }
        if (searchNume != myArray[i] && i == 99){
            printf("%d",step);

        }
    }

int size = std :: size(myArray);


//    int BinarCal(int myArray[] , int *step , int size, int target);
    int b = BinarCal( myArray , &step , size, searchNume);


}

```

## video 
https://youtu.be/rpBOkx93L2w
