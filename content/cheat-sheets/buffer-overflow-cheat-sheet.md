# Buffer Overflow
Type of attack where the an attacker will overload a buffer to then point to malicious code. Majority of the time, the developer has mis-calculated the array-size or string length which can lead to this type of attack. The developer does not do this on purpose but needs to make sure the that array is null terminated. 

## Commone Types
- Stack Buffer Overflow (Classic Buffer Overflow) - The attacker sends data to a program, which it store in an undersized stack buffer. The result is that information on the call stack is overwritten, including the functions return pointer. The data sets the value of the return pointer so that when the function returns, it transfers control to malicious code contained in the attacker's data. 

## Analysis

Buffer overflow vulnerabilities typically occur in code that:
  - Relies on external data to control its behavior
  - Depends upon properties of the data that are enforced outside of the immediate scope of the code
  - Is so complex that a programmer cannot predict its behavior

So make sure to keep that in context when analyzing developers code. 


## References
- https://stackoverflow.com/questions/574159/what-is-a-buffer-overflow-and-how-do-i-cause-one
- https://owasp.org/www-community/vulnerabilities/Buffer_Overflow