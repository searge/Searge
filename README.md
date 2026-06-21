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
🌞 Morning                3318 commits        ███████░░░░░░░░░░░░░░░░░░   26.11 % 
🌆 Daytime                5801 commits        ███████████░░░░░░░░░░░░░░   45.64 % 
🌃 Evening                3282 commits        ██████░░░░░░░░░░░░░░░░░░░   25.82 % 
🌙 Night                  308 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   02.42 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 14 hrs 25 mins      ████████████░░░░░░░░░░░░░   47.10 % 
YAML                     3 hrs 45 mins       ███░░░░░░░░░░░░░░░░░░░░░░   12.25 % 
Org                      2 hrs 44 mins       ██░░░░░░░░░░░░░░░░░░░░░░░   08.95 % 
Python                   2 hrs 22 mins       ██░░░░░░░░░░░░░░░░░░░░░░░   07.75 % 
Other                    2 hrs 4 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   06.79 % 

🔥 Editors: 
Claude Code              18 hrs 9 mins       ███████████████░░░░░░░░░░   59.34 % 
Zed                      6 hrs 29 mins       █████░░░░░░░░░░░░░░░░░░░░   21.22 % 
VS Code                  2 hrs 59 mins       ██░░░░░░░░░░░░░░░░░░░░░░░   09.79 % 
Emacs                    1 hr 49 mins        █░░░░░░░░░░░░░░░░░░░░░░░░   05.96 % 
Unknown Wakatime         51 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.82 % 

💻 Operating System: 
Linux                    30 hrs 36 mins      █████████████████████████   100.00 % 
```


 Last Updated on 21/06/2026 00:35:00 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
