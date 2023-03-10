# starpyramid

### 별 피라미드

스캐너를 불러와 사용자가 입력한 값 만큼 별을 출력 할 수 있도록 한다.

n은 사용자가 입력한 값이고, i는 for문을 반복하는 횟수이다. 이 2중으로된 3개의 for문에서 가장 큰 틀이 되어 i<=n, i는 n보다 작거나 같으므로 입력한 값 만큼의 줄 수가 되어준다.

하위 for문의 k방을 생성하여 n-i, 입력받은 값과 현재 i번째줄을 빼주므로 n-i만큼의 공백을 띄워준다.

n-i만큼의 공백을 띄운 후 별의 갯수를 ix2-1, 현재 i번째줄x2-1을 해줌으로써 별 피라미드를 별 1개,3개,5개...씩 사용자가 입력 한 값만큼 출력해준다.

k만큼의 공백과 j만큼의 별을 출력한 후 줄을 한 칸 내려준다.

이 작업을 n번만큼 반복한다.

![image](https://user-images.githubusercontent.com/114748816/224201165-549a7511-dc4e-4481-98a4-7e93e93aa1e1.png)

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		
		int n;
		int i=0;
		
		
		
		System.out.print("몇 단 피라미드입니까?: ");
		Scanner sc = new Scanner(System.in);			//입력한 값 만큼의 피라미드를 출력할 수 있도록 Scanner를 불러옴
		n = sc.nextInt();			
		
		for (i=1; i<=n; i++) { 
			for (int k=1; k<=n-i; k++) { 			//k=1, n(입력받은 값)-i만큼 공백 띄우기, k값 증가
				System.out.print(" "); 			//공백띄우고 위 for로 돌아가기
			}	 		     			//k값이 n-i보다 커졌으므로 별 출력
			
			for (int j=1; j<=i*2-1; j++) {			// j=1, ix2-1개만큼 별 출력, j값 증가
				System.out.print("*"); 			// 별 출력 후 위 for로 돌아가기
			}			       			// j값이 ix2-1보다 커졌으므로 줄 내리기
			System.out.println(""); 			//n만큼 줄 내리기
		}
	}
