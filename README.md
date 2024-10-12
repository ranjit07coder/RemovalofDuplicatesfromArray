# RemovalofDuplicatesfromArray
//Program for removal of Duplicate elements from the given sorted array.
//pseudo code 
class Solution {
    public int removeDuplicates(int[] nums) {
        int j=1;
        for(int i=1;i<nums.length;i++){
            if(nums[i]!=nums[i-1]){
                nums[j]=nums[i];
                j++;    
            }
        }
        return j;
    }
  public static void main (String[] args){
      int[] nums = {1,1,2};
      removeDuplicates(int[] nums);
  }
}

//output 
// 2, [1,2]
