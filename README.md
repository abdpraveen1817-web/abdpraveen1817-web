```md
<!-- PROFILE README: Create a public repository named exactly abdpraveen1817-web -->

<div align="center">

  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=26&pause=1000&color=2F81F7&center=true&vCenter=true&width=600&lines=Hi%2C+I'm+Praveen+%F0%9F%91%8B;Student+at+GCT;Learning+to+build+great+things;Welcome+to+my+GitHub+profile!" alt="Animated introduction" />

  <br />

  <a href="https://github.com/abdpraveen1817-web">
    <img src="https://komarev.com/ghpvc/?username=abdpraveen1817-web&label=Profile%20views&color=2f81f7&style=flat" alt="Profile views" />
  </a>

</div>

---

## 👨‍💻 About Me

I’m **Praveen**, a student at **GCT** and an aspiring developer learning to turn ideas into useful, beautiful software.

- 🌱 Currently learning **Git, GitHub, and web development**
- 🛠️ Building small projects and improving every day
- 🎯 Goal: create projects I’m proud to share
- 📫 Reach me: **add-your-email-here**

## 🧰 Tools I’m Learning

<p>
  <img src="https://skillicons.dev/icons?i=html,css,js,git,github,vscode,figma&theme=dark" alt="Skills" />
</p>

> Keep only the icons for tools you actually use. More icons do not make a profile more professional.

## 📌 Featured Projects

| Project | What it is | Tech |
| :--- | :--- | :--- |
| [My first project](https://github.com/abdpraveen1817-web/PROJECT_NAME) | A short, clear one-sentence description. | HTML, CSS, JavaScript |
| [Learning notes](https://github.com/abdpraveen1817-web/learning-notes) | Notes and mini-exercises from my coding journey. | Markdown |

## 📊 GitHub Activity

<div align="center">

  <img height="165" src="https://github-readme-stats.vercel.app/api?username=abdpraveen1817-web&show_icons=true&hide_border=true&rank_icon=github&theme=transparent" alt="GitHub statistics" />
  <img height="165" src="https://github-readme-streak-stats.herokuapp.com?user=abdpraveen1817-web&theme=transparent&hide_border=true" alt="GitHub contribution streak" />

</div>

## 🐍 Contribution Animation

<div align="center">
  <img src="https://raw.githubusercontent.com/abdpraveen1817-web/abdpraveen1817-web/output/github-contribution-grid-snake-dark.svg" alt="Animated contribution snake" />
</div>

## 🤝 Connect With Me

<p>
  <a href="https://www.linkedin.com/in/YOUR_LINKEDIN_USERNAME/">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
  </a>
  <a href="mailto:your.email@example.com">
    <img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" />
  </a>
</p>

<div align="center">

  _Thanks for visiting — I’m always learning._

</div>
```

---

```yaml
name: Generate contribution snake

on:
  schedule:
    - cron: "0 0 * * *"
  workflow_dispatch:
  push:
    branches:
      - main

jobs:
  build:
    runs-on: ubuntu-latest
    permissions:
      contents: write
    steps:
      - name: Generate snake animation
        uses: Platane/snk/svg-only@v3
        with:
          github_user_name: abdpraveen1817-web
          outputs: |
            dist/github-contribution-grid-snake.svg
            dist/github-contribution-grid-snake-dark.svg?palette=github-dark

      - name: Publish snake animation
        uses: crazy-max/ghaction-github-pages@v4
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```
