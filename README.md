#include<iostream>
#include<ctime>
#include<cstdlib>
using namespace std;
int main()
{
srand(time(0));
int secretnum=rand()%100+1;
int guess;
int attempts=0;
cout<<"Try to guess the secret number "<<endl;
cin>>secretnum;
do{
cout<<"Enter your guess"<<endl;
cin>>guess;
attempts++;
if(guess==secretnum){
cout<<"congratulations!You guessed the right number in"<<attempts<<"attempts"<<endl;

}
else if(guess<secretnum){
cout<<"Try bigger number"<<endl;
}else{
cout<<"Try smaller number"<<endl;
}
}while(guess!=secretnum);
return 0;

}
