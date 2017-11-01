rollingcounter
==============

숫자를 휘리릭 돌면서 목표지점에 까지  카운트 하는 jQuery 플러그인 

http://yakuyaku.github.io/rollingcounter.



사용 안내
Html 작성
출력할 숫자의 속성( data-count ) 값을 할당


<div class="counter" data-count="12312312"></div>
<button id="oneMore"> 다시 돌려라  버튼 </button>
<div class="counter" data-count="9871"></div>
<div class="counter" data-count="51513"></div>

script 작성
옵션 설명

animte : 애니메이션 효과 사용 여부 ( true/false )
attrCount : 카운트할 값이 들어가는 속성명
delayTime : 숫자별 애니메이션 간격
waitTime : 대기 시간
oneMore : 마지막에 바로 출력하지말고 한번더 돌려라 (true/false)

$(".counter").rollingCounter({
    animate : true,
    attrCount : 'data-count',
    delayTime : 20 ,
    waitTime : 1 ,
    easing : 'easeOutBounce',
    duration : 1000
});
