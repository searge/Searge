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
![Code Time](http://img.shields.io/badge/Code%20Time-4%2C351%20hrs%2050%20mins-blue?style=flat)

**I'm an Early 🐤** 

```text
🌞 Morning                3153 commits        ███████░░░░░░░░░░░░░░░░░░   26.48 % 
🌆 Daytime                5408 commits        ███████████░░░░░░░░░░░░░░   45.42 % 
🌃 Evening                3039 commits        ██████░░░░░░░░░░░░░░░░░░░   25.52 % 
🌙 Night                  306 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   02.57 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Other                    10 hrs 21 mins      █████████░░░░░░░░░░░░░░░░   37.13 % 
Markdown                 5 hrs 59 mins       █████░░░░░░░░░░░░░░░░░░░░   21.49 % 
Terraform                4 hrs               ████░░░░░░░░░░░░░░░░░░░░░   14.34 % 
YAML                     3 hrs 52 mins       ███░░░░░░░░░░░░░░░░░░░░░░   13.86 % 
sh                       1 hr 51 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   06.67 % 

🔥 Editors: 
VS Code                  24 hrs 6 mins       ██████████████████████░░░   86.44 % 
Zsh                      2 hrs 10 mins       ██░░░░░░░░░░░░░░░░░░░░░░░   07.81 % 
Emacs                    1 hr 4 mins         █░░░░░░░░░░░░░░░░░░░░░░░░   03.84 % 
Unknown Editor           19 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.15 % 
Zed                      10 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   00.60 % 

💻 Operating System: 
Linux                    27 hrs 53 mins      █████████████████████████   100.00 % 
```


 Last Updated on 26/04/2026 00:19:33 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
