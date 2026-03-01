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
![Code Time](http://img.shields.io/badge/Code%20Time-4%2C185%20hrs%2033%20mins-blue?style=flat)

**I'm an Early 🐤** 

```text
🌞 Morning                2479 commits        ██████░░░░░░░░░░░░░░░░░░░   25.83 % 
🌆 Daytime                4327 commits        ███████████░░░░░░░░░░░░░░   45.09 % 
🌃 Evening                2503 commits        ███████░░░░░░░░░░░░░░░░░░   26.08 % 
🌙 Night                  287 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   02.99 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       8 hrs 41 mins       ████████████░░░░░░░░░░░░░   46.42 % 
Markdown                 4 hrs 49 mins       ██████░░░░░░░░░░░░░░░░░░░   25.82 % 
YAML                     3 hrs 54 mins       █████░░░░░░░░░░░░░░░░░░░░   20.91 % 
TOML                     15 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.42 % 
Docker                   14 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.30 % 

🔥 Editors: 
VS Code                  9 hrs 36 mins       █████████████░░░░░░░░░░░░   51.39 % 
Zsh                      8 hrs 41 mins       ████████████░░░░░░░░░░░░░   46.42 % 
Cursor                   20 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.83 % 
Obsidian                 4 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.36 % 

💻 Operating System: 
Linux                    18 hrs 42 mins      █████████████████████████   100.00 % 
```


 Last Updated on 01/03/2026 00:10:55 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
