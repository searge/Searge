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
![Code Time](http://img.shields.io/badge/Code%20Time-3%2C703%20hrs%2029%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                2012 commits        ███████░░░░░░░░░░░░░░░░░░   26.43 % 
🌆 Daytime                3248 commits        ███████████░░░░░░░░░░░░░░   42.66 % 
🌃 Evening                2090 commits        ███████░░░░░░░░░░░░░░░░░░   27.45 % 
🌙 Night                  264 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.47 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       2 hrs 28 mins       █████████░░░░░░░░░░░░░░░░   37.64 % 
YAML                     2 hrs 9 mins        ████████░░░░░░░░░░░░░░░░░   32.71 % 
Bash                     1 hr                ████░░░░░░░░░░░░░░░░░░░░░   15.19 % 
Markdown                 23 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   05.95 % 
Go                       15 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.88 % 

🔥 Editors: 
VS Code                  3 hrs 56 mins       ███████████████░░░░░░░░░░   59.95 % 
Zsh                      2 hrs 28 mins       █████████░░░░░░░░░░░░░░░░   37.64 % 
Obsidian                 9 mins              █░░░░░░░░░░░░░░░░░░░░░░░░   02.41 % 
Vim                      0 secs              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.00 % 

💻 Operating System: 
Linux                    6 hrs 35 mins       █████████████████████████   100.00 % 
```


 Last Updated on 07/09/2025 00:07:44 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
