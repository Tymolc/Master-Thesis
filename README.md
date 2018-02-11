# template-thesis-hci

This repo aims to help master students getting started with their master thesis.

# Master Thesis

A master thesis at the HCI chair is a great opportunity to learn – but it's not the only one. Maybe you have not worked on a single project for more than a semester full time. Thus, explore possible options before committing too early. 
Ready? Great, let's dive in!

Keep a logbook every day to capture key insights and project progress,  preferably with figures. You can plan ahead to have a project roadmap and also keep your backlog in this document.
I'd append to the logbook at the top (reversed order).

# Registration and deadlines
In the past, students have chosen freely the date of registering the thesis with the Studienreferat. After this registration, you have 6 months remaining. 

Put your deadline 3 weeks+ after the UIST/CHI deadline so that you can 
(a) use the walkthrough, videos, and figures you developed with your advisor and 
(b) have sufficient time to write a good thesis document to satisfy the second examiner.

Otherwise, there may be the risk of not being able to dedicate enough time for the thesis when working towards a demo for conference submission.

# Second Examiner
Typically, the second examiner gets chosen after the thesis is handed in and defended. To have the chance to personally convince the second examiner with your great defence presentation make the person has to be picked already. To that end, consider reminding Prof. Baudisch – not only early, but also often – about picking a second examiner.

# Getting started
To start your own repo for your thesis, run the following commands in a terminal:

```
git init mythesis
cd mythesis
git pull git@bitbucket.org:hpihci/template-thesis-hci.git master
```

You can also use the last command to update your copy of the template.

To generate masterthesis.pdf run
```
cd latex
pdflatex masterthesis.tex
```

Customize `latex/classicthesis-config.tex` to your needs.

## Installing dirtytalk

On Windows when using MiKTeX you will have to install the package `dirtytalk` manually.

1. Download it from here https://www.ctan.org/pkg/dirtytalk
2. On MiKTeX, after you've unzipped  `dirtytalk.zip` in some directory, you'll have to compile the file `dirtytalk.ins` to produce `dirtytalk.sty`. To do this run `latex dirtytalk.ins`.
3. To make it usable, if you made an installation for all users, create a TeXMFlocal directory (not in MiKTeX roots) if not already done, and declare as `root` with `MiKTeX Settings(Admin)`, `Root tab`, with the `Add…` button, like this: 
4. Then copy `dirtytalk.sty` in `TeXMFlocal\tex\latex\dirtytalk\`, and `dirtytalk.pdf` in `TeXMFlocal\latex\doc\dirtytalk\`.
5. Finally, refresh the FNDB (under `General` tab).
6. If you made a per-user installation do the same with `MiKTeX Settings`.
These instructions were taken from https://tex.stackexchange.com/a/329815.