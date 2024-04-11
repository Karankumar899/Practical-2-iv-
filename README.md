# Practical-2-iv-
#include<iostream>
using namespace std;

int main()
{
    int x[110],n,i,j,temp;
    cout<<"Enter The No of Limit : ";
    cin>>n;
 
    cout<<"Enter Value :"<<endl;
    for(i=0;i<n;i++)
    {
        cin>>x[i];
    }
 
    for(i=0;i<n;i++)
    {
        for(j=i+1;j<n;j++)
        {
            if(x[i]>x[j])
            {
                temp=x[i];
                x[i]=x[j];
                x[j]=temp;
            }
        }
    }
 
    cout<<"Sorted Array is : "<<endl;
    for(i=0;i<n;i++)
    {
        cout<<x[i]<<endl;
    }
    return 0;
}
