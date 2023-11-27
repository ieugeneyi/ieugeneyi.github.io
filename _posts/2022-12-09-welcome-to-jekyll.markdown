---
layout: post
title:  "[자료구조] Intellij - SVN 연동하기"
date:   2022-12-09 17:17:36 +09:00
categories: DataStructure
---

Intellij에서 SVN 연동하는 방법



### 1. svn.exe download
https://www.visualsvn.com/downloads/
![](https://velog.velcdn.com/images/ieugeneyi/post/0a07e63a-7614-4a1b-8170-3be99b82b06c/image.JPG)

### 2. Intellij에 경로 입력 (File > Settings > Version Control > Subversion)
![](https://velog.velcdn.com/images/ieugeneyi/post/31856d2f-c016-45cd-903f-fd930a2d0120/image.JPG)
<br>압축해제한 경로를 입력한다. (svn.exe 까지 입력할것)

### 3. svn 저장소 등록 (VCS > Browse VCS Repository > Browse Subversion Repository ) 
![](https://velog.velcdn.com/images/ieugeneyi/post/42e3f1a4-bea7-4d25-a70b-1891943a0fcc/image.png)
<br>하단 + 버튼을 눌러 사용하고자 하는 Repository URL을 입력한다.

### 4. Intellij와 svn 연동 (File > Settings > Version Control  > '+' 버튼 클릭  > VCS : Subversion 선택 )
![](https://velog.velcdn.com/images/ieugeneyi/post/cdfeb06f-1241-41d1-a63f-63a57dddf7ca/image.JPG)

### 5. Project Share 하기 (VCS > Import into Version Control > Share Project (Subversion) )
![](https://velog.velcdn.com/images/ieugeneyi/post/1cd9b039-0136-4850-8620-34553a85624f/image.png)

![](https://velog.velcdn.com/images/ieugeneyi/post/42cfd7fa-9ecb-4498-90db-db958342d54c/image.png)
<br>Share할 Repository 선택 후 Share 

> **❓ Create /tags and /branches ? **
trunk폴더에 share하면서, tags, branches 폴더도 생성하라는 뜻으로,
svn 디렉토리는 **trunk / branches / tags** 세가지가 존재.
trunk : main 개발작업을 하는 폴더 
branches : 현재 소스는 유지보수하면서, 새로운 기능을 개발할 때 사용
tags : 릴리즈된 소스를 따로 보관하는 폴더 (개발이 아닌 보관을 위한 폴더 ) 

