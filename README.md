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
🌞 Morning                1997 commits        ███████░░░░░░░░░░░░░░░░░░   26.35 % 
🌆 Daytime                3234 commits        ███████████░░░░░░░░░░░░░░   42.67 % 
🌃 Evening                2084 commits        ███████░░░░░░░░░░░░░░░░░░   27.50 % 
🌙 Night                  264 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.48 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       9 hrs 40 mins       ██████████████░░░░░░░░░░░   54.16 % 
Markdown                 4 hrs 31 mins       ██████░░░░░░░░░░░░░░░░░░░   25.34 % 
YAML                     2 hrs 20 mins       ███░░░░░░░░░░░░░░░░░░░░░░   13.07 % 
TOML                     16 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.55 % 
Go                       16 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.53 % 

🔥 Editors: 
Zsh                      9 hrs 40 mins       ██████████████░░░░░░░░░░░   54.16 % 
VS Code                  7 hrs 6 mins        ██████████░░░░░░░░░░░░░░░   39.75 % 
Obsidian                 55 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   05.15 % 
Vim                      10 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   00.94 % 

💻 Operating System: 
Linux                    17 hrs 52 mins      █████████████████████████   100.00 % 
```


 Last Updated on 17/08/2025 00:09:08 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
