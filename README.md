# check-palidrome
#include<iostream>
using namespace std;
bool re(char name[],int n)
{
	int s=0;
	int e=n-1;
	while(s<=e)
	{
		if(name[s] != name[e])
		{
			return 0;
		}
		else
		{
			s++;
			e--;
		}
		
	}
	return -1;
}

int Length(char name[])
{
	int c=0;
	for(int i=0;name[i] !='\0';i++)
	{
		c++;
	}
	return c;
}
int main()
{
	char name[20];
	cin>>name;
	cout<<name<<endl;
	cout<<"Length of name is"<<endl;
	int len=Length(name);
	
	cout<<len<<endl;
	cout<<"check paildrome"<<re(name,len);

}
