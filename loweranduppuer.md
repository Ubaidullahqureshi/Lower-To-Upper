#include<iostream>
#include<ctype.h>
#include<stdlib.h>
using namespace std;
	//Declare the function prototype 
	void convertToUppercase ( char * );
		int main(){
			char s [ 11 ] = "Ubaidullah";
			cout << "The String before conversion is : " << s << '\n';
			
			//Function call
			convertToUppercase( s );
			cout << "The String after conversion is" << s;
		}
		
		void convertToUppercase ( char *sptr){
			while ( *sptr != '\0' ){
				if ( islower ( *sptr ) )
					*sptr = toupper ( *sptr );   // Convert To uppercase
				++sptr;							// move sptr to next character
			}
		}
