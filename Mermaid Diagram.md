```mermaid
graph TD

A[Markdown]-->B[Terminal Usage]

subgraph g1[OS and General Knowledge]
B-->C[Basic Terminal Commands]
end

subgraph g2[Learn a Language]
C-->D[C/C++]-->E[Python]-->F[C#]-.->F1{{Go}}
end

F-.->F2{{Unity}}

subgraph g3[Build Systems]
F-.->F3[CMake]-.->F3*{{Make}}
end

subgraph g4[Package Management]
F3-->g41[Conda]-->g42[Poetry]
end

subgraph g5[VCS and Repo Hosting]
g42-->g51[Git]-->g52[Github]-.->g53{{GitLab}}
end

subgraph g6[CI/CD]
g52-->g61[Github Actions]
end

subgraph g7[Documentation]
g61-.->g71{{Doxygen}}-.->g72{{MkDocs}}-.->g73{{DocFX}}
end

subgraph g8[Formatting and Linting]
g73-.->g81{{Clang-Format}}-.->g82{{Clang-Tidy}}-.->g83{{Black}}-.->g84{{Pylint}}
end

subgraph g9[Testing]
g61-->g91[Unit Testing]-->g92[Integration Testing]
end

subgraph g10[Containerization]
g92-->g101[Docker]-.->g102{{Kubernetes}}
end

subgraph g11[Networking]
g101-->g111[Internet]-->g112[HTTP]-->g113[WebSockets]
end

subgraph g12[Learn about APIs]
g113-->g121[REST]-.->g122{{gRPC}}-.->g123{{GraphQL}}
end

subgraph g13[Relational Database]
g111-.->g131{{PostgreSQL}}-.->g132{{SQLite}}-.->g133{{MySQL}}
end

