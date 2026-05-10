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
🌞 Morning                3189 commits        ███████░░░░░░░░░░░░░░░░░░   26.44 % 
🌆 Daytime                5451 commits        ███████████░░░░░░░░░░░░░░   45.19 % 
🌃 Evening                3123 commits        ██████░░░░░░░░░░░░░░░░░░░   25.89 % 
🌙 Night                  300 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   02.49 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
YAML                     7 hrs 27 mins       ████████░░░░░░░░░░░░░░░░░   31.98 % 
Other                    5 hrs 45 mins       ██████░░░░░░░░░░░░░░░░░░░   24.67 % 
Org                      4 hrs 15 mins       █████░░░░░░░░░░░░░░░░░░░░   18.25 % 
Markdown                 2 hrs 52 mins       ███░░░░░░░░░░░░░░░░░░░░░░   12.30 % 
Svelte                   36 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.62 % 

🔥 Editors: 
Zed                      15 hrs 41 mins      █████████████████░░░░░░░░   67.26 % 
Unknown Editor           3 hrs 15 mins       ███░░░░░░░░░░░░░░░░░░░░░░   13.99 % 
Emacs                    2 hrs 44 mins       ███░░░░░░░░░░░░░░░░░░░░░░   11.78 % 
Zsh                      1 hr 30 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   06.46 % 
VS Code                  6 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.46 % 

💻 Operating System: 
Linux                    23 hrs 20 mins      █████████████████████████   100.00 % 
```


 Last Updated on 10/05/2026 00:24:47 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
