# dsa9
# kadane's algorithm
#  Find the contiguous sub-array(containing at least one number) which has the maximum sum and return its sum.
gfg

long maxSubarraySum(int arr[], int n){
        
        // Your code here
        int csum=arr[0];
        int osum=arr[0];
        for(int i=1;i<n;i++)
        {
            if(csum>0)
            csum+=arr[i];
            else 
            csum=arr[i];
            if(csum>osum)
            osum=csum;
            
        }
        return osum;
    }
