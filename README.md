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
🌞 Morning                3346 commits        ███████░░░░░░░░░░░░░░░░░░   26.03 % 
🌆 Daytime                5859 commits        ███████████░░░░░░░░░░░░░░   45.57 % 
🌃 Evening                3336 commits        ██████░░░░░░░░░░░░░░░░░░░   25.95 % 
🌙 Night                  315 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   02.45 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 9 hrs 42 mins       ██████████░░░░░░░░░░░░░░░   38.67 % 
YAML                     6 hrs 14 mins       ██████░░░░░░░░░░░░░░░░░░░   24.88 % 
Org                      2 hrs 55 mins       ███░░░░░░░░░░░░░░░░░░░░░░   11.65 % 
Python                   2 hrs 6 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   08.41 % 
JSON                     1 hr 11 mins        █░░░░░░░░░░░░░░░░░░░░░░░░   04.73 % 

🔥 Editors: 
Claude Code              13 hrs 15 mins      █████████████░░░░░░░░░░░░   52.83 % 
Zed                      6 hrs 47 mins       ███████░░░░░░░░░░░░░░░░░░   27.05 % 
Unknown Wakatime         2 hrs 44 mins       ███░░░░░░░░░░░░░░░░░░░░░░   10.95 % 
Emacs                    1 hr 1 min          █░░░░░░░░░░░░░░░░░░░░░░░░   04.08 % 
VS Code                  45 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.99 % 

💻 Operating System: 
Linux                    25 hrs 5 mins       █████████████████████████   100.00 % 
```


 Last Updated on 28/06/2026 00:32:44 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
