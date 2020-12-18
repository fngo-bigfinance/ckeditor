Ckeditor5 Online Build 사용법
==========

- [Ckeditor5 Online Build](https://ckeditor.com/ckeditor-5/online-builder/) 에 접속하여 사용할 에디터, 라이브러리를 선택합니다
<br>
이후 파일을 다운로드 합니다

      | build 
      | LICENSE.md 
      | package.json 
      | README.md 
      | sample 
      | src 
      | webpack.config.js 
  
- [Fngo Ckeditor Repository](https://github.com/fngo-bigfinance/ckeditor) 클론 받습니다. README.md, sample 은 필요가 없으니 제외한 후 파일을 교체해 줍니다 
        
  
- 교체한 프로젝트를 commit && push 합니다
  1. branch 사용 전략은 논의가 필요합니다. 현재 테스트 종료 후 마스터 브랜치에만 커밋을 하였습니다
  2. 추후 에디터 작업 시에는 feature 브랜치 생성 후 admin-front 프로젝트의 package.json 에 브랜치를 변경한 후 테스트를 진행 한 후 PR로 머지를 하면 될 것 같습니다

- 브랜치가 깃허브에 올라간 시점부터 admin-front 의 package.json 에서 해당 브랜치를 바로 사용 할 수 있습니다. <br> node_module 폴더 삭제 후 npm install && yarn start 로 admin page 테스트를 진행 하시면 됩니다
