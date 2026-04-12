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
🌞 Morning                2799 commits        ██████░░░░░░░░░░░░░░░░░░░   25.63 % 
🌆 Daytime                4967 commits        ███████████░░░░░░░░░░░░░░   45.48 % 
🌃 Evening                2853 commits        ███████░░░░░░░░░░░░░░░░░░   26.12 % 
🌙 Night                  302 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   02.77 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Other                    15 hrs 23 mins      ████████████░░░░░░░░░░░░░   49.12 % 
sh                       3 hrs 56 mins       ███░░░░░░░░░░░░░░░░░░░░░░   12.56 % 
Markdown                 3 hrs 3 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   09.77 % 
Org                      2 hrs 56 mins       ██░░░░░░░░░░░░░░░░░░░░░░░   09.39 % 
YAML                     1 hr 45 mins        █░░░░░░░░░░░░░░░░░░░░░░░░   05.64 % 

🔥 Editors: 
VS Code                  16 hrs 37 mins      █████████████░░░░░░░░░░░░   53.03 % 
Zsh                      10 hrs 58 mins      █████████░░░░░░░░░░░░░░░░   35.00 % 
Emacs                    2 hrs 57 mins       ██░░░░░░░░░░░░░░░░░░░░░░░   09.46 % 
Zed                      40 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.16 % 
Obsidian                 6 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.35 % 

💻 Operating System: 
Linux                    31 hrs 20 mins      █████████████████████████   100.00 % 
```


 Last Updated on 12/04/2026 00:16:13 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
