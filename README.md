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
🌞 Morning                2765 commits        ██████░░░░░░░░░░░░░░░░░░░   25.69 % 
🌆 Daytime                4876 commits        ███████████░░░░░░░░░░░░░░   45.31 % 
🌃 Evening                2818 commits        ███████░░░░░░░░░░░░░░░░░░   26.19 % 
🌙 Night                  302 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   02.81 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Other                    3 hrs 46 mins       ██████░░░░░░░░░░░░░░░░░░░   24.63 % 
Python                   2 hrs 6 mins        ███░░░░░░░░░░░░░░░░░░░░░░   13.71 % 
YAML                     1 hr 33 mins        ███░░░░░░░░░░░░░░░░░░░░░░   10.21 % 
sh                       1 hr 33 mins        ███░░░░░░░░░░░░░░░░░░░░░░   10.19 % 
Terraform                1 hr 33 mins        ███░░░░░░░░░░░░░░░░░░░░░░   10.16 % 

🔥 Editors: 
VS Code                  6 hrs 33 mins       ███████████░░░░░░░░░░░░░░   42.77 % 
Zsh                      5 hrs 36 mins       █████████░░░░░░░░░░░░░░░░   36.54 % 
Emacs                    2 hrs 23 mins       ████░░░░░░░░░░░░░░░░░░░░░   15.60 % 
Zed                      43 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.72 % 
Vim                      2 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.32 % 

💻 Operating System: 
Linux                    15 hrs 19 mins      █████████████████████████   100.00 % 
```


 Last Updated on 05/04/2026 00:14:41 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
