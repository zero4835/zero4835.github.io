---
layout: post
title: 全端練習筆記
date: 2023-07-11
Author: Natsusaka
tags: [full-stack, note]
comments: true
toc: true
--- 

我的目標是做出一個帶有登入、論壇的平台，使用React + SpringMVC + MySQL，

## Structure
##### Back-end
+ Model
+ Repo
+ Service
+ Controller
##### Front-end
+ Component
+ Page
+ Route(undone)

### 登入介面

使用JWT作為Token驗證,用把id和email加入其中

```
public String createToken(Integer userId, String email) {
        Algorithm algorithm = Algorithm.HMAC256(secret);
        return JWT.create()
                .withClaim("mid", userId)
                .withClaim("email", email)
                .sign(algorithm);
    }
```
![](https://img.onl/tNxBH5)

### 註冊介面
![](https://img.onl/G4byTp)

## 資料庫
資料庫使用JPA來將實體的物件持久化到資料庫中

![](https://img.onl/b0V5DR)

帶有使用者名稱和頭像的登入狀態

![](https://img.onl/3b6W7y)










