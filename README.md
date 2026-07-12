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
![Code Time](http://img.shields.io/badge/Code%20Time-4%2C692%20hrs%2010%20mins-blue?style=flat)

**I'm an Early 🐤** 

```text
🌞 Morning                3205 commits        ███████░░░░░░░░░░░░░░░░░░   26.34 % 
🌆 Daytime                5590 commits        ███████████░░░░░░░░░░░░░░   45.93 % 
🌃 Evening                3066 commits        ██████░░░░░░░░░░░░░░░░░░░   25.19 % 
🌙 Night                  309 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   02.54 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 7 hrs 5 mins        ██████████░░░░░░░░░░░░░░░   38.91 % 
YAML                     4 hrs 24 mins       ██████░░░░░░░░░░░░░░░░░░░   24.20 % 
Org                      2 hrs 14 mins       ███░░░░░░░░░░░░░░░░░░░░░░   12.30 % 
Other                    1 hr 43 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   09.48 % 
sh                       1 hr 6 mins         ██░░░░░░░░░░░░░░░░░░░░░░░   06.06 % 

🔥 Editors: 
Claude Code              11 hrs 7 mins       ███████████████░░░░░░░░░░   60.98 % 
Zed                      2 hrs 37 mins       ████░░░░░░░░░░░░░░░░░░░░░   14.38 % 
VS Code                  1 hr 45 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   09.67 % 
Zsh                      1 hr 6 mins         ██░░░░░░░░░░░░░░░░░░░░░░░   06.06 % 
Emacs                    50 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.61 % 

💻 Operating System: 
Linux                    18 hrs 14 mins      █████████████████████████   100.00 % 
```


 Last Updated on 12/07/2026 01:34:20 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
