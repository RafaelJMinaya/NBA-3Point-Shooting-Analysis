# NBA 3-Point Shooting Trends Analysis 🏀

## 0. Overview
The NBA has experienced numerous transformative eras since the ABA-NBA merger, each bringing revolutionary changes to the game. One of the most significant eras is the current 3-Point Revolution, which began in the mid-2010s. Over the past decade, the prominence of the 3-point shot has dramatically reshaped the game, a stark contrast to earlier decades. This study analyzes NBA game and season data from 1999–2000 to 2022–2023 regular seasons to observe 3-point shooting trends and provide a comprehensive scoring analysis focused on contemporary player shooting behaviors.

![Joel-Embiid-DESKTOP-RAFAEL](https://github.com/user-attachments/assets/1605895d-5f13-4710-a535-eb5cffe2bdee)

Key Questions:

1. When and how did the NBA 3-Point boom emerge in the past 20 years?
2. What are some common shooting habits of today's players compared to their veteran counterparts from the early 2000s?

<br>
<br>

## 1. Data Overview
For this exploration of 3-point shooting, we'll implement different NBA shooting datasets found on Kaggle. All DataFrames have been cleaned to have no missing or null values (please look into the code to see different processes applied to clean data).

**Team Statistics Dataset**:
>Mostly comprised of Field Goals made and attempt rates by teams throughout many seasons.

**Individual Player Shooting Dataset**:
>Focuses on providing player shooting rates from different distances on the court.

**Yearly Positional Shooting Datasets**:
>This collection of datasets provides positional data of every shot attempted by every player in the NBA within the specified season.

<br>
<br>

## 2. Shooting Breakdowns
2.1  **3-Pointers vs 2-Pointers**
![__results___9_1](https://github.com/user-attachments/assets/c3e712b1-2ed7-4302-bc08-6704aad2843b)

Over the past 20 years, we see a gradual growth of 3s being attempted per game by players. From 1 out of every 5 shots attempted being a 3-pointer in the 1999-2000 season to almost 2 in every 5 shots in the present NBA being a 3.

To some, this might not be an astronomical jump in shooting rates but it's staggering to see such a jump, especially for on-lookers of the sport who felt the shockwaves of such a change in player output with such things as points per game and Field Goal percentages.

<br>

2.2 **Are Players Making These 3s?**

Focusing on Field Goal (FG) percentage did this three-point boom affect how well players were shooting the 3 ball?

![__results___12_0](https://github.com/user-attachments/assets/788674c9-f159-4188-a080-d53dfa58910f)

Visually we see something interesting happen with FG percentage as we do with FGA rates as both trend upward as we approach the present. Even while shooting a higher percentage of 3s NBA players maintained and kept up by making their 3s at a high level.

Looking closely we can also observe an inflection point in the 2014-2015 season, where the rate of 3-pointers made continuously goes upwards with a slight dip that then goes back up in the 2022-2023 season (which exceeds any 3-point made rates in any of the past 20 NBA seasons).

<br>

2.3 **3-Point Shot by Position**

Now that we see this from a top-down point of view looking at all players, what kind of effect did the 3-point shot have on each of the five positions in the NBA, each having their unique strengths and weakness when it comes to shooting the basketball.

![__results___15_1](https://github.com/user-attachments/assets/d2bf5a8c-3339-4604-94e7-d12dd4a0cdeb)

Initially, at the start of the millennia, we see the 3 positions with the most long-range shooting proficiency (see next graph) Point Guards (PG), Shooting Guards (SG), and Small Forwards (SF) maintain high rates of 3-point attempts ranging from about 20% to 30% per game. The two remaining positions, Centers (C) and Power Forwards (PF) start the millennia shooting an incredibly low rate of 3s with PFs shooting them at a rate of about 10% per game and Cs closer to 2%.

As time progresses we see not only a spike in attempts for PGs, SGs, and SFs as one would expect with players with the skill set to do so but also from PFs and Cs who historically are opposites from a shooting skills standpoint. PFs would go on to shoot 3s at a rate of past 40% per game in some seasons while Cs who would barely attempt a 3-Pointers in the early 2000s now shot them at a rate just above 20% per game.

For folks who watch NBA basketball regularly this change can be seen on the court with the last two winners of the NBA MVP award being 2 Centers (Joel Embiid and Nikola Jokic) who shot an extensive amount of 3s in each of their MVP-winning seasons and even before.

![__results___17_1](https://github.com/user-attachments/assets/1843d015-a2a8-40b6-b421-4c2dbb1dc94a)

Looking at the rate at which player was making 3s it's not surprising to see PGs, SGs, and SFs shooting at such a high rate but what's more surprising is PFs and Cs catching up with their shorter and quicker counterparts in the 3-point-making department.

<br>

2.4 **Is there any team success coming from these 3s?**

Using Playoff appearances by a team as our metric of success (making the playoffs signifies you are one of the top 8 teams in your respective Conference), I've illustrated the number of attempts from the 3-point range for a team that made the playoffs in that specific season and those who did not.

![__results___20_1](https://github.com/user-attachments/assets/39b7dab4-70c6-4572-91c2-93fcaa27b7fa)

From our graph, we see playoffs-making teams continually attempted more 3s than their non-playoff-making counterparts since the beginning of the millennia (even if it's by a small margin).

<br>
<br>

## 3. Shot Mapping
3.1 **Shot Frequency**

To get a better understanding of what was happening on the court we can examine shot location data which gives us the ability to map onto a plane all shots attempted during an entire season.

>Note: Due to a majority of basketball shots happening directly under or next to the rim, a maximum cutoff for shots was established when visualizing the entire court so hexbins around the rim would not drown out other hexbins. The maximum cut-off chosen was 400 shots.

![__results___24_0](https://github.com/user-attachments/assets/921b6f76-25a5-4e37-89c5-ca633fe958e5)

From charts of the 2003-2004 season to that of the 2022-2023 season we see a gradual movement away from the mid-range shot (long 2-pointer) to an increase in 3-pointers as the years went on. Alongside the increase in 3s, there was also an increase in shots concentrating around the ring pointing to a polarity in shot selection for players; in their minds, it's either I shot a 3-Pointer or I take a more efficient/easier shot around the rim.

The death of the midrange (long 2-pointer) shot is clear to see here with the heat map showing shot regions from the 2003-04 season being brighter in the space between the 3-Point line and the key (aka the paint). That brightness/volume shot volume then slowly starts to migrate further and further.

<br>

3.2 **Shot Distance Distribution**

What interesting things can we discover if we visualize the percentage of shots taken from specific shot distances?

![__results___27_1](https://github.com/user-attachments/assets/9148f92b-ed74-4285-85eb-a669177a9d70)

Looking into the percentage of shots attempted from certain distances on the court one can see most shot rates from certain distances staying around a similar percentage range while one in particular almost being gone completely. The "16ft to 3-Point line shot (24ft)" is almost going extinct with the boom of the 3-Point shot eating away at shots that would be taken at that distance historically.

However, the mid-range shot (long 2-pointer) isn't necessarily dead as stars like Kevin Durant, Demar Derozan, and Devin Booker are still known for incorporating such a shot into their shot portfolio.

<br>

3.3 **Jokić vs Shaq**

The difference in shot selection for players is made even more evident by just looking at the shot selection of the most dominant Centers from their respective eras, Shaquille O'Neal and Nikola Jokić.

![__results___30_0](https://github.com/user-attachments/assets/a8277d28-83b7-4db0-86e0-ecfbb6b79b95)

<br>
<br>

## 4. Building A Scouting Report (Past vs Present)

Let us take a more granular look at how shooting habits have changed over time by comparing two seasons of Lebron James' career and utilizing machine learning models. Why pick Lebron James for this evaluation? He provides us with a very unique look into a player that still plays at the relatively same pace and efficiency today as he did in the early 2000s when he started his NBA career. Still averaging 25+ points per game in his 21st season he's found ways to evolve his playstyle with the times making him a perfect candidate for our comparison.

<br>

4.1 **Data Preprocessing**

![image](https://github.com/user-attachments/assets/58ecccf7-d069-4b0a-883e-14dd39a10310)

![image](https://github.com/user-attachments/assets/98724857-e146-41f1-a5d5-cfaaca2428c0)

<br>

4.2 **Model Selection and Hyperparameter Tuning**

Let's start the process of building and comparing different classification models with default parameters and then applying more complex tools to make our models more accurate.

Important note that both datasets for each season will be tested on models separately to ensure that the appropriate model is being chosen correctly for each dataset.

<br>

***2003-2004 Season Dataset: Model Analysis***

Training and Performance Metrics w/ Default Parameters

![image](https://github.com/user-attachments/assets/452ad8a5-727a-46c5-b6e8-960b717240be)

Feature Importance w/ Default Parameters

![image](https://github.com/user-attachments/assets/19c4dcfe-43b9-45b6-b0d3-ed1b9788f2be)

Confusion Matrices w/ Default Parameters

![image](https://github.com/user-attachments/assets/e249b97b-1ef4-416c-8eeb-5bd9bc403531)

Applying k-Fold Cross Validation

![image](https://github.com/user-attachments/assets/ed043841-ed1a-44d5-921e-082ad2121bd2)

Hyperparameter Tuning our Best Performing Model (Gradient Boosting)

![image](https://github.com/user-attachments/assets/c575ceb6-5ab0-4e7d-9107-caaa87137cdb)

<br>

***2022-2023 Season Dataset: Model Analysis***

Training and Performance Metrics w/ Default Parameters

![image](https://github.com/user-attachments/assets/f3b2b83d-7c86-4e18-b66d-c3b171c4c61c)

Feature Importance w/ Default Parameters

![image](https://github.com/user-attachments/assets/46195c90-fe9f-40ed-95b1-c837d8487c99)

Confusion Matrices w/ Default Parameters

![image](https://github.com/user-attachments/assets/1b8c40f3-7b7e-44b2-8c8b-f5a8b6879168)

Applying k-Fold Cross Validation

![image](https://github.com/user-attachments/assets/208a2f8d-baf0-45ad-867a-055316c9a216)

Hyperparameter Tuning our Best Performing Model (Gradient Boosting)

![image](https://github.com/user-attachments/assets/52e59739-3cbf-4e91-995e-8587d6a6f21e)


Gradient Boosted Trees is the model we'll use for both data sets as it boasts the highest Accuracy and Precision score after tuning all the classification models tested. It's important as well to point out feature importance with how Gradient Boosting and Random Forest both hold shot coordinate features 'LOC_X' and 'LOC_Y' at a much higher relevance than Logistic Regression which holds 'SHOT_DISTANCE' as the most important feature in its prediction model.

<br>

4.3 **Lebron 2004**

Starting with raw shot charts we see shots closer to the rim (specifically less than 8 ft) drown out any other shot distance LeBron is making in terms of volume.

![__results___42_1](https://github.com/user-attachments/assets/5aea06c3-1297-4820-89bc-62acc0f45d89)

![__results___42_2](https://github.com/user-attachments/assets/a197e63f-d0e2-47fa-856b-989cb9432b26)

Now using our Gradient Boosted model let's look at a kdeplot for location mapping to get a better picture of how Lebron's shooting habits and hotpots.

![__results___44_0](https://github.com/user-attachments/assets/97c762dc-a724-4953-a556-2b817bb5032d)

![__results___45_0](https://github.com/user-attachments/assets/7074d149-fa23-4fb6-93c1-a87ea40e62e3)

Coaches during and after the 2003-04 season would evaluate LeBron's shot diet as that of a strong finisher at the rim with a deadly baseline jump shot from both left and right. These findings indicate optimal defensive locations to guard LeBron due to his success in those regions.

<br>

4.4 **Lebron 2023**

Now the same for the 2022-23 season

![__results___48_1](https://github.com/user-attachments/assets/586a2bae-448e-4918-a773-cfb194f31618)

![__results___48_2](https://github.com/user-attachments/assets/c84e8ccd-9fce-4ae1-ac48-e77a1a4585d4)

We see a clear difference in Lebron's shooting habits with the distribution graph on the right showing us a higher volume of 3-Pointers (24+ft) shot by Lebron in the 2022-23 season in comparison to his rookie season in 2003-04.

![__results___50_0](https://github.com/user-attachments/assets/edcd8948-7de4-4c25-93bc-a189ec1c6ecd)

![__results___51_0](https://github.com/user-attachments/assets/22085214-7753-40c6-b477-3c89c4414589)

LeBron's evolution is very interesting to see as he still attacks the basket in his 21st season with the same tenacity as when he did in his rookie season with the biggest change coming in his willingness to shoot more 3s, especially from that top right position which is his favorite.

<br>
<br>

## 5. Conclusion

The NBA today finds itself in the middle of one of its most defining eras with the 3-point boom. With players like Stephen Curry being the poster child for this new era, the staggering effects of such a paradigm shift in the league but also in basketball as a whole have had indescribable impacts on how basketball at all levels is played, coached, and even examined. With the upward trend of NBA players attempting and making more 3-point shots from the beginning of the 21st century to the present being clear, the offensive capabilities of NBA teams (made evident with higher than-ever final point totals and player points per game) have reached levels never before seen. A change like this however doesn't come with the impact of just one player like Stephen Curry but with there being external factors or influences on and off the court which radically changed systems within the league.

Starting around the 2013-14 and 2014-2015 seasons behind the scenes the NBA was also going through another revolution in the form of the analytics boom. Teams like the Houston Rockets with offensive-minded Head Coach Mike D'Antoni and star player James Harden were the faces of this new offensive-minded movement. If one individual and their team could be labeled as leading the way behind the scenes it was Houston Rockets General Manager Daryl Morey. With his analytics-focused basketball philosophy, labeled “Moreyball,” Morey pushed for his team to concentrate on more “statistical sound” shot attempts which focused less on mid-range shots and more on 3s and shots closer to the basket.

Morey's philosophy sent shockwaves through the NBA and other teams followed suit. Using data similar to how Morey did, in this study, we showcased how vital it is for coaches, trainers, and higher-up executives within teams to find and follow important trends. Such findings can then be acted upon to make well-informed decisions to prepare for the future of not just the NBA but of all of basketball.

<br>
<br>

## 6. Acknowledgments

JP Hwang for his substack and medium articles which inspired my use of heatmaps as a visualization tool.

>https://github.com/databyjp

Bradley Fay and Savvas Tjortjoglou for providing a template for drawing NBA Courts within Python with the code in his Github.

>https://github.com/bradleyfay
>https://savvastjortjoglou.com/nba-shot-sharts.html

Thank you to Dominic Samangy for starting my interest in NBA data visualization with his incredible visuals on Twitter focusing on individual players and teams.

>https://github.com/DomSamangy

Thank you to the Kaggle members and their datasets which made this project possible (links to all of them below)

>https://www.kaggle.com/datasets/sumitrodatta/nba-aba-baa-stats

>https://www.kaggle.com/datasets/justinas/nba-players-data

>https://www.kaggle.com/datasets/nathanlauga/nba-games







