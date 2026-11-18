
    A([Start]) --> B[/Display welcome message/]
    B --> C[/Input child's name, age, weight, height/]
    C --> D[/Input number of medications N/]
    D --> E[Initialize Medication_List as empty]
    E --> F[Set i = 1]
    F --> G{i <= N?}
    G -- No --> M[/Display child's information/]
    M --> O[/Display Medication_List/]
    O --> P[/Display completion message/]
    P --> Q([End])
    G -- Yes --> H[/Input medication name/]
    H --> I{Prescription available?}
    I -- No --> J[/Display warning message/]
    I -- Yes --> K[/Input dose, frequency, times and duration/]
    K --> L[Add medication to Medication_List]
    J --> R[Increase i by 1]
    L --> R
    R --> G
