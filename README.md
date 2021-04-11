# Java_Day01
자바(Java) 프로그래밍 초급과정 1일차

ex01
package ex01;

/*
 * 작성자: 박민지
 * 작성일: 2021.04.10
 */


public class First {
	public static void main(String ar[]) {
		System.out.println("Hello Java!!");//출력해라.
	}
}

package ex01.ex02;

public class Second {
	public static void main(String ar[]) {
		//숫자, 문자, 날짜
		int num; //정수형 숫자 //변수 선언
		num=10;//double, float //초기화(=값을 설정했다)
		
		int num1=20; //변수 선언과 초기화를 동시에 했음
		
		int num2=1, num3=2, num4=0; //한줄에 여러개 넣어도 가능(제약없음)
		
		int result=num+num1; //대입연산자
		// 3+5=6
		System.out.println("덧셈결과 : "+result);//결합연산(=연결연산자)- 숫자는숫자랑, 문자는문자랑
	}
}

ex02
package test;

public class Ex01 {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		//long(8byte) > int(4byte) > short(2byte) > byte(1byte)
		//double(8byte) > float(4byte)

		int age;
		double //(=float) value;
		value=age=1; //= value=age=(int)1.0; (int)가 강제변환
		System.out.println(value);
		String str; // _,$
		
		//save() x, run1() o
		
		String first, First; //둘은 아예 다른변수
	}

}

package test;

public class P50 {
	public static void maiin(String ar[]) {
		//boolean(true, false), -를 판단할수 있는것, char(2byte), 
		//public(=폴더안의 폴더) > protected(=폴더안에 있는 파일까지만) > default > private
		//class, abstract(추상), interface, extends,  implements, enum
		//new(=예약어), instanceof, this, super, null(비워있는값, 알수없는 값)
		//void(=출력하지 않겠다!!!), return
		//제어문(조건문) - if, else, switch, case, default, for, do, while, break, continue
		//true, false
		//try, catch, finally, throw, throws
		//package, import, synchronized, final, static(공유할때 쓰는 개념)		
		
	}

	void sum(){

	}
}

ex03
package p53;

public class VarEx {
	public static void main(String ar[]) {
		//세공간을 만들고, 각 값을 입력한 다음 값의 위치를 바꾸는 방법 
		int x=3, y=5;
		int temp;
		temp=x;
		x=y;
		y=temp; //같다라는 뜻은 ==, =은 대입(왼->오)
		
		
		//x=y; //x가 결과, 항상 오른쪽에서 왼쪽으로
		System.out.println("x값 :"+x+", y값 : "+y);
		
	}

}

ex04
package p55;

public class VarScope {
	public static void main(String ar[]) {
		int v1=15;
		
		boolean bool=true;
		
		if(bool)
			System.out.println("참");
			
		if(2>1)
			System.out.println("참");
		
		else System.out.println("거짓"); //{}중가로와 ;의 중요성 복습!
			
		
	}	
	
	boolean isEmpty() {
		return true;
	}
}

package p61;

public class IntLiter {
	public static void main(String ar[]) {
		int var1=0b1011; //2진수 -> 알파벳b 사용
		int var2=0206; //02부터면 8진수
		int var3=365; //십진수 (일반적인 숫자=정수)
		int var4=0xB3; //16진수
		
		System.out.println("이진수(1011) :"+var1);
	}
}

package p62;

public class LongEx {
	public static void main(String ar[]) {
		long var1=10L;
		long var2=20L;
		long var3=10000000000L; //정수의 범위를 넘으면 인식x 그래서 L을 붙여야된다
		float f1=1.1f; //일반적으로 정밀도를 위해 double을 많이씀, 메모리가 작은 float를 쓸때 f사용
		double d1=1.1;
	}

}

package p64;

public class UniEx {
	public static void main(String ar[]) {
		char c1='a';  //" " 사용 -> 문자열(string), character는 문자라서 -> ' '사용
		//문자는 양의범위(unsigned)만 가진다
		int num;
		num=c1; //"숫자 :"+num => 97<accii 코드표>
		c1=(char)num; //num(3)을 c1(2)에 넣어야 되기 때문에 (char)을 써서 문자로 변환
		//유니코드!!
		
		System.out.println("숫자 : "+c1); //c1대신에 num 넣으면 결과는 97나옴
	}
}


package p66;

public class EscapeEx {
	public static void main(String ar[]) {
		System.out.println("번호\t이름\t직업");
		
		//p.69
		boolean stop=false;
		
		if(stop) {
			System.out.println("중지합니다.");
		}else {
			System.out.println("시작합니다.");
		}
	}
}

package p73;

public class promotionEx {
	public static void main(String ar[]) {
		byte byteValue=10;
		int intValue=byteValue; //unsigned
		short shortValue;
		
		//Casting
		char charValue='가';
		shortValue=(short)charValue; //short가 음수범위를 가지고 있기에 오류나서 강제형변화해주어야한다
		//intValue=charValue;
	}
}

package p76;

public class ByteOperationEx {
	public static void main(String ar[]) {
		byte num1=10;
		byte num2=20;
		//byte result=num1+num2;//저장공간끼리 연산을 해버리면 byte가 자동으로 int로 바뀜 그래서 오류뜸
		//그래서 byte result=(byte)(num1+num2); 이렇게 하면 가능(배운곳까지)
		//num1+num2 은 저장공간(이미값이있는)끼리의 연산 *한번더 복습!
		System.out.println("답");
		
		
		//p.80 code
		int x=1;
		int y=2;
		//double result = x/y; //정수 범위에서 0.5는 포함이 안되기 때문에 0.0이 나옴
		double result=(double)x/y; //그래서 double을 씌워줘야된다.
		System.out.println("실수 결과값: "+result); 
		
		System.out.println(y+"123"); //"123"이 문자열이여서 결과가 2123으로 나옴
	}
}

