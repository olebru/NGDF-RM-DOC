 
 ## Risk - Quick

 ```mermaid
flowchart TD
Rescue(Redning)
Vis(Sikt)
Flow(Strøm)
Restr(Trangt)
Familiar(Kjennskap til dette systemet)
Lines(Linesystem inntakt)
LocalBrief(Mulightet for grunndig brief med lokalkjent?)
BackupTeam(Standby team tilgjengelig?)

Go(Go)
Stop(Stopp)

Rescue -->|Usansynlig, recovery|Stop
Rescue-->|Ja mulig|Lines
Lines-->|Yes|Familiar
Lines-->|Nei|Stop
Familiar-->|Ja|Vis
Familiar-->|Nei|LocalBrief
LocalBrief-->|Ja|Vis
LocalBrief-->|Nei|Stop
Vis-->|>2m|Restr
Vis-->|<2m|Stop
Restr-->|Ja|Flow
Flow-->|Ja|Stop
Flow-->|Nei|BackupTeam
BackupTeam-->|Ja|Go
BackupTeam-->|Ja|Stop
 ```