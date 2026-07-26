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
🌞 Morning                3179 commits        ███████░░░░░░░░░░░░░░░░░░   26.20 % 
🌆 Daytime                5581 commits        ████████████░░░░░░░░░░░░░   46.00 % 
🌃 Evening                3064 commits        ██████░░░░░░░░░░░░░░░░░░░   25.26 % 
🌙 Night                  308 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   02.54 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 7 hrs 29 mins       ████████████░░░░░░░░░░░░░   48.42 % 
YAML                     3 hrs 17 mins       █████░░░░░░░░░░░░░░░░░░░░   21.26 % 
Python                   1 hr 9 mins         ██░░░░░░░░░░░░░░░░░░░░░░░   07.51 % 
Org                      1 hr 4 mins         ██░░░░░░░░░░░░░░░░░░░░░░░   06.95 % 
Other                    52 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   05.67 % 

🔥 Editors: 
Claude Code              10 hrs 16 mins      █████████████████░░░░░░░░   66.50 % 
Zed                      2 hrs 44 mins       ████░░░░░░░░░░░░░░░░░░░░░   17.73 % 
Unknown Wakatime         1 hr 20 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   08.70 % 
Emacs                    23 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.58 % 
Exec Wakatime            20 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.22 % 

💻 Operating System: 
Linux                    15 hrs 27 mins      █████████████████████████   100.00 % 
```


 Last Updated on 26/07/2026 01:37:09 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
