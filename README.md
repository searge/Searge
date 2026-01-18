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
🌞 Morning                2212 commits        ███████░░░░░░░░░░░░░░░░░░   26.38 % 
🌆 Daytime                3590 commits        ███████████░░░░░░░░░░░░░░   42.81 % 
🌃 Evening                2309 commits        ███████░░░░░░░░░░░░░░░░░░   27.54 % 
🌙 Night                  274 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.27 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       8 hrs 33 mins       ██████████░░░░░░░░░░░░░░░   40.50 % 
Markdown                 6 hrs 3 mins        ███████░░░░░░░░░░░░░░░░░░   28.63 % 
YAML                     2 hrs 57 mins       ████░░░░░░░░░░░░░░░░░░░░░   14.03 % 
JSON                     1 hr 3 mins         █░░░░░░░░░░░░░░░░░░░░░░░░   04.99 % 
Go                       56 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.49 % 

🔥 Editors: 
VS Code                  12 hrs 34 mins      ███████████████░░░░░░░░░░   59.50 % 
Zsh                      8 hrs 33 mins       ██████████░░░░░░░░░░░░░░░   40.50 % 
Vim                      0 secs              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.00 % 

💻 Operating System: 
Linux                    21 hrs 8 mins       █████████████████████████   100.00 % 
```


 Last Updated on 18/01/2026 00:09:38 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
