# day-5-AIML

non_even_prime = []
for num in range(2, 100):
    for i in range(2, num):
        if (num % i) == 0:
            break
    else:
        if len(non_even_prime) == 20:
            break
        else:
            if num % 2 !=0:
                non_even_prime.append(num)
print(non_even_prime)


from IPython.core.interactiveshell import InteractiveShell
InteractiveShell.ast_node_interactivity = "all"

s = "LetsUpgrade"

s.upper()
s.swapcase()
s.lower()
s.count('e')
s.casefold()
s.endswith('d')
s.isalnum()
s.find('s')
s.isalpha()
' '.join(s)
s.isupper()
s.islower()
s.index('t')
s.isdigit()
s.replace('LetsUpgrade',"Hello shyam")



from collections import Counter

string1 = "Redefining"
string2 = "definingRe"

# Polindrome - string1
# Anagram needs two strings
rev = string1[::-1]

if string1 == rev:
    print(string1, "is Polindrome")
elif Counter(string1) == Counter(string2):
    print(string1,'and',string2 ,'is Anagram')
else:
    print('None of them')


import re
def remspchar(s):
    final = (re.sub('[!@#$-._+#]',' ',s)).lower()
    print(final)
s = "@_shyam#LetsUpgrade!!!"
remspchar(s)
