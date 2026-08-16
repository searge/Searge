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
![Code Time](http://img.shields.io/badge/Code%20Time-4%2C172%20hrs%2031%20mins-blue?style=flat)

![AI Code Time](http://img.shields.io/badge/AI%20Code%20Time-508%20hrs%2031%20mins-blue?style=flat)

**I'm an Early 🐤** 

```text
🌞 Morning                3071 commits        ███████░░░░░░░░░░░░░░░░░░   26.19 % 
🌆 Daytime                5282 commits        ███████████░░░░░░░░░░░░░░   45.05 % 
🌃 Evening                3057 commits        ███████░░░░░░░░░░░░░░░░░░   26.07 % 
🌙 Night                  314 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   02.68 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
YAML                     9 hrs 51 mins       ██████░░░░░░░░░░░░░░░░░░░   23.45 % 
Markdown                 8 hrs 58 mins       █████░░░░░░░░░░░░░░░░░░░░   21.36 % 
Org                      6 hrs 3 mins        ████░░░░░░░░░░░░░░░░░░░░░   14.41 % 
Java                     5 hrs 41 mins       ███░░░░░░░░░░░░░░░░░░░░░░   13.55 % 
Python                   4 hrs 21 mins       ███░░░░░░░░░░░░░░░░░░░░░░   10.35 % 

🔥 Editors: 
Claude Code              33 hrs 43 mins      ████████████████████░░░░░   80.23 % 
Zed                      4 hrs 14 mins       ███░░░░░░░░░░░░░░░░░░░░░░   10.11 % 
Unknown Wakatime         1 hr 38 mins        █░░░░░░░░░░░░░░░░░░░░░░░░   03.92 % 
Emacs                    59 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.36 % 
VS Code                  50 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.02 % 

💻 Operating System: 
Linux                    42 hrs 1 min        █████████████████████████   100.00 % 
```

🤖 **AI Coding This Week** 

```text
⏱ AI Coding Time: 39 hrs 5 mins (93.02%)

✍️ 12,364 lines written by AI, 720 lines written by hand (94.5% AI-written)

🔤 56,664,493 Input Tokens, 2,056,898 Output Tokens

💵 $1089.21 Estimated AI Cost This Week

🧠 44 AI Sessions, 405 AI Prompts

Opus                     8,574 lines         █████████████████░░░░░░░░   67.73 % 
Fable                    3,880 lines         ████████░░░░░░░░░░░░░░░░░   30.65 % 
GPT                      206 lines           ░░░░░░░░░░░░░░░░░░░░░░░░░   01.63 % 
Codex-Exec               0 lines             ░░░░░░░░░░░░░░░░░░░░░░░░░   00.00 % 

🔎 AI Coding Insights:
🤖 AI-Driven — 94.5% of written lines came from AI
📄 Detailed Prompter — average 1,077 characters per prompt
🔁 Iterative Prompter — average 9 prompts per session
🚀 High AI Trust — 5.61% of changed lines were hand-edited
```


 Last Updated on 16/08/2026 00:41:08 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
