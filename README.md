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
🌞 Morning                3368 commits        ██████░░░░░░░░░░░░░░░░░░░   25.96 % 
🌆 Daytime                5912 commits        ███████████░░░░░░░░░░░░░░   45.57 % 
🌃 Evening                3373 commits        ██████░░░░░░░░░░░░░░░░░░░   26.00 % 
🌙 Night                  320 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   02.47 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
YAML                     7 hrs 8 mins        ██████████░░░░░░░░░░░░░░░   41.74 % 
Markdown                 4 hrs 40 mins       ███████░░░░░░░░░░░░░░░░░░   27.33 % 
Other                    1 hr 38 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   09.59 % 
Org                      1 hr 13 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   07.13 % 
Bash                     55 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   05.36 % 

🔥 Editors: 
Claude Code              8 hrs 58 mins       █████████████░░░░░░░░░░░░   52.43 % 
Zed                      4 hrs 19 mins       ██████░░░░░░░░░░░░░░░░░░░   25.29 % 
VS Code                  1 hr 42 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   09.98 % 
Unknown Wakatime         1 hr 23 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   08.16 % 
Emacs                    32 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.17 % 

💻 Operating System: 
Linux                    17 hrs 6 mins       █████████████████████████   100.00 % 
```


 Last Updated on 05/07/2026 00:29:21 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
