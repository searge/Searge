# Hi, I'm Searge <img src="images/vulcan.webp" style="display: inline-block; margin: 0; height: 2rem" alt="Vulcan salute" />

## DevOps Engineer at [Smile Ukraine](https://smile-ukraine.com/en)

[![Stand With Ukraine](https://raw.githubusercontent.com/vshymanskyy/StandWithUkraine/main/badges/StandWithUkraine.svg)](https://stand-with-ukraine.pp.ua)
<a rel="me" href="https://hachyderm.io/@Searge">![@Searge@hachyderm.io](https://img.shields.io/badge/-@Searge-%232B90D9?logo=mastodon&logoColor=white)</a>

```python
# %%
"""Creating a class for keeping track of knowledge."""
import json
from dataclasses import asdict, make_dataclass

from rich import print

person = make_dataclass(
    "Person",
    [
        ("nick", str),
        ("name", str),
        ("pipelines", list[str]),
        ("web_services", list[str]),
        ("languages", list[str]),
        ("databases", list[str]),
        ("misc", list[str]),
        ("ongoing", list[str]),
    ],
    namespace={"to_json": lambda self: json.dumps(asdict(self), indent=4)},
)

# %%
# @title Initializing classes and creating lists
if __name__ == "__main__":
    pipelines    = ['GitLab Ci', 'GitHub Actions', 'AWS CodePipeline', 'Jenkins']
    web_services = ['nginx', 'apache', 'varnish', 'fastly', 'elastic', 'solr']
    languages    = ['YAML', 'Bash', 'Python', 'JS', 'Web']
    databases    = ['SQLite', 'PostgreSQL', 'Percona', 'DynamoDB', 'Redis']
    misc         = ['Ansible', 'Linux', 'LXC', 'Docker', 'Terraform', 'AWS']
    ongoing      = ['LPIC', 'Full Stack Web', 'AWS']

    me = person('@Searge', 'Sergij Boremchuk',
                pipelines, web_services, languages, databases, misc, ongoing)

    print(me.to_json())

# %%

```

<sub>Thanks @rednafi for idea of script :wink:</sub>

### Statistics

[Skyline for 2021](https://skyline.github.com/Searge/2021)

![Visitors](https://komarev.com/ghpvc/?username=searge&label=Profile%20views&color=0e75b6&style=flat) 
<!--START_SECTION:waka-->
![Code Time](http://img.shields.io/badge/Code%20Time-4%2C221%20hrs%2058%20mins-blue?style=flat)

**I'm an Early 🐤** 

```text
🌞 Morning                2615 commits        ██████░░░░░░░░░░░░░░░░░░░   25.82 % 
🌆 Daytime                4555 commits        ███████████░░░░░░░░░░░░░░   44.98 % 
🌃 Evening                2662 commits        ███████░░░░░░░░░░░░░░░░░░   26.29 % 
🌙 Night                  294 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   02.90 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       3 hrs 53 mins       ███████░░░░░░░░░░░░░░░░░░   27.87 % 
Markdown                 3 hrs 26 mins       ██████░░░░░░░░░░░░░░░░░░░   24.70 % 
Org                      2 hrs 3 mins        ████░░░░░░░░░░░░░░░░░░░░░   14.68 % 
PowerShell               51 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   06.14 % 
JSON                     46 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   05.53 % 

🔥 Editors: 
VS Code                  8 hrs 37 mins       ███████████████░░░░░░░░░░   61.80 % 
Zsh                      3 hrs 53 mins       ███████░░░░░░░░░░░░░░░░░░   27.87 % 
Emacs                    1 hr 16 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   09.10 % 
Vim                      10 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.24 % 

💻 Operating System: 
Linux                    12 hrs 53 mins      ███████████████████████░░   92.34 % 
Windows                  1 hr 4 mins         ██░░░░░░░░░░░░░░░░░░░░░░░   07.66 % 
```


 Last Updated on 15/03/2026 00:13:10 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
