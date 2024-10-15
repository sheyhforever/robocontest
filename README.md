#include <iostream>

#include <vector>

using namespace std;

int main() {

 long long n;

 cin >> n;

 vector<long long> a(n);

 for (int i = 0; i < n; ++i) {

 cin >> a[i];

 }

 long long d, m;

 cin >> d >> m;

 long long k = 0;

 for (int i = 0; i <= n - m; ++i) {

 long long sum = 0;

 for (int j = i; j < i + m; ++j) {

 sum += a[j];
   }

 if (sum == d) {

 k += 1;

 }

 }

 cout << k << endl;

 return 0;

}
