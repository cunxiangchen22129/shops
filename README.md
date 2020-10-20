 
import java.util.*;
public class zuoye3 {
	public static void main(String[] args) {
		Scanner input=new Scanner(System.in);
		System.out.println("MyShopping");
		System.out.println("**********************************************");
		System.out.println("Product Number ");
		System.out.println("**********************************************");
		String choose="y";  //
		String name="";  //
		double m=0.0;    //
		double zong=0.0;  //
		double zhe=0.8;
		while(choose.equals("y")) {    //
			System.out.print("Product Number：");
			int num=input.nextInt();
			System.out.print("Purchase quantity：");
			int shu=input.nextInt();
			switch(num) {
			case 1:
				name="apple";
				m=6.0;
				break;
			case 2:
				name="orages";
				m=2.5;
				break;
			
			}
			System.out.println(name+"$"+m+"\t"+"Number"+shu+"Total"+"$"+(m*shu));  //
			zong=m*shu; //
			System.out.print("Wanna buy more（y/n）");
			choose=input.next();   //注�?
		} 
		System.out.println("Discount："+zhe);	
		System.out.println("Pay："+zong*zhe);	//
		System.out.print("Cash?：");
		double s=input.nextDouble();
		System.out.println("Change："+(s-zong*zhe));
		System.out.println("Total");   //
  }
}
