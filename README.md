프로젝트 BUILD 과정
1.먼저 유레카 수업을 들으며 포스트 업로드 까지 실습을 진행하였다.
2.기본 테마가 아닌 다른 테마를 적용시키기 위해 http://jekyllthemes.org/ 사이트에서 테마를 탐색하였다.
3.Jekyll BlogFolio Theme 선택하였고, bloggame 폴더에 git clone하여 복사하였다.
4.gemfile을 제외한 다른 파일들을 blog 파일에 붙여넣었다.
5.add > commit > push후 블로그에 접속하였을 때 테마는 정상적으로 적용되었지만 링크가 404not found 오류가 발생하였다.
5-1.오류가 발생한 이유는 포스트를 클릭하였을 때 minho2002.github.io/2021/12/16/first-post/로 가야 하지만 minho2002.github.io/jekyll-theme-blogfolio/2021/12/16/first-post/인 없는 페이지로 간 것이였다.
6.이를 해결하기위한 방법을 모색하다가, _config.yml의 baseurl이 /jekyll-theme-blogfolio가 되어 있는것을 발견하고 빈 문자열""로 변경해 주어 해결할 수 있었다.
7.템플릿의 dummy 정보를 나의 정보로 바꾸어 주었다.
7-1._config.yml : 나의 이름, 이메일, url, 제목, 깃허브 아이디 등 (트위터는 계정이 없어 설정 X)
7-2.data/about.json : about(나의 정보 : 학번 이름)
7-3.data/header.json : 학번
7-4.data/portfolio.json : 포트폴리오(아직까지 만든 포트폴리오가 없으므로 none으로 설정)
8.Jekyll, Markdown에 대해 정리한 포스트를 업로드하였다.
