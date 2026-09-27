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
![Code Time](http://img.shields.io/badge/Code%20Time-4%2C331%20hrs%2021%20mins-blue?style=flat)

![AI Code Time](http://img.shields.io/badge/AI%20Code%20Time-683%20hrs%2014%20mins-blue?style=flat)

**I'm an Early 🐤** 

```text
🌞 Morning                3196 commits        ██████░░░░░░░░░░░░░░░░░░░   25.97 % 
🌆 Daytime                5550 commits        ███████████░░░░░░░░░░░░░░   45.10 % 
🌃 Evening                3221 commits        ███████░░░░░░░░░░░░░░░░░░   26.18 % 
🌙 Night                  338 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   02.75 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 11 hrs 16 mins      ████████░░░░░░░░░░░░░░░░░   30.87 % 
Other                    7 hrs 37 mins       █████░░░░░░░░░░░░░░░░░░░░   20.87 % 
YAML                     6 hrs 31 mins       ████░░░░░░░░░░░░░░░░░░░░░   17.87 % 
shell script             2 hrs 27 mins       ██░░░░░░░░░░░░░░░░░░░░░░░   06.72 % 
Org                      1 hr 59 mins        █░░░░░░░░░░░░░░░░░░░░░░░░   05.45 % 

🔥 Editors: 
Claude Code              28 hrs 31 mins      ████████████████████░░░░░   78.06 % 
Zed                      5 hrs               ███░░░░░░░░░░░░░░░░░░░░░░   13.70 % 
Codex Unknown            1 hr 48 mins        █░░░░░░░░░░░░░░░░░░░░░░░░   04.96 % 
Emacs                    54 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.50 % 
Zsh                      10 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   00.49 % 

💻 Operating System: 
Linux                    36 hrs 32 mins      █████████████████████████   100.00 % 
```

🤖 **AI Coding This Week** 

```text
⏱ AI Coding Time: 34 hrs 3 mins (93.18%)

✍️ 2,733 lines written by AI, 4 lines written by hand (99.85% AI-written)

🔤 13,762,609 Input Tokens, 1,688,218 Output Tokens

💵 $505.35 Estimated AI Cost This Week

🧠 22 AI Sessions, 379 AI Prompts

Opus                     1,404 lines         █████████████░░░░░░░░░░░░   51.37 % 
GPT                      1,329 lines         ████████████░░░░░░░░░░░░░   48.63 % 
Codex-Exec               0 lines             ░░░░░░░░░░░░░░░░░░░░░░░░░   00.00 % 
Fable                    0 lines             ░░░░░░░░░░░░░░░░░░░░░░░░░   00.00 % 

🔎 AI Coding Insights:
🤖 AI-Driven — 99.85% of written lines came from AI
📄 Detailed Prompter — average 770 characters per prompt
🔁 Iterative Prompter — average 17 prompts per session
🚀 High AI Trust — 0.4% of changed lines were hand-edited
```


 Last Updated on 27/09/2026 02:25:14 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
