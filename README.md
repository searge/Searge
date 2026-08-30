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
![Code Time](http://img.shields.io/badge/Code%20Time-4%2C204%20hrs%2027%20mins-blue?style=flat)

![AI Code Time](http://img.shields.io/badge/AI%20Code%20Time-538%20hrs%2041%20mins-blue?style=flat)

**I'm an Early 🐤** 

```text
🌞 Morning                3169 commits        ██████░░░░░░░░░░░░░░░░░░░   25.92 % 
🌆 Daytime                5523 commits        ███████████░░░░░░░░░░░░░░   45.18 % 
🌃 Evening                3176 commits        ██████░░░░░░░░░░░░░░░░░░░   25.98 % 
🌙 Night                  356 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   02.91 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 9 hrs 39 mins       ███████████░░░░░░░░░░░░░░   42.41 % 
Org                      4 hrs 39 mins       █████░░░░░░░░░░░░░░░░░░░░   20.44 % 
YAML                     3 hrs 4 mins        ███░░░░░░░░░░░░░░░░░░░░░░   13.51 % 
Other                    1 hr 29 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   06.56 % 
Python                   53 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.89 % 

🔥 Editors: 
Claude Code              16 hrs 16 mins      ██████████████████░░░░░░░   71.51 % 
Zed                      3 hrs 18 mins       ████░░░░░░░░░░░░░░░░░░░░░   14.54 % 
Emacs                    1 hr 34 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   06.90 % 
Codex Unknown            47 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.50 % 
Zsh                      22 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.65 % 

💻 Operating System: 
Linux                    22 hrs 45 mins      █████████████████████████   100.00 % 
```

🤖 **AI Coding This Week** 

```text
⏱ AI Coding Time: 20 hrs 15 mins (89.02%)

✍️ 3,831 lines written by AI, 39 lines written by hand (98.99% AI-written)

🔤 11,556,001 Input Tokens, 1,088,253 Output Tokens

💵 $289.06 Estimated AI Cost This Week

🧠 29 AI Sessions, 267 AI Prompts

Fable                    2,476 lines         ███████████████░░░░░░░░░░   60.97 % 
Opus                     947 lines           ██████░░░░░░░░░░░░░░░░░░░   23.32 % 
GPT                      638 lines           ████░░░░░░░░░░░░░░░░░░░░░   15.71 % 
Codex-Exec               0 lines             ░░░░░░░░░░░░░░░░░░░░░░░░░   00.00 % 
Haiku                    0 lines             ░░░░░░░░░░░░░░░░░░░░░░░░░   00.00 % 

🔎 AI Coding Insights:
🤖 AI-Driven — 98.99% of written lines came from AI
📚 Verbose Prompter — average 1,851 characters per prompt
🔁 Iterative Prompter — average 9 prompts per session
🚀 High AI Trust — 1.43% of changed lines were hand-edited
```


 Last Updated on 30/08/2026 02:15:58 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
