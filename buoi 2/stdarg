#include <stdio.h>
#include <stdarg.h>
#define tong(...)     sum(__VA_ARG__,'a')
int sum(int count,...){
va_list args;
va_list check;

va_start(args,count);
va_copy(check,args);

int result = count;
while (va_arg(check,char) !='a')
{
     result += va_arg(args, int);
}
va_end(args);
return result;
}
int main()
{
printf("tong:  %d\n", tong(1 2 3 4 5));
return 0;
}
