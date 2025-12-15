graph TD
    %% Divine Sphere
    D[God] --> |inspires| A1[Faithful Artists]
    J[Jesus] --> |model/theme| A1
    HS[Holy Spirit] --> |illuminates| A1
    S[Saints] --> |intercede| F1[Catholic Believers]
    D --> |grants graces| F1
    
    %% Humans - Believers
    F1 --> |contemplate| IM1[Sacred Art]
    F1 --> |venerate through| IM1
    F2[Non-Artist Believers] --> |commission| A1
    F2 --> |patronize| A1
    F1 --> |pray before| IM1
    
    %% Artists
    A1 --> |create| IM1
    A1 --> |follow| N1[Traditional Norms]
    A1 --> |use| DISP1[Computers]
    A1 --> |collaborate with| DEV[Developers]
    
    %% Developers
    DEV --> |create| ALG[Algorithms/Software]
    DEV --> |train| DB[AI Databases]
    DEV --> |develop| PLAT[Platforms]
    DEV --> |program| AI[AI Models]
    
    %% Machines - Devices
    DISP1 --> |execute| ALG
    DISP2[Mobile Phones] --> |access| PLAT
    DISP1 --> |connect to| PLAT
    DISP2 --> |display| IM1
    
    %% Services - AI
    AI --> |process| DB
    AI --> |assist creation| A1
    AI --> |generate references| IM2[Non-Sacred Art Images]
    DB --> |contain data| IM1
    DB --> |influence| AI
    
    %% Platforms
    PLAT --> |host| AI
    PLAT --> |distribute| IM1
    PLAT --> |connect| F1
    PLAT --> |facilitate access| A1
    
    %% Images
    IM1 --> |follow| N1
    IM1 --> |represent| D
    IM1 --> |represent| J
    IM1 --> |represent| S
    IM2 --> |reference| IM1
    IM2 --> |may inspire| A1
    
    %% Norms
    N1 --> |guide| A1
    N1 --> |validate| IM1
    N1 --> |preserve tradition| F1
    N1 --> |guide contemplation| F1
    
    %% Feedback loops
    F1 --> |feedback| A1
    F1 --> |demand| PLAT
    IM1 --> |inspire prayer| F1
    F1 --> |share| DISP2
    
    %% Styling
    classDef divine fill:#FFD700,stroke:#B8860B,stroke-width:3px
    classDef human fill:#87CEEB,stroke:#4682B4,stroke-width:2px
    classDef machine fill:#DDA0DD,stroke:#9370DB,stroke-width:2px
    classDef image fill:#98FB98,stroke:#228B22,stroke-width:2px
    classDef norm fill:#F0E68C,stroke:#DAA520,stroke-width:2px
    
    class D,J,HS,S divine
    class F1,F2,A1,DEV human
    class DISP1,DISP2,AI,DB,PLAT,ALG machine
    class IM
