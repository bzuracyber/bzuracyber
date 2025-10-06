# <a href="https://www.linkedin.com/in/daniel-bzura-0b3a9b1b5/">Daniel Bzura's</a> Project Portfolio

## Platform Security and Terraform Labs

- **[Container Security Lab with Docker and EKS](https://github.com/bzuracyber/container-security-lab-docker-eks)**
- **[Simple Terraform Deployment](https://github.com/bzuracyber/simple-terraform-lab)**
- **[CI/CD Pipeline Security](https://github.com/bzuracyber/CI-CD-Security-Pipeline-with-SAST-and-IaC-Scanning)**

## Vulnerability Management

- **[Vulnerability Management Program Implementation](https://github.com/bzuracyber/Vulnerability-Management)**
- **[Programmatic Vulnerability Remediations (PowerShell and BASH)](https://github.com/bzuracyber/Automated-Vulnerability-Remediation)**

## Compliance Automation Projects
- **[Compliance-as-Code Pipeline](https://github.com/bzuracyber/Azure-Compliance-as-Code-Pipeline)**  

<hr/>
apiVersion: networking.k8s.io/v1
kind: NetworkPolicy
metadata:
  name: allow-backend-service1-ingress
spec:
  podSelector:
    matchLabels:
      app: replace-with-service2-label
  policyTypes:
  - replace-with-policy-type
  ingress:
  - from:
    - podSelector:
        matchLabels:
          app: replace-with-service1-label
    ports:
    - protocol: TCP
      port: replace-with-service2-listening-port
