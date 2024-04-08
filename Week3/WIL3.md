## Weekly I Learned 2

2024 GDSC 개발 입문 스터디에서 배운 것(3주차)   

> 1. Git log   
>   commit 기록을 최신 순으로 확   
>   --oneline 옵션 사용하면 각 커밋 한 줄에 요약
>   commit ID를 이용해서 commit 식별(SHA-3 해시 함수를 사용)    
>   Head: 현재 작업 중인 위치, 현재 작업중인 브랜치의 가장 최근 commit, 새로운 commit이 생기면 Head도 변경

> 2. commit --amend   
>   마지막 commit의 내용에 변경이 있을 때 사용    
>   완전히 새로운 commit으로 대체, commit id가 바뀜  
>   git commit --amend -m “커밋 메시지": vim진입 없이 commit 메시지 수정    
>   git commit --amend --no-edit: commit 메시지 수정 없이 commit 수정    
>   다른 사람이 작업기반으로 쓰는 commit에 사용하지 않기
    
> 4. reset
>   commit을 제거하는 데 사용    
>   돌아갈 commit의 id를 사용, git reset ‘--option’ “<commit id>"    
>   soft: 커밋만 취소, 변경 사항이 Staging Area로 돌아감     
>   mixed: 변경 사항이 working directory로 돌아감
>   hard: 커밋을 취소, 변경 사항을 모두 제거하고 이전 커밋으로 돌아감

> 4.  revert   
>   commit을 제거하지 않고 되돌림, 되돌리기 위한 새로운 commit이 생성됨    
>   reset vs revert -> reset은 commit을 삭제하므로 위험, 다른 브랜치에도 영향을 줄 수 있음,
 => commit을 삭제하기보다 생성하여 되돌리는 revert가 안전   

