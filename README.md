# AgeOfAnalytics
This repository holds a machine learning pipeline for analysing high level Age of Empires 2 games.

The goal is to build an analytical pipeline that can mine out effective strategy and tactical choices in high level games. By doing so, I hope to understand in more (emperical and analytical) detail the cutting edge of the game's meta.

# Technology
- AOE2 recordings can be accessed (with some difficulties) from the aoe.ms/replay API. The script in this repository borrows heavily from [this repository](https://github.com/dj0wns/AoE_Rec_Opening_Analysis/tree/main). dj0wns was the first I've seen to tackle AOE2 analytics - this profect follows a similar trajectory
- [My python package developed to mine out key statistics from a .AOE2RECORD file](https://github.com/byrnesy924/AgeAlyser_2)
- That package relies upon [this fork](https://github.com/AoEInsights/aoc-mgz) of [this a AOE2 recorded games parser](https://github.com/happyleavesaoc/aoc-mgz)


# Repository structure
- python script scrapes for games and continually stores them in blob storage
- this repository analyses the games using AgeAlyser2
- The resulting data is processed and analysed