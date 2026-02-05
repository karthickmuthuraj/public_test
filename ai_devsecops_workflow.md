## AI DevSecOps Workflow

```mermaid
graph TD
    accTitle: AI DevSecOps Workflow
    accDescr: A flowchart illustrating the lifecycle of an AI model from data sourcing to continuous monitoring, highlighting security integrations at each stage.

    subgraph "Data Sourcing & Management"
        A[Data Ingestion] --> B{Data Quality & Bias Checks};
        B --> C[Data Encryption];
    end
    style "Data Sourcing & Management" fill:#e8f5e9

    subgraph "Model Development"
        D[Feature Engineering] --> E[Model Training];
        E --> F{Threat Modeling};
        F --> G[Secure Coding & SAST];
    end
    style "Model Development" fill:#e3f2fd

    subgraph "CI/CD Pipeline"
        H[Code Commit] --> I{CI Orchestration};
        I --> J[DAST & Dependency Scanning];
        J --> K[Container Scanning];
        K --> L[Model Validation];
        L --> M[Signed & Versioned Model];
    end
    style "CI/CD Pipeline" fill:#f3e5f5

    subgraph "Model Deployment"
        N[Model Registry] --> O{Deployment to Staging};
        O --> P[Security & Penetration Testing];
        P --> Q{Production Deployment};
    end
    style "Model Deployment" fill:#fff3e0

    subgraph "Continuous Monitoring"
        R[Deployed Model] --> S{Performance Monitoring};
        S --> T[Drift Detection];
        T --> U[Security Incident Monitoring];
        U --> V[Feedback Loop to Development];
    end
    style "Continuous Monitoring" fill:#fffde7

    C --> D;
    G --> H;
    M --> N;
    Q --> R;

    classDef security fill:#f96,stroke:#333,stroke-width:2px;
    class B,F,G,J,K,P,U security
```

## Operational Issues in AI Workflows

```mermaid
mindmap
  accTitle: Operational Issues in AI Workflows
  accDescr: A mindmap showing various categories of operational issues in AI, including data, model, infrastructure, security, and compliance issues.

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
