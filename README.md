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
![Code Time](http://img.shields.io/badge/Code%20Time-3%2C901%20hrs%2028%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                2161 commits        ███████░░░░░░░░░░░░░░░░░░   26.51 % 
🌆 Daytime                3466 commits        ███████████░░░░░░░░░░░░░░   42.51 % 
🌃 Evening                2252 commits        ███████░░░░░░░░░░░░░░░░░░   27.62 % 
🌙 Night                  274 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.36 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       11 hrs 39 mins      ████████████████████░░░░░   78.69 % 
YAML                     48 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   05.51 % 
JSON                     36 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.07 % 
Terraform                28 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.25 % 
Markdown                 28 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.22 % 

🔥 Editors: 
Zsh                      11 hrs 39 mins      ████████████████████░░░░░   78.69 % 
VS Code                  2 hrs 47 mins       █████░░░░░░░░░░░░░░░░░░░░   18.85 % 
Sublime Text             17 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.94 % 
Vim                      4 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.52 % 

💻 Operating System: 
Linux                    14 hrs 48 mins      █████████████████████████   100.00 % 
```


 Last Updated on 07/12/2025 00:08:18 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
