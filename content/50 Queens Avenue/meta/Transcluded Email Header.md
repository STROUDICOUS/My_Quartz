---
icon: FiCode
Subject: Garden Gate
share: "True"
myCodeProperty: "dv.header(1, `From: ${dv.current().SentBy}`);const dateTime = dv.current().file.frontmatter['DateTime'];function formatDateTime(dateTime) {    const date = new Date(dateTime);    const options = { weekday: 'short', year: 'numeric', month: 'long', day: 'numeric' };    let day = date.getDate();    let formattedDate = new Intl.DateTimeFormat('en-GB', options).format(date);    let ordinal = day + (day % 10 == 1 && day != 11 ? 'st' : (day % 10 == 2 && day != 12 ? 'nd' : (day % 10 == 3 && day != 13 ? 'rd' : 'th')));    formattedDate = formattedDate.replace(day, ordinal);    let timePart = date.toLocaleTimeString('en-GB', { hour: '2-digit', minute: '2-digit', hour12: true }).toLowerCase().replace(\" \", \"\");    timePart = timePart.replace(\":\", \".\");    return `${formattedDate} at ${timePart}`;}const formattedDateTime = dateTime ? formatDateTime(dateTime) : \"Date not provided\";dv.paragraph(`### On ${formattedDateTime}`);"
SentBy: "[[Paul Stroud]]"
---
<h1><span><p>From: <a data-tooltip-position="top" aria-label="50 Queens Avenue/supporting information/Paul Stroud.md" data-href="50 Queens Avenue/supporting information/Paul Stroud.md" href="50 Queens Avenue/supporting information/Paul Stroud.md" class="internal-link" target="_blank" rel="noopener">Paul Stroud</a></p></span></h1><p><span><h3 data-heading="On Date not provided">On Date not provided</h3></span></p>

<h1><span><p>From: <a data-tooltip-position="top" aria-label="50 Queens Avenue/supporting information/Paul Stroud.md" data-href="50 Queens Avenue/supporting information/Paul Stroud.md" href="50 Queens Avenue/supporting information/Paul Stroud.md" class="internal-link" target="_blank" rel="noopener">Paul Stroud</a></p></span></h1><p><span><h2 data-heading="From: [[50 Queens Avenue/supporting information/Paul Stroud.md|Paul Stroud]] On Date not provided">From: <a data-tooltip-position="top" aria-label="50 Queens Avenue/supporting information/Paul Stroud.md" data-href="50 Queens Avenue/supporting information/Paul Stroud.md" href="50 Queens Avenue/supporting information/Paul Stroud.md" class="internal-link" target="_blank" rel="noopener">Paul Stroud</a> On Date not provided</h2></span></p>

# Header 1
## Header 2
### Header 3
#### Header 4
##### Header 5
###### Header 6


