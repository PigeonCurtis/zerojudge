#include <iostream>
#include <vector>
using namespace std;
int main() {
    int n,a,b,c;
    cin>>n;
    for(int i=0;i<n;i++){
        cin>>a>>b>>c;
        vector <int>v;
        for(int j=a+1;j<b;j++){
            if(j%c != 0)
                v.push_back(j);
            else
                continue;
        }
        if (v.size() == 0)
            cout << "No free parking spaces.";
        else{
            for(int j = 0;j < v.size();j++){
                cout << v[j] << ' ';
            }
        }
        cout<<'\n';
    }
}
