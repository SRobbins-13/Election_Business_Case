## Business Case - Project Proposal
Samuel Robbins

#### Opportunity
The 2020 election cycle saw unprecedented political advertising spending, with nearly [$8.5 billion spent](https://www.forbes.com/sites/howardhomonoff/2020/12/08/2020-political-ad-spending-exploded-did-it-work/) across TV, radio, and digital media. Prior to the November election, more than [5 million political ads](https://www.pbs.org/newshour/show/unprecedented-spending-for-2020-political-ads) were aired on tv alone. This trend is not likely to abate, with large ad buys already influencing more [local races](https://www.ajc.com/politics/the-race-for-city-hall-may-the-ads-be-ever-in-your-favor/MOPH3Q4HI5BO5GZN2TUCAGWONQ/) across the country. Potential voters are exposed to so many ads during an election cycle, it's not enough to just have a good ad, you need to know who to show it to. Data science is a useful tool in deciding where money should be spent for the most effective voter outreach. The guiding question for this project is which cities/states have the best potential to reach voters for a reasonable cost.

##### *Client*
The client for this project is a progressive political ad company, such as [Putnam Partners](https://putnampartners.net/political-campaigns), that is looking for insights into where to direct their political ad spending. They want to reach the highest number of voters for most economical price, while staying on budget and attempting to win the most competitive seats.

##### *Impact*
The desired impact of this project is to inform decisions about where to direct ad spending in competitive races to reach potential voters by weighing factors like media market costs, average partisan swing, and number of voters. The impact hypothesis then, is that swing states/seats outside of major media markets (e.g. New York, LA, Miami) that have a higher average Democratic Party performance are the best places to direct political ad spending for greater impact. These markets will be cheaper on average and more likely to reach a winning margin of potential voters.

#### Data
##### *Data Description*
The first dataset I plan to use is precinct level voting data from both the district and county level for house races and presidential races respectively. This data is available from [MIT Election Labs](https://electionlab.mit.edu/data). The raw data contains ~1,000,000 rows of vote data, containing features like state, county name, county location, jurisdiction, major party nominees and vote totals (in counts not percentages).

The second dataset I plan to use is from the [Wesleyan Media Project](https://mediaproject.wesleyan.edu/dataaccess/), and contains data tracking "all broadcast television political advertising from the 210 media markets in the United States", including their cost, duration, tone, and ad sponsor. 

##### *Solution Path*
The proposed solution path is to take past election data and determine how the partisan swing of a district has evolved in recent elections. I will narrow the dataset down to the districts that are either trending toward the Democratic party or have been within 5 pts in the last two elections. This will allow me to focus only on the districts that are most competitive. I will then merge the voting history dataset with the media costs dataset based on a districts location. This will allow me to make a map of media costs and voting history across the US and integrate the two to determine the best locations for focused ad spending.  

##### *Criteria for Success*
The success of the project will ultimately be determined during the next election when voters make decisions after consuming the political ads. Once those results are in, success would be a higher, but not necessarily winning, number of Democratic voters than the previous election, indicating that some persuarsion was accomplished in that ad district.

##### *Assumptions and Risks*
- One major assumption of this project design is that people can be persuaded by being shown political ads. In the age of polarization that the US finds itself in, partisan identities are strongly held and those voters may not be receptive to any political ads.
- Another assumption is that people are even paying attention to political ads. Manny folks may passively observe ads without really taking them in.
- One risk in this project is that an individual ad is not viewed in a vacuum. At present, this analysis does not account for negative ads from opponents that could be playing in the same districts and media markets and can't assess how the contrasting ads are influencing the individual race until real-time polling is conducted.

##### Tools
Excel will be used for cleaning and connecting the datasets described above, and preliminary data exploration. Tableau will be used for data visualization and mapping.

##### MVP Goal
The MVP goal for this project will be a more detailed project proposal with a more developed impact hypothesis and some preliminary results about the top 10-20 competitive districts.
