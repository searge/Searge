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
🌞 Morning                2656 commits        ██████░░░░░░░░░░░░░░░░░░░   25.80 % 
🌆 Daytime                4631 commits        ███████████░░░░░░░░░░░░░░   44.98 % 
🌃 Evening                2713 commits        ███████░░░░░░░░░░░░░░░░░░   26.35 % 
🌙 Night                  296 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   02.87 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Python                   7 hrs 4 mins        ██████████░░░░░░░░░░░░░░░   41.16 % 
sh                       2 hrs 24 mins       ████░░░░░░░░░░░░░░░░░░░░░   14.05 % 
Org                      1 hr 47 mins        ███░░░░░░░░░░░░░░░░░░░░░░   10.43 % 
YAML                     1 hr 32 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   09.00 % 
Markdown                 1 hr 26 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   08.42 % 

🔥 Editors: 
VS Code                  12 hrs 10 mins      ██████████████████░░░░░░░   70.85 % 
Zsh                      2 hrs 24 mins       ████░░░░░░░░░░░░░░░░░░░░░   14.05 % 
Emacs                    1 hr 34 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   09.17 % 
Zed                      1 hr 1 min          █░░░░░░░░░░░░░░░░░░░░░░░░   05.93 % 

💻 Operating System: 
Linux                    17 hrs 11 mins      █████████████████████████   100.00 % 
```


 Last Updated on 29/03/2026 00:13:53 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
