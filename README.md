### Hi there 👋

<!--
**nguyenhung111/nguyenhung111** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
<!--START_SECTION:waka-->
<!--END_SECTION:waka-->
name: Waka Readme

on:
  # for manual workflow trigger
  workflow_dispatch:
  schedule:
    # runs at 12 AM UTC (5:30 AM IST)
    - cron: "0 0 * * *"

jobs:
  update-readme:
    name: WakaReadme DevAND
    runs-on: mac-latest
    steps:
      - uses: nguyehung111/README@master
        with:
          WAKATIME_API_KEY: ${{ secrets.WAKATIME_API_KEY }}
