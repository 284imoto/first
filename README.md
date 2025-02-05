```mermaid
graph TD;
    A[Input Image (224x224x3)] --> B[Conv3-64] --> C[Conv3-64] --> D[MaxPool]
    D --> E[Conv3-128] --> F[Conv3-128] --> G[MaxPool]
    G --> H[Conv3-256] --> I[Conv3-256] --> J[Conv3-256] --> K[MaxPool]
    K --> L[Conv3-512] --> M[Conv3-512] --> N[Conv3-512] --> O[MaxPool]
    O --> P[Conv3-512] --> Q[Conv3-512] --> R[Conv3-512] --> S[MaxPool]
    S --> T[Flatten]
    T --> U[FC-4096] --> V[FC-4096] --> W[FC-1000]
    W --> X[Softmax]
    X --> Y[Output (Class Probabilities)]
# first
