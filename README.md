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
🌞 Morning                3249 commits        ███████░░░░░░░░░░░░░░░░░░   26.31 % 
🌆 Daytime                5615 commits        ███████████░░░░░░░░░░░░░░   45.47 % 
🌃 Evening                3182 commits        ██████░░░░░░░░░░░░░░░░░░░   25.77 % 
🌙 Night                  302 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   02.45 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Org                      19 hrs 13 mins      ███████████░░░░░░░░░░░░░░   42.27 % 
YAML                     8 hrs 19 mins       █████░░░░░░░░░░░░░░░░░░░░   18.30 % 
Other                    7 hrs 1 min         ████░░░░░░░░░░░░░░░░░░░░░   15.44 % 
Markdown                 5 hrs 37 mins       ███░░░░░░░░░░░░░░░░░░░░░░   12.37 % 
Bash                     1 hr 11 mins        █░░░░░░░░░░░░░░░░░░░░░░░░   02.62 % 

🔥 Editors: 
Zed                      25 hrs 2 mins       ██████████████░░░░░░░░░░░   55.02 % 
Emacs                    12 hrs 4 mins       ███████░░░░░░░░░░░░░░░░░░   26.56 % 
Claude Code              5 hrs 46 mins       ███░░░░░░░░░░░░░░░░░░░░░░   12.71 % 
Zsh                      2 hrs 5 mins        █░░░░░░░░░░░░░░░░░░░░░░░░   04.59 % 
Vim                      30 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.12 % 

💻 Operating System: 
Linux                    45 hrs 29 mins      █████████████████████████   100.00 % 
```


 Last Updated on 24/05/2026 00:28:26 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
