import java.util.*;
class EXPSubscriptions{
    Scanner sc=new Scanner(System.in);
    public int TO()
    {
        int to[]={3,3,3,3,3,5,6};
        int i,Tot=0;
        
        
        for(i=0;i<7;i++)
        {
            Tot=Tot+to[i];
        }
        return Tot;
    }
    public double ExpHindu()
    {
        double Hint=0,Hindu[]={2.5,2.5,2.5,2.5,2.5,4,4};
        int i;
        
        for(i=0;i<7;i++)
        {
            Hint=Hint+Hindu[i];
        }
        return Hint;
    }
    public int ET()
    {
        int Et[]={4,4,4,4,4,4,10};
        int i,Ett=0;
        
        for(i=0;i<7;i++)
        {
            Ett=Ett+Et[i];
        }
        return Ett;
    }
    public double ExpBm()
    {
        double Bmt=0,Bm[]={1.5,1.5,1.5,1.5,1.5,1.5,1.5};
        int i;
        
        for(i=0;i<7;i++)
        {
            Bmt=Bmt+Bm[i];
        }
        return Bmt;
    }
    public int HT()
    {
        int Ht[]={2,2,2,2,2,4,4};
        int i,Htt=0;
        for(i=0;i<7;i++)
        {
            Htt=Htt+Ht[i];
        }
        return Htt;
    }
    public static void main(String args[])
    {
        EXPSubscriptions ms=new EXPSubscriptions();
        int In;
        Scanner sc=new Scanner(System.in);
        In=sc.nextInt();
        if(ms.TO()+ms.ExpHindu()<=In)
        {
            System.out.println("{'toi','hindu'}");
        }
        if(ms.TO()+ms.ET()<=In)
        {
            System.out.println("{'toi','et'}");
        }
        if(ms.TO()+ms.ExpBm()<=In)
        {
            System.out.println("{'toi','bm'}");
        }
        if(ms.TO()+ms.HT()<=In)
        {
            System.out.println("{'toi','ht'}");
        }if(ms.ExpHindu()+ms.ET()<=In)
        {
            System.out.println("{'hindu','et'}");
        }
        if(ms.ExpHindu()+ms.ExpBm()<=In)
        {
            System.out.println("{'hindu','bm'}");
        }
        if(ms.ExpHindu()+ms.HT()<=In)
        {
            System.out.println("{'hindu','ht'}");
        }
        if(ms.ET()+ms.ExpBm()<=In)
        {
            System.out.println("{'et','bm'}");
        }
        if(ms.ET()+ms.HT()<=In)
        {
            System.out.println("{'et','ht'}");
        }
        if(ms.ExpBm()+ms.HT()<=In)
        {
            System.out.println("{'bm','ht'}");
        }
        
        
    }
}
