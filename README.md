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
![Code Time](http://img.shields.io/badge/Code%20Time-4%2C178%20hrs%2029%20mins-blue?style=flat)

![AI Code Time](http://img.shields.io/badge/AI%20Code%20Time-514%20hrs%2047%20mins-blue?style=flat)

**I'm an Early 🐤** 

```text
🌞 Morning                3112 commits        ███████░░░░░░░░░░░░░░░░░░   26.07 % 
🌆 Daytime                5384 commits        ███████████░░░░░░░░░░░░░░   45.11 % 
🌃 Evening                3105 commits        ███████░░░░░░░░░░░░░░░░░░   26.02 % 
🌙 Night                  334 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   02.80 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 3 hrs 30 mins       ████████░░░░░░░░░░░░░░░░░   31.74 % 
YAML                     3 hrs 27 mins       ████████░░░░░░░░░░░░░░░░░   31.34 % 
Org                      2 hrs 1 min         █████░░░░░░░░░░░░░░░░░░░░   18.25 % 
Other                    1 hr 9 mins         ███░░░░░░░░░░░░░░░░░░░░░░   10.41 % 
TOML                     11 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.67 % 

🔥 Editors: 
Claude Code              6 hrs 9 mins        ██████████████░░░░░░░░░░░   55.67 % 
Zed                      2 hrs 12 mins       █████░░░░░░░░░░░░░░░░░░░░   19.93 % 
Codex Unknown            1 hr 57 mins        ████░░░░░░░░░░░░░░░░░░░░░   17.71 % 
Emacs                    24 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.74 % 
Zsh                      16 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.46 % 

💻 Operating System: 
Linux                    11 hrs 3 mins       █████████████████████████   100.00 % 
```

🤖 **AI Coding This Week** 

```text
⏱ AI Coding Time: 9 hrs 6 mins (82.33%)

✍️ 1,223 lines written by AI, 11 lines written by hand (99.11% AI-written)

🔤 4,101,598 Input Tokens, 290,723 Output Tokens

💵 $77.93 Estimated AI Cost This Week

🧠 20 AI Sessions, 114 AI Prompts

Fable                    873 lines           █████████████████░░░░░░░░   66.24 % 
GPT                      445 lines           ████████░░░░░░░░░░░░░░░░░   33.76 % 
Opus                     0 lines             ░░░░░░░░░░░░░░░░░░░░░░░░░   00.00 % 

🔎 AI Coding Insights:
🤖 AI-Driven — 99.11% of written lines came from AI
📄 Detailed Prompter — average 1,390 characters per prompt
🔁 Iterative Prompter — average 6 prompts per session
🚀 High AI Trust — 14.47% of changed lines were hand-edited
```


 Last Updated on 23/08/2026 00:43:49 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
