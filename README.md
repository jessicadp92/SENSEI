# SENSEI — Scraper for ENhanced AnalySis to Evaluate Illicit Trends

SENSEI is a research platform for monitoring online services and analyzing illicit trends across the web, with a particular focus on Dark Web markets. It aims to support the investigation of illegal online activities by extracting transaction-related information, analyzing user behavior, and identifying patterns and relationships between potentially connected criminal activities.

The platform was developed to provide analytical support for cybersecurity research and Law Enforcement Agencies (LEAs) investigating illicit online markets.

## 🚀 Overview

SENSEI combines web monitoring and data analysis to help researchers investigate the dynamics of illicit online services.

Its research objectives include:

- **Illicit trend analysis:** Identify and analyze trends in online illicit activities over time.
- **Behavioral analysis:** Examine transaction patterns and behavioral characteristics of vendors and customers.
- **Vendor network analysis:** Investigate relationships between vendors and other entities involved in online markets.
- **Cross-market and geographical analysis:** Compare trends across different countries and time periods to investigate the movement and distribution of illicit goods.
- **Investigation support:** Provide analytical insights that can help researchers and Law Enforcement Agencies investigate potentially related criminal activities.

These capabilities are intended to turn information collected from online services into structured insights that support the study of illicit online economies.

## 🏗️ Repository Structure

The repository contains the main platform, supporting data and configuration files, and dedicated analysis components.

```text
SENSEI/
├── ANITA/                       # Related project components
├── DATA/                        # Data resources
├── DB Dumps/                    # Database dump resources
├── Old docker/                  # Legacy Docker configuration
├── Platform/                    # Main platform
├── projects/
│   └── trend-analysis/           # Trend analysis component
├── Dockerfile
├── SENSEI-docker-compose.yml
├── mysql.yml
├── platform-backend-dockerfile
├── platform-frontend-dockerfile
└── README.md
```

The repository also contains database resources and additional configuration files used by the platform.

## 🛠️ Getting Started

### Prerequisites

Before running SENSEI, make sure the following tools are available in your environment:

- [Git](https://git-scm.com/)
- [Docker](https://www.docker.com/)
- Docker Compose

Additional configuration may be required depending on the database, services, and environment used by your deployment.

### Installation

Clone the repository:

```bash
git clone https://github.com/jessicadp92/SENSEI.git
cd SENSEI
```

### Running with Docker

The repository includes Docker-related configuration for building and running the platform.

First, create the Docker network expected by the existing configuration:

```bash
docker network create anita-network
```

Then build and start the services:

```bash
docker compose -f SENSEI-docker-compose.yml up --build
```

**Note:** The exact startup procedure depends on the Docker Compose configuration and the environment-specific settings. Database configuration, credentials, ports, and service dependencies may need to be reviewed before running the platform. Consult the configuration files and any applicable setup notes in the repository.

To stop the services, use:

```bash
docker compose -f SENSEI-docker-compose.yml down
```

## 🔬 Research Background

SENSEI was introduced as a platform for studying illicit online markets and understanding the behavior of the actors operating within them. Its research contribution lies in combining web monitoring with analytical capabilities for investigating transaction patterns, temporal trends, vendor relationships, and potential connections between criminal activities.

The platform was presented in the context of service-oriented computing research, with the goal of supporting data-driven investigations of illicit online services.

## 📄 Reference Publication

De Pascale, J., Cascavilla, G., Tamburri, D. A., & Van Den Heuvel, W.-J. (2023). **SENSEI: Scraper for ENhanced AnalySis to Evaluate Illicit Trends.** In *Service-Oriented Computing – ICSOC 2022 Workshops*, Lecture Notes in Computer Science, vol. 13821, pp. 374–383. Springer.

- [DOI: 10.1007/978-3-031-26507-5_36](https://doi.org/10.1007/978-3-031-26507-5_36)
- [Publication page — Tilburg University](https://research.tilburguniversity.edu/en/publications/sensei-scraper-for-enhanced-analysis-to-evaluate-illicit-trends/)
- [Preprint — SSRN](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3976047)

### BibTeX

```bibtex
@inproceedings{de2022sensei,
  title={Sensei: scraper for enhanced analysis to evaluate illicit trends},
  author={De Pascale, Jessica and Cascavilla, Giuseppe and Tamburri, Damian A and Van Den Heuvel, Willem-Jan},
  booktitle={International Conference on Service-Oriented Computing},
  pages={374--383},
  year={2022},
  organization={Springer}
}
```

## ⚖️ Responsible Use

SENSEI is intended for cybersecurity research, the analysis of illicit online activities, and investigation support. Data collection and analysis should comply with applicable laws, ethical requirements, privacy obligations, and institutional policies.

## 👩‍💻 Authors and Contributors

SENSEI was developed as a collaborative research project.

For the scientific background and original research contributions, please refer to the publication cited above.

## 📜 License

Check the repository for applicable licensing terms before redistributing or reusing the software.
