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
![Code Time](http://img.shields.io/badge/Code%20Time-4%2C294%20hrs%2053%20mins-blue?style=flat)

![AI Code Time](http://img.shields.io/badge/AI%20Code%20Time-639%20hrs%2040%20mins-blue?style=flat)

**I'm an Early 🐤** 

```text
🌞 Morning                3148 commits        ███████░░░░░░░░░░░░░░░░░░   26.11 % 
🌆 Daytime                5424 commits        ███████████░░░░░░░░░░░░░░   44.99 % 
🌃 Evening                3167 commits        ███████░░░░░░░░░░░░░░░░░░   26.27 % 
🌙 Night                  318 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   02.64 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
YAML                     6 hrs 45 mins       ██████░░░░░░░░░░░░░░░░░░░   24.28 % 
Org                      5 hrs 54 mins       █████░░░░░░░░░░░░░░░░░░░░   21.20 % 
Markdown                 5 hrs 49 mins       █████░░░░░░░░░░░░░░░░░░░░   20.88 % 
Other                    4 hrs 36 mins       ████░░░░░░░░░░░░░░░░░░░░░   16.55 % 
Bash                     1 hr 30 mins        █░░░░░░░░░░░░░░░░░░░░░░░░   05.40 % 

🔥 Editors: 
Claude Code              23 hrs 26 mins      █████████████████████░░░░   84.09 % 
Zed                      2 hrs 42 mins       ██░░░░░░░░░░░░░░░░░░░░░░░   09.73 % 
Emacs                    59 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.56 % 
Zsh                      28 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.71 % 
Vim                      12 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   00.76 % 

💻 Operating System: 
Linux                    27 hrs 52 mins      █████████████████████████   100.00 % 
```

🤖 **AI Coding This Week** 

```text
⏱ AI Coding Time: 25 hrs 29 mins (91.46%)

✍️ 6,355 lines written by AI, 120 lines written by hand (98.15% AI-written)

🔤 9,471,775 Input Tokens, 1,326,034 Output Tokens

💵 $384.47 Estimated AI Cost This Week

🧠 13 AI Sessions, 259 AI Prompts

Opus                     4,486 lines         █████████████████░░░░░░░░   68.72 % 
Fable                    1,936 lines         ███████░░░░░░░░░░░░░░░░░░   29.66 % 
GPT                      106 lines           ░░░░░░░░░░░░░░░░░░░░░░░░░   01.62 % 
Codex-Exec               0 lines             ░░░░░░░░░░░░░░░░░░░░░░░░░   00.00 % 

🔎 AI Coding Insights:
🤖 AI-Driven — 98.15% of written lines came from AI
📝 Concise Prompter — average 394 characters per prompt
🔁 Iterative Prompter — average 20 prompts per session
🚀 High AI Trust — 2.08% of changed lines were hand-edited
```


 Last Updated on 20/09/2026 02:13:51 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
