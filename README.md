# 579A---Raising-Bacteria

#include <iostream>
#include <math.h>

using namespace std;

int main()
{

	long long num;
	cin >> num;

	int cnt = 0;
	
	for (int i = 0 ; i < log2((double)num)+1 ; i++)
		if (num & (1 << i))
			cnt++;
	
	cout << cnt;
	
	return 0;
}
