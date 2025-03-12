R Programomg

R version 4.4.1 (2024-06-14 ucrt) -- "Race for Your Life"
Copyright (C) 2024 The R Foundation for Statistical Computing
Platform: x86_64-w64-mingw32/x64

R은 자유 소프트웨어이며, 어떠한 형태의 보증없이 배포됩니다.
또한, 일정한 조건하에서 이것을 재배포 할 수 있습니다.
배포와 관련된 상세한 내용은 'license()' 또는 'licence()'을 통하여 확인할 수 있습니다.

R은 많은 기여자들이 참여하는 공동프로젝트입니다.
'contributors()'라고 입력하시면 이에 대한 더 많은 정보를 확인하실 수 있습니다.
그리고, R 또는 R 패키지들을 출판물에 인용하는 방법에 대해서는 'citation()'을 통해 확인하시길 부탁드립니다.

'demo()'를 입력하신다면 몇가지 데모를 보실 수 있으며, 'help()'를 입력하시면 온라인 도움말을 이용하실 수 있습니다.
또한, 'help.start()'의 입력을 통하여 HTML 브라우저에 의한 도움말을 사용하실수 있습니다
R의 종료를 원하시면 'q()'을 입력해주세요.

a<-17
print(a)
v1<-c(-1,0,1)
v2<-c("hello", "hi", "~!")
print(v1)
print(v2)
v3<-c(-1,1,0,"Hello", "~!")
print(v3)
v4<-list(-1,1,0,"Hello", "~!")
print(v4)
str(v4)
str(v3)

length(v3)
length(v4)
length(v2)

##matrix
x<-c(1,1,0,2,1,1,3,1,0)
length(x)
##3X3 matrix
A<-matrix(x, nrow = 3, ncol = 3)
print(A)
## dim-3 matrix
xx<-c(1,2,3,4,5,6)
arr<-array(xx, dim = c(2,2,3))
print(arr[,,1])
print(arr[,,2])
print(arr[,,3])

##조건문/반복문
x<-1:10
print(x)
y<-10:1
print(y)
str(x)
str(y)
a<-10
if(a %% 2 ==0){
  print("Even")
}else {
  print("Odd")
}
##if~ else if~ else
a<-2
b<-3
c<-1
#finding #maximum
if(a>b & a>c){
  print(a)
}else if(b>c & b>a){
  print(b)
}else{
  print(c)
}
#iteration 
for (i in 1:10){
  print(3*i)
}

sum<-0
for (i in 1:10){
  sum<-sum+i
}
print(sum)
fac<-1
for (i in 1:10){
  fac<-fac*i
}
print(fac)
for (i in 1:10){
  print(paste("3 *", i, "=", 3*i))
}

##function
gugudan<-function(dan){
  for (i in 1:10){
    print(paste( dan, "*", i, "=", dan*i))
  }
}
gugudan(3)
