# Date Formats
```chronos
- [2020] A year
- [2020-02] A month
- [2020-02-28] A day
- [2020-02-28T12] An hour
- [2020-02-28T12:30] A minute
- [2020-02-28T12:30:09] A second
```

# Single Event
```chronos
- [1879-03-14] Einstein born
```

# Date Range
```chronos
-  [1991~2001] Time I believed in Santa
```
  


# Event with Description
```chronos
- [1991~2001] Time I believed in Santa | ended when my brother tried to videotape Santa with a hidden camera

# Hover on a timeline item to see its description
```


# Groups
```chronos
@ [1892-10-08~1941-08-31] {Marina Tsvetaeva} 1892-1941
- [1916] {Marina Tsvetaeva} "Подруга"
- [1928] {Marina Tsvetaeva}  "Поэма концов"
- [1941] {Marina Tsvetaeva} "Записки о поэзии"

@ [1899-08-24~1986-06-14] {Jorge Luis Borges} 1899-1986
- [1944] {Jorge Luis Borges} "Ficciones"
- [1949] {Jorge Luis Borges} "El Aleph"
- [1962] {Jorge Luis Borges} "Labyrinths"
```

# Periods
```chronos
@ [-300~250] Yayoi Period
- [-100] Introduction of rice cultivation
- [-57] Japan's first recorded contact with China
```
  
# Colored Periods
```chronos
@ [-300~250] #red Yayoi Period
- [-100] Introduction of rice cultivation
- [-57] Japan's first recorded contact with China

@ [250~538] Kofun Period
- [250] Construction of keyhole-shaped kofun burial mounds begins
- [369] Yamato state sends envoys to Korea
```

# Colored Events
```chronos
- [2001~2009] #red Bush
- [2009~2017] #blue Obama
- [2017~2021] #red Trump
- [2021~2025] #blue Biden
@ [2020-03~2023-05] #pink COVID19

# You can also use custom hex-code colors like #dd6689
```

# Points
```chronos
- [2024-02-26~2024-03-10] Tournament
* [2024-02-26] Game 1 | Austin
* [2024-02-28] Game 2 | Los Angeles
* [2024-03-06] Game 3 | Tokyo
* [2024-03-10] Game 4 | Jakarta
```


# Markers
```chronos
= [1440] Invention of the Gutenberg Press

- [1455] Gutenberg Bible Printed
@ [1501~1600] The Spread of Printing
- [1517] Martin Luther's 95 Theses
```

# Order By Start
```chronos
> ORDERBY start

- [2026~2028] Event D
- [2024~2028] Event B
- [2025~2030] #red Event C
- [2020~2030] #red Event A
```

# Order By Color and Date
```chronos
> ORDERBY color|start

- [2026~2028] Event D
- [2024~2028] Event B
- [2025~2030] #red Event C
- [2020~2030] #red Event A
```


# Default View Range
```chronos
> DEFAULTVIEW -3000|3000
# Offset the default centered view with custom start|end dates

- [2024] AGI
```

# Don't Stack Items
```chronos
> NOSTACK
# Note: NOSTACK is all or nothing... overlapping items will override eachother

- [2019~2021] {Group A} baz
- [2021~2022] #red {Group A}  foo
- [2021~2022] {Group B} bar
- [2022~2025] #red {Group B} bam
```


# Advanced: Cold War Timeline
```chronos
- [1945-07-17] {Europe} Potsdam Conference | where post-WWII Europe is divided
- [1947-03-12] {USA} Truman Doctrine | committing the U.S. to containing communism
- [1948-06-24~1949-05-12] {Europe} Berlin Blockade | and Airlift in response to Soviet actions in Berlin
- [1949-04-04] {Europe} Formation of NATO

@ [1957~1969] #cyan {USSR} Space Race
@ [1957~1969] #cyan {USA} Space Race
- [1950-06-25~1953-07-27] {Asia} Korean War | between North and South Korea
- [1955-05-14] {USSR} Warsaw Pact | in response to NATO
- [1957-10-04] #cyan {USSR} Sputnik launched | initiating the Space Race
- [1961-04-17] {Cuba} Bay of Pigs Invasion | in Cuba

- [1962-10-16] {Cuba} Cuban Missile Crisis | a peak confrontation between the U.S. and USSR
- [1963-08-05] {Global} Partial Nuclear Test Ban Treaty signed
- [1969-07-20] #cyan {USA} Apollo 11 Moon landing | U.S. wins the Space Race
- [1972-05-26] {Global} SALT I signed | first Strategic Arms Limitation Treaty

- [1979-12-24~1989-02-15] {USSR} Soviet-Afghan War | straining Soviet resources
- [1983-03-23] {USA} Reagan announces the Strategic Defense Initiative (SDI)
- [1986-04-26] {USSR} Chernobyl nuclear disaster
- [1987-12-08] {Global} INF Treaty | signed, eliminating intermediate-range nuclear missiles

- [1989-11-09] {Europe} Fall of the Berlin Wall | symbolizing the end of Cold War tensions
- [1991-07-31] {Global} START I Treaty signed | further arms reduction
- [1991-12-26] {USSR} Dissolution of the Soviet Union | officially ending the Cold War

= [1991-12-26] End of the Cold War
```
# Different Groups with Colors
Dream Theater Band Members over years
```chronos
@ [1989~2027] {Albums} 1987-2027  
= [1989] When Dream and Day Unite
= [1992] Images and Words
= [1994] Awake
= [1997] Falling into Infinity
= [1999] Metropolis Pt. 2: Scenes from a Memory
= [2002] Six Degrees of Inner Turbulence
= [2003] Train of Thought
= [2005] Octavarium
= [2007] Systematic Chaos
= [2009] Black Clouds & Silver Linings
= [2011] A Dramatic Turn of Events
= [2013] Dream Theater
= [2016] The Astonishing
= [2019] Distance Over Time
= [2021] A View from the Top of the World
= [2025] Parasomnia
@ [1987~1990] #red {Charles Dominici} 1987-1989
@ [1991~2027] #red {James Labrie} 1991-present
@ [1987~2027] #blue {John Petrucci} 1987-present
@ [1987~2027] #yellow {John Myung} 1987-present
@ [1987~1995] #green {Kevin Moore} 1987-1994
@ [1995~2000] #green {Derek Sherinian} 1995-1999
@ [1999~2027] #green {Jordan Rudess} 1999-present
@ [1987~2011] #brown {Mike Portnoy} 1987-2010
@ [2011~2024] #brown {Mike Mangini} 2011-2023
@ [2024~2027] #brown {Mike Portnoy} 2024-present

```