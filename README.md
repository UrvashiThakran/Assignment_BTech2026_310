# Assignment_BTech2026_310

# Coding Questions :27.01.25

OOPS:

Problem Statement:

Ques1:Area and Circumference of circle

Ques 2:Get Model,Year and Company name using getter and setter methods.

Platform Used:Programiz

Code1:

Code 2:

DBMS:

Platform Used:LeetCode

 Ques 1:Dublicate Emails

 Ques 2:Customer  who never order

 Code 1:

SELECT email
FROM Person
GROUP BY email
HAVING COUNT(email)>1

Code 2:

SeLECT name as Customers
From Customers
where id not in(select customerId from Orders)

DSA:

 Ques 1:IsPallindrome

 Ques 2:Remove duplicate element fron sorted array.

 Ques 3:Remove element


Platform Used:LeetCode

 Code 1:
 
class Solution 
{
public:
    bool isPalindrome(int x)
    {
        int num;
        long rev=0;
        int temp=x;
        if(x<0)
        {
           return false;
        }
        while(x!=0)
        {
          num=x%10;
          rev=(rev*10)+num;
          x=x/10;
        }
        if(rev==temp)
        {
          return true;
        }
        else
        {
        return false;
        }
    }
};


Code 2:

class Solution
{
public:
    int removeDuplicates(vector<int>& nums) 
    {
        int j=1;
        for(int i=1;i<nums.size();i++)
        {
           if(nums[i]!=nums[i-1])
           {
            nums[j]=nums[i];
            j++;
           }
        }
        return j;
    }
};

Code 3:

class Solution 
{
public:
    int removeDuplicates(vector<int>& nums) 
    {
        int j=1;
        for(int i=1;i<nums.size();i++)
        {
           if(nums[i]!=nums[i-1])
           {
            nums[j]=nums[i];
            j++;
           }
        }
        return j;
    }
};


