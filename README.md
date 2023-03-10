# starpyramid

### 별 피라미드

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		
		int n;
		int i=0;
		
		
		
		System.out.print("몇 단 피라미드입니까?: ");
		Scanner sc = new Scanner(System.in);
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

}
