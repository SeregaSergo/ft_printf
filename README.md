# ft_printf
It's a simplified reproduction of libc printf without using standard output (supported conversions cspdiuxX%)

This function supports the following conversions "cspdiuxX%" and flags "+0- #".
Simbols are printed one by one without buffering.

#Use
-make

Then you can use static library libftprintf.a witch contains function ft_printf.
