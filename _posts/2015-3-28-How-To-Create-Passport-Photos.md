---
layout: post
title: How to Create Passport Photos
---

미국에서 여권 사진 만드는 법:
1. 사진을 찍는다.
2. http://travel.state.gov/…/engl…/passports/photos/photos.html 에 가서 사진을 사이즈에 맞게 자른다 (600 x 600 pixel로 잘라줌).
3. (imagemagick을 설치한 후) convert photo.jpg \( +clone +clone \) +append \( +clone \) -append photo_to_print.jpg (가로 3, 세로 2 줄로 해서 현상하기 좋게 만들어 줌)
4. http://photos1.walmart.com/walmart/home/ 에서 4x6 으로 주문
가격: $0.19