# endianness [200]
---
![image](https://github.com/HAW-THL/Write-ups/assets/90260119/d009728f-0cd7-4c64-8190-b09366167d26)

- Login with NetCat

```
nc titan.picoctf.net 65351
```

![image](https://github.com/HAW-THL/Write-ups/assets/90260119/4c44322b-b4d6-4ba9-a282-221b101ec460)

- Convert the word "oyqci" with [CyberChef](https://gchq.github.io/CyberChef/) to Hex.

![image](https://github.com/HAW-THL/Write-ups/assets/90260119/8376a717-4bb9-46ae-87df-629659e142d6)

```
6f 79 71 63 69
```
- The Output is our big Endian which we can now convert with CyberChef to a little Endian (instead of CyberChef I prefer [save-editor](https://www.save-editor.com/tools/wse_hex.html) )

![image](https://github.com/HAW-THL/Write-ups/assets/90260119/30454a29-3422-49fc-add9-df2c9aacbaeb)

```
69 63 71 79 6f
```
- This Output is our little Endian

> Here you can see what's going on in the background

![image](https://github.com/HAW-THL/Write-ups/assets/90260119/74078ce7-7d82-42d4-bcdf-398062de5ca4)

- Now we enter our results

![image](https://github.com/HAW-THL/Write-ups/assets/90260119/6263976c-a267-4969-a5f4-eab044162ac3)

```
picoCTF{3ndi4n_sw4p_su33ess_25c5f083}
```
