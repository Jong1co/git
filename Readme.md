## submodule

- .gitmodules 파일 : 하위 프로젝트 url 의 매핑 정보를 담은 설정파일

- git diff --cached <폴더 이름>

해당 명령어로 확인해보면 아래처럼 나옴

```
diff --git a/sub-lib b/sub-lib
new file mode 160000
index 0000000..cfa8b41
--- /dev/null
+++ b/sub-lib
@@ -0,0 +1 @@
+Subproject commit cfa8b41578fcc6c99691c73d945bf4107c00746f
```

즉, 디렉토리를 서브모듈로 취급하기 때문에 디렉토리 아래 파일을 직접 추적하지 않음

- git diff : commit 이나 branch 사이에 다른 점, 혹은 파일이나 repository와 working directory 사이의 다른 점을 보여주는 명령어.

- git diff, git diff HEAD : 변경사항 확인
- git diff [option] [file name] : 특정한 파일에 대한 변경사항
- git diff [branch1].. [branch2] : 브랜치 간 변경사항

git diff --staged : staging area와 repository head 커밋 사이의 변경사항 확인
