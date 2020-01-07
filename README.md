# SOOSAN INT tech blog

## Requirements (for testing)

- [Jekyll] 1.4.3+
- [RDiscount]

## Setup

### OSX
`$ ./install-mac.sh`

## How to write a post
1. _post 디렉토리 밑에 [Markdown] 문법으로 포스트를 작성합니다.[yyyy-mm-dd-제목.md]
2. 해당 내용을 커밋하고 메인 저장소에 푸시합니다.

        $ git add -A
        $ git commit -m "Add a post..."
        $ git push

## Testing
1. 커밋 전에 로컬 서버에서 글이 잘 써졌는지 확인하는 것이 좋습니다.

        $ jekyll serve

## Writing Tips
1. _post 폴더 내의 파일에서 YAML Front Matter block에 <code>author</code>와 <code>author-email</code>을 넣을수 있습니다. <code>author</code>는 작성한 사람, 그리고 <code>author-email</code>은 작성자 이메일, 이렇게 추가 정보를 입력할 수 있고 실제 포스트에는 mail링크가 걸리게 됩니다. ( <code>author</code>만 있으면 링크 없음 )
2. 역시 _post 폴더 내의 파일에서 YAML Front Matter block에 <code>publish</code>란에 <code>false</code>를 입력하면 게시물을 볼 수 없습니다. 포스팅 리스트에는 뜨지만 글 내용은 Coming Soon이 뜹니다. draft작업이 다 끝나면 <code>publish</code>를 <code>true</code>로 하거나 혹은 그냥 <code>publish</code> 자체를 지워주시면 됩니다.
3. 프로필 사진은 `images/profile/{email_address}.png` 로 넣어주시면 <code>author-email</code>와 매치된 사진이 화면에 나타납니다.
4. 포스트에서 사용하는 image는 `images/yyyy-mm-dd` 디렉토리에 정리하여 혼란한 `images` 디렉토리가 되지 않도록 합니다.
5. 팀 소개는 `about.html`을 수정합니다.

  [Jekyll]: http://jekyllrb.com
  [Markdown]: http://daringfireball.net/projects/markdown/
  [RDiscount]: http://dafoster.net/projects/rdiscount/

## Acknowledgement
Many thanks to Spoqa team who made their blog open source. Thank you.
