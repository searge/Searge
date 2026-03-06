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
🌞 Morning                2506 commits        ██████░░░░░░░░░░░░░░░░░░░   25.81 % 
🌆 Daytime                4387 commits        ███████████░░░░░░░░░░░░░░   45.18 % 
🌃 Evening                2531 commits        ███████░░░░░░░░░░░░░░░░░░   26.06 % 
🌙 Night                  287 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   02.96 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       6 hrs 31 mins       ████████░░░░░░░░░░░░░░░░░   32.05 % 
Org                      6 hrs 30 mins       ████████░░░░░░░░░░░░░░░░░   31.95 % 
Markdown                 2 hrs 34 mins       ███░░░░░░░░░░░░░░░░░░░░░░   12.66 % 
YAML                     2 hrs               ██░░░░░░░░░░░░░░░░░░░░░░░   09.87 % 
HCL                      33 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.74 % 

🔥 Editors: 
VS Code                  13 hrs 25 mins      ████████████████░░░░░░░░░   65.87 % 
Zsh                      6 hrs 31 mins       ████████░░░░░░░░░░░░░░░░░   32.05 % 
Emacs                    25 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.07 % 
Vim                      0 secs              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.02 % 

💻 Operating System: 
Linux                    20 hrs 22 mins      █████████████████████████   100.00 % 
```


 Last Updated on 06/03/2026 08:41:40 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
