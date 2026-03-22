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
🌞 Morning                2625 commits        ██████░░░░░░░░░░░░░░░░░░░   25.81 % 
🌆 Daytime                4562 commits        ███████████░░░░░░░░░░░░░░   44.86 % 
🌃 Evening                2687 commits        ███████░░░░░░░░░░░░░░░░░░   26.42 % 
🌙 Night                  296 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   02.91 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       3 hrs 56 mins       ███████░░░░░░░░░░░░░░░░░░   26.28 % 
Markdown                 3 hrs 23 mins       ██████░░░░░░░░░░░░░░░░░░░   22.55 % 
YAML                     1 hr 31 mins        ███░░░░░░░░░░░░░░░░░░░░░░   10.13 % 
Org                      1 hr 13 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   08.15 % 
Terraform                1 hr 1 min          ██░░░░░░░░░░░░░░░░░░░░░░░   06.82 % 

🔥 Editors: 
VS Code                  9 hrs 50 mins       ████████████████░░░░░░░░░   65.45 % 
Zsh                      3 hrs 56 mins       ███████░░░░░░░░░░░░░░░░░░   26.28 % 
Cursor                   33 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.72 % 
Emacs                    13 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.45 % 
Zed                      8 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.91 % 

💻 Operating System: 
Linux                    15 hrs 1 min        █████████████████████████   100.00 % 
```


 Last Updated on 22/03/2026 00:12:40 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
