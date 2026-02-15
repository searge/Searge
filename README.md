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
🌞 Morning                2283 commits        ███████░░░░░░░░░░░░░░░░░░   26.16 % 
🌆 Daytime                3815 commits        ███████████░░░░░░░░░░░░░░   43.71 % 
🌃 Evening                2358 commits        ███████░░░░░░░░░░░░░░░░░░   27.02 % 
🌙 Night                  271 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.11 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       14 hrs 36 mins      ██████████░░░░░░░░░░░░░░░   40.60 % 
YAML                     10 hrs 10 mins      ███████░░░░░░░░░░░░░░░░░░   28.29 % 
Markdown                 6 hrs 37 mins       █████░░░░░░░░░░░░░░░░░░░░   18.44 % 
TOML                     1 hr 3 mins         █░░░░░░░░░░░░░░░░░░░░░░░░   02.96 % 
Python                   46 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.15 % 

🔥 Editors: 
VS Code                  17 hrs 52 mins      ████████████░░░░░░░░░░░░░   49.70 % 
Zsh                      14 hrs 36 mins      ██████████░░░░░░░░░░░░░░░   40.60 % 
Zed                      1 hr 55 mins        █░░░░░░░░░░░░░░░░░░░░░░░░   05.37 % 
Obsidian                 1 hr 28 mins        █░░░░░░░░░░░░░░░░░░░░░░░░   04.08 % 
Vim                      5 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.25 % 

💻 Operating System: 
Linux                    35 hrs 58 mins      █████████████████████████   100.00 % 
```


 Last Updated on 15/02/2026 00:11:49 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
