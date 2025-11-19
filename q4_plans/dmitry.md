SaaS VP of CO – OKRs (Q4 2025)
Objective
Key Results
Status/Metrics
Objective 1: 
Execute $3.1M PA CR for Khoros
Deliver $3.1M PA cost reduction (CR).

Execute via 3 kanbans ($1M per kanban) as planned by David S.

All approved CO tickets executed in a timely manner.

Zero CO-related production outages.
Target: $3.1M reduction.


SLA adherence on CO tickets.


Outage count = 0.
Objective 2: 
Execute $500k PA CR for Rest of ESW


Deliver $500k PA cost reduction for ESW portfolio. Preliminary targets

Use 1 kanban slot for execution.

Seed kanban with high-quality hypotheses actionable within the quarter.

Zero CO-related production outages.
Target: $500k reduction driven both by kanban and cost anomaly detection.


Hypothesis → actionability conversion tracked.


SLA adherence on CO tickets.


Outage count = 0.
Objective 3: 
Build AI-Driven Cost Anomaly Analysis Process
Automatic pipeline receives AWS Cost Anomaly alerts.


AI agent enriches anomalies with Cost Explorer/CloudWatch data.


Report automatically generated and delivered to account owner & SaaS DRI.


Known noise (usage tiers, amortization gaps) excluded from reporting.
% anomalies successfully processed and delivered to account owners

% of anomalies remediated within the quarter

Cost savings $$ PA



Objective 4: 
Build AI Runbooks for Health Checks After CO Changes
Runbooks cover at least 60% of CO tickets.


Automatically pull resource metadata (name, region, etc.) from GitHub issue.


Use ReadOnly AWS IAM role to collect environment data.


Automatically publish runbook output as a GitHub issue comment.
Coverage % of CO tickets.

% automation of metadata collection.
Objective 5:
Streamline Cost Reporting
There is a Spec that documents decisions around
amortization of upfront reservations and AWS marketplace yearly contracts
separate tracking of AI, EY and Wine Cellar costs.

There is a script that implements these decisions and automatically produces sheets such as Unblended - Q325-W8- AWS Actual vs Budget  Weekly Report 24 Aug 2025 and ESW Weekly AWS Budget (auto-updated) [Prod]




Supporting Data (DOK1/2)
Cost Amortization
Time-Based Amortization
Costs like Marketplace contracts and reservation upfront fees should be spread over 1 or 3 years. If not, they distort the lookback window -- spiking spend when they hit, and lowballing it when they don’t. That throws off forecasts and triggers avoidable back-and-forth with BUs.
Costs such as Backup storage charges that are charged on the 1st of the month should be spread over all days of the month.
Account Based Amortization - Costs such as Support fees, unused centrally purchased Savings Plans and cRIs should be spread across all accounts proportionately to their spend.
Cost Anomalies
Daily spend should be compared to the same day last week, not the day before. Most products run on weekly cycles, so comparing across weeks gives a cleaner signal.
Tiered costs such as S3 Storage and CloudWatch custom metrics: Set the cost anomaly threshold above 10% for S3 Storage to avoid false alarms when usage rolls from the $0.021/GB tier at month-end to the $0.023/GB tier at the start of the next month, and ignore MetricMonitorUsage spikes caused by use of $0.30 tier before switching to $0.10.
Costs bound to monthly pricing (such as EBS volume pricing) are higher per day in shorter months (such as February).
Q4 budget vs trailing 4 quarters average
Source sheet
Accounts highlighted in yellow are primary targets for investigation


BU
Class
Account Number
Account Name
Final Budget 2025-Q4
DIFF TO AVG
IgniteTech
Khoros Product
820054669588
Community Production ($)
$1,473,949
#N/A
IgniteTech
Khoros Product
180770971501
Care Production ($)
$1,350,738
#N/A
SaaS
SaaS Central
646253092271
Central
$686,598
94.20%
IgniteTech
Khoros Product
519148787890
Community Analytics Production ($)
$449,627
#N/A
IgniteTech
Khoros Product
947339144938
Marketing Production ($)
$446,818
#N/A
IgniteTech
Khoros Product
764203154397
Umbrella ($)
$400,334
#N/A
IgniteTech
Khoros Product
642760139656
Care Development ($)
$224,507
#N/A
IgniteTech
Jive Product
663559125979
jive-microservices-prod
$165,623
137.14%
IgniteTech
Khoros Product
361242680605
Community Development ($)
$118,506
#N/A
JigTree
Tivian Product
687746416010
tivian-xi-gmbh-production-de
$116,034
60.99%
Academics
Academics
182821611732
Prod-Alpha-Products
$93,956
134.87%
Academics
Academics
182821611732
(Exception) Recharging
$92,000
132.99%
Academics
Academics
515451715086
RAPIDAPI
$90,770
74.40%
Crossover
AWORK Product
908937782078
Prod-Crossover-XOApplications
$90,664
57.40%
Crossover
AWORK Product
104042860393
CrossOver
$89,222
128.93%
Central Support
Central support
899084202472
CoreSupport
$87,881
127.20%
IgniteTech
Jive Product
467524913882
jive-data-prod
$83,243
129.94%
IgniteTech
Jive Product
816069152650
Prod-IgniteTech-Jive
$80,224
#N/A
JigTree
Influitive Product
645720856124
AdvocateHub
$78,935
115.47%
IgniteTech
Jive Product
870846026232
jive-reco-prod
$77,219
100.02%
GFI
GFI Product
382834336226
Prod-Ignite-AppManager
$76,696
89.27%
IgniteTech
Jive Product
938797060115
vmcaws-jive-prod
$73,709
94.42%
Skyvera
Cloudsense Product
861276110329
Skyvera-Cloudsense-Prod
$70,827
#N/A
Crossover
AWORK Product
637423337752
Prod-Crossover-XoAIAssist
$65,524
152.60%
IgniteTech
Jive Product
517449413234
jive-infra-pipeline
$64,085
78.77%
JigTree
Kayako Product
086775481754
KayakoProd
$59,909
104.15%
Aurea e-Commerce
SLI Product
610092376560
Prod-Think3-SLIVMWARE
$59,342
108.62%
SaaS
SaaS Central
887704487240
CentralNetwork
$58,768
121.96%
JigTree
Messageone Product


(Exception) Recharging
$53,805
#N/A
IgniteTech
Jive Product
050451399198
Dev-IgniteTech-Jive
$53,510
#N/A
Crossover
AWORK Product
980921732366
Dev-Crossover-XoAIAssist
$51,917
#N/A
Central Support
Central support
060795935566
Prod-CentralSupport-KayakoCSProd
$50,115
#N/A
IgniteTech
Fog Bugz Product
450308135469
vmcaws-fogbugz-prod
$47,963
104.73%
IgniteTech
Khoros Product
441519177493
Corporate IT ($)
$45,031
#N/A
JigTree
Stratifyd Product
818160864477
Stratifyd Taste Analytics
$42,927
81.28%
JigTree
Tivian Product
201526351103
tivian-inc-production-us-cxi
$38,944
87.89%
SaaS
SaaS Central
572481847476
VDI
$38,941
22.24%
JigTree
Jigsaw Platform Product
404347245419
jig-prod
$37,724
102.72%
IgniteTech
Khoros Product
215874735434
Transit VPC ($)
$35,968
#N/A
IgniteTech
Khoros Product
052386936954
Community Analytics Development ($)
$35,566
#N/A
Totogi
TelcoDR
194313366991
Dev-DevFactory-LoadTestTotogiChargingAsAService
$34,878
107.38%
IgniteTech
Khoros Product
460151422989
Internal Services ($)
$33,555
#N/A
Crossover
AWORK Product
206786789429
Prod-Crossover-XOAppS3
$33,059
80.13%
Totogi
TelcoDR
617147411452
Prod-TelcoDR-telcodrtotogipresales1
$32,045
108.69%
LiveWorksheets
LiveWorksheets
051010810752
Prod
$31,668
94.65%
Contently
Contently Product
727712672144
Contently-Prod
$30,660
72.09%
IgniteTech
Ignite MISC Product
442426872992
Prod-IgniteTech-MyPersonas
$29,972
121.01%
Skyvera
Cloudsense Product
930519385031
CloudSense-Main
$29,437
119.25%
Totogi
TelcoDR
366471124629
Dev-DevFactory-DevTotogiChargingAsAService
$29,396
98.74%
IgniteTech
Ignite MISC Product
590183748006
Exp-IgniteTech-Personas
$29,064
91.36%
GFI
GFI Product
774538614749
Prod-CentralEngineering-Metal
$28,141
108.45%
IgniteTech
Jive Product
403612517204
jive-infra-prod
$28,008
97.90%
IgniteTech
Jive Product
811034720611
jive-microservices-pipeline
$26,676
110.36%
CloudFix
Aurea CloudFix Product
438051315841
Dev-CentralFunctions-CostOptimization
$24,891
162.70%
Tech Super Builders
Tech Super Builders
565944437804
Exp-Gauntlet-olympiclabs
$24,372
#N/A
IgniteTech
AnswerHub Product
937078055954
AnswerHub
$24,134
97.95%
Skyvera
STL Product
084375383684
Dev-SkyVera-STLDevOps
$24,089
117.64%
SaaS
SaaS Central
803334545221
Devfactory
$23,658
89.64%
JigTree
Kayako Product
654654284640
Jigsaw
$23,082
118.82%
Totogi
TelcoDR
266643203619
Prod-DevFactory-ProdTotogiChargingAsAService
$21,750
31.80%
JigTree
Tivian Product
239384733251
tivian-inc-production-us
$19,085
50.49%
Totogi
Totogi
799148289882
Prod-Totogi-CCAB
$18,868
85.13%
CloudFix
Aurea CloudFix Product
061081614506
Prod-AureaEnterprise-CloudFixProd
$18,447
131.92%
CNU
TU
082830052325
CodenationProd
$17,807
117.02%
IgniteTech
Ignite MISC Product
394287148065
Prod-Ignite-Tooling
$17,560
182.65%
JigTree
Playbooks Product
858958919402
PowerDialer for LMP
$16,923
57.41%
Skyvera
Cloudsense Product
842675985815
Skyvera-Cloudsense-Dev
$15,933
#N/A
JigTree
Tivian Product
130229005749
tivian-xi-gmbh-sandbox-de
$15,835
75.03%
SaaS
SaaS Central
583161073698
CentralDevTest
$15,747
114.45%
JigTree
Tivian Product
572801793087
tivian-xi-gmbh-development
$14,877
60.83%
GFI
GFI Product
074272777017
Dev-AureaSMB-GFI
$14,523
69.93%
Central Finance
Central Finance
479395885256
Int-CentralFunctions-CentralFinance
$14,149
185.99%
GFI
GFI Product
285199437787
GFI-Production
$13,267
100.31%
GFI
Kerio Product
129462265457
KerioDev
$13,162
184.45%
Skyvera
Mobilogy Product
462836960916
MobilogyEWS
$13,076
104.83%
Central Product
Central Product
992382370892
Prod-CentralProduct-productmind
$12,650
175.34%
Central Engineering
Central Engineering
897543225555
Prod-DevFactory-DFDevFlowsPROD
$11,961
158.26%
IgniteTech
IgniteTech Services
905418180661
Exp-IgniteTech-GENAI
$11,958
156.39%
Skyvera
NewNet Product
104075470635
NewNet
$11,816
125.29%
JigTree
Stratifyd Product
163510359818
Stratifyd Postgres
$11,798
67.68%
IgniteTech
Khoros Product
219578106441
Marketing Publishing Prod ($)
$11,656
#N/A
SaaS
SaaS Central
446735561331
Enterprise SaaS
$11,325
105.27%
SaaS
SaaS Central
313161139354
Operations Sys
$10,863
90.82%
JigTree
ACRM Product
835567349407
Update Operations
$10,524
90.47%
Academics
Academics
678572752603
Prod-JoeRandD-AlphaSchool
$10,125
96.41%
IgniteTech
StreetSmart Product
431452840136
VMCAWS-StreetSmart-Prod
$10,056
100.57%
IgniteTech
DNN Product
994672346694
vmcaws-dnn
$9,981
98.04%
Totogi
TelcoDR
764119721991
Prod-TelcoDR-TotogiPS
$9,961
136.30%
Totogi
TelcoDR
891377171970
Prod-Totogi-preprod
$9,839
63.63%
IgniteTech
ObjectStore Product
877439529387
ObjectstoreDev
$9,635
100.80%
JigTree
ACRM Product
156019071920
Dev-AureaEnterprise-ACRMWeb
$9,037
81.58%
JigTree
Stratifyd Product
466263447257
Stratifyd Support Systems
$8,948
76.62%
Academics
Academics
493888978727
Prod-Academics-lightciimport
$8,945
#N/A
CNU
TU
018066703918
Dev-DevFactory-TUQ32022InclusionIndex
$8,769
78.34%
Tech Super Builders
Tech Super Builders
474668398195
Prod-Gauntlet
$8,477
#N/A
GFI
GFI Product
623140692365
Dev-AureaSMB-gfimailessentials
$8,335
148.39%
Aurea e-Commerce
SLI Product
472290013053
SliSysDev
$8,287
84.76%
Aurea e-Commerce
SLI Product
448794654961
prod-avolin-sli-search4
$8,248
96.47%
GFI
GFI Product
171718550113
Dev-Ignite-AppManagerDev
$8,158
135.84%
IgniteTech
Ignite Local Search Product
726584805687
Placeable
$7,973
101.11%
JigTree
ISTA (AES) Product
522267007504
Aurea SaaSOps - AES
$7,937
106.76%
Crossover
AWORK Product
431184104557
Dev-Crossover-WorkSmart
$7,460
49.96%
Totogi
Totogi
677015454621
Dev-Totogi-bssmagic
$6,823
#N/A
Totogi
TelcoDR
128564496312
Prod-DevFactory-openappstmforum
$6,796
105.15%
Totogi
TelcoDR
471112892932
Prod-Totogi-TotogiMSZain
$6,655
45.10%
Skyvera
Cloudsense Product
094325448796
CloudSense-Integration
$6,617
89.26%
IgniteTech
Khoros Product
584263334748
Marketing Publishing Dev ($)
$6,449
#N/A
Skyvera
NewNet Product
943423155328
Prod-ZephyrTel-NewNetFirewall
$6,131
85.59%
JigTree
Messageone Product
680095798327
MessageOne Production
$6,033
98.36%
Academics
Academics
750697792272
Dev-JoeRandD-alphamanualcoachbot
$5,971
112.28%
JigTree
Aurea Platform Product
892905447879
AureaInternal
$5,921
103.63%
GFI
Kerio Product
233505949748
KerioBusinessSystems
$5,780
101.21%
Totogi
TelcoDR
975049952463
Prod-Totogi-IWFZain
$5,595
75.47%
CNU
TU
324613809385
Prod-CNU-coachbotrewriteti
$5,546
59.08%
Skyvera
Kandy Product
824221571066
Dev-Kandy-Lab
$5,531
132.14%
New Renewals
New Renewals
524963845153
Prod-DevFactory-SalesInfrastructure
$5,407
118.91%
IgniteTech
Sococo Product
429878810765
Prod-Think3-SOC5K
$5,238
104.57%
IgniteTech
Jive Product
011880796339
JivesITOps
$5,235
98.96%
LiveWorksheets
LiveWorksheets
277909509535
LiveWorksheets
$5,167
70.79%
CloudFix
Aurea CloudFix Product
472628968186
Dev-AureaEnterprise-CloudFixQA
$5,152
108.20%
CloudFix
Aurea CloudFix Product
994222729242
Prod-CentralFunctions-awscrioptimizer
$5,020
136.77%



