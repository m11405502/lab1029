```mermaid

graph TD

&nbsp;   %% === User Roles ===

&nbsp;   GC(\[General Contractor 👷])

&nbsp;   SUP(\[Supplier 🏭])



&nbsp;   %% === System Boundary ===

&nbsp;   subgraph System \[🌐 VITA Platform]

&nbsp;       direction TB



&nbsp;       %% === Level 1 - Core Screens ===

&nbsp;       SCR1(\[🏠 Homepage])

&nbsp;       SCR2(\[🔐 Login / Register])

&nbsp;       SCR3(\[📦 Orders Dashboard])

&nbsp;       SCR4(\[🔎 Supplier Directory])

&nbsp;       SCR5(\[💬 Messaging ])

&nbsp;       SCR6(\[👤 Profile ])

&nbsp;       SCR7(\[🔔 Notifications ])

&nbsp;       SCR8(\[📊 Reports])

&nbsp;       SCR9(\[💳 Payments])

&nbsp;       SCR10(\[📰 Blog])



&nbsp;       %% === Level 2 - Subscreens / Components ===

&nbsp;       subgraph Subscreens \[ ]

&nbsp;           direction TB

&nbsp;           SUB1(\[🧾 Order Details ])

&nbsp;           SUB2(\[📝 New Order Form ])

&nbsp;           SUB3(\[📬 Message Thread ])

&nbsp;           SUB4(\[⚙️ Edit Profile ])

&nbsp;           SUB5(\[🏗️ Supplier Details ])

&nbsp;       end

&nbsp;   end



&nbsp;   %% === Connections (Hierarchy) ===

&nbsp;   GC --> SCR2

&nbsp;   GC --> SCR3

&nbsp;   GC --> SCR4

&nbsp;   GC --> SCR5

&nbsp;   GC --> SCR6

&nbsp;   GC --> SCR7

&nbsp;   GC --> SCR8

&nbsp;   GC --> SCR9

&nbsp;   GC --> SCR10



&nbsp;   SUP --> SCR4

&nbsp;   SUP --> SCR5

&nbsp;   SUP --> SCR6



&nbsp;   SCR3 --> SUB1

&nbsp;   SCR3 --> SUB2

&nbsp;   SCR5 --> SUB3

&nbsp;   SCR6 --> SUB4

&nbsp;   SCR4 --> SUB5

