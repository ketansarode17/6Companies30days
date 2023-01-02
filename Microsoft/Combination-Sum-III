class Solution {
    private:
    vector<vector<int>>ans;
    vector<int>temp;
    void generatePermutations(int num,int k,int n)
    {
        if(n<0)return;
        if(k==0)
        {
            if(n==0){ans.push_back(temp);}
            return;
        }
        for(int i=num;i<=9;i++)
        {
            temp.push_back(i);
            generatePermutations(i+1,k-1,n-i);
            temp.pop_back();
        }
    }
public:
    vector<vector<int>> combinationSum3(int k, int n) {
        generatePermutations(1,k,n);
        return ans;
    }
};
