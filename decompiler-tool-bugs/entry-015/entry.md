# entry-015

Uses an ASM Bug to cause to not showing up try catch block

## How
OW2's ASM will not show the try catch block inclusive the zero division, because ASM think's thats impossible and will skip it. 
Somehow if an other instruction is added inside the try catch block it will show again.

## Example Code
```Java
  try {
			int ignored = 0 / 0;
		} catch (ArithmeticException e) {}
``` 

