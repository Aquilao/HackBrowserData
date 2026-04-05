<div align="center">
<img src="LOGO.png" alt="hack-browser-data logo" width="440px" />
</div> 

# HackBrowserData

[![Lint](https://github.com/moonD4rk/HackBrowserData/actions/workflows/lint.yml/badge.svg)](https://github.com/moonD4rk/HackBrowserData/actions/workflows/lint.yml) [![Build](https://github.com/moonD4rk/HackBrowserData/actions/workflows/build.yml/badge.svg)](https://github.com/moonD4rk/HackBrowserData/actions/workflows/build.yml) [![Release](https://github.com/moonD4rk/HackBrowserData/actions/workflows/release.yml/badge.svg)](https://github.com/moonD4rk/HackBrowserData/actions/workflows/release.yml) [![Tests](https://github.com/moonD4rk/HackBrowserData/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/moonD4rk/HackBrowserData/actions/workflows/test.yml) [![codecov](https://codecov.io/gh/moonD4rk/HackBrowserData/branch/main/graph/badge.svg?token=KWJCN38657)](https://codecov.io/gh/moonD4rk/HackBrowserData)

`HackBrowserData` is a command-line tool for decrypting and exporting browser data (passwords, history, cookies, bookmarks, credit cards, download history, localStorage and extensions) from the browser. It supports the most popular browsers on the market and runs on Windows, macOS and Linux.

> Disclaimer: This tool is only intended for security research. Users are responsible for all legal and related liabilities resulting from the use of this tool. The original author does not assume any legal responsibility.

## Recent Updates

### Firefox 144+ Support

HackBrowserData now supports decryption of saved passwords in Firefox 144 and later versions.

Starting from Firefox 144, Mozilla migrated password encryption from 3DES to AES-256-CBC to enhance security. HackBrowserData has been updated accordingly and remains fully compatible with the latest Firefox encryption scheme.

For more details:
- [Firefox 144.0 Release Notes](https://www.firefox.com/en-US/firefox/144.0/releasenotes/)
- [How Firefox securely saves passwords](https://support.mozilla.org/en-US/kb/how-firefox-securely-saves-passwords)


## Supported Browser

### Windows
| Browser            | Password | Cookie | Bookmark | History |
|:-------------------|:--------:|:------:|:--------:|:-------:|
| Google Chrome      |    ✅     |   ✅    |    ✅     |    ✅    |
| Google Chrome Beta |    ✅     |   ✅    |    ✅     |    ✅    |
| Chromium           |    ✅     |   ✅    |    ✅     |    ✅    |
| Microsoft Edge     |    ✅     |   ✅    |    ✅     |    ✅    |
| 360 Speed          |    ✅     |   ✅    |    ✅     |    ✅    |
| QQ                 |    ✅     |   ✅    |    ✅     |    ✅    |
| Brave              |    ✅     |   ✅    |    ✅     |    ✅    |
| Opera              |    ✅     |   ✅    |    ✅     |    ✅    |
| OperaGX            |    ✅     |   ✅    |    ✅     |    ✅    |
| Vivaldi            |    ✅     |   ✅    |    ✅     |    ✅    |
| Yandex             |    ✅     |   ✅    |    ✅     |    ✅    |
| CocCoc             |    ✅     |   ✅    |    ✅     |    ✅    |
| Firefox            |    ✅     |   ✅    |    ✅     |    ✅    |
| Firefox Beta       |    ✅     |   ✅    |    ✅     |    ✅    |
| Firefox Dev        |    ✅     |   ✅    |    ✅     |    ✅    |
| Firefox ESR        |    ✅     |   ✅    |    ✅     |    ✅    |
| Firefox Nightly    |    ✅     |   ✅    |    ✅     |    ✅    |
| Internet Explorer  |    ❌     |   ❌    |    ❌     |    ❌    |


### MacOS

Based on Apple's security policy, some browsers **require a current user password** to decrypt.

| Browser            | Password | Cookie | Bookmark | History |
|:-------------------|:--------:|:------:|:--------:|:-------:|
| Google Chrome      |    ✅     |   ✅    |    ✅     |    ✅    |
| Google Chrome Beta |    ✅     |   ✅    |    ✅     |    ✅    |
| Chromium           |    ✅     |   ✅    |    ✅     |    ✅    |
| Microsoft Edge     |    ✅     |   ✅    |    ✅     |    ✅    |
| Brave              |    ✅     |   ✅    |    ✅     |    ✅    |
| Opera              |    ✅     |   ✅    |    ✅     |    ✅    |
| OperaGX            |    ✅     |   ✅    |    ✅     |    ✅    |
| Vivaldi            |    ✅     |   ✅    |    ✅     |    ✅    |
| CocCoc             |    ✅     |   ✅    |    ✅     |    ✅    |
| Yandex             |    ✅     |   ✅    |    ✅     |    ✅    |
| Arc                |    ✅     |   ✅    |    ✅     |    ✅    |
| Firefox            |    ✅     |   ✅    |    ✅     |    ✅    |
| Firefox Beta       |    ✅     |   ✅    |    ✅     |    ✅    |
| Firefox Dev        |    ✅     |   ✅    |    ✅     |    ✅    |
| Firefox ESR        |    ✅     |   ✅    |    ✅     |    ✅    |
| Firefox Nightly    |    ✅     |   ✅    |    ✅     |    ✅    |
| Safari             |    ❌     |   ❌    |    ❌     |    ❌    |

### Linux

| Browser            | Password | Cookie | Bookmark | History |
|:-------------------|:--------:|:------:|:--------:|:-------:|
| Google Chrome      |    ✅     |   ✅    |    ✅     |    ✅    |
| Google Chrome Beta |    ✅     |   ✅    |    ✅     |    ✅    |
| Chromium           |    ✅     |   ✅    |    ✅     |    ✅    |
| Microsoft Edge Dev |    ✅     |   ✅    |    ✅     |    ✅    |
| Brave              |    ✅     |   ✅    |    ✅     |    ✅    |
| Opera              |    ✅     |   ✅    |    ✅     |    ✅    |
| Vivaldi            |    ✅     |   ✅    |    ✅     |    ✅    |
| Firefox            |    ✅     |   ✅    |    ✅     |    ✅    |
| Firefox Beta       |    ✅     |   ✅    |    ✅     |    ✅    |
| Firefox Dev        |    ✅     |   ✅    |    ✅     |    ✅    |
| Firefox ESR        |    ✅     |   ✅    |    ✅     |    ✅    |
| Firefox Nightly    |    ✅     |   ✅    |    ✅     |    ✅    |


## Getting started

### Install

Installation of `HackBrowserData` is dead-simple, just download [the release for your system](https://github.com/moonD4rk/HackBrowserData/releases) and run the binary.

> In some situations, this security tool will be treated as a virus by Windows Defender or other antivirus software and can not be executed. The code is all open source, you can modify and compile by yourself.

### Building from source

only support `go 1.20+` with go generics.

```bash
$ git clone https://github.com/moonD4rk/HackBrowserData

$ cd HackBrowserData/cmd/hack-browser-data

$ go build
```

### Cross compile

Here's an example of use `macOS` building for `Windows` and `Linux`

#### For Windows

```shell
GOOS=windows GOARCH=amd64 go build
```

#### For Linux

````shell
GOOS=linux GOARCH=amd64 go build
````

### Run

You can double-click to run, or use command line.

```powershell
PS C:\Users\moond4rk\Desktop> .\hack-browser-data.exe -h
NAME:
   hack-browser-data - Export passwords|bookmarks|cookies|history|credit cards|download history|localStorage|extensions from browser
USAGE:
   [hack-browser-data -b chrome -f json --dir results --zip]
   Export all browsing data (passwords/cookies/history/bookmarks) from browser
   Github Link: https://github.com/moonD4rk/HackBrowserData
VERSION:
   0.4.6

GLOBAL OPTIONS:
   --verbose, --vv                   verbose (default: false)
   --compress, --zip                 compress result to zip (default: false)
   --browser value, -b value         available browsers: all|360|brave|chrome|chrome-beta|chromium|coccoc|dc|edge|firefox|opera|opera-gx|qq|sogou|vivaldi|yandex (default: "all")
   --results-dir value, --dir value  export dir (default: "results")
   --format value, -f value          output format: csv|json (default: "csv")
   --profile-path value, -p value    custom profile dir path, get with chrome://version
   --full-export, --full             is export full browsing data (default: true)
   --help, -h                        show help
   --version, -v                     print the version

```

For example, the following is an automatic scan of the browser on the current computer, outputting the decryption results in `JSON` format and compressing as `zip`.

```powershell
PS C:\Users\moond4rk\Desktop> .\hack-browser-data.exe -b all -f json --dir results --zip

PS C:\Users\moond4rk\Desktop> ls -l .\results\
    Directory: C:\Users\moond4rk\Desktop\results
    
Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----         7/15/2024  10:55 PM          44982 results.zip
```


### Run with custom browser profile folder

If you want to export data from a custom browser profile folder, you can use the `-p` parameter to specify the path of the browser profile folder. PS: use double quotes to wrap the path.
```powershell
PS C:\Users\moond4rk\Desktop> .\hack-browser-data.exe -b chrome -p "C:\Users\User\AppData\Local\Microsoft\Edge\User Data\Default"

[NOTICE] [browsingdata.go:59,Output] output to file results/chrome_creditcard.csv success  
[NOTICE] [browsingdata.go:59,Output] output to file results/chrome_bookmark.csv success  
[NOTICE] [browsingdata.go:59,Output] output to file results/chrome_cookie.csv success  
[NOTICE] [browsingdata.go:59,Output] output to file results/chrome_history.csv success  
[NOTICE] [browsingdata.go:59,Output] output to file results/chrome_download.csv success  
[NOTICE] [browsingdata.go:59,Output] output to file results/chrome_password.csv success  
```

## Contributing

We welcome and appreciate any contributions made by the community (GitHub issues/pull requests, email feedback, etc.).

Please see the [Contribution Guide](CONTRIBUTING.md) before contributing.


## Contributors

<!-- readme: collaborators,contributors -start -->
<table>
	<tbody>
		<tr>
            <td align="center">
                <a href="https://github.com/moonD4rk">
                    <img src="https://avatars.githubusercontent.com/u/24284231?v=4" width="100;" alt="moonD4rk"/>
                    <br />
                    <sub><b>Roger</b></sub>
                </a>
            </td>
            <td align="center">
                <a href="https://github.com/Aquilao">
                    <img src="https://avatars.githubusercontent.com/u/25531497?v=4" width="100;" alt="Aquilao"/>
                    <br />
                    <sub><b>Aquilao Official</b></sub>
                </a>
            </td>
            <td align="center">
                <a href="https://github.com/uinfziuna8n">
                    <img src="https://avatars.githubusercontent.com/u/43719451?v=4" width="100;" alt="uinfziuna8n"/>
                    <br />
                    <sub><b>uinfziuna8n</b></sub>
                </a>
            </td>
            <td align="center">
                <a href="https://github.com/VMpc">
                    <img src="https://avatars.githubusercontent.com/u/50967051?v=4" width="100;" alt="VMpc"/>
                    <br />
                    <sub><b>Cyrus</b></sub>
                </a>
            </td>
            <td align="center">
                <a href="https://github.com/stevenlele">
                    <img src="https://avatars.githubusercontent.com/u/15964380?v=4" width="100;" alt="stevenlele"/>
                    <br />
                    <sub><b>stevenlele</b></sub>
                </a>
            </td>
            <td align="center">
                <a href="https://github.com/camandel">
                    <img src="https://avatars.githubusercontent.com/u/5462153?v=4" width="100;" alt="camandel"/>
                    <br />
                    <sub><b>Carlo Mandelli</b></sub>
                </a>
            </td>
		</tr>
		<tr>
            <td align="center">
                <a href="https://github.com/slimwang">
                    <img src="https://avatars.githubusercontent.com/u/14370794?v=4" width="100;" alt="slimwang"/>
                    <br />
                    <sub><b>slimwang</b></sub>
                </a>
            </td>
            <td align="center">
                <a href="https://github.com/ac0d3r">
                    <img src="https://avatars.githubusercontent.com/u/26270009?v=4" width="100;" alt="ac0d3r"/>
                    <br />
                    <sub><b>zznQ</b></sub>
                </a>
            </td>
            <td align="center">
                <a href="https://github.com/slark-yuxj">
                    <img src="https://avatars.githubusercontent.com/u/95608083?v=4" width="100;" alt="slark-yuxj"/>
                    <br />
                    <sub><b>YuXJ</b></sub>
                </a>
            </td>
            <td align="center">
                <a href="https://github.com/mirefly">
                    <img src="https://avatars.githubusercontent.com/u/4984681?v=4" width="100;" alt="mirefly"/>
                    <br />
                    <sub><b>mirefly</b></sub>
                </a>
            </td>
            <td align="center">
                <a href="https://github.com/lc6464">
                    <img src="https://avatars.githubusercontent.com/u/64722907?v=4" width="100;" alt="lc6464"/>
                    <br />
                    <sub><b>LC</b></sub>
                </a>
            </td>
            <td align="center">
                <a href="https://github.com/zhe6652">
                    <img src="https://avatars.githubusercontent.com/u/24725680?v=4" width="100;" alt="zhe6652"/>
                    <br />
                    <sub><b>zhe6652</b></sub>
                </a>
            </td>
		</tr>
		<tr>
            <td align="center">
                <a href="https://github.com/testwill">
                    <img src="https://avatars.githubusercontent.com/u/8717479?v=4" width="100;" alt="testwill"/>
                    <br />
                    <sub><b>guoguangwu</b></sub>
                </a>
            </td>
            <td align="center">
                <a href="https://github.com/chensonghi">
                    <img src="https://avatars.githubusercontent.com/u/113400678?v=4" width="100;" alt="chensonghi"/>
                    <br />
                    <sub><b>chleynx</b></sub>
                </a>
            </td>
            <td align="center">
                <a href="https://github.com/BeichenDream">
                    <img src="https://avatars.githubusercontent.com/u/43266206?v=4" width="100;" alt="BeichenDream"/>
                    <br />
                    <sub><b>beichen</b></sub>
                </a>
            </td>
            <td align="center">
                <a href="https://github.com/SantiiRepair">
                    <img src="https://avatars.githubusercontent.com/u/94815926?v=4" width="100;" alt="SantiiRepair"/>
                    <br />
                    <sub><b>Santiago Ramirez</b></sub>
                </a>
            </td>
            <td align="center">
                <a href="https://github.com/dexhek">
                    <img src="https://avatars.githubusercontent.com/u/39654918?v=4" width="100;" alt="dexhek"/>
                    <br />
                    <sub><b>Ciprian Conache</b></sub>
                </a>
            </td>
            <td align="center">
                <a href="https://github.com/a-urth">
                    <img src="https://avatars.githubusercontent.com/u/3456803?v=4" width="100;" alt="a-urth"/>
                    <br />
                    <sub><b>a-urth</b></sub>
                </a>
            </td>
		</tr>
		<tr>
            <td align="center">
                <a href="https://github.com/Amir-78">
                    <img src="https://avatars.githubusercontent.com/u/68391526?v=4" width="100;" alt="Amir-78"/>
                    <br />
                    <sub><b>Amir.</b></sub>
                </a>
            </td>
		</tr>
	<tbody>
</table>
<!-- readme: collaborators,contributors -end -->

## Stargazers over time
[![Star History Chart](https://api.star-history.com/svg?repos=moond4rk/hackbrowserdata&type=Date)](https://github.com/moond4rk/HackBrowserData)


## 404StarLink 2.0 - Galaxy
`HackBrowserData` is a part of 404Team [StarLink-Galaxy](https://github.com/knownsec/404StarLink2.0-Galaxy), if you have any questions about `HackBrowserData` or want to find a partner to communicate with，please refer to the [Starlink group](https://github.com/knownsec/404StarLink2.0-Galaxy#community).
<a href="https://github.com/knownsec/404StarLink2.0-Galaxy" target="_blank"><img src="https://raw.githubusercontent.com/knownsec/404StarLink-Project/master/logo.png" align="middle"/></a>

##  JetBrains OS licenses
``HackBrowserData`` had been being developed with `GoLand` IDE under the **free JetBrains Open Source license(s)** granted by JetBrains s.r.o., hence I would like to express my thanks here.

<a href="https://www.jetbrains.com/?from=HackBrowserData" target="_blank"><img src="https://raw.githubusercontent.com/moonD4rk/staticfiles/master/picture/jetbrains-variant-4.png" width="256" align="middle"/></a>

