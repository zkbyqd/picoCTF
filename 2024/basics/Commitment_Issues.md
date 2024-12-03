# Commitment Issues [50]
---
![image](https://github.com/HAW-THL/Write-ups/assets/90260119/b9e80ad7-b42e-4698-b5d4-18ca6519aa82)

- Download the given file "challenge.zip"
```
wget https://artifacts.picoctf.net/c_titan/75/challenge.zip
```

![image](https://github.com/HAW-THL/Write-ups/assets/90260119/2c33340d-d6c8-4cf4-837a-09a91447e706)

- Unzip the zip file
```
unzip challenge.zip
```

![image](https://github.com/HAW-THL/Write-ups/assets/90260119/354c2f88-817f-4ce7-b573-7307e9983ecf)

- Let's take a look at what can be found in the "drop-in" folder
```
cd drop-in/ && ls -la
```

![image](https://github.com/HAW-THL/Write-ups/assets/90260119/7b468c16-84de-452b-ae5c-02ca115c7604)

- Now let's take a look at the "message.txt"
```
cat message.txt
```

![image](https://github.com/HAW-THL/Write-ups/assets/90260119/048ec8d6-03a5-4aae-8303-f89664de13fe)

- We can't do anything with the content of the "message.txt" yet, so let's take a look at the logs in the hidden ".git" folder first
```
git log
```

![image](https://github.com/HAW-THL/Write-ups/assets/90260119/f71b20be-4c7b-49a5-9d3e-43ffb6548a38)

- Here we can see which previous commits have been made. One of them shows "create flag" with the ID "6603cb4ff0c4ea293798c03a32e0d78d5ab12ca2"

- With "Checkout" we can change past commits with the IDs

```
git checkout 6603cb4ff0c4ea293798c03a32e0d78d5ab12ca2
```

![image](https://github.com/HAW-THL/Write-ups/assets/90260119/69e83290-fd62-41bb-af39-5d4a4b2b32af)

- To find the flag, let's take another look at the "message.txt"

```
cat message.txt
```

![image](https://github.com/HAW-THL/Write-ups/assets/90260119/4cc50399-9336-422c-8c1e-ecb35cfa48e3)

```
picoCTF{s@n1t1z3_9539be6b}
```
