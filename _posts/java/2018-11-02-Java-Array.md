---
layout: post
title: Array
categories: [java]
tags: [java]
comments: true
---

### 2차원 배열

- 2개의 int값을 가지는 배열을 3개 생성한다

~~~
int arr2[][] = new int[3][2];
~~~

- 각 배열의 크기를 다르게 지정해줄 수 있다
- 처음에는 1차원 배열 크기만 정해주고 그 후에 2차원 배열의 크기를 정한다

~~~
int arr2[][] = new int[3][];     // 1차원 배열의 크기를  설정
arr[0] = new int[2];             // 각 배열 크기를  다르게 할 수도 있다          
arr[1] = new int[4];
arr[2] = new int[8];
~~~

- 선언, 생성, 초기화를 동시에 함
~~~
#int arr3[][] = {0번배열, 1번배열 3번배열} ;
~~~

### 2차원 배열 순회

~~~
int arr3[][] = {array, array, array};
for(int i = 0; i < arr3.length; ++i)
{
    for(int j = 0; j < arr3[i].length; ++j)
     {
     System.out.println("arr3["+i+"]["+j+"]="+arr3[i][j]);
     }
}
~~~

### 배열 복사

~~~
System.arraycopy(src, srcPos, dest, destPos, length);
~~~
- src : 복사원본
- srcPos : 복사원본의  복사 시작 위치
- dest : 복사할 대상
- destPos : 복사할 대상의 복사 시작 위치
- length : 복사할 길이

<div id="disqus_thread"></div>
<script>

/**
*  RECOMMENDED CONFIGURATION VARIABLES: EDIT AND UNCOMMENT THE SECTION BELOW TO INSERT DYNAMIC VALUES FROM YOUR PLATFORM OR CMS.
*  LEARN WHY DEFINING THESE VARIABLES IS IMPORTANT: https://disqus.com/admin/universalcode/#configuration-variables*/
/*
var disqus_config = function () {
this.page.url = PAGE_URL;  // Replace PAGE_URL with your page's canonical URL variable
this.page.identifier = PAGE_IDENTIFIER; // Replace PAGE_IDENTIFIER with your page's unique identifier variable
};
*/
(function() { // DON'T EDIT BELOW THIS LINE
var d = document, s = d.createElement('script');
s.src = 'https://parkwonhui.disqus.com/embed.js';
s.setAttribute('data-timestamp', +new Date());
(d.head || d.body).appendChild(s);
})();
</script>
<noscript>Please enable JavaScript to view the <a href="https://disqus.com/?ref_noscript">comments powered by Disqus.</a></noscript>
                            