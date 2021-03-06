# অবদান স্বীকার #

এই প্রকল্পটি একটি ফর্ক। [মূল রিপোটি](https://github.com/senchalabs/cssbeautify) দেখুন।


# সিএসএস বিউটিফাই #

সিএসএস বিউটিফাই [সিএসএস](http://www.w3.org/Style/CSS/) এ লিখিত স্টাইলের নতুন রূপ তৈরির জন্য করা জাভাস্ক্রিপ্ট ইমপ্লিমেন্টেশন।

নিচে একটি স্টাইল দেয়া হলোঃ

```css
menu{color:red} navigation{background-color:#333}
```

সিএসএস বিউটিফাই যা করবেঃ

```css
menu {
    color: red
}

navigation {
    background-color: #333
}
```

[amirmehrabi.github.io/cssstyler/](https://amirmehrabi.github.io/cssstyler/) তে এটি অনলাইনে চেষ্টা করুন।

আরও উদাহরণের জন্য, এর [টেস্ট স্যুট](http://cssbeautify.com/test/) দেখুন।


# স্ক্রিনশট #

![screencapture-localhost-cssstyler-index-en-html-2019-10-15-15_36_23](https://user-images.githubusercontent.com/3878847/66830108-93ad8700-ef61-11e9-95d9-df30792b5aef.png)

## cssbeautify() ফাংশন ব্যবহার ##

সিএসএস বিউটিফাই জাভাস্ক্রিপ্ট দিয়ে লেখা হওয়ায় সেখানে জাভাস্ক্রিপ্ট রান হয়, সেখানে এটিও রান করা যাবে।

এপিআইটি একদম সহজ।

```javascript
var result = cssbeautify(style, options);
```

**options** ফরম্যাট ঠিক করার জন্য ঐচ্ছিক অবজেক্ট। এখন পর্যন্ত অপশনগুলো হলোঃ 

  *  <code>indent</code> ডিক্লারেশনের ইন্ডেন্টেশনের জন্য ব্যবহৃত (ডিফল্ট ৪টি স্পেস)
  *  <code>openbrace</code> কার্কি ব্রেসের অবস্থান ঠিক করে, হয় *end-of-line* (ডিফল্ট) বা *separate-line*.
  *  <code>autosemicolon</code> সর্বদা শেষ রুলসেটের পরে সেমিকলন বসায় (ডিফল্ট *false*)

কল উদাহরণঃ

```javascript
var beautified = cssbeautify('menu{opacity:.7}', {
    indent: '  ',
    openbrace: 'separate-line',
    autosemicolon: true
});
```

## অবদান রাখুন ##

আপনার অবদান স্বাগতম! আরও তথ্যের জন্য অনুগ্রহপূর্বক [অবদান গাইড](https://github.com/AmirMehrabi/cssstyler/blob/master/CONTRIBUTING.md) পড়ুন।

## লাইসেন্স ##

Copyright (C) 2012 Sencha Inc.
Copyright (C) 2011 Sencha Inc.

এতদ্বারা নিন্মরূপ শর্তে বিনামূল্যে যেকোনো ব্যক্তিকে অনুমতি দেয়া হলো যে এই সফটওয়্যার এবং সংশ্লিষ্ট ডকুমেন্টেশন ফাইল ("সফটওয়্যার") নিয়ে বিনা বাধায় ব্যবহার, অনুলিপি, পরিবর্তন, একত্রীকরণ, প্রকাশ, বিতরণ, লাইসেন্সকরণ এবং/অথবা বিক্রির মতো কাজ করার জন্য এর অনুলিপি রাখা যাবে।

উপরোক্ত কপিরাইট নোটিশ এবং এই অনুমতি পত্র এই সফটওয়্যারের সকল কপিতে অথবা অংশে অন্তর্ভুক্ত করতে হবে।

এই সফটওয়্যারটি কোনোরূপ ওয়ারেন্টি ছাড়া প্রদান করা হচ্ছে। এই সফটওয়ার থেকে, এর বাইরের এবং এর ভিতরের কোনো বিষয়ে কখনোও এটির লেখকবৃন্দ এবং কপিরাইট হোল্ডার দায়ী হবেন না।
