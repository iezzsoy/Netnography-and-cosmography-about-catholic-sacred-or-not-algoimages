[file name]: Actors.md
[file content begin]
[[ALGORITHMIC ICONOGRAPHY IN CONTEMPORARY CATHOLIC UNIVERSES]] â€” [[Bruno Latour]] â€” [[Actor-Network Theory]] 

Humans
	Believers (Roman Catholics)
		Artists
		Non-artists
	Developers (*devs*)

Machines
	Devices
		Computers
		Mobile phones
	Services
		AI models (artificial intelligence)
			Training databases
	Platforms

God
	Grace
	Saints

Images
	Art
		Sacred
	Non-art
		Referred to as sacred
	Norms
		Tradition of symbolic representation of the sacred for Catholic veneration

DIAGRAM:

	classDiagram
    %% Abstract class Humans
    class Humans {
        <<abstract>>
        +String name
        +String belief
        +contemplate()
        +pray()
        +interact()
    }
    
    %% Subclasses Humans
    class CatholicBelievers {
        +String parish
        +String devotion
        +contemplateArt()
        +venerateImage()
        +prayBefore()
        +commissionArtwork()
    }
    
    class Artists {
        +String style
        +String technique
        +createSacredArt()
        +followNorms()
        +receiveInspiration()
        +useTools()
    }
    
    class Developers {
        +String language
        +String specialty
        +createAlgorithm()
        +trainAI()
        +developPlatform()
        +programSoftware()
    }
    
    %% Abstract class Non-Humans
    class NonHumans {
        <<abstract>>
        +influence()
        +process()
        +store()
    }
    
    %% Subclasses Divine
    class DivineEntities {
        <<abstract>>
        +String nature
        +inspire()
        +grantGrace()
        +intercede()
    }
    
    class God {
        +String omnipotence
        +inspireArtists()
        +grantGraces()
        +beRepresented()
    }
    
    class Jesus {
        +String incarnation
        +beModel()
        +beTheme()
        +save()
    }
    
    class HolySpirit {
        +String wisdom
        +illuminate()
        +inspire()
        +sanctify()
    }
    
    class Saints {
        +String virtue
        +String patronage
        +intercede()
        +beVenerated()
        +setExample()
    }
    
    %% Subclasses Technological
    class Machines {
        <<abstract>>
        +String type
        +process()
        +execute()
        +connect()
    }
    
    class Devices {
        +String hardware
        +String OS
        +runSoftware()
        +displayContent()
        +connectToNetwork()
    }
    
    class Computers {
        +String processor
        +createArt()
        +editImage()
        +runAI()
    }
    
    class MobilePhones {
        +String model
        +accessPlatforms()
        +share()
        +view()
    }
    
    class Services {
        <<abstract>>
        +String functionality
        +process()
        +respond()
        +learn()
    }
    
    class AIModels {
        +String architecture
        +String dataset
        +generateDigitalImage()
        +assistCreation()
        +processData()
    }
    
    class Databases {
        +String content
        +storeImages()
        +trainModels()
        +preserveTradition()
    }
    
    class Platforms {
        +String interface
        +hostServices()
        +connectUsers()
        +distributeContent()
    }
    
    %% Content Classes
    class Images {
        <<abstract>>
        +String format
        +String meaning
        +beContemplated()
        +conveyMessage()
    }
    
    class SacredArt {
        +String symbolism
        +String tradition
        +String human_author
        +representDivine()
        +inspireFaith()
        +followNorms()
        +receiveBlessing()
    }
    
    class DigitalImages {
        +String AI_origin
        +String prompt
        +String quality
        +beGeneratedByAI()
        +referenceSacrality()
        +assistArtists()
    }
    
    class Norms {
        +String tradition
        +String rules
        +guideArtists()
        +validateImages()
        +preserveTradition()
    }
    
    %% Inheritance Relationships
    Humans <|-- CatholicBelievers
    Humans <|-- Artists  
    Humans <|-- Developers
    
    NonHumans <|-- DivineEntities
    NonHumans <|-- Machines
    NonHumans <|-- Images
    NonHumans <|-- Norms
    
    DivineEntities <|-- God
    DivineEntities <|-- Jesus
    DivineEntities <|-- HolySpirit
    DivineEntities <|-- Saints
    
    Machines <|-- Devices
    Machines <|-- Services
    
    Devices <|-- Computers
    Devices <|-- MobilePhones
    
    Services <|-- AIModels
    Services <|-- Databases  
    Services <|-- Platforms
    
    Images <|-- SacredArt
    Images <|-- DigitalImages
    
    %% Association Relationships
    DivineEntities --> Artists : inspires
    Artists --> SacredArt : creates
    CatholicBelievers --> SacredArt : contemplates
    Developers --> AIModels : develops
    Developers --> Platforms : creates
    Artists --> Devices : uses
    AIModels --> Databases : trains_with
    AIModels --> DigitalImages : generates
    SacredArt --> Norms : follows
    Platforms --> SacredArt : distributes
    Platforms --> DigitalImages : distributes
    CatholicBelievers --> Devices : uses
    Databases --> SacredArt : stores
    DigitalImages --> Artists : assists
[file content end]
