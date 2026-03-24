# Table of Contents
- [Random line from a list](#1-random-line-from-a-list)
- [Variables](#0-variables)

## 1. **Random line from a list**
**🤖 Nightbot:** User, this run will end on: Chapter. This command has been used 4 times.
<details>
  <summary>📋Example Command📋</summary> 
  
```
$(user), this run will end on: $(eval a="$(urlfetch json https://raw.githubusercontent.com/AmRazzie/SR-Nightbot-Commands/refs/heads/main/Channels/Razzie/!fate/hl1)".split(";");a[Math.floor(Math.random()*a.length)]) This command has been used $(count) times.
```
</details>
<details>
  <summary>📋Template📋</summary>
    
```
$(user)<TEXT HERE> $(eval a="$(urlfetch json <URL TO THE RAW FILE>)".split(";");a[Math.floor(Math.random()*a.length)])
```
</details>

## 2. **Random number**
**🤖 Nightbot:** There is 55% chance that throw. 
<details>
  <summary>📋Example Command📋</summary> 
  
```
There is $(eval Math.floor(Math.random()*110))% chance that $(query).
```
</details>
<details>
	<summary>📋Template📋</summary>

```
<TEXT> $(eval Math.floor(Math.random()*<NUMBER>))<TEXT> $(query).
```
</details>

## 0. **Variables**
- **$(user)** = Mentions user that used the command.
- **$(touser)** = Mentions user if nothing is typed, otherwise same as **$(query)**
- **$(query)** = Returns text typed after !command.
- **$(count)** = Prints how many times command has been used.

