
class Solution
{
    public boolean findPair(int arr[], int size, int n)
    {
        //code here.
        ///sort->2 3 5 5 20 80
        Arrays.sort(arr);
        for(int i=0;i<arr.length-1;i++)
        {
            for(int j=i+1;j<arr.length;j++)
            {
                if(arr[j]-arr[i]==n)
                {
                    return true;
                }
            }
        }
        return false;
    }
}
