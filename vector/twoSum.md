## Two Sum 

Problem: Given a vector of integers and a target sum, find two numbers in the vector that add up to the target. Return the indices of the two numbers.

## Example: 

    nums = {2, 7, 11, 15}, target = 9. Output: {0, 1} (because nums[0] + nums[1] == 9).

## Solutions in c++:

    #include <iostream>
    #include <vector>
    #include <unordered_map>
    using namespace std;

    vector<int> twoSum(vector<int> n,int target){
        unordered_map<int,int> mp;
        for(int i=0;i<n.size();i++){
            int com=target-n[i];
            if(mp.count(com)){
                cout<<"result :"<<mp[com]<<","<<i<<endl;
                cout<<"result1 :"<<com<<","<<n[i]<<endl;
                return {mp[com],i};
            }
            mp[n[i]]=i;
        }
        return {};
    }
    int main() {
        cout << "Try programiz.pro"<<endl;
        vector<int> v;
        v.push_back(45);
        v.push_back(5);
        v.push_back(415);
        v.push_back(45);
        for(auto &i:v){
            cout<<i<<endl;
        }
        vector<int> result = twoSum(v,460);
        for(auto &i:result){
            cout<<i<<endl;
        }
        return 0;
    }