# 2019-Kaggle-Bowl

This is from 2019 Kaggle bowl competetion- https://www.kaggle.com/c/data-science-bowl-2019/overview
Feature engineering done in two different versions differently. Best cohen-Kappa score .50 for Kaggle submision 
where top score is .57.

## Description and Challenge of the project¶

In this project game analytics data for kids given by PBS KIDS. In this app kids can play
games, watch clips and perform different activities and after some game session they are assigned
test.Kids can take multiple tests or single test or many records for kids with no test.
If they cam solve test correctly in single attempt then their accuracy group is 3, if two attempt
to solve correctly then accuracy group is 2, if multiple atempts then 1 if could not solve then 0.
Dataset is hierchical. For every apps installed, one installation id is assigned. We can consider
one kid has one installation id (assuming no shared device). One kid can play multiple game sessions
and one game session might have multiple events. Some of the variables like activity types, title, world
etc. are in game session level and some event related variables are at lower level.
Target variable is accuracy group.
The challenge is in train data accuracy group is at game session level
but we have to predict in test data at installation id level, in higher level.
Moreover only 1000 test records are given but Kaggle is measuring accuracy on 8 MM records.
