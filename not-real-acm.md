# Real Problem



## is prime?

```cpp
//  判断n是否为素数
bool isPrime(int n)
{
    if (n == 1)         //  如果是1，直接返回false
        return false;
    if (n == 2)         //  如果是2，直接返回true
        return true;
   
    for (int i = 2; i <= int(sqrt(n)); ++i) {  //  用sqrt(n)， 而不是n/2
        if (n % i == 0) {   //  找到了一个因数
            return false
        }
    }
    
    return true;
}
```



```cpp
bool is_prime[100000005];

// 构造素数筛
void constructPrime ()
{
    memset(is_prime, true, 100000005);
    is_prime[0] = false;
    is_prime[1] = false;
    for (int index = 2; index <= 100000000; index++) {
        if (is_prime[index] == true) {
            int j = index + index;
            while (j <= 100000000) {
                is_prime[j] = false;
                j += index;
            }
        }
    }
}
```



## is Palindrome

```cpp
//  判断是否是回文
bool isPalindrome (string s)
{
    string::iterator front = s.begin();
    string::iterator back  = s.end()-1;
    
    bool is_palindrome = true;
    while (front < back) {
        if (*front != *back) {
            is_palindrome = false;
            break;
        }
        ++front;
        --back;
    }
    return is_palindrome;
}
```



