# testing_KAU_collavoration

1. Git repository를 clone 한다. "git clone https://github.com/esc16/testing_KAU_collavoration.git"
2. Notepad로 Text file을 만든다. 파일명은 "영문이름+학번.txt"(Ex : dean_kim_1994.rtf or dean_kim_1994.txt) Text file의 내용은 자기소개와 현재 KAU에서 맡고 있는 Role 설명한다.
3. 현재의 repository status를 확인한다. "git status"
4. dean_kim_1994.rtf 파일이 추가되었지만 untracked 되고 있을 것을 확인한다.

   Untracked files:
  (use "git add <file>..." to include in what will be committed)
	**dean_kim_1994.rtf**

  nothing added to commit but untracked files present (use "**git add**" to track)
  
5. Local repository에 create된 파일을 Add한다. "git add dean_kim_1994.rtf"
6. Local repository에 commit을 한다. "git commit -m "add Dean Kim's intdoduction"
7. 현재의 repository status를 확인한다. "git status"
  
   On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "**git push**" to publish your local commits)

8. 9번을 수행하기 전에 다른 멤버가 먼저 push 했을 수도 있으므로 pull 명령으로 repository르 sync 한다. "git pull". 
9. Remote repository에 push 명령으로 publish한다. "git push"
10. 다른 멤버의 소개파일을 열어서 자기 이름과 학번을 그리고 환영인사를 추가한다. 예제에서는 **dean_kim_1994.rtf** 파일에 오타가 있어서 해당 파일을 수정했다.  
11. 현재의 repository status를 확인한다. "git status"
  
  On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   dean_kim_1994.rtf

no changes added to commit (use "git add" and/or "git commit -a")
  
12. dean_kim_1994.rtf가 modified 상태인 것을 확인 할 수있다. 변경된 파일을 commit하기 위해서는 "git add" 또는 "git commit -a"을 수행하라고 조언을 하는데 "git commit -a"를 add와 commit을 동시에 수행해서 편리하다. 만약 여러개의 파일을 변경했지만 특정 파일만 add하고 싶다면 반드시 "git add"를 사용하기 바란다.(참고 : https://yuja-kong.tistory.com/48)
13. Local repository에 변경된 파일을 Add한다. "git add dean_kim_1994.rtf"
14. Local repository에 commit을 한다. git commit -m "correct the typo", commit 메세지는 각자의 상황에 맞게 작성하기 바란다.
15. Remote repository에 push 명령으로 publish한다. "git push"
  
  
