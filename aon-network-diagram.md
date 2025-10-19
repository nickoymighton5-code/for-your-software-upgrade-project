```mermaid
flowchart TD
    A[ A: Kick off meeting <br/> (8) ] --> B[ B: Define requirements <br/> (16) ]
    A --> C[ C: Design graphics <br/> (36) ]
    B --> D[ D: Assign software team <br/> (8) ]
    B --> H[ H: Assign training team <br/> (8) ]
    C --> E[ E: Redesign software <br/> (40) ]
    D --> E
    E --> F[ F: Build the software <br/> (40) ]
    F --> G[ G: Vendor Internal test <br/> (16) ]
    G --> J[ J: Release software <br/> (8) ]
    H --> I[ I: Train on redesign <br/> (48) ]
    I --> K[ K: Customer Test <br/> (16) ]
    J --> K
    K --> L[ L: Integrated systems <br/> (24) ]

    classDef critical fill:#ff9999,stroke:#333,stroke-width:2px;
    class A,C,E,F,G,J,K,L critical;
    classDef slack fill:#99ff99,stroke:#333,stroke-width:2px;
    class B,D,H,I slack;
