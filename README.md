# roottreesol2.0

#include <bits/stdc++.h>
using namespace std;


int main()
{
    int t;
    cin>>t;
    while(t--){
        int n;
        cin>>n;
        vector<int> child(n+1);
        int x,y;
        for(int i=1;i<n;i++){
            cin>>x>>y;
            child[y]++;
        }
        int count1=0;
        for(int i=1;i<=n;i++){
            if(child[i]==0) count1++;
        }
        cout<<count1-1<<endl;
    }
}
