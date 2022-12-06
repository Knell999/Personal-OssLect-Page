## Add

특정 파일 스테이징

```
git add {파일명} 
```

변경된 모든 파일 스테이징

```
git add * 
```


## Commit

커밋 합치기

```
git rebase -i HEAD~4 // 최신 4개의 커밋을 하나로 합치기
```

커밋 메세지 수정

```
$ git commit --amend // 마지막 커밋메세지 수정(ref)
```

간단한 commit방법

```
$ git add {변경한 파일병}
$ git commit -m “{변경 내용}"
```

커밋 이력 확인

```
$ git log // 모든 커밋로그 확인
$ git log -3 // 최근 3개 커밋로그 확인
$ git log --pretty=oneline // 각 커밋을 한 줄로 표시
$ git reflog // reset 혹은 rebase로 없어진 과거의 커밋 이력 확인
```

커밋 취소

```
$ git reset HEAD^ // 마지막 커밋 삭제
$ git reset --hard HEAD // 마지막 커밋 상태로 되돌림
$ git reset HEAD * // 스테이징을 언스테이징으로 변경, ref
```
