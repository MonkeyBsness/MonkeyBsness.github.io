# Echoes on the Hardwood: Unlocking the Stories Behind the NBA’s Greatest Numbers
<figure>
  <img src="/images/NBA_logo.png"  style="width:100%">
</figure>

Basketball is a game of poetry in motion. It’s the squeak of sneakers on polished hardwood, the roar of a playoff crowd, and the impossible arc of a buzzer-beater. But underneath the highlight reels and the legendary moments lies a quiet, unblinking witness to history: the box score.

Before diving into the grand narratives, I had to do some housekeeping. Combining through decades of data requires filtering out the noise. I spent time cleaning the archives, removing players who only played a handful of games to avoid skewed averages, and identifying missing data from the 1960s and 70s (an era before turnovers, blocks, and three-pointers were officially tracked). Profiling this data gave me a clear picture: we have a pristine record of modern basketball, alongside a fragmented but beautiful portrait of the game's pioneers.

___

## Efficiency vs. Volume
>*Is there a correlation between high scoring volume and overall scoring efficiency among the top 100 all-time scorers?*

### The Process
To answer this, I looked exclusively at the NBA’s VIP lounge: the top 100 all-time leading scorers. These are the players who have carried franchises on their backs. But I wanted to know how they got their points. Did they just shoot the ball every time down the court, or were they mathematical savants? I mapped their total career points against their True Shooting PercentSage, a metric that combines two-pointers, three-pointers, and free throws to give a true reflection of a player's scoring efficiency.
### The Findings
The common myth in basketball is that if you shoot more, your efficiency drops. The "volume chucker" is a known trope. However, the data tells a breathtakingly different story about the all-time greats.

Among the top 100 scorers, the correlation between scoring more points and losing efficiency is virtually non-existent. In fact, the players at the absolute peak of the scoring mountain, names like LeBron James and Kevin Durant, boast True Shooting Percentages well above the league average (often hovering around 55% to 60%+).

There is one striking anomaly: Stephen Curry. When you look at the visualization, Curry sits on an island. He has the volume of a primary scorer but the efficiency (over 62%) of a 7-foot center who only dunks. The data proves that the greatest scorers don't just take more shots; they take better shots. Conversely, some players from the early 2000s "hero ball" era rank high in volume but noticeably lower in efficiency, a reflection of the grueling, isolation-heavy style of their time.



<figure>
  <img src="/images/v1.png"  style="width:100%">
  <figcaption style="font-size: 12px; color: gray; text-align: center;">A scatter plot where the X-axis is Total Career Points and the Y-axis is True Shooting Percentage. Each dot represents a player.</figcaption>
</figure>

<figure>
  <img src="/images/v2.png"  style="width:100%">
  <figcaption style="font-size: 12px; color: gray; text-align: center;">A bar chart showing the True Shooting Percentage of 1980s/1990s big men alongside 2000s isolation guards.</figcaption>
</figure>


___

## The Impact of the 3-Point Era
>*How drastically does the average points per game differ between players who have recorded 3-point statistics versus those from the pre-3-point era?*

### The Process
The three-point line was introduced to the NBA in 1979. Before that, the game was a brutal, bruising battle for the paint. To understand how this single painted line on the floor changed the sport, I split our history book in half. I separated the players who had "null" or zero data in the 3-point attempt column (the pioneers of the 50s, 60s, and 70s) from the players who actively recorded 3-point stats. I then calculated the average points per game across both eras.
### The Findings
You might expect that the modern era, with its barrage of three-pointers, would feature drastically higher individual scoring averages across the board. The reality is far more nuanced.

While the ceiling for average role players has risen in the 3-point era, the pre-3-point era featured statistical titans who warped the averages. Players were scoring 30 to 50 points a game without a three-point line, driving the pre-1979 averages up.

However, when we look at the median player, the average guy on the roster, the 3-point era shows a noticeable bump in per-game scoring. The floor is spaced out. In the 1960s, if you weren't a dominant big man or a lightning-fast guard, points were hard to come by. Today, a role player whose only job is to stand in the corner and shoot threes can comfortably average 10-12 points per game. The three-point line didn't necessarily create better superstar scorers, but it democratized scoring, allowing the entire roster to get in on the action.

<figure>
  <img src="/images/v3.png"  style="width:100%">
  <figcaption style="font-size: 12px; color: gray; text-align: center;">A side-by-side box plot comparing the distribution of Points Per Game for the Pre-3-Point Era vs. the Modern Era.</figcaption>
</figure>

___

## Playmaking vs. Scoring
>*Among the top 500 players in total assists, what is the ratio of Assists to Turnovers, and does elite playmaking negatively correlate with elite scoring?*

### The Process
Point guards are the conductors of the NBA orchestra. But a good pass is only as valuable as the possession itself. To measure a playmaker's true worth, I looked at the top 500 assist leaders in NBA history and calculated their Assist-to-Turnover ratio (how many good passes they make for every mistake). Then, I cross-referenced this ratio with their total career points to see if the ultimate passers had to sacrifice their own scoring to get their teammates involved.
### The Findings
There is a profound philosophical divide in NBA history, beautifully illustrated by this data.

On one side, we have the "Pure Point Guards", men like John Stockton and Steve Nash. These players possess an almost supernatural Assist-to-Turnover ratio (often 3-to-1 or 4-to-1). They rarely make mistakes. However, their total career points, while respectable, are capped. They viewed themselves as facilitators first.

On the other side, we have the "Combo Guards", players like James Harden, Russell Westbrook, and even LeBron James (a forward playing as a maestro). Their assist totals are astronomically high, but their turnovers are equally staggering, resulting in a much lower AST/TOV ratio (closer to 2-to-1 or even 1.5-to-1). Why? Because they hold the ball constantly and take immense risks.

The data answers our question clearly: Yes, surgical, mistake-free playmaking almost always negatively correlates with elite scoring volume. The players who score 30,000 points while racking up 10,000 assists do so through sheer, overwhelming usage rates, accepting high turnovers as the cost of doing business. The tidy, flawless floor general is rarely the man leading the league in scoring.

<figure>
  <img src="/images/v4.png"  style="width:100%">
  <figcaption style="font-size: 12px; color: gray; text-align: center;">A bubble chart where the X-axis is Career Points and the Y-axis is Career Assists. The size of the bubble represents the player's Assist-to-Turnover Ratio.</figcaption>
</figure>

___

## Free Throw Reliance
>*For the top 50 all-time leading scorers, what percentage of their total career points comes directly from free throws, and who relies on the charity stripe the most?*

### The Process
We celebrate the slam dunks and the deep threes, but championships are often won when the clock is stopped and a player is standing alone 15 feet from the basket. I wanted to know who built their legendary point totals at the charity stripe. Taking our top 50 all-time scorers, I took their total Free Throws Made and divided it by their total Points to find the percentage of their career scoring that came entirely from free throws.
### The Findings
This was perhaps the most eye-opening discovery of the entire dataset. When we think of the NBA's greatest scorers, we picture unstoppable moves: Kareem's skyhook, Jordan's fadeaway, Curry's jumper. But the numbers reveal that for a specific breed of superstar, getting fouled was their deadliest weapon.

On average, a top-50 scorer gets about 18-20% of their career points from the free-throw line. But the extremes are fascinating. James Harden and Karl Malone are the undisputed kings of the whistle. Nearly 30% of Harden's career points come from free throws. His signature step-back three isn't just a shot; it's bait for defenders to foul him. Similarly, Karl Malone used his immense physical strength to draw contact in the paint relentlessly in the 1990s.

Contrast this with a player like Kareem Abdul-Jabbar. The NBA's former all-time leading scorer has one of the lowest free-throw reliance percentages in the top 50 (around 16%). His skyhook was so unblockable that defenders couldn't even get close enough to foul him.

The data tells us a gritty truth: you don't score 25,000 points in the NBA just by being a great shooter. You get there by understanding the rules of the game, embracing physical contact, and making the opponent pay when the clock stops.

<figure>
  <img src="/images/v5.png"  style="width:100%">
  <figcaption style="font-size: 12px; color: gray; text-align: center;">A bar chart listing a selection of the top 50 scorers. The bars represent total career points, but they are visually split into two distinct colors: one representing points from field goals, and a highlighted section representing points from free throws.</figcaption>
</figure>

___

## The Final Buzzer
Numbers alone are just ink on a page. But when we ask the right questions, data can transform into a historical text. We learn that Stephen Curry broke the math of the sport. We learn that the three-point line lifted up the average player, but couldn't outshine the sheer dominance of the 1960s superstars. We see the sacrifice of the pure point guard, and we respect the bruises earned by the kings of the free-throw line.

The next time you watch a game, look past the final score. Look at the efficiency, the turnovers, the free throws. Because that is where the real story of basketball is written.

___

***Reference:***
https://www.nba.com/stats/alltime-leaders?StatCategory=PTS