# shell00

## ex01
cat : 파일 받아와서 text로 출력

## ex02
ls : list directory contents
ls -l : list in long format.

**권한 10자리**
1 : 파일 형식(d : directory, l : link, - : file)
2~4: user 권한 (r: read, w: write, x: execute)
5~7: group 권한 (r: read, w: write, x: execute)
8~10: other 권한 (r: read, w: write, x: execute)

chmod : 권한 변경
chmod 777 [filename] (777: 각 자리는 u, g, o 권한을 의미, 숫자는 r(2^2) + w(2^1) x(2^0)의 합을 의미)
ex) 777은 -rwxrwxrwx

**타임스템프 변경**
touch -t MMDDhhmm [filename]

**링크 만들기**
ln : 링크
ln -s : 심볼릭 링크

**text 입력**
vim으로 편집
vim -n

## ex03

## ex04
U : use time file creation
t : ?
F : 디렉토리 : /, executable : *, symbolic : @ ... 
m: 쉽표로 분리

## ex05
git log : git log 보여줌
-5 5개 커밋 보여줌
--pretty : 보여주는 형식을 지정할 때 사용
