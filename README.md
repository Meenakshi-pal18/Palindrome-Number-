# Palindrome-Number-
class Solution {
public:
    bool isPalindrome(int x) {
        long long res=0;
        int dup=x;
        while(x>0){
            int id=x%10;
            res=res*10+id;
            x=x/10;
        }
        if(dup==res){
           return true;
        }
       else{
        return false;
       }
    }
};
