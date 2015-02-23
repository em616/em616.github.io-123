---
published: true
layout: post
title: Intimiteti ne Facebook 
---

##  Intimiteti ne Facebook 

Ckemi djema?
Ne kete postim te rradhes po ju flas pak per intimitetin qe na ofron facebook.
Pothujase te gjith jemi ne dijene se faqe si facebook japin per qeverite informacione tonat personale.
Sot duke analizuar nje program me packet sniffer verejta nje lidhje nga kompjuteri im me facebook mbasi kisha mbyllur facebookun.
Pak e cuditshme apo jo? Dhe nuk eshte thjesht kontrollimi i cookies, por dhe mbase e heqen komplet nga browseri facebookun.
Mundet akoma te shikoj se cfar websajtesh po vizitoni, dhe gjera tjera qe akoma nuk i dij per kete.
Nuk jam i sigurte se cfar eshte por mendoj qe ideja eshte mbledhja e sa me shum te dhenave personale per cdo njerin nga ne dhe ti perdori per arsyet e veta.

Well, te dalim fiks ne teme.
Mbasi mbylla ne browser cdo gje qe ka nje lidhje me facebook, normalisht duhet te besojme qe cdogje eshte e mbyllur, dhe nuk ke me pune mete.
Kjo qe po ju shfaqi me poshte eshte, mbas mbylljes se facebook nga kompjuteri im.
E Cila verteton lidhje mes kompjuterit tim dhe 2 serverave te facebook.

> en@em616:~# lsof -i | grep facebook
firefox   19180         enn   34u  IPv4 483659      0t0  TCP fLcReW.local:58367-edge-star-ecmp-01-ams2.facebook.com:https (ESTABLISHED)
firefox   19180         enn   53u  IPv4 480796      0t0  TCP fLcReW.local:39191-channel-ecmp-06-frc1.facebook.com:https (ESTABLISHED)

Per fat te keq e njejta gje me ndodhi edhe me browser privat si TOR. Dhe per veten nuk me doket asgje e mire.
Dhe nuk e kuptoj se cfar menyre eshte ajo qe facebook perdor per te arritur kete. Por te mendoj qe sikur cdo webfaqe qe vizitojme te vazhdoj me te njejtin proces?

Menyrat per ta bllokuar kete lidhja jane 2.
E pare e thjeshte. Ristartoni browserin :)
Ose nese je perdorues linuxi perdorni kete komande.

> sudo ngrep -q -d any 'facebook.com' -K 10
