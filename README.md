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
![Code Time](http://img.shields.io/badge/Code%20Time-4%2C108%20hrs%2028%20mins-blue?style=flat)

![AI Code Time](http://img.shields.io/badge/AI%20Code%20Time-447%20hrs%201%20min-blue?style=flat)

**I'm an Early 🐤** 

```text
🌞 Morning                3186 commits        ███████░░░░░░░░░░░░░░░░░░   26.22 % 
🌆 Daytime                5591 commits        ████████████░░░░░░░░░░░░░   46.01 % 
🌃 Evening                3068 commits        ██████░░░░░░░░░░░░░░░░░░░   25.24 % 
🌙 Night                  308 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   02.53 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
YAML                     8 hrs 12 mins       ████████░░░░░░░░░░░░░░░░░   32.24 % 
Markdown                 7 hrs 19 mins       ███████░░░░░░░░░░░░░░░░░░   28.74 % 
Bash                     3 hrs 30 mins       ███░░░░░░░░░░░░░░░░░░░░░░   13.75 % 
Python                   2 hrs 1 min         ██░░░░░░░░░░░░░░░░░░░░░░░   07.96 % 
Org                      1 hr 17 mins        █░░░░░░░░░░░░░░░░░░░░░░░░   05.06 % 

🔥 Editors: 
Claude Code              19 hrs 1 min        ███████████████████░░░░░░   74.63 % 
Zed                      2 hrs 43 mins       ███░░░░░░░░░░░░░░░░░░░░░░   10.67 % 
Unknown Wakatime         2 hrs 2 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   08.03 % 
Exec Wakatime            39 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.61 % 
VS Code                  31 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.06 % 

💻 Operating System: 
Linux                    25 hrs 28 mins      █████████████████████████   100.00 % 
```

🤖 **AI Coding This Week** 

```text
⏱ AI Coding Time: 23 hrs 24 mins (91.87%)

✍️ 14,877 lines written by AI, 48 lines written by hand (99.68% AI-written)

🔤 644,834,130 Input Tokens, 1,400,110 Output Tokens

💵 $3115.45 Estimated AI Cost This Week

🧠 33 AI Sessions, 205 AI Prompts

Opus                     11,809 lines        ██████████████████████░░░   87.13 % 
GPT                      1,744 lines         ███░░░░░░░░░░░░░░░░░░░░░░   12.87 % 
Sonnet                   0 lines             ░░░░░░░░░░░░░░░░░░░░░░░░░   00.00 % 
Exec-Wakatime            0 lines             ░░░░░░░░░░░░░░░░░░░░░░░░░   00.00 % 
Vscode-Wakatime          0 lines             ░░░░░░░░░░░░░░░░░░░░░░░░░   00.00 % 

🔎 AI Coding Insights:
🤖 AI-Driven — 99.68% of written lines came from AI
📄 Detailed Prompter — average 1,281 characters per prompt
🔁 Iterative Prompter — average 6 prompts per session
🚀 High AI Trust — 0.52% of changed lines were hand-edited
```


 Last Updated on 02/08/2026 01:37:34 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
