## AI DevSecOps Workflow

```mermaid
graph TD
    accTitle: AI DevSecOps Workflow
    accDescr: A flowchart depicting the end-to-end AI DevSecOps process, organized into five stages: Data Sourcing & Management, Model Development, CI/CD Pipeline, Model Deployment, and Continuous Monitoring. It highlights the integration of security checks throughout the lifecycle.
    subgraph "Data Sourcing & Management"
        A[Data Ingestion] --> B{Data Quality & Bias Checks};
        B --> C[Data Encryption];
    end

    subgraph "Model Development"
        D[Feature Engineering] --> E[Model Training];
        E --> F{Threat Modeling};
        F --> G[Secure Coding & SAST];
    end

    subgraph "CI/CD Pipeline"
        H[Code Commit] --> I{CI Orchestration};
        I --> J[DAST & Dependency Scanning];
        J --> K[Container Scanning];
        K --> L[Model Validation];
        L --> M[Signed & Versioned Model];
    end

    subgraph "Model Deployment"
        N[Model Registry] --> O{Deployment to Staging};
        O --> P[Security & Penetration Testing];
        P --> Q{Production Deployment};
    end

    subgraph "Continuous Monitoring"
        R[Deployed Model] --> S{Performance Monitoring};
        S --> T[Drift Detection];
        T --> U[Security Incident Monitoring];
        U --> V[Feedback Loop to Development];
    end

    C --> D;
    G --> H;
    M --> N;
    Q --> R;

    classDef security fill:#f96,stroke:#333,stroke-width:2px;
    B,C,F,G,J,K,P,U:::security
```

## Operational Issues in AI Workflows

```mermaid
mindmap
    accTitle: Operational Issues in AI Workflows
    accDescr: A mindmap categorizing operational issues in AI workflows into five main areas: Data Issues, Model Issues, Infrastructure Issues, Security Issues, and Compliance Issues.
  root((Operational Issues in AI Workflows))
    ::icon(fa fa-brain)
    Data Issues
      ::icon(fa fa-database)
      Data Drift
      Data Quality Degradation
      Data Poisoning
      Privacy Leaks
    Model Issues
      ::icon(fa fa-robot)
      Model Degradation
      Concept Drift
      Adversarial Attacks
      Explainability Issues
    Infrastructure Issues
      ::icon(fa fa-server)
      Pipeline Failures
      Scalability Problems
      Resource Starvation
      Latency Increases
    Security Issues
      ::icon(fa fa-shield-alt)
      Model Evasion
      Inference Attacks
      Vulnerabilities in Dependencies
      Unauthorized Access
    Compliance Issues
      ::icon(fa fa-gavel)
      Regulatory Violations (GDPR, CCPA)
      Audit Trail Gaps
      Unfair Bias
```
