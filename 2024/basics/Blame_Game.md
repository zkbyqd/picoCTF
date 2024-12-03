# Blame Game [50]
![image](https://github.com/zkbyqd/Write-ups/assets/90260119/b551131d-b276-4a90-89d1-edb473c4a948)

```
wget https://artifacts.picoctf.net/c_titan/157/challenge.zip && unzip challenge.zip
```
![image](https://github.com/zkbyqd/Write-ups/assets/90260119/596bac39-7317-4d6c-8441-6d88e1831e5c)

```
cd drop-in/ && ls -la
```
![image](https://github.com/zkbyqd/Write-ups/assets/90260119/00149462-983b-4a53-9d79-370dc9189c81)

- Now we use "git log" on a specified file:
```
git log message.py
```
![image](https://github.com/zkbyqd/Write-ups/assets/90260119/ff2aa13e-d009-42a7-9ce5-5add3580d339)

- As you can see, the flag is the author of the commit "optimize file size of prod code"
```
picoCTF{@sk_th3_1nt3rn_cfca95b2}
```
