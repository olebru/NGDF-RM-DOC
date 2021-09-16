
 flowchart TD
 1(Experienced Team)-->|No|Stop(No go, perform full plan process)
 1 -->|Yes|2(Known Cave?)
 2-->|No|Stop
 2-->|Yes|3(Envorionment)
 3-->|Tight|Stop
 3-->|Large passages|4(High flow)
 4-->|Yes|Stop
 4-->|No|5(Visibility)
 5-->|Poor|Stop
 5-->|Good|6(Backup team ready)
 6-->|No|7(Easy Rescue? Type1)
 7-->|Yes|Go
 7-->|No|Stop
