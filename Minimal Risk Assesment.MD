flowchart TD
Rescue(Realistic rescue)
Vis(Visibility)
Flow(High Flow)
Restr(Restricted)
Familiar(Experience in this cave)
Lines(Linesystem intact and known)
LocalBrief(Can get brief from someone with good knowledge)
BackupTeam(Backup team onsite)

Go(Go)
Stop(Stop)

Rescue -->|No, recovery|Stop
Rescue-->|Yes, possible|Lines
Lines-->|Yes|Familiar
Lines-->|No|Stop
Familiar-->|Yes|Vis
Familiar-->|No|LocalBrief
LocalBrief-->|Yes|Vis
LocalBrief-->|No|Stop
Vis-->|>2m|Restr
Vis-->|<2m|Stop
Restr-->|Yes|Flow
Flow-->|Yes|Stop
Flow-->|No|BackupTeam
BackupTeam-->|Yes|Go
BackupTeam-->|No|Stop
