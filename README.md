# SuperRepoOfModTest     
Parent repo of a submodule     
##Getting Started     
###Clone the repository     
 1024  20250409-162819 `git clone git@github.com:rjt/SuperRepoOfModTest.git`     
 1026  20250409-162829 `cd SuperRepoOfModTest/`     
 1028  20250409-162845 `ls -latr .git/ `     
 1029  20250409-163024 `git submodule add git@github.com:rjt/SubModOfSuperRepo.git SubModule`     
 1030  20250409-163027 `ls -latr`   
 1031  20250409-163032 `cat .gitmodules `   
 1032  20250409-163129 `git commit `   
 1033  20250409-163232 `git push   `   
 1034  20250409-163723 `git subtree   `   
 1035  20250409-163748 `git --version   `   
 1036  20250409-163826 `git worktree list   `   
 1038  20250409-163915 `git whatchanged    `   
 1039  20250409-163924 `git log   `   
 1040  20250409-163932 `cat .gitmodules    `   
 1041  20250409-164017 `cat .git/config    `   
 1045  20250409-164306 history | tail -n 22 > README.md    

###cat .gitmodule  
[submodule "SubModule"]  
	path = SubModule   
	url = git@github.com:rjt/SubModOfSuperRepo.git  
   
### stream editing practice   
sed -ibak -E -e 's|( git .*$)| `\1`   |' -e 's|` git|`git|' ./README.md   
sed -ibak -E -e 's|( cat .*$)| `\1`   |' -e 's|` cat|`cat|' ./README.md   
