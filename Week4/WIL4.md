## Weekly I Learned 4

2024 GDSC 개발 입문 스터디에서 배운 것(4주차)   

> 1. 브랜치 관리   
>   필요한 이유: 서로 작업에 영향 X, 각 브랜치가 어떤 작업 하는지 알려줌, main 브랜치 보호   
>   규칙: 승인 없이 pull request를 병합할 수 없게 제한, 특정 브랜치에 push 가능자를 제한    
    
> 2. git flow   
>   종류: Main(main, develop), Supporting(feature, release, hotfix)     
>   main(master): 기본으로 생성되고 영원히 존재하는 브랜치, 병합될 떄마다 새 버전 생성  
>   develop: 영원히 존재하는 두번째 브랜치, feature 브랜치의 기반    
>   feature: develop에서 분기, 기능 개발 후 다시 develop으로 병합    
>   release: 배포 준비를 위한 브랜치, 버그 수정, develop에서 분기 후 main으로 병합
>   hotfix: 배포 환경에서 즉각적 수정 필요시 사용, main에서 분기, main, develop에 병합
    
> 3. github flow
>   종류: main, feature    
>   main: 항상 배포 가능 상태로 유지, 병합 전 충준한 test 필요    
>   feature: main에서 분기, 다시 main으로 병합, 코드 리뷰 중요, 목적을 이름에 명시

> 4. 좋은 개발자의 태도   
>   convention을 만들어 사용    
>   구글링을 잘 활용    
>   코드에 대한 주인 의식 갖기    
>   좋은 질문을 하기    
