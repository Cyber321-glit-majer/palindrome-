# palindrome-
check whether the given string is a palindrome or not

**
Input1:
Hello

Output1:
String is not palindrome

Input2:
madam

Output2:
String is palindrome

**CODE**
```

#include <iostream>
#include <string.h>
using namespace std;
int main() {
    string s;
    getline(cin, s);
    int low = 0;
    int high = s.size() - 1;
    int flag = 0;
    while (low < high) {
        if (s[low] != s[high]) {
            flag = 1;
            break;
        }
        low++;
        high--;
    }
  
    if (flag == 0)
        cout << "String is palindrome";
    else
        cout << "String is not palindrome";
    return 0;
}
