# 下樓梯
    /ex:輸入 4
    輸出 _
	  |_
	    |_
	      |_
		|_
# 作法
```
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Floor
{
    class Program
    {
        static void Main(string[] args)
        {
            int num;
            Console.Write("輸入階梯數:");
            num = int.Parse(Console.ReadLine());
            for(int k=1;k<=num;k++)
            {
                Console.WriteLine("_");
                for(int i =1;i<=k;i++)
                {    
                    if(i==1)
                    {
                        Console.Write(" ");
                    }
                    else
                    {
                        Console.Write("  ");      
                    }                               
                }                
                Console.Write("|");
                if(k == num)
                {
                    Console.Write("_");
                }
            }            
            Console.ReadKey();
        }
    }
}
```
