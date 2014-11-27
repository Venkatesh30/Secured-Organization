/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */

/**
 *
 * @author Venkatesh
 */
import java.util.*;
public class info_sec_prj {
    static HashMap hm = new HashMap();
    static List<String> l1 = new ArrayList<String>();
    static List<String> l2 = new ArrayList<String>();  
    static List<String> l3 = new ArrayList<String>();
    static List<String> l4 = new ArrayList<String>();
    static List<String> l5 = new ArrayList<String>();
    static String[] access={"Read","Write","Update","Insert","Delete","Full"};
    static double[] ctrs_ind=new double[50];
    static double[] ctrs_WU=new double[50];
    static double[] ctrs_WI=new double[50];
    static double[] ctrs_RW=new double[50];
    static double[] ctrs_UD=new double[50];
    static double[] ctrs_RU=new double[50];
    static double[] ctrs_ID=new double[50];
    static double[] ctrs_RD=new double[50];
    static double[] ctrs_WD=new double[50];
    static double[] ctrs_RWD=new double[50];
    static double[] ctrs_RWU=new double[50];
    static double[] ctrs_WUD=new double[50];
    static double[] ctrs_WUI=new double[50];
    static int pairs = 13;
    public static void main(String[] args) {
        create();
        System.out.println("Director   : "+hm.get("Director"));
        System.out.println("Manager    : "+hm.get("Manager"));
        System.out.println("Accountant : "+hm.get("Accountant"));
        System.out.println("Cashier    : "+hm.get("Cashier"));
        System.out.println("Clerk      : "+hm.get("Clerk"));
        System.out.println("");
        for(int i=0;i<50;i++)
        {
            double max=0;
            String pair="";
            check_1(i);
            if(ctrs_ind[i]>max)
            {
                max=ctrs_ind[i];
                pair="Individual Assignment";
            }                
            check_2_WU(i);
            if(ctrs_WU[i]>max)
            {
                max=ctrs_WU[i];
                pair="Write Update Pair";
            }                
            WI.WI_pair(i);
            if(ctrs_WI[i]>max)
            {
                max=ctrs_WI[i];
                pair="Write Insert Pair";
            }
            RW.RW_pair(i);
            if(ctrs_RW[i]>max)
            {
                max=ctrs_RW[i];
                pair="Read Write Pair";
            }
            UD.UD_pair(i);
            if(ctrs_UD[i]>max)
            {
                max=ctrs_UD[i];
                pair="Update Delete Pair";
            }
            RU.RU_pair(i);
            if(ctrs_RU[i]>max)
            {
                max=ctrs_RU[i];
                pair="Read Update Pair";
            }
            ID.ID_pair(i);
            if(ctrs_ID[i]>max)
            {
                max=ctrs_ID[i];
                pair="Insert Delete Pair";
            }
            RD.RD_pair(i);
            if(ctrs_RD[i]>max)
            {
                max=ctrs_RD[i];
                pair="Read Delete Pair";
            }
            WD.WD_pair(i);
            if(ctrs_WD[i]>max)
            {
                max=ctrs_WD[i];
                pair="Write Delete Pair";
            }
            RWD.RWD_pair(i);
            if(ctrs_RWD[i]>max)
            {
                max=ctrs_RWD[i];
                pair="Read Write Delete Pair";
            }
            RWU.RWU_pair(i);
            if(ctrs_RWU[i]>max)
            {
                max=ctrs_RWU[i];
                pair="Read Write Update Pair";
            }
            WUD.WUD_pair(i);
            if(ctrs_WUD[i]>max)
            {
                max=ctrs_WUD[i];
                pair="Write Update Delete Pair";
            }
            WUI.WUI_pair(i);
            if(ctrs_WUI[i]>max)
            {
                max=ctrs_WUI[i];
                pair="Write Update Insert Pair";
            }
            System.out.println("Interation "+(i+1)+" has max accuracy of "+max+" for "+pair);
            //System.out.println(getmax(i));
            //System.out.println(ctrs_ind[i]+" "+ctrs_WU[i]+" "+ctrs_WI[i]);
        }        
        compute.comp();
    }
    static void getmax(int i)
    {
        
    }
    static void create()
    {
        l1.add("Read");
        l1.add("Write");
        l1.add("Insert");
        l1.add("Update");
        l1.add("Delete");
        l1.add("Full");
        l2.add("Read");
        l2.add("Write");
        l2.add("Insert");
        l2.add("Update");
        l2.add("Delete");
        l3.add("Read");
        l3.add("Write");
        l3.add("Update");
        l3.add("Delete");
        l4.add("Read");
        l4.add("Write");
        l4.add("Update");
        l4.add("Write");
        l4.add("Insert");
        l5.add("Write");
        l5.add("Insert");
        hm.put("Director",l1);
        hm.put("Manager",l2);
        hm.put("Accountant",l3);
        hm.put("Cashier",l4);
        hm.put("Clerk",l5);
    }
    static void check_1(int z)
    {
        //System.out.println("Individual Assignments");
        double ctr=0;
        for(int i=0;i<12;i++)
        {
            List<String> l6 = new ArrayList<String>();
            for(int j=0;j<6;j++)
            {
                double random = Math.random();
                if(random>0.5)
                {
                    //System.out.print(access[j]+" ");
                    l6.add(access[j]);
                }                    
            }
            //System.out.println(l6);
            if(i==0 || i==5)
            {
                if(l1.containsAll(l6))
                    ctr++;
            }
            else if(i==1 || i==6)
            {
                if(l2.containsAll(l6))
                    ctr++;
            }
            else if(i==2 || i==7)
            {
                if(l3.containsAll(l6))
                    ctr++;
            }
            else if(i==3 || i==8 || i==10)
            {
                if(l4.containsAll(l6))
                    ctr++;
            }
            else if(i==4 || i==9 || i==11)
            {
                if(l5.containsAll(l6))
                    ctr++;
            }
            //System.out.println("");
        }
        //System.out.println(ctr);
        double percent=(ctr/12)*100;
        //System.out.println(percent);
        ctrs_ind[z]=percent;
    }
    static void check_2_WU(int z)
    {
        //System.out.println("Write Update Pair");
        double ctr=0;
        for(int i=0;i<12;i++)
        {
            List<String> l6 = new ArrayList<String>();
            for(int j=0;j<6;j++)
            {
                double random = Math.random();
                if(random>0.5)
                {
                    if(j==1||j==2)
                    {
                        //System.out.print(access[j+1]+" ");
                        l6.add(access[j]);
                        l6.add(access[j+1]);
                    }
                    //System.out.print(access[j]+" ");
                    else
                    {
                        l6.add(access[j]);
                    }
                    //l6.add(access[j]);
                }                    
            }
            HashSet hs = new HashSet();
            hs.addAll(l6);
            l6.clear();
            l6.addAll(hs);
            //System.out.println(l6);
            if(i==0 || i==5)
            {
                if(l1.containsAll(l6))
                    ctr++;
            }
            else if(i==1 || i==6)
            {
                if(l2.containsAll(l6))
                    ctr++;
            }
            else if(i==2 || i==7)
            {
                if(l3.containsAll(l6))
                    ctr++;
            }
            else if(i==3 || i==8 || i==10)
            {
                if(l4.containsAll(l6))
                    ctr++;
            }
            else if(i==4 || i==9 || i==11)
            {
                if(l5.containsAll(l6))
                    ctr++;
            }            
        }
        //System.out.println(ctr);
        double percent=(ctr/12)*100;
        //System.out.println(percent);
        ctrs_WU[z]=percent;
    }
}
