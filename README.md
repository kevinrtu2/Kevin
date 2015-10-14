# Kevin
public class Frequency
{
   /**
      Returns an array of the frequencies of each element in a.
      That is, if the returned array is f, then a[i] occurs f[i]
      times in a.
      @return the frequency array
      Example of how it works: given a new list of size 5 with elements [1, 3, 5, 3, 4]
      Goes through the list and if one element is equal to another, you add to count
      So if you check for 1 and see that 1 == 1 only once, there is only 1 to count
      Same process with 3 except you see 3 == 3 twice, so count == 2;
      same Process with 5 and count == 2;
   */
   public static int[] frequencyOfElements(int[] a)
   {
      int[] list = new int[a.length];
      for (int i = 0; i < a.length; i++)
      {
    	  int count = 0;
    	  for (int j = 0; j < a.length; j++)
    	  {
    		  if (a[i] == a[j])
    		  {
    			  count++;
    		  }
    	  }
    	  list[i] = count;
      }
      return list;
   }
}
