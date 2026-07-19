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
🌞 Morning                3175 commits        ███████░░░░░░░░░░░░░░░░░░   26.21 % 
🌆 Daytime                5571 commits        ███████████░░░░░░░░░░░░░░   45.99 % 
🌃 Evening                3060 commits        ██████░░░░░░░░░░░░░░░░░░░   25.26 % 
🌙 Night                  308 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   02.54 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 15 hrs 20 mins      ████████████░░░░░░░░░░░░░   47.70 % 
YAML                     7 hrs 27 mins       ██████░░░░░░░░░░░░░░░░░░░   23.21 % 
Org                      2 hrs 34 mins       ██░░░░░░░░░░░░░░░░░░░░░░░   08.00 % 
Bash                     1 hr 29 mins        █░░░░░░░░░░░░░░░░░░░░░░░░   04.64 % 
Python                   1 hr 7 mins         █░░░░░░░░░░░░░░░░░░░░░░░░   03.51 % 

🔥 Editors: 
Claude Code              15 hrs 8 mins       ████████████░░░░░░░░░░░░░   47.10 % 
VS Code                  8 hrs 32 mins       ███████░░░░░░░░░░░░░░░░░░   26.55 % 
Zed                      5 hrs 38 mins       ████░░░░░░░░░░░░░░░░░░░░░   17.55 % 
Emacs                    1 hr 17 mins        █░░░░░░░░░░░░░░░░░░░░░░░░   04.00 % 
Obsidian                 40 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.09 % 

💻 Operating System: 
Linux                    32 hrs 9 mins       █████████████████████████   100.00 % 
```


 Last Updated on 19/07/2026 01:33:46 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
