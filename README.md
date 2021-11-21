# otw-narnia

Narnia is a wargame on OverTheWire. You can play it at https://overthewire.org/wargames/narnia/

Since the tools on the systems of OverTheWire are outdated and I did not find any page where I can download the complete sources, I decided to publish them here.

No solutions here. Only the plain sourcecode to hack at home, without needing to SSH into OTW's servers.

## Compile instructions

For Arch users:  
Enable multilib repository, since we're going to combile 32Bit.   
Then: `pacman -S multilib-devel`


```
gcc narnia1.c -o narnia1 -w -g -Wno-format -Wno-format-security -fno-stack-protector -mpreferred-stack-boundary=2 -z execstack -no-pie -Wl,-z,norelro -m32
```

Since I have not played all levels, I can not promise the instructions work for all.
