# ArraysLab
This project required the creation of different methods related to reading arrays and calculating the values within in different ways.

# public static int[] sum(int[] arr1, int[] arr2) {
		int[] arrSum = new int[arr1.length]; 
		for(int i = 0;i < arr1.length;i++)
			 arrSum[i] = arr1[i]+arr2[i];
		return arrSum;		
	}
traverses the array with a for loop and adds each value together
  
# public static int[] append(int[] arr, int num) {
		int[] arrAppend = new int[arr.length+1];
		for (int i = 0; i<arr.length; i++) {
			arrAppend[i] = arr[i];
		}
		arrAppend[arrAppend.length-1] = num; 
		return arrAppend;
	}
Creates a new, appended array and returns it.  

# public static int[] remove(int[] arr, int idx) {
		int[] arrRemove = new int[arr.length-1];
			for(int i = 0; i<arr.length-1; i++) {
				if(i >= idx) {
					arrRemove[i] = arr[i+1]; 
				}else {
					arrRemove[i] = arr[i];
				}
			}
		return arrRemove;
	}
 traverses the array and adds values to a new array. When the index of idx is being evaluated, the next value is added to the array instead.

	public static int sumEven(int[] arr) {
		int even = 0;
		for(int i = 0;i<arr.length;i++) {
			if(i%2==0) {
				even+=arr[i];
			}
		}
		return even;
	}
 traverses the array and adds only the even numbers to a running value which is then returns at the end.
 
This project taught us how to manage arrays and manipulate their contents. 
