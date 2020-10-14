# shell00

## ex01
cat : 파일 받아와서 text로 출력

## ex02
ls : list directory contents
ls -l : list in long format.

**tar 압축 풀기**
tar -xvf

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
F : 디렉토리 : /, executable : *, symbolic : @ ... 
m: 쉽표로 분리

## ex05
git log : git log 보여줌
-5 : 마지막 5개 로그
--pretty : 보여주는 형식을 지정할 때 사용
%H : long id 보여줌
%h : short id 보여줌

## ex06
git ls-files : Show information about files in the index and working tree
-i : ignored (ignore된 파일)
-o : others - show other(i,e untracked) files in the output (추적하지 않는 파일 포함)
--exclude-standard: add the standard git exclusions (정상적인 파일은 포함시키지 않음)

## ex07
**방법 1**
patch -p[depth] < [diff file] -> 어떤 파일 설정할지 물음 -> 해당 파일을 patch 시킴.

**방법 2**
patch [원본 파일] [diff file] > [새로운 파일]

## ex08
find . : 현재 폴더에서 
-name : 이름으로 검색
-delete : 해당 파일 삭제
**-a, -o**
[expression1] -a [expression2]
True if both expression1 and expression2 are true.
[expression1] -o [expression2]
True if either expression1 or expression2 are true.

## ex09
0부터 시작하기 때문에 41로 해야 함
**magic file 생성**
file -C -m (C : Compile, m: magic-file)
41 string 42 42 file
41번째 byte에 string으로 42가 오면 42 file로 분류
