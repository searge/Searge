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
![Code Time](http://img.shields.io/badge/Code%20Time-4%2C279%20hrs%2043%20mins-blue?style=flat)

![AI Code Time](http://img.shields.io/badge/AI%20Code%20Time-623%20hrs%2021%20mins-blue?style=flat)

**I'm an Early 🐤** 

```text
🌞 Morning                3146 commits        ███████░░░░░░░░░░░░░░░░░░   26.14 % 
🌆 Daytime                5411 commits        ███████████░░░░░░░░░░░░░░   44.96 % 
🌃 Evening                3160 commits        ███████░░░░░░░░░░░░░░░░░░   26.26 % 
🌙 Night                  318 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   02.64 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 9 hrs 23 mins       ███████░░░░░░░░░░░░░░░░░░   29.38 % 
YAML                     9 hrs 1 min         ███████░░░░░░░░░░░░░░░░░░   28.23 % 
Other                    5 hrs 50 mins       █████░░░░░░░░░░░░░░░░░░░░   18.30 % 
Python                   4 hrs 49 mins       ████░░░░░░░░░░░░░░░░░░░░░   15.07 % 
XML                      58 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.05 % 

🔥 Editors: 
Claude Code              27 hrs 39 mins      ██████████████████████░░░   86.52 % 
Zed                      3 hrs 32 mins       ███░░░░░░░░░░░░░░░░░░░░░░   11.10 % 
Emacs                    27 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.44 % 
Vim                      8 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.45 % 
Zsh                      5 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.28 % 

💻 Operating System: 
Linux                    31 hrs 57 mins      █████████████████████████   100.00 % 
```

🤖 **AI Coding This Week** 

```text
⏱ AI Coding Time: 29 hrs 27 mins (92.14%)

✍️ 6,202 lines written by AI, 124 lines written by hand (98.04% AI-written)

🔤 16,401,799 Input Tokens, 1,762,621 Output Tokens

💵 $462.78 Estimated AI Cost This Week

🧠 30 AI Sessions, 327 AI Prompts

Opus                     5,904 lines         ████████████████████████░   95.18 % 
GPT                      190 lines           █░░░░░░░░░░░░░░░░░░░░░░░░   03.06 % 
Fable                    109 lines           ░░░░░░░░░░░░░░░░░░░░░░░░░   01.76 % 
Codex-Vscode             0 lines             ░░░░░░░░░░░░░░░░░░░░░░░░░   00.00 % 
Codex-Exec               0 lines             ░░░░░░░░░░░░░░░░░░░░░░░░░   00.00 % 

🔎 AI Coding Insights:
🤖 AI-Driven — 98.04% of written lines came from AI
📄 Detailed Prompter — average 734 characters per prompt
🔁 Iterative Prompter — average 11 prompts per session
🚀 High AI Trust — 6.2% of changed lines were hand-edited
```


 Last Updated on 13/09/2026 01:56:50 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
