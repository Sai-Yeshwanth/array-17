import java.util.Scanner;

class Add{
	static int arr[] = new int[100];
	
	static float sum=0;
	static Scanner input = new Scanner(System.in);
	public static void find()
	{
		System.out.println("Enter size of array:");
		int n = input.nextInt();
		int MAX=0;
		int MIN=999;
		System.out.println("Enter "+ n +" elements of array");
		for(int i=0;i<n;i++)
		{
			arr[i] = input.nextInt();
		}
		for(int i=0;i<n;i++)
		{
			if(arr[i]==12)
			{
				sum++;
			}
			if(arr[i]==23)
			{
				sum++;
			}
		}
		if(sum==2)
		{
			System.out.println("12,23 are present in array");
		}
		else if(sum==1)
		{
			System.out.println("only one element of 12 and 23 are found in array");
		}
		else
		{
			System.out.println("elements not found");
		}
	}
}

public class Jala {

	public static void main(String[] args) {
		Add a = new Add();
		a.find();
	}
}
