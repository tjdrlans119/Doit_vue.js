# 이 둘의 차이는....


## 리턴되는 응답 형태가 다르다.

## 예를 들어

## get 으로 요청(request)하면

## vueAxios의 응답(response)는
{data: {…}, status: 200, statusText: "OK", headers: {…}  (....생략....) }
data: {fe1: "Angular", fe2: "React", fe3: "Vue.js", fe4: "Backbone.js", be1: "Spring", …}
headers: {content-type: "text/plain; charset=utf-8", cache-control: "max-age=300", expires: "Fri, 08 Feb 2019 18:05:45 GMT"}
(....생략....)
response: "{↵	"fe1": "Angular",↵	"fe2": "React",↵	"fe3": "Vue.js",↵	"fe4": "Backbone.js",↵	"be1": "Spring",↵	"be2": "Django",↵	"be3": "Node.js"↵}↵"
responseText: "{↵	"fe1": "Angular",↵	"fe2": "React",↵	"fe3": "Vue.js",↵	"fe4": "Backbone.js",↵	"be1": "Spring",↵	"be2": "Django",↵	"be3": "Node.js"↵}↵"
responseType: ""
responseURL: "https://raw.githubusercontent.com/joshua1988/doit-vuejs/master/data/demo.json"
(....생략....)

## 이런식으로 오고


## 뷰 리소스의 응답(response)는
q {url: "https://raw.githubusercontent.com/joshua1988/doit-vuejs/master/data/demo.json", ok: true, status: 200, statusText: "OK", headers: I, …}
body: {fe1: "Angular", fe2: "React", fe3: "Vue.js", fe4: "Backbone.js", be1: "Spring", …}
bodyText: "{↵	"fe1": "Angular",↵	"fe2": "React",↵	"fe3": "Vue.js",↵	"fe4": "Backbone.js",↵	"be1": "Spring",↵	"be2": "Django",↵	"be3": "Node.js"↵}↵"
headers: I {map: {…}}
ok: true
status: 200
statusText: "OK"
url: "https://raw.githubusercontent.com/joshua1988/doit-vuejs/master/data/demo.json"
data: (...)
__proto__: Object


### 사실... 비슷하게 느껴진다 가공을 한번 더 하고 안하고의 차이라고 생각된다.
