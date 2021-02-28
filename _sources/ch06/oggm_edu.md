# OGGM-Edu

OGGM-Edu ([http://edu.oggm.org](https://edu.oggm.org)) is an educational website about glaciers.

I briefly summarize its main goals and history here: the interested reader is invited to have a look at 
[the platform itself](https://edu.oggm.org) to explore its content!

```{figure} https://edu.oggm.org/en/latest/_static/logos/oggm_edu_s_alpha.png
:width: 40%
:align: left
```

## Concept

OGGM-Edu's main goal is to provide interactive tools and materials for instructors who want to 
teach about glaciers and glacier modelling at school, in workshops or at the university.
It does not provide much fundamental textbook material, unless at places where we found it very necessary. 
In general, we link to more comprehensive, additional online resources such as
[AntarcticGlaciers.org](http://www.antarcticglaciers.org/) for the theoretical background.

Everything on OGGM-Edu is open-source: one can find all our content, apps, and website [on GitHub](https://github.com/OGGM/oggm-edu). 
The platform is designed to be collaborative, and any interested person can contribute via GitHub with a new experiment, 
a typo correction, a translation...

Finally, all OGGM-Edu tools should work in the web browser and do not require installation: instructors simply need to 
make sure that students have a computer with an internet connection to get them started.

## Content

OGGM-Edu offers four largely independent components that can be combined for a longer class: 

- [Graphics](https://edu.oggm.org/en/latest/#title-graphics): open access images and graphics that
  illustrate some basic concepts about glaciers and that can be used in lectures or presentations. 
  They were designed for a general audience and are a good entry point to glaciers. 
- [Interactive web applications](https://edu.oggm.org/en/latest/#title-apps): ready to use, interactive graphics on the web.
  They come with introduction materials and videos about how to use them, as well as example questions which can be explored in class. 
  The targeted audience is very broad, from school children to adults, with
  or without scientific background.
- [Interactive Notebooks](https://edu.oggm.org/en/latest/#title-notebooks): [Jupyter notebooks](https://jupyter.org/) that combine narrative text, 
  equations, executable code and visualisations in one document. They are designed for students willing to run and develop their 
  own experiments. The targeted audience are students at the undergrad or graduate level with some 
  programming experience, or under the supervision of an instructor who can show them how to run the experiments.  
- [OGGM tutorials](https://edu.oggm.org/en/latest/oggm_tuto.html): for current and future users of the Open Global Glacier Model.
    
## Known applications in classes

It is very difficult for us to know the extent to which OGGM-Edu is already used (or considered for use) in classes.
Feedback so far on social media or on CRYOLIST has been very positive, but we haven't received concrete improvement suggestions
or bugfix requests either (which can be seen as a good or a bad thing).

Here are some examples of application we are aware of:
- OGGM-Edu (apps, notebooks) is used as part of the practical sessions in the "Cryosphere in the Climate System" 
  lecture, taught in the master program "Atmospheric Sciences" at the University Innsbruck.  
- OGGM-Edu (apps + edited and translated notebooks) has benn used for a week-long workshop for undergraduate students 
  in Peru.
- The OGGM-Edu apps were used in at least three university-level classes for which we received positive feedback from
  the instructors themselves [on social media](https://twitter.com/iceclimate/status/1359280232990199809) and per mail.

## Project history, funding and outlook

The OGGM-Edu website was launched at the end of 2018. The main bulk of the website development was done by myself,
and large parts of the content has been writen by master students. I was able to hire a student (Zora Schirmeister) 
early in the process thanks to  a small digital sciences grant offered by the University of Innsbruck to work on the 
first notebooks. 

In 2019, I applied and obtained a much larger grant from an outreach scheme of the University of Innsbruck 
("Förderkreis **1669** – **Wissen**schafft Gesell**schaft**", 20k€),
which allowed me to hire four students (Zora Schirmeister, Patrick Schmitt, Daniel Frisinghelli, Alzbeta Medvedova)
to work part-time on the project for one year. This led to the development of the four web applications, 
and to the development of several new notebooks.

I also applied and obtained a 10k€ computational resources grant from Google Cloud's "Data Solutions for Change"
(a programme now discontinued). This grant allowed us to host the applications on controlled resources instead of free,
but unreliable ones. This allowed us to provide a "hub" (online computer resources) to Lizz Ultee's students during 
[her workshop in Peru](https://oggm.org/2019/12/06/OGGM-Edu-AGU/). Again, the main advantage of these resources 
being the complete removal of the installation's burden. At the end of this Google grant in 2020, we moved OGGM-hub
and the hosting of our applications to our own HPC facilities in Bremen.

Today, I think that the platform is useful as it is. Since 2020, the improvements to the platform have been incremental, 
mostly with improvements to the interactive apps (which, we believe, are the most used tools on the platform). Further
improvements might come from the instructors themselves - for example, the "glaciers as water resources" notebook
was developed as part of Lizz Ultee's workshop.

Like for software, the main obstacle towards further large scale developments are: funding, staff, and time.
Again, traditional funding schemes are not really appropriate for OGGM-Edu. Many funders now explicitly ask
for an outreach component (a role that OGGM-Edu could fill for OGGM related projects), and if there is 
interest from project staff to invest time in OGGM-Edu's development, it is likely to continue to grow.

I think that the students who worked on OGGM-Edu should be very proud of what they have achieved! 
