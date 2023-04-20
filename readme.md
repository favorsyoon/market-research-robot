# 재미있는 놀이 brainstorming

market research robot for MarketInsight ,TradingOptimizing, MarketMaster ,

MarketInsight
MarketMaster

<details>
<summary>GPT 답변</summary>
 
MarketMax
TradeEase
MarketGuru
TradeOptima
MarketWizard
TradeNavigator
MarketGenie
TradeStrategist
MarketOptimizer
TradeMastermind

</details>

<details>
<summary> 뉴스 크롤링 하는 순서 정리 </summary>
 
1. 아래 URL로 들어간다. 
2. 아래 URL은 네이버뉴스(네이버전용 탭 키워드검색후 query={}, 옵션을 1일로 설정)
url = 'https://search.naver.com/search.naver?where=news&query={}&sm=tab_opt&sort=0&photo=0&field=0&pd=4&ds=&de=&docid=&related=0&mynews=0&office_type=0&office_section_code=0&news_office_checked=&nso=so%3Ar%2Cp%3A1d&is_sug_officeid=0'

3. 1페이지를 완전히 크롤링 한다.
4. 2페이지를 클릭한다.
5. 2페이지를 완전히 크롤링 한다.
6. 5초 휴식한다.
7. 3페이지로 넘어간다.

간단 HTML 만들기도 가능

</details>

<details>
<summary> 페이지 링크 넘어가는 크롤링 코드</summary>
<div class="sc_page"> <a role="button" class="btn_prev" aria-disabled="true"><i class="spnew ico_page_arr">이전</i></a><div class="sc_page_inner"><a href="?where=news&amp;sm=tab_pge&amp;query=2%EC%B0%A8%EC%A0%84%EC%A7%80&amp;sort=0&amp;photo=0&amp;field=0&amp;pd=4&amp;ds=2023.04.19.10.47&amp;de=2023.04.20.10.47&amp;cluster_rank=236&amp;mynews=0&amp;office_type=0&amp;office_section_code=0&amp;news_office_checked=&amp;nso=so:r,p:1d,a:all&amp;start=1" onclick="return goOtherCR(this, 'a=nws.paging&amp;r=1&amp;u='+urlencode(urlexpand(this.href)));" role="button" class="btn" aria-pressed="true">1</a><a href="?where=news&amp;sm=tab_pge&amp;query=2%EC%B0%A8%EC%A0%84%EC%A7%80&amp;sort=0&amp;photo=0&amp;field=0&amp;pd=4&amp;ds=2023.04.19.10.47&amp;de=2023.04.20.10.47&amp;cluster_rank=236&amp;mynews=0&amp;office_type=0&amp;office_section_code=0&amp;news_office_checked=&amp;nso=so:r,p:1d,a:all&amp;start=11" onclick="return goOtherCR(this, 'a=nws.paging&amp;r=2&amp;u='+urlencode(urlexpand(this.href)));" role="button" class="btn" aria-pressed="false">2</a><a href="?where=news&amp;sm=tab_pge&amp;query=2%EC%B0%A8%EC%A0%84%EC%A7%80&amp;sort=0&amp;photo=0&amp;field=0&amp;pd=4&amp;ds=2023.04.19.10.47&amp;de=2023.04.20.10.47&amp;cluster_rank=236&amp;mynews=0&amp;office_type=0&amp;office_section_code=0&amp;news_office_checked=&amp;nso=so:r,p:1d,a:all&amp;start=21" onclick="return goOtherCR(this, 'a=nws.paging&amp;r=3&amp;u='+urlencode(urlexpand(this.href)));" role="button" class="btn" aria-pressed="false">3</a><a href="?where=news&amp;sm=tab_pge&amp;query=2%EC%B0%A8%EC%A0%84%EC%A7%80&amp;sort=0&amp;photo=0&amp;field=0&amp;pd=4&amp;ds=2023.04.19.10.47&amp;de=2023.04.20.10.47&amp;cluster_rank=236&amp;mynews=0&amp;office_type=0&amp;office_section_code=0&amp;news_office_checked=&amp;nso=so:r,p:1d,a:all&amp;start=31" onclick="return goOtherCR(this, 'a=nws.paging&amp;r=4&amp;u='+urlencode(urlexpand(this.href)));" role="button" class="btn" aria-pressed="false">4</a><a href="?where=news&amp;sm=tab_pge&amp;query=2%EC%B0%A8%EC%A0%84%EC%A7%80&amp;sort=0&amp;photo=0&amp;field=0&amp;pd=4&amp;ds=2023.04.19.10.47&amp;de=2023.04.20.10.47&amp;cluster_rank=236&amp;mynews=0&amp;office_type=0&amp;office_section_code=0&amp;news_office_checked=&amp;nso=so:r,p:1d,a:all&amp;start=41" onclick="return goOtherCR(this, 'a=nws.paging&amp;r=5&amp;u='+urlencode(urlexpand(this.href)));" role="button" class="btn" aria-pressed="false">5</a><a href="?where=news&amp;sm=tab_pge&amp;query=2%EC%B0%A8%EC%A0%84%EC%A7%80&amp;sort=0&amp;photo=0&amp;field=0&amp;pd=4&amp;ds=2023.04.19.10.47&amp;de=2023.04.20.10.47&amp;cluster_rank=236&amp;mynews=0&amp;office_type=0&amp;office_section_code=0&amp;news_office_checked=&amp;nso=so:r,p:1d,a:all&amp;start=51" onclick="return goOtherCR(this, 'a=nws.paging&amp;r=6&amp;u='+urlencode(urlexpand(this.href)));" role="button" class="btn" aria-pressed="false">6</a><a href="?where=news&amp;sm=tab_pge&amp;query=2%EC%B0%A8%EC%A0%84%EC%A7%80&amp;sort=0&amp;photo=0&amp;field=0&amp;pd=4&amp;ds=2023.04.19.10.47&amp;de=2023.04.20.10.47&amp;cluster_rank=236&amp;mynews=0&amp;office_type=0&amp;office_section_code=0&amp;news_office_checked=&amp;nso=so:r,p:1d,a:all&amp;start=61" onclick="return goOtherCR(this, 'a=nws.paging&amp;r=7&amp;u='+urlencode(urlexpand(this.href)));" role="button" class="btn" aria-pressed="false">7</a><a href="?where=news&amp;sm=tab_pge&amp;query=2%EC%B0%A8%EC%A0%84%EC%A7%80&amp;sort=0&amp;photo=0&amp;field=0&amp;pd=4&amp;ds=2023.04.19.10.47&amp;de=2023.04.20.10.47&amp;cluster_rank=236&amp;mynews=0&amp;office_type=0&amp;office_section_code=0&amp;news_office_checked=&amp;nso=so:r,p:1d,a:all&amp;start=71" onclick="return goOtherCR(this, 'a=nws.paging&amp;r=8&amp;u='+urlencode(urlexpand(this.href)));" role="button" class="btn" aria-pressed="false">8</a><a href="?where=news&amp;sm=tab_pge&amp;query=2%EC%B0%A8%EC%A0%84%EC%A7%80&amp;sort=0&amp;photo=0&amp;field=0&amp;pd=4&amp;ds=2023.04.19.10.47&amp;de=2023.04.20.10.47&amp;cluster_rank=236&amp;mynews=0&amp;office_type=0&amp;office_section_code=0&amp;news_office_checked=&amp;nso=so:r,p:1d,a:all&amp;start=81" onclick="return goOtherCR(this, 'a=nws.paging&amp;r=9&amp;u='+urlencode(urlexpand(this.href)));" role="button" class="btn" aria-pressed="false">9</a><a href="?where=news&amp;sm=tab_pge&amp;query=2%EC%B0%A8%EC%A0%84%EC%A7%80&amp;sort=0&amp;photo=0&amp;field=0&amp;pd=4&amp;ds=2023.04.19.10.47&amp;de=2023.04.20.10.47&amp;cluster_rank=236&amp;mynews=0&amp;office_type=0&amp;office_section_code=0&amp;news_office_checked=&amp;nso=so:r,p:1d,a:all&amp;start=91" onclick="return goOtherCR(this, 'a=nws.paging&amp;r=10&amp;u='+urlencode(urlexpand(this.href)));" role="button" class="btn" aria-pressed="false">10</a></div><a href="?where=news&amp;sm=tab_pge&amp;query=2%EC%B0%A8%EC%A0%84%EC%A7%80&amp;sort=0&amp;photo=0&amp;field=0&amp;pd=4&amp;ds=2023.04.19.10.47&amp;de=2023.04.20.10.47&amp;cluster_rank=236&amp;mynews=0&amp;office_type=0&amp;office_section_code=0&amp;news_office_checked=&amp;nso=so:r,p:1d,a:all&amp;start=11" role="button" class="btn_next" aria-disabled="false" onclick="return goOtherCR(this, 'a=nws.paging&amp;r=2&amp;u='+urlencode(urlexpand(this.href)));"><i class="spnew ico_page_arr">다음</i></a> </div>

위 element는 페이지 버튼 element다.
셀레니움 라이브러리를 이용해서 크롤링을 한다.

1.  1페이지 완전히 크롤링한다.
2.  2페이지로 클릭해서 이동한다.
3.  2초 휴식
4.  2페이지에 있는 뉴스링크들을 모두 크롤링 한다.

</details>
