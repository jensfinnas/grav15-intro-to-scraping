### Simple scraping with Xpaths

This repo: http://bit.ly/grav15-scraping

####Links you need

- [Chrome Scraper extension](https://chrome.google.com/webstore/detail/scraper/mbigbapnjcgaffohmbkdlecaccepngjd)
- [Swedish MPs](http://www.riksdagen.se/sv/ledamoter-partier/Hitta-ledamot/Bokstavsordning/)
- [XPath Tester](http://codebeautify.org/Xpath-Tester).


####More tutorials

- https://dataist.wordpress.com/2012/10/12/get-started-with-screenscraping-using-google-chromes-scraper-extension/
- http://schoolofdata.org/handbook/recipes/scraper-extension-for-chrome/


####Sample code

<code>
	<ul>
		<li>
			Name: <strong class="name">Donatello</strong>
		</li>
		<li>
			Name: <strong class="name">Michelangelo</strong>
		</li>
		<li>
			Name: <strong class="name">Raffaello</strong>
		</li>
		<li>
			Name: <strong class="name">Leonardo</strong>
		</li>
	</ul>
</code>

Get the all names: `//li/strong`
Or: `//strong[@class="name"]` 
Get first name: `//li/strong[1]`

#### XPath basics

|Expression|What is does|
-------------------------
|`//`|Search whole document|
|`//div[2]`|Get n:th tag|
|`//div[2]/table[1]/tr[3]`|Get n:th, inside n:th, inside n:th tag...|
|`//div[@class="class-name"]`|Get by attribute|
|`//div[@id="download"]`|Could be any attribute|
|`//div/text()`|Get text content of tag|


