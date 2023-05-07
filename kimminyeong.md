 **hello world 출력**
 
 public class HelloworldApp {
	 public static void main(String[] args) {
		 System.out.println("Hello World!!");
	 }
 }

**데스크톱 어플리케이션 만들기**

import javax.swing.*;   
 import java.awt.Dimension;
 import java.awt.Toolkit;
 public class HelloworldApp{
     public static void main(String[] args){
         javax.swing.SwingUtilities.invokeLater(new Runnable() {
             public void run() {
                 JFrame frame = new JFrame("HelloWorld GUI");
                 frame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
                 frame.setPreferredSize(new Dimension(400, 300));
                 JLabel label = new JLabel("Hello World!!", SwingConstants.CENTER);
                 frame.getContentPane().add(label);
                 Dimension dim = Toolkit.getDefaultToolkit().getScreenSize();
                 frame.setLocation(dim.width/2-400/2, dim.height/2-300/2);

                 frame.pack();
                 frame.setVisible(true);
             }
         });
     }
 }

 **데이터 타입**

 public class Datatype{
	public static void main(String[] args) {
		System.out.prinln(6);//Number
		System.out.println("six");//String
		
		System.out.println("6");//String6
		
		System.out.println(6+6);//12
		System.out.println("6+6")//66
		
		System.out.println(6*6);//36
		//System.out.println("6*6");//
		
		System.out.println("1111".length());//4
		System.out.println(1111.length());
	}
}

**연산**

public class Number {

	public static void main(String[] args) {
		
		System.out.println(6 + 2); //8
		System.out.println(6 - 2); //4
		System.out.println(6*2); //12
		System.out.println(6/2); //3
	}

}

**문자열**

public class StringApp {

	public static void main(String[] args) {
		
		System.out.println("Hello world"); //String
		System.out.println('H'); //Character
		System.out.println("H");
		
		System.out.println("Hello"
				+ " World");
		//new line
		System.out.println("Hello\nWorld"); 
		//escape
		System.out.println("Hello \"World\""); //Hello"World"
		
	}

}

**문자열2**

public class StringOperation {

	public static void main(String[] args) {
		
		System.out.println("Hello World".length()); //11
		System.out.println("Hello,[[[name]]]...bye.".replace("[[[name]]]", "duru"));

	}

}
