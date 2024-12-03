# Binary Search [100]
---
![image](https://github.com/HAW-THL/Write-ups/assets/90260119/42a3b3a7-d753-48cd-a046-2f50f6c7b090)

- Login with SSH:
```bash
ssh -p 52760 ctf-player@atlas.picoctf.net
```
- Enter Password
```
84b12bae
```

- Accept the Fingerprint with "yes"

![image](https://github.com/HAW-THL/Write-ups/assets/90260119/f145c332-bd36-46a3-a082-6638444ebb0e)

> First Hint

![image](https://github.com/HAW-THL/Write-ups/assets/90260119/3a809609-56ed-459e-a954-ad5a91f50ed1)

![image](https://github.com/HAW-THL/Write-ups/assets/90260119/7a2fdf2f-a3d5-4c9e-818f-94f4d0fad8a1)

- 500
> Always start with 500, as it is half of 1 and 1000

- 750
> So that we can narrow down the largest possible range, we start with 750

- 600
> 750 is too high, 600 is too low

- 650
> higher than 600 but lower than 650

- 625
> take half to test the largest possible range again

- 615
> we got lucky with 615

```
picoCTF{g00d_gu355_2e90d29b}
```
