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
🌞 Morning                3127 commits        ███████░░░░░░░░░░░░░░░░░░   26.54 % 
🌆 Daytime                5313 commits        ███████████░░░░░░░░░░░░░░   45.09 % 
🌃 Evening                3046 commits        ██████░░░░░░░░░░░░░░░░░░░   25.85 % 
🌙 Night                  298 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   02.53 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
YAML                     9 hrs 31 mins       ███████░░░░░░░░░░░░░░░░░░   29.72 % 
Org                      8 hrs 7 mins        ██████░░░░░░░░░░░░░░░░░░░   25.35 % 
Markdown                 5 hrs 16 mins       ████░░░░░░░░░░░░░░░░░░░░░   16.49 % 
Other                    4 hrs 19 mins       ███░░░░░░░░░░░░░░░░░░░░░░   13.52 % 
sh                       1 hr 52 mins        █░░░░░░░░░░░░░░░░░░░░░░░░   05.86 % 

🔥 Editors: 
Zed                      18 hrs 20 mins      ██████████████░░░░░░░░░░░   57.28 % 
Emacs                    5 hrs 40 mins       ████░░░░░░░░░░░░░░░░░░░░░   17.73 % 
Unknown Editor           4 hrs 21 mins       ███░░░░░░░░░░░░░░░░░░░░░░   13.59 % 
Zsh                      2 hrs 43 mins       ██░░░░░░░░░░░░░░░░░░░░░░░   08.50 % 
VS Code                  48 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.52 % 

💻 Operating System: 
Linux                    32 hrs 1 min        █████████████████████████   100.00 % 
```


 Last Updated on 03/05/2026 00:23:03 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
