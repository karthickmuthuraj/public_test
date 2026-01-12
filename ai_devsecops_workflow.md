## AI DevSecOps Workflow

```mermaid
graph TD
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

    click A "https://en.wikipedia.org/wiki/Extract,_transform,_load" "ETL on Wikipedia"
    click B "https://en.wikipedia.org/wiki/Data_quality" "Data Quality on Wikipedia"
    click C "https://en.wikipedia.org/wiki/Encryption" "Encryption on Wikipedia"
    click D "https://en.wikipedia.org/wiki/Feature_engineering" "Feature Engineering on Wikipedia"
    click E "https://en.wikipedia.org/wiki/Training,_validation,_and_test_data_sets" "Model Training on Wikipedia"
    click F "https://en.wikipedia.org/wiki/Threat_model" "Threat Modeling on Wikipedia"
    click G "https://en.wikipedia.org/wiki/Secure_coding" "Secure Coding on Wikipedia"
    click H "https://en.wikipedia.org/wiki/Commit_(version_control)" "Commit on Wikipedia"
    click I "https://en.wikipedia.org/wiki/CI/CD" "CI/CD on Wikipedia"
    click J "https://en.wikipedia.org/wiki/Dynamic_application_security_testing" "DAST on Wikipedia"
    click K "https://en.wikipedia.org/wiki/Container_security" "Container Scanning on Wikipedia"
    click L "https://en.wikipedia.org/wiki/Model_validation" "Model Validation on Wikipedia"
    click M "https://en.wikipedia.org/wiki/Digital_signature" "Digital Signature on Wikipedia"
    click O "https://en.wikipedia.org/wiki/Deployment_environment" "Staging Environment on Wikipedia"
    click P "https://en.wikipedia.org/wiki/Penetration_test" "Penetration Testing on Wikipedia"
    click Q "https://en.wikipedia.org/wiki/Deployment_environment#Production_environment" "Production Environment on Wikipedia"
    click S "https://en.wikipedia.org/wiki/Application_performance_management" "Performance Monitoring on Wikipedia"
    click T "https://en.wikipedia.org/wiki/Concept_drift" "Drift Detection on Wikipedia"
    click U "https://en.wikipedia.org/wiki/Security_information_and_event_management" "SIEM on Wikipedia"
    click V "https://en.wikipedia.org/wiki/Feedback" "Feedback Loop on Wikipedia"
    click N "https://en.wikipedia.org/wiki/MLOps" "MLOps on Wikipedia"
    click R "https://en.wikipedia.org/wiki/Cloud_computing" "Cloud Computing on Wikipedia"
```

## Operational Issues in AI Workflows

```mermaid
mindmap
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

    click "Data Drift" "https://en.wikipedia.org/wiki/Concept_drift" "Concept Drift on Wikipedia"
    click "Data Quality Degradation" "https://en.wikipedia.org/wiki/Data_quality" "Data Quality on Wikipedia"
    click "Data Poisoning" "https://en.wikipedia.org/wiki/Adversarial_machine_learning" "Adversarial Machine Learning on Wikipedia"
    click "Privacy Leaks" "https://en.wikipedia.org/wiki/Data_breach" "Data Breach on Wikipedia"
    click "Model Degradation" "https://en.wikipedia.org/wiki/Concept_drift" "Concept Drift on Wikipedia"
    click "Concept Drift" "https://en.wikipedia.org/wiki/Concept_drift" "Concept Drift on Wikipedia"
    click "Adversarial Attacks" "https://en.wikipedia.org/wiki/Adversarial_machine_learning" "Adversarial Machine Learning on Wikipedia"
    click "Explainability Issues" "https://en.wikipedia.org/wiki/Explainable_artificial_intelligence" "Explainable AI on Wikipedia"
    click "Pipeline Failures" "https://en.wikipedia.org/wiki/CI/CD" "CI/CD on Wikipedia"
    click "Scalability Problems" "https://en.wikipedia.org/wiki/Scalability" "Scalability on Wikipedia"
    click "Resource Starvation" "https://en.wikipedia.org/wiki/Resource_starvation" "Resource Starvation on Wikipedia"
    click "Latency Increases" "https://en.wikipedia.org/wiki/Latency_(engineering)" "Latency on Wikipedia"
    click "Model Evasion" "https://en.wikipedia.org/wiki/Adversarial_machine_learning" "Adversarial Machine Learning on Wikipedia"
    click "Inference Attacks" "https://en.wikipedia.org/wiki/Inference_attack" "Inference Attack on Wikipedia"
    click "Vulnerabilities in Dependencies" "https://en.wikipedia.org/wiki/Software_supply_chain" "Software Supply Chain on Wikipedia"
    click "Unauthorized Access" "https://en.wikipedia.org/wiki/Authorization" "Authorization on Wikipedia"
    click "Regulatory Violations (GDPR, CCPA)" "https://en.wikipedia.org/wiki/General_Data_Protection_Regulation" "GDPR on Wikipedia"
    click "Audit Trail Gaps" "https://en.wikipedia.org/wiki/Audit_trail" "Audit Trail on Wikipedia"
    click "Unfair Bias" "https://en.wikipedia.org/wiki/Algorithmic_bias" "Algorithmic Bias on Wikipedia"
```
