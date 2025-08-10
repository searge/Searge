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
![Code Time](http://img.shields.io/badge/Code%20Time-3%2C652%20hrs%2026%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1974 commits        ███████░░░░░░░░░░░░░░░░░░   26.18 % 
🌆 Daytime                3221 commits        ███████████░░░░░░░░░░░░░░   42.71 % 
🌃 Evening                2082 commits        ███████░░░░░░░░░░░░░░░░░░   27.61 % 
🌙 Night                  264 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.50 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       12 hrs 52 mins      ████████████░░░░░░░░░░░░░   49.06 % 
YAML                     4 hrs 22 mins       ████░░░░░░░░░░░░░░░░░░░░░   16.65 % 
Python                   2 hrs 39 mins       ███░░░░░░░░░░░░░░░░░░░░░░   10.12 % 
Markdown                 1 hr 57 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   07.48 % 
Docker                   1 hr 32 mins        █░░░░░░░░░░░░░░░░░░░░░░░░   05.85 % 

🔥 Editors: 
Zsh                      12 hrs 52 mins      ████████████░░░░░░░░░░░░░   49.06 % 
VS Code                  12 hrs 50 mins      ████████████░░░░░░░░░░░░░   48.91 % 
Obsidian                 31 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.98 % 
Vim                      0 secs              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.05 % 

💻 Operating System: 
Linux                    26 hrs 14 mins      █████████████████████████   100.00 % 
```


 Last Updated on 10/08/2025 00:08:06 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
