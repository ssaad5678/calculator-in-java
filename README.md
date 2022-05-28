import java.util.*;
public class SwitchExample {
	public static void main(String[] args) {
		System.out.print("Welcome to Saad's calculator");
		do {
        Scanner sc=new Scanner(System.in);
        System.out.println("Choose "
        		+ "\n1.Addition"
        		+ "\n2.Subtraction"
        		+ "\n3.Multiplication"
        		+ "\n4.Division");
        System.out.print("enter the choice:");
        int  choice=sc.nextInt();
    	switch(choice) {
    	case 1:
    		System.out.println("You have chosen addition");
    		Scanner sca=new Scanner(System.in);
    		System.out.print("enter the first number:\t");
    		int a=sca.nextInt();
    		System.out.print("enter the second number");
    		int b=sca.nextInt();
    		addition(a,b);
    		break;
    	case 2:
    		System.out.println("you have chosen subtraction");
    		Scanner sce=new Scanner(System.in);
    		System.out.println("enter the first number:\t");
    		int c=sce.nextInt();
    		System.out.println("enter the second number");
    		int d=sce.nextInt();
    		subtract(c,d);
    		break;
    	case 3:
    		System.out.println("you have chosen multiplication");
    		Scanner scf=new Scanner(System.in);
    		System.out.println("enter the first number:\t");
    		int g=scf.nextInt();
    		System.out.println("enter the second number");
    		int h=scf.nextInt();
    		multi(g,h);
    		break;
    	case 4:
    		System.out.println("you have chosen division");
    		Scanner scg=new Scanner(System.in);
    		System.out.println("enter the first number:\t");
    		int k=scg.nextInt();
    		System.out.println("enter the second number");
    		int l=scg.nextInt();
    		divi(k,l);
    		break;
    	default:
    		System.out.println("please enter correct choice");
    		break;
    	}
    }while(true);
    	
     }

static void addition(int a,int b) {
    int c=a+b;
	System.out.println("the value after addition is:"+c);
}
static void subtract(int c,int d) {
    int e=c-d;
	System.out.println("subtraction is"+e);
}
static void multi(int g,int h) {
	int f=g*h;
	System.out.println("multiplication is:"+f);
}
static void divi(int k,int l) {
	int i=k*l;
	System.out.println("division is:"+i);
}
	
}
