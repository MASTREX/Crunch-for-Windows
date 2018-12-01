- # Crunch-for-Windows
Password creation Tool


# Command

>crunch min max charset options

The min and max are the minimum and maximum lengths (respectively) for your desired wordlist. By default charset is not required, but
you can use it to limit the characters of your wordlist to the ones you specify. If you choose to use charset then you must maintain
the correct order, which is lowUP123@%# (lowercase letters, then uppercase letters, then numbers and finally symbols). You can skip
any of them, but the order must always remain the same.


Examples:

> crunch 2 6 qrs347

The command above will produce a wordlist for every possible combination of the characters qrs347 from 2 to 6 characters in length.

Options:

- -b : the maximum size of the wordlist (requires -o START)
- -c : numbers of lines to write to the wordlist (requires -o START)
- -d : limit the number of duplicate characters
- -e : stop generating words at a certain string
- -f : specify a list of character sets from the charset.lst file
- -i : invert the order of characters in the wordlist
- -l : allows the literal interpretation of @,%^ when using -t
- -o : the output wordlist file
- -p : print permutations without repeating characters (cannot be used with -s)
- -q : Like the -p option except it reads the strings from a specified file
- -r : resume a previous session (cannot be used with -s)
- -s : specify a particular string to begin the wordlist with
- -t : set a specific pattern of @,%^
- -z : compress the output wordlist file, accompanied by -o

Reference:

- @ represents lowercase letters
- , represents uppercase letters
- % represents numbers
- ^ represents special characters
