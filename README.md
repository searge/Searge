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
![Code Time](http://img.shields.io/badge/Code%20Time-3%2C886%20hrs%2040%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                2111 commits        ███████░░░░░░░░░░░░░░░░░░   26.40 % 
🌆 Daytime                3420 commits        ███████████░░░░░░░░░░░░░░   42.77 % 
🌃 Evening                2197 commits        ███████░░░░░░░░░░░░░░░░░░   27.47 % 
🌙 Night                  269 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.36 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       8 hrs 26 mins       ██████████████████░░░░░░░   71.57 % 
Markdown                 1 hr 57 mins        ████░░░░░░░░░░░░░░░░░░░░░   16.66 % 
YAML                     1 hr 2 mins         ██░░░░░░░░░░░░░░░░░░░░░░░   08.83 % 
JSON                     18 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.66 % 
Git Config               1 min               ░░░░░░░░░░░░░░░░░░░░░░░░░   00.18 % 

🔥 Editors: 
Zsh                      8 hrs 26 mins       ██████████████████░░░░░░░   71.57 % 
VS Code                  3 hrs 19 mins       ███████░░░░░░░░░░░░░░░░░░   28.24 % 
Vim                      1 min               ░░░░░░░░░░░░░░░░░░░░░░░░░   00.20 % 

💻 Operating System: 
Linux                    11 hrs 47 mins      █████████████████████████   100.00 % 
```


 Last Updated on 30/11/2025 00:08:30 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
