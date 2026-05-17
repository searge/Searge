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
![Code Time](http://img.shields.io/badge/Code%20Time-4%2C440%20hrs%2033%20mins-blue?style=flat)

**I'm an Early 🐤** 

```text
🌞 Morning                3205 commits        ███████░░░░░░░░░░░░░░░░░░   26.40 % 
🌆 Daytime                5504 commits        ███████████░░░░░░░░░░░░░░   45.35 % 
🌃 Evening                3129 commits        ██████░░░░░░░░░░░░░░░░░░░   25.78 % 
🌙 Night                  300 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   02.47 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Org                      9 hrs 7 mins        ███████░░░░░░░░░░░░░░░░░░   28.34 % 
YAML                     6 hrs 33 mins       █████░░░░░░░░░░░░░░░░░░░░   20.36 % 
Markdown                 4 hrs 21 mins       ███░░░░░░░░░░░░░░░░░░░░░░   13.56 % 
Other                    3 hrs 38 mins       ███░░░░░░░░░░░░░░░░░░░░░░   11.30 % 
sh                       2 hrs 12 mins       ██░░░░░░░░░░░░░░░░░░░░░░░   06.84 % 

🔥 Editors: 
Zed                      15 hrs 34 mins      ████████████░░░░░░░░░░░░░   48.42 % 
Unknown Editor           6 hrs 53 mins       █████░░░░░░░░░░░░░░░░░░░░   21.42 % 
Emacs                    5 hrs 19 mins       ████░░░░░░░░░░░░░░░░░░░░░   16.55 % 
Zsh                      3 hrs 32 mins       ███░░░░░░░░░░░░░░░░░░░░░░   11.02 % 
VS Code                  46 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.38 % 

💻 Operating System: 
Linux                    32 hrs 10 mins      █████████████████████████   100.00 % 
```


 Last Updated on 17/05/2026 00:26:24 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
