# MTFed: Multitask Clinical Representation Learning viaMulti-Institutional Federation with EMR Privacy Preserving

The source code of Multi-Variable Sequential Medical Records Representation Learning in MTFed.

Thanks for your interest in our work. More details about the experiment, case study and visualization system will be released before WWW2020.

## Visualization

Welcome to test the prototype of our visualization tool:

http://47.93.42.104/covid/64 (Alive)

http://47.93.42.104/covid/218 (Dead)

Health Status Trajectory and High-risk Biomarkers Visualization:

https://anonymous20201020.github.io/MTFed-DeadGraph/

Architecture of MTFed

![Architecture of MTFed](https://raw.githubusercontent.com/anonymous20201020/MTFed/main/architecture%20of%20MTFed.jpg)

Federal Collaborators of MTFed

![Federal Collaborators of MTFed](https://raw.githubusercontent.com/anonymous20201020/MTFed/main/federal%20collaborators%20of%20MTFed.png)

Federated Clustering

![Federated Clustering](https://raw.githubusercontent.com/anonymous20201020/MTFed/main/federated%20clustering.png)

Table 4. Avg. LOS risk score of clusters visited by the case patient 64

| Record | Date      | Cluster ID | Condition          | Avg. LOS Risk | #Records in TJH | #Records in HMH |      Important Features      |
| :----: | :-------: | :--------: | :----------------: | :-----------: | :-------------: | :-------------: | :--------------------------: |
|   1    | Feb.5     | 7          | Medium Risk        | 34.586        | 10              |       57        |   fibrinogen, serum sodium   |
|   2    | Feb.5     | 13         | Medium Risk        | 32.577        | 24              |       68        | fibrinogen, lymphocyte count |
|   3    | Feb.5     | 37         | Low Risk           | 15.054        | 35              |       57        |  ferritin, lymphocyte count  |
|   4    | Feb.5     | 17         | Low Risk           | 15.487        | 73              |       58        |  ferritin, lymphocyte count  |
|   5    | Feb.5     | 23         | Low Risk           | 16.571        | 97              |       55        | fibrinogen, lymphocyte count |
|   6    | Feb.10    | 20         | Low Risk           | 14.719        | 133             |       59        |      ferritin, albumin       |
|   7    | Feb.11    | 76         | Low Risk           | 12.629        | 221             |       53        |         FDP, albumin         |
|   8    | Feb.11    | 4          | Low Risk           | 8.421         | 236             |       89        |  FDP, prothrombin activity   |
|   9    | Feb.11    | 15         | Low Risk           | 8.056         | 273             |       90        |  FDP, prothrombin activity   |
| 10-12  | Feb.11    | 46         | Close to discharge | 6.739         | 267             |       73        |     FDP, eosinophils(%)      |
| 13-15  | Feb.11-12 | 47         | Close to discharge | 6.514         | 268             |        0        |     FDP, eosinophils(%)      |
| 16-17  | Feb.14-16 | 22         | Close to discharge | 4.887         | 2589            |        0        |    FDP, eosinophils count    |
| 18-20  | Feb.16    | 64         | Close to discharge | 3.724         | 285             |        0        |    FDP, eosinophils count    |
| 21-24  | Feb.16-18 | 39         | Close to discharge | 2.166         | 171             |        0        |    FDP, eosinophils count    |
|   25   | Feb.18    | 28         | Close to discharge | 1.973         | 6               |       279       |        TCO2V, calcium        |


## Requirements

- Install python, pytorch. We use Python 3.7.3, Pytorch 1.1.
- If you plan to use GPU computation, install CUDA

## Data preparation

1. The Tongji Hospital COVID-19 Collaborator is introduced at: 
   https://www.nature.com/articles/s42256-020-0180-7
2. The HM Hospitals COVID-19 Collaborator is introduced at: 
   https://www.hmhospitales.com/prensa/notas-de-prensa/comunicado-covid-data-save-lives.
3. The PhysioNet Collaborator is introduced at: 
   https://physionet.org.
