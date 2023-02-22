# Kombinasyon
www.patika.dev
--------------


import java.util.Scanner;

public class Kombinasyon 
{

	public static void main(String[] args) 
	{
		int nFaktoriyel =1;
		int rFaktoriyel =1;
		int nrFaktoriyel =1;
		Scanner scanner = new Scanner(System.in);
		
		System.out.println("n sayisini giriniz: ");
		int n = scanner.nextInt();
		System.out.println("r sayisini giriniz: ");
		int r = scanner.nextInt();
		
		for(int i=1; i<n; i++)
		{
			nFaktoriyel *=i;
		}
		
		for(int i=1; i<r; i++)
		{
			rFaktoriyel *=i;
		}
		
		for(int i=1; i<(n-r); i++)
		{
			nrFaktoriyel *=i;
		}
		
		System.out.println("C(n,r)=" + "C(" + n + "," + r + ")=" + (nFaktoriyel / (rFaktoriyel * nrFaktoriyel)));
	}

}
