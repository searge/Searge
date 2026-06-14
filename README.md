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
🌞 Morning                3316 commits        ███████░░░░░░░░░░░░░░░░░░   26.17 % 
🌆 Daytime                5794 commits        ███████████░░░░░░░░░░░░░░   45.73 % 
🌃 Evening                3253 commits        ██████░░░░░░░░░░░░░░░░░░░   25.67 % 
🌙 Night                  307 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   02.42 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 3 hrs 22 mins       ██████░░░░░░░░░░░░░░░░░░░   24.97 % 
YAML                     2 hrs 16 mins       ████░░░░░░░░░░░░░░░░░░░░░   16.87 % 
Other                    2 hrs 12 mins       ████░░░░░░░░░░░░░░░░░░░░░   16.38 % 
Org                      1 hr 22 mins        ███░░░░░░░░░░░░░░░░░░░░░░   10.17 % 
Text                     51 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   06.40 % 

🔥 Editors: 
Claude Code              6 hrs 9 mins        ███████████░░░░░░░░░░░░░░   45.55 % 
VS Code                  2 hrs 17 mins       ████░░░░░░░░░░░░░░░░░░░░░   16.96 % 
Zed                      2 hrs               ████░░░░░░░░░░░░░░░░░░░░░   14.89 % 
Unknown Wakatime         1 hr 57 mins        ████░░░░░░░░░░░░░░░░░░░░░   14.43 % 
Emacs                    57 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   07.12 % 

💻 Operating System: 
Linux                    13 hrs 30 mins      █████████████████████████   100.00 % 
```


 Last Updated on 14/06/2026 00:34:17 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
