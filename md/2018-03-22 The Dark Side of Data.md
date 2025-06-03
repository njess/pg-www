https://hackernoon.com/the-dark-side-of-data-confessions-of-a-former-data-hitman-60da81123306

# The Dark Side of Data (Confessions of a Former Data Hitman)

![image](https://hackernoon.imgix.net/hn-images/1*TLEvQimDABAg502vFcWCcw.png?auto=format&fit=max&w=1920)

Every few minutes, Michael (names have been changed) heard his office mate’s computer let out of a soft “beep.” He and Trey had stayed late at the office after dinner to see if they could build a detection model — taking in all the data they had: locations, times, correspondence.

Every unassuming beep represented something far more sinister: detection of one of the company’s users cheating on their spouse.

Satisfied with their work, they parted ways for the weekend. But by Monday, this little experiment had to be shut down: with more training data, the beeps had become more and more frequent — until they became so numerous that the beeps had become a constant droning tone.

This was more than a decade ago at one of the tech giants. Welcome to the dark side of data.

I’ve held off on writing about this topic for some time — an equal mix of personal discomfort and professional involvement in the space. I spent nearly two years in the underworld of data brokers, creators, and the most shrewd operators (in a former life, with a lot more parties and yachts than my current humble hustle).

What has surfaced this month is just the tip of the iceberg of what’s already happening with millions of users (including your very own) data, right now. Earlier this week, a former Facebook employee  [publicly stated](https://amp.theguardian.com/news/2018/mar/20/facebook-data-cambridge-analytica-sandy-parakilas?CMP=share_btn_tw&__twitter_impression=true&ref=hackernoon.com)  that “a majority of Facebook users” could have had their data harvested by app developers without their knowledge.

Facebook has touched the third rail like no company before — none of the many data vendors have had the triumvirate of I) swaying a major election, II) with customer data they owned and shared, that III) generated them profit when third-parties purchased media on their platform using said data.

What I will say before going further — most of the uses for data start out from a good place. But with great power comes great responsibility — and often, the lines get blurry quickly.

It seems innocuous to help a restaurant find their existing customers and get them to come back more frequently. It starts simply with your corner family Italian restaurant. But somehow it begins to feel different when the same tactics are deployed by one of the largest fast food companies driving the obesity epidemic in the country. But who are we to say they shouldn’t target people who can scarcely find a filling meal for the same price?

Lots of shades of grey…which leaves the door ajar for a simply breathtaking amount of entrepreneurial activity.

### **Spies & Data Brokers**

To get a good view of how the customer data business evolved, it’s best we look to the very start. Dun & Bradstreet, today a $4.5B publicly traded company, provides commercial data and insights. It didn’t start that way. Instead, the founder built a giant ledger chronicling the life, family, and habits of every man in the trade industry. What better way to decide whether to give a man credit but to know where he goes to church and how much he drinks when he is at the bar? The credit bureaus  [were the NSA of the 19th century](https://www.theatlantic.com/technology/archive/2016/04/mass-surveillance-was-invented-by-credit-bureaus/479226/?ref=hackernoon.com).

Eventually, decisions of credit became more regulated. But the entrepreneurial activity abounded. One didn’t have to know a lot about people to have valuable signal: early mail order companies (and hucksters) would share their lists of buyers (and suckers).

The problem of course is that data is zero marginal cost. Once I’ve purchased your list of customers (for a dubious product), I can easily resell this list to others. A few steps away from the actual customer relationship, data feels very indirect and people will happily buy, sell, and model away.

Early commercial relationships had some safeguards — rather than sell you my customer list, I would simply rent it. (E.g. only allowing one catalogue to be sent per quarter this year.)

But how do I enforce these contract terms? In the physical world, I can embed “honeypots” on that list — specific people and addresses that shouldn’t receive mail from anyone else. If I get your catalogue after our agreement (or mail from other vendors), I know you’ve violated the terms of our agreement.

Unfortunately, digital complexity has made these kinds of arrangements so much harder to manage. If you give me your list of customers — just for one mailing — there’s no way you can prove if I’ve converted these addresses into email addresses or cookies (or Facebook custom audiences) and continue to market to these customers well after the term of our arrangement. There’s simply too much surface area.

From this increased surface area enables the darker side of data to emerge.

### **Sin #1: Leakage**

There are countless ways data can wind up in the wrong hands — perhaps your Facebook friend auth’ed an application that violated Facebook’s terms of service (Cambridge Analytica case). Or, worse, Equifax collects data about you that you cannot prevent them from doing — and their own ineptitude causes those records to be sold to the highest bidder, who certainly doesn’t have your best interests in mind.

Other cases are less acute and noticeable: every website you visit with ads is broadcasting your presence (and a host of other information) to every corner of the ad ecosystem, where countless players quietly listen, sell their aggregated log data, and let your data slip into unknown-to-you hands. Use an ad blocker and feel protected? Your TV may still  [be reporting everything you watch](https://www.washingtonpost.com/news/the-switch/wp/2017/02/06/these-smart-tvs-were-apparently-spying-on-their-owners/?utm_term=.5ff8b2b42f04&ref=hackernoon.com)  (and say) back to its masters.

Want to see just how far simple information spreads? Just ask a California resident, who  [under state civil code](https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?sectionNum=1798.83.&lawCode=CIV&ref=hackernoon.com)  can request information on all third parties who have received their information. One errant purchase can you have your personal information copied to dozens of data aggregators — and these are only the ones playing by the rules.

Other datasets move seamlessly. Do you know all the companies that your mobile provider licenses your location to? Scattered across dozens of nameless companies — most who probably don’t have strong information protection and employee access control like a Google might. It may be anonymized, but not for long.

### **Sin #2: Aggregation & De-Anonymizing**

We can all do our best to protect our individual information. But all it is takes a small bit of data about someone to deanonymize them out of an aggregated dataset (which we cannot control). If you have access to just one or two snippets of innocuous information about me, you can quickly connect many splinters of data, tying different ids together to create a profile. For example, if you looked at an anonymized set of browsing data (easily obtainable from your favorite ISP) and knew my zip code, you could easily find me. Who else looked at the civil state code link above today from my zip code? A state-level actor could, of course, find out this and far far more. But we’re not even talking about anyone so well equipped.

Where this takes an even more disquieting turn: protected areas. As a simple example: it’s not legal to make credit decisions based on race. But it’s entirely possible to mix available datasets together to build a model that is certainly correlated with race (and only target ads offering credit to those groups). Without auditors pulling apart the internals of a machine learning model, this remains hidden.

Worse still, medical data can be used in the mix as well — while one can’t share  [HIPAA](https://www.hhs.gov/hipaa/for-professionals/security/laws-regulations/index.html?ref=hackernoon.com)  protected data, it’s not hard to train a ‘model’ that gives propensity for diabetes or similar for any given piece of personally identifiable information (PII).

Often, the offenses aren’t so indirect. Facebook itself has been  [accused of letting landlords discriminate by race](https://gizmodo.com/facebook-still-lets-landlords-discriminate-by-race-and-1820650849?ref=hackernoon.com)  in apartment ads.

### **Sin #3: Psychographic Profiling**

Most people don’t mind being marketed to. Most people don’t mind if the marketing is more relevant than not. Where things become troubling is when relevant becomes perverse; when the pitch feels so tailored to an individual’s psyche that it is coercive. With data leakage, aggregation and some creativity, it becomes easy to find data deployed in ways that just make us uncomfortable and uneasy — and craft a message to hit someone most effectively based on their opinions, attitudes, interests, and lifestyle.

It’s already been 5 years since New York Times’  [massive story on personalization](http://www.nytimes.com/2012/02/19/magazine/shopping-habits.html?ref=hackernoon.com) — targeting a teenage mom with baby gear before her family knew she was pregnant. But this case is pretty elementary — it’s just based on an observable fact about a customer. What if advertisers knew your innermost psyche and what made you tick?

Some sites exist that predict how to best sell to an individual  [purely from data on their public Linkedin profile](https://www.crystalknows.com/?ref=hackernoon.com). Beyond our own internal biases — we are social creatures. Companies (aggregating and de-anonymizing data) will sell mappings of which of your friends (or celebrities you follow) are most likely to change your mind on any given topic.

Imagine opening the newspaper, and rather than reading an article for your town, you are reading an article specifically tailored to cause you anger. This is a weapon when deployed at scale. Think we’ve reached peak ad personalization? Wait until you see an ad where you are the protagonist flaunting the product. (Mirror AI, a  [recent graduate](https://techcrunch.com/2018/03/20/these-are-the-64-startups-unveiled-at-y-combinator-w18-demo-day-2/?ref=hackernoon.com)  of this week’s Y Combinator batch, is building easy emoji generators to do this.)

Having seen the ugly underbelly of this industry (which, it is worth noting, is full of mostly very good actors with the best intentions), I am glad to see our collective consciousness awakening to questions of how and where our personal data is being used, and for what purposes. Sunshine is the best disinfectant.