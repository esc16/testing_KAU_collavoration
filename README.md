# testing_KAU_collavoration
#2차 숙제
# 이번 숙제는 Git branch르 만들고 본인이름+학번으로 된 Directory(Folder)를 만든다음 방학동안에 할 일 파일을 만든다음 Main에 merge하는 것입니다.
# Git Tutorial 사이트에서 더 자세하게 공부 할 수 있습니다. https://backlog.com/git-tutorial/kr/stepup/stepup2_1.html
1. 먼저 Git init이나 clone으로 repository를 준비합니다. Bracn 생성전에 git repository가 update되어 있다면 "git pull" 명령어로 repository와 sync를 꼭 해야합니다.
   https://backlog.com/git-tutorial/kr/stepup/stepup2_1.html
2. 이제 이름+성+학번 으로 된 Branch를 만듭니다.(ex : git branch dean_kim_1994)
   https://backlog.com/git-tutorial/kr/stepup/stepup2_2.html
3. dean_kim_1994 branch를 사용하려면 checkout을 해야 합니다. (ex : git checkout dean_kim_1994)
	Switched to branch 'dean_kim_1994' <-- checkout이 성공 되었다면 왼쪽과 같은 메세지를 볼 수 있습니다.
	
4. git repository가 dean_kim_1994 branch로 switch되었으면 다음으로 숙제를 위해 branch 이름으로 된 Directory를 만듭니다.(ex : md dean_kim_1994)
5. 이제 windows notepad, MS Power Point, MS docs or 사용하고 싶은 편집기로 여름동안에 본인이 하고 싶은일, 이미 한일 또는 낙서등 자유롭게 작성해서 새로만든 Directory(ex : dean_kim_1994)에 저장을 합니다.
6. 저는 간단하게 몇일전에 새로 데려온 강아지를 소개해봤습니다.(심심해서...) Google Power point로 만든 파일을 PDF로 저장했습니다. File name은 Tanee.pdf로 정했습니다. 
7. 작성 후에는 꼭 add를 해줘야합니다. (ex : git add dean_kim_1994\Tanee.pdf or git add Tanee.pdf(dean_kim_1994 폴더로 cd(change directory)를 했다면))
8. 다음으로 commit을 합니다. local branch dean_kim_1994에 저장이 됩니다.(ex : git commit -m "add Tanee.pdf)
9. Cloud server에 branch 내용을 남기고 싶다면 꼭 push를 해야 합니다. branch가 생성된후에 push를 한번도 하지 않았으므로 "--set-upstream" 명령을 포함해야합니다. (ex : git push --set-upstream origin dean_kim_1994) 또 다시 변경사항을 push하고 싶다면 "git push"만 수행하면 됩니다.
10. 이제 branch dean_kim_1994의 작업이 완료 되었으므로 Main으로 merge하겠습니다. 자세한 설명을 아래 Tutorial을 참고하세요.
   https://backlog.com/git-tutorial/kr/stepup/stepup2_4.html
10. Git이 가르키고 있는 HEAD를 Main으로 Switch합니다. (ex : git checkout main)
        Switched to branch 'main'
        Your branch is up to date with 'origin/main'.
	
11. 이제 merge를 합니다. (ex : git merge dean_kim_1994)
        Updating 5ee3dc6..a544fd0
	Fast-forward
 	dean_kim_1994/Tanee.pdf | Bin 0 -> 397868 bytes
	 1 file changed, 0 insertions(+), 0 deletions(-)
        create mode 100644 dean_kim_1994/Tanee.pdf
12. merge를 했지만 local repository에만 적용이 되었습니다. Cloud server에 변경 사항을 저장하려면 "git push"를 해야합니다.
        Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
	To https://github.com/esc16/testing_KAU_collavoration.git
	   5ee3dc6..a544fd0  main -> main

13. 숙제는 여기까지 입니다. Branch 삭제 명령은 Tutorial에서 참조만 하시기 바랍니다.
    https://backlog.com/git-tutorial/kr/stepup/stepup2_5.html
    

#1차 숙제
# push 하기 전에 contributor로 등록을 해야합니다. Slack->study-git 채널에 github id 를 남겨주면 등록하겠습니다. 그리고 등록 후에 email에서 contributor를 수락해야합니다.

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
  
