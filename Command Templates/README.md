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

## 0. **Variables**
- **$(user)** = Mentions user that used the command.
- **$(count)** = Prints how many times command has been used.
