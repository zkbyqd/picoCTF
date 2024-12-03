# Time Machine [50]

![image](https://github.com/zkbyqd/Write-ups/assets/90260119/eee73562-d9bf-452f-b2d0-fa446425cd4c)

- This is a sub-task of the ["Commitment Issues"](https://github.com/HAW-THL/Write-ups/blob/main/picoCTF2024/General%20Skills/Commitment_Issues.md) challenge.

- Download "challenge.zip" and unzip it.
```
wget https://artifacts.picoctf.net/c_titan/160/challenge.zip && unzip challenge.zip
```

![image](https://github.com/zkbyqd/Write-ups/assets/90260119/ef5424a0-138b-46af-bb06-59d806a5e9ef)

- Where do I get the link from?

![image](https://github.com/zkbyqd/Write-ups/assets/90260119/dd77b5d2-aa90-4aac-adf8-1edde26a2a1d)
![image](https://github.com/zkbyqd/Write-ups/assets/90260119/841e36d0-7323-487e-bec1-fde9d98a4c9f)

- Change into the Folder and see what's in there.
```
cd drop-in/ && ls -la
```

![image](https://github.com/zkbyqd/Write-ups/assets/90260119/3bb2dd24-c7de-470a-b8f1-57a91a5750ba)

- Let's see what the "message.txt" says.
```
cat message.txt
```

![image](https://github.com/zkbyqd/Write-ups/assets/90260119/68d59946-c00f-42aa-9e34-87269fe34c0d)

- It shows the hint to check the commit logs.

```
git log
```

![image](https://github.com/zkbyqd/Write-ups/assets/90260119/6ceac377-6f58-43d2-ade8-dc96e7883014)

```
picoCTF{t1m3m@ch1n3_186cd7d7}
```
