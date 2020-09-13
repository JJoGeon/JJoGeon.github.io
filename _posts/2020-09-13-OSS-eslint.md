---
title: OSS - eslint
author: JJoGeon
date: 2020-09-13 22:00:00 +0900
categories: [OSS, eslint, sort-keys, 컨트리뷰톤]
tags: [OSS-eslint]
pin: false
---


## **1. 컨트리뷰톤을 참여 하다.**
이번에 OSS에서 진행하는 컨트리뷰톤에 참가 할 수 있게 되었다 !!  
컨트리뷰톤(Contributhon)은 '오픈소스 기여(contribute)'와 '마라톤(marathon)'의 합성어 라고 하는데  
쉽게 생각하면 각 프로젝트 주제에 맞는 활동을 통해 오픈소스에 기여 해보는 것을 말하는 것 같다.  

프론트엔드 개발자로 전향 하고 나서 eslint나 style-guide와 같은 코딩 스타일에 관한 부분에 많은 관심이 있었는데  
이번 컨트리뷰톤을 참가 하게 되면서 eslint에 대해 알아보고 실제로 이슈를 해결 하면서 어떤식으로 오픈소스에 기여하는지 알 수 있게 되었다.  

이 글은 컨트리뷰톤을 진행 하면서 어떤식으로 이슈를 찾았고, 해결 했고, 오픈소스에 코드를 기여하면 어떤 기분인지...?  
그 후기를 공유하는데 초점을 맞춰볼 생각이다!  
  
  
## **2. 진행 과정**
컨트리뷰톤은 아래와 같은 절차로 진행되었다 ! (**이건 팀마다 약간 다를 것이다.**)  
1. 간단하게 서로를 소개하고 컨트리뷰톤 관련 소개를 듣는다.
2. eslint 관련 이론 수업을 듣는다.
3. 각자 eslint 관련 이슈를 찾고 해결하여 기여한다.  
  
eslint 관련 이론으로는 멘토님께서 eslint가 무엇인지, AST 구조를 어떤식으로 코드에서 파싱 하고 있는지,  
프로젝트 구조가 어떻게 구성되어있는지 친절하게 알려 주셨다 !  
(아마 멘토님이 아니였으면 eslint입구에서 어슬렁 거리다가 포기 했을 것이다..ㅠㅠ 감사합니다. 멘토님!!)  
  
  
## **3. 이슈 찾기**
내가 생각하기에 가장 난해하고 어려웠던 구간 이였던 것 같다... @_@  
그래서 내가 컨트리뷰톤을 진행하면서 이슈를 찾았던 방법을 전수 해줄려고 한다 !! (**엄청난 꿀팁이다!! 뇌피셜이지만...ㅋ**)  
개인적으로 오픈소스에 기여하는 방법은 크게 두 가지로 나뉜다고 생각한다.  

**기여 하는 방법**
1. Docs와 같은 문서를 수정 및 추가하여 기여한다.
2. 직접 오픈소스 코드를 수정 및 추가하여 기여한다.  

문서 수정 같은 경우는 사실 영어를 잘 하지 못해서 별로 선호하는 방법의 기여는 아니라 바로 기여 리스트에서 제외했다.  
하지만 더 좋은 문서로 변경하거나 잘못된 부분을 찾는 것도 만만치 않고 되게 좋은 기여 방법이라고 생각한다!  
(영어만 잘했더라면...)  

그래서 나는 직접 오픈소스 코드를 수정 및 추가 하는 방법으로 기여를 하기로 결정 했었다.  
코드 기여를 하기 위해 나는 아래와 같은 방법으로 찾았다.  

**이슈 찾는 방법**
1. 기여 하고 싶은 오픈소스의 github 주소로 가기.
2. issue 탭으로 간 후에 원하는 라벨로 필터링
3. 맘에 드는 이슈를 확인하고 이슈 생성자에게 기여 해도 되냐고 물어보기
4. 이슈 해결하기

나 같은 경우는 기존 코드의 버그를 고치는 것 보단 새로운 기능을 추가하는걸 개인적으로 더 좋아해서 필터링을 할 때  
`accepted`, `enhancement`, `rule` 이렇게 필터를 해서 찾았다.  
여기서 이슈를 찾는데 첫번째 꿀팁은 `accepted`를 꼭!! 추가하는 것이다. 

인기가 많거나 유명한 오픈소스들은 이슈로 등록 되있더라도  
메인테이너 분들이 수락을 하지 않으면 진행 할 수 없다.  

따라서 이슈 중에 메인테이너 분들이 수락한 이슈 위주로 찾는 것이 PR을 올렸을 때 기다리는 시간을 줄일 수 있는  
`첫번째 꿀팁`이다 !  

나머지 라벨은 내가 하고 싶은 주제를 추가하면 된다.  

`두번째 꿀팁`으로는 이슈를 등록한 사람에게 내가 해도 되냐고 물어보는 것이다.  
왜냐면 이슈로 올리신 분이 먼저 해결 하고 있을 수도 있고, 자신이 해결 하려고 했을 수도 있기 때문이다.  
그래서 내가 해도 되는지를 물어보고 시작하는게 나중에 같은 이슈를 둘이서 해결 하고 있었다는 불상사를 피할 수 있는 방법이다.  

![자료1]({{site.url}}/assets/img/sample/ex1.png)  

위의 사진 자료와 같이 나는 관심있는 이슈를 찾았고  
관련 이슈를 올린 분에게 댓글을 달았는데 내가 해도 된다는 확인을 받았다 !!  

내가 찾은 이슈는 `sort-keys` 규칙에 `allowLineSeparatedGroups`옵션을 추가하는 이슈였다.  
간단하게 이슈를 설명 하자면 `sort-keys` 규칙은 하나의 Object 내에서 키들을 어떤 식으로 정렬 할건지  
정하는 eslint 규칙이다.  

```javascript
  /* eslint sort-keys: ["error", "asc"] */
  const obj1 = {
    a: 1,
    b: 2,
    c: 3  
  } // OK !

  /* eslint sort-keys: ["error", "asc"] */
  const obj2 = {
    b: 1,
    c: 2,

    a: 3
  } // ERROR !
```
근데 여기서 `obj2`를 보면 줄 바꿈으로 위의 `b,c` 키들과는 다른 그룹인 것 같은 느낌을 주고 있다.  
이때 현재 `sort-keys` 규칙으로는 저 상황을 정의 할 수 없어서 `allowLineSeparatedGroups`을 추가하고  
`allowLineSeparatedGroups`옵션의 `true | false`값에 따라 줄 바꿈으로 그룹을 나눌지 안 나눌지에 대한  
옵션을 추가하기로 했다.  

이슈 링크: [eslint-issue-12759](https://github.com/eslint/eslint/issues/12759)  

## **4. 이슈 해결**
오브젝트 내에서 줄바꿈을 확인 하는 것이 관건이라고 생각해서 스스로 줄바꿈을 확인 할 수 있는 방법에 포커스를 맞췄다.  
그 전에 `allowLineSeparatedGroups`라는 신규 옵션을 추가 하였다.  

```javascript
  const allowLineSeparatedGroups = options && options.allowLineSeparatedGroups || false;
```

저렇게 추가를 한 후에 내가 만든 규칙은 `allowLineSeparatedGroups` 옵션이 `true` 일때만 동작 하게 하려고 했다.  
(기존 옵션과 기능에 최대한 영향을 안주는 방향으로 개발 하려 노력했다!)

그 다음으로는 두 `Key` 사이에 줄바꿈으로 되있는 공백이 있는지 체크하는 로직을 만들었다.  
여기서 추가로 생각 해야할 부분은 사이에 주석이 있는지 없는지이다.  

주석 관련 정보는 `Property`에 있지 않고 `Token`에 있기 때문에 아래와 같이  
`Token`값을 활용해서 얻은 `commentOffset` 정보와 `Property`에서 얻은 `prevLine, thisLine` 정보를 활용해서  
해결 하기로 했다.

```javascript
  const beforeTokens = sourceCode.getTokensBefore(node, { includeComments: true });
  const commentOffset = getCommentOffset(prevEndLine, beforeTokens);
  const isLineSeparatedGroups = prevEndLine && checkLineSeparatedGroups(thisStartLine, prevEndLine, commentOffset);
```

필요한 정보들을 가공한 값을 활용 해서 아래의 조건을 추가 하는 것으로  
`allowLineSeparatedGroups`옵션 추가를 완료 했다!

```javascript
  if (allowLineSeparatedGroups && (isLineSeparatedGroups || thisName === null)) {
    stack.prevName = null;
    return;
  }
```

PR 링크 : [eslint-pull-12759](https://github.com/eslint/eslint/pull/13573)  

## **5. 후기**
이렇게 첫 오픈소스 기여는 `sort-keys` 규칙에 `allowLineSeparatedGroups`옵션을 추가하는 것으로 마무리 했다.  

오픈소스에 기여 해보면서 다양한 리뷰어들의 의견들도 들을 수 있었고,  
코드 작성 뿐만 아니라 문서 추가나 테스트 케이스 작성과 같은  
추가적인 작업에 대한 경험도 할 수 있어서 뜻깊은 시간이였던 것 같다.  

사실 코드를 남에게 보여주는게 굉장히 무서웠는데 (아직 코드를 잘 짠다고 생각 하지 않는다.)  
오픈소스에 기여하는 활동을 해보면서 코드를 보여주고 피드백 받는 것들이 무서운 것이 아니라는걸 알게됐다!!  

컨트리뷰톤이 끝나더라도 공감 가는 이슈나 해결 해보고 싶은 이슈가 있으면  
컨트리뷰톤과는 별개로 계속 기여를 해볼 예정이다.


