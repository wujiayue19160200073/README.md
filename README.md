//student-id:19160200073
public class Fibonacci
{
    public static void main(String[] args)
    {
        int of,i=0;
        do
        {
            i=1+i;
            of=Fibonacci.of(i);
            System.out.printf("Fibonacci.of(%d)==%d\n",i,of);
        }while(of>=200);
     }
    public static int of(int n)
    {
        if(n==1|n==2)
            return 1;
        else if(n>2)
            {
                int a=1,b=1,temp=0;
                for(int i=0;i<n-2;i++)
                    {
                        temp=a+b;
                        a=b;
                        b=temp;
                    }
                    return temp;
                }
                else
                return -1;
            }
    }
}