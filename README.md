<h1>Welcome to My GitHub! 👋</h1>


__Hi there!__  
I'm Jeremy, a tech enthusiast passionate about **web development** and **robotics**. This is the space where I share my projects, ideas, and collaborations, all driven by curiosity and a love for innovation.   


![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E)
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)

## Key Aspects  

🎓 I’m a student exploring robotics, web development, and automation.  
🤖 Learning to combine software and hardware to build innovative solutions.  
👨‍💻 My projects focus on gaining experience and improving my skills.  
💬 Always open to learning and collaborating on tech-related ideas.  

---
# stats and advances 


[![jeremy's GitHub stats](https://github-readme-stats.vercel.app/api?username=JDeleon2780&show_icons=true&theme=tokyonight)](https://github.com/JDeleon2780/github-readme-stats)
name: 🌸 Anilist watch list and reading list
category: social
description: |
  This plugin displays favorites animes, mangas and characters from a [AniList](https://anilist.co) account.
disclaimer: |
  This plugin is not affiliated, associated, authorized, endorsed by, or in any way officially connected with [AniList](https://anilist.co).
  All product and company names are trademarks™ or registered® trademarks of their respective holders.
examples:
  +for anime watchers: https://github.com/lowlighter/metrics/blob/examples/metrics.plugin.anilist.svg
  for manga readers: https://github.com/lowlighter/metrics/blob/examples/metrics.plugin.anilist.manga.svg
  +for waifus simp: https://github.com/lowlighter/metrics/blob/examples/metrics.plugin.anilist.characters.svg
index: 4
supports:
  - user
  - organization
scopes: []
inputs:

  plugin_anilist:
    description: |
      Enable aniList plugin
    type: boolean
    default: no
    extras:
      - metrics.run.puppeteer.scrapping

  plugin_anilist_user:
    type: string
    description: |
      AniList login
    default: .user.login
    preset: no

  plugin_anilist_medias:
    description: |
      Medias types
    type: array
    format: comma-separated
    default: anime, manga
    values:
      - anime
      - manga

  plugin_anilist_sections:
    description: |
      Displayed sections

      - `favorites` will display favorites from `plugin_anilist_medias`
      - `watching` will display animes currently in watching list
      - `reading` will display manga currently in reading list
      - `characters` will display liked characters
    type: array
    format: comma-separated
    default: favorites
    example: favorites, watching, characters
    values:
      - favorites
      - watching
      - reading
      - characters

  plugin_anilist_limit:
    description: |
      Display limit (medias)
    type: number
    default: 2
    min: 0
    zero: disable

  plugin_anilist_limit_characters:
    description: |
      Display limit (characters)
    type: number
    default: 22
    min: 0
    zero: disable

  plugin_anilist_shuffle:
    description: |
      Shuffle data

      Can be used to create varied outputs
    type: boolean
    default: yes
