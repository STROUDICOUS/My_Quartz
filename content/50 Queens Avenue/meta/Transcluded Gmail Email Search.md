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
description: "[[Hazem El Akhnawy|Hazem]] demands Adrienne and David redo the shareholder-agreed works to the [[Side Gate Issue|Side Gate]], threatening to hire a structural engineer if changes aren't made within 14 days."
icon: FiMail
OffenceType:
  - "[[Arbitrary, Unwarranted Deadline|Arbitrary, Unwarranted Deadline]]"
  - "[[Coercive Financial Ultimatum|Coercive Financial Ultimatum]]"
Progress: ingest
short_description: ""
share: "True"
myCodeProperty: "const currentSubject = dv.current().file.frontmatter['Subject'];const currentDateTime = dv.current().file.frontmatter['DateTime'];function gmailFormatDate(date, offset) {    const resultDate = new Date(date);    resultDate.setDate(resultDate.getDate() + offset);    return resultDate.toISOString().split('T')[0].replace(/-/g, '/');}const gmailFormattedFirstDate = currentDateTime ? gmailFormatDate(currentDateTime, -1) : `No start date`;const gmailFormattedLastDate = currentDateTime ? gmailFormatDate(currentDateTime, 1) : `No end date`;const searchFormattedDate = currentDateTime ? gmailFormatDate(currentDateTime, 0) : `No end date`;function displayFormatDate(dateString, offset) {  const dateObject = new Date(dateString);  dateObject.setDate(dateObject.getDate() + offset);  const formattedDate = [    dateObject.getDate().toString().padStart(2, '0'),    (dateObject.getMonth() + 1).toString().padStart(2, '0'),     dateObject.getFullYear()  ].join('-');  return formattedDate;}const displayFormattedFirstDate = currentDateTime ? displayFormatDate(currentDateTime, -1) : `No start date`;const displayFormattedLastDate = currentDateTime ? displayFormatDate(currentDateTime, 1) : `No end date`;const gmailSearchUrl = `https://mail.google.com/mail/u/0/#search/subject%3A(${encodeURIComponent(currentSubject)})+after%3A${encodeURIComponent(gmailFormattedFirstDate)}+before%3A${encodeURIComponent(gmailFormattedLastDate)}`;dv.paragraph(`> [!info]- Search in your email client\\n> <a href=\"${gmailSearchUrl}\">Search Gmail for \"${currentSubject}\" between ${displayFormattedFirstDate} and ${displayFormattedLastDate}</a>   \\`\\`\\`\\`\\`Subject: ${currentSubject} recieved: ${searchFormattedDate.replaceAll('/','-')}\\`\\`\\`\\`\\``);"
---
<p><span><div data-callout-metadata="" data-callout-fold="-" data-callout="info" class="callout is-collapsible is-collapsed node-insert-event drop-shadow"><div class="callout-title"><div class="callout-icon"><svg width="16" height="16"></svg></div><div class="callout-title-inner">Search in your email client</div><div class="callout-fold is-collapsed"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-chevron-down"><path d="m6 9 6 6 6-6"></path></svg></div></div><div class="callout-content" style="display: none;">
<p><a href="https://mail.google.com/mail/u/0/#search/subject%3A(Garden%20Gate)+after%3A2019%2F08%2F10+before%3A2019%2F08%2F12" target="_blank" rel="noopener">Search Gmail for "Garden Gate" between 10-08-2019 and 12-08-2019</a>   <code>Subject: Garden Gate recieved: 2019-08-11</code></p>
</div></div></span></p>

---
<p><span><div data-callout-metadata="" data-callout-fold="-" data-callout="info" class="callout is-collapsible is-collapsed node-insert-event drop-shadow"><div class="callout-title"><div class="callout-icon"><svg width="16" height="16"></svg></div><div class="callout-title-inner">Search in your email client</div><div class="callout-fold is-collapsed"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-chevron-down"><path d="m6 9 6 6 6-6"></path></svg></div></div><div class="callout-content" style="display: none;">
<p><a href="https://mail.google.com/mail/u/0/#search/subject%3A(Garden%20Gate)+after%3A2019%2F08%2F10+before%3A2019%2F08%2F12" target="_blank" rel="noopener">Search Gmail for "Garden Gate" between 10-08-2019 and 12-08-2019</a>   <code>Subject: Garden Gate recieved: 2019-08-11</code></p>
</div></div></span></p>

<p><span><div data-callout-metadata="" data-callout-fold="-" data-callout="info" class="callout is-collapsible node-insert-event drop-shadow"><div class="callout-title"><div class="callout-icon"><svg width="16" height="16"></svg></div><div class="callout-title-inner">Test</div></div></div></span></p><p><span><blockquote>
<p>Winning?</p>
</blockquote></span></p>
```
dv.paragraph(`> [!info]- Test`)
dv.paragraph(`> Winning?`)
```

<pre class="dataview dataview-error">Evaluation Error: SyntaxError: Unexpected end of input
    at DataviewInlineApi.eval (plugin:dataview:18638:21)
    at evalInContext (plugin:dataview:18639:7)
    at asyncEvalInContext (plugin:dataview:18649:32)
    at DataviewJSRenderer.render (plugin:dataview:18670:19)
    at DataviewJSRenderer.onload (plugin:dataview:18260:14)
    at e.load (app://obsidian.md/app.js:1:1158302)
    at DataviewApi.executeJs (plugin:dataview:19198:18)
    at eval (plugin:obsidian-mkdocs-publisher:24:34676)
    at Generator.next (&lt;anonymous&gt;)
    at n (plugin:obsidian-mkdocs-publisher:2:1084)</pre>
```
dv.paragraph(`> [!info] Test`)
dv.paragraph(`> Winning?`)
```

<p><span><div data-callout-metadata="" data-callout-fold="-" data-callout="info" class="callout is-collapsible is-collapsed node-insert-event drop-shadow"><div class="callout-title"><div class="callout-icon"><svg width="16" height="16"></svg></div><div class="callout-title-inner">Test</div><div class="callout-fold is-collapsed"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-chevron-down"><path d="m6 9 6 6 6-6"></path></svg></div></div><div class="callout-content" style="display: none;">
<p>This has been generated in dataviewjs</p>
</div></div></span></p>

```js
dv.paragraph('> [!info]- Test\nThis has been generated in dataviewjs')
```

<p><span><div data-callout-metadata="" data-callout-fold="" data-callout="info" class="callout node-insert-event drop-shadow"><div class="callout-title"><div class="callout-icon"><svg width="16" height="16"></svg></div><div class="callout-title-inner">Test</div></div></div></span></p><p><span><blockquote>
<p>Winning?</p>
</blockquote></span></p>
```
dv.paragraph(`> [!info] Test`)
dv.paragraph(`> Winning?`)
```

<p><span><div data-callout-metadata="" data-callout-fold="-" data-callout="info" class="callout is-collapsible is-collapsed node-insert-event drop-shadow"><div class="callout-title"><div class="callout-icon"><svg width="16" height="16"></svg></div><div class="callout-title-inner">Test</div><div class="callout-fold is-collapsed"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-chevron-down"><path d="m6 9 6 6 6-6"></path></svg></div></div><div class="callout-content" style="display: none;">
<p>Something here</p>
</div></div></span></p>
```
dv.paragraph('> [!info]- Test' + '\n' + '> Something here')

```
<p><span><div data-callout-metadata="" data-callout-fold="" data-callout="info" class="callout node-insert-event drop-shadow"><div class="callout-title"><div class="callout-icon"><svg width="16" height="16"></svg></div><div class="callout-title-inner">Test</div></div><div class="callout-content">
<p>Something here</p>
</div></div></span></p>
```
dv.paragraph('> [!info] Test' + '\n' + '> Something here')

```

> [!info]- Test
> This has not
