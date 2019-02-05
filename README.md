# Accessibility testing using pa11y

##  Test url:  https://bitsofco.de/
### Config file

```
>nano .pa11yci

{
  "defaults": {
    "hideElements": "#carbonads",
    "ignore": [ "notice", "warning" ]
  },
  "urls": [ "https://bitsofco.de" ]
}
```

### Test execution

```
$ pa11y-ci --threshold 10
Running Pa11y on 1 URLs:
 > https://bitsofco.de - 0 errors

✔ 1/1 URLs passed
```
##  Test url:  https://www.yahoo.com

```

$ pa11y-ci --threshold 10
Running Pa11y on 1 URLs:
 > http://www.yahoo.com - 44 errors

Errors in http://www.yahoo.com:

 • Iframe element requires a non-empty title attribute that identifies the frame.

   (#yui_3_18_0_3_1549234496883_101 > iframe)

   <iframe width="0" height="0" name="__cmpLocator" style="display: none;"></iframe>

 • Img element missing an alt attribute. Use the alt attribute to specify a short text alternative.

   (#yns-panel > div:nth-child(2) > ul > li:nth-child(1) > a > img)

   <img class="yns-img yns-redImg" src="https://s.yimg.com/cv/ae/news/Purple-News.png">

 • Img element missing an alt attribute. Use the alt attribute to specify a short text alternative.

   (#yns-panel > div:nth-child(2) > ul > li:nth-child(2) > a > img)

   <img class="yns-img yns-redImg" src="https://s.yimg.com/cv/ae/news/Purple-News.png">

 • Img element missing an alt attribute. Use the alt attribute to specify a short text alternative.

   (#yns-panel > div:nth-child(2) > ul > li:nth-child(3) > a > img)

   <img class="yns-img yns-redImg" src="https://s.yimg.com/cv/ae/news/Purple-News.png">

 • Img element missing an alt attribute. Use the alt attribute to specify a short text alternative.

   (#yns-panel > div:nth-child(2) > ul > li:nth-child(4) > a > img)

   <img class="yns-img yns-redImg" src="https://s.yimg.com/cv/ae/news/Purple-News.png">

 • Img element with empty alt text must have absent or empty title attribute.

   (#Stream > li:nth-child(1) > div:nth-child(2) > div:nth-child(3) > a > img)

   <img
   src="https://s.yimg.com/uu/api/res/1.2/TUrG2k6zIO3IGIfCxxzA5A--~B/Zmk9c3RyaW07aD0zODg7cHlvZmY9MDtxPTk1O3c9NzIwO3NtPTE7YXBwaWQ9eXRhY2h5b24-/https://media-mbst-pub-ue1.s3.amazonaws.com/creatr-uploaded-images/2019-02/2a805030-27ef-11e9-bd7b-feeaf79...

```
