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
![Code Time](http://img.shields.io/badge/Code%20Time-4%2C250%20hrs%2043%20mins-blue?style=flat)

![AI Code Time](http://img.shields.io/badge/AI%20Code%20Time-591%20hrs%2048%20mins-blue?style=flat)

**I'm an Early 🐤** 

```text
🌞 Morning                3231 commits        ██████░░░░░░░░░░░░░░░░░░░   25.68 % 
🌆 Daytime                5697 commits        ███████████░░░░░░░░░░░░░░   45.28 % 
🌃 Evening                3278 commits        ███████░░░░░░░░░░░░░░░░░░   26.05 % 
🌙 Night                  376 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   02.99 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 24 hrs 24 mins      ███████████░░░░░░░░░░░░░░   45.53 % 
YAML                     10 hrs 46 mins      █████░░░░░░░░░░░░░░░░░░░░   20.11 % 
Other                    7 hrs 49 mins       ████░░░░░░░░░░░░░░░░░░░░░   14.59 % 
Org                      5 hrs 3 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   09.43 % 
Go                       1 hr 37 mins        █░░░░░░░░░░░░░░░░░░░░░░░░   03.02 % 

🔥 Editors: 
Claude Code              47 hrs 38 mins      ██████████████████████░░░   88.88 % 
Zed                      4 hrs 10 mins       ██░░░░░░░░░░░░░░░░░░░░░░░   07.80 % 
Emacs                    1 hr 3 mins         ░░░░░░░░░░░░░░░░░░░░░░░░░   01.97 % 
Zsh                      23 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   00.74 % 
Codex Exec               8 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.27 % 

💻 Operating System: 
Linux                    53 hrs 36 mins      █████████████████████████   100.00 % 
```

🤖 **AI Coding This Week** 

```text
⏱ AI Coding Time: 51 hrs 28 mins (96.03%)

✍️ 10,270 lines written by AI, 539 lines written by hand (95.01% AI-written)

🔤 18,278,536 Input Tokens, 2,592,294 Output Tokens

💵 $794.99 Estimated AI Cost This Week

🧠 38 AI Sessions, 488 AI Prompts

Opus                     7,559 lines         ██████████████████░░░░░░░   71.22 % 
Fable                    2,816 lines         ███████░░░░░░░░░░░░░░░░░░   26.53 % 
GPT                      239 lines           █░░░░░░░░░░░░░░░░░░░░░░░░   02.25 % 
Codex-Exec               0 lines             ░░░░░░░░░░░░░░░░░░░░░░░░░   00.00 % 

🔎 AI Coding Insights:
🤖 AI-Driven — 95.01% of written lines came from AI
📄 Detailed Prompter — average 1,127 characters per prompt
🔁 Iterative Prompter — average 13 prompts per session
🚀 High AI Trust — 4.87% of changed lines were hand-edited
```


 Last Updated on 06/09/2026 01:47:26 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
