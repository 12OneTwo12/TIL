# CSS  
#### [ 2022-07-12 ]  
  
    어제 작성했던 html 파일이 내가 보던 웹 사이트들에 비해 너무 단조로워 보였다.  
    그러기에 조금 꾸며보고자 했다.  
    어떻게 해야할까.  
    찾아보니 CSS를 이용하면 된다고 한다.  
    그렇다면 CSS는 무엇일까?  
      
* #### CSS란  
    
  ![image url](https://github.com/12OneTwo12/TIL/blob/main/Html/og.jpg?raw=true)
    
      CSS는 Cascading Style Sheets의 약자인데, 마크업 언어가 실제 표시되는 방법을 기술하는 스타일 언어(style sheet language)로, HTML과 XHTML에 주로 쓰이며, XML에서도 사용할 수 있다.  
  간단하게 설명한다면 HTML은 웹사이트에서 화면에 표시되는 정보이며, CSS는 웹 사이트에서 화면에 표시되는 정보 들을 꾸며주는 역할을 한다.  
    
  예를 보면 더 쉽게 이해할 수 있는데 우리가 흔히 이용하는 네이버 웹 사이트에서 css가 없어졌다고 가정해보자.  
  
  ![image url](https://github.com/12OneTwo12/TIL/blob/main/CSS/naverwithoutcss.png?raw=true)  
    
  평소 우리가 보던 네이버와는 사뭇 다른 모습이다.  
  마치 무엇인가 많이 비어있는 것처럼 보이는 별로 손이 잘 안가게 되는 웹 사이트 처럼 생겼다.  
  실제 네이버 사이트와 비교해보면 더욱 잘 느낄 수 있는데                  [참조. [NAVER web site link]](https://www.naver.com/)   
  이처럼 우리의 눈은 이미 CSS를 이용한 웹 사이트들을 항상 겪고 있었다고 볼 수 있다.  
  그렇다면 내가 만든 html에도 적용 해보고자 한다.  
      
  
* #### CSS를 적용하는 방법  
  
  CSS를 적용하는 방법에는 크게 3가지가 있다고 한다.  
    
      *   Inline Style 적용 방식  
       
      *   Internal Style 적용 방식  
        
      *   External Style 적용 방식  
  
  * #### Inline Style이란  
  
    
      인라인 스타일이란 HTML 요소 내부에 style 속성을 사용하여 CSS 스타일을 적용하는 방법이다.  
      간단한 예제를 봐서 이해해보자.  
        
      ```html
        <html>
          <body>
            <h1 style="color:blue;">
              이 문장은 Inline Style로 꾸며봤습니다.
            </h1>
          </body>
        </html>
      ```  
        
       실행해본 결과 글씨가 파란색으로 변했다.  
       style이라고 하는 attribute를 지정하여 글씨의 색상을 파란색이라는 값(value)으로 바꾼 것이다.  
       그러나 이번엔 간단한 코드 였기에 바로 가능했지만 문장이 여러개라면 어떻게 해야할까?  
       매번 모든 태그들에 style을 지정해줘야 하는걸까?  
       상상만 해도 여간 불편한게 아닐 것이다. 다른 방법이 없을까?  
       
  * #### Internal Style이란  
  
       HTML 문서 내의 head 태그에 style 태그를 사용하여 CSS 스타일을 적용하는 방법이다.  
       마찬가지로 예제를 봐서 이해해보자.  
       
       ```html
        <html>
          <head>
            <style>
              .internal{
                  color: blue; 
               }
            </style>
          </head>
          
          <body>
            <h1 class="internal"> 이 문장은 Internal Style로 꾸며봤습니다.</h1>
          </body>
        <html>
       ```  
  
      실행결과 마찬가지로 글씨가 파란색으로 나왔다.  
      h1 태그를 internal이라는 class로 분류하였고,  
      head 태그 안에 style 태그를 사용하여 internal이라고 부르는 class의 글자 색을 파란색으로 바꿔줬다.  
      그렇다면 이것보다 주로 쓰이는 방법도 있을까?  
        
  * #### External Style이란  
   
      
