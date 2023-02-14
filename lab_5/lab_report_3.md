# Lab Report 3

### 1. `-name`-- Searches for files by their name.

* example 1 (search form written_2/non-fiction/OUP/Castro/ forall file name that end with ".txt")
    ```
    find written_2/non-fiction/OUP/Castro/ -name *.txt
    written_2/non-fiction/OUP/Castro/chA.txt
    written_2/non-fiction/OUP/Castro/chB.txt
    written_2/non-fiction/OUP/Castro/chC.txt
    written_2/non-fiction/OUP/Castro/chL.txt
    written_2/non-fiction/OUP/Castro/chM.txt
    written_2/non-fiction/OUP/Castro/chN.txt
    written_2/non-fiction/OUP/Castro/chO.txt
    written_2/non-fiction/OUP/Castro/chP.txt
    written_2/non-fiction/OUP/Castro/chQ.txt
    written_2/non-fiction/OUP/Castro/chR.txt
    written_2/non-fiction/OUP/Castro/chV.txt
    written_2/non-fiction/OUP/Castro/chW.txt
    written_2/non-fiction/OUP/Castro/chY.txt
    written_2/non-fiction/OUP/Castro/chZ.txt
    ```
    
* example 2 (search from written_2 for all file name contain"Po")
    ```
    find written_2/ -name *Po*
    written_2/travel_guides/berlitz2/Poland-History.txt
    written_2/travel_guides/berlitz2/Poland-WhatToDo.txt
    written_2/travel_guides/berlitz2/Portugal-History.txt
    written_2/travel_guides/berlitz2/Portugal-WhatToDo.txt
    written_2/travel_guides/berlitz2/Portugal-WhereToGo.txt
    ```
        

### 2. `-iname` -- Searches for files by their name but ignore the case.

* example 1 (search from written_2/non-fiction/OUP/ for allfile name that are ch4.txt ignore the case)
    ```
    find written_2/non-fiction/OUP/ -iname ch4.txt
    written_2/non-fiction/OUP/Berk/CH4.txt
    written_2/non-fiction/OUP/Kauffman/ch4.txt
    ```
    
* example 2 (search from written_2/travel_guides/berlitz2 forall file name that contain "history" ignore the case)
    ```
    find written_2/travel_guides/berlitz2 -iname *history*
    written_2/travel_guides/berlitz2/Algarve-History.txt
    written_2/travel_guides/berlitz2/Amsterdam-History.txt
    written_2/travel_guides/berlitz2/Athens-History.txt
    written_2/travel_guides/berlitz2/Bahamas-History.txt
    written_2/travel_guides/berlitz2/Bali-History.txt
    written_2/travel_guides/berlitz2/Barcelona-History.txt
    written_2/travel_guides/berlitz2/Beijing-History.txt
    written_2/travel_guides/berlitz2/Berlin-History.txt
    written_2/travel_guides/berlitz2/Bermuda-history.txt
    written_2/travel_guides/berlitz2/Budapest-History.txt
    written_2/travel_guides/berlitz2/California-History.txt
    written_2/travel_guides/berlitz2/Canada-History.txt
    written_2/travel_guides/berlitz2/CanaryIslands-History.txt
    written_2/travel_guides/berlitz2/Cancun-History.txt
    written_2/travel_guides/berlitz2/China-History.txt
    written_2/travel_guides/berlitz2/Costa-History.txt
    written_2/travel_guides/berlitz2/CostaBlanca-History.txt
    written_2/travel_guides/berlitz2/Crete-History.txt
    written_2/travel_guides/berlitz2/Cuba-History.txt
    written_2/travel_guides/berlitz2/Nepal-History.txt
    written_2/travel_guides/berlitz2/NewOrleans-History.txt
    written_2/travel_guides/berlitz2/Poland-History.txt
    written_2/travel_guides/berlitz2/Portugal-History.txt
    written_2/travel_guides/berlitz2/PuertoRico-History.txt
    written_2/travel_guides/berlitz2/Vallarta-History.txt
    ```
        

### 3. `-type`-- Search only only files or only directories(d for directoies, f for files)

* example 1 (Search from written_2/non-fiction/OUP/ for alldirectoies)
    ```
    find written_2/non-fiction/OUP/ -type d
    written_2/non-fiction/OUP/
    written_2/non-fiction/OUP/Abernathy
    written_2/non-fiction/OUP/Berk
    written_2/non-fiction/OUP/Castro
    written_2/non-fiction/OUP/Fletcher
    written_2/non-fiction/OUP/Kauffman
    written_2/non-fiction/OUP/Rybczynski
    ```
* example 2 (Search from written_2/non-fiction/OUP/ for allfiles)
    
    ```
    find written_2/non-fiction/OUP/ -type f
    written_2/non-fiction/OUP/Abernathy/ch1.txt
    written_2/non-fiction/OUP/Abernathy/ch14.txt
    written_2/non-fiction/OUP/Abernathy/ch15.txt
    written_2/non-fiction/OUP/Abernathy/ch2.txt
    written_2/non-fiction/OUP/Abernathy/ch3.txt
    written_2/non-fiction/OUP/Abernathy/ch6.txt
    written_2/non-fiction/OUP/Abernathy/ch7.txt
    written_2/non-fiction/OUP/Abernathy/ch8.txt
    written_2/non-fiction/OUP/Abernathy/ch9.txt
    written_2/non-fiction/OUP/Berk/CH4.txt
    written_2/non-fiction/OUP/Berk/ch1.txt
    written_2/non-fiction/OUP/Berk/ch2.txt
    written_2/non-fiction/OUP/Berk/ch7.txt
    written_2/non-fiction/OUP/Castro/chA.txt
    written_2/non-fiction/OUP/Castro/chB.txt
    written_2/non-fiction/OUP/Castro/chC.txt
    written_2/non-fiction/OUP/Castro/chL.txt
    written_2/non-fiction/OUP/Castro/chM.txt
    written_2/non-fiction/OUP/Castro/chN.txt
    written_2/non-fiction/OUP/Castro/chO.txt
    written_2/non-fiction/OUP/Castro/chP.txt
    written_2/non-fiction/OUP/Castro/chQ.txt
    written_2/non-fiction/OUP/Castro/chR.txt
    written_2/non-fiction/OUP/Castro/chV.txt
    written_2/non-fiction/OUP/Castro/chW.txt
    written_2/non-fiction/OUP/Castro/chY.txt
    written_2/non-fiction/OUP/Castro/chZ.txt
    written_2/non-fiction/OUP/Fletcher/ch1.txt
    written_2/non-fiction/OUP/Fletcher/ch10.txt
    written_2/non-fiction/OUP/Fletcher/ch2.txt
    written_2/non-fiction/OUP/Fletcher/ch5.txt
    written_2/non-fiction/OUP/Fletcher/ch6.txt
    written_2/non-fiction/OUP/Fletcher/ch9.txt
    written_2/non-fiction/OUP/Kauffman/ch1.txt
    written_2/non-fiction/OUP/Kauffman/ch10.txt
    written_2/non-fiction/OUP/Kauffman/ch3.txt
    written_2/non-fiction/OUP/Kauffman/ch4.txt
    written_2/non-fiction/OUP/Kauffman/ch5.txt
    written_2/non-fiction/OUP/Kauffman/ch6.txt
    written_2/non-fiction/OUP/Kauffman/ch7.txt
    written_2/non-fiction/OUP/Kauffman/ch8.txt
    written_2/non-fiction/OUP/Kauffman/ch9.txt
    written_2/non-fiction/OUP/Rybczynski/ch1.txt
    written_2/non-fiction/OUP/Rybczynski/ch2.txt
    written_2/non-fiction/OUP/Rybczynski/ch3.txt
    ```

### 4. `-exec`-- Execute command with find result as an argument

* example 1 (Search from written_2 for file name is find_alltxt and use it as an argument to execute the command after"-exec". argument goes into the "{}", "+" means end of thecommand)
    ```
    ls
    find_all.txt  written_2
    find . -name find_all.txt -exec rm {} +
    ls
    written_2
    ```
* example 2 (Search from written_2/non-fiction/OUP/Castro/ forfile name is chA.txt and use it as an argument to execute thecommand after "-exec". argument goes into the "{}", "+" meansend of the command)
    ```
    find written_2/non-fiction/OUP/Castro/chA.txt -exec cat {} +
    El Abuelo (Grandfather)
    An old-man figure called el abuelo (the grandfather) played the role ofa bogeyman in Hispano folklore. In literature it is sometimes spelledaguelo, and some scholars speculate that it may be a borrowed word fromthe language of the Pueblo Indians. In Spanish it means “grandfather,”and has become synonymous with coco, cucui, and bogeyman. This folkcharacter is more known in northern New Mexico than in other      partsof the Southwest. He appeared at Christmastime to test and disciplinechildren who did not know their catechism or prayers. He was a scaryfigure, dressed to terrify children with a black cape and a mask withlarge horns, and always carrying a whip. Children were terriblyfrightened because of his horrid appearance. Instead         of a maskhe sometimes had a tortilla plastered on his face, wore buffalo hornsand a horsetail, and of course carried the whip. A few days beforeChristmas, he’d knock  on the door of a home, give a bloodcurdling cry,crack his whip, and yell at the children, “Han sido buenos muchachosestos?” (Have these children been good?) The children would cringe andhide while the parents defended them. Then el abuelo would say, “Puesque recén y se acuestén” (Well, let them pray and go to bed). Sometimeshe made the children dance Las Palomitas, loosely translated as “thelittle doves.” Espinosa describes this experience. “After making thempray, he makes them form a circle, and, taking each other’s hands, theydance around the room with him, singing, Baila paloma de Juan turuntún(or durundún) [sic]
    ‘Turun tún tún
    Turun tun tún!’
    (Dance dove of Juan confused or disoriented
    Confused, confused!)
    ...
    ```

### 5. Work cited 
* Source for the four command: https://www.binarytides.comlinux-find-command-examples/