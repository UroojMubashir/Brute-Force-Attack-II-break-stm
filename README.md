#include <iostream>


using namespace std;


int main()
{
    int count=5;
    string passcode="123@Abc.";
    
    while(true){
        string userpasscode;
        cout<<"\nEnter password: ";
        cin>>userpasscode;
        
        if (passcode==userpasscode){
            cout<<"\nCorrect password.";
            break;
        }
        else{
            count--;
            
            if (count==0){
                cout<<"\nIncorrect password. The authorities have been alerted! ";
                break;
            }
            else{
               cout<<"\nIncorrect password. You have "<<count<<" attempts remaining!"; 
            }
        }
    }


    return 0;
}
