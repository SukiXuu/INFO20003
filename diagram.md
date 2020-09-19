# DIAGRAM

```text
Alice->Bob: Hello Bob, how are you?
Note right of Bob: Bob thinks
Bob-->Alice: I am good thanks!
```

```text
st=>start: Start
op=>operation: Your Operation
cond=>condition: Yes or No?
e=>end

st->op->cond
cond(yes)->e
cond(no)->op
```

```text
%% Example of sequence diagram
  sequenceDiagram
    Alice->>Bob: Hello Bob, how are you?
    alt is sick
    Bob->>Alice: Not so good :(
    else is well
    Bob->>Alice: Feeling fresh like a daisy
    end
    opt Extra response
    Bob->>Alice: Thanks for asking
    end
```

```text
%% Example with selection of syntaxes
        gantt
        dateFormat  YYYY-MM-DD
        title Semester2 ASSIGNMENT

        section MAST20004
        Assignment1:done, 2020-08-23,2020-08-24
        Assignment2:active,  des2, 2020-09-13,2020-09-14
        Assignment3: 

        section MAST20018
        Quiz1:done,2020-08-27, 2020-08-28
        Quiz2:done,2020-09-03, 2020-09-04
        Quiz3: 

        section INFO20003
        Assignment1     /15    数据库      :done, 2020-08-27, 2020-08-28
        Assignment2: 
        Quiz1     2.7/5          :done,   2020-08-16, 2020-08-17
        Quiz2     2.86/5,          :done, 2020-08-23, 2020-08-24
        Quiz3     5/5          :done, 2020-08-30, 2020-08-31
        Quiz4     5/5          :done, 2020-09-06, 2020-09-07
        Quiz5               :active, 2020-09-013, 2020-09-14

        section COMP10002
        Quiz1     7/10          :done,    ,2020-08-27 ,  2020-08-28
        Quiz2     7/10          :active,2020-09-10, 2020-09-11
        Quiz3     7/10          :active,2020-10-15, 2020-09-16
        Assignment1     /15          :active,2020-09-08, 2020-09-10
        Assignment2     /15          :  

        section COMP20008
        Assignment1 25% 爬虫:active, 2020-09-01, 2020-09-21
        Assignment2:
```

```text
    section Critical tasks
    Completed task in the critical line :crit, done, 2014-01-06,24h
    Implement parser and jison          :crit, done, after des1, 2d
    Create tests for parser             :crit, active, 3d
    Future task in critical line        :crit, 5d
    Create tests for renderer           :2d
    Add to mermaid                      :1d

    section Documentation
    Describe gantt syntax               :active, a1, after des1, 3d
    Add gantt diagram to demo page      :after a1  , 20h
          Add another diagram to demo page    : 48h
```

