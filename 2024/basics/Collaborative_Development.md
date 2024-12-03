# Collaborative Development [75]
---
![image](https://github.com/HAW-THL/Write-ups/assets/90260119/0f177702-3439-498a-aa97-34959104ccbc)

---

- Download the given file "challenge.zip"
```shell
wget https://artifacts.picoctf.net/c_titan/69/challenge.zip
```

![image](https://github.com/HAW-THL/Write-ups/assets/90260119/96cd13b4-4106-4c79-a049-a3e16dbf132d)

---

- Unzip the zip file
```shell
unzip challenge.zip
```

![image](https://github.com/HAW-THL/Write-ups/assets/90260119/4775ce17-8593-4d29-8290-6aea75378aa5)

---

- Let's take a look at what can be found in the "drop-in" folder
```shell
cd drop-in/ && ls -la
```

![image](https://github.com/HAW-THL/Write-ups/assets/90260119/76a63dcc-059b-4f86-9ac9-f72c5b359406)

---

- Now let's take a look at all the current branches
```shell
git branch -a
```

![image](https://github.com/HAW-THL/Write-ups/assets/90260119/5f66f754-74b9-4f87-a2a9-3a2de41cd9a0)

---

- There are three branches and each carries a part of the flag. You could now either call up all the flags and write them down individually or combine all the flags into one "main flag" in order to rule out possible problems
```shell
git checkout feature/part-1 && cat flag.py && git checkout feature/part-2 && cat flag.py && git checkout feature/part-3 && cat flag.py
```

![image](https://github.com/HAW-THL/Write-ups/assets/90260119/b41bb399-1005-496a-9c60-9b0bdd02172c)

---

```shell
picoCTF{t3@mw0rk_m@k3s_th3_dr3@m_w0rk_e4b79efb}
```
