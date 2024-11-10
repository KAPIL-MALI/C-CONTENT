C++ CONTENT 

NOTE: CTRL + / = COMMENT UNCOMMENT 


THERE ARE THREE TYPES OF DATA TYPES 
1.USER DEFINED DATA TYPE
*Struct
~ Union
Enum
2.BUILT IN DATA TYPE IN C++
int,float,char,
double = 3,1453534534,
boolean = booean is used when there is condition like TRUE OR FALSE. 
3.DERIVED DATA TYPE
1.Array
2.Function
3.Pointer
Note: These will be covered separately in different videos. For now
understanding that these are the derived defined data types should do!




VARIABLE SCOPE 
SCOPE: scope of a variable is the region in the code where the existence of a variable is valid.
ON THE BASIS OF SCOPE THE VARIABLE IS OF TWO TYPES 
1.LOCAL VARIABLES: Local variables are declared inside the braces of any
function and can be accessed only from there.
2.GLOBAL VARIABLES: Global variables are declared outside any function and
can be accessed from anywhere.
*******Can global and local variable have same name in C++? : Yes, we will see!


THE SUM OF TWO NUMBERS PROGRAM
#include <iostream>
using namespace std;
int main (){
    int A,B,SUM;
    
    cout <<"ENTER THE VALUE OF A:";
    cin >>A;
    
    cout <<"ENTER THE VALUE OF B:";
    cin >>B;
    
    SUM = A + B;
    
    cout<<"THE SUM OF " << A << " AND " << B << " IS: " << SUM << endl;
    
    return 0;
    
}

