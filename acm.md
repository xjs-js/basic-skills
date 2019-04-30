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

// Returns base raised to the power exponent:
// base^exponent 
double pow (double base, double exponent);

// Returns the absolute value of parameter n ( /n/ ).
          int abs (          int n);
     long int abs (     long int n);
long long int abs (long long int n);
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

### string

```cpp
// The substring is the portion of the object that starts at character position pos and spans len characters (or until the end of the string, whichever comes first).
string substr (size_t pos = 0, size_t len = npos) const;

// Returns the length of the string, in terms of bytes.
size_t length() const noexcept;

// Searches the string for the first occurrence of the sequence specified by its arguments.
// When pos is specified, the search only includes characters at or after position pos, ignoring any possible occurrences that include characters before pos.
size_t find (const string& str, size_t pos = 0) const;

string to_string(int value);


// upper or lower a string
for (auto & c: str) c = toupper(c);
for (auto & c: str) c = tolower(c);
```

### algorithm

```cpp
/* --------- reverse ----- begin ------------------------- */
//  逆序字符串，或者vector容器或者数组

template<class BidirIt>
void reverse(BidirIt first, BidirIt last);

// usage
vector<int> v{1,2,3};
reverse(begin(v), end(v));  // 3,2,1
int a[] = {4,5,6,7};
reverse(begin(a), end(a));  // 7,6,5,4

/* --------- reverse ----- end --------------------------- */


```



