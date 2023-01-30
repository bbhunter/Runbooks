# Password List Generation

## Password Lists

```
cewl www.site.com -m 5 -w passwords.txt
```

Generating a wordlist with cewl from website crawl(minimum 5 char):

```
crunch 6 6 0123456789ABCDEF -o passwords.txt
```

Generating wordlist with crunch containing the characters 0-9 and A-F 1-6 characters long

```
/usr/share/crunch/charset.lst
```

Pre-defined crunch character sets Kali Linux

```
crunch 4 4 -f /usr/share/crunch/charset.lst mixalpha
```

Using crunch pre-defined character sets(More can be found in the man page)

Crunch Custom translation placeholders

| Character     | Type                               |
| ------------- |:----------------------------------:|
| @             | Lower case alpha characters        |
| ,             | Upper case alpha characters        |
| %             | Numeric characters                 |
| ^             | Special characters including space |


Generating customer translation wordlist

```
crunch 8 8 -t ,@@^^%%%
```
