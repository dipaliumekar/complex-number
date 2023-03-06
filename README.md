# complex-number
package java;

import java.util.Scanner;

class Comp {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		//int ch=0;
        float n1,n2;
        Comp_Op cal= new Comp_Op();
        Scanner input = new Scanner(System.in);
        System.out.print("Enter first no.\n");
        n1=input.nextFloat();//real part
        n2=input.nextFloat();//imaginary part
        Comp_Op Object1= new Comp_Op(n1,n2);
        System.out.print("Enter thr second no.\n");
        n1=input.nextFloat();//real
        n2=input.nextFloat();//imaginary
        Comp_Op Object2=new Comp_Op(n1,n2);
        cal.AddNum(Object1,Object2);
        cal.SubNum(Object1,Object2);	
        

	}

}
 class Comp_Op
 {
	 float real,imag;
	 Comp_Op() //default constructor
	 {
		 real=0;
		 imag=0;
	 } 
	 
	 Comp_Op(float comp1,float comp2) //parameterized constructor
	 {
		 real=comp1;
		 imag=comp2;
	 }
	 public void AddNum(Comp_Op c1,Comp_Op c2)
	 {
		 float real,imag;
		 real=(c1.real+c2.real);
		 imag=(c1.imag+c2.imag);
		 System.out.println("Answer is:("+real+")+("+imag+")i");
		 
	 }
	 public void SubNum(Comp_Op c1,Comp_Op c2)
	 {
		 float real,imag;
		 real=(c1.real-c2.real);
		 imag=(c1.imag-c2.imag);
		 System.out.println("Answer is:("+real+")-("+imag+")i"); 
	 }

	 }
	 
 
