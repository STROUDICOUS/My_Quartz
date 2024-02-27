---
SentBy: "[[Hazem El Akhnawy]]"
To:
  - "[[David Sturrock Jeffrey|David Sturrock Jeffrey]]"
  - "[[Adrienne Jeffrey|Adrienne Jeffrey]]"
  - "[[Taghrid Choucair Vizoso|Taghrid Choucair Vizoso]]"
  - "[[Paul Stroud|Paul Stroud]]"
DateTime: 2019-08-11T22:41:00
Subject: Garden Gate
tags: 
Issue:
  - "[[Side Gate Issue|Side Gate Issue]]"
description: 
icon: FiMail
OffenceType:
  - "[[Arbitrary, Unwarranted Deadline|Arbitrary, Unwarranted Deadline]]"
  - "[[Coercive Financial Ultimatum|Coercive Financial Ultimatum]]"
Progress: ingest
short_description: ""
share: "True"
myCodeProperty: "const currentSubject = dv.current().file.frontmatter['Subject'];const currentDateTime = dv.current().file.frontmatter['DateTime'];function gmailFormatDate(date, offset) {    const resultDate = new Date(date);    resultDate.setDate(resultDate.getDate() + offset);    return resultDate.toISOString().split('T')[0].replace(/-/g, '/');}const gmailFormattedFirstDate = currentDateTime ? gmailFormatDate(currentDateTime, -1) : `No start date`;const gmailFormattedLastDate = currentDateTime ? gmailFormatDate(currentDateTime, 1) : `No end date`;const searchFormattedDate = currentDateTime ? gmailFormatDate(currentDateTime, 0) : `No end date`;function displayFormatDate(dateString, offset) {  const dateObject = new Date(dateString);  dateObject.setDate(dateObject.getDate() + offset);  const formattedDate = [    dateObject.getDate().toString().padStart(2, '0'),    (dateObject.getMonth() + 1).toString().padStart(2, '0'),     dateObject.getFullYear()  ].join('-');  return formattedDate;}const displayFormattedFirstDate = currentDateTime ? displayFormatDate(currentDateTime, -1) : `No start date`;const displayFormattedLastDate = currentDateTime ? displayFormatDate(currentDateTime, 1) : `No end date`;const gmailSearchUrl = `https://mail.google.com/mail/u/0/#search/subject%3A(${encodeURIComponent(currentSubject)})+after%3A${encodeURIComponent(gmailFormattedFirstDate)}+before%3A${encodeURIComponent(gmailFormattedLastDate)}`;dv.paragraph(`> [!info] Search in your email client\\n> - - - \\n_If you are a recipient of the above email, you will be able to use the **Gmail Link** (if you use Gmail) or copy the search criteria into your email search to find it._  \\n>\\n>  <a href=\"${gmailSearchUrl}\">Search Gmail for \"${currentSubject}\" between ${displayFormattedFirstDate} and ${displayFormattedLastDate}</a>\\n>Search Criteria:\\n>   \\`\\`\\`\\`\\`Subject: ${currentSubject} received: ${searchFormattedDate.replaceAll('/','-')}\\`\\`\\`\\`\\``);"
---
<p><span><div data-callout-metadata="" data-callout-fold="" data-callout="info" class="callout node-insert-event drop-shadow"><div class="callout-title"><div class="callout-icon"><svg width="16" height="16"></svg></div><div class="callout-title-inner">Search in your email client</div></div><div class="callout-content">
<hr>
<p><em>If you are a recipient of the above email, you will be able to use the <strong>Gmail Link</strong> (if you use Gmail) or copy the search criteria into your email search to find it.</em>  </p>
<p> <a href="https://mail.google.com/mail/u/0/#search/subject%3A(Garden%20Gate)+after%3A2019%2F08%2F10+before%3A2019%2F08%2F12" target="_blank" rel="noopener">Search Gmail for "Garden Gate" between 10-08-2019 and 12-08-2019</a><br>
Search Criteria:
<code>Subject: Garden Gate received: 2019-08-11</code></p>
</div></div></span></p>

---
<p><span><div data-callout-metadata="" data-callout-fold="" data-callout="info" class="callout node-insert-event drop-shadow"><div class="callout-title"><div class="callout-icon"><svg width="16" height="16"></svg></div><div class="callout-title-inner">Search in your email client</div></div><div class="callout-content">
<hr>
<p><em>If you are a recipient of the above email, you will be able to use the <strong>Gmail Link</strong> (if you use Gmail) or copy the search criteria into your email search to find it.</em>  </p>
<p> <a href="https://mail.google.com/mail/u/0/#search/subject%3A(Garden%20Gate)+after%3A2019%2F08%2F10+before%3A2019%2F08%2F12" target="_blank" rel="noopener">Search Gmail for "Garden Gate" between 10-08-2019 and 12-08-2019</a><br>
Search Criteria:
<code>Subject: Garden Gate received: 2019-08-11</code></p>
</div></div></span></p>

<p><span><div data-callout-metadata="" data-callout-fold="-" data-callout="info" class="callout is-collapsible node-insert-event drop-shadow"><div class="callout-title"><div class="callout-icon"><svg width="16" height="16"></svg></div><div class="callout-title-inner">Test</div></div></div></span></p><p><span><blockquote>
<p>Winning?</p>
</blockquote></span></p>
```
dv.paragraph(`> [!info]- Test`)
dv.paragraph(`> Winning?`)
```



<p><span><div data-callout-metadata="" data-callout-fold="" data-callout="info" class="callout node-insert-event drop-shadow"><div class="callout-title"><div class="callout-icon"><svg width="16" height="16"></svg></div><div class="callout-title-inner">Test This has been generated in dataviewjs</div></div></div></span></p>

<p><span><div data-callout-metadata="" data-callout-fold="-" data-callout="info" class="callout is-collapsible is-collapsed node-insert-event drop-shadow"><div class="callout-title"><div class="callout-icon"><svg width="16" height="16"></svg></div><div class="callout-title-inner">test  <em>test</em></div><div class="callout-fold is-collapsed"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-chevron-down"><path d="m6 9 6 6 6-6"></path></svg></div></div><div class="callout-content" style="display: none;">
<hr>
<p>test<br>
test</p>
</div></div></span></p>
```
dv.paragraph(`> [!info]- test  *test*\n> - - -\n> test\ntest`);
```



Works
<p><span><div data-callout-metadata="" data-callout-fold="" data-callout="info" class="callout node-insert-event drop-shadow"><div class="callout-title"><div class="callout-icon"><svg width="16" height="16"></svg></div><div class="callout-title-inner">test  <em>test</em></div></div><div class="callout-content">
<hr>
<p>test<br>
test</p>
</div></div></span></p>


---
> [!info]- Test
> This has not
> 


>[!info]- Search in your email client 
> <a href="https://mail.google.com/mail/u/0/#search/from%3A(taghrid.c.v%40gmail.com)%20to%3A(Hazem.e%40hotmail.co.uk%2C%20ichattiehughes%40gmail.com)%20subject%3A(Re%3A%20Repairs%20for%2050%20Queens%20Avenue)%20after%3A2020%2F09%2F13%20before%3A2020%2F09%2F15"> Search your Gmail client</a>



AYLVL