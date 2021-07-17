# Linkedlist
import java.util.*;
public class linkedlist
{ 
   public static void main(String args[])
   {
     Scanner sc=new Scanner(System.in);
      int n;
     LinkedList<Integer>A=new LinkedList<Integer>();
     System.out.println("Enter the n :");
       n=sc.nextInt();
     System.out.println("enter n values:");
     for(int i=0;i<n;i++)
    {
        int m;
      m=sc.nextInt();
      A.add(m);
    }
      System.out.println("Enter the value:");
      int  value=sc.nextInt();
    boolean ans = A.contains(value);
    if(ans)
   {
      int index=A.indexOf(value);
      A.remove(index);
       System.out.println(A);
   }
      else
   System.out.println("Element not found");
   }
}
