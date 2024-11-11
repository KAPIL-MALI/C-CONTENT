C++ CONTENT 
                                                                    INDEX
1.LINE NO.31 = NOTES 
2.LINE NO.35 = DATATYPES 
3.LINE NO.55 = VARIABLE SCOPE (LOCAL VARIABLE & GLOBAL VARIABLE)
4.LINE NO.95 = THE SUM OF TWO NUMBERS PROGRAM
5.LINE NO.118 = THE ARITHMETIC OPERATORS IN C++
6.LINE NO.165 = SCOPE RESOLUTION OPERATOR IN C++
7.LINE NO.195 = USE OF SIZE OF FLOAT(f), LONG AND DOUBLE(d) LITERALS.





















                            
NOTE: CTRL + / = COMMENT UNCOMMENT 
NOTE: VARIABLE DECLARED INSIDE A FUNCTION IS A LOCAL VARIABLEL.


*****************************************************************THERE ARE THREE TYPES OF DATA TYPES*************************************************************************
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





*****************************************************************************VARIABLE SCOPE********************************************************************************* 
SCOPE: scope of a variable is the region in the code where the existence of a variable is valid.
ON THE BASIS OF SCOPE THE VARIABLE IS OF TWO TYPES 
1.LOCAL VARIABLES: Local variables are declared inside the braces of any
function and can be accessed only from there.
Local Variable: Declared inside a function; accessible only within that function.
Local Variable: Exists only while the function is executing.

2.GLOBAL VARIABLES: Global variables are declared outside any function and
can be accessed from anywhere.
Global Variable: Declared outside any function; accessible throughout the entire program.
Lifetime:
Global Variable: Exists for the lifetime of the program.

*******Can global and local variable have same name in C++? : Yes, we will see!
local variables always take precedence over global variables when they have the same name inside a function.

CODE FOR UNDERSTANDING THE CONCEPT OF LOCAL VARIABLE AND GLOBAL VARIABLE
#include <iostream>
using namespace std;
int glo = 7;
void sum(){
    int a;
}

/*main function always takes presedence over the function and the value of main is given in the output */

int main() {
    int glo = 5;
    glo = 9;
    cout<<"CAPTAIN AMERICA"<<endl;
    cout<<glo;

    return 0;
}





**********************************************************************THE SUM OF TWO NUMBERS PROGRAM*************************************************************************
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





*********************************************************************DIFFERENT TYPES OF OPERATORS***************************************************************************
#include <iostream>
using namespace std;
int main() {
    
    int A = 6,B = 5;
    
    cout << "FOLLOWING ARE THE TYPES OF ARITHMETIC OPERATORS"<<endl;
    cout << "THE VALUE OF THE A + B IS "<< A+B << endl;
    cout << "THE VALUE OF THE A - B IS "<< A-B << endl;
    cout << "THE VALUE OF THE A * B IS "<< A*B << endl;
    cout << "THE VALUE OF THE A / B IS "<< A/B << endl;
    //an integers output is always integer.
    cout << "THE VALUE OF THE A % B IS "<< A%B << endl;
    // Modulus operation cannot be applied to floats.
    cout << "THE VALUE OF THE A++ IS "<< A++ << endl;//output6 +1=7
    cout << "THE VALUE OF THE ++A IS "<< ++A << endl;//output7+1= 8
    cout << "THE VALUE OF THE A-- IS "<< A-- << endl;//output8 -1=7
    cout << "THE VALUE OF THE --A IS "<< --A << endl;//output7-1= 6
    cout << endl;
    
    //ASSIGNMENT OPERATORS -> ARE USED TO ASSIGN VALUES IN THE VARIABLES
    //int a = 5,b = 4;
    //int c = 'k';
    
    //COMPARISON OPERATORS
    cout << "FOLLOWING ARE THE TYPES OF COMPARISON OPERATORS"<<endl;
    cout << "THE VALUE OF A==B IS "<< (A==B) << endl;
    cout << "THE VALUE OF A!=B IS "<< (A!=B) << endl;
    cout << "THE VALUE OF A<B IS "<< (A<B) << endl;
    cout << "THE VALUE OF A>B IS "<< (A>B) << endl;
    cout << "THE VALUE OF A<=B IS "<< (A<=B) << endl;
    cout << "THE VALUE OF A>=B IS "<< (A>=B) << endl;
    cout << endl;
    
    cout << "FOLLOWING ARE THE TYPES OF LOGICAL OPERATORS"<<endl;
    cout << "THE VALUE OF AND OPERATOR IS "<< ((A==B) && (A<B)) << endl;
    cout << "THE VALUE OF OR OPERATOR IS "<< ((A==B) || (A>B)) << endl;
    cout << "THE VALUE OF NOT OPERATOR IS "<< (!(A==B)) << endl;
  
    return 0;
}





*****************************************************************SCOPE RESOLUTION OPERATOR*********************************************************************************
#include<iostream>
using namespace std;
int C = 7;

int main (){
    
    int A;
    int B;
    int C;
    
    cout << "ENTER THE VALUE OF A: "<<endl;
    cin >> A;
    cout << "ENTER THE VALUE OF B: "<<endl;
    cin >> B;
    
    C = A+B;
    cout << "THE VALUE OF C IS "<<C<<endl;
    
    // IF YOU WANT TO ADD OR CALL THE GLOBAL C THEN USE THIS SCOPE RESOLUTION OPERATOR i.g. ::C;
    cout << "THE VALUE OF GLOBAL C IS "<<::C;
    
    return 0;
}





********************************************************USE OF SIZE OF FLOAT , LONG AND , DOUBLE LITERALS.*************************************************************
#include<iostream>
using namespace std;
int C = 7;

int main (){
    
    //f(F) and l(L) suffixes are used to let the compiler know that in what form the value 3.14 has been used.
    //otherwise by default the number is always double.
    
    float A = 3.14f;
    long double B = 3.14L;
 
 cout << "THE VALUE OF A IS " <<A<<endl<<"THE VALUE OF B IS "<<B;
 cout << endl;
  
 cout << "THE SIZE OF 3.14 IS "<<sizeof(3.14)<<endl;
 cout << "THE SIZE OF 3.14f IS "<<sizeof(3.14f)<<endl;
 cout << "THE SIZE OF 3.14F IS "<<sizeof(3.14F)<<endl;
 cout << "THE SIZE OF 3.14l IS "<<sizeof(3.14l)<<endl;
 cout << "THE SIZE OF 3.14L IS "<<sizeof(3.14L)<<endl;
 
    return 0;
}


