# ACM 

## 输入输出

### 输出3位整数，前面补0

```c
int a = 9;
printf("%03d", a);     // 009

printf("%xd", a);      // x是一个数字，右对齐
```



## 函数库

### cmath

```c
// Return the smallest integral value that is not less than x (as a floating-point value).
double ceil (double x);

// If no errors occur, the largest integer value not greater than arg, that is ⌊arg⌋, is returned.
float floor (float arg);
double floor (double arg);
long double floor (long double arg);

// If no errors occur, square root of arg (√arg), is returned.
// If a domain error occurs, an implementation-defined value is returned (NaN where supported)
// If a range error occurs due to underflow, the correct result (after rounding) is returned.
float sqrt (float arg);
double sqrt (double arg);
long double sqrt (long double arg);
```



### algorithm

```cpp
// Returns the smaller of a and b.
template< class T >
const T& min( const T& a, const T& b);

// Returns the greater of a and b
template< class T >
const T& max( const T& a, const T& b);
```





