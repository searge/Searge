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
🌞 Morning                3023 commits        ███████░░░░░░░░░░░░░░░░░░   26.40 % 
🌆 Daytime                5203 commits        ███████████░░░░░░░░░░░░░░   45.45 % 
🌃 Evening                2921 commits        ██████░░░░░░░░░░░░░░░░░░░   25.51 % 
🌙 Night                  302 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   02.64 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
YAML                     7 hrs 22 mins       ████████░░░░░░░░░░░░░░░░░   33.49 % 
Other                    5 hrs 38 mins       ██████░░░░░░░░░░░░░░░░░░░   25.68 % 
Markdown                 3 hrs 18 mins       ████░░░░░░░░░░░░░░░░░░░░░   15.01 % 
sh                       3 hrs 7 mins        ████░░░░░░░░░░░░░░░░░░░░░   14.20 % 
Org                      1 hr 21 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   06.20 % 

🔥 Editors: 
VS Code                  14 hrs 35 mins      █████████████████░░░░░░░░   66.31 % 
Zsh                      5 hrs 19 mins       ██████░░░░░░░░░░░░░░░░░░░   24.20 % 
Emacs                    1 hr 33 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   07.09 % 
Zed                      15 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.21 % 
Unknown Editor           14 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.11 % 

💻 Operating System: 
Linux                    21 hrs 59 mins      █████████████████████████   100.00 % 
```


 Last Updated on 19/04/2026 00:17:04 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
