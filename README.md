
##weibo-encryption 破解微博的参数,通过上传电话号码获取用户信息比如微博id，用户喜好等，微博采用的是叠加之后在溢出，
					一个账号基本可以一直上传，本人单个账号上传了10w电话，有效



##加密原理

* 通过反编译微博APP，破解接口中的参数，上传接口为：
    *  POST https://api.weibo.cn/2/contacts/upload/full?lang=zh_CN&sflag=1&cum=B8796A40 HTTP/1.1
		Host: api.weibo.cn
		Connection: keep-alive
		Content-Length: 4446
		X-Validator: rgk1Lc6kd3eA79qYKfpLS3Suhno0nHMVppZ69xmngzU=
		User-Agent: Nexus 5_4.4.3_weibo_8.10.0_android
		X-Sessionid: af63486f-fcd7-4155-b432-f9bfecf8a604
		Content-Type: multipart/form-data;boundary=------------1538995732566
		X-Log-Uid: 1904702193
		Accept-Encoding: gzip, deflate

		--------------1538995732566
		Content-Disposition: form-data; name="v_f"
		Content-Type: text/plain;charset:"UTF-8"
		Content-Transfer-Encoding: 8bit

		2
		--------------1538995732566
		Content-Disposition: form-data; name="uid"
		Content-Type: text/plain;charset:"UTF-8"
		Content-Transfer-Encoding: 8bit

		1904702193
		--------------1538995732566
		Content-Disposition: form-data; name="moduleID"
		Content-Type: text/plain;charset:"UTF-8"
		Content-Transfer-Encoding: 8bit

		700
		--------------1538995732566
		Content-Disposition: form-data; name="wb_version"
		Content-Type: text/plain;charset:"UTF-8"
		Content-Transfer-Encoding: 8bit

		3755
		--------------1538995732566
		Content-Disposition: form-data; name="devid"
		Content-Type: text/plain;charset:"UTF-8"
		Content-Transfer-Encoding: 8bit

		359250051841177
		--------------1538995732566
		Content-Disposition: form-data; name="c"
		Content-Type: text/plain;charset:"UTF-8"
		Content-Transfer-Encoding: 8bit

		android
		--------------1538995732566
		Content-Disposition: form-data; name="wm"
		Content-Type: text/plain;charset:"UTF-8"
		Content-Transfer-Encoding: 8bit

		5311_4002
		--------------1538995732566
		Content-Disposition: form-data; name="from"
		Content-Type: text/plain;charset:"UTF-8"
		Content-Transfer-Encoding: 8bit

		108A095010
		--------------1538995732566
		Content-Disposition: form-data; name="aid"
		Content-Type: text/plain;charset:"UTF-8"
		Content-Transfer-Encoding: 8bit

		01AiTwKue6ovmaTxynr545K7O4UnwUygYoWqJJob7_9gc8Is4.
		--------------1538995732566
		Content-Disposition: form-data; name="networktype"
		Content-Type: text/plain;charset:"UTF-8"
		Content-Transfer-Encoding: 8bit

		wifi
		--------------1538995732566
		Content-Disposition: form-data; name="skin"
		Content-Type: text/plain;charset:"UTF-8"
		Content-Transfer-Encoding: 8bit

		default
		--------------1538995732566
		Content-Disposition: form-data; name="ext"
		Content-Type: text/plain;charset:"UTF-8"
		Content-Transfer-Encoding: 8bit

		contactshow
		--------------1538995732566
		Content-Disposition: form-data; name="business"
		Content-Type: text/plain;charset:"UTF-8"
		Content-Transfer-Encoding: 8bit

		account
		--------------1538995732566
		Content-Disposition: form-data; name="i"
		Content-Type: text/plain;charset:"UTF-8"
		Content-Transfer-Encoding: 8bit

		dab8b20
		--------------1538995732566
		Content-Disposition: form-data; name="client_ua"
		Content-Type: text/plain;charset:"UTF-8"
		Content-Transfer-Encoding: 8bit

		LGE-Nexus 5__weibo__8.10.0__android__android4.4.3
		--------------1538995732566
		Content-Disposition: form-data; name="content"
		Content-Type: text/plain;charset:"UTF-8"
		Content-Transfer-Encoding: 8bit

		H4sIAAAAAAAAALzVy2oUQRQG4FcJWYuec6rObVyp08qATMIkjqhxUbeGQIgguPDtrVEysSdOFIRe
		9KKq/qa/bv6q/nT6cnizWi+2r15slldfr263w+ZidbZehKewG55vzpar5eLi+jadvG/X+cvJxffb
		8gx/rb7rS4bqWUy5qQSA0HJOGL25uCsq73Kv1wsMJCxBIttu5nJ4+/zyw/lw9a3fUku7uTlMbIbt
		ggANAewSIRrTx938sF7ea0+f/LffKeSCASkyNfGUWbSk/jZJSA3tzs9uTq4Oesw/TczlH6FQ//je
		DGrLDpwDcfaRUqVcR5z4reMe9+8Tc/kbphhSizXpmFNMGMZMTfvQinDLD/pz1D9NzOVX96KcGLGg
		SKqOkaEKgrNiYT/wm8LjfrXIs/aHCmWgUDOqAGiuschYqbhnNU/7/gThaHe6P/ZnkpjLD2ZWqFXA
		BKEAth0+Ekvum7q0uPf/lOEj/ZkmZuuPKhgUhX5YVifEZjlWTRZwdB7h3h/VeHcd9/+emMtP1ELl
		RLW6tZiyuwWmXDhw/xc0POh/3xx/3b8wp5+rjJJbE0FUCr1IGt241QCieSx7vwTuvm486p8k5vIH
		8hL7M/q575Q4lt4hDRhSYkrB274/ImzMJvFofyaJf/N//gEAAP//AwAW5hQLQQgAAA==

		--------------1538995732566
		Content-Disposition: form-data; name="gsid"
		Content-Type: text/plain;charset:"UTF-8"
		Content-Transfer-Encoding: 8bit

		_2A252tP3QDeRxGedH61YW8CzNwj-IHXVT4HYYrDV6PUJbkdAKLWenkWpNUPJ5hWKuVmAxRFNER5_lb3ce9iGUmKDq
		--------------1538995732566
		Content-Disposition: form-data; name="s"
		Content-Type: text/plain;charset:"UTF-8"
		Content-Transfer-Encoding: 8bit

		f287954d
		--------------1538995732566
		Content-Disposition: form-data; name="oldwm"
		Content-Type: text/plain;charset:"UTF-8"
		Content-Transfer-Encoding: 8bit

		5311_4002
		--------------1538995732566
		Content-Disposition: form-data; name="v_p"
		Content-Type: text/plain;charset:"UTF-8"
		Content-Transfer-Encoding: 8bit

		66
		--------------1538995732566
		Content-Disposition: form-data; name="ua"
		Content-Type: text/plain;charset:"UTF-8"
		Content-Transfer-Encoding: 8bit

		LGE-Nexus 5__weibo__8.10.0__android__android4.4.3
		--------------1538995732566
		Content-Disposition: form-data; name="ft"
		Content-Type: text/plain;charset:"UTF-8"
		Content-Transfer-Encoding: 8bit

		0
		--------------1538995732566--
	*  “--------------1538995732566--”：为时间轴
    *  “X-Validator: rgk1Lc6kd3eA79qYKfpLS3Suhno0nHMVppZ69xmngzU=”：通过登录获取的用户信息，登录知道可以保持不变
    *  “X-Sessionid: af63486f-fcd7-4155-b432-f9bfecf8a604”：通过登录的用户信息，登录之后可以保持不变
    *  “Content-Disposition: form-data; name="uid"”:登录后用户id,
    *  “Content-Disposition: form-data; name="devid"”：设备id，同一台设备保持不变
    *  “Content-Disposition: form-data; name="aid"”：登录之后保持不变
    *  “Content-Disposition: form-data; name="content"”：上传用户的参数，采用了多层加密
	*  其他参数都可以保持不变
	*	最重要的是content参数的加密
			*content是里面是手机号码进行加密
			
			*每个手机号码拼成：“[\"BEGIN:VCARD\\r\\nVERSION:3.0\\r\\nPRODID:Sina Weibo      Sync/1.0\\r\\nUID:e6d7b85566fea4be1c5ad0850be24208\\r\\nFN:cS \\r\\nTEL;TYPE\\u003dcell:15099916550\\r\\nREV:20180814T135035Z\\r\\nEND:VCARD\\r\\n\",\"BEGIN:VCARD\\r\\nVERSION:3.0\\r\\nPRODID:Sina Weibo Sync/1.0\\r\\nUID:1a3cec7e59e419473b0e1822479967a8\\r\\nFN:15989297907\\r\\nTEL;TYPE\\u003dcell:13265636450\\r\\nREV:20180814T135035Z\\r\\nEND:VCARD\\r\\n\",\"BEGIN:VCARD\\r\\nVERSION:3.0\\r\\nPRODID:Sina Weibo Sync/1.0\\r\\nUID:923bc1312452e69ab567ca5e7a627818\\r\\nFN:15989297907\\r\\nTEL;TYPE\\u003dcell:15989297907\\r\\nREV:20180814T135035Z\\r\\nEND:VCARD\\r\\n\"]”
			
			*最后所有电话号码结果为：content= “[[\"BEGIN:VCARD\\r\\nVERSION:3.0\\r\\nPRODID:Sina Weibo Sync/1.0\\r\\nUID:e6d7b85566fea4be1c5ad0850be24208\\r\\nFN:cS \\r\\nTEL;TYPE\\u003dcell:15099916550\\r\\nREV:20180814T135035Z\\r\\nEND:VCARD\\r\\n\",\"BEGIN:VCARD\\r\\nVERSION:3.0\\r\\nPRODID:Sina Weibo Sync/1.0\\r\\nUID:1a3cec7e59e419473b0e1822479967a8\\r\\nFN:15989297907\\r\\nTEL;TYPE\\u003dcell:13265636450\\r\\nREV:20180814T135035Z\\r\\nEND:VCARD\\r\\n\",\"BEGIN:VCARD\\r\\nVERSION:3.0\\r\\nPRODID:Sina Weibo Sync/1.0\\r\\nUID:923bc1312452e69ab567ca5e7a627818\\r\\nFN:15989297907\\r\\nTEL;TYPE\\u003dcell:15989297907\\r\\nREV:20180814T135035Z\\r\\nEND:VCARD\\r\\n\"],[\"BEGIN:VCARD\\r\\nVERSION:3.0\\r\\nPRODID:Sina Weibo Sync/1.0\\r\\nUID:e6d7b85566fea4be1c5ad0850be24208\\r\\nFN:cS \\r\\nTEL;TYPE\\u003dcell:15099916550\\r\\nREV:20180814T135035Z\\r\\nEND:VCARD\\r\\n\",\"BEGIN:VCARD\\r\\nVERSION:3.0\\r\\nPRODID:Sina Weibo Sync/1.0\\r\\nUID:1a3cec7e59e419473b0e1822479967a8\\r\\nFN:15989297907\\r\\nTEL;TYPE\\u003dcell:13265636450\\r\\nREV:20180814T135035Z\\r\\nEND:VCARD\\r\\n\",\"BEGIN:VCARD\\r\\nVERSION:3.0\\r\\nPRODID:Sina Weibo Sync/1.0\\r\\nUID:923bc1312452e69ab567ca5e7a627818\\r\\nFN:15989297907\\r\\nTEL;TYPE\\u003dcell:15989297907\\r\\nREV:20180814T135035Z\\r\\nEND:VCARD\\r\\n\"]]”
			
			*把所有电话号码拼成的结果进行加密Encripy.a(getPhoneDatas(content))，得到即为content
			
			*返回的结果没有加密
				*通过urlhttps://api.weibo.cn/2/friendships/contact_recommend_user?networktype=wifi&uicode=10000668&moduleID=701&wb_version=3728&user_id=6637823586&c=android&i=dab8b20&s=6730418a&ft=0&ua=LGE-Nexus%205__weibo__8.8.1__android__android4.4.3&wm=90061_90050&aid=01AiTwKue6ovmaTxynr545K7Oq5aE-EeMCqe8FuEKB76UmovY.&v_f=2&v_p=63&from=1088195010&gdid=359250051841177&gsid=_2A252d_LKDeRxGeBI6FUZ8i3JwzqIHXVTJQECrDV6PUJbmdAKLVTekWpNRpjm1YGrACObX0lHp19dMtwNQwIoQvSo&lang=zh_CN&skin=default&oldwm=90061_90050&scene=1&sflag=1&luicode=10000667&has_member=1&cum=D0D4D0E2
				获取上传的用户信息，可以获取到用户id，喜好以及电话号码等信息
			
	

##需要注意的问题
* 上传到500左右返回的信息会丢失之前上传的，但是新上传的手机号码可以返回信息

##有问题反馈

* 陌陌，微博，网易云，keeper，悦动圈，酷狗，百度等app也已经破解，后期持续更新
* 有问题可以QQ群：193990770，帮忙点个星星，谢谢！！！


##代码样例
* https://github.com/yuanchao1893/weibo_encryption/tree/master/example

