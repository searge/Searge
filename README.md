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
![Code Time](http://img.shields.io/badge/Code%20Time-3%2C941%20hrs%208%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                2187 commits        ███████░░░░░░░░░░░░░░░░░░   26.44 % 
🌆 Daytime                3532 commits        ███████████░░░░░░░░░░░░░░   42.70 % 
🌃 Evening                2278 commits        ███████░░░░░░░░░░░░░░░░░░   27.54 % 
🌙 Night                  275 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.32 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       11 hrs 36 mins      █████████████░░░░░░░░░░░░   52.45 % 
YAML                     7 hrs 4 mins        ████████░░░░░░░░░░░░░░░░░   31.95 % 
Markdown                 1 hr 44 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   07.84 % 
Other                    40 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.08 % 
Bash                     39 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.01 % 

🔥 Editors: 
Zsh                      11 hrs 36 mins      █████████████░░░░░░░░░░░░   52.45 % 
VS Code                  10 hrs 13 mins      ████████████░░░░░░░░░░░░░   46.23 % 
Sublime Text             17 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.30 % 
Obsidian                 0 secs              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.02 % 

💻 Operating System: 
Linux                    22 hrs 7 mins       █████████████████████████   100.00 % 
```


 Last Updated on 21/12/2025 00:09:07 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
