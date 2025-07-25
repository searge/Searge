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
**I'm an Early 🐤** 

```text
🌞 Morning                1954 commits        ███████░░░░░░░░░░░░░░░░░░   26.19 % 
🌆 Daytime                3185 commits        ███████████░░░░░░░░░░░░░░   42.69 % 
🌃 Evening                2057 commits        ███████░░░░░░░░░░░░░░░░░░   27.57 % 
🌙 Night                  264 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.54 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       11 hrs 43 mins      ███████████████░░░░░░░░░░   59.25 % 
YAML                     5 hrs 44 mins       ███████░░░░░░░░░░░░░░░░░░   29.02 % 
Go                       1 hr 9 mins         █░░░░░░░░░░░░░░░░░░░░░░░░   05.88 % 
Markdown                 36 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.11 % 
Python                   11 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   00.94 % 

🔥 Editors: 
Zsh                      11 hrs 43 mins      ███████████████░░░░░░░░░░   59.25 % 
VS Code                  7 hrs 58 mins       ██████████░░░░░░░░░░░░░░░   40.28 % 
Obsidian                 5 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.47 % 

💻 Operating System: 
Linux                    19 hrs 47 mins      █████████████████████████   100.00 % 
```


 Last Updated on 20/07/2025 00:08:20 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
