<h1 align="center">
  <br>
    🔍 Miscellaneous
  <br>
  <br>
</h1>


```pr0xh4ck © 2022```

---

# Agenda 
- [Search Engine](#search-engine)
- [Keywords Research](#keyword-research)
- [Mega Download Bypass](#mega-download-bypass)
- [Activation](#Activation)
- [Google Dorks](#google-dork)
- [Shodan Dork](#Shodan-Dork)
- [Ports list](#port-list)
- [Open Sources](#open-sources)
- [Never Stop Learning](#never-stop-learning)
- [Others](#Others)









---------------------------------------------------------------------------------------------------------------

#### search-engine
- [google](https://www.google.com/)
- [bing](https://www.bing.com)
- [yahoo](https://www.yahoo.com/)
- [duckduckgo](https://duckduckgo.com/)
- [yandex](https://yandex.com/)
- [baidu](https://www.baidu.com/)
- [ask](https://www.ask.com/)
- [excite](https://www.excite.com/)
- [fofa](https://fofa.so/)

  - [Google hacking database](https://www.exploit-db.com/google-hacking-database)
  - [Searchengine](https://searchengine.party/)
  - [Programable search](https://cse.google.com/cse?cx=957ae734f66a7a3e0#gsc.tab=0)
  - [Anonfiles search](https://cse.google.com/cse?cx=f9e53d19d3e812ef6)
  - [Pastebin search](https://cse.google.com/cse?cx=000977868543400066238:8pmcka2t6qy)
  - [Zippy Share Search](https://zippysharesearch.com/)
  - [File listing](https://filelisting.com/)
  - [Odcrawler](https://odcrawler.xyz/)
  - [Filechef](https://www.filechef.com/)
  - [Dedigger](https://www.dedigger.com/)
  - [Weboas](https://weboas.is/)
  - [Searchfiles](https://searchfiles.de/)
  - [Filesearch](https://www.filesearch.link/)
  - [Eyeofjustice](https://www.eyeofjustice.com/od/)
  - [Megadb](https://megadb.tweakly.net/search)


----
----


#### keyword-research
  - [keyword](https://www.keyword.io/)
  - [prnt.sc/hexfky](https://prnt.sc/hexfky) 


-----
-----


#### mega-download-bypass
> Tool
  - [megabasterd](https://github.com/tonikelope/megabasterd) - Yet another unofficial (and ugly) cross-platform MEGA downloader/uploader/streaming suite. 

> Proxy List
  - [free-proxy-list](https://free-proxy-list.net/)
  - [us-proxy](https://us-proxy.org/) - Get your free proxy  1
  - [proxyscrape](https://proxyscrape.com/free-proxy-list) - Get your free proxy 2
  - [advanced](https://advanced.name/freeproxy) - Get your free proxy 3
  - [premproxy](https://premproxy.com/list/) - Get your free proxy 4 
  - [sslproxies](https://www.sslproxies.org/) - Get your free proxy 5 
  - [proxynova](https://www.proxynova.com/) - Get your free proxy 6
  - [proxydb](http://proxydb.net/) - Get your free proxy 7

> Filter Proxies
```python
x = """
# delete this line and paste your proxy list then run
"""
for y in x.split("\n"):
  if(y[-4:] == "8080"):
    print(y)
```

> Or Go 
- [onecompiler](https://onecompiler.com/python/3xxtpynpn)


---------------------------
-----------------------

### Activation
- [Microsoft-Activation-Scripts](https://github.com/massgravel/Microsoft-Activation-Scripts) - A collection of scripts for activating Microsoft products using HWID / KMS38 / Online KMS activation methods with a focus on open-source code, less antivirus detection and user-friendliness. 














-----------------
--------------








----
---


#### google-dork

- [google-dorks](https://github.com/Proviesec/google-dorks) - Bug bounty google dork

- [google-hacking-database](https://www.exploit-db.com/google-hacking-database)

**intitle** – Specifying intitle, will tell google to show only those pages that have the term in their html title. For example intitle:”login page” will show those pages which have the term “login page” in the title text.

**allintitle** – Similar to intitle, but looks for all the specified terms in the title.

**inurl** – Searches for the specified term in the url. – For example inurl:”login.php” or inurl:login.jsp intitle:login.

**allinurl** – Same as inurl, but searches for all terms in the url.

**filetype** – Searches for specific file types. filetype:pdf will looks for pdf files in websites. Similarly filetype:txt looks for files with extension .txt – For example “sensitive but unclassified” filetype:pdf

**ext** – Similar to filetype. ext:pdf finds pdf extension files.

**intext** – Searches the content of the page. Somewhat like a plain google search. For example intext:”index of /” or Host=*.* intext:enc_UserPassword=* ext:pcf

**allintext** – Similar to intext, but searches for all terms to be present in the text.

**site** – Limits the search to a specific site only. – For example site:example.com

**cache** -  this dork will show you the cached version of any website

**'*'** - wildcard used to search pages that contain “anything” before your word.

**+** - used to concatenate words, useful to detect pages that use more than one specific key

**-** - minus operator is used to avoiding showing results that contain certain words

**|** - this is a logical operator,

If a hacker wishes to search by a field other than the URL, the following can be effectively substituted:

- intitle:
- inurl:
- intext:
- define:
- site:
- phonebook:
- maps:
- book:
- froogle:
- info:
- movie:
- weather:
- related:
- link:





----







----
## Google Dork

- Extension
```text
site: *.example.com ext:php OR ext:js OR ext:txt OR ext:pdf
```

- Open Redirect
```text
site: *.example.com inurl:& AND inurl:url
```

- SQL Injection
```text
site: *.example.com intext:"You have an error in your SQL syntax"
```

- File Type
```text
site: *.example.com filetype:pdf
```

- GraphQL 
```text
site: *.example.com inurl:/graphql/
```


------------------
-------------
### Shodan-Dork

Citrix - Find Citrix Gateway. Example: title:“citrix gateway”[/align]

Wifi Passwords - Helps to find the cleartext wifi passwords in Shodan. Example: html:“def_wirelesspassword”

Surveillance Cams - With username admin and password. Example: NETSurveillance uc-httpd

Fuel Pumps connected to internet - No auth required to access CLI terminal. Example: “privileged command” GET

Windows RDP Password - But may contain secondary windows auth. Example: “\x03\x00\x00\x0b\x06\xd0\x00\x00\x124\x00”

Mongo DB servers - It may give info about mongo db servers and dashboard. Example: “MongoDB Server Information” port:27017 -authentication

FTP servers allowing anonymous access - Complete Anon access. Example: “220” “230 Login successful.” port:21

Jenkins - Jenkins Unrestricted Dashboard. Example: x-jenkins 200

Hacked routers - Routers which got compromised. Example: hacked-router-help-sos

Open ATM - May allow for ATM Access availability. Example: NCR Port:“161”

Telnet Access - NO password required for telnet access. Example: port:23 console gateway

Misconfigured Wordpress Sites - The wp-config.php if accessed can give out the database credentials. Example: http.html:"* The wp-config.php creation script uses this file"

Hiring - Find sites hiring. Example: “X-Recruiting:”

Android Root Bridge - Find android root bridges with port 5555. Example: “Android Debug Bridge” “Device” port:5555

Etherium Miners - Shows the miners running ETH. Example: “ETH - Total speed”

Tesla Powerpack charging Status - Helps to find the charging status of tesla powerpack. Example: http.title:“Tesla PowerPack System” http.component:“d3” -ga3ca4f2


-----------------------------
--------------------------





## PGP(Pretty Good Privacy)

- Command for tool installation
```bash
sudo apt-get install gnupg2 gpa
```

- Create your key command
```bash
gpg --full-generate-key
```

- Open GUI tool
```bash
sudo gpa
```

------------------


### port-list

- [ports-list](https://github.com/maraisr/ports-list) - Offical list of UDP/TCP ports to descriptions



------------


### open-sources

- [videvo](https://www.videvo.net/) - Get your free video 



----------------------------------------------------
-----------------------------------------------------
### never-stop-learning

- How to Convert web browser to a Notepad
```html
data:text/html, <html contenteditable>
```
- Best Site to Download Free Software
- [getintopc](https://getintopc.com/)
- [piratepc](https://piratepc.me/)
- [free4pc](https://free4pc.org/)
- [ask4pc](https://ask4pc.net/)
- [up4pc](https://up4pc.com/)
- [dr-farfar](https://www.dr-farfar.com/)
- [mutaz](https://www.mutaz.net/)
- [filecr](https://filecr.com)



--------------------------------------------------------

---------------------------------------------------------


### Others

#### Mobile apps monetization
- [start](https://www.start.io/)











<p align="right">(<a href="#top">back to top</a>)</p>
