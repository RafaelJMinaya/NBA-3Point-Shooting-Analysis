# NBA 3-Point Shooting Trends Analysis 🏀

## 0. Overview
The NBA has experienced numerous transformative eras since the ABA-NBA merger, each bringing revolutionary changes to the game. One of the most significant eras is the current 3-Point Revolution, which began in the mid-2010s. Over the past decade, the prominence of the 3-point shot has dramatically reshaped the game, a stark contrast to earlier decades. This study analyzes NBA game and season data from 1999–2000 to 2022–2023 regular seasons to observe 3-point shooting trends and provide a comprehensive scoring analysis focused on contemporary player shooting behaviors.

![Joel-Embiid-DESKTOP-RAFAEL](https://github.com/user-attachments/assets/1605895d-5f13-4710-a535-eb5cffe2bdee)

Key Questions:

1. When and how did the NBA 3-Point boom emerge in the past 20 years?
2. What are some common shooting habits of today's players compared to their veteran counterparts from the early 2000s?




## 1. Data Overview¶
For this exploration of 3-point shooting, we'll be implementing the use of different NBA shooting datasets found on Kaggle. All DataFrames have been cleaned to have no missing or null values (please look into the code to see different processes applied to clean data).

**Team Statistics Dataset**:
>Mostly comprised of Field Goals made and attempt rates by teams throughout many seasons.

**Individual Player Shooting Dataset**:
>Focuses on providing player shooting rates from different distances on the court.

**Yearly Positional Shooting Datasets**:
>These collection of datasets provide positional data of every shot attempted by every player in the NBA within the specified season.



## 2. **Shooting Breakdowns**
2.1  **3-Pointers vs 2-Pointers**
![__results___9_1](https://github.com/user-attachments/assets/c3e712b1-2ed7-4302-bc08-6704aad2843b)

Over the past 20 years, we see a gradual growth of 3s being attempted per game by players. From 1 out of every 5 shots attempted being a 3-pointer in the 1999-2000 season to almost 2 in every 5 shots in the present NBA being a 3.

To some, this might not be an astronomical jump in shooting rates but it's staggering to see such a jump, especially for on-lookers of the sport who felt the shockwaves of such a change in player output with such things as points per game and Field Goal percentages.

<br>

2.2 Are Players Making These 3s?

Focusing on Field Goal (FG) percentage did this three-point boom have an effect of how well players were shooting the 3 ball?

![__results___12_0](https://github.com/user-attachments/assets/788674c9-f159-4188-a080-d53dfa58910f)

Visually we see something interesting happen with FG percentage as we do with FGA rates as both trend upward as we approach the present. Even while shooting a higher percentage of 3s NBA players maintained and kept up by making their 3s at a high level.

Looking closely we can also observe an inflection point in the 2014-2015 season, where the rate of 3-pointers made continuously goes upwards with a slight dip that then goes back up in the 2022-2023 season (which exceeds any 3-point made rates in any of the past 20 NBA seasons).

<br>

2.3 3-Point Shot by Position

Now that we see this from a top-down point of view looking at all players, what kind of effect did the 3-point shot have on each of the five positions in the NBA, each having their unique strengths and weakness when it comes to shooting the basketball.

![__results___15_1](https://github.com/user-attachments/assets/d2bf5a8c-3339-4604-94e7-d12dd4a0cdeb)

Initially, at the start of the millennia, we see the 3 positions with the most long-range shooting proficiency (see next graph) Point Guards (PG), Shooting Guards (SG), and Small Forwards (SF) maintain high rates of 3-point attempts ranging from about 20% to 30% per game. The two remaining positions, Centers (C) and Power Forwards (PF) start the millennia shooting an incredibly low rate of 3s with PFs shooting them at a rate of about 10% per game and Cs closer to 2%.

As time progresses we see not only a spike in attempts for PGs, SGs, and SFs as one would expect with players with the skill set to do so but also from PFs and Cs who historically are opposites from a shooting skills standpoint. PFs would go on to shoot 3s at a rate of past 40% per game in some seasons while Cs who would barely attempt a 3-Pointers in the early 2000s now shot them at a rate just above 20% per game.

For folks who watch NBA basketball regularly this change can be seen on the court with the last two winners of the NBA MVP award being 2 Centers (Joel Embiid and Nikola Jokic) who shot an extensive amount of 3s in each of their MVP-winning seasons and even before.

![__results___17_1](https://github.com/user-attachments/assets/1843d015-a2a8-40b6-b421-4c2dbb1dc94a)

Looking at the rate at which player was making 3s it's not surprising to see PGs, SGs, and SFs shooting at such a high rate but what's more surprising is PFs and Cs catching up with their shorter and quicker counterparts in the 3-point-making department.

2.4 Is there any team success coming from these 3s?

Using Playoff appearances by a team as our metric of success (making the playoffs signifies you are one of the top 8 teams in your respective Conference), I've illustrated the number of attempts from the 3-point range for a team that made the playoffs in that specific season and those who did not.




























































