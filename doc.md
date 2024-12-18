Projet SDP

V. Mousseau, M. Tydrichova

PFITZER PROJECT

Assigning Sales representatives to a territory

Murat K¨oksalan1, Sakine Batun2

Note: The information regarding the pharmaceutical sector and the company are accurate as collected
from various cited sources. The problem contains all the characteristics of the underlying problem faced
by Pfizer. It has been simplified for the purpose of keeping the model size manageable as a case study
and the data has been altered for reasons of confidentiality. The authors created the case material based
on past collaboration with Pfizer. All the characters introduced throughout the case are fictional.

Merih Caner, the vice president of logistics, has been thinking that it is about time to renew the
It has been several years since the last update and the demand
territories of the SRs countrywide.
structure for pharmaceutical products has changed substantially. He knows that it is important to keep
the total travel distance short and it is not a good idea to make drastic changes in the existing territories.
He also knows that maintaining a somewhat balanced workload among the SRs is important. They have
always considered these issues when updating the territories and he is confident that they are still crucial.
What he is not so sure about is whether or not they could adopt a more structured approach than trial
and error to come up with satisfactory territories. He calls his assistant, Serdar Altan, to a meeting to
discuss these issues.

1 Company Background: Pfizer Global
Pfizer Inc, founded in 1849 in Brooklyn-NY, aims to help people and animals live longer and healthier
lives. To attain this goal, the company “discovers and develops breakthrough medicines; provides infor-
mation on prevention, wellness, and treatment; and carries out high-quality manufacturing of medicines.”
Pfizer employs approximately 81,800 people worldwide. The company operates in over 150 countries, re-
flecting its influence and scale in the global pharmaceutical industry. More precisely, Pfizer has employees
in 60 countries, and the medicines developed and manufactured by the company are marketed/sold in
more than 150 countries.

Pfizer’s 2023 revenue is estimated at $58 billion to $61 billion. That’s down from the prior year, pri-
marily due to lower revenue from COVID-19 products, such as the Comirnaty vaccine and the Paxlovid
antiviral treatment. However, non-COVID products posted 6% to 8% operating growth driven by several
new launches and strategic acquisitions.

1Middle East Technical University Department

of

Industrial Engineering Ankara,

06531,

Turkey

koksalan@ie.metu.edu.tr

2University of Pittsburgh, Department of Industrial Engineering 1048 Benedum Hall, Pittsburgh, PA, 15261, USA,

sab79@pitt.edu

Pfizer invested approximately $10.7 billion in research and development (R&D) in 2023. This signifi-
cant investment highlights the company’s commitment to advancing its pipeline of medicines and vaccines,
including those beyond its COVID-19 portfolio. Additionally, Pfizer pursued strategic acquisitions, in-
cluding the $43 billion purchase of Seagen, aimed at bolstering its cancer treatment capabilities.

2 The Pharmaceutical Sector in Turkey

The emergence of pharmaceutical companies in Turkey dates back to the early nineteen hundreds. Large-
scale manufacturing started around 1923, and the manufacturing of pharmaceuticals shifted from drug-
stores to laboratories and small plants after 1928. Especially in the last 40 years, investments by foreign
companies have increased substantially because of Turkey’s proximity to the European market and its
qualified workforce.

The pharmaceutical industry in Turkey holds a significant position as an emerging market globally.
It is ranked as the 16th largest pharmaceutical market globally and the 6th largest in Europe, reflecting
its growing influence. The Turkish pharmaceutical market is characterized by its focus on generic drugs
and local production. Still, it also serves as a regional hub for multinational companies (Pfizer, but also
Sanofi, and Bayer. These companies often base their regional operations and R&D centers in Turkey,
taking advantage of the country’s strategic geographic location.

The annual sales of top pharmaceutical companies in Turkey, including Pfizer, indicate a highly com-
In 2023, Abdi ˙Ibrahim led with significant revenue, followed by global players like
petitive market.
Novartis and Pfizer. Pfizer’s sales in Turkey were estimated at approximately $250 million in 2023, con-
tributing to the company’s robust presence in the region. Overall, the Turkish pharmaceutical market
reached around $21.3 billion in 2023, showing steady growth. Figure 1 shows annual sales in 2022 and
2023 of the top pharmaceutical companies in Turkey.

Figure 1: annual sales in 2022 and 2023 of the top pharmaceutical companies in Turkey

2

3 Pfizer Turkey

As a part of Pfizer’s global expansion, Pfizer Turkey was founded in Istanbul in 1957. Despite initially hav-
ing a small plant designed to manufacture a few products, Pfizer Turkey expanded its capacity gradually
to satisfy the increasing demand. In 2023, Turkish pharmaceutical exports reached approximately $2.23
billion, showcasing the sector’s growth potential and strategic importance within the national economy.
Pfitzer Turkey had 7% of Turkey’s pharmaceutical exports. According to the activity reports of 2024,
the exports are increasing. Together with the imported products, Pfizer Turkey supplied 121 different
products with 356 different presentations, amounting to 144 million boxes of supply volume.

4 Assigning Regions to Sales Representatives

Pfizer Turkey’s immediate customers are medical doctors (MDs) since a vast majority of its products
are prescription drugs. Pharmaceutical sales representatives (SRs) of Pfizer regularly visit MDs. They
provide information such as indications and adverse effects of drugs, supply samples, discuss and obtain
feedback, and keep a close relationship with the MDs. There is strong evidence that this strategy helps
the sales of Pfizer’s products.

Each SR is assigned a working region, called a “sales territory” or simply a “territory,” which is a list
of MDs to be visited by him/her. Territories are formed by combining smaller geographical units, called
“bricks.” A brick is the smallest geographical region for which relevant information, such as sales data,
number of MDs, and MD profiles is available. Based on this information, Pfizer calculates an index value
for each brick. The index value is a composite figure developed at Pfizer that captures various factors
to show the workload of the brick in terms of the number of SRs required to work there. Typically, the
index value is less than one and a territory is composed of several bricks.

Each SR is located in an office at a certain brick. This brick is considered as the center of his/her
territory. The sum of index values of the bricks of an SR corresponds to his/her total workload and it
should be approximately 1. Naturally, it is not possible to achieve a workload of exactly 1 unit to each
SR as partial assignments of bricks to multiple SRs are undesirable.

In order to maintain overall travel efficiency, it is necessary to minimize the total distance traveled
by the SRs. The total distance traveled by an SR (within his/her territory) can be measured by the sum
of distances between the office (i.e., the center brick) and the (centers of the) bricks assigned to it as
demonstrated in Figure 2.

Figure 2: Territory of an SR

3

Due to the dynamic structure of the market, i.e., changes in number of customers or changes in the
sales of products in each brick, the index values change over time. Hence, sales territories should be
periodically reconstructed in order to maintain workload balance between territories. Another concern,
minimizing disruption, emerges at this point due to changing some of the existing territories and re-
constructing new ones. Disruption is defined as the inclusion of new bricks in the territories of SRs.
Disruption is undesirable as some of the established relationships between SRs and MDs cannot be uti-
lized anymore.

Serdar Altan has an M.B.A. degree and Merih Caner has a lot of confidence in his skills. Merih asked
him to bring Sevil Korkmaz along to the meeting as well. Sevil has an M.S. degree in Industrial Engineer-
ing. Serdar and Sevil recently completed a production-planning project and earned a good reputation in
the company despite their youth. Merih thinks that this is a good time to get them involved and start
the reorganization study of the territories.

Merih: You know the territories of our SRs were determined several years ago. Things have changed
quite a lot since then and we should be able to improve this. The variation between the workloads of
SRs seems to have increased a lot and I hear that some SRs are already complaining. I am not sure we
are doing the best we can do in terms of total travel distance either. We should be able to measure and
improve these as much as possible without creating too much disruption. I believe the timing is just right
to make some changes. In the past, we have done this with trial and error but I have always felt that
there should be a better way.

Sevil : I have also been thinking about this. It resembles a problem we have seen in our M.S. pro-
gram. We need to assign each brick to an SR and each SR has a work capacity. We can try to define a
mathematical model.

Serdar : Yes, I am also familiar with such models. I am not sure what our objective will be though.
We have different concerns. We need to consider the travel distance and make sure not to reassign too
many bricks.

Merih: You also need to make sure that there is a reasonable balance of workload among SRs. Oth-
erwise, they will all blame us. But it seems you have some ideas, why don’t you work on those a bit. Let
us schedule another meeting, would two days be enough to develop those ideas?

Serdar : We will do our best.

Sevil and Serdar were a bit worried after the meeting. Merih always expects quick results. On the
other hand, he has a good intuition on these matters and they knew that he would be very supportive
in case they had difficulties. They first collected the documents and studied the current situation. There
were 1000 bricks and 196 SRs nationwide. Looking at the overall workload and the trends, they knew
that there was no need for new SRs in the near future. They quickly realized that the model would have
too many binary variables to be of practical value. They remembered that large integer models would
cause computational difficulties and specialized software exploiting special structures could be necessary.
They started further analyzing the current system on the map.

Serdar : Doesn’t this problem have a special structure that would give integer results when solved as

a linear program? We should be able to solve the large problem without difficulty then.

Sevil : I also thought about it and looked it up. Our problem resembles the “assignment problem”
which has the structure you mentioned. But I think our different objectives will destroy this structure.

4

In order to see the trade-offs between the objectives and to obtain different solutions, we will have to
introduce additional constraints to the problem. My experience is that such constraints usually cause
problems. In any case, once we set up an example problem, we can solve the LP relaxation and see what
happens.

Serdar : Okay. Even if it does not give an integer solution, I find the LP relaxation very useful. It

yields a lot of insight.

Sevil : I agree. To reduce the problem size, we may perhaps use the geographical districts. It seems
that there are very few common aspects between districts. The problem seems to be naturally separable.

Serdar : Great! Then we would need to solve many small problems. If there are neighboring districts

for which this separation is not so clear, we can combine and solve them together.

They decided to take an example district and try to get some results before the meeting with Merih.
They chose a typical district of Istanbul having 4 SRs and 22 bricks. Table 1 shows the current structure
of the sales territories, i.e., the center brick of each SR and the bricks assigned to him/her. Tables 2
and 3 provide new index values of the bricks and the travel distances between these bricks and SR offices
(center bricks), respectively. Note that the index values over all bricks sum up to 4; this means that a
standard full-time job corresponds to a workload equal to 1. Figure 3 shows the brick locations.

SR Center brick
1
2
3
4

4
14
16
22

Assigned bricks
4, 5, 6, 7, 8, 15
10, 11, 12, 13, 14
9, 16, 17, 18
1, 2, 3, 19, 20, 21, 22

Table 1: Current Structure of Sales Territories

brick
1
2
3
4
5
6
7
8
9
10
11

index value
0.1609
0.1164
0.1026
0.1516
0.0939
0.1320
0.0687
0.0930
0.2116
0.2529
0.0868

brick
12
13
14
15
16
17
18
19
20
21
22

index value
0.0828
0.0975
0.8177
0.4115
0.3795
0.0710
0.0427
0.1043
0.0997
0.1698
0.2531

Table 2: Index values (workload) of bricks

Sevil and Serdar decided to treat the workload balance objective as a constraint. They also decided
to try to restrict the workload of each SR to the interval [0.8, 1.2] because they believed this level of
variation would be acceptable.

5

brick
1
2
3
4
5
6
7
8
9
10
11
12
13
14
15
16
17
18
19
20
21
22

1
16.16
19.00
25.29
0.00
3.07
1.22
2.80
2.87
3.80
12.35
11.11
21.99
8.82
7.93
9.34
8.31
7.31
7.55
11.13
17.49
11.03
36.12

SR

2
24.08
26.47
32.49
7.93
6.44
7.51
10.31
5.07
8.01
4.52
3.48
22.02
3.30
0.00
2.25
2.07
2.44
0.75
18.41
23.44
18.93
43.75

3
24.32
27.24
33.42
8.31
7.56
8.19
10.95
5.67
7.41
4.35
2.97
24.07
5.36
2.07
1.11
0.00
1.11
1.53
19.26
24.76
19.28
44.43

4
21.12
17.33
12.25
36.12
37.37
36.29
33.50
38.80
38.16
48.27
47.14
39.86
43.31
43.75
45.43
44.43
43.43
43.52
25.40
23.21
25.43
0.00

Table 3: Travel distances between SR offices and bricks (km)

Sevil : How do we measure the travel distance and the reassignment objectives? The travel distance
objective would be straightforward if an SR returned to the office after visiting each brick. I suppose
this is not a bad assumption. I believe this would not change the solutions much. If we try to incor-
porate the sequence of visiting the bricks into this problem, I am afraid it will be too complicated to solve.

Serdar : I agree. The additional benefit will also be marginal. To measure the disruption, couldn’t
we just count the number of bricks for which the new assignment is different from the current assignment?

Sevil : Wouldn’t we be counting them twice then? Assigning a brick to a new SR means removing it
from another SR’s territory. So, it may be more meaningful to count either the number of bricks assigned
to a different SR, or the number of bricks removed from an SR’s current territory.

Serdar : Yes, you’re right. We should be careful about it. When we just count, we are treating all
the bricks the same way. It is actually less desirable to disrupt a brick having a higher index value. New
relationships will have to be established between more MDs.

Sevil : Yes, that’s a good point. Why don’t we use the index values of bricks while measuring the
disruption? Would weighing each disrupted brick with its index value be a good metric to measure the
disruption?

Serdar: It surely would.

6

Figure 3: Brick Locations

They then discussed how to obtain different solutions. They checked their books and noted the def-
inition that “a solution is efficient if there is no other feasible solution that is at least as good in every
objective and strictly better in at least one objective.” They recalled from their graduate studies that
they had to make sure to obtain efficient solutions. They decided to use a method that would put an
upper bound on the disruption objective and minimize the distance traveled. By changing the upper
bound value, they would obtain several solutions.

Serdar : When we use this method, are we guaranteed to obtain an efficient solution? The second
objective is treated as a constraint and it seems to me that the model would not differentiate between
solutions that have the same minimum distance traveled but different disruption values so long as the
upper bound is satisfied.

Sevil : Exactly. The book discusses this issue right here. It says the solution found can be inefficient
because of this. But there is a practical solution. We can multiply the second objective’s value with a
very small positive constant and add to the distance traveled in the objective function. This trick breaks
ties in favor of solutions with better values in the “disruption” objective.

Serdar : I like this trick. Okay, we have very little time left before the meeting. It would be great if

we could obtain some solutions we can show to Merih.

They were able to obtain several efficient solutions and they were pleasantly surprised to see how
much they accomplished in two days. They explained what they did and showed their results to Merih.

Merih: These look good for a start. It gives me some idea about the possible solutions. Before making
a decision, I would like to see more solutions though. Would it make sense to obtain all efficient solutions?

7

Would they be too many?

Sevil : I think they could be too many in general. There may not be too many for this problem,

though. We can try and see.

Merih: I am also interested to see the effect of tightening the “balance” range. If the other objectives
do not deteriorate too much, I would like to have the workload balanced a little more. Perhaps you can
plot the solutions you obtain. I will also welcome any comments on the solutions that would facilitate
the decision. If we can analyze this district well, then we can make the decisions for other districts in a
similar way.

Serdar : We intended to prepare a plot but ran out of time. We will do it next time. Hopefully, we

will not be pressed with time as much now!

Merih: I understand. I will not give you a deadline this time. You let me know when you are ready.
Leaving the meeting, Sevil and Serdar were not sure if they were better off with or without the
deadline. They knew that they would work even harder now. It just occurred to them that Merih also
knew it. “No wonder he is the vice president.” Sevil thought.

8

Project organization

• The project is to be realized in groups of three students. the composition of the group should be

specified here before 18/12/2024, 17h.

• Two 3h sessions (18/12/2024 and 21/01/2025) are programmed during the course to work on the

project (the project will, however, require additional work).

• The project: the report + code, and data files used are to be posted on Edunao by February 2nd,

23:59.

• The defense will take place on February 4th, 2025. Each group will have 20mn (12 mn presentation
+ 8mn questions). All group members should be present and participate actively in the defense.

The work consists of three steps:

Step 1 (18/12/2024)

In this first step, we consider the center bricks as fixed. You should:

• formulate two mono-objective linear optimization models to solve the assignment problem using a

distance and a disruption objective,

• implement your two mono-objective models using GUROBI, and solve the instance with 22 Bricks

and 4 Sales Representatives,

• implement the epsilon-constraint scheme to compute the set of all non-dominated solutions,

• compute and represent the corresponding sets of non-dominated solutions for the 4x22 problem,

with interval workload constraints [0.8, 1.2], [0.85, 1.15], and [0.9, 1.1],

• check how your model scales up with the instance with 10 SRs and 100 zones.

• propose a visual representation of the solution in the decision space,

• your work for step 1 should be posted on Edunao before 18/12/2024, 18h.

Step 2

In this second step, we will consider extensions of the model developed in Step 1.

• Is your first model able to solve the 100 bricks / 10 SRs instances? compute and represent the

corresponding sets of non-dominated solutions.

• How to model the case for partially assigning bricks (i.e., assign a brick to multiple SRs?). Implement

this possibility and compare the results to your previous results.

• If the demand increases uniformly in all bricks (for example + 25%, it will be necessary to hire a
new sales representative. There is the question of where to locate his/her office (center brick).

9

Step 3

The location of the “center bricks” (SR offices) has a significant impact on the distance traveled by the
sales representatives. An important question is to generalize the model to allow a modification of the
“center bricks”.

• Formulate a bi-objective optimization problem in which positions of offices are variables and in

which the two objectives are the total distance (min), and the workload of SRs (MinMax),

• In this context of possibly modified center bricks, the disruption is redefined in terms of the number
of relocated offices (without any consideration of the changes in the assignment of bricks to SRs). As
this new disruption formulation (number of relocated offices) takes integer values in [0, number of
SRs], compute the sets of non-dominated solutions for the three-objective problem (total distance,
workload fairness, and number of relocated offices).

Step 4

In the first three steps, the question tackled relates to the computation of non-dominated solutions for
the assignment (or assignment-relocation) problem. The choice of a specific solution in the set of non-
dominated solutions is yet to be made. In this third step, you are asked to develop an additive preference
model (using the UTA method) to support the choice among solutions for the three criteria problem (total
distance, workload fairness, and number of relocated offices). To simulate the preferences of the decision
maker used as input in the UTA method, you will randomly generate and use a piecewise linear additive
model.

10


