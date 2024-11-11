#include <bits/stdc++.h>
using namespace std;

int main() {
	string name1,name2;
	getline(cin,name1);
	getline(cin,name2);
	for(int i=0;i<name1.size();i++)
	{
	    for(int j=0;j<name2.size();j++)
	    {
	        if(name1[i]==name2[j])
	        {
	            name1[i] = '*';
	            name2[j] = '*';
	        }
	    }
	}
	int count = 0;
	for(int i=0;i<name1.size();i++)
	{
	    if(name1[i]==' ')
	    {
	        continue;
	    }
	    if(name1[i] != '*')
	    {
	        count++;
	    }
	}
	for(int j=0;j<name2.size();j++)
	{
	    if(name2[j]==' ')
	    {
	        continue;
	    }
	    if(name2[j] != '*')
	    {
	        count++;
	    }
	}
	vector<char> flames = {'F','L','A','M','E','S'};
	int i=0;
	while(flames.size() > 1)
	{
	    i = (i+count-1)%flames.size();
	    flames.erase(flames.begin()+i);
	}
	cout << flames[0] << " ";
}
