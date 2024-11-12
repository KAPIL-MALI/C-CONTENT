C++ CONTENT 
                                                                    INDEX
1.LINE NO.32 = NOTES 
2.LINE NO.36 = DATATYPES 
3.LINE NO.56 = VARIABLE SCOPE (LOCAL VARIABLE & GLOBAL VARIABLE)
4.LINE NO.96 = THE SUM OF TWO NUMBERS PROGRAM
5.LINE NO.119 = THE ARITHMETIC OPERATORS IN C++
6.LINE NO.166 = SCOPE RESOLUTION OPERATOR IN C++
7.LINE NO.195 = USE OF SIZE OF FLOAT(f), LONG AND DOUBLE(d) LITERALS
8.LINE NO.224 = REFERENCE VARIABLE 
9.LINE NO.244 = TYPECASTING
10.LINE NO.273 = CHAR EXAMPEL OF REFERENCE VARIABLE,const keyword
11.LINE NO.299 = MANIPULATORS setw -> (iomanip)
12.LINE NO.326 = OPERATOR PRESEDENCE AND ASSOCIATIVITY
13.LINE NO.369 = CONTROL STATEMENTS(TYPES AND DIFFERENCE BETWEEN if-else and switch case statements)
14.LINE NO.388 = TYPES OF LOOPS(ALL THREE NICELY EXPLAINED)














                            
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





*******************************************************************REFERENCE VARIABLE****************************************************************************************
#include<iostream>
using namespace std;

int main (){

//kapil = k = captain america     
int a = 5;
int & b = a;//here & is used so that b does not make its own memory location.

cout << "the value of a is "<<a<<endl;
cout << "the value of b is "<<b;

    return 0;
}





******************************************************************************TYPE CASTING***********************************************************************************
#include<iostream>
using namespace std;


int main (){
int a = 5;
float b = 5.433;

//YOU CAN TAKE ANY ONE IN BRACKET.
cout << "the value of a is "<<(float)a<<endl;
cout << "the value of b is "<<(int)b<<endl;

cout << "the value of a is "<<float(a)<<endl;
cout << "the value of b is "<<int(b)<<endl;

int c = int(b);

cout << "THE EXPRESSION IS "<<a+b<<endl;
cout << "THE EXPRESSION IS "<<a+int(b)<<endl;
cout << "THE EXPRESSION IS "<<a+(int)b<<endl;

    return 0;
}





***********************************************************CHAR EXAMPLE OF THE REFERENCE VARIABLE****************************************************************************
*********************************************************************const keyword:******************************************************************************************
Makes the variable a constant, so its value cannot be changed once it’s initialized.
Data types: You can use const with any data type (int, float, double, bool, char, etc.).

#include <iostream>
using namespace std;

int main (){

    //NOTE:YOU CAN USE THIS FOR FLOAT ALSO
    //NOTE: IF VARIABLE IS DECLARED IN SUCH A WAY THAT 
    //const int a = 5;
    char C = 'C';
    cout <<"THE VALUE OF C IS "<<C<<endl;
    C = '4';
    a = 7;//this line will not work and error will occur.
    cout <<"THE VALUE OF C IS "<<C;
    
    return 0;
}





******************************************************************MANIPULATORS -> setw(iomanip)******************************************************************************
#include <iostream>
#include <iomanip>
using namespace std;

int main (){

    int A = 5;
    int B = 34;
    int C = 3433;
    
    cout << "THE VALUE OF A IS WITHOUT setw "<<A<<endl;
    cout << "THE VALUE OF B IS WITHOUT setw "<<B<<endl;
    cout << "THE VALUE OF C IS WITHOUT setw "<<C<<endl;
    cout << endl;
    
    cout << "THE VALUE OF A WITH setw "<<setw(4)<<A<<endl;
    cout << "THE VALUE OF B WITH setw "<<setw(4)<<B<<endl;
    cout << "THE VALUE OF C WITH setw "<<setw(4)<<C<<endl;
    //MANIPULATORS:setw -> iomanip , endl -> iostream.
    //SO WE LEARNT THAT setw IS USED TO TAKE SPACES ACCORDING TO OUT NEED IF THE NUMBERS LESS THEN IT WILL CREATE SPACES BUT THE COMMOND WILL STILL BE FOLLOWED,AND THIS COMES WITH THE iomanip HEADER FILE.
    return 0;}





*************************************************************OPERATOR PRESEDENCE AND ASSOCIATIVITY***************************************************************************



C++ Operator Precedence and Associativity Chart
Precedence	               Operator(s)	                                                          Description                                           Associativity
1	                         ::	                                                                    Scope resolution	                                    Left-to-right
2	                         ++, --, +, -, !, ~, *, &, sizeof, typeid, new, delete	                Unary operators	                                      Right-to-left
3	                         .*, ->*	                                                              Pointer-to-member	                                    Left-to-right
4	                         *, /, %	                                                              Multiplication, division, modulus	                    Left-to-right
5                        	 +, -	                                                                  Addition, subtraction	                                Left-to-right
6	                         <<, >>	                                                                Bitwise shift	                                        Left-to-right
7	                         <, <=, >, >=	                                                          Relational operators	                                Left-to-right
8	                         ==, !=	                                                                Equality operators	                                  Left-to-right
9	                         &	                                                                    Bitwise AND	                                          Left-to-right
10	                       ^	                                                                    Bitwise XOR	                                          Left-to-right
11	                       `                                                                      `                                                     Bitwise OR
12	                       &&	                                                                    Logical AND	                                          Left-to-right
13	                       `		                                                                                                                        `
14                      	 ?:	                                                                    Ternary conditional	                                  Right-to-left
15	                       =, +=, -=, *=, /=, %=, <<=, >>=, &=, ^=, `	                            =`	                                                  Assignment operators
16	                       ,	                                                                    Comma operator	                                      Left-to-right

EXAMPLE
#include <iostream>
#include <iomanip>
using namespace std;

int main (){

    int A = 5;
    int B = 6;
    int C = 3;
    
    cout <<"THE SOLUTION OF THE EQUATION IS "<<((((A*B)+C)-A)+B);
    
    return 0;
}





CONTROL STATEMENTS 
THEY ARE OF THREE TYPES 
1.SEQUENCE CONTROL STRUCTURE.
2.SELECTION STRUCTURE.
3.LOOP STRUCTURE.

1.SELECTION CONTROL STRUCTURE  INSIDE THE PROGRAM
1.if-else statement
2.if-else ladder
3.switch

DIFFERENCE BETWEEN if-else and switch case statements
if-else: Use for complex or range-based conditions; it's highly flexible but can become less readable with complexity.
switch: Use for distinct values of a single variable; it's efficient and readable for well-defined cases but lacks the flexibility of if-else.





*******************************************************************************TYPES OF LOOPS********************************************************************************
THERE ARE THREE TYPES OF LOOPS 
1.FOR LOOP
2.WHILE LOOP
3.DO WHILE LOOP(it is the loop which works at least once)

SYNTAX FOR FOR LOOP
/* for (initialization ; condition ; operation){
       loop body (c++ code) */

EXAMPLE OF FOR LOOP       
#include <iostream>
using namespace std;
int main (){
    
    int a = 1;
    
    for (a = 1; a <= 40; a++){
        cout <<a<<endl;
    }
    

    return 0;
}

EXAMPLE OF FOR LOOP
#include <iostream>
using namespace std;
int main (){
    int a = 0;
    
    for (int a = 0; a <= 20 ;a++);
        cout <<"a";
        
        return 0;
}

EXAMPLE OF A INFINITE FOR LOOP
#include <iostream>
using namespace std;
int main (){
    int a = 1;
    
    for (int a = 1; 5 <= 20 ;a++)
        cout <<a<<endl;
        
        return 0;
}


SYNTAX FOR WHILE LOOP
while(condition){
  c++ statements
  i++
  }

EXAMPLE OF WHILE LOOP
#include <iostream>
using namespace std;
int main (){
    int a = 1;
    
    while (a <= 7){
        cout <<a<<endl;
        a++;
    }
        
        return 0;
}
EXAMPLE OF INFINITE WHILE LOOP
#include <iostream>
using namespace std;
int main (){
    int a = 1;
    
    while (true){
        cout <<a<<endl;
        a++;
    }
        
        return 0;
}

SYNTAX OF DO WHILE LOOP
do{
  c++ statements
  i++;
  }while(condition);

  EXAMPLE OF DO WHILE LOOP
  #include <iostream>
  using namespace std;
  int main (){
  int a = 1;
    
    do {
        cout <<a<<endl;
        a++;
    }while (a <= 7);
        
        return 0;
  }

  EXAMPLE OF INFINITE DO WHILE LOOP
  #include <iostream>
  using namespace std;
  int main (){
      int a = 1;
    
    do {
        cout <<a<<endl;
        a++;
    }while (false);
        
        return 0;
}

TABLE OF 6 USING DO WHILE LOOP
#include <iostream>
using namespace std;
int main (){
    int a = 1;
    
    do {
        cout <<"6 * " <<a<< " = " <<a*6<<endl;
        a++;
    }while (a<=10);
        
        return 0;
}





  
