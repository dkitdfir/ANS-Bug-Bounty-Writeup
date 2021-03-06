# ANS-Bug-Bounty-Writeup

<b>Hacker 101 Capture The Flag [CTF] Challenge</b>

<b><i> [Flag 1] A little something to get you started</i></b>

The first one is relatively straightforward. The content says nothing but, 'Welcome to level 0. Enjoy your stay.' When the source code is viewed though, it is clear that a background image has been used. Flag 1 is available in the complete URL.

![](https://github.com/dkitdfir/ANS-Bug-Bounty-Writeup/blob/master/images/flag-1.png)

![](https://github.com/dkitdfir/ANS-Bug-Bounty-Writeup/blob/master/images/flag-1-1.png)

<b><i>[Flag 2] Micro-CMS v1</i></b>

In this scenario, creating a new page can be tested. The page id is shown in the URL after it is done. When the id is changed to 1 and viewed, the 'Testing' page is available. When the id is changed to 2 and viewed, the 'Markdown Test' page is available. These are the only 2 visible areas that are provided in addition to the custom page that was created. When other ids are checked, it is quite apparent that they give a 404 error which means the resources are not available with the exception of page number 7 that is forbidden. If editing the #7 page is tried, the form containing another flag can be viewed.

![](https://github.com/dkitdfir/ANS-Bug-Bounty-Writeup/blob/master/images/flag-2.png)

![](https://github.com/dkitdfir/ANS-Bug-Bounty-Writeup/blob/master/images/flag-2-1.png)

![](https://github.com/dkitdfir/ANS-Bug-Bounty-Writeup/blob/master/images/flag-2-2.png)

![](https://github.com/dkitdfir/ANS-Bug-Bounty-Writeup/blob/master/images/flag-2-3.png)

![](https://github.com/dkitdfir/ANS-Bug-Bounty-Writeup/blob/master/images/flag-2-4.png)

![](https://github.com/dkitdfir/ANS-Bug-Bounty-Writeup/blob/master/images/flag-2-5.png)

![](https://github.com/dkitdfir/ANS-Bug-Bounty-Writeup/blob/master/images/flag-2-6.png)

![](https://github.com/dkitdfir/ANS-Bug-Bounty-Writeup/blob/master/images/flag-2-7.png)

<b><i>[Flag 3] Micro-CMS v1</i></b>

For the 2nd Flag of Micro-CMS v1, SQLi can be tried on the 'Testing' page. Although no indication is shown on the default URL, trying the same on editing the page reveals another flag.

![](https://github.com/dkitdfir/ANS-Bug-Bounty-Writeup/blob/master/images/flag-3.png)

![](https://github.com/dkitdfir/ANS-Bug-Bounty-Writeup/blob/master/images/flag-3-1.png)

![](https://github.com/dkitdfir/ANS-Bug-Bounty-Writeup/blob/master/images/flag-3-2.png)

![](https://github.com/dkitdfir/ANS-Bug-Bounty-Writeup/blob/master/images/flag-3-3.png)

<b><i>[Flag 4] Micro-CMS v1</i></b>

If XSS vulnerability is tested on the 'Testing' page, flag 3 of the level could be retrieved.

![](https://github.com/dkitdfir/ANS-Bug-Bounty-Writeup/blob/master/images/flag-4.png)

![](https://github.com/dkitdfir/ANS-Bug-Bounty-Writeup/blob/master/images/flag-4-1.png)

<b><i>[Flag 5] Micro-CMS v1</i></b>

Script tags are not the only method to check for weaknesses. In the 'Markdown Test' page there is a button available associated with an image. An onclick parameter could be added to test further. The alert generated exposes the final Micro-CMS v1 flag.

![](https://github.com/dkitdfir/ANS-Bug-Bounty-Writeup/blob/master/images/flag-5.png)

![](https://github.com/dkitdfir/ANS-Bug-Bounty-Writeup/blob/master/images/flag-5-1.png)

![](https://github.com/dkitdfir/ANS-Bug-Bounty-Writeup/blob/master/images/flag-5-2.png)

<b><i>[Flag 6] Micro-CMS v2</i></b>

There is a login prompt. Trying weak credentials like admin, password does not help. SQLi can be attempted. It gives a traceback error with sensitive data like table name 'admins'. An SQL query can be used instead of the default credentials to perform a successful SQL injection attack and log in. A new flag is present on the private page that is now visible.

![](https://github.com/dkitdfir/ANS-Bug-Bounty-Writeup/blob/master/images/flag-6.png)

![](https://github.com/dkitdfir/ANS-Bug-Bounty-Writeup/blob/master/images/flag-6-1.png)

![](https://github.com/dkitdfir/ANS-Bug-Bounty-Writeup/blob/master/images/flag-6-2.png)

![](https://github.com/dkitdfir/ANS-Bug-Bounty-Writeup/blob/master/images/flag-6-3.png)

![](https://github.com/dkitdfir/ANS-Bug-Bounty-Writeup/blob/master/images/flag-6-4.png)

![](https://github.com/dkitdfir/ANS-Bug-Bounty-Writeup/blob/master/images/flag-6-5.png)






