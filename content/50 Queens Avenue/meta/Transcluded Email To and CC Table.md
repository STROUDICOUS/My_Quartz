---
myCodeProperty: "let markdownTable = '| To | CC |\\n| --- | --- |\\n';function extractText(item) {    if (!item) return '';    const match = item.match(/\\[\\[(?:[^\\]\\|]*\\|)?([^\\]]+)\\]\\]/);    return match ? match[1] : item;}const { To, CC } = dv.current().file.frontmatter;const maxCount = Math.max(To?.length || 0, CC?.length || 0);for (let i = 0; i < maxCount; i++) {    const toItem = To && i < To.length ? '[[' + extractText(To[i]) + '|' + extractText(To[i]) + ']]': '';    const ccItem = CC && i < CC.length ? '[[' + extractText(CC[i]) + '|' + extractText(CC[i]) + ']]': '';    markdownTable += `| ${toItem} | ${ccItem} |\\n`;}dv.paragraph(markdownTable);"
icon: FiCode
To:
  - "[[person1|person1]]"
  - "[[Adrienne Jeffrey|Adrienne Jeffrey]]"
  - "[[Bob and Mary Smart|Bob and Mary Smart]]"
CC:
  - "[[person3|person3]]"
DateTime: 2005-05-05T05:05:00
share: "true"
dg-publish: true
dg-home: true
---
<div><table class="dataview table-view-table"><thead class="table-view-thead"><tr class="table-view-tr-header"><th class="table-view-th"><span></span><span class="dataview small-text">1</span></th><th class="table-view-th"><span></span></th></tr></thead><tbody class="table-view-tbody"><tr><td><ul class="dataview dataview-ul dataview-result-list-ul"><li class="dataview-result-list-li"><span></span></li><li class="dataview-result-list-li"><span></span></li><li class="dataview-result-list-li"><span></span></li></ul></td><td><ul class="dataview dataview-ul dataview-result-list-ul"><li class="dataview-result-list-li"><span></span></li></ul></td></tr></tbody></table></div> 

<p><span style="overflow-x: auto;"><table>
<thead>
<tr>
<th>To</th>
<th>CC</th>
</tr>
</thead>
<tbody>
<tr>
<td><a data-href="person1" href="person1" class="internal-link" target="_blank" rel="noopener">person1</a></td>
<td><a data-href="person3" href="person3" class="internal-link" target="_blank" rel="noopener">person3</a></td>
</tr>
<tr>
<td><a data-href="Adrienne Jeffrey" href="Adrienne Jeffrey" class="internal-link" target="_blank" rel="noopener">Adrienne Jeffrey</a></td>
<td></td>
</tr>
<tr>
<td><a data-href="Bob and Mary Smart" href="Bob and Mary Smart" class="internal-link" target="_blank" rel="noopener">Bob and Mary Smart</a></td>
<td></td>
</tr>
</tbody>
</table></span></p>


| To                                   | Cc                          |    
| ------------------------------------ | --------------------------- | 
| [[Taghrid Choucair Vizoso\|Taghrid]] | [[Paul Stroud\|Paul]]       |  
|                                      | [[Hazem El Akhnawy\|Hazem]] |
<p><span style="overflow-x: auto;"><table>
<thead>
<tr>
<th>To</th>
<th>CC</th>
</tr>
</thead>
<tbody>
<tr>
<td><a data-href="person1" href="person1" class="internal-link" target="_blank" rel="noopener">person1</a></td>
<td><a data-href="person3" href="person3" class="internal-link" target="_blank" rel="noopener">person3</a></td>
</tr>
<tr>
<td><a data-href="Adrienne Jeffrey" href="Adrienne Jeffrey" class="internal-link" target="_blank" rel="noopener">Adrienne Jeffrey</a></td>
<td></td>
</tr>
<tr>
<td><a data-href="Bob and Mary Smart" href="Bob and Mary Smart" class="internal-link" target="_blank" rel="noopener">Bob and Mary Smart</a></td>
<td></td>
</tr>
</tbody>
</table></span></p>

![[Pasted image 20240226140003.png|Pasted image 20240226140003.png]]