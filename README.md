# codechef-code
To upload codes of codechef
#include <iostream>
using namespace std;

int main() 
{int P[100],N,t,cnt,i,k,n=0,j,T,m=0,flag;
    cin>>T;
    while(m<T){
    cnt=1;
	cin>>N;
	for(i=0;i<N;i++)
	    cin>>P[i];
	for(i=1;i<N;i++)
	{   k=i;
	    t=P[i];
	    for(j=5;j>0 && k>0;j--)
	    {flag=0;
	    if(t<P[k-1]){k--;}
	    else{flag=1;break;}}
	    if(flag==0){cnt++;}
	    
	}
	
	m++;
	cout<<cnt<<endl;
    }
	return 0;
}
