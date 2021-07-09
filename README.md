# Beer-and-Milky-cookies
import java.util.*;
import java.lang.*;
import java.io.*;

class BeerAndMilkyCookies
{
	public static void main (String[] args) throws java.lang.Exception
	{
	    try{
	 Scanner sc = new Scanner(System.in);
        int t = sc.nextInt();
       while (t-- > 0) {
           int n=sc.nextInt();
              String str[]=new String[n];
              for(int i=0;i<n;i++)
                  str[i]=sc.next();
              boolean a=true;
              for(int i=0;i<n-1;i++)
              {
                 if(str[i].equals("cookie") && !(str[i+1].equals("milk")))
                     {
                         a=false;
                         break;
                     }

              }
              if(str[n-1].equals("cookie"))
                  a=false;

              if(a)
                  System.out.println("YES");
              else if(!a)
                  System.out.println("NO");
                }
	    }catch(Exception e){
	        
	    }
	}
}
