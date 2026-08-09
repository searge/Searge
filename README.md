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
![Code Time](http://img.shields.io/badge/Code%20Time-4%2C127%20hrs%2034%20mins-blue?style=flat)

![AI Code Time](http://img.shields.io/badge/AI%20Code%20Time-464%20hrs%2018%20mins-blue?style=flat)

**I'm an Early 🐤** 

```text
🌞 Morning                3047 commits        ███████░░░░░░░░░░░░░░░░░░   26.31 % 
🌆 Daytime                5215 commits        ███████████░░░░░░░░░░░░░░   45.02 % 
🌃 Evening                3011 commits        ██████░░░░░░░░░░░░░░░░░░░   25.99 % 
🌙 Night                  310 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   02.68 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 8 hrs 35 mins       █████████░░░░░░░░░░░░░░░░   34.70 % 
YAML                     6 hrs 53 mins       ███████░░░░░░░░░░░░░░░░░░   27.81 % 
Org                      3 hrs 29 mins       ████░░░░░░░░░░░░░░░░░░░░░   14.11 % 
Go                       51 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.47 % 
Other                    46 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.10 % 

🔥 Editors: 
Claude Code              17 hrs 49 mins      ██████████████████░░░░░░░   71.99 % 
Zed                      3 hrs 52 mins       ████░░░░░░░░░░░░░░░░░░░░░   15.67 % 
Emacs                    53 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.62 % 
Obsidian                 36 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.46 % 
Codex CLI                28 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.90 % 

💻 Operating System: 
Linux                    24 hrs 46 mins      █████████████████████████   100.00 % 
```

🤖 **AI Coding This Week** 

```text
⏱ AI Coding Time: 22 hrs 7 mins (89.3%)

✍️ 7,948 lines written by AI, 87 lines written by hand (98.92% AI-written)

🔤 348,033,684 Input Tokens, 1,129,063 Output Tokens

💵 $1813.60 Estimated AI Cost This Week

🧠 29 AI Sessions, 236 AI Prompts

Opus                     8,201 lines         █████████████████████████   99.71 % 
GPT                      24 lines            ░░░░░░░░░░░░░░░░░░░░░░░░░   00.29 % 
Exec-Wakatime            0 lines             ░░░░░░░░░░░░░░░░░░░░░░░░░   00.00 % 
Claude-Code              0 lines             ░░░░░░░░░░░░░░░░░░░░░░░░░   00.00 % 

🔎 AI Coding Insights:
🤖 AI-Driven — 98.92% of written lines came from AI
📚 Verbose Prompter — average 2,049 characters per prompt
🔁 Iterative Prompter — average 8 prompts per session
🚀 High AI Trust — 2.27% of changed lines were hand-edited
```


 Last Updated on 09/08/2026 00:54:55 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
