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

使用JWT作為Token驗證

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




