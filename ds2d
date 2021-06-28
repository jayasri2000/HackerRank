#include <bits/stdc++.h>

using namespace std;

int ar[6][6];
int row=0;
int col=0;

int hourglass(int a,int b,int max){
    if(row==4)
    return max;
    else if(col==4){
    row++;
    col=0;    
    a=row;
    b=col;
    }
    
    int s=0;
    for(int i=a;i<a+3;i++)
    {
        if(i==a+1){
            s=s+ar[i][b+1];
            i++;
            }
        for(int j=b;j<b+3;j++){
            
            s=s+ar[i][j];
            
        }
        
    }
    if(s>max)
        max=s;
    
    col++;
    int result=hourglass(row,col,max);
    return result;
}
int main()
{
    for(int i=0;i<6;i++){
        for(int j=0;j<6;j++){
            cin>>ar[i][j];
        }
    }
    cout<<hourglass(row,col,0);
    return 0;
}
