#include<iostream>
using namespace std;
int main(){
		int a,temp;
	
		cout<<"enter the size of arry";
	cin>>a;
	int arr[a];
	for(int i=0;i<a;i++)
	{
		cout<<"enter element "<<i+1<<" ";
		cin>>arr[i];
	}
	for(int j =0;j<a;j++)
	{
		for(int k=(j+1);k<a;k++)
		{
			if(arr[j]>arr[k])
			{
				temp=arr[j];
				arr[j]=arr[k];
				arr[k]= temp;
			}
		for(int i=0;i<a;i++)
		{
			cout<<arr[i]<<"|";
			}
		cout<<endl;		
		}
	}
		cout<<"sorted"<<endl;
	for(int i =0;i<a;i++)
	{
		cout<<arr[i]<<"|";
	}
	return 0;

}
