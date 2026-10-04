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
![Code Time](http://img.shields.io/badge/Code%20Time-4%2C358%20hrs%2051%20mins-blue?style=flat)

![AI Code Time](http://img.shields.io/badge/AI%20Code%20Time-714%20hrs%2023%20mins-blue?style=flat)

**I'm an Early 🐤** 

```text
🌞 Morning                3246 commits        ██████░░░░░░░░░░░░░░░░░░░   25.85 % 
🌆 Daytime                5676 commits        ███████████░░░░░░░░░░░░░░   45.21 % 
🌃 Evening                3275 commits        ███████░░░░░░░░░░░░░░░░░░   26.09 % 
🌙 Night                  358 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   02.85 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 12 hrs 35 mins      █████████░░░░░░░░░░░░░░░░   37.85 % 
YAML                     7 hrs 33 mins       ██████░░░░░░░░░░░░░░░░░░░   22.73 % 
Other                    6 hrs 25 mins       █████░░░░░░░░░░░░░░░░░░░░   19.32 % 
JSON                     1 hr 23 mins        █░░░░░░░░░░░░░░░░░░░░░░░░   04.17 % 
Bash                     1 hr 15 mins        █░░░░░░░░░░░░░░░░░░░░░░░░   03.77 % 

🔥 Editors: 
Claude Code              29 hrs 2 mins       ██████████████████████░░░   87.25 % 
Zed                      2 hrs 53 mins       ██░░░░░░░░░░░░░░░░░░░░░░░   08.70 % 
Zsh                      55 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.77 % 
Emacs                    14 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   00.70 % 
Codex Exec               8 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.44 % 

💻 Operating System: 
Linux                    33 hrs 16 mins      █████████████████████████   100.00 % 
```

🤖 **AI Coding This Week** 

```text
⏱ AI Coding Time: 30 hrs 41 mins (92.2%)

✍️ 2,322 lines written by AI, 1,319 lines written by hand (63.77% AI-written)

🔤 13,104,003 Input Tokens, 1,970,094 Output Tokens

💵 $463.82 Estimated AI Cost This Week

🧠 28 AI Sessions, 461 AI Prompts

Opus                     1,694 lines         █████████████████░░░░░░░░   69.88 % 
Sonnet                   646 lines           ███████░░░░░░░░░░░░░░░░░░   26.65 % 
GPT                      84 lines            █░░░░░░░░░░░░░░░░░░░░░░░░   03.47 % 
Fable                    0 lines             ░░░░░░░░░░░░░░░░░░░░░░░░░   00.00 % 
Codex-Exec               0 lines             ░░░░░░░░░░░░░░░░░░░░░░░░░   00.00 % 

🔎 AI Coding Insights:
⚖️ Balanced with AI — 63.77% of written lines came from AI
📄 Detailed Prompter — average 627 characters per prompt
🔁 Iterative Prompter — average 16 prompts per session
🚀 High AI Trust — 35.89% of changed lines were hand-edited
```


 Last Updated on 04/10/2026 03:20:31 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
