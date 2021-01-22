### Task
Complete the code in the editor below. The variables i, d, and s, are already declared and initialized for you. You must:
1. Declare 3 variables: one of type int, one of type double, and one of type String.
2. Read 3 lines of input from stdin (according to the sequence given in the Input Format section below) and initialize your 3 variables.
3. Use the + operator to perform the following operations:
- Print the sum of  plus your int variable on a new line.
- Print the sum of  plus your double variable to a scale of one decimal place on a new line.
- Concatenate  with the string you read as input and print the result on a new line.

### Input Format
The first line contains an integer that you must sum with i.
The second line contains a double that you must sum with d.
The third line contains a string that you must concatenate with s.

### Output Format
Print the sum of both integers on the first line, the sum of both doubles (scaled to 1 decimal place) on the second line, and then the two concatenated strings on the third line.

### Sample Input
```markdown
12
4.0
is the best place to learn and practice coding!
```
### Sample Output
```markdown
16
8.0
HackerRank is the best place to learn and practice coding!
```
### Explanation
When we sum the integers 4 and 12, we get the integer 16.
When we sum the floating-point numbers 4.0 and 4.0, we get 8.0.
When we concatenate HackerRank with is the best place to learn and practice coding!, we get HackerRank is the best place to learn and practice coding.
### Source Code
```markdown
#include <iostream>
#include <iomanip>
#include <limits>

using namespace std;

int main() {
    int i = 4;
    double d = 4.0;
    string s = "HackerRank ";

    int num1;
    double num2;
    string str;
    double ans;
    
    cin >> num1;
    cin >> num2;
    cin.ignore();
    getline (cin, str);

    cout << i + num1 << endl;
    ans = num2 + d;

    std::cout << std:: fixed;
    std::cout << std::setprecision(1);
    std::cout << ans << endl;

    cout << s;
    cout << str;

    return 0;
}
```



This page is managed by Kheijhackt
