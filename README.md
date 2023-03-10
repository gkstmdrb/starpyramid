# starpyramid

### 별 피라미드

package project;
import java.util.Scanner;
public class dowhile {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		
		int n;
		int i=0;
		
		
		
		System.out.print("몇 단 피라미드입니까?: ");
		Scanner sc = new Scanner(System.in);
		n = sc.nextInt();
		
		for (i=1; i<=n; i++) { 
			for (int k=1; k<=n-i; k++) { //n(입력받은 값)-i만큼 공백 띄우기
				System.out.print(" ");
			}
			
			for (int j=1; j<=i*2-1; j++) { //ix2-1개만큼 별 출력
				System.out.print("*");
			}	
			System.out.println(""); //n만큼 줄 띄우기
		}
	}

}
