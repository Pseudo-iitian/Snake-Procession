// # Snake-Procession
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int r,l;
	string s;
	cin>>r;
	for(int i=0;i<r;i++){
	    cin>>l;
	    cin>>s;
	    int count=0,flag=1;
	    for(int j=0;j<l;j++){
	        if(s.at(j)=='H'){
	            count++;
	        }
	        else if(s.at(j)=='T'){
	            count--;
	        }
	        if(count<0 || count>1){
	            break;
	        }
	    }
	    if(count==0){
	        cout<<"Valid"<<endl;
	    }
	    else{
	        cout<<"Invalid"<<endl;
	    }
	}
	return 0;
}
