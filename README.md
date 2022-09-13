# Recursion
# prints sum of n natural numbers

public class Recursions{
	public static void printSum(int i ,int n , int sum) {
		if(i == n) {  // if i is equal to given n number 
			sum +=i;  // sum + i
			System.out.println("sum is: "+sum);  // prints sum of  n numbers
			return;
		}
		
		sum += i; // Here sum is o ...sum + i ,here i = 1 becomes sum +1 i.e, sum = 1
		printSum(i+1,n,sum); // Resursion // Here i = i+1 i.e, i = 1+1 = 2  
	}
	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		
		System.out.println("Enter the NUmber to begin");
		int i = sc.nextInt();  // NUmber to begin
		System.out.println("Enter the n number");
		int n = sc.nextInt(); // number to end
		int sum = 0; // sum starts with 0
		printSum(i,n,sum);
	}
}
