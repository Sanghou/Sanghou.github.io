---
layout: post
title:  "블로그 만드는 중"
date:   2020-02-27 13:25 +0530
categories: Javascript ReactJS Jekyll
---

뭔가 더 쉽게 만드는 방법이 있지 않을까
매번 date를 수동으로 계산해줘야 하는건가?
매번 default html에서 구축하니까
어쩔 수 없이 글 작성 시간을 이렇게 적어두는건가

시간 조작 하는 사람은 없겠지 :)

```javascript
const Razorpay = require('razorpay');

let rzp = Razorpay({
	key_id: 'KEY_ID',
	secret: 'name'
});

// capture request
rzp.capture(payment_id, cost)
	.then(function (data) {
		return 2;
	})
```

명령어를 실행할 때는 jekyll serve 명령어를 쓰던데..
저장을 잘 하고 세팅 조금 더 하면 될 거 같다.

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
