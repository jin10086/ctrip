# ctrip
indexurl http://you.ctrip.com/searchsite/sight/?query=%E5%8A%A8%E7%89%A9%E5%9B%AD&isAnswered=&isRecommended=&publishDate=&PageNo=1
detailurl xpath  response.xpath('//li[@class="cf"]/a/@href').extract()

detailurl http://you.ctrip.com/sight/dalian4/1100.html

title 标题 response.css('h1 a::text').extract_first() 
score 评分 response.css('.score b::text').extract_first()
dps 点评树response.css('.f_orange::text').extract_first()

景点信息
地址 response.css('.s_sight_addr::text').extract_first()
